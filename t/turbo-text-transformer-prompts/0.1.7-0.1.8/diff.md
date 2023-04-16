# Comparing `tmp/turbo_text_transformer_prompts-0.1.7.tar.gz` & `tmp/turbo_text_transformer_prompts-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_text_transformer_prompts-0.1.7.tar", max compression
+gzip compressed data, was "turbo_text_transformer_prompts-0.1.8.tar", max compression
```

## Comparing `turbo_text_transformer_prompts-0.1.7.tar` & `turbo_text_transformer_prompts-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     2007 2023-03-03 19:53:29.958567 turbo_text_transformer_prompts-0.1.7/README.md
--rw-r--r--   0        0        0      774 2023-03-04 21:45:46.855564 turbo_text_transformer_prompts-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      265 2023-03-02 21:35:52.671900 turbo_text_transformer_prompts-0.1.7/templates/alter.j2
--rw-r--r--   0        0        0      477 2023-03-04 20:49:54.272282 turbo_text_transformer_prompts-0.1.7/templates/assist.j2
--rw-r--r--   0        0        0       55 2023-03-02 17:14:44.488234 turbo_text_transformer_prompts-0.1.7/templates/chat.j2
--rw-r--r--   0        0        0       63 2023-03-02 17:18:53.675373 turbo_text_transformer_prompts-0.1.7/templates/code.j2
--rw-r--r--   0        0        0      440 2023-03-02 16:21:57.171112 turbo_text_transformer_prompts-0.1.7/templates/docstring.j2
--rw-r--r--   0        0        0       11 2023-03-02 17:04:53.985181 turbo_text_transformer_prompts-0.1.7/templates/empty.j2
--rw-r--r--   0        0        0      417 2023-03-04 13:53:53.193075 turbo_text_transformer_prompts-0.1.7/templates/fix_ocr.j2
--rw-r--r--   0        0        0      145 2023-03-04 19:42:57.723042 turbo_text_transformer_prompts-0.1.7/templates/html.j2
--rw-r--r--   0        0        0      181 2023-03-02 21:36:52.727501 turbo_text_transformer_prompts-0.1.7/templates/improvements.j2
--rw-r--r--   0        0        0       86 2023-03-04 15:13:00.273785 turbo_text_transformer_prompts-0.1.7/templates/poet.j2
--rw-r--r--   0        0        0     3992 2023-03-02 16:30:49.856054 turbo_text_transformer_prompts-0.1.7/templates/prose-to-script-2-shot.j2
--rw-r--r--   0        0        0      209 2023-03-04 15:22:03.857907 turbo_text_transformer_prompts-0.1.7/templates/prose2script.j2
--rw-r--r--   0        0        0      273 2023-03-04 16:27:49.570819 turbo_text_transformer_prompts-0.1.7/templates/readme.j2
--rw-r--r--   0        0        0      518 2023-03-02 17:01:26.417534 turbo_text_transformer_prompts-0.1.7/templates/researcher.j2
--rw-r--r--   0        0        0     3972 2023-03-02 16:32:37.718633 turbo_text_transformer_prompts-0.1.7/templates/script-to-prose-2-shot.j2
--rw-r--r--   0        0        0       74 2023-03-02 17:18:31.863455 turbo_text_transformer_prompts-0.1.7/templates/shell.j2
--rw-r--r--   0        0        0      256 2023-03-02 20:25:22.614651 turbo_text_transformer_prompts-0.1.7/templates/summary-2-shot.j2
--rw-r--r--   0        0        0      256 2023-03-02 20:25:05.898790 turbo_text_transformer_prompts-0.1.7/templates/summary.j2
--rw-r--r--   0        0        0       91 2023-03-04 15:11:00.462692 turbo_text_transformer_prompts-0.1.7/templates/whitman.j2
--rw-r--r--   0        0        0        0 2023-03-03 19:26:48.136962 turbo_text_transformer_prompts-0.1.7/tttp/__init__.py
--rw-r--r--   0        0        0      915 2023-03-04 13:29:45.936013 turbo_text_transformer_prompts-0.1.7/tttp/__main__.py
--rw-r--r--   0        0        0     1386 2023-03-04 13:29:29.036168 turbo_text_transformer_prompts-0.1.7/tttp/prompter.py
--rw-r--r--   0        0        0     2818 1970-01-01 00:00:00.000000 turbo_text_transformer_prompts-0.1.7/setup.py
--rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 turbo_text_transformer_prompts-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2210 2023-03-05 12:22:21.828232 turbo_text_transformer_prompts-0.1.8/README.md
+-rw-r--r--   0        0        0      774 2023-03-06 09:01:16.930199 turbo_text_transformer_prompts-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      265 2023-03-02 21:35:52.671900 turbo_text_transformer_prompts-0.1.8/templates/alter.j2
+-rw-r--r--   0        0        0      477 2023-03-04 20:49:54.272282 turbo_text_transformer_prompts-0.1.8/templates/assist.j2
+-rw-r--r--   0        0        0       55 2023-03-02 17:14:44.488234 turbo_text_transformer_prompts-0.1.8/templates/chat.j2
+-rw-r--r--   0        0        0      416 2023-03-06 09:00:24.814350 turbo_text_transformer_prompts-0.1.8/templates/code-summary.j2
+-rw-r--r--   0        0        0       63 2023-03-02 17:18:53.675373 turbo_text_transformer_prompts-0.1.8/templates/code.j2
+-rw-r--r--   0        0        0      440 2023-03-02 16:21:57.171112 turbo_text_transformer_prompts-0.1.8/templates/docstring.j2
+-rw-r--r--   0        0        0       11 2023-03-02 17:04:53.985181 turbo_text_transformer_prompts-0.1.8/templates/empty.j2
+-rw-r--r--   0        0        0      320 2023-03-05 15:10:07.852854 turbo_text_transformer_prompts-0.1.8/templates/fix_ocr.j2
+-rw-r--r--   0        0        0      145 2023-03-04 19:42:57.723042 turbo_text_transformer_prompts-0.1.8/templates/html.j2
+-rw-r--r--   0        0        0      181 2023-03-02 21:36:52.727501 turbo_text_transformer_prompts-0.1.8/templates/improvements.j2
+-rw-r--r--   0        0        0       86 2023-03-04 15:13:00.273785 turbo_text_transformer_prompts-0.1.8/templates/poet.j2
+-rw-r--r--   0        0        0     3992 2023-03-02 16:30:49.856054 turbo_text_transformer_prompts-0.1.8/templates/prose-to-script-2-shot.j2
+-rw-r--r--   0        0        0      209 2023-03-04 15:22:03.857907 turbo_text_transformer_prompts-0.1.8/templates/prose2script.j2
+-rw-r--r--   0        0        0      273 2023-03-04 16:27:49.570819 turbo_text_transformer_prompts-0.1.8/templates/readme.j2
+-rw-r--r--   0        0        0      518 2023-03-02 17:01:26.417534 turbo_text_transformer_prompts-0.1.8/templates/researcher.j2
+-rw-r--r--   0        0        0     3972 2023-03-02 16:32:37.718633 turbo_text_transformer_prompts-0.1.8/templates/script-to-prose-2-shot.j2
+-rw-r--r--   0        0        0       74 2023-03-02 17:18:31.863455 turbo_text_transformer_prompts-0.1.8/templates/shell.j2
+-rw-r--r--   0        0        0      256 2023-03-02 20:25:22.614651 turbo_text_transformer_prompts-0.1.8/templates/summary-2-shot.j2
+-rw-r--r--   0        0        0      256 2023-03-02 20:25:05.898790 turbo_text_transformer_prompts-0.1.8/templates/summary.j2
+-rw-r--r--   0        0        0       91 2023-03-04 15:11:00.462692 turbo_text_transformer_prompts-0.1.8/templates/whitman.j2
+-rw-r--r--   0        0        0        0 2023-03-03 19:26:48.136962 turbo_text_transformer_prompts-0.1.8/tttp/__init__.py
+-rw-r--r--   0        0        0      915 2023-03-04 13:29:45.936013 turbo_text_transformer_prompts-0.1.8/tttp/__main__.py
+-rw-r--r--   0        0        0     1386 2023-03-04 13:29:29.036168 turbo_text_transformer_prompts-0.1.8/tttp/prompter.py
+-rw-r--r--   0        0        0     3034 1970-01-01 00:00:00.000000 turbo_text_transformer_prompts-0.1.8/setup.py
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 turbo_text_transformer_prompts-0.1.8/PKG-INFO
```

### Comparing `turbo_text_transformer_prompts-0.1.7/README.md` & `turbo_text_transformer_prompts-0.1.8/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Turbo Text Transformer Prompts
 
