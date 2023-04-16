# Comparing `tmp/cc-ibet-2.1.4.tar.gz` & `tmp/cc-ibet-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc-ibet-2.1.4.tar", last modified: Fri Mar 31 15:29:13 2023, max compression
+gzip compressed data, was "cc-ibet-2.1.5.tar", last modified: Sun Apr 16 14:47:18 2023, max compression
```

## Comparing `cc-ibet-2.1.4.tar` & `cc-ibet-2.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-03-31 15:29:13.529731 cc-ibet-2.1.4/
--rw-r--r--   0 namle      (501) staff       (20)      289 2023-03-31 15:29:13.529807 cc-ibet-2.1.4/PKG-INFO
--rw-r--r--   0 namle      (501) staff       (20)      109 2023-02-07 08:22:49.000000 cc-ibet-2.1.4/README.md
-drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-03-31 15:29:13.528244 cc-ibet-2.1.4/cc_ibet.egg-info/
--rw-r--r--   0 namle      (501) staff       (20)      289 2023-03-31 15:29:13.000000 cc-ibet-2.1.4/cc_ibet.egg-info/PKG-INFO
--rw-r--r--   0 namle      (501) staff       (20)      265 2023-03-31 15:29:13.000000 cc-ibet-2.1.4/cc_ibet.egg-info/SOURCES.txt
--rw-r--r--   0 namle      (501) staff       (20)        1 2023-03-31 15:29:13.000000 cc-ibet-2.1.4/cc_ibet.egg-info/dependency_links.txt
--rw-r--r--   0 namle      (501) staff       (20)       51 2023-03-31 15:29:13.000000 cc-ibet-2.1.4/cc_ibet.egg-info/requires.txt
--rw-r--r--   0 namle      (501) staff       (20)        5 2023-03-31 15:29:13.000000 cc-ibet-2.1.4/cc_ibet.egg-info/top_level.txt
-drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-03-31 15:29:13.529519 cc-ibet-2.1.4/ibet/
--rw-r--r--   0 namle      (501) staff       (20)       90 2023-02-23 03:25:34.000000 cc-ibet-2.1.4/ibet/__init__.py
--rw-r--r--   0 namle      (501) staff       (20)    20536 2023-03-31 15:28:26.000000 cc-ibet-2.1.4/ibet/client.py
--rw-r--r--   0 namle      (501) staff       (20)      155 2023-02-07 10:14:14.000000 cc-ibet-2.1.4/ibet/exceptions.py
--rw-r--r--   0 namle      (501) staff       (20)      884 2023-03-31 15:13:13.000000 cc-ibet-2.1.4/ibet/settings.py
--rw-r--r--   0 namle      (501) staff       (20)       94 2023-02-07 08:22:49.000000 cc-ibet-2.1.4/pyproject.toml
--rw-r--r--   0 namle      (501) staff       (20)      400 2023-03-31 15:29:13.530066 cc-ibet-2.1.4/setup.cfg
--rw-r--r--   0 namle      (501) staff       (20)       52 2023-02-07 08:22:49.000000 cc-ibet-2.1.4/setup.py
+drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-04-16 14:47:18.532144 cc-ibet-2.1.5/
+-rw-r--r--   0 namle      (501) staff       (20)      289 2023-04-16 14:47:18.532221 cc-ibet-2.1.5/PKG-INFO
+-rw-r--r--   0 namle      (501) staff       (20)      109 2023-02-07 08:22:49.000000 cc-ibet-2.1.5/README.md
+drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-04-16 14:47:18.530866 cc-ibet-2.1.5/cc_ibet.egg-info/
+-rw-r--r--   0 namle      (501) staff       (20)      289 2023-04-16 14:47:18.000000 cc-ibet-2.1.5/cc_ibet.egg-info/PKG-INFO
+-rw-r--r--   0 namle      (501) staff       (20)      265 2023-04-16 14:47:18.000000 cc-ibet-2.1.5/cc_ibet.egg-info/SOURCES.txt
+-rw-r--r--   0 namle      (501) staff       (20)        1 2023-04-16 14:47:18.000000 cc-ibet-2.1.5/cc_ibet.egg-info/dependency_links.txt
+-rw-r--r--   0 namle      (501) staff       (20)       51 2023-04-16 14:47:18.000000 cc-ibet-2.1.5/cc_ibet.egg-info/requires.txt
+-rw-r--r--   0 namle      (501) staff       (20)        5 2023-04-16 14:47:18.000000 cc-ibet-2.1.5/cc_ibet.egg-info/top_level.txt
+drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-04-16 14:47:18.531931 cc-ibet-2.1.5/ibet/
+-rw-r--r--   0 namle      (501) staff       (20)       90 2023-02-23 03:25:34.000000 cc-ibet-2.1.5/ibet/__init__.py
+-rw-r--r--   0 namle      (501) staff       (20)    21304 2023-03-31 16:35:41.000000 cc-ibet-2.1.5/ibet/client.py
+-rw-r--r--   0 namle      (501) staff       (20)      155 2023-02-07 10:14:14.000000 cc-ibet-2.1.5/ibet/exceptions.py
+-rw-r--r--   0 namle      (501) staff       (20)      884 2023-03-31 15:13:13.000000 cc-ibet-2.1.5/ibet/settings.py
+-rw-r--r--   0 namle      (501) staff       (20)       94 2023-02-07 08:22:49.000000 cc-ibet-2.1.5/pyproject.toml
+-rw-r--r--   0 namle      (501) staff       (20)      400 2023-04-16 14:47:18.532461 cc-ibet-2.1.5/setup.cfg
+-rw-r--r--   0 namle      (501) staff       (20)       52 2023-02-07 08:22:49.000000 cc-ibet-2.1.5/setup.py
```

### Comparing `cc-ibet-2.1.4/ibet/client.py` & `cc-ibet-2.1.5/ibet/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,34 +158,39 @@
         self.random_ip()
         self._second_auth = None
 
         cookies = {
             'ASP.NET_SessionId': self.random_string(24),
             # 'ASP.NET_SessionId': 'nvlo4qjixbvynsdcesmoduep',
             '__RequestVerificationToken': '3Uk-fAGF7xXzlqhMBT8LErm5yXC2whG7guulHL-zPuesaBxxsB-IWg6ueIqPlnB0b8pS7UxWcOTJMcuAD3ECcyLYNtg1',
-            '.AspNetCore.Antiforgery.WDFpV_iIKZQ': 'CfDJ8By69Ukru-hPigpz_UzW9QA-zstDg28eeUcPavF6U9cKWfWLWfP9-9kd3QblpNaVQySxhzCXHNkBWdK-_PFXnkrjqSKtmCNe2Qnmu4VBSDA8YrD6MzcHVy3Jv0_WFevfnDGQELWvQcxXXx4BtTd1iuw'
+            '.AspNetCore.Antiforgery.WDFpV_iIKZQ': 'CfDJ8By69Ukru-hPigpz_UzW9QA-zstDg28eeUcPavF6U9cKWfWLWfP9-9kd3QblpNaVQySxhzCXHNkBWdK-_PFXnkrjqSKtmCNe2Qnmu4VBSDA8YrD6MzcHVy3Jv0_WFevfnDGQELWvQcxXXx4BtTd1iuw',
         }
 
         # r = self.get(self._url())
         # print(r.text)
 
         self.cookies = cookiejar_from_dict(cookies)
 
         login_data = self.login_form_data()
 
         r = self.post(self._url(), data=login_data, headers={
             'Content-Type': 'application/x-www-form-urlencoded',
             'referer': self._url(),
-            # 'Cookie': 'ASP.NET_SessionId=nvlo4qjixbvynsdcesmoduep; __RequestVerificationToken=3Uk-fAGF7xXzlqhMBT8LErm5yXC2whG7guulHL-zPuesaBxxsB-IWg6ueIqPlnB0b8pS7UxWcOTJMcuAD3ECcyLYNtg1; .AspNetCore.Antiforgery.WDFpV_iIKZQ=CfDJ8By69Ukru-hPigpz_UzW9QA-zstDg28eeUcPavF6U9cKWfWLWfP9-9kd3QblpNaVQySxhzCXHNkBWdK-_PFXnkrjqSKtmCNe2Qnmu4VBSDA8YrD6MzcHVy3Jv0_WFevfnDGQELWvQcxXXx4BtTd1iuw;'
+            'Cookie': 'ASP.NET_SessionId=nvlo4qjixbvynsdcesmoduep; __RequestVerificationToken=3Uk-fAGF7xXzlqhMBT8LErm5yXC2whG7guulHL-zPuesaBxxsB-IWg6ueIqPlnB0b8pS7UxWcOTJMcuAD3ECcyLYNtg1; _ga=GA1.1.566909788.1673076115; hidLanguage=en-US; LANGUAGE=en-US; .AspNetCore.Antiforgery.WDFpV_iIKZQ=CfDJ8By69Ukru-hPigpz_UzW9QA-zstDg28eeUcPavF6U9cKWfWLWfP9-9kd3QblpNaVQySxhzCXHNkBWdK-_PFXnkrjqSKtmCNe2Qnmu4VBSDA8YrD6MzcHVy3Jv0_WFevfnDGQELWvQcxXXx4BtTd1iuw; .AspNetCore.Session=CfDJ8By69Ukru+hPigpz/UzW9QC07+3IX+BJF9yYB6zzUj61dy7A+U+Ne1qJ4O7Ndm5ppLOFywACaBfhb2XyEOkC7YktHl00nYsJoRHFrdy1vrTUi94qbpK21vR0yNpCGxwx0ObzN39jmpQBjikAS+65bmmu7kd0/WmNz1wuht+q5OjZ; dct=9bf4f631d9582a91a2cd73564839292a; cf_clearance=dDp.s0qRDDoZ_2_RCcuH957Uv7cQjpaUMr2zZuyFdkA-1680279053-0-160; __asct=08db3203cad387a33Lbzt09REgKFeLrcMr+iapafK0k=; _ga_SP8H2QTQ14=GS1.1.1680278206.10.1.1680279774.0.0.0; __utms=5A68CBC3880DB831B987C268072873; lip=wrrCtcKUwoTClcKDwo7Dl8Ktw7/CksO2B8OOwovClsO4ZG0Aw5jCn8O0w6XDvkwFNlnDtxzCuRxjZsO3wpDDn2kKw53DskvCiEh/T8OYUcOz'
         }, hooks={
             'response': [self.login_error, self.first_login]
         })
 
+        print(r.url)
+
         self.session_domain = r.url
 
+        if r.status_code == 403 and 'Just a moment...' in r.text:
+            raise Exception('Cloudflare')
+
         if '/Common/Error' in r.url:
             # FIXME
             print(r.text)
             raise Exception('Common error')
 
         if 'RobotCaptcha/Index' in r.url:
             # FIXME
```

### Comparing `cc-ibet-2.1.4/ibet/settings.py` & `cc-ibet-2.1.5/ibet/settings.py`

 * *Files identical despite different names*

