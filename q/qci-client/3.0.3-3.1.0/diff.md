# Comparing `tmp/qci-client-3.0.3.tar.gz` & `tmp/qci-client-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qci-client-3.0.3.tar", last modified: Wed Mar  6 18:30:33 2024, max compression
+gzip compressed data, was "qci-client-3.1.0.tar", last modified: Wed Apr  3 20:05:50 2024, max compression
```

## Comparing `qci-client-3.0.3.tar` & `qci-client-3.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 mcampanelli   (501) staff       (20)        0 2024-03-06 18:30:33.971985 qci-client-3.0.3/
--rw-r--r--   0 mcampanelli   (501) staff       (20)      167 2023-02-23 22:37:33.000000 qci-client-3.0.3/.gitignore
--rw-r--r--   0 mcampanelli   (501) staff       (20)     3869 2024-03-05 23:45:00.000000 qci-client-3.0.3/.gitlab-ci.yml
--rw-r--r--   0 mcampanelli   (501) staff       (20)      531 2024-03-05 23:45:00.000000 qci-client-3.0.3/.mega-linter.yml
--rw-r--r--   0 mcampanelli   (501) staff       (20)    11354 2023-07-19 19:20:38.000000 qci-client-3.0.3/LICENSE
--rw-r--r--   0 mcampanelli   (501) staff       (20)       56 2023-07-20 19:36:36.000000 qci-client-3.0.3/MANIFEST.in
--rw-r--r--   0 mcampanelli   (501) staff       (20)     1625 2024-03-06 18:30:33.971758 qci-client-3.0.3/PKG-INFO
--rw-r--r--   0 mcampanelli   (501) staff       (20)      552 2024-03-05 23:45:00.000000 qci-client-3.0.3/README.md
--rw-r--r--   0 mcampanelli   (501) staff       (20)     2529 2024-03-05 23:45:00.000000 qci-client-3.0.3/pyproject.toml
-drwxr-xr-x   0 mcampanelli   (501) staff       (20)        0 2024-03-06 18:30:33.968293 qci-client-3.0.3/qci_client/
--rw-r--r--   0 mcampanelli   (501) staff       (20)      136 2024-02-27 04:03:58.000000 qci-client-3.0.3/qci_client/__init__.py
--rw-r--r--   0 mcampanelli   (501) staff       (20)     5744 2024-03-05 23:45:00.000000 qci-client-3.0.3/qci_client/base.py
--rw-r--r--   0 mcampanelli   (501) staff       (20)     5019 2024-03-05 23:45:00.000000 qci-client-3.0.3/qci_client/data_converter.py
--rw-r--r--   0 mcampanelli   (501) staff       (20)     1587 2024-02-27 04:03:58.000000 qci-client-3.0.3/qci_client/enum.py
--rw-r--r--   0 mcampanelli   (501) staff       (20)    26600 2024-03-05 23:45:00.000000 qci-client-3.0.3/qci_client/qci_client.py
--rw-r--r--   0 mcampanelli   (501) staff       (20)    11873 2024-02-27 04:03:58.000000 qci-client-3.0.3/qci_client/types.py
--rw-r--r--   0 mcampanelli   (501) staff       (20)    16130 2024-03-01 00:49:55.000000 qci-client-3.0.3/qci_client/utilities.py
-drwxr-xr-x   0 mcampanelli   (501) staff       (20)        0 2024-03-06 18:30:33.970773 qci-client-3.0.3/qci_client.egg-info/
--rw-r--r--   0 mcampanelli   (501) staff       (20)     1625 2024-03-06 18:30:33.000000 qci-client-3.0.3/qci_client.egg-info/PKG-INFO
--rw-r--r--   0 mcampanelli   (501) staff       (20)      513 2024-03-06 18:30:33.000000 qci-client-3.0.3/qci_client.egg-info/SOURCES.txt
--rw-r--r--   0 mcampanelli   (501) staff       (20)        1 2024-03-06 18:30:33.000000 qci-client-3.0.3/qci_client.egg-info/dependency_links.txt
--rw-r--r--   0 mcampanelli   (501) staff       (20)      240 2024-03-06 18:30:33.000000 qci-client-3.0.3/qci_client.egg-info/requires.txt
--rw-r--r--   0 mcampanelli   (501) staff       (20)       17 2024-03-06 18:30:33.000000 qci-client-3.0.3/qci_client.egg-info/top_level.txt
--rw-r--r--   0 mcampanelli   (501) staff       (20)       38 2024-03-06 18:30:33.972029 qci-client-3.0.3/setup.cfg
-drwxr-xr-x   0 mcampanelli   (501) staff       (20)        0 2024-03-06 18:30:33.970363 qci-client-3.0.3/tests/
--rw-r--r--   0 mcampanelli   (501) staff       (20)        0 2023-02-23 22:37:33.000000 qci-client-3.0.3/tests/__init__.py
--rw-r--r--   0 mcampanelli   (501) staff       (20)    12057 2024-03-01 00:49:55.000000 qci-client-3.0.3/tests/test_data_converter.py
--rw-r--r--   0 mcampanelli   (501) staff       (20)    28774 2024-03-05 23:45:00.000000 qci-client-3.0.3/tests/test_qci_client.py
--rw-r--r--   0 mcampanelli   (501) staff       (20)     5175 2024-03-01 00:49:55.000000 qci-client-3.0.3/tests/test_remote_jobs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:05:50.506949 qci-client-3.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-03 20:02:27.000000 qci-client-3.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5375 2024-04-03 20:02:27.000000 qci-client-3.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-03 20:02:27.000000 qci-client-3.1.0/.mega-linter.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11354 2024-04-03 20:02:27.000000 qci-client-3.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-03 20:02:27.000000 qci-client-3.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2157 2024-04-03 20:05:50.506949 qci-client-3.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-03 20:02:27.000000 qci-client-3.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2024-04-03 20:02:27.000000 qci-client-3.1.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:05:50.502949 qci-client-3.1.0/qci_client/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5234 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/data_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)    26746 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/qci_client.py
+-rw-rw-rw-   0 root         (0) root         (0)    13005 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/types.py
+-rw-rw-rw-   0 root         (0) root         (0)    16140 2024-04-03 20:02:27.000000 qci-client-3.1.0/qci_client/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:05:50.502949 qci-client-3.1.0/qci_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2157 2024-04-03 20:05:50.000000 qci-client-3.1.0/qci_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2024-04-03 20:05:50.000000 qci-client-3.1.0/qci_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 20:05:50.000000 qci-client-3.1.0/qci_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      264 2024-04-03 20:05:50.000000 qci-client-3.1.0/qci_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-03 20:05:50.000000 qci-client-3.1.0/qci_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 20:05:50.506949 qci-client-3.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:05:50.502949 qci-client-3.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 20:02:27.000000 qci-client-3.1.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12057 2024-04-03 20:02:27.000000 qci-client-3.1.0/tests/test_data_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)    29749 2024-04-03 20:02:27.000000 qci-client-3.1.0/tests/test_qci_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     7826 2024-04-03 20:02:27.000000 qci-client-3.1.0/tests/test_remote_jobs.py
```

### Comparing `qci-client-3.0.3/.gitlab-ci.yml` & `qci-client-3.1.0/.gitlab-ci.yml`

 * *Files 23% similar despite different names*

```diff
@@ -61,14 +61,66 @@
   artifacts:
     name: $CI_PROJECT_NAME-$CI_COMMIT_TAG
     when: always
     paths:
       - dist
     expire_in: never
 
