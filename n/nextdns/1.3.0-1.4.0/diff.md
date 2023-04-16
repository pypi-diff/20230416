# Comparing `tmp/nextdns-1.3.0.tar.gz` & `tmp/nextdns-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextdns-1.3.0.tar", last modified: Tue Feb 21 16:27:48 2023, max compression
+gzip compressed data, was "nextdns-1.4.0.tar", last modified: Sun Apr 16 08:37:31 2023, max compression
```

## Comparing `nextdns-1.3.0.tar` & `nextdns-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:27:48.662654 nextdns-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-02-21 16:27:36.000000 nextdns-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-21 16:27:36.000000 nextdns-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-02-21 16:27:48.662654 nextdns-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-02-21 16:27:36.000000 nextdns-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:27:48.662654 nextdns-1.3.0/nextdns/
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-02-21 16:27:36.000000 nextdns-1.3.0/nextdns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-02-21 16:27:36.000000 nextdns-1.3.0/nextdns/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-02-21 16:27:36.000000 nextdns-1.3.0/nextdns/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-02-21 16:27:36.000000 nextdns-1.3.0/nextdns/model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 16:27:36.000000 nextdns-1.3.0/nextdns/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:27:48.662654 nextdns-1.3.0/nextdns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-02-21 16:27:48.000000 nextdns-1.3.0/nextdns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-21 16:27:48.000000 nextdns-1.3.0/nextdns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 16:27:48.000000 nextdns-1.3.0/nextdns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-21 16:27:48.000000 nextdns-1.3.0/nextdns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-21 16:27:48.000000 nextdns-1.3.0/nextdns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-02-21 16:27:36.000000 nextdns-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-21 16:27:36.000000 nextdns-1.3.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-21 16:27:36.000000 nextdns-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 16:27:48.662654 nextdns-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-02-21 16:27:36.000000 nextdns-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:37:31.627553 nextdns-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-16 08:37:14.000000 nextdns-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-16 08:37:14.000000 nextdns-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-16 08:37:31.627553 nextdns-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-16 08:37:14.000000 nextdns-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:37:31.627553 nextdns-1.4.0/nextdns/
+-rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-04-16 08:37:14.000000 nextdns-1.4.0/nextdns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15228 2023-04-16 08:37:14.000000 nextdns-1.4.0/nextdns/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-16 08:37:14.000000 nextdns-1.4.0/nextdns/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-04-16 08:37:14.000000 nextdns-1.4.0/nextdns/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 08:37:14.000000 nextdns-1.4.0/nextdns/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:37:31.627553 nextdns-1.4.0/nextdns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-16 08:37:31.000000 nextdns-1.4.0/nextdns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-16 08:37:31.000000 nextdns-1.4.0/nextdns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 08:37:31.000000 nextdns-1.4.0/nextdns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 08:37:31.000000 nextdns-1.4.0/nextdns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 08:37:31.000000 nextdns-1.4.0/nextdns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-16 08:37:14.000000 nextdns-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-16 08:37:14.000000 nextdns-1.4.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 08:37:14.000000 nextdns-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 08:37:31.627553 nextdns-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-16 08:37:14.000000 nextdns-1.4.0/setup.py
```

### Comparing `nextdns-1.3.0/LICENSE` & `nextdns-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nextdns-1.3.0/PKG-INFO` & `nextdns-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextdns
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python wrapper for NextDNS API.
 Home-page: https://github.com/bieniu/nextdns
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `nextdns-1.3.0/README.md` & `nextdns-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nextdns-1.3.0/nextdns/__init__.py` & `nextdns-1.4.0/nextdns/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,27 +149,32 @@
             block_bypass_methods=profile_data.parental_control[ApiNames.BLOCK_BYPASS],
             safesearch=profile_data.parental_control[ApiNames.SAFESEARCH],
             youtube_restricted_mode=profile_data.parental_control[
                 ApiNames.YOUTUBE_RESTRICTED_MODE
             ],
             block_9gag=services.get(ParentalControlServices.NINEGAG, False),
             block_amazon=services.get(ParentalControlServices.AMAZON, False),
+            block_bereal=services.get(ParentalControlServices.BEREAL, False),
             block_blizzard=services.get(ParentalControlServices.BLIZZARD, False),
+            block_chatgpt=services.get(ParentalControlServices.CHATGPT, False),
             block_dailymotion=services.get(ParentalControlServices.DAILYMOTION, False),
             block_discord=services.get(ParentalControlServices.DISCORD, False),
             block_disneyplus=services.get(ParentalControlServices.DISNEYPLUS, False),
             block_ebay=services.get(ParentalControlServices.EBAY, False),
             block_facebook=services.get(ParentalControlServices.FACEBOOK, False),
             block_fortnite=services.get(ParentalControlServices.FORTNITE, False),
+            block_google_chat=services.get(ParentalControlServices.GOOGLE_CHAT, False),
+            block_hbomax=services.get(ParentalControlServices.HBOMAX, False),
             block_hulu=services.get(ParentalControlServices.HULU, False),
             block_imgur=services.get(ParentalControlServices.IMGUR, False),
             block_instagram=services.get(ParentalControlServices.INSTAGRAM, False),
             block_leagueoflegends=services.get(
                 ParentalControlServices.LEAGUEOFLEGENDS, False
             ),
+            block_mastodon=services.get(ParentalControlServices.MASTODON, False),
             block_messenger=services.get(ParentalControlServices.MESSENGER, False),
             block_minecraft=services.get(ParentalControlServices.MINECRAFT, False),
             block_netflix=services.get(ParentalControlServices.NETFLIX, False),
             block_pinterest=services.get(ParentalControlServices.PINTEREST, False),
             block_primevideo=services.get(ParentalControlServices.PRIMEVIDEO, False),
             block_reddit=services.get(ParentalControlServices.REDDIT, False),
             block_roblox=services.get(ParentalControlServices.ROBLOX, False),
@@ -189,18 +194,27 @@
             block_whatsapp=services.get(ParentalControlServices.WHATSAPP, False),
             block_xboxlive=services.get(ParentalControlServices.XBOXLIVE, False),
             block_youtube=services.get(ParentalControlServices.YOUTUBE, False),
             block_zoom=services.get(ParentalControlServices.ZOOM, False),
             block_dating=categories.get(ParentalControlCategories.DATING, False),
             block_gambling=categories.get(ParentalControlCategories.GAMBLING, False),
             block_piracy=categories.get(ParentalControlCategories.PIRACY, False),
+            block_playstation_network=services.get(
+                ParentalControlServices.PLAYSTATION_NETWORK, False
+            ),
             block_porn=categories.get(ParentalControlCategories.PORN, False),
             block_social_networks=categories.get(
                 ParentalControlCategories.SOCIAL_NETWORKS, False
             ),
+            block_online_gaming=categories.get(
+                ParentalControlCategories.ONLINE_GAMING, False
+            ),
+            block_video_streaming=categories.get(
+                ParentalControlCategories.VIDEO_STREAMING, False
+            ),
         )
 
     async def get_analytics_status(self, profile_id: str) -> AnalyticsStatus:
         """Get profile analytics status."""
         url = ENDPOINTS[ATTR_ANALYTICS].format(profile_id=profile_id, type="status")
         resp = await self._http_request("get", url)
```

