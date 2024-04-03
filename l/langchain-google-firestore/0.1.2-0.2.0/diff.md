# Comparing `tmp/langchain_google_firestore-0.1.2-py3-none-any.whl.zip` & `tmp/langchain_google_firestore-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 24825 bytes, number of entries: 18
--rw-r--r--  2.0 unx      898 b- defN 24-Mar-27 17:59 langchain_google_firestore/__init__.py
--rw-r--r--  2.0 unx     2956 b- defN 24-Mar-27 17:59 langchain_google_firestore/chat_message_history.py
--rw-r--r--  2.0 unx     1288 b- defN 24-Mar-27 17:59 langchain_google_firestore/common.py
--rw-r--r--  2.0 unx     4081 b- defN 24-Mar-27 17:59 langchain_google_firestore/document_converter.py
--rw-r--r--  2.0 unx     8042 b- defN 24-Mar-27 17:59 langchain_google_firestore/document_loader.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Mar-27 17:59 langchain_google_firestore/py.typed
--rw-r--r--  2.0 unx      597 b- defN 24-Mar-27 17:59 langchain_google_firestore/version.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-27 17:59 tests/__init__.py
--rw-r--r--  2.0 unx      705 b- defN 24-Mar-27 17:59 tests/conftest.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-27 17:59 tests/unit_tests/__init__.py
--rw-r--r--  2.0 unx     4874 b- defN 24-Mar-27 17:59 tests/unit_tests/test_chat_message_history.py
--rw-r--r--  2.0 unx    12831 b- defN 24-Mar-27 17:59 tests/unit_tests/test_document_converter.py
--rw-r--r--  2.0 unx    11531 b- defN 24-Mar-27 17:59 tests/unit_tests/test_document_loader.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-Mar-27 18:01 langchain_google_firestore-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    17681 b- defN 24-Mar-27 18:01 langchain_google_firestore-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-27 18:01 langchain_google_firestore-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       33 b- defN 24-Mar-27 18:01 langchain_google_firestore-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1693 b- defN 24-Mar-27 18:01 langchain_google_firestore-0.1.2.dist-info/RECORD
-18 files, 78660 bytes uncompressed, 21969 bytes compressed:  72.1%
+Zip file size: 30491 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      920 b- defN 24-Apr-03 18:53 langchain_google_firestore/__init__.py
+-rw-r--r--  2.0 unx     2941 b- defN 24-Apr-03 18:53 langchain_google_firestore/chat_message_history.py
+-rw-r--r--  2.0 unx     1309 b- defN 24-Apr-03 18:53 langchain_google_firestore/common.py
+-rw-r--r--  2.0 unx     4703 b- defN 24-Apr-03 18:53 langchain_google_firestore/document_converter.py
+-rw-r--r--  2.0 unx     8020 b- defN 24-Apr-03 18:53 langchain_google_firestore/document_loader.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-03 18:53 langchain_google_firestore/py.typed
+-rw-r--r--  2.0 unx    12399 b- defN 24-Apr-03 18:53 langchain_google_firestore/vectorstores.py
+-rw-r--r--  2.0 unx      597 b- defN 24-Apr-03 18:53 langchain_google_firestore/version.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 18:53 tests/__init__.py
+-rw-r--r--  2.0 unx     4874 b- defN 24-Apr-03 18:53 tests/test_chat_message_history.py
+-rw-r--r--  2.0 unx    16924 b- defN 24-Apr-03 18:53 tests/test_document_converter.py
+-rw-r--r--  2.0 unx    12105 b- defN 24-Apr-03 18:53 tests/test_document_loader.py
+-rw-r--r--  2.0 unx    14315 b- defN 24-Apr-03 18:53 tests/test_vectorstores.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-Apr-03 18:55 langchain_google_firestore-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17675 b- defN 24-Apr-03 18:55 langchain_google_firestore-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 18:55 langchain_google_firestore-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       33 b- defN 24-Apr-03 18:55 langchain_google_firestore-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1689 b- defN 24-Apr-03 18:55 langchain_google_firestore-0.2.0.dist-info/RECORD
+18 files, 109954 bytes uncompressed, 27655 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -12,44 +12,44 @@
 
 Filename: langchain_google_firestore/document_loader.py
 Comment: 
 
 Filename: langchain_google_firestore/py.typed
 Comment: 
 
-Filename: langchain_google_firestore/version.py
+Filename: langchain_google_firestore/vectorstores.py
 Comment: 
 
-Filename: tests/__init__.py
+Filename: langchain_google_firestore/version.py
 Comment: 
 
-Filename: tests/conftest.py
+Filename: tests/__init__.py
 Comment: 
 
-Filename: tests/unit_tests/__init__.py
+Filename: tests/test_chat_message_history.py
 Comment: 
 
-Filename: tests/unit_tests/test_chat_message_history.py
+Filename: tests/test_document_converter.py
 Comment: 
 
-Filename: tests/unit_tests/test_document_converter.py
+Filename: tests/test_document_loader.py
 Comment: 
 
-Filename: tests/unit_tests/test_document_loader.py
+Filename: tests/test_vectorstores.py
 Comment: 
 
