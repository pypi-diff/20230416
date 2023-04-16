# Comparing `tmp/teamplify-0.5.1.tar.gz` & `tmp/teamplify-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teamplify-0.5.1.tar", last modified: Mon Apr  3 20:57:18 2023, max compression
+gzip compressed data, was "teamplify-0.7.0.tar", last modified: Sun Apr 16 11:50:21 2023, max compression
```

## Comparing `teamplify-0.5.1.tar` & `teamplify-0.7.0.tar`

### file list

```diff
@@ -1,31 +1,29 @@
-drwxr-xr-x   0 oleg       (501) staff       (20)        0 2023-04-03 20:57:18.039332 teamplify-0.5.1/
--rw-r--r--   0 oleg       (501) staff       (20)     1066 2023-01-12 16:59:45.000000 teamplify-0.5.1/LICENSE
--rw-r--r--   0 oleg       (501) staff       (20)      272 2023-03-23 13:48:35.000000 teamplify-0.5.1/MANIFEST.in
--rw-r--r--   0 oleg       (501) staff       (20)    23510 2023-04-03 20:57:18.039398 teamplify-0.5.1/PKG-INFO
--rw-r--r--   0 oleg       (501) staff       (20)    23187 2023-04-03 07:16:46.000000 teamplify-0.5.1/README.md
--rw-r--r--   0 oleg       (501) staff       (20)       48 2023-01-12 16:59:45.000000 teamplify-0.5.1/requirements-tests.txt
--rw-r--r--   0 oleg       (501) staff       (20)       85 2023-01-12 16:59:45.000000 teamplify-0.5.1/requirements.txt
--rw-r--r--   0 oleg       (501) staff       (20)      251 2023-04-03 20:57:18.039604 teamplify-0.5.1/setup.cfg
--rw-r--r--   0 oleg       (501) staff       (20)     1255 2023-03-23 16:27:50.000000 teamplify-0.5.1/setup.py
-drwxr-xr-x   0 oleg       (501) staff       (20)        0 2023-04-03 20:57:18.037040 teamplify-0.5.1/teamplify.egg-info/
--rw-r--r--   0 oleg       (501) staff       (20)    23510 2023-04-03 20:57:18.000000 teamplify-0.5.1/teamplify.egg-info/PKG-INFO
--rw-r--r--   0 oleg       (501) staff       (20)      644 2023-04-03 20:57:18.000000 teamplify-0.5.1/teamplify.egg-info/SOURCES.txt
--rw-r--r--   0 oleg       (501) staff       (20)        1 2023-04-03 20:57:18.000000 teamplify-0.5.1/teamplify.egg-info/dependency_links.txt
--rw-r--r--   0 oleg       (501) staff       (20)       56 2023-04-03 20:57:18.000000 teamplify-0.5.1/teamplify.egg-info/entry_points.txt
--rw-r--r--   0 oleg       (501) staff       (20)      142 2023-04-03 20:57:18.000000 teamplify-0.5.1/teamplify.egg-info/requires.txt
--rw-r--r--   0 oleg       (501) staff       (20)       17 2023-04-03 20:57:18.000000 teamplify-0.5.1/teamplify.egg-info/top_level.txt
-drwxr-xr-x   0 oleg       (501) staff       (20)        0 2023-04-03 20:57:18.038787 teamplify-0.5.1/teamplify_runner/
--rw-r--r--   0 oleg       (501) staff       (20)       22 2023-04-03 20:33:28.000000 teamplify-0.5.1/teamplify_runner/__init__.py
-drwxr-xr-x   0 oleg       (501) staff       (20)        0 2023-04-03 20:57:18.038990 teamplify-0.5.1/teamplify_runner/backup/
--rw-r--r--   0 oleg       (501) staff       (20)       51 2023-01-12 16:59:45.000000 teamplify-0.5.1/teamplify_runner/backup/readme.txt
--rwxr-xr-x   0 oleg       (501) staff       (20)    12589 2023-04-03 20:32:34.000000 teamplify-0.5.1/teamplify_runner/cli.py
--rw-r--r--   0 oleg       (501) staff       (20)    13723 2023-04-03 20:39:58.000000 teamplify-0.5.1/teamplify_runner/configurator.py
--rw-r--r--   0 oleg       (501) staff       (20)     5304 2023-04-03 20:32:34.000000 teamplify-0.5.1/teamplify_runner/docker-compose.yml
--rw-r--r--   0 oleg       (501) staff       (20)      270 2023-01-12 16:59:45.000000 teamplify-0.5.1/teamplify_runner/mysql.cnf
--rw-r--r--   0 oleg       (501) staff       (20)       66 2023-01-12 16:59:45.000000 teamplify-0.5.1/teamplify_runner/postfix.cf
--rw-r--r--   0 oleg       (501) staff       (20)       22 2023-01-12 16:59:45.000000 teamplify-0.5.1/teamplify_runner/redis.conf
--rw-r--r--   0 oleg       (501) staff       (20)     1748 2023-01-12 16:59:45.000000 teamplify-0.5.1/teamplify_runner/utils.py
--rw-r--r--   0 oleg       (501) staff       (20)      766 2023-04-03 19:37:08.000000 teamplify-0.5.1/teamplify_runner/uwsgi_params.conf
--rw-r--r--   0 oleg       (501) staff       (20)      512 2023-04-03 19:39:47.000000 teamplify-0.5.1/teamplify_runner/vhost.conf
-drwxr-xr-x   0 oleg       (501) staff       (20)        0 2023-04-03 20:57:18.039123 teamplify-0.5.1/tests/
--rw-r--r--   0 oleg       (501) staff       (20)     2146 2023-03-23 16:27:25.000000 teamplify-0.5.1/tests/test_configurator.py
+drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-16 11:50:21.100014 teamplify-0.7.0/
+-rw-r--r--   0 ipeterov   (501) staff       (20)     1066 2023-04-12 15:29:52.000000 teamplify-0.7.0/LICENSE
+-rw-r--r--   0 ipeterov   (501) staff       (20)      272 2023-04-12 15:29:52.000000 teamplify-0.7.0/MANIFEST.in
+-rw-r--r--   0 ipeterov   (501) staff       (20)    23510 2023-04-16 11:50:21.100110 teamplify-0.7.0/PKG-INFO
+-rw-r--r--   0 ipeterov   (501) staff       (20)    23187 2023-04-12 15:29:52.000000 teamplify-0.7.0/README.md
+-rw-r--r--   0 ipeterov   (501) staff       (20)       48 2023-04-12 15:29:52.000000 teamplify-0.7.0/requirements-tests.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)      102 2023-04-12 21:17:51.000000 teamplify-0.7.0/requirements.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)      251 2023-04-16 11:50:21.100386 teamplify-0.7.0/setup.cfg
+-rw-r--r--   0 ipeterov   (501) staff       (20)     1255 2023-04-12 15:29:52.000000 teamplify-0.7.0/setup.py
+drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-16 11:50:21.097565 teamplify-0.7.0/teamplify.egg-info/
+-rw-r--r--   0 ipeterov   (501) staff       (20)    23510 2023-04-16 11:50:21.000000 teamplify-0.7.0/teamplify.egg-info/PKG-INFO
+-rw-r--r--   0 ipeterov   (501) staff       (20)      617 2023-04-16 11:50:21.000000 teamplify-0.7.0/teamplify.egg-info/SOURCES.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)        1 2023-04-16 11:50:21.000000 teamplify-0.7.0/teamplify.egg-info/dependency_links.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)       56 2023-04-16 11:50:21.000000 teamplify-0.7.0/teamplify.egg-info/entry_points.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)      159 2023-04-16 11:50:21.000000 teamplify-0.7.0/teamplify.egg-info/requires.txt
+-rw-r--r--   0 ipeterov   (501) staff       (20)       17 2023-04-16 11:50:21.000000 teamplify-0.7.0/teamplify.egg-info/top_level.txt
+drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-16 11:50:21.099724 teamplify-0.7.0/teamplify_runner/
+-rw-r--r--   0 ipeterov   (501) staff       (20)       22 2023-04-16 11:49:30.000000 teamplify-0.7.0/teamplify_runner/__init__.py
+drwxr-xr-x   0 ipeterov   (501) staff       (20)        0 2023-04-16 11:50:21.099876 teamplify-0.7.0/teamplify_runner/backup/
+-rw-r--r--   0 ipeterov   (501) staff       (20)       51 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/backup/readme.txt
+-rwxr-xr-x   0 ipeterov   (501) staff       (20)    13690 2023-04-16 11:43:21.000000 teamplify-0.7.0/teamplify_runner/cli.py
+-rw-r--r--   0 ipeterov   (501) staff       (20)    13723 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/configurator.py
+-rw-r--r--   0 ipeterov   (501) staff       (20)     5304 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/docker-compose.yml
+-rw-r--r--   0 ipeterov   (501) staff       (20)      270 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/mysql.cnf
+-rw-r--r--   0 ipeterov   (501) staff       (20)       66 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/postfix.cf
+-rw-r--r--   0 ipeterov   (501) staff       (20)       22 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/redis.conf
+-rw-r--r--   0 ipeterov   (501) staff       (20)     1748 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/utils.py
+-rw-r--r--   0 ipeterov   (501) staff       (20)      766 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/uwsgi_params.conf
+-rw-r--r--   0 ipeterov   (501) staff       (20)      512 2023-04-12 15:29:52.000000 teamplify-0.7.0/teamplify_runner/vhost.conf
```

### Comparing `teamplify-0.5.1/LICENSE` & `teamplify-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `teamplify-0.5.1/PKG-INFO` & `teamplify-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teamplify
-Version: 0.5.1
+Version: 0.7.0
 Summary: Teamplify on-premise runner
 Home-page: https://github.com/teamplify/teamplify-runner/
 Author: Teamplify
 Author-email: support@teamplify.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `teamplify-0.5.1/README.md` & `teamplify-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `teamplify-0.5.1/setup.py` & `teamplify-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `teamplify-0.5.1/teamplify.egg-info/PKG-INFO` & `teamplify-0.7.0/teamplify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teamplify
