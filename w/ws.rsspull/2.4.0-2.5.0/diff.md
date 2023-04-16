# Comparing `tmp/ws.rsspull-2.4.0.tar.gz` & `tmp/ws.rsspull-2.5.0.tar.gz`

## Comparing `ws.rsspull-2.4.0.tar` & `ws.rsspull-2.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/.coveragerc
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/.travis.yml
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/CHANGES.txt
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/README.rst
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/examplerun.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/changelog/.keep
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/src/ws/rsspull/__init__.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/src/ws/rsspull/feed.py
--rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/src/ws/rsspull/maildir.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/src/ws/rsspull/main.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/src/ws/rsspull/util.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/src/ws/rsspull/tests/__init__.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/src/ws/rsspull/tests/test_feed.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/src/ws/rsspull/tests/test_main.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/src/ws/rsspull/tests/fixture/config
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/src/ws/rsspull/tests/fixture/feeds.opml
--rw-r--r--   0        0        0    90261 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/src/ws/rsspull/tests/fixture/ongoing.xml
--rw-r--r--   0        0        0    19940 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/src/ws/rsspull/tests/fixture/samruby.xml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/.gitignore
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 ws_rsspull-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/.coveragerc
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/.travis.yml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/CHANGES.txt
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/README.rst
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/examplerun.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/changelog/.keep
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/src/ws/rsspull/__init__.py
+-rw-r--r--   0        0        0     8174 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/src/ws/rsspull/feed.py
+-rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/src/ws/rsspull/maildir.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/src/ws/rsspull/main.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/src/ws/rsspull/util.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/src/ws/rsspull/tests/__init__.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/src/ws/rsspull/tests/test_feed.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/src/ws/rsspull/tests/test_main.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/src/ws/rsspull/tests/fixture/config
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/src/ws/rsspull/tests/fixture/feeds.opml
+-rw-r--r--   0        0        0    90261 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/src/ws/rsspull/tests/fixture/ongoing.xml
+-rw-r--r--   0        0        0    19940 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/src/ws/rsspull/tests/fixture/samruby.xml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/.gitignore
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 ws_rsspull-2.5.0/PKG-INFO
```

### Comparing `ws_rsspull-2.4.0/CHANGES.txt` & `ws_rsspull-2.5.0/CHANGES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 CHANGES
 =======
 
 .. towncrier release notes start
 
+2.5.0 (2023-04-16)
+------------------
+
+Changes
++++++++
+
+- Make user-agent header configurable (useragent)
+
+
 2.4.0 (2023-04-04)
 ------------------
 
 Changes
 +++++++
 
 - Drop Python-2 support (py2)
```

### Comparing `ws_rsspull-2.4.0/README.rst` & `ws_rsspull-2.5.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 You need to create a configuration file in ``~/.rsspull/config``, like::
 
     [global]
     target = ~/Maildir/rss
     target_type = maildir
     logfile = ~/.rsspull/log
     workers = 1
+    user_agent = optional custom header
 
 For low-volume applications you can also send the emails via SMTP instead::
 
     [global]
     target = test@example.com
     target_type = smtp://my-smtp-server.example.com
```

#### html2text {}

```diff
@@ -4,19 +4,20 @@
 This way you can read your feeds using an email client (I use `claws`_, so I
 can access mailing lists, newsgroups and feeds all in one application). The
 heavy lifting is performed by the awesome `feedparser`_ library. .. _`claws`:
 http://claws-mail.org/ .. _`feedparser`: https://pypi.org/project/feedparser
 Installation ============ rsspull requires at least Python 3.3. You can install
 it from PyPI like this:: $ pip install ws.rsspull You need to create a
 configuration file in ``~/.rsspull/config``, like:: [global] target = ~/
