# Comparing `tmp/badgie-0.3.0.tar.gz` & `tmp/badgie-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badgie-0.3.0.tar", last modified: Fri Apr 14 23:35:30 2023, max compression
+gzip compressed data, was "badgie-0.4.0.tar", last modified: Sun Apr 16 06:56:54 2023, max compression
```

## Comparing `badgie-0.3.0.tar` & `badgie-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 23:35:30.916654 badgie-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-14 23:35:27.000000 badgie-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3700 2023-04-14 23:35:30.916654 badgie-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2808 2023-04-14 23:35:27.000000 badgie-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 23:35:30.912654 badgie-0.3.0/badgie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-14 23:35:28.000000 badgie-0.3.0/badgie/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 23:35:30.915654 badgie-0.3.0/badgie/badges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/badges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/badges/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/badges/brettops.py
--rw-rw-rw-   0 root         (0) root         (0)     1257 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/badges/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      511 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/badges/precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     4458 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1524 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 23:35:30.915654 badgie-0.3.0/badgie/providers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/providers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/providers/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/sources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 23:35:30.913653 badgie-0.3.0/badgie.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3700 2023-04-14 23:35:30.000000 badgie-0.3.0/badgie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      559 2023-04-14 23:35:30.000000 badgie-0.3.0/badgie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 23:35:30.000000 badgie-0.3.0/badgie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-14 23:35:30.000000 badgie-0.3.0/badgie.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-14 23:35:30.000000 badgie-0.3.0/badgie.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-14 23:35:30.000000 badgie-0.3.0/badgie.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-14 23:35:30.916654 badgie-0.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-04-14 23:35:28.000000 badgie-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.968898 badgie-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-16 06:56:51.000000 badgie-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3936 2023-04-16 06:56:54.968898 badgie-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2023-04-16 06:56:51.000000 badgie-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.962897 badgie-0.4.0/badgie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-16 06:56:52.000000 badgie-0.4.0/badgie/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.966898 badgie-0.4.0/badgie/badges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/badges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/badges/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/badges/brettops.py
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/badges/codestyle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/badges/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/badges/precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     5154 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.966898 badgie-0.4.0/badgie/detectors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/detectors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/detectors/precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.967898 badgie-0.4.0/badgie/providers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/providers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/providers/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.967898 badgie-0.4.0/badgie/sources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/sources/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.964897 badgie-0.4.0/badgie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3936 2023-04-16 06:56:54.000000 badgie-0.4.0/badgie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      677 2023-04-16 06:56:54.000000 badgie-0.4.0/badgie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 06:56:54.000000 badgie-0.4.0/badgie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-16 06:56:54.000000 badgie-0.4.0/badgie.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-16 06:56:54.000000 badgie-0.4.0/badgie.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-16 06:56:54.000000 badgie-0.4.0/badgie.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-16 06:56:54.969898 badgie-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-04-16 06:56:52.000000 badgie-0.4.0/setup.py
```

### Comparing `badgie-0.3.0/LICENSE` & `badgie-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `badgie-0.3.0/PKG-INFO` & `badgie-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.3.0
+Version: 0.4.0
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge template markdown
 Platform: UNKNOWN
@@ -27,14 +27,16 @@
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
 [![latest release](https://img.shields.io/gitlab/v/release/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/releases)
 [![pipeline status](https://gitlab.com/brettops/tools/badgie/badges/main/pipeline.svg)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![code style: black](https://img.shields.io/badge/code_style-black-000000.svg)](https://github.com/psf/black)
+[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 
 <!-- END BADGIE TIME -->
 
 Add all the badges with Badgie!
 
 ---
```

