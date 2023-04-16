# Comparing `tmp/termcs-0.1.0.tar.gz` & `tmp/termcs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/yu/code/python/binance/termcs/dist/.tmp-4_11wvxx/termcs-0.1.0.tar", last modified: Wed Mar 29 14:48:18 2023, max compression
+gzip compressed data, was "/home/yu/code/python/binance/termcs/dist/.tmp-ojjm2ogg/termcs-0.1.1.tar", last modified: Sun Apr 16 12:16:11 2023, max compression
```

## Comparing `termcs-0.1.0.tar` & `termcs-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 yu        (1000) yu        (1000)        0 2023-03-29 14:48:18.000000 termcs-0.1.0/
--rw-r--r--   0 yu        (1000) yu        (1000)     1049 2023-01-08 18:41:43.000000 termcs-0.1.0/LICENSE
--rw-r--r--   0 yu        (1000) yu        (1000)     6363 2023-03-29 14:48:18.000000 termcs-0.1.0/PKG-INFO
--rw-r--r--   0 yu        (1000) yu        (1000)     4372 2023-03-29 14:17:04.000000 termcs-0.1.0/README.md
--rw-r--r--   0 yu        (1000) yu        (1000)     1232 2023-03-29 14:23:44.000000 termcs-0.1.0/pyproject.toml
--rw-r--r--   0 yu        (1000) yu        (1000)       38 2023-03-29 14:48:18.000000 termcs-0.1.0/setup.cfg
-drwxr-xr-x   0 yu        (1000) yu        (1000)        0 2023-03-29 14:48:18.000000 termcs-0.1.0/termcs/
--rw-r--r--   0 yu        (1000) yu        (1000)       51 2023-03-21 11:59:13.000000 termcs-0.1.0/termcs/__init__.py
--rw-r--r--   0 yu        (1000) yu        (1000)     4306 2023-03-29 11:55:41.000000 termcs-0.1.0/termcs/bottomWidget.py
--rw-r--r--   0 yu        (1000) yu        (1000)     7408 2023-03-29 11:24:45.000000 termcs-0.1.0/termcs/cryptoTable.py
--rw-r--r--   0 yu        (1000) yu        (1000)     2273 2023-03-29 13:15:38.000000 termcs-0.1.0/termcs/screener.py
--rw-r--r--   0 yu        (1000) yu        (1000)     2398 2023-03-29 11:51:07.000000 termcs-0.1.0/termcs/termcs.css
--rw-r--r--   0 yu        (1000) yu        (1000)      681 2023-03-29 13:18:15.000000 termcs-0.1.0/termcs/termcs.py
--rw-r--r--   0 yu        (1000) yu        (1000)      642 2023-01-07 17:27:29.000000 termcs-0.1.0/termcs/topWidget.py
--rw-r--r--   0 yu        (1000) yu        (1000)     1105 2023-03-23 14:51:32.000000 termcs-0.1.0/termcs/utils.py
--rw-r--r--   0 yu        (1000) yu        (1000)     9033 2023-03-29 11:07:51.000000 termcs-0.1.0/termcs/worker.py
-drwxr-xr-x   0 yu        (1000) yu        (1000)        0 2023-03-29 14:48:18.000000 termcs-0.1.0/termcs.egg-info/
--rw-r--r--   0 yu        (1000) yu        (1000)     6363 2023-03-29 14:48:18.000000 termcs-0.1.0/termcs.egg-info/PKG-INFO
--rw-r--r--   0 yu        (1000) yu        (1000)      385 2023-03-29 14:48:18.000000 termcs-0.1.0/termcs.egg-info/SOURCES.txt
--rw-r--r--   0 yu        (1000) yu        (1000)        1 2023-03-29 14:48:18.000000 termcs-0.1.0/termcs.egg-info/dependency_links.txt
--rw-r--r--   0 yu        (1000) yu        (1000)       38 2023-03-29 14:48:18.000000 termcs-0.1.0/termcs.egg-info/entry_points.txt
--rw-r--r--   0 yu        (1000) yu        (1000)       34 2023-03-29 14:48:18.000000 termcs-0.1.0/termcs.egg-info/requires.txt
--rw-r--r--   0 yu        (1000) yu        (1000)        7 2023-03-29 14:48:18.000000 termcs-0.1.0/termcs.egg-info/top_level.txt
+drwxr-xr-x   0 yu        (1000) yu        (1000)        0 2023-04-16 12:16:11.000000 termcs-0.1.1/
+-rw-r--r--   0 yu        (1000) yu        (1000)     1049 2023-01-08 18:41:43.000000 termcs-0.1.1/LICENSE
+-rw-r--r--   0 yu        (1000) yu        (1000)     6363 2023-04-16 12:16:11.000000 termcs-0.1.1/PKG-INFO
+-rw-r--r--   0 yu        (1000) yu        (1000)     4372 2023-04-12 13:08:54.000000 termcs-0.1.1/README.md
+-rw-r--r--   0 yu        (1000) yu        (1000)     1232 2023-04-16 12:15:45.000000 termcs-0.1.1/pyproject.toml
+-rw-r--r--   0 yu        (1000) yu        (1000)       38 2023-04-16 12:16:11.000000 termcs-0.1.1/setup.cfg
+drwxr-xr-x   0 yu        (1000) yu        (1000)        0 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs/
+-rw-r--r--   0 yu        (1000) yu        (1000)       51 2023-04-12 13:08:54.000000 termcs-0.1.1/termcs/__init__.py
+-rw-r--r--   0 yu        (1000) yu        (1000)     4306 2023-04-12 13:08:54.000000 termcs-0.1.1/termcs/bottomWidget.py
+-rw-r--r--   0 yu        (1000) yu        (1000)     2239 2023-04-12 18:25:43.000000 termcs-0.1.1/termcs/screener.py
+-rw-r--r--   0 yu        (1000) yu        (1000)     7282 2023-04-16 11:48:35.000000 termcs-0.1.1/termcs/screenerTable.py
+-rw-r--r--   0 yu        (1000) yu        (1000)     2376 2023-04-12 15:02:50.000000 termcs-0.1.1/termcs/termcs.css
+-rw-r--r--   0 yu        (1000) yu        (1000)      563 2023-04-12 15:17:07.000000 termcs-0.1.1/termcs/termcs.py
+-rw-r--r--   0 yu        (1000) yu        (1000)      642 2023-04-12 13:08:54.000000 termcs-0.1.1/termcs/topWidget.py
+-rw-r--r--   0 yu        (1000) yu        (1000)     1511 2023-04-12 15:13:39.000000 termcs-0.1.1/termcs/utils.py
+-rw-r--r--   0 yu        (1000) yu        (1000)     8557 2023-04-16 11:44:43.000000 termcs-0.1.1/termcs/worker.py
+drwxr-xr-x   0 yu        (1000) yu        (1000)        0 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/
+-rw-r--r--   0 yu        (1000) yu        (1000)     6363 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/PKG-INFO
+-rw-r--r--   0 yu        (1000) yu        (1000)      387 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/SOURCES.txt
+-rw-r--r--   0 yu        (1000) yu        (1000)        1 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/dependency_links.txt
+-rw-r--r--   0 yu        (1000) yu        (1000)       38 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/entry_points.txt
+-rw-r--r--   0 yu        (1000) yu        (1000)       34 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/requires.txt
+-rw-r--r--   0 yu        (1000) yu        (1000)        7 2023-04-16 12:16:11.000000 termcs-0.1.1/termcs.egg-info/top_level.txt
```

### Comparing `termcs-0.1.0/LICENSE` & `termcs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `termcs-0.1.0/PKG-INFO` & `termcs-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termcs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Terminal crypto screener
 Author: Riyum
 License: Copyright (c) 2023 Riyum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: termcs Version: 0.1.0 Summary: Terminal crypto
+Metadata-Version: 2.1 Name: termcs Version: 0.1.1 Summary: Terminal crypto
 screener Author: Riyum License: Copyright (c) 2023 Riyum Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
```

