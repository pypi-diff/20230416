# Comparing `tmp/django-cookie_consent_gutsh-0.0.2.tar.gz` & `tmp/django-cookie_consent_gutsh-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cookie_consent_gutsh-0.0.2.tar", last modified: Sat Apr 15 17:11:13 2023, max compression
+gzip compressed data, was "django-cookie_consent_gutsh-0.1.0.tar", last modified: Sun Apr 16 10:55:31 2023, max compression
```

## Comparing `django-cookie_consent_gutsh-0.0.2.tar` & `django-cookie_consent_gutsh-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-15 17:11:13.873246 django-cookie_consent_gutsh-0.0.2/
--rw-r--r--   0 gutsh      (501) staff       (20)     1074 2023-04-15 14:55:37.000000 django-cookie_consent_gutsh-0.0.2/LICENSE
--rw-r--r--   0 gutsh      (501) staff       (20)      147 2023-04-14 11:24:09.000000 django-cookie_consent_gutsh-0.0.2/MANIFEST.in
--rw-r--r--   0 gutsh      (501) staff       (20)     1171 2023-04-15 17:11:13.873560 django-cookie_consent_gutsh-0.0.2/PKG-INFO
--rw-r--r--   0 gutsh      (501) staff       (20)      577 2023-04-15 14:50:58.000000 django-cookie_consent_gutsh-0.0.2/README.md
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-15 17:11:13.863791 django-cookie_consent_gutsh-0.0.2/cookie_consent/
--rw-r--r--   0 gutsh      (501) staff       (20)        0 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-0.0.2/cookie_consent/__init__.py
--rw-r--r--   0 gutsh      (501) staff       (20)      108 2023-04-15 13:09:46.000000 django-cookie_consent_gutsh-0.0.2/cookie_consent/admin.py
--rw-r--r--   0 gutsh      (501) staff       (20)      159 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-0.0.2/cookie_consent/apps.py
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-15 17:11:13.866239 django-cookie_consent_gutsh-0.0.2/cookie_consent/migrations/
--rw-r--r--   0 gutsh      (501) staff       (20)      732 2023-04-15 12:52:39.000000 django-cookie_consent_gutsh-0.0.2/cookie_consent/migrations/0001_initial.py
--rw-r--r--   0 gutsh      (501) staff       (20)        0 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-0.0.2/cookie_consent/migrations/__init__.py
--rw-r--r--   0 gutsh      (501) staff       (20)      327 2023-04-15 13:30:14.000000 django-cookie_consent_gutsh-0.0.2/cookie_consent/models.py
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-15 17:11:13.850226 django-cookie_consent_gutsh-0.0.2/cookie_consent/static/
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-15 17:11:13.850347 django-cookie_consent_gutsh-0.0.2/cookie_consent/static/cookie_consent/
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-15 17:11:13.868106 django-cookie_consent_gutsh-0.0.2/cookie_consent/static/cookie_consent/css/
--rw-r--r--   0 gutsh      (501) staff       (20)      149 2023-04-15 15:22:56.000000 django-cookie_consent_gutsh-0.0.2/cookie_consent/static/cookie_consent/css/README.md
--rw-r--r--   0 gutsh      (501) staff       (20)      462 2023-04-14 09:46:39.000000 django-cookie_consent_gutsh-0.0.2/cookie_consent/static/cookie_consent/css/index.css
--rw-r--r--   0 gutsh      (501) staff       (20)      245 2023-04-14 09:46:39.000000 django-cookie_consent_gutsh-0.0.2/cookie_consent/static/cookie_consent/css/index.css.map
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-15 17:11:13.850643 django-cookie_consent_gutsh-0.0.2/cookie_consent/templates/
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-15 17:11:13.850745 django-cookie_consent_gutsh-0.0.2/cookie_consent/templates/cookie_consent/
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-15 17:11:13.869014 django-cookie_consent_gutsh-0.0.2/cookie_consent/templates/cookie_consent/includes/
--rw-r--r--   0 gutsh      (501) staff       (20)      704 2023-04-15 13:27:04.000000 django-cookie_consent_gutsh-0.0.2/cookie_consent/templates/cookie_consent/includes/consent.html
--rw-r--r--   0 gutsh      (501) staff       (20)       60 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-0.0.2/cookie_consent/tests.py
--rw-r--r--   0 gutsh      (501) staff       (20)      180 2023-04-15 12:36:12.000000 django-cookie_consent_gutsh-0.0.2/cookie_consent/urls.py
--rw-r--r--   0 gutsh      (501) staff       (20)     1249 2023-04-15 13:29:26.000000 django-cookie_consent_gutsh-0.0.2/cookie_consent/views.py
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-15 17:11:13.872422 django-cookie_consent_gutsh-0.0.2/django_cookie_consent_gutsh.egg-info/
--rw-r--r--   0 gutsh      (501) staff       (20)     1171 2023-04-15 17:11:13.000000 django-cookie_consent_gutsh-0.0.2/django_cookie_consent_gutsh.egg-info/PKG-INFO
--rw-r--r--   0 gutsh      (501) staff       (20)      786 2023-04-15 17:11:13.000000 django-cookie_consent_gutsh-0.0.2/django_cookie_consent_gutsh.egg-info/SOURCES.txt
--rw-r--r--   0 gutsh      (501) staff       (20)        1 2023-04-15 17:11:13.000000 django-cookie_consent_gutsh-0.0.2/django_cookie_consent_gutsh.egg-info/dependency_links.txt
--rw-r--r--   0 gutsh      (501) staff       (20)       12 2023-04-15 17:11:13.000000 django-cookie_consent_gutsh-0.0.2/django_cookie_consent_gutsh.egg-info/requires.txt
--rw-r--r--   0 gutsh      (501) staff       (20)       15 2023-04-15 17:11:13.000000 django-cookie_consent_gutsh-0.0.2/django_cookie_consent_gutsh.egg-info/top_level.txt
--rw-r--r--   0 gutsh      (501) staff       (20)      547 2023-04-15 15:02:33.000000 django-cookie_consent_gutsh-0.0.2/pyproject.toml
--rw-r--r--   0 gutsh      (501) staff       (20)      937 2023-04-15 17:11:13.874329 django-cookie_consent_gutsh-0.0.2/setup.cfg
--rw-r--r--   0 gutsh      (501) staff       (20)       38 2023-04-14 11:20:52.000000 django-cookie_consent_gutsh-0.0.2/setup.py
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.489233 django-cookie_consent_gutsh-0.1.0/
+-rw-r--r--   0 gutsh      (501) staff       (20)     1074 2023-04-15 14:55:37.000000 django-cookie_consent_gutsh-0.1.0/LICENSE
+-rw-r--r--   0 gutsh      (501) staff       (20)      147 2023-04-14 11:24:09.000000 django-cookie_consent_gutsh-0.1.0/MANIFEST.in
+-rw-r--r--   0 gutsh      (501) staff       (20)     1499 2023-04-16 10:55:31.489437 django-cookie_consent_gutsh-0.1.0/PKG-INFO
+-rw-r--r--   0 gutsh      (501) staff       (20)      905 2023-04-16 10:53:45.000000 django-cookie_consent_gutsh-0.1.0/README.md
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.478237 django-cookie_consent_gutsh-0.1.0/cookie_consent/
+-rw-r--r--   0 gutsh      (501) staff       (20)        0 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/__init__.py
+-rw-r--r--   0 gutsh      (501) staff       (20)      108 2023-04-15 13:09:46.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/admin.py
+-rw-r--r--   0 gutsh      (501) staff       (20)      159 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/apps.py
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.479420 django-cookie_consent_gutsh-0.1.0/cookie_consent/migrations/
+-rw-r--r--   0 gutsh      (501) staff       (20)      732 2023-04-15 12:52:39.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/migrations/0001_initial.py
+-rw-r--r--   0 gutsh      (501) staff       (20)        0 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/migrations/__init__.py
+-rw-r--r--   0 gutsh      (501) staff       (20)      327 2023-04-15 13:30:14.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/models.py
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.468588 django-cookie_consent_gutsh-0.1.0/cookie_consent/static/
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.468772 django-cookie_consent_gutsh-0.1.0/cookie_consent/static/cookie_consent/
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.482829 django-cookie_consent_gutsh-0.1.0/cookie_consent/static/cookie_consent/css/
+-rw-r--r--   0 gutsh      (501) staff       (20)      149 2023-04-15 15:22:56.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/static/cookie_consent/css/README.md
+-rw-r--r--   0 gutsh      (501) staff       (20)      462 2023-04-14 09:46:39.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/static/cookie_consent/css/index.css
+-rw-r--r--   0 gutsh      (501) staff       (20)      245 2023-04-14 09:46:39.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/static/cookie_consent/css/index.css.map
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.469066 django-cookie_consent_gutsh-0.1.0/cookie_consent/templates/
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.469199 django-cookie_consent_gutsh-0.1.0/cookie_consent/templates/cookie_consent/
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.484656 django-cookie_consent_gutsh-0.1.0/cookie_consent/templates/cookie_consent/includes/
+-rw-r--r--   0 gutsh      (501) staff       (20)      704 2023-04-15 13:27:04.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/templates/cookie_consent/includes/consent.html
+-rw-r--r--   0 gutsh      (501) staff       (20)       60 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/tests.py
+-rw-r--r--   0 gutsh      (501) staff       (20)      180 2023-04-15 12:36:12.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/urls.py
+-rw-r--r--   0 gutsh      (501) staff       (20)     1249 2023-04-15 13:29:26.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/views.py
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.488697 django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/
+-rw-r--r--   0 gutsh      (501) staff       (20)     1499 2023-04-16 10:55:31.000000 django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/PKG-INFO
+-rw-r--r--   0 gutsh      (501) staff       (20)      786 2023-04-16 10:55:31.000000 django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/SOURCES.txt
+-rw-r--r--   0 gutsh      (501) staff       (20)        1 2023-04-16 10:55:31.000000 django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/dependency_links.txt
+-rw-r--r--   0 gutsh      (501) staff       (20)       12 2023-04-16 10:55:31.000000 django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/requires.txt
+-rw-r--r--   0 gutsh      (501) staff       (20)       15 2023-04-16 10:55:31.000000 django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/top_level.txt
+-rw-r--r--   0 gutsh      (501) staff       (20)      547 2023-04-15 17:36:38.000000 django-cookie_consent_gutsh-0.1.0/pyproject.toml
+-rw-r--r--   0 gutsh      (501) staff       (20)      937 2023-04-16 10:55:31.490196 django-cookie_consent_gutsh-0.1.0/setup.cfg
+-rw-r--r--   0 gutsh      (501) staff       (20)       38 2023-04-14 11:20:52.000000 django-cookie_consent_gutsh-0.1.0/setup.py
```

### Comparing `django-cookie_consent_gutsh-0.0.2/LICENSE` & `django-cookie_consent_gutsh-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cookie_consent_gutsh-0.0.2/PKG-INFO` & `django-cookie_consent_gutsh-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
 00000020: 676f 2d63 6f6f 6b69 655f 636f 6e73 656e  go-cookie_consen
 00000030: 745f 6775 7473 680a 5665 7273 696f 6e3a  t_gutsh.Version:
-00000040: 2030 2e30 2e32 0a53 756d 6d61 7279 3a20   0.0.2.Summary: 
+00000040: 2030 2e31 2e30 0a53 756d 6d61 7279 3a20   0.1.0.Summary: 
 00000050: 436f 6f6b 6965 2063 6f6e 7365 6e74 2063  Cookie consent c
 00000060: 6f6d 706f 6e65 6e74 2066 6f72 2061 6e79  omponent for any
 00000070: 2044 6a61 6e67 6f20 7765 622d 7369 7465   Django web-site
 00000080: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
 00000090: 733a 2f2f 7777 772e 6261 7273 6b69 796c  s://www.barskiyl
 000000a0: 6162 2e63 6f6d 2f0a 4175 7468 6f72 3a20  ab.com/.Author: 
 000000b0: 4172 7465 6d20 4261 7273 6b69 690a 4175  Artem Barskii.Au
@@ -34,41 +34,61 @@
 00000210: 2e38 0a44 6573 6372 6970 7469 6f6e 2d43  .8.Description-C
 00000220: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
 00000230: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
 00000240: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
 00000250: 0a0a 2320 436f 6f6b 6965 2063 6f6e 7365  ..# Cookie conse
 00000260: 6e74 0a0a 436f 6f6b 6965 2063 6f6e 7365  nt..Cookie conse
 00000270: 6e74 2069 7320 6120 446a 616e 676f 2061  nt is a Django a
