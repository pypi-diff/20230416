# Comparing `tmp/ShynaTermux-0.89.3.tar.gz` & `tmp/ShynaTermux-0.89.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShynaTermux-0.89.3.tar", last modified: Fri Dec  2 13:17:40 2022, max compression
+gzip compressed data, was "ShynaTermux-0.89.4.tar", last modified: Sun Apr 16 16:07:13 2023, max compression
```

## Comparing `ShynaTermux-0.89.3.tar` & `ShynaTermux-0.89.4.tar`

### file list

```diff
@@ -1,25 +1,20 @@
-drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2022-12-02 13:17:40.127195 ShynaTermux-0.89.3/
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)     1070 2022-12-01 16:08:07.000000 ShynaTermux-0.89.3/LICENSE
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      284 2022-12-02 13:17:40.127195 ShynaTermux-0.89.3/PKG-INFO
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)       46 2022-12-01 16:08:07.000000 ShynaTermux-0.89.3/README.md
-drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2022-12-02 13:17:40.127195 ShynaTermux-0.89.3/ShynaTermux/
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)     2278 2022-12-01 16:08:07.000000 ShynaTermux-0.89.3/ShynaTermux/ShTermuxSetup.py
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)     2976 2022-12-01 16:08:07.000000 ShynaTermux-0.89.3/ShynaTermux/ShynaCloseAlarm.py
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)     7545 2022-12-01 16:08:07.000000 ShynaTermux-0.89.3/ShynaTermux/ShynaMakeAlarm.py
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)     2473 2022-12-01 16:08:07.000000 ShynaTermux-0.89.3/ShynaTermux/ShynaTalkToMe.py
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)      867 2022-12-01 16:08:07.000000 ShynaTermux-0.89.3/ShynaTermux/Shyna_check_charge.py
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)     1677 2022-12-01 16:08:07.000000 ShynaTermux-0.89.3/ShynaTermux/Shyna_get_connection.py
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)     2326 2022-12-01 16:08:07.000000 ShynaTermux-0.89.3/ShynaTermux/Shyna_get_location.py
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)      471 2022-12-01 16:08:07.000000 ShynaTermux-0.89.3/ShynaTermux/Shyna_setup_test.py
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)      947 2022-12-01 16:08:07.000000 ShynaTermux-0.89.3/ShynaTermux/Shyna_speak_sentence.py
--rw-rw-r--   0 shyna     (1000) shyna     (1000)     6812 2022-12-02 13:16:55.000000 ShynaTermux-0.89.3/ShynaTermux/Sleep_toggle.py
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2022-12-01 16:08:07.000000 ShynaTermux-0.89.3/ShynaTermux/__init__.py
-drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2022-12-02 13:17:40.127195 ShynaTermux-0.89.3/ShynaTermux.egg-info/
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      284 2022-12-02 13:17:40.000000 ShynaTermux-0.89.3/ShynaTermux.egg-info/PKG-INFO
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      558 2022-12-02 13:17:40.000000 ShynaTermux-0.89.3/ShynaTermux.egg-info/SOURCES.txt
--rw-rw-r--   0 shyna     (1000) shyna     (1000)        1 2022-12-02 13:17:40.000000 ShynaTermux-0.89.3/ShynaTermux.egg-info/dependency_links.txt
--rw-rw-r--   0 shyna     (1000) shyna     (1000)      108 2022-12-02 13:17:40.000000 ShynaTermux-0.89.3/ShynaTermux.egg-info/requires.txt
--rw-rw-r--   0 shyna     (1000) shyna     (1000)       12 2022-12-02 13:17:40.000000 ShynaTermux-0.89.3/ShynaTermux.egg-info/top_level.txt
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)      143 2022-12-01 16:08:07.000000 ShynaTermux-0.89.3/pyproject.toml
--rw-rw-r--   0 shyna     (1000) shyna     (1000)       38 2022-12-02 13:17:40.127195 ShynaTermux-0.89.3/setup.cfg
--rwxrwxr-x   0 shyna     (1000) shyna     (1000)      714 2022-12-02 13:16:55.000000 ShynaTermux-0.89.3/setup.py
+drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-04-16 16:07:13.986551 ShynaTermux-0.89.4/
+-rwxrwxr-x   0 shyna     (1000) shyna     (1000)     1070 2023-04-16 15:53:49.000000 ShynaTermux-0.89.4/LICENSE
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      284 2023-04-16 16:07:13.986551 ShynaTermux-0.89.4/PKG-INFO
+-rwxrwxr-x   0 shyna     (1000) shyna     (1000)       46 2023-04-16 15:53:49.000000 ShynaTermux-0.89.4/README.md
+drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-04-16 16:07:13.986551 ShynaTermux-0.89.4/ShynaTermux/
+-rwxrwxr-x   0 shyna     (1000) shyna     (1000)     2229 2023-04-16 16:05:52.000000 ShynaTermux-0.89.4/ShynaTermux/ShynaTermuxSetup.py
+-rwxrwxr-x   0 shyna     (1000) shyna     (1000)      859 2023-04-16 16:05:52.000000 ShynaTermux-0.89.4/ShynaTermux/Shyna_check_charge.py
+-rwxrwxr-x   0 shyna     (1000) shyna     (1000)     1677 2023-04-16 15:53:49.000000 ShynaTermux-0.89.4/ShynaTermux/Shyna_get_connection.py
+-rwxrwxr-x   0 shyna     (1000) shyna     (1000)     2451 2023-04-16 16:05:52.000000 ShynaTermux-0.89.4/ShynaTermux/Shyna_get_location.py
+-rwxrwxr-x   0 shyna     (1000) shyna     (1000)      431 2023-04-16 16:05:52.000000 ShynaTermux-0.89.4/ShynaTermux/Shyna_setup_test.py
+-rwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-04-16 15:53:49.000000 ShynaTermux-0.89.4/ShynaTermux/__init__.py
+drwxrwxr-x   0 shyna     (1000) shyna     (1000)        0 2023-04-16 16:07:13.986551 ShynaTermux-0.89.4/ShynaTermux.egg-info/
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      284 2023-04-16 16:07:13.000000 ShynaTermux-0.89.4/ShynaTermux.egg-info/PKG-INFO
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)      407 2023-04-16 16:07:13.000000 ShynaTermux-0.89.4/ShynaTermux.egg-info/SOURCES.txt
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)        1 2023-04-16 16:07:13.000000 ShynaTermux-0.89.4/ShynaTermux.egg-info/dependency_links.txt
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)       41 2023-04-16 16:07:13.000000 ShynaTermux-0.89.4/ShynaTermux.egg-info/requires.txt
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)       12 2023-04-16 16:07:13.000000 ShynaTermux-0.89.4/ShynaTermux.egg-info/top_level.txt
+-rwxrwxr-x   0 shyna     (1000) shyna     (1000)      119 2023-04-16 16:05:52.000000 ShynaTermux-0.89.4/pyproject.toml
+-rw-rw-r--   0 shyna     (1000) shyna     (1000)       38 2023-04-16 16:07:13.986551 ShynaTermux-0.89.4/setup.cfg
+-rwxrwxr-x   0 shyna     (1000) shyna     (1000)      616 2023-04-16 16:05:52.000000 ShynaTermux-0.89.4/setup.py
```

### Comparing `ShynaTermux-0.89.3/LICENSE` & `ShynaTermux-0.89.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ShynaTermux-0.89.3/ShynaTermux/ShTermuxSetup.py` & `ShynaTermux-0.89.4/ShynaTermux/ShynaTermuxSetup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import nltk
 import os
 
 
 class ShynaTermuxSetup:
     """We need setup few things to make it work and test"""
     case_env = ''
 
