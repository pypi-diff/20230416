# Comparing `tmp/samosa-0.1.4.tar.gz` & `tmp/samosa-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samosa-0.1.4.tar", last modified: Mon Oct 17 12:58:09 2022, max compression
+gzip compressed data, was "samosa-0.2.5.tar", last modified: Sun Apr 16 10:44:53 2023, max compression
```

## Comparing `samosa-0.1.4.tar` & `samosa-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-rw-r--   0 user      (1000) user      (1000)    34020 2022-10-17 12:49:47.091684 samosa-0.1.4/COPYING
--rw-rw-r--   0 user      (1000) user      (1000)    34020 2022-09-20 10:34:01.691268 samosa-0.1.4/LICENSES/AGPL-3.0-or-later.txt
--rw-rw-r--   0 user      (1000) user      (1000)    17023 2022-10-17 12:49:47.091684 samosa-0.1.4/LICENSES/CC-BY-4.0.txt
--rw-rw-r--   0 user      (1000) user      (1000)     7048 2022-09-20 10:34:01.987267 samosa-0.1.4/LICENSES/CC0-1.0.txt
--rwxrwxr-x   0 user      (1000) user      (1000)      119 2022-10-17 12:49:47.091684 samosa-0.1.4/LICENSES/LicenseRef-DCO-1.1-license.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1078 2022-09-20 10:34:02.239266 samosa-0.1.4/LICENSES/MIT.txt
--rw-rw-r--   0 user      (1000) user      (1000)     3852 2022-10-17 12:49:47.091684 samosa-0.1.4/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      920 2022-09-20 10:31:40.819942 samosa-0.1.4/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-09-05 19:43:31.181836 samosa-0.1.4/samosa/__init__.py
--rwxrwxr-x   0 user      (1000) user      (1000)      621 2022-09-20 10:31:40.843942 samosa-0.1.4/samosa/cli.py
--rwxrwxr-x   0 user      (1000) user      (1000)     6407 2022-09-26 12:58:44.334810 samosa-0.1.4/samosa/git.py
--rw-------   0 user      (1000) user      (1000)     1481 2022-09-28 18:05:21.481553 samosa-0.1.4/samosa/resource/WORKFLOW.md
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-08-19 15:26:37.559922 samosa-0.1.4/samosa/resource/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      313 2022-08-23 18:06:28.554341 samosa-0.1.4/samosa/resource/pre-commit
--rw-------   0 user      (1000) user      (1000)     4124 2022-10-17 12:58:09.768731 samosa-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    34020 2023-04-16 10:40:49.037045 samosa-0.2.5/COPYING
+-rw-r--r--   0        0        0    34020 2022-09-20 10:34:01.691268 samosa-0.2.5/LICENSES/AGPL-3.0-or-later.txt
+-rw-r--r--   0        0        0    17023 2022-10-17 12:49:47.091684 samosa-0.2.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0        0        0     7048 2022-09-20 10:34:01.987267 samosa-0.2.5/LICENSES/CC0-1.0.txt
+-rwxr-xr-x   0        0        0      119 2023-04-16 10:40:49.037045 samosa-0.2.5/LICENSES/LicenseRef-DCO-1.1-license.txt
+-rw-r--r--   0        0        0     1078 2022-09-20 10:34:02.239265 samosa-0.2.5/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     3985 2023-04-16 10:44:42.109886 samosa-0.2.5/README.md
+-rw-r--r--   0        0        0      829 2023-04-16 10:44:53.105931 samosa-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 10:43:51.633685 samosa-0.2.5/src/samosa/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-16 10:43:51.633685 samosa-0.2.5/src/samosa/cli.py
+-rwxr-xr-x   0        0        0     6406 2023-04-16 10:43:51.633685 samosa-0.2.5/src/samosa/git.py
+-rw-r--r--   0        0        0     1503 2023-04-16 10:44:42.117886 samosa-0.2.5/src/samosa/resource/WORKFLOW.md
+-rw-r--r--   0        0        0        0 2023-04-16 10:43:51.633685 samosa-0.2.5/src/samosa/resource/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-16 10:43:51.633685 samosa-0.2.5/src/samosa/resource/pre-commit
+-rw-r--r--   0        0        0      287 2023-04-16 10:43:51.633685 samosa-0.2.5/tests/test_git.py
+-rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 samosa-0.2.5/PKG-INFO
```

### Comparing `samosa-0.1.4/COPYING` & `samosa-0.2.5/COPYING`

 * *Files identical despite different names*

### Comparing `samosa-0.1.4/LICENSES/AGPL-3.0-or-later.txt` & `samosa-0.2.5/LICENSES/AGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `samosa-0.1.4/LICENSES/CC-BY-4.0.txt` & `samosa-0.2.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `samosa-0.1.4/LICENSES/CC0-1.0.txt` & `samosa-0.2.5/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `samosa-0.1.4/LICENSES/MIT.txt` & `samosa-0.2.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `samosa-0.1.4/README.md` & `samosa-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Samosa (समोसा)
 
 Enforce a triangular Git workflow. If this is not possible, explain why.
 
 ## Usage
 
 ```bash
-cd <repository-folder>
+cd [repository-folder]
 samosa
 ```
 
 If any checks fail, Samosa will attempt to make a correction. If the correction
 cannot be made automatically, Samosa will make a suggestion and terminate with
 exit code 1 (error).
 
