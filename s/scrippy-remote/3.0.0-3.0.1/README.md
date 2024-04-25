# Comparing `tmp/scrippy-remote-3.0.0.tar.gz` & `tmp/scrippy_remote-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrippy-remote-3.0.0.tar", last modified: Tue Mar 12 10:37:19 2024, max compression
+gzip compressed data, was "scrippy_remote-3.0.1.tar", last modified: Thu Apr 25 02:07:05 2024, max compression
```

## Comparing `scrippy-remote-3.0.0.tar` & `scrippy_remote-3.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.715288 scrippy-remote-3.0.0/
--rwxr-xr-x   0 root         (0) root         (0)     1179 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5843 2024-03-12 10:37:19.715288 scrippy-remote-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4255 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)      210 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1344 2024-03-12 10:37:19.717288 scrippy-remote-3.0.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)       38 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.599291 scrippy-remote-3.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.623291 scrippy-remote-3.0.0/src/scrippy_remote/
--rw-r--r--   0 root         (0) root         (0)      222 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/src/scrippy_remote/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.637290 scrippy-remote-3.0.0/src/scrippy_remote/cifs/
--rw-r--r--   0 root         (0) root         (0)     6801 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/src/scrippy_remote/cifs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.646290 scrippy-remote-3.0.0/src/scrippy_remote/ftp/
--rw-r--r--   0 root         (0) root         (0)    14396 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/src/scrippy_remote/ftp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.646290 scrippy-remote-3.0.0/src/scrippy_remote/ftp/clients/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/src/scrippy_remote/ftp/clients/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.647290 scrippy-remote-3.0.0/src/scrippy_remote/ftp/clients/errors/
--rw-r--r--   0 root         (0) root         (0)      165 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/src/scrippy_remote/ftp/clients/errors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.656290 scrippy-remote-3.0.0/src/scrippy_remote/ftp/clients/ftp/
--rw-r--r--   0 root         (0) root         (0)    11576 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/src/scrippy_remote/ftp/clients/ftp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.667289 scrippy-remote-3.0.0/src/scrippy_remote/ftp/clients/ftpes/
--rw-r--r--   0 root         (0) root         (0)     1701 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/src/scrippy_remote/ftp/clients/ftpes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.668289 scrippy-remote-3.0.0/src/scrippy_remote/ftp/clients/ftps/
--rw-r--r--   0 root         (0) root         (0)     4341 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/src/scrippy_remote/ftp/clients/ftps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.681289 scrippy-remote-3.0.0/src/scrippy_remote/local/
--rw-r--r--   0 root         (0) root         (0)     4427 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/src/scrippy_remote/local/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.692288 scrippy-remote-3.0.0/src/scrippy_remote/ssh/
--rw-r--r--   0 root         (0) root         (0)    18011 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/src/scrippy_remote/ssh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.708288 scrippy-remote-3.0.0/src/scrippy_remote.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5843 2024-03-12 10:37:19.000000 scrippy-remote-3.0.0/src/scrippy_remote.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      751 2024-03-12 10:37:19.000000 scrippy-remote-3.0.0/src/scrippy_remote.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-12 10:37:19.000000 scrippy-remote-3.0.0/src/scrippy_remote.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      293 2024-03-12 10:37:19.000000 scrippy-remote-3.0.0/src/scrippy_remote.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-12 10:37:19.000000 scrippy-remote-3.0.0/src/scrippy_remote.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 10:37:19.708288 scrippy-remote-3.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)     2523 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/tests/test_cifs_files.py
--rw-r--r--   0 root         (0) root         (0)     6745 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/tests/test_ftp_files.py
--rw-r--r--   0 root         (0) root         (0)     6155 2024-03-12 10:36:11.000000 scrippy-remote-3.0.0/tests/test_ssh_files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.571675 scrippy_remote-3.0.1/
+-rwxr-xr-x   0 root         (0) root         (0)     1179 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5843 2024-04-25 02:07:05.571675 scrippy_remote-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4255 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      210 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1344 2024-04-25 02:07:05.611674 scrippy_remote-3.0.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)       38 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.409680 scrippy_remote-3.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.436679 scrippy_remote-3.0.1/src/scrippy_remote/
+-rw-r--r--   0 root         (0) root         (0)      222 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/src/scrippy_remote/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.449679 scrippy_remote-3.0.1/src/scrippy_remote/cifs/
+-rw-r--r--   0 root         (0) root         (0)     6801 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/src/scrippy_remote/cifs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.461679 scrippy_remote-3.0.1/src/scrippy_remote/ftp/
+-rw-r--r--   0 root         (0) root         (0)    14396 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/src/scrippy_remote/ftp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.479678 scrippy_remote-3.0.1/src/scrippy_remote/ftp/clients/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/src/scrippy_remote/ftp/clients/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.480678 scrippy_remote-3.0.1/src/scrippy_remote/ftp/clients/errors/
+-rw-r--r--   0 root         (0) root         (0)      165 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/src/scrippy_remote/ftp/clients/errors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.496677 scrippy_remote-3.0.1/src/scrippy_remote/ftp/clients/ftp/
+-rw-r--r--   0 root         (0) root         (0)    11576 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/src/scrippy_remote/ftp/clients/ftp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.507677 scrippy_remote-3.0.1/src/scrippy_remote/ftp/clients/ftpes/
+-rw-r--r--   0 root         (0) root         (0)     1701 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/src/scrippy_remote/ftp/clients/ftpes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.508677 scrippy_remote-3.0.1/src/scrippy_remote/ftp/clients/ftps/
+-rw-r--r--   0 root         (0) root         (0)     4341 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/src/scrippy_remote/ftp/clients/ftps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.519677 scrippy_remote-3.0.1/src/scrippy_remote/local/
+-rw-r--r--   0 root         (0) root         (0)     4427 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/src/scrippy_remote/local/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.534676 scrippy_remote-3.0.1/src/scrippy_remote/ssh/
+-rw-r--r--   0 root         (0) root         (0)    18481 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/src/scrippy_remote/ssh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.565675 scrippy_remote-3.0.1/src/scrippy_remote.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5843 2024-04-25 02:07:05.000000 scrippy_remote-3.0.1/src/scrippy_remote.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      751 2024-04-25 02:07:05.000000 scrippy_remote-3.0.1/src/scrippy_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 02:07:05.000000 scrippy_remote-3.0.1/src/scrippy_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      293 2024-04-25 02:07:05.000000 scrippy_remote-3.0.1/src/scrippy_remote.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-25 02:07:05.000000 scrippy_remote-3.0.1/src/scrippy_remote.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:07:05.565675 scrippy_remote-3.0.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     2523 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/tests/test_cifs_files.py
+-rw-r--r--   0 root         (0) root         (0)     6745 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/tests/test_ftp_files.py
+-rw-r--r--   0 root         (0) root         (0)     6155 2024-04-25 02:06:06.000000 scrippy_remote-3.0.1/tests/test_ssh_files.py
```

### Comparing `scrippy-remote-3.0.0/LICENSE` & `scrippy_remote-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrippy-remote-3.0.0/PKG-INFO` & `scrippy_remote-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrippy-remote
-Version: 3.0.0
+Version: 3.0.1
 Summary: "Client SSH, SFTP et FTP pour le cadriciel Scrippy."
 Home-page: https://codeberg.org/scrippy/scrippy-remote
 Author: Michael Costa, Florent Chevalier
 Author-email: michael.costa@mcos.nc, florent.chevalier.nc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scrippy-remote-3.0.0/README.md` & `scrippy_remote-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `scrippy-remote-3.0.0/setup.cfg` & `scrippy_remote-3.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 3.0.0
+version = 3.0.1
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
```

