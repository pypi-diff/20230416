# Comparing `tmp/fluke-api-0.2.0.tar.gz` & `tmp/fluke-api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluke-api-0.2.0.tar", last modified: Sat Mar 25 12:24:37 2023, max compression
+gzip compressed data, was "fluke-api-0.3.0.tar", last modified: Sun Apr 16 15:36:52 2023, max compression
```

## Comparing `fluke-api-0.2.0.tar` & `fluke-api-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:24:37.843687 fluke-api-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-25 12:24:15.000000 fluke-api-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-03-25 12:24:37.843687 fluke-api-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-03-25 12:24:15.000000 fluke-api-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:24:37.843687 fluke-api-0.2.0/fluke/
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-03-25 12:24:15.000000 fluke-api-0.2.0/fluke/_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-25 12:24:15.000000 fluke-api-0.2.0/fluke/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-03-25 12:24:15.000000 fluke-api-0.2.0/fluke/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    45116 2023-03-25 12:24:15.000000 fluke-api-0.2.0/fluke/_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-25 12:24:15.000000 fluke-api-0.2.0/fluke/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-03-25 12:24:15.000000 fluke-api-0.2.0/fluke/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    74101 2023-03-25 12:24:15.000000 fluke-api-0.2.0/fluke/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:24:37.843687 fluke-api-0.2.0/fluke_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-03-25 12:24:37.000000 fluke-api-0.2.0/fluke_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-25 12:24:37.000000 fluke-api-0.2.0/fluke_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 12:24:37.000000 fluke-api-0.2.0/fluke_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-25 12:24:37.000000 fluke-api-0.2.0/fluke_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-25 12:24:37.000000 fluke-api-0.2.0/fluke_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-25 12:24:15.000000 fluke-api-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 12:24:37.843687 fluke-api-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 12:24:37.843687 fluke-api-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-03-25 12:24:15.000000 fluke-api-0.2.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)   136621 2023-03-25 12:24:15.000000 fluke-api-0.2.0/tests/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:36:52.335945 fluke-api-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 15:36:38.000000 fluke-api-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-16 15:36:52.335945 fluke-api-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-16 15:36:38.000000 fluke-api-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:36:52.335945 fluke-api-0.3.0/fluke/
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-04-16 15:36:38.000000 fluke-api-0.3.0/fluke/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-16 15:36:38.000000 fluke-api-0.3.0/fluke/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44133 2023-04-16 15:36:38.000000 fluke-api-0.3.0/fluke/_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-16 15:36:38.000000 fluke-api-0.3.0/fluke/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24682 2023-04-16 15:36:38.000000 fluke-api-0.3.0/fluke/_iohandlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-16 15:36:38.000000 fluke-api-0.3.0/fluke/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80956 2023-04-16 15:36:38.000000 fluke-api-0.3.0/fluke/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:36:52.335945 fluke-api-0.3.0/fluke_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-16 15:36:52.000000 fluke-api-0.3.0/fluke_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-16 15:36:52.000000 fluke-api-0.3.0/fluke_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:36:52.000000 fluke-api-0.3.0/fluke_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-16 15:36:52.000000 fluke-api-0.3.0/fluke_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 15:36:52.000000 fluke-api-0.3.0/fluke_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-16 15:36:38.000000 fluke-api-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 15:36:52.335945 fluke-api-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:36:52.335945 fluke-api-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-16 15:36:38.000000 fluke-api-0.3.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164383 2023-04-16 15:36:38.000000 fluke-api-0.3.0/tests/test_storage.py
```

### Comparing `fluke-api-0.2.0/LICENSE` & `fluke-api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fluke-api-0.2.0/PKG-INFO` & `fluke-api-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluke-api
-Version: 0.2.0
+Version: 0.3.0
 Summary: Move your data around
 Author: Manos Stoumpos
 Author-email: manosstoumpos@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/manoss96/fluke
 Project-URL: Bug Tracker, https://github.com/manoss96/fluke/issues
 Project-URL: Documentation, https://fluke.rtfd.io
```

### Comparing `fluke-api-0.2.0/README.md` & `fluke-api-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fluke-api-0.2.0/fluke/_exceptions.py` & `fluke-api-0.3.0/fluke/_exceptions.py`

 * *Files identical despite different names*

### Comparing `fluke-api-0.2.0/fluke/_handlers.py` & `fluke-api-0.3.0/fluke/_handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 import os as _os
-import io as _io
 from abc import ABC as _ABC
 from abc import abstractmethod as _absmethod
-from shutil import copyfileobj as _copyfileobj
-from typing import Optional as _Optional
 from typing import Iterator as _Iterator
+from typing import Optional as _Optional
 
 
 import boto3 as _boto3
 import paramiko as _prmk
 from azure.identity import ClientSecretCredential as _CSC
 from azure.storage.blob import ContainerClient as _ContainerClient
 
 
 from .auth import AWSAuth as _AWSAuth
 from .auth import AzureAuth as _AzureAuth
 from .auth import RemoteAuth as _RemoteAuth
 from ._cache import CacheManager as _CacheManager
+from ._iohandlers import _FileReader
+from ._iohandlers import _FileWriter
+from ._iohandlers import LocalFileReader as _LocalFileReader
+from ._iohandlers import LocalFileWriter as _LocalFileWriter
+from ._iohandlers import RemoteFileReader as _RemoteFileReader
+from ._iohandlers import RemoteFileWriter as _RemoteFileWriter
+from ._iohandlers import AWSS3FileReader as _AWSS3FileReader
+from ._iohandlers import AWSS3FileWriter as _AWSS3FileWriter
+from ._iohandlers import AzureBlobReader as _AzureBlobReader
+from ._iohandlers import AzureBlobWriter as _AzureBlobWriter
 from ._exceptions import UnknownKeyTypeError as _UKTE
 from ._helper import join_paths as _join_paths
 from ._helper import infer_separator as _infer_sep
 from ._helper import relativize_path as _relativize
 
 
 class ClientHandler(_ABC):
     '''
     An abstract class which serves as the \
-    base class for all client-like classes.
+    base class for all client-handler-like classes.
 
     :param bool cache: Indicates whether it is allowed for \
         any fetched data to be cached for faster subsequent \
         access. Defaults to ``False``.
     '''
 
+
     def __init__(self, cache: bool):
         '''
         An abstract class which serves as the \
-        base class for all client-like classes.
+        base class for all client-handler-like classes.
 
         :param bool cache: Indicates whether it is allowed for \
             any fetched data to be cached for faster subsequent \
             access. Defaults to ``False``.
         '''
+
         self.__cache_manager = _CacheManager() if cache else None
 
 
     def is_cacheable(self) -> bool:
         '''
         Returns a value indicating whether this \
         handler instance has been defined so that \
@@ -57,22 +67,22 @@
     def purge(self) -> None:
         '''
         If cacheable, then purges the handler's cache, \
         else does nothing.
         '''
         if self.is_cacheable():
             self.__cache_manager.purge()
-            self.__cache_manager = _CacheManager()
 
 
     def get_file_size(self, file_path: str) -> int:
         '''
         Returns the size of a file in bytes.
         
-        :param str file_path: The path of the file in question.
+        :param str file_path: The absolute path of the \
+            file in question.
 
         :note: This method will go on to fetch the requested value \
             from a remote resource only when one of the following is \
             true:
             - Caching has not been enabled.
             - Caching has not been enabled, though \
               the requested value has not been cached.
@@ -91,28 +101,31 @@
             return self._get_file_size_impl(file_path)
         
 
     def get_file_metadata(self, file_path: str) -> dict[str, str]:
         '''
         Returns a dictionary containing the metadata of a file.
         
-        :param str file_path: The path of the file in question.
+        :param str file_path: The absolute path of the file \
+            in question.
         
         :note: This method will go on to fetch the requested value \
             from a remote resource only when one of the following is \
             true:
             - Caching has not been enabled.
             - Caching has not been enabled, though \
               the requested value has not been cached.
 
             In the second case, the value will be cached \
             after it has been retrieved.
         '''
         if self.is_cacheable():
-            if (metadata := self.__cache_manager.get_metadata(file_path=file_path)) is not None:
+            if (metadata := self.__cache_manager.get_metadata(
+                file_path=file_path)
+            ) is not None:
                 return metadata
             else:
                 metadata = self._get_file_metadata_impl(file_path)
                 self.__cache_manager.cache_metadata(file_path, metadata)
                 return metadata
         else:
             return self._get_file_metadata_impl(file_path)
@@ -122,16 +135,16 @@
         self,
         dir_path: str,
         recursively: bool,
         include_dirs: bool,
         show_abs_path: bool
     ) -> _Iterator[str]:
         '''
-        Returns an iterator capable of going through the paths \
-        of the dictionary's contents as strings.
+        Returns an iterator capable of going through \
+        the directory's contents as their paths.
 
         :param str dir_path: The absolute path of the directory \
             whose contents are to be iterated.
         :param bool recursively: Indicates whether the directory \
             is to be traversed recursively or not. If set to  ``False``, \
             then only those files that reside directly within the \
             directory are to be considered. If set to ``True``, \
@@ -155,14 +168,15 @@
                 child=p,
                 sep=_infer_sep(dir_path)
             ), iterator)
 
         if self.is_cacheable():
             # Grab content iterator from cache if it exists.
             if (iterator := self.__cache_manager.get_content_iterator(
+                dir_path=dir_path,
                 recursively=recursively,
                 include_dirs=include_dirs)
             ) is not None:
                 return iterator if show_abs_path \
                     else relativize_iter(iterator)
             # Else...
             else:
@@ -171,19 +185,21 @@
                 #       contents are cached via their absolute paths.
                 iterator = self._traverse_dir_impl(
                     dir_path=dir_path,
                     recursively=recursively,
                     show_abs_path=True)
                 # Cache all contents.
                 self.__cache_manager.cache_contents(
+                    dir_path=dir_path,
                     iterator=iterator,
                     recursively=recursively,
                     is_file=self.is_file)
                 # Reset iterator by grabbing it from cache.
                 iterator = self.__cache_manager.get_content_iterator(
+                    dir_path=dir_path,
                     recursively=recursively,
                     include_dirs=include_dirs)
                 if show_abs_path:
                     return iterator
                 else:
                     return relativize_iter(iterator)
         else:
@@ -260,68 +276,59 @@
         :param str path: The path of the directory \
             that is to be created.
         '''
         pass
 
 
     @_absmethod
-    def read(
-        self,
-        file_path: str,
-        buffer: _io.BytesIO,
-        include_metadata: bool
-    ) -> _Optional[dict[str, str]]:
-        '''
-        Reads the bytes of a file into the provided buffer. \
-        Returns either ``None`` or a dictionary containing \
-        file metadata, depending on the value of parameter \
-        ``include_metadata``.
+    def get_reader(self, file_path: str) -> '_FileReader':
+        '''
+        Returns a ``_FileReader`` class instance \
+        used for reading from a file.
 
-        :param str file_path: The absolute path of the \
-            file in question.
-        :param BytesIO buffer: A buffer to download the \
-            file into.
-        :param bool include_metadata: Indicates whether \
-            to download any existing file metadata as well.
+        :param str file_path: The absolute path of \
+            the file in question.
         '''
         pass
 
 
     @_absmethod
-    def write(
+    def get_writer(
         self,
         file_path: str,
-        buffer: _io.BytesIO,
-        metadata: _Optional[dict[str, str]]
-    ) -> None:
-        '''
-        Writes the bytes contained within the provided \
-        buffer into the specified path.
-
-        :param str file_path: The absolute path of the \
-            file in question.
-        :param BytesIO buffer: A buffer containing the \
-            file's bytes.
-        :param dict[str, str] | None: If not ``None``, \
-            then assigns the provided metadata to the file \
-            during the upload.
+        metadata: _Optional[dict[str, str]],
+        in_chunks: bool
+    ) -> '_FileWriter':
+        '''
+        Returns an ``_FileWriter`` class instance \
+        used for writing to a file.
+
+        :param str file_path: The absolute path of \
+            the file in question.
+        :param dict[str, str] | None metadata: A \
+            dictionary containing the metadata that \
+            are to be assigned to the file in question. \
+            If ``None``, then no metadata are assigned.
+        :param bool in_chunks: Indicates whether to \
+            write the file in distinct chunks or \
+            all at once.
         '''
         pass
 
 
     @_absmethod
     def _traverse_dir_impl(
         self,
         dir_path: str,
         recursively: bool,
         show_abs_path: bool
     ) -> _Iterator[str]:
         '''
-        Returns an iterator capable of going through the paths \
-        of the dictionary's contents as strings.
+        Returns an iterator capable of going through \
+        the directory's contents as their paths.
 
         :param str dir_path: The absolute path of the directory \
             whose contents are to be iterated.
         :param bool recursively: Indicates whether the directory \
             is to be traversed recursively or not. If set to  ``False``, \
             then only those files that reside directly within the \
             directory are to be considered. If set to ``True``, \
@@ -361,14 +368,17 @@
         pass
 
 
 class FileSystemHandler(ClientHandler):
     '''
     A class used in handling all local file \
     system operations.
+
+    :param str file_path: The absolute path of \
+        the file in question.
     '''
 
     def __init__(self):
         '''
         A class used in handling all local file \
         system operations.
         '''
@@ -424,62 +434,52 @@
         '''
         Creates a directory into the provided path.
 
         :param str path: The path of the directory \
             that is to be created.
         '''
         _os.makedirs(path, exist_ok=True)
-    
 
-    def read(
-        self,
-        file_path: str,
-        buffer: _io.BytesIO,
-        include_metadata: bool
-    ) -> _Optional[dict[str, str]]:
-        '''
-        Reads the bytes of a file into the provided buffer. \
-        Returns either ``None`` or a dictionary containing \
-        file metadata, depending on the value of parameter \
-        ``include_metadata``.
 
-        :param str file_path: The absolute path of the \
-            file in question.
-        :param BytesIO buffer: A buffer to download the \
-            file into.
-        :param bool include_metadata: Indicates whether \
-            to download any existing file metadata as well.
+    def get_reader(self, file_path: str) -> _LocalFileReader:
         '''
-        with open(file=file_path, mode='rb') as file:
-            _copyfileobj(fsrc=file, fdst=buffer)
+        Returns a ``LocalFileReader`` class instance \
+        used for reading from a file which resides \
+        within the local file system.
+
+        :param str file_path: The absolute path of \
+            the file in question.
+        '''
+        return _LocalFileReader(
+            file_path=file_path,
+            file_size=self.get_file_size(file_path))
 
 
-    def write(
+    def get_writer(
         self,
         file_path: str,
-        buffer: _io.BytesIO,
-        metadata: _Optional[dict[str, str]]
-    ) -> None:
+        metadata: _Optional[dict[str, str]],
+        in_chunks: bool
+    ) -> _LocalFileWriter:
+        '''
+        Returns an ``LocalFileWriter`` class instance \
+        used for writing to a file which resides within \
+        the local file system.
+
+        :param str file_path: The absolute path of \
+            the file in question.
+        :param dict[str, str] | None metadata: A \
+            dictionary containing the metadata that \
+            are to be assigned to the file in question. \
+            If ``None``, then no metadata are assigned.
+        :param bool in_chunks: Indicates whether to \
+            write the file in distinct chunks or \
+            all at once.
         '''
-        Writes the bytes contained within the provided \
-        buffer into the specified path.
-
-        :param str file_path: The absolute path of the \
-            file in question.
-        :param BytesIO buffer: A buffer containing the \
-            file's bytes.
-        :param dict[str, str] | None: If not ``None``, \
-            then assigns the provided metadata to the file \
-            during the upload.
-        '''
-        # Create any necessary directories.
-        self.mkdir(_os.path.dirname(file_path))
-        # Write file.
-        with open(file=file_path, mode='wb') as file:
-            _copyfileobj(fsrc=buffer, fdst=file)
+        return _LocalFileWriter(file_path=file_path)
     
 
     def _get_file_size_impl(self, file_path) -> int:
         '''
         Fetches and returns the size of a file in bytes.
 
         :param str file_path: The path of the file in question.
@@ -500,16 +500,16 @@
     def _traverse_dir_impl(
         self,
         dir_path: str,
         recursively: bool,
         show_abs_path: bool
     ) -> _Iterator[str]:
         '''
-        Returns an iterator capable of going through the paths \
-        of the dictionary's contents as strings.
+        Returns an iterator capable of going through \
+        the directory's contents as their paths.
 
         :param str dir_path: The absolute path of the directory \
             whose contents are to be iterated.
         :param bool recursively: Indicates whether the directory \
             is to be traversed recursively or not. If set to  ``False``, \
             then only those files that reside directly within the \
             directory are to be considered. If set to ``True``, \
@@ -551,15 +551,15 @@
     connections to a remote server.
 
     :param RemoteAuth auth: A ``RemoteAuth`` instance used \
         for authenticating with a remote machine.
     :param bool cache: Indicates whether it is allowed for \
         any fetched data to be cached for faster subsequent \
         access. Defaults to ``False``.
-    '''
+    '''        
 
     def __init__(self, auth: _RemoteAuth, cache: bool):
         '''
         A class used in handling the SSH and SFTP \
         connections to a remote server.
 
         :param RemoteAuth auth: A ``RemoteAuth`` instance used \
@@ -596,14 +596,16 @@
 
         credentials = self.__auth.get_credentials()
 
         public_key = credentials.pop('public_key')
         key_type = credentials.pop('key_type')
         verify_host = credentials.pop('verify_host')
 
+        print(f"\nEstablishing connection to '{credentials['hostname']}'...")
+
         # Load all known hosts.
         ssh.load_system_host_keys()
 
         # If 'verify_host' has been set to 'False',
         # then automatically add any host to the list of
         # known hosts.
         if not verify_host:
@@ -642,14 +644,15 @@
         try:
             ssh.connect(**credentials)
         except _prmk.SSHException as e:
             raise e
 
         self.__ssh = ssh
         self.__sftp = ssh.open_sftp()
+        print("Connection established!")
 
 
     def close_connections(self):
         '''
         Closes the SSH/SFTP connection to \
         the remote server.
         '''
@@ -682,92 +685,63 @@
 
         :param str file_path: The absolute path of the \
             file in question.
         '''
         from stat import S_ISDIR as _is_dir
         return not _is_dir(self.__sftp.stat(path=file_path).st_mode)
     
-
+    
     def mkdir(self, path: str) -> None:
         '''
         Creates a directory into the provided path.
 
         :param str path: The path of the directory \
             that is to be created.
         '''
         self.__sftp.mkdir(path=path)
-    
 
-    def read(
-        self,
-        file_path: str,
-        buffer: _io.BytesIO,
-        include_metadata: bool
-    ) -> _Optional[dict[str, str]]:
-        '''
-        Reads the bytes of a file into the provided buffer. \
-        Returns either ``None`` or a dictionary containing \
-        file metadata, depending on the value of parameter \
-        ``include_metadata``.
 
-        :param str file_path: The absolute path of the \
-            file in question.
-        :param BytesIO buffer: A buffer to download the \
-            file into.
-        :param bool include_metadata: Indicates whether \
-            to download any existing file metadata as well.
+    def get_reader(self, file_path: str) -> _RemoteFileReader:
         '''
-        self.__sftp.getfo(remotepath=file_path, fl=buffer)
+        Returns a ``RemoteFileReader`` class instance \
+        used for reading from a file which resides \
+        within a remote file system.
 
+        :param str file_path: The absolute path of \
+            the file in question.
+        '''
+        return _RemoteFileReader(
+            file_path=file_path,
+            file_size=self.get_file_size(file_path),
+            sftp=self.__sftp)
 
-    def write(
+
+    def get_writer(
         self,
         file_path: str,
-        buffer: _io.BytesIO,
-        metadata: _Optional[dict[str, str]]
-    ) -> None:
+        metadata: _Optional[dict[str, str]],
+        in_chunks: bool
+    ) -> _RemoteFileWriter:
+        '''
+        Returns a ``RemoteFileWriter`` class instance \
+        used for writing to a file which resides within \
+        a remote file system.
+
+        :param str file_path: The absolute path of \
+            the file in question.
+        :param dict[str, str] | None metadata: A \
+            dictionary containing the metadata that \
+            are to be assigned to the file in question. \
+            If ``None``, then no metadata are assigned.
+        :param bool in_chunks: Indicates whether to \
+            write the file in distinct chunks or \
+            all at once.
         '''
-        Writes the bytes contained within the provided \
-        buffer into the specified path.
-
-        :param str file_path: The absolute path of the \
-            file in question.
-        :param BytesIO buffer: A buffer containing the \
-            file's bytes.
-        :param dict[str, str] | None: If not ``None``, \
-            then assigns the provided metadata to the file \
-            during the upload.
-        '''
-
-        sep = _infer_sep(file_path)
-
-        def get_parent_dir(file_path: str) -> _Optional[str]:
-            '''
-            Returns the path to the parent directory \
-            of the provided file path. Returns ``None`` \
-            if said directory is the root directory.
-
-            :param str file_path: The path of the file \
-                in question.
-            '''
-            file_path = file_path.rstrip(sep)
-            if sep in file_path:
-                return f"{sep.join(file_path.split(sep)[:-1])}{sep}"
-            return None
-
-        # Create any directories necessary.
-        parent_dir, non_existing_dirs = file_path, []
-        while (parent_dir := get_parent_dir(parent_dir)) is not None:
-            if not self.path_exists(path=parent_dir):
-                non_existing_dirs.append(parent_dir)
-        for dir in reversed(non_existing_dirs):
-            self.mkdir(path=dir)
-
-        # Write file from buffer.
-        self.__sftp.putfo(fl=buffer, remotepath=file_path)
+        return _RemoteFileWriter(
+            file_path=file_path, sftp=self.__sftp)
 
 
     def _get_file_size_impl(self, file_path) -> int:
         '''
         Fetches and returns the size of a file in bytes.
 
         :param str file_path: The path of the file in question.
@@ -789,16 +763,16 @@
     def _traverse_dir_impl(
         self,
         dir_path: str,
         recursively: bool,
         show_abs_path: bool
     ) -> _Iterator[str]:
         '''
-        Returns an iterator capable of going through the paths \
-        of the dictionary's contents as strings.
+        Returns an iterator capable of going through \
+        the directory's contents as their paths.
 
         :param str dir_path: The absolute path of the directory \
             whose contents are to be iterated.
         :param bool recursively: Indicates whether the directory \
             is to be traversed recursively or not. If set to  ``False``, \
             then only those files that reside directly within the \
             directory are to be considered. If set to ``True``, \
@@ -914,18 +888,20 @@
         '''
         Opens an HTTP connection to the Amazon S3 bucket.
         '''
 
         if self.__bucket is not None:
             return
 
+        print(f"\nEstablishing connection to '{self.__bucket_name}' Amazon S3 bucket...")
         self.__bucket = _boto3.resource(
             service_name='s3',
             **self.__auth.get_credentials()
         ).Bucket(self.__bucket_name)
+        print("Connection established.")
 
 
     def close_connections(self):
         '''
         Closes the HTTP connection to the Amazon S3 bucket.
         '''
         if self.__bucket is not None:
@@ -969,76 +945,68 @@
             path relative to the parent directory.
         '''
         for _ in self.__bucket.objects.filter(Prefix=path):
             return True
         return False
         
     
-
     def mkdir(self, path: str) -> None:
         '''
         Creates a directory into the provided path.
 
         :param str path: The path of the directory \
             that is to be created.
         '''
         self.__bucket.put_object(
             Key=path,
             ContentType='application/x-directory; charset=UTF-8')
-    
+        
 
-    def read(
-        self,
-        file_path: str,
-        buffer: _io.BytesIO,
-        include_metadata: bool
-    ) -> _Optional[dict[str, str]]:
-        '''
-        Reads the bytes of a file into the provided buffer. \
-        Returns either ``None`` or a dictionary containing \
-        file metadata, depending on the value of parameter \
-        ``include_metadata``.
+    def get_reader(self, file_path: str) -> _AWSS3FileReader:
+        '''
+        Returns an ``AWSS3FileReader`` class instance \
+        used for reading from a file which resides within \
+        an Amazon S3 bucket.
 
-        :param str file_path: The absolute path of the \
-            file in question.
-        :param BytesIO buffer: A buffer to download the \
-            file into.
-        :param bool include_metadata: Indicates whether \
-            to download any existing file metadata as well.
-        '''
-        obj = self.__bucket.Object(key=file_path)
-        obj.download_fileobj(Fileobj=buffer)
-        if include_metadata:
-            return obj.metadata
-        
+        :param str file_path: The absolute path of \
+            the file in question.
+        '''
+        return _AWSS3FileReader(
+            file_path=file_path,
+            file_size=self.get_file_size(file_path),
+            bucket=self.__bucket)
 
