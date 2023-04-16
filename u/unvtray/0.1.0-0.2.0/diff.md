# Comparing `tmp/unvtray-0.1.0.tar.gz` & `tmp/unvtray-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unvtray-0.1.0.tar", last modified: Wed Apr 12 20:19:29 2023, max compression
+gzip compressed data, was "unvtray-0.2.0.tar", last modified: Sun Apr 16 04:57:41 2023, max compression
```

## Comparing `unvtray-0.1.0.tar` & `unvtray-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:19:29.008203 unvtray-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:19:29.008203 unvtray-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:19:29.008203 unvtray-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-12 20:19:17.000000 unvtray-0.1.0/.github/workflows/build-and-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 20:19:17.000000 unvtray-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-12 20:19:17.000000 unvtray-0.1.0/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 20:19:17.000000 unvtray-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    42782 2023-04-12 20:19:29.008203 unvtray-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-12 20:19:17.000000 unvtray-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-12 20:19:17.000000 unvtray-0.1.0/example.png
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-12 20:19:17.000000 unvtray-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:19:29.008203 unvtray-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:19:29.008203 unvtray-0.1.0/unvtray/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-12 20:19:17.000000 unvtray-0.1.0/unvtray/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:19:29.008203 unvtray-0.1.0/unvtray/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   203376 2023-04-12 20:19:17.000000 unvtray-0.1.0/unvtray/assets/FreeMonoBold.otf
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-12 20:19:17.000000 unvtray-0.1.0/unvtray/assets/unvanquished.png
--rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-04-12 20:19:17.000000 unvtray-0.1.0/unvtray/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-12 20:19:17.000000 unvtray-0.1.0/unvtray/tray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:19:29.008203 unvtray-0.1.0/unvtray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42782 2023-04-12 20:19:28.000000 unvtray-0.1.0/unvtray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-12 20:19:29.000000 unvtray-0.1.0/unvtray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:19:28.000000 unvtray-0.1.0/unvtray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 20:19:28.000000 unvtray-0.1.0/unvtray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 20:19:28.000000 unvtray-0.1.0/unvtray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 20:19:28.000000 unvtray-0.1.0/unvtray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.129049 unvtray-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.121049 unvtray-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-16 04:57:32.000000 unvtray-0.2.0/.github/workflows/build-and-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-16 04:57:32.000000 unvtray-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 04:57:32.000000 unvtray-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-16 04:57:41.125049 unvtray-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-16 04:57:32.000000 unvtray-0.2.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2484 2023-04-16 04:57:32.000000 unvtray-0.2.0/make_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/package/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.121049 unvtray-0.2.0/package/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/package/icons/128x128/
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-04-16 04:57:32.000000 unvtray-0.2.0/package/icons/128x128/unvtray.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/package/icons/256x256/
+-rw-r--r--   0 runner    (1001) docker     (123)    56350 2023-04-16 04:57:32.000000 unvtray-0.2.0/package/icons/256x256/unvtray.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/package/icons/32x32/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-16 04:57:32.000000 unvtray-0.2.0/package/icons/32x32/unvtray.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/package/icons/512x512/
+-rw-r--r--   0 runner    (1001) docker     (123)   165906 2023-04-16 04:57:32.000000 unvtray-0.2.0/package/icons/512x512/unvtray.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/package/icons/64x64/
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-04-16 04:57:32.000000 unvtray-0.2.0/package/icons/64x64/unvtray.png
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-16 04:57:32.000000 unvtray-0.2.0/package/net.unvanquished.unvtray.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-16 04:57:32.000000 unvtray-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 04:57:41.129049 unvtray-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/unvtray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/unvtray/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   203376 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/assets/FreeMonoBold.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   218008 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/assets/unvanquished.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-16 04:57:32.000000 unvtray-0.2.0/unvtray/tray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:57:41.125049 unvtray-0.2.0/unvtray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-16 04:57:41.000000 unvtray-0.2.0/unvtray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-16 04:57:41.000000 unvtray-0.2.0/unvtray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 04:57:41.000000 unvtray-0.2.0/unvtray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 04:57:41.000000 unvtray-0.2.0/unvtray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 04:57:41.000000 unvtray-0.2.0/unvtray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 04:57:41.000000 unvtray-0.2.0/unvtray.egg-info/top_level.txt
```

### Comparing `unvtray-0.1.0/.github/workflows/build-and-publish.yml` & `unvtray-0.2.0/.github/workflows/build-and-publish.yml`

 * *Files identical despite different names*

### Comparing `unvtray-0.1.0/LICENSE.txt` & `unvtray-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unvtray-0.1.0/pyproject.toml` & `unvtray-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,39 @@
 name = "unvtray"
 description = "Unvanquished Tray"
 readme = "README.md"
 authors = [
     {name = "Maximilian Stahlberg", email = "viech@unvanquished.net"},
 ]
 keywords = ["unvanquished"]