### Comparing `nextdns-1.3.0/nextdns/const.py` & `nextdns-1.4.0/nextdns/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,33 @@
     ),
     ParentalControlServicesAttrs.BLOCK_XBOXLIVE: SettingDescription(
         ENDPOINTS[ATTR_PARENTAL_CONTROL_SERVICE], ParentalControlServices.XBOXLIVE
     ),
     ParentalControlServicesAttrs.BLOCK_SIGNAL: SettingDescription(
         ENDPOINTS[ATTR_PARENTAL_CONTROL_SERVICE], ParentalControlServices.SIGNAL
     ),
+    ParentalControlServicesAttrs.BLOCK_BEREAL: SettingDescription(
+        ENDPOINTS[ATTR_PARENTAL_CONTROL_SERVICE], ParentalControlServices.BEREAL
+    ),
+    ParentalControlServicesAttrs.BLOCK_GOOGLE_CHAT: SettingDescription(
+        ENDPOINTS[ATTR_PARENTAL_CONTROL_SERVICE], ParentalControlServices.GOOGLE_CHAT
+    ),
+    ParentalControlServicesAttrs.BLOCK_CHATGPT: SettingDescription(
+        ENDPOINTS[ATTR_PARENTAL_CONTROL_SERVICE], ParentalControlServices.CHATGPT
+    ),
+    ParentalControlServicesAttrs.BLOCK_HBOMAX: SettingDescription(
+        ENDPOINTS[ATTR_PARENTAL_CONTROL_SERVICE], ParentalControlServices.HBOMAX
+    ),
+    ParentalControlServicesAttrs.BLOCK_MASTODON: SettingDescription(
+        ENDPOINTS[ATTR_PARENTAL_CONTROL_SERVICE], ParentalControlServices.MASTODON
+    ),
+    ParentalControlServicesAttrs.BLOCK_PLAYSTATION_NETWORK: SettingDescription(
+        ENDPOINTS[ATTR_PARENTAL_CONTROL_SERVICE],
+        ParentalControlServices.PLAYSTATION_NETWORK,
+    ),
     ParentalControlCategoriesAttrs.BLOCK_DATING: SettingDescription(
         ENDPOINTS[ATTR_PARENTAL_CONTROL_CATEGORY], ParentalControlCategories.DATING
     ),
     ParentalControlCategoriesAttrs.BLOCK_GAMBLING: SettingDescription(
         ENDPOINTS[ATTR_PARENTAL_CONTROL_CATEGORY], ParentalControlCategories.GAMBLING
     ),
     ParentalControlCategoriesAttrs.BLOCK_PIRACY: SettingDescription(
@@ -284,11 +303,19 @@
     ParentalControlCategoriesAttrs.BLOCK_PORN: SettingDescription(
         ENDPOINTS[ATTR_PARENTAL_CONTROL_CATEGORY], ParentalControlCategories.PORN
     ),
     ParentalControlCategoriesAttrs.BLOCK_SOCIAL_NETWORKS: SettingDescription(
         ENDPOINTS[ATTR_PARENTAL_CONTROL_CATEGORY],
         ParentalControlCategories.SOCIAL_NETWORKS,
     ),
+    ParentalControlCategoriesAttrs.BLOCK_VIDEO_STREAMING: SettingDescription(
+        ENDPOINTS[ATTR_PARENTAL_CONTROL_CATEGORY],
+        ParentalControlCategories.VIDEO_STREAMING,
+    ),
+    ParentalControlCategoriesAttrs.BLOCK_ONLINE_GAMING: SettingDescription(
+        ENDPOINTS[ATTR_PARENTAL_CONTROL_CATEGORY],
+        ParentalControlCategories.ONLINE_GAMING,
+    ),
 }
 
 ALLOWED_LOGS_LOCATION = ("ch", "eu", "gb", "us")
 ALLOWED_LOGS_RETENTION = (1, 6, 24, 168, 720, 2160, 4320, 8760, 17520)