-Version: 0.5.1
+Version: 0.7.0
 Summary: Teamplify on-premise runner
 Home-page: https://github.com/teamplify/teamplify-runner/
 Author: Teamplify
 Author-email: support@teamplify.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `teamplify-0.5.1/teamplify.egg-info/SOURCES.txt` & `teamplify-0.7.0/teamplify.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,9 +17,8 @@
 teamplify_runner/docker-compose.yml
 teamplify_runner/mysql.cnf
 teamplify_runner/postfix.cf
 teamplify_runner/redis.conf
 teamplify_runner/utils.py
 teamplify_runner/uwsgi_params.conf
 teamplify_runner/vhost.conf
-teamplify_runner/backup/readme.txt
-tests/test_configurator.py
+teamplify_runner/backup/readme.txt
```

### Comparing `teamplify-0.5.1/teamplify_runner/cli.py` & `teamplify-0.7.0/teamplify_runner/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 import os
+import time
 from datetime import datetime
 
 import click
+import requests
 
 from teamplify_runner import __version__
 from teamplify_runner.configurator import BASE_DIR, ConfigurationError, \
     Configurator
 from teamplify_runner.utils import cd, run
 
 
@@ -24,14 +26,54 @@
     port = env['WEB_PORT']
     root_url = 'http://' + env['WEB_HOST']
     if port != '80':
         root_url += ':' + port
     return root_url
 
 
