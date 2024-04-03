# Comparing `tmp/httpx-oauth-0.9.0.tar.gz` & `tmp/httpx-oauth-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpx-oauth-0.9.0.tar", last modified: Fri Aug 12 13:29:23 2022, max compression
+gzip compressed data, was "httpx-oauth-0.9.1.tar", last modified: Fri Aug 12 13:59:32 2022, max compression
```

## Comparing `httpx-oauth-0.9.0.tar` & `httpx-oauth-0.9.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      230 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/.editorconfig
--rw-r--r--   0        0        0       19 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      143 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1219 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      655 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1239 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/.gitignore
--rw-r--r--   0        0        0     1074 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/LICENSE
--rw-r--r--   0        0        0      412 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/Makefile
--rw-r--r--   0        0        0     1573 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/README.md
--rw-r--r--   0        0        0     1196 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/docs/fastapi.md
--rw-r--r--   0        0        0       17 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/docs/index.md
--rw-r--r--   0        0        0     8040 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/docs/oauth2.md
--rw-r--r--   0        0        0       61 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/__init__.py
--rw-r--r--   0        0        0      116 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/branding.py
--rw-r--r--   0        0        0        0 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/clients/__init__.py
--rw-r--r--   0        0        0     1869 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/clients/discord.py
--rw-r--r--   0        0        0     3139 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/clients/facebook.py
--rw-r--r--   0        0        0     5905 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/clients/github.py
--rw-r--r--   0        0        0     3503 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/clients/google.py
--rw-r--r--   0        0        0     3737 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/clients/linkedin.py
--rw-r--r--   0        0        0     2721 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/clients/microsoft.py
--rw-r--r--   0        0        0     1421 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/clients/okta.py
--rw-r--r--   0        0        0     4210 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/clients/reddit.py
--rw-r--r--   0        0        0      229 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/errors.py
--rw-r--r--   0        0        0        0 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/integrations/__init__.py
--rw-r--r--   0        0        0     1474 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/integrations/fastapi.py
--rw-r--r--   0        0        0     5565 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/oauth2.py
--rw-r--r--   0        0        0        0 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/py.typed
--rw-r--r--   0        0        0      251 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/httpx_oauth/typing.py
--rw-r--r--   0        0        0      553 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/mkdocs.yml
--rw-r--r--   0        0        0     1383 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      277 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/setup.cfg
--rw-r--r--   0        0        0        0 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     1382 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0       35 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/mock/error.json
--rw-r--r--   0        0        0      112 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/mock/facebook_success_long_lived_access_token.json
--rw-r--r--   0        0        0      173 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/mock/google_success_access_token.json
--rw-r--r--   0        0        0      103 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/mock/google_success_refresh_token.json
--rw-r--r--   0        0        0     4838 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/mock/reddit_success_identity.json
--rw-r--r--   0        0        0      212 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/test_branding.py
--rw-r--r--   0        0        0     3733 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/test_clients_discord.py
--rw-r--r--   0        0        0     3400 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/test_clients_facebook.py
--rw-r--r--   0        0        0     3139 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/test_clients_github.py
--rw-r--r--   0        0        0     2132 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/test_clients_google.py
--rw-r--r--   0        0        0     3082 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/test_clients_linkedin.py
--rw-r--r--   0        0        0     2766 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/test_clients_microsoft.py
--rw-r--r--   0        0        0     1866 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/test_clients_okta.py
--rw-r--r--   0        0        0     8839 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/test_clients_reddit.py
--rw-r--r--   0        0        0     4364 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/test_integrations_fastapi.py
--rw-r--r--   0        0        0     8040 2022-08-12 13:28:54.171171 httpx-oauth-0.9.0/tests/test_oauth2.py
--rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 httpx-oauth-0.9.0/setup.py
--rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 httpx-oauth-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      230 2022-08-12 13:59:11.800704 httpx-oauth-0.9.1/.editorconfig
+-rw-r--r--   0        0        0       19 2022-08-12 13:59:11.800704 httpx-oauth-0.9.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      143 2022-08-12 13:59:11.800704 httpx-oauth-0.9.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1219 2022-08-12 13:59:11.800704 httpx-oauth-0.9.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      655 2022-08-12 13:59:11.800704 httpx-oauth-0.9.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1239 2022-08-12 13:59:11.800704 httpx-oauth-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1074 2022-08-12 13:59:11.800704 httpx-oauth-0.9.1/LICENSE
+-rw-r--r--   0        0        0      412 2022-08-12 13:59:11.800704 httpx-oauth-0.9.1/Makefile
+-rw-r--r--   0        0        0     1573 2022-08-12 13:59:11.800704 httpx-oauth-0.9.1/README.md
+-rw-r--r--   0        0        0     1196 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/docs/fastapi.md
+-rw-r--r--   0        0        0       17 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/docs/index.md
+-rw-r--r--   0        0        0     8040 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/docs/oauth2.md
+-rw-r--r--   0        0        0       61 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/__init__.py
+-rw-r--r--   0        0        0      116 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/branding.py
+-rw-r--r--   0        0        0        0 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/clients/__init__.py
+-rw-r--r--   0        0        0     1869 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/clients/discord.py
+-rw-r--r--   0        0        0     3100 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/clients/facebook.py
+-rw-r--r--   0        0        0     5850 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/clients/github.py
+-rw-r--r--   0        0        0     3448 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/clients/google.py
+-rw-r--r--   0        0        0     3698 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/clients/linkedin.py
+-rw-r--r--   0        0        0     2666 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/clients/microsoft.py
+-rw-r--r--   0        0        0     1421 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/clients/okta.py
+-rw-r--r--   0        0        0     4210 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/clients/reddit.py
+-rw-r--r--   0        0        0      229 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/errors.py
+-rw-r--r--   0        0        0        0 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/integrations/__init__.py
+-rw-r--r--   0        0        0     1474 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/integrations/fastapi.py
+-rw-r--r--   0        0        0     5565 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/oauth2.py
+-rw-r--r--   0        0        0        0 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/py.typed
+-rw-r--r--   0        0        0      251 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/httpx_oauth/typing.py
+-rw-r--r--   0        0        0      553 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/mkdocs.yml
+-rw-r--r--   0        0        0     1383 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      277 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/setup.cfg
+-rw-r--r--   0        0        0        0 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     1382 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0       35 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/mock/error.json
+-rw-r--r--   0        0        0      112 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/mock/facebook_success_long_lived_access_token.json
+-rw-r--r--   0        0        0      173 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/mock/google_success_access_token.json
+-rw-r--r--   0        0        0      103 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/mock/google_success_refresh_token.json
+-rw-r--r--   0        0        0     4838 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/mock/reddit_success_identity.json
+-rw-r--r--   0        0        0      212 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/test_branding.py
+-rw-r--r--   0        0        0     3733 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/test_clients_discord.py
+-rw-r--r--   0        0        0     3400 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/test_clients_facebook.py
+-rw-r--r--   0        0        0     3139 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/test_clients_github.py
+-rw-r--r--   0        0        0     2132 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/test_clients_google.py
+-rw-r--r--   0        0        0     3082 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/test_clients_linkedin.py
+-rw-r--r--   0        0        0     2766 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/test_clients_microsoft.py
+-rw-r--r--   0        0        0     1866 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/test_clients_okta.py
+-rw-r--r--   0        0        0     8839 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/test_clients_reddit.py
+-rw-r--r--   0        0        0     4364 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/test_integrations_fastapi.py
+-rw-r--r--   0        0        0     8040 2022-08-12 13:59:11.804704 httpx-oauth-0.9.1/tests/test_oauth2.py
+-rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 httpx-oauth-0.9.1/setup.py
+-rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 httpx-oauth-0.9.1/PKG-INFO
```

### Comparing `httpx-oauth-0.9.0/.github/workflows/build.yml` & `httpx-oauth-0.9.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/.github/workflows/documentation.yml` & `httpx-oauth-0.9.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/.gitignore` & `httpx-oauth-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/LICENSE` & `httpx-oauth-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/README.md` & `httpx-oauth-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/docs/fastapi.md` & `httpx-oauth-0.9.1/docs/fastapi.md`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/docs/oauth2.md` & `httpx-oauth-0.9.1/docs/oauth2.md`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/httpx_oauth/clients/discord.py` & `httpx-oauth-0.9.1/httpx_oauth/clients/discord.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/httpx_oauth/clients/facebook.py` & `httpx-oauth-0.9.1/httpx_oauth/clients/facebook.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 AUTHORIZE_ENDPOINT = "https://www.facebook.com/v5.0/dialog/oauth"
 ACCESS_TOKEN_ENDPOINT = "https://graph.facebook.com/v5.0/oauth/access_token"
 BASE_SCOPES = ["email", "public_profile"]
 PROFILE_ENDPOINT = "https://graph.facebook.com/v5.0/me"
 
 
 LOGO_SVG = """
-<?xml version="1.0" encoding="UTF-8"?>
 <svg width="256px" height="256px" viewBox="0 0 256 256" version="1.1" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid">
     <title>Facebook</title>
     <g>
         <path d="M256,128 C256,57.3075 198.6925,0 128,0 C57.3075,0 0,57.3075 0,128 C0,191.8885 46.80775,244.8425 108,254.445 L108,165 L75.5,165 L75.5,128 L108,128 L108,99.8 C108,67.72 127.1095,50 156.3475,50 C170.35175,50 185,52.5 185,52.5 L185,84 L168.8595,84 C152.95875,84 148,93.86675 148,103.98925 L148,128 L183.5,128 L177.825,165 L148,165 L148,254.445 C209.19225,244.8425 256,191.8885 256,128" fill="#1877F2"></path>
         <path d="M177.825,165 L183.5,128 L148,128 L148,103.98925 C148,93.86675 152.95875,84 168.8595,84 L185,84 L185,52.5 C185,52.5 170.35175,50 156.3475,50 C127.1095,50 108,67.72 108,99.8 L108,128 L75.5,128 L75.5,165 L108,165 L108,254.445 C114.51675,255.4675 121.196,256 128,256 C134.804,256 141.48325,255.4675 148,254.445 L148,165 L177.825,165" fill="#FFFFFF"></path>
     </g>
 </svg>
```

### Comparing `httpx-oauth-0.9.0/httpx_oauth/clients/github.py` & `httpx-oauth-0.9.1/httpx_oauth/clients/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 ACCESS_TOKEN_ENDPOINT = "https://github.com/login/oauth/access_token"
 BASE_SCOPES = ["user", "user:email"]
 PROFILE_ENDPOINT = "https://api.github.com/user"
 EMAILS_ENDPOINT = "https://api.github.com/user/emails"
 
 
 LOGO_SVG = """
