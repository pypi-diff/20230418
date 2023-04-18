# Comparing `tmp/sett_rs-0.2.2-cp39-none-win_amd64.whl.zip` & `tmp/sett_rs-0.3.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2491197 bytes, number of entries: 8
--rw-r--r--  4.6 unx     1565 b- defN 22-Nov-23 13:46 sett_rs-0.2.2.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 22-Nov-23 13:46 sett_rs-0.2.2.dist-info/WHEEL
--rw-r--r--  4.6 unx     1971 b- defN 22-Nov-23 13:46 sett_rs/pgp.py
--rw-r--r--  4.6 unx        0 b- defN 22-Nov-23 13:46 sett_rs/py.typed
--rw-r--r--  4.6 unx     2612 b- defN 22-Nov-23 13:46 sett_rs/_sett_rs.pyi
--rw-r--r--  4.6 unx      222 b- defN 22-Nov-23 13:46 sett_rs/__init__.py
--rwxr-xr-x  4.6 unx  6241280 b- defN 22-Nov-23 13:46 sett_rs/_sett_rs.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      594 b- defN 22-Nov-23 13:46 sett_rs-0.2.2.dist-info/RECORD
-8 files, 6248339 bytes uncompressed, 2490177 bytes compressed:  60.1%
+Zip file size: 3593553 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     1706 b- defN 23-Apr-18 14:26 sett_rs-0.3.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Apr-18 14:26 sett_rs-0.3.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     2950 b- defN 23-Apr-18 14:26 sett_rs/pgp.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Apr-18 14:26 sett_rs/py.typed
+-rw-r--r--  4.6 unx     3097 b- defN 23-Apr-18 14:26 sett_rs/_sett_rs.pyi
+-rw-r--r--  4.6 unx      236 b- defN 23-Apr-18 14:26 sett_rs/__init__.py
+-rwxr-xr-x  4.6 unx  8604160 b- defN 23-Apr-18 14:26 sett_rs/_sett_rs.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      594 b- defN 23-Apr-18 14:26 sett_rs-0.3.0.dist-info/RECORD
+8 files, 8612839 bytes uncompressed, 3592533 bytes compressed:  58.3%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: sett_rs-0.2.2.dist-info/METADATA
+Filename: sett_rs-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: sett_rs-0.2.2.dist-info/WHEEL
+Filename: sett_rs-0.3.0.dist-info/WHEEL
 Comment: 
 
 Filename: sett_rs/pgp.py
 Comment: 
 
 Filename: sett_rs/py.typed
 Comment: 
@@ -15,11 +15,11 @@
 
 Filename: sett_rs/__init__.py
 Comment: 
 
 Filename: sett_rs/_sett_rs.cp39-win_amd64.pyd
 Comment: 
 
-Filename: sett_rs-0.2.2.dist-info/RECORD
+Filename: sett_rs-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sett_rs/pgp.py

```diff
@@ -1,12 +1,12 @@
 """Python bindings for PGP key related objects in the sett rust crate."""
-
 import os
 from dataclasses import dataclass
-from typing import Tuple
+from datetime import datetime
+from typing import Optional, Tuple, Union
 
 from ._sett_rs import (
     Key as Key,
     KeyType as KeyType,
     UserID as UserID,
     Validity as Validity,
     read_cert,
@@ -35,39 +35,66 @@
     """
 
     uids: Tuple[UserID, ...]
     keys: Tuple[Key, ...]
     validity: Validity
 
     @classmethod
-    def from_bytes(cls, src: bytes) -> "Cert":
+    def from_bytes(
+        cls, src: bytes, end_relax: Union[int, datetime, None] = None
+    ) -> "Cert":
+        if isinstance(end_relax, datetime):
+            end_relax = int(end_relax.timestamp())
         try:
-            c = read_cert(src)
+            c = read_cert(src, end_relax)
         except RuntimeError as e:
             raise KeyParsingError(detail=str(e)) from e
 
         return cls(uids=tuple(c.uids), keys=tuple(c.keys), validity=c.validity)
 
     @classmethod
-    def from_file(cls, src_file: str) -> "Cert":
+    def from_file(
+        cls, src_file: str, end_relax: Union[int, datetime, None] = None
+    ) -> "Cert":
+        if isinstance(end_relax, datetime):
+            end_relax = int(end_relax.timestamp())
         with open(os.path.expanduser(src_file), mode="rb") as f:
-            return cls.from_bytes(src=f.read())
+            return cls.from_bytes(src=f.read(), end_relax=end_relax)
 
     @property
     def primary_key(self) -> Key:
         return self.keys[0]
 
     @property
     def fingerprint(self) -> str:
         return self.primary_key.fingerprint
 
     @property
     def key_id(self) -> str:
         return self.primary_key.key_id
 
     @property
-    def uid(self) -> UserID:
-        return self.uids[0]
+    def uid(self) -> Optional[UserID]:
+        return next(iter(self.uids), None)
 
     @property
     def subkeys(self) -> Tuple[Key, ...]:
         return self.keys[1:]
+
+    @property
+    def name(self) -> Optional[str]:
+        return self.uid.name if self.uid else None
+
+    @property
+    def email(self) -> Optional[str]:
+        return self.uid.email if self.uid else None
+
+    @property
+    def comment(self) -> Optional[str]:
+        return self.uid.comment if self.uid else None
+
+    @property
+    def user_id(self) -> Optional[str]:
+        return str(self.uid) if self.uid else None
+
+    def __str__(self) -> str:
+        return f"{str(self.uid) if self.uid else 'No user ID'} - {self.fingerprint}"
```

