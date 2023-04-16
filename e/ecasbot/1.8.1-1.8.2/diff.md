# Comparing `tmp/ecasbot-1.8.1.tar.gz` & `tmp/ecasbot-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecasbot-1.8.1.tar", last modified: Fri Feb 10 14:49:13 2023, max compression
+gzip compressed data, was "ecasbot-1.8.2.tar", last modified: Sun Apr 16 13:35:20 2023, max compression
```

## Comparing `ecasbot-1.8.1.tar` & `ecasbot-1.8.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-02-10 14:49:13.224616 ecasbot-1.8.1/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      134 2023-01-14 12:46:51.000000 ecasbot-1.8.1/.bandit.yml
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)    35141 2018-08-07 15:49:55.000000 ecasbot-1.8.1/LICENSE
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      178 2023-01-14 12:46:51.000000 ecasbot-1.8.1/MANIFEST.in
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     3068 2023-02-10 14:49:13.224616 ecasbot-1.8.1/PKG-INFO
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2303 2022-12-25 10:28:05.000000 ecasbot-1.8.1/README.md
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-02-10 14:49:13.219616 ecasbot-1.8.1/licenses/
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)    11357 2022-05-07 14:34:35.000000 ecasbot-1.8.1/licenses/noto-emoji.LICENSE.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1240 2023-02-10 14:49:03.000000 ecasbot-1.8.1/pyproject.toml
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)       38 2023-02-10 14:49:13.224616 ecasbot-1.8.1/setup.cfg
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-02-10 14:49:13.217616 ecasbot-1.8.1/src/
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-02-10 14:49:13.221616 ecasbot-1.8.1/src/ecasbot/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)    40685 2023-02-10 14:49:03.000000 ecasbot-1.8.1/src/ecasbot/__init__.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2156 2023-01-14 12:46:51.000000 ecasbot-1.8.1/src/ecasbot/chkmsg.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2974 2023-01-14 12:46:51.000000 ecasbot-1.8.1/src/ecasbot/chkusr.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      535 2023-02-08 14:20:08.000000 ecasbot-1.8.1/src/ecasbot/exceptions.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      894 2023-01-14 12:46:51.000000 ecasbot-1.8.1/src/ecasbot/extractor.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-02-10 14:49:13.222616 ecasbot-1.8.1/src/ecasbot/messages/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      648 2023-01-14 12:46:51.000000 ecasbot-1.8.1/src/ecasbot/messages/__init__.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1023 2023-01-14 12:46:51.000000 ecasbot-1.8.1/src/ecasbot/messages/factory.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-02-10 14:49:13.223616 ecasbot-1.8.1/src/ecasbot/messages/locales/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      362 2023-01-14 12:46:51.000000 ecasbot-1.8.1/src/ecasbot/messages/locales/__init__.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     5291 2023-01-26 10:59:39.000000 ecasbot-1.8.1/src/ecasbot/messages/locales/en.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     9686 2023-01-26 10:59:39.000000 ecasbot-1.8.1/src/ecasbot/messages/locales/ru.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2555 2023-02-08 14:20:08.000000 ecasbot-1.8.1/src/ecasbot/permissions.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1194 2023-02-10 14:49:03.000000 ecasbot-1.8.1/src/ecasbot/ranges.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-02-10 14:49:13.224616 ecasbot-1.8.1/src/ecasbot/scripts/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      114 2023-01-14 12:46:51.000000 ecasbot-1.8.1/src/ecasbot/scripts/__init__.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      414 2023-01-14 12:46:51.000000 ecasbot-1.8.1/src/ecasbot/scripts/runbot.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)    12725 2023-02-08 14:20:08.000000 ecasbot-1.8.1/src/ecasbot/settings.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-02-10 14:49:13.222616 ecasbot-1.8.1/src/ecasbot.egg-info/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     3068 2023-02-10 14:49:13.000000 ecasbot-1.8.1/src/ecasbot.egg-info/PKG-INFO
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      738 2023-02-10 14:49:13.000000 ecasbot-1.8.1/src/ecasbot.egg-info/SOURCES.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)        1 2023-02-10 14:49:13.000000 ecasbot-1.8.1/src/ecasbot.egg-info/dependency_links.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)       56 2023-02-10 14:49:13.000000 ecasbot-1.8.1/src/ecasbot.egg-info/entry_points.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      104 2023-02-10 14:49:13.000000 ecasbot-1.8.1/src/ecasbot.egg-info/requires.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)        8 2023-02-10 14:49:13.000000 ecasbot-1.8.1/src/ecasbot.egg-info/top_level.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1431 2023-01-26 10:59:39.000000 ecasbot-1.8.1/tox.ini
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.049436 ecasbot-1.8.2/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      134 2023-01-14 12:46:51.000000 ecasbot-1.8.2/.bandit.yml
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)    35141 2018-08-07 15:49:55.000000 ecasbot-1.8.2/LICENSE
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      178 2023-01-14 12:46:51.000000 ecasbot-1.8.2/MANIFEST.in
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     3068 2023-04-16 13:35:20.049436 ecasbot-1.8.2/PKG-INFO
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2303 2022-12-25 10:28:05.000000 ecasbot-1.8.2/README.md
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.043436 ecasbot-1.8.2/licenses/
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)    11357 2022-05-07 14:34:35.000000 ecasbot-1.8.2/licenses/noto-emoji.LICENSE.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1240 2023-04-16 13:35:09.000000 ecasbot-1.8.2/pyproject.toml
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)       38 2023-04-16 13:35:20.049436 ecasbot-1.8.2/setup.cfg
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.041436 ecasbot-1.8.2/src/
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.046436 ecasbot-1.8.2/src/ecasbot/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)    40962 2023-04-16 13:35:09.000000 ecasbot-1.8.2/src/ecasbot/__init__.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2156 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/chkmsg.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2974 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/chkusr.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      535 2023-02-08 14:20:08.000000 ecasbot-1.8.2/src/ecasbot/exceptions.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      894 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/extractor.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.047436 ecasbot-1.8.2/src/ecasbot/messages/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      648 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/messages/__init__.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1023 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/messages/factory.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.048436 ecasbot-1.8.2/src/ecasbot/messages/locales/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      362 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/messages/locales/__init__.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     5291 2023-01-26 10:59:39.000000 ecasbot-1.8.2/src/ecasbot/messages/locales/en.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     9686 2023-01-26 10:59:39.000000 ecasbot-1.8.2/src/ecasbot/messages/locales/ru.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2391 2023-04-16 13:35:09.000000 ecasbot-1.8.2/src/ecasbot/permissions.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1194 2023-02-10 14:49:03.000000 ecasbot-1.8.2/src/ecasbot/ranges.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.049436 ecasbot-1.8.2/src/ecasbot/scripts/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      114 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/scripts/__init__.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      414 2023-01-14 12:46:51.000000 ecasbot-1.8.2/src/ecasbot/scripts/runbot.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)    12725 2023-02-08 14:20:08.000000 ecasbot-1.8.2/src/ecasbot/settings.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-16 13:35:20.047436 ecasbot-1.8.2/src/ecasbot.egg-info/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     3068 2023-04-16 13:35:20.000000 ecasbot-1.8.2/src/ecasbot.egg-info/PKG-INFO
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      738 2023-04-16 13:35:20.000000 ecasbot-1.8.2/src/ecasbot.egg-info/SOURCES.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)        1 2023-04-16 13:35:20.000000 ecasbot-1.8.2/src/ecasbot.egg-info/dependency_links.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)       56 2023-04-16 13:35:20.000000 ecasbot-1.8.2/src/ecasbot.egg-info/entry_points.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      104 2023-04-16 13:35:20.000000 ecasbot-1.8.2/src/ecasbot.egg-info/requires.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)        8 2023-04-16 13:35:20.000000 ecasbot-1.8.2/src/ecasbot.egg-info/top_level.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1431 2023-01-26 10:59:39.000000 ecasbot-1.8.2/tox.ini
```

### Comparing `ecasbot-1.8.1/LICENSE` & `ecasbot-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/PKG-INFO` & `ecasbot-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecasbot
-Version: 1.8.1
+Version: 1.8.2
 Summary: EC AntiSpam bot for the Telegram messenger
 Author-email: Vitaly Zaitsev <vitaly@easycoding.org>
 License: GPL-3.0-or-later
 Project-URL: homepage, https://github.com/xvitaly/ecasbot
 Project-URL: documentation, https://github.com/xvitaly/ecasbot/blob/master/docs/README.md
 Project-URL: repository, https://github.com/xvitaly/ecasbot
 Keywords: anti-spam,bot,database-less,telegram,telegram-api,telegram-bot
