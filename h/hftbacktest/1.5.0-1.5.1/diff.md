# Comparing `tmp/hftbacktest-1.5.0.tar.gz` & `tmp/hftbacktest-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hftbacktest-1.5.0.tar", last modified: Fri Apr  7 13:49:50 2023, max compression
+gzip compressed data, was "hftbacktest-1.5.1.tar", last modified: Sun Apr 16 13:35:56 2023, max compression
```

## Comparing `hftbacktest-1.5.0.tar` & `hftbacktest-1.5.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-07 13:49:50.597083 hftbacktest-1.5.0/
--rw-r--r--   0 kaz       (1000) kaz       (1000)     1079 2022-11-14 13:24:06.000000 hftbacktest-1.5.0/LICENSE
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     8304 2023-04-07 13:49:50.597083 hftbacktest-1.5.0/PKG-INFO
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     5948 2023-04-05 15:42:48.000000 hftbacktest-1.5.0/README.rst
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-07 13:49:50.593083 hftbacktest-1.5.0/hftbacktest/
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     7007 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/__init__.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)      830 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/assettype.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     7792 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/backtest.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-07 13:49:50.597083 hftbacktest-1.5.0/hftbacktest/data/
--rw-r--r--   0 kaz       (1000) kaz       (1000)     1118 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/data/__init__.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-07 13:49:50.597083 hftbacktest-1.5.0/hftbacktest/data/utils/
--rw-r--r--   0 kaz       (1000) kaz       (1000)       44 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/data/utils/__init__.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)    10186 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/data/utils/binancefutures.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)     1275 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/data/utils/snapshot.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)     5943 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/data/utils/tardis.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)     7534 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/data/validation.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     6194 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/marketdepth.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-07 13:49:50.597083 hftbacktest-1.5.0/hftbacktest/models/
--rw-rw-r--   0 kaz       (1000) kaz       (1000)        0 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/models/__init__.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     7375 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/models/latencies.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     2516 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/models/queue.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     4143 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/order.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-07 13:49:50.597083 hftbacktest-1.5.0/hftbacktest/proc/
--rw-r--r--   0 kaz       (1000) kaz       (1000)        0 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/proc/__init__.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     5831 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/proc/local.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    14751 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/proc/nopartialfillexchange.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)    22059 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/proc/partialfillexchange.py
--rw-r--r--   0 kaz       (1000) kaz       (1000)     5903 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/proc/proc.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     3252 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/reader.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     8902 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/stat.py
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     2149 2023-04-07 10:42:05.000000 hftbacktest-1.5.0/hftbacktest/state.py
-drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-07 13:49:50.597083 hftbacktest-1.5.0/hftbacktest.egg-info/
--rw-rw-r--   0 kaz       (1000) kaz       (1000)     8304 2023-04-07 13:49:50.000000 hftbacktest-1.5.0/hftbacktest.egg-info/PKG-INFO
--rw-rw-r--   0 kaz       (1000) kaz       (1000)      886 2023-04-07 13:49:50.000000 hftbacktest-1.5.0/hftbacktest.egg-info/SOURCES.txt
--rw-rw-r--   0 kaz       (1000) kaz       (1000)        1 2023-04-07 13:49:50.000000 hftbacktest-1.5.0/hftbacktest.egg-info/dependency_links.txt
--rw-rw-r--   0 kaz       (1000) kaz       (1000)        1 2023-02-22 13:33:16.000000 hftbacktest-1.5.0/hftbacktest.egg-info/not-zip-safe
--rw-rw-r--   0 kaz       (1000) kaz       (1000)       48 2023-04-07 13:49:50.000000 hftbacktest-1.5.0/hftbacktest.egg-info/requires.txt
--rw-rw-r--   0 kaz       (1000) kaz       (1000)       12 2023-04-07 13:49:50.000000 hftbacktest-1.5.0/hftbacktest.egg-info/top_level.txt
--rw-r--r--   0 kaz       (1000) kaz       (1000)     1247 2023-04-07 13:49:50.601082 hftbacktest-1.5.0/setup.cfg
--rw-r--r--   0 kaz       (1000) kaz       (1000)       61 2023-02-22 13:27:55.000000 hftbacktest-1.5.0/setup.py
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.435825 hftbacktest-1.5.1/
+-rw-r--r--   0 kaz       (1000) kaz       (1000)     1079 2022-11-14 13:24:06.000000 hftbacktest-1.5.1/LICENSE
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     6872 2023-04-16 13:35:56.435825 hftbacktest-1.5.1/PKG-INFO
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     5763 2023-04-16 13:34:17.000000 hftbacktest-1.5.1/README.rst
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.431825 hftbacktest-1.5.1/hftbacktest/
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)    11501 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/__init__.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     1011 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/assettype.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)    13846 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/backtest.py
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.431825 hftbacktest-1.5.1/hftbacktest/data/
+-rw-r--r--   0 kaz       (1000) kaz       (1000)     1592 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/data/__init__.py
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.431825 hftbacktest-1.5.1/hftbacktest/data/utils/
+-rw-r--r--   0 kaz       (1000) kaz       (1000)       44 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/data/utils/__init__.py
+-rw-r--r--   0 kaz       (1000) kaz       (1000)    11299 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/data/utils/binancefutures.py
+-rw-r--r--   0 kaz       (1000) kaz       (1000)     2160 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/data/utils/snapshot.py
+-rw-r--r--   0 kaz       (1000) kaz       (1000)     6707 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/data/utils/tardis.py
+-rw-r--r--   0 kaz       (1000) kaz       (1000)    11514 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/data/validation.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     6194 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/marketdepth.py
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.435825 hftbacktest-1.5.1/hftbacktest/models/
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)        0 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/models/__init__.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)    10007 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/models/latencies.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     3305 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/models/queue.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     4143 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/order.py
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.435825 hftbacktest-1.5.1/hftbacktest/proc/
+-rw-r--r--   0 kaz       (1000) kaz       (1000)        0 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/proc/__init__.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     5866 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/proc/local.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)    14794 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/proc/nopartialfillexchange.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)    22145 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/proc/partialfillexchange.py
+-rw-r--r--   0 kaz       (1000) kaz       (1000)     5903 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/proc/proc.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     3252 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/reader.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)    13631 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/stat.py
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     2149 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/state.py
+-rw-r--r--   0 kaz       (1000) kaz       (1000)      876 2023-04-16 12:29:54.000000 hftbacktest-1.5.1/hftbacktest/typing.py
+drwxrwxr-x   0 kaz       (1000) kaz       (1000)        0 2023-04-16 13:35:56.431825 hftbacktest-1.5.1/hftbacktest.egg-info/
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)     6872 2023-04-16 13:35:56.000000 hftbacktest-1.5.1/hftbacktest.egg-info/PKG-INFO
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)      908 2023-04-16 13:35:56.000000 hftbacktest-1.5.1/hftbacktest.egg-info/SOURCES.txt
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)        1 2023-04-16 13:35:56.000000 hftbacktest-1.5.1/hftbacktest.egg-info/dependency_links.txt
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)        1 2023-02-22 13:33:16.000000 hftbacktest-1.5.1/hftbacktest.egg-info/not-zip-safe
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)       48 2023-04-16 13:35:56.000000 hftbacktest-1.5.1/hftbacktest.egg-info/requires.txt
+-rw-rw-r--   0 kaz       (1000) kaz       (1000)       12 2023-04-16 13:35:56.000000 hftbacktest-1.5.1/hftbacktest.egg-info/top_level.txt
+-rw-r--r--   0 kaz       (1000) kaz       (1000)     1249 2023-04-16 13:35:56.435825 hftbacktest-1.5.1/setup.cfg
+-rw-r--r--   0 kaz       (1000) kaz       (1000)       61 2023-02-22 13:27:55.000000 hftbacktest-1.5.1/setup.py
```

### Comparing `hftbacktest-1.5.0/LICENSE` & `hftbacktest-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.0/PKG-INFO` & `hftbacktest-1.5.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,181 +1,188 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.5.0
+Version: 1.5.1
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
-Project-URL: Docs, https://github.com/nkaz001/hftbacktest/wiki
+Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
 Project-URL: GitHub: repo, https://github.com/nkaz001/hftbacktest
