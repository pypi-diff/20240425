# Comparing `tmp/scriptonite-0.9.11.tar.gz` & `tmp/scriptonite-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptonite-0.9.11.tar", max compression
+gzip compressed data, was "scriptonite-1.0.0.tar", max compression
```

## Comparing `scriptonite-0.9.11.tar` & `scriptonite-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1006 2024-04-24 07:19:42.027260 scriptonite-0.9.11/README.md
--rw-r--r--   0        0        0      566 2024-04-24 11:07:56.176095 scriptonite-0.9.11/pyproject.toml
--rw-r--r--   0        0        0      132 2024-04-24 10:20:40.388982 scriptonite-0.9.11/scriptonite/__init__.py
--rw-r--r--   0        0        0     6681 2024-04-24 09:46:50.049014 scriptonite-0.9.11/scriptonite/configuration.py
--rw-r--r--   0        0        0     3601 2024-04-24 09:48:01.049660 scriptonite-0.9.11/scriptonite/email.py
--rw-r--r--   0        0        0     4719 2024-04-24 11:01:25.170127 scriptonite-0.9.11/scriptonite/logging.py
--rw-r--r--   0        0        0     2144 2024-04-24 09:48:17.236143 scriptonite-0.9.11/scriptonite/utilities.py
--rw-r--r--   0        0        0     1612 1970-01-01 00:00:00.000000 scriptonite-0.9.11/PKG-INFO
+-rw-r--r--   0        0        0     1006 2024-04-24 07:19:42.027260 scriptonite-1.0.0/README.md
+-rw-r--r--   0        0        0      565 2024-04-25 13:46:08.227814 scriptonite-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-04-24 10:20:40.388982 scriptonite-1.0.0/scriptonite/__init__.py
+-rw-r--r--   0        0        0     6711 2024-04-25 13:24:13.508953 scriptonite-1.0.0/scriptonite/configuration.py
+-rw-r--r--   0        0        0     3684 2024-04-25 13:39:04.091012 scriptonite-1.0.0/scriptonite/email.py
+-rw-r--r--   0        0        0     6219 2024-04-25 13:44:01.026519 scriptonite-1.0.0/scriptonite/logging.py
+-rw-r--r--   0        0        0     2144 2024-04-25 13:24:15.083137 scriptonite-1.0.0/scriptonite/utilities.py
+-rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 scriptonite-1.0.0/PKG-INFO
```

### Comparing `scriptonite-0.9.11/README.md` & `scriptonite-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `scriptonite-0.9.11/pyproject.toml` & `scriptonite-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scriptonite"
-version = "0.9.11"
+version = "1.0.0"
 description = "A toolkit for scripting in Python"
 authors = ["Andrea Mistrali <andrea@mistrali.pw>"]
 maintainers = ["Andrea Mistrali <andrea@mistrali.pw>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `scriptonite-0.9.11/scriptonite/configuration.py` & `scriptonite-1.0.0/scriptonite/configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,43 +8,44 @@
 import yaml
 import os
 import typing as t
 import errno
 from .utilities import dictObj
 
 
-def yaml_load(fd):
+def yaml_load(fd: t.BinaryIO) -> str:
     """
     Utility to load a yaml file
     """
     return yaml.load(fd, Loader=yaml.Loader)
 
 
 class Configuration(dictObj):
+    """
+        Create a configuration, as a dict.
+
+        Can create it from:
+        - a default dict passed at init;
+        - environment variables, prefixed with a specific string;
+        - a yaml or json file;
+    """
 
     def __init__(self,
                  defaults: dict[str, t.Any] = {},
                  env_prefix: str | None = None,
                  configfile: str | None = None,
                  file_loader: t.Callable[[t.IO[t.Any]],
                                          t.Mapping[str, t.Any]] = yaml_load):
         """
-        Create a configuration, as a dict.
-        Can create it from:
-        - a default dict passed at init;
-        - environment variables, prefixed with a specific string;
-        - a yaml or json file;
-
-        Parameters:
-        - **defaults**: a dict of initial values
-        - **env_prefix**: the prefix to use to look up environment variables
-        - **configfile**: a configuration file to read
-        - **file_loader**: the loader to use to parse the config file,
-                       defaults to `yaml_load` function, you can use
-                       `json.load` or `toml.load` to parse other formats
+        :param defaults: a dict of initial values
+        :param env_prefix: the prefix to use to look up environment variables
+        :param configfile: a configuration file to read
+        :param file_loader: the loader to use to parse the config file,
+                            defaults to `yaml_load` function, you can use
+                            `json.load` or `toml.load` to parse other formats
         """
         super().__init__(defaults or {})
 
         if env_prefix:
             self.from_environ(prefix=env_prefix)
 
         if configfile:
@@ -56,22 +57,22 @@
                      loads: t.Callable[[str], t.Any] = json.loads) -> bool:
         """
         Loads configuration parsing environment variables.
         Prefix is the prefix of the variables (that will be stripped).
         Variables can build structures, using `__` as separator
         between the levels.
 
-        Parameters:
-        - **prefix**: the environment prefix
-        - **loads**: a function to parse and normalize environment variables
+        :param prefix: the environment prefix
+        :param loads: a function to parse and normalize environment variables
                  values, best to use is `json.load` that will convert
                  numeric values to numbers and string like "true" or "false"
                  to python boolean
 
         Examples:
+
             - `PREFIX_ANSWER=42` -> `answer`: 42
             - `PREFIX_A__B=1` -> `{'a': {'b': 1}}`
         """
         prefix = f"{prefix}_"
         len_prefix = len(prefix)
 
         for key in sorted(os.environ):
@@ -108,20 +109,20 @@
                   silent: bool = False,
                   text: bool = True,) -> bool:
         """
         Loads and parses a file, updating the config with the content.
         Wants a `load` method to use to parse the file.
 
         Parameters:
-        - **filename**: the file to load
-        - **silent**: do not stop if file does not exist;
-        - **text**: open file as text if True, as binary if False
-        - **load**: a function to parse the file, we have `yaml_load` to load
-                YAML files, you can use `json.load` or `toml.load` to load
-                other formats.
+        :param filename: the file to load
+        :param silent: do not stop if file does not exist;
+        :param text: open file as text if True, as binary if False
+        :param load: a function to parse the file, we have `yaml_load` to load
+                     YAML files, you can use `json.load` or `toml.load` to load
+                     other formats.
 
         Example:
         ```
         conf.from_file('conf.json', load=json.load)
         ```
 
         **NOTE**:
@@ -143,29 +144,31 @@
         return self.from_mapping(obj)
 
     def from_yaml(self,
                   filename: str | os.PathLike[str],
                   silent: bool = False,
                   text: bool = True) -> bool:
         """
-        Syntax sugar to load a YAML file
+        Syntax sugar to load a YAML file.
+
         Parameters are the same as `from_file`, apart for the `load` parameter
         that is hardcoded to `yaml_load`
         """
         return self.from_file(filename,
                               silent=silent,
                               text=text,
                               load=yaml_load)
 
     def from_json(self,
                   filename: str | os.PathLike[str],
                   silent: bool = False,
                   text: bool = True) -> bool:
         """
-        Syntax sugar to load a JSON file
+        Syntax sugar to load a JSON file.
+
         Parameters are the same ad `from_file`, apart for the `load` parameter
         that is hardcoded to `json.load`
         """
         return self.from_file(filename,
                               silent=silent,
                               text=text,
                               load=json.load)
```

### Comparing `scriptonite-0.9.11/scriptonite/email.py` & `scriptonite-1.0.0/scriptonite/email.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-from curses.ascii import EM
+from dataclasses import dataclass
 import smtplib
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.mime.base import MIMEBase
 from email import encoders
-import logging
-
-log = logging.getLogger(__name__)
-log.setLevel(logging.INFO)
 
 
 class EmailMessage:
     """
     An email message.
 
-    Attributes are:
-    - **sender**: the From field of the email
-    - **recipient**: the To field of the email
-    - **subject**: well, the subject of the email
-    - **body**: the text part of the message
-    - **cclist**: a list of email addresses that will receive a copy of the email
     """
 
     def __init__(self, sender: str,
-                 recipient: str,
+                 recipients: list,
                  subject: str,
                  body: str,
                  cclist: list = []):
+        """
+        :param sender: the From field of the email
+        :param recipients: the To field of the email, is a list
+        :param subject: well, the subject of the email
+        :param body: the text part of the message
+        :param cclist: a list of email addresses that will receive
+                       a copy of the email
+
+        To send an email to a single address use
+        `recipient=["recipient@domain"]`
 
+        """
         message = MIMEMultipart()
         message['From'] = sender
-        message['To'] = recipient
+        message['To'] = ",".join(recipients)
         if cclist:
             message['Cc'] = ','.join(cclist)
         message['Subject'] = subject
 
         # Attach body
         message.attach(MIMEText(body, 'plain'))
 
-        self.payload = message
+        self._payload = message
 
     def attach_file(self,
                     attachment: str) -> None:
         """
         Attach a file to the email
 