```

### Comparing `ecasbot-1.8.1/README.md` & `ecasbot-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/licenses/noto-emoji.LICENSE.txt` & `ecasbot-1.8.2/licenses/noto-emoji.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/pyproject.toml` & `ecasbot-1.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 # SPDX-FileCopyrightText: 2017-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 [project]
 name = "ecasbot"
-version = "1.8.1"
+version = "1.8.2"
 license = { text = "GPL-3.0-or-later" }
 readme = "README.md"
 dependencies = [
     "requests>=2.28.0",
-    "pytelegrambotapi>=4.10.0",
+    "pytelegrambotapi>=4.11.0",
     "emoji>=2.2.0"
 ]
 authors = [
     { name = "Vitaly Zaitsev", email="vitaly@easycoding.org" }
 ]
 description = "EC AntiSpam bot for the Telegram messenger"
 keywords = [
```

### Comparing `ecasbot-1.8.1/src/ecasbot/__init__.py` & `ecasbot-1.8.2/src/ecasbot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -571,15 +571,16 @@
             if message.reply_to_message:
                 username = self.__get_actual_username(message)
                 userid = self.__get_actual_userid(message)
                 if message.from_user.id != userid and self.__check_restriction_allowed(message):
                     mutereq = ParamExtractor(message.text)
                     mutetime = int(time.time()) + (int(float(mutereq.param) * 86400) if mutereq.index != -1 else 0)
                     self.__bot.restrict_chat_member(message.chat.id, userid, until_date=mutetime,
-                                                    permissions=self.__perm.restrict)
+                                                    permissions=self.__perm.restrict,
+                                                    use_independent_chat_permissions=True)
                     logmsg = self.__get_lm('as_amute').format(message.from_user.first_name, message.from_user.id,
                                                               username, userid, message.chat.id, message.chat.title,
                                                               mutetime if mutereq.index != -1 else 'forever')
                 else:
                     logmsg = self.__get_lm('as_resprot').format(message.from_user.first_name, message.from_user.id,
                                                                 username, userid, message.chat.id,
                                                                 message.chat.title)
