# Comparing `tmp/sqlalchemy-iris-0.6.0b2.tar.gz` & `tmp/sqlalchemy-iris-0.6.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-iris-0.6.0b2.tar", last modified: Thu Mar 23 13:54:51 2023, max compression
+gzip compressed data, was "sqlalchemy-iris-0.6.1b1.tar", last modified: Sun Apr 16 12:08:32 2023, max compression
```

## Comparing `sqlalchemy-iris-0.6.0b2.tar` & `sqlalchemy-iris-0.6.1b1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:54:51.019209 sqlalchemy-iris-0.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-23 13:54:23.000000 sqlalchemy-iris-0.6.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-03-23 13:54:51.019209 sqlalchemy-iris-0.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-23 13:54:23.000000 sqlalchemy-iris-0.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:54:51.007208 sqlalchemy-iris-0.6.0b2/intersystems_iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_BufferReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_BufferWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_ConnectionInformation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_ConnectionParameters.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_Constant.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    20005 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_DBList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_Device.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_GatewayContext.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_GatewayException.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_GatewayUtility.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRIS.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISConnection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISEmbedded.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISGlobalNode.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISGlobalNodeView.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISOREF.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISObject.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISReference.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_InStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_LegacyIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_ListItem.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_ListReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_ListWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_LogFileStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_MessageHeader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_OutStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_PrintStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_PythonGateway.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/_SharedMemorySocket.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:54:51.011209 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_Column.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    94603 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_DBAPI.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_Descriptor.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_IRISStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_Parameter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_ParameterCollection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12186 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_ResultSetRow.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_SQLType.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:54:51.011209 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/preparser/
--rw-rw-rw-   0 runner    (1001) docker     (123)    78424 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/preparser/_PreParser.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/preparser/_Scanner.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/preparser/_Token.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/preparser/_TokenList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/preparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:54:51.015209 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_BusinessHost.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_BusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_BusinessProcess.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_BusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_Common.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_Director.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_IRISBusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_IRISBusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_IRISInboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_IRISOutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_InboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_OutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:54:51.015209 sqlalchemy-iris-0.6.0b2/iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      922 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/iris/iris_site.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/iris/irisbuiltins.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/iris/irisloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:54:51.015209 sqlalchemy-iris-0.6.0b2/irisnative/
--rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/irisnative/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-03-23 13:54:45.000000 sqlalchemy-iris-0.6.0b2/irisnative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-23 13:54:51.019209 sqlalchemy-iris-0.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-23 13:54:23.000000 sqlalchemy-iris-0.6.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:54:51.019209 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-23 13:54:23.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40356 2023-03-23 13:54:23.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-23 13:54:23.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-03-23 13:54:23.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/information_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-23 13:54:23.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-23 13:54:23.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/provision.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-03-23 13:54:23.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-03-23 13:54:23.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:54:51.019209 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-03-23 13:54:50.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-03-23 13:54:50.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 13:54:50.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-23 13:54:50.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 13:54:50.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-23 13:54:50.000000 sqlalchemy-iris-0.6.0b2/sqlalchemy_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:54:51.019209 sqlalchemy-iris-0.6.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-03-23 13:54:23.000000 sqlalchemy-iris-0.6.0b2/tests/test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:08:32.953198 sqlalchemy-iris-0.6.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-16 12:08:10.000000 sqlalchemy-iris-0.6.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-16 12:08:32.953198 sqlalchemy-iris-0.6.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-16 12:08:10.000000 sqlalchemy-iris-0.6.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:08:32.945198 sqlalchemy-iris-0.6.1b1/intersystems_iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_BufferReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_BufferWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_ConnectionInformation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_ConnectionParameters.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_Constant.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    20104 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_DBList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_Device.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_GatewayContext.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_GatewayException.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_GatewayUtility.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRIS.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISConnection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISEmbedded.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISGlobalNode.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISGlobalNodeView.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISOREF.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISObject.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISReference.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_InStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_LegacyIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_ListItem.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_ListReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_ListWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_LogFileStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_MessageHeader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_OutStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_PrintStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_PythonGateway.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/_SharedMemorySocket.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:08:32.949198 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_Column.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    95424 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_DBAPI.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_Descriptor.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_IRISStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_Parameter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_ParameterCollection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12810 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_ResultSetRow.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_SQLType.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:08:32.949198 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/preparser/
+-rw-rw-rw-   0 runner    (1001) docker     (123)    78828 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/preparser/_PreParser.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/preparser/_Scanner.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/preparser/_Token.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/preparser/_TokenList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/preparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:08:32.949198 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_BusinessHost.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_BusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_BusinessProcess.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_BusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_Common.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_Director.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_IRISBusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_IRISBusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_IRISInboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_IRISOutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_InboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_OutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:08:32.949198 sqlalchemy-iris-0.6.1b1/iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      922 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/iris/iris_site.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/iris/irisbuiltins.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/iris/irisloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:08:32.953198 sqlalchemy-iris-0.6.1b1/irisnative/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/irisnative/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-04-16 12:08:28.000000 sqlalchemy-iris-0.6.1b1/irisnative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-16 12:08:32.953198 sqlalchemy-iris-0.6.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-16 12:08:10.000000 sqlalchemy-iris-0.6.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:08:32.953198 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-16 12:08:10.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40355 2023-04-16 12:08:10.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-16 12:08:10.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-16 12:08:10.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/information_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-16 12:08:10.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-16 12:08:10.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/provision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-16 12:08:10.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-16 12:08:10.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:08:32.953198 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-16 12:08:32.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-16 12:08:32.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 12:08:32.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-16 12:08:32.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-16 12:08:32.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-16 12:08:32.000000 sqlalchemy-iris-0.6.1b1/sqlalchemy_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:08:32.953198 sqlalchemy-iris-0.6.1b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-16 12:08:10.000000 sqlalchemy-iris-0.6.1b1/tests/test_suite.py
```

### Comparing `sqlalchemy-iris-0.6.0b2/LICENSE` & `sqlalchemy-iris-0.6.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/PKG-INFO` & `sqlalchemy-iris-0.6.1b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-iris
-Version: 0.6.0b2
+Version: 0.6.1b1
 Summary: InterSystems IRIS for SQLAlchemy
 Home-page: https://github.com/caretdev/sqlalchemy-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/sqlalchemy-iris
 Project-URL: Tracker, https://github.com/caretdev/sqlalchemy-iris/issues