-Maildir/rss target_type = maildir logfile = ~/.rsspull/log workers = 1 For low-
-volume applications you can also send the emails via SMTP instead:: [global]
-target = test@example.com target_type = smtp://my-smtp-server.example.com List
-the feeds you want to pull in an OPML file at ``~/.rsspull/feeds.opml``:: <?xml
-version="1.0" encoding="utf-8"?>
+Maildir/rss target_type = maildir logfile = ~/.rsspull/log workers = 1
+user_agent = optional custom header For low-volume applications you can also
+send the emails via SMTP instead:: [global] target = test@example.com
+target_type = smtp://my-smtp-server.example.com List the feeds you want to pull
+in an OPML file at ``~/.rsspull/feeds.opml``:: <?xml version="1.0"
+encoding="utf-8"?>
 rsspull rsspull@localhost
 
  Notes about the format: * You can group your feeds (using nested ````), this
 does not matter to rsspull. * The ``text`` attribute is used as the folder
 name, relative to the ``maildir`` setting in ``~/.rsspull/config``. If you run
 rsspull on an IMAP server, you can create folder hierarchies by using something
 like ``text=".rss.tech.ongoing"`` (check you IMAP server documentation how it
```

### Comparing `ws_rsspull-2.4.0/src/ws/rsspull/feed.py` & `ws_rsspull-2.5.0/src/ws/rsspull/feed.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 import requests
 import smtplib
 import ws.rsspull.maildir
 import ws.rsspull.util
 import xml.dom.minidom
 
 
-USER_AGENT = ('Mozilla/5.0 (X11; U; Linux i686; en-US; rv:1.8.1.2)'
-              ' Gecko/20070220 Firefox/2.0.0.2')
 log = logging.getLogger(__name__)
 
 
 class Entry(object):
 
     def __init__(self, feed, item):
         self.feed = feed
@@ -128,14 +126,15 @@
 
 
 class Feed(object):
 
     workdir = None
     target = None
     target_type = None
+    user_agent = None
 
     recipient = 'rsspull <rsspull@localhost>'
 
     @staticmethod
     def parseOPML(config):
         doc = xml.dom.minidom.parse(config)
         feeds = []
@@ -171,17 +170,17 @@
             open(self.md5, 'w').close()
 
     # delegates to feedparser
     def __getattr__(self, name):
         return getattr(self.feed, name)
 
     def download(self):
-        headers = {
-            'User-Agent': USER_AGENT
-        }
+        headers = {}
+        if self.user_agent:
+            headers['User-Agent'] = self.user_agent
         if os.path.exists(self.file):
             headers['If-Modified-Since'] = email.utils.formatdate(
                 os.stat(self.file).st_mtime)
 
         log.info('Downloading %s <%s>' % (self.name, self.url))
 
         try:
```

### Comparing `ws_rsspull-2.4.0/src/ws/rsspull/maildir.py` & `ws_rsspull-2.5.0/src/ws/rsspull/maildir.py`

 * *Files identical despite different names*

### Comparing `ws_rsspull-2.4.0/src/ws/rsspull/main.py` & `ws_rsspull-2.5.0/src/ws/rsspull/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 def rsspull(confdir):
     confdir = os.path.expanduser(confdir)
     config = ConfigParser()
     config.read(os.path.join(confdir, 'config'))
     Feed.workdir = os.path.join(confdir, 'cache')
     Feed.target = os.path.expanduser(config.get('global', 'target'))
     Feed.target_type = os.path.expanduser(config.get('global', 'target_type'))
+    Feed.user_agent = config.get('global', 'user_agent')
 
     ws.rsspull.util.setupLogging(os.path.expanduser(
         config.get('global', 'logfile')))
     log = logging.getLogger(__name__)
     log.info('Reading feed configuration from %s' % confdir)
     feeds = Feed.parseOPML(os.path.join(confdir, 'feeds.opml'))
```

### Comparing `ws_rsspull-2.4.0/src/ws/rsspull/util.py` & `ws_rsspull-2.5.0/src/ws/rsspull/util.py`

 * *Files identical despite different names*

### Comparing `ws_rsspull-2.4.0/src/ws/rsspull/tests/test_feed.py` & `ws_rsspull-2.5.0/src/ws/rsspull/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `ws_rsspull-2.4.0/src/ws/rsspull/tests/test_main.py` & `ws_rsspull-2.5.0/src/ws/rsspull/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ws_rsspull-2.4.0/src/ws/rsspull/tests/fixture/feeds.opml` & `ws_rsspull-2.5.0/src/ws/rsspull/tests/fixture/feeds.opml`

 * *Files identical despite different names*

### Comparing `ws_rsspull-2.4.0/src/ws/rsspull/tests/fixture/ongoing.xml` & `ws_rsspull-2.5.0/src/ws/rsspull/tests/fixture/ongoing.xml`

 * *Files identical despite different names*

### Comparing `ws_rsspull-2.4.0/src/ws/rsspull/tests/fixture/samruby.xml` & `ws_rsspull-2.5.0/src/ws/rsspull/tests/fixture/samruby.xml`

 * *Files identical despite different names*

### Comparing `ws_rsspull-2.4.0/pyproject.toml` & `ws_rsspull-2.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ws_rsspull-2.4.0/PKG-INFO` & `ws_rsspull-2.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ws.rsspull
-Version: 2.4.0
+Version: 2.5.0
 Summary: Downloads RSS/Atom feeds and converts them to Maildir messages
 Project-URL: Repository, https://github.com/wosc/rsspull
 Author-email: Wolfgang Schnerring <wosc@wosc.de>
 License:  BSD-3-Clause
 Requires-Python: >=3.7
 Requires-Dist: feedparser
 Requires-Dist: html2text
@@ -44,14 +44,15 @@
 You need to create a configuration file in ``~/.rsspull/config``, like::
 
     [global]
     target = ~/Maildir/rss
     target_type = maildir
     logfile = ~/.rsspull/log
     workers = 1
+    user_agent = optional custom header
 
 For low-volume applications you can also send the emails via SMTP instead::
 
     [global]
     target = test@example.com
     target_type = smtp://my-smtp-server.example.com
 
@@ -127,14 +128,23 @@
 
 
 CHANGES
 =======
 
 .. towncrier release notes start
 
+2.5.0 (2023-04-16)
+------------------
+
+Changes
++++++++
+
+- Make user-agent header configurable (useragent)
+
+
 2.4.0 (2023-04-04)
 ------------------
 
 Changes
 +++++++
 
 - Drop Python-2 support (py2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ws.rsspull Version: 2.4.0 Summary: Downloads RSS/
+Metadata-Version: 2.1 Name: ws.rsspull Version: 2.5.0 Summary: Downloads RSS/
 Atom feeds and converts them to Maildir messages Project-URL: Repository,
 https://github.com/wosc/rsspull Author-email: Wolfgang Schnerring
 wosc.de> License: BSD-3-Clause Requires-Python: >=3.7 Requires-Dist: feedparser
 Requires-Dist: html2text Requires-Dist: requests Provides-Extra: test Requires-
 Dist: pytest; extra == 'test' Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: setuptools; extra == 'test' Description-Content-Type: text/x-rst
 ======= rsspull ======= .. image:: https://travis-ci.org/wosc/rsspull.png :
@@ -11,19 +11,20 @@
 This way you can read your feeds using an email client (I use `claws`_, so I
 can access mailing lists, newsgroups and feeds all in one application). The
 heavy lifting is performed by the awesome `feedparser`_ library. .. _`claws`:
 http://claws-mail.org/ .. _`feedparser`: https://pypi.org/project/feedparser
 Installation ============ rsspull requires at least Python 3.3. You can install
 it from PyPI like this:: $ pip install ws.rsspull You need to create a
 configuration file in ``~/.rsspull/config``, like:: [global] target = ~/
-Maildir/rss target_type = maildir logfile = ~/.rsspull/log workers = 1 For low-
-volume applications you can also send the emails via SMTP instead:: [global]
-target = test@example.com target_type = smtp://my-smtp-server.example.com List
-the feeds you want to pull in an OPML file at ``~/.rsspull/feeds.opml``:: <?xml
-version="1.0" encoding="utf-8"?>
+Maildir/rss target_type = maildir logfile = ~/.rsspull/log workers = 1
+user_agent = optional custom header For low-volume applications you can also
+send the emails via SMTP instead:: [global] target = test@example.com
+target_type = smtp://my-smtp-server.example.com List the feeds you want to pull
+in an OPML file at ``~/.rsspull/feeds.opml``:: <?xml version="1.0"
+encoding="utf-8"?>
 rsspull rsspull@localhost
 
  Notes about the format: * You can group your feeds (using nested ````), this
 does not matter to rsspull. * The ``text`` attribute is used as the folder
 name, relative to the ``maildir`` setting in ``~/.rsspull/config``. If you run
 rsspull on an IMAP server, you can create folder hierarchies by using something
 like ``text=".rss.tech.ongoing"`` (check you IMAP server documentation how it
@@ -41,21 +42,23 @@
 the original HTML and one converted into markdown-like plaintext (via
 `html2text`_), so most of the time opening in a browser isn't even necessary
 since you can read the post right in the email client. * Can use several worker
 threads to download and parse feeds to increase performance, since quite some
 time is spent waiting for downloads to complete (the ``workers`` setting in
 ``~/.rsspull/config``). * Has been in daily usage since 2007, so it definitely
 Works For Me(tm). .. _`html2text`: https://pypi.python.org/pypi/html2text
-CHANGES ======= .. towncrier release notes start 2.4.0 (2023-04-04) -----------
-------- Changes +++++++ - Drop Python-2 support (py2) - Switch from setup.py to
-pyproject.toml (wheel) 2.3.1 (2023-03-20) ------------------ - Escape '/' in
-feed names to avoid prevent file names 2.3.0 (2018-04-03) ------------------ -
-Make SMTP server configurable. 2.2.1 (2018-03-30) ------------------ - Fix
-Python-3 unicode issues. 2.2 (2018-03-24) ---------------- - Support sending
-messages via SMTP as an alternative to writing into Maildir. - Add commandline
-option to set config directory. 2.1 (2018-03-06) ---------------- - Switch from
-urllib2 to requests. - Make Python-3 compatible. 2.0 (2014-02-22) -------------
---- - Switch from spawning curl to using urllib2. - Package as egg. 1.2 (2013-
-10-03) ---------------- - Use stdlib xml parser instead of python-xml. 1.1
-(2009-05-23) ---------------- - Write messages directly to Maildir instead of
-using procmail. - Send messages as multipart, text and html. 1.0 (2007-03-31) -
---------------- - First release, inspired by http://newspipe.sourceforge.net/.
+CHANGES ======= .. towncrier release notes start 2.5.0 (2023-04-16) -----------
+------- Changes +++++++ - Make user-agent header configurable (useragent) 2.4.0
+(2023-04-04) ------------------ Changes +++++++ - Drop Python-2 support (py2) -
+Switch from setup.py to pyproject.toml (wheel) 2.3.1 (2023-03-20) -------------
+----- - Escape '/' in feed names to avoid prevent file names 2.3.0 (2018-04-03)
+------------------ - Make SMTP server configurable. 2.2.1 (2018-03-30) --------
+---------- - Fix Python-3 unicode issues. 2.2 (2018-03-24) ---------------- -
+Support sending messages via SMTP as an alternative to writing into Maildir. -
+Add commandline option to set config directory. 2.1 (2018-03-06) --------------
+-- - Switch from urllib2 to requests. - Make Python-3 compatible. 2.0 (2014-02-
+22) ---------------- - Switch from spawning curl to using urllib2. - Package as
+egg. 1.2 (2013-10-03) ---------------- - Use stdlib xml parser instead of
+python-xml. 1.1 (2009-05-23) ---------------- - Write messages directly to
+Maildir instead of using procmail. - Send messages as multipart, text and html.
+1.0 (2007-03-31) ---------------- - First release, inspired by http://
+newspipe.sourceforge.net/.
```

