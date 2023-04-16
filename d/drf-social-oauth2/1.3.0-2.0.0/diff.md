# Comparing `tmp/drf-social-oauth2-1.3.0.tar.gz` & `tmp/drf-social-oauth2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-social-oauth2-1.3.0.tar", last modified: Sun Apr  2 20:16:00 2023, max compression
+gzip compressed data, was "drf-social-oauth2-2.0.0.tar", last modified: Sun Apr 16 15:47:25 2023, max compression
```

## Comparing `drf-social-oauth2-1.3.0.tar` & `drf-social-oauth2-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-02 20:16:00.451350 drf-social-oauth2-1.3.0/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     3561 2022-01-21 09:44:31.000000 drf-social-oauth2-1.3.0/CHANGELOG.rst
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1080 2020-06-27 18:20:06.000000 drf-social-oauth2-1.3.0/LICENSE.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)       81 2020-06-27 18:20:06.000000 drf-social-oauth2-1.3.0/MANIFEST.in
--rw-r--r--   0 wagner.delima   (502) staff       (20)    17270 2023-04-02 20:16:00.451014 drf-social-oauth2-1.3.0/PKG-INFO
--rw-r--r--   0 wagner.delima   (502) staff       (20)    16495 2023-04-02 20:14:23.000000 drf-social-oauth2-1.3.0/README.rst
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-02 20:16:00.446674 drf-social-oauth2-1.3.0/drf_social_oauth2/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1183 2023-04-02 20:09:06.000000 drf-social-oauth2-1.3.0/drf_social_oauth2/__init__.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2599 2022-01-13 22:12:11.000000 drf-social-oauth2-1.3.0/drf_social_oauth2/authentication.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)      687 2020-07-04 17:15:21.000000 drf-social-oauth2-1.3.0/drf_social_oauth2/backends.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1166 2022-01-06 11:17:42.000000 drf-social-oauth2-1.3.0/drf_social_oauth2/oauth2_backends.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     5432 2022-01-21 09:44:31.000000 drf-social-oauth2-1.3.0/drf_social_oauth2/oauth2_endpoints.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     4630 2020-07-05 09:16:42.000000 drf-social-oauth2-1.3.0/drf_social_oauth2/oauth2_grants.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)      546 2023-04-02 20:09:06.000000 drf-social-oauth2-1.3.0/drf_social_oauth2/serializers.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)      558 2023-03-26 14:38:31.000000 drf-social-oauth2-1.3.0/drf_social_oauth2/settings.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1766 2022-01-13 22:12:11.000000 drf-social-oauth2-1.3.0/drf_social_oauth2/test_settings.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2221 2023-04-02 12:11:34.000000 drf-social-oauth2-1.3.0/drf_social_oauth2/urls.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     9117 2023-04-02 20:09:06.000000 drf-social-oauth2-1.3.0/drf_social_oauth2/views.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-02 20:16:00.449020 drf-social-oauth2-1.3.0/drf_social_oauth2.egg-info/
--rw-r--r--   0 wagner.delima   (502) staff       (20)    17270 2023-04-02 20:16:00.000000 drf-social-oauth2-1.3.0/drf_social_oauth2.egg-info/PKG-INFO
--rw-r--r--   0 wagner.delima   (502) staff       (20)      823 2023-04-02 20:16:00.000000 drf-social-oauth2-1.3.0/drf_social_oauth2.egg-info/SOURCES.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-02 20:16:00.000000 drf-social-oauth2-1.3.0/drf_social_oauth2.egg-info/dependency_links.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-02 20:07:05.000000 drf-social-oauth2-1.3.0/drf_social_oauth2.egg-info/not-zip-safe
--rw-r--r--   0 wagner.delima   (502) staff       (20)      120 2023-04-02 20:16:00.000000 drf-social-oauth2-1.3.0/drf_social_oauth2.egg-info/requires.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)       24 2023-04-02 20:16:00.000000 drf-social-oauth2-1.3.0/drf_social_oauth2.egg-info/top_level.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)      274 2023-03-26 14:58:52.000000 drf-social-oauth2-1.3.0/pyproject.toml
--rw-r--r--   0 wagner.delima   (502) staff       (20)       38 2023-04-02 20:16:00.452365 drf-social-oauth2-1.3.0/setup.cfg
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1276 2023-04-02 20:09:06.000000 drf-social-oauth2-1.3.0/setup.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-02 20:16:00.449338 drf-social-oauth2-1.3.0/tests/
--rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2020-08-30 10:08:43.000000 drf-social-oauth2-1.3.0/tests/__init__.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-02 20:16:00.450558 drf-social-oauth2-1.3.0/tests/drf_social_oauth2/
--rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2020-08-30 10:08:43.000000 drf-social-oauth2-1.3.0/tests/drf_social_oauth2/__init__.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2081 2021-12-29 16:09:48.000000 drf-social-oauth2-1.3.0/tests/drf_social_oauth2/test_authentication.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     5577 2023-03-26 14:38:31.000000 drf-social-oauth2-1.3.0/tests/drf_social_oauth2/test_oauth2_endpoints.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-16 15:47:25.345432 drf-social-oauth2-2.0.0/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     3561 2022-01-21 09:44:31.000000 drf-social-oauth2-2.0.0/CHANGELOG.rst
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1080 2020-06-27 18:20:06.000000 drf-social-oauth2-2.0.0/LICENSE.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       81 2020-06-27 18:20:06.000000 drf-social-oauth2-2.0.0/MANIFEST.in
+-rw-r--r--   0 wagner.delima   (502) staff       (20)    20590 2023-04-16 15:47:25.344896 drf-social-oauth2-2.0.0/PKG-INFO
+-rw-r--r--   0 wagner.delima   (502) staff       (20)    19790 2023-04-16 14:33:15.000000 drf-social-oauth2-2.0.0/README.rst
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-16 15:47:25.335068 drf-social-oauth2-2.0.0/drf_social_oauth2/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1379 2023-04-16 14:33:15.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/__init__.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2599 2022-01-13 22:12:11.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/authentication.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1253 2023-04-16 14:33:15.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/backends.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1166 2022-01-06 11:17:42.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/oauth2_backends.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     5432 2022-01-21 09:44:31.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/oauth2_endpoints.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     4630 2020-07-05 09:16:42.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/oauth2_grants.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      546 2023-04-02 20:09:06.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/serializers.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      558 2023-03-26 14:38:31.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/settings.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1766 2022-01-13 22:12:11.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/test_settings.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2221 2023-04-02 12:11:34.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/urls.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     9117 2023-04-02 20:09:06.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/views.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-16 15:47:25.339845 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)    20590 2023-04-16 15:47:25.000000 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/PKG-INFO
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      823 2023-04-16 15:47:25.000000 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/SOURCES.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-16 15:47:25.000000 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/dependency_links.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-16 14:29:16.000000 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/not-zip-safe
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      120 2023-04-16 15:47:25.000000 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/requires.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       24 2023-04-16 15:47:25.000000 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/top_level.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      274 2023-03-26 14:58:52.000000 drf-social-oauth2-2.0.0/pyproject.toml
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       38 2023-04-16 15:47:25.346556 drf-social-oauth2-2.0.0/setup.cfg
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1276 2023-04-02 20:09:06.000000 drf-social-oauth2-2.0.0/setup.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-16 15:47:25.340586 drf-social-oauth2-2.0.0/tests/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2020-08-30 10:08:43.000000 drf-social-oauth2-2.0.0/tests/__init__.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-16 15:47:25.342836 drf-social-oauth2-2.0.0/tests/drf_social_oauth2/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2023-04-16 13:51:16.000000 drf-social-oauth2-2.0.0/tests/drf_social_oauth2/__init__.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2081 2021-12-29 16:09:48.000000 drf-social-oauth2-2.0.0/tests/drf_social_oauth2/test_authentication.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     5577 2023-04-16 14:20:37.000000 drf-social-oauth2-2.0.0/tests/drf_social_oauth2/test_oauth2_endpoints.py
```

### Comparing `drf-social-oauth2-1.3.0/CHANGELOG.rst` & `drf-social-oauth2-2.0.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/LICENSE.txt` & `drf-social-oauth2-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/PKG-INFO` & `drf-social-oauth2-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: drf-social-oauth2
-Version: 1.3.0
-Summary: python-social-auth and oauth2 support for django-rest-framework.
+Version: 2.0.0
+Summary: drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework.
 Home-page: https://github.com/wagnerdelima/drf-social-oauth2
 Author: Wagner de Lima
 Author-email: waglds@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -257,16 +257,16 @@
             'drf_social_oauth2.authentication.SocialAuthentication',
         )
     }
 
 Listed below are a few examples of supported backends that can be used for social authentication.
 
 
