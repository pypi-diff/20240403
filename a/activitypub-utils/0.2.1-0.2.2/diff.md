# Comparing `tmp/activitypub-utils-0.2.1.tar.gz` & `tmp/activitypub-utils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activitypub-utils-0.2.1.tar", last modified: Sun Mar 31 15:39:15 2024, max compression
+gzip compressed data, was "activitypub-utils-0.2.2.tar", last modified: Wed Apr  3 17:56:20 2024, max compression
```

## Comparing `activitypub-utils-0.2.1.tar` & `activitypub-utils-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-03-31 15:39:15.109060 activitypub-utils-0.2.1/
--rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2022-11-14 16:23:17.000000 activitypub-utils-0.2.1/LICENSE.md
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1918 2024-03-31 15:39:15.109060 activitypub-utils-0.2.1/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      418 2024-03-27 17:16:45.000000 activitypub-utils-0.2.1/README.md
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-03-31 15:39:15.109060 activitypub-utils-0.2.1/activitypub_utils.egg-info/
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1918 2024-03-31 15:39:15.000000 activitypub-utils-0.2.1/activitypub_utils.egg-info/PKG-INFO
--rw-r--r--   0 zoey      (1000) zoey      (1000)      432 2024-03-31 15:39:15.000000 activitypub-utils-0.2.1/activitypub_utils.egg-info/SOURCES.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-03-31 15:39:15.000000 activitypub-utils-0.2.1/activitypub_utils.egg-info/dependency_links.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)      178 2024-03-31 15:39:15.000000 activitypub-utils-0.2.1/activitypub_utils.egg-info/requires.txt
--rw-r--r--   0 zoey      (1000) zoey      (1000)        8 2024-03-31 15:39:15.000000 activitypub-utils-0.2.1/activitypub_utils.egg-info/top_level.txt
-drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-03-31 15:39:15.109060 activitypub-utils-0.2.1/aputils/
--rw-r--r--   0 zoey      (1000) zoey      (1000)      742 2024-03-28 03:16:55.000000 activitypub-utils-0.2.1/aputils/__init__.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     9847 2024-03-28 02:40:35.000000 activitypub-utils-0.2.1/aputils/algorithms.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     6049 2024-03-27 17:16:45.000000 activitypub-utils-0.2.1/aputils/enums.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)      395 2024-03-27 17:16:45.000000 activitypub-utils-0.2.1/aputils/errors.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)    16530 2024-03-27 17:16:45.000000 activitypub-utils-0.2.1/aputils/message.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)    12459 2024-03-28 00:50:12.000000 activitypub-utils-0.2.1/aputils/misc.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     9218 2024-03-27 17:16:45.000000 activitypub-utils-0.2.1/aputils/objects.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)        0 2024-03-27 17:16:45.000000 activitypub-utils-0.2.1/aputils/py.typed
--rw-r--r--   0 zoey      (1000) zoey      (1000)     4140 2024-03-28 03:37:58.000000 activitypub-utils-0.2.1/aputils/request_classes.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     9891 2024-03-28 02:51:00.000000 activitypub-utils-0.2.1/aputils/signer.py
--rw-r--r--   0 zoey      (1000) zoey      (1000)     1976 2024-03-28 01:09:45.000000 activitypub-utils-0.2.1/pyproject.toml
--rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-03-31 15:39:15.109060 activitypub-utils-0.2.1/setup.cfg
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-03 17:56:20.362771 activitypub-utils-0.2.2/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    24909 2022-11-14 16:23:17.000000 activitypub-utils-0.2.2/LICENSE.md
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1944 2024-04-03 17:56:20.362771 activitypub-utils-0.2.2/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      418 2024-03-27 17:16:45.000000 activitypub-utils-0.2.2/README.md
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-03 17:56:20.358771 activitypub-utils-0.2.2/activitypub_utils.egg-info/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1944 2024-04-03 17:56:20.000000 activitypub-utils-0.2.2/activitypub_utils.egg-info/PKG-INFO
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      452 2024-04-03 17:56:20.000000 activitypub-utils-0.2.2/activitypub_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        1 2024-04-03 17:56:20.000000 activitypub-utils-0.2.2/activitypub_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      178 2024-04-03 17:56:20.000000 activitypub-utils-0.2.2/activitypub_utils.egg-info/requires.txt
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        8 2024-04-03 17:56:20.000000 activitypub-utils-0.2.2/activitypub_utils.egg-info/top_level.txt
+drwxr-xr-x   0 zoey      (1000) zoey      (1000)        0 2024-04-03 17:56:20.358771 activitypub-utils-0.2.2/aputils/
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      742 2024-04-03 17:18:25.000000 activitypub-utils-0.2.2/aputils/__init__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     9467 2024-04-03 17:43:36.000000 activitypub-utils-0.2.2/aputils/__main__.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     9997 2024-04-03 15:10:57.000000 activitypub-utils-0.2.2/aputils/algorithms.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     6095 2024-03-31 15:43:20.000000 activitypub-utils-0.2.2/aputils/enums.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)      395 2024-03-27 17:16:45.000000 activitypub-utils-0.2.2/aputils/errors.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    16530 2024-03-27 17:16:45.000000 activitypub-utils-0.2.2/aputils/message.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)    12394 2024-04-03 15:56:22.000000 activitypub-utils-0.2.2/aputils/misc.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     9208 2024-03-31 15:45:56.000000 activitypub-utils-0.2.2/aputils/objects.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)        0 2024-03-27 17:16:45.000000 activitypub-utils-0.2.2/aputils/py.typed
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     4140 2024-03-28 03:37:58.000000 activitypub-utils-0.2.2/aputils/request_classes.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     9975 2024-03-31 15:44:34.000000 activitypub-utils-0.2.2/aputils/signer.py
+-rw-r--r--   0 zoey      (1000) zoey      (1000)     1996 2024-04-03 15:11:20.000000 activitypub-utils-0.2.2/pyproject.toml
+-rw-r--r--   0 zoey      (1000) zoey      (1000)       38 2024-04-03 17:56:20.362771 activitypub-utils-0.2.2/setup.cfg
```

### Comparing `activitypub-utils-0.2.1/LICENSE.md` & `activitypub-utils-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `activitypub-utils-0.2.1/PKG-INFO` & `activitypub-utils-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: activitypub-utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: Various classes and functions for ActivityPub servers
-Author-email: Izalia Mae <admin@barkshark.xyz>
+Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Homepage, https://git.barkshark.xyz/barkshark/aputils
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/aputils/issues
 Project-URL: Documentation, https://docs.barkshark.xyz/aputils
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/aputils
 Keywords: python module
 Platform: any
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pycryptodome==3.19.0
 Provides-Extra: docs
 Requires-Dist: furo==2024.1.29; extra == "docs"
 Requires-Dist: sphinx==7.2.6; extra == "docs"
```