-<?xml version="1.0" encoding="UTF-8" standalone="no"?>
 <svg width="256px" height="250px" viewBox="0 0 256 250" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" preserveAspectRatio="xMidYMid">
     <g>
         <path d="M128.00106,0 C57.3172926,0 0,57.3066942 0,128.00106 C0,184.555281 36.6761997,232.535542 87.534937,249.460899 C93.9320223,250.645779 96.280588,246.684165 96.280588,243.303333 C96.280588,240.251045 96.1618878,230.167899 96.106777,219.472176 C60.4967585,227.215235 52.9826207,204.369712 52.9826207,204.369712 C47.1599584,189.574598 38.770408,185.640538 38.770408,185.640538 C27.1568785,177.696113 39.6458206,177.859325 39.6458206,177.859325 C52.4993419,178.762293 59.267365,191.04987 59.267365,191.04987 C70.6837675,210.618423 89.2115753,204.961093 96.5158685,201.690482 C97.6647155,193.417512 100.981959,187.77078 104.642583,184.574357 C76.211799,181.33766 46.324819,170.362144 46.324819,121.315702 C46.324819,107.340889 51.3250588,95.9223682 59.5132437,86.9583937 C58.1842268,83.7344152 53.8029229,70.715562 60.7532354,53.0843636 C60.7532354,53.0843636 71.5019501,49.6441813 95.9626412,66.2049595 C106.172967,63.368876 117.123047,61.9465949 128.00106,61.8978432 C138.879073,61.9465949 149.837632,63.368876 160.067033,66.2049595 C184.49805,49.6441813 195.231926,53.0843636 195.231926,53.0843636 C202.199197,70.715562 197.815773,83.7344152 196.486756,86.9583937 C204.694018,95.9223682 209.660343,107.340889 209.660343,121.315702 C209.660343,170.478725 179.716133,181.303747 151.213281,184.472614 C155.80443,188.444828 159.895342,196.234518 159.895342,208.176593 C159.895342,225.303317 159.746968,239.087361 159.746968,243.303333 C159.746968,246.709601 162.05102,250.70089 168.53925,249.443941 C219.370432,232.499507 256,184.536204 256,128.00106 C256,57.3066942 198.691187,0 128.00106,0 Z M47.9405593,182.340212 C47.6586465,182.976105 46.6581745,183.166873 45.7467277,182.730227 C44.8183235,182.312656 44.2968914,181.445722 44.5978808,180.80771 C44.8734344,180.152739 45.876026,179.97045 46.8023103,180.409216 C47.7328342,180.826786 48.2627451,181.702199 47.9405593,182.340212 Z M54.2367892,187.958254 C53.6263318,188.524199 52.4329723,188.261363 51.6232682,187.366874 C50.7860088,186.474504 50.6291553,185.281144 51.2480912,184.70672 C51.8776254,184.140775 53.0349512,184.405731 53.8743302,185.298101 C54.7115892,186.201069 54.8748019,187.38595 54.2367892,187.958254 Z M58.5562413,195.146347 C57.7719732,195.691096 56.4895886,195.180261 55.6968417,194.042013 C54.9125733,192.903764 54.9125733,191.538713 55.713799,190.991845 C56.5086651,190.444977 57.7719732,190.936735 58.5753181,192.066505 C59.3574669,193.22383 59.3574669,194.58888 58.5562413,195.146347 Z M65.8613592,203.471174 C65.1597571,204.244846 63.6654083,204.03712 62.5716717,202.981538 C61.4524999,201.94927 61.1409122,200.484596 61.8446341,199.710926 C62.5547146,198.935137 64.0575422,199.15346 65.1597571,200.200564 C66.2704506,201.230712 66.6095936,202.705984 65.8613592,203.471174 Z M75.3025151,206.281542 C74.9930474,207.284134 73.553809,207.739857 72.1039724,207.313809 C70.6562556,206.875043 69.7087748,205.700761 70.0012857,204.687571 C70.302275,203.678621 71.7478721,203.20382 73.2083069,203.659543 C74.6539041,204.09619 75.6035048,205.261994 75.3025151,206.281542 Z M86.046947,207.473627 C86.0829806,208.529209 84.8535871,209.404622 83.3316829,209.4237 C81.8013,209.457614 80.563428,208.603398 80.5464708,207.564772 C80.5464708,206.498591 81.7483088,205.631657 83.2786917,205.606221 C84.8005962,205.576546 86.046947,206.424403 86.046947,207.473627 Z M96.6021471,207.069023 C96.7844366,208.099171 95.7267341,209.156872 94.215428,209.438785 C92.7295577,209.710099 91.3539086,209.074206 91.1652603,208.052538 C90.9808515,206.996955 92.0576306,205.939253 93.5413813,205.66582 C95.054807,205.402984 96.4092596,206.021919 96.6021471,207.069023 Z" fill="#161614"></path>
     </g>
 </svg>
 """
```

### Comparing `httpx-oauth-0.9.0/httpx_oauth/clients/google.py` & `httpx-oauth-0.9.1/httpx_oauth/clients/google.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     "https://www.googleapis.com/auth/userinfo.profile",
     "https://www.googleapis.com/auth/userinfo.email",
 ]
 PROFILE_ENDPOINT = "https://people.googleapis.com/v1/people/me"
 
 
 LOGO_SVG = """