@@ -595,15 +596,16 @@
         Remove all restrictions on sender of message replied by this command
         or specified in mandatory Telegram user ID.
         :param message: Message, triggered this event.
         """
         try:
             if message.reply_to_message:
                 self.__bot.restrict_chat_member(message.chat.id, message.reply_to_message.from_user.id,
-                                                permissions=self.__perm.unrestrict)
+                                                permissions=self.__perm.unrestrict,
+                                                use_independent_chat_permissions=True)
                 logmsg = self.__get_lm('as_aunres').format(message.from_user.first_name, message.from_user.id,
                                                            message.reply_to_message.from_user.first_name,
                                                            message.reply_to_message.from_user.id, message.chat.id,
                                                            message.chat.title)
                 self.__logger.warning(logmsg)
                 self.__notify_admin(message, logmsg)
                 self.__clean_command(message)
@@ -755,15 +757,16 @@
                                                                        state.until_date)
                         else:
                             # Limit users reached half-goal permanently (366 or 367 for leap years days)...
                             limtime = 31708800 if score >= self.__settings.nickgoal / 2 else self.__settings.bantime
                             # Restrict all new users for specified in config time...
                             self.__bot.restrict_chat_member(message.chat.id, new_chat_member.id,
                                                             until_date=int(time.time()) + limtime,
-                                                            permissions=self.__perm.join)
+                                                            permissions=self.__perm.join,
+                                                            use_independent_chat_permissions=True)
                             actmsg = self.__get_lm('as_rest').format(new_chat_member.first_name,
                                                                      new_chat_member.id, score,
                                                                      message.chat.id,
                                                                      message.chat.title,
                                                                      limtime / 86400)
                     # Writing to log and notifying subscribers if enabled...
                     self.__logger.warning(actmsg)
```

### Comparing `ecasbot-1.8.1/src/ecasbot/chkmsg.py` & `ecasbot-1.8.2/src/ecasbot/chkmsg.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/src/ecasbot/chkusr.py` & `ecasbot-1.8.2/src/ecasbot/chkusr.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/src/ecasbot/exceptions.py` & `ecasbot-1.8.2/src/ecasbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/src/ecasbot/extractor.py` & `ecasbot-1.8.2/src/ecasbot/extractor.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/src/ecasbot/messages/__init__.py` & `ecasbot-1.8.2/src/ecasbot/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/src/ecasbot/messages/factory.py` & `ecasbot-1.8.2/src/ecasbot/messages/factory.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/src/ecasbot/messages/locales/en.py` & `ecasbot-1.8.2/src/ecasbot/messages/locales/en.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/src/ecasbot/messages/locales/ru.py` & `ecasbot-1.8.2/src/ecasbot/messages/locales/ru.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/src/ecasbot/permissions.py` & `ecasbot-1.8.2/src/ecasbot/permissions.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,24 +29,22 @@
         """
         return self.__up
 
     def __init__(self):
         """
         Main constructor of the Permissions class.
         """