-00000280: 7070 2074 6f20 636f 6e64 7563 7420 636f  pp to conduct co
-00000290: 6e73 656e 7420 636f 6d70 6f6e 656e 7420  nsent component 
-000002a0: 666f 7220 7765 622d 636f 6f6b 6965 732e  for web-cookies.
-000002b0: 0a44 6574 6169 6c65 6420 646f 6375 6d65  .Detailed docume
-000002c0: 6e74 6174 696f 6e20 6973 2069 6e20 7468  ntation is in th
-000002d0: 6520 2264 6f63 7322 2064 6972 6563 746f  e "docs" directo
-000002e0: 7279 2e0a 0a23 2320 5175 6963 6b20 7374  ry...## Quick st
-000002f0: 6172 740a 0a31 2e20 4164 6420 2263 6f6f  art..1. Add "coo
-00000300: 6b69 655c 5f63 6f6e 7365 6e74 2220 746f  kie\_consent" to
-00000310: 2079 6f75 7220 6049 4e53 5441 4c4c 4544   your `INSTALLED
-00000320: 5f41 5050 5360 2073 6574 7469 6e67 206c  _APPS` setting l
-00000330: 696b 6520 7468 6973 3a3a 0a60 6060 0a20  ike this::.```. 
-00000340: 2020 2049 4e53 5441 4c4c 4544 5f41 5050     INSTALLED_APP
-00000350: 5320 3d20 5b0a 2020 2020 2020 2020 2263  S = [.        "c
-00000360: 6f6f 6b69 655f 636f 6e73 656e 7422 2c0a  ookie_consent",.
-00000370: 2020 2020 2020 2020 2e2e 2e2c 0a20 2020          ...,.   
-00000380: 205d 0a60 6060 0a32 2e20 496e 636c 7564   ].```.2. Includ
-00000390: 6520 7468 6520 636f 6f6b 6965 5c5f 636f  e the cookie\_co
-000003a0: 6e73 656e 7420 5552 4c63 6f6e 6620 696e  nsent URLconf in
-000003b0: 2079 6f75 7220 7072 6f6a 6563 7420 7572   your project ur
-000003c0: 6c73 2e70 7920 6c69 6b65 2074 6869 733a  ls.py like this:
-000003d0: 3a0a 6060 600a 2020 2020 7061 7468 2822  :.```.    path("
-000003e0: 636f 6f6b 6965 5f63 6f6e 7365 6e74 2f22  cookie_consent/"
-000003f0: 2c20 696e 636c 7564 6528 2263 6f6f 6b69  , include("cooki
-00000400: 655f 636f 6e73 656e 742e 7572 6c73 2229  e_consent.urls")
-00000410: 292c 0a60 6060 0a33 2e20 5275 6e20 6060  ),.```.3. Run ``
-00000420: 7079 7468 6f6e 206d 616e 6167 652e 7079  python manage.py
-00000430: 206d 6967 7261 7465 6060 2074 6f20 6372   migrate`` to cr
-00000440: 6561 7465 2074 6865 206d 6f64 656c 732e  eate the models.
-00000450: 0a34 2e20 5374 6172 7420 7468 6520 6465  .4. Start the de
-00000460: 7665 6c6f 706d 656e 7420 7365 7276 6572  velopment server
-00000470: 2061 6e64 2076 6973 6974 2068 7474 703a   and visit http:
-00000480: 2f2f 3132 372e 302e 302e 313a 3830 3030  //127.0.0.1:8000
-00000490: 2f2e 0a                                  /..
+00000280: 7070 2074 6f20 7368 6f77 2063 6f6e 7365  pp to show conse
+00000290: 6e74 2063 6f6d 706f 6e65 6e74 2066 6f72  nt component for
+000002a0: 2077 6562 2d63 6f6f 6b69 6573 2e0a 0a23   web-cookies...#
+000002b0: 2320 5175 6963 6b20 7374 6172 740a 0a31  # Quick start..1
+000002c0: 2e20 4164 6420 2263 6f6f 6b69 655c 5f63  . Add "cookie\_c
+000002d0: 6f6e 7365 6e74 2220 746f 2079 6f75 7220  onsent" to your 
+000002e0: 6049 4e53 5441 4c4c 4544 5f41 5050 5360  `INSTALLED_APPS`
+000002f0: 2073 6574 7469 6e67 206c 696b 6520 7468   setting like th
+00000300: 6973 3a0a 6060 600a 2020 2020 494e 5354  is:.```.    INST
+00000310: 414c 4c45 445f 4150 5053 203d 205b 0a20  ALLED_APPS = [. 
+00000320: 2020 2020 2020 2022 636f 6f6b 6965 5f63         "cookie_c
+00000330: 6f6e 7365 6e74 222c 0a20 2020 2020 2020  onsent",.       
+00000340: 202e 2e2e 2c0a 2020 2020 5d0a 6060 600a   ...,.    ].```.
+00000350: 322e 2049 6e63 6c75 6465 2074 6865 2063  2. Include the c
+00000360: 6f6f 6b69 655c 5f63 6f6e 7365 6e74 2055  ookie\_consent U
+00000370: 524c 636f 6e66 2069 6e20 796f 7572 2070  RLconf in your p
+00000380: 726f 6a65 6374 2075 726c 732e 7079 206c  roject urls.py l
+00000390: 696b 6520 7468 6973 3a0a 6060 600a 2020  ike this:.```.  
+000003a0: 2020 7061 7468 2822 636f 6f6b 6965 5f63    path("cookie_c
+000003b0: 6f6e 7365 6e74 2f22 2c20 696e 636c 7564  onsent/", includ
+000003c0: 6528 2263 6f6f 6b69 655f 636f 6e73 656e  e("cookie_consen
+000003d0: 742e 7572 6c73 2229 292c 0a60 6060 0a33  t.urls")),.```.3
+000003e0: 2e20 5275 6e20 6070 7974 686f 6e20 6d61  . Run `python ma
+000003f0: 6e61 6765 2e70 7920 6d69 6772 6174 6560  nage.py migrate`
+00000400: 2074 6f20 6372 6561 7465 2074 6865 206d   to create the m
+00000410: 6f64 656c 732e 0a34 2e20 496e 636c 7564  odels..4. Includ
+00000420: 6520 636f 6e73 656e 7420 7465 6d70 6c61  e consent templa
+00000430: 7465 2069 6e20 796f 7572 2077 6562 2d73  te in your web-s
+00000440: 6974 6520 7465 6d70 6c61 7465 732e 0a20  ite templates.. 
+00000450: 200a 2020 466f 7220 6578 616d 706c 652c   .  For example,
+00000460: 2049 2776 6520 696e 636c 7564 6564 2074   I've included t
+00000470: 6861 7420 7465 7874 2069 6e20 6d79 2062  hat text in my b
+00000480: 6173 6520 7465 6d70 6c61 7465 3a0a 0a20  ase template:.. 
+00000490: 2060 6060 0a20 207b 2520 626c 6f63 6b20   ```.  {% block 
+000004a0: 636f 6f6b 6965 5f63 6f6e 7365 6e74 2025  cookie_consent %
+000004b0: 7d0a 2020 2020 3c6c 696e 6b20 7265 6c3d  }.    <link rel=
+000004c0: 2273 7479 6c65 7368 6565 7422 2068 7265  "stylesheet" hre
+000004d0: 663d 227b 2520 7374 6174 6963 2027 636f  f="{% static 'co
+000004e0: 6f6b 6965 5f63 6f6e 7365 6e74 2f63 7373  okie_consent/css
+000004f0: 2f69 6e64 6578 2e63 7373 2720 257d 223e  /index.css' %}">
+00000500: 0a20 2020 207b 2520 696e 636c 7564 6520  .    {% include 
+00000510: 2763 6f6f 6b69 655f 636f 6e73 656e 742f  'cookie_consent/
+00000520: 696e 636c 7564 6573 2f63 6f6e 7365 6e74  includes/consent
+00000530: 2e68 746d 6c27 2025 7d0a 2020 2020 3c73  .html' %}.    <s
+00000540: 6372 6970 7420 7479 7065 3d22 6d6f 6475  cript type="modu
+00000550: 6c65 2220 7372 633d 222f 6173 7365 7473  le" src="/assets
+00000560: 2f6a 732f 746f 6f6c 6b69 742f 636f 6f6b  /js/toolkit/cook
+00000570: 6965 5f63 6f6e 7365 6e74 2e6a 7322 3e3c  ie_consent.js"><
+00000580: 2f73 6372 6970 743e 0a20 207b 2520 656e  /script>.  {% en
+00000590: 6462 6c6f 636b 2025 7d0a 2020 6060 600a  dblock %}.  ```.
+000005a0: 352e 2053 7461 7274 2074 6865 2064 6576  5. Start the dev
+000005b0: 656c 6f70 6d65 6e74 2073 6572 7665 7220  elopment server 
+000005c0: 616e 6420 7669 7369 7420 6e65 6365 7373  and visit necess
+000005d0: 6172 7920 7061 6765 732e 0a              ary pages..
```

### Comparing `django-cookie_consent_gutsh-0.0.2/cookie_consent/migrations/0001_initial.py` & `django-cookie_consent_gutsh-0.1.0/cookie_consent/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cookie_consent_gutsh-0.0.2/cookie_consent/templates/cookie_consent/includes/consent.html` & `django-cookie_consent_gutsh-0.1.0/cookie_consent/templates/cookie_consent/includes/consent.html`

 * *Files identical despite different names*

### Comparing `django-cookie_consent_gutsh-0.0.2/cookie_consent/views.py` & `django-cookie_consent_gutsh-0.1.0/cookie_consent/views.py`

 * *Files identical despite different names*

### Comparing `django-cookie_consent_gutsh-0.0.2/django_cookie_consent_gutsh.egg-info/PKG-INFO` & `django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
 00000020: 676f 2d63 6f6f 6b69 652d 636f 6e73 656e  go-cookie-consen
 00000030: 742d 6775 7473 680a 5665 7273 696f 6e3a  t-gutsh.Version:
-00000040: 2030 2e30 2e32 0a53 756d 6d61 7279 3a20   0.0.2.Summary: 
+00000040: 2030 2e31 2e30 0a53 756d 6d61 7279 3a20   0.1.0.Summary: 
 00000050: 436f 6f6b 6965 2063 6f6e 7365 6e74 2063  Cookie consent c
 00000060: 6f6d 706f 6e65 6e74 2066 6f72 2061 6e79  omponent for any
 00000070: 2044 6a61 6e67 6f20 7765 622d 7369 7465   Django web-site
 00000080: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
 00000090: 733a 2f2f 7777 772e 6261 7273 6b69 796c  s://www.barskiyl
 000000a0: 6162 2e63 6f6d 2f0a 4175 7468 6f72 3a20  ab.com/.Author: 
 000000b0: 4172 7465 6d20 4261 7273 6b69 690a 4175  Artem Barskii.Au
@@ -34,41 +34,61 @@
 00000210: 2e38 0a44 6573 6372 6970 7469 6f6e 2d43  .8.Description-C
 00000220: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
 00000230: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
 00000240: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
 00000250: 0a0a 2320 436f 6f6b 6965 2063 6f6e 7365  ..# Cookie conse
 00000260: 6e74 0a0a 436f 6f6b 6965 2063 6f6e 7365  nt..Cookie conse
 00000270: 6e74 2069 7320 6120 446a 616e 676f 2061  nt is a Django a
