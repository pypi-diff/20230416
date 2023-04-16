# Comparing `tmp/bloodyAD-0.2.6.tar.gz` & `tmp/bloodyAD-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloodyAD-0.2.6.tar", last modified: Mon Feb 13 19:08:32 2023, max compression
+gzip compressed data, was "bloodyAD-1.0.0.tar", last modified: Sun Apr 16 21:48:26 2023, max compression
```

## Comparing `bloodyAD-0.2.6.tar` & `bloodyAD-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-02-13 19:08:32.511994 bloodyAD-0.2.6/
--rwxrwx---   0 silver    (1000) silver    (1001)     1068 2022-09-07 15:23:19.000000 bloodyAD-0.2.6/LICENSE
--rw-r--r--   0 silver    (1000) silver    (1001)     8353 2023-02-13 19:08:32.511994 bloodyAD-0.2.6/PKG-INFO
--rw-r--r--   0 silver    (1000) silver    (1001)     7606 2023-01-19 13:52:09.000000 bloodyAD-0.2.6/README.md
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-02-13 19:08:32.508659 bloodyAD-0.2.6/bloodyAD/
--rw-r--r--   0 silver    (1000) silver    (1001)      148 2022-12-26 08:56:42.000000 bloodyAD-0.2.6/bloodyAD/__init__.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-02-13 19:08:32.511994 bloodyAD-0.2.6/bloodyAD/cli_modules/
--rw-r--r--   0 silver    (1000) silver    (1001)        0 2022-12-26 08:53:44.000000 bloodyAD-0.2.6/bloodyAD/cli_modules/__init__.py
--rw-r--r--   0 silver    (1000) silver    (1001)     3734 2023-02-08 15:08:21.000000 bloodyAD-0.2.6/bloodyAD/cli_modules/add.py
--rw-r--r--   0 silver    (1000) silver    (1001)     9028 2023-02-13 18:20:30.000000 bloodyAD-0.2.6/bloodyAD/cli_modules/get.py
--rw-r--r--   0 silver    (1000) silver    (1001)     2722 2023-02-10 11:17:31.000000 bloodyAD-0.2.6/bloodyAD/cli_modules/remove.py
--rw-r--r--   0 silver    (1000) silver    (1001)     1620 2023-02-10 13:40:08.000000 bloodyAD-0.2.6/bloodyAD/cli_modules/set.py
--rw-r--r--   0 silver    (1000) silver    (1001)     5137 2023-02-13 17:53:40.000000 bloodyAD-0.2.6/bloodyAD/config.py
--rw-r--r--   0 silver    (1000) silver    (1001)     1805 2023-02-08 15:00:01.000000 bloodyAD-0.2.6/bloodyAD/exceptions.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-02-13 19:08:32.511994 bloodyAD-0.2.6/bloodyAD/formatters/
--rw-r--r--   0 silver    (1000) silver    (1001)        0 2023-02-10 15:42:23.000000 bloodyAD-0.2.6/bloodyAD/formatters/__init__.py
--rw-r--r--   0 silver    (1000) silver    (1001)     6121 2023-02-10 13:39:19.000000 bloodyAD-0.2.6/bloodyAD/formatters/accesscontrol.py
--rw-r--r--   0 silver    (1000) silver    (1001)     1625 2023-02-08 15:05:50.000000 bloodyAD-0.2.6/bloodyAD/formatters/common.py
--rw-r--r--   0 silver    (1000) silver    (1001)     5029 2023-02-08 15:06:03.000000 bloodyAD-0.2.6/bloodyAD/formatters/cryptography.py
--rw-r--r--   0 silver    (1000) silver    (1001)     8497 2023-02-08 14:52:01.000000 bloodyAD-0.2.6/bloodyAD/formatters/dns.py
--rw-r--r--   0 silver    (1000) silver    (1001)     2238 2023-02-13 17:59:27.000000 bloodyAD-0.2.6/bloodyAD/formatters/formatters.py
--rw-r--r--   0 silver    (1000) silver    (1001)     1597 2023-02-10 13:39:19.000000 bloodyAD-0.2.6/bloodyAD/formatters/helpers.py
--rw-r--r--   0 silver    (1000) silver    (1001)    16245 2023-01-13 20:47:24.000000 bloodyAD-0.2.6/bloodyAD/formatters/ldaptypes.py
--rw-r--r--   0 silver    (1000) silver    (1001)    23266 2023-01-16 17:02:26.000000 bloodyAD-0.2.6/bloodyAD/formatters/structure.py
--rwxrwx---   0 silver    (1000) silver    (1001)   376797 2023-02-09 09:55:20.000000 bloodyAD-0.2.6/bloodyAD/formatters/winerror.py
--rwxr-xr-x   0 silver    (1000) silver    (1001)     5791 2023-01-19 13:33:13.000000 bloodyAD-0.2.6/bloodyAD/main.py
--rw-r--r--   0 silver    (1000) silver    (1001)     3950 2023-02-08 15:01:35.000000 bloodyAD-0.2.6/bloodyAD/md4.py
--rw-r--r--   0 silver    (1000) silver    (1001)    15256 2023-02-13 18:09:32.000000 bloodyAD-0.2.6/bloodyAD/modules.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-02-13 19:08:32.511994 bloodyAD-0.2.6/bloodyAD/patch/
--rw-r--r--   0 silver    (1000) silver    (1001)    46939 2023-02-10 11:04:06.000000 bloodyAD-0.2.6/bloodyAD/patch/ldap3_patch.py
--rw-r--r--   0 silver    (1000) silver    (1001)      552 2023-02-13 18:21:12.000000 bloodyAD-0.2.6/bloodyAD/patch/winacl_patch.py
--rw-r--r--   0 silver    (1000) silver    (1001)    12690 2023-02-10 16:09:38.000000 bloodyAD-0.2.6/bloodyAD/utils.py
-drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-02-13 19:08:32.511994 bloodyAD-0.2.6/bloodyAD.egg-info/
--rw-r--r--   0 silver    (1000) silver    (1001)     8353 2023-02-13 19:08:32.000000 bloodyAD-0.2.6/bloodyAD.egg-info/PKG-INFO
--rw-r--r--   0 silver    (1000) silver    (1001)      888 2023-02-13 19:08:32.000000 bloodyAD-0.2.6/bloodyAD.egg-info/SOURCES.txt
--rw-r--r--   0 silver    (1000) silver    (1001)        1 2023-02-13 19:08:32.000000 bloodyAD-0.2.6/bloodyAD.egg-info/dependency_links.txt
--rw-r--r--   0 silver    (1000) silver    (1001)       48 2023-02-13 19:08:32.000000 bloodyAD-0.2.6/bloodyAD.egg-info/entry_points.txt
--rw-r--r--   0 silver    (1000) silver    (1001)      176 2023-02-13 19:08:32.000000 bloodyAD-0.2.6/bloodyAD.egg-info/requires.txt
--rw-r--r--   0 silver    (1000) silver    (1001)        9 2023-02-13 19:08:32.000000 bloodyAD-0.2.6/bloodyAD.egg-info/top_level.txt
--rw-r--r--   0 silver    (1000) silver    (1001)       38 2023-02-13 19:08:32.511994 bloodyAD-0.2.6/setup.cfg
--rw-r--r--   0 silver    (1000) silver    (1001)     1340 2023-02-10 15:41:01.000000 bloodyAD-0.2.6/setup.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.775577 bloodyAD-1.0.0/
+-rwxrwx---   0 silver    (1000) silver    (1001)     1068 2022-09-07 15:23:19.000000 bloodyAD-1.0.0/LICENSE
+-rw-r--r--   0 silver    (1000) silver    (1001)     8342 2023-04-16 21:48:26.775577 bloodyAD-1.0.0/PKG-INFO
+-rw-r--r--   0 silver    (1000) silver    (1001)     7595 2023-03-27 18:43:52.000000 bloodyAD-1.0.0/README.md
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.772246 bloodyAD-1.0.0/bloodyAD/
+-rw-r--r--   0 silver    (1000) silver    (1001)      108 2023-03-28 10:43:06.000000 bloodyAD-1.0.0/bloodyAD/__init__.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.772246 bloodyAD-1.0.0/bloodyAD/cli_modules/
+-rw-r--r--   0 silver    (1000) silver    (1001)        0 2022-12-26 08:53:44.000000 bloodyAD-1.0.0/bloodyAD/cli_modules/__init__.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    16094 2023-04-16 20:55:01.000000 bloodyAD-1.0.0/bloodyAD/cli_modules/add.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    10343 2023-04-16 20:45:02.000000 bloodyAD-1.0.0/bloodyAD/cli_modules/get.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     8942 2023-04-16 20:41:09.000000 bloodyAD-1.0.0/bloodyAD/cli_modules/remove.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     3332 2023-04-16 20:41:09.000000 bloodyAD-1.0.0/bloodyAD/cli_modules/set.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     1920 2023-03-18 13:00:15.000000 bloodyAD-1.0.0/bloodyAD/exceptions.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.772246 bloodyAD-1.0.0/bloodyAD/formatters/
+-rw-r--r--   0 silver    (1000) silver    (1001)        0 2023-02-10 15:42:23.000000 bloodyAD-1.0.0/bloodyAD/formatters/__init__.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     5952 2023-04-12 13:41:14.000000 bloodyAD-1.0.0/bloodyAD/formatters/accesscontrol.py
+-rw-r--r--   0 silver    (1000) silver    (1001)   118418 2023-04-16 20:41:10.000000 bloodyAD-1.0.0/bloodyAD/formatters/adschema.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     2594 2023-04-16 20:41:09.000000 bloodyAD-1.0.0/bloodyAD/formatters/common.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     5029 2023-02-08 15:06:03.000000 bloodyAD-1.0.0/bloodyAD/formatters/cryptography.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     8547 2023-04-16 20:24:41.000000 bloodyAD-1.0.0/bloodyAD/formatters/dns.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     1773 2023-04-16 20:46:39.000000 bloodyAD-1.0.0/bloodyAD/formatters/formatters.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     2016 2023-04-16 20:41:10.000000 bloodyAD-1.0.0/bloodyAD/formatters/helpers.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    16246 2023-03-18 13:05:44.000000 bloodyAD-1.0.0/bloodyAD/formatters/ldaptypes.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    23266 2023-01-16 17:02:26.000000 bloodyAD-1.0.0/bloodyAD/formatters/structure.py
+-rwxrwx---   0 silver    (1000) silver    (1001)   486395 2023-03-18 13:06:07.000000 bloodyAD-1.0.0/bloodyAD/formatters/winerror.py
+-rwxr-xr-x   0 silver    (1000) silver    (1001)     8007 2023-04-16 20:41:10.000000 bloodyAD-1.0.0/bloodyAD/main.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     3950 2023-02-08 15:01:35.000000 bloodyAD-1.0.0/bloodyAD/md4.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.775577 bloodyAD-1.0.0/bloodyAD/network/
+-rw-r--r--   0 silver    (1000) silver    (1001)     2537 2023-03-18 13:00:15.000000 bloodyAD-1.0.0/bloodyAD/network/config.py
+-rw-r--r--   0 silver    (1000) silver    (1001)     8680 2023-04-16 20:57:57.000000 bloodyAD-1.0.0/bloodyAD/network/ldap.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.775577 bloodyAD-1.0.0/bloodyAD/patch/
+-rw-r--r--   0 silver    (1000) silver    (1001)    47840 2023-03-18 13:05:45.000000 bloodyAD-1.0.0/bloodyAD/patch/ldap3_patch.py
+-rw-r--r--   0 silver    (1000) silver    (1001)    16697 2023-04-16 20:51:07.000000 bloodyAD-1.0.0/bloodyAD/utils.py
+drwxr-xr-x   0 silver    (1000) silver    (1001)        0 2023-04-16 21:48:26.772246 bloodyAD-1.0.0/bloodyAD.egg-info/
+-rw-r--r--   0 silver    (1000) silver    (1001)     8342 2023-04-16 21:48:26.000000 bloodyAD-1.0.0/bloodyAD.egg-info/PKG-INFO
+-rw-r--r--   0 silver    (1000) silver    (1001)      902 2023-04-16 21:48:26.000000 bloodyAD-1.0.0/bloodyAD.egg-info/SOURCES.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)        1 2023-04-16 21:48:26.000000 bloodyAD-1.0.0/bloodyAD.egg-info/dependency_links.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)       48 2023-04-16 21:48:26.000000 bloodyAD-1.0.0/bloodyAD.egg-info/entry_points.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)      190 2023-04-16 21:48:26.000000 bloodyAD-1.0.0/bloodyAD.egg-info/requires.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)        9 2023-04-16 21:48:26.000000 bloodyAD-1.0.0/bloodyAD.egg-info/top_level.txt
+-rw-r--r--   0 silver    (1000) silver    (1001)       38 2023-04-16 21:48:26.775577 bloodyAD-1.0.0/setup.cfg
+-rw-r--r--   0 silver    (1000) silver    (1001)     1365 2023-04-16 20:41:10.000000 bloodyAD-1.0.0/setup.py
```

### Comparing `bloodyAD-0.2.6/LICENSE` & `bloodyAD-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bloodyAD-0.2.6/PKG-INFO` & `bloodyAD-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bloodyAD
-Version: 0.2.6
+Version: 1.0.0
 Summary: AD Privesc Swiss Army Knife
 Home-page: https://github.com/CravateRouge/bloodyAD
-Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v0.2.6.tar.gz
+Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.0.tar.gz
 Author: CravateRouge
 Author-email: baptiste.crepin@ntymail.com
 License: MIT
 Keywords: Active Directory,Privilege Escalation
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -49,23 +49,23 @@
 pacman -S krb5
 ```
 
 A python package is available:
 
 ```ps1
 pip install bloodyAD
-bloodyAD --host 172.16.1.15 -d bloody.local -k changePassword john.doe 'Password123!'
+bloodyAD --host 172.16.1.15 -d bloody.local -k set password john.doe 'Password123!'
 ```
 
 Or you can clone the repo:
 
 ```ps1
 git clone --depth 1 https://github.com/CravateRouge/bloodyAD
 pip install .
-bloodyAD --host 172.16.1.15 -d bloody.local -k changePassword john.doe 'Password123!'
+bloodyAD --host 172.16.1.15 -d bloody.local -k set password john.doe 'Password123!'
 ```
 
 ### Dependencies
 
 - Python 3
 - DSinternals
 - Impacket
@@ -73,15 +73,15 @@
 - Gssapi (linux) or Winkerberos (Windows)
 
 ## Usage
 
 Simple usage:
 
 ```ps1
-bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 changePassword john.doe 'Password123!'
+bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 set password john.doe 'Password123!'
 ```
 
 **Note:** You can find more examples on <https://cravaterouge.github.io/> and in the documentation folder of this project
 
 List of all available functions:
 
 ```ps1
@@ -111,81 +111,77 @@
     get                 [GET] function category
     remove              [REMOVE] function category
 ```
 
 Help text to use a specific function:
 
 ```ps1
-[bloodyAD]$ bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 changePassword -h
-usage: 
-    Change the target password without knowing the old one using LDAPS or RPC
-    Args:
-        identity: sAMAccountName, DN, GUID or SID of the target (You must have write permission on it)
-        new_pass: new password for the target
-    
-       [-h] [func_args ...]
+[bloodyAD]$ bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 set password -h
+usage: bloodyAD.py set password [-h] [--oldpass OLDPASS] target newpass
 
 positional arguments:
-  func_args
+  target             sAMAccountName, DN, GUID or SID of the target
+  newpass            new password for the target
 
-optional arguments:
-  -h, --help  show this help message and exit
+options:
+  -h, --help         show this help message and exit
+  --oldpass OLDPASS  old password of the target, mandatory if you don't have "change password" permission on the target (default: None)
   ```
 
 ## How it works
 
 bloodyAD communicates with a DC using mainly the LDAP protocol in order to get information or add/modify/delete AD objects. ~~A password cannot be updated with LDAP, it must be a secure connection that is LDAPS or SAMR. A DC doesn't have LDAPS activated by default because it must be configured (with a certificate) so SAMR is used in those cases.~~ Exchange of sensitive information such as passwords are now supported using cleartext LDAP.
 
 ## Useful commands
 
 ```ps1
 # Get group members
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes Users member 
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get object Users --attr member 
 
 # Get minimum password length policy
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes 'DC=bloody,DC=local' minPwdLength
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get object 'DC=bloody,DC=local' --attr minPwdLength
 
 # Get AD functional level
-bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes 'DC=bloody,DC=local' msDS-Behavior-Version
+bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 get object 'DC=bloody,DC=local' --attr msDS-Behavior-Version
 
 # Get all users of the domain
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getChildObjects 'DC=bloody,DC=local' user
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get children 'DC=bloody,DC=local' --type user
 
 # Get all computers of the domain
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getChildObjects 'DC=bloody,DC=local' computer
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get children 'DC=bloody,DC=local' --type computer
 
 # Get all containers of the domain
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getChildObjects 'DC=bloody,DC=local' container
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get children 'DC=bloody,DC=local' --type container
 
 # Enable DONT_REQ_PREAUTH for ASREPRoast
-bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 setUserAccountControl john.doe 0x400000
+bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 add uac john.doe DONT_REQ_PREAUTH
 
 # Disable ACCOUNTDISABLE
-bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 setUserAccountControl john.doe 0x0002 False
+bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 remove uac john.doe ACCOUNTDISABLE
 
 # Get UserAccountControl flags
-bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes john.doe userAccountControl
+bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 get object john.doe --attr userAccountControl
 
 # Read GMSA account password
-bloodyAD -u john.doe -d bloody -p Password512 --host 192.168.10.2 getObjectAttributes gmsaAccount$ msDS-ManagedPassword
+bloodyAD -u john.doe -d bloody -p Password512 --host 192.168.10.2 get object 'gmsaAccount$' --attr msDS-ManagedPassword
 
 # Read LAPS password
-bloodyAD -u john.doe -d bloody -p Password512 --host 192.168.10.2 getObjectAttributes COMPUTER$ ms-Mcs-AdmPwd
+bloodyAD -u john.doe -d bloody -p Password512 --host 192.168.10.2 get object 'COMPUTER$' --attr ms-Mcs-AdmPwd
 
 # Read quota for adding computer objects to domain
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes 'DC=bloody,DC=local' ms-DS-MachineAccountQuota
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get object 'DC=bloody,DC=local' --attr ms-DS-MachineAccountQuota
 
 # Add a new DNS entry
-bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 add domainDNSRecord my_machine_name 192.168.10.48
+bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 add dnsRecord my_machine_name 192.168.10.48
 
 # Remove a DNS entry
-bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 remove domainDNSRecord my_machine_name 192.168.10.48
+bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 remove dnsRecord my_machine_name 192.168.10.48
 
 # Get AD DNS records
-bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 get domainDNSRecord
+bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 get dnsDump
 
 ```
 
 ## Acknowledgements
 - Thanks to [impacket](https://github.com/fortra/impacket) contributors. [Structures](https://github.com/fortra/impacket/blob/master/impacket/structure.py) and several [LDAP attacks](https://github.com/fortra/impacket/blob/master/impacket/examples/ntlmrelayx/attacks/ldapattack.py) are based on their work.
 - Thanks to [@PowerShellMafia](https://github.com/PowerShellMafia) team ([PowerView.ps1](https://github.com/PowerShellMafia/PowerSploit/blob/master/Recon/PowerView.ps1)) and their work on AD which inspired this tool.
 - Thanks to [@dirkjanm](https://github.com/dirkjanm) ([adidnsdump.py](https://github.com/dirkjanm/adidnsdump)) and ([@Kevin-Robertson](https://github.com/Kevin-Robertson))([Invoke-DNSUpdate.ps1](https://github.com/Kevin-Robertson/Powermad/blob/master/Invoke-DNSUpdate.ps1)) for their work on AD DNS which inspired DNS functionnalities.
```