-        Parameters:
-        - **attachment**: full path to the file to be attached
+        :param attachment: full path to the file to be attached
         """
         with open(attachment, 'rb') as fd:
-            self.payload.attach_data(fd.read(),
-                                     filename=attachment)
+            self._payload.attach_data(fd.read(),
+                                      filename=attachment)
 
-    def attach_data(self, data: bytes,
+    def attach_data(self, stream: bytes,
                     filename: str) -> None:
         """
         Attach a bytes object to the message, useful if you built a file in the
         script and need to send it without having to save it in a
         temporary file
 
-        Parameters:
-        - **data**: the bytes stream that we want to attach
-        - **filename**: the name of the attachment
+        :param stream: the bytes stream that we want to attach
+        :param filename: the name of the attachment
         """
         part = MIMEBase("application", "octet-stream")
-        part.set_payload(data)
+        part.set_payload(stream)
         encoders.encode_base64(part)
         part.add_header("Content-Disposition",
                         f"attachment; filename={filename}")
-        self.payload.attach(part)
+        self._payload.attach(part)
 
 
+@dataclass
 class EmailSender:
     """
     A connector to an SMTP server
-
-    Parameters:
-    - **server**: the server name
-    - **port**: the server port, defaults to 587 (submission)
-    - **username**: the username used to authenticate
-    - **password**: the password used to authenticate
-    - **starttls**: if we want to use STARTTLS
-
-    If username and password are empty authentication will be disabled
     """
 
     def __init__(self, server: str,
                  username: str = "",
                  password: str = "",
                  starttls: bool = True,
                  port: int = 587) -> None:
+        """
+        :param server: the server name
+        :param port: the server port, defaults to 587 (submission)
+        :param username: the username used to authenticate
+        :param password: the password used to authenticate
+        :param starttls: if we want to use STARTTLS
+        :type server: str
+
+        If `username` and `password` are empty authentication will be disabled
+        """
+
         self.server = server
         self.port = port
         self.username = username
         self.password = password
-        self.auth = bool(self.username and self.password)
+        self._auth = bool(self.username and self.password)
         self.starttls = starttls
 
     def send(self, message: EmailMessage) -> None:
         """
         Send an EmailMessage object, built with the above class
         Errors are not trapped and exception will be raised, it is up to the
         calling script to trap them
 
-        Parameters:
-        - **message**: an EmailMessage object
+        :param message: an EmailMessage object
         """
         with smtplib.SMTP(self.server, self.port) as server:
             if self.starttls:
                 server.starttls()  # Enable secure connection
-            if self.auth:
+            if self._auth:
                 server.login(self.username, self.password)
-            server.send_message(message.payload)
-            log.info('Email sent successfully.')
+            server.send_message(message._payload)
```

### Comparing `scriptonite-0.9.11/scriptonite/logging.py` & `scriptonite-1.0.0/scriptonite/logging.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 from functools import singledispatchmethod
+from gzip import FCOMMENT
+from typing import Any
 import datetime
 import logging
 import sys
 
 
 class DeltaTimeFormatter(logging.Formatter):
     """
     adds a `delta` attribute to the record, with the relative
     time since the start of logging
     """
 
-    def format(self, record):
+    def format(self, record: logging.LogRecord) -> str:
         duration = datetime.datetime.fromtimestamp(
             (record.relativeCreated / 1000), datetime.UTC)
         record.delta = duration.strftime("%H:%M:%S.%f")
         return super().format(record)
 
 
 class LogFilter(logging.Filter):
     """
     Filter out some log messages based on qualifier name
-
-    Parameters:
-    - **qualname**: log message qualifier name, the `name` field of the log record
-                can be a a list[str] to silence several qualname in one shot
-
     """
 
-    def __init__(self, qualname: str | list) -> None:
-        self.qualname = qualname
+    def __init__(self, qualname: str) -> None:
+        """
+        :param qualname: log message qualifier name, the `name` field of the
+                         log record. Can be a `str` or a `list of str`
+
+        """
+        self._qualname = qualname
 
     def filter(self, record: logging.LogRecord) -> bool:
-        return not record.name == self.qualname
+        if type(self._qualname) is list:
+            return record.name not in self._qualname
+        else:
+            return record.name != self._qualname
 
 
 class Logger(logging.Logger):
     """
     The root logger, already setup.
     This class creates an instance of the Root Logger already configured to
     write logs to `stderr` in a chosen format.
 
-    It can autodetect if input is a tty (interactive script) and set format to
+    It can autodetect if input is a tty(interactive script) and set format to
     `cli`, i.e. plain, shorter date/time or to `json` format, with full date if
     input is not a tty, for example running from a job
 
