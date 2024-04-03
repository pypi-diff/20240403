# Comparing `tmp/sigstore_rekor_types-0.0.8.tar.gz` & `tmp/sigstore_rekor_types-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigstore_rekor_types-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sigstore_rekor_types-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigstore_rekor_types-0.0.8.tar` & `sigstore_rekor_types-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    10174 2023-10-04 17:52:09.503798 sigstore_rekor_types-0.0.8/LICENSE
--rw-r--r--   0        0        0      867 2023-10-04 17:52:09.503798 sigstore_rekor_types-0.0.8/README.md
--rw-r--r--   0        0        0     2096 2023-10-04 17:52:09.503798 sigstore_rekor_types-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      102 2023-10-04 17:52:09.503798 sigstore_rekor_types-0.0.8/sigstore_rekor_types/__init__.py
--rw-r--r--   0        0        0    24042 2023-10-04 17:52:09.503798 sigstore_rekor_types-0.0.8/sigstore_rekor_types/_internal.py
--rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 sigstore_rekor_types-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-10-04 18:44:20.526995 sigstore_rekor_types-0.0.9/LICENSE
+-rw-r--r--   0        0        0      867 2023-10-04 18:44:20.526995 sigstore_rekor_types-0.0.9/README.md
+-rw-r--r--   0        0        0     2096 2023-10-04 18:44:20.526995 sigstore_rekor_types-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      102 2023-10-04 18:44:20.526995 sigstore_rekor_types-0.0.9/sigstore_rekor_types/__init__.py
+-rw-r--r--   0        0        0    24111 2023-10-04 18:44:20.526995 sigstore_rekor_types-0.0.9/sigstore_rekor_types/_internal.py
+-rw-r--r--   0        0        0        0 2023-10-04 18:44:20.526995 sigstore_rekor_types-0.0.9/sigstore_rekor_types/py.typed
+-rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 sigstore_rekor_types-0.0.9/PKG-INFO
```

### Comparing `sigstore_rekor_types-0.0.8/LICENSE` & `sigstore_rekor_types-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sigstore_rekor_types-0.0.8/README.md` & `sigstore_rekor_types-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sigstore_rekor_types-0.0.8/pyproject.toml` & `sigstore_rekor_types-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sigstore_rekor_types-0.0.8/sigstore_rekor_types/_internal.py` & `sigstore_rekor_types-0.0.9/sigstore_rekor_types/_internal.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, RootModel, StrictInt, StrictStr
 
 
 class ProposedEntry(BaseModel):
     kind: StrictStr
 
 
-class Format(Enum):
+class Format(str, Enum):
     """Specifies the format of the signature."""
 
     PGP = "pgp"
     MINISIGN = "minisign"
     X509 = "x509"
     SSH = "ssh"
 
@@ -54,40 +54,40 @@
     )
 
 
 class PublicKey1(BaseModel):
     """The public key that can verify the signature; this can also be an X509 code signing certificate that contains the raw public key information."""
 
     content: Optional[str] = Field(
-        None,
+        default=None,
         description=(
             "Specifies the content of the public key or code signing certificate inline within the"
             " document"
         ),
     )
 
 
 class Signature1(BaseModel):
     """Information about the detached signature associated with the entry."""
 
     content: Optional[str] = Field(
-        None,
+        default=None,
         description="Specifies the content of the signature inline within the document",
     )
     public_key: Optional[PublicKey1] = Field(
-        None,
+        default=None,
         alias="publicKey",
         description=(
             "The public key that can verify the signature; this can also be an X509 code signing"
             " certificate that contains the raw public key information"
         ),
     )
 
 
-class Algorithm(Enum):
+class Algorithm(str, Enum):
     """The hashing function used to compute the hash value."""
 
     SHA256 = "sha256"
 
 
 class Hash(BaseModel):
     """Specifies the hash algorithm and value for the content."""
@@ -99,15 +99,15 @@
     value: StrictStr = Field(..., description="The hash value for the content")
 
 
 class Data(BaseModel):
     """Information about the content associated with the entry."""
 
     hash: Optional[Hash] = Field(
-        None,
+        default=None,
         description="Specifies the hash algorithm and value for the content",
     )
 
 
 class HashedrekordV001Schema(BaseModel):
     """Schema for Hashed Rekord object."""
 
@@ -154,15 +154,15 @@
         description="Specifies the metadata inline within the document",
     )
 
 
 class TufV001Schema(BaseModel):
     """Schema for TUF metadata entries."""
 
-    spec_version: Optional[StrictStr] = Field(None, description="TUF specification version")
+    spec_version: Optional[StrictStr] = Field(default=None, description="TUF specification version")
     metadata: Metadata = Field(..., description="TUF metadata")
     root: Root = Field(
         ...,
         description="root metadata containing about the public keys used to sign the manifest",
     )
 
 