```

### Comparing `sqlalchemy-iris-0.6.0b2/README.md` & `sqlalchemy-iris-0.6.1b1/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_BufferWriter.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_BufferWriter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_ConnectionInformation.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_ConnectionInformation.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_ConnectionParameters.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_ConnectionParameters.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_Constant.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_Constant.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_DBList.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_DBList.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,16 @@
     def _grab_oref_unicode(cls, buffer, offset, length, *args):
         return intersystems_iris._IRISOREF._IRISOREF(cls._grab_unicode_string(buffer, offset, length))
 
     @classmethod
     def _set(cls, buffer, offset, data, locale, is_unicode, compact_double):
         func = cls._set_switcher.get(type(data), None)
         if func is None:
-            raise Exception("Unsupported argument type: " + str(type(data)))
+            # raise Exception("Unsupported argument type: " + str(type(data)))
+            return cls._stuff_str(buffer, offset, str(data), locale, is_unicode, compact_double)
         else:
             return func(buffer, offset, data, locale, is_unicode, compact_double)
 
     @classmethod
     def _set_undefined(cls, buffer, offset):
         buffer[offset] = 1
         return offset + 1
```

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_Device.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_Device.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_GatewayContext.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_GatewayContext.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_GatewayUtility.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_GatewayUtility.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRIS.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRIS.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISConnection.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISConnection.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISEmbedded.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISEmbedded.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISGlobalNode.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISGlobalNode.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISGlobalNodeView.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISGlobalNodeView.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISIterator.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISIterator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISList.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISList.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISNative.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISObject.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISObject.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_IRISReference.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_IRISReference.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_InStream.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_InStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_LegacyIterator.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_LegacyIterator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_ListReader.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_ListReader.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_ListWriter.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_ListWriter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_LogFileStream.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_LogFileStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_MessageHeader.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_MessageHeader.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_OutStream.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_OutStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_PrintStream.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_PrintStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_PythonGateway.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_PythonGateway.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/_SharedMemorySocket.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/_SharedMemorySocket.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/__init__.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_Column.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_Column.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_DBAPI.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_DBAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from . import _Message
 import intersystems_iris.dbapi._Parameter
 import intersystems_iris.dbapi._Column
 from ._ResultSetRow import _ResultSetRow
 import intersystems_iris.dbapi._ParameterCollection
 import intersystems_iris.dbapi.preparser._PreParser
 from intersystems_iris.dbapi._Parameter import ParameterMode
-from intersystems_iris.dbapi.preparser._PreParser import StatementType
+from intersystems_iris.dbapi.preparser._PreParser import StatementType, MultiValuesInsert
 from intersystems_iris._IRISConnection import Feature
 from intersystems_iris._InStream import _InStream
 from intersystems_iris.dbapi._IRISStream import (IRISStream, IRISBinaryStream, )
 from ._SQLType import SQLType
 
 from .._IRISNative import connect as native_connect
 from .._IRISEmbedded import _IRISEmbedded
@@ -28,19 +28,21 @@
 
 def embedded_connect(*args, hostname = None, port = None,  namespace = None, username = None, password = None, **kw):
     connection = _IRISEmbedded()
     connection.connect(hostname, port,  namespace, username, password, **kw)
     return connection
 
 def connect(*args, embedded=False, hostname = None, port = None,  namespace = None, username = None, password = None, **kw):
-    if not embedded:
-        return native_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
-    else:
-        return embedded_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
-
+    try:
+        if not embedded:
+            return native_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
+        else:
+            return embedded_connect(*args, hostname=hostname, port=port, namespace=namespace, username=username, password=password, **kw)
+    except Exception as e:
+        raise DatabaseError(e)
 
 class ServerReturnType(enum.IntEnum):
     NO_RETURN_VALUE = 0
     IGNORE_RETURN_VALUE = 1
     HAS_RETURN_VALUE = 2
     NULL_RETURN_VALUE = 3
 
@@ -56,14 +58,17 @@
 paramstyle = "qmark"
 
 class _BaseCursor:
     embedded = False
     def __init__(self, connection):
         self._connection = connection
         
+        self.statement = None
+        self._parsed_statement = None
+        
         self._columns = None
         self._rowcount = -1
         self.arraysize = 1
 
         self._result_set = None
 
         self._rsrow = None
@@ -184,15 +189,23 @@
         self._rowcount = -1
         self._exec_params = None
         self._statementType = StatementType.UPDATE
         self.statementFeatureOption = 0
         self.maxRowItemCount = 0
         self._is_batch_update = False
 
+    def _is_alive(self):
+        if self._closed:
+            raise InterfaceError("Cursor is closed")
+        if self._connection == None or self._connection.isClosed():
+            raise InterfaceError("Connection not open")
+
     def direct_execute(self, operation, *params):
+        self._is_alive()
+
         self.statement = operation
         if len(params) == 1 and (isinstance(params[0], tuple) or isinstance(params[0], list)):
             self.params = params[0]
         else:
             self.params = params
         self._params.set_input_params(self.params)
 
@@ -200,35 +213,45 @@
         self._cleanup()
         self._preparse()
 
         self._execute()
         return self._rowcount
 
     def execute(self, operation, params=()):
+        self._is_alive()
+
         self.statement = operation
         if params and not isinstance(params, list) and not isinstance(params, tuple):
             params = (params, )
         self.params = params if params is not None else ()
         self._params.set_input_params(self.params)
 
         self._cleanup()
-        self._preparse()
+        try:
+            self._preparse()
+        except MultiValuesInsert as ex:
+            # convert to executemany
+            params = params or ex.params
+            params_count = int(len(params) / ex.rows)
+            new_params = [params[i:i + params_count] for i in range(0, len(params), params_count)]
+            return self.executemany(ex.query, new_params)
+        except Exception:
+            raise
 
         if self._statementType == StatementType.UPDATE:
             self._cursor_type = CursorType.PREPARED
             self._prepare()
         else:
             self._cursor_type = CursorType.DEFAULT
 
         self._execute()
         return self._rowcount
 
     def add_batch(self):
-        if self._closed:
-            raise InterfaceError("Cursor is closed")
+        self._is_alive()
         
         if self._params._array_bound:
             if len(self._params._params_list) > 0:
                 cnt = 0
                 first = True
                 for i in range(self._params._user_parameters_size):
                     i = i + 1
@@ -249,19 +272,19 @@
                 if len(param._values) != self._parameter_sets:
                     if self._parameter_sets != 1:
                         if len(param._values) + 1 == self._parameter_sets:
                             param._values.append(param._values[len(param._values) - 1])
                             continue
 
     def executemany(self, operation, seq_of_params):
+        self._is_alive()
         self._rowcount = 0
-        if self._closed:
-            raise InterfaceError("Cursor is closed")
-        if self._connection == None or self._connection.isClosed():
-            raise InterfaceError("Connection not open")
+
+        if not isinstance(seq_of_params, tuple) and not isinstance(seq_of_params, list):
+            seq_of_params = tuple(seq_of_params)
 
         self.statement = operation
         self.params = seq_of_params
         self._params.set_input_params(self.params)
 
         self._cursor_type = CursorType.PREPARED
         self._cleanup()
@@ -285,14 +308,22 @@
             if mode == ParameterMode.INPUT_OUTPUT or mode == ParameterMode.OUTPUT:
                 raise ValueError("INOUT/OUT parameters not permitted")
 
         self._prepared_update_execute()
 
         return self._rowcount
 
+    def _process_sqlcode(self, sqlcode, message=None):
+        self._sqlcode = sqlcode
+        if sqlcode in [0, 100]:
+            return
+        if abs(sqlcode) in [108, 119, 121, 122]:
+            raise IntegrityError(message)
+        raise DatabaseError(message)
+
     def _preparse(self):
         csql = self._connection._pre_preparse_cache.get(self.statement)
         if csql != None:
             self._has_return_value = csql._has_return_value
             self._params = copy.deepcopy(csql._params)
             self._params.set_input_params(self.params)
             self._parsed_statement = csql._parsed_statement
@@ -305,25 +336,28 @@
             if isinstance(item, list) or isinstance(item, tuple):
                 if not self._is_batch_update:
                     raise TypeError("Unsupported argument type: " + str(type(item)))
                 for ele in item:
                     if intersystems_iris._DBList._DBList._set_switcher.get(type(ele), None) == None:
                         raise TypeError("Unsupported argument type: " + str(type(ele)))
             elif intersystems_iris._DBList._DBList._set_switcher.get(type(item), None) is None:
-                raise TypeError("Unsupported argument type: " + str(type(item)))
+                item = str(item)
+                # raise TypeError("Unsupported argument type: " + str(type(item)))
             if i == 0:
                 count = len(item) if isinstance(item, list) or isinstance(item, tuple) else 1
             else:
                 curr_count = len(item) if isinstance(item, list) or isinstance(item, tuple) else 1
                 if count != curr_count:
                     raise Exception("Parameter count does not match")
 
         parser = intersystems_iris.dbapi.preparser._PreParser._PreParser(self._connection._connection_info._delimited_ids, embedded=self.embedded)
         try:
             pOut = parser.PreParse(self.statement, self._params)
+        except MultiValuesInsert:
+            raise
         except Exception as e:
             raise InterfaceError("Error parsing statement '" + self.statement + "':\n" + str(e))
 
         if len(self.params) > 0:
             item = self.params[0]
             if (isinstance(item, list) or isinstance(item, tuple)) and not self._is_batch_update:
                 raise TypeError("Unsupported argument type: " + str(type(item)))
@@ -364,15 +398,15 @@
                 elif item == '?':
                     unknown_count = unknown_count + 1
 
             if len(self.params) > 0:
                 item = self.params[0]
                 param_count = len(item) if isinstance(item, list) or isinstance(item, tuple) else len(self.params)
                 if param_count != unknown_count:
-                    raise Exception("Parameter mismatch")
+                    raise Exception(f"Parameter mismatch: {param_count}/{unknown_count}")
         else:
             if self._cursor_type == CursorType.CALLABLE:
                 i = 0
                 for param in self._params._params_list:
                     if param.mode == ParameterMode.RETURN_VALUE:
                         continue
                     else:
@@ -395,15 +429,15 @@
                 for item in temp_list_data:
                     if item == 'c':
                         replaced_count = replaced_count + 1
                     elif item == '?':
                         unknown_count = unknown_count + 1
 
                 if unknown_count != len(self.params):
-                    raise Exception("Incorrect number of parameters")
+                    raise Exception(f"Incorrect number of parameters: {unknown_count}/{replaced_count}/{len(self.params)}")
 
     def _is_not_default_or_replaced(self, param):
         mode = param.mode
         if mode != ParameterMode.REPLACED_LITERAL and mode != ParameterMode.DEFAULT_PARAMETER and mode != ParameterMode.INPUT:
             raise Exception("Parameters not allowed in Cursor class")
 
     def _validate_parameters(self):
@@ -433,14 +467,15 @@
             raise InterfaceError("Cursor is closed")
         if self._connection == None or self._connection.isClosed():
             raise InterfaceError("Connection not open")
 
         exec_switcher = {
             StatementType.QUERY: self._execute_query,
             StatementType.CALL: self._execute_update,
+            StatementType.STMT_USE: self._execute_update,
             StatementType.UPDATE: self._execute_update,
             StatementType.DDL_OTHER: self._execute_update,
             StatementType.DDL_ALTER_DROP: self._execute_update
         }
         exec_func = exec_switcher.get(self._statementType, None)
         if exec_func is None:
             raise NotImplementedErrorDBAPI(f'StatementType {self._statementType.name} not implemented')
@@ -643,14 +678,19 @@
         self._fetch_done = False
         self._output_parameter_list = None
 
         self._lastrowid = None
 
         self._closed = False
 
+    def _process_sqlcode(self, sqlcode, message=None):
+        if sqlcode in [0, 100]:
+            return
+        super()._process_sqlcode(sqlcode, self._get_error_info(sqlcode))
+
     def _get_cached_info(self):
         if not self._connection._preparedCache or not hasattr(self._connection._preparedCache, '__iter__'):
             return False
         if self._parsed_statement in self._connection._preparedCache:
             self._prepare_cached(self._connection._preparedCache[self._parsed_statement])
             return True
         else:
@@ -730,15 +770,15 @@
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [0])
             sqlcode = self._in_message.wire.header._get_function_code()
             if sqlcode not in [0, 100]:
-                raise InterfaceError(self._get_error_info(sqlcode))
+                raise DatabaseError(self._get_error_info(sqlcode))
 
         # process metadata
         try:
             if self._connection._isFastOption():
                 self._check_statement_feature(self._in_message.wire)
             else:
                 self.statementFeatureOption = Feature.optionNone
@@ -910,16 +950,15 @@
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, _InStream.FETCH_DATA, [404, 100])
             self._sqlcode = self._in_message.wire.header._get_function_code()
             self._handle_error_504(self._sqlcode)
             if self._sqlcode == 404:
                 return
-            if self._sqlcode not in [0, 100]:
-                raise InterfaceError(self._get_error_info(self._sqlcode))
+            self._process_sqlcode(self._sqlcode)
 
         self._current_wire = self._in_message.wire
         self._result_set = [self._current_wire]
         self._rs_index = 0
         
         self._rowcount = -1
 
@@ -944,15 +983,15 @@
             self._out_message._send(sequence_number)
 
             try:
                 # retrieve metadata
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 sqlcode = self._in_message.wire.header._get_function_code()
                 if sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(sqlcode))
+                    raise DatabaseError(self._get_error_info(sqlcode))
 
                 self._process_stored_procedure_metadata(self._in_message.wire, True)
                 if self._multiple_result_sets:
                     # todo
                     return
 
                 self._cache_prepared_statement()
@@ -993,30 +1032,29 @@
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             try:
                 # retrieve metadata
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 sqlcode = self._in_message.wire.header._get_function_code()
-                if sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(sqlcode))
+                self._process_sqlcode(sqlcode)
 
                 if self._connection._isFastOption():
                     self._check_statement_feature(self._in_message.wire)
                 else:
                     self.statementFeatureOption = Feature.optionNone
                 self._get_column_info(self._in_message.wire)
                 self._get_parameter_info(self._in_message.wire)
                 self._cache_prepared_statement()
 
                 # retrieve data
                 self._in_message._read_message_sql(sequence_number, self._statement_id, _InStream.FETCH_DATA, [100])
                 self._sqlcode = self._in_message.wire.header._get_function_code()
                 if self._sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(self._sqlcode))
+                    raise DatabaseError(self._get_error_info(self._sqlcode))
 
             except IndexError:
                 raise DatabaseError("Server response message terminated prematurely")
             except TypeError:
                 raise DatabaseError("Unexpected server response message format")
 
         self._current_wire = self._in_message.wire
@@ -1044,22 +1082,19 @@
 
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [404, 100])
-            sqlcode = self._in_message.wire.header._get_function_code()
-            if sqlcode == 404:
+            self._sqlcode = self._in_message.wire.header._get_function_code()
+            if self._sqlcode == 404:
                 self._update404()
                 return
-            if sqlcode == 119:
-                raise IntegrityError(self._get_error_info(sqlcode))
-            if sqlcode not in [0, 100]:
-                raise InterfaceError(self._get_error_info(sqlcode))
+            self._process_sqlcode(self._sqlcode)
 
     def _send_direct_update_request(self):
         # send DU message
         with self._connection._lock:
             self._statement_id = self._connection._get_new_statement_id()
             # message header
             self._out_message.wire._write_header(_Message.DIRECT_UPDATE)
@@ -1078,16 +1113,15 @@
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             try:
                 # retrieve response
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 self._sqlcode = self._in_message.wire.header._get_function_code()
-                if self._sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(self._sqlcode))
+                self._process_sqlcode(self._sqlcode)
 
                 addToCache = self._get_parameter_info(self._in_message.wire)
                 
                 notDDL = bool(self._statementType != StatementType.DDL_ALTER_DROP 
                                   and self._statementType != StatementType.DDL_OTHER)
                 if notDDL and addToCache:
                     self._cache_prepared_statement()
@@ -1110,17 +1144,16 @@
             
             # send message
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [0])
-            self._sqlcode = self._in_message.wire.header._get_function_code()
-            if self._sqlcode not in [0, 100]:
-                raise InterfaceError(self._get_error_info(self._sqlcode))
+            sqlcode = self._in_message.wire.header._get_function_code()
+            self._process_sqlcode(sqlcode)
 
             self._process_stored_procedure_metadata(self._in_message.wire, False)
             if self._multiple_result_sets:
                 return
         self._cache_prepared_statement()
         return
 
@@ -1276,16 +1309,15 @@
             # send
             sequence_number = self._connection._get_new_sequence_number()
             self._out_message._send(sequence_number)
 
             # retrieve response
             self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [404, 100])
             self._sqlcode = self._in_message.wire.header._get_function_code()
-            if self._sqlcode not in [0, 100,]:
-                raise InterfaceError(self._get_error_info(self._sqlcode))
+            self._process_sqlcode(self._sqlcode)
             if self._sqlcode == 404:
                 self._update404(404)
             else:
                 self._get_output_parameters(self._in_message.wire)
         return
 
     def _stored_procedure_query(self):
@@ -1315,14 +1347,15 @@
                 return
             elif self._sqlcode == 100:
                 self._handle_error_100(100)
                 return
             self._get_output_parameters(self._in_message.wire)
             self._in_message._read_message_sql(sequence_number, self._statement_id, _InStream.FETCH_DATA, [100])
             self._sqlcode = self._in_message.wire.header._get_function_code()
+            self._process_sqlcode(self._sqlcode)
             if self._sqlcode == 100:
                 self._handle_error_100(100)
 
             self._current_wire = self._in_message.wire
             self._result_set = [self._current_wire]
             self._rs_index = 0
 
@@ -1619,15 +1652,15 @@
         # with self._connection._lock:
         #     self._out_message.wire._write_header(_Message.GET_AUTO_GENERATED_KEYS)
         #     sequence_number = self._connection._get_new_sequence_number()
         #     self._out_message._send(sequence_number)
         #     self._in_message._read_message_sql(sequence_number)
         #     self._sqlcode = self._in_message.wire.header._get_function_code()
         #     if self._sqlcode != 100:
-        #         raise InterfaceError(self._get_error_info(self._sqlcode))
+        #         raise DatabaseError(self._get_error_info(self._sqlcode))
         #     self._get_column_info(self._in_message.wire)
         #     self._lastrowid = self._in_message.wire._get()
 
         self.execute('SELECT LAST_IDENTITY()')
         self._lastrowid = self.fetchone()[0]
         return self._lastrowid
 
@@ -1778,16 +1811,15 @@
                 intersystems_iris._MessageHeader._MessageHeader._set_statement_id(self._out_message.wire.buffer, self._statement_id)
 
                 sequence_number = self._connection._get_new_sequence_number()
                 self._out_message._send(sequence_number)
 
                 self._in_message._read_message_sql(sequence_number, self._statement_id, 0, [100])
                 self._sqlcode = self._in_message.wire.header._get_function_code()
-                if self._sqlcode not in [0, 100]:
-                    raise InterfaceError(self._get_error_info(self._sqlcode))                
+                self._process_sqlcode(self._sqlcode)
             self._result_set.append(self._in_message.wire)
 
         if self._sqlcode == 404:
             self._query404()
             return
 
         if self._rs_index + 1 == len(self._result_set):
@@ -1892,23 +1924,24 @@
                 self._scroll_flag = False
             else:
                 if self.fetchone_helper():
                     retval = self._rsrow._offsets
 
         if retval is None:
             return retval
-        return retval[:]
+        return retval.as_tuple()
+        # return tuple(retval[:])
 
     def fetchmany(self, size = None):
         if self._result_set == None:
             raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
 
         if self._current_wire == None:
             if self._cursor_ptr > self._last_row_in_warehouse_dict:
-                return None
+                return []
             if size is None:
                 size = self.arraysize
             if self._rs_index == 0:
                 if self._cursor_ptr < len(self._warehouse):
                     rows = []
                     for i in range(size):
                         row = self._warehouse[self._cursor_ptr]
@@ -1933,24 +1966,24 @@
             size = self.arraysize
 
         rows = []
         for i in range(size):
             row = self.fetchone()
             if row is None:
                 break
-            rows.append(row[:])
+            rows.append(row)
         return rows
 
     def fetchall(self):
         if self._result_set == None:
             raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
         
         if self._current_wire == None:
             if self._cursor_ptr > self._last_row_in_warehouse_dict:
-                return None
+                return []
             if self._rs_index == 0:
                 if self._cursor_ptr < len(self._warehouse):
                     rows = []
                     while 1:
                         row = self._warehouse[self._cursor_ptr]
                         rows.append(row[:])
                         if self._cursor_ptr + 1 >= len(self._warehouse):
@@ -1969,15 +2002,16 @@
                     self._cursor_ptr += 1
                 return rows
         
         rows = []
         while self._current_wire is not None:
             row = self.fetchone()
             if not row: break
-            rows.append(row[:])
+            rows.append(row)
+        
         return rows
 
 class EmbdeddedCursor(_BaseCursor):
     embedded = True
     _result_set = None
 
     def __init__(self, connection: _IRISEmbedded) -> None:
@@ -2040,20 +2074,14 @@
                 _column_info.isHidden,
                 _column_info.isIdentity,
                 _column_info.isKeyColumn,
                 _column_info.isRowId,
             ]
             self._columns.append(intersystems_iris.dbapi._Column._Column(name, odbctype, precision, scale, nullable, label, tableName, schema, catalog, additionalData, slotPosition))
 
-    def _process_sqlcode(self, sqlcode, message):
-        if sqlcode == -119:
-            raise IntegrityError(message)
-        if sqlcode not in [0, 100]:
-            raise InterfaceError(message)
-
     @property
     def lastrowid(self):
         return self._lastrowid
 
     def _prepare_new(self):
         statement = self._parsed_statement
         sqlcode = 0
@@ -2157,33 +2185,34 @@
         return self._rowcount
         
     def fetchone(self):
         if self._result_set == None:
             raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
         
         try:
-            row = self._result_set.__next__()
+            values = self._result_set.__next__()
         except:
             return None
 
-        row = [None if v == '' else '' if v == '\x00' else v for v in row]
+        values = [None if v == '' else '' if v == '\x00' else v for v in values]
+        row = namedtuple('Row', [col.name for col in self._columns], rename=True)
 
         _types = {
             SQLType.BIGINT: int,
             SQLType.BINARY: bytes,
             SQLType.BIT: bool,
             SQLType.INTEGER: int,
             SQLType.VARCHAR: str,
             SQLType.LONGVARBINARY: IRISBinaryStream,
             SQLType.LONGVARCHAR: IRISStream,
         }
         
         if self._columns:
             for _column in self._columns:
-                value = row[_column.slotPosition - 1]
+                value = values[_column.slotPosition - 1]
 
                 ctype = _column.type
                 value_type = _types[ctype] if ctype in _types else None
                 try:
                     if type(value) == float:
                         value = decimal.Decimal(str(value))
                     elif not _column.tableName and not _column.schema:
@@ -2194,16 +2223,16 @@
                         stream = value_type(self._connection, value, embedded=True)
                         value = stream.fetch()
                     elif not isinstance(value, value_type):
                         value = value_type(value)
                 except Exception as ex:
                     raise ex
                     pass
-                row[_column.slotPosition - 1] = value
-        return row
+                values[_column.slotPosition - 1] = value
+        return row(*values)
 
     def fetchall(self):
         if self._result_set == None:
             raise InterfaceError("Either execute has not yet been called, or the previous call of execute did not return a result set")
 
         rows = []
         while True:
```

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_Descriptor.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_Descriptor.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_IRISStream.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_IRISStream.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_Message.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_Message.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_Parameter.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_Parameter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_ParameterCollection.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_ParameterCollection.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_ResultSetRow.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_ResultSetRow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,27 @@
+from datetime import datetime
+from collections import namedtuple
 from ._SQLType import SQLType
 from .._DBList import _DBList
 from .._ListItem import _ListItem
 from ._IRISStream import IRISStream, IRISBinaryStream
 from ._Column import _Column
 