@@ -32,15 +31,14 @@
                 os.popen("pkg install sox clang libxml2 libxslt --assume-yes").readline()
                 os.popen("pkg install termux-api --assume-yes").readline()
                 os.popen('pkg install MATHLIB="m" pip install numpy').readline()
                 os.popen("pip install --upgrade ShynaTime ShynaDatabase ShynaTermux ShynaProcess").readline()
                 # os.popen('+')
                 dbhost_cmd = """termux-notification --on-delete 'termux-tts-speak "hey Shivam"' -t 'Hey Shivam' """
                 os.popen(dbhost_cmd)
-                nltk.download('all')
             else:
                 pass
         except Exception as e:
             print(e)
 
 
 if __name__ == '__main__':
```

### Comparing `ShynaTermux-0.89.3/ShynaTermux/Shyna_check_charge.py` & `ShynaTermux-0.89.4/ShynaTermux/Shyna_check_charge.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
-from ShynaProcess import ShynaSpeak
+from ShynaDatabase import Shdatabase
 
 
 class ShynaCharge:
-    s_process = ShynaSpeak.ShynaSpeak()
 
     def check_charge(self):
         try:
             dic_charge = os.popen('termux-battery-status').read()
             dic_charge = eval(dic_charge)
             charge = dic_charge['percentage']
             status = dic_charge['status']
             if int(charge) < 15 and str(status).lower() == 'discharging':