+Note this is automatically installed when you do `pip install turbo-text-transformer`. This repo is just for storing the templates.
+
 Designed for use with [turbo-text-transformer](https://github.com/fergusfettes/turbo-text-transformer).
 
-You pipe some text in, the template is applied, then you pipe it into `ttt` which will process it with eg. OpenAI.
+You pipe some text in, the template is applied, then you pipe it into `ttt` (from `pip install turbo-text-transformer`) which will process it with eg. OpenAI.
 
 ```
 cat pyproject.toml tttp/__main__.py | tttp -t readme | ttt > README.md
 ```
 
 Turbo Text Transformer Prompts is a command-line tool that allows users to generate text files from pre-configured templates using user input prompts. The tool uses Jinja2 templating engine to render text files from templates.
 
@@ -16,46 +18,53 @@
 pip install turbo-text-transformer-prompts
 ```
 
 You will also need to clone the repository containing the templates you want to use. For example:
 
 ```sh
 mkdir -p ~/.config/ttt/
-git clone https://github.com/fergusfettes/turbo-text-transformer-prompts ~/.config/tttp
+git clone https://github.com/fergusfettes/turbo-text-transformer-prompts ~/.config/ttt
 ```
 
 ## Template Structure
 
-A template is a text file written in Jinja2 syntax. The file should have the `.j2` extension and be placed inside the `templates` directory.
+A template is a text file written in Jinja2 syntax. The file should have the `.j2` extension and be placed inside the `templates` directory. They will be installed in the `~/.config/ttt/templates` directory.
 
-The template can contain placeholders for user input. Placeholders are enclosed in double curly braces and contain a variable name. For example:
+This is a smiple example of a template:
 
 ```jinja
-Hello, {{ name }}!
+Context: Provide only code as output.
+Prompt: {{prompt}}
+Code:
 ```
 
-This template will prompt the user to enter a value for the `name` variable.
+It will just output a code snippet based on the query.
 
-## Prompt Files
+You can also pass a list of flags to the prompt to fine tune the control, such as this:
 
-Prompt files can be used to predefine the values to be filled in the template. Prompt files are text files that contain a prompt message followed by the values to be filled, one per line. For example:
+```jinja
+This is an example of minimally altering some given code to achieve a specific task.
 
-```
-Please enter your name:
-John Doe
-```
+I received the following code:
 
-To use a prompt file, specify the file using the `--prompt` option:
+`{{language}}
+{{prompt}}
+`
 
-```sh
-tttp --filename simple --prompt /path/to/prompt/file
+My task was to make minimal alterations to this code to: "{{task}}".
+
+The altered code is below.
+
+`{{language}}
 ```
 
-If there are any values that need to be added or changed from
+For this one, you can pass the 'task' and 'language' arguments to make it more specific.
 
 ## Contributing
 
+PULL REQUESTS WITH MORE TEMPLATES VERY WELCOME!
+
 If you find a bug or would like to contribute to Turbo Text Transformer Prompts, please create a new GitHub issue or pull request.
 
 #  License
 
 Turbo Text Transformer Prompts is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
```

### Comparing `turbo_text_transformer_prompts-0.1.7/pyproject.toml` & `turbo_text_transformer_prompts-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turbo-text-transformer-prompts"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["fergus <fergusfettes@gmail.com>"]
 readme = "README.md"
 packages = [{include = "tttp"}]
 include = [{path = "templates/*.j2"}]
 
 [tool.poetry.dependencies]
@@ -17,15 +17,15 @@
 ipdb = "^0.13.11"
 
 [tool.poetry.scripts]
 tttp = "tttp.__main__:main"
 
 [project]
 name = "turbo-text-transformer-prompts"
-version = "0.1.7"
+version = "0.1.8"
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.scripts]
 tttp = "tttp.__main__:main"