-Facebook Example
-^^^^^^^^^^^^^^^^
+Facebook Integration
+^^^^^^^^^^^^^^^^^^^^
 
 To use Facebook as the authorization backend of your REST API, your settings.py file should look like this:
 
 .. code-block:: python
 
     AUTHENTICATION_BACKENDS = (
         # Others auth providers (e.g. Google, OpenId, etc)
@@ -310,16 +310,16 @@
 
 For testing purposes, you can use the access token ``<user_access_token>`` from https://developers.facebook.com/tools/accesstoken/.
 
 For more information on how to configure python-social-auth with Facebook visit
 http://python-social-auth.readthedocs.io/en/latest/backends/facebook.html.
 
 
-Google Example
-^^^^^^^^^^^^^^
+Google Integration
+^^^^^^^^^^^^^^^^^^
 
 To use Google OAuth2 as the authorization backend of your REST API, your settings.py file should look like this:
 
 .. code-block:: python
 
     AUTHENTICATION_BACKENDS = (
         # Others auth providers (e.g. Facebook, OpenId, etc)
@@ -363,26 +363,86 @@
 ``SOCIAL_AUTH_GOOGLE_OAUTH2_SECRET``.
 
 For testing purposes, you can use the access token ``<user_access_token>`` from
 https://developers.google.com/oauthplayground/.
 
     1. Visit the OAuth 2.0 Playground
     2. Select Google OAuth2 API v2 and authorize for https://www.googleapis.com/auth/userinfo.email and https://www.googleapis.com/auth/userinfo.profile
-
     3. Exchange Authorization code for tokens and get access token
     4. Use the access token as the token parameter in the /convert-token endpoint.
 
 If you would like a step-by-step tutorial, see this link, by @djangokatya:
 https://djangokatya.com/2021/04/09/social-login-for-django-rest-framefork-for-newbies-a-k-a-for-me/
 
 For more information on how to configure python-social-auth with Google visit
 https://python-social-auth.readthedocs.io/en/latest/backends/google.html#google-oauth2.
 
 
-GitHub Example
+Google OpenID Integration
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+OpenID and access tokens are two different concepts that are used in authentication and authorization systems.
+
+OpenID is an open standard that allows users to authenticate with multiple websites and applications using a single
+set of credentials. When a user logs in using OpenID, they are redirected to their OpenID provider, which authenticates
+them and provides the website or application with a unique identifier for the user. The identifier can be used to
+retrieve the user's profile information, but it does not provide any authorization to access APIs or services.
+
+Access tokens, on the other hand, are used to authorize API requests on behalf of the user.
+When a user logs in and grants permission to access their data, an access token is generated and returned to the client
+application. The access token is used to authenticate the client application and authorize it to make API requests on
+behalf of the user. The access token contains information such as the permissions granted to the client application,
+the expiration time, and a signature that verifies the token's authenticity.
+
+In summary, OpenID is used to authenticate users and provide a unique identifier for them, while access tokens are
+used to authorize API requests on behalf of the user. While OpenID and access tokens are both important components
+of authentication and authorization systems, they serve different purposes and should not be confused with each other.
+
+In order to authenticate with Open ID, proceed as follows:
+
+
+.. code-block:: python
+
+    AUTHENTICATION_BACKENDS = (
+        # Others auth providers (e.g. Facebook, OpenId, etc)
+        ...
+        # Google  OAuth2
+        'drf_social_oauth2.backends.GoogleIdentityBackend',
+        # drf-social-oauth2
+        'drf_social_oauth2.backends.DjangoOAuth2',
+        # Django
+        'django.contrib.auth.backends.ModelBackend',
+    )
+
+    # Google configuration
+    SOCIAL_AUTH_GOOGLE_OAUTH2_KEY = <your app id goes here>
+    SOCIAL_AUTH_GOOGLE_OAUTH2_SECRET = <your app secret goes here>
+
+    # Define SOCIAL_AUTH_GOOGLE_OAUTH2_SCOPE to get extra permissions from Google.
+    SOCIAL_AUTH_GOOGLE_OAUTH2_SCOPE = [
+        'https://www.googleapis.com/auth/userinfo.email',
+        'https://www.googleapis.com/auth/userinfo.profile',
+    ]
+
+
+For testing purposes, you can use the id token ``<id_token>`` from
+https://developers.google.com/oauthplayground/.
+
+    1. Visit the OAuth 2.0 Playground.
+    2. Select Google OAuth2 API v2 and authorize for openid.
+    3. Exchange Authorization code for tokens and get access token.
+    4. Use the access token as the token parameter in the /convert-token endpoint.
+
+If you want to have your open id token validated, copy it and hit this url,
+https://oauth2.googleapis.com/tokeninfo?id_token=your_token_here.
+
+You can test these settings by running the following command::
+
+    curl -X POST -d "grant_type=convert_token&client_id=<django-oauth-generated-client_id>&client_secret=<django-oauth-generated-client_secret>&backend=google-identity&token=<google_openid_token>" http://localhost:8000/auth/convert-token
+
 ^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     AUTHENTICATION_BACKENDS = (
         # Others auth providers (e.g. Facebook, OpenId, etc)
         ...
@@ -411,26 +471,27 @@
 
 Now, visit https://github.com/settings/tokens and create a new token. Select the user checkbox, as to grant user access.
 The click on the Generate Token button. Use the access token as the token parameter in the /convert-token endpoint.
 
 Running local tests
 ^^^^^^^^^^^^^^^^^^^
 
-You may find drf-social-oauth2's unit tests in the tests/ directory. In order to run the tests locally, you can either
-use pytest directly or coverage itself. Prior to running the test cases you need to install the local dependencies by:
+You may find drf-social-oauth2's unit tests in the tests/ directory. In order to run the tests locally, you need to
+build the docker image and execute the test run command with the following commands below:
 
-    $ pip3 install -r requirements.test.txt
 
-Then you can just run pytest in your terminal:
+    $ docker-compose -f docker-compose.tests.yml build --no-cache
+    $ docker-compose -f docker-compose.tests.yml up --exit-code-from app
 
-    $ pytest
+Then, destroy all containers created in your local system:
 
-or call coverage to get the most updated test coverage:
+    $ docker-compose -f docker-compose.tests.yml down
 
-    $ coverage run --source='.' -m pytest && coverage html
+Your local environment has a htmlcov/ folder with the test coverage. See the index.html file for more info about the
+coverage of the project.
 
 
 Customize token expiration
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 You can set the expiry time for tokens as follows:
```

### Comparing `drf-social-oauth2-1.3.0/README.rst` & `drf-social-oauth2-2.0.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -237,16 +237,16 @@
             'drf_social_oauth2.authentication.SocialAuthentication',
         )
     }
 
 Listed below are a few examples of supported backends that can be used for social authentication.
 
 
-Facebook Example
-^^^^^^^^^^^^^^^^
+Facebook Integration
+^^^^^^^^^^^^^^^^^^^^
 
 To use Facebook as the authorization backend of your REST API, your settings.py file should look like this:
 
 .. code-block:: python
 
     AUTHENTICATION_BACKENDS = (
         # Others auth providers (e.g. Google, OpenId, etc)
@@ -290,16 +290,16 @@
 
 For testing purposes, you can use the access token ``<user_access_token>`` from https://developers.facebook.com/tools/accesstoken/.
 
 For more information on how to configure python-social-auth with Facebook visit
 http://python-social-auth.readthedocs.io/en/latest/backends/facebook.html.
 
 
-Google Example
-^^^^^^^^^^^^^^
+Google Integration
+^^^^^^^^^^^^^^^^^^
 
 To use Google OAuth2 as the authorization backend of your REST API, your settings.py file should look like this:
 
 .. code-block:: python
 
     AUTHENTICATION_BACKENDS = (
         # Others auth providers (e.g. Facebook, OpenId, etc)
@@ -343,26 +343,86 @@
 ``SOCIAL_AUTH_GOOGLE_OAUTH2_SECRET``.
 
 For testing purposes, you can use the access token ``<user_access_token>`` from
 https://developers.google.com/oauthplayground/.
 
     1. Visit the OAuth 2.0 Playground
     2. Select Google OAuth2 API v2 and authorize for https://www.googleapis.com/auth/userinfo.email and https://www.googleapis.com/auth/userinfo.profile
-
     3. Exchange Authorization code for tokens and get access token
     4. Use the access token as the token parameter in the /convert-token endpoint.
 
 If you would like a step-by-step tutorial, see this link, by @djangokatya:
 https://djangokatya.com/2021/04/09/social-login-for-django-rest-framefork-for-newbies-a-k-a-for-me/
 
 For more information on how to configure python-social-auth with Google visit
 https://python-social-auth.readthedocs.io/en/latest/backends/google.html#google-oauth2.
 
 
-GitHub Example
+Google OpenID Integration
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+OpenID and access tokens are two different concepts that are used in authentication and authorization systems.
+
+OpenID is an open standard that allows users to authenticate with multiple websites and applications using a single
+set of credentials. When a user logs in using OpenID, they are redirected to their OpenID provider, which authenticates
+them and provides the website or application with a unique identifier for the user. The identifier can be used to
+retrieve the user's profile information, but it does not provide any authorization to access APIs or services.
+
+Access tokens, on the other hand, are used to authorize API requests on behalf of the user.
+When a user logs in and grants permission to access their data, an access token is generated and returned to the client
+application. The access token is used to authenticate the client application and authorize it to make API requests on
+behalf of the user. The access token contains information such as the permissions granted to the client application,
+the expiration time, and a signature that verifies the token's authenticity.
+
+In summary, OpenID is used to authenticate users and provide a unique identifier for them, while access tokens are
+used to authorize API requests on behalf of the user. While OpenID and access tokens are both important components
+of authentication and authorization systems, they serve different purposes and should not be confused with each other.
+
+In order to authenticate with Open ID, proceed as follows:
+
+
+.. code-block:: python
+
+    AUTHENTICATION_BACKENDS = (
+        # Others auth providers (e.g. Facebook, OpenId, etc)
+        ...
+        # Google  OAuth2
+        'drf_social_oauth2.backends.GoogleIdentityBackend',
+        # drf-social-oauth2
+        'drf_social_oauth2.backends.DjangoOAuth2',
+        # Django
+        'django.contrib.auth.backends.ModelBackend',
+    )
+
+    # Google configuration
+    SOCIAL_AUTH_GOOGLE_OAUTH2_KEY = <your app id goes here>
+    SOCIAL_AUTH_GOOGLE_OAUTH2_SECRET = <your app secret goes here>
+
+    # Define SOCIAL_AUTH_GOOGLE_OAUTH2_SCOPE to get extra permissions from Google.
+    SOCIAL_AUTH_GOOGLE_OAUTH2_SCOPE = [
+        'https://www.googleapis.com/auth/userinfo.email',
+        'https://www.googleapis.com/auth/userinfo.profile',
+    ]
+
+
+For testing purposes, you can use the id token ``<id_token>`` from
+https://developers.google.com/oauthplayground/.
+
+    1. Visit the OAuth 2.0 Playground.
+    2. Select Google OAuth2 API v2 and authorize for openid.
+    3. Exchange Authorization code for tokens and get access token.
+    4. Use the access token as the token parameter in the /convert-token endpoint.
+
+If you want to have your open id token validated, copy it and hit this url,
+https://oauth2.googleapis.com/tokeninfo?id_token=your_token_here.
+
+You can test these settings by running the following command::
+
+    curl -X POST -d "grant_type=convert_token&client_id=<django-oauth-generated-client_id>&client_secret=<django-oauth-generated-client_secret>&backend=google-identity&token=<google_openid_token>" http://localhost:8000/auth/convert-token
+
 ^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     AUTHENTICATION_BACKENDS = (
         # Others auth providers (e.g. Facebook, OpenId, etc)
         ...
@@ -391,26 +451,27 @@
 
 Now, visit https://github.com/settings/tokens and create a new token. Select the user checkbox, as to grant user access.
 The click on the Generate Token button. Use the access token as the token parameter in the /convert-token endpoint.
 
 Running local tests
 ^^^^^^^^^^^^^^^^^^^
 
-You may find drf-social-oauth2's unit tests in the tests/ directory. In order to run the tests locally, you can either
-use pytest directly or coverage itself. Prior to running the test cases you need to install the local dependencies by:
+You may find drf-social-oauth2's unit tests in the tests/ directory. In order to run the tests locally, you need to
+build the docker image and execute the test run command with the following commands below:
 
-    $ pip3 install -r requirements.test.txt
 
-Then you can just run pytest in your terminal:
+    $ docker-compose -f docker-compose.tests.yml build --no-cache
+    $ docker-compose -f docker-compose.tests.yml up --exit-code-from app
 
-    $ pytest
+Then, destroy all containers created in your local system:
 
-or call coverage to get the most updated test coverage:
+    $ docker-compose -f docker-compose.tests.yml down
 
-    $ coverage run --source='.' -m pytest && coverage html
+Your local environment has a htmlcov/ folder with the test coverage. See the index.html file for more info about the
+coverage of the project.
 
 
 Customize token expiration
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 You can set the expiry time for tokens as follows:
```

### Comparing `drf-social-oauth2-1.3.0/drf_social_oauth2/__init__.py` & `drf-social-oauth2-2.0.0/drf_social_oauth2/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """
-python-social-auth and oauth2 support for django-rest-framework.
-drf-social-oauth2 makes it easy to integrate Django social authentication with major OAuth2 providers, i.e., Facebook, Twitter, Google, etc.
+drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework.
+drf-social-oauth2 offers support to oauth2 authentication and authorization.
+It's one of the easiest frameworks to integrate Oauth2 to your Django Rest Framework application.
+By using drf-social-oauth2 you can authenticate with major vendors such as Google, Facebook, Instagram, Github, Twitter
+and a ton more!
 """
-__version__ = '1.3.0'
+
+__version__ = '2.0.0'
 
 try:
     from secrets import SystemRandom
 except ImportError:
     from random import SystemRandom
```

### Comparing `drf-social-oauth2-1.3.0/drf_social_oauth2/authentication.py` & `drf-social-oauth2-2.0.0/drf_social_oauth2/authentication.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/drf_social_oauth2/oauth2_backends.py` & `drf-social-oauth2-2.0.0/drf_social_oauth2/oauth2_backends.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/drf_social_oauth2/oauth2_endpoints.py` & `drf-social-oauth2-2.0.0/drf_social_oauth2/oauth2_endpoints.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/drf_social_oauth2/oauth2_grants.py` & `drf-social-oauth2-2.0.0/drf_social_oauth2/oauth2_grants.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/drf_social_oauth2/serializers.py` & `drf-social-oauth2-2.0.0/drf_social_oauth2/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/drf_social_oauth2/settings.py` & `drf-social-oauth2-2.0.0/drf_social_oauth2/settings.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/drf_social_oauth2/test_settings.py` & `drf-social-oauth2-2.0.0/drf_social_oauth2/test_settings.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/drf_social_oauth2/urls.py` & `drf-social-oauth2-2.0.0/drf_social_oauth2/urls.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/drf_social_oauth2/views.py` & `drf-social-oauth2-2.0.0/drf_social_oauth2/views.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/drf_social_oauth2.egg-info/PKG-INFO` & `drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: drf-social-oauth2
-Version: 1.3.0
-Summary: python-social-auth and oauth2 support for django-rest-framework.
+Version: 2.0.0
+Summary: drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework.
 Home-page: https://github.com/wagnerdelima/drf-social-oauth2
 Author: Wagner de Lima
 Author-email: waglds@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -257,16 +257,16 @@
             'drf_social_oauth2.authentication.SocialAuthentication',
         )
     }
 
 Listed below are a few examples of supported backends that can be used for social authentication.
 
 
-Facebook Example
-^^^^^^^^^^^^^^^^
+Facebook Integration
+^^^^^^^^^^^^^^^^^^^^
 
 To use Facebook as the authorization backend of your REST API, your settings.py file should look like this:
 
 .. code-block:: python
 
     AUTHENTICATION_BACKENDS = (
         # Others auth providers (e.g. Google, OpenId, etc)
@@ -310,16 +310,16 @@
 
 For testing purposes, you can use the access token ``<user_access_token>`` from https://developers.facebook.com/tools/accesstoken/.
 
 For more information on how to configure python-social-auth with Facebook visit
 http://python-social-auth.readthedocs.io/en/latest/backends/facebook.html.
 
 
-Google Example
-^^^^^^^^^^^^^^
+Google Integration
+^^^^^^^^^^^^^^^^^^
 
 To use Google OAuth2 as the authorization backend of your REST API, your settings.py file should look like this:
 
 .. code-block:: python
 
     AUTHENTICATION_BACKENDS = (
         # Others auth providers (e.g. Facebook, OpenId, etc)
@@ -363,26 +363,86 @@
 ``SOCIAL_AUTH_GOOGLE_OAUTH2_SECRET``.
 
 For testing purposes, you can use the access token ``<user_access_token>`` from
 https://developers.google.com/oauthplayground/.
 
     1. Visit the OAuth 2.0 Playground
     2. Select Google OAuth2 API v2 and authorize for https://www.googleapis.com/auth/userinfo.email and https://www.googleapis.com/auth/userinfo.profile
-
     3. Exchange Authorization code for tokens and get access token
     4. Use the access token as the token parameter in the /convert-token endpoint.
 
 If you would like a step-by-step tutorial, see this link, by @djangokatya:
 https://djangokatya.com/2021/04/09/social-login-for-django-rest-framefork-for-newbies-a-k-a-for-me/
 
 For more information on how to configure python-social-auth with Google visit
 https://python-social-auth.readthedocs.io/en/latest/backends/google.html#google-oauth2.
 
 
-GitHub Example
+Google OpenID Integration
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+OpenID and access tokens are two different concepts that are used in authentication and authorization systems.
+
+OpenID is an open standard that allows users to authenticate with multiple websites and applications using a single
+set of credentials. When a user logs in using OpenID, they are redirected to their OpenID provider, which authenticates
+them and provides the website or application with a unique identifier for the user. The identifier can be used to
+retrieve the user's profile information, but it does not provide any authorization to access APIs or services.
+
+Access tokens, on the other hand, are used to authorize API requests on behalf of the user.
+When a user logs in and grants permission to access their data, an access token is generated and returned to the client
+application. The access token is used to authenticate the client application and authorize it to make API requests on
+behalf of the user. The access token contains information such as the permissions granted to the client application,
+the expiration time, and a signature that verifies the token's authenticity.
+
+In summary, OpenID is used to authenticate users and provide a unique identifier for them, while access tokens are
+used to authorize API requests on behalf of the user. While OpenID and access tokens are both important components
+of authentication and authorization systems, they serve different purposes and should not be confused with each other.
+
+In order to authenticate with Open ID, proceed as follows:
+
+
+.. code-block:: python
+
+    AUTHENTICATION_BACKENDS = (
+        # Others auth providers (e.g. Facebook, OpenId, etc)
+        ...
+        # Google  OAuth2
+        'drf_social_oauth2.backends.GoogleIdentityBackend',
+        # drf-social-oauth2
+        'drf_social_oauth2.backends.DjangoOAuth2',
+        # Django
+        'django.contrib.auth.backends.ModelBackend',
+    )
+
+    # Google configuration
+    SOCIAL_AUTH_GOOGLE_OAUTH2_KEY = <your app id goes here>
+    SOCIAL_AUTH_GOOGLE_OAUTH2_SECRET = <your app secret goes here>
+
+    # Define SOCIAL_AUTH_GOOGLE_OAUTH2_SCOPE to get extra permissions from Google.
+    SOCIAL_AUTH_GOOGLE_OAUTH2_SCOPE = [
+        'https://www.googleapis.com/auth/userinfo.email',
+        'https://www.googleapis.com/auth/userinfo.profile',
+    ]
+
+
+For testing purposes, you can use the id token ``<id_token>`` from
+https://developers.google.com/oauthplayground/.
+
+    1. Visit the OAuth 2.0 Playground.
+    2. Select Google OAuth2 API v2 and authorize for openid.
+    3. Exchange Authorization code for tokens and get access token.
+    4. Use the access token as the token parameter in the /convert-token endpoint.
+
+If you want to have your open id token validated, copy it and hit this url,
+https://oauth2.googleapis.com/tokeninfo?id_token=your_token_here.
+
+You can test these settings by running the following command::
+
+    curl -X POST -d "grant_type=convert_token&client_id=<django-oauth-generated-client_id>&client_secret=<django-oauth-generated-client_secret>&backend=google-identity&token=<google_openid_token>" http://localhost:8000/auth/convert-token
+
 ^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     AUTHENTICATION_BACKENDS = (
         # Others auth providers (e.g. Facebook, OpenId, etc)
         ...
@@ -411,26 +471,27 @@
 
 Now, visit https://github.com/settings/tokens and create a new token. Select the user checkbox, as to grant user access.
 The click on the Generate Token button. Use the access token as the token parameter in the /convert-token endpoint.
 
 Running local tests
 ^^^^^^^^^^^^^^^^^^^
 
-You may find drf-social-oauth2's unit tests in the tests/ directory. In order to run the tests locally, you can either
-use pytest directly or coverage itself. Prior to running the test cases you need to install the local dependencies by:
+You may find drf-social-oauth2's unit tests in the tests/ directory. In order to run the tests locally, you need to
+build the docker image and execute the test run command with the following commands below:
 
-    $ pip3 install -r requirements.test.txt
 
-Then you can just run pytest in your terminal:
+    $ docker-compose -f docker-compose.tests.yml build --no-cache
+    $ docker-compose -f docker-compose.tests.yml up --exit-code-from app
 
-    $ pytest
+Then, destroy all containers created in your local system:
 
-or call coverage to get the most updated test coverage:
+    $ docker-compose -f docker-compose.tests.yml down
 
-    $ coverage run --source='.' -m pytest && coverage html
+Your local environment has a htmlcov/ folder with the test coverage. See the index.html file for more info about the
+coverage of the project.
 
 
 Customize token expiration
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 You can set the expiry time for tokens as follows:
```

### Comparing `drf-social-oauth2-1.3.0/drf_social_oauth2.egg-info/SOURCES.txt` & `drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/setup.py` & `drf-social-oauth2-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/tests/drf_social_oauth2/test_authentication.py` & `drf-social-oauth2-2.0.0/tests/drf_social_oauth2/test_authentication.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-1.3.0/tests/drf_social_oauth2/test_oauth2_endpoints.py` & `drf-social-oauth2-2.0.0/tests/drf_social_oauth2/test_oauth2_endpoints.py`

 * *Files identical despite different names*

