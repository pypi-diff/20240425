# Comparing `tmp/types-pyOpenSSL-24.0.0.20240417.tar.gz` & `tmp/types-pyOpenSSL-24.1.0.20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyOpenSSL-24.0.0.20240417.tar", last modified: Wed Apr 17 02:17:32 2024, max compression
+gzip compressed data, was "types-pyOpenSSL-24.1.0.20240425.tar", last modified: Thu Apr 25 02:19:38 2024, max compression
```

## Comparing `types-pyOpenSSL-24.0.0.20240417.tar` & `types-pyOpenSSL-24.1.0.20240425.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:32.517490 types-pyOpenSSL-24.0.0.20240417/
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:32.517490 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-17 02:16:41.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/SSL.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-04-17 02:16:41.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/crypto.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 02:16:41.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/rand.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 02:16:41.000000 types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-17 02:17:32.517490 types-pyOpenSSL-24.0.0.20240417/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:17:32.517490 types-pyOpenSSL-24.0.0.20240417/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:32.517490 types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 02:17:32.000000 types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:38.030770 types-pyOpenSSL-24.1.0.20240425/
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-25 02:19:37.000000 types-pyOpenSSL-24.1.0.20240425/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 02:19:37.000000 types-pyOpenSSL-24.1.0.20240425/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:38.030770 types-pyOpenSSL-24.1.0.20240425/OpenSSL-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-25 02:19:37.000000 types-pyOpenSSL-24.1.0.20240425/OpenSSL-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-25 02:18:23.000000 types-pyOpenSSL-24.1.0.20240425/OpenSSL-stubs/SSL.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 02:18:23.000000 types-pyOpenSSL-24.1.0.20240425/OpenSSL-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-25 02:18:23.000000 types-pyOpenSSL-24.1.0.20240425/OpenSSL-stubs/crypto.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 02:19:37.000000 types-pyOpenSSL-24.1.0.20240425/OpenSSL-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-25 02:18:23.000000 types-pyOpenSSL-24.1.0.20240425/OpenSSL-stubs/rand.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-25 02:18:23.000000 types-pyOpenSSL-24.1.0.20240425/OpenSSL-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-25 02:19:38.030770 types-pyOpenSSL-24.1.0.20240425/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 02:19:38.030770 types-pyOpenSSL-24.1.0.20240425/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-25 02:19:37.000000 types-pyOpenSSL-24.1.0.20240425/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 02:19:38.030770 types-pyOpenSSL-24.1.0.20240425/types_pyOpenSSL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-25 02:19:37.000000 types-pyOpenSSL-24.1.0.20240425/types_pyOpenSSL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-25 02:19:38.000000 types-pyOpenSSL-24.1.0.20240425/types_pyOpenSSL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 02:19:37.000000 types-pyOpenSSL-24.1.0.20240425/types_pyOpenSSL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-25 02:19:37.000000 types-pyOpenSSL-24.1.0.20240425/types_pyOpenSSL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 02:19:37.000000 types-pyOpenSSL-24.1.0.20240425/types_pyOpenSSL.egg-info/top_level.txt
```

### Comparing `types-pyOpenSSL-24.0.0.20240417/CHANGELOG.md` & `types-pyOpenSSL-24.1.0.20240425/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 24.1.0.20240425 (2024-04-25)
+
+Bump OpenSSL to 24.1.* (#11816)
+
+Mark a few classes and functions as deprecated
+
+Closes: #11812
+
 ## 24.0.0.20240417 (2024-04-17)
 
 Remove remaining bare `Incomplete`s (#11768)
 
 Enable Y065
 
 ## 24.0.0.20240311 (2024-03-11)
```

### Comparing `types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/SSL.pyi` & `types-pyOpenSSL-24.1.0.20240425/OpenSSL-stubs/SSL.pyi`

 * *Files identical despite different names*

### Comparing `types-pyOpenSSL-24.0.0.20240417/OpenSSL-stubs/crypto.pyi` & `types-pyOpenSSL-24.1.0.20240425/OpenSSL-stubs/crypto.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from _typeshed import Incomplete, StrOrBytesPath
 from collections.abc import Callable, Iterable, Sequence
 from datetime import datetime
 from typing import Any
-from typing_extensions import TypeAlias
+from typing_extensions import TypeAlias, deprecated
 
 from cryptography.hazmat.primitives.asymmetric.dsa import DSAPrivateKey, DSAPublicKey
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey, RSAPublicKey
 from cryptography.x509 import Certificate, CertificateRevocationList, CertificateSigningRequest
 
 _Key: TypeAlias = DSAPrivateKey | DSAPublicKey | RSAPrivateKey | RSAPublicKey
 
@@ -94,35 +94,35 @@
     def get_version(self) -> int: ...
     def set_pubkey(self, pkey: PKey) -> None: ...
     def set_version(self, version: int) -> None: ...
     def sign(self, pkey: PKey, digest: str) -> None: ...
     def to_cryptography(self) -> CertificateSigningRequest: ...
     def verify(self, pkey: PKey) -> bool: ...
 
-# deprecated
+@deprecated("X509Extension support in pyOpenSSL is deprecated. You should use the APIs in cryptography.")
 class X509Extension:
     def __init__(
         self, type_name: bytes, critical: bool, value: bytes, subject: X509 | None = None, issuer: X509 | None = None
     ) -> None: ...
     def get_critical(self) -> bool: ...
     def get_data(self) -> bytes: ...
     def get_short_name(self) -> bytes: ...
 
-# deprecated
+@deprecated("CRL support in pyOpenSSL is deprecated. You should use the APIs in cryptography.")
 class Revoked:
     def __init__(self) -> None: ...
     def all_reasons(self) -> list[bytes]: ...
     def get_reason(self) -> bytes | None: ...
     def get_rev_date(self) -> bytes: ...
     def get_serial(self) -> bytes: ...
     def set_reason(self, reason: bytes | None) -> None: ...
     def set_rev_date(self, when: bytes) -> None: ...
     def set_serial(self, hex_str: bytes) -> None: ...
 
-# deprecated
+@deprecated("CRL support in pyOpenSSL is deprecated. You should use the APIs in cryptography.")
 class CRL:
     def __init__(self) -> None: ...
     def add_revoked(self, revoked: Revoked) -> None: ...
     def export(self, cert: X509, key: PKey, type: int = 1, days: int = 100, digest: bytes = ...) -> bytes: ...
     @classmethod
     def from_cryptography(cls, crypto_crl: CertificateRevocationList) -> CRL: ...
     def get_issuer(self) -> X509Name: ...
@@ -162,45 +162,27 @@
     EXPLICIT_POLICY: int
     INHIBIT_MAP: int
     NOTIFY_POLICY: int
     CHECK_SS_SIGNATURE: int
     CB_ISSUER_CHECK: int
     PARTIAL_CHAIN: int
 
-# deprecated
-class PKCS12:
-    def __init__(self) -> None: ...
-    def export(self, passphrase: bytes | None = None, iter: int = 2048, maciter: int = 1) -> bytes: ...
-    def get_ca_certificates(self) -> tuple[X509, ...]: ...
-    def get_certificate(self) -> X509: ...
-    def get_friendlyname(self) -> bytes | None: ...
-    def get_privatekey(self) -> PKey: ...
-    def set_ca_certificates(self, cacerts: Iterable[X509] | None) -> None: ...
-    def set_certificate(self, cert: X509) -> None: ...
-    def set_friendlyname(self, name: bytes | None) -> None: ...
-    def set_privatekey(self, pkey: PKey) -> None: ...
-
-# deprecated
-class NetscapeSPKI:
-    def __init__(self) -> None: ...
-    def b64_encode(self) -> bytes: ...
-    def get_pubkey(self) -> PKey: ...
-    def set_pubkey(self, pkey: PKey) -> None: ...
-    def sign(self, pkey: PKey, digest: str) -> None: ...
-    def verify(self, key: PKey) -> bool: ...
-
 def get_elliptic_curves() -> set[_EllipticCurve]: ...
 def get_elliptic_curve(name: str) -> _EllipticCurve: ...
 def dump_certificate(type: int, cert: X509) -> bytes: ...
 def load_certificate(type: int, buffer: bytes) -> X509: ...
 def dump_certificate_request(type: int, req: X509Req) -> bytes: ...
 def load_certificate_request(type: int, buffer: bytes) -> X509Req: ...
 def dump_privatekey(
     type: int, pkey: PKey, cipher: str | None = None, passphrase: bytes | Callable[[], bytes] | None = None
 ) -> bytes: ...
 def load_privatekey(type: int, buffer: str | bytes, passphrase: bytes | Callable[[], bytes] | None = None) -> PKey: ...
 def dump_publickey(type: int, pkey: PKey) -> bytes: ...
 def load_publickey(type: int, buffer: str | bytes) -> PKey: ...
-def dump_crl(type: int, crl: CRL) -> bytes: ...  # deprecated
-def load_crl(type: int, buffer: str | bytes) -> CRL: ...  # deprecated
+@deprecated("sign() is deprecated. Use the equivalent APIs in cryptography.")
 def sign(pkey: PKey, data: str | bytes, digest: str) -> bytes: ...  # deprecated
+@deprecated("verify() is deprecated. Use the equivalent APIs in cryptography.")
 def verify(cert: X509, signature: bytes, data: str | bytes, digest: str) -> None: ...  # deprecated
+@deprecated("CRL support in pyOpenSSL is deprecated. You should use the APIs in cryptography.")
+def dump_crl(type: int, crl: CRL) -> bytes: ...
+@deprecated("CRL support in pyOpenSSL is deprecated. You should use the APIs in cryptography.")
+def load_crl(type: int, buffer: str | bytes) -> CRL: ...
```

### Comparing `types-pyOpenSSL-24.0.0.20240417/PKG-INFO` & `types-pyOpenSSL-24.1.0.20240425/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyOpenSSL
-Version: 24.0.0.20240417
+Version: 24.1.0.20240425
 Summary: Typing stubs for pyOpenSSL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,20 +22,20 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyOpenSSL`.
 
 This version of `types-pyOpenSSL` aims to provide accurate annotations
-for `pyOpenSSL==24.0.*`.
+for `pyOpenSSL==24.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyOpenSSL. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
```

### Comparing `types-pyOpenSSL-24.0.0.20240417/setup.py` & `types-pyOpenSSL-24.1.0.20240425/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyOpenSSL`.
 
 This version of `types-pyOpenSSL` aims to provide accurate annotations
-for `pyOpenSSL==24.0.*`.
+for `pyOpenSSL==24.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyOpenSSL. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="24.0.0.20240417",
+      version="24.1.0.20240425",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md",
```

### Comparing `types-pyOpenSSL-24.0.0.20240417/types_pyOpenSSL.egg-info/PKG-INFO` & `types-pyOpenSSL-24.1.0.20240425/types_pyOpenSSL.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyOpenSSL
-Version: 24.0.0.20240417
+Version: 24.1.0.20240425
 Summary: Typing stubs for pyOpenSSL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyOpenSSL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,20 +22,20 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyOpenSSL`.
 
 This version of `types-pyOpenSSL` aims to provide accurate annotations
-for `pyOpenSSL==24.0.*`.
+for `pyOpenSSL==24.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyOpenSSL. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `273e9ea6ddc2d5cad2db7dd25a0383a61be15675` and was tested
+with mypy 1.10.0, pyright 1.1.360, and
 pytype 2024.4.11.
```