### Comparing `activitypub-utils-0.2.1/activitypub_utils.egg-info/PKG-INFO` & `activitypub-utils-0.2.2/activitypub_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: activitypub-utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: Various classes and functions for ActivityPub servers
-Author-email: Izalia Mae <admin@barkshark.xyz>
+Author-email: Zoey Mae <admin@barkshark.xyz>
 License: CNPL 7+
 Project-URL: Homepage, https://git.barkshark.xyz/barkshark/aputils
 Project-URL: Bug Tracker, https://git.barkshark.xyz/barkshark/aputils/issues
 Project-URL: Documentation, https://docs.barkshark.xyz/aputils
 Project-URL: Source Code, https://git.barkshark.xyz/barkshark/aputils
 Keywords: python module
 Platform: any
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pycryptodome==3.19.0
 Provides-Extra: docs
 Requires-Dist: furo==2024.1.29; extra == "docs"
 Requires-Dist: sphinx==7.2.6; extra == "docs"
```

### Comparing `activitypub-utils-0.2.1/aputils/__init__.py` & `activitypub-utils-0.2.2/aputils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 from .algorithms import Algorithm, HS2019, RsaSha256
 from .algorithms import get as get_algorithm, register as register_algorithm
 from .errors import InvalidKeyError, SignatureFailureError
 from .message import Attachment, Message, Property
 from .misc import Digest, HttpDate, JsonBase, MessageDate, Signature
 from .objects import HostMeta, HostMetaJson, Nodeinfo, Webfinger, WellKnownNodeinfo