-Filename: langchain_google_firestore-0.1.2.dist-info/LICENSE
+Filename: langchain_google_firestore-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_firestore-0.1.2.dist-info/METADATA
+Filename: langchain_google_firestore-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_firestore-0.1.2.dist-info/WHEEL
+Filename: langchain_google_firestore-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_firestore-0.1.2.dist-info/top_level.txt
+Filename: langchain_google_firestore-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_firestore-0.1.2.dist-info/RECORD
+Filename: langchain_google_firestore-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_firestore/__init__.py

```diff
@@ -8,18 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from langchain_google_firestore.chat_message_history import FirestoreChatMessageHistory
-from langchain_google_firestore.document_loader import FirestoreLoader, FirestoreSaver
-
+from .chat_message_history import FirestoreChatMessageHistory
+from .document_loader import FirestoreLoader, FirestoreSaver
+from .vectorstores import FirestoreVectorStore
 from .version import __version__
 
 __all__ = [
-    "__version__",
     "FirestoreChatMessageHistory",
     "FirestoreLoader",
     "FirestoreSaver",
+    "FirestoreVectorStore",
+    "__version__",
 ]
```

## langchain_google_firestore/chat_message_history.py

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import json
-from typing import TYPE_CHECKING, Any, Iterator, List, Optional
+from typing import TYPE_CHECKING, List, Optional
 
 from google.cloud import firestore  # type: ignore
 from langchain_core.chat_history import BaseChatMessageHistory
 from langchain_core.messages import BaseMessage, messages_from_dict
 
 from .common import client_with_user_agent  # type: ignore
 from .version import __version__
@@ -41,15 +41,15 @@
         """Chat Message History for Google Cloud Firestore.
         Args:
             session_id: Arbitrary key that is used to store the messages of a single
                 chat session. This is the document_path of a document.
             collection: The single `/`-delimited path to a Firestore collection.
             client: Client for interacting with the Google Cloud Firestore API.
         """
-        self.client = client_with_user_agent(client, USER_AGENT)
+        self.client = client_with_user_agent(USER_AGENT, client)
         self.session_id = session_id
         self.doc_ref = self.client.collection(collection).document(session_id)
         self.messages: List[BaseMessage] = []
         self._load_messages()
 
     def _load_messages(self) -> None:
         doc = self.doc_ref.get()
```

## langchain_google_firestore/common.py

```diff
@@ -8,27 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Optional
+
 from google.cloud import firestore  # type: ignore
 from google.cloud.firestore_v1.services.firestore.transports.base import (  # type: ignore
     DEFAULT_CLIENT_INFO,
 )
 
 
 def client_with_user_agent(
-    client: firestore.Client | None, user_agent: str
+    user_agent: str, client: Optional[firestore.Client] = None
 ) -> firestore.Client:
     client_info = DEFAULT_CLIENT_INFO
     client_info.user_agent = user_agent
     if not client:
         client = firestore.Client(client_info=client_info)
     client_agent = client._client_info.user_agent
     if not client_agent:
         client._client_info.user_agent = user_agent
     elif user_agent not in client_agent:
         client._client_info.user_agent = " ".join([user_agent, client_agent])
     return client
-    return client
```

## langchain_google_firestore/document_converter.py

```diff
@@ -11,43 +11,50 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import json
-from typing import TYPE_CHECKING, Any, List
+from typing import TYPE_CHECKING, Any, List, Optional
 
 from google.cloud.firestore import DocumentReference, GeoPoint  # type: ignore
+from google.cloud.firestore_v1.vector import Vector  # type: ignore
 from langchain_core.documents import Document
 
 if TYPE_CHECKING:
-    from google.cloud.firestore import Client, DocumentReference, DocumentSnapshot
+    from google.cloud.firestore import Client, DocumentSnapshot
 
 
 FIRESTORE_TYPE = "firestore_type"
 DOC_REF = "document_reference"
 GEOPOINT = "geopoint"
+VECTOR = "vector"
 
 
 def convert_firestore_document(
     document: DocumentSnapshot,
-    page_content_fields: List[str] = [],
-    metadata_fields: List[str] = [],
+    page_content_fields: Optional[List[str]] = None,
+    metadata_fields: Optional[List[str]] = None,
 ) -> Document:
     data_doc = document.to_dict()
     metadata = {
         "reference": {
             "path": document.reference.path,
             FIRESTORE_TYPE: DOC_REF,
         }
     }
 
+    # Check for vector fields and move them from the data_doc to the metadata
+    vector_keys = [k for k in data_doc if isinstance(data_doc[k], Vector)]
+    for k in vector_keys:
+        metadata[k] = _convert_from_firestore(data_doc.pop(k))
+
     set_page_fields = set(
-        page_content_fields or (data_doc.keys() - set(metadata_fields))
+        page_content_fields or (data_doc.keys() - set(metadata_fields or []))
     )
     set_metadata_fields = set(metadata_fields or (data_doc.keys() - set_page_fields))
 
     page_content = {}
 
     for k in sorted(set_metadata_fields):
         if k in data_doc:
@@ -100,26 +107,33 @@
         }
     elif isinstance(val, GeoPoint):
         val_converted = {
             "latitude": val.latitude,
             "longitude": val.longitude,
             FIRESTORE_TYPE: GEOPOINT,
         }
