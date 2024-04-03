# Comparing `tmp/bibt_gcp_storage-0.0.8.tar.gz` & `tmp/bibt_gcp_storage-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Jan 10 16:45:46 2024, max compression
+gzip compressed data, last modified: Wed Jan 10 20:30:50 2024, max compression
```

## Comparing `bibt_gcp_storage-0.0.8.tar` & `bibt_gcp_storage-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      441 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/.bumpversion.cfg
--rw-r--r--   0        0        0     1259 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      483 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/.readthedocs.yml
--rw-r--r--   0        0        0      288 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0        0 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/MANIFEST.in
--rw-r--r--   0        0        0       52 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/requirements-dev.txt
--rw-r--r--   0        0        0       29 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/requirements.txt
--rw-r--r--   0        0        0       17 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/.github/CODEOWNERS
--rw-r--r--   0        0        0      142 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/.github/dependabot.yml
--rw-r--r--   0        0        0     2493 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0        0        0      212 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/bibt/gcp/storage/__init__.py
--rw-r--r--   0        0        0     7951 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/bibt/gcp/storage/classes.py
--rw-r--r--   0        0        0     1186 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/bibt/gcp/storage/methods.py
--rw-r--r--   0        0        0       20 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/bibt/gcp/storage/params.py
--rw-r--r--   0        0        0       22 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/bibt/gcp/storage/version.py
--rw-r--r--   0        0        0      634 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/docs/Makefile
--rw-r--r--   0        0        0     2757 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/docs/conf.py
--rw-r--r--   0        0        0     2456 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/docs/contributing.rst
--rw-r--r--   0        0        0     2428 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/docs/index.rst
--rw-r--r--   0        0        0      790 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/docs/make.bat
--rw-r--r--   0        0        0       32 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/docs/requirements.txt
--rw-r--r--   0        0        0    15093 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/docs/_static/bibt.ico
--rw-r--r--   0        0        0     2125 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/docs/_static/custom.css
--rw-r--r--   0        0        0      273 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/docs/modules/storage.rst
--rw-r--r--   0        0        0        0 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/tests/test.py
--rw-r--r--   0        0        0     3945 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/.gitignore
--rw-r--r--   0        0        0     1054 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/LICENSE
--rw-r--r--   0        0        0     1204 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/README.md
--rw-r--r--   0        0        0     1149 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2266 2024-01-10 16:45:46.000000 bibt_gcp_storage-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      441 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/.bumpversion.cfg
+-rw-r--r--   0        0        0     1259 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      483 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/.readthedocs.yml
+-rw-r--r--   0        0        0      288 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/MANIFEST.in
+-rw-r--r--   0        0        0       52 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/requirements-dev.txt
+-rw-r--r--   0        0        0       29 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/requirements.txt
+-rw-r--r--   0        0        0       17 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/.github/CODEOWNERS
+-rw-r--r--   0        0        0      142 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     2493 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0        0        0      212 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/bibt/gcp/storage/__init__.py
+-rw-r--r--   0        0        0     8252 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/bibt/gcp/storage/classes.py
+-rw-r--r--   0        0        0     1186 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/bibt/gcp/storage/methods.py
+-rw-r--r--   0        0        0       20 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/bibt/gcp/storage/params.py
+-rw-r--r--   0        0        0       22 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/bibt/gcp/storage/version.py
+-rw-r--r--   0        0        0      634 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/docs/Makefile
+-rw-r--r--   0        0        0     2757 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/docs/conf.py
+-rw-r--r--   0        0        0     2456 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/docs/contributing.rst
+-rw-r--r--   0        0        0     2428 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/docs/index.rst
+-rw-r--r--   0        0        0      790 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/docs/make.bat
+-rw-r--r--   0        0        0       32 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/docs/requirements.txt
+-rw-r--r--   0        0        0    15093 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/docs/_static/bibt.ico
+-rw-r--r--   0        0        0     2125 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/docs/_static/custom.css
+-rw-r--r--   0        0        0      273 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/docs/modules/storage.rst
+-rw-r--r--   0        0        0        0 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/tests/test.py
+-rw-r--r--   0        0        0     3945 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1054 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1204 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/README.md
+-rw-r--r--   0        0        0     1149 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2266 2024-01-10 20:30:50.000000 bibt_gcp_storage-0.0.9/PKG-INFO
```

### Comparing `bibt_gcp_storage-0.0.8/.pre-commit-config.yaml` & `bibt_gcp_storage-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bibt_gcp_storage-0.0.8/.github/workflows/publish-to-pypi.yaml` & `bibt_gcp_storage-0.0.9/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `bibt_gcp_storage-0.0.8/bibt/gcp/storage/classes.py` & `bibt_gcp_storage-0.0.9/bibt/gcp/storage/classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,24 +22,32 @@
         gcloud account.
     """
 
     def __init__(self, project_id=None, credentials=None):
         self._client = storage.Client(project=project_id, credentials=credentials)
 
     def _ensure_valid_client(self):
-        if not self._client._transport._credentials.valid:
+        if (
+            not self._client._transport._credentials.valid
+            or not self._client._transport._credentials.expiry
+        ):
             logging.info(
                 "Refreshing client credentials, token expired: "
                 f"[{self._client._transport._credentials.expiry}]"
             )
             request = google.auth.transport.requests.Request()
             self._client._transport._credentials.refresh(request=request)
             logging.info(
                 f"New expiration: [{self._client._transport._credentials.expiry}]"
             )
+        else:
+            logging.debug(
+                f"Token is valid: [{self._client._transport._credentials.valid}] "
+                f"expires: [{self._client._transport._credentials.expiry}]"
+            )
         return
 
     def create_bucket(self, bucket_name, project_id=None, location="US"):
         """Creates a bucket in GCS.
 
         :param str bucket_name: The desired name for the bucket. Note that
             bucket names must be **universally** unique in GCP, and need to
```