@@ -32,15 +32,15 @@
 See WORKFLOW.md for a detailed workflow that results in a samosa standard
 repository.
 
 ## Roadmap (don't hold your breath)
 
 - `samosa clone`: interactive prompts that follow the suggested workflow
 - `samosa checkout`: in samosa repository, checkout a new branch, hooked up
-  correctly
+    correctly
 - `samosa refresh`: fetch all, and pull main
 - `samosa log`: show log since `upstream/main`
 - `samosa diff`: show diff from `upstream/main`
 
 ## Suggestions
 
 ### Sole maintainer: origin = upstream
@@ -49,14 +49,15 @@
 upstream repositories. In this case, set both to the same value. When
 contribution activity justifies a project repository outside your personal
 namespace, create it and update your "upstream" value.
 
 ## Out of scope
 
 - Detecting/supporting other workflows.
+- [Oh shit, git!](https://wizardzines.com/zines/oh-shit-git/)
 
 ## Acknowledgements
 
 WORKFLOW.md and the associated pre-commit bash script are derived from Aaron
 Bull Schaefer's excellent
 [Git Triangular Workflow](https://gist.github.com/elasticdog/164fe1bb75ad645abd30d545382a1542).
 License details are included in the relevant files.
@@ -65,54 +66,60 @@
 
 - [Git 2.5, including multiple worktrees and triangular workflows](https://github.blog/2015-07-29-git-2-5-including-multiple-worktrees-and-triangular-workflows/)
 - [Triangle workflows](https://gist.github.com/anjohnson/8994c95ab2a06f7d2339)
 - [Forking workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow)
 - [Integration-manager workflow](https://git-scm.com/book/tl/v2/Distributed-Git-Distributed-Workflows#_integration_manager)
 - [Git forking workflow, what names for the remotes?](https://stackoverflow.com/q/38965156/236081)
 
+<!-- start @generated footer -->
+
 # Development environment
 
 ## Install prerequisites
 
 - Python 3.10
 - pdm
+- make
 
 ## Instructions
 
 - Fork the upstream repository.
-- `git clone <fork-url>`
+- `git clone [fork-url]`
+- `cd [project-folder]`
 - Run `make develop` to initialise your development environment.
 
 You can use any text editor or IDE that supports virtualenv / pdm. See the
 Makefile for toolchain details.
 
 Please `make test` and `make lint` before submitting changes.
 
 ## Make targets
 
 ```
-USAGE: make <target>
+USAGE: make [target]
 
 help    : Show this message.
 develop : Set up Python development environment.
 run     : Run from source.
 clean   : Remove all build artefacts.
 test    : Run tests and generate coverage report.
 lint    : Fix or warn about linting errors.
 build   : Clean, test, lint, then generate new build artefacts.
 publish : Upload build artefacts to PyPI.
 ```
 
 # Sharing and contributions
 
-Samosa (समोसा) \
-<https://gitlab.com/lofidevops/samosa> \
-Copyright 2022 David Seaward and contributors \
+```
+Samosa (समोसा)
+https://lofidevops.neocities.org
+Copyright 2022 David Seaward and contributors
 SPDX-License-Identifier: AGPL-3.0-or-later
+```
 
 Shared under AGPL-3.0-or-later. We adhere to the Contributor Covenant 2.1, and
 certify origin per DCO 1.1 with a signed-off-by line. Contributions under the
 same terms are welcome.
 
 Submit security and conduct issues as private tickets. Sign commits with
 `git commit --signoff`. For a software bill of materials run `reuse spdx`. For
-more details see LICENSES, CONDUCT and DCO.
+more details see CONDUCT, COPYING and CONTRIBUTING.
```

### Comparing `samosa-0.1.4/pyproject.toml` & `samosa-0.2.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 [project]
 name = "samosa"
-version = "0.1.4"
 description = "Enforce a triangular Git workflow. If this is not possible, explain why."
-authors = [
-    { name = "David Seaward", email = "david@librem.one" },
-]
-dependencies = [
-    "pygit2>=1.10.0",
-]
+authors = []
+dependencies = []
 requires-python = ">=3.10"
 readme = "README.md"
+dynamic = []
+version = "0.2.5"
 
 [project.license]
 text = "AGPL-3.0-or-later"
 
 [project.optional-dependencies]
 
 [project.scripts]
 samosa = "samosa.cli:invoke"
 
+[project.urls]
+Source = "https://gitlab.com/lfdo/toolchain/samosa"
+Project = "https://lofidevops.neocities.org"
+
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "reuse>=1.0.0",
-    "mdformat>=0.7.16",
+    "carmine>=0.0.3",
 ]
 
-[tool.syllabub.files]
-body = "static/body.md"
-logo = "static/logo.png"
+[tool.pdm.version]
+source = "scm"
 
 [tool.syllabub.project]
 conduct = "contributor-covenant-2.1"
 copyright = "Copyright 2022 David Seaward and contributors"
 origin = "DCO-1.1-git-signoff"
-sbom = "reuse spdx"
 title = "Samosa (समोसा)"
-url = "https://gitlab.com/lofidevops/samosa"
```

### Comparing `samosa-0.1.4/samosa/git.py` & `samosa-0.2.5/src/samosa/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,14 @@
             errors.append(
                 f"Pre-commit hook is missing and cannot be added. Please create .git/hooks/pre-commit"
             )
 
     # PRE-COMMIT HOOK IS EXECUTABLE
 
     if os.path.isfile(pre_commit_path):
-
         # set owner execution
         mode = os.stat(pre_commit_path).st_mode
         os.chmod(pre_commit_path, mode | stat.S_IXUSR | stat.S_IXGRP | stat.S_IXOTH)
 
         # confirm owner execution
         if os.stat(pre_commit_path).st_mode & stat.S_IXUSR:
             pre_commit_status = "Set"
```

### Comparing `samosa-0.1.4/samosa/resource/WORKFLOW.md` & `samosa-0.2.5/src/samosa/resource/WORKFLOW.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,58 +5,58 @@
 # SPDX-License-Identifier: AGPL-3.0-or-later
 -->
 
 # How to set up a triangular Git workflow from scratch
 
 1. On the host (e.g. GitHub), fork the upstream repository under your namespace
 
-2. Clone your fork to a local repository
+1. Clone your fork to a local repository
 
-   ```
-   git clone <url-of-your-fork>
-   cd <project>
-   ```
+    ```
+    git clone <url-of-your-fork>
+    cd <project>
+    ```
 
-3. Add the upstream as a remote
+1. Add the upstream as a remote
 
-   ```
-   git remote add upstream <url-of-upstream>
-   git fetch upstream
-   ```
+    ```
+    git remote add upstream <url-of-upstream>
+    git fetch upstream
+    ```
 
-4. If they aren't already defined globally, set `user.name` and `user.email`
+1. If they aren't already defined globally, set `user.name` and `user.email`
 
-   ```
-   git config --local user.name "<your name>"
-   git config --local user.mail "<name@address.domain>"
-   ```
+    ```
+    git config --local user.name "<your name>"
+    git config --local user.mail "<name@address.domain>"
+    ```
 
-5. Configure the default push target to `origin` (your forked copy) using the
-   *current* branch name:
+1. Configure the default push target to `origin` (your forked copy) using the
+    *current* branch name:
 
-   ```
-   git config remote.pushdefault origin
-   git config push.default current
-   ```
+    ```
+    git config remote.pushdefault origin
+    git config push.default current
+    ```
 
-6. Prevent accidental commits directly on the `main` branch using a pre-commit
-   hook:
+1. Prevent accidental commits directly on the `main` branch using a pre-commit
+    hook:
 
-   ```
-   $ cat .git/hooks/pre-commit
-   #!/usr/bin/env bash
+    ```
+    $ cat .git/hooks/pre-commit
+    #!/usr/bin/env bash
 
-   current_branch=$(git symbolic-ref -q HEAD | sed -e 's|^refs/heads/||')
+    current_branch=$(git symbolic-ref -q HEAD | sed -e 's|^refs/heads/||')
 
-   if [[ $current_branch = 'main' ]]; then
-           echo 'Direct commits to the main branch are not allowed.'
-           exit 1
-   fi
-   ```
+    if [[ $current_branch = 'main' ]]; then
+        echo 'Direct commits to the main branch are not allowed.'
+        exit 1
+    fi
+    ```
 
-7. Set your local `main` branch to track `upstream/main`:
+1. Set your local `main` branch to track `upstream/main`:
 
-   ```
-   git branch main --set-upstream-to=upstream/main
-   ```
+    ```
+    git branch main --set-upstream-to=upstream/main
+    ```
 
 Your repository is now samosa standard!
```

### Comparing `samosa-0.1.4/PKG-INFO` & `samosa-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: samosa
-Version: 0.1.4
+Version: 0.2.5
 Summary: Enforce a triangular Git workflow. If this is not possible, explain why.
 License: AGPL-3.0-or-later
-Author-email: David Seaward <david@librem.one>
+Project-URL: Source, https://gitlab.com/lfdo/toolchain/samosa
+Project-URL: Project, https://lofidevops.neocities.org
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Samosa (समोसा)
 
 Enforce a triangular Git workflow. If this is not possible, explain why.
 
 ## Usage
 
 ```bash
-cd <repository-folder>
+cd [repository-folder]
 samosa
 ```
 
 If any checks fail, Samosa will attempt to make a correction. If the correction
 cannot be made automatically, Samosa will make a suggestion and terminate with
 exit code 1 (error).
 
@@ -41,15 +42,15 @@
 See WORKFLOW.md for a detailed workflow that results in a samosa standard
 repository.
 
 ## Roadmap (don't hold your breath)
 
 - `samosa clone`: interactive prompts that follow the suggested workflow
 - `samosa checkout`: in samosa repository, checkout a new branch, hooked up
-  correctly
+    correctly
 - `samosa refresh`: fetch all, and pull main
 - `samosa log`: show log since `upstream/main`
 - `samosa diff`: show diff from `upstream/main`
 
 ## Suggestions
 
 ### Sole maintainer: origin = upstream
@@ -58,14 +59,15 @@
 upstream repositories. In this case, set both to the same value. When
 contribution activity justifies a project repository outside your personal
 namespace, create it and update your "upstream" value.
 
 ## Out of scope
 
 - Detecting/supporting other workflows.
+- [Oh shit, git!](https://wizardzines.com/zines/oh-shit-git/)
 
 ## Acknowledgements
 
 WORKFLOW.md and the associated pre-commit bash script are derived from Aaron
 Bull Schaefer's excellent
 [Git Triangular Workflow](https://gist.github.com/elasticdog/164fe1bb75ad645abd30d545382a1542).
 License details are included in the relevant files.
@@ -74,55 +76,60 @@
 
 - [Git 2.5, including multiple worktrees and triangular workflows](https://github.blog/2015-07-29-git-2-5-including-multiple-worktrees-and-triangular-workflows/)
 - [Triangle workflows](https://gist.github.com/anjohnson/8994c95ab2a06f7d2339)
 - [Forking workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow)
 - [Integration-manager workflow](https://git-scm.com/book/tl/v2/Distributed-Git-Distributed-Workflows#_integration_manager)
 - [Git forking workflow, what names for the remotes?](https://stackoverflow.com/q/38965156/236081)
 
+<!-- start @generated footer -->
+
 # Development environment
 
 ## Install prerequisites
 
 - Python 3.10
 - pdm
+- make
 
 ## Instructions
 
 - Fork the upstream repository.
-- `git clone <fork-url>`
+- `git clone [fork-url]`
+- `cd [project-folder]`
 - Run `make develop` to initialise your development environment.
 
 You can use any text editor or IDE that supports virtualenv / pdm. See the
 Makefile for toolchain details.
 
 Please `make test` and `make lint` before submitting changes.
 
 ## Make targets
 
 ```
-USAGE: make <target>
+USAGE: make [target]
 
 help    : Show this message.
 develop : Set up Python development environment.
 run     : Run from source.
 clean   : Remove all build artefacts.
 test    : Run tests and generate coverage report.
 lint    : Fix or warn about linting errors.
 build   : Clean, test, lint, then generate new build artefacts.
 publish : Upload build artefacts to PyPI.
 ```
 
 # Sharing and contributions
 
-Samosa (समोसा) \
-<https://gitlab.com/lofidevops/samosa> \
-Copyright 2022 David Seaward and contributors \
+```
+Samosa (समोसा)
+https://lofidevops.neocities.org
+Copyright 2022 David Seaward and contributors
 SPDX-License-Identifier: AGPL-3.0-or-later
+```
 
 Shared under AGPL-3.0-or-later. We adhere to the Contributor Covenant 2.1, and
 certify origin per DCO 1.1 with a signed-off-by line. Contributions under the
 same terms are welcome.
 
 Submit security and conduct issues as private tickets. Sign commits with
 `git commit --signoff`. For a software bill of materials run `reuse spdx`. For
-more details see LICENSES, CONDUCT and DCO.
-
+more details see CONDUCT, COPYING and CONTRIBUTING.
```