-    def write(
+
+    def get_writer(
         self,
         file_path: str,
-        buffer: _io.BytesIO,
-        metadata: _Optional[dict[str, str]]
-    ) -> None:
-        '''
-        Writes the bytes contained within the provided \
-        buffer into the specified path.
-
-        :param str file_path: The absolute path of the \
-            file in question.
-        :param BytesIO buffer: A buffer containing the \
-            file's bytes.
-        :param dict[str, str] | None: If not ``None``, \
-            then assigns the provided metadata to the file \
-            during the upload.
-        '''
-        self.__bucket.upload_fileobj(
-            Key=file_path,
-            Fileobj=buffer,
-            ExtraArgs={ "Metadata": metadata }
-                if metadata is not None else None)
-        
+        metadata: _Optional[dict[str, str]],
+        in_chunks: bool
+    ) -> _AWSS3FileWriter:
+        '''
+        Returns an ``AWSS3FileWriter`` class instance \
+        used for writing to a file which resides within \
+        an Amazon S3 bucket.
+
+        :param str file_path: The absolute path of \
+            the file in question.
+        :param dict[str, str] | None metadata: A \
+            dictionary containing the metadata that \
+            are to be assigned to the file in question. \
+            If ``None``, then no metadata are assigned.
+        :param bool in_chunks: Indicates whether to \
+            write the file in distinct chunks or \
+            all at once.
+        '''
+        return _AWSS3FileWriter(
+            file_path=file_path,
+            metadata=metadata,
+            in_chunks=in_chunks,
+            bucket=self.__bucket)
+    
 
     def _get_file_size_impl(self, file_path) -> int:
         '''
         Fetches and returns the size of a file in bytes.
 
         :param str file_path: The absolute path of the \
             file in question.
@@ -1058,16 +1026,16 @@
     def _traverse_dir_impl(
         self,
         dir_path: str,
         recursively: bool,
         show_abs_path: bool
     ) -> _Iterator[str]:
         '''
-        Returns an iterator capable of going through the paths \
-        of the dictionary's contents as strings.
+        Returns an iterator capable of going through \
+        the directory's contents as their paths.
 
         :param str dir_path: The absolute path of the directory \
             whose contents are to be iterated.
         :param bool recursively: Indicates whether the directory \
             is to be traversed recursively or not. If set to  ``False``, \
             then only those files that reside directly within the \
             directory are to be considered. If set to ``True``, \
@@ -1079,18 +1047,18 @@
             path of the contents.
 
         :note: The resulting iterator may vary depending on the \
             value of parameter ``recursively``.
         '''
         paginator = self.__bucket.meta.client.get_paginator('list_objects')
 
-        delimiter = '' if recursively else '/'
-
         sep = _infer_sep(dir_path)
 
+        delimiter = '' if recursively else sep
+
         def page_iterator():
             yield from paginator.paginate(
                 Bucket=self.__bucket_name,
                 Prefix=dir_path,
                 Delimiter=delimiter)
 
         def object_iterator(response):
@@ -1199,24 +1167,25 @@
         '''
 
         if self.__container is not None:
             return
 
         credentials = self.__auth.get_credentials()
 
+        print(f"\nEstablishing connection to '{self.__container_name}' Azure blob container...")
         if 'conn_string' in credentials:
             self.__container = _ContainerClient.from_connection_string(
                 conn_str=credentials['conn_string'],
                 container_name=self.__container_name)
         else:
             self.__container = _ContainerClient(
                 account_url=credentials.pop('account_url'),
                 container_name=self.__container_name,
                 credential=_CSC(**credentials))
-
+        print("Connection established!")
 
     def close_connections(self):
         '''
         Closes the HTTP connection to the Azure blob container.
         '''
         if self.__container is not None:
             self.__container.close()
@@ -1252,65 +1221,58 @@
 
         :param str path: The path of the directory \
             that is to be created.
         '''
         with self.__container.get_blob_client(blob=f"{path}DUMMY") as blob:
             blob.create_append_blob()
             blob.delete_blob()
-    
 
-    def read(
-        self,
-        file_path: str,
-        buffer: _io.BytesIO,
-        include_metadata: bool
-    ) -> _Optional[dict[str, str]]:
-        '''
-        Reads the bytes of a file into the provided buffer. \
-        Returns either ``None`` or a dictionary containing \
-        file metadata, depending on the value of parameter \
-        ``include_metadata``.
 
-        :param str file_path: The absolute path of the \
-            file in question.
-        :param BytesIO buffer: A buffer to download the \
-            file into.
-        :param bool include_metadata: Indicates whether \
-            to download any existing file metadata as well.
-        '''
-        blob = self.__container.download_blob(blob=file_path)
-        blob.readinto(stream=buffer)
-        if include_metadata:
-            return blob.properties.metadata
-        
+    def get_reader(self, file_path: str) -> _AzureBlobReader:
+        '''
+        Returns an ``AzureBlobReader`` class instance \
+        used for reading from a file which resides within \
+        an Azure blob container.
 
-    def write(
-        self,
-        file_path: str,
-        buffer: _io.BytesIO,
-        metadata: _Optional[dict[str, str]]
-    ) -> None:
+        :param str file_path: The absolute path of \
+            the file in question.
         '''
-        Writes the bytes contained within the provided \
-        buffer into the specified path.
+        return _AzureBlobReader(
+            file_path=file_path,
+            file_size=self.get_file_size(file_path),
+            container=self.__container)
 
-        :param str file_path: The absolute path of the \
-            file in question.
-        :param BytesIO buffer: A buffer containing the \
-            file's bytes.
-        :param dict[str, str] | None: If not ``None``, \
-            then assigns the provided metadata to the file \
-            during the upload.
-        '''
-        self.__container.upload_blob(
-            name=file_path,
-            data=buffer,
-            metadata=metadata if metadata is not None else None,
-            overwrite=True)
-        
+
+    def get_writer(
+        self,
+        file_path: str,
+        metadata: _Optional[dict[str, str]],
+        in_chunks: bool
+    ) -> _AzureBlobWriter:
+        '''
+        Returns an ``AzureBlobWriter`` class instance \
+        used for writing to a file which resides within \
+        an Azure blob container.
+
+        :param str file_path: The absolute path of \
+            the file in question.
+        :param dict[str, str] | None metadata: A \
+            dictionary containing the metadata that \
+            are to be assigned to the file in question. \
+            If ``None``, then no metadata are assigned.
+        :param bool in_chunks: Indicates whether to \
+            write the file in distinct chunks or \
+            all at once.
+        '''
+        return _AzureBlobWriter(
+            file_path=file_path,
+            metadata=metadata,
+            in_chunks=in_chunks,
+            container=self.__container)
+     
 
     def _get_file_size_impl(self, file_path) -> int:
         '''
         Fetches and returns the size of a file in bytes.
 
         :param str file_path: The absolute path of the \
             file in question.
@@ -1333,16 +1295,16 @@
     def _traverse_dir_impl(
         self,
         dir_path: str,
         recursively: bool,
         show_abs_path: bool
     ) -> _Iterator[str]:
         '''
-        Returns an iterator capable of going through the paths \
-        of the dictionary's contents as strings.
+        Returns an iterator capable of going through \
+        the directory's contents as their paths.
 
         :param str dir_path: The absolute path of the directory \
             whose contents are to be iterated.
         :param bool recursively: Indicates whether the directory \
             is to be traversed recursively or not. If set to  ``False``, \
             then only those files that reside directly within the \
             directory are to be considered. If set to ``True``, \
```

### Comparing `fluke-api-0.2.0/fluke/_helper.py` & `fluke-api-0.3.0/fluke/_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,29 +13,32 @@
 
     if len(paths) == 0:
         return ''
 
     path = paths[0]
 
     for i in range(1, len(paths)):
-        path = f"{path.rstrip(sep)}{sep}{paths[i].lstrip(sep)}"
+        if not path.endswith(sep):
+            path += sep
+        path += paths[i]
 
     return path
 
 
 def relativize_path(parent: str, child: str, sep: str) -> str:
     '''
     Modifies the child path so that it is \
     relative to the parent path.
 
     :param str parent: The parent path.
     :param str child: The child path.
     :param str sep: The path separator used.
     '''
-    return child.removeprefix(parent).lstrip(sep)
+    return child.removeprefix(parent)
+    #return child.removeprefix(parent).removeprefix(sep)
 
 
 def infer_separator(path: str) -> str:
     '''
     Infers the separator from the provided path \
     and returns it. If no separator can be inferred, \
     this method will return ``/``.
@@ -45,14 +48,19 @@
     '''
     bs = '\\'
     seps = {'/', 2 * bs, '>'}
 
     if path in seps:
         return path
     
+    # NOTE: Replace any double occurrence of a separator
+    #       as this causes catastrophic backtracking.
+    for sep in seps:
+        path = path.replace(2 * sep, sep)
+    
     seps = ''.join(seps)
     match = _re.fullmatch(
         pattern=fr"({4 * bs}|[{seps}])?(?:[^{seps}])+((?(1)\1|(?:{4 * bs}|[{seps}])))?(?:[^{seps}]+(?(1)\1|\2)?)*",
         string=path,
     )
 
     if match is None:
```

### Comparing `fluke-api-0.2.0/fluke/auth.py` & `fluke-api-0.3.0/fluke/auth.py`

 * *Files identical despite different names*

### Comparing `fluke-api-0.2.0/fluke/storage.py` & `fluke-api-0.3.0/fluke/storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,27 +9,25 @@
     'LocalDir',
     'RemoteFile',
     'RemoteDir'
 ]
 
 
 import os as _os
-import io as _io
 import typing as _typ
 import warnings as _warn
 from abc import ABC as _ABC
 from abc import abstractmethod as _absmethod
 
 
 from tqdm import tqdm as _tqdm
 
 
 from ._helper import join_paths as _join_paths
 from ._helper import infer_separator as _infer_sep
-from ._errors import Error as _Error
 from .auth import AWSAuth as _AWSAuth
 from .auth import AzureAuth as _AzureAuth
 from .auth import RemoteAuth as _RemoteAuth
 from ._handlers import ClientHandler as _ClientHandler
 from ._handlers import FileSystemHandler as _FileSystemHandler
 from ._handlers import SSHClientHandler as _SSHClientHandler
 from ._handlers import AWSClientHandler as _AWSClientHandler
@@ -137,113 +135,228 @@
             self.__metadata.update({ key: val })
 
 
     def get_size(self) -> int:
         '''
         Returns the file's size in bytes.
         '''
-        return self._get_handler().get_file_size(self.get_path())
+        return self._get_handler().get_file_size(
+            file_path=self.get_path())
     
 
     def read(self) -> bytes:
         '''
-        Reads and returns the file's bytes.
+        Reads and returns the file's contents in bytes.
         '''
-        with _io.BytesIO() as buffer:
-            self._get_handler().read(
-                file_path=self.get_path(),
-                buffer=buffer,
-                include_metadata=False)
-            return buffer.getvalue()
+        with self.__handler.get_reader(self.get_path()) as reader:
+            return reader.read()
+        
+
+    def read_range(
+        self,
+        start: _typ.Optional[int],
+        end: _typ.Optional[int]
+    ) -> bytes:
+        '''
+        Returns the file contents that correspond to the \
+        provided byte range.
+
+        :param int | None start: The point in file from which \
+            to begin reading bytes. If ``None``, then begin \
+            reading from the start of the file.
+        :param int | None end: The point in file at which \
+            to stop reading bytes. If ``None``, then stop \
+            reading at the end of the file.
+        '''
+        with self.__handler.get_reader(file_path=self.get_path()) as reader:
+            return reader.read_range(start, end)
+        
+
+    def read_chunks(self, chunk_size: int = 8192) -> _typ.Iterator[bytes]:
+        '''
+        Returns an iterator capable of going through the file's \
+        contents as distinct chunks of bytes.
+
+        :param int chunk_size: The file chunk size in bytes. \
+            Defaults to ``8192``.
+        '''
+        with self.__handler.get_reader(file_path=self.get_path()) as reader:
+            yield from reader.read_chunks(chunk_size=chunk_size)
+
+
+    def read_text(
+        self,
+        encoding: str = 'utf-8'
+    ) -> str:
+        '''
+        Reads and returns the file's contents as text.
+
+        :param str encoding: The encoding with which to decode \
+            the bytes. Defaults to ``utf-8``.
+
+        :note: See
+            `Standard Encodings <https://docs.python.org/3/library/codecs.html#standard-encodings>`_ \
+            for all available encodings.
+        '''
+        return self.read().decode(encoding)
+        
+
+    def read_lines(
+        self,
+        chunk_size: _typ.Optional[int] = None,
+        encoding: str = 'utf-8'
+    ) -> _typ.Iterator[str]:
+        '''
+        Returns an iterator capable of going through \
+        the file line-by-line.
+
+        :param int | None chunk_size: If not ``None``, then the file \
+            is read in distinct chunks, whose size are equal to this \
+            parameter value. Defaults to ``None``.
+        :param str encoding: The encoding with which to decode \
+            the bytes. Defaults to ``utf-8``.
+
+        :note: See
+            `Standard Encodings <https://docs.python.org/3/library/codecs.html#standard-encodings>`_ \
+            for all available encodings.
+        '''
+        if chunk_size is None:
+            for line in self.read_text(encoding).split('\n'):
+                yield line
+        else:
+            text_temp = ''
+            for chunk in self.read_chunks(chunk_size):
+                text_chunks = chunk.decode(encoding).split('\n')
+                if len(text_chunks) > 1:
+                    yield text_temp + text_chunks[0]
+                    for line in text_chunks[1:-1]:
+                        yield line
+                    text_temp = ''
+                text_temp += text_chunks[-1]
+            yield text_temp
 
 
     def transfer_to(
         self,
         dst: '_Directory',
         overwrite: bool = False,
-        include_metadata: bool = False
-    ) -> None:
-        '''
-        Copies the file into the provided directory.
+        include_metadata: bool = False,
+        chunk_size: _typ.Optional[int] = None,
+        suppress_output: bool = False
+    ) -> bool:
+        '''
+        Copies the file into the provided directory. \
+        Returns ``True`` if everything went as expected, \
+        else returns ``False``.
 
         :param _Directory dst: A ``_Directory`` class instance, \
             which represents the transfer operation's destination.
         :param bool overwrite: Indicates whether to overwrite \
             the file if it already exists. Defaults to ``False``.
         :param bool include_metadata: Indicates whether any \
             existing metadata are to be assigned to the resulting \
             file. Defaults to ``False``.
-
-        :raises OverwriteError: File already exists while parameter \
-            ``overwrite`` has been set to ``False``.
-        '''
+        :param int | None chunk_size: If not ``None``, then files are \
+            transferred in chunks, whose size are equal to this parameter \
+            value. Defaults to ``None``.
+        :param bool suppress_output: If set to ``True``, then \
+            suppresses all output. Defaults to ``False``.
+        '''
+        source = self.get_uri() \
+            if isinstance(self, _NonLocalFile) \
+            else self.get_path()
+        
         destination = dst.get_uri() \
             if isinstance(dst, _NonLocalDir) \
             else dst.get_path()
-        print(f'\nCopying file "{self.get_path()}" into "{destination}".')
+        
+        if not suppress_output:
+            print(f'\nTransferring file "{source}" into "{destination}".')
 
-        file_name = self.get_name()
-        error = None
+        dst_fp = dst._to_absolute(self.get_name(), replace_sep=True)
 
-        if not overwrite and dst.path_exists(file_name):
-            raise _OverwriteError(
-                file_path=_join_paths(self._get_separator(), destination, file_name))
-        else:
-            with _io.BytesIO() as buffer:
-                # Read file contents (and metadata optionally)
-                try:
-                    metadata = self.__handler.read(self.get_path(), buffer, include_metadata)
-                    # Update metadata dictionary if necessary.
-                    if include_metadata and (custom_metadata := self.get_metadata()):
-                        metadata = custom_metadata
-                    # Rewind buffer.
-                    buffer.seek(0)
-                    # Write file contents.
-                    dst_file_path = _join_paths(dst._get_separator(), dst.get_path(), file_name)
-                    try:
-                        dst._get_handler().write(
-                            file_path=dst_file_path,
-                            buffer=buffer,
-                            metadata=metadata)
-                        # Upsert the destination's metadata dictionary.
-                        if metadata is not None:
-                            dst._upsert_metadata(file_path=dst_file_path, metadata=metadata)
-                    except Exception as e:
-                        error = _Error(uri=dst_file_path, is_src=False, msg=str(e))
-                except Exception as e:
-                    error = _Error(uri=self.get_uri(), is_src=True, msg=str(e))
-                
-        if error is None:
-            print("Operation successful!")
-        else:
-            print(f"Operation unsuccessful: {error.get_message()}")
+        try:
+            # Raise an "OverwriteError" if file exists
+            # in destination and "overwrite" is "False".
+            if not overwrite and dst.path_exists(dst_fp):
+                raise _OverwriteError(file_path=dst_fp)
+            # Define metadata dictionary.
+            if include_metadata:
+                if custom_metadata := self.get_metadata():
+                    metadata = custom_metadata
+                else:
+                    metadata = self.__handler.get_file_metadata(
+                        file_path=self.get_path())
+            else:
+                metadata = None
+            # Perform the file transfer.
+            with (
+                _tqdm(
+                    disable=(
+                        suppress_output or
+                        chunk_size is None
+                    ),
+                    desc="Progress",
+                    unit='bytes',
+                    total=self.get_size()
+                ) as progress,
+                self.__handler.get_reader(
+                    file_path=self.get_path()
+                ) as reader,
+                dst._get_handler().get_writer(
+                    file_path=dst_fp,
+                    metadata=metadata,
+                    in_chunks=chunk_size is not None
+                ) as writer
+            ):
+                if chunk_size is None:
+                    writer.write(reader.read())
+                else:
+                    for chunk in reader.read_chunks(chunk_size):
+                        progress.update(n=writer.write(chunk))
+            # Upsert metadata to destination if not "None".
+            if metadata is not None:
+                dst._upsert_metadata(
+                    file_path=dst_fp,
+                    metadata=metadata)
+            if not suppress_output:
+                print("Operation successful!")
+        except Exception as e:
+            if not suppress_output:
+                print(f"Operation unsuccessful: {e}")
+            return False
+          
+        return True
     
 
     def _get_close_after_use(self) -> bool:
         '''
         Returns a value indicating whether all open connections \
         should close before the instance destructor is called.
         '''
-        return self.__close_after_use
-    
+        try:
+            return self.__close_after_use
+        except AttributeError:
+            return True
 
-    def _get_handler(self) -> _ClientHandler:
-        '''
-        Returns this instance's ``ClientHandler``.
-        '''
-        return self.__handler
-    
 
     def _get_separator(self) -> str:
         '''
         Returns the file's path separator.
         '''
         return self.__separator
     
 
+    def _get_handler(self) -> _ClientHandler:
+        '''
+        Returns this instance's ``ClientHandler``.
+        '''
+        return self.__handler
+    
+
     def __new__(
         cls,
         *args,
         **kwargs
     ) -> 'LocalFile':
         '''
         Creates an instance of this class.
@@ -303,15 +416,15 @@
             handler=_FileSystemHandler())
         
 
     def get_uri(self) -> str:
         '''
         Returns the file's URI.
         '''
-        return f"file:///{self.get_path().lstrip(self._get_separator())}"
+        return f"file:///{self.get_path().removeprefix(self._get_separator())}"
 
 
     @classmethod
     def _create_file(
         cls,
         path: str,
         handler: _FileSystemHandler,
@@ -330,15 +443,15 @@
         _File.__init__(
             instance,
             path=path,
             metadata=metadata,
             handler=handler,
             close_after_use=False)
         return instance
-
+    
 
 class _NonLocalFile(_File, _ABC):
     '''
     An abstract class which serves as the base class for \
     all file-like classes that represent either remote files \
     or files in the cloud.
 
@@ -417,15 +530,16 @@
         The class destructor method.
         '''
         if self._get_close_after_use():
             if (handler := self._get_handler()) is not None:
                 # Purge cache.
                 self.purge()
                 # Warn if connections are open.
-                if  handler.is_open():
+                if handler.is_open():
+                    # Display warning.
                     msg = f'You might want to consider instantiating class "{self.__class__.__name__}"'
                     msg += " through the use of a context manager by utilizing Python's"
                     msg += ' "with" statement, or by simply invoking an instance\'s'
                     msg += ' "close" method after being done using it.'
                     _warn.warn(msg, ResourceWarning)
                     # Close connections.
                     self.close()
@@ -469,19 +583,19 @@
             access. Defaults to ``False``.
 
         :raises InvalidPathError: The provided path \
             does not exist.
         :raises InvalidFileError: The provided path \
             points to a directory.
         '''
-        # Instantiate a connection handler,
-        # if none has been set.
-        if (ssh_handler := self._get_handler()) is None:
-            ssh_handler = _SSHClientHandler(auth=auth, cache=cache)
-            self.__host = auth.get_credentials()['hostname']
+        # Instantiate a connection handler.
+        ssh_handler = _SSHClientHandler(auth=auth, cache=cache)
+
+        # Set up hostname.
+        self.__host = auth.get_credentials()['hostname']
 
         super().__init__(
             path=path,
             handler=ssh_handler)
 
         if not ssh_handler.path_exists(path=path):
             self.close()
@@ -500,15 +614,15 @@
         return self.__host
 
 
     def get_uri(self) -> str:
         '''
         Returns the file's URI.
         '''