### Comparing `scrippy-remote-3.0.0/src/scrippy_remote/cifs/__init__.py` & `scrippy_remote-3.0.1/src/scrippy_remote/cifs/__init__.py`

 * *Files identical despite different names*

### Comparing `scrippy-remote-3.0.0/src/scrippy_remote/ftp/__init__.py` & `scrippy_remote-3.0.1/src/scrippy_remote/ftp/__init__.py`

 * *Files identical despite different names*

### Comparing `scrippy-remote-3.0.0/src/scrippy_remote/ftp/clients/ftp/__init__.py` & `scrippy_remote-3.0.1/src/scrippy_remote/ftp/clients/ftp/__init__.py`

 * *Files identical despite different names*

### Comparing `scrippy-remote-3.0.0/src/scrippy_remote/ftp/clients/ftpes/__init__.py` & `scrippy_remote-3.0.1/src/scrippy_remote/ftp/clients/ftpes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrippy-remote-3.0.0/src/scrippy_remote/ftp/clients/ftps/__init__.py` & `scrippy_remote-3.0.1/src/scrippy_remote/ftp/clients/ftps/__init__.py`

 * *Files identical despite different names*

### Comparing `scrippy-remote-3.0.0/src/scrippy_remote/local/__init__.py` & `scrippy_remote-3.0.1/src/scrippy_remote/local/__init__.py`

 * *Files identical despite different names*