### Comparing `bloodyAD-0.2.6/README.md` & `bloodyAD-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -29,23 +29,23 @@
 pacman -S krb5
 ```
 
 A python package is available:
 
 ```ps1
 pip install bloodyAD
-bloodyAD --host 172.16.1.15 -d bloody.local -k changePassword john.doe 'Password123!'
+bloodyAD --host 172.16.1.15 -d bloody.local -k set password john.doe 'Password123!'
 ```
 
 Or you can clone the repo:
 
 ```ps1
 git clone --depth 1 https://github.com/CravateRouge/bloodyAD
 pip install .
-bloodyAD --host 172.16.1.15 -d bloody.local -k changePassword john.doe 'Password123!'
+bloodyAD --host 172.16.1.15 -d bloody.local -k set password john.doe 'Password123!'
 ```
 
 ### Dependencies
 
 - Python 3
 - DSinternals
 - Impacket
@@ -53,15 +53,15 @@
 - Gssapi (linux) or Winkerberos (Windows)
 
 ## Usage
 
 Simple usage:
 
 ```ps1
-bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 changePassword john.doe 'Password123!'
+bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 set password john.doe 'Password123!'
 ```
 
 **Note:** You can find more examples on <https://cravaterouge.github.io/> and in the documentation folder of this project
 
 List of all available functions:
 
 ```ps1
@@ -91,81 +91,77 @@
     get                 [GET] function category
     remove              [REMOVE] function category
 ```
 
 Help text to use a specific function:
 
 ```ps1
-[bloodyAD]$ bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 changePassword -h
-usage: 
-    Change the target password without knowing the old one using LDAPS or RPC
-    Args:
-        identity: sAMAccountName, DN, GUID or SID of the target (You must have write permission on it)
-        new_pass: new password for the target
-    
-       [-h] [func_args ...]
+[bloodyAD]$ bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 set password -h
+usage: bloodyAD.py set password [-h] [--oldpass OLDPASS] target newpass
 
 positional arguments:
-  func_args
+  target             sAMAccountName, DN, GUID or SID of the target
+  newpass            new password for the target
 
-optional arguments:
-  -h, --help  show this help message and exit
+options:
+  -h, --help         show this help message and exit
+  --oldpass OLDPASS  old password of the target, mandatory if you don't have "change password" permission on the target (default: None)
   ```
 
 ## How it works
 
 bloodyAD communicates with a DC using mainly the LDAP protocol in order to get information or add/modify/delete AD objects. ~~A password cannot be updated with LDAP, it must be a secure connection that is LDAPS or SAMR. A DC doesn't have LDAPS activated by default because it must be configured (with a certificate) so SAMR is used in those cases.~~ Exchange of sensitive information such as passwords are now supported using cleartext LDAP.
 
 ## Useful commands
 
 ```ps1
 # Get group members
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes Users member 
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get object Users --attr member 
 
 # Get minimum password length policy
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes 'DC=bloody,DC=local' minPwdLength
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get object 'DC=bloody,DC=local' --attr minPwdLength
 
 # Get AD functional level
-bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes 'DC=bloody,DC=local' msDS-Behavior-Version
+bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 get object 'DC=bloody,DC=local' --attr msDS-Behavior-Version
 
 # Get all users of the domain
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getChildObjects 'DC=bloody,DC=local' user
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get children 'DC=bloody,DC=local' --type user
 
 # Get all computers of the domain
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getChildObjects 'DC=bloody,DC=local' computer
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get children 'DC=bloody,DC=local' --type computer
 
 # Get all containers of the domain
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getChildObjects 'DC=bloody,DC=local' container
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get children 'DC=bloody,DC=local' --type container
 
 # Enable DONT_REQ_PREAUTH for ASREPRoast
-bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 setUserAccountControl john.doe 0x400000
+bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 add uac john.doe DONT_REQ_PREAUTH
 
 # Disable ACCOUNTDISABLE
-bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 setUserAccountControl john.doe 0x0002 False
+bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 remove uac john.doe ACCOUNTDISABLE
 
 # Get UserAccountControl flags
-bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes john.doe userAccountControl
+bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 get object john.doe --attr userAccountControl
 
 # Read GMSA account password
-bloodyAD -u john.doe -d bloody -p Password512 --host 192.168.10.2 getObjectAttributes gmsaAccount$ msDS-ManagedPassword
+bloodyAD -u john.doe -d bloody -p Password512 --host 192.168.10.2 get object 'gmsaAccount$' --attr msDS-ManagedPassword
 
 # Read LAPS password
-bloodyAD -u john.doe -d bloody -p Password512 --host 192.168.10.2 getObjectAttributes COMPUTER$ ms-Mcs-AdmPwd
+bloodyAD -u john.doe -d bloody -p Password512 --host 192.168.10.2 get object 'COMPUTER$' --attr ms-Mcs-AdmPwd
 
 # Read quota for adding computer objects to domain
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes 'DC=bloody,DC=local' ms-DS-MachineAccountQuota
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get object 'DC=bloody,DC=local' --attr ms-DS-MachineAccountQuota
 
 # Add a new DNS entry
-bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 add domainDNSRecord my_machine_name 192.168.10.48
+bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 add dnsRecord my_machine_name 192.168.10.48
 
 # Remove a DNS entry
-bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 remove domainDNSRecord my_machine_name 192.168.10.48
+bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 remove dnsRecord my_machine_name 192.168.10.48
 
 # Get AD DNS records
-bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 get domainDNSRecord
+bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 get dnsDump
 
 ```
 
 ## Acknowledgements
 - Thanks to [impacket](https://github.com/fortra/impacket) contributors. [Structures](https://github.com/fortra/impacket/blob/master/impacket/structure.py) and several [LDAP attacks](https://github.com/fortra/impacket/blob/master/impacket/examples/ntlmrelayx/attacks/ldapattack.py) are based on their work.
 - Thanks to [@PowerShellMafia](https://github.com/PowerShellMafia) team ([PowerView.ps1](https://github.com/PowerShellMafia/PowerSploit/blob/master/Recon/PowerView.ps1)) and their work on AD which inspired this tool.
 - Thanks to [@dirkjanm](https://github.com/dirkjanm) ([adidnsdump.py](https://github.com/dirkjanm/adidnsdump)) and ([@Kevin-Robertson](https://github.com/Kevin-Robertson))([Invoke-DNSUpdate.ps1](https://github.com/Kevin-Robertson/Powermad/blob/master/Invoke-DNSUpdate.ps1)) for their work on AD DNS which inspired DNS functionnalities.
```

### Comparing `bloodyAD-0.2.6/bloodyAD/cli_modules/get.py` & `bloodyAD-1.0.0/bloodyAD/cli_modules/get.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,248 +1,283 @@
-from bloodyAD.formatters import formatters, ldaptypes, accesscontrol
-from bloodyAD.utils import LOG, getDefaultNamingContext, search, getOrganizationalUnits, getObjectSID, resolvDN
-import json, logging
-from functools import lru_cache
+from bloodyAD import utils
+from bloodyAD.utils import LOG
+from typing import Literal
 import ldap3
 from ldap3.core.exceptions import LDAPNoSuchObjectResult
