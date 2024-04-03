# Comparing `tmp/mse-lib-sgx-2.3.0a4.tar.gz` & `tmp/mse-lib-sgx-3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse-lib-sgx-2.3.0a4.tar", last modified: Wed Apr  3 08:19:47 2024, max compression
+gzip compressed data, was "mse-lib-sgx-3.0a1.tar", last modified: Wed Aug  9 07:56:57 2023, max compression
```

## Comparing `mse-lib-sgx-2.3.0a4.tar` & `mse-lib-sgx-3.0a1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:19:47.265517 mse-lib-sgx-2.3.0a4/
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-03 08:19:47.265517 mse-lib-sgx-2.3.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 08:19:47.265517 mse-lib-sgx-2.3.0a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:19:47.257517 mse-lib-sgx-2.3.0a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:19:47.261517 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/base64url.py
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/globs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:19:47.261517 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/sgx/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/sgx/key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/sgx/quote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:19:47.261517 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-03 08:19:47.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-03 08:19:47.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:19:47.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 08:19:47.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-03 08:19:47.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 08:19:47.000000 mse-lib-sgx-2.3.0a4/src/mse_lib_sgx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:19:47.261517 mse-lib-sgx-2.3.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/tests/test_cert_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-03 08:19:11.000000 mse-lib-sgx-2.3.0a4/tests/test_conf_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 07:56:56.999551 mse-lib-sgx-3.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-09 07:56:56.999551 mse-lib-sgx-3.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-09 07:56:56.999551 mse-lib-sgx-3.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 07:56:56.999551 mse-lib-sgx-3.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 07:56:56.999551 mse-lib-sgx-3.0a1/src/mse_lib_sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx/base64url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx/http_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 07:56:56.999551 mse-lib-sgx-3.0a1/src/mse_lib_sgx/sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx/sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx/sgx/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx/sgx/quote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 07:56:56.999551 mse-lib-sgx-3.0a1/src/mse_lib_sgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-09 07:56:56.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-09 07:56:56.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 07:56:56.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-09 07:56:56.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-09 07:56:56.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-09 07:56:56.000000 mse-lib-sgx-3.0a1/src/mse_lib_sgx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 07:56:56.999551 mse-lib-sgx-3.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/tests/test_cert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-09 07:56:11.000000 mse-lib-sgx-3.0a1/tests/test_conf_server.py
```

### Comparing `mse-lib-sgx-2.3.0a4/PKG-INFO` & `mse-lib-sgx-3.0a1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,23 @@
 Metadata-Version: 2.1
 Name: mse-lib-sgx
-Version: 2.3.0a4
+Version: 3.0a1
 Summary: Library to bootstrap WSGI/ASGI application for Gramine
 Author-email: Cosmian Tech <tech@cosmian.com>
 License: MIT
 Classifier: Development Status :: 6 - Mature
+Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: cryptography<43.0.0,>=42.0.5
-Requires-Dist: intel-sgx-ra<3.0.0,>=2.2.0
-Requires-Dist: hypercorn[uvloop]<0.17.0,>=0.16.0
-Requires-Dist: h2<4.2.0,>=4.1.0
-Requires-Dist: mse-lib-crypto<2.0,>=1.4
 Provides-Extra: dev
-Requires-Dist: black<25.0.0,>=24.3.0; extra == "dev"
-Requires-Dist: isort<6.0.0,>=5.13.2; extra == "dev"
-Requires-Dist: pylint<4.0.0,>=3.1.0; extra == "dev"
-Requires-Dist: pycodestyle<3.0.0,>=2.11.1; extra == "dev"
-Requires-Dist: pydocstyle<7.0.0,>=6.3.0; extra == "dev"
-Requires-Dist: mypy<2.0.0,>=1.9.0; extra == "dev"
-Requires-Dist: pytest<9.0.0,>=8.1.1; extra == "dev"
 Provides-Extra: deploy