-<?xml version="1.0" encoding="UTF-8" standalone="no"?>
 <svg width="256px" height="262px" viewBox="0 0 256 262" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" preserveAspectRatio="xMidYMid">
 	<g>
 		<path d="M255.878,133.451 C255.878,122.717 255.007,114.884 253.122,106.761 L130.55,106.761 L130.55,155.209 L202.497,155.209 C201.047,167.249 193.214,185.381 175.807,197.565 L175.563,199.187 L214.318,229.21 L217.003,229.478 C241.662,206.704 255.878,173.196 255.878,133.451" fill="#4285F4"></path>
 		<path d="M130.55,261.1 C165.798,261.1 195.389,249.495 217.003,229.478 L175.807,197.565 C164.783,205.253 149.987,210.62 130.55,210.62 C96.027,210.62 66.726,187.847 56.281,156.37 L54.75,156.5 L14.452,187.687 L13.925,189.152 C35.393,231.798 79.49,261.1 130.55,261.1" fill="#34A853"></path>
 		<path d="M56.281,156.37 C53.525,148.247 51.93,139.543 51.93,130.55 C51.93,121.556 53.525,112.853 56.136,104.73 L56.063,103 L15.26,71.312 L13.925,71.947 C5.077,89.644 0,109.517 0,130.55 C0,151.583 5.077,171.455 13.925,189.152 L56.281,156.37" fill="#FBBC05"></path>
 		<path d="M130.55,50.479 C155.064,50.479 171.6,61.068 181.029,69.917 L217.873,33.943 C195.245,12.91 165.798,0 130.55,0 C79.49,0 35.393,29.301 13.925,71.947 L56.136,104.73 C66.726,73.253 96.027,50.479 130.55,50.479" fill="#EB4335"></path>
 	</g>