-        return f"sftp://{self.__host}/{self.get_path().lstrip(self._get_separator())}"
+        return f"sftp://{self.__host}/{self.get_path().removeprefix(self._get_separator())}"
     
 
     @classmethod
     def _create_file(
         cls,
         path: str,
         host: str,
@@ -531,15 +645,15 @@
         _File.__init__(
             instance,
             path=path,
             metadata=metadata,
             handler=handler,
             close_after_use=False)
         return instance
-    
+
 
     def __enter__(self) -> 'RemoteFile':
         '''
         Enter the runtime context related to this instance.
         '''
         return self
 
@@ -556,15 +670,16 @@
         which can then be accessed via the instance's \
         ``get_metadata`` method.
 
         :note: Any metadata set via the ``set_metadata`` \
             method will be overriden after invoking this \
             method.
         '''
-        metadata = self._get_handler().get_file_metadata(self.get_path())
+        metadata = self._get_handler().get_file_metadata(
+            self.get_path())
         self.set_metadata(metadata=metadata)
 
 
 class AWSS3File(_CloudFile):
     '''
     This class represents an object which resides \
     within an Amazon S3 bucket.
@@ -579,17 +694,19 @@
         access.
 
     :raises InvalidPathError: The provided path \
         does not exist.
     :raises InvalidFileError: The provided path \
         points to a directory.
 
-    :note: The provided path must not begin with a separator.
-        - Wrong: ``/path/to/file.txt``
-        - Right: ``path/to/file.txt``
+    :note: The provided path must not begin with \
+        a separator.
+
+            * Wrong: ``/path/to/file.txt``
+            * Right: ``path/to/file.txt``
     '''
 
     def __init__(
         self,
         auth: _AWSAuth,
         bucket: str,
         path: str,
@@ -609,32 +726,31 @@
             access. Defaults to ``False``.
 
         :raises InvalidPathError: The provided path \
             does not exist.
         :raises InvalidFileError: The provided path \
             points to a directory.
 
-        :note: The provided path must not begin with a separator.
-            - Wrong: ``/path/to/file.txt``
-            - Right: ``path/to/file.txt``
+        :note: The provided path must not begin with \
+            a separator.
+                
+                * Wrong: ``/path/to/file.txt``
+                * Right: ``path/to/file.txt``
         '''
         # Validate path.
         sep = _infer_sep(path=path)
-
         if path.startswith(sep):
             raise _IPE(path=path)
         
-        # Instantiate a connection handler,
-        # if none has been set.
-        if (aws_handler := self._get_handler()) is None:
-            aws_handler = _AWSClientHandler(
-                auth=auth,
-                bucket=bucket,
-                cache=cache)
-        
+        # Instantiate a connection handler.
+        aws_handler = _AWSClientHandler(
+            auth=auth,
+            bucket=bucket,
+            cache=cache)
+
         super().__init__(
             path=path,
             handler=aws_handler)
 
         if not aws_handler.path_exists(path=path):
             if aws_handler.dir_exists(path=path):
                 self.close()
@@ -668,16 +784,14 @@
         handler: _AWSClientHandler,
         metadata: dict[str, str]
     ) -> 'AWSS3File':
         '''
         Creates and returns an ``AWSS3File`` instance.
 
         :param str path: The path pointing to the file.
-        :param str host: The name of the host in which \
-            the file resides.
         :param AWSClientHandler handler: An ``AWSClientHandler`` \
             class instance.
         :param dict[str, str] metadata: A dictionary containing \
             any metadata associated with the file.
         '''
         instance = cls.__new__(cls)
         _File.__init__(
@@ -713,17 +827,19 @@
     :raises AzureBlobContainerNotFoundError: The \
         specified container does not exist.
     :raises InvalidPathError: The provided path \
         does not exist.
     :raises InvalidFileError: The provided path \
         points to a directory.
 
-    :note: The provided path must not begin with a separator.
-        - Wrong: ``/path/to/file.txt``
-        - Right: ``path/to/file.txt``
+    :note: The provided path must not begin with \
+        a separator.
+            
+            * Wrong: ``/path/to/file.txt``
+            * Right: ``path/to/file.txt``
     '''
 
     def __init__(
         self,
         auth: _AzureAuth,
         container: str,
         path: str,
@@ -745,30 +861,30 @@
         :raises AzureBlobContainerNotFoundError: The \
             specified container does not exist.
         :raises InvalidPathError: The provided path \
             does not exist.
         :raises InvalidFileError: The provided path \
             points to a directory.
 
-        :note: The provided path must not begin with a separator.
-            - Wrong: ``/path/to/file.txt``
-            - Right: ``path/to/file.txt``
+        :note: The provided path must not begin with \
+            a separator.
+                
+                * Wrong: ``/path/to/file.txt``
+                * Right: ``path/to/file.txt``
         '''
         # Validate path.
         sep = _infer_sep(path=path)
         if path.startswith(sep):
             raise _IPE(path=path)
 
-        # Instantiate a connection handler,
-        # if none has been set.
-        if (azr_handler := self._get_handler()) is None:
-            azr_handler = _AzureClientHandler(
-                auth=auth,
-                container=container,
-                cache=cache)
+        # Instantiate a connection handler.
+        azr_handler = _AzureClientHandler(
+            auth=auth,
+            container=container,
+            cache=cache)
         
         # Infer storage account.
         self.__storage_account = auth._get_storage_account()
         
         super().__init__(
             path=path,
             handler=azr_handler)
@@ -803,29 +919,31 @@
         return uri
     
 
     @classmethod
     def _create_file(
         cls,
         path: str,
+        storage_account: str,
         handler: _AzureClientHandler,
         metadata: dict[str, str]
     ) -> 'AzureBlobFile':
         '''
         Creates and returns an ``AzureBlobFile`` instance.
 
         :param str path: The path pointing to the file.
-        :param str host: The name of the host in which \
-            the file resides.
-        :param AWSClientHandler handler: An ``AzureClientHandler`` \
+        :param str storage_account: The name of the storage \
+            account to which the blob's container belongs.
+        :param AzureClientHandler handler: An ``AzureClientHandler`` \
             class instance.
         :param dict[str, str] metadata: A dictionary containing \
             any metadata associated with the file.
         '''
         instance = cls.__new__(cls)
+        instance.__storage_account = storage_account
         _File.__init__(
             instance,
             path=path,
             metadata=metadata,
             handler=handler,
             close_after_use=False)
         return instance
@@ -840,39 +958,54 @@
 
 class _Directory(_ABC):
     '''
     An abstract class which serves as the base class \
     for all directory-like classes.
 
     :param str path: The path pointing to the directory.
+    :param dict[str, dict[str, str]] metadata: A dictionary \
+        containing file metadata.
     :param ClientHandler handler: A ``ClientHandler`` class \
         instance used for interacting with the underlying handler.
+    :param bool close_after_use: This value indicates whether \
+        all open connections should close before the instance \
+        destructor is called.
     '''
 
     def __init__(
         self,
         path: str,
+        metadata: dict[str, dict[str, str]],
         handler: _ClientHandler,
+        close_after_use: bool = True
     ):
         '''
         An abstract class which serves as the base class \
         for all directory-like classes.
 
         :param str path: The path pointing to the directory.
+        :param dict[str, dict[str, str]] metadata: A dictionary \
+            containing file metadata.
         :param ClientHandler handler: A ``ClientHandler`` class \
             instance used for interacting with the underlying handler.
+        :param bool close_after_use: This value indicates whether \
+            all open connections should close before the instance \
+            destructor is called.
         '''
         sep = _infer_sep(path)
-        self.__path = f"{path.rstrip(sep)}{sep}" if path != '' else path
+        self.__path = (
+            f"{path.removesuffix(sep)}{sep}"
+            if path != '' else path)
         self.__name = name if (
-                name := self.__path.rstrip(sep).split(sep)[-1]
+                name := self.__path.removesuffix(sep).split(sep)[-1]
             ) != '' else None
         self.__separator = sep
         self.__handler = handler
-        self.__metadata: dict[str, dict[str, str]] = dict()
+        self.__metadata = metadata
+        self.__close_after_use = close_after_use
 
 
     def get_path(self) -> str:
         '''
         Returns the path to the directory.
         '''
         return self.__path
@@ -894,15 +1027,15 @@
         :param str file_path: Either the absolute path \
             or the path relative to the directory of the \
             file in question.
 
         :raises InvalidFileError: The provided path does \
             not point to a file within the directory.
         '''
-        return dict(self._get_metadata_ref(file_path=file_path))
+        return dict(self._get_file_metadata_ref(file_path=file_path))
 
 
     def set_metadata(self, file_path: str, metadata: dict[str, str]) -> None:
         '''
         Associates the provided metadata with \
         the file located in the given path.
 
@@ -961,16 +1094,16 @@
 
     def traverse(
         self,
         recursively: bool = False,
         show_abs_path: bool = False
     ) -> _typ.Iterator[str]:
         '''
-        Returns an iterator capable of traversing the dictionary's \
-        contents as strings representing their paths.
+        Returns an iterator capable of traversing the directory \
+        by going through the paths of its contents.
 
         :param bool recursively: Indicates whether the directory \
             is to be traversed recursively or not. If set to  ``False``, \
             then only those files that reside directly within the \
             directory are to be considered. If set to ``True``, \
             then all files are considered, no matter whether they \
             reside directly within the directory or within any of \
@@ -991,16 +1124,16 @@
 
     def get_contents(
         self,
         recursively: bool = False,
         show_abs_path: bool = False
     ) -> list[str]:
         '''
-        Returns an iterator capable of traversing the dictionary's \
-        contents as strings representing their paths.
+        Returns a list containing the paths that \
+        correspond to the directory's contents.
 
         :param bool recursively: Indicates whether the directory \
             is to be traversed recursively or not. If set to  ``False``, \
             then only those files that reside directly within the \
             directory are to be considered. If set to ``True``, \
             then all files are considered, no matter whether they \
             reside directly within the directory or within any of \
@@ -1101,19 +1234,22 @@
 
     def transfer_to(
         self,
         dst: '_Directory',
         recursively: bool = False,
         overwrite: bool = False,
         include_metadata: bool = False,
-        show_progress: bool = True
-    ) -> None:
+        chunk_size: _typ.Optional[int] = None,
+        suppress_output: bool = False,
+    ) -> bool:
         '''
         Copies all files within this directory into \
-        the destination directory.
+        the destination directory. Returns ``True`` if \
+        all files were successfully transferred, else returns \
+        ``False``.
 
         :param _Directory dst: A ``_Directory`` class instance, \
             which represents the transfer operation's destination.
         :param bool recursively: Indicates whether the directory \
             is to be traversed recursively or not. If set to  ``False``, \
             then only those files that reside directly within the \
             directory are to be considered. If set to ``True``, \
@@ -1121,271 +1257,265 @@
             reside directly within the directory or within any of \
             its subdirectories. Defaults to ``False``.
         :param bool overwrite: Indicates whether to overwrite \
             any files if they already exist. Defaults to ``False``.
         :param bool include_metadata: Indicates whether any \
             existing metadata are to be assigned to the resulting \
             files. Defaults to ``False``.
-        :param bool show_progress: Indicates whether to display \
-            a loading bar on the progress of the operations. \
-            Defaults to ``True``.
+        :param int | None chunk_size: If not ``None``, then files are \
+            transferred in chunks, whose size are equal to this parameter \
+            value. Defaults to ``None``.
+        :param bool suppress_output: If set to ``True``, then \
+            suppresses all output. Defaults to ``False``.
         '''
-        destination = dst.get_uri() \
-            if isinstance(dst, _NonLocalDir) \
-            else dst.get_path()
-
-        print_msg = f'\nCopying files from "{self.get_path()}" '
-        print_msg += f'into "{destination}".'
-        print(print_msg)
-
         # Store the directory's files in a list.
         file_paths = [fp for fp in self.__handler.traverse_dir(
             dir_path = self.get_path(),
             recursively=recursively,
             include_dirs=False,
             show_abs_path=True)]
 
-        errors: list[_Error] = list()
         total_num_files = len(file_paths)
+        failures = 0
+        dst_dirs = dict()
 
-        # Iterate through all files that are to be transfered.
-        for fp in _tqdm(
-            iterable=file_paths,
-            disable=not show_progress,
-            desc="Progress",
-            unit='files',
-            total=total_num_files
-        ):
-            rel_fp = self._to_relative(fp, replace_sep=False)
-            if not overwrite and dst.path_exists(rel_fp):
-                errors.append(_Error(
-                    uri=_join_paths(dst._get_separator(), destination, rel_fp),
-                    is_src=False,
-                    msg='File already exists. Try setting "overwrite" to "True".'))
-                continue
-
-            with _io.BytesIO() as buffer:
-                try:
-                    # Read file contents (and metadata optionally).
-                    metadata = self.__handler.read(fp, buffer, include_metadata)
-                    # Update metadata dictionary if necessary.
-                    if include_metadata and (custom_metadata := self.get_metadata(fp)):
-                        metadata = custom_metadata
-                    # Rewind buffer.
-                    buffer.seek(0)
-                    # Write file contents.
-                    dst_fp = dst._to_absolute(rel_fp, replace_sep=True)
-                    dst._get_handler().write(
-                        file_path=dst_fp,
-                        buffer=buffer,
-                        metadata=metadata)
-                    # Upsert the destination's metadata dictionary.
-                    if metadata is not None:
-                        dst._upsert_metadata(file_path=dst_fp, metadata=metadata)
-                except Exception as e:
-                    errors.append(_Error(uri=self.get_uri(), is_src=True, msg=str(e)))
+        # Iterate through all files that are to be transferred.
+        for i, fp in enumerate(file_paths):
 
-        if len(errors) == 0:
-            print(f'Operation successful: Copied all {total_num_files} files!')
+            # Define src and dst paths.
+            rel_fp = self._to_relative(path=fp, replace_sep=False)
+            dst_sep = dst._get_separator()
+            dst_fp = (dst_sep
+                .join(dst._to_absolute(path=rel_fp, replace_sep=True)
+                .split(dst_sep)[:-1])
+                + dst_sep)
+            
+            # Fetch src file and dst directory.
+            src_file = self.get_file(path=fp)
+            if dst_fp in dst_dirs:
+                dst_dir = dst_dirs[dst_fp]
+            else:
+                dst_dir = dst._get_subdir_impl(dst_fp)
+                dst_dirs.update({dst_fp: dst_dir})
+
+            # Perform the transfer.
+            if not src_file.transfer_to(
+                dst=dst_dir,
+                overwrite=overwrite,
+                include_metadata=include_metadata,
+                chunk_size=chunk_size,
+                suppress_output=suppress_output
+            ):
+                failures += 1
+
+            if not suppress_output:
+                print(f"Total progress: {i+1}/{total_num_files} files.")
+
+        if failures == 0:
+            if not suppress_output:
+                print(f'\nOperation successful: All {total_num_files} files were transferred!')
+            return True
         else:
-            msg = "Operation unsuccessful: Failed to copy "
-            msg += f"{len(errors)} out of {total_num_files} files."
-            msg += f"\n\nDisplaying {len(errors)} errors:\n"
-            for err in errors:
-                msg += str(err)
-            print(msg)
+            if not suppress_output:
+                msg = f"\nOperation unsuccessful: {failures} out of "
+                msg += f"{total_num_files} files failed to be transferred."
+                print(msg)
+            return False
     
-
-    def traverse_files(
-        self,
-        recursively: bool = False
-    ) -> _typ.Iterator[_File]:
-        '''
-        Returns an iterator capable of going through the \
-        dictionaries files as ``File`` instances.
-
-        :param bool recursively: Indicates whether the directory \
-            is to be traversed recursively or not. If set to  ``False``, \
-            then only those files that reside directly within the \
-            directory are to be considered. If set to ``True``, \
-            then all files are considered, no matter whether they \
-            reside directly within the directory or within any of \
-            its subdirectories. Defaults to ``False``.
-
-        :note: The resulting iterator may vary depending on the \
-            value of parameter ``recursively``.
-        '''
-        for file_path in self.__handler.traverse_dir(
-            dir_path=self.get_path(),
-            recursively=recursively,
-            include_dirs=False,
-            show_abs_path=True
-        ):
-            yield self.get_file(file_path)
-
-
-    def get_files(
-        self,
-        recursively: bool = False,
-        show_abs_path: bool = False
-    ) -> dict[str, _File]:
+    
+    def _get_close_after_use(self) -> bool:
         '''
-        Returns a dictionary mapping file paths to ``File`` instances \
-        regarding the files contained within the directory.
-
-        :param bool recursively: Indicates whether the directory \
-            is to be traversed recursively or not. If set to  ``False``, \
-            then only those files that reside directly within the \
-            directory are to be considered. If set to ``True``, \
-            then all files are considered, no matter whether they \
-            reside directly within the directory or within any of \
-            its subdirectories. Defaults to ``False``.
-        :param bool show_abs_path: Determines whether to include the \
-            files' absolute path or their path relative to this directory. \
-            Defaults to ``False``.
-
-        :note: The resulting iterator may vary depending on the \
-            value of parameter ``recursively``.
+        Returns a value indicating whether all open connections \
+        should close before the instance destructor is called.
         '''
-        file_dict = dict()
-        for file_path in self.__handler.traverse_dir(
-            dir_path=self.get_path(),
-            recursively=recursively,
-            include_dirs=False,
-            show_abs_path=show_abs_path
-        ):
-            file_dict.update({ file_path: self.get_file(file_path)})
-        return file_dict
-
+        try:
+            return self.__close_after_use
+        except AttributeError:
+            return True
+    
 
     def _get_separator(self) -> str:
         '''
-        Returns the path's separator.
+        Returns the directory path's separator.
         '''
         return self.__separator
     
 
     def _get_handler(self) -> _ClientHandler:
         '''
         Returns this instance's ``ClientHandler``.
         '''
         return self.__handler
     
 
+    def _get_metadata_ref(self) -> dict[str, dict[str, str]]:
+        '''
+        Returns a reference to the metadata dictionary.
+        '''
+        return self.__metadata
+    
+
+    def _get_file_metadata_ref(self, file_path: str) -> dict[str, str]:
+        '''
+        Returns a reference to the metadata dictionary \
+        that corresponds to the specified file. If said \
+        dictionary doesn't exist, then this method creates it \
+        and returns it.
+
+        :param str file_path: Either the absolute path \
+            or the path relative to the directory of the \
+            file in question.
+
+        :raises InvalidFileError: The provided path does \
+            not point to a file within the directory.
+        '''
+        if not (self.path_exists(file_path) and self.is_file(file_path)):
+            raise _IFE(path=file_path)
+        
+        abs_path = self._to_absolute(path=file_path, replace_sep=False)
+        
+        if abs_path not in self.__metadata:
+            self.__metadata.update({abs_path: dict()})
+
+        return self.__metadata.get(abs_path)
+    
+
     def _to_relative(self, path: str, replace_sep: bool) -> str:
         '''
         Transforms the provided path so that it is \
         relative to the directory.
 
         :param str path: The provided path.
         :param bool replace_sep: Indicates whether \
             to replace the provided path's separator \
             with the separator used by this directory.
         '''
         if replace_sep:
             sep = _infer_sep(path)
             path = path.replace(sep, self._get_separator())
-        return path.removeprefix(self.__path).lstrip(self._get_separator())
+        return path.removeprefix(self.__path)
     
 
     def _to_absolute(self, path: str, replace_sep: bool) -> str:
         '''
         Transforms the provided path so that it is \
         absolute.
 
         :param str path: The provided path.
         :param bool replace_sep: Indicates whether \
             to replace the provided path's separator \
             with the separator used by this directory.
         '''
-        path = self._to_relative(path, replace_sep)
-        return _join_paths(self._get_separator(), self.__path, path)
-    
-
-    def _get_metadata_ref(self, file_path: str) -> dict[str, str]:
-        '''
-        Returns the reference to the metadata dictionary \
-        that corresponds to the specified path. If said \
-        dictionary doesn't exist, then this method creates it \
-        and returns it.
-
-        :param str file_path: Either the absolute path \
-            or the path relative to the directory of the \
-            file in question.
-
-        :raises InvalidFileError: The provided path does \
-            not point to a file within the directory.
-        '''
-        if not (self.path_exists(file_path) and self.is_file(file_path)):
-            raise _IFE(path=file_path)
-        
-        rel_path = self._to_relative(path=file_path, replace_sep=False)
-        
-        if rel_path not in self.__metadata:
-            self.__metadata.update({rel_path: dict()})
-
-        return self.__metadata.get(rel_path)
-    
+        path = self._to_relative(path, replace_sep=False)
+        path = _join_paths(self._get_separator(), self.__path, path)
+        if replace_sep:
+            sep = _infer_sep(path)
+            path = path.replace(sep, self._get_separator())
+        return path
+            
 
     def _upsert_metadata(self, file_path: str, metadata: dict[str, str]) -> None:
         '''
         Updates the metadata dictionary by \
         upserting the provided metadata.
 
         :param str file_path: Either the absolute path \
             or the path relative to the directory of the \
             file in question.
         :param dict[str, str] metadata: A dictionary \
             containing the metadata that are to be \
             associated with the file.
         '''
-        # NOTE: Update the metadata dictionary without
-        #       creating a new reference.
-        rel_path = self._to_relative(path=file_path, replace_sep=False)
+        abs_path = self._to_absolute(path=file_path, replace_sep=False)
 
-        if rel_path not in self.__metadata:
-            self.__metadata.update({rel_path: dict()})
+        if abs_path not in self.__metadata:
+            self.__metadata.update({abs_path: dict()})
 
-        self.__metadata[rel_path].clear()
+        # NOTE: Update the metadata dictionary without
+        #       creating a new reference.
+        self.__metadata[abs_path].clear()
 
         for (key, val) in metadata.items():
-            self.__metadata[rel_path].update({ key: val })
+            self.__metadata[abs_path].update({ key: val })
     
 
     def __new__(cls, *args, **kwargs) -> '_Directory':
         '''
         Creates an instance of this class.
 
         :note: This method defines field ``__handler`` \
             so that throwing an exception before invoking \
             the parent constructor does not result in a \
             second exception being thrown due to ``__del__``.
         '''
-        instance = super().__new__(cls)
+        instance = object.__new__(cls)
         instance.__handler = None
         return instance
     
 
     @_absmethod
     def get_uri(self) -> str:
         '''
         Returns the directory's URI.
         '''
         pass
 
 
     @_absmethod
-    def get_file(self, file_path: str) -> '_File':
+    def get_file(self, path: str) -> '_File':
         '''
         Returns the file residing in the specified \
         path as a ``_File`` instance.
 
-        :param str file_path: Either the absolute path \
+        :param str path: Either the absolute path or the \
+            path relative to the directory of the file in \
+            question.
+
+        :raises InvalidPathError: The provided path \
+            does not exist.
+        :raises InvalidFileError: The provided path does \
+            not point to a file within the directory.
+        '''
+        pass
+
+    
+    @_absmethod
+    def get_subdir(self, path: str) -> '_Directory':
+        '''
+        Returns the directory residing in the specified \
+        path as a ``_Directory`` instance.
+
+        :param str path: Either the absolute path or the \
+            path relative to the directory of the subdirectory \
+            in question.
+
+        :raises InvalidPathError: The provided path \
+            does not exist.
+        :raises InvalidDirectoryError: The provided path \
+            does not point to a subdirectory within the \
+            directory.
+        '''
+        pass
+
+
+    @_absmethod
+    def _get_subdir_impl(self, dir_path: str) -> '_Directory':
+        '''
+        Returns the directory residing in the specified \
+        path as a ``_Directory`` instance.
+
+        :param str dir_path: Either the absolute path \
             or the path relative to the directory of the \
-            file in question.
+            subdirectory in question.
+
+        :raises InvalidPathError: The provided path \
+            does not exist.
+        :raises InvalidDirectoryError: The provided path \
+            does not point to a subdirectory within the \
+            directory.
         '''
         pass
 
 
 class LocalDir(_Directory):
     '''
     This class represents a directory which resides \
@@ -1430,89 +1560,122 @@
                 raise _IPE(path)
         elif not _os.path.isdir(path):
             raise _IDE(path)
 
         sep = _infer_sep(path=path)
 
         super().__init__(
-            path=f"{_os.path.abspath(path).replace(_os.sep, sep).rstrip(sep)}{sep}",
+            path=f"{_os.path.abspath(path).replace(_os.sep, sep).removesuffix(sep)}{sep}",
+            metadata=dict(),
             handler=_FileSystemHandler())
 
 
     def get_uri(self) -> str:
         '''
         Returns the directory's URI.
         '''
         sep = self._get_separator()
-        return f"file:///{self.get_path().lstrip(sep)}"
+        return f"file:///{self.get_path().removeprefix(sep)}"
 
 
-    def get_file(self, file_path: str) -> LocalFile:
+    def get_file(self, path: str) -> LocalFile:
         '''
         Returns the file residing in the specified \
         path as a ``LocalFile`` instance.
 
-        :param str file_path: Either the absolute path \
-            or the path relative to the directory of the \
-            file in question.
+        :param str path: Either the absolute path or the \
+            path relative to the directory of the file in \
+            question.
+
+        :raises InvalidPathError: The provided path \
+            does not exist.
+        :raises InvalidFileError: The provided path does \
+            not point to a file within the directory.
         '''
-        file_path = self._to_absolute(path=file_path, replace_sep=False)
+        if not self.path_exists(path):
+            raise _IPE(path=path)
+        if not self.is_file(path):
+            raise _IFE(path=path)
+        
+        path = self._to_absolute(path=path, replace_sep=False)
         return LocalFile._create_file(
-            path=file_path,
+            path=path,
             handler=self._get_handler(),
-            metadata=self._get_metadata_ref(file_path))
+            metadata=self._get_file_metadata_ref(path))
     
 
-    def traverse_files(
-        self,
-        recursively: bool = False
-    ) -> _typ.Iterator[LocalFile]:
+    def get_subdir(self, path: str) -> 'LocalDir':
         '''
-        Returns an iterator capable of going through the \
-        dictionaries files as ``File`` instances.
+        Returns the directory residing in the specified \
+        path as a ``LocalDir`` instance.
 
-        :param bool recursively: Indicates whether the directory \
-            is to be traversed recursively or not. If set to  ``False``, \
-            then only those files that reside directly within the \
-            directory are to be considered. If set to ``True``, \
-            then all files are considered, no matter whether they \
-            reside directly within the directory or within any of \
-            its subdirectories. Defaults to ``False``.
+        :param str path: Either the absolute path or the \
+            path relative to the directory of the subdirectory \
+            in question.
 
-        :note: The resulting iterator may vary depending on the \
-            value of parameter ``recursively``.
+        :raises InvalidPathError: The provided path \
+            does not exist.
+        :raises InvalidDirectoryError: The provided path \
+            does not point to a subdirectory within the \
+            directory.
         '''
-        yield from super().traverse_files(recursively=recursively)
 
+        if not self.path_exists(path):
+            raise _IPE(path=path)
+        if self.is_file(path):
+            raise _IDE(path=path)
+        
+        return self._get_subdir_impl(path)
+    
 
-    def get_files(
-        self,
-        recursively: bool = False,
-        show_abs_path: bool = False
-    ) -> dict[str, LocalFile]:
+    @classmethod
+    def _create_dir(
+        cls,
+        path: str,
+        handler: _FileSystemHandler,
+        metadata: dict[str, str]
+    ) -> 'LocalDir':
         '''
-        Returns a dictionary mapping file paths to ``File`` instances \
-        regarding the files contained within the directory.
+        Creates and returns a ``LocalDir`` instance.
 
-        :param bool recursively: Indicates whether the directory \
-            is to be traversed recursively or not. If set to  ``False``, \
-            then only those files that reside directly within the \
-            directory are to be considered. If set to ``True``, \
-            then all files are considered, no matter whether they \
-            reside directly within the directory or within any of \
-            its subdirectories. Defaults to ``False``.
-        :param bool show_abs_path: Determines whether to include the \
-            files' absolute path or their path relative to this directory. \
-            Defaults to ``False``.
+        :param str path: The path pointing to the directory.
+        :param FileSystemHandler handler: A ``FileSystemHandler`` \
+            class instance.
+        :param dict[str, str] metadata: A dictionary containing \
+            file metadata.
+        '''
+        instance = cls.__new__(cls)
+        _Directory.__init__(
+            instance,
+            path=path,
+            metadata=metadata,
+            handler=handler,
+            close_after_use=False)
+        path = instance.get_path()
+        return instance
+    
 
-        :note: The resulting iterator may vary depending on the \
-            value of parameter ``recursively``.
+    def _get_subdir_impl(self, dir_path: str) -> 'LocalDir':
         '''
-        return super().get_files(
-            recursively=recursively, show_abs_path=show_abs_path)
+        Returns the directory residing in the specified \
+        path as a ``LocalDir`` instance.
+
+        :param str dir_path: Either the absolute path \
+            or the path relative to the directory of the \
+            subdirectory in question.
+        '''        
+        sep = self._get_separator()
+        dir_path = f"{dir_path.removesuffix(sep)}{sep}"
+        dir_path = self._to_absolute(
+            path=dir_path, replace_sep=False)
+        
+        return __class__._create_dir(
+            path=dir_path,
+            handler=self._get_handler(),
+            metadata=self._get_metadata_ref())
 
 
 class _NonLocalDir(_Directory, _ABC):
     '''
     An abstract class which serves as the base class for \
     all directory-like classes that represent either remote \
     directories or directories in the cloud.
@@ -1531,15 +1694,15 @@
         all directory-like classes that represent either remote \
         directories or directories in the cloud.
 
         :param str path: The path pointing to the directory.
         :param ClientHandler handler: A ``ClientHandler`` class \
             instance used for interacting with the underlying handler.
         '''
-        super().__init__(path=path, handler=handler)
+        super().__init__(path=path, metadata=dict(), handler=handler)
         self.open()
 
 
     def is_cacheable(self) -> bool:
         '''
         Returns ``True`` if directory has been \
         defined as cacheable, else returns ``False``.
@@ -1565,46 +1728,48 @@
     def close(self) -> None:
         '''
         Closes all open connections.
         '''
         self._get_handler().close_connections()
 
 
-    def __del__(self) -> None:
-        '''
-        The class destructor method.
-        '''
-        handler = self._get_handler()
-        if handler is not None and handler.is_open():
-            # Purge cache (if it exists).
-            self.purge()
-            # Close any open connections.
-            self.close()
-            # Display warning.
-            msg = f'You might want to consider instantiating class "{self.__class__.__name__}"'
-            msg += " through the use of a context manager by utilizing Python's"
-            msg += ' "with" statement, or by simply invoking an instance\'s'
-            msg += ' "close" method after being done using it.'
-            _warn.warn(msg, ResourceWarning)
-    
-
     def __enter__(self) -> '_NonLocalDir':
         '''
         Enter the runtime context related to this instance.
         '''
         return self
 
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         '''
         Exit the runtime context related to this object. 
         '''
         self.close()
 
 