-from ldap3.protocol.formatters.formatters import format_sid
 
 
-def dnsRecord(
-    conn,
-    zone: str = None,
-    include_tombstoned: bool = False,
-    include_rootservers: bool = False,
-    no_legacy: bool = False,
-    no_forest: bool = False,
-    no_domain: bool = False,
-):
+def children(conn, target: str, type: str = "*"):
+    """
+    Lists children for a given target object
+
+    :param target: sAMAccountName, DN, GUID or SID of the target
+    :param type: objectClass of object to fetch: user, computer, group, organizationalUnit, container, groupPolicyContainer, etc
+    """
+    return conn.ldap.bloodysearch(
+        target, f"(objectClass={type})", search_scope=ldap3.SUBTREE, attr=""
+    )
+
+
+# TODO: Fetch records from Global Catalog and also other partitions stored on other DC if possible
+def dnsDump(conn, zone: str = None, detail: bool = False):
     """
     Retrieves DNS records of the Active Directory readable by the user
 
     :param zone: if set, prints only records in this zone
-    :param include_tombstoned: if set, includes tombstoned records
-    :param include_rootservers: if set, includes DNS root servers
-    :param no_legacy: if set, excludes records in main partition
-    :param no_forest: if set, excludes records in forest partition
-    :param no_domain: if set, excludes records in domain partition
-    """
-    ldap_conn = conn.getLdapConnection()
-
-    naming_context = getDefaultNamingContext(ldap_conn)
-    containers = []
-    container = ""
-    if not no_legacy:
-        container = naming_context
-        if zone:
-            container = f"DC={zone},CN=MicrosoftDNS,CN=System,{container}"
-        containers.append(container)
-    if not no_forest:
-        container = f"DC=ForestDnsZones,{naming_context}"
-        if zone:
-            container = f"DC={zone},CN=MicrosoftDNS,{container}"
-        containers.append(container)
-    if not no_domain:
-        container = f"DC=DomainDnsZones,{naming_context}"
-        if zone:
-            container = f"DC={zone},CN=MicrosoftDNS,{container}"
-        containers.append(container)
-
-    printable_entries = ""
-    record_list = []
-    for container_dn in containers:
-        res = None
+    :param detail: if set includes system records such as _ldap, _kerberos...
+    """
+    entries = None
+    filter = "(objectClass=dnsNode)"
+
+    if not detail:
+        prefix_filter = ""
+        for prefix in [
+            "gc",
+            "_gc.*",
+            "_kerberos.*",
+            "_kpasswd.*",
+            "_ldap.*",
+            "_msdcs",
+            "@",
+            "DomainDnsZones",
+            "ForestDnsZones",
+        ]:
+            prefix_filter += f"(!(name={prefix}))"
+        filter = f"(&{filter}{prefix_filter})"
+
+    for nc in conn.ldap.appNCs + [conn.ldap.domainNC]:
         try:
-            res = search(
-                conn,
-                container_dn,
-                ldap_filter="(objectClass=dnsNode)",
-                attr=["dnsRecord", "dNSTombstoned"],
+            entries = conn.ldap.bloodysearch(
+                nc,
+                filter,
                 search_scope=ldap3.SUBTREE,
+                attr=["dnsRecord", "name", "objectClass"],
             )
         except LDAPNoSuchObjectResult:
             continue
 
-        for entry in res:
-            # Ignore searchResRef entry
-            if entry["type"] == "searchResRef":
-                continue
-            if entry["attributes"]["dNSTombstoned"] and not include_tombstoned:
+        for entry in entries:
+            domain_suffix = entry["distinguishedName"].split(",")[1]
+            domain_suffix = domain_suffix.split("=")[1]
+
+            # RootDNSServers and ..TrustAnchors are system records not interesting for offensive normally
+            if domain_suffix == "RootDNSServers" or domain_suffix == "..TrustAnchors":
                 continue
-            dn = entry["dn"][3:]
-            hostname = ""
-            skip = False
-            for level in dn.split(",CN=")[0].split(",DC="):
-                if level == "RootDNSServers":
-                    skip = not include_rootservers
-                    break
-                if level == "@":
-                    continue
-                hostname += level + "."
-            # Ignore this entry
-            if skip:
+
+            if zone and zone not in domain_suffix:
                 continue
 
-            if not hostname:
-                hostname = "."
+            domain_name = entry["name"]
+            if (
+                len(domain_suffix.split(".in-addr.arpa")) < 2
+            ):  # If it's not a reverse lookup, domain suffix is parent name
+                domain_name = domain_name + "." + domain_suffix
+
+            if domain_name == "@":  # @ is for dnsZone info
+                domain_name = domain_suffix
 
-            for record in entry["attributes"]["dnsRecord"]:
-                printable_entries += hostname
-                record_data = None
+            yield_entry = {"domain": domain_name}
+            for record in entry["dnsRecord"]:
                 try:
                     if record["Type"] in ["A", "AAAA", "NS", "CNAME", "PTR", "TXT"]:
-                        record_data = [record["Data"], record["Type"]]
+                        yield_entry[record["Type"]] = record["Data"]
                     elif record["Type"] == "MX":
-                        record_data = [record["Data"]["Name"], record["Type"]]
+                        yield_entry[record["Type"]] = record["Data"]["Name"]
                     elif record["Type"] == "SRV":
-                        record_data = [
-                            f"{record['Data']['Target']}:{record['Data']['Port']}",
-                            record["Type"],
-                        ]
+                        yield_entry[record["Type"]] = (
+                            f"{record['Data']['Target']}:{record['Data']['Port']}"
+                        )
                     elif record["Type"] == "SOA":
-                        record_data = [
+                        yield_entry[record["Type"]] = [
                             record["Data"]["PrimaryServer"],
-                            record["Data"]["zoneAdminEmail"],
-                            record["Type"],
+                            record["Data"]["zoneAdminEmail"].replace(".", "@", 1),
                         ]
-                    else:
-                        LOG.warn("[!] Record type: " + record["Type"] + " not supported yet! Raise an issue if you think it matters")
-                        continue
-
                 except KeyError:
                     LOG.error("[-] KeyError for record: " + record)
                     continue
-
-                for data in record_data:
-                    printable_entries += f" :-> {data}"
-                printable_entries += "\n"
-                record_list.append([hostname, record_data])
-
-    LOG.info(printable_entries)
-    return record_list
+            yield yield_entry
 
 
-@lru_cache
-def membership(
-    conn,
-    target: str,
-    no_recurse: bool = False
-):
+def membership(conn, target: str, no_recurse: bool = False):
     """
-    Retrieves all groups an object belongs to
+    Retrieves SID and SAM Account Names of all groups a target belongs to
 
     :param target: sAMAccountName, DN, GUID or SID of the target
-    :param no_recurse: list groups recursively
+    :param no_recurse: if set, doesn't retrieve groups where target isn't a direct member
     """
     # We fetch primaryGroupID, since this group is not reflected in memberOf
-    # Additionally we get objectSid to have the domain sid it is helpfuf
-    # to resolv the primary group RID to a DN
-    # Finally we had the special identity groups: Authenticated Users and Everyone
-
-    data = search(conn, target, attr=["objectSid", "memberOf", "primaryGroupID"])
-    data = data[0]["attributes"]
-    groups = data["memberOf"]
-
-    if data["primaryGroupID"]:
-        domain_sid = "-".join(data["objectSid"].split("-")[:-1])
-        primary_group_sid = domain_sid + "-" + str(data["primaryGroupID"])
-        ldap_conn = conn.getLdapConnection()
-        primary_group_dn = resolvDN(ldap_conn, primary_group_sid)
-        groups.append(primary_group_dn)
-
-    found_groups = set(groups)
-    if not no_recurse:
-        for group in groups:
-            new_group = membership(conn, group, no_recurse)
-            found_groups.update(new_group)
-
-    groups_json = json.dumps(sorted(list(found_groups)), indent=4, sort_keys=True)
-    LOG.info(groups_json)
-
-    return found_groups
+    # Additionally we get objectSid to have the domain sid
+    # it is helpful to resolve the primary group RID to a DN
+    # Finally we add the special identity groups: Authenticated Users and Everyone
+
+    filter = ""
+    if no_recurse:
+        entries = conn.ldap.bloodysearch(target, attr=["objectSid", "memberOf"])
+        for entry in entries:
+            for group in entry["memberOf"]:
+                filter += f"(distinguishedName={group})"
+        if not filter:
+            LOG.warning("[!] No direct group membership found")
+            return []
+    else:
+        # [MS-ADTS] 3.1.1.4.5.19 tokenGroups, tokenGroupsNoGCAcceptable
+        attr = "tokenGroups"
+        entries = conn.ldap.bloodysearch(target, attr=[attr])
+        for entry in entries:
+            for groupSID in entry[attr]:
+                filter += f"(objectSID={groupSID})"
+        if not filter:
+            LOG.warning("no GC Server available, the set of groups might be incomplete")
+            attr = "tokenGroupsNoGCAcceptable"
+            entries = conn.ldap.bloodysearch(target, attr=[attr])
+            for entry in entries:
+                for groupSID in entry[attr]:
+                    filter += f"(objectSID={groupSID})"
+
+    entries = conn.ldap.bloodysearch(
+        conn.ldap.domainNC,
+        f"(|{filter})",
+        search_scope=ldap3.SUBTREE,
+        attr=["objectSID", "sAMAccountName"],
+    )
+    return entries
 
 
 def object(
-    conn,
-    target: str,
-    attr: str = "*",
-    resolve_sd: bool = False,
-    raw: bool = False
+    conn, target: str, attr: str = "*", resolve_sd: bool = False, raw: bool = False
 ):
     """
-    Retrieves LDAP attributes for the target object provided
+    Retrieves LDAP attributes for the target object provided, binary data will be outputed in base64
 
     :param target: sAMAccountName, DN, GUID or SID of the target
     :param attr: name of the attribute to retrieve, retrieves all the attributes by default
     :param resolve_sd: if set, permissions linked to a security descriptor will be resolved !!resolving can take some time!!
     :param raw: if set, will return attributes as sent by the server without any formatting, binary data will be outputed in base64
     """
+    entries = conn.ldap.bloodysearch(target, attr=attr, raw=raw)
+    rendered_entries = utils.renderSearchResult(entries)
+    if resolve_sd and not raw:
+        for entry in rendered_entries:
+            if "nTSecurityDescriptor" in entry:
+                entry["nTSecurityDescriptor"] = utils.renderSD(
+                    entry["nTSecurityDescriptor"], conn
+                )
+            yield entry
+    else:
+        yield from rendered_entries
 
-    old_resolving = formatters.RESOLVING
-    if resolve_sd:
-        formatters.RESOLVING = True
-    
-    object_res = search(conn, target, attr=attr)
-    formatters.RESOLVING = old_resolving
 
-    if raw:
-        object_attributes = object_res[0]["raw_attributes"]
-    else:
-        # We call response_to_json because it automatically converts
-        # non printable objects into JSON
-        object_json = conn.getLdapConnection().response_to_json()
-        # And then we remove the "entries" container unnecessary for one object/entry
-        object_attributes = json.loads(object_json)["entries"][0]["attributes"]
-        
-    printable_object = json.dumps(object_attributes, indent=4, sort_keys=True)
-    LOG.info(printable_object)
-
-    return object_attributes
-
-
-def writableOU(
-    conn, 
-    target: str,
-    page_size: int = 1000
+def search(
+    conn,
+    searchbase: str,
+    filter: str = "(objectClass=*)",
+    attr: str = "*",
+    raw: bool = False,
 ):
     """
-    Retrieves Organizational Units writable by target
+    Searches in LDAP database, binary data will be outputed in base64
 
