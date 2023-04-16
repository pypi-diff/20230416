# Comparing `tmp/ddcci_plasmoid_backend-0.1.4.tar.gz` & `tmp/ddcci_plasmoid_backend-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddcci_plasmoid_backend-0.1.4.tar", max compression
+gzip compressed data, was "ddcci_plasmoid_backend-0.1.5.tar", max compression
```

## Comparing `ddcci_plasmoid_backend-0.1.4.tar` & `ddcci_plasmoid_backend-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     3126 2023-04-11 20:59:26.584966 ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/Node.py
--rw-r--r--   0        0        0     3393 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/Node_test.py
--rw-r--r--   0        0        0      889 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/__init__.py
--rw-r--r--   0        0        0     3484 2023-04-12 12:46:00.782718 ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/__main__.py
--rw-r--r--   0        0        0     6132 2023-04-12 12:46:00.782718 ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/ddcci.py
--rw-r--r--   0        0        0     1967 2023-04-12 12:46:00.786051 ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/ddcci_test.py
--rw-r--r--   0        0        0      631 2023-04-12 12:47:17.500355 ddcci_plasmoid_backend-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 ddcci_plasmoid_backend-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1008 2023-04-16 10:57:22.596457 ddcci_plasmoid_backend-0.1.5/README.md
+-rw-r--r--   0        0        0     3132 2023-04-16 10:14:42.667713 ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/Node.py
+-rw-r--r--   0        0        0     3419 2023-04-16 10:14:42.667713 ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/Node_test.py
+-rw-r--r--   0        0        0      889 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/__init__.py
+-rw-r--r--   0        0        0     3568 2023-04-15 11:26:35.695349 ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/__main__.py
+-rw-r--r--   0        0        0     6132 2023-04-12 12:46:00.782718 ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/ddcci.py
+-rw-r--r--   0        0        0     1967 2023-04-12 12:46:00.786051 ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/ddcci_test.py
+-rw-r--r--   0        0        0     1064 2023-04-16 11:03:51.161773 ddcci_plasmoid_backend-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1947 1970-01-01 00:00:00.000000 ddcci_plasmoid_backend-0.1.5/PKG-INFO
```

### Comparing `ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/Node.py` & `ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/Node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from dataclasses import field
-from typing import Optional
+from typing import Optional, Dict
 
 
 class Node:
     parent: Optional[Node]
     indentation: int
     key: str
     value: str
     children: list[Node] = field(default_factory=list)
 
-    child_by_key: dict[str, Node]
+    child_by_key: Dict[str, Node]
 
     def __init__(self, parent: Optional[Node], indentation: int, key: str = '', value: str = ''):
         """
         Create a new node and set it as the child of the parent.
         """
         self.parent = parent
         self.key = key
```

### Comparing `ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/Node_test.py` & `ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/Node_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from typing import Tuple
+
 import pytest as pytest
 
 from ddcci_plasmoid_backend.Node import Node
 
 
 @pytest.fixture
-def sample_nodes() -> tuple[Node, Node, Node]:
+def sample_nodes() -> Tuple[Node, Node, Node]:
     parent = Node(parent=None, indentation=0)
     child1 = Node(parent=parent, indentation=1, key='key1', value='val1')
     child2 = Node(parent=parent, indentation=1, key='key2', value='val2')
     return parent, child1, child2
 
 
 def test_init(sample_nodes):
```

### Comparing `ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/__init__.py` & `ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/__main__.py` & `ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,35 +10,34 @@
 from typing import NoReturn
 
 import fasteners
 
 from ddcci_plasmoid_backend import ddcci
 from ddcci_plasmoid_backend.__init__ import get_parser
 
-arguments = vars(get_parser().parse_args())
 
-logging.basicConfig(format='%(levelname)s %(name)s: %(message)s',
-                    level=logging.DEBUG if arguments['debug'] else logging.INFO)
-# supress log message `DEBUG asyncio: Using selector: EpollSelector`
-logging.getLogger('asyncio').setLevel(logging.WARNING)
-logger = logging.getLogger(__name__)
-logger.debug(f'Running version {version("ddcci-plasmoid-backend")} in debug mode')
-
-
-def handle_error(error: str | subprocess.CalledProcessError) -> NoReturn:
-    if isinstance(error, subprocess.CalledProcessError):
-        error = err.stderr if err.stderr else err.stdout
-    print(json.dumps({
-        'command': arguments['command'],
-        'error': error.replace('\n', ' ')
-    }))
-    sys.exit(1)
+def main():
+    arguments = vars(get_parser().parse_args())
 
+    logging.basicConfig(format='%(levelname)s %(name)s: %(message)s',
+                        level=logging.DEBUG if arguments['debug'] else logging.INFO)
+    # supress log message `DEBUG asyncio: Using selector: EpollSelector`
+    logging.getLogger('asyncio').setLevel(logging.WARNING)
+    logger = logging.getLogger(__name__)
+    logger.debug(f'Running version {version("ddcci-plasmoid-backend")} in debug mode')
+
+    def handle_error(error: str | subprocess.CalledProcessError) -> NoReturn:
+        if isinstance(error, subprocess.CalledProcessError):
+            error = err.stderr if err.stderr else err.stdout
+        print(json.dumps({
+            'command': arguments['command'],
+            'error': error.replace('\n', ' ')
+        }))
+        sys.exit(1)
 
-if __name__ == '__main__':
     logger.debug(f'Command: {arguments["command"]}')
 
     if arguments['command'] == 'version':
         print(version('ddcci-plasmoid-backend'))
         sys.exit(0)
 
     # include the username in the lock file. Otherwise, if user A creates a lock, user B may not have the permissions
@@ -88,7 +87,11 @@
                     }
                 }))
             except subprocess.CalledProcessError as err:
                 logger.debug(err)
                 handle_error(err)
 
     sys.exit(0)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/ddcci.py` & `ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/ddcci.py`

 * *Files identical despite different names*

### Comparing `ddcci_plasmoid_backend-0.1.4/ddcci_plasmoid_backend/ddcci_test.py` & `ddcci_plasmoid_backend-0.1.5/ddcci_plasmoid_backend/ddcci_test.py`

 * *Files identical despite different names*

