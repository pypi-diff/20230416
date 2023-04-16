# Comparing `tmp/pr-review-bot-0.1.1.tar.gz` & `tmp/pr-review-bot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr-review-bot-0.1.1.tar", last modified: Sun Apr 16 03:57:14 2023, max compression
+gzip compressed data, was "pr-review-bot-0.2.0.tar", last modified: Sun Apr 16 04:11:14 2023, max compression
```

## Comparing `pr-review-bot-0.1.1.tar` & `pr-review-bot-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:57:14.144160 pr-review-bot-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 03:57:02.000000 pr-review-bot-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-04-16 03:57:14.144160 pr-review-bot-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-16 03:57:02.000000 pr-review-bot-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:57:14.140160 pr-review-bot-0.1.1/pr_review_bot/
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-16 03:57:02.000000 pr-review-bot-0.1.1/pr_review_bot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:57:14.144160 pr-review-bot-0.1.1/pr_review_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-04-16 03:57:14.000000 pr-review-bot-0.1.1/pr_review_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-16 03:57:14.000000 pr-review-bot-0.1.1/pr_review_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 03:57:14.000000 pr-review-bot-0.1.1/pr_review_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-16 03:57:14.000000 pr-review-bot-0.1.1/pr_review_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 03:57:14.000000 pr-review-bot-0.1.1/pr_review_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-16 03:57:02.000000 pr-review-bot-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 03:57:14.144160 pr-review-bot-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:57:14.144160 pr-review-bot-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-16 03:57:02.000000 pr-review-bot-0.1.1/tests/test_pr_review_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:11:14.100895 pr-review-bot-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 04:10:58.000000 pr-review-bot-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-16 04:11:14.100895 pr-review-bot-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-16 04:10:58.000000 pr-review-bot-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:11:14.100895 pr-review-bot-0.2.0/pr_review_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-16 04:10:58.000000 pr-review-bot-0.2.0/pr_review_bot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:11:14.100895 pr-review-bot-0.2.0/pr_review_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-16 04:11:14.000000 pr-review-bot-0.2.0/pr_review_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-16 04:11:14.000000 pr-review-bot-0.2.0/pr_review_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 04:11:14.000000 pr-review-bot-0.2.0/pr_review_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-16 04:11:14.000000 pr-review-bot-0.2.0/pr_review_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 04:11:14.000000 pr-review-bot-0.2.0/pr_review_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-16 04:10:58.000000 pr-review-bot-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 04:11:14.100895 pr-review-bot-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:11:14.100895 pr-review-bot-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-16 04:10:58.000000 pr-review-bot-0.2.0/tests/test_pr_review_bot.py
```

### Comparing `pr-review-bot-0.1.1/LICENSE` & `pr-review-bot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pr-review-bot-0.1.1/PKG-INFO` & `pr-review-bot-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-review-bot
-Version: 0.1.1
+Version: 0.2.0
 Summary: Automated PR review bot using GPT-3.5-turbo
 Author-email: Kyryl Truskovskyi <truskovskiyk@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,18 +205,72 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pr-reviewer
-Use LLM to help you with PR review 
 
+Streamline Your GitHub Pull Requests with AI, co-authored with GPT4.
 
-https://platform.openai.com/account/api-keys
-https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
+🚀 Excited to announce our new open-source project: PR Review Bot, a GitHub Pull Request review bot powered by OpenAI's GPT-3.5-turbo!
+🤖 PR Review Bot automatically reviews open PRs in your GitHub repository, providing helpful feedback and even approving or requesting changes based on the analysis of the PR text and comments.
+🔧 Save time and effort in your development workflow by automating the initial review process, ensuring PRs adhere to your project's guidelines and best practices.
 