-Description: ===========
-        HftBacktest
-        ===========
-        
-        |codacy| |codeql| |pypi| |downloads| |license|
-        
-        High-Frequency Trading Backtesting Tool in Python
-        ====================================================================
-        
-        This Python framework is designed for developing high-frequency trading and market-making strategies. It focuses on accounting for both feed and order latencies, as well as the order queue position for order fill simulation. The framework aims to provide more accurate market replay-based backtesting, based on full order book and trade tick feed data.
-        
-        Key Features
-        ============
-        
-        * Working in `Numba <https://numba.pydata.org/>`_ JIT function.
-        * Complete tick-by-tick simulation with a variable time interval.
-        * Full order book reconstruction based on L2 feeds(Market-By-Price).
-        * Backtest accounting for both feed and order latency, using provided models or your own custom model.
-        * Order fill simulation that takes into account the order queue position, using provided models or your own custom model.
-        
-        
-        Getting started
-        ===============
-        
-        Installation
-        ------------
-        
-        hftbacktest supports Python 3.7+. You can install hftbacktest using ``pip``:
-        
-        .. code-block:: console
-        
-         pip install hftbacktest
-        
-        Or you can clone the latest development version from the Git repository with:
-        
-        .. code-block:: console
-        
-         git clone https://github.com/nkaz001/hftbacktest
-        
-        Data Source & Format
-        --------------------
-        
-        Please see `Data <https://github.com/nkaz001/hftbacktest/wiki/Data>`_ or `Data Preparation <https://github.com/nkaz001/hftbacktest/blob/master/examples/Data%20Preparation.ipynb>`_.
-        
-        A Quick Example
-        ---------------
-        
-        Get a glimpse of what backtesting with hftbacktest looks like with these code snippets:
-        
-        .. code-block:: python
-        
-            @njit
-            def simple_two_sided_quote(hbt, stat):
-                max_position = 5
-                half_spread = hbt.tick_size * 20
-                skew = 1
-                order_qty = 0.1 
-                last_order_id = -1
-        
-                bid_order_price_tick_as_id = -1
-                ask_order_price_tick_as_id = -1
-        
-                while hbt.run:
-                    # Check every 0.1s
-                    if not hbt.elapse(0.1 * 1e6):
-                        return False
-        
-                    # Clear cancelled, filled or expired orders.
-                    hbt.clear_inactive_orders()
-        
-                    # Obtain the current mid-price and compute the reservation price.
-                    mid_price = (hbt.best_bid + hbt.best_ask) / 2.0
-                    reservation_price = mid_price - skew * hbt.position * hbt.tick_size
-        
-                    bid_order_price = reservation_price - half_spread
-                    ask_order_price = reservation_price + half_spread
-        
-                    # Cancel the existing bid order.
-                    existing_bid_order = hbt.orders.get(bid_order_price_tick_as_id)
-                    if existing_bid_order is not None and existing_bid_order.cancellable:
-                        hbt.cancel(existing_bid_order.order_id)
-                        last_order_id = existing_bid_order.order_id
-        
-                    # Cancel the existing ask order.
-                    existing_ask_order = hbt.orders.get(ask_order_price_tick_as_id)
-                    if existing_ask_order is not None and existing_ask_order.cancellable:
-                        hbt.cancel(existing_ask_order.order_id)
-                        last_order_id = existing_ask_order.order_id
-        
-                    if hbt.position < max_position:
-                        # Submit a new post-only limit bid order.
-                        bid_order_price_tick_as_id = round(bid_order_price / hbt.tick_size)
-                        hbt.submit_buy_order(
-                            bid_order_price_tick_as_id,
-                            bid_order_price,
-                            order_qty,
-                            GTX
-                        )
-                        last_order_id = bid_order_price_tick_as_id
-        
-                    if hbt.position > -max_position:
-                        # Submit a new post-only limit ask order.
-                        ask_order_price_tick_as_id = round(ask_order_price / hbt.tick_size)
-                        hbt.submit_sell_order(
-                            ask_order_price_tick_as_id,
-                            ask_order_price,
-                            order_qty,
-                            GTX
-                        )
-                        last_order_id = ask_order_price_tick_as_id
-        
-                    # All order requests are considered to be requested at the same time.
-                    # Wait until one of the order responses is received.
-                    if last_order_id >= 0:
-                        hbt.wait_order_response(last_order_id)
-        
-                    # Record the current state for stat calculation.
-                    stat.record(hbt)
-                return True
-        
-            
-        Examples
-        ========
-        
-        You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
-        
-        Documentation
-        =============
-        * `Data <https://github.com/nkaz001/hftbacktest/wiki/Data>`_
-        * `Latency model <https://github.com/nkaz001/hftbacktest/wiki/Latency-model>`_
-        * `Order fill <https://github.com/nkaz001/hftbacktest/wiki/Order-fill>`_
-        
-        .. |python| image:: https://img.shields.io/pypi/pyversions/hftbacktest.svg?style=plastic
-            :alt: |Python Version
-            :target: https://badge.fury.io/py/tensorflow
-        
-        .. |codacy| image:: https://app.codacy.com/project/badge/Grade/e2cef673757a45b18abfc361779feada
-            :alt: |Codacy
-            :target: https://www.codacy.com/gh/nkaz001/hftbacktest/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=nkaz001/hftbacktest&amp;utm_campaign=Badge_Grade
-        
-        .. |codeql| image:: https://github.com/nkaz001/hftbacktest/actions/workflows/codeql.yml/badge.svg?branch=master&event=push
-            :alt: |CodeQL
-            :target: https://github.com/nkaz001/hftbacktest/actions/workflows/codeql.yml
-        
-        .. |pypi| image:: https://badge.fury.io/py/hftbacktest.svg
-            :alt: |Package Version
-            :target: https://pypi.org/project/hftbacktest
-            
-        .. |downloads| image:: https://static.pepy.tech/badge/hftbacktest
-            :alt: |Downloads
-            :target: https://pepy.tech/project/hftbacktest
-        
-        .. |license| image:: https://img.shields.io/badge/License-MIT-green.svg
-            :alt: |License
-            :target: https://github.com/nkaz001/hftbacktest/blob/master/LICENSE
-        
 Keywords: hft,high-frequency trading,trading,market-making,backtest
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Python: >=3.7
+License-File: LICENSE
+
+===========
+HftBacktest
+===========
+
+|codacy| |codeql| |pypi| |downloads| |license| |docs|
+
+High-Frequency Trading Backtesting Tool in Python
+====================================================================
+
+This Python framework is designed for developing high-frequency trading and market-making strategies. It focuses on accounting for both feed and order latencies, as well as the order queue position for order fill simulation. The framework aims to provide more accurate market replay-based backtesting, based on full order book and trade tick feed data.
+
+Key Features
+============
+
+* Working in `Numba <https://numba.pydata.org/>`_ JIT function.
+* Complete tick-by-tick simulation with a variable time interval.
+* Full order book reconstruction based on L2 feeds(Market-By-Price).
+* Backtest accounting for both feed and order latency, using provided models or your own custom model.
+* Order fill simulation that takes into account the order queue position, using provided models or your own custom model.
+
+
+Getting started
+===============
+
+Installation
+------------
+
+hftbacktest supports Python 3.7+. You can install hftbacktest using ``pip``:
+
+.. code-block:: console
+
+ pip install hftbacktest
+
+Or you can clone the latest development version from the Git repository with:
+
+.. code-block:: console
+
+ git clone https://github.com/nkaz001/hftbacktest
+
+Data Source & Format
+--------------------
+
+Please see `Data <https://hftbacktest.readthedocs.io/en/latest/data.html>`_ or `Data Preparation <https://hftbacktest.readthedocs.io/en/latest/tutorials/Data%20Preparation.html>`_.
+
+A Quick Example
+---------------
+
+Get a glimpse of what backtesting with hftbacktest looks like with these code snippets:
+
+.. code-block:: python
+
+    @njit
+    def simple_two_sided_quote(hbt, stat):
+        max_position = 5
+        half_spread = hbt.tick_size * 20
+        skew = 1
+        order_qty = 0.1 
+        last_order_id = -1
+        order_id = 0
+
+        while hbt.run:
+            # Check every 0.1s
+            if not hbt.elapse(0.1 * 1e6):
+                return False
+
+            # Clear cancelled, filled or expired orders.
+            hbt.clear_inactive_orders()
+
+            # Obtain the current mid-price and compute the reservation price.
+            mid_price = (hbt.best_bid + hbt.best_ask) / 2.0
+            reservation_price = mid_price - skew * hbt.position * hbt.tick_size
+
+            buy_order_price = reservation_price - half_spread
+            sell_order_price = reservation_price + half_spread
+
+            last_order_id = -1
+            # Cancel all outstanding orders
+            for order in hbt.orders.values():
+                if order.cancellable:
+                    hbt.cancel(order.order_id)
+                    last_order_id = order.order_id    
+			
+            # All order requests are considered to be requested at the same time.
+            # Wait until one of the order cancellation responses is received.
+            if last_order_id >= 0:
+                hbt.wait_order_response(last_order_id)
+				
+            # Clear cancelled, filled or expired orders.
+            hbt.clear_inactive_orders()
+
+	    last_order_id = -1
+            if hbt.position < max_position:
+                # Submit a new post-only limit bid order.
+                order_id += 1
+                hbt.submit_buy_order(
+                    order_id,
+                    buy_order_price,
+                    order_qty,
+                    GTX
+                )
+                last_order_id = order_id
+
+            if hbt.position > -max_position:
+                # Submit a new post-only limit ask order.
+                order_id += 1
+                hbt.submit_sell_order(
+                    order_id,
+                    sell_order_price,
+                    order_qty,
+                    GTX
+                )
+                last_order_id = order_id
+
+            # All order requests are considered to be requested at the same time.
+            # Wait until one of the order responses is received.
+            if last_order_id >= 0:
+                hbt.wait_order_response(last_order_id)
+
+            # Record the current state for stat calculation.
+            stat.record(hbt)
+        return True
+
+    
+Examples
+========
+
+You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
+
+Documentation
+=============
+
+See `here <https://hftbacktest.readthedocs.io/en/latest/>`_.
+
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/hftbacktest.svg?style=plastic
+    :alt: |Python Version
+    :target: https://badge.fury.io/py/tensorflow
+
+.. |codacy| image:: https://app.codacy.com/project/badge/Grade/e2cef673757a45b18abfc361779feada
+    :alt: |Codacy
+    :target: https://www.codacy.com/gh/nkaz001/hftbacktest/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=nkaz001/hftbacktest&amp;utm_campaign=Badge_Grade
+
+.. |codeql| image:: https://github.com/nkaz001/hftbacktest/actions/workflows/codeql.yml/badge.svg?branch=master&event=push
+    :alt: |CodeQL
+    :target: https://github.com/nkaz001/hftbacktest/actions/workflows/codeql.yml
+
+.. |pypi| image:: https://badge.fury.io/py/hftbacktest.svg
+    :alt: |Package Version
+    :target: https://pypi.org/project/hftbacktest
+    
+.. |downloads| image:: https://static.pepy.tech/badge/hftbacktest
+    :alt: |Downloads
+    :target: https://pepy.tech/project/hftbacktest
+
+.. |license| image:: https://img.shields.io/badge/License-MIT-green.svg
+    :alt: |License
+    :target: https://github.com/nkaz001/hftbacktest/blob/master/LICENSE
+    
+.. |docs| image:: https://readthedocs.org/projects/hftbacktest/badge/?version=latest
+    :target: https://hftbacktest.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
```

### Comparing `hftbacktest-1.5.0/README.rst` & `hftbacktest-1.5.1/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===========
 HftBacktest
 ===========
 