### Comparing `termcs-0.1.0/README.md` & `termcs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `termcs-0.1.0/pyproject.toml` & `termcs-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "termcs"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name="Riyum" }]
 description = "Terminal crypto screener"
 requires-python = ">=3.7"
 readme = "README.md"
 license = {file = 'LICENSE'}
 classifiers = [
     "Environment :: Console",
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.11",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
     "License :: OSI Approved :: MIT License",
     ]
 dependencies = [
-    "textual >= 0.15.0",
+    "textual >= 0.19.1",
     "binance-connector",
 ]
 
 [tool.setuptools]
 packages = ["termcs"]
 
 [tool.setuptools.package-data]
```

### Comparing `termcs-0.1.0/termcs/bottomWidget.py` & `termcs-0.1.1/termcs/bottomWidget.py`

 * *Files identical despite different names*

### Comparing `termcs-0.1.0/termcs/cryptoTable.py` & `termcs-0.1.1/termcs/screenerTable.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,229 +1,223 @@
+import re
 from threading import Lock
-from typing import List
 from time import time
-import re
+from typing import List
 
 from rich.text import Text
 from textual.app import ComposeResult
-from textual.reactive import reactive
-from textual.widgets import Static, DataTable, Label
-from textual.containers import Vertical, Horizontal
+from textual.containers import Horizontal, Vertical
 from textual.message import Message
