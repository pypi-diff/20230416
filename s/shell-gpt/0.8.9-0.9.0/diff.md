# Comparing `tmp/shell_gpt-0.8.9.tar.gz` & `tmp/shell_gpt-0.9.0.tar.gz`

## Comparing `shell_gpt-0.8.9.tar` & `shell_gpt-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,24 @@
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/LICENSE
--rw-r--r--   0        0        0    15996 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/README.md
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/pyproject.toml
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/__main__.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/app.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/cache.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/client.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/config.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/make_prompt.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/handlers/__init__.py
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/handlers/chat_handler.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/handlers/default_handler.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/handlers/handler.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/sgpt/handlers/repl_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/__init__.py
--rw-r--r--   0        0        0    12909 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/test_integration.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/test_unit.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/LICENSE
--rw-r--r--   0        0        0    15996 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/README.md
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/pyproject.toml
--rw-r--r--   0        0        0    18024 2020-02-02 00:00:00.000000 shell_gpt-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/LICENSE
+-rw-r--r--   0        0        0    18734 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/README.md
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/__main__.py
+-rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/app.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/cache.py
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/client.py
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/config.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/make_prompt.py
+-rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/role.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/handlers/__init__.py
+-rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/handlers/chat_handler.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/handlers/default_handler.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/handlers/handler.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/handlers/repl_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0    15148 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/tests/test_integration.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/tests/test_unit.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/LICENSE
+-rw-r--r--   0        0        0    18734 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/README.md
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    20762 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/PKG-INFO
```

### Comparing `shell_gpt-0.8.9/LICENSE` & `shell_gpt-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.9/README.md` & `shell_gpt-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Shell GPT
-A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
+# ShellGPT
+A command-line productivity tool powered by OpenAI's GPT models. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort. ShellGPT is cross-platform compatible and supports all major operating systems, including Linux, macOS, and Windows with all major shells, such as PowerShell, CMD, Bash, Zsh, Fish, and many others.
 
 https://user-images.githubusercontent.com/16740832/231569156-a3a9f9d4-18b1-4fff-a6e1-6807651aa894.mp4
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.8
+pip install shell-gpt==0.9.0
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -214,29 +214,49 @@
 >>> Change port to 443
 import requests
 response = requests.get('https://localhost:443')
 print(response.text)
 ```
 
 ### Chat sessions
-To list all the current chat sessions, use the `--list-chat` option:
+To list all the current chat sessions, use the `--list-chats` option:
 ```shell
-sgpt --list-chat
+sgpt --list-chats
 # .../shell_gpt/chat_cache/number
 # .../shell_gpt/chat_cache/python_request
 ```
 To show all the messages related to a specific chat session, use the `--show-chat` option followed by the session name:
 ```shell
 sgpt --show-chat number
 # user: please remember my favorite number: 4
 # assistant: I will remember that your favorite number is 4.
 # user: what would be my favorite number + 4?
 # assistant: Your favorite number is 4, so if we add 4 to it, the result would be 8.
 ```
 
+### Roles
+ShellGPT allows you to create custom roles, which can be utilized to generate code, shell commands, or to fulfill your specific needs. To create a new role, use the `--create-role` option followed by the role name. You will be prompted to provide a description for the role, along with other details. This will create a JSON file in `~/.config/shell_gpt/roles` with the role name. Inside this directory, you can also edit default `sgpt` roles, such as **shell**, **code**, and **default**. Use the `--list-roles` option to list all available roles, and the `--show-role` option to display the details of a specific role. Here's an example of a custom role:
+```shell
+sgpt --create-role json
+# Enter role description: You are JSON generator, provide only valid json as response.
+# Enter expecting result, e.g. answer, code, shell command, etc.: json
+sgpt --role json "random: user, password, email, address"
+{
+  "user": "JohnDoe",
+  "password": "p@ssw0rd",
+  "email": "johndoe@example.com",
+  "address": {
+    "street": "123 Main St",
+    "city": "Anytown",
+    "state": "CA",
+    "zip": "12345"
+  }
+}
+```
+
 ### Request cache
 Control cache using `--cache` (default) and `--no-cache` options. This caching applies for all `sgpt` requests to OpenAI API:
 ```shell
 sgpt "what are the colors of a rainbow"
 # -> The colors of a rainbow are red, orange, yellow, green, blue, indigo, and violet.
 ```
 Next time, same exact query will get results from local cache instantly. Note that `sgpt "what are the colors of a rainbow" --temperature 0.5` will make a new request, since we didn't provide `--temperature` (same applies to `--top-probability`) on previous request.
@@ -260,40 +280,50 @@
 CACHE_PATH=/tmp/shell_gpt/cache
 # Request timeout in seconds.
 REQUEST_TIMEOUT=60
 # Default OpenAI model to use.
 DEFAULT_MODEL=gpt-3.5-turbo
 # Default color for OpenAI completions.
 DEFAULT_COLOR=magenta
+# Force use system role messages (not recommended).
+SYSTEM_ROLES=false
 ```
 Possible options for `DEFAULT_COLOR`: black, red, green, yellow, blue, magenta, cyan, white, bright_black, bright_red, bright_green, bright_yellow, bright_blue, bright_magenta, bright_cyan, bright_white.
 