-    :param target: sAMAccountName, DN, GUID or SID of the target
-    :param page_size: number of OUs to fetch in each request
+    :param searchbase: DN of the parent object
+    :param filter: filter to apply to the LDAP search (see Microsoft LDAP filter syntax)
+    :param attr: attributes to retrieve separated by a comma
+    :param raw: if set, will return attributes as sent by the server without any formatting, binary data will be outputed in base64
     """
+    entries = conn.ldap.bloodysearch(
+        searchbase,
+        filter,
+        search_scope=ldap3.SUBTREE,
+        attr=attr.split(","),
+        raw=raw,
+        generator=True,
+    )
 
-    # Fetch group membership
-    LOG.setLevel(logging.WARNING)
-    groups = membership(conn, target)
-    LOG.setLevel(logging.INFO)
-
-    groups_sid = [format_sid(getObjectSID(conn, group)) for group in groups]
-    groups_sid.append("S-1-5-11")
-    groups_sid.append("S-1-1-0")
-
-    # Walk the OU hierarchy
-    attr = ["ntSecurityDescriptor", "distinguishedName"]
-    vulnerable_ous = set()
-    interesting_perms = ["FULL_CONTROL", "GENERIC_ALL", "GENERIC_WRITE", "ADS_RIGHT_DS_CREATE_CHILD"]
-    for ou in getOrganizationalUnits(conn, attributes=attr, page_size=page_size):
-
-        sd = ldaptypes.SR_SECURITY_DESCRIPTOR(data=ou["raw_attributes"]["nTSecurityDescriptor"][0])
-
-        ownerSid = sd["OwnerSid"].formatCanonical()
-        if ownerSid in groups_sid:
-            LOG.info(f"owner of {ou['attributes']['distinguishedName']}")
-            vulnerable_ous.update(ou['attributes']['distinguishedName'])
-            continue
+    return utils.renderSearchResult(entries)
+
+
+# TODO: Search writable for application partitions too?
+def writable(
+    conn,
+    otype: Literal["ALL", "OU", "USER", "COMPUTER", "GROUP", "DOMAIN", "GPO"] = "ALL",
+    right: Literal["ALL", "WRITE", "CHILD"] = "ALL",
+    detail: bool = False,
+    # partition: Literal["DOMAIN", "DNS", "ALL"] = "DOMAIN"
+):
+    """
+    Retrieves objects writable by client
 