-license = {file = "LICENSE.txt"}
+license = {text = "GPL-3.0-or-later"}
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python :: 3",
     "Topic :: Games/Entertainment :: First Person Shooters",
     "Topic :: Games/Entertainment :: Real Time Strategy",
 ]
 requires-python = ">=3.3"
 dependencies = ["pillow", "pystray"]
 dynamic = ["version"]
 
+[project.urls]
+Homepage = "https://unvanquished.net"
+Repository = "https://github.com/Unvanquished/unvanquished-tray-browser"
+
 [project.scripts]
 unvtray = "unvtray.__main__:run"
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 
+[tool.setuptools]
+packages = ["unvtray"]
+
 [tool.setuptools.package-data]
 "unvtray.assets" = ["*.otf", "*.png"]
 
 [tool.black]
 line-length = 79
```

### Comparing `unvtray-0.1.0/unvtray/__main__.py` & `unvtray-0.2.0/unvtray/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # You should have received a copy of the GNU General Public License along with
 # this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import time
 from sched import scheduler
 
 from . import tray
-from .query import ServerList
+from .servers import ServerList
 
 TRAY_WAKEUP_TIME = 0.2
 TRAY_REFRESH_TIME = 5
 MAIN_UPDATE_TIME = 60
 
 
 def setup(tray_icon):
```

### Comparing `unvtray-0.1.0/unvtray/assets/FreeMonoBold.otf` & `unvtray-0.2.0/unvtray/assets/FreeMonoBold.otf`

 * *Files identical despite different names*

### Comparing `unvtray-0.1.0/unvtray/query.py` & `unvtray-0.2.0/unvtray/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,89 +11,128 @@
 # FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for
 # more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import logging
-import os
+import re
 from functools import wraps
 from itertools import islice
-from multiprocessing.pool import ThreadPool
 from socket import AF_INET, SOCK_DGRAM, socket
 from time import perf_counter
 from time import time as unix_time
 
-LOGLEVEL = os.getenv("LOGLEVEL", "INFO").upper()
-logging.basicConfig(level=LOGLEVEL)
-logger = logging.getLogger("Unvanquished Tray")
-
-PROTOCOL = 86
-PREFIX = b"\xff\xff\xff\xff"
-RECORD_SEP = b"\\"
-SERVER_RECORD_LEN = 7  # IPv4, port, separator
+from .common import QUERY_PREFIX, RECORD_SEP, SOCKET_TIMEOUT, logger
+from .ping import Ping
+
 GET_STATUS_BUFFER = 2**14
-Q_GET_SERVERS = PREFIX + f"getservers {PROTOCOL}".encode("ascii")
-R_GET_SERVERS = PREFIX + b"getserversResponse" + RECORD_SEP
-Q_GET_STATUS = PREFIX + b"getstatus"
-R_GET_STATUS = PREFIX + b"statusResponse\n" + RECORD_SEP
-
-SOCKET_TIMEOUT = 1
-
-
-def strip_colors(string):
-    stripped = ""
-    chars = list(string)
-    while chars:
-        c = chars.pop(0)
-        if c == "^" and chars:
-            d = chars.pop(0)
-            if d == "#":
-                chars = chars[6:]
-        else:
-            stripped += c
-    return stripped
+Q_GET_STATUS = QUERY_PREFIX + b"getstatus"
+R_GET_STATUS = QUERY_PREFIX + b"statusResponse\n" + RECORD_SEP
+
+MAX_SERVER_NAME_CHARS = 60
+MAX_MAP_NAME_CHARS = 20
 
 
 class Server:
     @staticmethod