-        self.__jp = ChatPermissions(can_send_messages=True, can_send_media_messages=False, can_send_audios=False,
-                                    can_send_documents=False, can_send_photos=False, can_send_videos=False,
-                                    can_send_video_notes=False, can_send_voice_notes=False, can_send_polls=False,
-                                    can_send_other_messages=False, can_add_web_page_previews=False,
-                                    can_change_info=False, can_invite_users=False, can_pin_messages=False,
-                                    can_manage_topics=False)
-        self.__rp = ChatPermissions(can_send_messages=False, can_send_media_messages=False, can_send_audios=False,
-                                    can_send_documents=False, can_send_photos=False, can_send_videos=False,
-                                    can_send_video_notes=False, can_send_voice_notes=False, can_send_polls=False,
-                                    can_send_other_messages=False, can_add_web_page_previews=False,
-                                    can_change_info=False, can_invite_users=False, can_pin_messages=False,
-                                    can_manage_topics=False)
-        self.__up = ChatPermissions(can_send_messages=True, can_send_media_messages=True, can_send_audios=True,
-                                    can_send_documents=True, can_send_photos=True, can_send_videos=True,
-                                    can_send_video_notes=True, can_send_voice_notes=True, can_send_polls=True,
-                                    can_send_other_messages=True, can_add_web_page_previews=True, can_change_info=True,
-                                    can_invite_users=True, can_pin_messages=True, can_manage_topics=True)
+        self.__jp = ChatPermissions(can_send_messages=True, can_send_audios=False, can_send_documents=False,
+                                    can_send_photos=False, can_send_videos=False, can_send_video_notes=False,
+                                    can_send_voice_notes=False, can_send_polls=False, can_send_other_messages=False,
+                                    can_add_web_page_previews=False, can_change_info=False, can_invite_users=False,
+                                    can_pin_messages=False, can_manage_topics=False)
+        self.__rp = ChatPermissions(can_send_messages=False, can_send_audios=False, can_send_documents=False,
+                                    can_send_photos=False, can_send_videos=False, can_send_video_notes=False,
+                                    can_send_voice_notes=False, can_send_polls=False, can_send_other_messages=False,
+                                    can_add_web_page_previews=False, can_change_info=False, can_invite_users=False,
+                                    can_pin_messages=False, can_manage_topics=False)
+        self.__up = ChatPermissions(can_send_messages=True, can_send_audios=True, can_send_documents=True,
+                                    can_send_photos=True, can_send_videos=True, can_send_video_notes=True,
+                                    can_send_voice_notes=True, can_send_polls=True, can_send_other_messages=True,
+                                    can_add_web_page_previews=True, can_change_info=True, can_invite_users=True,
+                                    can_pin_messages=True, can_manage_topics=True)
```

### Comparing `ecasbot-1.8.1/src/ecasbot/ranges.py` & `ecasbot-1.8.2/src/ecasbot/ranges.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/src/ecasbot/settings.py` & `ecasbot-1.8.2/src/ecasbot/settings.py`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/src/ecasbot.egg-info/PKG-INFO` & `ecasbot-1.8.2/src/ecasbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecasbot
-Version: 1.8.1
+Version: 1.8.2
 Summary: EC AntiSpam bot for the Telegram messenger
 Author-email: Vitaly Zaitsev <vitaly@easycoding.org>
 License: GPL-3.0-or-later
 Project-URL: homepage, https://github.com/xvitaly/ecasbot
 Project-URL: documentation, https://github.com/xvitaly/ecasbot/blob/master/docs/README.md
 Project-URL: repository, https://github.com/xvitaly/ecasbot
 Keywords: anti-spam,bot,database-less,telegram,telegram-api,telegram-bot
```

### Comparing `ecasbot-1.8.1/src/ecasbot.egg-info/SOURCES.txt` & `ecasbot-1.8.2/src/ecasbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecasbot-1.8.1/tox.ini` & `ecasbot-1.8.2/tox.ini`

 * *Files identical despite different names*