```

### Comparing `turbo_text_transformer_prompts-0.1.7/templates/prose-to-script-2-shot.j2` & `turbo_text_transformer_prompts-0.1.8/templates/prose-to-script-2-shot.j2`

 * *Files identical despite different names*

### Comparing `turbo_text_transformer_prompts-0.1.7/templates/researcher.j2` & `turbo_text_transformer_prompts-0.1.8/templates/researcher.j2`

 * *Files identical despite different names*

### Comparing `turbo_text_transformer_prompts-0.1.7/templates/script-to-prose-2-shot.j2` & `turbo_text_transformer_prompts-0.1.8/templates/script-to-prose-2-shot.j2`

 * *Files identical despite different names*

### Comparing `turbo_text_transformer_prompts-0.1.7/tttp/__main__.py` & `turbo_text_transformer_prompts-0.1.8/tttp/__main__.py`

 * *Files identical despite different names*

### Comparing `turbo_text_transformer_prompts-0.1.7/tttp/prompter.py` & `turbo_text_transformer_prompts-0.1.8/tttp/prompter.py`

 * *Files identical despite different names*

### Comparing `turbo_text_transformer_prompts-0.1.7/setup.py` & `turbo_text_transformer_prompts-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['click>=8.1.3,<9.0.0', 'ipython>=8.10.0,<9.0.0', 'jinja2>=3.1.2,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['tttp = tttp.__main__:main']}
 
 setup_kwargs = {
     'name': 'turbo-text-transformer-prompts',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': '',
-    'long_description': '# Turbo Text Transformer Prompts\n\nDesigned for use with [turbo-text-transformer](https://github.com/fergusfettes/turbo-text-transformer).\n\nYou pipe some text in, the template is applied, then you pipe it into `ttt` which will process it with eg. OpenAI.\n\n```\ncat pyproject.toml tttp/__main__.py | tttp -t readme | ttt > README.md\n```\n\nTurbo Text Transformer Prompts is a command-line tool that allows users to generate text files from pre-configured templates using user input prompts. The tool uses Jinja2 templating engine to render text files from templates.\n\n## How to Run\n\n```sh\npip install turbo-text-transformer-prompts\n```\n\nYou will also need to clone the repository containing the templates you want to use. For example:\n\n```sh\nmkdir -p ~/.config/ttt/\ngit clone https://github.com/fergusfettes/turbo-text-transformer-prompts ~/.config/tttp\n```\n\n## Template Structure\n\nA template is a text file written in Jinja2 syntax. The file should have the `.j2` extension and be placed inside the `templates` directory.\n\nThe template can contain placeholders for user input. Placeholders are enclosed in double curly braces and contain a variable name. For example:\n\n```jinja\nHello, {{ name }}!\n```\n\nThis template will prompt the user to enter a value for the `name` variable.\n\n## Prompt Files\n\nPrompt files can be used to predefine the values to be filled in the template. Prompt files are text files that contain a prompt message followed by the values to be filled, one per line. For example:\n\n```\nPlease enter your name:\nJohn Doe\n```\n\nTo use a prompt file, specify the file using the `--prompt` option:\n\n```sh\ntttp --filename simple --prompt /path/to/prompt/file\n```\n\nIf there are any values that need to be added or changed from\n\n## Contributing\n\nIf you find a bug or would like to contribute to Turbo Text Transformer Prompts, please create a new GitHub issue or pull request.\n\n#  License\n\nTurbo Text Transformer Prompts is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.\n',
+    'long_description': '# Turbo Text Transformer Prompts\n\nNote this is automatically installed when you do `pip install turbo-text-transformer`. This repo is just for storing the templates.\n\nDesigned for use with [turbo-text-transformer](https://github.com/fergusfettes/turbo-text-transformer).\n\nYou pipe some text in, the template is applied, then you pipe it into `ttt` (from `pip install turbo-text-transformer`) which will process it with eg. OpenAI.\n\n```\ncat pyproject.toml tttp/__main__.py | tttp -t readme | ttt > README.md\n```\n\nTurbo Text Transformer Prompts is a command-line tool that allows users to generate text files from pre-configured templates using user input prompts. The tool uses Jinja2 templating engine to render text files from templates.\n\n## How to Run\n\n```sh\npip install turbo-text-transformer-prompts\n```\n\nYou will also need to clone the repository containing the templates you want to use. For example:\n\n```sh\nmkdir -p ~/.config/ttt/\ngit clone https://github.com/fergusfettes/turbo-text-transformer-prompts ~/.config/ttt\n```\n\n## Template Structure\n\nA template is a text file written in Jinja2 syntax. The file should have the `.j2` extension and be placed inside the `templates` directory. They will be installed in the `~/.config/ttt/templates` directory.\n\nThis is a smiple example of a template:\n\n```jinja\nContext: Provide only code as output.\nPrompt: {{prompt}}\nCode:\n```\n\nIt will just output a code snippet based on the query.\n\nYou can also pass a list of flags to the prompt to fine tune the control, such as this:\n\n```jinja\nThis is an example of minimally altering some given code to achieve a specific task.\n\nI received the following code:\n\n`{{language}}\n{{prompt}}\n`\n\nMy task was to make minimal alterations to this code to: "{{task}}".\n\nThe altered code is below.\n\n`{{language}}\n```\n\nFor this one, you can pass the \'task\' and \'language\' arguments to make it more specific.\n\n## Contributing\n\nPULL REQUESTS WITH MORE TEMPLATES VERY WELCOME!\n\nIf you find a bug or would like to contribute to Turbo Text Transformer Prompts, please create a new GitHub issue or pull request.\n\n#  License\n\nTurbo Text Transformer Prompts is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.\n',
     'author': 'fergus',
     'author_email': 'fergusfettes@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `turbo_text_transformer_prompts-0.1.7/PKG-INFO` & `turbo_text_transformer_prompts-0.1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo-text-transformer-prompts
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: fergus
 Author-email: fergusfettes@gmail.com
 Requires-Python: >3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,17 +12,19 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: ipython (>=8.10.0,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Turbo Text Transformer Prompts
 
+Note this is automatically installed when you do `pip install turbo-text-transformer`. This repo is just for storing the templates.
+
 Designed for use with [turbo-text-transformer](https://github.com/fergusfettes/turbo-text-transformer).
 
-You pipe some text in, the template is applied, then you pipe it into `ttt` which will process it with eg. OpenAI.
+You pipe some text in, the template is applied, then you pipe it into `ttt` (from `pip install turbo-text-transformer`) which will process it with eg. OpenAI.
 
 ```
 cat pyproject.toml tttp/__main__.py | tttp -t readme | ttt > README.md
 ```
 
 Turbo Text Transformer Prompts is a command-line tool that allows users to generate text files from pre-configured templates using user input prompts. The tool uses Jinja2 templating engine to render text files from templates.
 
@@ -32,47 +34,54 @@
 pip install turbo-text-transformer-prompts
 ```
 
 You will also need to clone the repository containing the templates you want to use. For example:
 
 ```sh
 mkdir -p ~/.config/ttt/
-git clone https://github.com/fergusfettes/turbo-text-transformer-prompts ~/.config/tttp
+git clone https://github.com/fergusfettes/turbo-text-transformer-prompts ~/.config/ttt
 ```
 
 ## Template Structure
 
-A template is a text file written in Jinja2 syntax. The file should have the `.j2` extension and be placed inside the `templates` directory.
+A template is a text file written in Jinja2 syntax. The file should have the `.j2` extension and be placed inside the `templates` directory. They will be installed in the `~/.config/ttt/templates` directory.
 
-The template can contain placeholders for user input. Placeholders are enclosed in double curly braces and contain a variable name. For example:
+This is a smiple example of a template:
 
 ```jinja
-Hello, {{ name }}!
+Context: Provide only code as output.
+Prompt: {{prompt}}
+Code:
 ```
 
-This template will prompt the user to enter a value for the `name` variable.
+It will just output a code snippet based on the query.
 
-## Prompt Files
+You can also pass a list of flags to the prompt to fine tune the control, such as this:
 
-Prompt files can be used to predefine the values to be filled in the template. Prompt files are text files that contain a prompt message followed by the values to be filled, one per line. For example:
+```jinja
+This is an example of minimally altering some given code to achieve a specific task.
 
-```
-Please enter your name:
-John Doe
-```
+I received the following code:
 
-To use a prompt file, specify the file using the `--prompt` option:
+`{{language}}
+{{prompt}}
+`
 
-```sh
-tttp --filename simple --prompt /path/to/prompt/file
+My task was to make minimal alterations to this code to: "{{task}}".
+
+The altered code is below.
+
+`{{language}}
 ```
 
-If there are any values that need to be added or changed from
+For this one, you can pass the 'task' and 'language' arguments to make it more specific.
 
 ## Contributing
 
+PULL REQUESTS WITH MORE TEMPLATES VERY WELCOME!
+
 If you find a bug or would like to contribute to Turbo Text Transformer Prompts, please create a new GitHub issue or pull request.
 
 #  License
 
 Turbo Text Transformer Prompts is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
```