```

### Comparing `activitypub-utils-0.2.1/aputils/algorithms.py` & `activitypub-utils-0.2.2/aputils/algorithms.py`

 * *Files 2% similar despite different names*

```diff
@@ -343,15 +343,20 @@
 		headers = {key.lower(): value for key, value in headers.items()}
 		headers["(request-target)"] = f"{method.lower()} {path}"
 
 		if signature.created is not None:
 			headers["(created)"] = str(signature.created)
 
 		if signature.expires is not None:
-			if signature.expires_date > HttpDate.new_utc():
+			current = HttpDate.new_utc()
+
+			if signature.created_date > current:
+				raise SignatureFailureError("Signature creation date is in the future")
+
+			if signature.expires_date < HttpDate.new_utc():
 				raise SignatureFailureError("Signature has expired")
 
 			headers["(expires)"] = str(signature.expires)
 
 		return headers
```

### Comparing `activitypub-utils-0.2.1/aputils/enums.py` & `activitypub-utils-0.2.2/aputils/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 import enum
 import typing
 
 if typing.TYPE_CHECKING:
 	from collections.abc import Sequence
 	from typing import Any
 
-	Self = typing.TypeVar("Self", bound="Enum")
+	try:
+		from typing import Self
+
+	except ImportError:
+		from typing_extensions import Self
 
 
 class classproperty(property):
 	def __get__(self, owner_self: Any, owner_cls: type | None = None) -> Any:
 		return self.fget(owner_cls) # type: ignore
```

### Comparing `activitypub-utils-0.2.1/aputils/message.py` & `activitypub-utils-0.2.2/aputils/message.py`

 * *Files identical despite different names*

### Comparing `activitypub-utils-0.2.1/aputils/misc.py` & `activitypub-utils-0.2.2/aputils/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import base64
 import json
 import typing
 
+from Crypto.Hash import SHA256, SHA512
 from datetime import datetime, timezone
 from functools import wraps
-from Crypto.Hash import SHA256, SHA512
+from typing import Any
 
 from .enums import AlgorithmType
 
 if typing.TYPE_CHECKING:
 	from collections.abc import Callable, Sequence
 	from datetime import tzinfo
-	from typing import Any
 
 	try:
 		from typing import Self
 
 	except ImportError:
 		from typing_extensions import Self
 
@@ -91,17 +91,17 @@
 		if isinstance(value, (dict, str, bytes)):
 			return self.validate(value)
 
 		raise TypeError(f"Cannot compare '{type(value).__name__}' to 'Digest'")
 
 
 	@classmethod
-	def new(cls: type[Digest],
+	def new(cls: type[Self],
 			body: dict[str, Any] | str | bytes,
-			size: int = 256) -> Digest:
+			size: int = 256) -> Self:
 		"""
 			Generate a new body digest
 
 			:param body: Message body to hash
 			:param size: SHA hash size
 		"""
 
@@ -117,15 +117,15 @@
 		raw_hash = HASHES[f"sha{size}"].new(data=body)
 		digest = base64.b64encode(raw_hash.digest()).decode("utf-8")
 
 		return cls(digest, f"SHA-{size}")
 
 
 	@classmethod
-	def parse(cls: type[Digest], digest: str | None) -> Digest | None:
+	def parse(cls: type[Self], digest: str | None) -> Self | None:
 		"""
 			Create a new digest from a digest header
 
 			:param digest: Digest header
 		"""
 
 		if not digest:
@@ -133,15 +133,15 @@
 
 		alg, digest = digest.split("=", 1)
 		return cls(digest, alg)
 
 
 	@classmethod
 	@deprecated("Digest.parse", "0.1.9", "0.3.0")
-	def new_from_digest(cls: type[Digest], digest: str | None) -> Digest | None:
+	def new_from_digest(cls: type[Self], digest: str | None) -> Self | None:
 		"""
 			Create a new digest from a digest header
 
 			:param digest: Digest header
 		"""
 
 		return cls.parse(digest)