-        for ace in sd["Dacl"]["Data"]:
-            aceSid = ace["Ace"]["Sid"].formatCanonical()
-            if aceSid in groups_sid:
-                aceType = ace["TypeName"]
-                if aceType == 'ACCESS_ALLOWED_ACE':
-                    aceMask = accesscontrol.decodeAccessMask(ace["Ace"]["Mask"])
-                    for perm in aceMask:
-                        if perm in interesting_perms:
-                            LOG.info(f"{perm} on {ou['attributes']['distinguishedName']}")
-                            vulnerable_ous.update(ou['attributes']['distinguishedName'])
+    :param otype: type of writable object to retrieve
+    :param right: type of right to search
+    :param detail: if set, displays attributes/object types you can write/create for the object
+    """
+    #:param partition: directory partition a.k.a naming context to explore
 
-    return vulnerable_ous
+    if otype == "ALL":
+        objectClass = "*"
+    elif otype == "OU":
+        objectClass = "container"
+    elif otype == "GPO":
+        objectClass = "groupPolicyContainer"
+    else:
+        objectClass = otype
+
+    attr_params = {}
+    genericReturn = (
+        (lambda a: [b for b in a])
+        if detail
+        else (lambda a: ["permission"] if a else [])
+    )
+    if right == "WRITE" or right == "ALL":
+        attr_params["allowedAttributesEffective"] = {
+            "lambda": genericReturn,
+            "right": "WRITE",
+        }
+
+        def testSDRights(a):  # Mask defined in MS-ADTS for allowedAttributesEffective
+            r = []
+            if not a:
+                return r
+            if a & 3:
+                r.append("OWNER")
+            if a & 4:
+                r.append("DACL")
+            if a & 8:
+                r.append("SACL")
+            return r
+
+        attr_params["sDRightsEffective"] = {"lambda": testSDRights, "right": "WRITE"}
+    if right == "CHILD" or right == "ALL":
+        attr_params["allowedChildClassesEffective"] = {
+            "lambda": genericReturn,
+            "right": "CREATE_CHILD",
+        }
+
+    searchbases = []
+    # if partition == "DOMAIN":
+    searchbases.append(conn.ldap.domainNC)
+    # elif partition == "DNS":
+    #     searchbases.append(conn.ldap.applicationNCs) # A definir https://learn.microsoft.com/en-us/windows/win32/ad/enumerating-application-directory-partitions-in-a-forest
+    # else:
+    #     searchbases.append(conn.ldap.NCs) # A definir
+    right_entry = {}
+    for searchbase in searchbases:
+        for entry in conn.ldap.bloodysearch(
+            searchbase,
+            f"(objectClass={objectClass})",
+            search_scope=ldap3.SUBTREE,
+            attr=attr_params.keys(),
+            generator=True,
+        ):
+            for attr_name in entry:
+                if attr_name not in attr_params:
+                    continue
+                key_names = attr_params[attr_name]["lambda"](entry[attr_name])
+                for name in key_names:
+                    if name not in right_entry:
+                        right_entry[name] = []
+                    right_entry[name].append(attr_params[attr_name]["right"])
+
+            if right_entry:
+                yield {
+                    **{"distinguishedName": entry["distinguishedName"]},
+                    **right_entry,
+                }
+                right_entry = {}
```

### Comparing `bloodyAD-0.2.6/bloodyAD/exceptions.py` & `bloodyAD-1.0.0/bloodyAD/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,24 @@
 
 
 class ResultError(LDAPError):
     def __init__(self, result):
         self.result = result
 
         if self.result["result"] == 50:
-            self.message = "[-] Could not modify object, the server reports insufficient rights: " + self.result["message"]
+            self.message = (
+                "[-] Could not modify object, the server reports insufficient rights: "
+                + self.result["message"]
+            )
         elif self.result["result"] == 19:
-            self.message = "[-] Could not modify object, the server reports a constrained violation: " + self.result["message"]
+            self.message = (
+                "[-] Could not modify object, the server reports a constrained"
+                " violation: "
+                + self.result["message"]
+            )
         else:
             self.message = "[-] The server returned an error: " + self.result["message"]
 
         super().__init__(self.message)
 
 
 class NoResultError(LDAPError):
```

### Comparing `bloodyAD-0.2.6/bloodyAD/formatters/accesscontrol.py` & `bloodyAD-1.0.0/bloodyAD/formatters/accesscontrol.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 UNPROTECTED_DACL_SECURITY_INFORMATION = 0x20000000
 PROTECTED_SACL_SECURITY_INFORMATION = 0x40000000
 PROTECTED_DACL_SECURITY_INFORMATION = 0x80000000
 ATTRIBUTE_SECURITY_INFORMATION = 0x00000020
 SCOPE_SECURITY_INFORMATION = 0x00000040
 BACKUP_SECURITY_INFORMATION = 0x00010000
 
-# https://docs.microsoft.com/en-us/windows/win32/secauthz/access-rights-and-access-masks
+# https://docs.microsoft.com/en-us/windows/win32/api/iads/ne-iads-ads_rights_enum
 ACCESS_FLAGS = {
     # Flag constants
     "GENERIC_READ": 0x80000000,
     "GENERIC_WRITE": 0x40000000,
     "GENERIC_EXECUTE": 0x20000000,
     "GENERIC_ALL": 0x10000000,
     "MAXIMUM_ALLOWED": 0x02000000,
@@ -79,20 +79,14 @@
     "DONT_REQ_PREAUTH": 0x400000,
     "PASSWORD_EXPIRED": 0x800000,
     "TRUSTED_TO_AUTH_FOR_DELEGATION": 0x1000000,
     "PARTIAL_SECRETS_ACCOUNT": 0x04000000,
 }
 
 
-# https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/manage/understand-security-identifiers
-WELLKNOWN_DOMAIN_RID = {
-        513: "Domain Users"
-}
-
-
 @lru_cache
 def decodeAccessMask(mask):
     tmp_mask = [(key, val) for key, val in ACCESS_FLAGS.items() if mask.hasPriv(val)]
     pretty_mask = []
     for i in range(0, len(tmp_mask)):
         isDuplicate = False
         for j in range(i + 1, len(tmp_mask)):
```

### Comparing `bloodyAD-0.2.6/bloodyAD/formatters/cryptography.py` & `bloodyAD-1.0.0/bloodyAD/formatters/cryptography.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-0.2.6/bloodyAD/formatters/dns.py` & `bloodyAD-1.0.0/bloodyAD/formatters/dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             record_data.fromCanonical(data, port, priority, weight)
         elif dnstype == "TXT":
             record_data = DNS_RPC_RECORD_STRING()
             record_data.fromCanonical(data)
         else:
             raise TypeError(f"{dnstype} not supported")
 
-        self["Data"] = record_data
+        self["Data"] = record_data.getData()
 
 
 class DNS_RPC_RECORD_A(Structure):
     """
     DNS_RPC_RECORD_A - [MS-DNSP] section 2.2.2.2.4.1
     """
 
@@ -151,16 +151,16 @@
     def formatCanonical(self):
         ind = 0
         labels = []
         for i in range(self["LabelCount"]):
             nextlen = int.from_bytes(self["RawName"][ind : ind + 1], byteorder="big")
             labels.append(self["RawName"][ind + 1 : ind + 1 + nextlen].decode("utf-8"))
             ind += nextlen + 1
-        # For the final dot
-        labels.append("")
+        # For the final dot, but do we really want to display it?
+        # labels.append("")
         return ".".join(labels)
 
     def fromCanonical(self, canonical):
         # Removes empty strings
         labels = [label for label in canonical.split(".") if label]
         label_count = 0
         raw_name = b""
```

### Comparing `bloodyAD-0.2.6/bloodyAD/formatters/formatters.py` & `bloodyAD-1.0.0/bloodyAD/formatters/formatters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,28 @@
-import bloodyAD.patch.winacl_patch
 from bloodyAD.formatters import (
     accesscontrol,
     common,
     cryptography,
     dns,
-    ldaptypes,
-    helpers,
 )
-from bloodyAD import formatters
 import base64
 from winacl.dtyp.security_descriptor import SECURITY_DESCRIPTOR
 
-RESOLVING = False
 
 def formatAccountControl(userAccountControl):
     userAccountControl = int(userAccountControl.decode())
     return [
         key
         for key, val in accesscontrol.ACCOUNT_FLAGS.items()
         if userAccountControl & val == val
     ]
 
 
 def formatSD(sd_bytes):
-    if not RESOLVING:
-        return SECURITY_DESCRIPTOR.from_bytes(sd_bytes).to_sddl()
-
-    sd = ldaptypes.SR_SECURITY_DESCRIPTOR(data=sd_bytes)
-    pretty_sd = {}
-    if sd["OffsetOwner"] != 0:
-        pretty_sd["Owner"] = helpers.resolveSid(sd["OwnerSid"].formatCanonical())
-    if sd["OffsetGroup"] != 0:
-        pretty_sd["Group"] = helpers.resolveSid(sd["GroupSid"].formatCanonical())
-    if sd["OffsetSacl"] != 0:
-        pretty_sd["Sacl"] = base64.b64encode(sd["Sacl"].getData())
-    if sd["OffsetDacl"] != 0:
-        pretty_aces = []
-        for ace in sd["Dacl"].aces:
-            pretty_aces.append(accesscontrol.decodeAce(ace))
-        pretty_sd["Dacl"] = pretty_aces
-    return pretty_sd
+    return SECURITY_DESCRIPTOR.from_bytes(sd_bytes).to_sddl()
 
 
 def formatFunctionalLevel(behavior_version):
     behavior_version = behavior_version.decode()
     return (
         common.FUNCTIONAL_LEVEL[behavior_version]
         if behavior_version in common.FUNCTIONAL_LEVEL
@@ -59,18 +38,28 @@
         else objectVersion
     )
 
 
 def formatGMSApass(managedPassword):
     gmsa_blob = cryptography.MSDS_MANAGEDPASSWORD_BLOB(managedPassword)
     ntlm_hash = "aad3b435b51404eeaad3b435b51404ee:" + gmsa_blob.toNtHash()
-    return  f"NTLM {ntlm_hash} B64ENCODED {base64.b64encode(gmsa_blob['CurrentPassword'])}"
+    return {
+        "NTLM": ntlm_hash,
+        "B64ENCODED": base64.b64encode(gmsa_blob["CurrentPassword"]).decode(),
+    }
 
 
 def formatDnsRecord(dns_record):
     return dns.Record(dns_record).toDict()
 
 
+def formatWellKnownObjects(wellKnown_object):
+    dn_binary = common.DNBinary(wellKnown_object)
+    if dn_binary.binary_value in common.WELLKNOWN_GUID:
+        dn_binary.binary_value = common.WELLKNOWN_GUID[dn_binary.binary_value]
+    return dn_binary
+
+
 def formatKeyCredentialLink(key_dnbinary):
     return cryptography.KEYCREDENTIALLINK_BLOB(
         common.DNBinary(key_dnbinary).value
     ).toString()
```

### Comparing `bloodyAD-0.2.6/bloodyAD/formatters/helpers.py` & `bloodyAD-1.0.0/bloodyAD/formatters/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import uuid
 from functools import lru_cache
 
+# TODO change ldap_conn with conn.ldap and verify no formatting functions use ldap_conn (not a good pattern)
 ldap_conn = None
 
 
+@lru_cache
 def ldap_search(base_dn, filter, attr):
     try:
         if (
             not ldap_conn.search(base_dn, filter, attributes=attr)
             or not len(ldap_conn.entries)
             or attr not in ldap_conn.entries[0]
         ):
@@ -16,30 +18,34 @@
         return None
 
     return ldap_conn.entries[0][attr].value
 
 
 @lru_cache
 def resolveSid(sid):
+    # TODO: Get rid of search for wellknown security or merge it with one after
     r = ldap_search(
-        "CN=WellKnown Security"
-        f" Principals,{ldap_conn.server.info.other['configurationNamingContext'][0]}",
+        (
+            "CN=WellKnown Security"
+            f" Principals,{ldap_conn.server.info.other['configurationNamingContext'][0]}"
+        ),
         f"(objectSid={sid})",
         "name",
     )
     if r:
         return r
     r = ldap_search(
         ldap_conn.server.info.other["rootDomainNamingContext"][0],
         f"(objectSid={sid})",
         "sAMAccountName",
     )
     return r if r else sid
 
 
+@lru_cache
 def resolveGUID(guid_raw):
     attr = "name"
     guid_canonical = str(uuid.UUID(bytes_le=guid_raw))
     guid_str = "\\" + "\\".join(["{:02x}".format(b) for b in guid_raw])
     schema_dn = ldap_conn.server.info.other["schemaNamingContext"][0]
     r = ldap_search(
         f"CN=Extended-Rights,{ldap_conn.server.info.other['configurationNamingContext'][0]}",
@@ -49,8 +55,10 @@
     if not r:
         r = ldap_search(schema_dn, f"(schemaIDGUID={guid_str})", attr)
         return r if r else guid_canonical
     if not ldap_conn.search(
         schema_dn, f"(attributeSecurityGUID={guid_str})", attributes=attr
     ) or not len(ldap_conn.entries):
         return r
-    return {r: [entry[attr].value for entry in ldap_conn.entries]}
+    # TODO: return dict instead of str, functions calling it for str must transform it themselves
+    # return {r: [entry[attr].value for entry in ldap_conn.entries]}
+    return ",".join(sorted([entry[attr].value for entry in ldap_conn.entries]))
```

### Comparing `bloodyAD-0.2.6/bloodyAD/formatters/ldaptypes.py` & `bloodyAD-1.0.0/bloodyAD/formatters/ldaptypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # Global constant if the library should recalculate ACE sizes in objects that are decoded/re-encoded.
 # This defaults to True, but this causes the ACLs to not match on a binary level
 # since Active Directory for some reason sometimes adds null bytes to the end of ACEs.
 # This is valid according to the spec (see 2.4.4), but since impacket encodes them more efficiently
 # this should be turned off if running unit tests.
 RECALC_ACE_SIZE = True
 
+
 # LDAP SID structure - based on SAMR_RPC_SID, except the SubAuthority is LE here
 class LDAP_SID_IDENTIFIER_AUTHORITY(Structure):
     structure = (("Value", "6s"),)
 
 
 class LDAP_SID(Structure):
     structure = (
```

### Comparing `bloodyAD-0.2.6/bloodyAD/formatters/structure.py` & `bloodyAD-1.0.0/bloodyAD/formatters/structure.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-0.2.6/bloodyAD/md4.py` & `bloodyAD-1.0.0/bloodyAD/md4.py`

 * *Files identical despite different names*

### Comparing `bloodyAD-0.2.6/bloodyAD/patch/ldap3_patch.py` & `bloodyAD-1.0.0/bloodyAD/patch/ldap3_patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -216,128 +216,182 @@
                 )
             else:
                 log(BASIC, "instantiated Connection: <%r>", self)
 
 
 Connection.__init__ = __init__
 
-def bind(self,
-             read_server_info=True,
-             controls=None):
-        """Bind to ldap Server with the authentication method and the user defined in the connection
-        :param read_server_info: reads info from server
-        :param controls: LDAP controls to send along with the bind operation
-        :type controls: list of tuple
-        :return: bool
-        """
-        if log_enabled(BASIC):
-            log(BASIC, 'start BIND operation via <%s>', self)
-        self.last_error = None
-        with self.connection_lock:
-            if self.lazy and not self._executing_deferred:
-                if self.strategy.pooled:
-                    self.strategy.validate_bind(controls)
-                self._deferred_bind = True
-                self._bind_controls = controls
-                self.bound = True
-                if log_enabled(BASIC):
-                    log(BASIC, 'deferring bind for <%s>', self)
-            else:
-                self._deferred_bind = False
-                self._bind_controls = None
-                if self.closed:  # try to open connection if closed
-                    self.open(read_server_info=False)
-                if self.authentication == ANONYMOUS:
+
+def bind(self, read_server_info=True, controls=None):
+    """Bind to ldap Server with the authentication method and the user defined in the connection
+    :param read_server_info: reads info from server
+    :param controls: LDAP controls to send along with the bind operation
+    :type controls: list of tuple
+    :return: bool
+    """
+    if log_enabled(BASIC):
+        log(BASIC, "start BIND operation via <%s>", self)
+    self.last_error = None
+    with self.connection_lock:
+        if self.lazy and not self._executing_deferred:
+            if self.strategy.pooled:
+                self.strategy.validate_bind(controls)
+            self._deferred_bind = True
+            self._bind_controls = controls
+            self.bound = True
+            if log_enabled(BASIC):
+                log(BASIC, "deferring bind for <%s>", self)
+        else:
+            self._deferred_bind = False
+            self._bind_controls = None
+            if self.closed:  # try to open connection if closed
+                self.open(read_server_info=False)
+            if self.authentication == ANONYMOUS:
+                if log_enabled(PROTOCOL):
+                    log(PROTOCOL, "performing anonymous BIND for <%s>", self)
+                if not self.strategy.pooled:
+                    request = bind_operation(
+                        self.version,
+                        self.authentication,
+                        self.user,
+                        "",
+                        auto_encode=self.auto_encode,
+                    )
                     if log_enabled(PROTOCOL):
-                        log(PROTOCOL, 'performing anonymous BIND for <%s>', self)
-                    if not self.strategy.pooled:
-                        request = bind_operation(self.version, self.authentication, self.user, '', auto_encode=self.auto_encode)
-                        if log_enabled(PROTOCOL):
-                            log(PROTOCOL, 'anonymous BIND request <%s> sent via <%s>', bind_request_to_dict(request), self)
-                        response = self.post_send_single_response(self.send('bindRequest', request, controls))
-                    else:
-                        response = self.strategy.validate_bind(controls)  # only for REUSABLE
-                elif self.authentication == SIMPLE:
+                        log(
+                            PROTOCOL,
+                            "anonymous BIND request <%s> sent via <%s>",
+                            bind_request_to_dict(request),
+                            self,
+                        )
+                    response = self.post_send_single_response(
+                        self.send("bindRequest", request, controls)
+                    )
+                else:
+                    response = self.strategy.validate_bind(
+                        controls
+                    )  # only for REUSABLE
+            elif self.authentication == SIMPLE:
+                if log_enabled(PROTOCOL):
+                    log(PROTOCOL, "performing simple BIND for <%s>", self)
+                if not self.strategy.pooled:
+                    request = bind_operation(
+                        self.version,
+                        self.authentication,
+                        self.user,
+                        self.password,
+                        auto_encode=self.auto_encode,
+                    )
+                    if log_enabled(PROTOCOL):
+                        log(
+                            PROTOCOL,
+                            "simple BIND request <%s> sent via <%s>",
+                            bind_request_to_dict(request),
+                            self,
+                        )
+                    response = self.post_send_single_response(
+                        self.send("bindRequest", request, controls)
+                    )
+                else:
+                    response = self.strategy.validate_bind(
+                        controls
+                    )  # only for REUSABLE
+            elif self.authentication == SASL:
+                if self.sasl_mechanism in SASL_AVAILABLE_MECHANISMS:
                     if log_enabled(PROTOCOL):
-                        log(PROTOCOL, 'performing simple BIND for <%s>', self)
+                        log(PROTOCOL, "performing SASL BIND for <%s>", self)
                     if not self.strategy.pooled:
-                        request = bind_operation(self.version, self.authentication, self.user, self.password, auto_encode=self.auto_encode)
-                        if log_enabled(PROTOCOL):
-                            log(PROTOCOL, 'simple BIND request <%s> sent via <%s>', bind_request_to_dict(request), self)
-                        response = self.post_send_single_response(self.send('bindRequest', request, controls))
+                        response = self.do_sasl_bind(controls)
                     else:
-                        response = self.strategy.validate_bind(controls)  # only for REUSABLE
-                elif self.authentication == SASL:
-                    if self.sasl_mechanism in SASL_AVAILABLE_MECHANISMS:
-                        if log_enabled(PROTOCOL):
-                            log(PROTOCOL, 'performing SASL BIND for <%s>', self)
-                        if not self.strategy.pooled:
-                            response = self.do_sasl_bind(controls)
-                        else:
-                            response = self.strategy.validate_bind(controls)  # only for REUSABLE
-                    else:
-                        self.last_error = 'requested SASL mechanism not supported'
-                        if log_enabled(ERROR):
-                            log(ERROR, '%s for <%s>', self.last_error, self)
-                        raise LDAPSASLMechanismNotSupportedError(self.last_error)
-                elif self.authentication == NTLM:
-                    if self.user and self.password is not None and len(self.user.split('\\')) == 2:
-                        if log_enabled(PROTOCOL):
-                            log(PROTOCOL, 'performing NTLM BIND for <%s>', self)
-                        if not self.strategy.pooled:
-                            response = self.do_ntlm_bind(controls)
-                        else:
-                            response = self.strategy.validate_bind(controls)  # only for REUSABLE
-                    else:  # user or password missing
-                        self.last_error = 'NTLM needs domain\\username and a password'
-                        if log_enabled(ERROR):
-                            log(ERROR, '%s for <%s>', self.last_error, self)
-                        raise LDAPUnknownAuthenticationMethodError(self.last_error)
+                        response = self.strategy.validate_bind(
+                            controls
+                        )  # only for REUSABLE
                 else:
-                    self.last_error = 'unknown authentication method'
+                    self.last_error = "requested SASL mechanism not supported"
                     if log_enabled(ERROR):
-                        log(ERROR, '%s for <%s>', self.last_error, self)
-                    raise LDAPUnknownAuthenticationMethodError(self.last_error)
-
-                if not self.strategy.sync and not self.strategy.pooled and self.authentication not in (SASL, NTLM):  # get response if asynchronous except for SASL and NTLM that return the bind result even for asynchronous strategy
-                    _, result = self.get_response(response)
+                        log(ERROR, "%s for <%s>", self.last_error, self)
+                    raise LDAPSASLMechanismNotSupportedError(self.last_error)
+            elif self.authentication == NTLM:
+                if (
+                    self.user
+                    and self.password is not None
+                    and len(self.user.split("\\")) == 2
+                ):
                     if log_enabled(PROTOCOL):
-                        log(PROTOCOL, 'async BIND response id <%s> received via <%s>', result, self)
-                elif self.strategy.sync:
-                    result = self.result
-                    if log_enabled(PROTOCOL):
-                        log(PROTOCOL, 'BIND response <%s> received via <%s>', result, self)
-                elif self.strategy.pooled or self.authentication in (SASL, NTLM):  # asynchronous SASL and NTLM or reusable strtegy get the bind result synchronously
-                    result = response
-                else:
-                    self.last_error = 'unknown authentication method'
+                        log(PROTOCOL, "performing NTLM BIND for <%s>", self)
+                    if not self.strategy.pooled:
+                        response = self.do_ntlm_bind(controls)
+                    else:
+                        response = self.strategy.validate_bind(
+                            controls
+                        )  # only for REUSABLE
+                else:  # user or password missing
+                    self.last_error = "NTLM needs domain\\username and a password"
                     if log_enabled(ERROR):
-                        log(ERROR, '%s for <%s>', self.last_error, self)
+                        log(ERROR, "%s for <%s>", self.last_error, self)
                     raise LDAPUnknownAuthenticationMethodError(self.last_error)
+            else:
+                self.last_error = "unknown authentication method"
+                if log_enabled(ERROR):
+                    log(ERROR, "%s for <%s>", self.last_error, self)
+                raise LDAPUnknownAuthenticationMethodError(self.last_error)
+
+            if (
+                not self.strategy.sync
+                and not self.strategy.pooled
+                and self.authentication not in (SASL, NTLM)
+            ):  # get response if asynchronous except for SASL and NTLM that return the bind result even for asynchronous strategy
+                _, result = self.get_response(response)
+                if log_enabled(PROTOCOL):
+                    log(
+                        PROTOCOL,
+                        "async BIND response id <%s> received via <%s>",
+                        result,
+                        self,
+                    )
+            elif self.strategy.sync:
+                result = self.result
+                if log_enabled(PROTOCOL):
+                    log(PROTOCOL, "BIND response <%s> received via <%s>", result, self)
+            elif self.strategy.pooled or self.authentication in (
+                SASL,
+                NTLM,
+            ):  # asynchronous SASL and NTLM or reusable strtegy get the bind result synchronously
+                result = response
+            else:
+                self.last_error = "unknown authentication method"
+                if log_enabled(ERROR):
+                    log(ERROR, "%s for <%s>", self.last_error, self)
+                raise LDAPUnknownAuthenticationMethodError(self.last_error)
+
+            if result is None:
+                # self.bound = True if self.strategy_type == REUSABLE else False
+                self.bound = False
+            elif result is True:
+                self.bound = True
+            elif result is False:
+                self.bound = False
+            else:
+                self.bound = True if result["result"] == RESULT_SUCCESS else False
+                if (
+                    not self.bound
+                    and result
+                    and result["description"]
+                    and not self.last_error
+                ):
+                    self.last_error = result["description"]
+
+            if read_server_info and self.bound:
+                self.refresh_server_info()
+        self._entries = []
 
-                if result is None:
-                    # self.bound = True if self.strategy_type == REUSABLE else False
-                    self.bound = False
-                elif result is True:
-                    self.bound = True
-                elif result is False:
-                    self.bound = False
-                else:
-                    self.bound = True if result['result'] == RESULT_SUCCESS else False
-                    if not self.bound and result and result['description'] and not self.last_error:
-                        self.last_error = result['description']
-
-                if read_server_info and self.bound:
-                    self.refresh_server_info()
-            self._entries = []
-
-            if log_enabled(BASIC):
-                log(BASIC, 'done BIND operation, result <%s>', self.bound)
+        if log_enabled(BASIC):
+            log(BASIC, "done BIND operation, result <%s>", self.bound)
 
-            return self._prepare_return_value(self.bound, self.result)
+        return self._prepare_return_value(self.bound, self.result)
 
 
 Connection.bind = bind
 
 
 def do_ntlm_bind(self, controls):
     if log_enabled(BASIC):
@@ -396,16 +450,18 @@
                         )
                         if not self.strategy.sync:
                             _, result = self.get_response(response)
                         else:
                             if log_enabled(PROTOCOL):
                                 log(
                                     PROTOCOL,
-                                    "NTLM SICILY NEGOTIATE response <%s>"
-                                    " received via <%s>",
+                                    (
+                                        "NTLM SICILY NEGOTIATE response <%s>"
+                                        " received via <%s>"
+                                    ),
                                     response[0],
                                     self,
                                 )
                             result = response[0]
 
                         if result["result"] == RESULT_SUCCESS:
                             request = bind_operation(
```

### Comparing `bloodyAD-0.2.6/bloodyAD.egg-info/PKG-INFO` & `bloodyAD-1.0.0/bloodyAD.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bloodyAD
-Version: 0.2.6
+Version: 1.0.0
 Summary: AD Privesc Swiss Army Knife
 Home-page: https://github.com/CravateRouge/bloodyAD
-Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v0.2.6.tar.gz
+Download-URL: https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.0.tar.gz
 Author: CravateRouge
 Author-email: baptiste.crepin@ntymail.com
 License: MIT
 Keywords: Active Directory,Privilege Escalation
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -49,23 +49,23 @@
 pacman -S krb5
 ```
 
 A python package is available:
 
 ```ps1
 pip install bloodyAD
-bloodyAD --host 172.16.1.15 -d bloody.local -k changePassword john.doe 'Password123!'
+bloodyAD --host 172.16.1.15 -d bloody.local -k set password john.doe 'Password123!'
 ```
 
 Or you can clone the repo:
 
 ```ps1
 git clone --depth 1 https://github.com/CravateRouge/bloodyAD
 pip install .
-bloodyAD --host 172.16.1.15 -d bloody.local -k changePassword john.doe 'Password123!'
+bloodyAD --host 172.16.1.15 -d bloody.local -k set password john.doe 'Password123!'
 ```
 
 ### Dependencies
 
 - Python 3
 - DSinternals
 - Impacket
@@ -73,15 +73,15 @@
 - Gssapi (linux) or Winkerberos (Windows)
 
 ## Usage
 
 Simple usage:
 
 ```ps1
-bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 changePassword john.doe 'Password123!'
+bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 set password john.doe 'Password123!'
 ```
 
 **Note:** You can find more examples on <https://cravaterouge.github.io/> and in the documentation folder of this project
 
 List of all available functions:
 
 ```ps1
@@ -111,81 +111,77 @@
     get                 [GET] function category
     remove              [REMOVE] function category
 ```
 
 Help text to use a specific function:
 
 ```ps1
-[bloodyAD]$ bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 changePassword -h
-usage: 
-    Change the target password without knowing the old one using LDAPS or RPC
-    Args:
-        identity: sAMAccountName, DN, GUID or SID of the target (You must have write permission on it)
-        new_pass: new password for the target
-    
-       [-h] [func_args ...]
+[bloodyAD]$ bloodyAD --host 172.16.1.15 -d bloody.local -u jane.doe -p :70016778cb0524c799ac25b439bd6a31 set password -h
+usage: bloodyAD.py set password [-h] [--oldpass OLDPASS] target newpass
 
 positional arguments:
-  func_args
+  target             sAMAccountName, DN, GUID or SID of the target
+  newpass            new password for the target
 
-optional arguments:
-  -h, --help  show this help message and exit
+options:
+  -h, --help         show this help message and exit
+  --oldpass OLDPASS  old password of the target, mandatory if you don't have "change password" permission on the target (default: None)
   ```
 
 ## How it works
 
 bloodyAD communicates with a DC using mainly the LDAP protocol in order to get information or add/modify/delete AD objects. ~~A password cannot be updated with LDAP, it must be a secure connection that is LDAPS or SAMR. A DC doesn't have LDAPS activated by default because it must be configured (with a certificate) so SAMR is used in those cases.~~ Exchange of sensitive information such as passwords are now supported using cleartext LDAP.
 
 ## Useful commands
 
 ```ps1
 # Get group members
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes Users member 
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get object Users --attr member 
 
 # Get minimum password length policy
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes 'DC=bloody,DC=local' minPwdLength
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get object 'DC=bloody,DC=local' --attr minPwdLength
 
 # Get AD functional level
-bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes 'DC=bloody,DC=local' msDS-Behavior-Version
+bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 get object 'DC=bloody,DC=local' --attr msDS-Behavior-Version
 
 # Get all users of the domain
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getChildObjects 'DC=bloody,DC=local' user
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get children 'DC=bloody,DC=local' --type user
 
 # Get all computers of the domain
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getChildObjects 'DC=bloody,DC=local' computer
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get children 'DC=bloody,DC=local' --type computer
 
 # Get all containers of the domain
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getChildObjects 'DC=bloody,DC=local' container
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get children 'DC=bloody,DC=local' --type container
 
 # Enable DONT_REQ_PREAUTH for ASREPRoast
-bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 setUserAccountControl john.doe 0x400000
+bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 add uac john.doe DONT_REQ_PREAUTH
 
 # Disable ACCOUNTDISABLE
-bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 setUserAccountControl john.doe 0x0002 False
+bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 remove uac john.doe ACCOUNTDISABLE
 
 # Get UserAccountControl flags
-bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes john.doe userAccountControl
+bloodyAD -u Administrator -d bloody -p Password512! --host 192.168.10.2 get object john.doe --attr userAccountControl
 
 # Read GMSA account password
-bloodyAD -u john.doe -d bloody -p Password512 --host 192.168.10.2 getObjectAttributes gmsaAccount$ msDS-ManagedPassword
+bloodyAD -u john.doe -d bloody -p Password512 --host 192.168.10.2 get object 'gmsaAccount$' --attr msDS-ManagedPassword
 
 # Read LAPS password
-bloodyAD -u john.doe -d bloody -p Password512 --host 192.168.10.2 getObjectAttributes COMPUTER$ ms-Mcs-AdmPwd
+bloodyAD -u john.doe -d bloody -p Password512 --host 192.168.10.2 get object 'COMPUTER$' --attr ms-Mcs-AdmPwd
 
 # Read quota for adding computer objects to domain
-bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 getObjectAttributes 'DC=bloody,DC=local' ms-DS-MachineAccountQuota
+bloodyAD -u john.doe -d bloody -p Password512! --host 192.168.10.2 get object 'DC=bloody,DC=local' --attr ms-DS-MachineAccountQuota
 
 # Add a new DNS entry
-bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 add domainDNSRecord my_machine_name 192.168.10.48
+bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 add dnsRecord my_machine_name 192.168.10.48
 
 # Remove a DNS entry
-bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 remove domainDNSRecord my_machine_name 192.168.10.48
+bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 remove dnsRecord my_machine_name 192.168.10.48
 
 # Get AD DNS records
-bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 get domainDNSRecord
+bloodyAD -u stan.dard -p Password123! -d bloody.local --host 192.168.10.2 get dnsDump
 
 ```
 
 ## Acknowledgements
 - Thanks to [impacket](https://github.com/fortra/impacket) contributors. [Structures](https://github.com/fortra/impacket/blob/master/impacket/structure.py) and several [LDAP attacks](https://github.com/fortra/impacket/blob/master/impacket/examples/ntlmrelayx/attacks/ldapattack.py) are based on their work.
 - Thanks to [@PowerShellMafia](https://github.com/PowerShellMafia) team ([PowerView.ps1](https://github.com/PowerShellMafia/PowerSploit/blob/master/Recon/PowerView.ps1)) and their work on AD which inspired this tool.
 - Thanks to [@dirkjanm](https://github.com/dirkjanm) ([adidnsdump.py](https://github.com/dirkjanm/adidnsdump)) and ([@Kevin-Robertson](https://github.com/Kevin-Robertson))([Invoke-DNSUpdate.ps1](https://github.com/Kevin-Robertson/Powermad/blob/master/Invoke-DNSUpdate.ps1)) for their work on AD DNS which inspired DNS functionnalities.
```

### Comparing `bloodyAD-0.2.6/bloodyAD.egg-info/SOURCES.txt` & `bloodyAD-1.0.0/bloodyAD.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 LICENSE
 README.md
 setup.py
 bloodyAD/__init__.py
-bloodyAD/config.py
 bloodyAD/exceptions.py
 bloodyAD/main.py
 bloodyAD/md4.py
-bloodyAD/modules.py
 bloodyAD/utils.py
 bloodyAD.egg-info/PKG-INFO
 bloodyAD.egg-info/SOURCES.txt
 bloodyAD.egg-info/dependency_links.txt
 bloodyAD.egg-info/entry_points.txt
 bloodyAD.egg-info/requires.txt
 bloodyAD.egg-info/top_level.txt
 bloodyAD/cli_modules/__init__.py
 bloodyAD/cli_modules/add.py
 bloodyAD/cli_modules/get.py
 bloodyAD/cli_modules/remove.py
 bloodyAD/cli_modules/set.py
 bloodyAD/formatters/__init__.py
 bloodyAD/formatters/accesscontrol.py
+bloodyAD/formatters/adschema.py
 bloodyAD/formatters/common.py
 bloodyAD/formatters/cryptography.py
 bloodyAD/formatters/dns.py
 bloodyAD/formatters/formatters.py
 bloodyAD/formatters/helpers.py
 bloodyAD/formatters/ldaptypes.py
 bloodyAD/formatters/structure.py
 bloodyAD/formatters/winerror.py
-bloodyAD/patch/ldap3_patch.py
-bloodyAD/patch/winacl_patch.py
+bloodyAD/network/config.py
+bloodyAD/network/ldap.py
+bloodyAD/patch/ldap3_patch.py
```

### Comparing `bloodyAD-0.2.6/setup.py` & `bloodyAD-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="bloodyAD",
-    version="0.2.6",
+    version="1.0.0",
     description="AD Privesc Swiss Army Knife",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="CravateRouge",
     author_email="baptiste.crepin@ntymail.com",
     url="https://github.com/CravateRouge/bloodyAD",
     download_url=(
-        "https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v0.2.6.tar.gz"
+        "https://github.com/CravateRouge/bloodyAD/archive/refs/tags/v1.0.0.tar.gz"
     ),
     license="MIT",
     install_requires=[
         "cryptography>=37.0.2",
         "ldap3>=2.9.1",
-        "winacl>=0.1.6",
+        "winacl>=0.1.7",
         'gssapi>=1.8.1 ; platform_system=="Linux" or platform_system=="Darwin"',
         'winkerberos>=0.9.0; platform_system=="Windows"',
+        "pyasn1>=0.4.8",
     ],
     keywords=["Active Directory", "Privilege Escalation"],
     classifiers=[
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

