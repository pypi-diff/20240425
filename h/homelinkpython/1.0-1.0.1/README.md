# Comparing `tmp/homelinkpython-1.0.tar.gz` & `tmp/homelinkpython-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homelinkpython-1.0.tar", last modified: Wed Apr 24 00:08:54 2024, max compression
+gzip compressed data, was "homelinkpython-1.0.1.tar", last modified: Thu Apr 25 04:48:16 2024, max compression
```

## Comparing `homelinkpython-1.0.tar` & `homelinkpython-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jon       (1000) jon       (1000)        0 2024-04-24 00:08:54.071397 homelinkpython-1.0/
--rw-r--r--   0 jon       (1000) jon       (1000)    35149 2024-04-23 22:13:20.000000 homelinkpython-1.0/LICENSE
--rw-r--r--   0 jon       (1000) jon       (1000)      353 2024-04-24 00:08:54.071397 homelinkpython-1.0/PKG-INFO
--rw-r--r--   0 jon       (1000) jon       (1000)       62 2024-04-23 22:13:20.000000 homelinkpython-1.0/README.md
-drwxr-xr-x   0 jon       (1000) jon       (1000)        0 2024-04-24 00:08:54.070397 homelinkpython-1.0/homelink_python/
--rw-r--r--   0 jon       (1000) jon       (1000)       19 2024-04-23 23:33:55.000000 homelinkpython-1.0/homelink_python/__init__.py
--rw-r--r--   0 jon       (1000) jon       (1000)      185 2024-04-23 23:49:47.000000 homelinkpython-1.0/homelink_python/cli.py
--rw-r--r--   0 jon       (1000) jon       (1000)    10412 2024-04-23 23:53:01.000000 homelinkpython-1.0/homelink_python/client.py
--rw-r--r--   0 jon       (1000) jon       (1000)      996 2024-04-23 23:51:58.000000 homelinkpython-1.0/homelink_python/net.py
--rw-r--r--   0 jon       (1000) jon       (1000)     7040 2024-04-23 23:08:12.000000 homelinkpython-1.0/homelink_python/packet.py
--rw-r--r--   0 jon       (1000) jon       (1000)     1300 2024-04-23 23:53:21.000000 homelinkpython-1.0/homelink_python/security.py
-drwxr-xr-x   0 jon       (1000) jon       (1000)        0 2024-04-24 00:08:54.071397 homelinkpython-1.0/homelinkpython.egg-info/
--rw-r--r--   0 jon       (1000) jon       (1000)      353 2024-04-24 00:08:54.000000 homelinkpython-1.0/homelinkpython.egg-info/PKG-INFO
--rw-r--r--   0 jon       (1000) jon       (1000)      410 2024-04-24 00:08:54.000000 homelinkpython-1.0/homelinkpython.egg-info/SOURCES.txt
--rw-r--r--   0 jon       (1000) jon       (1000)        1 2024-04-24 00:08:54.000000 homelinkpython-1.0/homelinkpython.egg-info/dependency_links.txt
--rw-r--r--   0 jon       (1000) jon       (1000)       65 2024-04-24 00:08:54.000000 homelinkpython-1.0/homelinkpython.egg-info/entry_points.txt
--rw-r--r--   0 jon       (1000) jon       (1000)       13 2024-04-24 00:08:54.000000 homelinkpython-1.0/homelinkpython.egg-info/requires.txt
--rw-r--r--   0 jon       (1000) jon       (1000)       16 2024-04-24 00:08:54.000000 homelinkpython-1.0/homelinkpython.egg-info/top_level.txt
--rw-r--r--   0 jon       (1000) jon       (1000)       38 2024-04-24 00:08:54.071397 homelinkpython-1.0/setup.cfg
--rw-r--r--   0 jon       (1000) jon       (1000)      679 2024-04-24 00:02:09.000000 homelinkpython-1.0/setup.py
+drwxr-xr-x   0 jon       (1000) jon       (1000)        0 2024-04-25 04:48:16.314301 homelinkpython-1.0.1/
+-rw-r--r--   0 jon       (1000) jon       (1000)    35149 2024-04-23 22:13:20.000000 homelinkpython-1.0.1/LICENSE
+-rw-r--r--   0 jon       (1000) jon       (1000)      355 2024-04-25 04:48:16.314301 homelinkpython-1.0.1/PKG-INFO
+-rw-r--r--   0 jon       (1000) jon       (1000)       62 2024-04-23 22:13:20.000000 homelinkpython-1.0.1/README.md
+drwxr-xr-x   0 jon       (1000) jon       (1000)        0 2024-04-25 04:48:16.314301 homelinkpython-1.0.1/homelink_python/
+-rw-r--r--   0 jon       (1000) jon       (1000)       21 2024-04-25 04:48:13.000000 homelinkpython-1.0.1/homelink_python/__init__.py
+-rw-r--r--   0 jon       (1000) jon       (1000)      185 2024-04-23 23:49:47.000000 homelinkpython-1.0.1/homelink_python/cli.py
+-rw-r--r--   0 jon       (1000) jon       (1000)    10410 2024-04-25 04:44:35.000000 homelinkpython-1.0.1/homelink_python/client.py
+-rw-r--r--   0 jon       (1000) jon       (1000)      996 2024-04-23 23:51:58.000000 homelinkpython-1.0.1/homelink_python/net.py
+-rw-r--r--   0 jon       (1000) jon       (1000)     7040 2024-04-23 23:08:12.000000 homelinkpython-1.0.1/homelink_python/packet.py
+-rw-r--r--   0 jon       (1000) jon       (1000)     1300 2024-04-23 23:53:21.000000 homelinkpython-1.0.1/homelink_python/security.py
+drwxr-xr-x   0 jon       (1000) jon       (1000)        0 2024-04-25 04:48:16.314301 homelinkpython-1.0.1/homelinkpython.egg-info/
+-rw-r--r--   0 jon       (1000) jon       (1000)      355 2024-04-25 04:48:16.000000 homelinkpython-1.0.1/homelinkpython.egg-info/PKG-INFO
+-rw-r--r--   0 jon       (1000) jon       (1000)      410 2024-04-25 04:48:16.000000 homelinkpython-1.0.1/homelinkpython.egg-info/SOURCES.txt
+-rw-r--r--   0 jon       (1000) jon       (1000)        1 2024-04-25 04:48:16.000000 homelinkpython-1.0.1/homelinkpython.egg-info/dependency_links.txt
+-rw-r--r--   0 jon       (1000) jon       (1000)       65 2024-04-25 04:48:16.000000 homelinkpython-1.0.1/homelinkpython.egg-info/entry_points.txt
+-rw-r--r--   0 jon       (1000) jon       (1000)       13 2024-04-25 04:48:16.000000 homelinkpython-1.0.1/homelinkpython.egg-info/requires.txt
+-rw-r--r--   0 jon       (1000) jon       (1000)       16 2024-04-25 04:48:16.000000 homelinkpython-1.0.1/homelinkpython.egg-info/top_level.txt
+-rw-r--r--   0 jon       (1000) jon       (1000)       38 2024-04-25 04:48:16.314301 homelinkpython-1.0.1/setup.cfg
+-rw-r--r--   0 jon       (1000) jon       (1000)      679 2024-04-24 00:02:09.000000 homelinkpython-1.0.1/setup.py
```

### Comparing `homelinkpython-1.0/LICENSE` & `homelinkpython-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `homelinkpython-1.0/homelink_python/client.py` & `homelinkpython-1.0.1/homelink_python/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                 randomBytes(32),
                 hashString(password).encode("UTF-8"),
                 bytes([0] * 8),
                 randomBytes(24),
             )
             registerRequestPacket = RegisterRequestPacket(
                 connectionId,
-                self.host_id,
+                self.hostId,
                 self.serviceId,
                 rsaEncrypt(passwordData, self.serverPublicKey),
             )
             data = RegisterRequestPacket.serialize(registerRequestPacket)
             self.controlSocket.sendto(data, self.serverUdpAddress)
             try:
                 data, _ = self.controlSocket.recvfrom(1024)
@@ -123,15 +123,15 @@
                 randomBytes(28),
                 hashString(password).encode("UTF-8"),
                 bytes([0] * 8),
                 randomBytes(24),
             )
             loginRequestPacket = LoginRequestPacket(
                 connectionId,
-                self.host_id,
+                self.hostId,
                 self.serviceId,
                 rsaEncrypt(passwordData, self.serverPublicKey),
             )
             data = LoginRequestPacket.serialize(loginRequestPacket)
             self.controlSocket.sendto(data, self.serverUdpAddress)
             try:
                 data, _ = self.controlSocket.recvfrom(1024)
```

### Comparing `homelinkpython-1.0/homelink_python/net.py` & `homelinkpython-1.0.1/homelink_python/net.py`

 * *Files identical despite different names*

### Comparing `homelinkpython-1.0/homelink_python/packet.py` & `homelinkpython-1.0.1/homelink_python/packet.py`

 * *Files identical despite different names*

### Comparing `homelinkpython-1.0/homelink_python/security.py` & `homelinkpython-1.0.1/homelink_python/security.py`

 * *Files identical despite different names*

### Comparing `homelinkpython-1.0/setup.py` & `homelinkpython-1.0.1/setup.py`

 * *Files identical despite different names*