```

### Comparing `nextdns-1.3.0/nextdns/exceptions.py` & `nextdns-1.4.0/nextdns/exceptions.py`

 * *Files identical despite different names*

### Comparing `nextdns-1.3.0/nextdns/model.py` & `nextdns-1.4.0/nextdns/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -229,29 +229,35 @@
 
     block_bypass_methods: bool
     safesearch: bool
     youtube_restricted_mode: bool
 
     block_9gag: bool
     block_amazon: bool
+    block_bereal: bool
     block_blizzard: bool
+    block_chatgpt: bool
     block_dailymotion: bool
     block_discord: bool
     block_disneyplus: bool
     block_ebay: bool
     block_facebook: bool
     block_fortnite: bool
+    block_google_chat: bool
+    block_hbomax: bool
     block_hulu: bool
     block_imgur: bool
     block_instagram: bool
     block_leagueoflegends: bool
+    block_mastodon: bool
     block_messenger: bool
     block_minecraft: bool
     block_netflix: bool
     block_pinterest: bool
+    block_playstation_network: bool
     block_primevideo: bool
     block_reddit: bool
     block_roblox: bool
     block_signal: bool
     block_skype: bool
     block_snapchat: bool
     block_spotify: bool
@@ -270,14 +276,16 @@
     block_zoom: bool
 
     block_dating: bool
     block_gambling: bool
     block_piracy: bool
     block_porn: bool
     block_social_networks: bool
+    block_online_gaming: bool
+    block_video_streaming: bool
 
 
 @dataclass
 class ProfileInfo(NextDnsData):
     """ProfileInfo class."""
 
     id: str  # noqa: A003
@@ -293,30 +301,36 @@
     profile_id: str | None = None
 
 
 class ParentalControlServices(StrEnum):
     """Service type for parental control."""
 
     AMAZON = "amazon"
+    BEREAL = "bereal"
     BLIZZARD = "blizzard"
+    CHATGPT = "chatgpt"
     DAILYMOTION = "dailymotion"
     DISCORD = "discord"
     DISNEYPLUS = "disneyplus"
     EBAY = "ebay"
     FACEBOOK = "facebook"
     FORTNITE = "fortnite"
+    GOOGLE_CHAT = "google-chat"
+    HBOMAX = "hbomax"
     HULU = "hulu"
     IMGUR = "imgur"
     INSTAGRAM = "instagram"
     LEAGUEOFLEGENDS = "leagueoflegends"