+🌟 Key features:
+- Automatically reviews open PRs
+- Leverages OpenAI's GPT-3.5-turbo for intelligent analysis and feedback
+- Can be easily customized to fit your project needs
+- Easy to set up and use
+- Costs analysis of each review
+
+## Example 
+
+![alt text](./docs/example.png)
+
+## Install
+
+```
+pip install pr-review-bot
+```
+
+
+## Setup
+
+```
+export PR_REVIEW_BOT_TOKEN='your github token'
+export PR_REVIEW_BOT_OPEN_AI_KEY='your open ai key'
+export PR_REVIEW_BOT_OWNER='github user'
+export PR_REVIEW_BOT_REPO_NAME='github repo'
+```
+
+How to get [Github token](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
+How to get [Open AI key](https://platform.openai.com/account/api-keys)
+
+
+## Usage
+
+To review all open pull requests:
+
+```
+pr-review-bot review-all-open-pr
+```
+
+To review a specific pull request:
+
+```
+pr-review-bot review-pr <PR nuber>
+```
+
+For help:
+
+
+```
+pr-review-bot --help
+```
+
+## Testing 
 
 
 ```
-python pr_review_bot.py review-pr --pr_number <PR_NUMBER>
+pytest --cov=pr_review_bot test_pr_review_bot.py
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pr-review-bot-0.1.1/pr_review_bot/__init__.py` & `pr-review-bot-0.2.0/pr_review_bot/__init__.py`

 * *Files identical despite different names*

### Comparing `pr-review-bot-0.1.1/pr_review_bot.egg-info/PKG-INFO` & `pr-review-bot-0.2.0/pr_review_bot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-review-bot
-Version: 0.1.1
+Version: 0.2.0
 Summary: Automated PR review bot using GPT-3.5-turbo
 Author-email: Kyryl Truskovskyi <truskovskiyk@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,18 +205,72 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pr-reviewer
-Use LLM to help you with PR review 
 
+Streamline Your GitHub Pull Requests with AI, co-authored with GPT4.
 
-https://platform.openai.com/account/api-keys
-https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
+🚀 Excited to announce our new open-source project: PR Review Bot, a GitHub Pull Request review bot powered by OpenAI's GPT-3.5-turbo!
+🤖 PR Review Bot automatically reviews open PRs in your GitHub repository, providing helpful feedback and even approving or requesting changes based on the analysis of the PR text and comments.
+🔧 Save time and effort in your development workflow by automating the initial review process, ensuring PRs adhere to your project's guidelines and best practices.
 
+🌟 Key features:
+- Automatically reviews open PRs
+- Leverages OpenAI's GPT-3.5-turbo for intelligent analysis and feedback
+- Can be easily customized to fit your project needs
+- Easy to set up and use
+- Costs analysis of each review
+
+## Example 
+
+![alt text](./docs/example.png)
+
+## Install
+
+```
+pip install pr-review-bot
+```
+
+
+## Setup
+
+```
+export PR_REVIEW_BOT_TOKEN='your github token'
+export PR_REVIEW_BOT_OPEN_AI_KEY='your open ai key'
+export PR_REVIEW_BOT_OWNER='github user'
+export PR_REVIEW_BOT_REPO_NAME='github repo'
+```
+
+How to get [Github token](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
+How to get [Open AI key](https://platform.openai.com/account/api-keys)
+
+
+## Usage
+
+To review all open pull requests:
+
+```
+pr-review-bot review-all-open-pr
+```
+
+To review a specific pull request:
+
+```
+pr-review-bot review-pr <PR nuber>
+```
+
+For help:
+
+
+```
+pr-review-bot --help
+```
+
+## Testing 
 
 
 ```
-python pr_review_bot.py review-pr --pr_number <PR_NUMBER>
+pytest --cov=pr_review_bot test_pr_review_bot.py
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pr-review-bot-0.1.1/pyproject.toml` & `pr-review-bot-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pr-review-bot"
-version = "0.1.1"
+version = "0.2.0"
 description = "Automated PR review bot using GPT-3.5-turbo"
 authors = [
     {name = "Kyryl Truskovskyi", email = "truskovskiyk@gmail.com"}
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
```

### Comparing `pr-review-bot-0.1.1/tests/test_pr_review_bot.py` & `pr-review-bot-0.2.0/tests/test_pr_review_bot.py`

 * *Files identical despite different names*