+from textual.reactive import reactive
+from textual.widgets import DataTable, Label, Static
 
-from .worker import STATS_WEIGHT, TERMCS_WEIGHT, WEIGHT_LIMIT, Pair, RequestType, Worker
-from .utils import RepeatedTimer
+from .utils import RepeatedTimer, ShutdownMsg
+from .worker import QuoteCurrency, RequestType, Worker
 
 
-class CryptoTable(Static):
+class ScreenerTable(Static):
     """
-    fetch market data from Binance into DataTable.
+    DataTable filled with market data from Binance.
     child widgets updated by their respect threads that initialized in on_mount()
     """
 
     search_pattern = reactive("", init=False)
     full_table = reactive(False)
     show_pair = reactive(False)
 
     def __init__(self) -> None:
         super().__init__()
         self.worker = Worker(thresh=60)
         self.table = DataTable(zebra_stripes=True, show_cursor=False)
-        self.sort_col = 3  # 24h change
+        self.sort_key = lambda x: x[1]["change24"]  # sort by 24h price change
         self.rev = True
         self.lock = Lock()
-        self.initTable()
 
     def compose(self) -> ComposeResult:
-        yield Vertical(Label("", id="asset_count_label"), classes="label")
-        yield Vertical(Label("", id="eta_label"), classes="label")
-        yield Vertical(Label("", id="warning_label"), classes="label")
+        yield Vertical(Label("", id="pair_count_label"), classes="screener_label")
+        yield Vertical(Label("", id="eta_label"), classes="screener_label")
+        yield Vertical(Label("", id="warning_label"), classes="screener_label")
         yield Horizontal(self.table, id="table")
 
     def on_mount(self) -> None:
-        self.updateTableStats()
+        self.fillWorkerBuffer()
+        self.initTable()
         self.tableStats_caller = RepeatedTimer(1, self.updateTableStats)
-        self.worker_caller = RepeatedTimer(3, self.fillWorkerBuffer)
+        self.refresh_caller = RepeatedTimer(3, self._refresh)
         self.table.focus()
+        self.updateTableStats()
 
     def watch_search_pattern(self) -> None:
-        self.table.clear(True)
-        self.initTable()
+        self.updateTable()
 
     def on_data_table_header_selected(self, msg: Message) -> None:
-        """sort the table according to a selected column index"""
-        self.sort_col = msg.column_index + 1
+        """set the sort key for the selected column and update the table"""
         self.rev = not self.rev
-        self.table.clear(True)
-        self.initTable()
+        if msg.column_index == 0:
+            self.sort_key = None
+        else:
+            keys = list(list(self.worker.buff.values())[0])
+            self.sort_key = lambda x: x[1][keys[msg.column_index]]
+
+        self.updateTable()
 
     def fillWorkerBuffer(self):
-        self.lock.acquire()
-        self.worker.fetchAll()
-        self.lock.release()
+        with self.lock:
+            self.worker.fetchAll()
+
+    def _refresh(self):
+        """fetch market data and fill the DataTable"""
+        self.fillWorkerBuffer()
+        self.app.call_from_thread(self.updateTable)
 
     def fullTable(self) -> None:
         self.full_table = not self.full_table
-        self.table.clear(True)
-        self.initTable()
+        self.updateTable()
 