@@ -195,15 +195,15 @@
     value: StrictStr = Field(..., description="The hash value for the chart")
 
 
 class Chart(BaseModel):
     """Information about the Helm chart associated with the entry."""
 
     hash: Optional[Hash1] = Field(
-        None,
+        default=None,
         description="Specifies the hash algorithm and value for the chart",
     )
 
 
 class HelmV001Schema(BaseModel):
     """Schema for Helm object."""
 
@@ -235,24 +235,24 @@
         ...,
         description="The hashing function used to compute the hash value",
     )
     value: StrictStr = Field(..., description="The hash value for the envelope's payload")
 
 
 class Content(BaseModel):
-    envelope: Optional[StrictStr] = Field(None, description="envelope")
+    envelope: Optional[StrictStr] = Field(default=None, description="envelope")
     hash: Optional[Hash2] = Field(
-        None,
+        default=None,
         description=(
             "Specifies the hash algorithm and value encompassing the entire signed envelope; this"
             " is computed by the rekor server, client-provided values are ignored"
         ),
     )
     payload_hash: Optional[PayloadHash] = Field(
-        None,
+        default=None,
         alias="payloadHash",
         description=(
             "Specifies the hash algorithm and value covering the payload within the DSSE envelope;"
             " this is computed by the rekor server, client-provided values are ignored"
         ),
     )
 
@@ -268,29 +268,29 @@
     )
 
 
 class Signature2(BaseModel):
     """a signature of the envelope's payload along with the public key for the signature."""
 
     keyid: Optional[StrictStr] = Field(
-        None,
+        default=None,
         description="optional id of the key used to create the signature",
     )
     sig: str = Field(..., description="signature of the payload")
     public_key: str = Field(
         ...,
         alias="publicKey",
         description="public key that corresponds to this signature",
     )
 
 
 class Envelope(BaseModel):
     """dsse envelope."""
 
-    payload: Optional[str] = Field(None, description="payload of the envelope")
+    payload: Optional[str] = Field(default=None, description="payload of the envelope")
     payload_type: StrictStr = Field(
         ...,
         alias="payloadType",
         description="type describing the payload",
     )
     signatures: List[Signature2] = Field(
         ...,
@@ -318,43 +318,37 @@
     )
     value: StrictStr = Field(..., description="The hash value of the payload")
 
 
 class Content1(BaseModel):
     envelope: Envelope = Field(..., description="dsse envelope")
     hash: Optional[Hash3] = Field(
-        None,
+        default=None,
         description=(
             "Specifies the hash algorithm and value encompassing the entire signed envelope"
         ),
     )
     payload_hash: Optional[PayloadHash1] = Field(
-        None,
+        default=None,
         alias="payloadHash",
         description=(
             "Specifies the hash algorithm and value covering the payload within the DSSE envelope"
         ),
     )
 
 
 class IntotoV002Schema(BaseModel):
     """Schema for intoto object."""
 
     content: Content1
 
 
-class PayloadHash2(BaseModel):
+class PayloadHash2(Hash):
     """Specifies the hash algorithm and value for the content."""
 
-    algorithm: Algorithm = Field(
-        ...,
-        description="The hashing function used to compute the hash value",
-    )
-    value: StrictStr = Field(..., description="The hash value for the content")
-
 
 class EnvelopeHash(BaseModel):
     """Specifies the hash algorithm and value for the COSE envelope."""
 
     algorithm: Algorithm = Field(
         ...,
         description="The hashing function used to compute the hash value",
@@ -362,33 +356,33 @@
     value: StrictStr = Field(..., description="The hash value for the envelope")
 
 
 class Data1(BaseModel):
     """Information about the content associated with the entry."""
 
     payload_hash: Optional[PayloadHash2] = Field(
-        None,
+        default=None,
         alias="payloadHash",
         description="Specifies the hash algorithm and value for the content",
     )
     envelope_hash: Optional[EnvelopeHash] = Field(
-        None,
+        default=None,
         alias="envelopeHash",
         description="Specifies the hash algorithm and value for the COSE envelope",
     )
     aad: Optional[str] = Field(
-        None,
+        default=None,
         description="Specifies the additional authenticated data required to verify the signature",
     )
 
 
 class CoseV001Schema(BaseModel):
     """Schema for cose object."""
 
-    message: Optional[str] = Field(None, description="The COSE Sign1 Message")
+    message: Optional[str] = Field(default=None, description="The COSE Sign1 Message")
     public_key: str = Field(
         ...,
         alias="publicKey",
         description="The public key that can verify the signature",
     )
     data: Data1 = Field(..., description="Information about the content associated with the entry")
 
@@ -422,15 +416,15 @@
     )
 
 
 class JarV001Schema(BaseModel):
     """Schema for JAR entries."""
 
     signature: Optional[Signature3] = Field(
-        None,
+        default=None,
         description="Information about the included signature in the JAR file",
     )
 
 
 class Tsr(BaseModel):
     """Information about the tsr file associated with the entry."""
 