+    def __del__(self) -> None:
+        '''
+        The class destructor method.
+        '''
+        if self._get_close_after_use():
+            if (handler := self._get_handler()) is not None:
+                # Purge cache.
+                self.purge()
+                # Warn if connections are open.
+                if handler.is_open():
+                    # Display warning.
+                    msg = f'You might want to consider instantiating class "{self.__class__.__name__}"'
+                    msg += " through the use of a context manager by utilizing Python's"
+                    msg += ' "with" statement, or by simply invoking an instance\'s'
+                    msg += ' "close" method after being done using it.'
+                    _warn.warn(msg, ResourceWarning)
+                    # Close connections.
+                    self.close()
+
+
 class RemoteDir(_NonLocalDir):
     '''
     This class represents a directory which resides \
     within a remote file system.
 
     :param RemoteAuth auth: A ``RemoteAuth`` \
         instance used for authenticating with a remote \
@@ -1646,34 +1811,35 @@
             in case it does not already exist, instead of an exception being \
             thrown. Defaults to ``False``.
 
         :raises InvalidPathError: The provided path \
             does not exist.
         :raises InvalidDirectoryError: The provided path \
             does not point to a directory.
-        '''
-        # Validate path.
-        if path == '':
-            raise _IPE(path=path)
-        
+        '''        
         ssh_handler = _SSHClientHandler(auth=auth, cache=cache)
+        self.__host = auth.get_credentials()['hostname']
 
         super().__init__(
             path=path,
             handler=ssh_handler)
-
-        self.__host = auth.get_credentials()['hostname']
+        
+        # Validate path.
+        if path == '':
+            self.close()
+            raise _IPE(path=path)
 
         if not ssh_handler.path_exists(path=path):
             if create_if_missing:
                 ssh_handler.mkdir(path=path)
             else:
                 self.close()
                 raise _IPE(path)
         if ssh_handler.is_file(file_path=path):
+            self.close()
             raise _IDE(path)
 
 
     def get_hostname(self) -> str:
         '''
         Returns the name of the host in which \
         this directory resides.
@@ -1681,81 +1847,116 @@
         return self.__host
 
 
     def get_uri(self) -> str:
         '''
         Returns the directory's URI.
         '''
-        return f"sftp://{self.__host}/{self.get_path().lstrip(self._get_separator())}"
+        return f"sftp://{self.__host}/{self.get_path().removeprefix(self._get_separator())}"
     
 
-    def get_file(self, file_path: str) -> RemoteFile:
+    def get_file(self, path: str) -> RemoteFile:
         '''
         Returns the file residing in the specified \
         path as a ``RemoteFile`` instance.
 
-        :param str file_path: Either the absolute path \
-            or the path relative to the directory of the \
-            file in question.
+        :param str path: Either the absolute path or the \
+            path relative to the directory of the file in \
+            question.
+
+        :raises InvalidPathError: The provided path \
+            does not exist.
+        :raises InvalidFileError: The provided path does \
+            not point to a file within the directory.
         '''
-        file_path = self._to_absolute(file_path, replace_sep=False)
+        if not self.path_exists(path):
+            raise _IPE(path=path)
+        if not self.is_file(path):
+            raise _IFE(path=path)
+        
+        path = self._to_absolute(path, replace_sep=False)
         return RemoteFile._create_file(
-            path=file_path,
+            path=path,
             host=self.get_hostname(),
             handler=self._get_handler(),
-            metadata=self._get_metadata_ref(file_path))
+            metadata=self._get_file_metadata_ref(path))
     
 
-    def traverse_files(
-        self,
-        recursively: bool = False
-    ) -> _typ.Iterator[RemoteFile]:
+    def get_subdir(self, path: str) -> 'RemoteDir':
         '''
-        Returns an iterator capable of going through the \
-        dictionaries files as ``File`` instances.
+        Returns the subdirectory residing in the specified \
+        path as a ``RemoteDir`` instance.
 
-        :param bool recursively: Indicates whether the directory \
-            is to be traversed recursively or not. If set to  ``False``, \
-            then only those files that reside directly within the \
-            directory are to be considered. If set to ``True``, \
-            then all files are considered, no matter whether they \
-            reside directly within the directory or within any of \
-            its subdirectories. Defaults to ``False``.
+        :param str path: Either the absolute path or the \
+            path relative to the directory of the subdirectory \
+            in question.
 
-        :note: The resulting iterator may vary depending on the \
-            value of parameter ``recursively``.
+        :raises InvalidPathError: The provided path \
+            does not exist.
+        :raises InvalidDirectoryError: The provided path \
+            does not point to a subdirectory within the \
+            directory.
         '''
-        yield from super().traverse_files(recursively=recursively)
-
+        if not self.path_exists(path):
+            raise _IPE(path=path)
+        if self.is_file(path):
+            raise _IDE(path=path)
+        
+        return self._get_subdir_impl(path)
+    
 
-    def get_files(
-        self,
-        recursively: bool = False,
-        show_abs_path: bool = False
-    ) -> dict[str, RemoteFile]:
+    @classmethod
+    def _create_dir(
+        cls,
+        path: str,
+        host: str,
+        handler: _SSHClientHandler,
+        metadata: dict[str, str]
+    ) -> 'RemoteDir':
         '''
-        Returns a dictionary mapping file paths to ``File`` instances \
-        regarding the files contained within the directory.
+        Creates and returns a ``LocalDir`` instance.
 
-        :param bool recursively: Indicates whether the directory \
-            is to be traversed recursively or not. If set to  ``False``, \
-            then only those files that reside directly within the \
-            directory are to be considered. If set to ``True``, \
-            then all files are considered, no matter whether they \
-            reside directly within the directory or within any of \
-            its subdirectories. Defaults to ``False``.
-        :param bool show_abs_path: Determines whether to include the \
-            files' absolute path or their path relative to this directory. \
-            Defaults to ``False``.
+        :param str path: The path pointing to the directory.
+        :param str host: The name of the host in which \
+            the directory resides.
+        :param SSHClientHandler handler: An ``SSHClientHandler`` \
+            class instance.
+        :param dict[str, str] metadata: A dictionary containing \
+            file metadata.
+        '''
+        instance = cls.__new__(cls)
+        instance.__host = host
+        _Directory.__init__(
+            instance,
+            path=path,
+            metadata=metadata,
+            handler=handler,
+            close_after_use=False)
+        return instance
+    
 
-        :note: The resulting iterator may vary depending on the \
-            value of parameter ``recursively``.
+    def _get_subdir_impl(self, dir_path: str) -> 'RemoteDir':
         '''
-        return super().get_files(
-            recursively=recursively, show_abs_path=show_abs_path)
+        Returns the directory residing in the specified \
+        path as a ``RemoteDir`` instance.
+
+        :param str dir_path: Either the absolute path \
+            or the path relative to the directory of the \
+            subdirectory in question.
+        '''        
+        sep = self._get_separator()
+        dir_path = f"{dir_path.removesuffix(sep)}{sep}"
+        dir_path = self._to_absolute(
+            path=dir_path, replace_sep=False)
+        
+        return __class__._create_dir(
+            path=dir_path,
+            host=self.get_hostname(),
+            handler=self._get_handler(),
+            metadata=self._get_metadata_ref())
     
 
     def __enter__(self) -> 'RemoteDir':
         '''
         Enter the runtime context related to this instance.
         '''
         return super().__enter__()
@@ -1820,17 +2021,19 @@
         to which the provided path points will be automatically created \
         in case it does not already exist, instead of an exception being \
         thrown. Defaults to ``False``.
 
     :raises InvalidPathError: The provided path \
         does not exist.
 
-    :note: The provided path must not begin with a separator.
-        - Wrong: ``/path/to/dir/``
-        - Right: ``path/to/dir/``
+    :note: The provided path must not begin with \
+        a separator.
+            
+            * Wrong: ``/path/to/dir``
+            * Right: ``path/to/dir``
     '''
     def __init__(
         self,
         auth: _AWSAuth,
         bucket: str,
         path: _typ.Optional[str] = None,
         cache: bool = False,
@@ -1854,17 +2057,19 @@
             to which the provided path points will be automatically created \
             in case it does not already exist, instead of an exception being \
             thrown. Defaults to ``False``.
 
         :raises InvalidPathError: The provided path \
             does not exist.
 
-        :note: The provided path must not begin with a separator.
-            - Wrong: ``/path/to/dir/``
-            - Right: ``path/to/dir/``
+        :note: The provided path must not begin with \
+            a separator.
+                
+                * Wrong: ``/path/to/dir``
+                * Right: ``path/to/dir``
         '''
         # Validate path.
         if path is None:
             path = ''
         else:
             sep = _infer_sep(path=path)
             if path.startswith(sep):
@@ -1876,20 +2081,23 @@
             bucket=bucket,
             cache=cache)
 
         super().__init__(
             path=path,
             handler=aws_handler)
 
-        if not aws_handler.dir_exists(path=path):
-            if create_if_missing:
-                aws_handler.mkdir(path=path)
-            else:
-                self.close()
-                raise _IPE(path)
+        # Create directory or throw an exception
+        # depending on the value of "create_if_missing".
+        if path != '':
+            if not aws_handler.dir_exists(path=path):
+                if create_if_missing:
+                    aws_handler.mkdir(path=path)
+                else:
+                    self.close()
+                    raise _IPE(path)
 
 
     def get_bucket_name(self) -> str:
         '''
         Returns the name of the bucket in which \
         the directory resides.
         '''
@@ -1899,77 +2107,121 @@
     def get_uri(self) -> str:
         '''
         Returns the directory's URI.
         '''
         return f"s3://{self.get_bucket_name()}/{self.get_path()}"
     
 
-    def get_file(self, file_path: str) -> AWSS3File:
+    def get_file(self, path: str) -> AWSS3File:
         '''
         Returns the file residing in the specified \
         path as a ``AWSS3File`` instance.
 
-        :param str file_path: Either the absolute path \
-            or the path relative to the directory of the \
-            file in question.
+        :param str path: Either the absolute path or the \
+            path relative to the directory of the file in \
+            question.
+
+        :raises InvalidPathError: The provided path \
+            does not exist.
+        :raises InvalidFileError: The provided path does \
+            not point to a file within the directory.
+
+        :note: The provided path, if absolute, must not \
+            begin with a separator.
+
+                * Wrong: ``/path/to/file.txt``
+                * Right: ``path/to/file.txt``
         '''
-        file_path = self._to_absolute(file_path, replace_sep=False)
+        if not self.path_exists(path):
+            if self._get_handler().dir_exists(
+                self._to_absolute(path, False)
+            ):
+                raise _IFE(path=path)
+            raise _IPE(path=path)
+        
+        path = self._to_absolute(path, replace_sep=False)
         return AWSS3File._create_file(
-            path=file_path,
+            path=path,
             handler=self._get_handler(),
-            metadata=self._get_metadata_ref(file_path))
-
+            metadata=self._get_file_metadata_ref(path))
+    
 
-    def traverse_files(
-        self,
-        recursively: bool = False
-    ) -> _typ.Iterator[AWSS3File]:
+    def get_subdir(self, path: str) -> 'AWSS3Dir':
         '''
-        Returns an iterator capable of going through the \
-        dictionaries files as ``File`` instances.
+        Returns the directory residing in the specified \
+        path as an ``AWSS3Dir`` instance.
 
-        :param bool recursively: Indicates whether the directory \
-            is to be traversed recursively or not. If set to  ``False``, \
-            then only those files that reside directly within the \
-            directory are to be considered. If set to ``True``, \
-            then all files are considered, no matter whether they \
-            reside directly within the directory or within any of \
-            its subdirectories. Defaults to ``False``.
+        :param str path: Either the absolute path or the \
+            path relative to the directory of the subdirectory \
+            in question.
 
-        :note: The resulting iterator may vary depending on the \
-            value of parameter ``recursively``.
+        :raises InvalidPathError: The provided path \
+            does not exist.
+
+        :note: The provided path, if absolute, must not \
+            begin with a separator.
+
+                * Wrong: ``/path/to/dir``
+                * Right: ``path/to/dir``
         '''
-        yield from super().traverse_files(recursively=recursively)
+        sep = self._get_separator()
+        path = f"{path.removesuffix(sep)}{sep}"
+        abs_path = self._to_absolute(
+            path=path, replace_sep=False)
+
+        if not self._get_handler().dir_exists(abs_path):
+            raise _IPE(path=path)
+        
+        return self._get_subdir_impl(path)
 
 
-    def get_files(
-        self,
-        recursively: bool = False,
-        show_abs_path: bool = False
-    ) -> dict[str, AWSS3File]:
+    @classmethod
+    def _create_dir(
+        cls,
+        path: str,
+        handler: _AWSClientHandler,
+        metadata: dict[str, str]
+    ) -> 'AWSS3Dir':
         '''
-        Returns a dictionary mapping file paths to ``File`` instances \
-        regarding the files contained within the directory.
+        Creates and returns an ``AWSS3Dir`` instance.
 
-        :param bool recursively: Indicates whether the directory \
-            is to be traversed recursively or not. If set to  ``False``, \
-            then only those files that reside directly within the \
-            directory are to be considered. If set to ``True``, \
-            then all files are considered, no matter whether they \
-            reside directly within the directory or within any of \
-            its subdirectories. Defaults to ``False``.
-        :param bool show_abs_path: Determines whether to include the \
-            files' absolute path or their path relative to this directory. \
-            Defaults to ``False``.
+        :param str path: The path pointing to the directory.
+        :param AWSClientHandler handler: An ``AWSClientHandler`` \
+            class instance.
+        :param dict[str, str] metadata: A dictionary containing \
+            file metadata.
+        '''
+        instance = cls.__new__(cls)
+        _Directory.__init__(
+            instance,
+            path=path,
+            metadata=metadata,
+            handler=handler,
+            close_after_use=False)
+        return instance
+    
 
-        :note: The resulting iterator may vary depending on the \
-            value of parameter ``recursively``.
+    def _get_subdir_impl(self, dir_path: str) -> 'AWSS3Dir':
+        '''
+        Returns the directory residing in the specified \
+        path as an ``AWSS3Dir`` instance.
+
+        :param str dir_path: Either the absolute path \
+            or the path relative to the directory of the \
+            subdirectory in question.
         '''
-        return super().get_files(
-            recursively=recursively, show_abs_path=show_abs_path)
+        sep = self._get_separator()
+        dir_path = f"{dir_path.removesuffix(sep)}{sep}"
+        abs_dir_path = self._to_absolute(
+            path=dir_path, replace_sep=False)
+        
+        return __class__._create_dir(
+            path=abs_dir_path,
+            handler=self._get_handler(),
+            metadata=self._get_metadata_ref())
     
 
     def __enter__(self) -> 'AWSS3Dir':
         '''
         Enter the runtime context related to this instance.
         '''
         return super().__enter__()
@@ -1993,20 +2245,20 @@
     :param bool create_if_missing: If set to ``True``, then the directory \
         to which the provided path points will be automatically created \
         in case it does not already exist, instead of an exception being \
         thrown. Defaults to ``False``.
 
     :raises InvalidPathError: The provided path \
         does not exist.
-    :raises InvalidDirectoryError: The provided path \
-        does not point to a directory.
 
-    :note: The provided path must not begin with a separator.
-        - Wrong: ``/path/to/dir/``
-        - Right: ``path/to/dir/``
+    :note: The provided path must not begin with \
+        a separator.
+            
+            * Wrong: ``/path/to/dir``
+            * Right: ``path/to/dir``
     '''
     def __init__(
         self,
         auth: _AzureAuth,
         container: str,
         path: _typ.Optional[str] = None,
         cache: bool = False,
@@ -2032,21 +2284,23 @@
             thrown. Defaults to ``False``.
 
         :raises InvalidPathError: The provided path \
             does not exist.
         :raises InvalidDirectoryError: The provided path \
             does not point to a directory.
 
-        :note: The provided path must not begin with a separator.
-            - Wrong: ``/path/to/dir/``
-            - Right: ``path/to/dir/``
+        :note: The provided path must not begin with \
+            a separator.
+                
+                * Wrong: ``/path/to/dir``
+                * Right: ``path/to/dir``
         '''        
         # Validate path.
         if path is None:
-            path = '/'
+            path = ''
         else:
             sep = _infer_sep(path=path)
             if path.startswith(sep):
                 raise _IPE(path=path)
             
         # Instantiate a connection handler.
         azr_handler = _AzureClientHandler(
@@ -2064,20 +2318,21 @@
         # Throw an exception if container does not exist.
         if not azr_handler.container_exists():
             self.close()
             raise _ABCNFE(container)
 
         # Create directory or throw an exception
         # depending on the value of "create_if_missing".
-        if not azr_handler.path_exists(path=path):
-            if create_if_missing:
-                azr_handler.mkdir(path=path)
-            else:
-                self.close()
-                raise _IPE(path)
+        if path != '':
+            if not azr_handler.path_exists(path=path):
+                if create_if_missing:
+                    azr_handler.mkdir(path=path)
+                else:
+                    self.close()
+                    raise _IPE(path)
 
 
     def get_container_name(self) -> str:
         '''
         Returns the name of the bucket in which \
         the directory resides.
         '''
@@ -2089,77 +2344,126 @@
         Returns the directory's URI.
         '''
         uri = f"abfss://{self.get_container_name()}@{self.__storage_account}"
         uri += f".dfs.core.windows.net/{self.get_path()}"
         return uri
     
 
-    def get_file(self, file_path: str) -> AzureBlobFile:
+    def get_file(self, path: str) -> AzureBlobFile:
         '''
         Returns the file residing in the specified \
         path as a ``AzureBlobFile`` instance.
 
-        :param str file_path: Either the absolute path \
-            or the path relative to the directory of the \
-            file in question.
+        :param str path: Either the absolute path or the \
+            path relative to the directory of the file in \
+            question.
+
+        :raises InvalidPathError: The provided path \
+            does not exist.
+        :raises InvalidFileError: The provided path does \
+            not point to a file within the directory.
+
+        :note: The provided path, if absolute, must not \
+            begin with a separator.
+
+                * Wrong: ``/path/to/file.txt``
+                * Right: ``path/to/file.txt``
         '''
-        file_path = self._to_absolute(file_path, replace_sep=False)
+
+        if not self.path_exists(path):
+            raise _IPE(path=path)
+        if not self.is_file(path):
+            raise _IFE(path=path)
+        
+        path = self._to_absolute(path, replace_sep=False)
         return AzureBlobFile._create_file(
-            path=file_path,
+            path=path,
+            storage_account=self.__storage_account,
             handler=self._get_handler(),
-            metadata=self._get_metadata_ref(file_path))
+            metadata=self._get_file_metadata_ref(path))
     
 
-    def traverse_files(
-        self,
-        recursively: bool = False
-    ) -> _typ.Iterator[AzureBlobFile]:
+    def get_subdir(self, path: str) -> 'AzureBlobDir':
         '''
-        Returns an iterator capable of going through the \
-        dictionaries files as ``File`` instances.
+        Returns the directory residing in the specified \
+        path as an ``AzureBlobDir`` instance.
 
-        :param bool recursively: Indicates whether the directory \
-            is to be traversed recursively or not. If set to  ``False``, \
-            then only those files that reside directly within the \
-            directory are to be considered. If set to ``True``, \
-            then all files are considered, no matter whether they \
-            reside directly within the directory or within any of \
-            its subdirectories. Defaults to ``False``.
+        :param str path: Either the absolute path or the \
+            path relative to the directory of the subdirectory \
+            in question.
 
-        :note: The resulting iterator may vary depending on the \
-            value of parameter ``recursively``.
-        '''
-        yield from super().traverse_files(recursively=recursively)
+        :raises InvalidPathError: The provided path \
+            does not exist.
 
+        :note: The provided path, if absolute, must not \
+            begin with a separator.
 
-    def get_files(
-        self,
-        recursively: bool = False,
-        show_abs_path: bool = False
-    ) -> dict[str, AzureBlobFile]:
+                * Wrong: ``/path/to/dir``
+                * Right: ``path/to/dir``
         '''
-        Returns a dictionary mapping file paths to ``File`` instances \
-        regarding the files contained within the directory.
+        sep = self._get_separator()
+        path = f"{path.removesuffix(sep)}{sep}"
 
-        :param bool recursively: Indicates whether the directory \
-            is to be traversed recursively or not. If set to  ``False``, \
-            then only those files that reside directly within the \
-            directory are to be considered. If set to ``True``, \
-            then all files are considered, no matter whether they \
-            reside directly within the directory or within any of \
-            its subdirectories. Defaults to ``False``.
-        :param bool show_abs_path: Determines whether to include the \
-            files' absolute path or their path relative to this directory. \
-            Defaults to ``False``.
+        if not self.path_exists(path):
+            raise _IPE(path=path)
+        
+        return self._get_subdir_impl(path)
+    
 
-        :note: The resulting iterator may vary depending on the \
-            value of parameter ``recursively``.
+    @classmethod
+    def _create_dir(
+        cls,
+        path: str,
+        storage_account: str,
+        handler: _AzureClientHandler,
+        metadata: dict[str, str]
+    ) -> 'AzureBlobDir':
+        '''
+        Creates and returns an ``AzureBlobDir`` instance.
+
+        :param str path: The path pointing to the directory.
+        :param str storage_account: The name of the storage \
+            account to which the blob directory's container \
+            belongs.
+        :param AzureClientHandler handler: An ``AzureClientHandler`` \
+            class instance.
+        :param dict[str, str] metadata: A dictionary containing \
+            file metadata.
         '''
-        return super().get_files(
-            recursively=recursively, show_abs_path=show_abs_path)
+        instance = cls.__new__(cls)
+        instance.__storage_account = storage_account
+        _Directory.__init__(
+            instance,
+            path=path,
+            metadata=metadata,
+            handler=handler,
+            close_after_use=False)
+        return instance
     
+
+    def _get_subdir_impl(self, dir_path: str) -> 'AzureBlobDir':
+        '''
+        Returns the directory residing in the specified \
+        path as an ``AzureBlobDir`` instance.
+
+        :param str dir_path: Either the absolute path \
+            or the path relative to the directory of the \
+            subdirectory in question.
+        '''
+        sep = self._get_separator()
+        dir_path = f"{dir_path.removesuffix(sep)}{sep}"
+        
+        dir_path = self._to_absolute(
+            path=dir_path, replace_sep=False)
+        
+        return __class__._create_dir(
+            path=dir_path,
+            storage_account=self.__storage_account,
+            handler=self._get_handler(),
+            metadata=self._get_metadata_ref())
+
     
     def __enter__(self) -> 'AzureBlobDir':
         '''
         Enter the runtime context related to this instance.
         '''
         return super().__enter__()
```

### Comparing `fluke-api-0.2.0/fluke_api.egg-info/PKG-INFO` & `fluke-api-0.3.0/fluke_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluke-api
-Version: 0.2.0
+Version: 0.3.0
 Summary: Move your data around
 Author: Manos Stoumpos
 Author-email: manosstoumpos@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/manoss96/fluke
 Project-URL: Bug Tracker, https://github.com/manoss96/fluke/issues
 Project-URL: Documentation, https://fluke.rtfd.io
```

### Comparing `fluke-api-0.2.0/pyproject.toml` & `fluke-api-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fluke-api"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   {email = "manosstoumpos@gmail.com"},
   {name = "Manos Stoumpos"}
 ]
 description = "Move your data around"
 keywords = ["data", "transfer", "file", "filesystem", "cloud"]
 readme = "README.md"
```

### Comparing `fluke-api-0.2.0/tests/test_auth.py` & `fluke-api-0.3.0/tests/test_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from unittest import TestCase
-
+import unittest
 
 from fluke.auth import RemoteAuth, AWSAuth, AzureAuth
 
 
-class TestRemoteAuth(TestCase):
+class TestRemoteAuth(unittest.TestCase):
 
     HOST = "HOST"
     USERNAME = "USERNAME"
     PASSWORD = "PASSWORD"
     PKEY = "PATH/TO/PKEY"
     PASSPHRASE = "PASSPHRASE"
     PORT = 22
@@ -64,15 +63,15 @@
             'key_type': credentials['key_type'].value
         })
         self.assertEqual(
             auth.get_credentials(),
             credentials)
         
 
-class TestAWSAuth(TestCase):
+class TestAWSAuth(unittest.TestCase):
 
     AWS_ACCESS_KEY_ID = "AWS_ACCESS_KEY_ID"
     AWS_SECRET_ACCESS_KEY = "AWS_SECRET_ACCESS_KEY"
     AWS_SESSION_TOKEN = "AWS_SESSION_TOKEN"
     REGION = AWSAuth.Region.EUROPE_WEST_1
 
     def test_get_credentials(self):
@@ -85,15 +84,15 @@
         auth = AWSAuth(**credentials)
         credentials.update({'region_name': credentials.pop('region').value})
         self.assertEqual(
             auth.get_credentials(),
             credentials)
         
 
-class TestAzureAuth(TestCase):
+class TestAzureAuth(unittest.TestCase):
 
     ACCOUNT_URL = "ACCOUNT_URL"
     TENANT_ID = "TENANT_ID"
     CLIENT_ID = "CLIENT_ID"
     CLIENT_SECRET = "CLIENT_SECRET"
     CONNECTION_STRING = "CONNECTION_STRING"
 