+docs-branch:
+  stage: build
+  rules:
+    - if: $CI_COMMIT_BRANCH
+  <<: *build_module
+  script:
+    - echo Creating documentation artifact that expires in 1 week.
+    - apt-get install -y --no-install-recommends zip
+    - cd docs
+    - mkdir dist
+    - mkdir dist/html
+    - mkdir dist/xml
+    - make clean
+    - sphinx-build -b html source build/html
+    - sphinx-build -b xml source build/xml
+    - cd build/html
+    - zip -r ../../dist/html/${CI_PROJECT_NAME}-docs-${CI_COMMIT_BRANCH}-${CI_COMMIT_SHORT_SHA}.zip *
+    - cd ../xml
+    - zip -r ../../dist/xml/${CI_PROJECT_NAME}-docs-${CI_COMMIT_BRANCH}-${CI_COMMIT_SHORT_SHA}.zip *.xml
+  artifacts:
+    name: $CI_PROJECT_NAME-docs-$CI_COMMIT_BRANCH-$CI_COMMIT_SHORT_SHA
+    when: always
+    paths:
+      - docs/dist
+    expire_in: 1 week
+
+docs-tag:
+  stage: build
+  rules:
+    - if: '$CI_COMMIT_TAG =~ /^v[0-9]+\.[0-9]+\.[0-9]+$/' # Enforce semver in tag.
+  <<: *build_module
+  script:
+    - echo Creating documentation artifact that expires never.
+    - apt-get install -y --no-install-recommends zip
+    - cd docs
+    - mkdir dist
+    - mkdir dist/html
+    - mkdir dist/xml
+    - make clean
+    - sphinx-build -b html source build/html
+    - sphinx-build -b xml source build/xml
+    - cd build/html
+    - zip -r ../../dist/html/${CI_PROJECT_NAME}-docs-${CI_COMMIT_BRANCH}-${CI_COMMIT_SHORT_SHA}.zip *
+    - cd ../xml
+    - zip -r ../../dist/xml/${CI_PROJECT_NAME}-docs-${CI_COMMIT_BRANCH}-${CI_COMMIT_SHORT_SHA}.zip *.xml
+  artifacts:
+    name: $CI_PROJECT_NAME-docs-$CI_COMMIT_BRANCH-$CI_COMMIT_SHORT_SHA
+    when: always
+    paths:
+      - docs/dist
+    expire_in: never
+
 code-check-semgrep:
   stage: test
   allow_failure: true
   image: returntocorp/semgrep-agent:v1
   variables:
     SEMGREP_RULES: >-
       p/security-audit
@@ -106,16 +158,14 @@
     - python -m coverage run --source=qci_client -m pytest -v -m "offline and not timing"
     - python -m coverage report -m
     # Python linters/autoformatters.
     # - python -m pylint .
     # - python -m black --check .
   parallel:
     matrix:
-      # Include Python 3.11 in matrix once supported, tested, and CI build works.
-      # See QCIEN-2174 and QCIEN-2147.
       - PYTHON_VERSION: ['3.8.18', '3.9.18', '3.10.13', '3.11.8', '3.12.2']
 
 publish-package-dev:
   stage: publish
   rules:
     - if: '$CI_COMMIT_TAG =~ /^v[0-9]+\.[0-9]+\.[0-9]+$/' # Enforce semver in tag.
   <<: *build_module
```

### Comparing `qci-client-3.0.3/.mega-linter.yml` & `qci-client-3.1.0/.mega-linter.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ---
 # Configuration file for MegaLinter
 # See all available variables at https://megalinter.github.io/configuration/ and in linters documentation
 
 APPLY_FIXES: none # all, none, or list of linter keys