+def from_timestamp_posix(posix):
+    time = int(posix)
+    if time > 0:
+        time ^= 0x1000000000000000 
+    else:
+        time |= 0xF000000000000000 
+
+    time /= 1000000
+
+    value = datetime.utcfromtimestamp(time).replace(tzinfo=None)
+    return value
+
 class _ResultSetRow:
     _locale = "latin-1"
     _connection = None
 
     def __init__(self, connection, columns=None, rowcount=0, ):
         self._connection = connection
         # index from user-inputted columns to columns received from server
@@ -105,14 +119,19 @@
             self._locale = rsrow._locale
 
         def __getattr__(self, key):
             return self.__getitem__(key)
 
         def get(self):
             return self[:]
+        
+        def as_tuple(self):
+            row = namedtuple('Row', [col.name for col in self._columns], rename=True)
+            values = self[:]
+            return row(*values)
 
         def __getitem__(self, key):
             if isinstance(key, str):
                 key = key.lower()
                 if key not in self._name_dict_keys:
                     raise KeyError("Column '" + key + "' does not exist")
                 return self[self._name_dict[key][0] + 1]
@@ -134,14 +153,17 @@
                 self._list_item.next_offset = self._offsets[key]
                 _DBList._get_list_element(self._list_item)
                 item = _DBList._get(self._list_item, self._locale)
                 _column: _Column = self._columns[idx]
                 ctype = _column.type
                 value_type = self._types[ctype] if ctype in self._types else None
                 try:
+                    if ctype == SQLType.TIMESTAMP_POSIX:
+                        item = from_timestamp_posix(item)
+
                     if _column.tableName == 'None' and _column.schema == 'None':
                         # Ignore for anonymous tables
                         pass
                     elif item is None:
                         pass
                     elif issubclass(value_type, IRISStream):
                         stream = value_type(self._connection, item)
```

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/_SQLType.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/_SQLType.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/preparser/_PreParser.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/preparser/_PreParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,29 @@
+import re
 import functools
 import enum
 import intersystems_iris._IRISList
 import intersystems_iris.dbapi._DBAPI
 import intersystems_iris.dbapi._Parameter
 import intersystems_iris.dbapi.preparser._Token
 import intersystems_iris.dbapi.preparser._TokenList
 import intersystems_iris.dbapi.preparser._Scanner
 from intersystems_iris.dbapi._Parameter import ParameterMode
 from intersystems_iris.dbapi.preparser._Token import TOKEN
 from intersystems_iris.dbapi.preparser._Scanner import ParseToken
 
+class MultiValuesInsert(Exception):
+
+    def __init__(self, *args: object, query: str, rows: int, params=None) -> None:
+        super().__init__(*args)
+        self.query = query
+        self.rows = rows
+        self.params = params
+    
+
 # May want to move to its own file eventually
 # SQL Statement Types
 class StatementType(enum.IntEnum):
     UPDATE = 0
     QUERY = 1
     CALL = 2
     SYNC_COMMIT = 3
@@ -539,56 +549,56 @@
             new_query += _query(False)
             
             return found, new_query
         except:
             return False, query
         
     def InsertMultiValues(self, query):
-        try:
-            new_query = ''
-            values_list = []
-
-            tokens = self.m_Tokens.GetEnumerator()
-            while tokens.MoveNext() and not tokens.Current().UpperEquals("INSERT"):
-                new_query += tokens.Current().Lexeme + ' '
-            if not tokens.MoveNext() or not tokens.Current().UpperEquals("INTO"):
-                return False, query
-            new_query += 'INSERT INTO '
-            while tokens.MoveNext() and not tokens.Current().UpperEquals("VALUES"):
-                new_query += tokens.Current().Lexeme + ' '
+        new_query = ''
+        values_list = []
 
-            values = ''
-            while tokens.MoveNext():
-                assert tokens.Current().TokenType is TOKEN.OPEN_PAREN
-                open_parens = 1
-                while tokens.MoveNext() or open_parens > 0:
-                    token = tokens.Current()
-                    if token.TokenType is TOKEN.OPEN_PAREN:
-                        open_parens += 1
-                    elif token.TokenType is TOKEN.CLOSE_PAREN:
-                        open_parens -= 1
-                    if open_parens == 0:
-                        break
-                    values += token.Lexeme
-                    values += ' '
-                values_list.append(values)
-                values = ''
-                if not tokens.MoveNext() or tokens.Current().TokenType is not TOKEN.COMMA:
+        tokens = self.m_Tokens.GetEnumerator()
+        while tokens.MoveNext() and not tokens.Current().UpperEquals("INSERT"):
+            new_query += tokens.Current().Lexeme + ' '
+        if not tokens.MoveNext() or not tokens.Current().UpperEquals("INTO"):
+            return False, query
+        new_query += 'INSERT INTO '
+        while tokens.MoveNext() and not tokens.Current().UpperEquals("VALUES"):
+            new_query += tokens.Current().Lexeme + ' '
+
+        values = ''
+        params = []
+        while tokens.MoveNext():
+            assert tokens.Current().TokenType is TOKEN.OPEN_PAREN
+            open_parens = 1
+            while tokens.MoveNext() or open_parens > 0:
+                token = tokens.Current()
+                if token.TokenType is TOKEN.OPEN_PAREN:
+                    open_parens += 1
+                elif token.TokenType is TOKEN.CLOSE_PAREN:
+                    open_parens -= 1
+                if open_parens == 0:
                     break
-            
-            if len(values_list) <= 1:
-                return False, query
-
-            new_query += ' SELECT '
-            new_query += ' UNION ALL SELECT '.join(values_list)
-
-            return True, new_query
-        except:
+                if token.TokenType is TOKEN.CONSTANT:
+                    values += '?'
+                    params += [token.Lexeme] 
+                else:    
+                    values += token.Lexeme
+                values += ' '
+            values_list.append(values)
+            values = ''
+            if not tokens.MoveNext() or tokens.Current().TokenType is not TOKEN.COMMA:
+                break
+        
+        if len(values_list) <= 1:
             return False, query
 
+        new_query += f" VALUES ({values_list[0]})"
+        raise MultiValuesInsert(query=new_query, rows=len(values_list), params=params)
+
     #  Parse a statement
     def Tokenize(self, p_strInput):
         #  Get a scanner on the sql string
         self.m_Scanner = intersystems_iris.dbapi.preparser._Scanner._Scanner(p_strInput)
         #  Create a new token list
         self.m_Tokens = intersystems_iris.dbapi.preparser._TokenList._TokenList()
         #  Scan the input string and break into tokens
@@ -753,15 +763,18 @@
         #  Do a table lookup to identify token
         if t_strIDUpper in self.s_KeywordTable:
             #  Found it, replace ID with specific type
             t_eToken = self.s_KeywordTable[t_strIDUpper]
             if (t_eToken == TOKEN.NOT):
                 t_strID = self.m_Scanner.checkForNotPredicates()
                 t_strIDUpper = t_strID.upper()
-        self.m_Tokens.Append(intersystems_iris.dbapi.preparser._Token._Token(t_eToken, t_strID, t_strIDUpper))
+        if t_strID == '%s':
+            self.m_Tokens.Append(intersystems_iris.dbapi.preparser._Token._Token(TOKEN.QUESTION_MARK, "?"))
+        else:
+            self.m_Tokens.Append(intersystems_iris.dbapi.preparser._Token._Token(t_eToken, t_strID, t_strIDUpper))
 
     # used for various operators
     def Tokenize_op(self, check_tokens = [ParseToken.tokEQUAL]):
         self.m_Scanner.BeginLexeme()
         if self.m_Scanner.PeekNextToken() in check_tokens:
             # Check for composite operators (e.g. <=, >=, !=, etc.)
             self.m_Scanner.NextToken()
```

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/preparser/_Scanner.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/preparser/_Scanner.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/preparser/_Token.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/preparser/_Token.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/dbapi/preparser/_TokenList.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/dbapi/preparser/_TokenList.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_BusinessHost.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_BusinessHost.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_BusinessOperation.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_BusinessOperation.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_BusinessProcess.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_BusinessProcess.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_BusinessService.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_BusinessService.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_Common.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_Common.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_Director.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_Director.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_IRISBusinessService.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_IRISBusinessService.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_IRISOutboundAdapter.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_IRISOutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_InboundAdapter.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_InboundAdapter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/_OutboundAdapter.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/_OutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/intersystems_iris/pex/__init__.py` & `sqlalchemy-iris-0.6.1b1/intersystems_iris/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/iris/__init__.py` & `sqlalchemy-iris-0.6.1b1/iris/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/iris/irisbuiltins.py` & `sqlalchemy-iris-0.6.1b1/iris/irisbuiltins.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/iris/irisloader.py` & `sqlalchemy-iris-0.6.1b1/iris/irisloader.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/irisnative/_IRISNative.py` & `sqlalchemy-iris-0.6.1b1/irisnative/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/setup.cfg` & `sqlalchemy-iris-0.6.1b1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlalchemy-iris
-version = 0.6.0b2
+version = 0.6.1b1
 description = InterSystems IRIS for SQLAlchemy
 long_description = file: README.md
 url = https://github.com/caretdev/sqlalchemy-iris
 maintainer = CaretDev
 maintainer_email = dmitry@caretdev.com
 license = MIT
 long_description_content_type = text/markdown