-                self.s_process.shyna_speaks(msg="Hey! Shiv please plugin the charger. My battery is low")
+                cmd = 'termux-tts-speak "Hey! Shiv please plugin the charger. My battery is low"'
+                os.popen(cmd)
             elif int(charge) > 95 and str(status).lower() == 'full':
-                self.s_process.shyna_speaks(msg="Hey! Shiv please unplug the charger. My battery is full")
+                cmd = 'termux-tts-speak "Hey! Shiv please unplug the charger. My battery is full"'
+                os.popen(cmd)
             else:
-                print("All good")
+                pass
         except Exception as e:
             print(e)
 
 
 if __name__ == '__main__':
     ShynaCharge().check_charge()
```

### Comparing `ShynaTermux-0.89.3/ShynaTermux/Shyna_get_connection.py` & `ShynaTermux-0.89.4/ShynaTermux/Shyna_get_connection.py`

 * *Files identical despite different names*

### Comparing `ShynaTermux-0.89.3/ShynaTermux/Shyna_get_location.py` & `ShynaTermux-0.89.4/ShynaTermux/Shyna_get_location.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
                                     + str(new_altitude) + "', '" + str(new_accuracy) + "', '" \
                                     + str(new_vertical_accuracy) + "', '" + str(new_bearing) + "', '" \
                                     + str(new_speed) + "', '" + str(new_elapsedMS) + "','" + str(new_provider) + "')"
                 self.s_data.create_insert_update_or_delete()
                 self.result = "Got Location"
             else:
                 self.result = "Empty location"
+                self.s_data.message = " I got empty location"
+                self.s_data.bot_send_broadcast_msg_to_master()
         except Exception as e:
             print(e)
             self.result = "Exception"
         finally:
             self.s_data.set_date_system(process_name='location_check')
             return self.result
```

### Comparing `ShynaTermux-0.89.3/setup.py` & `ShynaTermux-0.89.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup_args = dict(
      name='ShynaTermux',
-     version='0.89.3',
+     version='0.89.4',
      packages=find_packages(),
      author="Shivam Sharma",
      author_email="shivamsharma1913@gmail.com",
      description="Shyna Backend Functionality Package For Termux",
      long_description=long_description,
      long_description_content_type="text/markdown",
     )
 
-install_requires = ['ShynaTime', 'ShynaProcess', 'ShynaDatabase', "setuptools", "wheel", 'nltk','python-telegram-bot',
-                    'ShynaTelegramBotNotification']
+install_requires = ['ShynaTime', 'ShynaDatabase', "setuptools", "wheel"]
 
 if __name__ == '__main__':
     setup(**setup_args, install_requires=install_requires)
```