@@ -174,35 +174,35 @@
 class HttpDate(datetime):
 	"Datetime object with convenience methods for parsing and creating HTTP date strings"
 
 	FORMAT: str = "%a, %d %b %Y %H:%M:%S GMT"
 	"Format to pass to datetime when (de)serializing a raw HTTP date"
 
 
-	def __new__(cls: type[HttpDate],
+	def __new__(cls: type[Self],
 				year: int,
 				month: int,
 				day: int,
 				hour: int = 0,
 				minute: int = 0,
 				second: int = 0,
 				microsecond: int = 0,
-				tzinfo: tzinfo = timezone.utc) -> HttpDate:
+				tzinfo: tzinfo = timezone.utc) -> Self:
 
 		return datetime.__new__(
 			cls, year, month, day, hour, minute, second, microsecond, tzinfo
 		)
 
 
 	def __str__(self) -> str:
 		return self.to_string()
 
 
 	@classmethod
-	def parse(cls: type[HttpDate], date: str | int | float) -> HttpDate:
+	def parse(cls: type[Self], date: str | int | float) -> Self:
 		"""
 			Parse a unix timestamp or HTTP date in string format
 
 			:param date: Unix timestamp or string from an HTTP Date header
 		"""
 
 		if isinstance(date, (int | float)):
@@ -211,40 +211,40 @@
 		else:
 			data = cls.strptime(date, cls.FORMAT)
 
 		return data.replace(tzinfo=timezone.utc)
 
 
 	@classmethod
-	def new_from_datetime(cls: type[HttpDate], date: datetime) -> HttpDate:
+	def new_from_datetime(cls: type[Self], date: datetime) -> Self:
 		"""
 			Create a new ``HttpDate`` object from a ``datetime`` object
 
 			:param date: ``datetime`` object to convert
 		"""
 		return cls.fromisoformat(date.isoformat())
 
 
 	@classmethod
-	def new_utc(cls: type[HttpDate]) -> HttpDate:
+	def new_utc(cls: type[Self]) -> Self:
 		"Create a new ``HttpDate`` object from the current UTC time"
 		return cls.now(timezone.utc)
 
 
 	def timestamp(self) -> int:
 		"Return the date as a unix timestamp without microseconds"
 		return int(datetime.timestamp(self))
 
 
 	def to_string(self) -> str:
 		"Create an HTTP Date header string from the datetime object"
 		return self.strftime(self.FORMAT)
 
 
-class JsonBase(dict):
+class JsonBase(dict[str, Any]):
 	"A ``dict`` with methods to convert to JSON and back"
 
 	@classmethod
 	@deprecated("JsonBase.parse", "0.1.5", "0.2.0")
 	def new_from_json(cls: type[Self], data: str | bytes | dict | Self) -> Self:
 		"""
 			Parse a JSON object
@@ -384,15 +384,15 @@
 		}
 
 		str_data = ", ".join(f"{key}={value}" for key, value in data.items())
 		return f"Signature({str_data})"
 
 
 	@classmethod
-	def new_from_headers(cls: type[Signature], headers: dict[str, str]) -> Signature:
+	def new_from_headers(cls: type[Self], headers: dict[str, str]) -> Self:
 		"""
 			Parse the signature from a header dict
 
 			:param dict[str,str] headers: Header key/value pairs
 			:raises KeyError: When the signature header(s) cannot be found
 			:raises NotImplementedError: When a newer unsupported signature standard is provided
 		"""
@@ -409,27 +409,27 @@
 			key, value = chunk.split("=", 1)
 			data[key.lower()] = value.strip("\"")
 
 		return cls(**data) # type: ignore
 
 
 	@classmethod
-	def parse(cls: type[Signature], data: str) -> Signature:
+	def parse(cls: type[Self], data: str) -> Self:
 		"""
 			Parse a Signature in string format
 
 			:param str string: Signature string
 		"""
 
 		return cls.new_from_headers({"signature": data})
 
 
 	@classmethod
 	@deprecated("Signature.parse", "0.1.9", "0.3.0")
-	def new_from_signature(cls: type[Signature], string: str) -> Signature:
+	def new_from_signature(cls: type[Self], string: str) -> Self:
 		"""
 			Parse a Signature header
 
 			:param str string: Signature header string
 		"""
 
 		return cls.new_from_headers({"signature": string})
```

### Comparing `activitypub-utils-0.2.1/aputils/objects.py` & `activitypub-utils-0.2.2/aputils/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 	NodeinfoServiceOutbound,
 	NodeinfoVersion
 )
 
 if typing.TYPE_CHECKING:
 	from typing import Any
 
+	try:
+		from typing import Self
+
+	except ImportError:
+		from typing_extensions import Self
+
 
 class NewWebFingerType(typing.TypedDict):
 	subject: str
 	aliases: list[str]
 	links: list[dict[str, str]]
 
 
@@ -30,20 +36,20 @@
 	usage: dict[str, int | dict[str, int]]
 	metadata: dict[str, Any] | None
 
 
 class HostMeta(str):
 	"An object that represents the ``/.well-known/host-meta`` endpoint"
 
-	def __new__(cls: type[HostMeta], data: str) -> HostMeta:
+	def __new__(cls: type[Self], data: str) -> Self:
 		return str.__new__(cls, data)
 
 
 	@classmethod
-	def new(cls: type[HostMeta], domain: str) -> HostMeta:
+	def new(cls: type[Self], domain: str) -> Self:
 		"""
 			Generate a new host-meta xml string
 
 			:param domain: Domain to use for the template url
 		"""
 		return cls(f"""<?xml version="1.0" encoding="UTF-8">
 <XRD xmlns="http://docs.oasis-open.org/ns/xri/xrd-1.0">
