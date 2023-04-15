# Comparing `tmp/pyllnu-0.2.0a1.tar.gz` & `tmp/pyllnu-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllnu-0.2.0a1.tar", max compression
+gzip compressed data, was "pyllnu-0.2.1.tar", max compression
```

## Comparing `pyllnu-0.2.0a1.tar` & `pyllnu-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1078 2023-03-22 20:09:44.670093 pyllnu-0.2.0a1/LICENSE
--rw-r--r--   0        0        0      683 2023-03-22 20:09:44.670093 pyllnu-0.2.0a1/README.md
--rw-r--r--   0        0        0      583 2023-03-22 20:10:03.059412 pyllnu-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0      407 2023-03-22 20:09:44.670093 pyllnu-0.2.0a1/src/pyllnu/__init__.py
--rw-r--r--   0        0        0     4069 2023-03-22 20:09:44.670093 pyllnu-0.2.0a1/src/pyllnu/constants.py
--rw-r--r--   0        0        0     8401 2023-03-22 20:09:44.671093 pyllnu-0.2.0a1/src/pyllnu/dhcp.py
--rw-r--r--   0        0        0     1830 2023-03-22 20:09:44.671093 pyllnu-0.2.0a1/src/pyllnu/eth.py
--rw-r--r--   0        0        0      177 2023-03-22 20:09:44.671093 pyllnu-0.2.0a1/src/pyllnu/exceptions.py
--rw-r--r--   0        0        0      233 2023-03-22 20:09:44.671093 pyllnu-0.2.0a1/src/pyllnu/icmp.py
--rw-r--r--   0        0        0     4904 2023-03-22 20:09:44.671093 pyllnu-0.2.0a1/src/pyllnu/ipv4.py
--rw-r--r--   0        0        0     4120 2023-03-22 20:09:44.671093 pyllnu-0.2.0a1/src/pyllnu/ipv6.py
--rw-r--r--   0        0        0     3879 2023-03-22 20:09:44.671093 pyllnu-0.2.0a1/src/pyllnu/parser.py
--rw-r--r--   0        0        0      272 2023-03-22 20:09:44.671093 pyllnu-0.2.0a1/src/pyllnu/struct_ancestor.py
--rw-r--r--   0        0        0     6978 2023-03-22 20:09:44.671093 pyllnu-0.2.0a1/src/pyllnu/tcp.py
--rw-r--r--   0        0        0     2814 2023-03-22 20:09:44.671093 pyllnu-0.2.0a1/src/pyllnu/udp.py
--rw-r--r--   0        0        0     2021 2023-03-22 20:09:44.671093 pyllnu-0.2.0a1/src/pyllnu/util.py
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 pyllnu-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-15 22:45:07.838022 pyllnu-0.2.1/LICENSE
+-rw-r--r--   0        0        0      550 2023-04-15 22:45:07.838022 pyllnu-0.2.1/README.md
+-rw-r--r--   0        0        0      584 2023-04-15 22:45:26.466202 pyllnu-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      536 2023-04-15 22:45:07.838022 pyllnu-0.2.1/src/pyllnu/__init__.py
+-rw-r--r--   0        0        0     4064 2023-04-15 22:45:07.838022 pyllnu-0.2.1/src/pyllnu/constants.py
+-rw-r--r--   0        0        0     8652 2023-04-15 22:45:07.838022 pyllnu-0.2.1/src/pyllnu/dhcp.py
+-rw-r--r--   0        0        0     4472 2023-04-15 22:45:07.839022 pyllnu-0.2.1/src/pyllnu/eth.py
+-rw-r--r--   0        0        0      506 2023-04-15 22:45:07.839022 pyllnu-0.2.1/src/pyllnu/exceptions.py
+-rw-r--r--   0        0        0      233 2023-04-15 22:45:07.839022 pyllnu-0.2.1/src/pyllnu/icmp.py
+-rw-r--r--   0        0        0     4896 2023-04-15 22:45:07.839022 pyllnu-0.2.1/src/pyllnu/ipv4.py
+-rw-r--r--   0        0        0     4120 2023-04-15 22:45:07.839022 pyllnu-0.2.1/src/pyllnu/ipv6.py
+-rw-r--r--   0        0        0     3880 2023-04-15 22:45:07.839022 pyllnu-0.2.1/src/pyllnu/parser.py
+-rw-r--r--   0        0        0      273 2023-04-15 22:45:07.839022 pyllnu-0.2.1/src/pyllnu/struct_ancestor.py
+-rw-r--r--   0        0        0     6978 2023-04-15 22:45:07.839022 pyllnu-0.2.1/src/pyllnu/tcp.py
+-rw-r--r--   0        0        0     2814 2023-04-15 22:45:07.839022 pyllnu-0.2.1/src/pyllnu/udp.py
+-rw-r--r--   0        0        0     5007 2023-04-15 22:45:07.839022 pyllnu-0.2.1/src/pyllnu/util.py
+-rw-r--r--   0        0        0     1335 1970-01-01 00:00:00.000000 pyllnu-0.2.1/PKG-INFO
```

### Comparing `pyllnu-0.2.0a1/LICENSE` & `pyllnu-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllnu-0.2.0a1/README.md` & `pyllnu-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # [Python Low-Level Network Utils](https://gitlab.com/debemdeboas/python-low-level-network-utils)
 
 <div align="center">