@@ -108,8 +107,12 @@
             AzureAuth(**credentials).get_credentials(),
             credentials)
         
     def test_from_connection_string(self):
         credentials = { 'conn_string': self.CONNECTION_STRING }
         self.assertEqual(
             AzureAuth.from_conn_string(**credentials).get_credentials(),
-            credentials)
+            credentials)
+        
+
+if __name__=="__main__": 
+     unittest.main()
```

### Comparing `fluke-api-0.2.0/tests/test_storage.py` & `fluke-api-0.3.0/tests/test_storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,14 +107,19 @@
         for file in sorted(fn):
             file_path = join_paths(dp.replace(os.sep, SEPARATOR), file)
             with open(file_path, "rb") as file:
                 bucket.upload_fileobj(
                     Key=file_path.replace(os.sep, SEPARATOR),
                     Fileobj=file,
                     ExtraArgs={ "Metadata": metadata })
+    # Finally, create a TMP dir.
+    with io.BytesIO() as empty_buffer:
+        bucket.upload_fileobj(
+            Key=join_paths(TEST_FILES_DIR, TMP_DIR_NAME, 'DUMMY'),
+            Fileobj=empty_buffer)
 
         
 def get_aws_s3_object(bucket_name: str, path: str):
     '''
     Returns an object within an Amazon S3 bucket.
 
     :param str bucket_name: The name of the Amazon S3 bucket.
@@ -155,16 +160,28 @@
 '''
 DIR_NAME = "dir"
 REL_DIR_PATH = f"{TEST_FILES_DIR}{SEPARATOR}{DIR_NAME}{SEPARATOR}"
 ABS_DIR_PATH = to_abs(REL_DIR_PATH)
 DIR_FILE_NAME = "file2.txt"
 REL_DIR_FILE_PATH = f"{REL_DIR_PATH}{DIR_FILE_NAME}"
 ABS_DIR_FILE_PATH = to_abs(REL_DIR_FILE_PATH)
-CONTENTS = [DIR_FILE_NAME, f'subdir{SEPARATOR}']
-RECURSIVE_CONTENTS = [DIR_FILE_NAME, f'subdir{SEPARATOR}file3.txt', f'subdir{SEPARATOR}file4.txt']
+DIR_SUBDIR_NAME = f"subdir{SEPARATOR}"
+REL_DIR_SUBDIR_PATH = f"{REL_DIR_PATH}{DIR_SUBDIR_NAME}"
+ABS_DIR_SUBDIR_PATH = to_abs(REL_DIR_SUBDIR_PATH)
+DIR_SUBDIR_FILE_NAME = "file3.txt"
+REL_DIR_SUBDIR_FILE_PATH = f"{REL_DIR_SUBDIR_PATH}{DIR_SUBDIR_FILE_NAME}"
+ABS_DIR_SUBDIR_FILE_PATH = to_abs(REL_DIR_SUBDIR_FILE_PATH)
+CONTENTS = [DIR_FILE_NAME, DIR_SUBDIR_NAME]
+RECURSIVE_CONTENTS = [
+    DIR_FILE_NAME,
+    f'{DIR_SUBDIR_NAME}{DIR_SUBDIR_FILE_NAME}',
+    f'{DIR_SUBDIR_NAME}file4.txt']
+TMP_DIR_NAME = 'TMP_DIR'
+
+
 def get_abs_contents(recursively: bool):
     return [
         join_paths(ABS_DIR_PATH, p) for p in (
             RECURSIVE_CONTENTS if recursively else CONTENTS
         )
     ]
 
@@ -188,14 +205,40 @@
 
 
 '''
 Helper Mock Classes
 '''
 class MockSFTPClient():
 
+    class MockSFTPFile():
+
+        def __init__(self, filename: str, mode: str) -> None:
+            self.__file = open(file=filename, mode=mode)
+
+        def seek(self, offset: int) -> None:
+            self.__file.seek(offset)
+
+        def tell(self) -> int:
+            return self.__file.tell()
+
+        def read(self, size: Optional[int] = None) -> None:
+            if size is None:
+                return self.__file.read()
+            return self.__file.read(size)
+        
+        def write(self, chunk: bytes) -> None:
+            self.__file.write(chunk)
+        
+        def flush(self) -> None:
+            self.__file.flush()
+
+        def close(self):
+            self.__file.close()
+            
+
     @staticmethod
     def get_mock_methods() -> dict[str, Mock]:
         '''
         Returns a dictionary containing all the \
         methods that are to be mocked.
         '''
         return {
@@ -224,23 +267,16 @@
         os.makedirs(name=path)
 
     @simulate_latency
     def listdir_attr(self, path: str) -> list[paramiko.SFTPAttributes]:
         return [self.stat(join_paths(path, f)) for f in sorted(os.listdir(path=path))]
     
     @simulate_latency
-    def getfo(self, remotepath, fl, callback=None, prefetch=True):
-        with open(remotepath, "rb") as fr:
-            fl.write(fr.read())
-            return fr.tell()
-        
-    @simulate_latency
-    def putfo(self, fl, remotepath, file_size=0, callback=None, confirm=True):
-        with open(remotepath, "wb") as fr:
-            fr.write(fl.read())
+    def open(self, filename: str, mode: str) -> MockSFTPFile:
+        return MockSFTPClient.MockSFTPFile(filename, mode)
 
     @simulate_latency
     def close(self):
         pass
 
 
 class MockContainerClient():
@@ -257,45 +293,105 @@
                 return self.name
             elif item == 'size':
                 return self.size
             raise ValueError()
 
     class MockStreamStorageDownloader():
 
-        def __init__(self, name: str, metadata: dict[str, str], size: int):
+        def __init__(
+            self, name: str,
+            metadata: dict[str, str],
+            size: int,
+            offset: Optional[int] = None,
+            length: Optional[int] = None
+        ):
             self.name = name
             self.size = size
             self.properties = MockContainerClient.MockBlobProperties(
                 name=name,
                 metadata=metadata,
                 size=size)
+            self.offset = offset
+            self.length = length
 
         @simulate_latency
-        def readinto(self, stream: io.BytesIO):
+        def read(self):
             with open(file=self.name, mode="rb") as file:
-                stream.write(file.read())
+                if self.offset is not None:
+                    file.seek(self.offset)
+                if self.length is None:
+                    return file.read()
+                return file.read(self.length)
 
     class MockBlobClient():
 
         def __init__(self, blob_name: str):
             self.blob_name: str = blob_name
+            self.metadata = {}
 
         @simulate_latency
         def exists(self) -> bool:
             return self.blob_name == '' or os.path.exists(self.blob_name)
 
         @simulate_latency  
         def create_append_blob(self):
-            os.makedirs(join_paths(*self.blob_name.split(SEPARATOR)[:-1]))
+            os.makedirs(join_paths(*self.blob_name.split(SEPARATOR)[:-1]), exist_ok=True)
             with (
                 open(file=self.blob_name, mode='wb') as file,
                 io.BytesIO() as empty_buffer
             ):
                 file.write(empty_buffer.read())
 
+        def set_blob_metadata(self, metadata: dict[str, str]) -> None:
+            self.metadata = metadata
+
+        @simulate_latency    
+        def download_blob(
+            self,
+            offset: Optional[int] = None,
+            length: Optional[int] = None
+        ):
+            file_path = to_abs(self.blob_name)
+            return MockContainerClient.MockStreamStorageDownloader(
+                name=file_path,
+                metadata=self.metadata,
+                size=os.stat(file_path).st_size,
+                offset=offset,
+                length=length)
+        
+        @simulate_latency   
+        def upload_blob(
+            self,
+            data: bytes,
+            length: int,
+            metadata: Optional[dict[str, str]],
+            overwrite: bool
+        ):
+            name = self.blob_name
+            # Raise error if file exists and overwrite
+            # has not been set to True.
+            if os.path.exists(name) and not overwrite:
+                raise OverwriteError(file_path=name)
+            # Write contents to file.
+            with open(file=name, mode="wb") as file:
+                file.write(data)
+            # Store metadata if not None.
+            if metadata is not None:
+                self.metadata = metadata
+
+        @simulate_latency
+        def append_block(
+            self,
+            data: bytes,
+            length: int
+        ):
+            # Write contents to file.
+            with open(file=self.blob_name, mode="ab") as file:
+                file.write(data)
+
         @simulate_latency
         def delete_blob(self):
             os.remove(self.blob_name)
 
         @simulate_latency
         def close(self):
             pass
@@ -387,40 +483,21 @@
                         None if obj_name.endswith(SEPARATOR)
                         else self.metadata[obj_name]
                     ),
                     size=os.stat(file_path).st_size) 
         else:
             raise ValueError()
                 
-
     @simulate_latency    
     def download_blob(self, blob: str):
         file_path = to_abs(blob)
         return MockContainerClient.MockStreamStorageDownloader(
             name=blob,
             metadata=self.metadata[blob],
             size=os.stat(file_path).st_size)
-    
-    @simulate_latency   
-    def upload_blob(
-        self,
-        name: str,
-        data: io.BytesIO,
-        metadata: Optional[dict[str, str]],
-        overwrite: bool
-    ):
-        # Raise error if file exists and overwrite
-        # has not been set to True.
-        if os.path.exists(name) and not overwrite:
-            raise OverwriteError(file_path=name)
-        # Update metadata.
-        self.metadata.update({name: metadata})
-        # Write contents to file.
-        with open(file=name, mode="wb") as file:
-            file.write(data.read())
 
     @simulate_latency
     def close(self):
         pass
 
 
 class TestLocalFile(unittest.TestCase):
@@ -445,15 +522,15 @@
 
     def test_get_name(self):
         file = self.build_file()
         self.assertEqual(file.get_name(), FILE_NAME)
 
     def test_get_uri(self):
         file = self.build_file()
-        self.assertEqual(file.get_uri(), f"file:///{ABS_FILE_PATH.lstrip(SEPARATOR)}")
+        self.assertEqual(file.get_uri(), f"file:///{ABS_FILE_PATH.removeprefix(SEPARATOR)}")
 
     def test_get_metadata(self):
         file = self.build_file()
         self.assertEqual(file.get_metadata(), {})
 
     def test_set_and_get_metadata(self):
         file = self.build_file()
@@ -475,43 +552,110 @@
         file = self.build_file()
         self.assertEqual(file.get_size(), 4)
 
     def test_read(self):
         file = self.build_file()
         self.assertEqual(file.read(), b"TEXT")
 
+    def test_read_chunks(self):
+        file = self.build_file()
+        data, chunk_size = b"TEXT", 1
+        with io.BytesIO(data) as buffer:
+            for chunk in file.read_chunks(chunk_size):
+                self.assertEqual(chunk, buffer.read(chunk_size))
+
+    def test_read_range(self):
+        file = self.build_file()
+        data, start, end = b"EX", 1, 3
+        self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_range_on_start_is_none(self):
+        file = self.build_file()
+        data, start, end = b"TE", None, 2
+        self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_range_on_end_is_none(self):
+        file = self.build_file()
+        data, start, end = b"XT", 2, None
+        self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_range_on_start_greater_than_end(self):
+        file = self.build_file()
+        data, start, end = b"", 100, 1
+        self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_text(self):
+        file = self.build_file()
+        data = "TEXT"
+        self.assertEqual(data, file.read_text())
+
+    def test_read_lines(self):
+        file = self.build_file()
+        data = "TEXT"
+        for line in file.read_lines():
+            self.assertEqual(data, line)
+
+    def test_read_lines_on_chunk_size(self):
+        file = self.build_file()
+        data = "TEXT"
+        for line in file.read_lines(chunk_size=1):
+            self.assertEqual(data, line)
+
     def test_transfer_to(self):
         file = self.build_file()
         dir = TestLocalDir.build_dir(path=ABS_DIR_PATH)
 
         # Copy file into dir.
         file.transfer_to(dst=dir)
         
         # Confirm that file was indeed copied.
         copy_path = join_paths(ABS_DIR_PATH, FILE_NAME)
-        self.assertTrue(os.path.exists(copy_path))
+
+        with (
+            open(ABS_FILE_PATH, mode='rb') as file,
+            open(copy_path, mode='rb') as copy
+        ):
+            self.assertEqual(file.read(), copy.read())
+
+        # Remove copy of the file.
+        os.remove(copy_path)
+
+    def test_transfer_to_on_chunk_size(self):
+        file = self.build_file()
+        dir = TestLocalDir.build_dir(path=ABS_DIR_PATH)
+
+        # Copy file into dir.
+        file.transfer_to(dst=dir, chunk_size=1)
+        
+        # Confirm that file was indeed copied.
+        copy_path = join_paths(ABS_DIR_PATH, FILE_NAME)
+
+        with (
+            open(ABS_FILE_PATH, mode='rb') as file,
+            open(copy_path, mode='rb') as copy
+        ):
+            self.assertEqual(file.read(), copy.read())
 
         # Remove copy of the file.
         os.remove(copy_path)
 
     def test_transfer_to_on_overwrite_error(self):
         file = self.build_file()
         dir = TestLocalDir.build_dir(path=ABS_DIR_PATH)
 
         # Copy file into dir.
         file.transfer_to(dst=dir)
         # Ensure OverwriteError is raised when trying
         # to copy file a second time.
-        self.assertRaises(OverwriteError, file.transfer_to, dst=dir)
+        self.assertFalse(file.transfer_to(dst=dir))
         
         # Remove copy of the file.
         copy_path = join_paths(ABS_DIR_PATH, FILE_NAME)
         os.remove(copy_path)
 
