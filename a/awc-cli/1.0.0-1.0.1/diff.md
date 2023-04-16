# Comparing `tmp/awc_cli-1.0.0-py2.py3-none-any.whl.zip` & `tmp/awc_cli-1.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 21514 bytes, number of entries: 18
--rw-r--r--  2.0 unx      122 b- defN 23-Apr-14 17:06 awc_cli/__init__.py
+Zip file size: 21634 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      122 b- defN 23-Apr-16 00:09 awc_cli/__init__.py
 -rw-r--r--  2.0 unx      508 b- defN 23-Apr-15 23:24 awc_cli/__main__.py
 -rw-r--r--  2.0 unx      423 b- defN 23-Apr-15 23:09 awc_cli/config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 17:08 awc_cli/py.typed
 -rw-r--r--  2.0 unx     2506 b- defN 23-Apr-15 22:20 awc_cli/repl.py
 -rw-r--r--  2.0 unx     1790 b- defN 23-Apr-15 23:14 awc_cli/util.py
 -rw-r--r--  2.0 unx      490 b- defN 23-Apr-15 21:10 awc_cli/cmd/__init__.py
--rw-r--r--  2.0 unx     2976 b- defN 23-Apr-15 23:15 awc_cli/cmd/admin_cmds.py
+-rw-r--r--  2.0 unx     3391 b- defN 23-Apr-16 00:10 awc_cli/cmd/admin_cmds.py
 -rw-r--r--  2.0 unx      290 b- defN 23-Apr-15 23:23 awc_cli/cmd/cmds.py
 -rw-r--r--  2.0 unx     3326 b- defN 23-Apr-15 23:23 awc_cli/cmd/mgr.py
 -rw-r--r--  2.0 unx     2335 b- defN 23-Apr-15 23:15 awc_cli/cmd/user_cmds.py
--rw-------  2.0 unx    35115 b- defN 23-Apr-15 23:29 awc_cli-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1092 b- defN 23-Apr-15 23:29 awc_cli-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-15 23:29 awc_cli-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Apr-15 23:29 awc_cli-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-15 23:29 awc_cli-1.0.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-15 23:07 awc_cli-1.0.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1397 b- defN 23-Apr-15 23:29 awc_cli-1.0.0.dist-info/RECORD
-18 files, 52535 bytes uncompressed, 19242 bytes compressed:  63.4%
+-rw-------  2.0 unx    35115 b- defN 23-Apr-16 00:12 awc_cli-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1092 b- defN 23-Apr-16 00:12 awc_cli-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-16 00:12 awc_cli-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Apr-16 00:12 awc_cli-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-16 00:12 awc_cli-1.0.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-15 23:07 awc_cli-1.0.1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1397 b- defN 23-Apr-16 00:12 awc_cli-1.0.1.dist-info/RECORD
+18 files, 52950 bytes uncompressed, 19362 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -27,29 +27,29 @@
 
 Filename: awc_cli/cmd/mgr.py
 Comment: 
 
 Filename: awc_cli/cmd/user_cmds.py
 Comment: 
 
-Filename: awc_cli-1.0.0.dist-info/LICENSE
+Filename: awc_cli-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: awc_cli-1.0.0.dist-info/METADATA
+Filename: awc_cli-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: awc_cli-1.0.0.dist-info/WHEEL
+Filename: awc_cli-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: awc_cli-1.0.0.dist-info/entry_points.txt
+Filename: awc_cli-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: awc_cli-1.0.0.dist-info/top_level.txt
+Filename: awc_cli-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: awc_cli-1.0.0.dist-info/zip-safe
+Filename: awc_cli-1.0.1.dist-info/zip-safe
 Comment: 
 
-Filename: awc_cli-1.0.0.dist-info/RECORD
+Filename: awc_cli-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awc_cli/__init__.py

```diff
@@ -1,7 +1,7 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """awc_cli"""
 
 from typing import Final
 
-__version__: Final[str] = "1.0.0"
+__version__: Final[str] = "1.0.1"
```

## awc_cli/cmd/admin_cmds.py