+    elif isinstance(val, Vector):
+        vector_map = val.to_map_value()
+        val_converted = {
+            "values": list(vector_map["value"]),
+            FIRESTORE_TYPE: VECTOR,
+        }
 
     return val_converted
 
 
 def _convert_from_langchain(val: Any, client: Client) -> Any:
     val_converted = val
     if isinstance(val, list):
         val_converted = [_convert_from_langchain(v, client) for v in val]
     elif isinstance(val, dict):
-        l = len(val)
         if val.get(FIRESTORE_TYPE) == DOC_REF:
             val_converted = DocumentReference(*val["path"].split("/"), client=client)
         elif val.get(FIRESTORE_TYPE) == GEOPOINT:
             val_converted = GeoPoint(val["latitude"], val["longitude"])
+        elif val.get(FIRESTORE_TYPE) == VECTOR:
+            val_converted = Vector(val["values"])
         else:
             val_converted = {
                 k: _convert_from_langchain(v, client) for k, v in val.items()
             }
     return val_converted
```

## langchain_google_firestore/document_loader.py

```diff
@@ -11,21 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import itertools
-from typing import TYPE_CHECKING, Any, Iterator, List, Optional
+from typing import TYPE_CHECKING, Iterator, List, Optional
 
-import more_itertools
 from google.cloud import firestore  # type: ignore
 from google.cloud.firestore import DocumentReference  # type: ignore
 from langchain_community.document_loaders.base import BaseLoader
 from langchain_core.documents import Document