+EXCLUDED_DIRECTORIES: ["docs"]
 DISABLE:
   - SPELL
 DISABLE_ERRORS_LINTERS:
   - COPYPASTE_JSCPD
   - REPOSITORY_DEVSKIM
 DISABLE_LINTERS:
   - PYTHON_BLACK  # done elsewhere
```

### Comparing `qci-client-3.0.3/LICENSE` & `qci-client-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qci-client-3.0.3/PKG-INFO` & `qci-client-3.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: qci-client
-Version: 3.0.3
+Version: 3.1.0
 Summary: Client Package for using Qatalyst Optimization Suite
 Author: Quantum Computing Inc.
 Author-email: support@quantumcomputinginc.com
 License: Apache 2.0
-Project-URL: documentation, https://qatalyst.quantumcomputinginc.com
+Project-URL: documentation, https://quantumcomputinginc.com/learn/reference-documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests<3,>=2.22.1
@@ -20,14 +20,15 @@
 Provides-Extra: dev
 Requires-Dist: black==23.1.0; extra == "dev"
 Requires-Dist: build<0.11,>=0.10.0; extra == "dev"
 Requires-Dist: check-manifest<0.49,>=0.48; extra == "dev"
 Requires-Dist: coverage[toml]<7,>=6.4.2; extra == "dev"
 Requires-Dist: pylint==2.16.2; extra == "dev"
 Requires-Dist: pytest<8,>=7.2.1; extra == "dev"
+Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "dev"
 Requires-Dist: twine<4,>=3.7.1; extra == "dev"
 
 # QCI Client
 
 ## Getting started
 
 ### Installation
@@ -38,16 +39,35 @@
 Install `qci-client` from the [public PyPI server](https://pypi.org/)
 into your Python virtual environment using--
 
 ```bash
 pip install qci-client
 ```
 
-### Environment Variables
+### Instantiating a Client
 
-These environment variables must be set in order to access the API--
+#### With Environment Variables
+
+To access the API, set these environment variables--
 
-- QCI_TOKEN - token for Qatalyst API
 <!-- markdown-link-check-disable-next-line -->
-- QCI_API_URL - Example: "https://api.qci-prod.com"
+- QCI_API_URL - URL for Qatalyst API, Example: "https://api.qci-prod.com"
+- QCI_TOKEN - refresh token string for securely accessing Qatalyst API
+
+then instantiate a `QciClient` as follows--
+
+```python
+from qci_client import QciClient
+
+client = QciClient()
+```
+
+#### Without Environment Variables
 
+Access the API without first defining environment variables by instantiating a
+`QciClient` as follows--
 
+```python
+from qci_client import QciClient
+
+client = QciClient(url="https://api.qci-prod.com", api_token="<secret-token>")
+```
```

### Comparing `qci-client-3.0.3/pyproject.toml` & `qci-client-3.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -54,19 +54,20 @@
     "build >=0.10.0, <0.11",
     "check-manifest >=0.48, <0.49",
     "coverage[toml] >=6.4.2, <7",
     # Try to match pylint version in megalinter that runs in CI:
     # https://github.com/oxsecurity/megalinter/blob/main/docs/descriptors/python_pylint.md#pylint-documentation
     "pylint ==2.16.2",
     "pytest >=7.2.1, <8",
+    "sphinx-rtd-theme >=1.3.0",
     "twine >=3.7.1, <4"
 ]
 
 [project.urls]
-    documentation = "https://qatalyst.quantumcomputinginc.com"
+    documentation = "https://quantumcomputinginc.com/learn/reference-documentation"
 
 [tool.setuptools.packages.find]
 include = [
   "qci_client",
   "tests",
 ]
 
@@ -82,12 +83,12 @@
 [tool.coverage.report]
 # FUTURE Get 100% coverage.
 # fail_under = 100
 
 [tool.pylint]
 max-line-length = 88
 recursive = true
-ignore = ["build"]
+ignore = ["build", "docs"]
 disable = [
     "duplicate-code",
     "line-too-long",
 ]
```

### Comparing `qci-client-3.0.3/qci_client/base.py` & `qci-client-3.1.0/qci_client/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,104 +1,100 @@
 """Base class for API clients."""
 
 from dataclasses import dataclass, field
+from datetime import datetime
 import functools
 import os
 from posixpath import join
-import time
-from typing import Callable, Dict, Optional
+from typing import Callable, Optional
 
 import requests
 from requests.adapters import HTTPAdapter, Retry
 
 # We are uploading files we want to retry when we receive certain error codes
 RETRY_TOTAL = 7
 BACKOFF_FACTOR = 2
 STATUS_FORCELIST = [502, 503, 504]
 
 
 @dataclass
 class BaseApi:  # pylint: disable=too-many-instance-attributes
-    """Base class for API clients."""
+    """
+    Base class for clients to QCi APIs, especially the authorization layer.
 
+    :param url: url basepath to API endpoint, including scheme, if None, then falls back
+        to QCI_API_URL environment variable
+    :param api_token: refresh token for authenticating to API, if None, then falls back
+        to QCI_TOKEN environment variable
+    :param access_tokens: url path fragment to specify access-tokens API endpoint
+    :param set_bearer_token_on_init: flag to turn on/off access token retrieval on
+        object initialization
+    :param timeout: number of seconds before timing out requests, None waits indefinitely
+    :param debug: flag to turn on/off debug prints
+    """
+
+    url: Optional[str] = None
     # Hide sensistive info to prevent accidental logging when printing client objects.
-    _bearer_info: dict = field(default_factory=dict, repr=False)
     api_token: Optional[str] = field(default=None, repr=False)
+    access_tokens: str = "auth/v1/access-tokens"
     set_bearer_token_on_init: bool = True