-
 class TestRemoteFile(unittest.TestCase):
 
     @staticmethod
     def build_file(path: str = ABS_FILE_PATH, cache: bool = False) -> RemoteFile:
         return RemoteFile(**{
             'auth': get_remote_auth_instance(hostname=HOST),
             'path': path,
@@ -541,15 +685,15 @@
 
     def test_get_hostname(self):
         with self.build_file() as file:
             self.assertEqual(file.get_hostname(), HOST)
 
     def test_get_uri(self):
         with self.build_file() as file:
-            self.assertEqual(file.get_uri(), f"sftp://{HOST}/{ABS_FILE_PATH.lstrip(os.sep)}")
+            self.assertEqual(file.get_uri(), f"sftp://{HOST}/{ABS_FILE_PATH.removeprefix(os.sep)}")
 
     def test_get_metadata(self):
         with self.build_file() as file:
             self.assertEqual(file.get_metadata(), {})
 
     def test_set_and_get_metadata(self):
         with self.build_file() as file:
@@ -571,32 +715,98 @@
         with self.build_file() as file:
             self.assertEqual(file.get_size(), 4)
 
     def test_read(self):
         with self.build_file() as file:
             self.assertEqual(file.read(), b"TEXT")
 
+    def test_read_chunks(self):
+        data, chunk_size = b"TEXT", 1
+        with (
+            self.build_file() as file,
+            io.BytesIO(data) as buffer
+        ):
+            for chunk in file.read_chunks(chunk_size):
+                self.assertEqual(chunk, buffer.read(chunk_size))
+
+    def test_read_range(self):
+        data, start, end = b"EX", 1, 3
+        with self.build_file() as file:
+            self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_range_on_start_is_none(self):
+        with self.build_file() as file:
+            data, start, end = b"TE", None, 2
+            self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_range_on_end_is_none(self):
+        with self.build_file() as file:
+            data, start, end = b"XT", 2, None
+            self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_range_on_start_greater_than_end(self):
+        with self.build_file() as file:
+            data, start, end = b"", 100, 1
+            self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_text(self):
+        with self.build_file() as file:
+            data = "TEXT"
+            self.assertEqual(data, file.read_text())
+
+    def test_read_lines(self):
+        with self.build_file() as file:
+            data = "TEXT"
+            for line in file.read_lines():
+                self.assertEqual(data, line)
+
+    def test_read_lines_on_chunk_size(self):
+        with self.build_file() as file:
+            data = "TEXT"
+            for line in file.read_lines(chunk_size=1):
+                self.assertEqual(data, line)
+
     def test_transfer_to(self):
         with self.build_file() as file:
             # Copy file into dir.
             file.transfer_to(dst=TestLocalDir.build_dir(path=ABS_DIR_PATH))
             # Confirm that file was indeed copied.
             copy_path = join_paths(ABS_DIR_PATH, FILE_NAME)
-            self.assertTrue(os.path.exists(copy_path))
+            with (
+                open(ABS_FILE_PATH, mode='rb') as file,
+                open(copy_path, mode='rb') as copy
+            ):
+                self.assertEqual(file.read(), copy.read())
+            # Remove copy of the file.
+            os.remove(copy_path)
+
+    def test_transfer_to_on_chunk_size(self):
+        with self.build_file() as file:
+            # Copy file into dir.
+            file.transfer_to(
+                dst=TestLocalDir.build_dir(path=ABS_DIR_PATH),
+                chunk_size=1)
+            # Confirm that file was indeed copied.
+            copy_path = join_paths(ABS_DIR_PATH, FILE_NAME)
+            with (
+                open(ABS_FILE_PATH, mode='rb') as file,
+                open(copy_path, mode='rb') as copy
+            ):
+                self.assertEqual(file.read(), copy.read())
             # Remove copy of the file.
             os.remove(copy_path)
 
     def test_transfer_to_on_overwrite_error(self):
         with self.build_file() as file:
             dir = TestLocalDir.build_dir(path=ABS_DIR_PATH)
             # Copy file into dir.
             file.transfer_to(dst=dir)
             # Ensure OverwriteError is raised when trying
             # to copy file a second time.
-            self.assertRaises(OverwriteError, file.transfer_to, dst=dir)
+            self.assertFalse(file.transfer_to(dst=dir))
             # Remove copy of the file.
             copy_path = join_paths(ABS_DIR_PATH, FILE_NAME)
             os.remove(copy_path)
 
     def test_transfer_to_on_include_metadata_set_to_false(self):
         with (
             mock_s3() as mocks3,
@@ -821,32 +1031,98 @@
         with self.build_file() as file:
             self.assertEqual(file.get_size(), 4)
 
     def test_read(self):
         with self.build_file() as file:
             self.assertEqual(file.read(), b"TEXT")
 
+    def test_read_chunks(self):
+        data, chunk_size = b"TEXT", 1
+        with (
+            self.build_file() as file,
+            io.BytesIO(data) as buffer
+        ):
+            for chunk in file.read_chunks(chunk_size):
+                self.assertEqual(chunk, buffer.read(chunk_size))
+
+    def test_read_range(self):
+        data, start, end = b"EX", 1, 3
+        with self.build_file() as file:
+            self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_range_on_start_is_none(self):
+        with self.build_file() as file:
+            data, start, end = b"TE", None, 2
+            self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_range_on_end_is_none(self):
+        with self.build_file() as file:
+            data, start, end = b"XT", 2, None
+            self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_range_on_start_greater_than_end(self):
+        with self.build_file() as file:
+            data, start, end = b"", 100, 1
+            self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_text(self):
+        with self.build_file() as file:
+            data = "TEXT"
+            self.assertEqual(data, file.read_text())
+
+    def test_read_lines(self):
+        with self.build_file() as file:
+            data = "TEXT"
+            for line in file.read_lines():
+                self.assertEqual(data, line)
+
+    def test_read_lines_on_chunk_size(self):
+        with self.build_file() as file:
+            data = "TEXT"
+            for line in file.read_lines(chunk_size=1):
+                self.assertEqual(data, line)
+
     def test_transfer_to(self):
         with self.build_file() as file:
             # Copy file into dir.
             file.transfer_to(dst=TestLocalDir.build_dir(path=ABS_DIR_PATH))
             # Confirm that file was indeed copied.
             copy_path = join_paths(ABS_DIR_PATH, FILE_NAME)
-            self.assertTrue(os.path.exists(copy_path))
+            with (
+                open(ABS_FILE_PATH, mode='rb') as file,
+                open(copy_path, mode='rb') as copy
+            ):
+                self.assertEqual(file.read(), copy.read())
+            # Remove copy of the file.
+            os.remove(copy_path)
+
+    def test_transfer_to_on_chunk_size(self):
+        with self.build_file() as file:
+            # Copy file into dir.
+            file.transfer_to(
+                dst=TestLocalDir.build_dir(path=ABS_DIR_PATH),
+                chunk_size=1)
+            # Confirm that file was indeed copied.
+            copy_path = join_paths(ABS_DIR_PATH, FILE_NAME)
+            with (
+                open(ABS_FILE_PATH, mode='rb') as file,
+                open(copy_path, mode='rb') as copy
+            ):
+                self.assertEqual(file.read(), copy.read())
             # Remove copy of the file.
             os.remove(copy_path)
 
     def test_transfer_to_on_overwrite_error(self):
         with self.build_file() as file:
             dir = TestLocalDir.build_dir(path=ABS_DIR_PATH)
             # Copy file into dir.
             file.transfer_to(dst=dir)
             # Ensure OverwriteError is raised when trying
             # to copy file a second time.
-            self.assertRaises(OverwriteError, file.transfer_to, dst=dir)
+            self.assertFalse(file.transfer_to(dst=dir))
             # Remove copy of the file.
             copy_path = join_paths(ABS_DIR_PATH, FILE_NAME)
             os.remove(copy_path)
 
     def test_transfer_to_on_include_metadata_set_to_false(self):
         with self.build_file() as file:
             dir_path = REL_DIR_PATH
@@ -1055,37 +1331,102 @@
             file.set_metadata(new_metadata)
             self.assertEqual(file.get_metadata(), new_metadata)
 
     def test_get_size(self):
         with self.build_file() as file:
             self.assertEqual(file.get_size(), 4)
 
-
     def test_read(self):
         with self.build_file() as file:
             self.assertEqual(file.read(), b"TEXT")
 
+    def test_read_chunks(self):
+        data, chunk_size = b"TEXT", 1
+        with (
+            self.build_file() as file,
+            io.BytesIO(data) as buffer
+        ):
+            for chunk in file.read_chunks(chunk_size):
+                self.assertEqual(chunk, buffer.read(chunk_size))
+
+    def test_read_range(self):
+        data, start, end = b"EX", 1, 3
+        with self.build_file() as file:
+            self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_range_on_start_is_none(self):
+        with self.build_file() as file:
+            data, start, end = b"TE", None, 2
+            self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_range_on_end_is_none(self):
+        with self.build_file() as file:
+            data, start, end = b"XT", 2, None
+            self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_range_on_start_greater_than_end(self):
+        with self.build_file() as file:
+            data, start, end = b"", 100, 1
+            self.assertEqual(data, file.read_range(start, end))
+
+    def test_read_text(self):
+        with self.build_file() as file:
+            data = "TEXT"
+            self.assertEqual(data, file.read_text())
+
+    def test_read_lines(self):
+        with self.build_file() as file:
+            data = "TEXT"
+            for line in file.read_lines():
+                self.assertEqual(data, line)
+
+    def test_read_lines_on_chunk_size(self):
+        with self.build_file() as file:
+            data = "TEXT"
+            for line in file.read_lines(chunk_size=1):
+                self.assertEqual(data, line)
+
     def test_transfer_to(self):
         with self.build_file() as file:
             # Copy file into dir.
             file.transfer_to(dst=TestLocalDir.build_dir(path=ABS_DIR_PATH))
             # Confirm that file was indeed copied.
             copy_path = join_paths(ABS_DIR_PATH, FILE_NAME)
-            self.assertTrue(os.path.exists(copy_path))
+            with (
+                open(ABS_FILE_PATH, mode='rb') as file,
+                open(copy_path, mode='rb') as copy
+            ):
+                self.assertEqual(file.read(), copy.read())
+            # Remove copy of the file.
+            os.remove(copy_path)
+
+    def test_transfer_to_on_chunk_size(self):
+        with self.build_file() as file:
+            # Copy file into dir.
+            file.transfer_to(
+                dst=TestLocalDir.build_dir(path=ABS_DIR_PATH),
+                chunk_size=1)
+            # Confirm that file was indeed copied.
+            copy_path = join_paths(ABS_DIR_PATH, FILE_NAME)
+            with (
+                open(ABS_FILE_PATH, mode='rb') as file,
+                open(copy_path, mode='rb') as copy
+            ):
+                self.assertEqual(file.read(), copy.read())
             # Remove copy of the file.
             os.remove(copy_path)
 
     def test_transfer_to_on_overwrite_error(self):
         with self.build_file() as file:
             dir = TestLocalDir.build_dir(path=ABS_DIR_PATH)
             # Copy file into dir.
             file.transfer_to(dst=dir)
             # Ensure OverwriteError is raised when trying
             # to copy file a second time.
-            self.assertRaises(OverwriteError, file.transfer_to, dst=dir)
+            self.assertFalse(file.transfer_to(dst=dir))
             # Remove copy of the file.
             copy_path = join_paths(ABS_DIR_PATH, FILE_NAME)
             os.remove(copy_path)
 
     def test_transfer_to_on_include_metadata_set_to_false(self):
         with (
             mock_s3() as mocks3,
@@ -1256,19 +1597,19 @@
         self.assertEqual(dir.get_path(), ABS_DIR_PATH)
 
     def test__get_separator(self):
         self.assertEqual(self.build_dir(path=os.getcwd())._get_separator(), os.sep)
 
     def test_get_name(self):
         dir = self.build_dir(path=ABS_DIR_PATH)
-        self.assertEqual(dir.get_name(), DIR_NAME.rstrip(SEPARATOR))
+        self.assertEqual(dir.get_name(), DIR_NAME.removesuffix(SEPARATOR))
 
     def test_get_uri(self):
         dir = self.build_dir(path=ABS_DIR_PATH)
-        self.assertEqual(dir.get_uri(), f"file:///{ABS_DIR_PATH.lstrip(SEPARATOR)}")
+        self.assertEqual(dir.get_uri(), f"file:///{ABS_DIR_PATH.removeprefix(SEPARATOR)}")
 
     def test_get_metadata_on_invalid_file_error(self):
         dir = self.build_dir()
         self.assertRaises(InvalidFileError, dir.get_metadata, file_path="NON_EXISTING_PATH")
 
     def test_get_metadata(self):
         dir = self.build_dir(path=ABS_DIR_PATH)
@@ -1429,50 +1770,90 @@
         self.assertEqual(self.build_dir(path=ABS_DIR_PATH).get_size(), 4)
 
     def test_get_size_on_recursively(self):
         self.assertEqual(self.build_dir(path=ABS_DIR_PATH).get_size(recursively=True), 16)
 
     def test_transfer_to(self):
         # Create a temporary dictionary.
-        tmp_dir_path = to_abs(REL_DIR_PATH.replace('dir', 'TMP_DIR'))
+        tmp_dir_path = to_abs(REL_DIR_PATH.replace('dir', TMP_DIR_NAME))
         os.mkdir(tmp_dir_path)
         # Copy the directory's contents into this tmp directory.
         self.build_dir(path=ABS_DIR_PATH).transfer_to(
             dst=self.build_dir(path=tmp_dir_path))
-        # Assert that the two directories contains the same contents
-        self.assertEqual(
-            ''.join(s for s in sorted(os.listdir(ABS_DIR_PATH)) if s.endswith('.txt')),
-            ''.join(s for s in sorted(os.listdir(tmp_dir_path))))
+        # Assert that the two directories contains the same contents.
+        original = [s for s in sorted(os.listdir(ABS_DIR_PATH)) if s.endswith('.txt')]
+        copies = [s for s in sorted(os.listdir(tmp_dir_path))]
+        # 1. Assert number of copied files are the same.
+        self.assertEqual(len(original), len(copies))
+        # 2. Iterate over all files.
+        for ofp, cfp in zip(original, copies):
+            # Assert their contents are the same.
+            with (
+                open(file=join_paths(ABS_DIR_PATH, ofp), mode='rb') as of,
+                open(file=join_paths(tmp_dir_path, cfp), mode='rb') as cp
+            ):
+                self.assertEqual(of.read(), cp.read())
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
     def test_transfer_to_on_recursively(self):
         # Create a temporary dictionary.
-        tmp_dir_name = 'TMP_DIR'
+        tmp_dir_name = TMP_DIR_NAME
         tmp_dir_path = to_abs(REL_DIR_PATH.replace('dir', tmp_dir_name))
         os.mkdir(tmp_dir_path)
         # Recursively copy the directory's contents
         # into this tmp directory.
         self.build_dir(path=ABS_DIR_PATH).transfer_to(
             dst=self.build_dir(path=tmp_dir_path),
             recursively=True)
-        # Assert that the two directories contain the same contents.
-        self.assertEqual(
-            ''.join(join_paths(dp, f).replace(
-                f'{SEPARATOR}dir{SEPARATOR}',
-                f'{SEPARATOR}{tmp_dir_name}{SEPARATOR}')
-                for dp, _, fn in os.walk(ABS_DIR_PATH) for f in fn),
-            ''.join(join_paths(dp, f)
-                for dp, _, fn in os.walk(tmp_dir_path) for f in fn))
+        # Assert that the two directories contains the same contents.
+        original = [join_paths(dp, f) for dp, _, fn in 
+                    os.walk(ABS_DIR_PATH) for f in fn]
+        copies = [join_paths(dp, f) for dp, _, fn in 
+                os.walk(tmp_dir_path) for f in fn]
+        # 1. Assert number of copied files are the same.
+        self.assertEqual(len(original), len(copies))
+        # 2. Iterate over all files.
+        for ofp, cfp in zip(original, copies):
+            # Assert their contents are the same.
+            with (
+                open(file=ofp, mode='rb') as of,
+                open(file=cfp, mode='rb') as cp
+            ):
+                self.assertEqual(of.read(), cp.read())
+        # Remove temporary directory.
+        shutil.rmtree(tmp_dir_path)
+
+    def test_transfer_to_on_chunk_size(self):
+        # Create a temporary dictionary.
+        tmp_dir_path = to_abs(REL_DIR_PATH.replace('dir', TMP_DIR_NAME))
+        os.mkdir(tmp_dir_path)
+        # Copy the directory's contents into this tmp directory.
+        self.build_dir(path=ABS_DIR_PATH).transfer_to(
+            dst=self.build_dir(path=tmp_dir_path),
+            chunk_size=1)
+        # Assert that the two directories contains the same contents.
+        original = [s for s in sorted(os.listdir(ABS_DIR_PATH)) if s.endswith('.txt')]
+        copies = [s for s in sorted(os.listdir(tmp_dir_path))]
+        # 1. Assert number of copied files are the same.
+        self.assertEqual(len(original), len(copies))
+        # 2. Iterate over all files.
+        for ofp, cfp in zip(original, copies):
+            # Assert their contents are the same.
+            with (
+                open(file=join_paths(ABS_DIR_PATH, ofp), mode='rb') as of,
+                open(file=join_paths(tmp_dir_path, cfp), mode='rb') as cp
+            ):
+                self.assertEqual(of.read(), cp.read())
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
     def test_transfer_to_on_overwrite_set_to_false(self):
         # Create a copy of the directory.
-        tmp_dir_name = 'TMP_DIR'
+        tmp_dir_name = TMP_DIR_NAME
         tmp_dir_path = to_abs(REL_DIR_PATH.replace('dir', tmp_dir_name))
         shutil.copytree(src=ABS_DIR_PATH, dst=tmp_dir_path)
         # While capturing stdout...
         with io.StringIO() as stdo:
             sys.stdout = stdo
             # Copy directory with "overwrite" set to "False".
             self.build_dir(path=ABS_DIR_PATH).transfer_to(
@@ -1483,15 +1864,15 @@
 
             self.assertTrue("Operation unsuccessful" in stdo.getvalue())
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
     def test_transfer_to_on_overwrite_set_to_true(self):
         # Create a copy of the directory.
-        tmp_dir_name = 'TMP_DIR'
+        tmp_dir_name = TMP_DIR_NAME
         tmp_dir_path = to_abs(REL_DIR_PATH.replace('dir', tmp_dir_name))
         shutil.copytree(src=ABS_DIR_PATH, dst=tmp_dir_path)
         # While capturing stdout...
         with io.StringIO() as stdo:
             sys.stdout = stdo
             # Copy directory with "overwrite" set to "True".
             self.build_dir(path=ABS_DIR_PATH).transfer_to(
@@ -1506,15 +1887,15 @@
 
     def test_transfer_to_on_include_metadata_set_to_false(self):
         # Set metadata for a directory's file.
         filename, metadata = DIR_FILE_NAME, {'1': '1'}
         dir = self.build_dir(path=ABS_DIR_PATH)
         dir.set_metadata(file_path=filename, metadata=metadata)
         # Create a temporary dictionary.
-        tmp_dir_path = to_abs(REL_DIR_PATH.replace('dir', 'TMP_DIR'))
+        tmp_dir_path = to_abs(REL_DIR_PATH.replace('dir', TMP_DIR_NAME))
         os.mkdir(tmp_dir_path)
         tmp_dir = self.build_dir(path=tmp_dir_path)
         # Copy the directory's contents into this
         # tmp directory without including metadata.
         dir.transfer_to(dst=tmp_dir, include_metadata=False)
         # Assert that no metadata were transfered.
         self.assertEqual(tmp_dir.get_metadata(file_path=filename), {})
@@ -1523,28 +1904,28 @@
 
     def test_transfer_to_on_include_metadata_set_to_true(self):
         # Set metadata for a directory's file.
         filename, metadata = DIR_FILE_NAME, {'1': '1'}
         dir = self.build_dir(path=ABS_DIR_PATH)
         dir.set_metadata(file_path=filename, metadata=metadata)
         # Create a temporary dictionary.
-        tmp_dir_path = to_abs(REL_DIR_PATH.replace('dir', 'TMP_DIR'))
+        tmp_dir_path = to_abs(REL_DIR_PATH.replace('dir', TMP_DIR_NAME))
         os.mkdir(tmp_dir_path)
         tmp_dir = self.build_dir(path=tmp_dir_path)
         # Copy the directory's contents into this
         # tmp directory while including metadata.
         dir.transfer_to(dst=tmp_dir, include_metadata=True)
         # Assert that the two directories contains the same contents.
         self.assertEqual(
             tmp_dir.get_metadata(file_path=filename),
             metadata)
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
-    def test_transfer_to_on_cloud_dir_include_metadata_set_to_true(self):
+    def test_transfer_to_on_aws_cloud_dir_include_metadata_set_to_true(self):
         # Set metadata for a directory's file.
         with mock_s3() as mocks3:
             # Create AWSS3 bucket.
             create_aws_s3_bucket(mocks3, BUCKET, METADATA)
             # Copy directory contents including metadata
             filename, metadata = DIR_FILE_NAME, {'2': '2'}
             dir = self.build_dir(path=ABS_DIR_PATH)
@@ -1553,82 +1934,80 @@
                 dir.transfer_to(dst=aws_dir, overwrite=True, include_metadata=True)
                 # Assert that the object's metadata have been modified.
                 self.assertEqual(
                     get_aws_s3_object(
                         aws_dir.get_bucket_name(),
                         REL_DIR_FILE_PATH).metadata,
                     metadata)
-                
-    def test_traverse_files(self):
-        dir = self.build_dir(path=ABS_DIR_PATH)
-        self.assertEqual(
-            ''.join(map(lambda file: file.get_path(), dir.traverse_files())),
-            ''.join(filter(lambda path: not path.endswith('/'), get_abs_contents(recursively=False))))
-
-    def test_traverse_files_on_recursively(self):
-        dir = self.build_dir(path=ABS_DIR_PATH)
-        self.assertEqual(
-            ''.join(map(lambda file: file.get_path(), dir.traverse_files(recursively=True))),
-            ''.join(get_abs_contents(recursively=True)))
-        
-    def test_get_files(self):
-        dir = self.build_dir(path=ABS_DIR_PATH)
-        files = dir.get_files()
-        self.assertEqual(
-            ''.join(map(lambda path: files[path].get_path(), files)),
-            ''.join(filter(lambda path: not path.endswith('/'), get_abs_contents(recursively=False))))
-
-    def test_get_files_on_recursively(self):
-        dir = self.build_dir(path=ABS_DIR_PATH)
-        files = dir.get_files(recursively=True)
-        self.assertEqual(
-            ''.join(map(lambda path: files[path].get_path(), files)),
-            ''.join(get_abs_contents(recursively=True)))
-        
-    def test_get_files_on_show_abs_path(self):
-        dir = self.build_dir(path=ABS_DIR_PATH)
-        files = dir.get_files(show_abs_path=True)
-        self.assertEqual(
-            ''.join(files),
-            ''.join(filter(lambda path: not path.endswith('/'), get_abs_contents(recursively=False))))
-        
-    def test_get_files_on_recursively_and_show_abs_path(self):
-        dir = self.build_dir(path=ABS_DIR_PATH)
-        files = dir.get_files(recursively=True, show_abs_path=True)
-        self.assertEqual(
-            ''.join(files),
-            ''.join(get_abs_contents(recursively=True)))
         
     def test_get_file(self):
-        dir = self.build_dir(path=ABS_DIR_PATH)
-        file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-        file = dir.get_file(file_path)
+        dir = self.build_dir()
+        file = dir.get_file(DIR_FILE_NAME)
         self.assertEqual(file.get_path(), ABS_DIR_FILE_PATH)
 
+    def test_get_file_on_invalid_path_error(self):
+        dir = self.build_dir()
+        self.assertRaises(InvalidPathError, dir.get_file, "NON_EXISTING_PATH")
+
+    def test_get_file_on_invalid_file_error(self):
+        dir = self.build_dir()
+        self.assertRaises(InvalidFileError, dir.get_file, DIR_SUBDIR_NAME)
+
+    def test_get_subdir(self):
+        dir = self.build_dir()
+        subdir = dir.get_subdir(DIR_SUBDIR_NAME)
+        self.assertEqual(subdir.get_path(), ABS_DIR_SUBDIR_PATH)
+
+    def test_get_subdir_on_invalid_path_error(self):
+        dir = self.build_dir()
+        self.assertRaises(InvalidPathError, dir.get_subdir, "NON_EXISTING_PATH")
+
+    def test_get_subdir_on_invalid_directory_error(self):
+        dir = self.build_dir()
+        self.assertRaises(InvalidDirectoryError, dir.get_subdir, DIR_FILE_NAME)
+
     def test_file_shared_metadata_on_modify_from_dir(self):
         # Create dir and get file.
-        dir = self.build_dir(path=ABS_DIR_PATH)
-        file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-        file = dir.get_file(file_path)
+        dir = self.build_dir()
+        file = dir.get_file(DIR_FILE_NAME)
         # Change metadata via "Dir" API.
-        dir.set_metadata(file_path, METADATA)
+        dir.set_metadata(DIR_FILE_NAME, METADATA)
         # Assert file metadata have been changed.
         self.assertEqual(file.get_metadata(), METADATA)
 
     def test_file_shared_metadata_on_modify_from_file(self):
         # Create dir and get file.
-        dir = self.build_dir(path=ABS_DIR_PATH)
-        file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-        file = dir.get_file(file_path)
+        dir = self.build_dir()
+        file = dir.get_file(DIR_FILE_NAME)
         # Change metadata via "File" API.
         file.set_metadata(METADATA)
         # Assert file metadata have been changed.
-        self.assertEqual(dir.get_metadata(file_path), METADATA)
-        
+        self.assertEqual(dir.get_metadata(DIR_FILE_NAME), METADATA)
 
+    def test_subdir_shared_metadata_on_modify_from_dir(self):
+        # Create dir and get file.
+        dir = self.build_dir()
+        subdir = dir.get_subdir(DIR_SUBDIR_NAME)
+        # Change metadata via "Dir" API.
+        dir.set_metadata(
+            DIR_SUBDIR_NAME + DIR_SUBDIR_FILE_NAME, METADATA)
+        # Assert file metadata have been changed.
+        self.assertEqual(
+            subdir.get_metadata(DIR_SUBDIR_FILE_NAME), METADATA)
+
+    def test_subdir_shared_metadata_on_modify_from_subdir(self):
+        # Create dir and get file.
+        dir = self.build_dir()
+        subdir = dir.get_subdir(DIR_SUBDIR_NAME)
+        # Change metadata via "File" API.
+        subdir.set_metadata(DIR_SUBDIR_FILE_NAME, METADATA)
+        # Assert file metadata have been changed.
+        self.assertEqual(
+            dir.get_metadata(DIR_SUBDIR_NAME + DIR_SUBDIR_FILE_NAME), METADATA)
+        
 
 class TestRemoteDir(unittest.TestCase):
 
     def setUp(self):
         for k, v in MockSFTPClient.get_mock_methods().items():
             patch(k, v).start()
 
@@ -1660,25 +2039,28 @@
 
     def test_constructor_on_empty_path_error(self):
         self.assertRaises(InvalidPathError, self.build_dir, path="")
 
     def test_constructor_on_invalid_path_error(self):
         self.assertRaises(InvalidPathError, self.build_dir, path="NON_EXISTING_PATH")
 
+    def test_constructor_on_invalid_directory_error(self):
+        self.assertRaises(InvalidDirectoryError, self.build_dir, path=ABS_DIR_FILE_PATH)
+
     def test_get_hostname(self):
         with self.build_dir() as dir:
             self.assertEqual(dir.get_hostname(), HOST)
 
     def test_get_name(self):
         with self.build_dir() as dir:
             self.assertEqual(dir.get_name(), DIR_NAME)    
 
     def test_get_uri(self):
         with self.build_dir() as dir:
-            self.assertEqual(dir.get_uri(), f"sftp://{HOST}/{ABS_DIR_PATH.lstrip(os.sep)}")
+            self.assertEqual(dir.get_uri(), f"sftp://{HOST}/{ABS_DIR_PATH.removeprefix(os.sep)}")
             
     def test_set_and_get_metadata(self):
         with self.build_dir() as dir:
             file_path = ABS_DIR_FILE_PATH
             metadata = {'a': '1'}
             dir.set_metadata(file_path=file_path, metadata=metadata)
             self.assertEqual(dir.get_metadata(file_path=file_path), metadata)
@@ -1838,47 +2220,90 @@
 
     def test_get_size_on_recursively(self):
         with self.build_dir() as dir:
             self.assertEqual(dir.get_size(recursively=True), 16)
 
     def test_transfer_to(self):
         # Create a temporary dictionary.
-        tmp_dir_path = ABS_DIR_PATH.replace(DIR_NAME, 'TMP_DIR')
+        tmp_dir_path = ABS_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME)
         os.mkdir(tmp_dir_path)
         # Copy the directory's contents into this tmp directory.
         with self.build_dir() as dir:
             dir.transfer_to(dst=LocalDir(path=tmp_dir_path))
-        # Assert that the two directories contain the same contents.
-        self.assertEqual(
-            ''.join(s for s in sorted(os.listdir(REL_DIR_PATH)) if s.endswith('.txt')),
-            ''.join(s for s in sorted(os.listdir(tmp_dir_path))))
+        # Assert that the two directories contains the same contents.
+        original = [s for s in sorted(os.listdir(ABS_DIR_PATH)) if s.endswith('.txt')]
+        copies = [s for s in sorted(os.listdir(tmp_dir_path))]
+        # 1. Assert number of copied files are the same.
+        self.assertEqual(len(original), len(copies))
+        # 2. Iterate over all files.
+        for ofp, cfp in zip(original, copies):
+            # Assert their contents are the same.
+            with (
+                open(file=join_paths(ABS_DIR_PATH, ofp), mode='rb') as of,
+                open(file=join_paths(tmp_dir_path, cfp), mode='rb') as cp
+            ):
+                self.assertEqual(of.read(), cp.read())
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
     def test_transfer_to_on_recursively(self):
         # Create a temporary dictionary.
-        tmp_dir_path = ABS_DIR_PATH.replace(DIR_NAME, 'TMP_DIR')
+        tmp_dir_path = ABS_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME)
         os.mkdir(tmp_dir_path)
         # Copy the directory's contents into this tmp directory.
         with self.build_dir() as dir:
             dir.transfer_to(
                 dst=LocalDir(path=tmp_dir_path),
                 recursively=True)
-        # Assert that the two directories contain the same contents.
-        self.assertEqual(
-            ''.join(join_paths(dp, f).removeprefix(REL_DIR_PATH)
-                for dp, _, fn in os.walk(REL_DIR_PATH) for f in fn),
-            ''.join(join_paths(dp, f).removeprefix(tmp_dir_path)
-                for dp, _, fn in os.walk(tmp_dir_path) for f in fn))
+        # Assert that the two directories contains the same contents.
+        original = [join_paths(dp, f) for dp, _, fn in 
+                    os.walk(ABS_DIR_PATH) for f in fn]
+        copies = [join_paths(dp, f) for dp, _, fn in 
+                os.walk(tmp_dir_path) for f in fn]
+        # 1. Assert number of copied files are the same.
+        self.assertEqual(len(original), len(copies))
+        # 2. Iterate over all files.
+        for ofp, cfp in zip(original, copies):
+            # Assert their contents are the same.
+            with (
+                open(file=ofp, mode='rb') as of,
+                open(file=cfp, mode='rb') as cp
+            ):
+                self.assertEqual(of.read(), cp.read())
+        # Remove temporary directory.
+        shutil.rmtree(tmp_dir_path)
+
+    def test_transfer_to_on_chunk_size(self):
+        # Create a temporary dictionary.
+        tmp_dir_path = ABS_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME)
+        os.mkdir(tmp_dir_path)
+        # Copy the directory's contents into this tmp directory.
+        with self.build_dir() as dir:
+            dir.transfer_to(
+                dst=LocalDir(path=tmp_dir_path),
+                chunk_size=1)
+        # Assert that the two directories contains the same contents.
+        original = [s for s in sorted(os.listdir(ABS_DIR_PATH)) if s.endswith('.txt')]
+        copies = [s for s in sorted(os.listdir(tmp_dir_path))]
+        # 1. Assert number of copied files are the same.
+        self.assertEqual(len(original), len(copies))
+        # 2. Iterate over all files.
+        for ofp, cfp in zip(original, copies):
+            # Assert their contents are the same.
+            with (
+                open(file=join_paths(ABS_DIR_PATH, ofp), mode='rb') as of,
+                open(file=join_paths(tmp_dir_path, cfp), mode='rb') as cp
+            ):
+                self.assertEqual(of.read(), cp.read())
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
     def test_transfer_to_on_overwrite_set_to_false(self):
         # Create a copy of the directory.
-        tmp_dir_name = 'TMP_DIR'
+        tmp_dir_name = TMP_DIR_NAME
         tmp_dir_path = ABS_DIR_PATH.replace(DIR_NAME, tmp_dir_name)
         shutil.copytree(src=ABS_DIR_PATH, dst=tmp_dir_path)
         # While capturing stdout...
         with (
             io.StringIO() as stdo,
             self.build_dir() as dir
         ):
@@ -1892,15 +2317,15 @@
 
             self.assertTrue("Operation unsuccessful" in stdo.getvalue())
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
     def test_transfer_to_on_overwrite_set_to_true(self):
         # Create a copy of the directory.
-        tmp_dir_name = 'TMP_DIR'
+        tmp_dir_name = TMP_DIR_NAME
         tmp_dir_path = ABS_DIR_PATH.replace(DIR_NAME, tmp_dir_name)
         shutil.copytree(src=ABS_DIR_PATH, dst=tmp_dir_path)
         # While capturing stdout...
         with (
             io.StringIO() as stdo,
             self.build_dir() as dir
         ):
@@ -1918,15 +2343,15 @@
 
     def test_transfer_to_on_include_metadata_set_to_false(self):
         # Set metadata for a directory's file.
         filename, metadata = ABS_DIR_FILE_PATH, {'1': '1'}
         with self.build_dir() as dir:
             dir.set_metadata(file_path=filename, metadata=metadata)
             # Create a temporary dictionary.
-            tmp_dir_path = ABS_DIR_PATH.replace(DIR_NAME, 'TMP_DIR')
+            tmp_dir_path = ABS_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME)
             os.makedirs(tmp_dir_path)
             tmp_dir = LocalDir(path=tmp_dir_path)
             # Copy the directory's contents into this
             # tmp directory without including metadata.
             dir.transfer_to(dst=tmp_dir, include_metadata=False)
         # Assert that no metadata have been transfered.
         self.assertEqual(tmp_dir.get_metadata(
@@ -1936,128 +2361,129 @@
 
     def test_transfer_to_on_include_metadata_set_to_true(self):
         # Set metadata for a directory's file.
         filename, metadata = ABS_DIR_FILE_PATH, {'1': '1'}
         with self.build_dir() as dir:
             dir.set_metadata(file_path=filename, metadata=metadata)
             # Create a temporary dictionary.
-            tmp_dir_path = ABS_DIR_PATH.replace(DIR_NAME, 'TMP_DIR')
+            tmp_dir_path = ABS_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME)
             os.mkdir(tmp_dir_path)
             tmp_dir = LocalDir(path=tmp_dir_path)
             # Copy the directory's contents into this
             # tmp directory without including metadata.
             dir.transfer_to(dst=tmp_dir, include_metadata=True)
         # Assert the file's metadata are the same.
         self.assertEqual(
             tmp_dir.get_metadata(
                 file_path=filename.replace(ABS_DIR_PATH, '')),
             metadata)
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
-
-    def test_transfer_to_on_cloud_dir_include_metadata_set_to_true(self):
-        # Set metadata for a directory's file.
-        with mock_s3() as mocks3:
-            # Create AWSS3 bucket.
-            create_aws_s3_bucket(mocks3, BUCKET, METADATA)
-            # Copy directory contents including metadata
-            filename, metadata = ABS_DIR_FILE_PATH, {'2': '2'}
+                
+    def test_transfer_to_as_dst(self):
+        # Get source file.
+        src_file = TestLocalFile.build_file()
+        # Create a temporary "remote" dictionary.
+        tmp_dir_path = to_abs(REL_DIR_PATH.replace('dir', TMP_DIR_NAME))
+        os.mkdir(tmp_dir_path)
+        with self.build_dir(path=tmp_dir_path) as remote_dir:
+            # Copy file into dir.
+            src_file.transfer_to(dst=remote_dir)
+            # Confirm that file was indeed copied.
+            copy_path = join_paths(tmp_dir_path, FILE_NAME)
             with (
-                self.build_dir() as dir,
-                TestAWSS3Dir().build_dir() as aws_dir
+                open(ABS_FILE_PATH, mode='rb') as file,
+                open(copy_path, mode='rb') as copy
             ):
-                dir.set_metadata(file_path=filename, metadata=metadata)
-                dir.transfer_to(dst=aws_dir, overwrite=True, include_metadata=True)
-                # Assert that the object's metadata have been modified.
-                self.assertEqual(
-                    get_aws_s3_object(
-                        aws_dir.get_bucket_name(),
-                        REL_DIR_FILE_PATH).metadata,
-                    metadata)
-                
-    def test_transfer_to_as_destination(self):
-        # Create a "remote" temporary dictionary.
-        tmp_dir_path = REL_DIR_PATH.replace(DIR_NAME, 'TMP_DIR')
+                self.assertEqual(file.read(), copy.read())
+        shutil.rmtree(tmp_dir_path)
+
+    def test_transfer_to_as_dst_on_chunk_size(self):
+        # Get source file.
+        src_file = TestLocalFile.build_file()
+        # Create a temporary "remote" dictionary.
+        tmp_dir_path = to_abs(REL_DIR_PATH.replace('dir', TMP_DIR_NAME))
         os.mkdir(tmp_dir_path)
-        # Copy the local dir's contents into this
-        # "remote" tmp directory.
-        with self.build_dir(path=tmp_dir_path) as dir:
-            TestLocalDir.build_dir(ABS_DIR_PATH).transfer_to(dir)
-        # Assert that the two directories contain the same contents.
-        self.assertEqual(
-            ''.join(s for s in sorted(os.listdir(ABS_DIR_PATH)) if s.endswith('.txt')),
-            ''.join(s for s in sorted(os.listdir(tmp_dir_path))))
-        # Remove temporary directory.
+        with self.build_dir(path=tmp_dir_path) as remote_dir:
+            # Copy file into dir.
+            src_file.transfer_to(dst=remote_dir, chunk_size=1)
+            # Confirm that file was indeed copied.
+            copy_path = join_paths(tmp_dir_path, FILE_NAME)
+            with (
+                open(ABS_FILE_PATH, mode='rb') as file,
+                open(copy_path, mode='rb') as copy
+            ):
+                self.assertEqual(file.read(), copy.read())
         shutil.rmtree(tmp_dir_path)
 
-    def test_traverse_files(self):
+        
+    def test_get_file(self):
         with self.build_dir() as dir:
-            self.assertEqual(
-                ''.join(map(lambda file: file.get_path(), dir.traverse_files())),
-                ''.join(filter(lambda path: not path.endswith('/'), get_abs_contents(recursively=False))))
+            file = dir.get_file(DIR_FILE_NAME)
+            self.assertEqual(file.get_path(), ABS_DIR_FILE_PATH)
 
-    def test_traverse_files_on_recursively(self):
-        with self.build_dir() as dir:
-            self.assertEqual(
-                ''.join(map(lambda file: file.get_path(), dir.traverse_files(recursively=True))),
-                ''.join(get_abs_contents(recursively=True)))
-        
-    def test_get_files(self):
+    def test_get_file_on_invalid_path_error(self):
         with self.build_dir() as dir:
-            files = dir.get_files()
-            self.assertEqual(
-                ''.join(map(lambda path: files[path].get_path(), files)),
-                ''.join(filter(lambda path: not path.endswith('/'), get_abs_contents(recursively=False))))
+            self.assertRaises(InvalidPathError, dir.get_file, "NON_EXISTING_PATH")
 
-    def test_get_files_on_recursively(self):
+    def test_get_file_on_invalid_file_error(self):
         with self.build_dir() as dir:
-            files = dir.get_files(recursively=True)
-            self.assertEqual(
-                ''.join(map(lambda path: files[path].get_path(), files)),
-                ''.join(get_abs_contents(recursively=True)))
-        
-    def test_get_files_on_show_abs_path(self):
+            self.assertRaises(InvalidFileError, dir.get_file, DIR_SUBDIR_NAME)
+
+    def test_get_subdir(self):
         with self.build_dir() as dir:
-            files = dir.get_files(show_abs_path=True)
-            self.assertEqual(
-                ''.join(files),
-                ''.join(filter(lambda path: not path.endswith('/'), get_abs_contents(recursively=False))))
-        
-    def test_get_files_on_recursively_and_show_abs_path(self):
+            subdir = dir.get_subdir(DIR_SUBDIR_NAME)
+            self.assertEqual(subdir.get_path(), ABS_DIR_SUBDIR_PATH)
+
+    def test_get_subdir_on_invalid_path_error(self):
         with self.build_dir() as dir:
-            files = dir.get_files(recursively=True, show_abs_path=True)
-            self.assertEqual(
-                ''.join(files),
-                ''.join(get_abs_contents(recursively=True)))
-        
-    def test_get_file(self):
+            self.assertRaises(InvalidPathError, dir.get_subdir, "NON_EXISTING_PATH")
+
+    def test_get_subdir_on_invalid_directory_error(self):
         with self.build_dir() as dir:
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            file = dir.get_file(file_path)
-            self.assertEqual(file.get_path(), ABS_DIR_FILE_PATH)
+            self.assertRaises(InvalidDirectoryError, dir.get_subdir, DIR_FILE_NAME)
 
     def test_file_shared_metadata_on_modify_from_dir(self):
         with self.build_dir() as dir:
             # Access file via dir.
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            file = dir.get_file(file_path)
+            file = dir.get_file(DIR_FILE_NAME)
             # Change metadata via "Dir" API.
-            dir.set_metadata(file_path, METADATA)
+            dir.set_metadata(DIR_FILE_NAME, METADATA)
             # Assert file metadata have been changed.
             self.assertEqual(file.get_metadata(), METADATA)
 
     def test_file_shared_metadata_on_modify_from_file(self):
         with self.build_dir() as dir:
             # Access file via dir.
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            file = dir.get_file(file_path)
+            file = dir.get_file(DIR_FILE_NAME)
             # Change metadata via "File" API.
             file.set_metadata(METADATA)
             # Assert file metadata have been changed.
-            self.assertEqual(dir.get_metadata(file_path), METADATA)
+            self.assertEqual(dir.get_metadata(DIR_FILE_NAME), METADATA)
+
+    def test_subdir_shared_metadata_on_modify_from_dir(self):
+        # Create dir and get file.
+        with self.build_dir() as dir:
+            subdir = dir.get_subdir(DIR_SUBDIR_NAME)
+            # Change metadata via "Dir" API.
+            dir.set_metadata(
+                DIR_SUBDIR_NAME + DIR_SUBDIR_FILE_NAME, METADATA)
+            # Assert file metadata have been changed.
+            self.assertEqual(
+                subdir.get_metadata(DIR_SUBDIR_FILE_NAME), METADATA)
+
+    def test_subdir_shared_metadata_on_modify_from_subdir(self):
+        # Create dir and get file.
+        with self.build_dir() as dir:
+            subdir = dir.get_subdir(DIR_SUBDIR_NAME)
+            # Change metadata via "File" API.
+            subdir.set_metadata(DIR_SUBDIR_FILE_NAME, METADATA)
+            # Assert file metadata have been changed.
+            self.assertEqual(
+                dir.get_metadata(DIR_SUBDIR_NAME + DIR_SUBDIR_FILE_NAME), METADATA)
         
     '''
     Test connection methods.
     '''
     def test_open(self):
         dir = self.build_dir()
         dir.close()
@@ -2182,17 +2608,16 @@
 
     def test_file_shared_cache_on_cache_via_dir(self):
         with (
             self.build_dir(cache=False) as no_cache_dir,
             self.build_dir(cache=True) as cache_dir
         ):
             # Access file via both dirs.
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            no_cache_file = no_cache_dir.get_file(file_path)
-            cache_file = cache_dir.get_file(file_path)
+            no_cache_file = no_cache_dir.get_file(DIR_FILE_NAME)
+            cache_file = cache_dir.get_file(DIR_FILE_NAME)
             # Count total size for both dirs.
             _ = no_cache_dir.get_size()
             _ = cache_dir.get_size()
             # Time no-cache-file's "get_size"
             t = time.time()
             _ = no_cache_file.get_size()
             normal_time = time.time() - t
@@ -2205,30 +2630,72 @@
 
     def test_file_shared_cache_on_cache_via_file(self):
         with (
             self.build_dir(cache=False) as no_cache_dir,
             self.build_dir(cache=True) as cache_dir
         ):
             # Count size of files via both dirs using the "File" API.
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            for file in no_cache_dir.get_files().values():
-                _ = file.get_size()
-            for file in cache_dir.get_files().values():
-                _ = file.get_size()
+            for path in no_cache_dir.traverse():
+                try:
+                    _ = no_cache_dir.get_file(path).get_size()
+                    _ = cache_dir.get_file(path).get_size()
+                except:
+                    continue
             # Time no-cache-dir's "get_size"
             t = time.time()
             _ = no_cache_dir.get_size()
             normal_time = time.time() - t
             # Time cache-dir's "get_size"
             t = time.time()
             _ = cache_dir.get_size()
             cache_time = time.time() - t
             # Compare fetch times.
             self.assertGreater(normal_time, cache_time)
 
+    def test_subdir_shared_cache_on_cache_via_dir(self):
+        with (
+            self.build_dir(cache=False) as no_cache_dir,
+            self.build_dir(cache=True) as cache_dir
+        ):
+            # Access subdir via both dirs.
+            no_cache_subdir = no_cache_dir.get_subdir(DIR_SUBDIR_NAME)
+            cache_subdir = cache_dir.get_subdir(DIR_SUBDIR_NAME)
+            # Count total size for both dirs.
+            _ = no_cache_dir.get_size(recursively=True)
+            _ = cache_dir.get_size(recursively=True)
+            # Time no-cache-subdir's "get_size"
+            t = time.time()
+            _ = no_cache_subdir.get_size()
+            normal_time = time.time() - t
+            # Time cache-subdir's "get_size"
+            t = time.time()
+            _ = cache_subdir.get_size()
+            cache_time = time.time() - t
+            # Compare fetch times.
+            self.assertGreater(normal_time, cache_time)
+
+    def test_subdir_shared_cache_on_cache_via_subdir(self):
+        with (
+            self.build_dir(cache=False) as no_cache_dir,
+            self.build_dir(cache=True) as cache_dir
+        ):
+            # Count size of both subdirs.
+            _ = no_cache_dir.get_subdir(DIR_SUBDIR_NAME).get_size()
+            _ = cache_dir.get_subdir(DIR_SUBDIR_NAME).get_size()
+            # Time no-cache-dir's "get_size"
+            t = time.time()
+            _ = no_cache_dir.get_size(recursively=True)
+            normal_time = time.time() - t
+            # Time cache-dir's "get_size"
+            t = time.time()
+            _ = cache_dir.get_size(recursively=True)
+            cache_time = time.time() - t
+            # Compare fetch times.
+            self.assertGreater(normal_time, cache_time)
+
 
 class TestAWSS3Dir(unittest.TestCase):
 
     MOCK_S3 = mock_s3()
 
     def get_abs_contents(self, recursively: bool):
         return [join_paths(REL_DIR_PATH, p) for p in (
@@ -2528,51 +2995,93 @@
 
     def test_get_size_on_recursively(self):
         with self.build_dir() as dir:
             self.assertEqual(dir.get_size(recursively=True), 16)
 
     def test_transfer_to(self):
         # Create a temporary dictionary.
-        tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, 'TMP_DIR'))
+        tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME))
         os.mkdir(tmp_dir_path)
         # Copy the directory's contents into this tmp directory.
         with self.build_dir() as dir:
             dir.transfer_to(dst=TestLocalDir.build_dir(path=tmp_dir_path))
-        # Assert that the two directories contain the same contents.
-        self.assertEqual(
-            ''.join(s for s in sorted(self.iterate_aws_s3_dir_objects())),
-            ''.join(s for s in sorted(os.listdir(tmp_dir_path))))
+        # Assert that the two directories contains the same contents.
+        original = [s for s in sorted(self.iterate_aws_s3_dir_objects(show_abs_path=True))]
+        copies = [s for s in sorted(os.listdir(tmp_dir_path))]
+        # 1. Assert number of copied files are the same.
+        self.assertEqual(len(original), len(copies))
+        # 2. Iterate over all files.
+        for ofp, cfp in zip(original, copies):
+            # Assert their contents are the same.
+            with (
+                io.BytesIO() as buffer,
+                open(file=join_paths(tmp_dir_path, cfp), mode='rb') as cp
+            ):
+                get_aws_s3_object(BUCKET, ofp).download_fileobj(buffer)
+                self.assertEqual(buffer.getvalue(), cp.read())
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
     def test_transfer_to_on_recursively(self):
         # Create a temporary dictionary.
-        tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, 'TMP_DIR'))
+        tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME))
         os.mkdir(tmp_dir_path)
         # Copy the directory's contents into this tmp directory.
         with self.build_dir() as dir:
             dir.transfer_to(
                 dst=TestLocalDir.build_dir(path=tmp_dir_path),
                 recursively=True)