+Switch `SYSTEM_ROLES` to force use [system roles](https://help.openai.com/en/articles/7042661-chatgpt-api-transition-guide) messages, this is not recommended, since it doesn't perform well with current GPT models.
+
 ### Full list of arguments
 ```text
-╭─ Arguments ────────────────────────────────────────────────────────────────────────────────────────────────╮
-│   prompt      [PROMPT]  The prompt to generate completions for.                                            │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --model            [gpt-3.5-turbo|gpt-4|gpt-4-32k]  OpenAI GPT model to use. [default: gpt-3.5-turbo]      │
-│ --temperature      FLOAT RANGE [0.0<=x<=1.0]        Randomness of generated output. [default: 0.1]         │
-│ --top-probability  FLOAT RANGE [0.1<=x<=1.0]        Limits highest probable tokens (words). [default: 1.0] │
-│ --editor                                            Open $EDITOR to provide a prompt. [default: no-editor] │
-│ --cache                                             Cache completion results. [default: cache]             │
-│ --help                                              Show this message and exit.                            │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Assistance Options ───────────────────────────────────────────────────────────────────────────────────────╮
-│ --shell  -s                 Generate and execute shell commands.                                           │
-│ --code       --no-code      Generate only code. [default: no-code]                                         │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Chat Options ─────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --chat        TEXT  Follow conversation with id, use "temp" for quick session. [default: None]             │
-│ --repl        TEXT  Start a REPL (Read–eval–print loop) session. [default: None]                           │
-│ --show-chat   TEXT  Show all messages from provided chat id. [default: None]                               │
-│ --list-chat         List all existing chat ids. [default: no-list-chat]                                    │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────╮
+│   prompt      [PROMPT]  The prompt to generate completions for.                                             │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --model            [gpt-3.5-turbo|gpt-4|gpt-4-32k]  OpenAI GPT model to use. [default: gpt-3.5-turbo]       │
+│ --temperature      FLOAT RANGE [0.0<=x<=1.0]        Randomness of generated output. [default: 0.1]          │
+│ --top-probability  FLOAT RANGE [0.1<=x<=1.0]        Limits highest probable tokens (words). [default: 1.0]  │
+│ --editor                                            Open $EDITOR to provide a prompt. [default: no-editor]  │
+│ --cache                                             Cache completion results. [default: cache]              │
+│ --help                                              Show this message and exit.                             │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Assistance Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --shell  -s                 Generate and execute shell commands.                                            │
+│ --code       --no-code      Generate only code. [default: no-code]                                          │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Chat Options ──────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --chat        TEXT  Follow conversation with id, use "temp" for quick session. [default: None]              │
+│ --repl        TEXT  Start a REPL (Read–eval–print loop) session. [default: None]                            │
+│ --show-chat   TEXT  Show all messages from provided chat id. [default: None]                                │
+│ --list-chats        List all existing chat ids. [default: no-list-chats]                                    │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Role Options ──────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --role         TEXT  System role for GPT model. [default: None]                                             │
+│ --create-role  TEXT  Create role. [default: None]                                                           │
+│ --show-role    TEXT  Show role. [default: None]                                                             │
+│ --list-roles         List roles. [default: no-list-roles]                                                   │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## Docker
 Run the container using the `OPENAI_API_KEY` environment variable, and a docker volume to store cache:
 ```shell
 docker run --rm \
            --env OPENAI_API_KEY="your OPENAI API key" \
```

### Comparing `shell_gpt-0.8.9/pyproject.toml` & `shell_gpt-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.9/sgpt/app.py` & `shell_gpt-0.9.0/sgpt/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
-shell-gpt: An interface to OpenAI's ChatGPT (GPT-3.5) API
-
-This module provides a simple interface for OpenAI's ChatGPT API using Typer
+This module provides a simple interface for OpenAI API using Typer
 as the command line interface. It supports different modes of output including
 shell commands and code, and allows users to specify the desired OpenAI model
 and length and other options of the output. Additionally, it supports executing
 shell commands directly from the interface.
-
-API Key is stored locally for easy use in future runs.
 """
 # To allow users to use arrow keys in the REPL.
 import readline  # noqa: F401
 import sys
 
 import typer
-
-# Click is part of typer.
 from click import BadArgumentUsage, MissingParameter
 
-from sgpt import ChatHandler, DefaultHandler, OpenAIClient, ReplHandler, cfg
+from sgpt.client import OpenAIClient
+from sgpt.config import cfg
+from sgpt.handlers.chat_handler import ChatHandler
+from sgpt.handlers.default_handler import DefaultHandler
+from sgpt.handlers.repl_handler import ReplHandler
+from sgpt.role import DefaultRoles, SystemRole
 from sgpt.utils import ModelOptions, get_edited_prompt, run_command
 
 
 def main(
     prompt: str = typer.Argument(
         None,
         show_default=False,
@@ -76,25 +75,48 @@
     ),
     show_chat: str = typer.Option(
         None,
         help="Show all messages from provided chat id.",
         callback=ChatHandler.show_messages_callback,
         rich_help_panel="Chat Options",
     ),
-    list_chat: bool = typer.Option(
+    list_chats: bool = typer.Option(
         False,
         help="List all existing chat ids.",
         callback=ChatHandler.list_ids,
         rich_help_panel="Chat Options",
     ),
+    role: str = typer.Option(
+        None,
+        help="System role for GPT model.",
+        rich_help_panel="Role Options",
+    ),
+    create_role: str = typer.Option(
+        None,
+        help="Create role.",
+        callback=SystemRole.create,
+        rich_help_panel="Role Options",
+    ),
+    show_role: str = typer.Option(
+        None,
+        help="Show role.",
+        callback=SystemRole.show,
+        rich_help_panel="Role Options",
+    ),
+    list_roles: bool = typer.Option(
+        False,
+        help="List roles.",
+        callback=SystemRole.list,
+        rich_help_panel="Role Options",
+    ),
 ) -> None:
     stdin_passed = not sys.stdin.isatty()
 
     if stdin_passed and not repl:
-        prompt = sys.stdin.read() + (prompt or "")
+        prompt = f"{sys.stdin.read()}\n\n{prompt or ''}"
 
     if not prompt and not editor and not repl:
         raise MissingParameter(param_hint="PROMPT", param_type="string")
 
     if shell and code:
         raise BadArgumentUsage("--shell and --code options cannot be used together.")
 
@@ -107,36 +129,38 @@
     if editor:
         prompt = get_edited_prompt()
 
     api_host = cfg.get("OPENAI_API_HOST")
     api_key = cfg.get("OPENAI_API_KEY")
     client = OpenAIClient(api_host, api_key)
 
+    role_class = DefaultRoles.get(shell, code) if not role else SystemRole.get(role)
+
     if repl:
         # Will be in infinite loop here until user exits with Ctrl+C.
-        ReplHandler(client, repl, shell, code).handle(
+        ReplHandler(client, repl, role_class).handle(
             prompt,
             model=model.value,
             temperature=temperature,
             top_probability=top_probability,
             chat_id=repl,
             caching=cache,
         )
 
     if chat:
-        full_completion = ChatHandler(client, chat, shell, code).handle(
+        full_completion = ChatHandler(client, chat, role_class).handle(
             prompt,
             model=model.value,
             temperature=temperature,
             top_probability=top_probability,
             chat_id=chat,
             caching=cache,
         )
     else:
-        full_completion = DefaultHandler(client, shell, code).handle(
+        full_completion = DefaultHandler(client, role_class).handle(
             prompt,
             model=model.value,
             temperature=temperature,
             top_probability=top_probability,
             caching=cache,
         )
```

### Comparing `shell_gpt-0.8.9/sgpt/cache.py` & `shell_gpt-0.9.0/sgpt/cache.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.9/sgpt/client.py` & `shell_gpt-0.9.0/sgpt/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from pathlib import Path
 from typing import Dict, Generator, List
 
 import requests
 
-from sgpt import Cache, cfg
+from .cache import Cache
+from .config import cfg
 
 CACHE_LENGTH = int(cfg.get("CACHE_LENGTH"))
 CACHE_PATH = Path(cfg.get("CACHE_PATH"))
 REQUEST_TIMEOUT = int(cfg.get("REQUEST_TIMEOUT"))
 
 
 class OpenAIClient:
@@ -23,15 +24,15 @@
         self,
         messages: List[Dict[str, str]],
         model: str = "gpt-3.5-turbo",
         temperature: float = 1,
         top_probability: float = 1,
     ) -> Generator[str, None, None]:
         """
-        Make request to OpenAI ChatGPT API, read more:
+        Make request to OpenAI API, read more:
         https://platform.openai.com/docs/api-reference/chat
 
         :param messages: List of messages {"role": user or assistant, "content": message_string}
         :param model: String gpt-3.5-turbo or gpt-3.5-turbo-0301
         :param temperature: Float in 0.0 - 1.0 range.
         :param top_probability: Float in 0.0 - 1.0 range.
         :return: Response body JSON.
```

### Comparing `shell_gpt-0.8.9/sgpt/config.py` & `shell_gpt-0.9.0/sgpt/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,34 +2,36 @@
 from getpass import getpass
 from pathlib import Path
 from tempfile import gettempdir
 from typing import Any
 
 from click import UsageError
 
-from sgpt.utils import ModelOptions
+from .utils import ModelOptions
 
 CONFIG_FOLDER = os.path.expanduser("~/.config")
-CONFIG_PATH = Path(CONFIG_FOLDER) / "shell_gpt" / ".sgptrc"
+SHELL_GPT_CONFIG_FOLDER = Path(CONFIG_FOLDER) / "shell_gpt"
+SHELL_GPT_CONFIG_PATH = SHELL_GPT_CONFIG_FOLDER / ".sgptrc"
+ROLE_STORAGE_PATH = SHELL_GPT_CONFIG_FOLDER / "roles"
+CHAT_CACHE_PATH = Path(gettempdir()) / "chat_cache"
+CACHE_PATH = Path(gettempdir()) / "cache"
 
 # TODO: Refactor ENV variables with SGPT_ prefix.
 DEFAULT_CONFIG = {
     # TODO: Refactor it to CHAT_STORAGE_PATH.
-    "CHAT_CACHE_PATH": os.getenv(
-        "CHAT_CACHE_PATH", str(Path(gettempdir()) / "shell_gpt" / "chat_cache")
-    ),
-    "CACHE_PATH": os.getenv(
-        "CACHE_PATH", str(Path(gettempdir()) / "shell_gpt" / "cache")
-    ),
+    "CHAT_CACHE_PATH": os.getenv("CHAT_CACHE_PATH", str(CHAT_CACHE_PATH)),
+    "CACHE_PATH": os.getenv("CACHE_PATH", str(CACHE_PATH)),
     "CHAT_CACHE_LENGTH": int(os.getenv("CHAT_CACHE_LENGTH", "100")),
     "CACHE_LENGTH": int(os.getenv("CHAT_CACHE_LENGTH", "100")),
     "REQUEST_TIMEOUT": int(os.getenv("REQUEST_TIMEOUT", "60")),
     "DEFAULT_MODEL": os.getenv("DEFAULT_MODEL", ModelOptions.GPT3.value),
     "OPENAI_API_HOST": os.getenv("OPENAI_API_HOST", "https://api.openai.com"),
     "DEFAULT_COLOR": os.getenv("DEFAULT_COLOR", "magenta"),
+    "ROLE_STORAGE_PATH": os.getenv("ROLE_STORAGE_PATH", str(ROLE_STORAGE_PATH)),
+    "SYSTEM_ROLES": os.getenv("SYSTEM_ROLES", "false"),
     # New features might add their own config variables here.
 }
 
 
 class Config(dict):  # type: ignore
     def __init__(self, config_path: Path, **defaults: Any):
         self.config_path = config_path
@@ -73,8 +75,8 @@
         # Prioritize environment variables over config file.
         value = os.getenv(key) or super().get(key)
         if not value:
             raise UsageError(f"Missing config key: {key}")
         return value
 
 
-cfg = Config(CONFIG_PATH, **DEFAULT_CONFIG)
+cfg = Config(SHELL_GPT_CONFIG_PATH, **DEFAULT_CONFIG)
```

### Comparing `shell_gpt-0.8.9/sgpt/make_prompt.py` & `shell_gpt-0.9.0/sgpt/make_prompt.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.9/sgpt/utils.py` & `shell_gpt-0.9.0/sgpt/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,24 @@
 import os
 import platform
 import shlex
 from enum import Enum
 from tempfile import NamedTemporaryFile
+from typing import Any, Callable
 
+import typer
 from click import BadParameter
 
 
 class ModelOptions(str, Enum):
     GPT3 = "gpt-3.5-turbo"
     GPT4 = "gpt-4"
     GPT4_32K = "gpt-4-32k"
 
 
-class CompletionModes(Enum):
-    NORMAL = "normal"
-    SHELL = "shell"
-    CODE = "code"
-
-    @classmethod
-    def get_mode(cls, shell: bool, code: bool) -> "CompletionModes":
-        if shell:
-            return CompletionModes.SHELL
-        if code:
-            return CompletionModes.CODE
-        return CompletionModes.NORMAL
-
-
 def get_edited_prompt() -> str:
     """
     Opens the user's default editor to let them
     input a prompt, and returns the edited text.
 
     :return: String prompt.
     """
@@ -63,7 +51,17 @@
             else f'cmd.exe /c "{command}"'
         )
     else:
         shell = os.environ.get("SHELL", "/bin/sh")
         full_command = f"{shell} -c {shlex.quote(command)}"
 
     os.system(full_command)