-
-    # User-definable url's and endpoints
-    url: Optional[str] = None
-    authorize: Optional[str] = None
-
-    # Default endpoints and url
-    _authorize: str = "auth/v1/access-tokens"
-    _download: str = "contents"
-    _add_headers: Optional[Dict[str, str]] = None
-
-    # Constants
-    _user_not_authorized: str = "user not authorized"
-
     # Request timeout in seconds for connection & read. None for infinite timeout.
-    timeout: Optional[float] = 5 * 60.0
-
+    timeout: Optional[float] = None
     debug: bool = False
 
     def __post_init__(self):
-        self.api_token = self.api_token if self.api_token else os.getenv("QCI_TOKEN")
-        if self.api_token is None:
-            raise AssertionError(
-                "QCI_TOKEN environment variable is empty. Specify api_token or add the "
-                "necessary environment variable"
-            )
-
         self.url = self.url if self.url else os.getenv("QCI_API_URL")
+
         if self.url is None:
             raise AssertionError(
                 "QCI_API_URL environment variable is empty. Specify url or add the "
                 "necessary environment variable"
             )
 
         # removing trailling / so can add paths simply
         self.url.rstrip("/")
 
-        self.authorize = self.authorize if self.authorize else self._authorize
+        self.api_token = self.api_token if self.api_token else os.getenv("QCI_TOKEN")
+
+        if self.api_token is None:
+            raise AssertionError(
+                "QCI_TOKEN environment variable is empty. Specify api_token or add the "
+                "necessary environment variable"
+            )
 
         self.session = requests.Session()
         retries = Retry(
             total=RETRY_TOTAL,
             backoff_factor=BACKOFF_FACTOR,
             status_forcelist=STATUS_FORCELIST,
         )
         self.session.mount("https://", HTTPAdapter(max_retries=retries))
 
+        self._bearer_info = {}
+
         if self.set_bearer_token_on_init:
             self.set_bearer_token()
 
     @property
     def auth_url(self) -> str:
         """Return the URL used for authorization."""
-
-        return join(self.url, self.authorize)
+        return join(self.url, self.access_tokens)
 
     @property
     def headers_without_token(self):
         """Headers without cached bearer token."""
         headers = {
             "Content-Type": "application/json",
             "Connection": "close",
         }
 
         if self.timeout is not None:
             # Provide client's request timeout to server (latency provides some buffer).
             headers.update({"X-Request-Timeout-Nano": str(int(10**9 * self.timeout))})
 
-        # allow additional headers to be passed through
-        if self._add_headers is not None:
-            headers.update(self._add_headers)
-
         return headers
 
     @property
     def headers(self):
         """Headers with cached bearer token."""
         headers = self.headers_without_token
         headers["Authorization"] = f"Bearer {self._bearer_info.get('access_token', '')}"
@@ -141,21 +137,25 @@
 
     def set_bearer_token(self) -> None:
         """Set bearer token from request."""
         resp = self.get_bearer_token()
         self._bearer_info = resp.json()
 
     def is_bearer_token_expired(self) -> bool:
-        """
-        Is current time > 'expires' time.
-        TODO: expires_in should be 'expires_at'
-        """
-        # TODO: this should eventually read 'expires_at'
+        """Is current time > 'expires' time."""
+        if "expires_at_rfc3339" not in self._bearer_info:
+            return True
+
+        expiration = datetime.strptime(
+            self._bearer_info["expires_at_rfc3339"], "%Y-%m-%dT%H:%M:%SZ"
+        )
+        seconds_to_expiration = (expiration - datetime.utcnow()).total_seconds()
+
         # adding 10 second buffer for expiration
-        return int(time.time()) + 10 >= self._bearer_info.get("expires_in", 0)
+        return seconds_to_expiration < 10
 
     @staticmethod
     def refresh_token(func) -> Callable:
         """Return a wrapper function that can check an auth token."""
 
         @functools.wraps(func)
         def check_token(api, *args, **kwargs):
```

### Comparing `qci-client-3.0.3/qci_client/data_converter.py` & `qci-client-3.1.0/qci_client/data_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,21 +67,24 @@
     # num_vars * step_len < 30k => step_len < 30k/num_vars
     chunk_ratio = MEMORY_MAX / soln_mem
     step_len = floor(chunk_ratio) if chunk_ratio >= 1 else 1
     return step_len
 
 def data_to_json(file: dict, debug: bool = False) -> dict:
     """
-    Converts data in file input into JSON string that can be passed to Qatalyst REST API
-    :param file: file object whose data of type numpy.ndarray, scipy.sparse.spmatrix, or networkx.Graph is to be converted to JSON
-    :param debug: Optional, if set to True, enables debug output (default = False for no debug output)
+    Converts data in file input into JSON-serializable dictionary that can be passed to Qatalyst REST API
 
-    :return: string (JSON format)
-    :note: could add support for matrices stored as lists
+    Args:
+        file: file dictionary whose data of type numpy.ndarray, scipy.sparse.spmatrix, or networkx.Graph is to be converted
+        debug: Optional, if set to True, enables debug output (default = False for no debug output)
+
+    Returns:
+        file dictionary with JSON-serializable data
     """
+    # TODO: could add support for matrices stored as lists
     start = time.perf_counter()
 
     supported_file_types = [
         "graph",
         "qubo",
         "hamiltonian",
         "objective",
@@ -115,15 +118,17 @@
                 "support networkx.Graph data"
             )
 
         data_ls = []
 
         if sp.isspmatrix_dok(data):
             for idx, val in zip(data.keys(), data.values()):
