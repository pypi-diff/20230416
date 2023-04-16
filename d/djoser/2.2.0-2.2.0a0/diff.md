# Comparing `tmp/djoser-2.2.0.tar.gz` & `tmp/djoser-2.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djoser-2.2.0.tar", max compression
+gzip compressed data, was "djoser-2.2.0a0.tar", max compression
```

## Comparing `djoser-2.2.0.tar` & `djoser-2.2.0a0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1083 2023-04-02 09:37:37.622141 djoser-2.2.0/LICENSE
--rw-r--r--   0        0        0     4006 2023-04-02 12:22:03.336409 djoser-2.2.0/README.rst
--rw-r--r--   0        0        0       50 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/.codacy.yml
--rw-r--r--   0        0        0       22 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/__init__.py
--rw-r--r--   0        0        0      267 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/compat.py
--rw-r--r--   0        0        0     6972 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/conf.py
--rw-r--r--   0        0        0      720 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/constants.py
--rw-r--r--   0        0        0     1861 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/email.py
--rw-r--r--   0        0        0     3172 2023-04-16 11:40:20.430515 djoser-2.2.0/djoser/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4769 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3635 2023-04-16 11:40:20.434515 djoser-2.2.0/djoser/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6993 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3863 2023-04-16 11:40:20.434515 djoser-2.2.0/djoser/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6811 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3330 2023-04-16 11:40:20.438515 djoser-2.2.0/djoser/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5119 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4523 2023-04-16 11:40:20.438515 djoser-2.2.0/djoser/locale/ka/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6034 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/locale/ka/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1798 2023-04-16 11:40:20.442515 djoser-2.2.0/djoser/locale/me/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4076 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/locale/me/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3163 2023-04-16 11:40:20.434515 djoser-2.2.0/djoser/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4995 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3052 2023-04-16 11:40:20.438515 djoser-2.2.0/djoser/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4845 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4216 2023-04-16 11:40:20.442515 djoser-2.2.0/djoser/locale/ru_RU/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6151 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/locale/ru_RU/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      574 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/permissions.py
--rw-r--r--   0        0        0    11180 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/serializers.py
--rw-r--r--   0        0        0      271 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/signals.py
--rw-r--r--   0        0        0        0 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/social/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/social/backends/__init__.py
--rw-r--r--   0        0        0      132 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/social/backends/facebook.py
--rw-r--r--   0        0        0     2014 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/social/serializers.py
--rw-r--r--   0        0        0        0 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/social/token/__init__.py
--rw-r--r--   0        0        0      316 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/social/token/jwt.py
--rw-r--r--   0        0        0      210 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/social/urls.py
--rw-r--r--   0        0        0     1099 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/social/views.py
--rw-r--r--   0        0        0     1014 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/templates/email/activation.html
--rw-r--r--   0        0        0      616 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/templates/email/confirmation.html
--rw-r--r--   0        0        0      565 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/templates/email/password_changed_confirmation.html
--rw-r--r--   0        0        0     1216 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/templates/email/password_reset.html
--rw-r--r--   0        0        0      565 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/templates/email/username_changed_confirmation.html
--rw-r--r--   0        0        0     1216 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/templates/email/username_reset.html
--rw-r--r--   0        0        0       57 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/urls/__init__.py
--rw-r--r--   0        0        0      240 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/urls/authtoken.py
--rw-r--r--   0        0        0      244 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/urls/base.py
--rw-r--r--   0        0        0      350 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/urls/jwt.py
--rw-r--r--   0        0        0     1188 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/utils.py
--rw-r--r--   0        0        0    12862 2023-04-02 10:52:38.779937 djoser-2.2.0/djoser/views.py
--rw-r--r--   0        0        0        0 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/webauthn/__init__.py
--rw-r--r--   0        0        0       98 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/webauthn/apps.py
--rw-r--r--   0        0        0     1471 2023-04-02 10:52:38.759938 djoser-2.2.0/djoser/webauthn/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/webauthn/migrations/__init__.py
--rw-r--r--   0        0        0      554 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/webauthn/models.py
--rw-r--r--   0        0        0     2050 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/webauthn/serializers.py
--rw-r--r--   0        0        0      517 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/webauthn/urls.py
--rw-r--r--   0        0        0      293 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/webauthn/utils.py
--rw-r--r--   0        0        0     5687 2023-04-02 09:37:37.622141 djoser-2.2.0/djoser/webauthn/views.py
--rw-r--r--   0        0        0     2956 2023-04-16 11:15:02.303560 djoser-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     5684 1970-01-01 00:00:00.000000 djoser-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-02 09:37:37.622141 djoser-2.2.0a0/LICENSE
+-rw-r--r--   0        0        0     4006 2023-04-02 12:22:03.336409 djoser-2.2.0a0/README.rst
+-rw-r--r--   0        0        0       50 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/.codacy.yml
+-rw-r--r--   0        0        0       22 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/__init__.py
+-rw-r--r--   0        0        0      267 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/compat.py
+-rw-r--r--   0        0        0     6972 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/conf.py
+-rw-r--r--   0        0        0      720 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/constants.py
+-rw-r--r--   0        0        0     1861 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/email.py
+-rw-r--r--   0        0        0     3172 2023-04-02 12:51:50.009423 djoser-2.2.0a0/djoser/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4769 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3635 2023-04-02 12:51:50.013423 djoser-2.2.0a0/djoser/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6993 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3863 2023-04-02 12:51:50.013423 djoser-2.2.0a0/djoser/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6811 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3330 2023-04-02 12:51:50.013423 djoser-2.2.0a0/djoser/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5119 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4523 2023-04-02 12:51:50.017423 djoser-2.2.0a0/djoser/locale/ka/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6034 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/locale/ka/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1798 2023-04-02 12:51:50.021423 djoser-2.2.0a0/djoser/locale/me/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4076 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/locale/me/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3163 2023-04-02 12:51:50.013423 djoser-2.2.0a0/djoser/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4995 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3052 2023-04-02 12:51:50.017423 djoser-2.2.0a0/djoser/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4845 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4216 2023-04-02 12:51:50.021423 djoser-2.2.0a0/djoser/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6151 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/locale/ru_RU/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      574 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/permissions.py
+-rw-r--r--   0        0        0    11180 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/serializers.py
+-rw-r--r--   0        0        0      271 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/signals.py
+-rw-r--r--   0        0        0        0 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/social/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/social/backends/__init__.py
+-rw-r--r--   0        0        0      132 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/social/backends/facebook.py
+-rw-r--r--   0        0        0     2014 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/social/serializers.py
+-rw-r--r--   0        0        0        0 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/social/token/__init__.py
+-rw-r--r--   0        0        0      316 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/social/token/jwt.py
+-rw-r--r--   0        0        0      210 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/social/urls.py
+-rw-r--r--   0        0        0     1099 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/social/views.py
+-rw-r--r--   0        0        0     1014 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/templates/email/activation.html
+-rw-r--r--   0        0        0      616 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/templates/email/confirmation.html
+-rw-r--r--   0        0        0      565 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/templates/email/password_changed_confirmation.html
+-rw-r--r--   0        0        0     1216 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/templates/email/password_reset.html
+-rw-r--r--   0        0        0      565 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/templates/email/username_changed_confirmation.html
+-rw-r--r--   0        0        0     1216 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/templates/email/username_reset.html
+-rw-r--r--   0        0        0       57 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/urls/__init__.py
+-rw-r--r--   0        0        0      240 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/urls/authtoken.py
+-rw-r--r--   0        0        0      244 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/urls/base.py
+-rw-r--r--   0        0        0      350 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/urls/jwt.py
+-rw-r--r--   0        0        0     1188 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/utils.py
+-rw-r--r--   0        0        0    12862 2023-04-02 10:52:38.779937 djoser-2.2.0a0/djoser/views.py
+-rw-r--r--   0        0        0        0 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/webauthn/__init__.py
+-rw-r--r--   0        0        0       98 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/webauthn/apps.py
+-rw-r--r--   0        0        0     1471 2023-04-02 10:52:38.759938 djoser-2.2.0a0/djoser/webauthn/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/webauthn/migrations/__init__.py
+-rw-r--r--   0        0        0      554 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/webauthn/models.py
+-rw-r--r--   0        0        0     2050 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/webauthn/serializers.py
+-rw-r--r--   0        0        0      517 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/webauthn/urls.py
+-rw-r--r--   0        0        0      293 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/webauthn/utils.py
+-rw-r--r--   0        0        0     5687 2023-04-02 09:37:37.622141 djoser-2.2.0a0/djoser/webauthn/views.py
+-rw-r--r--   0        0        0     2992 2023-04-02 12:48:53.874220 djoser-2.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0     5725 1970-01-01 00:00:00.000000 djoser-2.2.0a0/PKG-INFO
```

### Comparing `djoser-2.2.0/LICENSE` & `djoser-2.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/README.rst` & `djoser-2.2.0a0/README.rst`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/conf.py` & `djoser-2.2.0a0/djoser/conf.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/constants.py` & `djoser-2.2.0a0/djoser/constants.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/email.py` & `djoser-2.2.0a0/djoser/email.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/de/LC_MESSAGES/django.mo` & `djoser-2.2.0a0/djoser/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/de/LC_MESSAGES/django.po` & `djoser-2.2.0a0/djoser/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/es/LC_MESSAGES/django.mo` & `djoser-2.2.0a0/djoser/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/es/LC_MESSAGES/django.po` & `djoser-2.2.0a0/djoser/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/fr/LC_MESSAGES/django.mo` & `djoser-2.2.0a0/djoser/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/fr/LC_MESSAGES/django.po` & `djoser-2.2.0a0/djoser/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/ja/LC_MESSAGES/django.mo` & `djoser-2.2.0a0/djoser/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/ja/LC_MESSAGES/django.po` & `djoser-2.2.0a0/djoser/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/ka/LC_MESSAGES/django.mo` & `djoser-2.2.0a0/djoser/locale/ka/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/ka/LC_MESSAGES/django.po` & `djoser-2.2.0a0/djoser/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/me/LC_MESSAGES/django.mo` & `djoser-2.2.0a0/djoser/locale/me/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/me/LC_MESSAGES/django.po` & `djoser-2.2.0a0/djoser/locale/me/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/pl/LC_MESSAGES/django.mo` & `djoser-2.2.0a0/djoser/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/pl/LC_MESSAGES/django.po` & `djoser-2.2.0a0/djoser/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/pt_BR/LC_MESSAGES/django.mo` & `djoser-2.2.0a0/djoser/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/pt_BR/LC_MESSAGES/django.po` & `djoser-2.2.0a0/djoser/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/ru_RU/LC_MESSAGES/django.mo` & `djoser-2.2.0a0/djoser/locale/ru_RU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/locale/ru_RU/LC_MESSAGES/django.po` & `djoser-2.2.0a0/djoser/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/permissions.py` & `djoser-2.2.0a0/djoser/permissions.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/serializers.py` & `djoser-2.2.0a0/djoser/serializers.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/social/serializers.py` & `djoser-2.2.0a0/djoser/social/serializers.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/social/views.py` & `djoser-2.2.0a0/djoser/social/views.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/templates/email/activation.html` & `djoser-2.2.0a0/djoser/templates/email/activation.html`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/templates/email/confirmation.html` & `djoser-2.2.0a0/djoser/templates/email/confirmation.html`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/templates/email/password_changed_confirmation.html` & `djoser-2.2.0a0/djoser/templates/email/password_changed_confirmation.html`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/templates/email/password_reset.html` & `djoser-2.2.0a0/djoser/templates/email/password_reset.html`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/templates/email/username_changed_confirmation.html` & `djoser-2.2.0a0/djoser/templates/email/username_changed_confirmation.html`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/templates/email/username_reset.html` & `djoser-2.2.0a0/djoser/templates/email/username_reset.html`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/utils.py` & `djoser-2.2.0a0/djoser/utils.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/views.py` & `djoser-2.2.0a0/djoser/views.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/webauthn/migrations/0001_initial.py` & `djoser-2.2.0a0/djoser/webauthn/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/webauthn/models.py` & `djoser-2.2.0a0/djoser/webauthn/models.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/webauthn/serializers.py` & `djoser-2.2.0a0/djoser/webauthn/serializers.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/webauthn/urls.py` & `djoser-2.2.0a0/djoser/webauthn/urls.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/djoser/webauthn/views.py` & `djoser-2.2.0a0/djoser/webauthn/views.py`

 * *Files identical despite different names*

### Comparing `djoser-2.2.0/pyproject.toml` & `djoser-2.2.0a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "djoser"
-version = "2.2.0"
+version = "2.2.0a0"
 description = "REST implementation of Django authentication system."
 authors = [
     "Sunscrapers <info@sunscrapers.com>",
 ]
 maintainers = [
     "Tomasz Wojcik <djoser@tomwojcik.com>",
 ]
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Django",
+    "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
```

### Comparing `djoser-2.2.0/PKG-INFO` & `djoser-2.2.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: djoser
-Version: 2.2.0
+Version: 2.2.0a0
 Summary: REST implementation of Django authentication system.
 Home-page: https://github.com/sunscrapers/djoser
 License: MIT
 Author: Sunscrapers
 Author-email: info@sunscrapers.com
 Maintainer: Tomasz Wojcik
 Maintainer-email: djoser@tomwojcik.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