-    def setPair(self, p: Pair) -> None:
-        self.worker.setPair(p)
-        self.table.clear(True)
-        self.worker_caller.stop()
-        self.fillWorkerBuffer()
-        self.worker_caller.start()
-        self.initTable()
+    def setQuoteCurrency(self, qc: QuoteCurrency) -> bool:
+        if self.worker.setQuoteCurrency(qc):
+            self.fillWorkerBuffer()
+            self.updateTable()
+            return True
+        else:
+            return False
 
     def showPair(self) -> None:
         self.show_pair = not self.show_pair
         self.table.clear(True)
         self.initTable()
 
     def stop(self) -> None:
-        self.active = False
-        self.worker_caller.stop()
+        self.refresh_caller.stop()
         self.tableStats_caller.stop()
 
-    def hasWeight(self) -> bool:
-        """
-        used by the parent widget to check if the stats request
-        can be made by the worker
-        """
-        return self.worker.hasWeightFor(RequestType.STATS, user=True)
-
     def updateTableStats(self) -> None:
         """update the labels above the table"""
 
-        """
-        Since this function is invoked every second,
-        it's worth checking whether the worker has faced any connectivity problems
-        """
+        # check if the worker encountered any connection errors
         if self.worker.kill:
-            self.stop()
-            self.app.exit("Connection problem ,check your internet, aborting...")
+            self.post_message(
+                ShutdownMsg("Connection problem ,check your internet, aborting...")
+            )
 
-        if WEIGHT_LIMIT - TERMCS_WEIGHT - self.worker.used_weight < STATS_WEIGHT:
+        if not self.worker.hasWeightFor(RequestType.STATS, user=True):
             self.query_one("#eta_label", Label).styles.margin = (0, 0)
             self.query_one("#warning_label", Label).styles.margin = (0, 0, 1, 0)
             self.query_one("#warning_label", Label).update(
                 "!!! CHANGE PAIR RESTRICTION ENABLED !!!"
             )
         else:
             self.query_one("#warning_label", Label).styles.margin = (0, 0)
             self.query_one("#eta_label", Label).styles.margin = (0, 0, 1, 0)
             self.query_one("#warning_label", Label).update()
 
