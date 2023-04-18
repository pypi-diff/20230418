# Comparing `tmp/naver-net-0.0.2.post1.tar.gz` & `tmp/naver-net-0.0.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naver-net-0.0.2.post1.tar", last modified: Fri Jul 15 14:58:28 2022, max compression
+gzip compressed data, was "naver-net-0.0.2.post2.tar", last modified: Tue Apr 18 01:36:45 2023, max compression
```

## Comparing `naver-net-0.0.2.post1.tar` & `naver-net-0.0.2.post2.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxrwxrwx   0        0        0        0 2022-07-15 14:58:28.055768 naver-net-0.0.2.post1/
--rw-rw-rw-   0        0        0      454 2022-07-15 14:58:28.055768 naver-net-0.0.2.post1/PKG-INFO
--rw-rw-rw-   0        0        0        6 2021-09-30 15:45:55.000000 naver-net-0.0.2.post1/README.md
-drwxrwxrwx   0        0        0        0 2022-07-15 14:58:27.993195 naver-net-0.0.2.post1/naver_net/
--rw-rw-rw-   0        0        0     1021 2021-10-25 17:56:59.000000 naver-net-0.0.2.post1/naver_net/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-15 14:58:28.005559 naver-net-0.0.2.post1/naver_net/bus/
--rw-rw-rw-   0        0        0      160 2021-09-30 14:11:21.000000 naver-net-0.0.2.post1/naver_net/bus/__init__.py
--rw-rw-rw-   0        0        0     1050 2021-10-19 16:17:38.000000 naver-net-0.0.2.post1/naver_net/bus/busclient.py
-drwxrwxrwx   0        0        0        0 2022-07-15 14:58:28.008559 naver-net-0.0.2.post1/naver_net/dns/
--rw-rw-rw-   0        0        0      160 2021-09-30 14:11:21.000000 naver-net-0.0.2.post1/naver_net/dns/__init__.py
--rw-rw-rw-   0        0        0    14155 2021-09-30 21:48:03.000000 naver-net-0.0.2.post1/naver_net/dns/dnsserver.py
-drwxrwxrwx   0        0        0        0 2022-07-15 14:58:28.012943 naver-net-0.0.2.post1/naver_net/host/
--rw-rw-rw-   0        0        0      160 2021-09-30 14:11:21.000000 naver-net-0.0.2.post1/naver_net/host/__init__.py
--rw-rw-rw-   0        0        0      459 2021-09-30 16:35:23.000000 naver-net-0.0.2.post1/naver_net/host/hostname.py
-drwxrwxrwx   0        0        0        0 2022-07-15 14:58:28.016697 naver-net-0.0.2.post1/naver_net/mail/
--rw-rw-rw-   0        0        0     2147 2022-07-15 14:56:48.000000 naver-net-0.0.2.post1/naver_net/mail/__init__.py
--rw-rw-rw-   0        0        0       36 2021-09-30 16:38:32.000000 naver-net-0.0.2.post1/naver_net/main.py
-drwxrwxrwx   0        0        0        0 2022-07-15 14:58:28.046811 naver-net-0.0.2.post1/naver_net/proxy/
--rw-rw-rw-   0        0        0      160 2021-09-30 14:11:21.000000 naver-net-0.0.2.post1/naver_net/proxy/__init__.py
--rw-rw-rw-   0        0        0      128 2021-09-30 21:57:56.000000 naver-net-0.0.2.post1/naver_net/proxy/proxyclient.py
--rw-rw-rw-   0        0        0      321 2021-09-30 21:58:40.000000 naver-net-0.0.2.post1/naver_net/proxy/proxyserver.py
-drwxrwxrwx   0        0        0        0 2022-07-15 14:58:28.052758 naver-net-0.0.2.post1/naver_net/vpn/
--rw-rw-rw-   0        0        0      214 2021-10-19 16:07:54.000000 naver-net-0.0.2.post1/naver_net/vpn/__init__.py
--rw-rw-rw-   0        0        0    22229 2021-10-19 16:14:09.000000 naver-net-0.0.2.post1/naver_net/vpn/client.py
--rw-rw-rw-   0        0        0      108 2021-09-30 16:32:06.000000 naver-net-0.0.2.post1/naver_net/vpn/generate_fernet_key.py
--rw-rw-rw-   0        0        0     2289 2021-10-19 16:07:25.000000 naver-net-0.0.2.post1/naver_net/vpn/hub.py
--rw-rw-rw-   0        0        0     3930 2021-09-30 16:32:06.000000 naver-net-0.0.2.post1/naver_net/vpn/protocol.py
-drwxrwxrwx   0        0        0        0 2022-07-15 14:58:28.003559 naver-net-0.0.2.post1/naver_net.egg-info/
--rw-rw-rw-   0        0        0      454 2022-07-15 14:58:27.000000 naver-net-0.0.2.post1/naver_net.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      650 2022-07-15 14:58:27.000000 naver-net-0.0.2.post1/naver_net.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-15 14:58:27.000000 naver-net-0.0.2.post1/naver_net.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-07-15 14:58:27.000000 naver-net-0.0.2.post1/naver_net.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-07-15 14:58:27.000000 naver-net-0.0.2.post1/naver_net.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-15 14:58:28.056768 naver-net-0.0.2.post1/setup.cfg
--rw-rw-rw-   0        0        0      765 2022-07-15 14:57:26.000000 naver-net-0.0.2.post1/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-15 14:58:28.053769 naver-net-0.0.2.post1/test/
--rw-rw-rw-   0        0        0      198 2021-09-29 14:12:13.000000 naver-net-0.0.2.post1/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:36:45.353201 naver-net-0.0.2.post2/
+-rw-rw-rw-   0        0        0      415 2023-04-18 01:36:45.352222 naver-net-0.0.2.post2/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 01:36:45.298351 naver-net-0.0.2.post2/naver_net/
+-rw-rw-rw-   0        0        0     1021 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:36:45.322924 naver-net-0.0.2.post2/naver_net/bus/
+-rw-rw-rw-   0        0        0      160 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/bus/__init__.py
+-rw-rw-rw-   0        0        0     1050 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/bus/busclient.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:36:45.327930 naver-net-0.0.2.post2/naver_net/dns/
+-rw-rw-rw-   0        0        0      160 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/dns/__init__.py
+-rw-rw-rw-   0        0        0    14155 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/dns/dnsserver.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:36:45.331930 naver-net-0.0.2.post2/naver_net/host/
+-rw-rw-rw-   0        0        0      160 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/host/__init__.py
+-rw-rw-rw-   0        0        0      459 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/host/hostname.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:36:45.332926 naver-net-0.0.2.post2/naver_net/mail/
+-rw-rw-rw-   0        0        0     1628 2023-04-18 00:10:18.000000 naver-net-0.0.2.post2/naver_net/mail/__init__.py
+-rw-rw-rw-   0        0        0       36 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/main.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:36:45.339926 naver-net-0.0.2.post2/naver_net/proxy/
+-rw-rw-rw-   0        0        0      160 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/proxy/__init__.py
+-rw-rw-rw-   0        0        0      128 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/proxy/proxyclient.py
+-rw-rw-rw-   0        0        0      321 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/proxy/proxyserver.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:36:45.350200 naver-net-0.0.2.post2/naver_net/vpn/
+-rw-rw-rw-   0        0        0      214 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/vpn/__init__.py
+-rw-rw-rw-   0        0        0    22905 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/vpn/client.py
+-rw-rw-rw-   0        0        0      112 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/vpn/generate_fernet_key.py
+-rw-rw-rw-   0        0        0     2361 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/vpn/hub.py
+-rw-rw-rw-   0        0        0     4082 2023-04-18 00:04:52.000000 naver-net-0.0.2.post2/naver_net/vpn/protocol.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:36:45.317925 naver-net-0.0.2.post2/naver_net.egg-info/
+-rw-rw-rw-   0        0        0      415 2023-04-18 01:36:45.000000 naver-net-0.0.2.post2/naver_net.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      633 2023-04-18 01:36:45.000000 naver-net-0.0.2.post2/naver_net.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 01:36:45.000000 naver-net-0.0.2.post2/naver_net.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-18 01:36:45.000000 naver-net-0.0.2.post2/naver_net.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-18 01:36:45.000000 naver-net-0.0.2.post2/naver_net.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 01:36:45.353201 naver-net-0.0.2.post2/setup.cfg
+-rw-rw-rw-   0        0        0      765 2023-04-18 01:36:36.000000 naver-net-0.0.2.post2/setup.py
```

### Comparing `naver-net-0.0.2.post1/naver_net/__init__.py` & `naver-net-0.0.2.post2/naver_net/__init__.py`

 * *Files identical despite different names*

### Comparing `naver-net-0.0.2.post1/naver_net/bus/busclient.py` & `naver-net-0.0.2.post2/naver_net/bus/busclient.py`

 * *Files identical despite different names*

### Comparing `naver-net-0.0.2.post1/naver_net/dns/dnsserver.py` & `naver-net-0.0.2.post2/naver_net/dns/dnsserver.py`

 * *Files identical despite different names*

### Comparing `naver-net-0.0.2.post1/naver_net/vpn/hub.py` & `naver-net-0.0.2.post2/naver_net/vpn/hub.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-#!/usr/bin/env python3
-
-import socket 
-import logging
-import datetime 
-import protocol
-
-
-MAX_PACKET_SIZE = 8192
-HOST_ADVERT_TIMEOUT_SEC = 60
-
-logging.basicConfig(level=logging.DEBUG)
-log = logging.getLogger(__name__)
-
-
-class VPNHub():
-    def __init__(self, args, **kwargs):
-        self.args = args | kwargs
-        self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        self.hosts = {}
-        self.main(self.args)
-
-    def main(self):
-        log.info('starting server at [%s]:%s' %
-                 (self.args.addr, self.args.port))
-        self.sock.bind((self.args.addr, self.args.port))
-
-        try:
-            self.main_loop()
-        finally:
-            log.info('closing server socket')
-            self.sock.close()
-
-    def main_loop(self):
-        # hosts map (addr,port) -> ts_last_packet
-
-        while True:
-            try:
-                packet = protocol.receive()
-            except protocol.MalformedPacket as e:
-                log.debug('skipping malformed packet: %s' % e)
-                continue
-
-            if packet.magic is not protocol.Magic.C2H:
-                log.debug('non-c2h packet, ignoring')
-                continue
-
-            self.hosts[packet.peer] = datetime.datetime.now()
-
-            c2h = packet.payload
-            assert c2h is not None
-            assert isinstance(c2h, protocol.Packet_c2h)
-
-            self.broadcast_peer(packet.peer, c2h, self.hosts)
-
-    def broadcast_peer(self,  src_peer, packet, hosts, ):
-        log.debug('broadcasting: %s:%d' % src_peer)
-
-        data = protocol.to_bytes(protocol.Magic.H2C, protocol.Packet_h2c(
-            src_addr=src_peer[0], src_port=src_peer[1], protocol_version=packet.protocol_version, session_id=packet.session_id, ))
-
-        # make a copy because iteration may delete stale entries
-        now = datetime.datetime.now()
-        for peer, ts_last_advert in list(hosts.items()):
-            if (now - ts_last_advert).total_seconds() > HOST_ADVERT_TIMEOUT_SEC:
-                log.debug('deleting stale host %s:%d' % peer)
-                del hosts[peer]
-            elif peer == src_peer:
-                pass  # don't echo the packet back to the sender
-            else:
-                log.debug('  -> %s:%d' % peer)
-                self.sock.sendto(data, peer)
+#!/usr/bin/env python3
+
+import socket 
+import logging
+import datetime 
+import protocol
+
+
+MAX_PACKET_SIZE = 8192
+HOST_ADVERT_TIMEOUT_SEC = 60
+
+logging.basicConfig(level=logging.DEBUG)
+log = logging.getLogger(__name__)
+
+
+class VPNHub():
+    def __init__(self, args, **kwargs):
+        self.args = args | kwargs
+        self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self.hosts = {}
+        self.main(self.args)
+
+    def main(self):
+        log.info('starting server at [%s]:%s' %
+                 (self.args.addr, self.args.port))
+        self.sock.bind((self.args.addr, self.args.port))
+
+        try:
+            self.main_loop()
+        finally:
+            log.info('closing server socket')
+            self.sock.close()
+
+    def main_loop(self):
+        # hosts map (addr,port) -> ts_last_packet
+
+        while True:
+            try:
+                packet = protocol.receive()
+            except protocol.MalformedPacket as e:
+                log.debug('skipping malformed packet: %s' % e)
+                continue
+
+            if packet.magic is not protocol.Magic.C2H:
+                log.debug('non-c2h packet, ignoring')
+                continue
+
+            self.hosts[packet.peer] = datetime.datetime.now()
+
+            c2h = packet.payload
+            assert c2h is not None
+            assert isinstance(c2h, protocol.Packet_c2h)
+
+            self.broadcast_peer(packet.peer, c2h, self.hosts)
+
+    def broadcast_peer(self,  src_peer, packet, hosts, ):
+        log.debug('broadcasting: %s:%d' % src_peer)
+
+        data = protocol.to_bytes(protocol.Magic.H2C, protocol.Packet_h2c(
+            src_addr=src_peer[0], src_port=src_peer[1], protocol_version=packet.protocol_version, session_id=packet.session_id, ))
+
+        # make a copy because iteration may delete stale entries
+        now = datetime.datetime.now()
+        for peer, ts_last_advert in list(hosts.items()):
+            if (now - ts_last_advert).total_seconds() > HOST_ADVERT_TIMEOUT_SEC:
+                log.debug('deleting stale host %s:%d' % peer)
+                del hosts[peer]
+            elif peer == src_peer:
+                pass  # don't echo the packet back to the sender
+            else:
+                log.debug('  -> %s:%d' % peer)
+                self.sock.sendto(data, peer)
```

### Comparing `naver-net-0.0.2.post1/naver_net/vpn/protocol.py` & `naver-net-0.0.2.post2/naver_net/vpn/protocol.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-import struct
-import socket
-import collections
-from enum import Enum
-from typing import NamedTuple, Tuple, Union, Optional
-
-VERSION : int = 4
-MAX_PACKET_SIZE : int = 8192
-
-class Magic(Enum):
-    C2H      = 0x01
-    H2C      = 0x02
-    C2C_PING = 0x04
-    C2C_PONG = 0x05
-    C2C_AUTH = 0x06
-    C2C_DATA = 0x08
-
-Peer = Tuple[str, int]
-
-class Packet_h2c(NamedTuple):
-    src_addr : str
-    src_port : int
-    protocol_version : int
-    session_id : int
-
-class Packet_c2h(NamedTuple):
-    protocol_version : int
-    session_id : int
-
-class Packet_ping(NamedTuple):
-    payload : bytes
-
-class Packet_auth_enc(NamedTuple):
-    payload_enc : bytes
-
-class Packet_data(NamedTuple):
-    is_encrypted : bool
-    payload : bytes
-
-Packet = Union[
-    Packet_h2c,
-    Packet_c2h,
-    Packet_ping,
-    Packet_auth_enc,
-    Packet_data
-]
-
-class Packet_rx(NamedTuple):
-    peer : Peer
-    magic : Magic
-    payload : Optional[Packet]
-
-class MalformedPacket(Exception):
-    pass
-
-def _read_c_string(bs : bytes) -> Tuple[str, bytes]:
-    nul = bs.find(0)
-    if nul < 0:
-        raise MalformedPacket('NUL byte not found')
-
-    return bs[:nul].decode('ascii'), bs[nul+1:]
-
-def to_bytes(magic : Magic, packet : Packet) -> bytes:
-    if magic is Magic.C2H:
-        assert isinstance(packet, Packet_c2h)
-        return \
-            bytes([magic.value, packet.protocol_version]) \
-            + struct.pack('>L', packet.session_id)
-
-    elif magic is Magic.H2C:
-        assert isinstance(packet, Packet_h2c)
-        return \
-            bytes([magic.value]) \
-            + socket.inet_aton(packet.src_addr) \
-            + struct.pack('>H', packet.src_port) \
-            + bytes([int(packet.protocol_version)]) \
-            + struct.pack('>L', packet.session_id)
-
-    elif magic is Magic.C2C_PING:
-        assert isinstance(packet, Packet_ping)
-        return \
-            bytes([magic.value]) \
-            + packet.payload
-
-    elif magic is Magic.C2C_PONG:
-        return bytes([magic.value])
-
-    elif magic is Magic.C2C_AUTH:
-        assert isinstance(packet, Packet_auth_enc)
-        return \
-            bytes([magic.value]) \
-            + packet.payload_enc
-
-    elif magic is Magic.C2C_DATA:
-        assert isinstance(packet, Packet_data)
-        return \
-            bytes([magic.value, int(packet.is_encrypted)]) \
-            + packet.payload
-    else:
-        raise MalformedPacket('unknown tx magic: 0x%02x' % magic.value)
-
-def receive(sock : socket.socket) -> Packet_rx:
-    try:
-        data, peer = sock.recvfrom(MAX_PACKET_SIZE)
-        magic, data = Magic(data[0]), data[1:]
-
-        payload : Optional[Packet]
-        if magic is Magic.C2H:
-            protocol_version = data[0]
-            session_id, = struct.unpack('>L', data[1:5])
-            payload = Packet_c2h(protocol_version, session_id)
-
-        elif magic is Magic.H2C:
-            src_addr = socket.inet_ntoa(data[:4])
-            src_port, = struct.unpack('>H', data[4:6])
-            protocol_version = data[6]
-            session_id, = struct.unpack('>L', data[7:11])
-            payload = Packet_h2c(src_addr, src_port, protocol_version, session_id)
-
-        elif magic is Magic.C2C_PING:
-            payload = Packet_ping(payload=data)
-
-        elif magic is Magic.C2C_PONG:
-            payload = None
-
-        elif magic is Magic.C2C_AUTH:
-            payload = Packet_auth_enc(payload_enc=data)
-
-        elif magic is Magic.C2C_DATA:
-            payload = Packet_data(is_encrypted=bool(data[0]), payload=data[1:])
-
-        else:
-            raise MalformedPacket('unknown magic: 0x%02x' % magic)
-
-        return Packet_rx(
-            peer=peer,
-            magic=magic,
-            payload=payload,
-        )
-    except IndexError as e:
-        raise MalformedPacket(str(e))
-
-def sendto(
-    sock : socket.socket,
-    peer : Peer,
-    magic : Magic,
-    packet : Packet,
-) -> None:
-    sock.sendto(
-        to_bytes(magic, packet),
-        peer,
-    )
+import struct
+import socket
+import collections
+from enum import Enum
+from typing import NamedTuple, Tuple, Union, Optional
+
+VERSION : int = 4
+MAX_PACKET_SIZE : int = 8192
+
+class Magic(Enum):
+    C2H      = 0x01
+    H2C      = 0x02
+    C2C_PING = 0x04
+    C2C_PONG = 0x05
+    C2C_AUTH = 0x06
+    C2C_DATA = 0x08
+
+Peer = Tuple[str, int]
+
+class Packet_h2c(NamedTuple):
+    src_addr : str
+    src_port : int
+    protocol_version : int
+    session_id : int
+
+class Packet_c2h(NamedTuple):
+    protocol_version : int
+    session_id : int
+
+class Packet_ping(NamedTuple):
+    payload : bytes
+
+class Packet_auth_enc(NamedTuple):
+    payload_enc : bytes
+
+class Packet_data(NamedTuple):
+    is_encrypted : bool
+    payload : bytes
+
+Packet = Union[
+    Packet_h2c,
+    Packet_c2h,
+    Packet_ping,
+    Packet_auth_enc,
+    Packet_data
+]
+
+class Packet_rx(NamedTuple):
+    peer : Peer
+    magic : Magic
+    payload : Optional[Packet]
+
+class MalformedPacket(Exception):
+    pass
+
+def _read_c_string(bs : bytes) -> Tuple[str, bytes]:
+    nul = bs.find(0)
+    if nul < 0:
+        raise MalformedPacket('NUL byte not found')
+
+    return bs[:nul].decode('ascii'), bs[nul+1:]
+
+def to_bytes(magic : Magic, packet : Packet) -> bytes:
+    if magic is Magic.C2H:
+        assert isinstance(packet, Packet_c2h)
+        return \
+            bytes([magic.value, packet.protocol_version]) \
+            + struct.pack('>L', packet.session_id)
+
+    elif magic is Magic.H2C:
+        assert isinstance(packet, Packet_h2c)
+        return \
+            bytes([magic.value]) \
+            + socket.inet_aton(packet.src_addr) \
+            + struct.pack('>H', packet.src_port) \
+            + bytes([int(packet.protocol_version)]) \
+            + struct.pack('>L', packet.session_id)
+
+    elif magic is Magic.C2C_PING:
+        assert isinstance(packet, Packet_ping)
+        return \
+            bytes([magic.value]) \
+            + packet.payload
+
+    elif magic is Magic.C2C_PONG:
+        return bytes([magic.value])
+
+    elif magic is Magic.C2C_AUTH:
+        assert isinstance(packet, Packet_auth_enc)
+        return \
+            bytes([magic.value]) \
+            + packet.payload_enc
+
+    elif magic is Magic.C2C_DATA:
+        assert isinstance(packet, Packet_data)
+        return \
+            bytes([magic.value, int(packet.is_encrypted)]) \
+            + packet.payload
+    else:
+        raise MalformedPacket('unknown tx magic: 0x%02x' % magic.value)
+
+def receive(sock : socket.socket) -> Packet_rx:
+    try:
+        data, peer = sock.recvfrom(MAX_PACKET_SIZE)
+        magic, data = Magic(data[0]), data[1:]
+
+        payload : Optional[Packet]
+        if magic is Magic.C2H:
+            protocol_version = data[0]
+            session_id, = struct.unpack('>L', data[1:5])
+            payload = Packet_c2h(protocol_version, session_id)
+
+        elif magic is Magic.H2C:
+            src_addr = socket.inet_ntoa(data[:4])
+            src_port, = struct.unpack('>H', data[4:6])
+            protocol_version = data[6]
+            session_id, = struct.unpack('>L', data[7:11])
+            payload = Packet_h2c(src_addr, src_port, protocol_version, session_id)
+
+        elif magic is Magic.C2C_PING:
+            payload = Packet_ping(payload=data)
+
+        elif magic is Magic.C2C_PONG:
+            payload = None
+
+        elif magic is Magic.C2C_AUTH:
+            payload = Packet_auth_enc(payload_enc=data)
+
+        elif magic is Magic.C2C_DATA:
+            payload = Packet_data(is_encrypted=bool(data[0]), payload=data[1:])
+
+        else:
+            raise MalformedPacket('unknown magic: 0x%02x' % magic)
+
+        return Packet_rx(
+            peer=peer,
+            magic=magic,
+            payload=payload,
+        )
+    except IndexError as e:
+        raise MalformedPacket(str(e))
+
+def sendto(
+    sock : socket.socket,
+    peer : Peer,
+    magic : Magic,
+    packet : Packet,
+) -> None:
+    sock.sendto(
+        to_bytes(magic, packet),
+        peer,
+    )
```

### Comparing `naver-net-0.0.2.post1/naver_net.egg-info/SOURCES.txt` & `naver-net-0.0.2.post2/naver_net.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,9 +17,8 @@
 naver_net/proxy/__init__.py
 naver_net/proxy/proxyclient.py
 naver_net/proxy/proxyserver.py
 naver_net/vpn/__init__.py
 naver_net/vpn/client.py
 naver_net/vpn/generate_fernet_key.py
 naver_net/vpn/hub.py
-naver_net/vpn/protocol.py
-test/__init__.py
+naver_net/vpn/protocol.py
```

### Comparing `naver-net-0.0.2.post1/setup.py` & `naver-net-0.0.2.post2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='naver-net',
-    version='0.0.2-1',
+    version='0.0.2-2',
     packages=setuptools.find_packages(),
     author="Jose Cuevas",
     author_email="jose.cuevas.cv@gmail.com",
     description="A Net Persistence Ancestor Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jacr6/naver-net",
```