-    def _valid_or(default=None):
+    def strip_colors(string):
+        stripped = ""
+        chars = list(string)
+        while chars:
+            c = chars.pop(0)
+            if c == "^" and chars:
+                d = chars.pop(0)
+                if d == "#":
+                    chars = chars[6:]
+            else:
+                stripped += c
+        return stripped
+
+    @staticmethod
+    def strip_emoticons(string):
+        """Removes emoticon tags and normalizes whitespace."""
+        return re.sub(r"\s*(\[.*?\]|\s)\s*", " ", string).strip()
+
+    @staticmethod
+    def _valid_or(default=None, *, fallback=None, cache=False):
+        """Return a default if the last request did not produce a valid config.
+
+        This decorates methods of :class:`Server`. The method will be executed
+        if and only if the last server refresh, if any, was successful: the
+        server must have provided a configuration that has passed initial
+        sanity checks. If the method is either not executed or is executed and
+        raises an exception, then the decorator returns the provided default
+        value. In the latter case, the exception is further logged. If the
+        method is successfully executed, then its return value is forwarded.
+
+        Instead of a constant default, a fallback method can be provided that
+        will be run instead of the (skipped or failed) decorated method and
+        whose return value is then forwarded. This fallback should not depend
+        on a valid configuration being provided by the server.
+
+        If further caching is enabled, any return value forwarded in the
+        presence of a server configuration will be cached within that
+        configuration and returned immediately on a subsequent request.
+        """
+        assert default is None or fallback is None
+
         def wrapper(method):
             @wraps(method)
             def wrapped(server, *args, **kwargs):
                 if server._config:
-                    return method(server, *args, **kwargs)
+                    if cache and method in server._config:
+                        return server._config[method]
+
+                    try:
+                        value = method(server, *args, **kwargs)
+                    except Exception as error:
+                        logger.warn(
+                            f"Failed to obtain {method.__name__}"
+                            f" for {server.address}: {error}"
+                        )
+                        value = fallback(server) if fallback else default
+
+                    if cache:
+                        server._config[method] = value
+
+                    return value
                 else:
-                    return default
+                    return fallback(server) if fallback else default
 
             return wrapped
 
         return wrapper
 
     def __init__(self, host, port):
         self._host = host
         self._port = port
 
         self._config = None
-        self._ping = None
+        self._ping = Ping()
 
         self._last_refresh = 0
         self._last_refresh_error = None
 
     def __hash__(self):
         return hash(self._host) ^ hash(self._port)
 
     def __eq__(self, other):
         return self._host == other._host and self._port == other._port
 