-        # Assert that the two directories contain the same contents.
-            expected_results = []
-            for dp, dn, fn in os.walk(tmp_dir_path):
-                dn.sort()
-                for f in sorted(fn):
-                    expected_results.append(
-                        join_paths(dp, f).removeprefix(tmp_dir_path))
-        self.assertEqual(
-            ''.join(s for s in self.iterate_aws_s3_dir_objects(recursively=True)),
-            ''.join(expected_results))
+        # Assert that the two directories contains the same contents.
+        original = [s for s in sorted(self.iterate_aws_s3_dir_objects(
+            recursively=True, show_abs_path=True))]
+        copies = [join_paths(dp, f) for dp, _, fn in 
+                os.walk(tmp_dir_path) for f in fn]
+        # 1. Assert number of copied files are the same.
+        self.assertEqual(len(original), len(copies))
+        # 2. Iterate over all files.
+        for ofp, cfp in zip(original, copies):
+            # Assert their contents are the same.
+            with (
+                io.BytesIO() as buffer,
+                open(cfp, mode='rb') as cp
+            ):
+                get_aws_s3_object(BUCKET, ofp).download_fileobj(buffer)
+                self.assertEqual(buffer.getvalue(), cp.read())
+        # Remove temporary directory.
+        shutil.rmtree(tmp_dir_path)
+
+    def test_transfer_to_on_chunk_size(self):
+        # Create a temporary dictionary.
+        tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME))
+        os.mkdir(tmp_dir_path)
+        # Copy the directory's contents into this tmp directory.
+        with self.build_dir() as dir:
+            dir.transfer_to(
+                dst=TestLocalDir.build_dir(path=tmp_dir_path),
+                chunk_size=1)
+        # Assert that the two directories contains the same contents.
+        original = [s for s in sorted(self.iterate_aws_s3_dir_objects(show_abs_path=True))]
+        copies = [s for s in sorted(os.listdir(tmp_dir_path))]
+        # 1. Assert number of copied files are the same.
+        self.assertEqual(len(original), len(copies))
+        # 2. Iterate over all files.
+        for ofp, cfp in zip(original, copies):
+            # Assert their contents are the same.
+            with (
+                io.BytesIO() as buffer,
+                open(file=join_paths(tmp_dir_path, cfp), mode='rb') as cp
+            ):
+                get_aws_s3_object(BUCKET, ofp).download_fileobj(buffer)
+                self.assertEqual(buffer.getvalue(), cp.read())
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
     def test_transfer_to_on_overwrite_set_to_false(self):
         # Create a copy of the directory.
-        tmp_dir_name = 'TMP_DIR'
+        tmp_dir_name = TMP_DIR_NAME
         tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, tmp_dir_name))
         shutil.copytree(src=ABS_DIR_PATH, dst=tmp_dir_path)
         # While capturing stdout...
         with (
             io.StringIO() as stdo,
             self.build_dir() as dir
         ):
@@ -2586,15 +3095,15 @@
 
             self.assertTrue("Operation unsuccessful" in stdo.getvalue())
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
     def test_transfer_to_on_overwrite_set_to_true(self):
         # Create a copy of the directory.
-        tmp_dir_name = 'TMP_DIR'
+        tmp_dir_name = TMP_DIR_NAME
         tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, tmp_dir_name))
         shutil.copytree(src=ABS_DIR_PATH, dst=tmp_dir_path)
         # While capturing stdout...
         with (
             io.StringIO() as stdo,
             self.build_dir() as dir
         ):
@@ -2659,94 +3168,152 @@
             dir.transfer_to(dst=tmp_dir, include_metadata=True)
         # Assert the file's metadata are the same.
         self.assertEqual(
             tmp_dir.get_metadata(file_path=filename),
             METADATA)
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
-
-    def test_transfer_to_on_include_metadata_to_cloud_dir(self):
-        # Set metadata for a directory's file.
-        filename, metadata = DIR_FILE_NAME, {'2': '2'}
-        with self.build_dir() as dir:
-            dir.set_metadata(file_path=filename, metadata=metadata)
-            # Copy directory contents into itself.
-            dir.transfer_to(dst=dir, overwrite=True, include_metadata=True)
-        # Assert that the object's metadata have been modified.
-        self.assertEqual(
-            get_aws_s3_object(BUCKET, REL_DIR_FILE_PATH).metadata,
-            metadata)
         
-    def test_traverse_files(self):
-        with self.build_dir() as dir:
-            self.assertEqual(
-                ''.join(map(lambda file: file.get_path(), dir.traverse_files())),
-                ''.join(filter(lambda path: not path.endswith('/'), self.get_abs_contents(recursively=False))))
+    def test_transfer_to_as_dst(self):
+        # Get source file.
+        src_file = TestLocalFile.build_file()
+        # Get tmp dir path (already created in bucket).
+        tmp_dir_path = REL_DIR_PATH.replace('dir', TMP_DIR_NAME)
+        with self.build_dir(path=tmp_dir_path) as aws_dir:
+            # Copy file into dir.
+            src_file.transfer_to(dst=aws_dir)
+            # Confirm that file was indeed copied.
+            copy_path = join_paths(tmp_dir_path, FILE_NAME)
+            with (
+                open(ABS_FILE_PATH, mode='rb') as file,
+                io.BytesIO() as buffer
+            ):
+                get_aws_s3_object(
+                    bucket_name=BUCKET, path=copy_path
+                ).download_fileobj(buffer)
+                self.assertEqual(
+                    file.read(),
+                    buffer.getvalue())
 
-    def test_traverse_files_on_recursively(self):
-        with self.build_dir() as dir:
+    def test_transfer_to_as_dst_on_chunk_size(self):
+        # Get source file.
+        src_file = TestLocalFile.build_file()
+        # Get tmp dir path (already created in bucket).
+        tmp_dir_path = REL_DIR_PATH.replace('dir', TMP_DIR_NAME)
+        with self.build_dir(path=tmp_dir_path) as aws_dir:
+            # Copy file into dir.
+            src_file.transfer_to(dst=aws_dir, chunk_size=1000)
+            # Confirm that file was indeed copied.
+            copy_path = join_paths(tmp_dir_path, FILE_NAME)
+            with (
+                open(ABS_FILE_PATH, mode='rb') as file,
+                io.BytesIO() as buffer
+            ):
+                get_aws_s3_object(
+                    bucket_name=BUCKET, path=copy_path
+                ).download_fileobj(buffer)
+                self.assertEqual(
+                    file.read(),
+                    buffer.getvalue())
+
+    def test_transfer_to_as_dst_on_include_metadata(self):
+        # Get source file and metadata.
+        src_file = TestLocalFile.build_file()
+        metadata = {'2': '2'}
+        src_file.set_metadata(metadata=metadata)
+        # Get tmp dir path (already created in bucket).
+        tmp_dir_path = REL_DIR_PATH.replace('dir', TMP_DIR_NAME)
+        with self.build_dir(path=tmp_dir_path) as aws_dir:
+            # Copy file into dir.
+            src_file.transfer_to(dst=aws_dir, include_metadata=True)
+            # Confirm that metadata was indeed assigned.
+            copy_path = join_paths(tmp_dir_path, FILE_NAME)
+            self.assertEqual(
+                get_aws_s3_object(BUCKET, copy_path).metadata,
+                metadata)
+        
+    def test_transfer_to_as_dst_on_chunk_size_and_include_metadata(self):
+        # Get source file and metadata.
+        src_file = TestLocalFile.build_file()
+        metadata = {'2': '2'}
+        src_file.set_metadata(metadata=metadata)
+        # Get tmp dir path (already created in bucket).
+        tmp_dir_path = REL_DIR_PATH.replace('dir', TMP_DIR_NAME)
+        with self.build_dir(path=tmp_dir_path) as aws_dir:
+            # Copy file into dir.
+            src_file.transfer_to(
+                dst=aws_dir,
+                include_metadata=True,
+                chunk_size=1000)
+            # Confirm that metadata was indeed assigned.
+            copy_path = join_paths(tmp_dir_path, FILE_NAME)
             self.assertEqual(
-                ''.join(map(lambda file: file.get_path(), dir.traverse_files(recursively=True))),
-                ''.join(self.get_abs_contents(recursively=True)))
+                get_aws_s3_object(BUCKET, copy_path).metadata,
+                metadata)
         
-    def test_get_files(self):
+    def test_get_file(self):
         with self.build_dir() as dir:
-            files = dir.get_files()
-            self.assertEqual(
-                ''.join(map(lambda path: files[path].get_path(), files)),
-                ''.join(filter(lambda path: not path.endswith('/'),
-                    self.get_abs_contents(recursively=False))))
+            file = dir.get_file(DIR_FILE_NAME)
+            self.assertEqual(file.get_path(), REL_DIR_FILE_PATH)
 
-    def test_get_files_on_recursively(self):
+    def test_get_file_on_invalid_path_error(self):
         with self.build_dir() as dir:
-            files = dir.get_files(recursively=True)
-            self.assertEqual(
-                ''.join(map(lambda path: files[path].get_path(), files)),
-                ''.join(self.get_abs_contents(recursively=True)))
-        
-    def test_get_files_on_show_abs_path(self):
+            self.assertRaises(InvalidPathError, dir.get_file, "NON_EXISTING_PATH")
+
+    def test_get_file_on_invalid_file_error(self):
         with self.build_dir() as dir:
-            files = dir.get_files(show_abs_path=True)
-            self.assertEqual(
-                ''.join(files),
-                ''.join(filter(lambda path: not path.endswith('/'),
-                    self.get_abs_contents(recursively=False))))
-        
-    def test_get_files_on_recursively_and_show_abs_path(self):
+            self.assertRaises(InvalidFileError, dir.get_file, DIR_SUBDIR_NAME)
+
+    def test_get_subdir(self):
         with self.build_dir() as dir:
-            files = dir.get_files(recursively=True, show_abs_path=True)
-            self.assertEqual(
-                ''.join(files),
-                ''.join(self.get_abs_contents(recursively=True)))
-        
-    def test_get_file(self):
+            subdir = dir.get_subdir(DIR_SUBDIR_NAME)
+            self.assertEqual(subdir.get_path(), REL_DIR_SUBDIR_PATH)
+
+    def test_get_subdir_on_invalid_path_error(self):
         with self.build_dir() as dir:
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            file = dir.get_file(file_path)
-            self.assertEqual(file.get_path(), REL_DIR_FILE_PATH)
+            self.assertRaises(InvalidPathError, dir.get_subdir, "NON_EXISTING_PATH")
 
     def test_file_shared_metadata_on_modify_from_dir(self):
         with self.build_dir() as dir:
             # Access file via dir.
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            file = dir.get_file(file_path)
+            file = dir.get_file(DIR_FILE_NAME)
             # Change metadata via "Dir" API.
-            dir.set_metadata(file_path, METADATA)
+            dir.set_metadata(DIR_FILE_NAME, METADATA)
             # Assert file metadata have been changed.
             self.assertEqual(file.get_metadata(), METADATA)
 
     def test_file_shared_metadata_on_modify_from_file(self):
         with self.build_dir() as dir:
             # Access file via dir.
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            file = dir.get_file(file_path)
+            file = dir.get_file(DIR_FILE_NAME)
             # Change metadata via "File" API.
             file.set_metadata(METADATA)
             # Assert file metadata have been changed.
-            self.assertEqual(dir.get_metadata(file_path), METADATA)
+            self.assertEqual(dir.get_metadata(DIR_FILE_NAME), METADATA)
+
+    def test_subdir_shared_metadata_on_modify_from_dir(self):
+        # Create dir and get file.
+        with self.build_dir() as dir:
+            subdir = dir.get_subdir(DIR_SUBDIR_NAME)
+            # Change metadata via "Dir" API.
+            dir.set_metadata(
+                DIR_SUBDIR_NAME + DIR_SUBDIR_FILE_NAME, METADATA)
+            # Assert file metadata have been changed.
+            self.assertEqual(
+                subdir.get_metadata(DIR_SUBDIR_FILE_NAME), METADATA)
+
+    def test_subdir_shared_metadata_on_modify_from_subdir(self):
+        # Create dir and get file.
+        with self.build_dir() as dir:
+            subdir = dir.get_subdir(DIR_SUBDIR_NAME)
+            # Change metadata via "File" API.
+            subdir.set_metadata(DIR_SUBDIR_FILE_NAME, METADATA)
+            # Assert file metadata have been changed.
+            self.assertEqual(
+                dir.get_metadata(DIR_SUBDIR_NAME + DIR_SUBDIR_FILE_NAME), METADATA)
         
     '''
     Test connection methods.
     '''
     def test_open(self):
         dir = self.build_dir()
         dir.close()
@@ -2909,17 +3476,16 @@
 
     def test_file_shared_cache_on_cache_via_dir(self):
         with (
             self.build_dir(cache=False) as no_cache_dir,
             self.build_dir(cache=True) as cache_dir
         ):
             # Access file via both dirs.
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            no_cache_file = no_cache_dir.get_file(file_path)
-            cache_file = cache_dir.get_file(file_path)
+            no_cache_file = no_cache_dir.get_file(DIR_FILE_NAME)
+            cache_file = cache_dir.get_file(DIR_FILE_NAME)
             # Count total size for both dirs.
             _ = no_cache_dir.get_size()
             _ = cache_dir.get_size()
             # Time no-cache-file's "get_size"
             t = time.time()
             _ = no_cache_file.get_size()
             normal_time = time.time() - t