```

### Comparing `httpx-oauth-0.9.0/httpx_oauth/clients/linkedin.py` & `httpx-oauth-0.9.1/httpx_oauth/clients/linkedin.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 ACCESS_TOKEN_ENDPOINT = "https://www.linkedin.com/oauth/v2/accessToken"
 BASE_SCOPES = ["r_emailaddress", "r_liteprofile", "r_basicprofile"]
 PROFILE_ENDPOINT = "https://api.linkedin.com/v2/me"
 EMAIL_ENDPOINT = "https://api.linkedin.com/v2/emailAddress"
 
 
 LOGO_SVG = """
-<?xml version="1.0" encoding="UTF-8"?>
 <svg width="256px" height="256px" viewBox="0 0 256 256" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" preserveAspectRatio="xMidYMid">
     <g>
         <path d="M218.123122,218.127392 L180.191928,218.127392 L180.191928,158.724263 C180.191928,144.559023 179.939053,126.323993 160.463756,126.323993 C140.707926,126.323993 137.685284,141.757585 137.685284,157.692986 L137.685284,218.123441 L99.7540894,218.123441 L99.7540894,95.9665207 L136.168036,95.9665207 L136.168036,112.660562 L136.677736,112.660562 C144.102746,99.9650027 157.908637,92.3824528 172.605689,92.9280076 C211.050535,92.9280076 218.138927,118.216023 218.138927,151.114151 L218.123122,218.127392 Z M56.9550587,79.2685282 C44.7981969,79.2707099 34.9413443,69.4171797 34.9391618,57.260052 C34.93698,45.1029244 44.7902948,35.2458562 56.9471566,35.2436736 C69.1040185,35.2414916 78.9608713,45.0950217 78.963054,57.2521493 C78.9641017,63.090208 76.6459976,68.6895714 72.5186979,72.8184433 C68.3913982,76.9473153 62.7929898,79.26748 56.9550587,79.2685282 M75.9206558,218.127392 L37.94995,218.127392 L37.94995,95.9665207 L75.9206558,95.9665207 L75.9206558,218.127392 Z M237.033403,0.0182577091 L18.8895249,0.0182577091 C8.57959469,-0.0980923971 0.124827038,8.16056231 -0.001,18.4706066 L-0.001,237.524091 C0.120519052,247.839103 8.57460631,256.105934 18.8895249,255.9977 L237.033403,255.9977 C247.368728,256.125818 255.855922,247.859464 255.999,237.524091 L255.999,18.4548016 C255.851624,8.12438979 247.363742,-0.133792868 237.033403,0.000790807055" fill="#0A66C2"></path>
     </g>
 </svg>
 """