### Comparing `bibt_gcp_storage-0.0.8/bibt/gcp/storage/methods.py` & `bibt_gcp_storage-0.0.9/bibt/gcp/storage/methods.py`

 * *Files identical despite different names*

### Comparing `bibt_gcp_storage-0.0.8/docs/Makefile` & `bibt_gcp_storage-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bibt_gcp_storage-0.0.8/docs/conf.py` & `bibt_gcp_storage-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bibt_gcp_storage-0.0.8/docs/contributing.rst` & `bibt_gcp_storage-0.0.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bibt_gcp_storage-0.0.8/docs/index.rst` & `bibt_gcp_storage-0.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bibt_gcp_storage-0.0.8/docs/make.bat` & `bibt_gcp_storage-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bibt_gcp_storage-0.0.8/docs/_static/bibt.ico` & `bibt_gcp_storage-0.0.9/docs/_static/bibt.ico`

 * *Files identical despite different names*

### Comparing `bibt_gcp_storage-0.0.8/docs/_static/custom.css` & `bibt_gcp_storage-0.0.9/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `bibt_gcp_storage-0.0.8/.gitignore` & `bibt_gcp_storage-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bibt_gcp_storage-0.0.8/LICENSE` & `bibt_gcp_storage-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bibt_gcp_storage-0.0.8/README.md` & `bibt_gcp_storage-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bibt_gcp_storage-0.0.8/pyproject.toml` & `bibt_gcp_storage-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -21,13 +21,13 @@
   "Topic :: Utilities",
 ]
 dependencies = ["google-cloud-storage==2.14.0"]
 description = "Functionality often used by BITS Blue Team (GCP GCS)."
 name = "bibt-gcp-storage"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.7"
-version = "0.0.8"
+version = "0.0.9"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/broadinstitute/bibt-gcp-storage/issues"
 "Documentation" = "https://bibt-gcp-storage.readthedocs.io/en/latest/"
 "Homepage" = "https://github.com/broadinstitute/bibt-gcp-storage"
```

### Comparing `bibt_gcp_storage-0.0.8/PKG-INFO` & `bibt_gcp_storage-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibt-gcp-storage
-Version: 0.0.8
+Version: 0.0.9
 Summary: Functionality often used by BITS Blue Team (GCP GCS).
 Project-URL: Bug Tracker, https://github.com/broadinstitute/bibt-gcp-storage/issues
 Project-URL: Documentation, https://bibt-gcp-storage.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/broadinstitute/bibt-gcp-storage
 Author-email: Matthew OBrien <mobrien@broadinstitute.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

