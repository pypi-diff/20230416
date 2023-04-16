# Comparing `tmp/just_logger-0.2.0.tar.gz` & `tmp/just_logger-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "just_logger-0.2.0.tar", last modified: Sun Apr  9 02:06:55 2023, max compression
+gzip compressed data, was "just_logger-0.2.1.tar", last modified: Sun Apr 16 05:09:45 2023, max compression
```

## Comparing `just_logger-0.2.0.tar` & `just_logger-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 02:06:55.958595 just_logger-0.2.0/
--rw-rw-rw-   0        0        0     1064 2023-04-05 10:40:08.000000 just_logger-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      414 2023-04-09 02:06:55.958595 just_logger-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       89 2023-04-05 10:40:08.000000 just_logger-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 02:06:55.822213 just_logger-0.2.0/just_logger/
--rw-rw-rw-   0        0        0       47 2023-04-09 01:43:51.000000 just_logger-0.2.0/just_logger/__init__.py
--rw-rw-rw-   0        0        0     3113 2023-04-05 13:55:36.000000 just_logger-0.2.0/just_logger/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-09 02:06:55.942959 just_logger-0.2.0/just_logger.egg-info/
--rw-rw-rw-   0        0        0      414 2023-04-09 02:06:55.000000 just_logger-0.2.0/just_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-04-09 02:06:55.000000 just_logger-0.2.0/just_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 02:06:55.000000 just_logger-0.2.0/just_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-09 02:06:55.000000 just_logger-0.2.0/just_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 02:06:55.958595 just_logger-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      735 2023-04-09 02:06:26.000000 just_logger-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 05:09:45.153905 just_logger-0.2.1/
+-rw-rw-rw-   0        0        0     1064 2023-04-05 10:40:08.000000 just_logger-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1196 2023-04-16 05:09:45.151909 just_logger-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-04-16 05:04:20.000000 just_logger-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 05:09:44.843906 just_logger-0.2.1/just_logger/
+-rw-rw-rw-   0        0        0       47 2023-04-09 01:43:51.000000 just_logger-0.2.1/just_logger/__init__.py
+-rw-rw-rw-   0        0        0     3386 2023-04-14 16:06:33.000000 just_logger-0.2.1/just_logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-16 05:09:45.130909 just_logger-0.2.1/just_logger.egg-info/
+-rw-rw-rw-   0        0        0     1196 2023-04-16 05:09:44.000000 just_logger-0.2.1/just_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-04-16 05:09:44.000000 just_logger-0.2.1/just_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 05:09:44.000000 just_logger-0.2.1/just_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-16 05:09:44.000000 just_logger-0.2.1/just_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 05:09:45.154906 just_logger-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      776 2023-04-16 05:04:37.000000 just_logger-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 05:09:45.140907 just_logger-0.2.1/test/
+-rw-rw-rw-   0        0        0     3070 2023-04-16 04:56:17.000000 just_logger-0.2.1/test/test_just_logger.py
```

### Comparing `just_logger-0.2.0/LICENSE` & `just_logger-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `just_logger-0.2.0/just_logger/logger.py` & `just_logger-0.2.1/just_logger/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,25 +21,34 @@
     INFO = logging.INFO
     WARNING = logging.WARNING
     ERROR = logging.ERROR
     CRITICAL = logging.CRITICAL
 
 
 class Logger:
-    def __init__(self, logger_name: str, level: LogLevel=LogLevel.INFO) -> None:
+    def __init__(self, logger_name: str, log_dir: str=None, level: LogLevel=LogLevel.INFO, storage_days: int=7) -> None:
         self.__sptr = '/'
         if platform.system() == 'windows':
             self.__sptr = '\\'
         
-        self.__logdir = os.path.join(os.getcwd(), 'logs') 
+        self.__storage_days = storage_days
+        if log_dir is None:
+            self.__logdir = os.path.join(os.getcwd(), 'logs') 
+        else:
+            self.__logdir = log_dir
+
         self.__logger = logging.getLogger(logger_name)
         self.__logger.setLevel(level.value)
         fmt = '[%(asctime)s - %(levelname)s] %(message)s'
         datefmt = '%Y/%m/%d %H:%M:%S %p'
         self.__formatter = logging.Formatter(fmt=fmt, datefmt=datefmt)
+    
+
+    def __del__(self) -> None:
+        print('Dispose all the resource.')
 
 
     def add_stream_handler(self, level: LogLevel=LogLevel.DEBUG) -> None:
         if self.__contains_handler(logging.StreamHandler):
             return
 
         handler = logging.StreamHandler()
@@ -55,15 +64,15 @@
         if not os.path.exists(self.__logdir):
             os.makedirs(self.__logdir)
         logfile = f'{self.__logdir}{self.__sptr}{logfile}'
         handler = logging.handlers.TimedRotatingFileHandler(
             logfile, 
             when='MIDNIGHT', 
             interval=1, 
-            backupCount=7, 
+            backupCount=self.__storage_days, 
             atTime=datetime.time(0, 0, 0, 0), 
             encoding='utf-8')
         handler.setLevel(level.value)
         handler.setFormatter(self.__formatter)
         self.__logger.addHandler(handler)
```