@@ -51,15 +57,15 @@
 </XRD>""")
 
 
 class HostMetaJson(JsonBase):
 	"An object that represents the ``/.well-known/host-meta.json`` endpoint"
 
 	@classmethod
-	def new(cls: type[HostMetaJson], domain: str) -> HostMetaJson:
+	def new(cls: type[Self], domain: str) -> Self:
 		"""
 			Generate a new host-meta dict
 
 			:param domain: Domain to use for the template url
 		"""
 		return cls({
 			"links": [
@@ -71,29 +77,29 @@
 		})
 
 
 class Nodeinfo(JsonBase):
 	"An object that represents a nodeinfo endpoint"
 
 	@classmethod
-	def new(cls: type[Nodeinfo],  # pylint: disable=too-many-locals,too-many-arguments
+	def new(cls: type[Self],  # pylint: disable=too-many-locals,too-many-arguments
 			name: str,
 			version: str,
 			protocols: list[NodeinfoProtocol | str] | str | None = None,
 			insrv: list[NodeinfoServiceInbound | str] | None = None,
 			outsrv: list[NodeinfoServiceOutbound | str] | None = None,
 			metadata: dict[str, Any] | None = None,
 			repo: str | None = None,
 			homepage: str | None = None,
 			open_regs: bool = True,
 			users: int = 0,
 			halfyear: int = 0,
 			month: int = 0,
 			posts: int = 0,
-			comments: int = 0) -> Nodeinfo:
+			comments: int = 0) -> Self:
 		"""
 			Create a new nodeinfo object. It will default to version 2.0 if ``repo`` and ``homeage``
 			are not set.
 
 			:param name: Software name to use. Can only include lowercase letters and "-", "_"
 				characters.
 			:param version: Version of the software.
@@ -181,20 +187,20 @@
 
 
 class Webfinger(JsonBase):
 	"An object that represents the ``/.well-known/webfinger`` endpoint"
 
 
 	@classmethod