## sett_rs/_sett_rs.pyi

```diff
@@ -1,78 +1,95 @@
 """Type hints (stub file) for the classes and functions exported from rust."""
 
 from datetime import datetime
 from enum import Enum
-from typing import Sequence, List, Optional, Callable, Any
+from typing import Sequence, List, Optional, Callable, Any, Union
 
 class SftpOpts:
     host: str
     port: int
     username: str
     destination_dir: str
     envelope_dir: Optional[str]
     pkey: Optional[str]
     pkey_password: Optional[str]
+    buf_size: Optional[int]
 
     def __init__(
         self,
         host: str,
         port: int,
         username: str,
         destination_dir: Optional[str] = None,
         envelope_dir: Optional[str] = None,
         pkey: Optional[str] = None,
         pkey_password: Optional[str] = None,
+        buf_size: Optional[int] = None,
     ) -> None: ...
 
-def sftp_upload(
+class S3Opts:
+    endpoint: str
+    bucket: str
+    region: str
+    profile: Optional[str]
+    access_key: Optional[str]
+    secret_key: Optional[str]
+    session_token: Optional[str]
+
+    def __init__(
+        self,
+        endpoint: str,
+        bucket: str,
+        region: str = "",
+        profile: Optional[str] = None,
+        access_key: Optional[str] = None,
+        secret_key: Optional[str] = None,
+        session_token: Optional[str] = None,
+    ) -> None: ...
+
+def transfer(
     files: Sequence[str],
-    host: str,
-    username: str,
-    destination_dir: str,
-    envelope_dir: Optional[str] = None,
-    pkey: Optional[str] = None,
-    pkey_password: Optional[str] = None,
+    destination: Union[S3Opts, SftpOpts],
     progress: Optional[Callable[[float], Any]] = None,
-    buf_size: Optional[int] = None,
     two_factor_callback: Optional[Callable[[], str]] = None,
 ) -> None: ...
 def encrypt(
     files: Sequence[str],
     recipients: Sequence[str],
     sender: Optional[str],
     password: Optional[str],
-    dry_run: bool,
-    force: bool,
+    dry_run: bool = False,
+    force: bool = False,
     output: Optional[str] = None,
     purpose: Optional[str] = None,
     transfer_id: Optional[int] = None,
     compression_level: Optional[int] = None,
     max_cpu: Optional[int] = None,
     progress: Optional[Callable[[float], Any]] = None,
-    remote: Optional[SftpOpts] = None,
+    remote: Union[S3Opts, SftpOpts, None] = None,
     two_factor_callback: Optional[Callable[[], str]] = None,
 ) -> Optional[str]: ...
 def decrypt(
     file: str,
     recipients: Sequence[str],
     signer: Optional[str],
     password: Optional[str],
-    dry_run: bool,
-    decrypt_only: bool,
+    dry_run: bool = False,
+    decrypt_only: bool = False,
     output: Optional[str] = None,
     max_cpu: Optional[int] = None,
     progress: Optional[Callable[[float], Any]] = None,
 ) -> Optional[str]: ...
 
 class KeyType(Enum):
     Public: Any
     Secret: Any
 
 class Validity(Enum):
+    Condemned: Any
     Expired: Any
     Invalid: Any
     Revoked: Any
     Unknown: Any
     Valid: Any
 
 class UserID:
@@ -94,8 +111,8 @@
 class Cert:
     key_id: str
     fingerprint: str
     uids: List[UserID]
     validity: Validity
     keys: List[Key]
 
-def read_cert(src: bytes) -> Cert: ...
+def read_cert(src: bytes, end_relax: Optional[int]) -> Cert: ...
```

## sett_rs/__init__.py

```diff
@@ -1,9 +1,10 @@
 from ._sett_rs import (
     decrypt as decrypt,
     encrypt as encrypt,
-    sftp_upload as sftp_upload,
+    transfer as transfer,
+    S3Opts as S3Opts,
     SftpOpts as SftpOpts,
 )
 from . import pgp as pgp
 
-__all__ = ["decrypt", "encrypt", "sftp_upload", "pgp"]
+__all__ = ["decrypt", "encrypt", "transfer", "pgp"]
```

## Comparing `sett_rs-0.2.2.dist-info/METADATA` & `sett_rs-0.3.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Metadata-Version: 2.1
 Name: sett_rs
-Version: 0.2.2
-Requires-Dist: pytest; extra == 'dev'
+Version: 0.3.0
+Requires-Dist: pylint==2.17.2; extra == 'dev'
+Requires-Dist: mypy==1.2.0; extra == 'dev'
+Requires-Dist: black==23.3.0; extra == 'dev'
+Requires-Dist: pytest==7.3.0; extra == 'dev'
 Provides-Extra: dev
 Summary: sett-rs Python bindings.
 Author: Gerhard Bräunlich <gerhard.braeunlich@id.ethz.ch>, Christian Ribeaud <christian.ribeaud@karakun.com>, Jarosław Surkont <jaroslaw.surkont@unibas.ch>
 Author-email: Gerhard Bräunlich <gerhard.braeunlich@id.ethz.ch>, Christian Ribeaud <christian.ribeaud@karakun.com>, Jarosław Surkont <jaroslaw.surkont@unibas.ch>
 License: LGPL-3.0-or-later
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://gitlab.com/biomedit/sett-rs
```