+def _wait_for_teamplify_start(url, max_minutes=5, check_interval_seconds=5):
+    click.echo(
+        '\nWaiting for Teamplify to start at %s,'
+        ' checking every %s seconds...' % (url, check_interval_seconds),
+        nl=False,
+    )
+
+    start_time = time.time()
+    while time.time() < start_time + max_minutes * 60:
+        response = requests.get(url).text
+
+        if 'window.BUILD_NUMBER' in response:
+            click.echo('\nTeamplify successfully started!')
+            return
+        elif any(
+            marker in response
+            for marker in (
+                'Welcome to nginx!',
+                'Teamplify is starting...',
+            )
+        ):
+            time.sleep(check_interval_seconds)
+            click.echo('.', nl=False)
+            continue
+        else:
+            raise RuntimeError(
+                '\n\nUnexpected response from Teamplify: %s\n\n'
+                'Please check the Troubleshooting guide:\n -> '
+                'https://github.com/teamplify/teamplify-runner/#troubleshooting'
+                % response,
+            )
+    else:
+        raise RuntimeError(
+            "\n\nTeamplify didn't start in %s minutes. "
+            'Please check the Troubleshooting guide:\n'
+            ' -> https://github.com/teamplify/teamplify-runner/#troubleshooting'
+            % max_minutes,
+        )
+
+
 def _start(env):
     click.echo('Starting services...')
     run('mkdir -p %s' % env['DB_BACKUP_MOUNT'])
     with cd(BASE_DIR):
         run(
             'docker-compose up '
             '--detach '
@@ -40,39 +82,37 @@
             '--scale worker_fat={worker_fat_count}'.format(
                 worker_slim_count=env['WORKER_SLIM_COUNT'],
                 worker_fat_count=env['WORKER_FAT_COUNT'],
             ),
             capture_output=False,
             env=env,
         )