@@ -2932,30 +3498,72 @@
 
     def test_file_shared_cache_on_cache_via_file(self):
         with (
             self.build_dir(cache=False) as no_cache_dir,
             self.build_dir(cache=True) as cache_dir
         ):
             # Count size of files via both dirs using the "File" API.
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            for file in no_cache_dir.get_files().values():
-                _ = file.get_size()
-            for file in cache_dir.get_files().values():
-                _ = file.get_size()
+            for path in no_cache_dir.traverse():
+                try:
+                    _ = no_cache_dir.get_file(path).get_size()
+                    _ = cache_dir.get_file(path).get_size()
+                except:
+                    continue
             # Time no-cache-dir's "get_size"
             t = time.time()
             _ = no_cache_dir.get_size()
             normal_time = time.time() - t
             # Time cache-dir's "get_size"
             t = time.time()
             _ = cache_dir.get_size()
             cache_time = time.time() - t
             # Compare fetch times.
             self.assertGreater(normal_time, cache_time)
 
+    def test_subdir_shared_cache_on_cache_via_dir(self):
+        with (
+            self.build_dir(cache=False) as no_cache_dir,
+            self.build_dir(cache=True) as cache_dir
+        ):
+            # Access subdir via both dirs.
+            no_cache_subdir = no_cache_dir.get_subdir(DIR_SUBDIR_NAME)
+            cache_subdir = cache_dir.get_subdir(DIR_SUBDIR_NAME)
+            # Count total size for both dirs.
+            _ = no_cache_dir.get_size(recursively=True)
+            _ = cache_dir.get_size(recursively=True)
+            # Time no-cache-subdir's "get_size"
+            t = time.time()
+            _ = no_cache_subdir.get_size()
+            normal_time = time.time() - t
+            # Time cache-subdir's "get_size"
+            t = time.time()
+            _ = cache_subdir.get_size()
+            cache_time = time.time() - t
+            # Compare fetch times.
+            self.assertGreater(normal_time, cache_time)
+
+    def test_subdir_shared_cache_on_cache_via_subdir(self):
+        with (
+            self.build_dir(cache=False) as no_cache_dir,
+            self.build_dir(cache=True) as cache_dir
+        ):
+            # Count size of both subdirs.
+            _ = no_cache_dir.get_subdir(DIR_SUBDIR_NAME).get_size()
+            _ = cache_dir.get_subdir(DIR_SUBDIR_NAME).get_size()
+            # Time no-cache-dir's "get_size"
+            t = time.time()
+            _ = no_cache_dir.get_size(recursively=True)
+            normal_time = time.time() - t
+            # Time cache-dir's "get_size"
+            t = time.time()
+            _ = cache_dir.get_size(recursively=True)
+            cache_time = time.time() - t
+            # Compare fetch times.
+            self.assertGreater(normal_time, cache_time)
+
 
 class TestAzureBlobDir(unittest.TestCase):
 
     def get_abs_contents(self, recursively: bool):
         return [join_paths(REL_DIR_PATH, p) for p in (
             RECURSIVE_CONTENTS if recursively else CONTENTS
         )]
@@ -2997,15 +3605,15 @@
             os.rmdir(dir_path)
 
     def test_constructor_on_invalid_path_error(self):
         self.assertRaises(InvalidPathError, self.build_dir, path="NON_EXISTING_PATH")
 
     def test_get_path_on_none_path(self):
         with self.build_dir(path=None) as dir:
-            self.assertEqual(dir.get_path(), SEPARATOR)  
+            self.assertEqual(dir.get_path(), '')  
 
     def test_get_name(self):
         with self.build_dir() as dir:
             self.assertEqual(dir.get_name(), DIR_NAME)
 
     def test_get_name_on_none_path(self):
         with self.build_dir(path=None) as dir:
@@ -3218,48 +3826,91 @@
 
     def test_get_size_on_recursively(self):
         with self.build_dir() as dir:
             self.assertEqual(dir.get_size(recursively=True), 16)
 
     def test_transfer_to(self):
         # Create a temporary dictionary.
-        tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, 'TMP_DIR'))
+        tmp_dir_path = REL_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME)
         os.mkdir(tmp_dir_path)
         # Copy the directory's contents into this tmp directory.
         with self.build_dir() as dir:
             dir.transfer_to(dst=LocalDir(path=tmp_dir_path))
-        # Assert that the two directories contain the same contents.
-        self.assertEqual(
-            ''.join(s for s in sorted(os.listdir(REL_DIR_PATH)) if s.endswith('.txt')),
-            ''.join(s for s in sorted(os.listdir(tmp_dir_path))))
+        # Assert that the two directories contains the same contents.
+        original = [s for s in sorted(os.listdir(ABS_DIR_PATH)) if s.endswith('.txt')]
+        copies = [s for s in sorted(os.listdir(tmp_dir_path))]
+        # 1. Assert number of copied files are the same.
+        self.assertEqual(len(original), len(copies))
+        # 2. Iterate over all files.
+        for ofp, cfp in zip(original, copies):
+            # Assert their contents are the same.
+            with (
+                open(file=join_paths(ABS_DIR_PATH, ofp), mode='rb') as of,
+                open(file=join_paths(tmp_dir_path, cfp), mode='rb') as cp
+            ):
+                self.assertEqual(of.read(), cp.read())
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
     def test_transfer_to_on_recursively(self):
         # Create a temporary dictionary.
-        tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, 'TMP_DIR'))
+        tmp_dir_path = REL_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME)
         os.mkdir(tmp_dir_path)
         # Copy the directory's contents into this tmp directory.
         with self.build_dir() as dir:
             dir.transfer_to(
                 dst=LocalDir(path=tmp_dir_path),
                 recursively=True)
-        # Assert that the two directories contain the same contents.
-        self.assertEqual(
-            ''.join(join_paths(dp, f).removeprefix(REL_DIR_PATH)
-                for dp, _, fn in os.walk(REL_DIR_PATH) for f in fn),
-            ''.join(join_paths(dp, f).removeprefix(tmp_dir_path)
-                for dp, _, fn in os.walk(tmp_dir_path) for f in fn))
+        # Assert that the two directories contains the same contents.
+        original = [join_paths(dp, f) for dp, _, fn in 
+                    os.walk(ABS_DIR_PATH) for f in fn]
+        copies = [join_paths(dp, f) for dp, _, fn in 
+                os.walk(tmp_dir_path) for f in fn]
+        # 1. Assert number of copied files are the same.
+        self.assertEqual(len(original), len(copies))
+        # 2. Iterate over all files.
+        for ofp, cfp in zip(original, copies):
+            # Assert their contents are the same.
+            with (
+                open(file=ofp, mode='rb') as of,
+                open(file=cfp, mode='rb') as cp
+            ):
+                self.assertEqual(of.read(), cp.read())
+        # Remove temporary directory.
+        shutil.rmtree(tmp_dir_path)
+
+    def test_transfer_to_on_chunk_size(self):
+        # Create a temporary dictionary.
+        tmp_dir_path = REL_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME)
+        os.mkdir(tmp_dir_path)
+        # Copy the directory's contents into this tmp directory.
+        with self.build_dir() as dir:
+            dir.transfer_to(
+                dst=LocalDir(path=tmp_dir_path),
+                chunk_size=1)
+        # Assert that the two directories contains the same contents.
+        original = [s for s in sorted(os.listdir(ABS_DIR_PATH)) if s.endswith('.txt')]
+        copies = [s for s in sorted(os.listdir(tmp_dir_path))]
+        # 1. Assert number of copied files are the same.
+        self.assertEqual(len(original), len(copies))
+        # 2. Iterate over all files.
+        for ofp, cfp in zip(original, copies):
+            # Assert their contents are the same.
+            with (
+                open(file=join_paths(ABS_DIR_PATH, ofp), mode='rb') as of,
+                open(file=join_paths(tmp_dir_path, cfp), mode='rb') as cp
+            ):
+                self.assertEqual(of.read(), cp.read())
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
     def test_transfer_to_on_overwrite_set_to_false(self):
         # Create a copy of the directory.
-        tmp_dir_name = 'TMP_DIR'
-        tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, tmp_dir_name))
+        tmp_dir_name = TMP_DIR_NAME
+        tmp_dir_path = REL_DIR_PATH.replace(DIR_NAME, tmp_dir_name)
         shutil.copytree(src=ABS_DIR_PATH, dst=tmp_dir_path)
         # While capturing stdout...
         with (
             io.StringIO() as stdo,
             self.build_dir() as dir
         ):
             sys.stdout = stdo
@@ -3272,16 +3923,16 @@
 
             self.assertTrue("Operation unsuccessful" in stdo.getvalue())
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
     def test_transfer_to_on_overwrite_set_to_true(self):
         # Create a copy of the directory.
-        tmp_dir_name = 'TMP_DIR'
-        tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, tmp_dir_name))
+        tmp_dir_name = TMP_DIR_NAME
+        tmp_dir_path = REL_DIR_PATH.replace(DIR_NAME, tmp_dir_name)
         shutil.copytree(src=ABS_DIR_PATH, dst=tmp_dir_path)
         # While capturing stdout...
         with (
             io.StringIO() as stdo,
             self.build_dir() as dir
         ):
             sys.stdout = stdo
@@ -3298,15 +3949,15 @@
 
     def test_transfer_to_on_include_metadata_set_to_false(self):
         # Set metadata for a directory's file.
         filename, metadata = 'file2.txt', {'1': '1'}
         with self.build_dir() as dir:
             dir.set_metadata(file_path=filename, metadata=metadata)
             # Create a temporary dictionary.
-            tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, 'TMP_DIR'))
+            tmp_dir_path = REL_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME)
             os.mkdir(tmp_dir_path)
             tmp_dir = TestLocalDir.build_dir(path=tmp_dir_path)
             # Copy the directory's contents into this
             # tmp directory without including metadata.
             dir.transfer_to(dst=tmp_dir, include_metadata=False)
         # Assert that no metadata have been transfered.
         self.assertEqual(tmp_dir.get_metadata(file_path=filename), {})
@@ -3315,15 +3966,15 @@
 
     def test_transfer_to_on_include_metadata_with_set_metadata(self):
         # Set metadata for a directory's file.
         filename, metadata = DIR_FILE_NAME, {'1': '1'}
         with self.build_dir() as dir:
             dir.set_metadata(file_path=filename, metadata=metadata)
             # Create a temporary dictionary.
-            tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, 'TMP_DIR'))
+            tmp_dir_path = REL_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME)
             os.mkdir(tmp_dir_path)
             tmp_dir = TestLocalDir.build_dir(path=tmp_dir_path)
             # Copy the directory's contents into this
             # tmp directory without including metadata.
             dir.transfer_to(dst=tmp_dir, include_metadata=True)
         # Assert the file's metadata are the same.
         self.assertEqual(
@@ -3333,126 +3984,162 @@
         shutil.rmtree(tmp_dir_path)
 
     def test_transfer_to_on_include_metadata_without_set_metadata(self):
         # Set metadata for a directory's file.
         filename = DIR_FILE_NAME
         with self.build_dir() as dir:
             # Create a temporary dictionary.
-            tmp_dir_path = to_abs(REL_DIR_PATH.replace(DIR_NAME, 'TMP_DIR'))
+            tmp_dir_path = REL_DIR_PATH.replace(DIR_NAME, TMP_DIR_NAME)
             os.mkdir(tmp_dir_path)
             tmp_dir = TestLocalDir.build_dir(path=tmp_dir_path)
             # Copy the directory's contents into this
             # tmp directory without including metadata.
             dir.transfer_to(dst=tmp_dir, include_metadata=True)
         # Assert the file's metadata are the same.
         self.assertEqual(
             tmp_dir.get_metadata(file_path=filename),
             METADATA)
         # Remove temporary directory.
         shutil.rmtree(tmp_dir_path)
 
-    def test_transfer_to_on_include_metadata_to_cloud_dir(self):
-        with mock_s3() as mocks3:
-            # Create AWSS3 bucket.
-            create_aws_s3_bucket(mocks3, BUCKET, METADATA)
-            # Copy directory contents including metadata
-            filename, metadata = DIR_FILE_NAME, {'2': '2'}
+    def test_transfer_to_as_dst(self):
+        # Get source file.
+        src_file = TestLocalFile.build_file()
+        # Create a temporary "blob" dictionary.
+        tmp_dir_path = REL_DIR_PATH.replace('dir', TMP_DIR_NAME)
+        os.mkdir(tmp_dir_path)
+        with self.build_dir(path=tmp_dir_path) as azr_dir:
+            # Copy file into dir.
+            src_file.transfer_to(dst=azr_dir)
+            # Confirm that file was indeed copied.
+            copy_path = join_paths(tmp_dir_path, FILE_NAME)
             with (
-                self.build_dir() as dir,
-                TestAWSS3Dir.build_dir() as aws_dir
+                open(ABS_FILE_PATH, mode='rb') as file,
+                open(copy_path, mode='rb') as copy
             ):
-                dir.set_metadata(file_path=filename, metadata=metadata)
-                dir.transfer_to(dst=aws_dir, overwrite=True, include_metadata=True)
-                # Assert that the object's metadata have been modified.
-                self.assertEqual(
-                    get_aws_s3_object(aws_dir.get_bucket_name(), REL_DIR_FILE_PATH).metadata,
-                    metadata)
-                
-    def test_transfer_to_as_destination(self):
-        # Create a "remote" temporary dictionary.
-        tmp_dir_path = REL_DIR_PATH.replace(DIR_NAME, 'TMP_DIR')
+                self.assertEqual(file.read(), copy.read())
+        shutil.rmtree(tmp_dir_path)
+
+    def test_transfer_to_as_dst_on_chunk_size(self):
+        # Get source file.
+        src_file = TestLocalFile.build_file()
+        # Create a temporary "blob" dictionary.
+        tmp_dir_path = REL_DIR_PATH.replace('dir', TMP_DIR_NAME)
         os.mkdir(tmp_dir_path)
-        # Copy the local dir's contents into this
-        # "remote" tmp directory.
-        with self.build_dir(path=tmp_dir_path) as dir:
-            TestLocalDir.build_dir(REL_DIR_PATH).transfer_to(dir)
-        # Assert that the two directories contain the same contents.
-        self.assertEqual(
-            ''.join(s for s in sorted(os.listdir(REL_DIR_PATH)) if s.endswith('.txt')),
-            ''.join(s for s in sorted(os.listdir(tmp_dir_path))))
-        # Remove temporary directory.
+        with self.build_dir(path=tmp_dir_path) as azr_dir:
+            # Copy file into dir.
+            src_file.transfer_to(dst=azr_dir, chunk_size=1)
+            # Confirm that file was indeed copied.
+            copy_path = join_paths(tmp_dir_path, FILE_NAME)
+            with (
+                open(ABS_FILE_PATH, mode='rb') as file,
+                open(copy_path, mode='rb') as copy
+            ):
+                self.assertEqual(file.read(), copy.read())
         shutil.rmtree(tmp_dir_path)
 
-    def test_traverse_files(self):
-        with self.build_dir() as dir:
+    def test_transfer_to_as_dst_on_include_metadata(self):
+        # Get source file and metadata.
+        src_file = TestLocalFile.build_file()
+        metadata = {'2': '2'}
+        src_file.set_metadata(metadata=metadata)
+        # Create a temporary "blob" dictionary.
+        tmp_dir_path = REL_DIR_PATH.replace('dir', TMP_DIR_NAME)
+        os.mkdir(tmp_dir_path)
+        with self.build_dir(path=tmp_dir_path) as azr_dir:
+            # Copy file into dir.
+            src_file.transfer_to(dst=azr_dir, include_metadata=True)
+            # Confirm that metadata was indeed assigned.
+            copy_path = join_paths(tmp_dir_path, FILE_NAME)
             self.assertEqual(
-                ''.join(map(lambda file: file.get_path(), dir.traverse_files())),
-                ''.join(filter(lambda path: not path.endswith('/'), self.get_abs_contents(recursively=False))))
+                azr_dir.get_metadata(file_path=copy_path),
+                metadata)
+        shutil.rmtree(tmp_dir_path)
 
-    def test_traverse_files_on_recursively(self):
-        with self.build_dir() as dir:
+    def test_transfer_to_as_dst_on_chunk_size_and_include_metadata(self):
+        # Get source file and metadata.
+        src_file = TestLocalFile.build_file()
+        metadata = {'2': '2'}
+        src_file.set_metadata(metadata=metadata)
+        # Create a temporary "blob" dictionary.
+        tmp_dir_path = REL_DIR_PATH.replace('dir', TMP_DIR_NAME)
+        os.mkdir(tmp_dir_path)
+        with self.build_dir(path=tmp_dir_path) as azr_dir:
+            # Copy file into dir.
+            src_file.transfer_to(
+                dst=azr_dir,
+                include_metadata=True,
+                chunk_size=1)
+            # Confirm that metadata was indeed assigned.
+            copy_path = join_paths(tmp_dir_path, FILE_NAME)
             self.assertEqual(
-                ''.join(map(lambda file: file.get_path(), dir.traverse_files(recursively=True))),
-                ''.join(self.get_abs_contents(recursively=True)))
+                azr_dir.get_metadata(file_path=copy_path),
+                metadata)
+        shutil.rmtree(tmp_dir_path)
         
-    def test_get_files(self):
+    def test_get_file(self):
         with self.build_dir() as dir:
-            files = dir.get_files()
-            self.assertEqual(
-                ''.join(map(lambda path: files[path].get_path(), files)),
-                ''.join(filter(lambda path: not path.endswith('/'),
-                    self.get_abs_contents(recursively=False))))
+            file = dir.get_file(DIR_FILE_NAME)
+            self.assertEqual(file.get_path(), REL_DIR_FILE_PATH)
 
-    def test_get_files_on_recursively(self):
+    def test_get_file_on_invalid_path_error(self):
         with self.build_dir() as dir:
-            files = dir.get_files(recursively=True)
-            self.assertEqual(
-                ''.join(map(lambda path: files[path].get_path(), files)),
-                ''.join(self.get_abs_contents(recursively=True)))
-        
-    def test_get_files_on_show_abs_path(self):
+            self.assertRaises(InvalidPathError, dir.get_file, "NON_EXISTING_PATH")
+
+    def test_get_file_on_invalid_file_error(self):
         with self.build_dir() as dir:
-            files = dir.get_files(show_abs_path=True)
-            self.assertEqual(
-                ''.join(files),
-                ''.join(filter(lambda path: not path.endswith('/'),
-                    self.get_abs_contents(recursively=False))))
-        
-    def test_get_files_on_recursively_and_show_abs_path(self):
+            self.assertRaises(InvalidFileError, dir.get_file, DIR_SUBDIR_NAME)
+
+    def test_get_subdir(self):
         with self.build_dir() as dir:
-            files = dir.get_files(recursively=True, show_abs_path=True)
-            self.assertEqual(
-                ''.join(files),
-                ''.join(self.get_abs_contents(recursively=True)))
-        
-    def test_get_file(self):
+            subdir = dir.get_subdir(DIR_SUBDIR_NAME)
+            self.assertEqual(subdir.get_path(), REL_DIR_SUBDIR_PATH)
+
+    def test_get_subdir_on_invalid_path_error(self):
         with self.build_dir() as dir:
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            file = dir.get_file(file_path)
-            self.assertEqual(file.get_path(), REL_DIR_FILE_PATH)
+            self.assertRaises(InvalidPathError, dir.get_subdir, "NON_EXISTING_PATH")
             
     def test_file_shared_metadata_on_modify_from_dir(self):
         with self.build_dir() as dir:
             # Access file via dir.
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            file = dir.get_file(file_path)
+            file = dir.get_file(DIR_FILE_NAME)
             # Change metadata via "Dir" API.
-            dir.set_metadata(file_path, METADATA)
+            dir.set_metadata(DIR_FILE_NAME, METADATA)
             # Assert file metadata have been changed.
             self.assertEqual(file.get_metadata(), METADATA)
 
     def test_file_shared_metadata_on_modify_from_file(self):
         with self.build_dir() as dir:
             # Access file via dir.
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            file = dir.get_file(file_path)
+            file = dir.get_file(DIR_FILE_NAME)
             # Change metadata via "File" API.
             file.set_metadata(METADATA)
             # Assert file metadata have been changed.
-            self.assertEqual(dir.get_metadata(file_path), METADATA)
+            self.assertEqual(dir.get_metadata(DIR_FILE_NAME), METADATA)
+
+    def test_subdir_shared_metadata_on_modify_from_dir(self):
+        # Create dir and get file.
+        with self.build_dir() as dir:
+            subdir = dir.get_subdir(DIR_SUBDIR_NAME)
+            # Change metadata via "Dir" API.
+            dir.set_metadata(
+                DIR_SUBDIR_NAME + DIR_SUBDIR_FILE_NAME, METADATA)
+            # Assert file metadata have been changed.
+            self.assertEqual(
+                subdir.get_metadata(DIR_SUBDIR_FILE_NAME), METADATA)
+
+    def test_subdir_shared_metadata_on_modify_from_subdir(self):
+        # Create dir and get file.
+        with self.build_dir() as dir:
+            subdir = dir.get_subdir(DIR_SUBDIR_NAME)
+            # Change metadata via "File" API.
+            subdir.set_metadata(DIR_SUBDIR_FILE_NAME, METADATA)
+            # Assert file metadata have been changed.
+            self.assertEqual(
+                dir.get_metadata(DIR_SUBDIR_NAME + DIR_SUBDIR_FILE_NAME), METADATA)
         
     '''
     Test connection methods.
     '''
     def test_open(self):
         dir = self.build_dir()
         dir.close()
@@ -3534,15 +4221,14 @@
             # Fetch contents from cache.
             t = time.time()
             _ = (_ for _ in dir.traverse())
             cache_time = time.time() - t
             # Compare fetch times.
             self.assertGreater(normal_time, cache_time)
 
-
     def test_load_metadata_from_cache_on_value(self):
         with self.build_dir(cache=True) as dir:
             dir.load_metadata()
             self.assertEqual(
                 dir.get_metadata(REL_DIR_FILE_PATH),
                 METADATA)
 
@@ -3617,17 +4303,16 @@
 
     def test_file_shared_cache_on_cache_via_dir(self):
         with (
             self.build_dir(cache=False) as no_cache_dir,
             self.build_dir(cache=True) as cache_dir
         ):
             # Access file via both dirs.
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            no_cache_file = no_cache_dir.get_file(file_path)
-            cache_file = cache_dir.get_file(file_path)
+            no_cache_file = no_cache_dir.get_file(DIR_FILE_NAME)
+            cache_file = cache_dir.get_file(DIR_FILE_NAME)
             # Count total size for both dirs.
             _ = no_cache_dir.get_size()
             _ = cache_dir.get_size()
             # Time no-cache-file's "get_size"
             t = time.time()
             _ = no_cache_file.get_size()
             normal_time = time.time() - t
@@ -3640,26 +4325,68 @@
 
     def test_file_shared_cache_on_cache_via_file(self):
         with (
             self.build_dir(cache=False) as no_cache_dir,
             self.build_dir(cache=True) as cache_dir
         ):
             # Count size of files via both dirs using the "File" API.
-            file_path = REL_DIR_FILE_PATH.removeprefix(REL_DIR_PATH)
-            for file in no_cache_dir.get_files().values():
-                _ = file.get_size()
-            for file in cache_dir.get_files().values():
-                _ = file.get_size()
+            for path in no_cache_dir.traverse():
+                try:
+                    _ = no_cache_dir.get_file(path).get_size()
+                    _ = cache_dir.get_file(path).get_size()
+                except:
+                    continue
             # Time no-cache-dir's "get_size"
             t = time.time()
             _ = no_cache_dir.get_size()
             normal_time = time.time() - t
             # Time cache-dir's "get_size"
             t = time.time()
             _ = cache_dir.get_size()
             cache_time = time.time() - t
             # Compare fetch times.
             self.assertGreater(normal_time, cache_time)
 
+    def test_subdir_shared_cache_on_cache_via_dir(self):
+        with (
+            self.build_dir(cache=False) as no_cache_dir,
+            self.build_dir(cache=True) as cache_dir
+        ):
+            # Access subdir via both dirs.
+            no_cache_subdir = no_cache_dir.get_subdir(DIR_SUBDIR_NAME)
+            cache_subdir = cache_dir.get_subdir(DIR_SUBDIR_NAME)
+            # Count total size for both dirs.
+            _ = no_cache_dir.get_size(recursively=True)
+            _ = cache_dir.get_size(recursively=True)
+            # Time no-cache-subdir's "get_size"
+            t = time.time()
+            _ = no_cache_subdir.get_size()
+            normal_time = time.time() - t
+            # Time cache-subdir's "get_size"
+            t = time.time()
+            _ = cache_subdir.get_size()
+            cache_time = time.time() - t
+            # Compare fetch times.
+            self.assertGreater(normal_time, cache_time)
+
+    def test_subdir_shared_cache_on_cache_via_subdir(self):
+        with (
+            self.build_dir(cache=False) as no_cache_dir,
+            self.build_dir(cache=True) as cache_dir
+        ):
+            # Count size of both subdirs.
+            _ = no_cache_dir.get_subdir(DIR_SUBDIR_NAME).get_size()
+            _ = cache_dir.get_subdir(DIR_SUBDIR_NAME).get_size()
+            # Time no-cache-dir's "get_size"
+            t = time.time()
+            _ = no_cache_dir.get_size(recursively=True)
+            normal_time = time.time() - t
+            # Time cache-dir's "get_size"
+            t = time.time()
+            _ = cache_dir.get_size(recursively=True)
+            cache_time = time.time() - t
+            # Compare fetch times.
+            self.assertGreater(normal_time, cache_time)
+
 
 if __name__=="__main__":
     unittest.main()
```