-|codacy| |codeql| |pypi| |downloads| |license|
+|codacy| |codeql| |pypi| |downloads| |license| |docs|
 
 High-Frequency Trading Backtesting Tool in Python
 ====================================================================
 
 This Python framework is designed for developing high-frequency trading and market-making strategies. It focuses on accounting for both feed and order latencies, as well as the order queue position for order fill simulation. The framework aims to provide more accurate market replay-based backtesting, based on full order book and trade tick feed data.
 
 Key Features
@@ -36,15 +36,15 @@
 .. code-block:: console
 
  git clone https://github.com/nkaz001/hftbacktest
 
 Data Source & Format
 --------------------
 
-Please see `Data <https://github.com/nkaz001/hftbacktest/wiki/Data>`_ or `Data Preparation <https://github.com/nkaz001/hftbacktest/blob/master/examples/Data%20Preparation.ipynb>`_.
+Please see `Data <https://hftbacktest.readthedocs.io/en/latest/data.html>`_ or `Data Preparation <https://hftbacktest.readthedocs.io/en/latest/tutorials/Data%20Preparation.html>`_.
 
 A Quick Example
 ---------------
 
 Get a glimpse of what backtesting with hftbacktest looks like with these code snippets:
 
 .. code-block:: python
@@ -52,66 +52,68 @@
     @njit
     def simple_two_sided_quote(hbt, stat):
         max_position = 5
         half_spread = hbt.tick_size * 20
         skew = 1
         order_qty = 0.1 
         last_order_id = -1
-
-        bid_order_price_tick_as_id = -1
-        ask_order_price_tick_as_id = -1
+        order_id = 0
 
         while hbt.run:
             # Check every 0.1s
             if not hbt.elapse(0.1 * 1e6):
                 return False
 
             # Clear cancelled, filled or expired orders.
             hbt.clear_inactive_orders()
 
             # Obtain the current mid-price and compute the reservation price.
             mid_price = (hbt.best_bid + hbt.best_ask) / 2.0
             reservation_price = mid_price - skew * hbt.position * hbt.tick_size
 
-            bid_order_price = reservation_price - half_spread
-            ask_order_price = reservation_price + half_spread
+            buy_order_price = reservation_price - half_spread
+            sell_order_price = reservation_price + half_spread
 
-            # Cancel the existing bid order.
-            existing_bid_order = hbt.orders.get(bid_order_price_tick_as_id)
-            if existing_bid_order is not None and existing_bid_order.cancellable:
-                hbt.cancel(existing_bid_order.order_id)
-                last_order_id = existing_bid_order.order_id
-
-            # Cancel the existing ask order.
-            existing_ask_order = hbt.orders.get(ask_order_price_tick_as_id)
-            if existing_ask_order is not None and existing_ask_order.cancellable:
-                hbt.cancel(existing_ask_order.order_id)
-                last_order_id = existing_ask_order.order_id
+            last_order_id = -1
+            # Cancel all outstanding orders
+            for order in hbt.orders.values():
+                if order.cancellable:
+                    hbt.cancel(order.order_id)
+                    last_order_id = order.order_id    
+			
+            # All order requests are considered to be requested at the same time.
+            # Wait until one of the order cancellation responses is received.
+            if last_order_id >= 0:
+                hbt.wait_order_response(last_order_id)
+				
+            # Clear cancelled, filled or expired orders.
+            hbt.clear_inactive_orders()
 
+	    last_order_id = -1
             if hbt.position < max_position:
                 # Submit a new post-only limit bid order.
-                bid_order_price_tick_as_id = round(bid_order_price / hbt.tick_size)
+                order_id += 1
                 hbt.submit_buy_order(
-                    bid_order_price_tick_as_id,
-                    bid_order_price,
+                    order_id,
+                    buy_order_price,
                     order_qty,
                     GTX
                 )
-                last_order_id = bid_order_price_tick_as_id
+                last_order_id = order_id
 
             if hbt.position > -max_position:
                 # Submit a new post-only limit ask order.
-                ask_order_price_tick_as_id = round(ask_order_price / hbt.tick_size)
+                order_id += 1
                 hbt.submit_sell_order(
-                    ask_order_price_tick_as_id,
-                    ask_order_price,
+                    order_id,
+                    sell_order_price,
                     order_qty,
                     GTX
                 )
-                last_order_id = ask_order_price_tick_as_id
+                last_order_id = order_id
 
             # All order requests are considered to be requested at the same time.
             # Wait until one of the order responses is received.
             if last_order_id >= 0:
                 hbt.wait_order_response(last_order_id)
 
             # Record the current state for stat calculation.
@@ -122,17 +124,17 @@
 Examples
 ========
 
 You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
 
 Documentation
 =============
-* `Data <https://github.com/nkaz001/hftbacktest/wiki/Data>`_
-* `Latency model <https://github.com/nkaz001/hftbacktest/wiki/Latency-model>`_
-* `Order fill <https://github.com/nkaz001/hftbacktest/wiki/Order-fill>`_
+
+See `here <https://hftbacktest.readthedocs.io/en/latest/>`_.
+
 
 .. |python| image:: https://img.shields.io/pypi/pyversions/hftbacktest.svg?style=plastic
     :alt: |Python Version
     :target: https://badge.fury.io/py/tensorflow
 
 .. |codacy| image:: https://app.codacy.com/project/badge/Grade/e2cef673757a45b18abfc361779feada
     :alt: |Codacy
@@ -149,7 +151,12 @@
 .. |downloads| image:: https://static.pepy.tech/badge/hftbacktest
     :alt: |Downloads
     :target: https://pepy.tech/project/hftbacktest
 
 .. |license| image:: https://img.shields.io/badge/License-MIT-green.svg
     :alt: |License
     :target: https://github.com/nkaz001/hftbacktest/blob/master/LICENSE
+    
+.. |docs| image:: https://readthedocs.org/projects/hftbacktest/badge/?version=latest
+    :target: https://hftbacktest.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
```

### Comparing `hftbacktest-1.5.0/hftbacktest/data/utils/binancefutures.py` & `hftbacktest-1.5.1/hftbacktest/data/utils/binancefutures.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,62 @@
 import gzip
 import json
+from typing import Optional, Literal
 
 import numpy as np
+from numpy.typing import NDArray
 