-                data_ls.append({"i": int(idx[0]), "j": int(idx[1]), "val": val})
+                # dok type has trouble subsequently serializing to json without type
+                # casts. For example, uint16 and float32 cause problems.
+                data_ls.append({"i": int(idx[0]), "j": int(idx[1]), "val": float(val)})
         elif sp.isspmatrix(data) or isinstance(data, np.ndarray):
             data = sp.coo_matrix(data)
 
             for i, j, val in zip(
                 data.row.tolist(), data.col.tolist(), data.data.tolist()
             ):
                 data_ls.append({"i": i, "j": j, "val": val})
```

### Comparing `qci-client-3.0.3/qci_client/enum.py` & `qci-client-3.1.0/qci_client/enum.py`

 * *Files identical despite different names*

### Comparing `qci-client-3.0.3/qci_client/qci_client.py` & `qci-client-3.1.0/qci_client/qci_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,27 @@
     CANCELLED = "CANCELLED"
 
 FINAL_STATUSES = frozenset([JobStatus.COMPLETED, JobStatus.ERRORED, JobStatus.CANCELLED])
 
 @dataclass
 class QciClient(BaseApi):  # pylint: disable=too-many-public-methods
     """
-    Provides requests for QCIs public API as well as utility functions for creating requests and processing entire jobs.
-    :param max_workers: int, number of threads for concurrent file download calls
+    Provides requests for QCi's public API for running optimization problems on Dirac
+    devices, including file uploads/downloads and submitting/retrieving entire jobs.
+
+    Accepts same parameters as :class:`qci_client.base.BaseApi` as well as:
+
     :param files: url path fragment to specify files API endpoint
     :param jobs: url path fragment to specify jobs API endpoint
+    :param max_workers: number of threads for concurrent file download calls
+    :param compress: compress file metadata and parts before uploading
     """
-    max_workers: int = 8
     files: str = "optimization/v1/files"
     jobs: str = "optimization/v1/jobs"