-        self.query_one("#asset_count_label", Label).update(
-            f"Assets: {self.worker.asset_count}"
+        self.query_one("#pair_count_label", Label).update(
+            f"Pairs: {self.worker.pair_count}"
         )
 
         eta = int(self.worker.update_time - time())
         self.query_one("#eta_label", Label).update(
             f"Update in: {eta if eta > 0 else 0}s"
         )
 
-    def prepTableData(self, sort: bool = False) -> List[List]:
-        """sort, filter and decorate the assets data, return a list of DataTable rows"""
-
-        # sort the data
-        if sort:
-            keys = list(list(self.worker.buff.values())[0])
-            self.worker.sortBuff(keys[self.sort_col], self.rev)
+    def prepTableData(self) -> List[List]:
+        """sort, filter and decorate the pairs data, return a list of DataTable rows"""
 
-        # get a list of the current assets
-        assets = self.worker.getAssets()
+        # get a sorted list of the current pairs
+        with self.lock:
+            pairs = [
+                [base_cur, data]
+                for base_cur, data in sorted(
+                    self.worker.buff.items(), key=self.sort_key, reverse=self.rev
+                )
+            ]
 
         # full / mini table
-        assets = assets if self.full_table else [*assets[:15], *assets[-15:]]
+        pairs = pairs if self.full_table else [*pairs[:15], *pairs[-15:]]
 
-        # prep filter
-        sp = self.search_pattern
+        # prep filter pattern
         try:
-            pattern = re.compile(sp.upper())
+            pattern = re.compile(self.search_pattern, re.IGNORECASE)
         except re.error:
             pattern = re.compile("")
 
-        # create rows for the DataTable
+        # create rows
         rows = []
-        for asset in assets:
+        for base_cur, data in pairs:
 
             # filter
-            if not pattern.search(asset["asset_name"]):
+            if not pattern.search(base_cur):
                 continue
 
             # decorations
-            name = asset["asset_name"]
+            name = Text(base_cur)
             if self.show_pair:
-                name = Text(asset["asset_name"])
-                name.append(asset["symbol"][-4:], style="#fafab4 italic")
+                name.append(data["quote_cur"], style="#fafab4 italic")
 
-            change = Text(str(asset["change24"]))
+            change = Text(str(data["change24"]))
             change.stylize(
                 "green"
-                if asset["change24"] > 0
-                else ("red" if asset["change24"] < 0 else "")
+                if data["change24"] > 0
+                else ("red" if data["change24"] < 0 else "")
             )
 
-            if asset["price"] < 10**-4:
-                price = f'{asset["price"]:.8f}'
-                high = f'{asset["high"]:.8f}'
-                low = f'{asset["low"]:.8f}'
+            if data["price"] < 10**-4:
+                price = f'{data["price"]:.8f}'
+                high = f'{data["high"]:.8f}'
+                low = f'{data["low"]:.8f}'
             else:
-                price = repr(asset["price"])
-                high = repr(asset["high"])
-                low = repr(asset["low"])
+                price = repr(data["price"])
+                high = repr(data["high"])
+                low = repr(data["low"])
 
-            low_change = repr(asset["low_change"])
-            high_change = repr(asset["high_change"])
+            low_change = repr(data["low_change"])
+            high_change = repr(data["high_change"])
 
             rows.append(
                 [
-                    asset["symbol"],
                     name,
                     price,
                     change,
                     high,
                     low,
                     high_change,
                     low_change,
-                    f'{asset["volume"]:,}',
+                    f'{data["volume"]:,}',
                 ]
             )
 
         return rows
 
-    def initTable(self) -> None:
-        """initialize an empty DataTable"""
+    def updateTable(self):
+        """update the DataTable with new data"""
+        pairs = self.prepTableData()
+        data_order = [str(k[0]) for k in pairs]
+        table_order = [k.value for k in self.table.rows.keys()]
+
+        # reinitialize the rows on sort diff
+        if data_order != table_order:
+            self.table.clear()
+            for pair in pairs:
+                self.table.add_row(*pair, key=str(pair[0]))
+            return
+
+        for pair in pairs:
+            row_k = str(pair[0])
+            for data, col_k in zip(pair[1:], list(self.table.columns.keys())[1:]):
+                self.table.update_cell(row_k, col_k, data)
+
+    def initTable(self):
+        """fill an empty DataTable"""
         self.col_keys = self.table.add_columns(
             *[
                 "Pair" if self.show_pair else "Asset",
                 "Price",
                 "Change",
                 "High",
                 "Low",
                 "High change",
                 "Low change",
                 "Volume",
             ]
         )
-
-        for asset in self.prepTableData(sort=True):
-            self.table.add_row(*asset[1:], key=asset[0])
-
-    def updateTable(self) -> None:
-        """update (an initialized) DataTable"""
-        for asset in self.prepTableData():
-            row_key = asset[0]
-            for data, col_key in zip(asset[2:], self.col_keys[1:]):
-                self.table.update_cell(row_key, col_key, data)
-
-    def _update(self) -> None:
-        """
-        called by a thread from Termcs
-        update the DataTable or clean and initialize on stats update
-        """
-        if self.worker.stats_update:
-            self.table.clear(True)
-            self.initTable()
-        else:
-            self.updateTable()
+        for pair in self.prepTableData():
+            self.table.add_row(*pair, key=str(pair[0]))
```

### Comparing `termcs-0.1.0/termcs/screener.py` & `termcs-0.1.1/termcs/screener.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,65 @@
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.screen import Screen
 from textual.widgets import DataTable, Input
 
 from .bottomWidget import BottomWidget, MyFooter
-from .cryptoTable import CryptoTable
+from .screenerTable import ScreenerTable
 from .topWidget import TopWidget
-from .worker import Pair
+from .utils import ShutdownMsg
+from .worker import QuoteCurrency
 
 
 class Screener(Screen):
 
     BINDINGS = [
         ("q", "quit", "Quit"),
         ("f", "full_table", "Full"),
-        ("b", "change_pair('busd')", "BUSD"),
-        ("t", "change_pair('usdt')", "USDT"),
-        ("o", "change_pair('both')", "Both"),
+        ("b", "set_quote_cur('busd')", "BUSD"),
+        ("t", "set_quote_cur('usdt')", "USDT"),
+        ("o", "set_quote_cur('both')", "Both"),
         ("p", "show_pair", "Pair"),
         Binding("slash", "search", "Search", key_display="/"),
         Binding("escape", "reset_focus", "Focus", False),
     ]
 
     def compose(self) -> ComposeResult:
         yield TopWidget()
-        yield CryptoTable()
+        yield ScreenerTable()
         yield BottomWidget()
 
-    async def action_quit(self) -> None:
-        self.query_one(CryptoTable).stop()
-        await self.app.action_quit()
+    def action_quit(self) -> None:
+        self.post_message(ShutdownMsg())
 
     async def action_full_table(self) -> None:
         self.query_one(BottomWidget).query_one(MyFooter).toggleKey("f")
-        self.query_one(CryptoTable).fullTable()
+        self.query_one(ScreenerTable).fullTable()
 
-    async def action_change_pair(self, p: str) -> None:
-        table = self.query_one(CryptoTable)
+    async def action_set_quote_cur(self, qc: QuoteCurrency) -> None:
+        table = self.query_one(ScreenerTable)
         footer = self.query_one(BottomWidget).query_one(MyFooter)
 
-        if table.hasWeight():
-            if p == "busd":
+        if table.setQuoteCurrency(qc):
+            if qc == QuoteCurrency.BUSD.value:
                 footer.toggleKey("b")
-                table.setPair(Pair.BUSD)
-            elif p == "usdt":
+            elif qc == QuoteCurrency.USDT.value:
                 footer.toggleKey("t")
-                table.setPair(Pair.USDT)
-            elif p == "both":
+            elif qc == QuoteCurrency.BOTH.value:
                 footer.toggleKey("o")
-                table.setPair(Pair.BOTH)
 
     async def action_show_pair(self) -> None:
         self.query_one(BottomWidget).query_one(MyFooter).toggleKey("p")
-        self.query_one(CryptoTable).showPair()
+        self.query_one(ScreenerTable).showPair()
 
     async def action_search(self) -> None:
         self.query_one(BottomWidget).toggle_search = True
 
     async def action_reset_focus(self) -> None:
         self.query_one(BottomWidget).toggle_search = False
         self.query_one(DataTable).focus()
 
     def on_input_changed(self, message: Input.Changed) -> None:
-        self.query_one(CryptoTable).search_pattern = message.value
+        self.query_one(ScreenerTable).search_pattern = message.value
 
-    def refreshTable(self):
-        self.query_one(CryptoTable)._update()
+    def shutdown(self):
+        self.query_one(ScreenerTable).stop()
```

### Comparing `termcs-0.1.0/termcs/termcs.css` & `termcs-0.1.1/termcs/termcs.css`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     background: $background-lighten-2;
     color: $text;
     text-opacity: 85%;
     content-align: center middle;
 }
 
 /* ----------- CryptoTable Labels ----------- */
-.label {
-    /* border: round blue; */
+
+.screener_label {
     height: auto;
     align: center top;
 }
 
 #eta_label {
     margin-bottom: 1;
 }
@@ -60,14 +60,15 @@
 DataTable {
     background: $background;
     color: $text;
     align: center top;
     width: auto;
     height: 91%;
     text-opacity: 85%;
+    scrollbar-gutter: stable;
     /* border: solid red; */
 }
 
 DataTable > .datatable--header {
     text-style: bold;
     background: $primary-background 80%;
     color: $text;
@@ -86,21 +87,20 @@
     color: $text;
 }
 
 DataTable > .datatable--hover {
     background: $panel-lighten-3 50%;
 }
 
-CryptoTable {
+ScreenerTable{
     margin-top: 1;
     height: 100%;
     width: 100%;
     color: $text;
     align: center middle;
-    /* border: solid magenta; */
 }
 
 /* ------------------------------------------- */
 
 BottomWidget {
     dock: bottom;
     color: $text;
```

### Comparing `termcs-0.1.0/termcs/topWidget.py` & `termcs-0.1.1/termcs/topWidget.py`

 * *Files identical despite different names*

### Comparing `termcs-0.1.0/termcs.egg-info/PKG-INFO` & `termcs-0.1.1/termcs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termcs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Terminal crypto screener
 Author: Riyum
 License: Copyright (c) 2023 Riyum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: termcs Version: 0.1.0 Summary: Terminal crypto
+Metadata-Version: 2.1 Name: termcs Version: 0.1.1 Summary: Terminal crypto
 screener Author: Riyum License: Copyright (c) 2023 Riyum Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
```

