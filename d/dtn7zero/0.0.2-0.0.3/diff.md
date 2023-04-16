# Comparing `tmp/dtn7zero-0.0.2.tar.gz` & `tmp/dtn7zero-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Data\Benutzer\Lukas\PyCharmProjects\daimpl-2022-holst\dist\.tmp-24z8aunf\dtn7zero-0.0.2.tar", last modified: Sat Apr  8 14:17:55 2023, max compression
+gzip compressed data, was "D:\Data\Benutzer\Lukas\PyCharmProjects\daimpl-2022-holst\dist\.tmp-7de2h_2r\dtn7zero-0.0.3.tar", last modified: Sun Apr 16 13:46:41 2023, max compression
```

## Comparing `dtn7zero-0.0.2.tar` & `dtn7zero-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/
--rw-rw-rw-   0        0        0    35184 2023-04-05 00:02:15.000000 dtn7zero-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     8437 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8228 2023-04-08 14:13:42.000000 dtn7zero-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/dtn7zero/
--rw-rw-rw-   0        0        0      245 2023-04-06 11:28:37.000000 dtn7zero-0.0.2/dtn7zero/__init__.py
--rw-rw-rw-   0        0        0     7551 2023-04-06 18:52:15.000000 dtn7zero-0.0.2/dtn7zero/api.py
--rw-rw-rw-   0        0        0    19507 2023-04-07 00:49:01.000000 dtn7zero-0.0.2/dtn7zero/bundle_protocol_agent.py
--rw-rw-rw-   0        0        0     1590 2023-04-07 00:24:01.000000 dtn7zero-0.0.2/dtn7zero/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/dtn7zero/convergence_layer_adapters/
--rw-rw-rw-   0        0        0      615 2023-03-10 14:43:33.000000 dtn7zero-0.0.2/dtn7zero/convergence_layer_adapters/__init__.py
--rw-rw-rw-   0        0        0     3282 2023-04-07 00:28:58.000000 dtn7zero-0.0.2/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py
--rw-rw-rw-   0        0        0    12464 2023-04-07 00:28:58.000000 dtn7zero-0.0.2/dtn7zero/convergence_layer_adapters/mtcp.py
--rw-rw-rw-   0        0        0     2127 2023-04-03 20:01:46.000000 dtn7zero-0.0.2/dtn7zero/data.py
--rw-rw-rw-   0        0        0     6492 2023-04-07 00:48:35.000000 dtn7zero-0.0.2/dtn7zero/endpoints.py
--rw-rw-rw-   0        0        0    15215 2023-04-07 00:28:58.000000 dtn7zero-0.0.2/dtn7zero/ipnd.py
-drwxrwxrwx   0        0        0        0 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/dtn7zero/routers/
--rw-rw-rw-   0        0        0     3128 2023-04-07 00:22:15.000000 dtn7zero-0.0.2/dtn7zero/routers/__init__.py
--rw-rw-rw-   0        0        0     4380 2023-04-07 00:28:58.000000 dtn7zero-0.0.2/dtn7zero/routers/simple_epidemic_router.py
-drwxrwxrwx   0        0        0        0 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/dtn7zero/storage/
--rw-rw-rw-   0        0        0     1271 2023-04-03 19:30:50.000000 dtn7zero-0.0.2/dtn7zero/storage/__init__.py
--rw-rw-rw-   0        0        0     2896 2023-04-03 19:30:50.000000 dtn7zero-0.0.2/dtn7zero/storage/simple_in_memory_storage.py
--rw-rw-rw-   0        0        0     2408 2023-04-07 00:24:34.000000 dtn7zero-0.0.2/dtn7zero/utility.py
-drwxrwxrwx   0        0        0        0 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/dtn7zero.egg-info/
--rw-rw-rw-   0        0        0     8437 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/dtn7zero.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/dtn7zero.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/dtn7zero.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/dtn7zero.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/dtn7zero.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-04-08 14:15:07.000000 dtn7zero-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-08 14:17:55.000000 dtn7zero-0.0.2/test/
--rw-rw-rw-   0        0        0      956 2023-04-07 00:50:38.000000 dtn7zero-0.0.2/test/test-api-background.py
--rw-rw-rw-   0        0        0      694 2023-04-06 18:49:09.000000 dtn7zero-0.0.2/test/test-api-ping.py
--rw-rw-rw-   0        0        0      563 2023-04-06 18:48:16.000000 dtn7zero-0.0.2/test/test-api-pong.py
--rw-rw-rw-   0        0        0      899 2023-04-06 18:42:36.000000 dtn7zero-0.0.2/test/test-api-synchronous.py
--rw-rw-rw-   0        0        0     1944 2023-04-06 15:33:01.000000 dtn7zero-0.0.2/test/test-bundle-protocol-agent-receiver.py
--rw-rw-rw-   0        0        0     2095 2023-04-06 15:35:14.000000 dtn7zero-0.0.2/test/test-bundle-protocol-agent-sender.py
--rw-rw-rw-   0        0        0     1443 2023-04-06 15:26:41.000000 dtn7zero-0.0.2/test/test-bundle-protocol-agent.py
--rw-rw-rw-   0        0        0     1711 2023-04-06 14:23:22.000000 dtn7zero-0.0.2/test/test-bundle-serialization.py
--rw-rw-rw-   0        0        0    15498 2023-04-05 13:35:10.000000 dtn7zero-0.0.2/test/test-bundle-size.py
--rw-rw-rw-   0        0        0     1688 2023-04-06 14:23:59.000000 dtn7zero-0.0.2/test/test-dtn7rs-rest-cla.py
--rw-rw-rw-   0        0        0     1236 2023-04-06 15:46:25.000000 dtn7zero-0.0.2/test/test-ipnd.py
--rw-rw-rw-   0        0        0     2028 2023-04-06 16:03:37.000000 dtn7zero-0.0.2/test/test-mtcp-intermediate.py
--rw-rw-rw-   0        0        0     2260 2023-04-06 14:24:54.000000 dtn7zero-0.0.2/test/test-mtcp-receiver.py
--rw-rw-rw-   0        0        0     2563 2023-04-06 14:25:13.000000 dtn7zero-0.0.2/test/test-mtcp-sender.py
--rw-rw-rw-   0        0        0     5282 2023-04-04 23:52:20.000000 dtn7zero-0.0.2/test/test-py-dtn7-functionality.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:46:41.000000 dtn7zero-0.0.3/
+-rw-rw-rw-   0        0        0    35184 2023-04-05 00:02:15.000000 dtn7zero-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     9975 2023-04-16 13:46:41.000000 dtn7zero-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9766 2023-04-16 13:16:20.000000 dtn7zero-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 13:46:40.000000 dtn7zero-0.0.3/dtn7zero/
+-rw-rw-rw-   0        0        0      261 2023-04-16 12:17:34.000000 dtn7zero-0.0.3/dtn7zero/__init__.py
+-rw-rw-rw-   0        0        0     9731 2023-04-16 12:14:44.000000 dtn7zero-0.0.3/dtn7zero/api.py
+-rw-rw-rw-   0        0        0    21246 2023-04-16 13:20:10.000000 dtn7zero-0.0.3/dtn7zero/bundle_protocol_agent.py
+-rw-rw-rw-   0        0        0     1506 2023-04-16 12:45:23.000000 dtn7zero-0.0.3/dtn7zero/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:46:40.000000 dtn7zero-0.0.3/dtn7zero/convergence_layer_adapters/
+-rw-rw-rw-   0        0        0      615 2023-03-10 14:43:33.000000 dtn7zero-0.0.3/dtn7zero/convergence_layer_adapters/__init__.py
+-rw-rw-rw-   0        0        0     3282 2023-04-07 00:28:58.000000 dtn7zero-0.0.3/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py
+-rw-rw-rw-   0        0        0    13077 2023-04-11 22:56:50.000000 dtn7zero-0.0.3/dtn7zero/convergence_layer_adapters/mtcp.py
+-rw-rw-rw-   0        0        0     2435 2023-04-11 23:08:59.000000 dtn7zero-0.0.3/dtn7zero/data.py
+-rw-rw-rw-   0        0        0     7598 2023-04-16 13:21:12.000000 dtn7zero-0.0.3/dtn7zero/endpoints.py
+-rw-rw-rw-   0        0        0    12902 2023-04-11 23:07:13.000000 dtn7zero-0.0.3/dtn7zero/ipnd.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:46:40.000000 dtn7zero-0.0.3/dtn7zero/routers/
+-rw-rw-rw-   0        0        0     3128 2023-04-07 00:22:15.000000 dtn7zero-0.0.3/dtn7zero/routers/__init__.py
+-rw-rw-rw-   0        0        0     4380 2023-04-16 12:43:55.000000 dtn7zero-0.0.3/dtn7zero/routers/simple_epidemic_router.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:46:40.000000 dtn7zero-0.0.3/dtn7zero/storage/
+-rw-rw-rw-   0        0        0     1402 2023-04-16 12:43:18.000000 dtn7zero-0.0.3/dtn7zero/storage/__init__.py
+-rw-rw-rw-   0        0        0     2941 2023-04-16 12:44:30.000000 dtn7zero-0.0.3/dtn7zero/storage/simple_in_memory_storage.py
+-rw-rw-rw-   0        0        0     4307 2023-04-16 13:29:52.000000 dtn7zero-0.0.3/dtn7zero/utility.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:46:40.000000 dtn7zero-0.0.3/dtn7zero.egg-info/
+-rw-rw-rw-   0        0        0     9975 2023-04-16 13:46:40.000000 dtn7zero-0.0.3/dtn7zero.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1095 2023-04-16 13:46:40.000000 dtn7zero-0.0.3/dtn7zero.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 13:46:40.000000 dtn7zero-0.0.3/dtn7zero.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 13:46:40.000000 dtn7zero-0.0.3/dtn7zero.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 13:46:40.000000 dtn7zero-0.0.3/dtn7zero.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-04-16 13:45:01.000000 dtn7zero-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 13:46:41.000000 dtn7zero-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 13:46:41.000000 dtn7zero-0.0.3/test/
+-rw-rw-rw-   0        0        0      956 2023-04-07 00:50:38.000000 dtn7zero-0.0.3/test/test-api-background.py
+-rw-rw-rw-   0        0        0      694 2023-04-06 18:49:09.000000 dtn7zero-0.0.3/test/test-api-ping.py
+-rw-rw-rw-   0        0        0      563 2023-04-06 18:48:16.000000 dtn7zero-0.0.3/test/test-api-pong.py
+-rw-rw-rw-   0        0        0      899 2023-04-06 18:42:36.000000 dtn7zero-0.0.3/test/test-api-synchronous.py
+-rw-rw-rw-   0        0        0     1944 2023-04-06 15:33:01.000000 dtn7zero-0.0.3/test/test-bundle-protocol-agent-receiver.py
+-rw-rw-rw-   0        0        0     2095 2023-04-06 15:35:14.000000 dtn7zero-0.0.3/test/test-bundle-protocol-agent-sender.py
+-rw-rw-rw-   0        0        0     1443 2023-04-06 15:26:41.000000 dtn7zero-0.0.3/test/test-bundle-protocol-agent.py
+-rw-rw-rw-   0        0        0     1711 2023-04-06 14:23:22.000000 dtn7zero-0.0.3/test/test-bundle-serialization.py
+-rw-rw-rw-   0        0        0    15498 2023-04-05 13:35:10.000000 dtn7zero-0.0.3/test/test-bundle-size.py
+-rw-rw-rw-   0        0        0     1688 2023-04-06 14:23:59.000000 dtn7zero-0.0.3/test/test-dtn7rs-rest-cla.py
+-rw-rw-rw-   0        0        0     1236 2023-04-06 15:46:25.000000 dtn7zero-0.0.3/test/test-ipnd.py
+-rw-rw-rw-   0        0        0     2028 2023-04-06 16:03:37.000000 dtn7zero-0.0.3/test/test-mtcp-intermediate.py
+-rw-rw-rw-   0        0        0     2260 2023-04-06 14:24:54.000000 dtn7zero-0.0.3/test/test-mtcp-receiver.py
+-rw-rw-rw-   0        0        0     2563 2023-04-06 14:25:13.000000 dtn7zero-0.0.3/test/test-mtcp-sender.py
+-rw-rw-rw-   0        0        0     5282 2023-04-04 23:52:20.000000 dtn7zero-0.0.3/test/test-py-dtn7-functionality.py
```

### Comparing `dtn7zero-0.0.2/LICENSE` & `dtn7zero-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/PKG-INFO` & `dtn7zero-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,39 @@
-Metadata-Version: 2.1
-Name: dtn7zero
-Version: 0.0.2
-Author-email: Lukas Holst <lh700@proton.me>
-License: AGPL-3.0
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dtn7zero
-This is a DTN7 python implementation (work-in-progress) with [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API.
+This is a DTN7 [RFC9171](https://datatracker.ietf.org/doc/html/rfc9171) compliant python implementation (work-in-progress) with a [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API.
 
 The current features are:
-- a full bundle protocol agent (without fragment or CRC support)
+- a full bundle protocol agent (without fragment, CRC, and status-report generation support -> todo)
 - a minimal TCP convergence layer
-- a [dtn7rs](https://github.com/dtn7/dtn7-rs) REST convergence layer
-- an ipnd module
-- a standalone 'external' endpoint (which connects to a [dtn7rs](https://github.com/dtn7/dtn7-rs))
+- a [dtn7-rs](https://github.com/dtn7/dtn7-rs) convergence layer, using the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md) interface
+- automatic local-network node-discovery via ipnd module
+- a standalone 'external' endpoint (which connects to a [dtn7-rs](https://github.com/dtn7/dtn7-rs) via the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md)) interface
 - a simplified [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API to easily get started
 - full MicroPython support (tested on an ESP32-GENERIC)
 - (currently uses epidemic routing and in-memory storage managing)
 - (with extendability for new convergence layer adapters, routing algorithms, and storage managers)
 
 ## Getting Started
-To use dtn7zero in your CPython environment, simply install it via pip (or pip3 on linux): \
-(currently the package is only available on the test instance)
+To use dtn7zero in your CPython environment, simply install it via pip (or pip3 on linux):
 ```shell
 $ pip install --upgrade dtn7zero
 ```
 The most simple example on what you can do:
 ```python
+import time
+
 from dtn7zero import setup, start_background_update_thread
 
 node_endpoint = setup("dtn://node1/", print)
 
 start_background_update_thread()
 
 node_endpoint.send(b'hello world', "dtn://node1/")
+
+time.sleep(1)
 ```
 Further examples for the 'simple' API can be found under `./examples` in the GitHub repository.
 
 For a deeper dive into the underlying concepts and the fully fletched dtn implementation, take a look at the 
 `dtn7zero.api` module implementation and the tests under `./tests`.
 
 ## MicroPython Installation Guide
@@ -82,15 +76,39 @@
 1. check your connection to the ESP32 with: `mpremote`
 2. deploy the changes of dtn7zero and dependencies onto the ESP32 (this can take a while): `python scripts/esp-deployment.py`
 3. done
 
 ### First dtn7zero Functionality Check On MicroPython
 1. you may check that wlan is connecting correctly (connect via `mpremote` and press **enable** for a soft reset)
 2. you may also check that you can import dtn7zero (connect via `mpremote` and `import dtn7zero`)
-3. you can also check that everything works (run the test script `mpremote run scripts/test-bundle-protocol-agent.py`)
+3. you can also check that everything works (run the test script `mpremote run examples/local_ping_echo.py`)
+
+### Additional MicroPython Tips & Tricks
+The mpremote tool is normally interrupted by using `ctrl+c`. A special case is the REPL (simply call `mpremote`), which
+can be exited by using `ctrl+~` (tested on windows).
+
+If you start a script on MicroPython (`mpremote run ...`) and disconnect the console (`mpremote` -> `ctrl+c`) then the script 
+keeps running.
+
+If you must access the REPL via mpremote, but a script is blocking, then call `mpremote` and press EN (enable) on the 
+ESP32 for a soft-reset. Press `ctrl+c` a few times to interrupt the `boot.py` or `main.py` script execution. The session
+state is stored, so any subsequent `mpremote` call will start at REPL as long as no power disconnect is performed.
+
+You can deploy a script as `main.py` on MicroPython to be run every time the microcontroller gets power. \
+You can also remove the script. MicroPython will only execute the script if it is present.
+```shell
+$ mpremote fs cp examples/remote_echo_callback.py :main.py
+$ mpremote fs rm :main.py
+```
+
+Regarding `boot.py`, it is used for user-specific setup code and this framework uses a generic boot script that adjusts
+the ESP32's frequency and connects to a Wi-Fi network (blocking until success). MicroPython will create a dummy `boot.py`
+if none is present. MicroPython will not create a dummy `main.py` is none is present. MicroPython will first execute
+the `boot.py` and then the `main.py` if it is present.
+
 
 ## Development Information
 
 ### Development Mode
 You can install this project locally to directly reflect code changes in your environment.
 Simply run this in the project root folder (requires at least pip v21.1):
 ```shell
@@ -147,12 +165,11 @@
    - non-official, but tested micropython [library](https://github.com/glenn20/micropython/blob/espnow-g20/docs/library/espnow.rst) available, as well as [builds](https://github.com/glenn20/micropython-espnow-images) with the current firmware
 
 3. Alternative: AP_STA mode for simultaneous AP and STA without explicit ESP-MESH usage
    - only available for [Arduino+C](https://techtutorialsx.com/2021/01/04/esp32-soft-ap-and-station-modes/)
    - [painlessMesh](https://gitlab.com/painlessMesh/painlessMesh) also uses this mode to build its mesh
 
 ### Open End Topics / Known Issues
-- interface between router and cla is inconsistent (different responsibilities for send and receive)
-- dtn7rs-rest-cla and in-memory storage together use too much RAM for MicroPython (therefore the rest-cla is disabled in the simple API)
-- additional group (for example: "dtn://group/~news") registration on singleton endpoints (can there be registrations from multiple local endpoints on the same group?)
+- fragment, CRC, status-report generation support
+- dtn7rs-rest-cla and in-memory storage together use too much RAM for MicroPython (therefore the dtn7rs-rest-cla is disabled in the simple API)
 - public repository
-- api documentation (currently all information must be gathered from doc-strings and examples)
+- public documentation (currently all information must be gathered from doc-strings and examples)
```

### Comparing `dtn7zero-0.0.2/README.md` & `dtn7zero-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,48 @@
+Metadata-Version: 2.1
+Name: dtn7zero
+Version: 0.0.3
+Author-email: Lukas Holst <lh700@proton.me>
+License: AGPL-3.0
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # dtn7zero
-This is a DTN7 python implementation (work-in-progress) with [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API.
+This is a DTN7 [RFC9171](https://datatracker.ietf.org/doc/html/rfc9171) compliant python implementation (work-in-progress) with a [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API.
 
 The current features are:
-- a full bundle protocol agent (without fragment or CRC support)
+- a full bundle protocol agent (without fragment, CRC, and status-report generation support -> todo)
 - a minimal TCP convergence layer
-- a [dtn7rs](https://github.com/dtn7/dtn7-rs) REST convergence layer
-- an ipnd module
-- a standalone 'external' endpoint (which connects to a [dtn7rs](https://github.com/dtn7/dtn7-rs))
+- a [dtn7-rs](https://github.com/dtn7/dtn7-rs) convergence layer, using the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md) interface
+- automatic local-network node-discovery via ipnd module
+- a standalone 'external' endpoint (which connects to a [dtn7-rs](https://github.com/dtn7/dtn7-rs) via the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md)) interface
 - a simplified [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API to easily get started
 - full MicroPython support (tested on an ESP32-GENERIC)
 - (currently uses epidemic routing and in-memory storage managing)
 - (with extendability for new convergence layer adapters, routing algorithms, and storage managers)
 
 ## Getting Started
-To use dtn7zero in your CPython environment, simply install it via pip (or pip3 on linux): \
-(currently the package is only available on the test instance)
+To use dtn7zero in your CPython environment, simply install it via pip (or pip3 on linux):
 ```shell
 $ pip install --upgrade dtn7zero
 ```
 The most simple example on what you can do:
 ```python
+import time
+
 from dtn7zero import setup, start_background_update_thread
 
 node_endpoint = setup("dtn://node1/", print)
 
 start_background_update_thread()
 
 node_endpoint.send(b'hello world', "dtn://node1/")
+
+time.sleep(1)
 ```
 Further examples for the 'simple' API can be found under `./examples` in the GitHub repository.
 
 For a deeper dive into the underlying concepts and the fully fletched dtn implementation, take a look at the 
 `dtn7zero.api` module implementation and the tests under `./tests`.
 
 ## MicroPython Installation Guide
@@ -73,15 +85,39 @@
 1. check your connection to the ESP32 with: `mpremote`
 2. deploy the changes of dtn7zero and dependencies onto the ESP32 (this can take a while): `python scripts/esp-deployment.py`
 3. done
 
 ### First dtn7zero Functionality Check On MicroPython
 1. you may check that wlan is connecting correctly (connect via `mpremote` and press **enable** for a soft reset)
 2. you may also check that you can import dtn7zero (connect via `mpremote` and `import dtn7zero`)
-3. you can also check that everything works (run the test script `mpremote run scripts/test-bundle-protocol-agent.py`)
+3. you can also check that everything works (run the test script `mpremote run examples/local_ping_echo.py`)
+
+### Additional MicroPython Tips & Tricks
+The mpremote tool is normally interrupted by using `ctrl+c`. A special case is the REPL (simply call `mpremote`), which
+can be exited by using `ctrl+~` (tested on windows).
+
+If you start a script on MicroPython (`mpremote run ...`) and disconnect the console (`mpremote` -> `ctrl+c`) then the script 
+keeps running.
+
+If you must access the REPL via mpremote, but a script is blocking, then call `mpremote` and press EN (enable) on the 
+ESP32 for a soft-reset. Press `ctrl+c` a few times to interrupt the `boot.py` or `main.py` script execution. The session
+state is stored, so any subsequent `mpremote` call will start at REPL as long as no power disconnect is performed.
+
+You can deploy a script as `main.py` on MicroPython to be run every time the microcontroller gets power. \
+You can also remove the script. MicroPython will only execute the script if it is present.
+```shell
+$ mpremote fs cp examples/remote_echo_callback.py :main.py
+$ mpremote fs rm :main.py
+```
+
+Regarding `boot.py`, it is used for user-specific setup code and this framework uses a generic boot script that adjusts
+the ESP32's frequency and connects to a Wi-Fi network (blocking until success). MicroPython will create a dummy `boot.py`
+if none is present. MicroPython will not create a dummy `main.py` is none is present. MicroPython will first execute
+the `boot.py` and then the `main.py` if it is present.
+
 
 ## Development Information
 
 ### Development Mode
 You can install this project locally to directly reflect code changes in your environment.
 Simply run this in the project root folder (requires at least pip v21.1):
 ```shell
@@ -138,12 +174,11 @@
    - non-official, but tested micropython [library](https://github.com/glenn20/micropython/blob/espnow-g20/docs/library/espnow.rst) available, as well as [builds](https://github.com/glenn20/micropython-espnow-images) with the current firmware
 
 3. Alternative: AP_STA mode for simultaneous AP and STA without explicit ESP-MESH usage
    - only available for [Arduino+C](https://techtutorialsx.com/2021/01/04/esp32-soft-ap-and-station-modes/)
    - [painlessMesh](https://gitlab.com/painlessMesh/painlessMesh) also uses this mode to build its mesh
 
 ### Open End Topics / Known Issues
-- interface between router and cla is inconsistent (different responsibilities for send and receive)
-- dtn7rs-rest-cla and in-memory storage together use too much RAM for MicroPython (therefore the rest-cla is disabled in the simple API)
-- additional group (for example: "dtn://group/~news") registration on singleton endpoints (can there be registrations from multiple local endpoints on the same group?)
+- fragment, CRC, status-report generation support
+- dtn7rs-rest-cla and in-memory storage together use too much RAM for MicroPython (therefore the dtn7rs-rest-cla is disabled in the simple API)
 - public repository
-- api documentation (currently all information must be gathered from doc-strings and examples)
+- public documentation (currently all information must be gathered from doc-strings and examples)
```

### Comparing `dtn7zero-0.0.2/dtn7zero/api.py` & `dtn7zero-0.0.3/dtn7zero/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from typing import Optional, List, Tuple, Callable
 
 from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
 from dtn7zero.constants import IPND_IDENTIFIER_MTCP, RUNNING_MICROPYTHON
 from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
 from dtn7zero.data import Node
-from dtn7zero.endpoints import LocalEndpoint
+from dtn7zero.endpoints import LocalEndpoint, LocalGroupEndpoint
 from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
 from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
 from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
 from py_dtn7.bundle import Bundle, PrimaryBlock
 
 if RUNNING_MICROPYTHON:
     import _thread
@@ -34,25 +34,50 @@
     def __init__(self, service_name, callback=None):
         self._callback = callback
         self._endpoint = LocalEndpoint(service_name, self._simplifying_callback if callback is not None else None)
 
     def _simplifying_callback(self, bundle: Bundle):
         self._callback(bundle.payload_block.data, bundle.primary_block.full_source_uri, bundle.primary_block.full_destination_uri, bundle.primary_block)
 
-    def send(self, payload: bytes, full_destination_address: str):
+    def send(self, payload: bytes, full_destination_address: str, anonymous: bool = False):
         """ sends a payload(message) to the specified node_id and service_name
         """
-        self._endpoint.start_transmission(payload, full_destination_address)
+        self._endpoint.start_transmission(payload, full_destination_address, anonymous=anonymous)
 
     def poll(self) -> Tuple[Optional[bytes], Optional[str], Optional[str], Optional[PrimaryBlock]]:
         """ polls a passive endpoint (without callback) for a new payload(message)
 
         use pythons value unpacking feature with the methods' signature like so:
 
-        payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock = my_endpoint.poll()
+        payload, full_source_uri, full_destination_uri, primary_block = my_endpoint.poll()
+
+        the primary block is provided for direct access to additional information
+        """
+        bundle = self._endpoint.poll()
+
+        if bundle is not None:
+            return bundle.payload_block.data, bundle.primary_block.full_source_uri, bundle.primary_block.full_destination_uri, bundle.primary_block
+        return None, None, None, None
+
+
+class SimpleGroupEndpoint:
+
+    def __init__(self, full_group_uri, callback=None):
+        self._callback = callback
+        self._endpoint = LocalGroupEndpoint(full_group_uri, self._simplifying_callback if callback is not None else None)
+
+    def _simplifying_callback(self, bundle: Bundle):
+        self._callback(bundle.payload_block.data, bundle.primary_block.full_source_uri, bundle.primary_block.full_destination_uri, bundle.primary_block)
+
+    def poll(self) -> Tuple[Optional[bytes], Optional[str], Optional[str], Optional[PrimaryBlock]]:
+        """ polls a passive endpoint (without callback) for a new payload(message)
+
+        use pythons value unpacking feature with the methods' signature like so:
+
+        payload, full_source_uri, full_destination_uri, primary_block = my_endpoint.poll()
 
         the primary block is provided for direct access to additional information
         """
         bundle = self._endpoint.poll()
 
         if bundle is not None:
             return bundle.payload_block.data, bundle.primary_block.full_source_uri, bundle.primary_block.full_destination_uri, bundle.primary_block
@@ -116,14 +141,40 @@
 
     endpoint = SimpleEndpoint(endpoint_identifier, receive_callback)
     BPA.register_endpoint(endpoint._endpoint)
 
     return endpoint
 
 
+def register_group(full_group_uri: str, receive_callback: Callable[[bytes, str, str, PrimaryBlock], None] = None) -> SimpleGroupEndpoint:
+    """ registers a group-endpoint at the bundle protocol agent over which you can receive group-addressed bundles
+
+    full_group_uri examples:
+        "dtn://news/~sport", "dtn://my-group/interesting/new/~topics"
+
+    receive_callback -> may be None, but then you need to manually poll the endpoint
+
+    receive_callback signature/example:
+
+    callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
+        pass
+
+    the primary block is provided for direct access to additional information
+    """
+    global BPA
+
+    if BPA is None:
+        raise Exception('setup(node_id) was not called!')
+
+    endpoint = SimpleGroupEndpoint(full_group_uri, receive_callback)
+    BPA.register_group_endpoint(endpoint._endpoint)
+
+    return endpoint
+
+
 def discover() -> List[Node]:
     """ returns a list of all currently known other nodes in the local network
     """
     global BPA
 
     if BPA is None:
         raise Exception('setup(node_id) was not called!')
```

### Comparing `dtn7zero-0.0.2/dtn7zero/bundle_protocol_agent.py` & `dtn7zero-0.0.3/dtn7zero/bundle_protocol_agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datetime import datetime, timezone, timedelta
 from typing import Dict, List
 
 from dtn7zero.data import BundleInformation, BundleStatusReportReasonCodes
 from dtn7zero.constants import SEND_STATUS_REPORTS_ENABLED, RUNNING_MICROPYTHON
-from dtn7zero.endpoints import LocalEndpoint
+from dtn7zero.endpoints import LocalEndpoint, LocalGroupEndpoint, _LocalEndpoint
 from dtn7zero.ipnd import IPND
 from dtn7zero.routers import Router
 from dtn7zero.storage import Storage
-from dtn7zero.utility import debug
+from dtn7zero.utility import debug, is_correct_node_uri, is_correct_endpoint_uri, is_correct_group_uri
 from py_dtn7.bundle import PrimaryBlock
 
 if RUNNING_MICROPYTHON:
     from wlan import connect, isconnected
 
 
 class BundleProtocolAgent:
@@ -19,72 +19,122 @@
     def __init__(self, full_node_uri: str, storage: Storage, router: Router, use_ipnd=True):
         """ The main RFC 9171 compliant bpa component.
 
         full_node_uri examples:
             dtn addressing scheme -> "dtn://node1/", "dtn://cool-node/"  # '/' at the end is mandatory
             ipn addressing scheme -> "ipn://12", "ipn://24.25"  # will be joined with the endpoints via '.'
         """
+        assert is_correct_node_uri(full_node_uri)
+
         self.full_node_uri = full_node_uri
         self.storage = storage
         self.router = router
-        self.local_registered_endpoints: Dict[str, LocalEndpoint] = {}
+        self.local_registered_endpoints: Dict[str, List[_LocalEndpoint]] = {}
 
         self.local_bundle_dispatch_queue: List[BundleInformation] = []  # this pipeline-stage is needed to prevent infinite-recursion if two local endpoints answer each other on every reception-callback
+        self.storage_retry_generator = None
+        self.router_poll_generator = None
 
         self.use_ipnd = use_ipnd
         if self.use_ipnd:
+            # on micropython we need to handle wireless connections manually
+            if RUNNING_MICROPYTHON and not isconnected():
+                connect()  # the microcontroller may be moved around, so connect to any available network instead of reconnect
+
             scheme_encoded, node_encoded = PrimaryBlock.from_full_uri(full_node_uri)
             self.ipnd = IPND(scheme_encoded, node_encoded, storage)
 
     def update(self):
         # on micropython we need to handle wireless connections manually
         if RUNNING_MICROPYTHON and not isconnected():
             connect()  # the microcontroller may be moved around, so connect to any available network instead of reconnect
 
         # update discovery
         if self.use_ipnd:
             self.ipnd.update()
 
-        # process new local bundles
-        while self.local_bundle_dispatch_queue:
+        # process stored/delayed bundle
+        if self.storage_retry_generator is None:
+            self.storage_retry_generator = self.storage.get_bundles_to_retry()
+
+        try:
+            self.bundle_dispatching(next(self.storage_retry_generator))
+        except StopIteration:
+            self.storage_retry_generator = None
+
+        # process one new local bundle
+        if self.local_bundle_dispatch_queue:
             self.bundle_reception(self.local_bundle_dispatch_queue.pop(0))
 
-        # process new remote bundles
-        # todo: check if there must be a max-counter to avoid a busy deadlock
-        for bundle_information in self.router.generator_poll_bundles():
-            self.bundle_reception(bundle_information)
-
-        # process stored/delayed bundles
-        for bundle_information in self.storage.get_bundles_to_retry():
-            self.bundle_dispatching(bundle_information)
+        # process new remote bundle
+        if self.router_poll_generator is None:
+            self.router_poll_generator = self.router.generator_poll_bundles()
+
+        try:
+            self.bundle_reception(next(self.router_poll_generator))
+        except StopIteration:
+            self.router_poll_generator = None
 
     def register_endpoint(self, endpoint: LocalEndpoint) -> LocalEndpoint:
         """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
         […] * commencing a registration (registering the node in an endpoint).
         """
         endpoint.bpa_register(self)
 
+        assert is_correct_endpoint_uri(endpoint.full_endpoint_uri)
+
         if endpoint.full_endpoint_uri in self.local_registered_endpoints:
+            endpoint.bpa_unregister()
             raise Exception('tried to register local endpoint {}, which is already registered as a local endpoint'.format(endpoint.endpoint_identifier))
 
-        self.local_registered_endpoints[endpoint.full_endpoint_uri] = endpoint
+        self.local_registered_endpoints[endpoint.full_endpoint_uri] = (endpoint,)
+
+        return endpoint
+
+    def register_group_endpoint(self, endpoint: LocalGroupEndpoint) -> LocalGroupEndpoint:
+        """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
+        […] * commencing a registration (registering the node in an endpoint).
+        """
+        assert is_correct_group_uri(endpoint.full_endpoint_uri)
+
+        endpoint.bpa_register(self)
+
+        if endpoint.full_endpoint_uri in self.local_registered_endpoints:
+            self.local_registered_endpoints[endpoint.full_endpoint_uri].append(endpoint)
+        else:
+            self.local_registered_endpoints[endpoint.full_endpoint_uri] = [endpoint]
 
         return endpoint
 
     def unregister_endpoint(self, endpoint: LocalEndpoint):
         """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
         […] * terminating a registration.
         """
         if endpoint.full_endpoint_uri not in self.local_registered_endpoints:
             raise Exception('tried to unregister non-existent local endpoint {}'.format(endpoint.endpoint_identifier))
 
         full_endpoint_uri = endpoint.full_endpoint_uri
-        self.local_registered_endpoints[full_endpoint_uri].bpa_unregister()
+        self.local_registered_endpoints[full_endpoint_uri][0].bpa_unregister()
         del self.local_registered_endpoints[full_endpoint_uri]
 
+    def unregister_group_endpoint(self, endpoint: LocalGroupEndpoint):
+        """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
+        […] * terminating a registration.
+        """
+        if endpoint.full_endpoint_uri not in self.local_registered_endpoints:
+            raise Exception('tried to unregister non-existent local group endpoint {}'.format(endpoint.full_endpoint_uri))
+
+        try:
+            self.local_registered_endpoints[endpoint.full_endpoint_uri].remove(endpoint)
+        except ValueError:
+            raise Exception('tried to unregister non-existent local group endpoint {}'.format(endpoint.full_endpoint_uri))
+
+        if not self.local_registered_endpoints[endpoint.full_endpoint_uri]:
+            del self.local_registered_endpoints[endpoint.full_endpoint_uri]
+
     def cancel_transmission(self, bundle_id: str) -> bool:
         """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
         […] * canceling a transmission.
         """
         # should only be called by a local endpoint
         # returns True if the bundle was still in local storage to delete, False otherwise
         return self.storage.remove_bundle(bundle_id)
@@ -146,21 +196,14 @@
 
             if flags.delete_bundle_if_block_cant_be_processed:
                 self.bundle_deletion(bundle_information, BundleStatusReportReasonCodes.BLOCK_UNSUPPORTED)
                 return
             elif flags.discard_block_if_block_cant_be_processed:
                 bundle.other_blocks.remove(block)
 
-        # There are two additional reasons to reject a bundle -> hop count exceeded and lifetime expired.
-        # The point at which they should be checked is unspecified, although section 5.4 Bundle Forwarding
-        # hints a check with "contraindication of forwarding".
-        # But, hop-count and bundle-age are updated at the latest point before sending, which gives the bundle an
-        # "unlimited" lifetime in this node anyway.
-        # todo: check if and where a lifetime-expired check is needed for stored bundles
-        # So, we can safely check both directly at bundle reception and let the next node deal with expiration caused by us.
         """ 4.4.3 Hop Count
         […] When a bundle's hop count exceeds its hop limit, the bundle SHOULD be deleted for the reason "Hop limit 
         exceeded", following the Bundle Deletion procedure defined in Section 5.10.
         """
         if bundle.hop_count_block and bundle.hop_count_block.hop_count >= bundle.hop_count_block.hop_limit:
             self.bundle_deletion(bundle_information, BundleStatusReportReasonCodes.HOP_LIMIT_EXCEEDED)
             return
@@ -180,15 +223,15 @@
 
     def bundle_dispatching(self, bundle_information: BundleInformation):
         """ RFC 9171, 5.3 Bundle Dispatching
         […] Step 1: If the bundle's destination endpoint is an endpoint of which the node is a member, 
         the Bundle Delivery procedure defined in Section 5.7 MUST be followed and, […] the node SHALL NOT undertake to 
         forward the bundle to itself in the course of performing the procedure described in Section 5.4. […]
         """
-        if bundle_information.bundle.primary_block.full_destination_uri in self.local_registered_endpoints:
+        if not bundle_information.locally_delivered and bundle_information.bundle.primary_block.full_destination_uri in self.local_registered_endpoints:
             self.local_bundle_delivery(bundle_information)
 
         """ RFC 9171, 5.3 Bundle Dispatching
         […] Step 2: Processing proceeds from Step 1 of Section 5.4.
         """
         self.bundle_forwarding(bundle_information)
 
@@ -207,16 +250,19 @@
         """ RFC 9171, 5.7 Local Bundle Delivery
         […] Step 2: Delivery depends on the state of the registration whose endpoint ID matches that of the destination 
         of the bundle:
         
         * An additional implementation-specific delivery deferral procedure MAY optionally be associated with the 
         registration. […]
         """
-        full_destination_uri = bundle_information.bundle.primary_block.full_destination_uri
-        self.local_registered_endpoints[full_destination_uri].bpa_local_bundle_delivery(bundle_information.bundle)
+        bundle_information.locally_delivered = True
+
+        # on group-endpoints there can be multiple registrations, on unicast-endpoints this is a 1-tuple
+        for endpoint in self.local_registered_endpoints[bundle_information.bundle.primary_block.full_destination_uri]:
+            endpoint.bpa_local_bundle_delivery(bundle_information.bundle)
 
     def bundle_forwarding(self, bundle_information: BundleInformation):
 
         """ RFC 9171, 5.4 Bundle Forwarding
         […] Step 1: The retention constraint "Forward pending" MUST be added to the bundle, and the bundle's 
         "Dispatch pending" retention constraint MUST be removed. […]
         """
@@ -247,15 +293,14 @@
             )
 
             if reason in no_failure_codes:
                 """ RFC 9171, 5.4.1 Forwarding Contraindicated
                 […] when -- at some future time -- the forwarding of this bundle ceases to be contraindicated, 
                 processing proceeds from Step 4 of Section 5.4. […]
                 """
-                # todo: maybe remove old bundles from storage -> is this a storage implementation matter?
                 storage_success, removed_bundle_informations = self.storage.delay_bundle(bundle_information)
 
                 if not storage_success:
                     reason = BundleStatusReportReasonCodes.DEPLETED_STORAGE
 
                 for removed_bundle_information in removed_bundle_informations:
                     if len(removed_bundle_information.forwarded_to_nodes) > 0:
@@ -273,15 +318,15 @@
                 """ RFC 9171, 5.4.2 Forwarding Failed
                 […] Step 1: The BPA MAY forward the bundle back to the node that sent it, as identified by the Previous 
                 Node Block, if present. This forwarding, if performed, SHALL be accomplished by performing Step 4 and 
                 Step 5 of Section 5.4 where the sole node selected for forwarding SHALL be the node that sent the 
                 bundle. […]
                 """
                 if bundle_information.bundle.previous_node_block:
-                    self.router.send_to_previous_node(self.full_node_uri, bundle_information)  # todo: check steps and implement correctly
+                    self.router.send_to_previous_node(self.full_node_uri, bundle_information)
 
                 """ RFC 9171, 5.4.2 Forwarding Failed
                 […] Step 2: If the bundle's destination endpoint is an endpoint of which the node is a member, 
                 then the bundle's "Forward pending" retention constraint MUST be removed. Otherwise, the bundle MUST be 
                 deleted: the Bundle Deletion procedure defined in Section 5.10 MUST be followed, citing the reason for 
                 which forwarding was determined to be contraindicated.
                 """
```

### Comparing `dtn7zero-0.0.2/dtn7zero/constants.py` & `dtn7zero-0.0.3/dtn7zero/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,32 +17,29 @@
 
 if RUNNING_MICROPYTHON:
     IPND_BEACON_MAX_SIZE = 256  # for some reason a bigger datagram receive leads to memory leaks ???
 else:
     IPND_BEACON_MAX_SIZE = 4096
 
 if RUNNING_MICROPYTHON:
-    MTCP_MAX_CONNECTIONS_STATE_WAITING = 1
-    MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE = 4
+    MTCP_MAX_CONNECTIONS_STATE_WAITING = 2
+    MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE = 3
     MTCP_TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE = 5000
 else:
     MTCP_MAX_CONNECTIONS_STATE_WAITING = 5
     MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE = 10000
     MTCP_TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE = 1000000
 
-MTCP_TIMEOUT_MILLISECONDS_STALLED_SEND = 500
-MTCP_TIMEOUT_SECONDS_OPEN_SEND_CONNECTION = 1
+MTCP_TIMEOUT_MILLISECONDS_STALLED_SEND = 2000
 
 PORT_BEACON_UDP = 7000
 PORT_REST = 3000
 PORT_MTCP = 16162
 PORT_IPND = 3003
 
-RETRY_INTERVAL_MILLISECONDS = 5000
-
 SEND_STATUS_REPORTS_ENABLED = False
 
 SIMPLE_EPIDEMIC_ROUTER_MIN_NODES_TO_FORWARD_TO = 3
 
 if RUNNING_MICROPYTHON:
     SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES = 7  # experimental setting
     SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS = 18  # experimental setting
```

### Comparing `dtn7zero-0.0.2/dtn7zero/convergence_layer_adapters/__init__.py` & `dtn7zero-0.0.3/dtn7zero/convergence_layer_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py` & `dtn7zero-0.0.3/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/dtn7zero/convergence_layer_adapters/mtcp.py` & `dtn7zero-0.0.3/dtn7zero/convergence_layer_adapters/mtcp.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 try:
     from cbor2 import dumps
 except ImportError:
     from cbor import dumps
 
 from dtn7zero.constants import PORT_MTCP, MTCP_MAX_CONNECTIONS_STATE_WAITING, SOCKET_RECEIVE_BUFFER_SIZE, \
     MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE, MTCP_TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE, \
-    MTCP_TIMEOUT_MILLISECONDS_STALLED_SEND, RUNNING_MICROPYTHON, MTCP_TIMEOUT_SECONDS_OPEN_SEND_CONNECTION, \
-    IPND_IDENTIFIER_MTCP
+    MTCP_TIMEOUT_MILLISECONDS_STALLED_SEND, RUNNING_MICROPYTHON, IPND_IDENTIFIER_MTCP
 from dtn7zero.convergence_layer_adapters import CLA
 from dtn7zero.data import Node
 from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout, debug, warning
 from py_dtn7 import Bundle
 
 
 TYPE_BYTES = 0x40
@@ -112,50 +111,62 @@
 
     return _receive_exactly_n_bytes(connection, aux)
 
 
 def _send_message(address, port, message):
     # create a standard ipv4 stream socket
     client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    client_socket.settimeout(MTCP_TIMEOUT_SECONDS_OPEN_SEND_CONNECTION)
-    # connect to node
-    # this will raise an error when it cannot be completed immediately
+    client_socket.settimeout(0)
+
+    '''
+    Connection Establishment Analysis
+
+    Problem
+    socket.settimeout(1) -> does not set the desired timeout on MicroPython (ESP32-GENERIC), 
+    but instead keeps the default timeout of about 12 seconds.
+
+    Analysis
+    The following OSError numbers (e.errno) are thrown on MicroPython on connecting with a non-blocking socket:
+    119 EINPROGRESS  -> thrown by the connect request on a non-blocking socket
+     11 EAGAIN       -> thrown if no data could be sent (also thrown on sending b'')
+
+    Solution
+    As we cannot be sure when the socket is connected we just skip the connect timeout and go straight to the deadlock timeout.
+    To be consistent on MicroPython and CPython we do this on both.
+    '''
+
     try:
         client_socket.connect((address, port))
     except OSError:
-        warning('mtcp could not connect to node: {}'.format(address))
-        raise RemoteClosedConnectionException()
-    # change to non-blocking mode
-    # MicroPython supports only one thread/process, and therefore we need to implement everything synchronous
-    client_socket.settimeout(0)
+        # this will raise an exception on non-blocking sockets
+        pass
 
     deadlock_check = get_current_clock_millis()
-
     while len(message) > 0 and not is_timestamp_older_than_timeout(deadlock_check, MTCP_TIMEOUT_MILLISECONDS_STALLED_SEND):
         try:
             bytes_sent = client_socket.send(message)
         # Windows behaviour??? If other end is forcibly closed it raises an ConnectionResetError -> OSError
-        except OSError as e:
-            if e.args[0] == 11:
-                # EAGAIN Error was raised, which states "try again, the buffer is full"
-                pass
-            else:
-                client_socket.close()
-                raise RemoteClosedConnectionException(e)
+        except OSError:
+            # We ignore all OSErrors.
+            # The correct way would be to check the errno for "busy" (MicroPython -> 11, CPython+Windows -> 10035)
+            # but, because it is implementation dependent, and we do not expect the receiver to immediately close the
+            # connection, we accept the rare case of a deadlock-timeout because of an early-closed socket.
+            pass
         else:
             # on 0 bytes sent the socket connection is closed
             if bytes_sent == 0:
                 client_socket.close()
                 raise RemoteClosedConnectionException("0 bytes")
             # update the message and length to send
             message = message[bytes_sent:]
             # update our deadlock-check as we managed to send some data
             deadlock_check = get_current_clock_millis()
 
     if len(message) > 0:
+        client_socket.close()
         raise RemoteStalledConnectionException()
 
     client_socket.close()
 
 
 class MTcpCLA(CLA):
 
@@ -202,15 +213,15 @@
     def _poll_from_open_receive_connections(self):
         serialized_bundle, from_node_address = None, None
 
         for address_tuple, (connection, last_received) in tuple(self.open_receive_connections.items()):
             try:
                 serialized_bundle = _read_full_message_or_none(connection)
             except RemoteClosedConnectionException:
-                warning('remote closed down incoming mtcp connection {}'.format(address_tuple))
+                debug('remote closed down incoming mtcp connection {}'.format(address_tuple))
                 if not RUNNING_MICROPYTHON:
                     connection.shutdown(socket.SHUT_RDWR)
                 connection.close()
                 del self.open_receive_connections[address_tuple]
             except ReceivedInvalidDataOnSocketException as e:
                 warning('incoming mtcp connection {} sent invalid data, discarding connection, error: {}'.format(address_tuple, e))
                 if not RUNNING_MICROPYTHON:
@@ -252,20 +263,20 @@
                 if serialized_bundle is not None:
                     from_node_address = address_tuple[0]
                     break
 
         return serialized_bundle, from_node_address
 
     def _check_for_new_connections(self):
-        while len(self.open_receive_connections) < MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE:
+        if len(self.open_receive_connections) < MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE:
             try:
                 client_socket, address_tuple = self.socket.accept()
             except OSError:
                 # no new connect request waiting
-                break
+                pass
             else:
                 # change to non-blocking mode to be able to poll without blocking
                 client_socket.settimeout(0)
 
                 # we allow multiple connections from one IP address, because if we accept the connection, the whole bundle
                 #  could be already transmitted before we can close the connection from our checks
                 #  -> would lead to false positive on the sender side
@@ -280,10 +291,11 @@
         message = dumps(serialized_bundle)
 
         if IPND_IDENTIFIER_MTCP in node.clas:
             try:
                 port = node.clas[IPND_IDENTIFIER_MTCP]
                 _send_message(node.address, port, message)
             except (RemoteClosedConnectionException, RemoteStalledConnectionException):
+                del node.clas[IPND_IDENTIFIER_MTCP]  # the node can re-announce it, but currently we cannot connect
                 return False
             return True
         return False
```

### Comparing `dtn7zero-0.0.2/dtn7zero/data.py` & `dtn7zero-0.0.3/dtn7zero/data.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,35 +20,41 @@
     HOP_LIMIT_EXCEEDED = 9
     TRAFFIC_PARED = 10
     BLOCK_UNSUPPORTED = 11
 
 
 class Node:
 
-    def __init__(self, address: str, eid: Tuple[int, str], clas: Dict[str, int]):
+    def __init__(self, address: str, eid: Tuple[int, str], clas: Dict[str, int], sequence_number: int):
         self.address = address  # the IP address of the node
         # todo: currently a node is identified by its IP address, maybe this requires changes sometime in the future.
         # storage also depends on the address field as the unique identifier of a node
 
         self.eid = eid  # DTN node id, a tuple of "address-type" (1 or 2) and "the node-id" in the correct format -> for type 1 (DTN) -> example: "//node1/"
         self.clas = clas  # a list of tuples, consisting of the ipnd-cla-identifier + application port
+        self.sequence_number = sequence_number
 
         self.latest_discovery = get_current_clock_millis()
 
     def merge_new_info(self, eid_scheme: int, eid_specific_part: str, clas: Dict[str, int]):
         if eid_specific_part is not None:
             self.eid = (eid_scheme, eid_specific_part)
         self.clas = clas  # replace with new information -> clas might have gotten deactivated
 
         self.latest_discovery = get_current_clock_millis()
 
+    def advance_sequence_number(self, new_sequence_number: int) -> bool:
+        old_sequence_number = self.sequence_number
+        self.sequence_number = new_sequence_number
+        return old_sequence_number + 1 == new_sequence_number
+
 
 class BundleInformation:
     RETENTION_CONSTRAINT_DISPATCH_PENDING = 'Dispatch pending'
     RETENTION_CONSTRAINT_FORWARD_PENDING = 'Forward pending'
 
     def __init__(self, bundle: Bundle):
         self.bundle = bundle
         self.retention_constraint = None
-        self.last_forwarding_attempt_ms = 0
+        self.locally_delivered = False
         self.received_at_ms = get_current_clock_millis()
         self.forwarded_to_nodes: List[Node] = []
```

### Comparing `dtn7zero-0.0.2/dtn7zero/endpoints.py` & `dtn7zero-0.0.3/dtn7zero/endpoints.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,76 @@
 from typing import Callable
 
 from dtn7zero.constants import RUNNING_MICROPYTHON, PORT_REST
 from dtn7zero.data import BundleInformation
 from dtn7zero.utility import debug
 from py_dtn7 import Bundle, DTNRESTClient, to_dtn_timestamp
-from py_dtn7.bundle import BundleProcessingControlFlags, PrimaryBlock, HopCountBlock, PayloadBlock, BundleAgeBlock, NONE_ENDPOINT_SPECIFIC_PART_NAME
+from py_dtn7.bundle import BundleProcessingControlFlags, PrimaryBlock, HopCountBlock, PayloadBlock, BundleAgeBlock, \
+    NONE_ENDPOINT_SPECIFIC_PART_NAME, URI_SCHEME_DTN_NAME
 
 
-class LocalEndpoint:
-    def __init__(self, endpoint_identifier: str, receive_callback=Callable[[Bundle], None]):
-        """ The LocalEndpoint is the entry-point for the application to send/receive bundles.
-
-        endpoint_identifier examples:
-            dtn addressing scheme -> "echo", "echo/subecho"
-            ipn addressing scheme -> "12", "24.15.16"
-
-        callback may be None, but then the endpoint should be regularly polled for new bundles.
-        """
+class _LocalEndpoint:
 
-        self.endpoint_identifier = endpoint_identifier
+    def __init__(self, receive_callback: Callable[[Bundle], None] = None):
+        self.bpa = None
         self.receive_callback = receive_callback
 
         if receive_callback is None:
             self.bundle_buffer: list[Bundle] = []
 
-        self.bpa = None
-
-        self.last_bundle_creation_time = 0
-        self.last_sequence_number = 0
-
     def bpa_local_bundle_delivery(self, bundle: Bundle):
         if self.receive_callback is None:
             self.bundle_buffer.append(bundle)
         else:
             self.receive_callback(bundle)
 
-    @property
-    def full_endpoint_uri(self):
-        if self.bpa.full_node_uri.startswith('dtn'):
-            return '{}{}'.format(self.bpa.full_node_uri, self.endpoint_identifier)
-        elif not self.endpoint_identifier:
-            return self.bpa.full_node_uri  # special case -> ipn addressing + '' empty endpoint (direct node endpoint)
-        else:
-            return '{}.{}'.format(self.bpa.full_node_uri, self.endpoint_identifier)
-
     def bpa_register(self, bpa):
         self.bpa = bpa
 
     def bpa_unregister(self):
         self.bpa = None
 
     def poll(self):
         if self.receive_callback is not None:
-            raise Exception('cannot poll active endpoint with callback {}'.format(self.endpoint_identifier))
+            raise Exception('cannot poll active endpoint with callback {}'.format(self.full_endpoint_uri))
         if not self.bundle_buffer:
             return None
         return self.bundle_buffer.pop(0)
 
+    @property
+    def full_endpoint_uri(self) -> str:
+        return 'dtn://none'
+
+
+class LocalEndpoint(_LocalEndpoint):
+    def __init__(self, endpoint_identifier: str, receive_callback: Callable[[Bundle], None] = None):
+        """ The LocalEndpoint is the entry-point for the application to send/receive bundles.
+
+        endpoint_identifier examples:
+            dtn addressing scheme -> "echo", "echo/subecho"
+            ipn addressing scheme -> "12", "24.15.16"
+
+        receive_callback may be None, but then the endpoint should be regularly polled for new bundles.
+        """
+        super().__init__(receive_callback)
+
+        self.endpoint_identifier = endpoint_identifier
+
+        self.last_bundle_creation_time = 0
+        self.last_sequence_number = 0
+
+    @property
+    def full_endpoint_uri(self) -> str:
+        if self.bpa.full_node_uri.startswith(URI_SCHEME_DTN_NAME):
+            return '{}{}'.format(self.bpa.full_node_uri, self.endpoint_identifier)
+        elif not self.endpoint_identifier:
+            return self.bpa.full_node_uri  # special case -> ipn addressing + '' empty endpoint (direct node endpoint)
+        else:
+            return '{}.{}'.format(self.bpa.full_node_uri, self.endpoint_identifier)
+
     def start_transmission(self, payload: bytes, full_destination_uri: str, lifetime: int = 3600 * 24 * 1000, anonymous=False) -> str:
         if self.bpa is None:
             raise Exception('cannot start transmission on unregistered LocalEndpoint {}'.format(self.endpoint_identifier))
 
         bundle_processing_control_flags = BundleProcessingControlFlags(0)
         bundle_processing_control_flags.set_flag(2)  # do not fragment bundle
 
@@ -74,15 +84,15 @@
             current_time = to_dtn_timestamp()
             if current_time == self.last_bundle_creation_time:
                 self.last_sequence_number += 1
             else:
                 self.last_bundle_creation_time = current_time
                 self.last_sequence_number = 0
 
-        if full_destination_uri.startswith('dtn'):
+        if full_destination_uri.startswith(URI_SCHEME_DTN_NAME):
             anonymous_uri = 'dtn:{}'.format(NONE_ENDPOINT_SPECIFIC_PART_NAME)
         else:
             anonymous_uri = 'ipn:{}'.format(NONE_ENDPOINT_SPECIFIC_PART_NAME)
 
         primary_block = PrimaryBlock.from_objects(
             full_destination_uri=full_destination_uri,
             full_source_uri=anonymous_uri if anonymous else self.full_endpoint_uri,
@@ -113,46 +123,68 @@
     def cancel_transmission(self, bundle_id: str) -> bool:
         if self.bpa is None:
             raise Exception('cannot cancel transmission on unregistered LocalEndpoint {}'.format(self.endpoint_identifier))
 
         return self.bpa.cancel_transmission(bundle_id)
 
 
-class RemoteEndpoint:
+class LocalGroupEndpoint(_LocalEndpoint):
+
+    def __init__(self, full_group_uri: str, receive_callback: Callable[[Bundle], None] = None):
+        """ The LocalGroupEndpoint can be used to receive bundles which are addressed to groups.
+
+        full_group_uri examples:
+            "dtn://news/~sport", "dtn://my-group/interesting/new/~topics"
 
-    def __init__(self, dtn7rs_ip: str, endpoint_specific_part: str):
+        Like the with unicast-endpoint (LocalEndpoint), an uri is matched in full.
+        There is no subgroup matching functionality.
+
+        receive_callback may be None, but then the endpoint should be regularly polled for new bundles.
+        """
+        super().__init__(receive_callback)
+
+        self.full_group_uri = full_group_uri
+
+    @property
+    def full_endpoint_uri(self) -> str:
+        return self.full_group_uri
+
+
+class ExternalEndpoint:
+
+    def __init__(self, dtn7rs_ip: str, endpoint_identifier: str):
         """
         This is a relic of a time when we could not generate bundles on our own.
 
         It is functional and encapsulated, meaning it requires no other dtn7zero dependencies to operate.
         """
-        self.endpoint_specific_part = endpoint_specific_part
+        self.endpoint_identifier = endpoint_identifier
 
         self.dtn_rest_client: DTNRESTClient = DTNRESTClient('http://{}'.format(dtn7rs_ip), PORT_REST)
 
-        self.dtn_rest_client.register(self.endpoint_specific_part)
+        self.dtn_rest_client.register(self.endpoint_identifier)
 
     def __del__(self):
-        self.dtn_rest_client.unregister(self.endpoint_specific_part)
+        self.dtn_rest_client.unregister(self.endpoint_identifier)
 
     @property
     def full_endpoint_address(self):
-        return '//{}/{}'.format(self.dtn_rest_client.node_id, self.endpoint_specific_part)
+        return '//{}/{}'.format(self.dtn_rest_client.node_id, self.endpoint_identifier)
 
     def poll(self):
-        raw_bundle = self.dtn_rest_client.fetch_endpoint(self.endpoint_specific_part)
+        raw_bundle = self.dtn_rest_client.fetch_endpoint(self.endpoint_identifier)
 
         if b'Nothing to receive' == raw_bundle:
             return None
         else:
             return Bundle.from_cbor(raw_bundle)
 
     def start_transmission(self, payload: bytes, full_destination_uri: str, lifetime: int = 3600 * 24 * 1000) -> str:
         if self.dtn_rest_client is None:
-            raise Exception('cannot start transmission on unregistered RemoteEndpoint {}'.format(self.endpoint_specific_part))
+            raise Exception('cannot start transmission on unregistered RemoteEndpoint {}'.format(self.endpoint_identifier))
 
         response = self.dtn_rest_client.send(payload=payload, destination=full_destination_uri, lifetime=lifetime)
 
         if response.status_code != 200:
             raise Exception('error occurred on generating a bundle on RemoteEndpoint {}'.format(self.full_endpoint_address))
 
         return ''  # currently we do not get the bundle-id of the generated bundle from the remote :(
```

### Comparing `dtn7zero-0.0.2/dtn7zero/ipnd.py` & `dtn7zero-0.0.3/dtn7zero/ipnd.py`

 * *Files 15% similar despite different names*

```diff
@@ -163,77 +163,14 @@
 
     def is_continuous_with_old_beacon_sequence_number(self, old_beacon_sequence_number: int):
         if old_beacon_sequence_number == 0xffffffff:
             return self.beacon_sequence_number == 0
         return self.beacon_sequence_number == old_beacon_sequence_number
 
 
-'''
-# Minimal-overhead-way of extracting and building beacon information.
-# Was in use until the beacon-class was identified as not being the memory leak.
-# Memory-leak seems to appear at the reading of UDP-datagrams > 256 byte.
-
-def extract_beacon_information_from(raw_data: bytes) -> Tuple[int, str, list, dict]:
-    block_data = loads(raw_data)
-
-    if block_data[0] != 7:
-        raise NotImplementedError('beacons with other versions than 7 are currently not supported')
-
-    flags = BeaconFlags(block_data[1])
-
-    expected_length = 3 + int(flags.eid_present) + int(flags.service_block_present) + int(flags.beacon_period_present)
-    if len(block_data) != expected_length:
-        raise IndexError('cannot decode beacon because actual length {} differs from length, suggested by flags {}. block data: {}'.format(len(block_data), expected_length, block_data))
-
-    if flags.eid_present:
-        if isinstance(block_data[2], int):
-            eid_scheme, eid_specific_part = block_data[3]
-        else:
-            eid_scheme, eid_specific_part = block_data[2]
-    else:
-        eid_scheme, eid_specific_part = None, None
-
-    if flags.service_block_present:
-        if flags.eid_present:
-            clas, services = block_data[4]
-        else:
-            clas, services = block_data[3]
-    else:
-        clas, services = (), {}
-
-    return eid_scheme, eid_specific_part, clas, services
-
-
-def create_minimal_output_beacon(eid_scheme, eid_specific_part):
-    flags = BeaconFlags()
-    flags.set_flag(0)
-    flags.set_flag(1)
-
-    return [7, flags.flags, (eid_scheme, eid_specific_part), 0, (((IPND_IDENTIFIER_MTCP, PORT_MTCP),), {})]
-
-
-def minimal_output_beacon_increase_counter_by_one(beacon):
-    # ipnd-thesis states to use an unsigned 32bit integer and wrap around on overflow
-    beacon[3] = (beacon[3] + 1) & 0xffffffff
-
-
-def minimal_output_beacon_add_unicast(beacon):
-    beacon[4][1][42] = (b'unicast',)
-
-
-def minimal_output_beacon_remove_unicast(beacon):
-    del beacon[4][1][42]
-
-
-def beacon_services_contain_unicast(services):
-    return 42 in services and services[42][0] == b'unicast'
-
-'''
-
-
 class IPND:
 
     """
     for now, we only support broadcast on all interfaces and IPv4 only.
     todo: extend functionality to filter network interfaces and support IPv6
     todo: extend functionality to delete nodes after a beacon timeout
     """
@@ -277,39 +214,39 @@
                 # eid_scheme, eid_specific_part, clas, services = extract_beacon_information_from(raw_data)
                 beacon = Beacon.from_cbor(raw_data)
             except Exception as e:
                 warning('could not decode beacon. error: {}'.format(e))
             else:
                 if address not in self.own_addresses:
                     existing_node = self.storage.get_node(address)
+
                     if existing_node is None:
                         debug('received beacon from new node: {}, size: {}'.format(address, len(raw_data)))
 
-                        # new_node = Node(address, (eid_scheme, eid_specific_part), dict(clas))
-                        new_node = Node(address, (beacon.eid_scheme, beacon.eid_specific_part), dict(beacon.service_block[0]))
+                        new_node = Node(address, (beacon.eid_scheme, beacon.eid_specific_part), dict(beacon.service_block[0]), beacon.beacon_sequence_number)
                         self.storage.add_node(new_node)
 
+                        sequence_number_matches = False
+                    else:
+                        debug('received beacon from known node: {}, size: {}'.format(address, len(raw_data)))
+                        # existing_node.merge_new_info(eid_scheme, eid_specific_part, dict(clas))
+                        existing_node.merge_new_info(beacon.eid_scheme, beacon.eid_specific_part, dict(beacon.service_block[0]))
+
+                        sequence_number_matches = existing_node.advance_sequence_number(beacon.beacon_sequence_number)
+
+                    if not sequence_number_matches:
                         # send back a uni-cast beacon to a previously unknown node for faster knowledge spread
                         # ideal case: it never received a beacon from us -> current state (sequence number) is new to the node
                         # not ideal case: beacons were exchanged concurrently -> state (sequence number) is duplicate, which is unspecified and ideally ignored
                         # dtn7zero specific detail: we add unicast information to the beacon, so there is no second unicast beacon sent back to us
 
-                        # if not beacon_services_contain_unicast(services):
-                        #     minimal_output_beacon_add_unicast(self.own_beacon)
-                        #     self.send_own_beacon_to(address)
-                        #     minimal_output_beacon_remove_unicast(self.own_beacon)
-
                         if not (42 in beacon.service_block[1] and beacon.service_block[1][42] == b'unicast'):
                             self.own_beacon.service_block[1][42] = b'unicast'
                             self.send_own_beacon_to(address)
                             del self.own_beacon.service_block[1][42]
-                    else:
-                        debug('received beacon from known node: {}, size: {}'.format(address, len(raw_data)))
-                        # existing_node.merge_new_info(eid_scheme, eid_specific_part, dict(clas))
-                        existing_node.merge_new_info(beacon.eid_scheme, beacon.eid_specific_part, dict(beacon.service_block[0]))
 
         if is_timestamp_older_than_timeout(self.last_beacon_broadcast, IPND_SEND_INTERVAL_MILLISECONDS):
             for address in self.broadcast_addresses:
                 self.send_own_beacon_to(address)
             # minimal_output_beacon_increase_counter_by_one(self.own_beacon)
             self.own_beacon.increment_beacon_sequence_number_by_one()
             self.last_beacon_broadcast = get_current_clock_millis()
```

### Comparing `dtn7zero-0.0.2/dtn7zero/routers/__init__.py` & `dtn7zero-0.0.3/dtn7zero/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/dtn7zero/routers/simple_epidemic_router.py` & `dtn7zero-0.0.3/dtn7zero/routers/simple_epidemic_router.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         if IPND_IDENTIFIER_MTCP in self.clas:
             for bundle_information in self._generator_poll_simple(self.clas[IPND_IDENTIFIER_MTCP]):
                 yield bundle_information
 
     def _generator_poll_simple(self, cla: CLA):
         bundle, node_address = cla.poll()
         while bundle is not None:
-            if not self.storage.get_seen(bundle.bundle_id):
+            if not self.storage.was_seen(bundle.bundle_id):
                 self.storage.store_seen(bundle.bundle_id, node_address)
 
                 bundle_information = BundleInformation(bundle)
 
                 node = self.storage.get_node(node_address)
                 if node is not None:  # if node is known, prevent the bundle from being sent back to that same node
                     bundle_information.forwarded_to_nodes.append(node)
@@ -41,15 +41,15 @@
                 yield bundle_information
             bundle, node_address = cla.poll()
 
     def _generator_poll_advanced(self, node: Node, cla: CLA):
         bundle_ids = cla.poll_ids(node)
 
         for bundle_id in bundle_ids:
-            if not self.storage.get_seen(bundle_id):
+            if not self.storage.was_seen(bundle_id):
                 bundle, node_polled_address = cla.poll(bundle_id, node)
                 if bundle is not None:
                     self.storage.store_seen(bundle_id, node_polled_address)
 
                     bundle_information = BundleInformation(bundle)
 
                     node = self.storage.get_node(node_polled_address)
```

### Comparing `dtn7zero-0.0.2/dtn7zero/storage/__init__.py` & `dtn7zero-0.0.3/dtn7zero/storage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
     def get_node(self, node_address: str) -> Optional[Node]:
         raise NotImplementedError('do not instantiate Storage class directly')
 
     def get_nodes(self) -> Iterable[Node]:
         raise NotImplementedError('do not instantiate Storage class directly')
 
+    def was_seen(self, bundle_id: str) -> bool:
+        raise NotImplementedError('do not instantiate Storage class directly')
+
     def get_seen(self, bundle_id: str) -> Optional[str]:
         raise NotImplementedError('do not instantiate Storage class directly')
 
     def store_seen(self, bundle_id: str, node: Optional[str]):
         raise NotImplementedError('do not instantiate Storage class directly')
 
     def remove_bundle(self, bundle_id: str) -> bool:
```

### Comparing `dtn7zero-0.0.2/dtn7zero/storage/simple_in_memory_storage.py` & `dtn7zero-0.0.3/dtn7zero/storage/simple_in_memory_storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import time
 from typing import Dict, Tuple, List, Optional, Iterable
 
-from dtn7zero.constants import RETRY_INTERVAL_MILLISECONDS, SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES, SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS
+from dtn7zero.constants import SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES, SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS
 from dtn7zero.data import BundleInformation, Node
 from dtn7zero.storage import Storage
 from dtn7zero.utility import get_oldest_bundle, get_oldest_bundle_id
 
 
 class SimpleInMemoryStorage(Storage):
 
@@ -22,28 +21,29 @@
 
     def get_nodes(self) -> Iterable[Node]:
         return self.nodes.values()
 
     def get_seen(self, bundle_id: str) -> Optional[str]:
         return self.bundle_ids.get(bundle_id)
 
+    def was_seen(self, bundle_id: str) -> bool:
+        return bundle_id in self.bundle_ids
+
     def store_seen(self, bundle_id: str, node_address):
         if node_address is None and self.bundle_ids.get(bundle_id, None) is not None:
             return  # we do not want to overwrite a valid node with None from an unknown source
 
         if len(self.bundle_ids) >= SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS:
             del self.bundle_ids[get_oldest_bundle_id(self.bundle_ids)]
         self.bundle_ids[bundle_id] = node_address
 
     def remove_bundle(self, bundle_id: str) -> bool:
         return self.bundles.pop(bundle_id, False)  # if the bundle exists it is 'truthy'
 
     def delay_bundle(self, bundle_information: BundleInformation) -> Tuple[bool, List[BundleInformation]]:
-        bundle_information.last_forwarding_attempt_ms = time.time_ns() // 1000000
-
         removed_bundles = []
 
         if bundle_information.bundle.bundle_id in self.bundles:
             return True, removed_bundles
 
         if len(self.bundles) >= SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES:
             self.garbage_collect()
@@ -60,10 +60,11 @@
 
     def garbage_collect(self):
         for bundle_id in list(self.bundles):
             if self.bundles[bundle_id].retention_constraint is None:
                 del self.bundles[bundle_id]
 
     def get_bundles_to_retry(self):
-        for bundle_id in list(self.bundles):
-            if time.time() - self.bundles[bundle_id].last_forwarding_attempt_ms > RETRY_INTERVAL_MILLISECONDS:
-                yield self.bundles[bundle_id]
+        # simply yield all stored bundles
+        # 1. reason: in-memory storage only stores a limited amount of bundles
+        # 2. router only forwards bundles where they have not been forwarded yet -> router filters
+        return (i for i in tuple(self.bundles.values()))
```

### Comparing `dtn7zero-0.0.2/dtn7zero.egg-info/PKG-INFO` & `dtn7zero-0.0.3/dtn7zero.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 Metadata-Version: 2.1
 Name: dtn7zero
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Lukas Holst <lh700@proton.me>
 License: AGPL-3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dtn7zero
-This is a DTN7 python implementation (work-in-progress) with [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API.
+This is a DTN7 [RFC9171](https://datatracker.ietf.org/doc/html/rfc9171) compliant python implementation (work-in-progress) with a [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API.
 
 The current features are:
-- a full bundle protocol agent (without fragment or CRC support)
+- a full bundle protocol agent (without fragment, CRC, and status-report generation support -> todo)
 - a minimal TCP convergence layer
-- a [dtn7rs](https://github.com/dtn7/dtn7-rs) REST convergence layer
-- an ipnd module
-- a standalone 'external' endpoint (which connects to a [dtn7rs](https://github.com/dtn7/dtn7-rs))
+- a [dtn7-rs](https://github.com/dtn7/dtn7-rs) convergence layer, using the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md) interface
+- automatic local-network node-discovery via ipnd module
+- a standalone 'external' endpoint (which connects to a [dtn7-rs](https://github.com/dtn7/dtn7-rs) via the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md)) interface
 - a simplified [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API to easily get started
 - full MicroPython support (tested on an ESP32-GENERIC)
 - (currently uses epidemic routing and in-memory storage managing)
 - (with extendability for new convergence layer adapters, routing algorithms, and storage managers)
 
 ## Getting Started
-To use dtn7zero in your CPython environment, simply install it via pip (or pip3 on linux): \
-(currently the package is only available on the test instance)
+To use dtn7zero in your CPython environment, simply install it via pip (or pip3 on linux):
 ```shell
 $ pip install --upgrade dtn7zero
 ```
 The most simple example on what you can do:
 ```python
+import time
+
 from dtn7zero import setup, start_background_update_thread
 
 node_endpoint = setup("dtn://node1/", print)
 
 start_background_update_thread()
 
 node_endpoint.send(b'hello world', "dtn://node1/")
+
+time.sleep(1)
 ```
 Further examples for the 'simple' API can be found under `./examples` in the GitHub repository.
 
 For a deeper dive into the underlying concepts and the fully fletched dtn implementation, take a look at the 
 `dtn7zero.api` module implementation and the tests under `./tests`.
 
 ## MicroPython Installation Guide
@@ -82,15 +85,39 @@
 1. check your connection to the ESP32 with: `mpremote`
 2. deploy the changes of dtn7zero and dependencies onto the ESP32 (this can take a while): `python scripts/esp-deployment.py`
 3. done
 
 ### First dtn7zero Functionality Check On MicroPython
 1. you may check that wlan is connecting correctly (connect via `mpremote` and press **enable** for a soft reset)
 2. you may also check that you can import dtn7zero (connect via `mpremote` and `import dtn7zero`)
-3. you can also check that everything works (run the test script `mpremote run scripts/test-bundle-protocol-agent.py`)
+3. you can also check that everything works (run the test script `mpremote run examples/local_ping_echo.py`)
+
+### Additional MicroPython Tips & Tricks
+The mpremote tool is normally interrupted by using `ctrl+c`. A special case is the REPL (simply call `mpremote`), which
+can be exited by using `ctrl+~` (tested on windows).
+
+If you start a script on MicroPython (`mpremote run ...`) and disconnect the console (`mpremote` -> `ctrl+c`) then the script 
+keeps running.
+
+If you must access the REPL via mpremote, but a script is blocking, then call `mpremote` and press EN (enable) on the 
+ESP32 for a soft-reset. Press `ctrl+c` a few times to interrupt the `boot.py` or `main.py` script execution. The session
+state is stored, so any subsequent `mpremote` call will start at REPL as long as no power disconnect is performed.
+
+You can deploy a script as `main.py` on MicroPython to be run every time the microcontroller gets power. \
+You can also remove the script. MicroPython will only execute the script if it is present.
+```shell
+$ mpremote fs cp examples/remote_echo_callback.py :main.py
+$ mpremote fs rm :main.py
+```
+
+Regarding `boot.py`, it is used for user-specific setup code and this framework uses a generic boot script that adjusts
+the ESP32's frequency and connects to a Wi-Fi network (blocking until success). MicroPython will create a dummy `boot.py`
+if none is present. MicroPython will not create a dummy `main.py` is none is present. MicroPython will first execute
+the `boot.py` and then the `main.py` if it is present.
+
 
 ## Development Information
 
 ### Development Mode
 You can install this project locally to directly reflect code changes in your environment.
 Simply run this in the project root folder (requires at least pip v21.1):
 ```shell
@@ -147,12 +174,11 @@
    - non-official, but tested micropython [library](https://github.com/glenn20/micropython/blob/espnow-g20/docs/library/espnow.rst) available, as well as [builds](https://github.com/glenn20/micropython-espnow-images) with the current firmware
 
 3. Alternative: AP_STA mode for simultaneous AP and STA without explicit ESP-MESH usage
    - only available for [Arduino+C](https://techtutorialsx.com/2021/01/04/esp32-soft-ap-and-station-modes/)
    - [painlessMesh](https://gitlab.com/painlessMesh/painlessMesh) also uses this mode to build its mesh
 
 ### Open End Topics / Known Issues
-- interface between router and cla is inconsistent (different responsibilities for send and receive)
-- dtn7rs-rest-cla and in-memory storage together use too much RAM for MicroPython (therefore the rest-cla is disabled in the simple API)
-- additional group (for example: "dtn://group/~news") registration on singleton endpoints (can there be registrations from multiple local endpoints on the same group?)
+- fragment, CRC, status-report generation support
+- dtn7rs-rest-cla and in-memory storage together use too much RAM for MicroPython (therefore the dtn7rs-rest-cla is disabled in the simple API)
 - public repository
-- api documentation (currently all information must be gathered from doc-strings and examples)
+- public documentation (currently all information must be gathered from doc-strings and examples)
```

### Comparing `dtn7zero-0.0.2/dtn7zero.egg-info/SOURCES.txt` & `dtn7zero-0.0.3/dtn7zero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/pyproject.toml` & `dtn7zero-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dtn7zero"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Lukas Holst", email = "lh700@proton.me"},
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "AGPL-3.0"}
```

### Comparing `dtn7zero-0.0.2/test/test-api-background.py` & `dtn7zero-0.0.3/test/test-api-background.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-api-ping.py` & `dtn7zero-0.0.3/test/test-api-ping.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-api-pong.py` & `dtn7zero-0.0.3/test/test-api-pong.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-api-synchronous.py` & `dtn7zero-0.0.3/test/test-api-synchronous.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-bundle-protocol-agent-receiver.py` & `dtn7zero-0.0.3/test/test-bundle-protocol-agent-receiver.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-bundle-protocol-agent-sender.py` & `dtn7zero-0.0.3/test/test-bundle-protocol-agent-sender.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-bundle-protocol-agent.py` & `dtn7zero-0.0.3/test/test-bundle-protocol-agent.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-bundle-serialization.py` & `dtn7zero-0.0.3/test/test-bundle-serialization.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-bundle-size.py` & `dtn7zero-0.0.3/test/test-bundle-size.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-dtn7rs-rest-cla.py` & `dtn7zero-0.0.3/test/test-dtn7rs-rest-cla.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-ipnd.py` & `dtn7zero-0.0.3/test/test-ipnd.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-mtcp-intermediate.py` & `dtn7zero-0.0.3/test/test-mtcp-intermediate.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-mtcp-receiver.py` & `dtn7zero-0.0.3/test/test-mtcp-receiver.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-mtcp-sender.py` & `dtn7zero-0.0.3/test/test-mtcp-sender.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.2/test/test-py-dtn7-functionality.py` & `dtn7zero-0.0.3/test/test-py-dtn7-functionality.py`

 * *Files identical despite different names*