+    max_workers: int = 8
     compress: bool = COMPRESS_DEFAULT
 
     _supported_job_types: ClassVar[frozenset] = frozenset(
         [
             "sample-qubo",
             "graph-partitioning",
             "sample-constraint",
@@ -343,25 +348,30 @@
         objective_file_id: Optional[str] = None,
         constraints_file_id: Optional[str] = None,
         job_name: Optional[str] = None,
         job_tags: Optional[list] = None,
     ) -> dict:
         """
         Constructs body for job submission requests
-        :param job_type: one of _supported_job_types
-        :param job_params: dict of params to be passed to job submission in "params" key
-        :param qubo_file_id: file id from files API for uploaded qubo
-        :param graph_file_id: file id from files API for uploaded graph
-        :param hamiltonian_file_id: file id from files API for uploaded hamiltonian
-        :param objective_file_id: file id from files API for uploaded objective
-        :param constraints_file_id: file id from files API for uploaded constraints
-        :param job_name: user specified name for job submission
-        :param job_tags: user specified labels for classifying and filtering user jobs after submission
-        :note: Need to add validation for job parameters
+
+        Args:
+            job_type: one of _supported_job_types
+            job_params: dict of params to be passed to job submission in "params" key
+            qubo_file_id: file id from files API for uploaded qubo
+            graph_file_id: file id from files API for uploaded graph
+            hamiltonian_file_id: file id from files API for uploaded hamiltonian
+            objective_file_id: file id from files API for uploaded objective
+            constraints_file_id: file id from files API for uploaded constraints
+            job_name: user specified name for job submission
+            job_tags: user specified labels for classifying and filtering user jobs after submission
+
+        Returns:
+            None
         """
+        # TODO: Need to add validation for job parameters
         self.validate_job_type(job_type=job_type)
 
         problem_config = {}
         device_config = {}
 
         if "sampler_type" not in job_params:
             raise ValueError(
@@ -406,42 +416,43 @@
             if not qubo_file_id:
                 raise AssertionError(
                     "qubo_file_id must be specified for job_type='sample-qubo'"
                 )
 
             problem_config["qubo_file_id"] = qubo_file_id
         elif job_type == 'sample-hamiltonian':
-            if device_name == 'dirac-1':
-                raise ValueError(
-                    f"{job_type} not supported on dirac-1. Consider using job_type "
-                    "sample-hamiltonian-ising for dirac-1."
-                )
-
-            # Optional parameter. Default to continuous solution.
-            if job_params.get("solution_precision") != 1:
-                problem_name = 'normalized_qudit_hamiltonian_optimization_continuous'
+            if device_name == 'dirac-2':
+                if job_params.get("solution_precision") != 1:
+                    problem_name = 'normalized_qudit_hamiltonian_optimization_continuous'
+                else:
+                    problem_name = 'normalized_qudit_hamiltonian_optimization_integer'
+            elif device_name == 'dirac-3':
+                problem_name = 'normalized_qudit_hamiltonian_optimization'
+
+                if "relaxation_schedule" in job_params:
+                    # Optional parameter.
+                    device_config["relaxation_schedule"] = job_params["relaxation_schedule"]
+
+                if "solution_precision" in job_params:
+                    # Optional parameter.
+                    device_config["solution_precision"] = job_params["solution_precision"]
+
+                if "sum_constraint" in job_params:
+                    # Optional parameter.
+                    device_config["sum_constraint"] = job_params["sum_constraint"]
             else:
-                problem_name = 'normalized_qudit_hamiltonian_optimization_integer'
+                raise ValueError(f"{job_type} not supported on {device_name}.")
 
             if not hamiltonian_file_id:
                 raise AssertionError(
                     "hamiltonian_file_id must be specified for "
                     "job_type='sample-hamiltonian'"
                 )
 
             problem_config["hamiltonian_file_id"] = hamiltonian_file_id
-
-            if "sum_constraint" not in job_params:
-                raise ValueError("Must define sum_constraint in job_params.")
-
-            device_config["sum_constraint"] = job_params["sum_constraint"]
-
-            if "relaxation_schedule" in job_params:
-                # Optional parameter.
-                device_config["relaxation_schedule"] = job_params["relaxation_schedule"]
         elif job_type == 'sample-hamiltonian-ising':
             if device_name in ('dirac-2', 'dirac-3'):
                 raise ValueError(
                     f"{job_type} not supported on dirac-2 and dirac-3. Consider using "
                     "job_type sample-hamiltonian for dirac-2 and dirac-3."
                 )
 
@@ -661,32 +672,29 @@
         self._check_response_error(response=response)
 
         return response.json()
 
     @BaseApi.refresh_token
     def zip_payload(self, payload: str) -> bytes:
         """
-        :param payload: str - json contents of file to be zipped
+        Zip contents of json file
 
-        return: zipped request_body
+        Args:
+            payload: str - json contents of file to be zipped
+
+        Returns:
+            zipped request_body
         """
         out = BytesIO()
         with gzip.GzipFile(fileobj=out, mode="w", compresslevel=6) as file:
             file.write(json.dumps(payload).encode("utf-8"))
         request_body = out.getvalue()
         out.close()
         return request_body
 
-    @BaseApi.refresh_token
-    def merge_two_dicts(self, x, y):  # pylint: disable=invalid-name
-        """Given two dictionaries, merge them into a new dict as a shallow copy."""
-        z = x.copy()  # pylint: disable=invalid-name
-        z.update(y)
-        return z
-
     def get_job_type_from_job_id(self, job_id: str) -> str:
         """
         Get job type from job ID.
 
         Args:
             job_id: ID of the job
```

### Comparing `qci-client-3.0.3/qci_client/types.py` & `qci-client-3.1.0/qci_client/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,27 @@
     Integer Normalized-Qudit Hamiltonian Optimization (NQHO) results file metadata
     configuration.
     """
 
     normalized_qudit_hamiltonian_optimization_integer_results: NqhoIntegerResultsMetadata  # pylint: disable=line-too-long
 
 
+class NqhoResultsMetadata(TypedDict):
+    """Normalized-Qudit Hamiltonian Optimization (NQHO) results file metadata."""
+
+
+class NqhoResultsMetadataConfig(TypedDict):
+    """
+    Normalized-Qudit Hamiltonian Optimization (NQHO) results file metadata
+    configuration.
+    """
+
+    normalized_qudit_hamiltonian_optimization_results: NqhoResultsMetadata
+
+
 class QlcboResultsMetadata(TypedDict):
     """
     Quadratic Linearly Constrained Binary Optimization (QLCBO) results file metadata.
     """
 
 
 class QlcboResultsMetadataConfig(TypedDict):
@@ -210,14 +223,15 @@
     organization_id: str
     user_id: str
     file_config: Union[
         GpResultsMetadataConfig,
         IhoResultsMetadataConfig,
         NqhoContinuousResultsMetadataConfig,
         NqhoIntegerResultsMetadataConfig,
+        NqhoResultsMetadataConfig,
         QlcboResultsMetadataConfig,
         QuboResultsMetadataConfig,
     ]
 
 
 # Request body for POSTing any file metadata.
 MetadataPostRequestBody = Union[
@@ -376,14 +390,37 @@
 
 class NqhoIntegerResultsPartConfig(TypedDict):
     """Integer NQHO results file part configuration."""
 
     normalized_qudit_hamiltonian_optimization_integer_results: NqhoIntegerResultsPart
 
 
+class NqhoResultsPartWithoutDistilled(TypedDict):
+    """NQHO results file part without distilled solution results."""
+
+    counts: List[int]
+    energies: List[float]
+    solutions: List[List[int]]
+
+
+class NqhoResultsPartWithDistilled(NqhoResultsPartWithoutDistilled):
+    """NQHO results file part with distilled solution results."""
+
+    distilled_energies: List[float]
+    distilled_solutions: List[List[int]]
+
+
+class NqhoResultsPartConfig(TypedDict):
+    """NQHO results file part configuration."""
+
+    normalized_qudit_hamiltonian_optimization_results: Union[
+        NqhoResultsPartWithoutDistilled, NqhoResultsPartWithDistilled,
+    ]
+
+
 class QlcboResultsPart(TypedDict):
     """QLCBO results file part."""
 
     counts: List[int]
     energies: List[float]
     feasibilities: List[bool]
     objective_values: List[float]
@@ -419,14 +456,15 @@
         HamiltonianPartConfig,
         ObjectivePartConfig,
         QuboPartConfig,
         GpResultsPartConfig,
         IhoResultsPartConfig,
         NqhoContinuousResultsPartConfig,
         NqhoIntegerResultsPartConfig,
+        NqhoResultsPartConfig,
         QlcboResultsPartConfig,
         QuboResultsPartConfig,
     ]
 
 
 class PartPatchResponseBody(TypedDict):
     """File part PATCH response body."""
@@ -456,14 +494,15 @@
         HamiltonianMetadataConfig,
         ObjectiveMetadataConfig,
         QuboMetadataConfig,
         GpResultsMetadataConfig,
         IhoResultsMetadataConfig,
         NqhoContinuousResultsMetadataConfig,
         NqhoIntegerResultsMetadataConfig,
+        NqhoResultsMetadataConfig,
         QlcboResultsMetadataConfig,
         QuboResultsMetadataConfig,
     ]
 
 
 class GetResponseBody(TypedDict):
     """Fields for GET file metadata responses."""
@@ -483,14 +522,15 @@
         HamiltonianPartConfig,
         ObjectivePartConfig,
         QuboPartConfig,
         GpResultsPartConfig,
         IhoResultsPartConfig,
         NqhoContinuousResultsPartConfig,
         NqhoIntegerResultsPartConfig,
+        NqhoResultsPartConfig,
         QlcboResultsPartConfig,
         QuboResultsPartConfig,
     ]
 
 
 class DeleteResponseBody(TypedDict):
     """File DELETE response body."""
