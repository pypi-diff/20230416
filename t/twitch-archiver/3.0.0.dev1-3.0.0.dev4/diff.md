# Comparing `tmp/twitch-archiver-3.0.0.dev1.tar.gz` & `tmp/twitch-archiver-3.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-archiver-3.0.0.dev1.tar", last modified: Thu Mar  9 10:17:14 2023, max compression
+gzip compressed data, was "twitch-archiver-3.0.0.dev4.tar", last modified: Sun Apr 16 04:20:58 2023, max compression
```

## Comparing `twitch-archiver-3.0.0.dev1.tar` & `twitch-archiver-3.0.0.dev4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 10:17:14.270023 twitch-archiver-3.0.0.dev1/
--rw-rw-rw-   0        0        0    34523 2022-03-22 11:59:38.000000 twitch-archiver-3.0.0.dev1/LICENSE
--rw-rw-rw-   0        0        0    10363 2023-03-09 10:17:14.270023 twitch-archiver-3.0.0.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     9733 2023-03-04 09:28:05.000000 twitch-archiver-3.0.0.dev1/README.md
--rw-rw-rw-   0        0        0      781 2023-03-09 10:16:56.000000 twitch-archiver-3.0.0.dev1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-09 10:17:14.270023 twitch-archiver-3.0.0.dev1/setup.cfg
--rw-rw-rw-   0        0        0       92 2023-01-15 12:54:49.000000 twitch-archiver-3.0.0.dev1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 10:17:14.256284 twitch-archiver-3.0.0.dev1/twitch_archiver.egg-info/
--rw-rw-rw-   0        0        0    10363 2023-03-09 10:17:14.000000 twitch-archiver-3.0.0.dev1/twitch_archiver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      561 2023-03-09 10:17:14.000000 twitch-archiver-3.0.0.dev1/twitch_archiver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 10:17:14.000000 twitch-archiver-3.0.0.dev1/twitch_archiver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-03-09 10:17:14.000000 twitch-archiver-3.0.0.dev1/twitch_archiver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-03-09 10:17:14.000000 twitch-archiver-3.0.0.dev1/twitch_archiver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-09 10:17:14.268022 twitch-archiver-3.0.0.dev1/twitcharchiver/
--rw-rw-rw-   0        0        0    11183 2023-03-09 08:52:42.000000 twitch-archiver-3.0.0.dev1/twitcharchiver/__init__.py
--rw-rw-rw-   0        0        0     3958 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev1/twitcharchiver/api.py
--rw-rw-rw-   0        0        0     3910 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev1/twitcharchiver/arguments.py
--rw-rw-rw-   0        0        0     5015 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev1/twitcharchiver/configuration.py
--rw-rw-rw-   0        0        0     7401 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev1/twitcharchiver/database.py
--rw-rw-rw-   0        0        0    10173 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev1/twitcharchiver/downloader.py
--rw-rw-rw-   0        0        0     4263 2023-03-04 09:28:05.000000 twitch-archiver-3.0.0.dev1/twitcharchiver/exceptions.py
--rw-rw-rw-   0        0        0     1672 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev1/twitcharchiver/logger.py
--rw-rw-rw-   0        0        0    40690 2023-03-09 10:02:35.000000 twitch-archiver-3.0.0.dev1/twitcharchiver/processing.py
--rw-rw-rw-   0        0        0    12861 2023-03-09 10:00:59.000000 twitch-archiver-3.0.0.dev1/twitcharchiver/stream.py
--rw-rw-rw-   0        0        0    11413 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev1/twitcharchiver/twitch.py
--rw-rw-rw-   0        0        0    25076 2023-03-04 09:27:57.000000 twitch-archiver-3.0.0.dev1/twitcharchiver/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:20:58.948715 twitch-archiver-3.0.0.dev4/
+-rw-rw-rw-   0        0        0    34523 2022-03-22 11:59:38.000000 twitch-archiver-3.0.0.dev4/LICENSE
+-rw-rw-rw-   0        0        0    10416 2023-04-16 04:20:58.948715 twitch-archiver-3.0.0.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     9786 2023-04-16 04:19:29.000000 twitch-archiver-3.0.0.dev4/README.md
+-rw-rw-rw-   0        0        0      781 2023-04-16 04:19:15.000000 twitch-archiver-3.0.0.dev4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 04:20:58.948715 twitch-archiver-3.0.0.dev4/setup.cfg
+-rw-rw-rw-   0        0        0       92 2023-01-15 12:54:49.000000 twitch-archiver-3.0.0.dev4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:20:58.936713 twitch-archiver-3.0.0.dev4/twitch_archiver.egg-info/
+-rw-rw-rw-   0        0        0    10416 2023-04-16 04:20:58.000000 twitch-archiver-3.0.0.dev4/twitch_archiver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      561 2023-04-16 04:20:58.000000 twitch-archiver-3.0.0.dev4/twitch_archiver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 04:20:58.000000 twitch-archiver-3.0.0.dev4/twitch_archiver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-16 04:20:58.000000 twitch-archiver-3.0.0.dev4/twitch_archiver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-16 04:20:58.000000 twitch-archiver-3.0.0.dev4/twitch_archiver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 04:20:58.947715 twitch-archiver-3.0.0.dev4/twitcharchiver/
+-rw-rw-rw-   0        0        0    11567 2023-04-16 04:16:02.000000 twitch-archiver-3.0.0.dev4/twitcharchiver/__init__.py
+-rw-rw-rw-   0        0        0     3958 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev4/twitcharchiver/api.py
+-rw-rw-rw-   0        0        0     3910 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev4/twitcharchiver/arguments.py
+-rw-rw-rw-   0        0        0     5015 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev4/twitcharchiver/configuration.py
+-rw-rw-rw-   0        0        0     7401 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev4/twitcharchiver/database.py
+-rw-rw-rw-   0        0        0    10173 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev4/twitcharchiver/downloader.py
+-rw-rw-rw-   0        0        0     4263 2023-03-04 09:28:05.000000 twitch-archiver-3.0.0.dev4/twitcharchiver/exceptions.py
+-rw-rw-rw-   0        0        0     1672 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev4/twitcharchiver/logger.py
+-rw-rw-rw-   0        0        0    41120 2023-04-16 04:17:34.000000 twitch-archiver-3.0.0.dev4/twitcharchiver/processing.py
+-rw-rw-rw-   0        0        0    13327 2023-03-18 05:40:32.000000 twitch-archiver-3.0.0.dev4/twitcharchiver/stream.py
+-rw-rw-rw-   0        0        0    11413 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev4/twitcharchiver/twitch.py
+-rw-rw-rw-   0        0        0    26558 2023-03-18 06:42:00.000000 twitch-archiver-3.0.0.dev4/twitcharchiver/utils.py
```

### Comparing `twitch-archiver-3.0.0.dev1/LICENSE` & `twitch-archiver-3.0.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev1/PKG-INFO` & `twitch-archiver-3.0.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 3.0.0.dev1
+Version: 3.0.0.dev4
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,15 @@
     * [Usage](#usage)
     * [Arguments](#arguments)
   * [Disclaimer](#disclaimer)
 
 ## Features
 * Archives both video and chat logs.
 * VODs can be downloaded as fast as your Internet connection (and storage) can handle.[^1]
-* Allows the downloading of live VODs before sections are muted or deleted.[^2]
+* Allows real-time archiving of Twitch streams.[^2]
 * Generates a readable chat log with timestamps and user badges.
 * Supports downloading streams which aren't being archived by Twitch.
 * Error notifications supported with pushbullet.
 * Supports archiving of subscriber-only VODs.
 
 [^1]: If you wish to speed up (or slow down) the downloading of VOD pieces, supply the '--threads NUMBER' argument to the script. This changes how many download threads are used to grab the individual video files. With the default of 20, I can max out my gigabit Internet while downloading to an M.2 drive.
 [^2]: There is one caveat with live archiving due to how Twitch presents ads. Ads are not downloaded, BUT while an ad is displayed, the actual stream output is not sent. This can result in missing segments under very rare circumstances, but any missing segments should be filled via a parallel VOD archival function. 
@@ -64,16 +64,17 @@
 2. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
 3. Download and install TA with `python -m pip install twitch-archiver`.
 
 #### Installing Manually
 
 1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
 2. Unpack the archive and enter the directory with `cd twitch-archiver`.
-2. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
-3. Build the package with `python -m build`, then install with `python -m pip install ./dist/twitch-archiver-*.tar.gz`.
+3. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
+4. Install Python "Build" package with `python -m pip install --upgrade build`.
+5. Build the package with `python -m build`, then install with `python -m pip install ./dist/twitch-archiver-*.tar.gz`.
 
 #### Installing as a Docker Container
 1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
 2. Unpack the archive and enter the directory with `cd twitch-archiver`.
 3. Build the container with `docker build . -t twitch-archiver`.
 4. Run the container with the following command. *Configuration can also be provided via environment variables (see [wiki]((https://github.com/Brisppy/twitch-archiver/wiki/Wiki#environment-variables)))*.
 ```bash
```

### Comparing `twitch-archiver-3.0.0.dev1/README.md` & `twitch-archiver-3.0.0.dev4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     * [Usage](#usage)
     * [Arguments](#arguments)
   * [Disclaimer](#disclaimer)
 
 ## Features
 * Archives both video and chat logs.
 * VODs can be downloaded as fast as your Internet connection (and storage) can handle.[^1]
-* Allows the downloading of live VODs before sections are muted or deleted.[^2]
+* Allows real-time archiving of Twitch streams.[^2]
 * Generates a readable chat log with timestamps and user badges.
 * Supports downloading streams which aren't being archived by Twitch.
 * Error notifications supported with pushbullet.
 * Supports archiving of subscriber-only VODs.
 
 [^1]: If you wish to speed up (or slow down) the downloading of VOD pieces, supply the '--threads NUMBER' argument to the script. This changes how many download threads are used to grab the individual video files. With the default of 20, I can max out my gigabit Internet while downloading to an M.2 drive.
 [^2]: There is one caveat with live archiving due to how Twitch presents ads. Ads are not downloaded, BUT while an ad is displayed, the actual stream output is not sent. This can result in missing segments under very rare circumstances, but any missing segments should be filled via a parallel VOD archival function. 
@@ -50,16 +50,17 @@
 2. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
 3. Download and install TA with `python -m pip install twitch-archiver`.
 
 #### Installing Manually
 
 1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
 2. Unpack the archive and enter the directory with `cd twitch-archiver`.
-2. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
-3. Build the package with `python -m build`, then install with `python -m pip install ./dist/twitch-archiver-*.tar.gz`.
+3. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
+4. Install Python "Build" package with `python -m pip install --upgrade build`.
+5. Build the package with `python -m build`, then install with `python -m pip install ./dist/twitch-archiver-*.tar.gz`.
 
 #### Installing as a Docker Container
 1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
 2. Unpack the archive and enter the directory with `cd twitch-archiver`.
 3. Build the container with `docker build . -t twitch-archiver`.
 4. Run the container with the following command. *Configuration can also be provided via environment variables (see [wiki]((https://github.com/Brisppy/twitch-archiver/wiki/Wiki#environment-variables)))*.
 ```bash
```

### Comparing `twitch-archiver-3.0.0.dev1/pyproject.toml` & `twitch-archiver-3.0.0.dev4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "twitch-archiver"
-version = "3.0.0.dev1"
+version = "3.0.0.dev4"
 authors = [
   { name="Brisppy", email="brisppy@protonmail.com" },
 ]
 description = "A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `twitch-archiver-3.0.0.dev1/twitch_archiver.egg-info/PKG-INFO` & `twitch-archiver-3.0.0.dev4/twitch_archiver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 3.0.0.dev1
+Version: 3.0.0.dev4
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,15 @@
     * [Usage](#usage)
     * [Arguments](#arguments)
   * [Disclaimer](#disclaimer)
 
 ## Features
 * Archives both video and chat logs.
 * VODs can be downloaded as fast as your Internet connection (and storage) can handle.[^1]
-* Allows the downloading of live VODs before sections are muted or deleted.[^2]
+* Allows real-time archiving of Twitch streams.[^2]
 * Generates a readable chat log with timestamps and user badges.
 * Supports downloading streams which aren't being archived by Twitch.
 * Error notifications supported with pushbullet.
 * Supports archiving of subscriber-only VODs.
 
 [^1]: If you wish to speed up (or slow down) the downloading of VOD pieces, supply the '--threads NUMBER' argument to the script. This changes how many download threads are used to grab the individual video files. With the default of 20, I can max out my gigabit Internet while downloading to an M.2 drive.
 [^2]: There is one caveat with live archiving due to how Twitch presents ads. Ads are not downloaded, BUT while an ad is displayed, the actual stream output is not sent. This can result in missing segments under very rare circumstances, but any missing segments should be filled via a parallel VOD archival function. 
@@ -64,16 +64,17 @@
 2. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
 3. Download and install TA with `python -m pip install twitch-archiver`.
 
 #### Installing Manually
 
 1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
 2. Unpack the archive and enter the directory with `cd twitch-archiver`.
-2. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
-3. Build the package with `python -m build`, then install with `python -m pip install ./dist/twitch-archiver-*.tar.gz`.
+3. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
+4. Install Python "Build" package with `python -m pip install --upgrade build`.
+5. Build the package with `python -m build`, then install with `python -m pip install ./dist/twitch-archiver-*.tar.gz`.
 
 #### Installing as a Docker Container
 1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
 2. Unpack the archive and enter the directory with `cd twitch-archiver`.
 3. Build the container with `docker build . -t twitch-archiver`.
 4. Run the container with the following command. *Configuration can also be provided via environment variables (see [wiki]((https://github.com/Brisppy/twitch-archiver/wiki/Wiki#environment-variables)))*.
 ```bash
```

### Comparing `twitch-archiver-3.0.0.dev1/twitch_archiver.egg-info/SOURCES.txt` & `twitch-archiver-3.0.0.dev4/twitch_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev1/twitcharchiver/__init__.py` & `twitch-archiver-3.0.0.dev4/twitcharchiver/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 
 from twitcharchiver.arguments import Arguments
 from twitcharchiver.configuration import Configuration
 from twitcharchiver.exceptions import TwitchAPIError
 from twitcharchiver.logger import Logger
 from twitcharchiver.processing import Processing
 from twitcharchiver.twitch import Twitch
-from twitcharchiver.utils import getenv, send_push, get_latest_version, version_tuple
+from twitcharchiver.utils import getenv, send_push, get_latest_version, version_tuple, check_update_available
 
-__version__ = '3.0.0'
+__version__ = '3.0.0.dev4'
 
 
 def main():
     """
     Main processing for twitch-archiver.
     """
     parser = argparse.ArgumentParser(argument_default=None, description=textwrap.dedent(f"""\
@@ -101,32 +101,36 @@
     parser.add_argument('-d', '--directory', action='store',
                         help='Directory to store archived VOD(s), use TWO slashes for Windows paths.\n'
                              '(default: %(default)s)', type=Path,
                         default=getenv('TWITCH_ARCHIVER_DIRECTORY', Path(os.getcwd())))
     parser.add_argument('-w', '--watch', action='store_true',
                         help='Continually check every 10 seconds for new streams/VODs from a specified channel.',
                         default=getenv('TWITCH_ARCHIVER_WATCH', False, True))
-    stream.add_argument('-S', '--stream-only', action='store_true',
-                        default=getenv('TWITCH_ARCHIVER_STREAM_ONLY', False, True),
-                        help='Only download streams which are currently live.')
-    stream.add_argument('-N', '--no-stream', action='store_true',
-                        help="Don't download streams which are currently live.",
-                        default=getenv("TWITCH_ARCHIVER_NO_STREAM", False, True))
+    stream.add_argument('-l', '--live-only', action='store_true',
+                        default=getenv('TWITCH_ARCHIVER_LIVE_ONLY', False, True),
+                        help='Only download streams / VODs which are currently live.')
+    stream.add_argument('-a', '--archive-only', action='store_true',
+                        help="Don't download streams / VODs which are currently live.",
+                        default=getenv("TWITCH_ARCHIVER_ARCHIVE_ONLY", False, True))
+    stream.add_argument('-R', '--real-time-archiver', action='store_true',
+                        help="Enable real-time stream archiver.\n"
+                             "Read https://github.com/Brisppy/twitch-archiver/wiki/Wiki#real-time-archiver.",
+                        default=getenv('TWITCH_ARCHIVER_REAL_TIME_ARCHIVER', False, True))
     parser.add_argument('-L', '--log-file', action='store', help='Output logs to specified file.', type=Path,
                         default=getenv("TWITCH_ARCHIVER_LOG_FILE", False))
     parser.add_argument('-I', '--config-dir', action='store', type=Path,
                         help='Directory to store configuration, VOD database and lock files.\n(default: %(default)s)',
                         default=getenv('TWITCH_ARCHIVER_CONFIG_DIR',
-                                             Path(os.path.expanduser("~"), '.config', 'twitch-archiver')))
+                                       Path(os.path.expanduser("~"), '.config', 'twitch-archiver')))
     parser.add_argument('-p', '--pushbullet-key', action='store',
                         help='Pushbullet key for sending pushes on error. Enabled by supplying key.',
                         default=getenv("TWITCH_ARCHIVER_PUSHBULLET_KEY", False))
     loglevel.add_argument('-Q', '--quiet', action='store_const', help='Disable all log output.', const=50, default=0)
     loglevel.add_argument('-D', '--debug', action='store_const', help='Enable debug logs.', const=10, default=0)
-    parser.add_argument('--version', action='version', version=f'{__name__} v{__version__}',
+    parser.add_argument('--version', action='version', version=f'Twitch Archiver v{__version__}',
                         help='Show version number and exit.')
     parser.add_argument('--show-config', action='store_true', help='Show saved config and exit.', default=False)
 
     # setup arguments
     args = Arguments()
     args.setup_args(parser.parse_args().__dict__)
 
@@ -140,15 +144,15 @@
         if args_sanitized[key]:
             args_sanitized.update({key: 24 * '*' + args_sanitized[key][24:]})
 
     log.debug('Arguments: %s', args_sanitized)
 
     # compare with current git version
     latest_version, release_notes = get_latest_version()
-    if version_tuple(__version__) < version_tuple(latest_version):
+    if check_update_available(__version__, latest_version):
         log.warning('New version of Twitch-Archiver available - Version %s:\n'
                     'https://github.com/Brisppy/twitch-archiver/releases/latest\nRelease notes:\n\n%s\n',
                     latest_version, release_notes)
     else:
         log.info('Twitch Archiver v%s - https://github.com/Brisppy/twitch-archiver', __version__)
 
     # load configuration from ini
@@ -173,15 +177,15 @@
         log.debug('No OAuth token found, or token is invalid or expiring soon - generating a new one.')
         try:
             config.set('oauth_token', call_twitch.generate_oauth_token())
             log.debug('New OAuth token is: %s', config.get_sanitized("oauth_token"))
             # store returned token
             config.save(Path(args.get('config_dir'), 'config.ini'))
         except TwitchAPIError as err:
-            log.error('OAuth token generation failed. Error: $s', str(err))
+            log.error('OAuth token generation failed. Error: %s', str(err))
             send_push(config.get('pushbullet_key'), 'OAuth token generation failed.', str(err))
             sys.exit(1)
 
     process = Processing(config.get(), args.get())
 
     while True:
         if args.get('channel') is not None:
```

### Comparing `twitch-archiver-3.0.0.dev1/twitcharchiver/api.py` & `twitch-archiver-3.0.0.dev4/twitcharchiver/api.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev1/twitcharchiver/arguments.py` & `twitch-archiver-3.0.0.dev4/twitcharchiver/arguments.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev1/twitcharchiver/configuration.py` & `twitch-archiver-3.0.0.dev4/twitcharchiver/configuration.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev1/twitcharchiver/database.py` & `twitch-archiver-3.0.0.dev4/twitcharchiver/database.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev1/twitcharchiver/downloader.py` & `twitch-archiver-3.0.0.dev4/twitcharchiver/downloader.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev1/twitcharchiver/exceptions.py` & `twitch-archiver-3.0.0.dev4/twitcharchiver/exceptions.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev1/twitcharchiver/logger.py` & `twitch-archiver-3.0.0.dev4/twitcharchiver/logger.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev1/twitcharchiver/processing.py` & `twitch-archiver-3.0.0.dev4/twitcharchiver/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,16 @@
         self.log = logging.getLogger()
 
         self.directory = args['directory']
         self.vod_directory = Path(self.directory)
         self.video = args['video']
         self.chat = args['chat']
         self.quality = args['quality']
-        self.stream_only = args['stream_only']
-        self.no_stream = args['no_stream']
+        self.live_only = args['live_only']
+        self.archive_only = args['archive_only']
         self.config_dir = args['config_dir']
         self.quiet = args['quiet']
         self.debug = args['debug']
 
         self.client_id = config['client_id']
         self.client_secret = config['client_secret']
         self.oauth_token = config['oauth_token']
@@ -105,41 +105,42 @@
             channel_data = self.call_twitch.get_api(f'streams?user_id={user_id}')['data']
             if channel_data and channel_data[0]['type'] == 'live':
                 channel_live = True
                 # ensure enough time has passed for vod api to update before archiving
                 stream_length = time_since_date(datetime.strptime(
                     channel_data[0]['started_at'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc).timestamp())
 
+                # TODO: ensure that if the stream ends, we clean up and merge segments
                 # while we wait for the api to update we must build a temporary buffer of any parts advertised in the
                 # meantime in case there is no vod and thus no way to retrieve them after the fact
-                if stream_length < 60:
-                    self.log.debug('Stream began less than 60s ago, delaying archival start until VOD API updated.')
+                if stream_length < 90:
+                    self.log.debug('Stream began less than 90s ago, delaying archival start until VOD API updated.')
                     # create temp dir for buffer
                     Path(tmp_buffer_dir).mkdir(parents=True, exist_ok=True)
 
                     stream.unsynced_setup(tmp_buffer_dir)
                     index_uri = self.call_twitch.get_channel_hls_index(channel, self.quality)
 
                     # download new parts every 4s
-                    for i in range(int((60 - stream_length) / 4)):
+                    for i in range(int((90 - stream_length) / 4)):
                         # grab required values
                         start_timestamp = int(datetime.utcnow().timestamp())
                         incoming_segments = m3u8.loads(Api.get_request(index_uri).text).data
 
                         # create buffer and download segments to temp dir
                         stream.build_unsynced_buffer(incoming_segments)
                         stream.download_buffer(tmp_buffer_dir)
 
                         # wait if less than 5s passed since grabbing more parts
                         processing_time = int(datetime.utcnow().timestamp() - start_timestamp)
                         if processing_time < 4:
                             sleep(4 - processing_time)
 
                     # wait any remaining time
-                    sleep((60 - stream_length) % 4)
+                    sleep((90 - stream_length) % 4)
 
             # retrieve available vods
             available_vods: dict[int: tuple[int]] = {}
             cursor = ''
             try:
                 while True:
                     _r = self.call_twitch.get_api(f'videos?user_id={user_id}&first=100&type=archive&after={cursor}')
@@ -150,25 +151,23 @@
                     available_vods.update(dict([(int(vod['stream_id']), (vod['id'])) for vod in _r['data']]))
                     cursor = _r['pagination']['cursor']
 
             except BaseException as e:
                 self.log.error('Error retrieving VODs from Twitch. Error: %s', str(e))
                 continue
 
-            self.log.info(f'Online VODs: {available_vods}' if self.debug
-                          else f'Online VODs: {len(available_vods)}')
+            self.log.debug(f'Online VODs: {available_vods}')
 
             # retrieve downloaded vods
             with Database(Path(self.config_dir, 'vods.db')) as db:
                 # dict containing stream_id: (vod_id, video_downloaded, chat_downloaded)
                 downloaded_vods = dict([(i[0], (i[1], i[2], i[3])) for i in db.execute_query(
                     'SELECT stream_id, vod_id, video_archived, chat_archived FROM vods WHERE user_id IS ?',
                     {'user_id': user_id})])
-            self.log.info(f'Downloaded vods: {downloaded_vods}' if self.debug
-                          else f'Downloaded vods: {len(downloaded_vods)}')
+            self.log.debug(f'Downloaded vods: {downloaded_vods}')
 
             # generate vod queue using downloaded and available vods
             vod_queue = {}
             for stream_id in available_vods.keys():
                 # add any vods not present in database
                 if stream_id not in downloaded_vods.keys():
                     vod_queue.update({stream_id: (available_vods[stream_id], self.video, self.chat)})
@@ -186,23 +185,26 @@
                                                   not downloaded_vods[stream_id][1] and self.video,
                                                   not downloaded_vods[stream_id][2] and self.chat)})
 
             # check if stream being archived to vod
             live_vod_exists = (channel_data and int(channel_data[0]['id']) in available_vods.keys())
 
             # move on if channel offline and no vods are available
-            if not self.stream_only and not channel_live and not available_vods:
+            if not self.live_only and not channel_live and not available_vods:
                 self.log.info('No VODs were found for %s.', user_name)
                 continue
 
-            if not channel_live and self.stream_only:
+            # move on if channel offline and we are only looking for live vods
+            if not channel_live and self.live_only:
+                self.log.info('Running in stream-only mode and no stream available for %s.', user_name)
                 continue
 
-            # archive stream in non-segmented mode if no paired vod exists
-            if not self.no_stream and channel_live and not live_vod_exists and self.video:
+            # archive stream in non-segmented mode if no paired vod exists, unless we are in no_stream mode or not
+            # archiving video.
+            if not self.archive_only and channel_live and not live_vod_exists and self.video:
                 self.log.info('Channel live but not being archived to a VOD, running stream archiver.')
                 self.log.debug('Creating lock file for stream.')
 
                 if create_lock(self.config_dir, channel_data[0]['id'] + '-stream-only'):
                     self.log.info('Lock file present for stream by %s (.lock.%s-stream-only), skipping.',
                                   user_name, channel_data[0]["id"])
 
@@ -210,15 +212,15 @@
                     # check if stream in database
                     with Database(Path(self.config_dir, 'vods.db')) as db:
                         downloaded_streams = [str(i[0]) for i in db.execute_query(
                             'SELECT stream_id FROM vods WHERE user_id IS ?', {'user_id': user_id})]
 
                     # Check if stream id in database
                     if channel_data[0]['id'] in downloaded_streams:
-                        self.log.info('Stream has already been downloaded.')
+                        self.log.info('Ignoring steam as it has already been downloaded.')
 
                     else:
                         try:
                             # move parts from temp stream buffer to output dir
                             # gather parts from temp dir
                             buffered_parts = [Path(p) for p in sorted(glob(str(Path(tmp_buffer_dir, '*.ts'))))]
                             # create output dir
@@ -267,19 +269,21 @@
 
             self.log.info('%s VOD(s) in download queue.', len(vod_queue))
             self.log.debug('VOD queue: %s', vod_queue)
 
             # begin processing each available vod
             for stream_id in vod_queue:
                 vod_id = vod_queue[stream_id][0]
-                # skip if we are only after the current stream
-                if channel_data and self.stream_only and stream_id != int(channel_data[0]['id']):
+
+                # skip if we are only after currently live streams, and stream_id is not live
+                if channel_data and self.live_only and stream_id != int(channel_data[0]['id']):
                     continue
 
-                if channel_data and self.no_stream and stream_id == int(channel_data[0]['id']):
+                # skip if we aren't after currently lives streams, and stream_id is live
+                if channel_data and self.archive_only and stream_id == int(channel_data[0]['id']):
                     self.log.info('Skipping VOD as it is live and no-stream argument provided.')
                     continue
 
                 self.log.debug('Processing VOD %s by %s', vod_id, user_name)
                 self.log.debug('Creating lock file for VOD.')
 
                 if create_lock(self.config_dir, stream_id):
@@ -428,15 +432,16 @@
         vod_live = self.call_twitch.get_vod_status(vod_json['user_id'], vod_json['created_at'])
 
         self.log.info("VOD %s", 'currently or recently live. Running in LIVE mode.' if vod_live else 'offline.')
 
         _r = None
 
         try:
-            if vod_live:
+            # begin real-time archiver if VOD still live and real-time archiver enabled
+            if self.real_time_archiver and vod_live:
                 stream = Stream(self.client_id, self.client_secret, self.oauth_token)
                 # concurrently grab live pieces and vod chunks
 
                 workers = []
 
                 # the stream module itself has no checks for what to download so this is done here
                 if get_video:
```

### Comparing `twitch-archiver-3.0.0.dev1/twitcharchiver/stream.py` & `twitch-archiver-3.0.0.dev4/twitcharchiver/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,22 +78,33 @@
         except TwitchAPIErrorNotFound:
             self.log.error('Stream offline.')
             return
 
         while True:
             start_timestamp = int(datetime.utcnow().timestamp())
 
-            try:
-                self.log.debug('Fetching incoming stream segments.')
-                incoming_segments = m3u8.loads(Api.get_request(index_uri).text).data
-
-            # stream has ended if exception encountered
-            except TwitchAPIErrorNotFound:
-                self.get_final_segment(self.buffer, output_dir, self.segment_ids)
-                return
+            # attempt to grab new segments from Twitch
+            for attempt in range(6):
+                if attempt > 4:
+                    return
+
+                try:
+                    self.log.debug('Fetching incoming stream segments.')
+                    incoming_segments = m3u8.loads(Api.get_request(index_uri).text).data
+                    break
+
+                # stream has ended if exception encountered
+                except TwitchAPIErrorNotFound:
+                    self.get_final_segment(self.buffer, output_dir, self.segment_ids)
+                    return
+
+                except requests.exceptions.ConnectTimeout:
+                    self.log.debug('Timed out attempting to fetch new stream segments, retrying. (Attempt %s)',
+                                   attempt + 1)
+                    continue
 
             # set latest segment and timestamp if new segment found
             if incoming_segments['segments'][-1]['uri'] != latest_segment:
                 latest_segment = incoming_segments['segments'][-1]['uri']
                 latest_segment_timestamp = int(datetime.now(timezone.utc).timestamp())
 
             # assume stream has ended once >20s has passed since the last segment was advertised
```

### Comparing `twitch-archiver-3.0.0.dev1/twitcharchiver/twitch.py` & `twitch-archiver-3.0.0.dev4/twitcharchiver/twitch.py`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev1/twitcharchiver/utils.py` & `twitch-archiver-3.0.0.dev4/twitcharchiver/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         if '.' in comment['createdAt']:
             created_time = \
                 datetime.strptime(comment['createdAt'], '%Y-%m-%dT%H:%M:%S.%fZ').replace(tzinfo=timezone.utc)
         else:
             created_time = \
                 datetime.strptime(comment['createdAt'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc)
 
-        comment_time = '{:.3f}'.format(get_time_difference(stream_start, created_time))
+        comment_time = f'{get_time_difference(stream_start, created_time):.3f}'
 
         # catch comments without commenter informations
         if comment['commenter']:
             user_name = str(comment['commenter']['displayName'])
         else:
             user_name = '~MISSING_COMMENTER_INFO~'
 
@@ -103,28 +103,28 @@
 
 
 def export_json(vod_json):
     """Exports all VOD information to a file.
 
     :param vod_json: dict of vod parameters retrieved from twitch
     """
-    with open(Path(vod_json['store_directory'], 'vod.json'), 'w') as json_out_file:
+    with open(Path(vod_json['store_directory'], 'vod.json'), 'w', encoding='utf8') as json_out_file:
         json_out_file.write(json.dumps(vod_json))
 
 
 def import_json(vod_json):
     """Imports all VOD information from a file.
 
     :param vod_json: dict of vod parameters retrieved from twitch
     """
     if Path(vod_json['store_directory'], 'vod.json').exists():
-        with open(Path(vod_json['store_directory'], 'vod.json'), 'r') as json_in_file:
+        with open(Path(vod_json['store_directory'], 'vod.json'), 'r', encoding='utf8') as json_in_file:
             return json.loads(json_in_file.read())
 
-    return
+    return []
 
 
 def combine_vod_parts(vod_json, print_progress=True):
     """Combines the downloaded VOD .ts parts.
 
     :param vod_json: dict of vod parameters retrieved from twitch
     :param print_progress: boolean whether to print progress bar
@@ -154,18 +154,18 @@
                 if print_progress:
                     progress.print_progress(pr, len(vod_parts))
 
     else:
         # merge all .ts files with ffmpeg concat demuxer as missing segments can cause corruption with
         # other method
 
-        log.debug(f'Discontinuity found, merging with ffmpeg.\n Discontinuity: {dicontinuity}')
+        log.debug('Discontinuity found, merging with ffmpeg.\n Discontinuity: %s', dicontinuity)
 
         # create file with list of parts for ffmpeg
-        with open(Path(vod_json['store_directory'], 'parts', 'segments.txt'), mode='w') as segment_file:
+        with open(Path(vod_json['store_directory'], 'parts', 'segments.txt'), 'w', encoding='utf8') as segment_file:
             for part in vod_parts:
                 segment_file.write(f"file '{part}'\n")
 
         with subprocess.Popen(f'ffmpeg -hide_banner -fflags +genpts -f concat -safe 0 -y -i '
                               f'"{str(Path(vod_json["store_directory"], "parts", "segments.txt"))}"'
                               f' -c copy "{str(Path(vod_json["store_directory"], "merged.ts"))}"',
                               shell=True, stderr=subprocess.PIPE, universal_newlines=True) as p:
@@ -177,15 +177,15 @@
                     current_time = \
                         int(current_time[0]) * 3600 + int(current_time[1]) * 60 + int(current_time[2][:2])
 
                     if print_progress:
                         progress.print_progress(int(current_time), vod_json['duration'])
 
             if p.returncode:
-                log.error(f'VOD merger exited with error. Command: {p.args}.')
+                log.error('VOD merger exited with error. Command: %s.', p.args)
                 raise VodConvertError(f'VOD merger exited with error. Command: {p.args}.')
 
 
 def convert_vod(vod_json, ignore_corruptions=None, print_progress=True):
     """Converts the VOD from a .ts format to .mp4.
 
     :param vod_json: dict of vod parameters retrieved from twitch
@@ -200,17 +200,17 @@
     corrupt_part_whitelist = set()
     if ignore_corruptions:
         # create corrupt part whitelist form provided (min, max) ranges. The given range is expanded +-2 as the
         # DTS timestamps can still be wonky past them
         [corrupt_part_whitelist.update(r) for r in [range(t[0] - 2, t[1] + 3) for t in ignore_corruptions]]
 
     # get dts offset of first part
-    with subprocess.Popen(
-            f'ffprobe -v quiet -print_format json -show_format -show_streams "{Path(vod_json["store_directory"], "parts", "00000.ts")}"', shell=True,
-            stdout=subprocess.PIPE, universal_newlines=True) as p:
+    with subprocess.Popen(f'ffprobe -v quiet -print_format json -show_format -show_streams '
+                          f'"{Path(vod_json["store_directory"], "parts", "00000.ts")}"', shell=True,
+                          stdout=subprocess.PIPE, universal_newlines=True) as p:
         ts_file_data = ''
         for line in p.stdout:
             ts_file_data += line
 
         dts_offset = float(json.loads(ts_file_data)['format']['start_time']) * 90000
 
     # create ffmpeg command
@@ -236,35 +236,34 @@
                     progress.print_progress(int(current_time), vod_json['duration'])
 
             elif 'Packet corrupt' in line:
                 try:
                     dts_timestamp = int(re.search(r'(?<=dts = ).*(?=\).)', line).group(0))
 
                 # Catch corrupt parts without timestamp, shows up as 'NOPTS'
-                except ValueError:
+                except ValueError as e:
                     raise VodConvertError("Corrupt packet encountered at unknown timestamp while converting VOD. "
-                                          "Delete 'parts' folder and re-download VOD.")
+                                          "Delete 'parts' folder and re-download VOD.") from e
 
                 corrupt_part = floor((dts_timestamp - dts_offset) / 90000 / 10)
 
                 # ignore if corrupt packet within ignore_corruptions range
                 if corrupt_part in corrupt_part_whitelist:
-                    log.debug(f'Ignoring corrupt packet as part in whitelist. Part: {corrupt_part}')
-                    pass
+                    log.debug('Ignoring corrupt packet as part in whitelist. Part: %s', corrupt_part)
 
                 else:
                     corrupt_parts.add(int(corrupt_part))
-                    log.error(f'Corrupt packet encountered. Part: {corrupt_part}')
+                    log.error('Corrupt packet encountered. Part: %s', corrupt_part)
 
     if p.returncode:
         log.debug('FFmpeg exited with error code, output dumped to VOD directory.')
-        with open(Path(vod_json["store_directory"], 'parts', 'ffmpeg.log'), 'w') as ffout:
+        with open(Path(vod_json["store_directory"], 'parts', 'ffmpeg.log'), 'w', encoding='utf8') as ffout:
             ffout.write(ffmpeg_log)
 
-        raise VodConvertError(f"VOD converter exited with error. Delete 'parts' directory and re-download VOD.")
+        raise VodConvertError("VOD converter exited with error. Delete 'parts' directory and re-download VOD.")
 
     if corrupt_parts:
         corrupted_ranges = to_ranges(corrupt_parts)
         formatted_ranges = []
         for t in corrupted_ranges:
             if t[0] == t[1]:
                 formatted_ranges.append(f'{t[0]}.ts')
@@ -273,14 +272,19 @@
 
         # raise error so we can try to recover
         raise CorruptPartError(corrupt_parts, formatted_ranges)
 
 
 # https://stackoverflow.com/a/43091576
 def to_ranges(iterable):
+    """Converts a list of integers to iterable sets of (low, high) (e.g [0, 1, 2, 5, 7, 8] -> (0, 2), (5, 5), (7, 8))
+
+    :param iterable: list of integers
+    :return: iterable generator of separate integer ranges
+    """
     iterable = sorted(set(iterable))
     for key, group in groupby(enumerate(iterable), lambda t: t[1] - t[0]):
         group = list(group)
         yield group[0][1], group[-1][1]
 
 
 def verify_vod_length(vod_json):
@@ -298,33 +302,32 @@
 
     # retrieve vod file duration
     p = subprocess.run(f'ffprobe -v quiet -i "{Path(vod_json["store_directory"], "vod.mp4")}" '
                        f'-show_entries format=duration -of default=noprint_wrappers=1:nokey=1',
                        shell=True, capture_output=True)
 
     if p.returncode:
-        log.error(f'VOD length verification exited with error. Command: {p.args}.')
+        log.error('VOD length verification exited with error. Command: %s.', p.args)
         raise VodConvertError(f'VOD length verification exited with error. Command: {p.args}.')
 
     try:
         downloaded_length = int(float(p.stdout.decode('ascii').rstrip()))
 
     except Exception as e:
-        log.error(f'Failed to fetch downloaded VOD length. VOD may not have downloaded correctly. {e}')
-        raise VodConvertError(str(e))
+        log.error('Failed to fetch downloaded VOD length. VOD may not have downloaded correctly. %s', str(e))
+        raise VodConvertError(str(e)) from e
 
-    log.debug(f'Downloaded VOD length is {downloaded_length}. Expected length is {vod_json["duration"]}.')
+    log.debug('Downloaded VOD length is %s. Expected length is %s.', downloaded_length, vod_json["duration"])
 
     # pass verification if downloaded file is within 2s of expected length
     if 2 >= downloaded_length - vod_json['duration'] >= -2:
         log.debug('VOD passed length verification.')
         return False
 
-    else:
-        return True
+    return True
 
 
 def cleanup_vod_parts(vod_directory):
     """Deletes temporary and transitional files used for archiving VOD videos.
 
     :param vod_directory: directory of downloaded vod which needs to be cleaned up
     """
@@ -360,57 +363,59 @@
     :return: time in seconds
     """
     duration = duration.replace('h', ':').replace('m', ':').replace('s', '').split(':')
 
     if len(duration) == 1:
         return int(duration[0])
 
-    elif len(duration) == 2:
+    if len(duration) == 2:
         return (int(duration[0]) * 60) + int(duration[1])
 
-    elif len(duration) == 3:
+    if len(duration) == 3:
         return (int(duration[0]) * 3600) + (int(duration[1]) * 60) + int(duration[2])
 
 
 def convert_to_hms(seconds):
     """Converts a given time in seconds to the format HHhMMmSSs.
 
     :param seconds: time in seconds
     :return: time in HHhMMmSSs format
     """
     minutes = seconds // 60
     hours = minutes // 60
 
-    return "%02dh%02dm%02ds" % (hours, minutes % 60, seconds % 60)
+    return f"{hours:02d}h{minutes % 60:02d}m{seconds % 60:02d}s"
 
 
 def create_lock(ini_path, vod_id):
     """Creates a lock file for a given VOD.
 
     :param ini_path: path to config directory
     :param vod_id: id of vod which lock file is created for
     :return: true if lock file creation fails
     """
     try:
-        with open(Path(ini_path, f'.lock.{vod_id}'), 'x') as _:
+        with open(Path(ini_path, f'.lock.{vod_id}'), 'x', encoding='utf8') as _:
             pass
+        return
 
     except FileExistsError:
         return True
 
 
 def remove_lock(config_dir, vod_id):
     """Removes a given lock file.
 
     :param config_dir: path to config directory
     :param vod_id: id of vod which lock file is created for
     :return: error if lock file removal fails
     """
     try:
         Path(config_dir, f'.lock.{vod_id}').unlink()
+        return
 
     except Exception as e:
         return e
 
 
 def time_since_date(timestamp):
     """Returns the time in seconds between a given datetime and now.
@@ -455,17 +460,46 @@
 
     return latest_version, release_notes
 
 
 # reference:
 #   https://stackoverflow.com/a/11887825
 def version_tuple(v):
+    """Convert
+
+    :param v:
+    :return:
+    """
     return tuple(map(int, (v.split("."))))
 
 
+def check_update_available(local_version, remote_version):
+    """Compares two software versions.
+
+    :param local_version: local version in use
+    :param remote_version: remote version to compare against
+    :return: True if remote version has a higher version number, otherwise False
+    """
+    # check if local version is 'special', as in a development build or release candidate
+    local_version_parts = local_version.split('.')
+    if len(local_version_parts) > 3:
+        log.warning(
+            'Currently using a development or release candidate build. These may be unfinished or contain serious '
+            'bugs. Report any issues you encounter to https://github.com/Brisppy/twitch-archiver/issues.')
+        # update is available if we are using a dev or release candidate build equal to or prior to
+        # the latest stable release
+        if version_tuple('.'.join(local_version_parts[:-1])) <= version_tuple(remote_version):
+            return True
+
+    elif version_tuple(local_version) < version_tuple(remote_version):
+        return True
+
+    return False
+
+
 def get_quality_index(desired_quality, available_qualities):
     """Finds the index of a user defined quality from a list of available stream qualities.
 
     :param desired_quality: desired quality to search for - best, worst or [resolution, framerate]
     :param available_qualities: list of available qualities as [[resolution, framerate], ...]
     :return: list index of desired quality if found
     """
@@ -505,21 +539,21 @@
         try:
             _r = requests.post(url="https://api.pushbullet.com/v2/pushes", headers=h, data=json.dumps(d),
                                timeout=10)
 
             if _r.status_code != 200:
                 if _r.json()['error']['code'] == 'pushbullet_pro_required':
                     log.error('Error sending push. Likely rate limited (500/month). '
-                              f'Error {_r.status_code}: {_r.text}')
+                              'Error %s: %s', _r.status_code, _r.text)
 
                 else:
-                    log.error(f'Error sending push. Error {_r.status_code}: {_r.text}')
+                    log.error('Error sending push. Error %s: %s', _r.status_code, _r.text)
 
         except Exception as e:
-            log.error(f'Error sending push. Error: {e}')
+            log.error('Error sending push. Error: %s', e)
 
 
 # reference:
 #   https://www.geeksforgeeks.org/compare-two-files-using-hashing-in-python/
 def get_hash(file):
     """Retrieves the hash for a given file.
 
@@ -582,21 +616,22 @@
     :return: environment variable value
     """
     val = os.getenv(name, default_val)
 
     if is_bool and isinstance(val, str):
         if val.upper() == "TRUE":
             return True
-        elif val.upper() == "FALSE":
+
+        if val.upper() == "FALSE":
             return False
-        else:
-            raise ValueError(f"Invalid boolean value (true or false) received for environment variable: {name}={val}")
-    else:
-        # return empty strings '' as None type
-        return val if val else None
+
+        raise ValueError(f"Invalid boolean value (true or false) received for environment variable: {name}={val}")
+
+    # return empty strings '' as None type
+    return val if val else None
 
 
 def format_vod_chapters(chapters):
     """Formats vod chapters retrieved from Twitch into an FFmpeg insertable format
 
     :param chapters: either a list of vod chapters or tuple containing (chapter_name, start, end)
     :return: chapters formatted as a string readable by ffmpeg
@@ -607,15 +642,15 @@
     TIMEBASE=1/1000
     START={start}
     END={end}
     title={title}
     
     """)
 
-    if type(chapters) == tuple:
+    if isinstance(chapters, tuple):
         formatted_chapters += chapter_base.format(
             start=chapters[1],
             end=chapters[2],
             title=chapters[0])
 
     else:
         # some chapters have no game attached and so the 'description' is used instead
@@ -648,15 +683,15 @@
         """Converts a given time in seconds to HHhMMmSSs.
 
         :param s: time in seconds
         :return: time formatted as HHhMMmSSs
         """
         m, s = divmod(s, 60)
         h, m = divmod(m, 60)
-        return '{:0>2}:{:0>2}:{:0>2}'.format(h, m, s)
+        return f'{h:0>2}:{m:0>2}:{s:0>2}'
 
     def print_progress(self, cur, total, last_frame=False):
         """Prints and updates a nice progress bar.
 
         :param cur: current progress out of total
         :param total: highest value of progress bar
         :param last_frame: boolean if last frame of progress bar
```