@@ -499,94 +493,94 @@
         description="The value of the computed digest over the payload within the envelope",
     )
 
 
 class DsseV001Schema(BaseModel):
     """Schema for DSSE envelopes."""
 
-    proposed_content: Optional[ProposedContent] = Field(None, alias="proposedContent")
+    proposed_content: Optional[ProposedContent] = Field(default=None, alias="proposedContent")
     signatures: Optional[List[Signature4]] = Field(
-        None,
+        default=None,
         description=(
             "extracted collection of all signatures of the envelope's payload; elements will be"
             " sorted by lexicographical order of the base64 encoded signature strings"
         ),
         min_length=1,
     )
     envelope_hash: Optional[EnvelopeHash1] = Field(
-        None,
+        default=None,
         alias="envelopeHash",
         description=(
             "Specifies the hash algorithm and value encompassing the entire envelope sent to Rekor"
         ),
     )
     payload_hash: Optional[PayloadHash3] = Field(
-        None,
+        default=None,
         alias="payloadHash",
         description=(
             "Specifies the hash algorithm and value covering the payload within the DSSE envelope"
         ),
     )
 
 
 class Attestation(BaseModel):
     data: Optional[Dict[str, Any]] = None
 
 
-class Format1(Enum):
+class Format1(str, Enum):
     PGP = "pgp"
     X509 = "x509"
     MINISIGN = "minisign"
     SSH = "ssh"
     TUF = "tuf"
 
 
 class PublicKey6(BaseModel):
     format: Format1
     content: Optional[str] = Field(
-        None,
+        default=None,
         pattern="^(?:[A-Za-z0-9+/]{4})*(?:[A-Za-z0-9+/]{2}==|[A-Za-z0-9+/]{3}=)?$",
     )
     url: Optional[AnyUrl] = None
 
 
-class Operator(Enum):
+class Operator(str, Enum):
     AND_ = "and"
     OR_ = "or"
 
 
 class SearchIndex(BaseModel):
     email: Optional[EmailStr] = None
-    public_key: Optional[PublicKey6] = Field(None, alias="publicKey")
+    public_key: Optional[PublicKey6] = Field(default=None, alias="publicKey")
     hash: Optional[StrictStr] = None
     operator: Optional[Operator] = None
 
 
 class EntryUuiD(RootModel[StrictStr]):
     root: StrictStr
 
 
 class LogIndex(RootModel[StrictInt]):
     root: StrictInt
 
 
 class SearchLogQuery(BaseModel):
     entry_uui_ds: Optional[List[EntryUuiD]] = Field(
-        None,
+        default=None,
         alias="entryUUIDs",
         max_length=10,
         min_length=1,
     )
     log_indexes: Optional[List[LogIndex]] = Field(
-        None,
+        default=None,
         alias="logIndexes",
         max_length=10,
         min_length=1,
     )
-    entries: Optional[List[ProposedEntry]] = Field(None, max_length=10, min_length=1)
+    entries: Optional[List[ProposedEntry]] = Field(default=None, max_length=10, min_length=1)
 
 
 class InactiveShardLogInfo(BaseModel):
     root_hash: StrictStr = Field(
         ...,
         alias="rootHash",
         description="The current hash value stored at the root of the merkle tree",
@@ -726,17 +720,17 @@
         ...,
         description="log entry schema for dsse envelopes",
         title="DSSE Schema",
     )
 
 
 class Verification(BaseModel):
-    inclusion_proof: Optional[InclusionProof] = Field(None, alias="inclusionProof")
+    inclusion_proof: Optional[InclusionProof] = Field(default=None, alias="inclusionProof")
     signed_entry_timestamp: Optional[str] = Field(
-        None,
+        default=None,
         alias="signedEntryTimestamp",
         description="Signature over the logID, logIndex, body and integratedTime.",
         pattern="^(?:[A-Za-z0-9+/]{4})*(?:[A-Za-z0-9+/]{2}==|[A-Za-z0-9+/]{3}=)?$",
     )
 
 
 class LogEntry1(BaseModel):
@@ -776,15 +770,18 @@
     )
     signed_tree_head: StrictStr = Field(
         ...,
         alias="signedTreeHead",
         description="The current signed tree head",
     )
     tree_id: StrictStr = Field(..., alias="treeID", description="The current treeID")
-    inactive_shards: Optional[List[InactiveShardLogInfo]] = Field(None, alias="inactiveShards")
+    inactive_shards: Optional[List[InactiveShardLogInfo]] = Field(
+        default=None,
+        alias="inactiveShards",
+    )
 
 
 class Rekord(ProposedEntry):
     """Rekord object."""
 
     api_version: StrictStr = Field(..., alias="apiVersion")
     spec: RekordSchema
```

### Comparing `sigstore_rekor_types-0.0.8/PKG-INFO` & `sigstore_rekor_types-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigstore-rekor-types
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python models for Rekor's API types
 Author-email: Trail of Bits <opensource@trailofbits.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: pydantic[email] >=2,<3
```