-	def new(cls: type[Webfinger],
+	def new(cls: type[Self],
 			handle: str,
 			domain: str,
 			actor: str,
 			profile: str | None = None,
-			interaction: str | None = None) -> Webfinger:
+			interaction: str | None = None) -> Self:
 		"""
 			Create a new webfinger object
 
 			:param handle: Username of the account
 			:param domain: Domain the account resides on
 			:param actor: URL that points to the ActivityPub Actor of the account
 			:param profile: URL that points to an HTML representation of the account
@@ -277,17 +283,17 @@
 		raise KeyError(link_type)
 
 
 class WellKnownNodeinfo(JsonBase):
 	"An object that represents the ``/.well-known/nodeinfo`` endpoint"
 
 	@classmethod
-	def new(cls: type[WellKnownNodeinfo],
+	def new(cls: type[Self],
 			v20: str | None = None,
-			v21: str | None = None) -> WellKnownNodeinfo:
+			v21: str | None = None) -> Self:
 		"""
 			Create a new ``WellKnownNodeinfo`` object by specifying the url(s)
 
 			:param v20: URL pointing to a nodeinfo v2.0 object
 			:param v21: Url pointing to a nodeinfo v2.1 object
 		"""
 
@@ -308,19 +314,19 @@
 				"href": v21
 			})
 
 		return cls({"links": data})
 
 
 	@classmethod
-	def new_template(cls: type[WellKnownNodeinfo],
+	def new_template(cls: type[Self],
 					domain: str,
 					path: str = "/nodeinfo",
 					v20: bool = True,
-					v21: bool = True) -> WellKnownNodeinfo:
+					v21: bool = True) -> Self:
 		"""
 			Create a new ``WellKnownNodeinfo`` object by specifying the domain, path, and which
 			versions to include.
 
 			:param domain: Domain to use for urls
 			:param path: Base path for urls
 			:param v20: If true, generate a Nodeinfo v2.0 url
```

### Comparing `activitypub-utils-0.2.1/aputils/request_classes.py` & `activitypub-utils-0.2.2/aputils/request_classes.py`

 * *Files identical despite different names*

### Comparing `activitypub-utils-0.2.1/aputils/signer.py` & `activitypub-utils-0.2.2/aputils/signer.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 from .misc import Signature, deprecated
 from .request_classes import SIGNERS, VALIDATORS
 
 if typing.TYPE_CHECKING:
 	from collections.abc import Callable
 	from typing import Any
 
+	try:
+		from typing import Self
+
+	except ImportError:
+		from typing_extensions import Self
+
 try:
 	from aiohttp.web import BaseRequest as AiohttpRequest
 
 except ImportError:
 	AiohttpRequest = None # type: ignore
 
 
@@ -112,18 +118,18 @@
 				msg = "Key must be an RsaKey, EccKey, Path, or a string representation of a key"
 				raise TypeError(msg)
 
 		object.__setattr__(self, key, value)
 
 
 	@classmethod
-	def new(cls: type[Signer],
+	def new(cls: type[Self],
 			keyid: str,
 			keytype: KeyType = KeyType.RSA,
-			size: int = 4096) -> Signer:
+			size: int = 4096) -> Self:
 		"""
 			Create a new signer with a generated ``RsaKey`` of the specified size
 
 			:param keyid: Url to a web resource which hosts the public key
 			:param keytype: Type of private key to generate
 			:param size: Size of RSA key in bits to generate. This is ignore for ECC keys.
 		"""
@@ -136,15 +142,15 @@
 		if keytype == KeyType.ECC:
 			return cls(ECC.generate(curve="Ed25519"), keyid)
 
 		raise TypeError(f"Invalid key type: {keytype}")
 
 
 	@classmethod
-	def new_from_actor(cls: type[Signer], actor: dict[str, Any]) -> Signer:
+	def new_from_actor(cls: type[Self], actor: dict[str, Any]) -> Self:
 		"""
 			Create a signer object from an ActivityPub actor dict
 
 			:param dict actor: ActivityPub Actor object
 		"""
 
 		return cls(actor["publicKey"]["publicKeyPem"], actor["publicKey"]["id"])
```

### Comparing `activitypub-utils-0.2.1/pyproject.toml` & `activitypub-utils-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["setuptools >= 38.3.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "activitypub-utils"
-authors = [{name = "Izalia Mae", email = "admin@barkshark.xyz"}]
+authors = [{name = "Zoey Mae", email = "admin@barkshark.xyz"}]
 description = "Various classes and functions for ActivityPub servers"
 license = {text = "CNPL 7+"}
 keywords = ["python module"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries :: Python Modules",
+    "Typing :: Typed"
 ]
 requires-python = ">= 3.8"
 dependencies = ["pycryptodome == 3.19.0"]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
```