```

### Comparing `qci-client-3.0.3/qci_client/utilities.py` & `qci-client-3.1.0/qci_client/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 # 15 * MebiByte (~15MB). See https://git.qci-dev.com/qci-dev/optimization-files-api/.
 MEMORY_MAX: int = 8 * 1000000  # 8MB
 
 
 def get_post_request_body(  # pylint: disable=too-many-branches,too-many-return-statements
     *, file: dict
 ) -> types.MetadataPostRequestBody:
-    """Format metadata body."""
+    """
+    Format metadata body.
+    """
     file_type = enum.get_file_type(file=file)
     file_config = file["file_config"][file_type.value]
     optional_fields = {}
 
     if "file_name" in file:
         optional_fields["file_name"] = file["file_name"]
```

### Comparing `qci-client-3.0.3/qci_client.egg-info/PKG-INFO` & `qci-client-3.1.0/qci_client.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: qci-client
-Version: 3.0.3
+Version: 3.1.0
 Summary: Client Package for using Qatalyst Optimization Suite
 Author: Quantum Computing Inc.
 Author-email: support@quantumcomputinginc.com
 License: Apache 2.0
-Project-URL: documentation, https://qatalyst.quantumcomputinginc.com
+Project-URL: documentation, https://quantumcomputinginc.com/learn/reference-documentation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests<3,>=2.22.1
@@ -20,14 +20,15 @@
 Provides-Extra: dev
 Requires-Dist: black==23.1.0; extra == "dev"
 Requires-Dist: build<0.11,>=0.10.0; extra == "dev"
 Requires-Dist: check-manifest<0.49,>=0.48; extra == "dev"
 Requires-Dist: coverage[toml]<7,>=6.4.2; extra == "dev"
 Requires-Dist: pylint==2.16.2; extra == "dev"
 Requires-Dist: pytest<8,>=7.2.1; extra == "dev"
+Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "dev"
 Requires-Dist: twine<4,>=3.7.1; extra == "dev"
 
 # QCI Client
 
 ## Getting started
 
 ### Installation
@@ -38,16 +39,35 @@
 Install `qci-client` from the [public PyPI server](https://pypi.org/)
 into your Python virtual environment using--
 
 ```bash
 pip install qci-client
 ```
 
-### Environment Variables
+### Instantiating a Client
 
-These environment variables must be set in order to access the API--
+#### With Environment Variables
+
+To access the API, set these environment variables--
 
-- QCI_TOKEN - token for Qatalyst API
 <!-- markdown-link-check-disable-next-line -->
-- QCI_API_URL - Example: "https://api.qci-prod.com"
+- QCI_API_URL - URL for Qatalyst API, Example: "https://api.qci-prod.com"
+- QCI_TOKEN - refresh token string for securely accessing Qatalyst API
+
+then instantiate a `QciClient` as follows--
+
+```python
+from qci_client import QciClient
+
+client = QciClient()
+```
+
+#### Without Environment Variables
 
+Access the API without first defining environment variables by instantiating a
+`QciClient` as follows--
 
+```python
+from qci_client import QciClient
+
+client = QciClient(url="https://api.qci-prod.com", api_token="<secret-token>")
+```
```

### Comparing `qci-client-3.0.3/qci_client.egg-info/SOURCES.txt` & `qci-client-3.1.0/qci_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qci-client-3.0.3/tests/test_data_converter.py` & `qci-client-3.1.0/tests/test_data_converter.py`

 * *Files identical despite different names*

### Comparing `qci-client-3.0.3/tests/test_qci_client.py` & `qci-client-3.1.0/tests/test_qci_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,44 +171,90 @@
                 },
                 "device_config": {
                     "dirac-1": {}
                 }
             }
         }
 