```

### Comparing `sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/base.py` & `sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -810,15 +810,15 @@
             if row:
                 return row[0]
         return None
 
     def get_isolation_level(self, connection):
         try:
             level = int(self._get_option(connection, "IsolationMode"))
-        except dbapi.InterfaceError:
+        except dbapi.DatabaseError:
             # caught access violation error
             # by default it's 0
             level = 0
         if level == 0:
             return "READ UNCOMMITTED"
         elif level == 1:
             return "READ COMMITTED"
```

### Comparing `sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/embedded.py` & `sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/embedded.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/information_schema.py` & `sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/information_schema.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/requirements.py` & `sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/requirements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/sqlalchemy_iris/types.py` & `sqlalchemy-iris-0.6.1b1/sqlalchemy_iris/types.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/sqlalchemy_iris.egg-info/PKG-INFO` & `sqlalchemy-iris-0.6.1b1/sqlalchemy_iris.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-iris
-Version: 0.6.0b2
+Version: 0.6.1b1
 Summary: InterSystems IRIS for SQLAlchemy
 Home-page: https://github.com/caretdev/sqlalchemy-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/sqlalchemy-iris
 Project-URL: Tracker, https://github.com/caretdev/sqlalchemy-iris/issues
```

### Comparing `sqlalchemy-iris-0.6.0b2/sqlalchemy_iris.egg-info/SOURCES.txt` & `sqlalchemy-iris-0.6.1b1/sqlalchemy_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy-iris-0.6.0b2/tests/test_suite.py` & `sqlalchemy-iris-0.6.1b1/tests/test_suite.py`

 * *Files identical despite different names*