-    <img src="https://gitlab.com/debemdeboas/python-low-level-network-utils/-/raw/main/doc/img/wireshark-hello-world.png" />
+    <img src="https://gitlab.com/debemdeboas/python-low-level-network-utils/-/raw/main/docs/img/wireshark-hello-world.png" />
 </div>
 
 PyLLNU implements the following protocols:
 
 - Ethernet
 - ICMP
 - IPv4
 - IPv6
 - TCP
 - UDP
 - DHCP
 
-This package allows developers to interact more easily with
-raw sockets.
-You can create IPv4 and IPv6 headers and packets and even build your own protocols.
-
-Raw sockets operate on [OSI layer 2](https://osi-model.com/network-layer/), the Data Link Layer. This layer is also known as the layer in which the Ethernet protocol operates.
+This package allows developers to interact more easily with binary network sockets and network
+protocols.
+You can create IPv4 and IPv6 headers, TCP and UDP packets, and even build your own protocols.
```

### Comparing `pyllnu-0.2.0a1/pyproject.toml` & `pyllnu-0.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pyllnu"
-version = "0.2.0-a1"
-description = "Low-level network utilities. Use raw sockets without the hassle!"
+version = "0.2.1"
+description = "Low-level network utilities. Interact with low-level sockets easily."
 authors = ["Rafael de Bem <debemrafael@gmail.com>"]
 maintainers = ["Rafael de Bem <debemrafael@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://gitlab.com/debemdeboas/python-low-level-network-utils"
 repository = "https://gitlab.com/debemdeboas/python-low-level-network-utils"
```

### Comparing `pyllnu-0.2.0a1/src/pyllnu/constants.py` & `pyllnu-0.2.1/src/pyllnu/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,49 @@
+"""
+This file contains all of the constant values
+used by this package.
+"""
 
 from enum import Enum
 from ipaddress import IPv4Address
 
 ################################################################################
 # ETHERNET CONSTANTS
 ################################################################################
 
 ETH_DEFAULT_NET_IFACE = 'eth0'
 
 ETH_FRAME_SIZE = 1518
-ETH_P_ALL = 3
 ETH_HEADER_FMT = '!6B6BH'
 ETH_MAC_BROADCAST = 'FF:FF:FF:FF:FF:FF'
 
 
 ################################################################################
 # IPV4 CONSTANTS
 ################################################################################
 
-IPV4_LOCALHOST = IPv4Address('127.0.0.1')
-IPV4_BROADCAST = IPv4Address('255.255.255.255')
+IPV4_LOCALHOST = '127.0.0.1'
+IPV4_BROADCAST = '255.255.255.255'
 
 IPV4_PACKET_TYPE = 0x0800
 
 
 ################################################################################
 # IPV6 CONSTANTS
 ################################################################################
 
+IPV6_LOCALHOST = '::1'
+
 IPV6_PACKET_TYPE = 0x86DD
 
-IPV6_HEADER_VERSION = 0x6  # 1 nibble
-IPV6_HEADER_TRAFFIC_CLASS = 0x0  # 8 bits
-IPV6_HEADER_FLOW_LABEL = 0x0  # 20 bits
-IPV6_HEADER_NEXT_HEADER = 0x6  # 8 bits
-IPV6_HEADER_HOP_LIMIT = 0xff  # 8 bits
+IPV6_HEADER_VERSION       = 0x6
+IPV6_HEADER_TRAFFIC_CLASS = 0x0
+IPV6_HEADER_FLOW_LABEL    = 0x0
+IPV6_HEADER_NEXT_HEADER   = 0x6
+IPV6_HEADER_HOP_LIMIT     = 0xff
 
 
 ################################################################################
 # TCP CONSTANTS
 ################################################################################
 
 TCP_PROTOCOL = 6
@@ -82,17 +87,18 @@
 DHCP_REQUEST  = 3
 DHCP_DECLINE  = 4
 DHCP_ACK      = 5
 DHCP_NACK     = 6
 DHCP_RELEASE  = 7
 
 # FIELD LENGTHS
-DHCP_MAX_CHADDR_LENGTH           = 16
-DHCP_MAX_SNAME_LENGTH            = 64
-DHCP_MAX_FILE_LENGTH             = 128
+DHCP_MAX_CHADDR_LENGTH = 16
+DHCP_MAX_SNAME_LENGTH  = 64
+DHCP_MAX_FILE_LENGTH   = 128
+
 DHCP_ETHERNET_HARDWARE_ADDRESS        = 1  #/* used in htype field of dhcp packet */
 DHCP_ETHERNET_HARDWARE_ADDRESS_LENGTH = 6  #/* length of Ethernet hardware addresses */
 
 # MISC DEFINITIONS
 DHCP_INFINITE_TIME = 0xffffffff
 DHCP_BROADCAST_FLAG = 32768
 
@@ -138,14 +144,14 @@
 
 class IPProtocolType(Enum):
     TCP  = TCP_PROTOCOL
     UDP  = UDP_PROTOCOL
     ICMP = ICMP_PROTOCOL
 
 
-class ApplicationPortType(Enum):
+class PortToApplicationType(Enum):
     SSH = 22
     DNS = 53
     DHCP_SERVER = 67
     DHCP_CLIENT = 68
     HTTP = 80
     HTTPS = 443
```

### Comparing `pyllnu-0.2.0a1/src/pyllnu/dhcp.py` & `pyllnu-0.2.1/src/pyllnu/dhcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,39 @@
+"""
+DHCP-related functionality.
 
-from ctypes import (POINTER, BigEndianStructure, c_char, c_ubyte, c_uint8,
-                    c_uint16, c_uint32, cast, memmove, pointer, sizeof)
+This module implements DHCP-like funcionality that
+can be used to build a pseudo-DHCP server.
+"""
+
+from ctypes import (POINTER, c_char, c_ubyte, c_uint8, c_uint16, c_uint32,
+                    cast, memmove, pointer, sizeof)
 from enum import Enum, auto
 from ipaddress import IPv4Address
 from typing import Any
 
 from src.pyllnu.constants import *
 from src.pyllnu.exceptions import *
 from src.pyllnu.ipv4 import ip_to_int
+from src.pyllnu.struct_ancestor import StructAncestor
 
 
 # DHCP EXCHANGE STATUS
 # This Enum represents an IP's status on the IP allocation pool.
 # If the IP has been offered to a client but not taken, it'S
 # marked as offered. If it's taken, it's marked as taken.
 # Otherwise, it's marked as free.
 class DHCPIPStatus(Enum):
     FREE    = auto()
     OFFERED = auto()
     TAKEN   = auto()
 
 
 # DHCP MESSAGE BIG-ENDIAN STRUCT
-class DHCPMessage(BigEndianStructure):
+class DHCPMessage(StructAncestor):
     _fields_ = [
         ('op',      c_uint8),  # 1 for client, 2 for server
         ('htype',   c_uint8),  # Ethernet: 1
         ('hlen',    c_uint8),  # MAC len: 6
         ('hops',    c_uint8),  # 0
         ('xid',     c_uint32), # Random from 0x0 to 0xffffffff
         ('secs',    c_uint16), # 0
@@ -106,20 +113,20 @@
                 raise DHCPError('Corrupt message')
             elif op_code == 0:
                 continue
             elif op_code == 0xff:
                 break
             elif op_code == DHCP_OPTION_MESSAGE_TYPE:
                 # Ignore len
-                msg_type = cast(buf[nstart:], POINTER(c_ubyte))[0]
+                msg_type = cast(buf[nstart:], POINTER(c_ubyte))[0] # type: ignore
                 nstart += sizeof(c_ubyte)
                 opts[op_code] = msg_type
             elif op_code == DHCP_OPTION_DNS:
                 dns = []
-                _len = cast(buf[nstart:], POINTER(c_ubyte))[0]
+                _len = cast(buf[nstart:], POINTER(c_ubyte))[0] # type: ignore
                 for i in range(0, _len, sizeof(c_uint32)):
                     if i + sizeof(c_uint32) >= _len:
                         break
                     dns.append(IPv4Address(buf[nstart:nstart+sizeof(c_uint32)][:]))
                     nstart += sizeof(c_uint32)
                 opts[op_code] = dns
             elif op_code == DHCP_OPTION_REQUESTED_ADDRESS or \
@@ -130,21 +137,21 @@
                 nstart += sizeof(c_uint32)
             elif op_code == DHCP_OPTION_LEASE_TIME or \
                  op_code == DHCP_OPTION_RENEWAL_TIME or \
                  op_code == DHCP_OPTION_REBINDING_TIME:
                 opts[op_code] = int.from_bytes(buf[nstart:nstart+sizeof(c_uint32)], 'big')
                 nstart += sizeof(c_uint32)
             elif op_code == DHCP_OPTION_HOST_NAME:
-                _len = cast(buf[nstart-1:], POINTER(c_ubyte))[0]
-                hostname = cast(buf[nstart:], POINTER(c_char))[:_len]
+                _len = cast(buf[nstart-1:], POINTER(c_ubyte))[0] # type: ignore
+                hostname = cast(buf[nstart:], POINTER(c_char))[:_len] # type: ignore
                 nstart += _len
-                opts[op_code] = hostname.decode('utf-8')
+                opts[op_code] = hostname.decode('utf-8') # type: ignore
             else:
                 print(f'[DHCP] WARN: RECEIVED UNKNOWN OPCODE {op_code}')
-                nstart += cast(buf[nstart-1:], POINTER(c_ubyte))[0]
+                nstart += cast(buf[nstart-1:], POINTER(c_ubyte))[0] # type: ignore
         return opts
 
 
     @staticmethod
     def unpack_msg(buf: bytes) -> tuple['DHCPMessage', dict]:
         msg = buf[:sizeof(DHCPMessage)]
         opts = buf[sizeof(DHCPMessage):]
```

### Comparing `pyllnu-0.2.0a1/src/pyllnu/ipv4.py` & `pyllnu-0.2.1/src/pyllnu/ipv4.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from src.pyllnu.struct_ancestor import StructAncestor
 
 
 class IPv4PseudoHeader(BigEndianStructure):
     """
     Represents a pseudo-header to be used when calculating the definitive
     header's checksum. This structure uses IPv4 (32-bit) addresses.
-    
+
     This header contains only a few fields from the original header.
     """
     _fields_ = [
         ('src_ip',      c_ubyte * 4),
         ('dst_ip',      c_ubyte * 4),
         ('len',         c_uint32),
         ('zero',        c_uint, 24),
@@ -91,15 +91,15 @@
         ipv4_hdr.src      = int(IPv4Address(src_ip))
         ipv4_hdr.dst      = int(IPv4Address(dst_ip))
         ipv4_hdr.options  = 0
         ipv4_hdr.padding  = 0
         ipv4_hdr.calc_checksum()
 
         return ipv4_hdr
-    
+
     def calc_checksum(self):
         """
         Calculates an IPv4 header's checksum in-place.
 
         Args:
             hdr (IPv4Header)
         """
```

### Comparing `pyllnu-0.2.0a1/src/pyllnu/ipv6.py` & `pyllnu-0.2.1/src/pyllnu/ipv6.py`

 * *Files identical despite different names*

### Comparing `pyllnu-0.2.0a1/src/pyllnu/parser.py` & `pyllnu-0.2.1/src/pyllnu/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 from ctypes import sizeof
 from typing import Any
 
 from src.pyllnu.constants import ETHPacketType, IPProtocolType
 from src.pyllnu.eth import unpack_eth_header
 from src.pyllnu.exceptions import UnknownProtocolError
 from src.pyllnu.ipv4 import IPv4Header
```

### Comparing `pyllnu-0.2.0a1/src/pyllnu/tcp.py` & `pyllnu-0.2.1/src/pyllnu/tcp.py`

 * *Files identical despite different names*

### Comparing `pyllnu-0.2.0a1/src/pyllnu/udp.py` & `pyllnu-0.2.1/src/pyllnu/udp.py`

 * *Files identical despite different names*

### Comparing `pyllnu-0.2.0a1/PKG-INFO` & `pyllnu-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyllnu
-Version: 0.2.0a1
-Summary: Low-level network utilities. Use raw sockets without the hassle!
+Version: 0.2.1
+Summary: Low-level network utilities. Interact with low-level sockets easily.
 Home-page: https://gitlab.com/debemdeboas/python-low-level-network-utils
 License: MIT
 Author: Rafael de Bem
 Author-email: debemrafael@gmail.com
 Maintainer: Rafael de Bem
 Maintainer-email: debemrafael@gmail.com
 Requires-Python: >=3.9
@@ -17,26 +17,24 @@
 Requires-Dist: netifaces (>=0.11.0,<0.12.0)
 Project-URL: Repository, https://gitlab.com/debemdeboas/python-low-level-network-utils
 Description-Content-Type: text/markdown
 
 # [Python Low-Level Network Utils](https://gitlab.com/debemdeboas/python-low-level-network-utils)
 
 <div align="center">
-    <img src="https://gitlab.com/debemdeboas/python-low-level-network-utils/-/raw/main/doc/img/wireshark-hello-world.png" />
+    <img src="https://gitlab.com/debemdeboas/python-low-level-network-utils/-/raw/main/docs/img/wireshark-hello-world.png" />
 </div>
 
 PyLLNU implements the following protocols:
 
 - Ethernet
 - ICMP
 - IPv4
 - IPv6
 - TCP
 - UDP
 - DHCP
 
-This package allows developers to interact more easily with
-raw sockets.
-You can create IPv4 and IPv6 headers and packets and even build your own protocols.
-
-Raw sockets operate on [OSI layer 2](https://osi-model.com/network-layer/), the Data Link Layer. This layer is also known as the layer in which the Ethernet protocol operates.
+This package allows developers to interact more easily with binary network sockets and network
+protocols.
+You can create IPv4 and IPv6 headers, TCP and UDP packets, and even build your own protocols.
```