-00000280: 7070 2074 6f20 636f 6e64 7563 7420 636f  pp to conduct co
-00000290: 6e73 656e 7420 636f 6d70 6f6e 656e 7420  nsent component 
-000002a0: 666f 7220 7765 622d 636f 6f6b 6965 732e  for web-cookies.
-000002b0: 0a44 6574 6169 6c65 6420 646f 6375 6d65  .Detailed docume
-000002c0: 6e74 6174 696f 6e20 6973 2069 6e20 7468  ntation is in th
-000002d0: 6520 2264 6f63 7322 2064 6972 6563 746f  e "docs" directo
-000002e0: 7279 2e0a 0a23 2320 5175 6963 6b20 7374  ry...## Quick st
-000002f0: 6172 740a 0a31 2e20 4164 6420 2263 6f6f  art..1. Add "coo
-00000300: 6b69 655c 5f63 6f6e 7365 6e74 2220 746f  kie\_consent" to
-00000310: 2079 6f75 7220 6049 4e53 5441 4c4c 4544   your `INSTALLED
-00000320: 5f41 5050 5360 2073 6574 7469 6e67 206c  _APPS` setting l
-00000330: 696b 6520 7468 6973 3a3a 0a60 6060 0a20  ike this::.```. 
-00000340: 2020 2049 4e53 5441 4c4c 4544 5f41 5050     INSTALLED_APP
-00000350: 5320 3d20 5b0a 2020 2020 2020 2020 2263  S = [.        "c
-00000360: 6f6f 6b69 655f 636f 6e73 656e 7422 2c0a  ookie_consent",.
-00000370: 2020 2020 2020 2020 2e2e 2e2c 0a20 2020          ...,.   
-00000380: 205d 0a60 6060 0a32 2e20 496e 636c 7564   ].```.2. Includ
-00000390: 6520 7468 6520 636f 6f6b 6965 5c5f 636f  e the cookie\_co
-000003a0: 6e73 656e 7420 5552 4c63 6f6e 6620 696e  nsent URLconf in
-000003b0: 2079 6f75 7220 7072 6f6a 6563 7420 7572   your project ur
-000003c0: 6c73 2e70 7920 6c69 6b65 2074 6869 733a  ls.py like this:
-000003d0: 3a0a 6060 600a 2020 2020 7061 7468 2822  :.```.    path("
-000003e0: 636f 6f6b 6965 5f63 6f6e 7365 6e74 2f22  cookie_consent/"
-000003f0: 2c20 696e 636c 7564 6528 2263 6f6f 6b69  , include("cooki
-00000400: 655f 636f 6e73 656e 742e 7572 6c73 2229  e_consent.urls")
-00000410: 292c 0a60 6060 0a33 2e20 5275 6e20 6060  ),.```.3. Run ``
-00000420: 7079 7468 6f6e 206d 616e 6167 652e 7079  python manage.py
-00000430: 206d 6967 7261 7465 6060 2074 6f20 6372   migrate`` to cr
-00000440: 6561 7465 2074 6865 206d 6f64 656c 732e  eate the models.
-00000450: 0a34 2e20 5374 6172 7420 7468 6520 6465  .4. Start the de
-00000460: 7665 6c6f 706d 656e 7420 7365 7276 6572  velopment server
-00000470: 2061 6e64 2076 6973 6974 2068 7474 703a   and visit http:
-00000480: 2f2f 3132 372e 302e 302e 313a 3830 3030  //127.0.0.1:8000
-00000490: 2f2e 0a                                  /..
+00000280: 7070 2074 6f20 7368 6f77 2063 6f6e 7365  pp to show conse
+00000290: 6e74 2063 6f6d 706f 6e65 6e74 2066 6f72  nt component for
+000002a0: 2077 6562 2d63 6f6f 6b69 6573 2e0a 0a23   web-cookies...#
+000002b0: 2320 5175 6963 6b20 7374 6172 740a 0a31  # Quick start..1
+000002c0: 2e20 4164 6420 2263 6f6f 6b69 655c 5f63  . Add "cookie\_c
+000002d0: 6f6e 7365 6e74 2220 746f 2079 6f75 7220  onsent" to your 
+000002e0: 6049 4e53 5441 4c4c 4544 5f41 5050 5360  `INSTALLED_APPS`
+000002f0: 2073 6574 7469 6e67 206c 696b 6520 7468   setting like th
+00000300: 6973 3a0a 6060 600a 2020 2020 494e 5354  is:.```.    INST
+00000310: 414c 4c45 445f 4150 5053 203d 205b 0a20  ALLED_APPS = [. 
+00000320: 2020 2020 2020 2022 636f 6f6b 6965 5f63         "cookie_c
+00000330: 6f6e 7365 6e74 222c 0a20 2020 2020 2020  onsent",.       
+00000340: 202e 2e2e 2c0a 2020 2020 5d0a 6060 600a   ...,.    ].```.
+00000350: 322e 2049 6e63 6c75 6465 2074 6865 2063  2. Include the c
+00000360: 6f6f 6b69 655c 5f63 6f6e 7365 6e74 2055  ookie\_consent U
+00000370: 524c 636f 6e66 2069 6e20 796f 7572 2070  RLconf in your p
+00000380: 726f 6a65 6374 2075 726c 732e 7079 206c  roject urls.py l
+00000390: 696b 6520 7468 6973 3a0a 6060 600a 2020  ike this:.```.  
+000003a0: 2020 7061 7468 2822 636f 6f6b 6965 5f63    path("cookie_c
+000003b0: 6f6e 7365 6e74 2f22 2c20 696e 636c 7564  onsent/", includ
+000003c0: 6528 2263 6f6f 6b69 655f 636f 6e73 656e  e("cookie_consen
+000003d0: 742e 7572 6c73 2229 292c 0a60 6060 0a33  t.urls")),.```.3
+000003e0: 2e20 5275 6e20 6070 7974 686f 6e20 6d61  . Run `python ma
+000003f0: 6e61 6765 2e70 7920 6d69 6772 6174 6560  nage.py migrate`
+00000400: 2074 6f20 6372 6561 7465 2074 6865 206d   to create the m
+00000410: 6f64 656c 732e 0a34 2e20 496e 636c 7564  odels..4. Includ
+00000420: 6520 636f 6e73 656e 7420 7465 6d70 6c61  e consent templa
+00000430: 7465 2069 6e20 796f 7572 2077 6562 2d73  te in your web-s
+00000440: 6974 6520 7465 6d70 6c61 7465 732e 0a20  ite templates.. 
+00000450: 200a 2020 466f 7220 6578 616d 706c 652c   .  For example,
+00000460: 2049 2776 6520 696e 636c 7564 6564 2074   I've included t
+00000470: 6861 7420 7465 7874 2069 6e20 6d79 2062  hat text in my b
+00000480: 6173 6520 7465 6d70 6c61 7465 3a0a 0a20  ase template:.. 
+00000490: 2060 6060 0a20 207b 2520 626c 6f63 6b20   ```.  {% block 
+000004a0: 636f 6f6b 6965 5f63 6f6e 7365 6e74 2025  cookie_consent %
+000004b0: 7d0a 2020 2020 3c6c 696e 6b20 7265 6c3d  }.    <link rel=
+000004c0: 2273 7479 6c65 7368 6565 7422 2068 7265  "stylesheet" hre
+000004d0: 663d 227b 2520 7374 6174 6963 2027 636f  f="{% static 'co
+000004e0: 6f6b 6965 5f63 6f6e 7365 6e74 2f63 7373  okie_consent/css
+000004f0: 2f69 6e64 6578 2e63 7373 2720 257d 223e  /index.css' %}">
+00000500: 0a20 2020 207b 2520 696e 636c 7564 6520  .    {% include 
+00000510: 2763 6f6f 6b69 655f 636f 6e73 656e 742f  'cookie_consent/
+00000520: 696e 636c 7564 6573 2f63 6f6e 7365 6e74  includes/consent
+00000530: 2e68 746d 6c27 2025 7d0a 2020 2020 3c73  .html' %}.    <s
+00000540: 6372 6970 7420 7479 7065 3d22 6d6f 6475  cript type="modu
+00000550: 6c65 2220 7372 633d 222f 6173 7365 7473  le" src="/assets
+00000560: 2f6a 732f 746f 6f6c 6b69 742f 636f 6f6b  /js/toolkit/cook
+00000570: 6965 5f63 6f6e 7365 6e74 2e6a 7322 3e3c  ie_consent.js"><
+00000580: 2f73 6372 6970 743e 0a20 207b 2520 656e  /script>.  {% en
+00000590: 6462 6c6f 636b 2025 7d0a 2020 6060 600a  dblock %}.  ```.
+000005a0: 352e 2053 7461 7274 2074 6865 2064 6576  5. Start the dev
+000005b0: 656c 6f70 6d65 6e74 2073 6572 7665 7220  elopment server 
+000005c0: 616e 6420 7669 7369 7420 6e65 6365 7373  and visit necess
+000005d0: 6172 7920 7061 6765 732e 0a              ary pages..
```

### Comparing `django-cookie_consent_gutsh-0.0.2/django_cookie_consent_gutsh.egg-info/SOURCES.txt` & `django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cookie_consent_gutsh-0.0.2/pyproject.toml` & `django-cookie_consent_gutsh-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-cookie_consent_gutsh"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
     { name="Artem Barskii", email="artemiy.barskiy@gmail.com" },
 ]
 description = "Cookie consent component for any Django web-site"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `django-cookie_consent_gutsh-0.0.2/setup.cfg` & `django-cookie_consent_gutsh-0.1.0/setup.cfg`

 * *Files identical despite different names*

