# Comparing `tmp/onvif-zeep-async-1.2.8.tar.gz` & `tmp/onvif-zeep-async-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-1.2.8.tar", last modified: Sat Apr 15 19:55:24 2023, max compression
+gzip compressed data, was "onvif-zeep-async-1.2.9.tar", last modified: Sat Apr 15 22:40:29 2023, max compression
```

## Comparing `onvif-zeep-async-1.2.8.tar` & `onvif-zeep-async-1.2.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 19:55:24.545513 onvif-zeep-async-1.2.8/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-1.2.8/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-1.2.8/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-15 19:55:24.545560 onvif-zeep-async-1.2.8/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 19:55:24.536796 onvif-zeep-async-1.2.8/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 19:55:24.537451 onvif-zeep-async-1.2.8/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    19158 2023-04-15 19:53:35.000000 onvif-zeep-async-1.2.8/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-15 19:55:02.000000 onvif-zeep-async-1.2.8/onvif/version.txt
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 19:55:24.544419 onvif-zeep-async-1.2.8/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 19:55:24.545293 onvif-zeep-async-1.2.8/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-15 19:55:24.000000 onvif-zeep-async-1.2.8/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1417 2023-04-15 19:55:24.000000 onvif-zeep-async-1.2.8/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-04-15 19:55:24.000000 onvif-zeep-async-1.2.8/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-04-15 19:55:24.000000 onvif-zeep-async-1.2.8/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-1.2.8/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-04-15 19:55:24.000000 onvif-zeep-async-1.2.8/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-15 19:55:24.000000 onvif-zeep-async-1.2.8/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-04-15 19:55:24.545791 onvif-zeep-async-1.2.8/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 19:55:24.545400 onvif-zeep-async-1.2.8/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.8/tests/test.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 22:40:29.727860 onvif-zeep-async-1.2.9/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-1.2.9/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-1.2.9/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-15 22:40:29.727908 onvif-zeep-async-1.2.9/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 22:40:29.719304 onvif-zeep-async-1.2.9/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 22:40:29.719973 onvif-zeep-async-1.2.9/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    20526 2023-04-15 22:40:06.000000 onvif-zeep-async-1.2.9/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-15 22:40:10.000000 onvif-zeep-async-1.2.9/onvif/version.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 22:40:29.726644 onvif-zeep-async-1.2.9/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 22:40:29.727602 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-15 22:40:29.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1417 2023-04-15 22:40:29.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-04-15 22:40:29.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-04-15 22:40:29.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-04-15 22:40:29.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-15 22:40:29.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-04-15 22:40:29.728137 onvif-zeep-async-1.2.9/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 22:40:29.727731 onvif-zeep-async-1.2.9/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/tests/test.py
```

### Comparing `onvif-zeep-async-1.2.8/.gitignore` & `onvif-zeep-async-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/.pre-commit-config.yaml` & `onvif-zeep-async-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/LICENSE` & `onvif-zeep-async-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/Makefile` & `onvif-zeep-async-1.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/PKG-INFO` & `onvif-zeep-async-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 1.2.8
+Version: 1.2.9
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-1.2.8/README.rst` & `onvif-zeep-async-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/examples/events.py` & `onvif-zeep-async-1.2.9/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/examples/rotate_image.py` & `onvif-zeep-async-1.2.9/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/examples/streaming.py` & `onvif-zeep-async-1.2.9/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/__init__.py` & `onvif-zeep-async-1.2.9/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/client.py` & `onvif-zeep-async-1.2.9/onvif/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,34 +2,40 @@
 import asyncio
 import contextlib
 import datetime as dt
 from functools import lru_cache
 import logging
 import os.path
 import ssl
-from typing import Any, Dict, Optional, Tuple
+from typing import IO, Any, Dict, Optional, Tuple, Union
 
 import httpx
 from httpx import AsyncClient, BasicAuth, DigestAuth
 from zeep.cache import SqliteCache
 from zeep.client import AsyncClient as BaseZeepAsyncClient, Settings
 from zeep.exceptions import Fault
 import zeep.helpers
+from zeep.loader import parse_xml
 from zeep.proxy import AsyncServiceProxy
 from zeep.transports import AsyncTransport
 from zeep.wsa import WsAddressingPlugin
+from zeep.wsdl import Document
 from zeep.wsse.username import UsernameToken
 
 from onvif.definition import SERVICES
 from onvif.exceptions import ONVIFAuthError, ONVIFError, ONVIFTimeoutError
 
 logger = logging.getLogger("onvif")
 logging.basicConfig(level=logging.INFO)
 logging.getLogger("zeep.client").setLevel(logging.CRITICAL)
 