+from more_itertools import chunked
 
 from .common import client_with_user_agent
 from .document_converter import (
     DOC_REF,
     FIRESTORE_TYPE,
     convert_firestore_document,
     convert_langchain_document,
@@ -57,37 +57,37 @@
             page_content_fields: The document field names to write into the `page_content`.
                 If an empty or None list is provided all fields will be written into
                 `page_content`. When only one field is provided only the value is written.
             metadata_fields: The document field names to write into the `metadata`.
                 By default it will write all fields that are not in `page_content` into `metadata`.
             client: Client for interacting with the Google Cloud Firestore API.
         """
-        self.client = client_with_user_agent(client, USER_AGENT_LOADER)
+        self.client = client_with_user_agent(USER_AGENT_LOADER, client)
         self.source = source
         self.page_content_fields = page_content_fields
         self.metadata_fields = metadata_fields
 
     def load(self) -> List[Document]:
         """Load Documents."""
         return list(self.lazy_load())
 
     def lazy_load(self) -> Iterator[Document]:
         """A lazy loader for Documents."""
         query = None
         if isinstance(self.source, DocumentReference):
             self.source._client = client_with_user_agent(
-                self.source._client, USER_AGENT_LOADER
+                USER_AGENT_LOADER, self.source._client
             )
             yield convert_firestore_document(self.source.get())
         else:
             if isinstance(self.source, str):
                 query = self.client.collection(self.source)
             else:
                 query = self.source
-                client_with_user_agent(query._client, USER_AGENT_LOADER)
+                client_with_user_agent(USER_AGENT_LOADER, query._client)
 
             for document_snapshot in query.stream():
                 yield convert_firestore_document(
                     document_snapshot,
                     self.page_content_fields,
                     self.metadata_fields,
                 )
@@ -104,15 +104,15 @@
         """Document Saver for Google Cloud Firestore.
         Args:
             collection: The single `/`-delimited path to a Firestore collection. If this
               value is present it will write documents with an auto generated id.
             client: Client for interacting with the Google Cloud Firestore API.
         """
         self.collection = collection
-        self.client = client_with_user_agent(client, USER_AGENT_SAVER)
+        self.client = client_with_user_agent(USER_AGENT_SAVER, client)
 
     def upsert_documents(
         self,
         documents: List[Document],
         merge: Optional[bool] = False,
         document_ids: Optional[List[str]] = None,
     ) -> None:
@@ -129,15 +129,15 @@
         if document_ids and len(document_ids) != len(documents):
             raise ValueError(
                 "`documents` and `document_ids` parameters must be the same length"
             )
 
         docs_list = itertools.zip_longest(documents, document_ids or [])
 
-        for batch in more_itertools.chunked(docs_list, WRITE_BATCH_SIZE):
+        for batch in chunked(docs_list, WRITE_BATCH_SIZE):
             for doc, doc_id in batch:
                 document_dict = convert_langchain_document(doc, self.client)
                 if self.collection:
                     doc_ref = self.client.collection(self.collection).document()
                 elif doc_id:
                     doc_ref = DocumentReference(*doc_id.split("/"), client=self.client)
                 elif document_dict.get("reference", {}).get(FIRESTORE_TYPE) == DOC_REF:
@@ -170,15 +170,15 @@
             the `documents` argument will be ignored.
 
         """
         db_batch = self.client.batch()
 
         docs_list = itertools.zip_longest(documents, document_ids or [])
 
-        for batch in more_itertools.chunked(docs_list, WRITE_BATCH_SIZE):
+        for batch in chunked(docs_list, WRITE_BATCH_SIZE):
             for doc, doc_id in batch:
                 document_path = None
                 if doc_id:
                     document_path = doc_id
                 elif doc:
                     document_dict = convert_langchain_document(doc, self.client)
                     if (
```

## langchain_google_firestore/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.2"
+__version__ = "0.2.0"
```

## Comparing `tests/unit_tests/test_chat_message_history.py` & `tests/test_chat_message_history.py`

 * *Files identical despite different names*

## Comparing `tests/unit_tests/test_document_converter.py` & `tests/test_document_converter.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,32 +8,41 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from unittest.mock import patch
+
 import pytest
-from google.cloud import firestore  # type: ignore
 from google.cloud.firestore import (  # type: ignore
     DocumentReference,
     DocumentSnapshot,
     GeoPoint,
 )
+from google.cloud.firestore_v1.vector import Vector  # type: ignore
 from langchain_core.documents import Document
 
 from langchain_google_firestore.document_converter import (
     DOC_REF,
     FIRESTORE_TYPE,
     GEOPOINT,
+    VECTOR,
     convert_firestore_document,
     convert_langchain_document,
 )
 
 
+@pytest.fixture(scope="module", autouse=True)
+def firestore_client():
+    with patch("google.cloud.firestore.Client") as _fixture:
+        yield _fixture
+
+
 @pytest.mark.parametrize(
     "document_snapshot,langchain_doc",
     [
         (
             DocumentSnapshot(
                 reference=DocumentReference("foo", "bar"),
                 data={"field_1": "data_1", "field_2": 2},
@@ -53,15 +62,19 @@
             ),
         ),
         (
             DocumentSnapshot(
                 reference=DocumentReference("foo", "bar"),
                 data={
                     "field_1": GeoPoint(1, 2),
-                    "field_2": ["data", 2, {"nested": DocumentReference("abc", "xyz")}],
+                    "field_2": [
+                        "data",
+                        2,
+                        {"nested": DocumentReference("abc", "xyz")},
+                    ],
                 },
                 exists=True,
                 read_time=None,
                 create_time=None,
                 update_time=None,
             ),
             Document(
@@ -246,26 +259,32 @@
                     FIRESTORE_TYPE: DOC_REF,
                 },
                 "data": {"page_content": "value"},
             },
         ),
         (
             Document(page_content="value", metadata={"reference": {}}),
-            {"reference": None, "data": {"page_content": "value", "reference": {}}},
+            {
+                "reference": None,
+                "data": {"page_content": "value", "reference": {}},
+            },
         ),
         (
             Document(
                 page_content="value",
                 metadata={"reference": {"path": "foo/bar", "unexpected_field": "data"}},
             ),
             {
                 "reference": None,
                 "data": {
                     "page_content": "value",
-                    "reference": {"path": "foo/bar", "unexpected_field": "data"},
+                    "reference": {
+                        "path": "foo/bar",
+                        "unexpected_field": "data",
+                    },
                 },
             },
         ),
         (
             Document(
                 page_content="value",
                 metadata={
@@ -283,15 +302,15 @@
                 "reference": {
                     "path": "foo/bar",
                     FIRESTORE_TYPE: DOC_REF,
                 },
                 "data": {
                     "page_content": "value",
                     "metadata_field": DocumentReference(
-                        *["abc", "xyz"], client=pytest.client
+                        *["abc", "xyz"], client=firestore_client
                     ),
                 },
             },
         ),
         (
             Document(
                 page_content='{"field_1": "val_1", "field_2": "val_2"}',
@@ -304,15 +323,19 @@
                 },
             ),
             {
                 "reference": {
                     "path": "foo/bar",
                     FIRESTORE_TYPE: DOC_REF,
                 },
-                "data": {"field_1": "val_1", "field_2": "val_2", "field_3": "val_3"},
+                "data": {
+                    "field_1": "val_1",
+                    "field_2": "val_2",
+                    "field_3": "val_3",
+                },
             },
         ),
         (
             Document(
                 page_content="",
                 metadata={
                     "reference": {
@@ -349,60 +372,183 @@
                 "reference": {
                     "path": "foo/bar",
                     FIRESTORE_TYPE: DOC_REF,
                 },
                 "data": {"point": GeoPoint(1, 2), "field_2": "val_2"},
             },
         ),
-        (Document(page_content="", metadata={}), {"reference": None, "data": {}}),
+        (
+            Document(page_content="", metadata={}),
+            {"reference": None, "data": {}},
+        ),
         (
             Document(
                 page_content='{"array":[1, "data", {"k_1":"v_1", "k_point": {"latitude":1, "longitude":0, "firestore_type": "geopoint"}}], "f_2":2}',
                 metadata={},
             ),
             {
                 "reference": None,
                 "data": {
-                    "array": [1, "data", {"k_1": "v_1", "k_point": GeoPoint(1, 0)}],
+                    "array": [
+                        1,
+                        "data",
+                        {"k_1": "v_1", "k_point": GeoPoint(1, 0)},
+                    ],
                     "f_2": 2,
                 },
             },
         ),
     ],
 )
 def test_convert_langchain_document(langchain_doc, firestore_doc):
-    return_doc = convert_langchain_document(langchain_doc, pytest.client)
+    return_doc = convert_langchain_document(langchain_doc, firestore_client)
     assert return_doc == firestore_doc
 
 
 @pytest.mark.parametrize(
     "firestore_doc",
     [
         (
             DocumentSnapshot(
-                reference=DocumentReference(*["foo", "bar"], client=pytest.client),
+                reference=DocumentReference(*["foo", "bar"], client=firestore_client),
                 data={
                     "field_1": GeoPoint(1, 2),
                     "field_2": [
                         "data",
                         2,
                         {
                             "nested": DocumentReference(
-                                *["abc", "xyz"], client=pytest.client
+                                *["abc", "xyz"], client=firestore_client
                             )
                         },
                     ],
                 },
                 exists=True,
                 read_time=None,
                 create_time=None,
                 update_time=None,
             )
         ),
     ],
 )
 def test_roundtrip_firestore(firestore_doc):
     langchain_doc = convert_firestore_document(firestore_doc)
-    roundtrip_doc = convert_langchain_document(langchain_doc, pytest.client)
+    roundtrip_doc = convert_langchain_document(langchain_doc, firestore_client)
+
+    assert roundtrip_doc["data"] == firestore_doc.to_dict()
+    assert roundtrip_doc["reference"]["path"] == firestore_doc.reference.path
+
+
+@pytest.mark.parametrize(
+    "firestore_doc, langchain_doc",
+    [
+        (
+            DocumentSnapshot(
+                reference=DocumentReference(*["foo", "bar"], client=firestore_client),
+                data={
+                    "embedding": Vector([1, 2, 3]),
+                    "content": "test_doc2",
+                },
+                exists=True,
+                read_time=None,
+                create_time=None,
+                update_time=None,
+            ),
+            Document(
+                page_content="test_doc2",
+                metadata={
+                    "reference": {
+                        "path": "foo/bar",
+                        FIRESTORE_TYPE: DOC_REF,
+                    },
+                    "embedding": {
+                        "values": [1, 2, 3],
+                        FIRESTORE_TYPE: VECTOR,
+                    },
+                },
+            ),
+        ),
+    ],
+)
+def test_vector_type_from_firestore(firestore_doc, langchain_doc):
+    """
+    Test vector type conversion from Firestore to LangChain.
+    """
+
+    assert convert_firestore_document(firestore_doc) == langchain_doc
+
+
+@pytest.mark.parametrize(
+    "langchain_doc, firestore_doc",
+    [
+        (
+            Document(
+                page_content="test_doc2",
+                metadata={
+                    "reference": {
+                        "path": "foo/bar",
+                        FIRESTORE_TYPE: DOC_REF,
+                    },
+                    "embedding": {
+                        "values": [1, 2, 3],
+                        FIRESTORE_TYPE: VECTOR,
+                    },
+                },
+            ),
+            {
+                "reference": {
+                    "path": "foo/bar",
+                    FIRESTORE_TYPE: DOC_REF,
+                },
+                "data": {
+                    "page_content": "test_doc2",
+                    "embedding": Vector([1, 2, 3]),
+                },
+            },
+        ),
+    ],
+)
+def test_vector_type_to_firestore(langchain_doc, firestore_doc):
+    """
+    Test vector type conversion from LangChain to Firestore.
+    """
+
+    assert convert_langchain_document(langchain_doc, firestore_client) == firestore_doc
+
+
+@pytest.mark.parametrize(
+    "firestore_doc",
+    [
+        (
+            DocumentSnapshot(
+                reference=DocumentReference(*["foo", "bar"], client=firestore_client),
+                data={
+                    "field_1": GeoPoint(1, 2),
+                    "field_2": [
+                        "data",
+                        2,
+                        {
+                            "nested": DocumentReference(
+                                *["abc", "xyz"], client=firestore_client
+                            )
+                        },
+                    ],
+                    "field_3": Vector([1, 2, 3]),
+                },
+                exists=True,
+                read_time=None,
+                create_time=None,
+                update_time=None,
+            )
+        ),
+    ],
+)
+def test_vector_type_roundtrip(firestore_doc):
+    """
+    Test vector type roundtrip conversion between LangChain and Firestore.
+    """
+
+    langchain_doc = convert_firestore_document(firestore_doc)
+    roundtrip_doc = convert_langchain_document(langchain_doc, firestore_client)
 
     assert roundtrip_doc["data"] == firestore_doc.to_dict()
     assert roundtrip_doc["reference"]["path"] == firestore_doc.reference.path
```

## Comparing `tests/unit_tests/test_document_loader.py` & `tests/test_document_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
 import unittest.mock as mock
+import uuid
 from unittest import TestCase
 
 import pytest
 from google.cloud.firestore import Client, CollectionGroup, FieldFilter  # type: ignore
 from langchain_core.documents import Document
 
 from langchain_google_firestore import FirestoreLoader, FirestoreSaver
@@ -30,16 +31,17 @@
 
 @pytest.fixture
 def client() -> Client:
     return Client()
 
 
 def test_firestore_write_roundtrip_and_load() -> None:
-    saver = FirestoreSaver("WriteRoundTrip")
-    loader = FirestoreLoader("WriteRoundTrip")
+    source = "WriteRoundTrip" + str(uuid.uuid4())
+    saver = FirestoreSaver(source)
+    loader = FirestoreLoader(source)
 
     docs = [Document(page_content="data", metadata={})]
 
     saver.upsert_documents(docs)
     # wait 1s for consistency
     time.sleep(1)
     written_docs = loader.load()
@@ -53,16 +55,17 @@
     assert written_docs[0].page_content == "data"
     assert written_docs[0].metadata != {}
     assert "reference" in written_docs[0].metadata
     assert len(deleted_docs) == 0
 
 
 def test_firestore_write_load_batch(test_case: TestCase) -> None:
-    saver = FirestoreSaver("WriteBatch")
-    loader = FirestoreLoader("WriteBatch")
+    source = "WriteBatch" + str(uuid.uuid4())
+    saver = FirestoreSaver(source)
+    loader = FirestoreLoader(source)
     NUM_DOCS = 1000
 
     docs = []
     expected_docs = []
     for i in range(NUM_DOCS):
         docs.append(Document(page_content=f"content {i}"))
         expected_docs.append(
@@ -87,23 +90,24 @@
     docs_after_delete = loader.load()
 
     test_case.assertCountEqual(expected_docs, docs_after_write)
     assert len(docs_after_delete) == 0
 
 
 def test_firestore_write_with_reference(test_case: TestCase) -> None:
+    source = "WriteRef" + str(uuid.uuid4())
     saver = FirestoreSaver()
-    loader = FirestoreLoader("WriteRef")
+    loader = FirestoreLoader(source)
 
     expected_doc = [
         Document(
             page_content='{"f1": 1, "f2": 2}',
             metadata={
                 "reference": {
-                    "path": "WriteRef/doc",
+                    "path": source + "/doc",
                     "firestore_type": "document_reference",
                 }
             },
         )
     ]
     saver.upsert_documents(expected_doc)
     # wait 1s for consistency
@@ -125,16 +129,17 @@
 
     test_case.assertRaises(
         ValueError, saver.upsert_documents, documents=doc_to_insert, document_ids=doc_id
     )
 
 
 def test_firestore_write_with_doc_id(test_case: TestCase) -> None:
+    source = "WriteId" + str(uuid.uuid4())
     saver = FirestoreSaver()
-    loader = FirestoreLoader("WriteId")
+    loader = FirestoreLoader(source)
 
     doc_to_insert = [
         Document(
             page_content='{"f1": 1, "f2": 2}',
             metadata={
                 "reference": {"path": "foo/bar", "firestore_type": "document_reference"}
             },
@@ -142,21 +147,21 @@
     ]
 
     expected_doc = [
         Document(
             page_content='{"f1": 1, "f2": 2}',
             metadata={
                 "reference": {
-                    "path": "WriteId/doc",
+                    "path": source + "/doc",
                     "firestore_type": "document_reference",
                 }
             },
         )
     ]
-    doc_id = ["WriteId/doc"]
+    doc_id = [source + "/doc"]
     saver.upsert_documents(documents=doc_to_insert, document_ids=doc_id)
     # wait 1s for consistency
     time.sleep(1)
     written_doc = loader.load()
     saver.delete_documents(written_doc, doc_id)
     # wait 1s for consistency
     time.sleep(1)
@@ -179,17 +184,18 @@
 def test_firestore_load_with_fields(
     page_fields,
     metadata_fields,
     expected_page_content,
     expected_metadata,
     test_case: TestCase,
 ):
-    saver = FirestoreSaver("WritePageFields")
+    source = "WritePageFields" + str(uuid.uuid4())
+    saver = FirestoreSaver(source)
     loader = FirestoreLoader(
-        source="WritePageFields",
+        source=source,
         page_content_fields=page_fields,
         metadata_fields=metadata_fields,
     )
 
     doc_to_insert = [
         Document(page_content='{"f1": "v1", "f2": "v2", "f3": "v3"}', metadata={})
     ]
@@ -207,23 +213,24 @@
     deleted_docs = loader.load()
 
     test_case.assertCountEqual(expected_doc, loaded_doc)
     assert len(deleted_docs) == 0
 
 
 def test_firestore_load_from_subcollection(test_case: TestCase):
+    source = "collection/doc/subcol" + str(uuid.uuid4())
     saver = FirestoreSaver()
-    loader = FirestoreLoader("collection/doc/subcol")
+    loader = FirestoreLoader(source)
 
     doc_to_insert = [
         Document(
             page_content="data",
             metadata={
                 "reference": {
-                    "path": "collection/doc/subcol/sdoc",
+                    "path": source + "/sdoc",
                     "firestore_type": "document_reference",
                 }
             },
         )
     ]
 
     saver.upsert_documents(doc_to_insert)
@@ -236,16 +243,17 @@
     deleted_docs = loader.load()
 
     test_case.assertCountEqual(doc_to_insert, loaded_doc)
     assert len(deleted_docs) == 0
 
 
 def test_firestore_load_from_query(test_case: TestCase, client: Client):
-    saver = FirestoreSaver("WriteQuery")
-    loader_cleanup = FirestoreLoader("WriteQuery")
+    source = "WriteQuery" + str(uuid.uuid4())
+    saver = FirestoreSaver(source)
+    loader_cleanup = FirestoreLoader(source)
 
     docs_to_insert = [
         Document(page_content='{"num": 20, "region": "west_coast"}'),
         Document(page_content='{"num": 20, "region": "south_coast"}'),
         Document(page_content='{"num": 30, "region": "west_coast"}'),
         Document(page_content='{"num": 0, "region": "east_coast"}'),
     ]
@@ -256,15 +264,15 @@
         ),
         Document(
             page_content='{"num": 30, "region": "west_coast"}',
             metadata={"reference": mock.ANY},
         ),
     ]
 
-    col_ref = client.collection("WriteQuery")
+    col_ref = client.collection(source)
     query = col_ref.where(filter=FieldFilter("region", "==", "west_coast"))
     loader = FirestoreLoader(query)
 
     saver.upsert_documents(docs_to_insert)
     # wait 1s for consistency
     time.sleep(1)
     loaded_docs = loader.load()
@@ -275,88 +283,98 @@
 
     test_case.assertCountEqual(expected_docs, loaded_docs)
     assert len(deleted_docs) == 0
 
 
 def test_firestore_load_from_col_group(test_case: TestCase, client: Client):
     saver = FirestoreSaver()
+    source_1 = "ColGroup" + str(uuid.uuid4())
+    source_2 = "foo" + str(uuid.uuid4())
 
     docs_to_insert = [
         Document(
             page_content="data_A",
             metadata={
                 "reference": {
-                    "path": "ColA/doc/ColGroup/doc1",
+                    "path": "ColA/doc/" + source_1 + "/doc1",
                     "firestore_type": "document_reference",
                 }
             },
         ),
         Document(
             page_content="data_B",
             metadata={
                 "reference": {
-                    "path": "ColB/doc/ColGroup/doc2",
+                    "path": "ColA/doc/" + source_1 + "/doc2",
                     "firestore_type": "document_reference",
                 }
             },
         ),
         Document(
             page_content="data_C",
             metadata={
-                "reference": {"path": "foo/bar", "firestore_type": "document_reference"}
+                "reference": {
+                    "path": source_2 + "/bar",
+                    "firestore_type": "document_reference",
+                }
             },
         ),
     ]
     expected_docs = [
         Document(
             page_content="data_A",
             metadata={
                 "reference": {
-                    "path": "ColA/doc/ColGroup/doc1",
+                    "path": "ColA/doc/" + source_1 + "/doc1",
                     "firestore_type": "document_reference",
                 }
             },
         ),
         Document(
             page_content="data_B",
             metadata={
                 "reference": {
-                    "path": "ColB/doc/ColGroup/doc2",
+                    "path": "ColA/doc/" + source_1 + "/doc2",
                     "firestore_type": "document_reference",
                 }
             },
         ),
     ]
 
     saver.upsert_documents(docs_to_insert)
     # wait 1s for consistency
     time.sleep(1)
 
-    col_ref = client.collection("ColGroup")
+    col_ref = client.collection(source_1)
     collection_group = CollectionGroup(col_ref)
     loader = FirestoreLoader(collection_group)
     loaded_docs = loader.load()
     saver.delete_documents(docs_to_insert)
 
     test_case.assertCountEqual(expected_docs, loaded_docs)
 
 
 def test_firestore_load_from_doc_ref(test_case: TestCase, client: Client):
     saver = FirestoreSaver()
 
+    source = "foo" + str(uuid.uuid4())
+
     doc_to_insert = [
         Document(
             page_content="data",
             metadata={
-                "reference": {"path": "foo/bar", "firestore_type": "document_reference"}
+                "reference": {
+                    "path": source + "/bar",
+                    "firestore_type": "document_reference",
+                }
             },
         )
     ]
 
-    doc_ref = client.collection("foo").document("bar")
+    doc_ref = client.collection(source).document("bar")
 
     saver.upsert_documents(doc_to_insert)
     # wait 1s for consistency
     time.sleep(1)
     loader = FirestoreLoader(doc_ref)
     loaded_doc = loader.load()
     saver.delete_documents(doc_to_insert)
@@ -370,16 +388,17 @@
     loaded_docs = loader.load()
 
     assert len(loaded_docs) == 0
 
 
 def test_firestore_custom_client() -> None:
     client = Client(database="(default)")
-    saver = FirestoreSaver("Custom", client=client)
-    loader = FirestoreLoader("Custom", client=client)
+    source = "Custom" + str(uuid.uuid4())
+    saver = FirestoreSaver(source, client=client)
+    loader = FirestoreLoader(source, client=client)
 
     docs = [Document(page_content="data", metadata={})]
 
     saver.upsert_documents(docs)
     # wait 1s for consistency
     time.sleep(1)
     written_docs = loader.load()
```

## Comparing `langchain_google_firestore-0.1.2.dist-info/LICENSE` & `langchain_google_firestore-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_firestore-0.1.2.dist-info/METADATA` & `langchain_google_firestore-0.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-firestore
-Version: 0.1.2
+Version: 0.2.0
 Summary: LangChain integrations for Google Cloud Firestore
 Author-email: Google LLC <googleapis-packages@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -211,21 +211,21 @@
 Project-URL: Bug Tracker, https://github.com/googleapis/langchain-google-firestore-python/issues
 Project-URL: Changelog, https://github.com/googleapis/langchain-google-firestore-python/blob/main/CHANGELOG.md
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: langchain-core <1.0.0,>=0.1.1
 Requires-Dist: langchain-community <1.0.0,>=0.0.18
-Requires-Dist: google-cloud-firestore <3.0.0,>=2.14.0
+Requires-Dist: google-cloud-firestore <3.0.0,>=2.16.0
 Requires-Dist: more-itertools <11.0.0,>=10.2.0
 Provides-Extra: test
 Requires-Dist: black[jupyter] ==23.12.1 ; extra == 'test'
 Requires-Dist: isort ==5.13.2 ; extra == 'test'
 Requires-Dist: mypy ==1.9.0 ; extra == 'test'
-Requires-Dist: pytest-asyncio ==0.23.5.post1 ; extra == 'test'
+Requires-Dist: pytest-asyncio ==0.23.6 ; extra == 'test'
 Requires-Dist: pytest ==7.4.4 ; extra == 'test'
 
 # Firestore for LangChain
 
 This package contains the [LangChain][langchain] integrations for Firestore.
 
 > **🧪 Preview:** This feature is covered by the Pre-GA Offerings Terms of the Google Cloud Terms of Service. Please note that pre-GA products and features might have limited support, and changes to pre-GA products and features might not be compatible with other pre-GA versions. For more information, see the [launch stage descriptions](https://cloud.google.com/products#product-launch-stages)
```

## Comparing `langchain_google_firestore-0.1.2.dist-info/RECORD` & `langchain_google_firestore-0.2.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-langchain_google_firestore/__init__.py,sha256=SF_0BrBuT08LvZ6mwd-Q-TpI-GAQEAUc4whDgmHehFk,898
-langchain_google_firestore/chat_message_history.py,sha256=Ocelhk_3i1WDOS_66OkvJk_PQD_8Su0LWqlAj4o6c4w,2956
-langchain_google_firestore/common.py,sha256=qANMZrVaS3_pGO31pjX0Bm3AkFufLBEcmddTgo44ZUY,1288
-langchain_google_firestore/document_converter.py,sha256=ItHqLv37A_H3KfJmtVO9p0UdDjUgfmH9NJvbBrvB8yk,4081
-langchain_google_firestore/document_loader.py,sha256=yg7gV4qe3O1jZf9Ze5kmNuUPh25gZ2-b4dozgn5cZ20,8042
+langchain_google_firestore/__init__.py,sha256=y0T6tgQjKQ4mJ9LqMVPfzc0bVbI-Kmp9UbtccFbJqDI,920
+langchain_google_firestore/chat_message_history.py,sha256=ag6S29jXY6lSTawl1soVXTVH9TVe3MmobZbbo5vwF7s,2941
+langchain_google_firestore/common.py,sha256=y4b-mP3Le3GbdS8pCMIf7sy5VcSftvkTFjGDcmPxE5E,1309
+langchain_google_firestore/document_converter.py,sha256=KFDvyKzA3CaYkXiMV0F_YloEtiKf708S16ZYOJwsp04,4703
+langchain_google_firestore/document_loader.py,sha256=YkeSNJeDVqYoMAVSRDS8qNJyyYc4s0O5jggTEb6dBZ4,8020
 langchain_google_firestore/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-langchain_google_firestore/version.py,sha256=CSYr0JwXc5Z4Db3PnHnAhFfSGqiH8AayAv6dOaxd1ks,597
+langchain_google_firestore/vectorstores.py,sha256=rinOn5RyK4oM6O56EIzOpw1OjAq0UxT2UMzceIP0r6c,12399
+langchain_google_firestore/version.py,sha256=c32tFkU7bcWMAeqBrDdHTYBzbZPaJPvhWqbKnyY_LxM,597
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/conftest.py,sha256=aGkv6kBNgUspy36R2TdFZg7r9GSIdejoXp0OQlPETjE,705
-tests/unit_tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/unit_tests/test_chat_message_history.py,sha256=ZExMtWtsGHqVx-OmoH5MSBD6L0OhInK1u3FbezARMJg,4874
-tests/unit_tests/test_document_converter.py,sha256=NwHVNesrnwquqUGqZv8YRTJhnX9KlK4zy082BjNo6kE,12831
-tests/unit_tests/test_document_loader.py,sha256=wOWfxedOcYNABpPuYnU06n-6njUQQWnVQ1tmTQGz7f8,11531
-langchain_google_firestore-0.1.2.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-langchain_google_firestore-0.1.2.dist-info/METADATA,sha256=UkLdArPJkjH8g2QSI6BT2o8-wGWNqWhFiOl9ekEbZ2U,17681
-langchain_google_firestore-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-langchain_google_firestore-0.1.2.dist-info/top_level.txt,sha256=v0bJ-rJBT8IaMWBUWqKXDb-8E5Q2MXamLYl-UdMkIFY,33
-langchain_google_firestore-0.1.2.dist-info/RECORD,,
+tests/test_chat_message_history.py,sha256=ZExMtWtsGHqVx-OmoH5MSBD6L0OhInK1u3FbezARMJg,4874
+tests/test_document_converter.py,sha256=EFw9so8gntJdWfKgA84Kilygq23JRSxv8MmiaUibzZE,16924
+tests/test_document_loader.py,sha256=94iTAjAitgFNQrUr_HdXsRRJJft7rKSBoQsBCZpkqNU,12105
+tests/test_vectorstores.py,sha256=8ctac3gn-6RDxwS0jEp7e73konft0fA5WYbQ6cEC8Ic,14315
+langchain_google_firestore-0.2.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+langchain_google_firestore-0.2.0.dist-info/METADATA,sha256=sD-SwW6cDjug0BOPSphdHG3-8Kuo4GIrHYI7BVQUWjk,17675
+langchain_google_firestore-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+langchain_google_firestore-0.2.0.dist-info/top_level.txt,sha256=v0bJ-rJBT8IaMWBUWqKXDb-8E5Q2MXamLYl-UdMkIFY,33
+langchain_google_firestore-0.2.0.dist-info/RECORD,,
```