+
+
+def option_callback(func: Callable) -> Callable:  # type: ignore
+    def wrapper(cls: Any, value: str) -> None:
+        if not value:
+            return
+        func(cls, value)
+        raise typer.Exit()
+
+    return wrapper
```

### Comparing `shell_gpt-0.8.9/sgpt/handlers/repl_handler.py` & `shell_gpt-0.9.0/sgpt/handlers/repl_handler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 from typing import Any
 
 import typer
 from rich import print as rich_print
 from rich.rule import Rule
 
-from sgpt.client import OpenAIClient
-from sgpt.handlers.chat_handler import ChatHandler
-from sgpt.utils import CompletionModes, run_command
+from ..client import OpenAIClient
+from ..role import DefaultRoles, SystemRole
+from ..utils import run_command
+from .chat_handler import ChatHandler
 
 
 class ReplHandler(ChatHandler):
-    def __init__(
-        self,
-        client: OpenAIClient,
-        chat_id: str,
-        shell: bool = False,
-        code: bool = False,
-        model: str = "gpt-3.5-turbo",
-    ):
-        super().__init__(client, chat_id, shell, code, model)
+    def __init__(self, client: OpenAIClient, chat_id: str, role: SystemRole) -> None:
+        super().__init__(client, chat_id, role)
 
     def handle(self, prompt: str, **kwargs: Any) -> None:  # type: ignore
         if self.initiated:
             rich_print(Rule(title="Chat History", style="bold magenta"))
             self.show_messages(self.chat_id)
             rich_print(Rule(style="bold magenta"))
 
         info_message = (
             "Entering REPL mode, press Ctrl+C to exit."
-            if not self.mode == CompletionModes.SHELL
+            if not self.role.name == DefaultRoles.SHELL.value
             else "Entering shell REPL mode, type [e] to execute commands or press Ctrl+C to exit."
         )
         typer.secho(info_message, fg="yellow")
 
         if not prompt:
             prompt = typer.prompt(">>>", prompt_suffix=" ")
         else:
@@ -40,14 +34,14 @@
 
         while True:
             full_completion = super().handle(prompt, **kwargs)
             prompt = typer.prompt(">>>", prompt_suffix=" ")
             if prompt == "exit()":
                 # This is also useful during tests.
                 raise typer.Exit()
-            if self.mode == CompletionModes.SHELL:
+            if self.role.name == DefaultRoles.SHELL.value:
                 if prompt == "e":
                     typer.echo()
                     run_command(full_completion)
                     typer.echo()
                     rich_print(Rule(style="bold magenta"))
                     prompt = typer.prompt(">>> ", prompt_suffix=" ")
```

### Comparing `shell_gpt-0.8.9/tests/test_integration.py` & `shell_gpt-0.9.0/tests/test_integration.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 from unittest import TestCase
 from unittest.mock import ANY, patch
 from uuid import uuid4
 
 import typer
 from typer.testing import CliRunner
 
-from sgpt import OpenAIClient, cfg, main
+from sgpt.app import main
+from sgpt.client import OpenAIClient
+from sgpt.config import cfg
 from sgpt.handlers.handler import Handler
+from sgpt.role import SystemRole
 
 runner = CliRunner()
 app = typer.Typer()
 app.command()(main)
 
 
 class TestShellGpt(TestCase):