### Comparing `badgie-0.3.0/README.md` & `badgie-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
 [![latest release](https://img.shields.io/gitlab/v/release/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/releases)
 [![pipeline status](https://gitlab.com/brettops/tools/badgie/badges/main/pipeline.svg)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![code style: black](https://img.shields.io/badge/code_style-black-000000.svg)](https://github.com/psf/black)
+[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 
 <!-- END BADGIE TIME -->
 
 Add all the badges with Badgie!
 
 ---
```

### Comparing `badgie-0.3.0/badgie/badges/_base.py` & `badgie-0.4.0/badgie/badges/_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import sys
 from dataclasses import dataclass
 from typing import Optional
 
 from termcolor import colored
 
-from ..models import Project, Remote
+from ..models import Hook, Project, Remote
 
 
 @dataclass(frozen=True)
 class Badge:
     project: Project
     remote: Optional[Remote] = None
+    hook: Optional[Hook] = None
 
     def __post_init__(self):
         print(
             colored(
                 "- adding a {name} badge".format(
                     name=colored(self.__class__.name, "blue", attrs=["bold"])
                 )
```

### Comparing `badgie-0.3.0/badgie/badges/brettops.py` & `badgie-0.4.0/badgie/badges/brettops.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 @register_badge
 class BrettOpsBadge(Badge):
     """
     Show that the repository is a BrettOps repository.
     """
 
     name = "brettops"
+    example = "https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50"
 
     remotes = (
         Remote(prefix="https://gitlab.com/brettops/containers/", name="container"),
         Remote(prefix="https://gitlab.com/brettops/packages/", name="package"),
         Remote(prefix="https://gitlab.com/brettops/pipelines/", name="pipeline"),
         Remote(prefix="https://gitlab.com/brettops/tools/", name="tool"),
         Remote(prefix="https://gitlab.com/brettops/ansible/roles/", name="role"),
```

### Comparing `badgie-0.3.0/badgie/badges/gitlab.py` & `badgie-0.4.0/badgie/badges/gitlab.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 @register_badge
 class GitLabLatestReleaseBadge(Badge):
     """
     Show the latest GitLab release by date.
     """
 
     name = "gitlab-latest-release"
+    example = "https://img.shields.io/gitlab/v/release/brettops/tools/badgie"
+
     link_title = "latest release"
 
     def get_badge_image_url(self):
         return f"https://img.shields.io/gitlab/v/release/{self.project.full_path}"
 
     def get_link_url(self):
         return f"{self.project.url}/-/releases"
@@ -23,15 +25,16 @@
     Show the most recent coverage score on the default branch.
     """
 
     name = "gitlab-coverage-report"
     link_title = "coverage report"
 
     def get_badge_image_url(self):
-        return f"{self.project.url}/badges/{self.project.ref}/coverage.svg"
+        # return f"{self.project.url}/badges/{self.project.ref}/coverage.svg"
+        return f"https://img.shields.io/gitlab/pipeline-status/{self.project.full_path}"
 
     def get_link_url(self):
         return f"{self.project.url}/-/commits/{self.project.ref}"
 
 
 @register_badge
 class GitLabPipelineStatusBadge(Badge):
```

### Comparing `badgie-0.3.0/badgie/cli.py` & `badgie-0.4.0/badgie/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 import sys
 
 from termcolor import colored
 
 from ._version import __version__
 from .badges._base import _BADGES
 from .badges.brettops import BrettOpsBadge
+from .badges.codestyle import CodeStyleBlackBadge, CodeStylePrettierBadge
 from .badges.gitlab import (
     GitLabCoverageReportBadge,
     GitLabLatestReleaseBadge,
     GitLabPipelineStatusBadge,
 )
 from .badges.precommit import PreCommitBadge
 from .constants import PATTERN_GIT_SSH
+from .detectors.precommit import PreCommitConfigDetector
 from .parser import parse_text
 from .providers import gitlab as gitlab_provider
-from .sources import get_badge_from_files, get_badge_from_remotes
+from .sources.base import get_badge_from_remotes
 
 RE_GIT_SSH = re.compile(PATTERN_GIT_SSH)
 
 logging.basicConfig(level=logging.WARNING)
 
 
 def get_badge_text(badges, format="markdown"):
@@ -60,14 +62,20 @@
 def find_badges(text):
     badges = []
     process = subprocess.run(["git", "remote", "-v"], text=True, capture_output=True)
     url = process.stdout.splitlines()[0].split("\t")[1].split(" ")[0]
     match = RE_GIT_SSH.match(url)
     if match:
         if match.group("host") == "gitlab.com":
+            print(
+                colored("- This looks like a", "white", attrs=["bold"]),
+                colored("GitLab", "blue", attrs=["bold"]),
+                colored("project", "white", attrs=["bold"]),
+                file=sys.stderr,
+            )
             glproject, project = gitlab_provider.get_project(match.group("path"))
 
             # add brettops badge
             new_badge = get_badge_from_remotes(
                 badge_class=BrettOpsBadge, project=project
             )
             if new_badge is not None:
@@ -91,20 +99,27 @@
                 if glpipeline.coverage is not None:
                     badges.append(
                         GitLabCoverageReportBadge(
                             project=project,
                         )
                     )
 
-            # add pre-commit badge
-            new_badge = get_badge_from_files(
-                badge_class=PreCommitBadge, project=project
-            )
-            if new_badge is not None:
-                badges.append(new_badge)
+            try:
+                detector = PreCommitConfigDetector(project=project)
+            except FileNotFoundError:
+                detector = None
+            if detector:
+                badges.append(PreCommitBadge(project=project))
+                new_badge = detector.get_badge(badge_class=CodeStyleBlackBadge)
+                if new_badge:
+                    badges.append(new_badge)
+                new_badge = detector.get_badge(badge_class=CodeStylePrettierBadge)
+                if new_badge:
+                    badges.append(new_badge)
+
     return badges
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-l", "--list", action=ListAction, help="list available badges")
     parser.add_argument(
```

### Comparing `badgie-0.3.0/badgie/parser.py` & `badgie-0.4.0/badgie/parser.py`

 * *Files identical despite different names*

### Comparing `badgie-0.3.0/badgie/providers/gitlab.py` & `badgie-0.4.0/badgie/providers/gitlab.py`

 * *Files identical despite different names*

### Comparing `badgie-0.3.0/badgie/sources.py` & `badgie-0.4.0/badgie/sources/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Type
 
-from .badges._base import Badge
-from .models import Project
+from ..badges._base import Badge
+from ..models import Project
 
 
 def get_badge_from_files(badge_class: Type[Badge], project: Project):
     try:
         files = getattr(badge_class, "files")
     except AttributeError:
         files = ()
```

### Comparing `badgie-0.3.0/badgie.egg-info/PKG-INFO` & `badgie-0.4.0/badgie.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.3.0
+Version: 0.4.0
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge template markdown
 Platform: UNKNOWN
@@ -27,14 +27,16 @@
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
 [![latest release](https://img.shields.io/gitlab/v/release/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/releases)
 [![pipeline status](https://gitlab.com/brettops/tools/badgie/badges/main/pipeline.svg)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![code style: black](https://img.shields.io/badge/code_style-black-000000.svg)](https://github.com/psf/black)
+[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 
 <!-- END BADGIE TIME -->
 
 Add all the badges with Badgie!
 
 ---
```

### Comparing `badgie-0.3.0/badgie.egg-info/SOURCES.txt` & `badgie-0.4.0/badgie.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -6,21 +6,25 @@
 badgie/__main__.py
 badgie/_version.py
 badgie/cli.py
 badgie/constants.py
 badgie/models.py
 badgie/parser.py
 badgie/py.typed
-badgie/sources.py
 badgie.egg-info/PKG-INFO
 badgie.egg-info/SOURCES.txt
 badgie.egg-info/dependency_links.txt
 badgie.egg-info/entry_points.txt
 badgie.egg-info/requires.txt
 badgie.egg-info/top_level.txt
 badgie/badges/__init__.py
 badgie/badges/_base.py
 badgie/badges/brettops.py
+badgie/badges/codestyle.py
 badgie/badges/gitlab.py
 badgie/badges/precommit.py
+badgie/detectors/__init__.py
+badgie/detectors/precommit.py
 badgie/providers/__init__.py
-badgie/providers/gitlab.py
+badgie/providers/gitlab.py
+badgie/sources/__init__.py
+badgie/sources/base.py
```

### Comparing `badgie-0.3.0/setup.py` & `badgie-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
```