-from hftbacktest import correct, validate_data
+from .. import correct, validate_data
 
 
-def convert(input_filename, output_filename=None, opt='', base_latency=0):
-    """
-    Collected Binance Futures stream file sample.
+def convert(
+        input_filename: str,
+        output_filename: Optional[str] = None,
+        opt: Literal['', 'm', 't', 'mt'] = '',
+        base_latency: float = 0
+) -> NDArray:
+    r"""
+    Converts raw Binance Futures feed stream file into a format compatible with HftBacktest.
+
+    File Format:
+
+    .. code-block::
+
+        local_timestamp raw_stream
+        1660228023037049 {"stream":"btcusdt@depth@0ms","data":{"e":"depthUpdate","E":1660228023941,"T":1660228023931,"s":"BTCUSDT","U":1801732831593,"u":1801732832589,"pu":1801732831561,"b":[["2467.10","0.000"],["12006.00","0.001"],["24427.70","4.350"],["24620.30","0.172"],["24644.00","44.832"],["24645.40","0.203"],["24652.80","4.900"],["24664.10","4.279"],["24666.50","0.554"],["24666.80","6.764"],["24668.70","7.428"],["24670.90","2.000"],["24671.00","0.000"],["24672.70","0.000"],["24688.30","0.000"]],"a":[["24653.60","0.000"],["24669.80","0.000"],["24670.20","0.000"],["24670.70","0.000"],["24670.90","0.000"],["24671.00","20.812"],["24672.10","0.000"],["24672.30","0.001"],["24674.60","1.520"],["24674.80","0.000"],["24684.20","4.519"],["24684.30","0.202"],["24685.00","0.937"],["24690.90","4.827"],["24693.60","1.500"],["24729.10","0.171"]]}}
+        1660228023038319 {"stream":"btcusdt@depth@0ms","data":{"e":"depthUpdate","E":1660228023977,"T":1660228023966,"s":"BTCUSDT","U":1801732832805,"u":1801732834115,"pu":1801732832589,"b":[["2467.10","0.008"],["24643.00","4.457"],["24656.30","0.010"],["24657.70","0.005"],["24658.80","1.000"],["24658.90","1.500"],["24659.50","3.781"],["24659.70","1.806"],["24659.90","0.105"],["24660.60","0.787"],["24666.30","5.033"],["24666.40","0.012"],["24666.50","0.556"],["24668.70","7.426"],["24668.90","0.000"],["24670.90","2.535"],["24680.00","0.000"],["24688.30","0.000"]],"a":[["24653.60","0.000"],["24670.10","0.000"],["24670.60","0.000"],["24670.70","0.000"],["24670.90","0.000"],["24671.00","20.642"],["24672.00","0.000"],["24672.10","0.000"],["24673.50","0.145"],["24673.60","1.567"],["24674.50","3.746"],["24674.60","1.520"],["24678.30","1.304"],["24678.40","0.001"],["24678.80","0.546"],["24678.90","0.002"],["24681.60","0.020"],["24681.70","0.613"],["24681.90","0.077"],["24682.10","3.000"],["24682.20","0.000"],["24683.70","0.163"],["24683.80","4.162"],["24684.00","1.227"],["24684.20","4.519"],["24684.30","0.202"],["24684.90","1.331"],["24685.70","0.156"],["24685.80","0.325"],["24686.70","0.648"],["24692.60","0.040"],["24700.00","47.420"],["24729.10","0.006"]]}}
+        1660228023043260 {"stream":"btcusdt@trade","data":{"e":"trade","E":1660228023980,"T":1660228023973,"s":"BTCUSDT","t":2691833663,"p":"24670.90","q":"0.022","X":"MARKET","m":true}}
+        1660228023052991 {"stream":"btcusdt@trade","data":{"e":"trade","E":1660228023991,"T":1660228023983,"s":"BTCUSDT","t":2691833664,"p":"24671.00","q":"0.001","X":"MARKET","m":false}}
+        1660228023071108 {"stream":"btcusdt@depth@0ms","data":{"e":"depthUpdate","E":1660228024010,"T":1660228024002,"s":"BTCUSDT","U":1801732834136,"u":1801732835323,"pu":1801732834115,"b":[["2467.10","0.000"],["12006.00","0.000"],["24599.40","0.641"],["24603.20","0.104"],["24625.50","0.152"],["24645.20","0.476"],["24646.80","0.081"],["24652.60","0.254"],["24664.10","4.279"],["24666.50","0.878"],["24668.80","0.004"],["24670.90","2.513"],["24688.30","0.000"],["24787.00","0.000"]],"a":[["24653.60","0.000"],["24668.10","0.000"],["24668.70","0.000"],["24669.50","0.000"],["24669.80","0.000"],["24670.00","0.000"],["24670.60","0.000"],["24670.70","0.000"],["24670.90","0.000"],["24671.00","20.641"],["24672.20","0.000"],["24672.30","0.001"],["24673.50","0.040"],["24673.90","0.105"],["24674.70","2.139"],["24674.80","0.000"],["24683.70","0.963"],["24683.90","0.009"],["24685.70","0.556"],["24709.30","0.254"],["24723.80","0.000"],["24728.30","0.193"],["24729.50","4.477"],["24739.40","0.807"],["24743.20","0.235"],["24795.00","0.130"]]}}
+        1660228023117894 {"stream":"btcusdt@depth@0ms","data":{"e":"depthUpdate","E":1660228024044,"T":1660228024034,"s":"BTCUSDT","U":1801732835406,"u":1801732836571,"pu":1801732835323,"b":[["2467.10","0.000"],["24337.10","2.462"],["24616.50","1.050"],["24619.00","0.235"],["24640.00","5.148"],["24649.80","2.805"],["24650.00","14.374"],["24651.90","3.000"],["24653.30","1.400"],["24658.70","1.142"],["24658.80","0.000"],["24659.60","3.263"],["24659.70","0.006"],["24660.50","0.840"],["24660.60","0.387"],["24662.20","0.202"],["24663.10","7.147"],["24664.00","0.922"],["24664.20","0.131"],["24664.50","0.027"],["24666.20","7.066"],["24666.40","0.012"],["24668.80","0.002"],["24669.30","0.002"],["24670.20","0.811"],["24670.90","5.817"],["24688.30","0.000"]],"a":[["24653.60","0.000"],["24669.80","0.000"],["24669.90","0.000"],["24670.90","0.000"],["24671.00","20.121"],["24672.10","0.000"],["24672.80","0.000"],["24674.60","1.520"],["24675.30","0.421"],["24681.20","0.239"],["24681.50","1.343"],["24681.60","0.020"],["24681.70","0.213"],["24683.60","2.929"],["24683.70","0.163"],["24683.80","2.162"],["24684.70","0.646"],["24684.90","0.731"],["24692.90","0.321"],["24693.10","0.040"],["24700.70","0.537"],["24703.60","0.210"],["24721.50","7.245"]]}}
+        1660228023125009 {"stream":"btcusdt@trade","data":{"e":"trade","E":1660228024062,"T":1660228024055,"s":"BTCUSDT","t":2691833665,"p":"24670.90","q":"0.002","X":"MARKET","m":true}}
+        1660228023128966 {"stream":"btcusdt@trade","data":{"e":"trade","E":1660228024067,"T":1660228024061,"s":"BTCUSDT","t":2691833666,"p":"24670.90","q":"0.020","X":"MARKET","m":true}}
+        1660228023138740 {"stream":"btcusdt@depth@0ms","data":{"e":"depthUpdate","E":1660228024077,"T":1660228024066,"s":"BTCUSDT","U":1801732836639,"u":1801732837803,"pu":1801732836571,"b":[["2467.10","0.000"],["24659.00","0.000"],["24659.30","2.500"],["24663.00","1.038"],["24664.20","0.118"],["24666.20","7.065"],["24666.50","0.554"],["24666.70","3.987"],["24666.80","7.088"],["24666.90","0.014"],["24667.40","1.506"],["24668.90","0.006"],["24670.10","0.272"],["24670.90","6.726"],["24688.30","0.000"]],"a":[["24653.60","0.000"],["24668.70","0.000"],["24670.30","0.000"],["24670.50","0.000"],["24670.90","0.000"],["24679.00","0.001"],["24703.10","1.500"],["24710.50","0.057"],["24728.30","0.028"],["24768.50","0.318"],["24980.10","5.446"],["25050.00","119.300"]]}}
+        1660228023149748 {"stream":"btcusdt@trade","data":{"e":"trade","E":1660228024088,"T":1660228024081,"s":"BTCUSDT","t":2691833667,"p":"24671.00","q":"0.063","X":"MARKET","m":false}}
+
+    Args:
+        input_filename: Input filename with path.
+        output_filename: If provided, the converted data will be saved to the specified filename in ``npz`` format.
+        opt: Additional processing options:
+
+             - ``m``: Processes ``markPriceUpdate`` stream with the following custom event IDs.
+
+                - index: ``100``
+                - mark price: ``101``
+                - funding rate: ``102``
+
+             - ``t``: Processes ``bookTicker`` stream with the following custom event IDs.
+
+                - best bid: ``103``
+                - best ask: ``104``
 
