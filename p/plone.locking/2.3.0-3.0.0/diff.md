# Comparing `tmp/plone.locking-2.3.0.tar.gz` & `tmp/plone.locking-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.locking-2.3.0.tar", last modified: Tue Feb  7 23:12:30 2023, max compression
+gzip compressed data, was "plone.locking-3.0.0.tar", last modified: Sat Apr 15 22:03:12 2023, max compression
```

## Comparing `plone.locking-2.3.0.tar` & `plone.locking-3.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:12:30.265578 plone.locking-2.3.0/
--rw-r--r--   0 maurits    (501) staff       (20)     4164 2023-02-07 23:12:29.000000 plone.locking-2.3.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-02-07 23:12:29.000000 plone.locking-2.3.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-02-07 23:12:29.000000 plone.locking-2.3.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     5896 2023-02-07 23:12:30.265741 plone.locking-2.3.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      583 2023-02-07 23:12:29.000000 plone.locking-2.3.0/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:12:30.256508 plone.locking-2.3.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-02-07 23:12:29.000000 plone.locking-2.3.0/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      675 2023-02-07 23:12:29.000000 plone.locking-2.3.0/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:12:30.256914 plone.locking-2.3.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)      244 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:12:30.262173 plone.locking-2.3.0/plone/locking/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:12:30.263715 plone.locking-2.3.0/plone/locking/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1838 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/browser/info.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1224 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/browser/info.py
--rw-r--r--   0 maurits    (501) staff       (20)     6196 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/browser/locking.py
--rw-r--r--   0 maurits    (501) staff       (20)     1062 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      548 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/events.py
--rw-r--r--   0 maurits    (501) staff       (20)     4161 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     6002 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/lockable.py
--rw-r--r--   0 maurits    (501) staff       (20)      974 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:12:30.265254 plone.locking-2.3.0/plone/locking/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     6839 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/tests/locking.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1192 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/tests/test_functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     1651 2023-02-07 23:12:29.000000 plone.locking-2.3.0/plone/locking/tests/test_views.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:12:30.259793 plone.locking-2.3.0/plone.locking.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     5896 2023-02-07 23:12:30.000000 plone.locking-2.3.0/plone.locking.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      825 2023-02-07 23:12:30.000000 plone.locking-2.3.0/plone.locking.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-07 23:12:30.000000 plone.locking-2.3.0/plone.locking.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-02-07 23:12:30.000000 plone.locking-2.3.0/plone.locking.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-07 23:12:30.000000 plone.locking-2.3.0/plone.locking.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      198 2023-02-07 23:12:30.000000 plone.locking-2.3.0/plone.locking.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-02-07 23:12:30.000000 plone.locking-2.3.0/plone.locking.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-02-07 23:12:29.000000 plone.locking-2.3.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      123 2023-02-07 23:12:30.266368 plone.locking-2.3.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1973 2023-02-07 23:12:29.000000 plone.locking-2.3.0/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 22:03:12.908931 plone.locking-3.0.0/
+-rw-r--r--   0 gil       (1000) gil       (1000)     4421 2023-04-15 22:03:12.000000 plone.locking-3.0.0/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 22:03:12.000000 plone.locking-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      149 2023-04-15 22:03:12.000000 plone.locking-3.0.0/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)     5912 2023-04-15 22:03:12.908931 plone.locking-3.0.0/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      563 2023-04-15 22:03:12.000000 plone.locking-3.0.0/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 22:03:12.906931 plone.locking-3.0.0/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)    15220 2023-04-15 22:03:12.000000 plone.locking-3.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      675 2023-04-15 22:03:12.000000 plone.locking-3.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 22:03:12.906931 plone.locking-3.0.0/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)      245 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 22:03:12.907930 plone.locking-3.0.0/plone/locking/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 22:03:12.908931 plone.locking-3.0.0/plone/locking/browser/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/browser/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2130 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/browser/info.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1201 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/browser/info.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6126 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/browser/locking.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1039 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)      540 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/events.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4067 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6090 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/lockable.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      900 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 22:03:12.908931 plone.locking-3.0.0/plone/locking/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6839 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/tests/locking.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)     1270 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/tests/test_functional.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1626 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone/locking/tests/test_views.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 22:03:12.907930 plone.locking-3.0.0/plone.locking.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)     5912 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone.locking.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      825 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone.locking.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone.locking.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone.locking.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone.locking.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      107 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone.locking.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 22:03:12.000000 plone.locking-3.0.0/plone.locking.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2900 2023-04-15 22:03:12.000000 plone.locking-3.0.0/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 22:03:12.909931 plone.locking-3.0.0/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1510 2023-04-15 22:03:12.000000 plone.locking-3.0.0/setup.py
```

### Comparing `plone.locking-2.3.0/CHANGES.rst` & `plone.locking-3.0.0/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,37 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.0 (2023-04-16)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7. (#1)
+
+
+New features:
+
+
+- Update the info viewlet css classes to Bootstrap 5.
+  [ewohnlich] (bs5)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (234bb1d6, 5cc689e5)
+
+
 2.3.0 (2023-02-08)
 ------------------
 
 Bug fixes:
 
 
 - Update to Zope4 only including troove classifiers. [jensens] (#19)
```

### Comparing `plone.locking-2.3.0/PKG-INFO` & `plone.locking-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,81 @@
 Metadata-Version: 2.1
 Name: plone.locking
-Version: 2.3.0
+Version: 3.0.0
 Summary: webdav locking support
 Home-page: https://pypi.org/project/plone.locking
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: locking webdav plone
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
-Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Overview
 ========
 
 Provides basic automatic locking support for Plone. Locks are stealable by
 default, meaning that a user with edit privileges will be able to steal
 another user's lock, but will be warned that someone else may be editing
 the same object. Used by Plone, Archetypes and plone.app.iterate
 
-Compatibility
--------------
+Version Information
+-------------------
 
-The versions 2.1.x (built from the master-branch) are used in Plone 5 and are not compatible with earlier Plone versions.
-
-Versions 2.0.x are used by Plone 4.x (but *may* also be compatible with earlier versions).
-
-Versions 1.x are used by Plone 3.
+- 3.x -> Plone 6.0+ only
+- 2.3.x -> used in Plone 5+ (not compatible with earlier Plone versions)
+- 2.0.x -> used by Plone 4.x (but *may* also be compatible with earlier versions).
+- Versions 1.x are used by Plone 3.
 
 Changelog
 =========
 
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.0 (2023-04-16)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7. (#1)
+
+
+New features:
+
+
+- Update the info viewlet css classes to Bootstrap 5.
+  [ewohnlich] (bs5)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (234bb1d6, 5cc689e5)
+
+
 2.3.0 (2023-02-08)
 ------------------
 
 Bug fixes:
 
 
 - Update to Zope4 only including troove classifiers. [jensens] (#19)
```

### Comparing `plone.locking-2.3.0/docs/LICENSE.GPL` & `plone.locking-3.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.locking-2.3.0/docs/LICENSE.txt` & `plone.locking-3.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.locking-2.3.0/plone/locking/browser/info.pt` & `plone.locking-3.0.0/plone/locking/browser/info.pt`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 <div id="plone-lock-status"
+     tal:define="
+       locked view/info/is_locked_for_current_user;
+       stealable view/lock_is_stealable;
+       lock_details view/lock_info;
+       icons python:context.restrictedTraverse('@@iconresolver');
+     "
      i18n:domain="plone"
-     tal:define="locked view/info/is_locked_for_current_user;
-                 stealable view/lock_is_stealable;
-                 lock_details view/lock_info;">
+>
   <tal:block condition="locked">
-    <dl class="portalMessage info">
-      <dt i18n:translate="label_locked">Locked</dt>
-      <dd>
-        <tal:author-page
-            tal:condition="lock_details/author_page"
-            i18n:translate="description_webdav_locked_by_author_on_time">
+    <div class="portalMessage info alert alert-info">
+      <tal:icon tal:replace="structure python:icons.tag('lock-fill', tag_alt='locked', tag_class='mb-1 me-2')" />
+      <strong i18n:translate="label_locked">Locked</strong>
+      <tal:author-page tal:condition="lock_details/author_page"
+                       i18n:translate="description_webdav_locked_by_author_on_time"
+      >
           This item was locked by
-          <a i18n:name="author"
-             tal:content="lock_details/fullname"
-             tal:attributes="href lock_details/author_page" />
-          <span i18n:name="time"
-                tal:content="lock_details/time_difference" /> ago.
-        </tal:author-page>
-        <tal:no-author-page
-            tal:condition="not:lock_details/author_page"
-            i18n:translate="description_webdav_locked_by_author_on_time">
+        <a tal:content="lock_details/fullname"
+           tal:attributes="
+             href lock_details/author_page;
+           "
+           i18n:name="author"
+        ></a>
+        <span tal:content="lock_details/time_difference"
+              i18n:name="time"
+        ></span>
+         ago.
+      </tal:author-page>
+      <tal:no-author-page tal:condition="not:lock_details/author_page"
+                          i18n:translate="description_webdav_locked_by_author_on_time"
+      >
           This item was locked by
-          <span i18n:name="author"
-                tal:content="lock_details/fullname" />
-          <span i18n:name="time"
-                tal:content="lock_details/time_difference" /> ago.
-        </tal:no-author-page>
-        <form tal:condition="stealable"
-              tal:attributes="action string:${context/absolute_url}/@@plone_lock_operations/force_unlock"
-              method="POST">
-          <span i18n:translate="description_webdav_locked_steal">
+        <span tal:content="lock_details/fullname"
+              i18n:name="author"
+        ></span>
+        <span tal:content="lock_details/time_difference"
+              i18n:name="time"
+        ></span>
+         ago.
+      </tal:no-author-page>
+      <form method="POST"
+            tal:condition="stealable"
+            tal:attributes="
+              action string:${context/absolute_url}/@@plone_lock_operations/force_unlock;
+            "
+      >
+        <span i18n:translate="description_webdav_locked_steal">
             If you are certain this user has abandoned the object,
             you may
-            <input type="submit"
-                   value="Unlock"
-                   i18n:name="unlock_button"
-                   i18n:attributes="value" />
+          <input type="submit"
+                 value="Unlock"
+                 i18n:attributes="value"
+                 i18n:name="unlock_button"
+          />
             the object. You will then be able to edit it.
-          </span>
-        </form>
-      </dd>
-    </dl>
+        </span>
+      </form>
+    </div>
   </tal:block>
 </div>
```

### Comparing `plone.locking-2.3.0/plone/locking/browser/info.py` & `plone.locking-3.0.0/plone/locking/browser/info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-from zope.interface import implementer
-from zope.component import getMultiAdapter
-
-from zope.viewlet.interfaces import IViewlet
-
 from Products.Five.browser import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
+from zope.component import getMultiAdapter
+from zope.interface import implementer
+from zope.viewlet.interfaces import IViewlet
 
 
 @implementer(IViewlet)
 class LockInfoViewlet(BrowserView):
     """This is a viewlet which is not hooked up anywhere. It is referenced
     from plone.app.layout. We do it this way to avoid having the  lower-level
     plone.locking depend on these packages, whilst still providing
     an implementation of the info box in a single place.
     """
 
-    template = ViewPageTemplateFile('info.pt')
+    template = ViewPageTemplateFile("info.pt")
 
     def __init__(self, context, request, view, manager):
-        super(LockInfoViewlet, self).__init__(context, request)
+        super().__init__(context, request)
         self.__parent__ = view
         self.context = context
         self.request = request
         self.view = view
         self.manager = manager
         self.info = getMultiAdapter((context, request), name="plone_lock_info")
```

### Comparing `plone.locking-2.3.0/plone/locking/browser/locking.py` & `plone.locking-3.0.0/plone/locking/browser/locking.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,72 @@
-# -*- coding: utf-8 -*-
 from Acquisition import aq_inner
-from DateTime import DateTime
 from datetime import timedelta
+from DateTime import DateTime
 from plone.locking.interfaces import ILockable
 from plone.locking.interfaces import IRefreshableLockable
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
 from Products.Five import BrowserView
 from zope.component import getUtility
 from zope.i18nmessageid import MessageFactory
 
 
-_ = MessageFactory('plone')
+_ = MessageFactory("plone")
 
 
 class LockingOperations(BrowserView):
-    """Lock acquisition and stealing operations
-    """
+    """Lock acquisition and stealing operations"""
 
     def redirect(self):
-        """Redirect to the context view if needed
-        """
+        """Redirect to the context view if needed"""
         url = self.context.absolute_url()
         registry = getUtility(IRegistry)
-        types_use_view = registry.get(
-            'plone.types_use_view_action_in_listings', [])
+        types_use_view = registry.get("plone.types_use_view_action_in_listings", [])
         if self.context.portal_type in types_use_view:
-            url += '/view'
+            url += "/view"
         self.request.RESPONSE.redirect(url)
 
     def force_unlock(self, redirect=True):
         """Steal the lock.
 
         If redirect is True, redirect back to the context URL, i.e. reload
         the page.
         """
         lockable = ILockable(self.context)
         lockable.unlock()
         if redirect:
             self.redirect()
 
     def create_lock(self, redirect=True):
-        """Lock the object if it is unlocked
-        """
+        """Lock the object if it is unlocked"""
         lockable = IRefreshableLockable(self.context, None)
         if lockable is not None:
             lockable.lock()
         if redirect:
             self.redirect()
 
     def safe_unlock(self, redirect=True):
-        """Unlock the object if the current user has the lock
-        """
+        """Unlock the object if the current user has the lock"""
         lockable = ILockable(self.context)
         if lockable.can_safely_unlock():
             lockable.unlock()
         if redirect:
             self.redirect()
 
     def refresh_lock(self, redirect=True):
-        """Reset the lock start time
-        """
+        """Reset the lock start time"""
         lockable = IRefreshableLockable(self.context, None)
         if lockable is not None:
             lockable.refresh_lock()
         if redirect:
             self.redirect()
 
 
 class LockingInformation(BrowserView):
-    """Lock information
-    """
+    """Lock information"""
 
     def is_locked(self):
         lockable = ILockable(aq_inner(self.context))
         return lockable.locked()
 
     def is_locked_for_current_user(self):
         """True if this object is locked for the current user (i.e. the
@@ -83,87 +75,89 @@
         lockable = ILockable(aq_inner(self.context))
         # Faster version - we rely on the fact that can_safely_unlock() is
         # True even if the object is not locked
         return not lockable.can_safely_unlock()
         # return lockable.locked() and not lockable.can_safely_unlock()
 
     def lock_is_stealable(self):
-        """Find out if the lock is stealable
-        """
+        """Find out if the lock is stealable"""
         lockable = ILockable(self.context)
         return lockable.stealable()
 
     def lock_info(self):
         """Get information about the current lock, a dict containing:
 
         creator - the id of the user who created the lock
         fullname - the full name of the lock creator
         author_page - a link to the home page of the author
         time - the creation time of the lock
         time_difference - a string representing the time since the lock was
         acquired.
         """
 
-        portal_membership = getToolByName(self.context, 'portal_membership')
-        portal_url = getToolByName(self.context, 'portal_url')
+        portal_membership = getToolByName(self.context, "portal_membership")
+        portal_url = getToolByName(self.context, "portal_url")
         lockable = ILockable(aq_inner(self.context))
         url = portal_url()
         for info in lockable.lock_info():
-            creator = info['creator']
-            time = info['time']
-            token = info['token']
-            lock_type = info['type']
+            creator = info["creator"]
+            time = info["time"]
+            token = info["token"]
+            lock_type = info["type"]
             # Get the fullname, but remember that the creator may not
             # be a member, but only Authenticated or even anonymous.
             # Same for the author_page
-            fullname = ''
-            author_page = ''
+            fullname = ""
+            author_page = ""
             member = portal_membership.getMemberById(creator)
             if member:
-                fullname = member.getProperty('fullname', '')
-                author_page = "%s/author/%s" % (url, creator)
-            if fullname == '':
-                fullname = creator or _('label_an_anonymous_user',
-                                        u'an anonymous user')
+                fullname = member.getProperty("fullname", "")
+                author_page = f"{url}/author/{creator}"
+            if fullname == "":
+                fullname = creator or _("label_an_anonymous_user", "an anonymous user")
             time_difference = self._getNiceTimeDifference(time)
 
             return {
-                'creator': creator,
-                'fullname': fullname,
-                'author_page': author_page,
-                'time': time,
-                'time_difference': time_difference,
-                'token': token,
-                'type': lock_type,
+                "creator": creator,
+                "fullname": fullname,
+                "author_page": author_page,
+                "time": time,
+                "time_difference": time_difference,
+                "token": token,
+                "type": lock_type,
             }
 
     def _getNiceTimeDifference(self, baseTime):
         now = DateTime()
         days = int(round(now - DateTime(baseTime)))
         delta = timedelta(now - DateTime(baseTime))
         days = delta.days
         hours = delta.seconds // 3600
         minutes = (delta.seconds - (hours * 3600)) // 60
 
-        dateString = u""
+        dateString = ""
         if days == 0:
             if hours == 0:
                 if delta.seconds < 120:
-                    dateString = _(u"1 minute")
+                    dateString = _("1 minute")
                 else:
-                    dateString = _(u"$m minutes", mapping={'m': minutes})
+                    dateString = _("$m minutes", mapping={"m": minutes})
             elif hours == 1:
-                dateString = _(u"$h hour and $m minutes", mapping={'h': hours, 'm': minutes})  # noqa
+                dateString = _(
+                    "$h hour and $m minutes", mapping={"h": hours, "m": minutes}
+                )  # noqa
             else:
-                dateString = _(u"$h hours and $m minutes", mapping={'h': hours, 'm': minutes})  # noqa
+                dateString = _(
+                    "$h hours and $m minutes", mapping={"h": hours, "m": minutes}
+                )  # noqa
         else:
             if days == 1:
-                dateString = _(u"$d day and $h hours", mapping={'d': days, 'h': hours})
+                dateString = _("$d day and $h hours", mapping={"d": days, "h": hours})
             else:
-                dateString = _(u"$d days and $h hours", mapping={'d': days, 'h': hours})
+                dateString = _("$d days and $h hours", mapping={"d": days, "h": hours})
         return dateString
 
 
 class LockingInformationFallback(BrowserView):
     """Fallback view for Lock information.
 
     This view exists to return sensible defaults if a content type does
```

### Comparing `plone.locking-2.3.0/plone/locking/configure.zcml` & `plone.locking-3.0.0/plone/locking/configure.zcml`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:browser="http://namespaces.zope.org/browser">
+    xmlns:browser="http://namespaces.zope.org/browser"
+    >
 
-    <adapter factory=".lockable.TTWLockable" />
+  <adapter factory=".lockable.TTWLockable" />
 
-    <include package="Products.CMFCore" file="configure.zcml" />
-
-    <browser:page
-        for=".interfaces.ITTWLockable"
-        name="plone_lock_operations"
-        class=".browser.locking.LockingOperations"
-        permission="cmf.ModifyPortalContent"
-        allowed_attributes="create_lock safe_unlock force_unlock refresh_lock"
-        />
-
-    <browser:page
-        for=".interfaces.ITTWLockable"
-        name="plone_lock_info"
-        class=".browser.locking.LockingInformation"
-        permission="zope2.View"
-        allowed_attributes="is_locked is_locked_for_current_user lock_is_stealable lock_info"
-        />
-
-    <browser:page
-        for="*"
-        name="plone_lock_info"
-        class=".browser.locking.LockingInformationFallback"
-        permission="zope2.View"
-        allowed_attributes="is_locked is_locked_for_current_user lock_is_stealable lock_info"
-        />
+  <include
+      package="Products.CMFCore"
+      file="configure.zcml"
+      />
+
+  <browser:page
+      name="plone_lock_operations"
+      for=".interfaces.ITTWLockable"
+      class=".browser.locking.LockingOperations"
+      allowed_attributes="create_lock safe_unlock force_unlock refresh_lock"
+      permission="cmf.ModifyPortalContent"
+      />
+
+  <browser:page
+      name="plone_lock_info"
+      for=".interfaces.ITTWLockable"
+      class=".browser.locking.LockingInformation"
+      allowed_attributes="is_locked is_locked_for_current_user lock_is_stealable lock_info"
+      permission="zope2.View"
+      />
+
+  <browser:page
+      name="plone_lock_info"
+      for="*"
+      class=".browser.locking.LockingInformationFallback"
+      allowed_attributes="is_locked is_locked_for_current_user lock_is_stealable lock_info"
+      permission="zope2.View"
+      />
 
 </configure>
```

### Comparing `plone.locking-2.3.0/plone/locking/events.py` & `plone.locking-3.0.0/plone/locking/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from plone.locking.interfaces import ILockable
 
+
 # These event handlers are not connected by default, but can be used for
 # a particular object event (used e.g. in Archetypes)
 
+
 def lockOnEditBegins(obj, event):
-    """Lock the object when a user start working on the object
-    """
+    """Lock the object when a user start working on the object"""
     lockable = ILockable(obj)
     if not lockable.locked():
         lockable.lock()
 
 
 def unlockAfterModification(obj, event):
-    """Release the DAV lock after save
-    """
+    """Release the DAV lock after save"""
     lockable = ILockable(obj)
     if lockable.can_safely_unlock():
         lockable.unlock()
```

### Comparing `plone.locking-2.3.0/plone/locking/interfaces.py` & `plone.locking-3.0.0/plone/locking/interfaces.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,67 +1,74 @@
-from zope.interface import implementer, Interface, Attribute
+from zope import schema
 from zope.annotation.interfaces import IAttributeAnnotatable
+from zope.interface import Attribute
+from zope.interface import implementer
+from zope.interface import Interface
 
-from zope import schema
 
 # Lock types, including the default
 
 # Timeouts are expressed in minutes
 DEFAULT_TIMEOUT = 10
-MAX_TIMEOUT = ((2 ** 32) - 1) // 60
+MAX_TIMEOUT = ((2**32) - 1) // 60
 
 
 class ILockType(Interface):
-    """Representation of a type of lock
-    """
+    """Representation of a type of lock"""
 
-    __name__ = schema.TextLine(title=u"Name",
-                               description=u"The unique name of the lock type")
-
-    stealable = schema.Bool(title=u"Stealable",
-                            description=u"Whether this type of lock is stealable")
-    user_unlockable = schema.Bool(title=u"User unlockable",
-                                  description=u"Whether this type of lock should be unlockable immediately")
-    timeout = schema.Int(title=u"lock timeout",
-                         description=u"Locking timeout in minutes")
+    __name__ = schema.TextLine(
+        title="Name", description="The unique name of the lock type"
+    )
+
+    stealable = schema.Bool(
+        title="Stealable", description="Whether this type of lock is stealable"
+    )
+    user_unlockable = schema.Bool(
+        title="User unlockable",
+        description="Whether this type of lock should be unlockable immediately",
+    )
+    timeout = schema.Int(title="lock timeout", description="Locking timeout in minutes")
 
 
 @implementer(ILockType)
-class LockType(object):
-
+class LockType:
     def __init__(self, name, stealable, user_unlockable, timeout=DEFAULT_TIMEOUT):
         self.__name__ = name
         self.stealable = stealable
         self.user_unlockable = user_unlockable
         self.timeout = timeout
 
-STEALABLE_LOCK = LockType(u"plone.locking.stealable", stealable=True, user_unlockable=True)
+
+STEALABLE_LOCK = LockType(
+    "plone.locking.stealable", stealable=True, user_unlockable=True
+)
 
 # Marker interfaces
 
+
 class ITTWLockable(IAttributeAnnotatable):
-    """Marker interface for objects that are lockable through-the-web
-    """
+    """Marker interface for objects that are lockable through-the-web"""
 
 
 class INonStealableLock(Interface):
-    """Mark an object with this interface to make locks be non-stealable.
-    """
+    """Mark an object with this interface to make locks be non-stealable."""
+
 
 # Functionality
 
+
 class ILockable(Interface):
     """A component that is lockable.
 
     Lock tokens are remembered (in annotations). Multiple locks can exist,
     based on lock types. The default lock type, STEALABLE_LOCK, is a lock
     that can be stolen (unless the object is marked with INonStealableLock).
 
     Most operations take the type as a parameter and operate on the lock token
-    assocaited with a particular type.
+    associated with a particular type.
     """
 
     def lock(lock_type=STEALABLE_LOCK, children=False):
         """Lock the object using the given key.
 
         If children is True, child objects will be locked as well.
         """
@@ -71,20 +78,18 @@
 
         If stealable_only is true, the operation will only have an effect on
         objects that are stealable(). Thus, non-stealable locks will need
         to pass stealable_only=False to actually get unlocked.
         """
 
     def clear_locks():
-        """Clear all locks on the object
-        """
+        """Clear all locks on the object"""
 
     def locked():
-        """True if the object is locked with any lock.
-        """
+        """True if the object is locked with any lock."""
 
     def can_safely_unlock(lock_type=STEALABLE_LOCK):
         """Determine if the current user can safely attempt to unlock the
         object.
 
         That means:
 
@@ -116,21 +121,22 @@
          - time    : the time at which the lock was acquired
          - token   : the underlying lock token
          - type    : the type of lock
         """
 
 
 class IRefreshableLockable(ILockable):
-    """ A component that is lockable and whose locks can be refreshed.
-    """
+    """A component that is lockable and whose locks can be refreshed."""
 
     def refresh_lock(lock_type=STEALABLE_LOCK):
-        """Refresh the lock so it expires later.
-        """
+        """Refresh the lock so it expires later."""
+
 
 # Configuration
 
+
 class ILockSettings(Interface):
-    """A component that looks up configuration settings for lock behavior.
-    """
-    lock_on_ttw_edit = Attribute('A property that reveals whether '
-                                 'through-the-web locking is enabled.')
+    """A component that looks up configuration settings for lock behavior."""
+
+    lock_on_ttw_edit = Attribute(
+        "A property that reveals whether " "through-the-web locking is enabled."
+    )
```

### Comparing `plone.locking-2.3.0/plone/locking/lockable.py` & `plone.locking-3.0.0/plone/locking/lockable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,62 @@
-from zope.interface import implementer
-from zope.component import adapter, queryAdapter
-
+from AccessControl import getSecurityManager
 from persistent.dict import PersistentDict
-
 from zope.annotation.interfaces import IAnnotations
+from zope.component import adapter
 from zope.component import getUtility
+from zope.component import queryAdapter
+from zope.interface import implementer
+
 
-from AccessControl import getSecurityManager
 try:
     from OFS.LockItem import LockItem
 except ImportError:
     # Zope2
     from webdav.LockItem import LockItem
 
-from plone.registry.interfaces import IRegistry
-from Products.CMFPlone.interfaces import IEditingSchema
-
-from plone.locking.interfaces import IRefreshableLockable
+from plone.base.interfaces import IEditingSchema
+from plone.locking.interfaces import ILockSettings
 from plone.locking.interfaces import INonStealableLock
+from plone.locking.interfaces import IRefreshableLockable
 from plone.locking.interfaces import ITTWLockable
 from plone.locking.interfaces import STEALABLE_LOCK
-from plone.locking.interfaces import ILockSettings
+from plone.registry.interfaces import IRegistry
+
 
 try:
     from plone.protect.auto import safeWrite
 except ImportError:
+
     def safeWrite(*args):
         pass
 
 
-ANNOTATION_KEY = 'plone.locking'
+ANNOTATION_KEY = "plone.locking"
 
 
 @adapter(ITTWLockable)
 @implementer(IRefreshableLockable)
-class TTWLockable(object):
-    """An object that is being locked through-the-web
-    """
+class TTWLockable:
+    """An object that is being locked through-the-web"""
 
     def __init__(self, context):
         self.context = context
         self.__locks = None
 
     def lock(self, lock_type=STEALABLE_LOCK, children=False):
         settings = queryAdapter(self.context, ILockSettings)
         if settings is None:
             registry = getUtility(IRegistry)
-            settings = registry.forInterface(IEditingSchema,
-                                             prefix='plone')
+            settings = registry.forInterface(IEditingSchema, prefix="plone")
         if settings is not None and settings.lock_on_ttw_edit is False:
             return
 
         if not self.locked():
             user = getSecurityManager().getUser()
-            depth = children and 'infinity' or 0
+            depth = children and "infinity" or 0
             timeout = int(lock_type.timeout * 60)
             lock = LockItem(user, depth=depth, timeout=timeout)
             token = lock.getLockToken()
             self.context._v_safe_write = True
             self.context.wl_setLock(token, lock)
 
             locks = self._locks()
@@ -67,26 +66,25 @@
 
     def refresh_lock(self, lock_type=STEALABLE_LOCK):
         if not self.locked():
             return
 
         key = self._locks().get(lock_type.__name__, None)
         if key:
-            lock = self.context.wl_getLock(key['token'])
+            lock = self.context.wl_getLock(key["token"])
             lock.refresh()
 
     def unlock(self, lock_type=STEALABLE_LOCK, stealable_only=True):
         if not self.locked():
             return
 
-        if not lock_type.stealable or not stealable_only \
-           or self.stealable(lock_type):
+        if not lock_type.stealable or not stealable_only or self.stealable(lock_type):
             key = self._locks().get(lock_type.__name__, None)
             if key:
-                self.context.wl_delLock(key['token'])
+                self.context.wl_delLock(key["token"])
                 del self._locks()[lock_type.__name__]
 
     def clear_locks(self):
         self.context.wl_clearLocks()
         self._locks().clear()
 
     def locked(self):
@@ -95,50 +93,54 @@
         else:
             return False
 
     def can_safely_unlock(self, lock_type=STEALABLE_LOCK):
         if not lock_type.user_unlockable:
             return False
 
-        info = self.lock_info()
+        lock_info = self.lock_info()
         # There is no lock, so return True
-        if len(info) == 0:
+        if len(lock_info) == 0:
             return True
 
         userid = getSecurityManager().getUser().getId() or None
-        for l in info:
+        for info in lock_info:
             # There is another lock of a different type
-            if not hasattr(l['type'], '__name__') or \
-               l['type'].__name__ != lock_type.__name__:
+            if (
+                not hasattr(info["type"], "__name__")
+                or info["type"].__name__ != lock_type.__name__
+            ):
                 return False
             # The lock is in fact held by the current user
-            if l['creator'] == userid:
+            if info["creator"] == userid:
                 return True
         return False
 
     def stealable(self, lock_type=STEALABLE_LOCK):
         # If the lock type is not stealable ever, return False
         if not lock_type.stealable:
             return False
         # Can't steal locks of a different type
-        for l in self.lock_info():
-            if not hasattr(l['type'], '__name__') or \
-               l['type'].__name__ != lock_type.__name__:
+        for info in self.lock_info():
+            if (
+                not hasattr(info["type"], "__name__")
+                or info["type"].__name__ != lock_type.__name__
+            ):
                 return False
         # The lock type is stealable, and the object is not marked as
         # non-stelaable, so return True
         if not INonStealableLock.providedBy(self.context):
             return True
         # Lock type is stealable, object is not stealable, but return True
         # anyway if we can safely unlock this object (e.g. we are the owner)
         return self.can_safely_unlock(lock_type)
 
     def lock_info(self):
         info = []
-        rtokens = dict([(v['token'], v['type']) for v in self._locks(False).values()])
+        rtokens = {v["token"]: v["type"] for v in self._locks(False).values()}
         jar = self.context._p_jar
         if jar is not None:
             isReadOnly = jar.isReadOnly()
         else:
             isReadOnly = False
         lock_mapping = self.context.wl_lockmapping(not isReadOnly)
         safeWrite(lock_mapping)
@@ -146,20 +148,22 @@
             if not lock.isValid():
                 continue  # Skip invalid/expired locks
             token = lock.getLockToken()
             creator = lock.getCreator()
             # creator can be None when locked by an anonymous user
             if creator is not None:
                 creator = creator[1]
-            info.append({
-                'creator': creator,
-                'time': lock.getModifiedTime(),
-                'token': token,
-                'type': rtokens.get(token, None),
-            })
+            info.append(
+                {
+                    "creator": creator,
+                    "time": lock.getModifiedTime(),
+                    "token": token,
+                    "type": rtokens.get(token, None),
+                }
+            )
         return info
 
     def _locks(self, create=True):
         if self.__locks is not None:
             return self.__locks
 
         annotations = IAnnotations(self.context)
```

### Comparing `plone.locking-2.3.0/plone/locking/testing.py` & `plone.locking-3.0.0/plone/locking/testing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-# -*- coding: utf-8 -*-
 from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
-from plone.app.testing import applyProfile
 from plone.app.testing import PloneSandboxLayer
 from plone.app.testing.layers import FunctionalTesting
 from plone.app.testing.layers import IntegrationTesting
 
 import doctest
 
 
 class PloneLockingLayer(PloneSandboxLayer):
     defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         import plone.locking
+
         self.loadZCML(package=plone.locking)
 
 
 PLONE_LOCKING_FIXTURE = PloneLockingLayer()
 
 PLONE_LOCKING_INTEGRATION_TESTING = IntegrationTesting(
     bases=(PLONE_LOCKING_FIXTURE,),
-    name='PloneLockingLayer:Integration',
+    name="PloneLockingLayer:Integration",
 )
 
 PLONE_LOCKING_FUNCTIONAL_TESTING = FunctionalTesting(
     bases=(PLONE_LOCKING_FIXTURE,),
-    name='PloneLockingLayer:Functional',
+    name="PloneLockingLayer:Functional",
 )
 
 optionflags = (
-    doctest.REPORT_ONLY_FIRST_FAILURE
-    | doctest.ELLIPSIS
-    | doctest.NORMALIZE_WHITESPACE
+    doctest.REPORT_ONLY_FIRST_FAILURE | doctest.ELLIPSIS | doctest.NORMALIZE_WHITESPACE
 )
```

### Comparing `plone.locking-2.3.0/plone/locking/tests/locking.rst` & `plone.locking-3.0.0/plone/locking/tests/locking.rst`

 * *Files identical despite different names*

### Comparing `plone.locking-2.3.0/plone/locking/tests/test_functional.py` & `plone.locking-3.0.0/plone/locking/tests/test_functional.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,51 @@
-# -*- coding: utf-8 -*-
 from plone.app.testing import login
 from plone.app.testing import logout
 from plone.app.testing import setRoles
-from plone.locking.testing import PLONE_LOCKING_FUNCTIONAL_TESTING
 from plone.locking.testing import optionflags
+from plone.locking.testing import PLONE_LOCKING_FUNCTIONAL_TESTING
 from plone.testing import layered
 from Products.CMFCore.utils import getToolByName
 
 import doctest
 import unittest
 
 
 def setup(doctest):
-    portal = doctest.globs['layer']['portal']
-    portal_membership = getToolByName(portal, 'portal_membership')
-    portal_membership.addMember('member1', 'secret', ('Member', ), [])
-    portal_membership.addMember('member2', 'secret', ('Member', ), [])
+    portal = doctest.globs["layer"]["portal"]
+    portal_membership = getToolByName(portal, "portal_membership")
+    portal_membership.addMember("member1", "secret", ("Member",), [])
+    portal_membership.addMember("member2", "secret", ("Member",), [])
 
     logout()
-    login(portal, 'member1')
-    setRoles(portal, 'member1', ['Manager', ])
-    portal.invokeFactory('Document', 'doc')
-    setRoles(portal, 'member1', ['Member', ])
+    login(portal, "member1")
+    setRoles(
+        portal,
+        "member1",
+        [
+            "Manager",
+        ],
+    )
+    portal.invokeFactory("Document", "doc")
+    setRoles(
+        portal,
+        "member1",
+        [
+            "Member",
+        ],
+    )
 
 
 def test_suite():
     suite = unittest.TestSuite()
     suite.addTest(
         layered(
             doctest.DocFileSuite(
-                'tests/locking.rst',
-                package='plone.locking',
+                "tests/locking.rst",
+                package="plone.locking",
                 optionflags=optionflags,
                 setUp=setup,
             ),
             layer=PLONE_LOCKING_FUNCTIONAL_TESTING,
         )
     )
     return suite
```

### Comparing `plone.locking-2.3.0/plone/locking/tests/test_views.py` & `plone.locking-3.0.0/plone/locking/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# -*- coding: utf-8 -*-
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
+from plone.dexterity.interfaces import IDexterityFTI
 from plone.locking.browser.locking import LockingInformation
 from plone.locking.browser.locking import LockingInformationFallback
 from plone.locking.testing import PLONE_LOCKING_INTEGRATION_TESTING
-from plone.dexterity.interfaces import IDexterityFTI
 from zope.component import queryUtility
 
 import unittest
 
 
 class TestLockInfoViewWithoutLocking(unittest.TestCase):
-
     layer = PLONE_LOCKING_INTEGRATION_TESTING
 
     view = "@@plone_lock_info"
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
```

### Comparing `plone.locking-2.3.0/plone.locking.egg-info/PKG-INFO` & `plone.locking-3.0.0/plone.locking.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,81 @@
 Metadata-Version: 2.1
 Name: plone.locking
-Version: 2.3.0
+Version: 3.0.0
 Summary: webdav locking support
 Home-page: https://pypi.org/project/plone.locking
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: locking webdav plone
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
-Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Overview
 ========
 
 Provides basic automatic locking support for Plone. Locks are stealable by
 default, meaning that a user with edit privileges will be able to steal
 another user's lock, but will be warned that someone else may be editing
 the same object. Used by Plone, Archetypes and plone.app.iterate
 
-Compatibility
--------------
+Version Information
+-------------------
 
-The versions 2.1.x (built from the master-branch) are used in Plone 5 and are not compatible with earlier Plone versions.
-
-Versions 2.0.x are used by Plone 4.x (but *may* also be compatible with earlier versions).
-
-Versions 1.x are used by Plone 3.
+- 3.x -> Plone 6.0+ only
+- 2.3.x -> used in Plone 5+ (not compatible with earlier Plone versions)
+- 2.0.x -> used by Plone 4.x (but *may* also be compatible with earlier versions).
+- Versions 1.x are used by Plone 3.
 
 Changelog
 =========
 
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.0 (2023-04-16)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7. (#1)
+
+
+New features:
+
+
+- Update the info viewlet css classes to Bootstrap 5.
+  [ewohnlich] (bs5)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (234bb1d6, 5cc689e5)
+
+
 2.3.0 (2023-02-08)
 ------------------
 
 Bug fixes:
 
 
 - Update to Zope4 only including troove classifiers. [jensens] (#19)
```

### Comparing `plone.locking-2.3.0/plone.locking.egg-info/SOURCES.txt` & `plone.locking-3.0.0/plone.locking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.locking-2.3.0/setup.py` & `plone.locking-3.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,49 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
 
-version = '2.3.0'
 
-setup(name='plone.locking',
-      version=version,
-      description="webdav locking support",
-      long_description=open("README.rst").read() + "\n" +
-                       open("CHANGES.rst").read(),
-      classifiers=[
-          "Development Status :: 5 - Production/Stable",
-          "Environment :: Web Environment",
-          "Framework :: Plone",
-          "Framework :: Plone :: 5.2",
-          "Framework :: Plone :: 6.0",
-          "Framework :: Plone :: Core",
-          "Framework :: Zope :: 4",
-          "Framework :: Zope :: 5",
-          "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
-          "Operating System :: OS Independent",
-          "Programming Language :: Python",
-          "Programming Language :: Python :: 2.7",
-          "Programming Language :: Python :: 3.7",
-          "Programming Language :: Python :: 3.8",
-          "Programming Language :: Python :: 3.9",
-          "Programming Language :: Python :: 3.10",
-          "Programming Language :: Python :: 3.11",
-        ],
-      keywords='locking webdav plone',
-      author='Plone Foundation',
-      author_email='plone-developers@lists.sourceforge.net',
-      url='https://pypi.org/project/plone.locking',
-      license='GPL version 2',
-      packages=find_packages(),
-      namespace_packages=['plone'],
-      include_package_data=True,
-      zip_safe=False,
-      python_requires=">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*",
-      extras_require=dict(
+version = "3.0.0"
+
+setup(
+    name="plone.locking",
+    version=version,
+    description="webdav locking support",
+    long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Web Environment",
+        "Framework :: Plone",
+        "Framework :: Plone :: 6.0",
+        "Framework :: Plone :: Core",
+        "Framework :: Zope :: 5",
+        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
+    keywords="locking webdav plone",
+    author="Plone Foundation",
+    author_email="plone-developers@lists.sourceforge.net",
+    url="https://pypi.org/project/plone.locking",
+    license="GPL version 2",
+    packages=find_packages(),
+    namespace_packages=["plone"],
+    include_package_data=True,
+    zip_safe=False,
+    python_requires=">=3.8",
+    extras_require=dict(
         test=[
-            'plone.app.contenttypes',
-            'plone.app.testing',
+            "plone.app.contenttypes[test]",
+            "plone.app.testing",
+            "plone.dexterity",
+            "plone.testing",
         ]
-      ),
-      install_requires=[
-        'setuptools',
-        'zope.annotation',
-        'zope.component',
-        'zope.i18nmessageid',
-        'zope.interface',
-        'zope.schema',
-        'zope.viewlet',
-        'Acquisition',
-        'DateTime',
-        'Products.CMFCore',
-        'ZODB',
-        'Zope',
-      ],
-      )
+    ),
+    install_requires=[
+        "setuptools",
+        "plone.base",
+    ],
+)
```