-Requires-Dist: build<2.0.0,>=1.1.1; extra == "deploy"
-Requires-Dist: wheel<0.44.0,>=0.43.0; extra == "deploy"
 
 # MicroService Encryption Lib SGX
 
 ## Overview
 
 MSE lib SGX bootstraps the execution of an encrypted ASGI/WSGI Python web application for [Gramine](https://gramine.readthedocs.io/).
```

### Comparing `mse-lib-sgx-2.3.0a4/README.md` & `mse-lib-sgx-3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `mse-lib-sgx-2.3.0a4/pyproject.toml` & `mse-lib-sgx-3.0a1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 [build-system]
-requires = ["setuptools>=68.0.0,<70.0.0"]
+requires = ["setuptools>=68.0.0,<69.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mse-lib-sgx"
 authors = [
     { name = "Cosmian Tech", email = "tech@cosmian.com" },
 ]
 description = "Library to bootstrap WSGI/ASGI application for Gramine"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 license = { text = "MIT" }
 classifiers = [
     "Development Status :: 6 - Mature",
+    "Environment :: Console",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: Implementation :: CPython"
 ]
 dependencies = [
-    "cryptography>=42.0.5,<43.0.0",
-    "intel-sgx-ra>=2.2.0,<3.0.0",
-    "hypercorn[uvloop]>=0.16.0,<0.17.0",
+    "cryptography>=41.0.1,<42.0.0",
+    "intel-sgx-ra>=2.0,<3.0",
+    "hypercorn[uvloop]>=0.14.3,<0.15.0",
     "h2>=4.1.0,<4.2.0",
-    "mse-lib-crypto>=1.4,<2.0"
+    "mse-lib-crypto>=1.3,<2.0"
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = { attr = "mse_lib_sgx.__version__" }
 
 [project.optional-dependencies]
 dev = [
-    "black>=24.3.0,<25.0.0",
-    "isort>=5.13.2,<6.0.0",
-    "pylint>=3.1.0,<4.0.0",
-    "pycodestyle>=2.11.1,<3.0.0",
+    "pylint>=2.17.4,<3.0.0",
+    "pycodestyle>=2.10.0,<3.0.0",
     "pydocstyle>=6.3.0,<7.0.0",
-    "mypy>=1.9.0,<2.0.0",
-    "pytest>=8.1.1,<9.0.0"
+    "mypy>=1.4.1,<2.0.0",
+    "black>=23.7.0,<24.0.0",
+    "isort>=5.12.0,<6.0.0",
+    "pytest>=7.4.0,<8.0.0"
 ]
 deploy = [
-    "build>=1.1.1,<2.0.0",
-    "wheel>=0.43.0,<0.44.0"
+    "build>=0.10.0,<0.11.0",
+    "wheel>=0.40.0,<0.41.0"
 ]
 
 [project.scripts]
 mse-bootstrap = "mse_lib_sgx.cli:run"
 
 [tool.pylint.MAIN]
 disable = [
```

### Comparing `mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/base64url.py` & `mse-lib-sgx-3.0a1/src/mse_lib_sgx/base64url.py`

 * *Files identical despite different names*

### Comparing `mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/certificate.py` & `mse-lib-sgx-3.0a1/src/mse_lib_sgx/certificate.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,25 +13,28 @@
 from cryptography.hazmat.primitives.serialization import (
     Encoding,
     NoEncryption,
     PrivateFormat,
     PublicFormat,
     load_pem_private_key,
 )
+from cryptography.x509.oid import NameOID
 from intel_sgx_ra.quote import Quote
 from intel_sgx_ra.ratls import SGX_QUOTE_EXTENSION_OID, get_quote_from_cert
 
 from mse_lib_sgx.sgx.quote import get_quote
 
 
 class Certificate:
     """Certificate class.
 
     Parameters
     ----------
+    enclave_id : str
+        A unique identifier acting for the CN of the root CA.
     subject_alternative_name : str
         Value subjectAltName to add in the X509 certificate.
     subject : x509.Name
         Ordered list of Relative Distinguished Names (RDNs).
         See `x509.Name`_.
     root_path : Path
         Path to store certificate and private key.
@@ -39,122 +42,159 @@
         Expiration date of the certificate.
     ratls : Optional[bytes]
         Bytes to insert in report_data of the SGX quote if RATLS certificate.
 
     Attributes
     ----------
     cert_path : Path
-        Path of the RATLS certificate created.
+        Path of the chain RATLS certificate created.
     key_path : Path
         Path of the private key.
     sk : ec.EllipticCurvePrivateKey
         Private key on SECP256R1.
     expiration_date : datetime
         Expiration date of the certificate.
     cert : x509.Certificate
         X.501 certificate.
+    ca_cert : x509.Certificate
+        X.501 root certificate.
     quote : Optional[Quote]
         Intel SGX quote to use for RATLS certificate if any.
 
     .. _x509.Name:
         https://cryptography.io/en/latest/x509/reference/#cryptography.x509.Name
 
     """
 
     def __init__(
         self,
+        enclave_id: str,
         subject_alternative_name: str,
         subject: x509.Name,
         root_path: Path,
         expiration_date: datetime,
         ratls: Optional[bytes],
     ):
         """Init constructor of SGXCertificate."""
         self.cert_path: Path = root_path / "cert.ratls.pem"
         self.key_path: Path = root_path / "key.ratls.pem"
+        self.expiration_date: datetime = expiration_date
+        self.ca_cert: x509.Certificate
+        self.quote: Optional[Quote] = None
         self.sk: ec.EllipticCurvePrivateKey = (
             ec.generate_private_key(curve=ec.SECP256R1())
             if not self.key_path.exists()
             else cast(
                 ec.EllipticCurvePrivateKey,
                 load_pem_private_key(data=self.key_path.read_bytes(), password=None),
             )
         )
-        self.expiration_date: datetime = expiration_date
-        self.cert: x509.Certificate
-        self.quote: Optional[Quote] = None
-        if self.key_path.exists() and self.cert_path.exists():
-            self.cert = x509.load_pem_x509_certificate(data=self.cert_path.read_bytes())
+
+        if self.key_path.exists() and self.cert_path:
+            certificates = x509.load_pem_x509_certificates(
+                data=self.cert_path.read_bytes()
+            )
+
+            (self.cert, self.ca_cert) = (certificates[0], certificates[1])
+
             if ratls is not None:
-                self.quote = get_quote_from_cert(self.cert)
+                self.quote = get_quote_from_cert(self.ca_cert)
+
         else:
+            ca_sk: ec.EllipticCurvePrivateKey = ec.generate_private_key(
+                curve=ec.SECP256R1()
+            )
+
             custom_extension: Optional[x509.ExtensionType] = None
             if ratls is not None:
                 pubkey_hash: bytes = hashlib.sha256(
-                    self.sk.public_key().public_bytes(
+                    ca_sk.public_key().public_bytes(
                         encoding=Encoding.X962,
                         format=PublicFormat.UncompressedPoint,
                     )
                 ).digest()
                 user_report_data: bytes = (
                     pubkey_hash + ratls if ratls is not None else pubkey_hash
                 )
                 self.quote = Quote.from_bytes(
                     get_quote(user_report_data=user_report_data)
                 )
                 custom_extension = x509.UnrecognizedExtension(
                     oid=SGX_QUOTE_EXTENSION_OID, value=bytes(self.quote)
                 )
-            self.cert = generate_x509(
+
+            # The subject of the root CA is built with the subject of the leaf certificate
+            # The CN is the name of the enclave
+            # (making easier to identify the root CA in the CA store)
+            ca_subject: x509.Name = x509.Name(
+                [
+                    subject.get_attributes_for_oid(NameOID.COUNTRY_NAME)[0],
+                    subject.get_attributes_for_oid(NameOID.STATE_OR_PROVINCE_NAME)[0],
+                    subject.get_attributes_for_oid(NameOID.LOCALITY_NAME)[0],
+                    subject.get_attributes_for_oid(NameOID.ORGANIZATION_NAME)[0],
+                    x509.NameAttribute(NameOID.COMMON_NAME, enclave_id),
+                ]
+            )
+
+            self.ca_cert = generate_x509(
+                subject=ca_subject,
+                private_key=ca_sk,
+                expiration_date=self.expiration_date,
+                custom_extension=custom_extension,
+            )
+
+            self.cert = generate_x509_from_root_ca(
                 subject_alternative_name=subject_alternative_name,
                 subject=subject,
+                issuer=ca_subject,
                 private_key=self.sk,
+                ca_private_key=ca_sk,
                 expiration_date=self.expiration_date,
-                custom_extension=custom_extension,
             )
+
             self.write(self.cert_path, self.key_path)
 
     def write(
         self, cert_path: Path, sk_path: Path, encoding: Encoding = Encoding.PEM
     ) -> None:
         """Write X509 certificate and private key to `cert_path` and `sk_path`.
 
         Parameters
         ----------
         cert_path : Path
-            Output path of the X509 certificate.
+            Output path of the X509 chain certificates.
         sk_path : Path
             Output path of the private key.
         encoding : Encoding
             Encoding used to write X509 certificate.
 
         """
-        cert_path.write_bytes(self.cert.public_bytes(encoding))
+        cert_path.write_bytes(
+            self.cert.public_bytes(encoding) + self.ca_cert.public_bytes(encoding)
+        )
+
         sk_path.write_bytes(
             self.sk.private_bytes(
                 encoding=Encoding.PEM,
                 format=PrivateFormat.PKCS8,
                 encryption_algorithm=NoEncryption(),
             )
         )
 
 
 def generate_x509(
-    subject_alternative_name: str,
     subject: x509.Name,
     private_key: ec.EllipticCurvePrivateKey,
     expiration_date: datetime,
     custom_extension: Optional[x509.ExtensionType] = None,
 ) -> x509.Certificate:
     """Build a self-signed X509 certificate given parameters.
 
     Parameters
     ----------
-    subject_alternative_name : str
-        Value subjectAltName to add in the X509 certificate.
     subject : x509.Name
         Ordered list of Relative Distinguished Names (RDNs).
         See `x509.Name`_.
     private_key : ec.EllipticCurvePrivateKey
         Private key to sign the X509 certificate.
     expiration_date : datetime
         Expiration date of the X509 certificate.
@@ -168,44 +208,98 @@
 
     .. _x509.Name:
         https://cryptography.io/en/latest/x509/reference/#cryptography.x509.Name
 
     """
     issuer: x509.Name = subject  # issuer=subject for self-signed certificate
 
+    builder: x509.CertificateBuilder = x509.CertificateBuilder()
+
+    builder = (
+        builder.subject_name(subject)
+        .issuer_name(issuer)
+        .public_key(private_key.public_key())
+        .serial_number(x509.random_serial_number())
+        .not_valid_before(datetime.utcnow())
+        .not_valid_after(expiration_date)
+    )
+
+    builder = builder.add_extension(
+        x509.BasicConstraints(ca=True, path_length=None),
+        critical=False,
+    )
+
+    if custom_extension is not None:
+        builder = builder.add_extension(custom_extension, critical=False)
+
+    return builder.sign(private_key=private_key, algorithm=hashes.SHA256())
+
+
+def generate_x509_from_root_ca(
+    subject_alternative_name: str,
+    subject: x509.Name,
+    issuer: x509.Name,
+    private_key: ec.EllipticCurvePrivateKey,
+    ca_private_key: ec.EllipticCurvePrivateKey,
+    expiration_date: datetime,
+) -> x509.Certificate:
+    """Build a self-signed X509 certificate given parameters.
+
+    Parameters
+    ----------
+    subject_alternative_name : str
+        Value subjectAltName to add in the X509 certificate.
+    subject : x509.Name
+        Ordered list of Relative Distinguished Names (RDNs).
+        See `x509.Name`_.
+    issuer : x509.Name
+        Ordered list of Relative Distinguished Names (RDNs).
+        See `x509.Name`_.
+    private_key : ec.EllipticCurvePrivateKey
+        Private key to sign the X509 certificate.
+    expiration_date : datetime
+        Expiration date of the X509 certificate.
+
+    Returns
+    -------
+    x509.Certificate
+        X509 certificate with input parameters.
+
+    .. _x509.Name:
+        https://cryptography.io/en/latest/x509/reference/#cryptography.x509.Name
+
+    """
     san: Union[x509.IPAddress, x509.DNSName]
     try:
         san = x509.IPAddress(ipaddress.ip_address(subject_alternative_name))
     except ValueError:
         san = x509.DNSName(subject_alternative_name)
 
+    csr = (
+        x509.CertificateSigningRequestBuilder()
+        .subject_name(subject)
+        .sign(private_key=private_key, algorithm=hashes.SHA256())
+    )
+
     builder: x509.CertificateBuilder = x509.CertificateBuilder()
 
     builder = (
-        builder.subject_name(subject)
+        builder.subject_name(csr.subject)
         .issuer_name(issuer)
-        .public_key(private_key.public_key())
+        .public_key(csr.public_key())
         .serial_number(x509.random_serial_number())
         .not_valid_before(datetime.utcnow())
         .not_valid_after(expiration_date)
         .add_extension(
             x509.SubjectAlternativeName([san]),
             critical=False,
         )
     )
 
-    if custom_extension is not None:
-        builder = builder.add_extension(custom_extension, critical=False)
-
-    builder = builder.add_extension(
-        x509.BasicConstraints(ca=True, path_length=None),
-        critical=True,
-    )
-
-    return builder.sign(private_key=private_key, algorithm=hashes.SHA256())
+    return builder.sign(private_key=ca_private_key, algorithm=hashes.SHA256())
 
 
 def to_wildcard_domain(domain: str) -> str:
     """Transform domain to wildcard domain.
 
     Parameters
     ----------
```

### Comparing `mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/cli.py` & `mse-lib-sgx-3.0a1/src/mse_lib_sgx/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,14 +184,15 @@
         if len(enclave_sk) != 32:
             raise SecurityError("Bad enclave sk length!")
 
         if x25519_pk_from_sk(enclave_sk) != enclave_pk:
             raise SecurityError("Malformed enclave's keypair!")
 
     cert: Certificate = Certificate(
+        enclave_id=str(args.id),
         subject_alternative_name=args.san if args.san else "localhost",
         subject=(
             x509.Name.from_rfc4514_string(args.subject)
             if args.subject
             else globs.SUBJECT
         ),
         root_path=globs.KEY_DIR_PATH,
```

### Comparing `mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/copy.py` & `mse-lib-sgx-3.0a1/src/mse_lib_sgx/copy.py`

 * *Files identical despite different names*

### Comparing `mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/globs.py` & `mse-lib-sgx-3.0a1/src/mse_lib_sgx/globs.py`

 * *Files identical despite different names*

### Comparing `mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/http_server.py` & `mse-lib-sgx-3.0a1/src/mse_lib_sgx/http_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 import logging
 import ssl
 import threading
 import time
 from http.server import BaseHTTPRequestHandler, HTTPServer
-from typing import Any, Dict, Optional
+from typing import Optional
 from uuid import UUID
 
 from mse_lib_crypto.seal_box import unseal
 
 from mse_lib_sgx import globs
 from mse_lib_sgx.base64url import base64url_decode
 from mse_lib_sgx.certificate import Certificate
@@ -60,28 +60,24 @@
             data = json.loads(body.decode("utf8"))
 
             if app_secrets := data.get("app_secrets"):
                 globs.SECRETS_PATH.parent.mkdir(parents=True, exist_ok=True)
                 globs.SECRETS_PATH.write_bytes(json.dumps(app_secrets).encode("utf-8"))
 
             if app_sealed_secrets := data.get("app_sealed_secrets"):
-                content: Dict[str, Any] = json.loads(
-                    unseal(
-                        base64url_decode(app_sealed_secrets),
-                        globs.ENCLAVE_SK_PATH.read_bytes(),
-                    )
-                )
-                if "code_secret_key" in content:
-                    globs.CODE_SECRET_KEY = bytes.fromhex(content["code_secret_key"])
-
-                    if len(globs.CODE_SECRET_KEY) != 32:
-                        raise CryptoError("Incorrect key length!")
                 globs.SEALED_SECRETS_PATH.parent.mkdir(parents=True, exist_ok=True)
                 globs.SEALED_SECRETS_PATH.write_bytes(
-                    json.dumps(content).encode("utf-8")
+                    json.dumps(
+                        json.loads(
+                            unseal(
+                                base64url_decode(app_sealed_secrets),
+                                globs.ENCLAVE_SK_PATH.read_bytes(),
+                            )
+                        )
+                    ).encode("utf-8")
                 )
 
             # Do not process queries which have not the `uuid` data field
             # Probably a robot
             if UUID(data["uuid"]) != globs.ID:
                 self.send_response_only(401)
                 self.end_headers()
```

### Comparing `mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/sgx/key.py` & `mse-lib-sgx-3.0a1/src/mse_lib_sgx/sgx/key.py`

 * *Files identical despite different names*

### Comparing `mse-lib-sgx-2.3.0a4/src/mse_lib_sgx/sgx/quote.py` & `mse-lib-sgx-3.0a1/src/mse_lib_sgx/sgx/quote.py`

 * *Files identical despite different names*

### Comparing `mse-lib-sgx-2.3.0a4/src/mse_lib_sgx.egg-info/PKG-INFO` & `mse-lib-sgx-3.0a1/src/mse_lib_sgx.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,23 @@
 Metadata-Version: 2.1
 Name: mse-lib-sgx
-Version: 2.3.0a4
+Version: 3.0a1
 Summary: Library to bootstrap WSGI/ASGI application for Gramine
 Author-email: Cosmian Tech <tech@cosmian.com>
 License: MIT
 Classifier: Development Status :: 6 - Mature
+Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: cryptography<43.0.0,>=42.0.5
-Requires-Dist: intel-sgx-ra<3.0.0,>=2.2.0
-Requires-Dist: hypercorn[uvloop]<0.17.0,>=0.16.0
-Requires-Dist: h2<4.2.0,>=4.1.0
-Requires-Dist: mse-lib-crypto<2.0,>=1.4
 Provides-Extra: dev
-Requires-Dist: black<25.0.0,>=24.3.0; extra == "dev"
-Requires-Dist: isort<6.0.0,>=5.13.2; extra == "dev"
-Requires-Dist: pylint<4.0.0,>=3.1.0; extra == "dev"
-Requires-Dist: pycodestyle<3.0.0,>=2.11.1; extra == "dev"
-Requires-Dist: pydocstyle<7.0.0,>=6.3.0; extra == "dev"
-Requires-Dist: mypy<2.0.0,>=1.9.0; extra == "dev"
-Requires-Dist: pytest<9.0.0,>=8.1.1; extra == "dev"
 Provides-Extra: deploy
-Requires-Dist: build<2.0.0,>=1.1.1; extra == "deploy"
-Requires-Dist: wheel<0.44.0,>=0.43.0; extra == "deploy"
 
 # MicroService Encryption Lib SGX
 
 ## Overview
 
 MSE lib SGX bootstraps the execution of an encrypted ASGI/WSGI Python web application for [Gramine](https://gramine.readthedocs.io/).
```

### Comparing `mse-lib-sgx-2.3.0a4/src/mse_lib_sgx.egg-info/SOURCES.txt` & `mse-lib-sgx-3.0a1/src/mse_lib_sgx.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 src/mse_lib_sgx/base64url.py
 src/mse_lib_sgx/certificate.py
 src/mse_lib_sgx/cli.py
 src/mse_lib_sgx/copy.py
 src/mse_lib_sgx/error.py
 src/mse_lib_sgx/globs.py
 src/mse_lib_sgx/http_server.py
-src/mse_lib_sgx/py.typed
 src/mse_lib_sgx.egg-info/PKG-INFO
 src/mse_lib_sgx.egg-info/SOURCES.txt
 src/mse_lib_sgx.egg-info/dependency_links.txt
 src/mse_lib_sgx.egg-info/entry_points.txt
 src/mse_lib_sgx.egg-info/requires.txt
 src/mse_lib_sgx.egg-info/top_level.txt
 src/mse_lib_sgx/sgx/__init__.py
```

### Comparing `mse-lib-sgx-2.3.0a4/tests/test_cert_utils.py` & `mse-lib-sgx-3.0a1/tests/test_cert_utils.py`

 * *Files identical despite different names*

### Comparing `mse-lib-sgx-2.3.0a4/tests/test_conf_server.py` & `mse-lib-sgx-3.0a1/tests/test_conf_server.py`

 * *Files identical despite different names*