```

### Comparing `httpx-oauth-0.9.0/httpx_oauth/clients/microsoft.py` & `httpx-oauth-0.9.1/httpx_oauth/clients/microsoft.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 AUTHORIZE_ENDPOINT = "https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize"
 ACCESS_TOKEN_ENDPOINT = "https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token"
 BASE_SCOPES = ["User.Read"]
 PROFILE_ENDPOINT = "https://graph.microsoft.com/v1.0/me"
 
 
 LOGO_SVG = """
-<?xml version="1.0" encoding="UTF-8" standalone="no"?>
 <svg width="100%" height="100%" viewBox="0 0 110 110" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xml:space="preserve" xmlns:serif="http://www.serif.com/" style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;">
     <rect x="0" y="0" width="51.927" height="51.927" style="fill:rgb(241,81,27);fill-rule:nonzero;"/>
     <rect x="57.334" y="0" width="51.926" height="51.927" style="fill:rgb(128,204,40);fill-rule:nonzero;"/>
     <rect x="0" y="57.354" width="51.925" height="51.927" style="fill:rgb(0,173,239);fill-rule:nonzero;"/>
     <rect x="57.334" y="57.354" width="51.926" height="51.927" style="fill:rgb(251,188,9);fill-rule:nonzero;"/>
 </svg>
 """