```diff
@@ -8,15 +8,15 @@
 import awc
 import awc.api
 import awc.sql
 import awc.sql.helpers
 import pypika.queries  # type: ignore
 import sqlparse  # type: ignore
 
-from ..util import run_sql
+from ..util import err, run_sql
 from . import Command
 from .mgr import CommandManager
 
 ADMIN_CMDS: typing.Final[CommandManager] = CommandManager(True)
 
 # generates automatic wrappers for some functions
 for __wrap_sql in (
@@ -126,7 +126,28 @@
             )
         ),
     )
 
     print(f"rejected user's {cmd.cmd!r} application")
 
     return 0
+
+
+@ADMIN_CMDS.new
+@ADMIN_CMDS.nonempty
+def censor(api: awc.Awc, cmd: Command) -> int:
+    """censor a comment
+    usage : censor <id>"""
+
+    try:
+        cid: int = int(cmd.cmd)
+    except ValueError:
+        return err("not a valid comment ID")
+
+    run_sql(
+        api,
+        awc.sql.helpers.censor_comments(awc.sql.Comment.cid == cid),  # type: ignore
+    )
+
+    print(f"censored #{cid}")
+
+    return 0
```

## Comparing `awc_cli-1.0.0.dist-info/LICENSE` & `awc_cli-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awc_cli-1.0.0.dist-info/METADATA` & `awc_cli-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awc-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: cli for https://server.ari-web.xyz/
 Home-page: https://ari-web.xyz/gh/awc-cli
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,comments,api,https,awc
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `awc_cli-1.0.0.dist-info/RECORD` & `awc_cli-1.0.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-awc_cli/__init__.py,sha256=2nb25nc8XIpi38HXTasLA_QMDHyZL1yjs2kuTE_jezM,122
+awc_cli/__init__.py,sha256=BnWDklXSaw-L8oMyeAbit2McjdFCiyX3-ExgbrTMFlc,122
 awc_cli/__main__.py,sha256=4yHZMkIHuTIIDs61cc1graPrMLDf52djTpUrIydnBHI,508
 awc_cli/config.py,sha256=LOb3rgb14ui92pGUmnk63JEiOoTO3VOxF9xFtvzN-Ic,423
 awc_cli/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 awc_cli/repl.py,sha256=W9u9tFpLX5K2Nw-_DfPyTPglUHzdvLs0DGYriJb6I4o,2506
 awc_cli/util.py,sha256=vxJ0DwU9Bwk87H4MfgBg7rkhMWd-aO_xskib4Uxq7To,1790
 awc_cli/cmd/__init__.py,sha256=jwBEdqk3lhwYnMuhY8Srkoo__3FYKd3q9DEv8BpEmeA,490
-awc_cli/cmd/admin_cmds.py,sha256=ZrIDzFKgWcOciP1jOW-JI8uSm9jnzZ4y4p8qm6zYoOU,2976
+awc_cli/cmd/admin_cmds.py,sha256=bLLfdYWGlPGuEcWItutgA-xwAJ-Xyx8OxYjTtVPADk4,3391
 awc_cli/cmd/cmds.py,sha256=dn2mhqcABK0qrdvNNz5PRQ9F5wNXW52nia2Ju6_n9Cw,290
 awc_cli/cmd/mgr.py,sha256=FUA5hl2UqKqoR6bKYwZCJTRg6_9163Lh3n17Rol2w7E,3326
 awc_cli/cmd/user_cmds.py,sha256=iytxNKB7aui4diTDybPnVUWF4ygltr2clqePR2K8v8A,2335
-awc_cli-1.0.0.dist-info/LICENSE,sha256=oo1Q3PR860k723dU4IFQHEp-dmJy49c3F_OdbhlHj88,35115
-awc_cli-1.0.0.dist-info/METADATA,sha256=g0Cr5SQ-hPKJBT2A17LkislNDuBzYp0UPupdzcuyzlU,1092
-awc_cli-1.0.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-awc_cli-1.0.0.dist-info/entry_points.txt,sha256=Bpjz7jmU8iLTFkxixEbvx_03RogoHocK_zDoVsGR8R0,46
-awc_cli-1.0.0.dist-info/top_level.txt,sha256=4NIrO2nFlQFYzCa0gD1_twziYc8me452Za3vtcFWans,8
-awc_cli-1.0.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-awc_cli-1.0.0.dist-info/RECORD,,
+awc_cli-1.0.1.dist-info/LICENSE,sha256=oo1Q3PR860k723dU4IFQHEp-dmJy49c3F_OdbhlHj88,35115
+awc_cli-1.0.1.dist-info/METADATA,sha256=7dEU45WsIEtOUrg0u_U2iRFO1wGkhEmSq7mYETA-e0A,1092
+awc_cli-1.0.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+awc_cli-1.0.1.dist-info/entry_points.txt,sha256=Bpjz7jmU8iLTFkxixEbvx_03RogoHocK_zDoVsGR8R0,46
+awc_cli-1.0.1.dist-info/top_level.txt,sha256=4NIrO2nFlQFYzCa0gD1_twziYc8me452Za3vtcFWans,8
+awc_cli-1.0.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+awc_cli-1.0.1.dist-info/RECORD,,
```