@@ -58,15 +61,15 @@
         }
         result = runner.invoke(app, self.get_arguments(**dict_arguments))
         assert result.exit_code == 0
         assert "git commit" in result.stdout
 
     def test_code(self):
         """
-        This test will request from ChatGPT a python code to make CLI app,
+        This test will request from OpenAI API a python code to make CLI app,
         which will be written to a temp file, and then it will be executed
         in shell with two positional int arguments. As the output we are
         expecting the result of multiplying them.
         """
         dict_arguments = {
             "prompt": (
                 "Create a command line application using Python that "
@@ -160,15 +163,15 @@
         assert "--code" not in dict_arguments
         dict_arguments["--shell"] = True
         result = runner.invoke(app, self.get_arguments(**dict_arguments))
         # If we have --code chat, we cannot use --shell.
         assert result.exit_code == 2
 
     def test_list_chat(self):
-        result = runner.invoke(app, ["--list-chat"])
+        result = runner.invoke(app, ["--list-chats"])
         assert result.exit_code == 0
         assert "test_" in result.stdout
 
     def test_show_chat(self):
         chat_name = uuid4()
         dict_arguments = {
             "prompt": "Remember my favorite number: 6",
@@ -303,31 +306,89 @@
     def test_model_option(self, mocked_get_completion):
         dict_arguments = {
             "prompt": "What is the capital of the Czech Republic?",
             "--model": "gpt-4",
         }
         result = runner.invoke(app, self.get_arguments(**dict_arguments))
         mocked_get_completion.assert_called_once_with(
-            ANY, "gpt-4", 0.1, 1.0, caching=False
+            messages=ANY,
+            model="gpt-4",
+            temperature=0.1,
+            top_probability=1.0,
+            caching=False,
         )
         assert result.exit_code == 0
 
     def test_color_output(self):
         color = cfg.get("DEFAULT_COLOR")
-        handler = Handler(OpenAIClient("test", "test"))
+        role = SystemRole.get("default")
+        handler = Handler(OpenAIClient("test", "test"), role=role)
         assert handler.color == color
         os.environ["DEFAULT_COLOR"] = "red"
-        handler = Handler(OpenAIClient("test", "test"))
+        handler = Handler(OpenAIClient("test", "test"), role=role)
         assert handler.color == "red"
 
     def test_simple_stdin(self):
         result = runner.invoke(app, input="What is the capital of Germany?\n")
         assert "Berlin" in result.stdout
 
     def test_shell_stdin_with_prompt(self):
         dict_arguments = {
             "prompt": "Sort by name",
             "--shell": True,
         }
         stdin = "What is in current folder\n"
         result = runner.invoke(app, self.get_arguments(**dict_arguments), input=stdin)
         assert result.stdout == "ls | sort\n"
+
+    def test_role(self):
+        test_role = Path(cfg.get("ROLE_STORAGE_PATH")) / "test_json.json"
+        test_role.unlink(missing_ok=True)
+        dict_arguments = {
+            "prompt": "test",
+            "--create-role": "test_json",
+        }
+        input = "You are a JSON generator, return only JSON as response.\n" "json\n"
+        result = runner.invoke(app, self.get_arguments(**dict_arguments), input=input)
+        assert result.exit_code == 0
+
+        dict_arguments = {
+            "prompt": "test",
+            "--list-roles": True,
+        }
+        result = runner.invoke(app, self.get_arguments(**dict_arguments))
+        assert result.exit_code == 0
+        assert "test_json" in result.stdout
+
+        dict_arguments = {
+            "prompt": "test",
+            "--show-role": "test_json",
+        }
+        result = runner.invoke(app, self.get_arguments(**dict_arguments))
+        assert result.exit_code == 0
+        assert "You are a JSON generator" in result.stdout
+
+        # Test with command line argument prompt.
+        dict_arguments = {
+            "prompt": "random username, password, email",
+            "--role": "test_json",
+        }
+        result = runner.invoke(app, self.get_arguments(**dict_arguments))
+        assert result.exit_code == 0
+        generated_json = json.loads(result.stdout)
+        assert "username" in generated_json
+        assert "password" in generated_json
+        assert "email" in generated_json
+
+        # Test with stdin prompt.
+        dict_arguments = {
+            "prompt": "",
+            "--role": "test_json",
+        }
+        stdin = "random username, password, email"
+        result = runner.invoke(app, self.get_arguments(**dict_arguments), input=stdin)
+        assert result.exit_code == 0
+        generated_json = json.loads(result.stdout)
+        assert "username" in generated_json
+        assert "password" in generated_json
+        assert "email" in generated_json
+        test_role.unlink(missing_ok=True)
```

### Comparing `shell_gpt-0.8.9/tests/test_unit.py` & `shell_gpt-0.9.0/tests/test_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import unittest
 
 import requests
 import requests_mock
 
-from sgpt import OpenAIClient
+from sgpt.client import OpenAIClient
 
 
 class TestMain(unittest.TestCase):
     API_HOST = os.getenv("OPENAI_HOST", "https://api.openai.com")
     API_URL = f"{API_HOST}/v1/chat/completions"
     # TODO: Fix tests.
```

### Comparing `shell_gpt-0.8.9/PKG-INFO` & `shell_gpt-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell_gpt
-Version: 0.8.9
+Version: 0.9.0
 Summary: A command-line productivity tool powered by OpenAI GPT models, will help you accomplish your tasks faster and more efficiently.
 Project-URL: homepage, https://github.com/ther1d/shell_gpt
 Project-URL: repository, https://github.com/ther1d/shell_gpt
 Project-URL: documentation, https://github.com/TheR1D/shell_gpt/blob/main/README.md
 Author-email: Farkhod Sadykov <farkhod@sadykov.dev>
 License-Expression: MIT
 License-File: LICENSE
@@ -38,22 +38,22 @@
 Requires-Dist: isort<6.0.0,>=5.12.0; extra == 'test'
 Requires-Dist: mypy==1.1.1; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.2.2; extra == 'test'
 Requires-Dist: requests-mock[fixture]<2.0.0,>=1.10.0; extra == 'test'
 Requires-Dist: types-requests==2.28.11.17; extra == 'test'
 Description-Content-Type: text/markdown
 
-# Shell GPT
-A command-line productivity tool powered by OpenAI's GPT-3.5 model. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort.
+# ShellGPT
+A command-line productivity tool powered by OpenAI's GPT models. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort. ShellGPT is cross-platform compatible and supports all major operating systems, including Linux, macOS, and Windows with all major shells, such as PowerShell, CMD, Bash, Zsh, Fish, and many others.
 
 https://user-images.githubusercontent.com/16740832/231569156-a3a9f9d4-18b1-4fff-a6e1-6807651aa894.mp4
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.8
+pip install shell-gpt==0.9.0
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -258,29 +258,49 @@
 >>> Change port to 443
 import requests
 response = requests.get('https://localhost:443')
 print(response.text)
 ```
 
 ### Chat sessions
-To list all the current chat sessions, use the `--list-chat` option:
+To list all the current chat sessions, use the `--list-chats` option:
 ```shell
-sgpt --list-chat
+sgpt --list-chats
 # .../shell_gpt/chat_cache/number
 # .../shell_gpt/chat_cache/python_request
 ```
 To show all the messages related to a specific chat session, use the `--show-chat` option followed by the session name:
 ```shell
 sgpt --show-chat number
 # user: please remember my favorite number: 4
 # assistant: I will remember that your favorite number is 4.
 # user: what would be my favorite number + 4?
 # assistant: Your favorite number is 4, so if we add 4 to it, the result would be 8.
 ```
 
+### Roles
+ShellGPT allows you to create custom roles, which can be utilized to generate code, shell commands, or to fulfill your specific needs. To create a new role, use the `--create-role` option followed by the role name. You will be prompted to provide a description for the role, along with other details. This will create a JSON file in `~/.config/shell_gpt/roles` with the role name. Inside this directory, you can also edit default `sgpt` roles, such as **shell**, **code**, and **default**. Use the `--list-roles` option to list all available roles, and the `--show-role` option to display the details of a specific role. Here's an example of a custom role:
+```shell
+sgpt --create-role json
+# Enter role description: You are JSON generator, provide only valid json as response.
+# Enter expecting result, e.g. answer, code, shell command, etc.: json
+sgpt --role json "random: user, password, email, address"
+{
+  "user": "JohnDoe",
+  "password": "p@ssw0rd",
+  "email": "johndoe@example.com",
+  "address": {
+    "street": "123 Main St",
+    "city": "Anytown",
+    "state": "CA",
+    "zip": "12345"
+  }
+}
+```
+
 ### Request cache
 Control cache using `--cache` (default) and `--no-cache` options. This caching applies for all `sgpt` requests to OpenAI API:
 ```shell
 sgpt "what are the colors of a rainbow"
 # -> The colors of a rainbow are red, orange, yellow, green, blue, indigo, and violet.
 ```
 Next time, same exact query will get results from local cache instantly. Note that `sgpt "what are the colors of a rainbow" --temperature 0.5` will make a new request, since we didn't provide `--temperature` (same applies to `--top-probability`) on previous request.
@@ -304,40 +324,50 @@
 CACHE_PATH=/tmp/shell_gpt/cache
 # Request timeout in seconds.
 REQUEST_TIMEOUT=60
 # Default OpenAI model to use.
 DEFAULT_MODEL=gpt-3.5-turbo
 # Default color for OpenAI completions.
 DEFAULT_COLOR=magenta
+# Force use system role messages (not recommended).
+SYSTEM_ROLES=false
 ```
 Possible options for `DEFAULT_COLOR`: black, red, green, yellow, blue, magenta, cyan, white, bright_black, bright_red, bright_green, bright_yellow, bright_blue, bright_magenta, bright_cyan, bright_white.
 
+Switch `SYSTEM_ROLES` to force use [system roles](https://help.openai.com/en/articles/7042661-chatgpt-api-transition-guide) messages, this is not recommended, since it doesn't perform well with current GPT models.
+
 ### Full list of arguments
 ```text
-╭─ Arguments ────────────────────────────────────────────────────────────────────────────────────────────────╮
-│   prompt      [PROMPT]  The prompt to generate completions for.                                            │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --model            [gpt-3.5-turbo|gpt-4|gpt-4-32k]  OpenAI GPT model to use. [default: gpt-3.5-turbo]      │
-│ --temperature      FLOAT RANGE [0.0<=x<=1.0]        Randomness of generated output. [default: 0.1]         │
-│ --top-probability  FLOAT RANGE [0.1<=x<=1.0]        Limits highest probable tokens (words). [default: 1.0] │
-│ --editor                                            Open $EDITOR to provide a prompt. [default: no-editor] │
-│ --cache                                             Cache completion results. [default: cache]             │
-│ --help                                              Show this message and exit.                            │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Assistance Options ───────────────────────────────────────────────────────────────────────────────────────╮
-│ --shell  -s                 Generate and execute shell commands.                                           │
-│ --code       --no-code      Generate only code. [default: no-code]                                         │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Chat Options ─────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --chat        TEXT  Follow conversation with id, use "temp" for quick session. [default: None]             │
-│ --repl        TEXT  Start a REPL (Read–eval–print loop) session. [default: None]                           │
-│ --show-chat   TEXT  Show all messages from provided chat id. [default: None]                               │
-│ --list-chat         List all existing chat ids. [default: no-list-chat]                                    │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────╮
+│   prompt      [PROMPT]  The prompt to generate completions for.                                             │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --model            [gpt-3.5-turbo|gpt-4|gpt-4-32k]  OpenAI GPT model to use. [default: gpt-3.5-turbo]       │
+│ --temperature      FLOAT RANGE [0.0<=x<=1.0]        Randomness of generated output. [default: 0.1]          │
+│ --top-probability  FLOAT RANGE [0.1<=x<=1.0]        Limits highest probable tokens (words). [default: 1.0]  │
+│ --editor                                            Open $EDITOR to provide a prompt. [default: no-editor]  │
+│ --cache                                             Cache completion results. [default: cache]              │
+│ --help                                              Show this message and exit.                             │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Assistance Options ────────────────────────────────────────────────────────────────────────────────────────╮
+│ --shell  -s                 Generate and execute shell commands.                                            │
+│ --code       --no-code      Generate only code. [default: no-code]                                          │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Chat Options ──────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --chat        TEXT  Follow conversation with id, use "temp" for quick session. [default: None]              │
+│ --repl        TEXT  Start a REPL (Read–eval–print loop) session. [default: None]                            │
+│ --show-chat   TEXT  Show all messages from provided chat id. [default: None]                                │
+│ --list-chats        List all existing chat ids. [default: no-list-chats]                                    │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Role Options ──────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --role         TEXT  System role for GPT model. [default: None]                                             │
+│ --create-role  TEXT  Create role. [default: None]                                                           │
+│ --show-role    TEXT  Show role. [default: None]                                                             │
+│ --list-roles         List roles. [default: no-list-roles]                                                   │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## Docker
 Run the container using the `OPENAI_API_KEY` environment variable, and a docker volume to store cache:
 ```shell
 docker run --rm \
            --env OPENAI_API_KEY="your OPENAI API key" \
```