-    Parameters:
-    - **level**: the logging level for the root logger;
-    - **format**: the log message format, by the default it is auto-detected
-    - **silence**: one or more qualifier names that we want to silence.
-               This is useful to silence logs from other modules that we use
-               in our script
     """
 
     FORMATS = {
         'json': {
             'format':
             '{ "DateTime": "%(asctime)s", '
             '"Name": "%(name)s", "Filename": "%(filename)s:%(lineno)d", '
@@ -75,21 +74,66 @@
         },
         'color': {
             'format': "\x1b[0;1m%(asctime)s,%(msecs)03d "
                       "\x1b[1;31m%(levelname)-8.8s "
                       "\x1b[1;34m[%(name)s/%(filename)s:%(lineno)d]: "
                       "\x1b[0m%(message)s",
             'datefmt': "%H:%M:%S"
+        },
+        'short': {
+            'format': "%(message)s"
         }
     }
+    """
+    Predefined formats:
+
+    - `json`: JSON message with full date
+    - `cli`: plain text message with short date, just time
+    - `color`: like `cli` but with colored message
+    - `relative`: plain text message with relative time
+    - `short`: just the message
+    """
+
+    @classmethod
+    def addFormat(cls, name: str,
+                  format: str,
+                  datefmt: str,
+                  formatter: Any | None = None) -> None:
+        """
+        Add a new format to the Logger class
+
+        :param name: name of the new format
+        :param format: format string
+        :param datefmt: date format string
+        :param formatter: a custom formatter, can be empty
+
+        for information on the format of `format` and `datefmt` strings, please
+        refer to the following documents:
+        - [Log record attributes](https: // docs.python.org/3/library/logging.html#logrecord-attributes)
+        - [Time formatting](https: // docs.python.org/3/library/time.html#time.strftime)
+        """
+        cls.FORMATS[name] = {
+            'format': format,
+            'datefmt': datefmt
+        }
+
+        if formatter:
+            cls.FORMATS[formatName]['formatter'] = formatter
 
     def __init__(self,
                  level: str | int = logging.INFO,
                  format: str | None = None,
                  silence: str | list | None = None):
+        """
+        :param level: the logging level for the root logger;
+        :param format: the log message format, by the default it is auto-detected
+        :param silence: one or more qualifier names that we want to silence.
+                   This is useful to silence logs from other modules that we use
+                   in our script
+        """
 
         # If the input is a tty use `cli` message format,
         # else use `json`
         if not format:
             # are we running interactively?
             isCli = sys.stdin and sys.stdin.isatty()
             format = "cli" if isCli else "json"
@@ -118,27 +162,27 @@
             self.silence(silence)
 
     @singledispatchmethod
     def silence(self, qualname: str) -> None:
         """
         Silence one qualname or a list of qualnames
 
-        Parameters:
-        - **qualname**: qualifier name to silence
+        :param qualname: one or more qualifier names to silence
+
+        You can pass a `str` or a `list[str]`
         """
         for handler in self._rootLogger.handlers:
             handler.addFilter(LogFilter(qualname))
 
     @silence.register
     def _(self, qualname: list) -> None:
         """
         Silence a list of qualnames
 
-        Parameters:
-        - *qualname**: list of qualifier names to silence
+        :param qualname: list of qualifier names to silence
         """
         for handler in self._rootLogger.handlers:
             for qual in qualname:
                 handler.addFilter(LogFilter(qual))
 
     def __getattr__(self, attr):
         """
```

### Comparing `scriptonite-0.9.11/scriptonite/utilities.py` & `scriptonite-1.0.0/scriptonite/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 
 class dictObj(dict):
     """
     A dict on steroids
     You can access keys as attributes
 
+    :param init: a dict of initial values
+
     Example:
-    c=Config({'a': 1, 'b': 2})
-    c.a == c['a'] -> True
 
-    Parameters:
-    - **init**: a dict of initial values
+        >> c=Config({'a': 1, 'b': 2})
+        >> c.a == c['a'] -> True
     """
 
     def __init__(self, init: dict | None) -> None:
         if init:
             for key, value in init.items():
                 self.__parse_value(key, value)
```

### Comparing `scriptonite-0.9.11/PKG-INFO` & `scriptonite-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriptonite
-Version: 0.9.11
+Version: 1.0.0
 Summary: A toolkit for scripting in Python
 License: GPL-3.0-or-later
 Author: Andrea Mistrali
 Author-email: andrea@mistrali.pw
 Maintainer: Andrea Mistrali
 Maintainer-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0
```