+    MASTODON = "mastodon"
     MESSENGER = "messenger"
     MINECRAFT = "minecraft"
     NETFLIX = "netflix"
     NINEGAG = "9gag"
     PINTEREST = "pinterest"
+    PLAYSTATION_NETWORK = "playstation-network"
     PRIMEVIDEO = "primevideo"
     REDDIT = "reddit"
     ROBLOX = "roblox"
     SIGNAL = "signal"
     SKYPE = "skype"
     SNAPCHAT = "snapchat"
     SPOTIFY = "spotify"
@@ -336,29 +350,35 @@
 
 
 class ParentalControlServicesAttrs(StrEnum):
     """Service type attributes for parental control."""
 
     BLOCK_9GAG = "block_9gag"
     BLOCK_AMAZON = "block_amazon"
+    BLOCK_BEREAL = "block_bereal"
     BLOCK_BLIZZARD = "block_blizzard"
+    BLOCK_CHATGPT = "block_chatgpt"
     BLOCK_DAILYMOTION = "block_dailymotion"
     BLOCK_DISCORD = "block_discord"
     BLOCK_DISNEYPLUS = "block_disneyplus"
     BLOCK_EBAY = "block_ebay"
     BLOCK_FACEBOOK = "block_facebook"
     BLOCK_FORTNITE = "block_fortnite"
+    BLOCK_GOOGLE_CHAT = "block_google_chat"
+    BLOCK_HBOMAX = "block_hbomax"
     BLOCK_HULU = "block_hulu"
     BLOCK_IMGUR = "block_imgur"
     BLOCK_INSTAGRAM = "block_instagram"
     BLOCK_LEAGUEOFLEGENDS = "block_leagueoflegends"
+    BLOCK_MASTODON = "block_mastodon"
     BLOCK_MESSENGER = "block_messenger"
     BLOCK_MINECRAFT = "block_minecraft"
     BLOCK_NETFLIX = "block_netflix"
     BLOCK_PINTEREST = "block_pinterest"
+    BLOCK_PLAYSTATION_NETWORK = "block_playstation_network"
     BLOCK_PRIMEVIDEO = "block_primevideo"
     BLOCK_REDDIT = "block_reddit"
     BLOCK_ROBLOX = "block_roblox"
     BLOCK_SIGNAL = "block_signal"
     BLOCK_SKYPE = "block_skype"
     BLOCK_SNAPCHAT = "block_snapchat"
     BLOCK_SPOTIFY = "block_spotify"
@@ -378,27 +398,31 @@
 
 
 class ParentalControlCategories(StrEnum):
     """Categories type for parental control."""
 
     DATING = "dating"
     GAMBLING = "gambling"
+    ONLINE_GAMING = "gaming"
     PIRACY = "piracy"
     PORN = "porn"
     SOCIAL_NETWORKS = "social-networks"
+    VIDEO_STREAMING = "video-streaming"
 
 
 class ParentalControlCategoriesAttrs(StrEnum):
     """Categories type attributes for parental control."""
 
-    BLOCK_DATING = "block_dating"
-    BLOCK_GAMBLING = "block_gambling"
-    BLOCK_PIRACY = "block_piracy"
-    BLOCK_PORN = "block_porn"
+    BLOCK_VIDEO_STREAMING = "block_video_streaming"
     BLOCK_SOCIAL_NETWORKS = "block_social_networks"
+    BLOCK_PORN = "block_porn"
+    BLOCK_PIRACY = "block_piracy"
+    BLOCK_ONLINE_GAMING = "block_online_gaming"
+    BLOCK_GAMBLING = "block_gambling"
+    BLOCK_DATING = "block_dating"
 
 
 class ApiNames(StrEnum):
     """Names type for API."""
 
     AI_THREAT_TETECTION = "aiThreatDetection"
     ALLOW_AFFILIATE = "allowAffiliate"
```

### Comparing `nextdns-1.3.0/nextdns.egg-info/PKG-INFO` & `nextdns-1.4.0/nextdns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextdns
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python wrapper for NextDNS API.
 Home-page: https://github.com/bieniu/nextdns
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `nextdns-1.3.0/pyproject.toml` & `nextdns-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -106,8 +106,8 @@
 [tool.ruff.pyupgrade]
 keep-runtime-typing = true
 
 [tool.ruff.mccabe]
 max-complexity = 25
 
 [tool.coverage.run]
-source = ["gios"]
+source = ["nextdns"]
```

### Comparing `nextdns-1.3.0/setup.py` & `nextdns-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup module for nextdns."""
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "1.3.0"
+VERSION = "1.4.0"
 
 with open("requirements.txt", encoding="utf-8") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="nextdns",
     version=VERSION,
```