-    local_timestamp raw_stream
-    1660228023037049 {"stream":"btcusdt@depth@0ms","data":{"e":"depthUpdate","E":1660228023941,"T":1660228023931,"s":"BTCUSDT","U":1801732831593,"u":1801732832589,"pu":1801732831561,"b":[["2467.10","0.000"],["12006.00","0.001"],["24427.70","4.350"],["24620.30","0.172"],["24644.00","44.832"],["24645.40","0.203"],["24652.80","4.900"],["24664.10","4.279"],["24666.50","0.554"],["24666.80","6.764"],["24668.70","7.428"],["24670.90","2.000"],["24671.00","0.000"],["24672.70","0.000"],["24688.30","0.000"]],"a":[["24653.60","0.000"],["24669.80","0.000"],["24670.20","0.000"],["24670.70","0.000"],["24670.90","0.000"],["24671.00","20.812"],["24672.10","0.000"],["24672.30","0.001"],["24674.60","1.520"],["24674.80","0.000"],["24684.20","4.519"],["24684.30","0.202"],["24685.00","0.937"],["24690.90","4.827"],["24693.60","1.500"],["24729.10","0.171"]]}}
-    1660228023038319 {"stream":"btcusdt@depth@0ms","data":{"e":"depthUpdate","E":1660228023977,"T":1660228023966,"s":"BTCUSDT","U":1801732832805,"u":1801732834115,"pu":1801732832589,"b":[["2467.10","0.008"],["24643.00","4.457"],["24656.30","0.010"],["24657.70","0.005"],["24658.80","1.000"],["24658.90","1.500"],["24659.50","3.781"],["24659.70","1.806"],["24659.90","0.105"],["24660.60","0.787"],["24666.30","5.033"],["24666.40","0.012"],["24666.50","0.556"],["24668.70","7.426"],["24668.90","0.000"],["24670.90","2.535"],["24680.00","0.000"],["24688.30","0.000"]],"a":[["24653.60","0.000"],["24670.10","0.000"],["24670.60","0.000"],["24670.70","0.000"],["24670.90","0.000"],["24671.00","20.642"],["24672.00","0.000"],["24672.10","0.000"],["24673.50","0.145"],["24673.60","1.567"],["24674.50","3.746"],["24674.60","1.520"],["24678.30","1.304"],["24678.40","0.001"],["24678.80","0.546"],["24678.90","0.002"],["24681.60","0.020"],["24681.70","0.613"],["24681.90","0.077"],["24682.10","3.000"],["24682.20","0.000"],["24683.70","0.163"],["24683.80","4.162"],["24684.00","1.227"],["24684.20","4.519"],["24684.30","0.202"],["24684.90","1.331"],["24685.70","0.156"],["24685.80","0.325"],["24686.70","0.648"],["24692.60","0.040"],["24700.00","47.420"],["24729.10","0.006"]]}}
-    1660228023043260 {"stream":"btcusdt@trade","data":{"e":"trade","E":1660228023980,"T":1660228023973,"s":"BTCUSDT","t":2691833663,"p":"24670.90","q":"0.022","X":"MARKET","m":true}}
-    1660228023052991 {"stream":"btcusdt@trade","data":{"e":"trade","E":1660228023991,"T":1660228023983,"s":"BTCUSDT","t":2691833664,"p":"24671.00","q":"0.001","X":"MARKET","m":false}}
-    1660228023071108 {"stream":"btcusdt@depth@0ms","data":{"e":"depthUpdate","E":1660228024010,"T":1660228024002,"s":"BTCUSDT","U":1801732834136,"u":1801732835323,"pu":1801732834115,"b":[["2467.10","0.000"],["12006.00","0.000"],["24599.40","0.641"],["24603.20","0.104"],["24625.50","0.152"],["24645.20","0.476"],["24646.80","0.081"],["24652.60","0.254"],["24664.10","4.279"],["24666.50","0.878"],["24668.80","0.004"],["24670.90","2.513"],["24688.30","0.000"],["24787.00","0.000"]],"a":[["24653.60","0.000"],["24668.10","0.000"],["24668.70","0.000"],["24669.50","0.000"],["24669.80","0.000"],["24670.00","0.000"],["24670.60","0.000"],["24670.70","0.000"],["24670.90","0.000"],["24671.00","20.641"],["24672.20","0.000"],["24672.30","0.001"],["24673.50","0.040"],["24673.90","0.105"],["24674.70","2.139"],["24674.80","0.000"],["24683.70","0.963"],["24683.90","0.009"],["24685.70","0.556"],["24709.30","0.254"],["24723.80","0.000"],["24728.30","0.193"],["24729.50","4.477"],["24739.40","0.807"],["24743.20","0.235"],["24795.00","0.130"]]}}
-    1660228023117894 {"stream":"btcusdt@depth@0ms","data":{"e":"depthUpdate","E":1660228024044,"T":1660228024034,"s":"BTCUSDT","U":1801732835406,"u":1801732836571,"pu":1801732835323,"b":[["2467.10","0.000"],["24337.10","2.462"],["24616.50","1.050"],["24619.00","0.235"],["24640.00","5.148"],["24649.80","2.805"],["24650.00","14.374"],["24651.90","3.000"],["24653.30","1.400"],["24658.70","1.142"],["24658.80","0.000"],["24659.60","3.263"],["24659.70","0.006"],["24660.50","0.840"],["24660.60","0.387"],["24662.20","0.202"],["24663.10","7.147"],["24664.00","0.922"],["24664.20","0.131"],["24664.50","0.027"],["24666.20","7.066"],["24666.40","0.012"],["24668.80","0.002"],["24669.30","0.002"],["24670.20","0.811"],["24670.90","5.817"],["24688.30","0.000"]],"a":[["24653.60","0.000"],["24669.80","0.000"],["24669.90","0.000"],["24670.90","0.000"],["24671.00","20.121"],["24672.10","0.000"],["24672.80","0.000"],["24674.60","1.520"],["24675.30","0.421"],["24681.20","0.239"],["24681.50","1.343"],["24681.60","0.020"],["24681.70","0.213"],["24683.60","2.929"],["24683.70","0.163"],["24683.80","2.162"],["24684.70","0.646"],["24684.90","0.731"],["24692.90","0.321"],["24693.10","0.040"],["24700.70","0.537"],["24703.60","0.210"],["24721.50","7.245"]]}}
-    1660228023125009 {"stream":"btcusdt@trade","data":{"e":"trade","E":1660228024062,"T":1660228024055,"s":"BTCUSDT","t":2691833665,"p":"24670.90","q":"0.002","X":"MARKET","m":true}}
-    1660228023128966 {"stream":"btcusdt@trade","data":{"e":"trade","E":1660228024067,"T":1660228024061,"s":"BTCUSDT","t":2691833666,"p":"24670.90","q":"0.020","X":"MARKET","m":true}}
-    1660228023138740 {"stream":"btcusdt@depth@0ms","data":{"e":"depthUpdate","E":1660228024077,"T":1660228024066,"s":"BTCUSDT","U":1801732836639,"u":1801732837803,"pu":1801732836571,"b":[["2467.10","0.000"],["24659.00","0.000"],["24659.30","2.500"],["24663.00","1.038"],["24664.20","0.118"],["24666.20","7.065"],["24666.50","0.554"],["24666.70","3.987"],["24666.80","7.088"],["24666.90","0.014"],["24667.40","1.506"],["24668.90","0.006"],["24670.10","0.272"],["24670.90","6.726"],["24688.30","0.000"]],"a":[["24653.60","0.000"],["24668.70","0.000"],["24670.30","0.000"],["24670.50","0.000"],["24670.90","0.000"],["24679.00","0.001"],["24703.10","1.500"],["24710.50","0.057"],["24728.30","0.028"],["24768.50","0.318"],["24980.10","5.446"],["25050.00","119.300"]]}}
-    1660228023149748 {"stream":"btcusdt@trade","data":{"e":"trade","E":1660228024088,"T":1660228024081,"s":"BTCUSDT","t":2691833667,"p":"24671.00","q":"0.063","X":"MARKET","m":false}}
+        base_latency: The value to be added to the feed latency.
+                      See :func:`.correct_local_timestamp`.
+    Returns:
+        Converted data compatible with HftBacktest.
     """
     rows = []
     with gzip.open(input_filename, 'r') as f:
         while True:
             line = f.readline()
             if not line:
                 break
```

### Comparing `hftbacktest-1.5.0/hftbacktest/data/validation.py` & `hftbacktest-1.5.1/hftbacktest/data/validation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 import sys
+from typing import Optional, Union, Literal
 
 import numpy as np
 import pandas as pd
 from numba import njit
+from numpy.typing import NDArray
+from pandas import DataFrame
 
-from ..reader import COL_EVENT, COL_EXCH_TIMESTAMP, COL_LOCAL_TIMESTAMP, COL_PRICE, COL_QTY, TRADE_EVENT, \
-    DEPTH_EVENT, DEPTH_CLEAR_EVENT, DEPTH_SNAPSHOT_EVENT
+from ..reader import (
+    COL_EVENT,
+    COL_EXCH_TIMESTAMP,
+    COL_LOCAL_TIMESTAMP,
+    COL_PRICE,
+    COL_QTY,
+    TRADE_EVENT,
+    DEPTH_EVENT,
+    DEPTH_CLEAR_EVENT,
+    DEPTH_SNAPSHOT_EVENT
+)
+
+
+Data = Union[NDArray, DataFrame]
 
 
 @njit
 def _validate_data(
         data,
         tick_size=None,
         lot_size=None,
@@ -68,19 +83,38 @@
         if local_timestamp != -1:
             prev_local_timestamp = local_timestamp
 
     return num_reversed_exch_timestamp
 
 
 def validate_data(
-        data,
-        tick_size=None,
-        lot_size=None,
-        err_bound=1e-8
-):
+        data: Data,
+        tick_size: Optional[float] = None,
+        lot_size: Optional[float] = None,
+        err_bound: float = 1e-8
+) -> int:
+    r"""
+    Validates the specified data for the following aspects, excluding user events. Validation results will be printed out:
+
+        - Ensures data's price aligns with tick_size.
+        - Ensures data's quantity aligns with lot_size.
+        - Ensures data's local timestamp is ordered.
+        - Ensures data's exchange timestamp is ordered.
+
+    Args:
+        data: Data to be validated.
+        tick_size: Minimum price increment for the given asset.
+        lot_size: Minimum order quantity for the given asset.
+        err_bound: Error bound used to verify if the specified ``tick_size`` or ``lot_size`` aligns with the price and
+                   quantity.
+
+    Returns:
+        The number of rows with reversed exchange timestamps.
+    """
+
     if isinstance(data, pd.DataFrame):
         num_reversed_exch_timestamp = _validate_data(data.to_numpy(), tick_size, lot_size, err_bound)
     elif isinstance(data, np.ndarray):
         num_reversed_exch_timestamp = _validate_data(data, tick_size, lot_size, err_bound)
     else:
         raise ValueError('Unsupported data type')
     if num_reversed_exch_timestamp > 0:
@@ -102,15 +136,34 @@
         print('local_timestamp is ahead of exch_timestamp by', -latency)
         for row_num in range(len(data)):
             data[row_num, COL_LOCAL_TIMESTAMP] += local_timestamp_offset
 
     return data
 
 
-def correct_local_timestamp(data, base_latency):
+def correct_local_timestamp(data: Data, base_latency: float) -> Data:
+    r"""
+    Adjusts the local timestamp if the feed latency is negative by offsetting the maximum negative latency value as
+    follows:
+
+    .. code-block::
+
+        feed_latency = local_timestamp - exch_timestamp
+        adjusted_local_timestamp = local_timestamp + min(feed_latency, 0) + base_latency
+
+    Args:
+        data: Data to be corrected.
+        base_latency: Due to discrepancies in system time between the exchange and the local machine, latency may be
+                      measured inaccurately, resulting in negative latency values. The conversion process automatically
+                      adjusts for positive latency but may still produce zero latency cases. By adding ``base_latency``,
+                      more realistic values can be obtained. Unit should be the same as the feed data's timestamp unit.
+
+    Returns:
+        Adjusted data with corrected timestamps
+    """
     if isinstance(data, pd.DataFrame):
         df_corr = pd.DataFrame(_correct_local_timestamp(data.to_numpy(), base_latency), columns=data.columns)
         for col in df_corr.columns:
             df_corr[col] = df_corr[col].astype(data[col].dtype)
         return df_corr
     elif isinstance(data, np.ndarray):
         return _correct_local_timestamp(data, base_latency)
@@ -122,15 +175,21 @@
 def _correct_exch_timestamp(data, num_corr):
     row_size, col_size = data.shape
     corr = np.zeros((row_size + num_corr, col_size), np.float64)
     prev_exch_timestamp = 0
     out_row_num = 0
     for row_num in range(len(data)):
         exch_timestamp = data[row_num, COL_EXCH_TIMESTAMP]
-        if exch_timestamp < prev_exch_timestamp:
+        event = data[row_num, COL_EVENT]
+        if exch_timestamp < prev_exch_timestamp and event in [
+            TRADE_EVENT,
+            DEPTH_EVENT,
+            DEPTH_CLEAR_EVENT,
+            DEPTH_SNAPSHOT_EVENT
+        ]:
             # This new row should be inserted ahead.
             found = False
             for i in range(out_row_num - 1, -1, -1):
                 if exch_timestamp < corr[i, COL_EXCH_TIMESTAMP] or found:
                     found = True
                     if i == 0 or \
                             (i > 0
@@ -145,15 +204,27 @@
         else:
             corr[out_row_num, :] = data[row_num, :]
             prev_exch_timestamp = exch_timestamp
         out_row_num += 1
     return corr[:out_row_num, :]
 
 
-def correct_exch_timestamp(data, num_corr):
+def correct_exch_timestamp(data: Data, num_corr: int) -> Data:
+    r"""
+    Corrects exchange timestamps that are reversed by splitting each row into separate events, ordered by both exchange
+    and local timestamps, through duplication. See ``data`` for details.
+
+    Args:
+        data: Data to be corrected.
+        num_corr: The number of rows to be corrected.
+
+    Returns:
+        Adjusted data with corrected exchange timestamps.
+    """
+
     if isinstance(data, pd.DataFrame):
         df_corr = pd.DataFrame(_correct_exch_timestamp(data.to_numpy(), num_corr), columns=data.columns)
         for col in df_corr.columns:
             df_corr[col] = df_corr[col].astype(data[col].dtype)
         return df_corr
     elif isinstance(data, np.ndarray):
         return _correct_exch_timestamp(data, num_corr)
@@ -169,34 +240,66 @@
     # Adjust local_timestamp in reverse order to have a value equal to or greater than the previous local_timestamp.
     for row_num in range(1, len(sorted_data)):
         if sorted_data[row_num, COL_LOCAL_TIMESTAMP] < sorted_data[row_num - 1, COL_LOCAL_TIMESTAMP]:
             sorted_data[row_num, COL_LOCAL_TIMESTAMP] = sorted_data[row_num - 1, COL_LOCAL_TIMESTAMP]
     return sorted_data
 
 
-def correct_exch_timestamp_adjust(data):
+def correct_exch_timestamp_adjust(data: Data) -> Data:
+    r"""
+    Corrects reversed exchange timestamps by adjusting the local timestamp value for proper ordering. It sorts the data
+    by exchange timestamp and fixes out-of-order local timestamps by setting their value to the previous value, ensuring
+    correct ordering.
+
+    Args:
+        data: Data to be corrected.
+
+    Returns:
+        Adjusted data with corrected exchange timestamps.
+    """
+
     if isinstance(data, pd.DataFrame):
         df_corr = pd.DataFrame(_correct_exch_timestamp_adjust(data.to_numpy()), columns=data.columns)
         for col in df_corr.columns:
             df_corr[col] = df_corr[col].astype(data[col].dtype)
         return df_corr
     elif isinstance(data, np.ndarray):
         return _correct_exch_timestamp_adjust(data)
     else:
         raise ValueError('Unsupported data type')
 
 
 def correct(
-        data,
-        base_latency,
-        tick_size=None,
-        lot_size=None,
-        err_bound=1e-8,
-        method='separate'
-):
+        data: Data,
+        base_latency: float,
+        tick_size: Optional[float] = None,
+        lot_size: Optional[float] = None,
+        err_bound: float = 1e-8,
+        method: Literal['separate', 'adjust'] = 'separate'
+) -> Data:
+    r"""
+    Validates the specified data and automatically corrects negative latency and unordered rows.
+    See :func:`.validate_data`, :func:`.correct_local_timestamp`, :func:`.correct_exch_timestamp`, and
+    :func:`.correct_exch_timestamp_adjust`.
+
+    Args:
+        data: Data to be checked and corrected.
+        base_latency: The value to be added to the feed latency. See :func:`.correct_local_timestamp`.
+        tick_size: Minimum price increment for the specified data.
+        lot_size: Minimum order quantity for the specified data.
+        err_bound: Error bound used to verify if the specified ``tick_size`` or ``lot_size`` aligns with the price and
+                   quantity.
+        method: The method to correct reversed exchange timestamp events.
+
+                    - ``separate``: Use :func:`.correct_local_timestamp`.
+                    - ``adjust``: Use :func:`.correct_exch_timestamp_adjust`.
+
+    Returns:
+        Corrected data
+    """
     data = correct_local_timestamp(data, base_latency)
     num_corr = validate_data(
         data,
         tick_size=tick_size,
         lot_size=lot_size,
         err_bound=err_bound
     )
@@ -205,8 +308,8 @@
     if method == 'separate':
         data = correct_exch_timestamp(data, num_corr)
     elif method == 'adjust':
         data = correct_exch_timestamp_adjust(data)
     else:
         raise ValueError('Invalid method')
     print('Correction is done.')
-    return data
+    return data
```

### Comparing `hftbacktest-1.5.0/hftbacktest/marketdepth.py` & `hftbacktest-1.5.1/hftbacktest/marketdepth.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.0/hftbacktest/models/queue.py` & `hftbacktest-1.5.1/hftbacktest/models/queue.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# These models are implemented as described in
-# https://quant.stackexchange.com/questions/3782/how-do-we-estimate-position-of-our-order-in-order-book
-# http://www.math.ualberta.ca/~cfrei/PIMS/Almgren5.pdf
-
-from numba.experimental import jitclass
-
 import numpy as np
 
 
-@jitclass
 class RiskAverseQueueModel:
+    r"""
+    Provides a conservative queue position model, where your order's queue position advances only when trades occur at
+    the same price level.
+    """
+
     def __init__(self):
         pass
 
     def new(self, order, proc):
         if order.side == 1:
             order.q[0] = proc.bid_depth.get(order.price_tick, 0)
         else:
@@ -28,14 +26,24 @@
         return round(order.q[0] / proc.lot_size) < 0
 
     def reset(self):
         pass
 
 
 class ProbQueueModel:
+    r"""
+    Provides a probability-based queue position model as described in
+    https://quant.stackexchange.com/questions/3782/how-do-we-estimate-position-of-our-order-in-order-book.
+
+    Your order's queue position advances when a trade occurs at the same price level or the quantity at the level
+    decreases. The advancement in queue position depends on the probability based on the relative queue position. To
+    avoid double counting the quantity decrease caused by trades, all trade quantities occurring at the level before
+    the book quantity changes will be subtracted from the book quantity changes.
+    """
+
     def __init__(self):
         pass
 
     def new(self, order, proc):
         if order.side == 1:
             order.q[0] = proc.bid_depth.get(order.price_tick, 0)
         else:
@@ -72,23 +80,32 @@
     def prob(self, front, back):
         return np.divide(self.f(back), self.f(back) + self.f(front))
 
     def reset(self):
         pass
 
 
-@jitclass
 class LogProbQueueModel(ProbQueueModel):
+    r"""
+    This model uses a logarithmic function ``log(1 + x)`` to adjust the probability.
+    """
+
     def f(self, x):
         return np.log(1 + x)
 
 
-@jitclass
 class IdentityProbQueueModel(ProbQueueModel):
+    r"""
+    This model uses an identity function ``x`` to adjust the probability.
+    """
+
     def f(self, x):
         return x
 
 
-@jitclass
 class SquareProbQueueModel(ProbQueueModel):
+    r"""
+    This model uses a square function ``x ** 2`` to adjust the probability.
+    """
+
     def f(self, x):
         return x ** 2
```

### Comparing `hftbacktest-1.5.0/hftbacktest/order.py` & `hftbacktest-1.5.1/hftbacktest/order.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.0/hftbacktest/proc/local.py` & `hftbacktest-1.5.1/hftbacktest/proc/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import numpy as np
 from numba import int64, float64
 from numba.experimental import jitclass
 
 from .proc import Proc, proc_spec
-from ..order import BUY, SELL, NEW, CANCELED, FILLED, EXPIRED, NONE, Order, LIMIT
-from ..reader import COL_EVENT, COL_LOCAL_TIMESTAMP, COL_SIDE, COL_PRICE, COL_QTY, DEPTH_CLEAR_EVENT, DEPTH_EVENT, \
-    DEPTH_SNAPSHOT_EVENT, TRADE_EVENT, USER_DEFINED_EVENT
+from ..order import BUY, NEW, CANCELED, FILLED, EXPIRED, NONE, Order
+from ..reader import (
+    COL_EVENT,
+    COL_LOCAL_TIMESTAMP,
+    COL_SIDE,
+    COL_PRICE,
+    COL_QTY,
+    DEPTH_CLEAR_EVENT,
+    DEPTH_EVENT,
+    DEPTH_SNAPSHOT_EVENT,
+    TRADE_EVENT,
+    USER_DEFINED_EVENT
+)
 
 
 class Local_(Proc):
     def __init__(
             self,
             reader,
             orders_to_exch,
```

### Comparing `hftbacktest-1.5.0/hftbacktest/proc/nopartialfillexchange.py` & `hftbacktest-1.5.1/hftbacktest/proc/nopartialfillexchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,25 @@
 from numba.experimental import jitclass
 from numba.typed.typeddict import Dict
 from numba.types import DictType
 
 from .proc import Proc, proc_spec
 from ..marketdepth import INVALID_MAX, INVALID_MIN
 from ..order import BUY, SELL, NEW, CANCELED, FILLED, EXPIRED, GTX, NONE, order_ladder_ty
-from ..reader import COL_EVENT, COL_EXCH_TIMESTAMP, COL_SIDE, COL_PRICE, COL_QTY, DEPTH_CLEAR_EVENT, DEPTH_EVENT, \
-    DEPTH_SNAPSHOT_EVENT, TRADE_EVENT
+from ..reader import (
+    COL_EVENT,
+    COL_EXCH_TIMESTAMP,
+    COL_SIDE,
+    COL_PRICE,
+    COL_QTY,
+    DEPTH_CLEAR_EVENT,
+    DEPTH_EVENT,
+    DEPTH_SNAPSHOT_EVENT,
+    TRADE_EVENT
+)
 
 
 class NoPartialFillExchange_(Proc):
     def __init__(
             self,
             reader,
             orders_to_local,
```

### Comparing `hftbacktest-1.5.0/hftbacktest/proc/partialfillexchange.py` & `hftbacktest-1.5.1/hftbacktest/proc/partialfillexchange.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,39 @@
 from numba.typed.typeddict import Dict
 from numba.types import DictType
 
 import numpy as np
 
 from .proc import Proc, proc_spec
 from ..marketdepth import INVALID_MAX, INVALID_MIN
-from ..order import BUY, SELL, NEW, CANCELED, FILLED, EXPIRED, PARTIALLY_FILLED, GTX, FOK, IOC, NONE, order_ladder_ty
-from ..reader import COL_EVENT, COL_EXCH_TIMESTAMP, COL_SIDE, COL_PRICE, COL_QTY, DEPTH_CLEAR_EVENT, DEPTH_EVENT, \
-    DEPTH_SNAPSHOT_EVENT, TRADE_EVENT
+from ..order import (
+    BUY,
+    SELL,
+    NEW,
+    CANCELED,
+    FILLED,
+    EXPIRED,
+    PARTIALLY_FILLED,
+    GTX,
+    FOK,
+    IOC,
+    NONE,
+    order_ladder_ty
+)
+from ..reader import (
+    COL_EVENT,
+    COL_EXCH_TIMESTAMP,
+    COL_SIDE,
+    COL_PRICE,
+    COL_QTY,
+    DEPTH_CLEAR_EVENT,
+    DEPTH_EVENT,
+    DEPTH_SNAPSHOT_EVENT,
+    TRADE_EVENT
+)
 
 
 class PartialFillExchange_(Proc):
     def __init__(
             self,
             reader,
             orders_to_local,
```

### Comparing `hftbacktest-1.5.0/hftbacktest/proc/proc.py` & `hftbacktest-1.5.1/hftbacktest/proc/proc.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.0/hftbacktest/reader.py` & `hftbacktest-1.5.1/hftbacktest/reader.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.0/hftbacktest/state.py` & `hftbacktest-1.5.1/hftbacktest/state.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.0/hftbacktest.egg-info/PKG-INFO` & `hftbacktest-1.5.1/hftbacktest.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,181 +1,188 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.5.0
+Version: 1.5.1
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
-Project-URL: Docs, https://github.com/nkaz001/hftbacktest/wiki
+Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
 Project-URL: GitHub: repo, https://github.com/nkaz001/hftbacktest
-Description: ===========
-        HftBacktest
-        ===========
-        
-        |codacy| |codeql| |pypi| |downloads| |license|
-        
-        High-Frequency Trading Backtesting Tool in Python
-        ====================================================================
-        
-        This Python framework is designed for developing high-frequency trading and market-making strategies. It focuses on accounting for both feed and order latencies, as well as the order queue position for order fill simulation. The framework aims to provide more accurate market replay-based backtesting, based on full order book and trade tick feed data.
-        
-        Key Features
-        ============
-        
-        * Working in `Numba <https://numba.pydata.org/>`_ JIT function.
-        * Complete tick-by-tick simulation with a variable time interval.
-        * Full order book reconstruction based on L2 feeds(Market-By-Price).
-        * Backtest accounting for both feed and order latency, using provided models or your own custom model.
-        * Order fill simulation that takes into account the order queue position, using provided models or your own custom model.
-        
-        
-        Getting started
-        ===============
-        
-        Installation
-        ------------
-        
-        hftbacktest supports Python 3.7+. You can install hftbacktest using ``pip``:
-        
-        .. code-block:: console
-        
-         pip install hftbacktest
-        
-        Or you can clone the latest development version from the Git repository with:
-        
-        .. code-block:: console
-        
-         git clone https://github.com/nkaz001/hftbacktest
-        
-        Data Source & Format
-        --------------------
-        
-        Please see `Data <https://github.com/nkaz001/hftbacktest/wiki/Data>`_ or `Data Preparation <https://github.com/nkaz001/hftbacktest/blob/master/examples/Data%20Preparation.ipynb>`_.
-        
-        A Quick Example
-        ---------------
-        
-        Get a glimpse of what backtesting with hftbacktest looks like with these code snippets:
-        
-        .. code-block:: python
-        
-            @njit
-            def simple_two_sided_quote(hbt, stat):
-                max_position = 5
-                half_spread = hbt.tick_size * 20
-                skew = 1
-                order_qty = 0.1 
-                last_order_id = -1
-        
-                bid_order_price_tick_as_id = -1
-                ask_order_price_tick_as_id = -1
-        
-                while hbt.run:
-                    # Check every 0.1s
-                    if not hbt.elapse(0.1 * 1e6):
-                        return False
-        
-                    # Clear cancelled, filled or expired orders.
-                    hbt.clear_inactive_orders()
-        
-                    # Obtain the current mid-price and compute the reservation price.
-                    mid_price = (hbt.best_bid + hbt.best_ask) / 2.0
-                    reservation_price = mid_price - skew * hbt.position * hbt.tick_size
-        
-                    bid_order_price = reservation_price - half_spread
-                    ask_order_price = reservation_price + half_spread
-        
-                    # Cancel the existing bid order.
-                    existing_bid_order = hbt.orders.get(bid_order_price_tick_as_id)
-                    if existing_bid_order is not None and existing_bid_order.cancellable:
-                        hbt.cancel(existing_bid_order.order_id)
-                        last_order_id = existing_bid_order.order_id
-        
-                    # Cancel the existing ask order.
-                    existing_ask_order = hbt.orders.get(ask_order_price_tick_as_id)
-                    if existing_ask_order is not None and existing_ask_order.cancellable:
-                        hbt.cancel(existing_ask_order.order_id)
-                        last_order_id = existing_ask_order.order_id
-        
-                    if hbt.position < max_position:
-                        # Submit a new post-only limit bid order.
-                        bid_order_price_tick_as_id = round(bid_order_price / hbt.tick_size)
-                        hbt.submit_buy_order(
-                            bid_order_price_tick_as_id,
-                            bid_order_price,
-                            order_qty,
-                            GTX
-                        )
-                        last_order_id = bid_order_price_tick_as_id
-        
-                    if hbt.position > -max_position:
-                        # Submit a new post-only limit ask order.
-                        ask_order_price_tick_as_id = round(ask_order_price / hbt.tick_size)
-                        hbt.submit_sell_order(
-                            ask_order_price_tick_as_id,
-                            ask_order_price,
-                            order_qty,
-                            GTX
-                        )
-                        last_order_id = ask_order_price_tick_as_id
-        
-                    # All order requests are considered to be requested at the same time.
-                    # Wait until one of the order responses is received.
-                    if last_order_id >= 0:
-                        hbt.wait_order_response(last_order_id)
-        
-                    # Record the current state for stat calculation.
-                    stat.record(hbt)
-                return True
-        
-            
-        Examples
-        ========
-        
-        You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
-        
-        Documentation
-        =============
-        * `Data <https://github.com/nkaz001/hftbacktest/wiki/Data>`_
-        * `Latency model <https://github.com/nkaz001/hftbacktest/wiki/Latency-model>`_
-        * `Order fill <https://github.com/nkaz001/hftbacktest/wiki/Order-fill>`_
-        
-        .. |python| image:: https://img.shields.io/pypi/pyversions/hftbacktest.svg?style=plastic
-            :alt: |Python Version
-            :target: https://badge.fury.io/py/tensorflow
-        
-        .. |codacy| image:: https://app.codacy.com/project/badge/Grade/e2cef673757a45b18abfc361779feada
-            :alt: |Codacy
-            :target: https://www.codacy.com/gh/nkaz001/hftbacktest/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=nkaz001/hftbacktest&amp;utm_campaign=Badge_Grade
-        
-        .. |codeql| image:: https://github.com/nkaz001/hftbacktest/actions/workflows/codeql.yml/badge.svg?branch=master&event=push
-            :alt: |CodeQL
-            :target: https://github.com/nkaz001/hftbacktest/actions/workflows/codeql.yml
-        
-        .. |pypi| image:: https://badge.fury.io/py/hftbacktest.svg
-            :alt: |Package Version
-            :target: https://pypi.org/project/hftbacktest
-            
-        .. |downloads| image:: https://static.pepy.tech/badge/hftbacktest
-            :alt: |Downloads
-            :target: https://pepy.tech/project/hftbacktest
-        
-        .. |license| image:: https://img.shields.io/badge/License-MIT-green.svg
-            :alt: |License
-            :target: https://github.com/nkaz001/hftbacktest/blob/master/LICENSE
-        
 Keywords: hft,high-frequency trading,trading,market-making,backtest
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Python: >=3.7
+License-File: LICENSE
+
+===========
+HftBacktest
+===========
+
+|codacy| |codeql| |pypi| |downloads| |license| |docs|
+
+High-Frequency Trading Backtesting Tool in Python
+====================================================================
+
+This Python framework is designed for developing high-frequency trading and market-making strategies. It focuses on accounting for both feed and order latencies, as well as the order queue position for order fill simulation. The framework aims to provide more accurate market replay-based backtesting, based on full order book and trade tick feed data.
+
+Key Features
+============
+
+* Working in `Numba <https://numba.pydata.org/>`_ JIT function.
+* Complete tick-by-tick simulation with a variable time interval.
+* Full order book reconstruction based on L2 feeds(Market-By-Price).
+* Backtest accounting for both feed and order latency, using provided models or your own custom model.
+* Order fill simulation that takes into account the order queue position, using provided models or your own custom model.
+
+
+Getting started
+===============
+
+Installation
+------------
+
+hftbacktest supports Python 3.7+. You can install hftbacktest using ``pip``:
+
+.. code-block:: console
+
+ pip install hftbacktest
+
+Or you can clone the latest development version from the Git repository with:
+
+.. code-block:: console
+
+ git clone https://github.com/nkaz001/hftbacktest
+
+Data Source & Format
+--------------------
+
+Please see `Data <https://hftbacktest.readthedocs.io/en/latest/data.html>`_ or `Data Preparation <https://hftbacktest.readthedocs.io/en/latest/tutorials/Data%20Preparation.html>`_.
+
+A Quick Example
+---------------
+
+Get a glimpse of what backtesting with hftbacktest looks like with these code snippets:
+
+.. code-block:: python
+
+    @njit
+    def simple_two_sided_quote(hbt, stat):
+        max_position = 5
+        half_spread = hbt.tick_size * 20
+        skew = 1
+        order_qty = 0.1 
+        last_order_id = -1
+        order_id = 0
+
+        while hbt.run:
+            # Check every 0.1s
+            if not hbt.elapse(0.1 * 1e6):
+                return False
+
+            # Clear cancelled, filled or expired orders.
+            hbt.clear_inactive_orders()
+
+            # Obtain the current mid-price and compute the reservation price.
+            mid_price = (hbt.best_bid + hbt.best_ask) / 2.0
+            reservation_price = mid_price - skew * hbt.position * hbt.tick_size
+
+            buy_order_price = reservation_price - half_spread
+            sell_order_price = reservation_price + half_spread
+
+            last_order_id = -1
+            # Cancel all outstanding orders
+            for order in hbt.orders.values():
+                if order.cancellable:
+                    hbt.cancel(order.order_id)
+                    last_order_id = order.order_id    
+			
+            # All order requests are considered to be requested at the same time.
+            # Wait until one of the order cancellation responses is received.
+            if last_order_id >= 0:
+                hbt.wait_order_response(last_order_id)
+				
+            # Clear cancelled, filled or expired orders.
+            hbt.clear_inactive_orders()
+
+	    last_order_id = -1
+            if hbt.position < max_position:
+                # Submit a new post-only limit bid order.
+                order_id += 1
+                hbt.submit_buy_order(
+                    order_id,
+                    buy_order_price,
+                    order_qty,
+                    GTX
+                )
+                last_order_id = order_id
+
+            if hbt.position > -max_position:
+                # Submit a new post-only limit ask order.
+                order_id += 1
+                hbt.submit_sell_order(
+                    order_id,
+                    sell_order_price,
+                    order_qty,
+                    GTX
+                )
+                last_order_id = order_id
+
+            # All order requests are considered to be requested at the same time.
+            # Wait until one of the order responses is received.
+            if last_order_id >= 0:
+                hbt.wait_order_response(last_order_id)
+
+            # Record the current state for stat calculation.
+            stat.record(hbt)
+        return True
+
+    
+Examples
+========
+
+You can find more examples in `examples <https://github.com/nkaz001/hftbacktest/tree/master/examples>`_ directory.
+
+Documentation
+=============
+
+See `here <https://hftbacktest.readthedocs.io/en/latest/>`_.
+
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/hftbacktest.svg?style=plastic
+    :alt: |Python Version
+    :target: https://badge.fury.io/py/tensorflow
+
+.. |codacy| image:: https://app.codacy.com/project/badge/Grade/e2cef673757a45b18abfc361779feada
+    :alt: |Codacy
+    :target: https://www.codacy.com/gh/nkaz001/hftbacktest/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=nkaz001/hftbacktest&amp;utm_campaign=Badge_Grade
+
+.. |codeql| image:: https://github.com/nkaz001/hftbacktest/actions/workflows/codeql.yml/badge.svg?branch=master&event=push
+    :alt: |CodeQL
+    :target: https://github.com/nkaz001/hftbacktest/actions/workflows/codeql.yml
+
+.. |pypi| image:: https://badge.fury.io/py/hftbacktest.svg
+    :alt: |Package Version
+    :target: https://pypi.org/project/hftbacktest
+    
+.. |downloads| image:: https://static.pepy.tech/badge/hftbacktest
+    :alt: |Downloads
+    :target: https://pepy.tech/project/hftbacktest
+
+.. |license| image:: https://img.shields.io/badge/License-MIT-green.svg
+    :alt: |License
+    :target: https://github.com/nkaz001/hftbacktest/blob/master/LICENSE
+    
+.. |docs| image:: https://readthedocs.org/projects/hftbacktest/badge/?version=latest
+    :target: https://hftbacktest.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
```

### Comparing `hftbacktest-1.5.0/hftbacktest.egg-info/SOURCES.txt` & `hftbacktest-1.5.1/hftbacktest.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 hftbacktest/assettype.py
 hftbacktest/backtest.py
 hftbacktest/marketdepth.py
 hftbacktest/order.py
 hftbacktest/reader.py
 hftbacktest/stat.py
 hftbacktest/state.py
+hftbacktest/typing.py
 hftbacktest.egg-info/PKG-INFO
 hftbacktest.egg-info/SOURCES.txt
 hftbacktest.egg-info/dependency_links.txt
 hftbacktest.egg-info/not-zip-safe
 hftbacktest.egg-info/requires.txt
 hftbacktest.egg-info/top_level.txt
 hftbacktest/data/__init__.py
```

### Comparing `hftbacktest-1.5.0/setup.cfg` & `hftbacktest-1.5.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = hftbacktest
 version = attr: hftbacktest.__version__
 url = https://github.com/nkaz001/hftbacktest
 project_urls = 
-	Docs = https://github.com/nkaz001/hftbacktest/wiki
+	Docs = https://hftbacktest.readthedocs.io/en/latest/
 	GitHub: issues = https://github.com/nkaz001/hftbacktest/issues
 	GitHub: repo = https://github.com/nkaz001/hftbacktest
 description = High-frequency trading and market making backtesting tool
 long_description = file: README.rst
 author = nkaz001
 author_email = nkaz001@protonmail.com
 keywords = hft, high-frequency trading, trading, market-making, backtest
```