+    @staticmethod
+    def _limit_to(string, length):
+        return string if len(string) <= length else f"{string[:length-1]}…"
+
     def __str__(self):
         return (
             f"{self.num_playing}+{self.num_spectating}"
-            f" on {self.stripped_name}"
-            f" ({self.map_name}, {self.ping * 1000:.0f} ms)"
+            f" on {self._limit_to(self.stripped_name, MAX_SERVER_NAME_CHARS)}"
+            f" ({self._limit_to(self.map_name, MAX_MAP_NAME_CHARS)},"
+            f" {self.ping * 1000:.0f} ms)"
         )
 
     def refresh(self):
         """Update the server status and ping.
 
         :raises RuntimeError:
             When the update has failed.
@@ -103,15 +142,15 @@
         con = socket(AF_INET, SOCK_DGRAM)
         con.settimeout(SOCKET_TIMEOUT)
         con.connect((self._host, self._port))
 
         t = perf_counter()
         con.send(Q_GET_STATUS)
         response = con.recv(GET_STATUS_BUFFER)
-        self._ping = perf_counter() - t
+        self._ping.register(perf_counter() - t)
 
         if not response:
             raise RuntimeError(
                 f"Failed to query status of game server at {self.address}:"
                 f" no response."
             )
 
@@ -152,15 +191,15 @@
                 logging.INFO
                 if error_str != self._last_refresh_error
                 else logging.DEBUG,
                 f"Failed to refresh game server {self.address}: {error_str}",
             )
 
             self._config = None
-            self._ping = None
+            self._ping.clear()
 
             self._last_refresh_error = error_str
         else:
             self._last_refresh_error = None
 
     @property
     def address(self):
@@ -182,48 +221,45 @@
         return (
             unix_time() - self._last_refresh
             if self._last_refresh
             else float("inf")
         )
 
     @property
-    @_valid_or(float("inf"))
     def ping(self):
-        assert self._ping
-        return self._ping
+        """A moving average of recent response times."""
+        return self._ping.mvavg
 
     @property
-    @_valid_or("unknown")
+    @_valid_or(fallback=lambda server: server.address)
     def name(self):
         """Name of the server as given."""
         assert self._config
         return self._config["sv_hostname"]
 
     @property
     def stripped_name(self):
         """Name of the server without color codes."""
-        return strip_colors(self.name)
+        return self.strip_emoticons(self.strip_colors(self.name))
 
     @property
     @_valid_or("unknown")
     def map_name(self):
         """Name of the server as given."""
         assert self._config
         return self._config["mapname"]
 
     @property
-    @_valid_or((0,) * 5)
+    @_valid_or((0,) * 5, cache=True)
     def player_stats(self):
+        """Reports number of players (S/A/H) and bots (A/H) as five numbers."""
         assert self._config
 
-        try:
-            B = self._config["B"]
-            P = self._config["P"]
-        except KeyError as error:
-            raise RuntimeError("No bot/player status fields found.") from error
+        B = self._config["B"]
+        P = self._config["P"]
 
         if len(B) != len(P):
             raise RuntimeError("Lengths of bot and player states do not match.")
 
         spectators, a_players, h_players, a_bots, h_bots = (0,) * 5
 
         for skill, team in zip(B, P):
@@ -258,215 +294,7 @@
         """Number of players on a team, excluding bots."""
         return sum(self.player_stats[1:3])
 
     @property
     def num_spectating(self):
         """Number of players not on a team."""
         return self.player_stats[0]
-
-
-class ServerList:
-    @staticmethod
-    def _check_refresh(method):
-        @wraps(method)
-        def wrapped(servers, *args, **kwargs):
-            current_time = unix_time()
-
-            if current_time - servers._last_update > servers._update_time:
-                servers.try_update_servers()
-
-            if current_time - servers._last_refresh > servers._refresh_time:
-                servers.refresh_servers()
-
-            return method(servers, *args, **kwargs)
-
-        return wrapped
-
-    def __init__(
-        self,
-        main_address="master.unvanquished.net",
-        main_port=27950,
-        *,
-        max_servers=2**9,
-        update_time=60.0,
-        refresh_time=1.0,
-    ):
-        self._host = main_address
-        self._port = main_port
-        self._max_servers = max_servers
-        self._update_time = update_time
-        self._refresh_time = refresh_time
-
-        self._servers = set()
-        self._last_update = 0
-        self._last_update_error = None
-        self._last_refresh = 0
-
-    @property
-    def _main_str(self):
-        return f"{self._host}:{self._port}"
-
-    def query_addresses(self):
-        logger.debug(f"Requesting server list from {self._main_str}.")
-
-        con = socket(AF_INET, SOCK_DGRAM)
-        con.settimeout(SOCKET_TIMEOUT)
-        con.connect((self._host, self._port))
-        con.send(Q_GET_SERVERS)
-        response = con.recv(len(R_GET_SERVERS) + 7 * self._max_servers)
-
-        if not response:
-            raise RuntimeError(
-                f"Failed to query main server at {self._main_str} for servers:"
-                f" no response."
-            )
-
-        if not response.startswith(R_GET_SERVERS):
-            raise RuntimeError(
-                f"Failed to query main server at {self._main_str}:"
-                f" bad response header."
-            )
-
-        response = response[len(R_GET_SERVERS) :]
-
-        if len(response) % SERVER_RECORD_LEN:
-            raise RuntimeError(
-                f"Main server at {self._main_str} sent faulty server list:"
-                f" payload has unexpected size of {len(response)}"
-                f" (not a multiple of {SERVER_RECORD_LEN})."
-            )
-
-        num_servers = len(response) // SERVER_RECORD_LEN
-
-        for i in range(num_servers):
-            ip0, ip1, ip2, ip3, port0, port1, sep = response[
-                SERVER_RECORD_LEN * i : SERVER_RECORD_LEN * (i + 1)
-            ]
-
-            if sep != ord(RECORD_SEP):
-                raise RuntimeError(
-                    f"Main server at {self._main_str} sent faulty server list:"
-                    f" unexpected separator byte {chr(sep)}."
-                )
-
-            server_addr = f"{ip0:d}.{ip1:d}.{ip2:d}.{ip3:d}"
-            server_port = (port0 << 8) + port1
-
-            yield server_addr, server_port
-
-    def update_servers(self):
-        """Retrieve a server list and refresh all servers.
-
-        :raises RuntimeError:
-            If the server list could not be retrieved.
-        """
-        self._servers.update(
-            Server(host, port) for host, port in self.query_addresses()
-        )
-        self._last_update = unix_time()
-
-        self.refresh_servers()
-
-    def try_update_servers(self):
-        """Try to retrieve a server list and refresh all servers on success."""
-        try:
-            self.update_servers()
-        except Exception as error:
-            error_str = str(error)
-
-            # Log new errors with INFO, repeated errors with DEBUG level.
-            logger.log(
-                logging.INFO
-                if error_str != self._last_update_error
-                else logging.DEBUG,
-                f"Failed to fetch servers from {self._main_str}: {error}",
-            )
-
-            self._last_update_error = error_str
-        else:
-            self._last_update_error = None
-
-    def refresh_servers(self):
-        """Refresh all currently known servers (failure resets status)."""
-        if self._servers:
-            with ThreadPool(len(self._servers)) as pool:
-                pool.map(Server.refresh_or_reset, self._servers)
-
-            self._last_refresh = unix_time()
-
-    def _ranking(self, server):
-        return (-server.num_playing, -server.num_spectating, server.ping)
-
-    @_check_refresh
-    def online(self):
-        """Whether any servers responded recently."""
-        if not self._servers:
-            return False
-
-        if not any(
-            server.age < 1.5 * self._refresh_time for server in self._servers
-        ):
-            return False
-
-        return True
-
-    @property
-    @_check_refresh
-    def sorted_entries(self):
-        return sorted(self._servers, key=self._ranking)
-
-    @_check_refresh
-    def filter(
-        self,
-        *,
-        only_responsive=True,
-        max_servers=None,
-        max_ping=None,
-        min_players=0,
-        min_playing=0,
-    ):
-        selected = []
-        for server in self._servers:
-            if only_responsive and not server.responsive:
-                continue
-
-            if max_ping is not None and server.ping > max_ping:
-                continue
-
-            if server.num_players < min_players:
-                continue
-
-            if server.num_playing < min_playing:
-                continue
-
-            selected.append(server)
-
-            if max_servers is not None and len(selected) >= max_servers:
-                break
-
-        servers = sorted(selected, key=self._ranking)
-
-        return servers if max_servers is None else servers[:max_servers]
-
-    @property
-    @_check_refresh
-    def max_playing(self):
-        """Largest number of active players on any server."""
-        return max(server.num_playing for server in self._servers)
-
-    @_check_refresh
-    def __str__(self):
-        return "\n".join(
-            f"{server.address:>21}"
-            f" | {server.ping * 1000:3.0f} ms"
-            f" | {a}:{h}+{spec} players"
-            f" | {ab}:{hb} bots"
-            f" | {server.map_name[:15]:>15}"
-            f" | {server.stripped_name}"
-            for server in self.sorted_entries
-            for spec, a, h, ab, hb in (server.player_stats,)
-        )
-
-
-if __name__ == "__main__":
-    servers = ServerList()
-    print(servers)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `unvtray-0.1.0/unvtray/tray.py` & `unvtray-0.2.0/unvtray/tray.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,98 +10,143 @@
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
 # FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for
 # more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program.  If not, see <https://www.gnu.org/licenses/>.
 
-import subprocess
 from functools import lru_cache
 from pathlib import Path
 
 from PIL import Image, ImageDraw, ImageFont
 from pystray import Icon, Menu, MenuItem
 
+from .launch import launch
+
 ASSET_DIR = Path(__file__).parent / "assets"
+ICON_FILE = ASSET_DIR / "unvanquished.png"
+FONT_FILE = ASSET_DIR / "FreeMonoBold.otf"
+
+HIGH_PLAYER_COUNT = 6
 
 
 @lru_cache()
-def make_icon(
-    text="",
-    color="gray",
-    text_color="white",
+def _load_base_icon(size):
+    return Image.open(str(ICON_FILE)).resize((size, size))
+
+
+@lru_cache()
+def _load_font(size):
+    return ImageFont.truetype(str(FONT_FILE), size=size)
+
+
+@lru_cache()
+def _make_icon(
+    *,
     size=64,
-    text_scale=2 / 3,
-    icon_file=str(ASSET_DIR / "unvanquished.png"),
-    font_file=str(ASSET_DIR / "FreeMonoBold.otf"),
+    text="",
+    text_color="lightgray",
+    text_size=44 / 64,
+    text_hori_margin=1 / 64,
+    text_vert_margin=-2 / 64,
+    bg_color="#555",
+    border_color="#222",
+    border_width=1 / 64
 ):
-    s = size
-    th = int(text_scale * size)  # text height
-    icon = Image.open(icon_file)
-    font = ImageFont.truetype(font_file, size=th)
-    tw = font.getlength(text)  # text width
-    canvas = ImageDraw.Draw(icon)
-    canvas.rectangle((s - tw, s - th, s, s), fill=color)
-    canvas.text(
-        (s - tw, s - th),
-        text,
-        align="right",
-        font=font,
-        fill=text_color,
-    )
+    icon = _load_base_icon(size).copy()
+
+    if text:
+        s = icon.size[0]
+        h = int(text_hori_margin * s)
+        v = int(text_vert_margin * s)
+        b = int(border_width * s)
+        th = int(text_size * s)  # text height
+        font = _load_font(th)
+        tw = font.getlength(text) + 2 * h  # text width
+
+        canvas = ImageDraw.Draw(icon)
+        canvas.rectangle(
+            (s - tw - 2 * b, s - th - 2 * v - 2 * b, s - 1, s - 1),
+            fill=border_color,
+        )
+        canvas.rectangle(
+            (s - tw - b, s - th - 2 * v - b, s - b - 1, s - b - 1),
+            fill=bg_color,
+        )
+        canvas.text(
+            (s - tw - b - 1 + h, s - th - b - v - 1),
+            text,
+            align="right",
+            font=font,
+            fill=text_color,
+        )
+
     return icon
 
 
-def connect_action(server):
+def make_icon(players=None, size=64):
+    icon_data = dict(size=size, text_color="#f9fcee")
+
+    if players is None:  # No data yet.
+        pass
+    elif players < 0:  # Disconnected.
+        icon_data["text"] = "?"
+        icon_data["bg_color"] = "darkred"
+    else:
+        icon_data["text"] = f"{players:d}"
+        icon_data["bg_color"] = "#233f47"  # dark teal
+
+        if players >= HIGH_PLAYER_COUNT:
+            icon_data["bg_color"] = "darkgreen"
+            icon_data["text_color"] = "#c7ffc7"
+
+    return _make_icon(**icon_data)
+
+
+def make_connect_action(server):
     def connect():
-        subprocess.call(["xdg-open", f"unv://{server.address}"])
+        launch(server)
 
     return connect
 
 
+def launch_action():
+    launch()
+
+
 def quit_action(icon):
     if icon.next_event:
         schedule, next_event = icon.next_event
         schedule.cancel(next_event)
         icon.next_event = None
 
     icon.stop()
 
 
 def make_menu(servers=None):
     items = []
 
     if servers:
         items.extend(
-            MenuItem(str(server), connect_action(server), default=not i)
+            MenuItem(str(server), make_connect_action(server), default=not i)
             for i, server in enumerate(servers.filter())
         )
+        items.append(Menu.SEPARATOR)
 
-    items.append(Menu.SEPARATOR)
+    items.append(MenuItem("Launch Unvanquished", launch_action))
     items.append(MenuItem("Quit", quit_action))
 
     menu = Menu(*items)
     return menu
 
 
-def make_tray(servers=None, *, player_threshold=6):
-    icon_data = dict(text_color="#e1e5d9")
-
+def make_tray(servers=None):
     if servers is None:
-        pass
+        icon = make_icon(None)
     elif not servers.online():
-        icon_data["text"] = "?"
-        icon_data["color"] = "darkred"
+        icon = make_icon(-1)
     else:
-        icon_data["text"] = f"{servers.max_playing:d}"
-        icon_data["color"] = "#233f47"  # dark teal
-
-        if servers.max_playing >= player_threshold:
-            icon_data["text_color"] = "lightgreen"
+        icon = make_icon(servers.max_playing)
 
-    tray = Icon(
-        name="Unvanquished Tray",
-        icon=make_icon(**icon_data),
-        menu=make_menu(servers),
-    )
+    tray = Icon(name="Unvanquished Tray", icon=icon, menu=make_menu(servers))
 
     return tray
```