-    root_url = _root_url(env)
-    click.echo(
-        '\nDone. It may take a few moments for the app to come online at:\n'
-        ' -> %s\n\n'
-        "If it isn't available immediately, please check again after "
-        'a minute or two. If you experience any problems with the '
-        'installation, please check the Troubleshooting guide:\n'
-        ' -> https://github.com/teamplify/teamplify-runner/#troubleshooting'
-        '' % root_url,
-    )
+
     if env['WEB_HOST'].lower() == 'localhost':
         click.echo(
             click.style('\nWARNING:', fg='yellow') +
             " you're running Teamplify on localhost. This is "
             'probably OK if you only need to run a demo on your local machine. '
             'However, in this mode it will not be available to anyone from the '
             "network. If you'd like to make it available on the network, you "
             'need to provide a publicly visible domain name that points to '
             'this server.',
         )
 
+    root_url = _root_url(env)
+    try:
+        _wait_for_teamplify_start(root_url)
+    except RuntimeError as e:
+        click.echo(click.style(str(e), fg='red'))
+        exit(1)
+
 
 def _create_admin(env, email, full_name):
     click.echo('Creating admin...')
-    cmd = 'docker exec -it teamplify_app ' \
+    cmd = 'docker exec teamplify_app ' \
           '/code/manage.py createadmin --email %s' % email
     if full_name:
         cmd += ' --full-name "%s"' % full_name
     run(cmd, capture_output=False, env=env)
 
 
 def _stop(env):
```

### Comparing `teamplify-0.5.1/teamplify_runner/configurator.py` & `teamplify-0.7.0/teamplify_runner/configurator.py`

 * *Files identical despite different names*

### Comparing `teamplify-0.5.1/teamplify_runner/docker-compose.yml` & `teamplify-0.7.0/teamplify_runner/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `teamplify-0.5.1/teamplify_runner/utils.py` & `teamplify-0.7.0/teamplify_runner/utils.py`

 * *Files identical despite different names*

### Comparing `teamplify-0.5.1/teamplify_runner/uwsgi_params.conf` & `teamplify-0.7.0/teamplify_runner/uwsgi_params.conf`

 * *Files identical despite different names*

### Comparing `teamplify-0.5.1/teamplify_runner/vhost.conf` & `teamplify-0.7.0/teamplify_runner/vhost.conf`

 * *Files identical despite different names*