-        cls.hamiltonian_job_body_continous = {
+        cls.hamiltonian_job_body_solution_precision_omitted = {
             "job_submission": {
                 "job_name": "job_0",
                 "problem_config": {
-                    "normalized_qudit_hamiltonian_optimization_continuous": {
+                    "normalized_qudit_hamiltonian_optimization": {
+                        "hamiltonian_file_id": cls.hamiltonian_file_id
+                    }
+                },
+                "device_config": {
+                    "dirac-3": {
+                        "relaxation_parameter": 1,
+                        "sum_constraint": 2.4,
+                    }
+                }
+            }
+        }
+
+        cls.hamiltonian_job_body_solution_precision_continuous = {
+            "job_submission": {
+                "job_name": "job_0",
+                "problem_config": {
+                    "normalized_qudit_hamiltonian_optimization": {
                         "hamiltonian_file_id": cls.hamiltonian_file_id
                     }
                 },
                 "device_config": {
                     "dirac-3": {
+                        "relaxation_parameter": 1,
                         "sum_constraint": 2.4,
-                        "relaxation_parameter": 1
+                        "solution_precision": 0.1,
                     }
                 }
             }
         }
 
+        cls.hamiltonian_job_body_solution_precision_integer = {
+            "job_submission": {
+                "job_name": "job_0",
+                "problem_config": {
+                    "normalized_qudit_hamiltonian_optimization": {
+                        "hamiltonian_file_id": cls.hamiltonian_file_id
+                    }
+                },
+                "device_config": {
+                    "dirac-3": {
+                        "relaxation_parameter": 1,
+                        "solution_precision": 1,
+                    }
+                }
+            }
+        }
+
+        cls.hamiltonian_job_body_continous = {
+            "job_submission": {
+                "job_name": "job_0",
+                "problem_config": {
+                    "normalized_qudit_hamiltonian_optimization_continuous": {
+                        "hamiltonian_file_id": cls.hamiltonian_file_id
+                    }
+                },
+                "device_config": {
+                    "dirac-2": {}
+                }
+            }
+        }
+
         cls.hamiltonian_job_body_integer = {
             "job_submission": {
                 "job_name": "job_0",
                 "problem_config": {
                     "normalized_qudit_hamiltonian_optimization_integer": {
                         "hamiltonian_file_id": cls.hamiltonian_file_id
                     },
                 },
                 "device_config": {
-                    "dirac-3": {
-                        "sum_constraint": 7,
-                        "solution_precision": 1
-                    }
+                    "dirac-2": {}
                 }
             }
         }
 
         cls.hamiltonian_job_body_ising = {
             "job_submission": {
                 "job_name": "job_0",
@@ -255,19 +301,14 @@
 
         # test job info has appropriate keys
         # self.assertEqual(self.job_info, set(response.keys()))  # FIXME
 
         result = self.q1.download_file(file_id=response["job_result"]["file_id"])
         result = list(result)
         # self.assertTrue(all(i in result[0] for i in result_keys))  # FIXME
-    
-    def test_add_headers(self):
-        """Test adding headers to client's requests."""
-        q_h = QciClient(_add_headers={"X-Fake-Header": "fake-header"})
-        self.assertTrue(q_h.headers["X-Fake-Header"], "fake-header")
 
     def test_upload_file_error(self):
         """Test uploading improperly formatted file."""
         with self.assertRaises(KeyError):
             error_input = {
                 "file_type": "graph",
                 "file_name": "qubo.json",
@@ -396,54 +437,41 @@
                             "num_samples": 24
                         }
                     }
                 }
             }
         )
 
-        with self.assertRaises(ValueError) as context:
-            self.q1.build_job_body(
-                job_type="sample-hamiltonian",
-                job_params={
-                    "n_samples": 24,
-                    "sampler_type": "dirac-3",
-                },
-                hamiltonian_file_id="hamiltonian_fid",
-            )
-
-        self.assertEqual(
-            str(context.exception),
-            "Must define sum_constraint in job_params."
-        )
-
         hamiltonian_body = self.q1.build_job_body(
             job_type="sample-hamiltonian",
             job_params={
                 "n_samples": 24,
                 "sampler_type": "dirac-3",
                 "sum_constraint": 200,
+                "solution_precision": 1,
             },
             hamiltonian_file_id="hamiltonian_fid",
             job_tags=["foobar_tag1", "foobar_tag2"],
         )
 
         self.assertDictEqual(
             hamiltonian_body,
             {
                 "job_submission": {
                     "job_tags": ["foobar_tag1", "foobar_tag2"],
                     "problem_config": {
-                        "normalized_qudit_hamiltonian_optimization_continuous": {
+                        "normalized_qudit_hamiltonian_optimization": {
                             "hamiltonian_file_id": "hamiltonian_fid",
                         }
                     },
                     "device_config": {
                         "dirac-3": {
                             "num_samples": 24,
                             "sum_constraint": 200,
+                            "solution_precision": 1,
                         }
                     }
                 }
             }
         )
 
         hamiltonian_body = self.q1.build_job_body(
@@ -457,43 +485,43 @@
         )
 
         self.assertDictEqual(
             hamiltonian_body,
             {
                 "job_submission": {
                     "problem_config": {
-                        "normalized_qudit_hamiltonian_optimization_integer": {
+                        "normalized_qudit_hamiltonian_optimization": {
                             "hamiltonian_file_id": "hamiltonian_fid",
                         }
                     },
                     "device_config": {
                         "dirac-3": {
                             "sum_constraint": 200,
+                            "solution_precision": 1,
                         }
                     }
                 }
             }
         )
 
         hamiltonian_body = self.q1.build_job_body(
             job_type="sample-hamiltonian",
             job_params={
                 "sampler_type": "dirac-3",
-                "sum_constraint": 2.4,
-                "solution_precision": None,
+                "sum_constraint": 2.4
             },
             hamiltonian_file_id="hamiltonian_fid"
         )
 
         self.assertDictEqual(
             hamiltonian_body,
             {
                 "job_submission": {
                     "problem_config": {
-                        "normalized_qudit_hamiltonian_optimization_continuous": {
+                        "normalized_qudit_hamiltonian_optimization": {
                             "hamiltonian_file_id": "hamiltonian_fid",
                         }
                     },
                     "device_config": {
                         "dirac-3": {
                             "sum_constraint": 2.4,
                         }
@@ -513,21 +541,22 @@
         )
 
         self.assertDictEqual(
             hamiltonian_body,
             {
                 "job_submission": {
                     "problem_config": {
-                        "normalized_qudit_hamiltonian_optimization_continuous": {
+                        "normalized_qudit_hamiltonian_optimization": {
                             "hamiltonian_file_id": "hamiltonian_fid",
                         }
                     },
                     "device_config": {
                         "dirac-3": {
                             "sum_constraint": 2.4,
+                            "solution_precision": 0.1,
                         }
                     }
                 }
             }
         )
 
         graph_body = self.q1.build_job_body(
```