### Comparing `scrippy-remote-3.0.0/src/scrippy_remote/ssh/__init__.py` & `scrippy_remote-3.0.1/src/scrippy_remote/ssh/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
     ``username``: String. The user name to use for authentication on remote host.
     ``password``: String. Optional, the password to use fo authentication on remote host. If the ``key`` argument is provided, then the ``password`` value will be use as the SSH key passphrase.
     ``host``: String. The remote host to connect to.
     ``port``: Int. Optional. The TCP remote port to connect to. Default: ``22``.
     ``key``: String. Optional. The SSH private key file name to use for authentication on remote host.
     ``missing_host_key_policy``: String. Optional. Define the behavior when a remote key is missing and remote host is unknown. This should be one of ``auto``, ``warn``, ``reject``. Default to ``warn`` which automatically add remote host key to the known keys and log a warning.
+    ``allow_agent``: Boolean. Optional. Do not use SSH agent if set to ``False``. Default: ``True``.
+    ``look_for_keys``: Boolean. Optional. Do not search for discoverable private keys if set to ``False``. Default: ``True``.
 
     Note:
       - When the ``password`` argument is provided alongside the ``key`` argument then it will be assumed that the provided password is a passphrase for the specified key.
       - The ``missing_host_key_policy`` allow one of the 4 following values:
         - ``auto``: Automatically add remote host key to the known keys.
         - ``warn``: Same as auto and log a warning.
         - ``reject``: Reject the host key, do not proceed to connection and raise an error.
@@ -49,20 +51,23 @@
     if not self.connected:
       self._connect()
     if self.sftp_client is None:
       self.sftp_client = self.client.open_sftp()
     return self.sftp_client
 
   def __init__(self, username, host, port=22,
-               password=None, key=None, missing_host_key_policy="warn"):
+               password=None, key=None, missing_host_key_policy="warn",
+               allow_agent=True, look_for_keys=True):
     self.username = username
     self.host = host
     self.port = port
     self.password = password
     self.key = key
+    self.allow_agent = allow_agent
+    self.look_for_keys = look_for_keys
     self.missing_host_key_policy = missing_host_key_policy
     self.client = None
     self.sftp_client = None
     self._list_local_dir = list_local_dir
     self._delete_local_file = delete_local_file
     self._delete_local_dir = delete_local_dir
     self._create_local_dirs = create_local_dirs
@@ -83,15 +88,17 @@
             self.missing_host_key_policy))
     self.client.load_system_host_keys()
     try:
       self.client.connect(hostname=self.host,
                           port=self.port,
                           username=self.username,
                           password=self.password,
-                          key_filename=self.key)
+                          key_filename=self.key,
+                          allow_agent=self.allow_agent,
+                          look_for_keys=self.look_for_keys)
     except (paramiko.ssh_exception.BadHostKeyException,
             paramiko.ssh_exception.AuthenticationException,
             paramiko.ssh_exception.SSHException,
             socket.error,
             socket.gaierror,
             paramiko.ssh_exception.NoValidConnectionsError) as err:
       raise ScrippyRemoteError(f"[SshConnectionError] {err.__class__.__name__}: {err}") from err
```

### Comparing `scrippy-remote-3.0.0/src/scrippy_remote.egg-info/PKG-INFO` & `scrippy_remote-3.0.1/src/scrippy_remote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrippy-remote
-Version: 3.0.0
+Version: 3.0.1
 Summary: "Client SSH, SFTP et FTP pour le cadriciel Scrippy."
 Home-page: https://codeberg.org/scrippy/scrippy-remote
 Author: Michael Costa, Florent Chevalier
 Author-email: michael.costa@mcos.nc, florent.chevalier.nc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scrippy-remote-3.0.0/src/scrippy_remote.egg-info/SOURCES.txt` & `scrippy_remote-3.0.1/src/scrippy_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrippy-remote-3.0.0/tests/test_cifs_files.py` & `scrippy_remote-3.0.1/tests/test_cifs_files.py`

 * *Files identical despite different names*

### Comparing `scrippy-remote-3.0.0/tests/test_ftp_files.py` & `scrippy_remote-3.0.1/tests/test_ftp_files.py`

 * *Files identical despite different names*

### Comparing `scrippy-remote-3.0.0/tests/test_ssh_files.py` & `scrippy_remote-3.0.1/tests/test_ssh_files.py`

 * *Files identical despite different names*