+_DEFAULT_SETTINGS = Settings()
+_DEFAULT_SETTINGS.strict = False
+_DEFAULT_SETTINGS.xml_huge_tree = True
+
 
 def create_no_verify_ssl_context() -> ssl.SSLContext:
     """Return an SSL context that does not verify the server certificate.
     This is a copy of aiohttp's create_default_context() function, with the
     ssl verify turned off and old SSL versions enabled.
 
     https://github.com/aio-libs/aiohttp/blob/33953f110e97eecc707e1402daa8d543f38a189b/aiohttp/connector.py#L911
@@ -81,14 +87,49 @@
         if self.dt_diff is not None:
             self.created += self.dt_diff
         result = super().apply(envelope, headers)
         self.created = old_created
         return result
 
 
+class AsyncSafeTransport:
+    """A transport that blocks all I/O for zeep."""
+
+    def load(self, *args: Any, **kwargs: Any) -> None:
+        """Load the given XML document.
+
+        This should never be called, but we want to raise
+        an error if it is so we know we're doing something wrong
+        and do not accidentally block the event loop.
+        """
+        raise RuntimeError("Loading is not supported in async mode")
+
+
+_ASYNC_TRANSPORT = AsyncSafeTransport()
+
+
+@lru_cache(maxsize=128)
+def _cached_parse_xml(path: str) -> Any:
+    """Load external XML document from disk."""
+    with open(os.path.expanduser(path), "rb") as fh:
+        return parse_xml(fh.read(), _ASYNC_TRANSPORT, settings=_DEFAULT_SETTINGS)
+
+
+class DocumentWithCache(Document):
+    """A WSDL document that supports caching."""
+
+    def _get_xml_document(self, url: Union[IO, str]) -> Any:
+        """Load external XML document from a file-like object or URL."""
+        if _path_isfile(url):
+            return _cached_parse_xml(url)
+        raise RuntimeError(
+            f"Cannot fetch {url} in async mode because it would block the event loop"
+        )
+
+
 class ZeepAsyncClient(BaseZeepAsyncClient):
     """Overwrite create_service method to be async."""
 
     def create_service(self, binding_name, address):
         """Create a new ServiceProxy for the given binding name and address.
         :param binding_name: The QName of the binding
         :param address: The address of the endpoint
@@ -170,29 +211,26 @@
         self.transport = (
             AsyncTransport(client=client, wsdl_client=wsdl_client)
             if no_cache
             else AsyncTransport(
                 client=client, wsdl_client=wsdl_client, cache=SqliteCache()
             )
         )
-        settings = Settings()
-        settings.strict = False
-        settings.xml_huge_tree = True
+        settings = _DEFAULT_SETTINGS
         self.zeep_client_authless = ZeepAsyncClient(
-            wsdl=url,
+            wsdl=DocumentWithCache(url, self.transport, settings=settings),
             transport=self.transport,
             settings=settings,
             plugins=[WsAddressingPlugin()],
         )
         self.ws_client_authless = self.zeep_client_authless.create_service(
             binding_name, self.xaddr
         )
-
         self.zeep_client = ZeepAsyncClient(
-            wsdl=url,
+            wsdl=DocumentWithCache(url, self.transport, settings=settings),
             wsse=wsse,
             transport=self.transport,
             settings=settings,
             plugins=[WsAddressingPlugin()],
         )
         self.ws_client = self.zeep_client.create_service(binding_name, self.xaddr)
```

### Comparing `onvif-zeep-async-1.2.8/onvif/definition.py` & `onvif-zeep-async-1.2.9/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/exceptions.py` & `onvif-zeep-async-1.2.9/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/addressing` & `onvif-zeep-async-1.2.9/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-1.2.9/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-1.2.9/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/display.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/envelope` & `onvif-zeep-async-1.2.9/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/events.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/media.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-1.2.9/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-1.2.9/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/search.wsdl` & `onvif-zeep-async-1.2.9/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-1.2.9/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/types.xsd` & `onvif-zeep-async-1.2.9/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-1.2.9/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-1.2.9/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/xml.xsd` & `onvif-zeep-async-1.2.9/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif/wsdl/xmlmime` & `onvif-zeep-async-1.2.9/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 1.2.8
+Version: 1.2.9
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-1.2.8/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/pylintrc` & `onvif-zeep-async-1.2.9/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/setup.py` & `onvif-zeep-async-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.8/tests/test.py` & `onvif-zeep-async-1.2.9/tests/test.py`

 * *Files identical despite different names*