```

### Comparing `httpx-oauth-0.9.0/httpx_oauth/clients/okta.py` & `httpx-oauth-0.9.1/httpx_oauth/clients/okta.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/httpx_oauth/clients/reddit.py` & `httpx-oauth-0.9.1/httpx_oauth/clients/reddit.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/httpx_oauth/integrations/fastapi.py` & `httpx-oauth-0.9.1/httpx_oauth/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/httpx_oauth/oauth2.py` & `httpx-oauth-0.9.1/httpx_oauth/oauth2.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/mkdocs.yml` & `httpx-oauth-0.9.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/pyproject.toml` & `httpx-oauth-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/tests/conftest.py` & `httpx-oauth-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/tests/mock/reddit_success_identity.json` & `httpx-oauth-0.9.1/tests/mock/reddit_success_identity.json`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/tests/test_clients_discord.py` & `httpx-oauth-0.9.1/tests/test_clients_discord.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/tests/test_clients_facebook.py` & `httpx-oauth-0.9.1/tests/test_clients_facebook.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/tests/test_clients_github.py` & `httpx-oauth-0.9.1/tests/test_clients_github.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/tests/test_clients_google.py` & `httpx-oauth-0.9.1/tests/test_clients_google.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/tests/test_clients_linkedin.py` & `httpx-oauth-0.9.1/tests/test_clients_linkedin.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/tests/test_clients_microsoft.py` & `httpx-oauth-0.9.1/tests/test_clients_microsoft.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/tests/test_clients_okta.py` & `httpx-oauth-0.9.1/tests/test_clients_okta.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/tests/test_clients_reddit.py` & `httpx-oauth-0.9.1/tests/test_clients_reddit.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/tests/test_integrations_fastapi.py` & `httpx-oauth-0.9.1/tests/test_integrations_fastapi.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/tests/test_oauth2.py` & `httpx-oauth-0.9.1/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `httpx-oauth-0.9.0/setup.py` & `httpx-oauth-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
          'pymdown-extensions',
          'bumpversion',
          'pytest-asyncio',
          'respx',
          'fastapi']}
 
 setup(name='httpx-oauth',
-      version='0.9.0',
+      version='0.9.1',
       description='Async OAuth client using HTTPX',
       author=None,
       author_email='François Voron <fvoron@gmail.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `httpx-oauth-0.9.0/PKG-INFO` & `httpx-oauth-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-oauth
-Version: 0.9.0
+Version: 0.9.1
 Summary: Async OAuth client using HTTPX
 Author-email: François Voron <fvoron@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: httpx-oauth Version: 0.9.0 Summary: Async OAuth
+Metadata-Version: 2.1 Name: httpx-oauth Version: 0.9.1 Summary: Async OAuth
 client using HTTPX Author-email: FranÃ§ois Voron
 gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License Classifier: Development
 Status :: 5 - Production/Stable Classifier: Framework :: AsyncIO Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python ::
 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

