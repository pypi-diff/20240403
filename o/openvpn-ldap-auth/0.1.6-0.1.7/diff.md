# Comparing `tmp/openvpn-ldap-auth-0.1.6.tar.gz` & `tmp/openvpn_ldap_auth-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvpn-ldap-auth-0.1.6.tar", max compression
+gzip compressed data, was "openvpn_ldap_auth-0.1.7.tar", max compression
```

## Comparing `openvpn-ldap-auth-0.1.6.tar` & `openvpn_ldap_auth-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1072 2022-06-04 23:11:13.470809 openvpn-ldap-auth-0.1.6/LICENSE
--rw-r--r--   0        0        0     5464 2022-06-04 23:11:13.470809 openvpn-ldap-auth-0.1.6/README.md
--rw-r--r--   0        0        0        0 2022-06-04 23:11:13.470809 openvpn-ldap-auth-0.1.6/openvpn_ldap_auth/__init__.py
--rwxr-xr-x   0        0        0     8178 2022-06-04 23:11:13.470809 openvpn-ldap-auth-0.1.6/openvpn_ldap_auth/main.py
--rw-r--r--   0        0        0     2384 2022-06-04 23:11:13.474809 openvpn-ldap-auth-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6508 2022-06-04 23:11:52.153396 openvpn-ldap-auth-0.1.6/setup.py
--rw-r--r--   0        0        0     6632 2022-06-04 23:11:52.153730 openvpn-ldap-auth-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-03 16:10:13.792032 openvpn_ldap_auth-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5517 2024-04-03 16:10:13.792032 openvpn_ldap_auth-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 16:10:13.792032 openvpn_ldap_auth-0.1.7/openvpn_ldap_auth/__init__.py
+-rwxr-xr-x   0        0        0     8448 2024-04-03 16:10:13.792032 openvpn_ldap_auth-0.1.7/openvpn_ldap_auth/main.py
+-rw-r--r--   0        0        0     2511 2024-04-03 16:10:13.792032 openvpn_ldap_auth-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6688 1970-01-01 00:00:00.000000 openvpn_ldap_auth-0.1.7/PKG-INFO
```

### Comparing `openvpn-ldap-auth-0.1.6/LICENSE` & `openvpn_ldap_auth-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openvpn-ldap-auth-0.1.6/README.md` & `openvpn_ldap_auth-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Then create `/etc/openvpn/ldap.yaml`:
 
 ```yaml
 ldap:
   url: 'ldaps://first.ldap.tld:636/ ldaps://second.ldap.tld:636/'
   bind_dn: 'uid=readonly,dc=example,dc=org'
   password: 'somesecurepassword'
-  timeout: 5 # optional
+  timeout: 5 # (optional) wait this many seconds for connection and response
 authorization:
   base_dn: 'ou=people,dc=example,dc=org'
   search_filter: '(uid={})' # optional, {} will be replaced with the username
   static_challenge: 'ignore' # optional, other values are prepend, append 
 ```
 
 Find out where `openvpn-ldap-auth` lives:
```

### Comparing `openvpn-ldap-auth-0.1.6/openvpn_ldap_auth/main.py` & `openvpn_ldap_auth-0.1.7/openvpn_ldap_auth/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,220 +5,235 @@
 import traceback
 from base64 import b64decode
 
 import ldap
 import yaml
 from cerberus import Validator
 from ldap.ldapobject import SimpleLDAPObject
+from ldap.filter import escape_filter_chars
 
-LDAP_CONFIG = '/etc/openvpn/ldap.yaml'
+LDAP_CONFIG = "/etc/openvpn/ldap.yaml"
 
-STATIC_CHALLENGE_IGNORE = 'ignore'
-STATIC_CHALLENGE_PREPEND = 'prepend'
-STATIC_CHALLENGE_APPEND = 'append'
+STATIC_CHALLENGE_IGNORE = "ignore"
+STATIC_CHALLENGE_PREPEND = "prepend"
+STATIC_CHALLENGE_APPEND = "append"
 STATIC_CHALLENGE_OPTS = (
     STATIC_CHALLENGE_IGNORE,
     STATIC_CHALLENGE_PREPEND,
-    STATIC_CHALLENGE_APPEND
+    STATIC_CHALLENGE_APPEND,
 )
 
 
 def setup_logging(verbosity: int):
     if verbosity == 4:
         level = logging.DEBUG
     elif verbosity == 3:
         level = logging.INFO
     else:
         level = logging.WARN
-    logging.basicConfig(format='%(asctime)s %(levelname)s: %(message)s', level=level)
+    logging.basicConfig(format="%(asctime)s %(levelname)s: %(message)s", level=level)
 
 
 class InvalidConfigException(Exception):
     """Raise when the config validation failed."""
 
 
 class LDAPException(Exception):
     """Raise when issues occur while interacting with the LDAP server."""
 
 
 class Config:
     """Encapsulate user-defined configuration."""
 
     LDAP_CONFIG_SCHEMA = {
-        'ldap': {
-            'required': True,
-            'type': 'dict',
-            'schema': {
-                'url': {
-                    'required': True,
-                    'type': 'string',
-                },
-                'bind_dn': {
-                    'required': True,
-                    'type': 'string',
-                },
-                'password': {
-                    'required': True,
-                    'type': 'string',
-                },
-                'timeout': {
-                    'type': 'integer',
-                    'default': 5,
+        "ldap": {
+            "required": True,
+            "type": "dict",
+            "schema": {
+                "url": {
+                    "required": True,
+                    "type": "string",
+                },
+                "bind_dn": {
+                    "required": True,
+                    "type": "string",
+                },
+                "password": {
+                    "required": True,
+                    "type": "string",
+                },
+                "timeout": {
+                    "type": "integer",
+                    "default": 5,
+                },
+            },
+        },
+        "authorization": {
+            "required": True,
+            "type": "dict",
+            "schema": {
+                "base_dn": {
+                    "required": True,
+                    "type": "string",
+                },
+                "search_filter": {
+                    "type": "string",
+                    "default": "(uid={})",
+                },
+                "static_challenge": {
+                    "type": "string",
+                    "allowed": STATIC_CHALLENGE_OPTS,
+                    "default": "ignore",
                 },
             },
         },
-        'authorization': {
-            'required': True,
-            'type': 'dict',
-            'schema': {
-                'base_dn': {
-                    'required': True,
-                    'type': 'string',
-                },
-                'search_filter': {
-                    'type': 'string',
-                    'default': '(uid={})',
-                },
-                'static_challenge': {
-                    'type': 'string',
-                    'allowed': STATIC_CHALLENGE_OPTS,
-                    'default': 'ignore',
-                }
-            }
-        }
     }
 
     def __init__(self, config: dict):
         validator = Validator()
         is_valid = validator.validate(config, self.LDAP_CONFIG_SCHEMA)
         if not is_valid:
             raise InvalidConfigException(f"Invalid config: {validator.errors}")
         self._config = validator.document  # use normalized copy
 
     @property
     def url(self) -> str:
-        return self._config['ldap']['url']
+        return self._config["ldap"]["url"]
 
     @property
     def bind_dn(self) -> str:
-        return self._config['ldap']['bind_dn']
+        return self._config["ldap"]["bind_dn"]
 
     @property
     def password(self) -> str:
-        return self._config['ldap']['password']
+        return self._config["ldap"]["password"]
 
     @property
     def timeout(self) -> int:
-        return self._config['ldap']['timeout']
+        return self._config["ldap"]["timeout"]
 
     @property
     def base_dn(self) -> str:
-        return self._config['authorization']['base_dn']
+        return self._config["authorization"]["base_dn"]
 
     @property
     def search_filter(self) -> str:
-        return self._config['authorization']['search_filter']
+        return self._config["authorization"]["search_filter"]
 
     @property
     def static_challenge_mode(self) -> str:
-        return self._config['authorization']['static_challenge']
+        return self._config["authorization"]["static_challenge"]
 
     @staticmethod
     def from_file(path: str):
-        with open(path, 'r', encoding='utf-8') as stream:
+        with open(path, "r", encoding="utf-8") as stream:
             config = yaml.safe_load(stream)
         return Config(config=config)
 
 
 class OpenVPNParameters:
-
     def __init__(self, static_challenge_mode: str):
         self.static_challenge_mode = static_challenge_mode
         self.user = None
         self._raw_password = None
         self._password = None
         self._challenge_response = None
         self.verbosity = None
         self.config_file = None
-        if os.environ.get('password', False):
+        if os.environ.get("password", False):
             self._extract_credentials_from_environment()
         else:
             self._extract_credentials_from_input_file()
         self._decode_password()
         self._extract_other_parameters_from_evironment()
 
     def _extract_credentials_from_environment(self):
-        self.user = os.environ['username']
-        self._raw_password = os.environ['password']
+        self.user = os.environ["username"]
+        self._raw_password = os.environ["password"]
 
     def _extract_credentials_from_input_file(self):
-        tmp_file = open(sys.argv[1], 'r', encoding='utf-8')
+        tmp_file = open(sys.argv[1], "r", encoding="utf-8")
         lines = tmp_file.readlines()
         self.user = lines[0].strip()
         self._raw_password = lines[1].strip()
 
     def _decode_password(self):
-        if self._raw_password.startswith('SCRV1'):
-            logging.debug('Extracting static-challenge password and OTP')
-            password_parts = self._raw_password.split(':')
+        if self._raw_password.startswith("SCRV1"):
+            logging.debug("Extracting static-challenge password and OTP")
+            password_parts = self._raw_password.split(":")
             self._password = b64decode(password_parts[1])
             self._challenge_response = b64decode(password_parts[2])
         else:
-            logging.debug('Using password verbatim')
+            logging.debug("Using password verbatim")
             self._password = self._raw_password
 
     def _extract_other_parameters_from_evironment(self):
-        self.verbosity = int(os.environ.get('verb', 1))
-        self.config_file = os.environ['config'] if 'config' in os.environ else None
+        self.verbosity = int(os.environ.get("verb", 1))
+        self.config_file = os.environ["config"] if "config" in os.environ else None
 
     @property
     def full_password(self):
         """Concatenate the actual password with the challenge response if applicable."""
         if self._challenge_response:
             if self.static_challenge_mode == STATIC_CHALLENGE_IGNORE:
-                logging.debug('Ignoring challenge reponse')
+                logging.debug("Ignoring challenge reponse")
                 return self._password
             elif self.static_challenge_mode == STATIC_CHALLENGE_PREPEND:
-                logging.debug('Prepending challenge reponse')
+                logging.debug("Prepending challenge reponse")
                 return self._challenge_response + self._password
             else:
-                logging.debug('Appending challenge reponse')
+                logging.debug("Appending challenge reponse")
                 return self._password + self._challenge_response
         else:
             return self._password
 
 
 class LDAPAuthenticator:
-
-    def __init__(self, ldap_url: str, bind_dn: str, bind_password: str, user_search_base: str,
-                 user_search_template: str, timeout: int):
+    def __init__(
+        self,
+        ldap_url: str,
+        bind_dn: str,
+        bind_password: str,
+        user_search_base: str,
+        user_search_template: str,
+        timeout: int,
+    ):
         self._ldap_url = ldap_url
         self._user_search_base = user_search_base
         self._user_search_template = user_search_template
         self._timeout = timeout
         self._connection = self._establish_ldap_connection(bind_dn, bind_password)
 
-    def _establish_ldap_connection(self, bind_dn: str, password: str) -> SimpleLDAPObject:
+    def _establish_ldap_connection(
+        self, bind_dn: str, password: str
+    ) -> SimpleLDAPObject:
         con = ldap.initialize(self._ldap_url)
         con.set_option(ldap.OPT_NETWORK_TIMEOUT, self._timeout)
+        con.set_option(ldap.OPT_TIMEOUT, self._timeout)
         try:
             con.simple_bind_s(bind_dn, password)
         except ldap.INVALID_CREDENTIALS:
             raise LDAPException(f"Invalid password for {bind_dn}")
         except ldap.LDAPError as e:
             raise LDAPException(f"Simple bind failed for {bind_dn}: {e}")
         return con
 
     def _find_user(self, username):
-        results = self._connection.search_s(base=self._user_search_base, scope=ldap.SCOPE_SUBTREE,
-                                            filterstr=self._user_search_template.format(username), attrlist=[])
+        results = self._connection.search_st(
+            base=self._user_search_base,
+            scope=ldap.SCOPE_SUBTREE,
+            filterstr=self._user_search_template.format(escape_filter_chars(username)),
+            attrlist=[],
+        )
         results = [result[0] for result in results]  # extract DNs only
 
         if len(results) > 1:
-            raise LDAPException(f"User {username} found multiple times: Please check authorization.search_filter")
+            raise LDAPException(
+                f"User {username} found multiple times: Please check authorization.search_filter"
+            )
         elif len(results) == 0:
             raise LDAPException(f"User {username} not found")
 
         return results[0]
 
     def authenticate(self, username: str, password: str):
         user_dn = self._find_user(username)
@@ -227,16 +242,22 @@
 
 def main():
     try:
         config = Config.from_file(LDAP_CONFIG)
         vpn_params = OpenVPNParameters(config.static_challenge_mode)
         setup_logging(vpn_params.verbosity)
         logging.info(f"Authenticating {vpn_params.user}")
-        authenticator = LDAPAuthenticator(config.url, config.bind_dn, config.password, config.base_dn,
-                                          config.search_filter, config.timeout)
+        authenticator = LDAPAuthenticator(
+            config.url,
+            config.bind_dn,
+            config.password,
+            config.base_dn,
+            config.search_filter,
+            config.timeout,
+        )
         authenticator.authenticate(vpn_params.user, vpn_params.full_password)
     except Exception as e:
         logging.error(f"Exception while authenticating: {e}")
         traceback.print_exc()
         sys.exit(1)
     sys.exit(0)
```

### Comparing `openvpn-ldap-auth-0.1.6/pyproject.toml` & `openvpn_ldap_auth-0.1.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openvpn-ldap-auth"
-version = "0.1.6"
+version = "0.1.7"
 description = "An auth verify script for OpenVPN to authenticate via LDAP."
 authors = ["Philipp Hossner <philipph@posteo.de>"]
 license = 'MIT'
 readme = 'README.md'
 homepage = 'https://github.com/phihos/python-openvpn-ldap-auth/'
 repository = 'https://github.com/phihos/python-openvpn-ldap-auth/'
 keywords = [
@@ -22,53 +22,56 @@
 
 packages = [{ include = "openvpn_ldap_auth" }, ]
 
 [tool.poetry.scripts]
 openvpn-ldap-auth = 'openvpn_ldap_auth.main:main'
 
 [tool.poetry.dependencies]
-python = "^3.6"
-PyYAML = "^5.4.1"
+python = ">= 3.8, < 3.13"
+PyYAML = "^6.0.1"
 python-ldap = "^3.3.1"
 Cerberus = "^1.3.2"
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2"
-pytest-timeout = "^1.4.2"
+[tool.poetry.group.dev.dependencies]
+pytest = ">=6.2,<9.0"
+pytest-timeout = ">=1.4.2,<3.0.0"
 pexpect = "^4.8.0"
-pyinstaller = "^4.2"
-plotly = "^4.14.3"
+pyinstaller = "^6.5.0"
+plotly = ">=4.14.3,<6.0.0"
 kaleido = "0.2.1"
 stdeb = "^0.10.0"
+tox = "^4.14.2"
+black = {version = "24.3.0", extras = ["d"]}
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = true
-envlist = python{36,37,38,39}-openvpn{24,25}
+envlist = python{38,39,310,311,312}-openvpn{24,25}
 basepython = python3
 
-[testenv:python{36,37,38,39}-openvpn{24,25}]
+[testenv:python{38,39,310,311,312}-openvpn{24,25}]
 skip_install = true
 setenv =
-    python36: python_version=3.6
-    python37: python_version=3.7
     python38: python_version=3.8
     python39: python_version=3.9
+    python310: python_version=3.10
+    python311: python_version=3.11
+    python312: python_version=3.12
     openvpn23: openvpn_version=2.3
     openvpn24: openvpn_version=2.4
     openvpn25: openvpn_version=2.5
-whitelist_externals =
+allowlist_externals =
     docker-compose
     bash
 commands_pre:
     docker-compose -f tests/resources/docker/docker-compose.yml up -d --build
     docker-compose -f tests/resources/docker/docker-compose.yml run openvpn bash -c 'openvpn --version || true'
 commands =
-    docker-compose -f tests/resources/docker/docker-compose.yml run openvpn bash -c 'poetry install && poetry build && ./pyinstaller.sh && mv dist/openvpn-ldap-auth /usr/bin/openvpn-ldap-auth-pyinstaller && pip install --upgrade --find-links=dist openvpn-ldap-auth && poetry run pytest {posargs}'
+    docker-compose -f tests/resources/docker/docker-compose.yml run openvpn bash -c 'poetry install && poetry build && ./pyinstaller.sh && mv dist/openvpn-ldap-auth /usr/bin/openvpn-ldap-auth-pyinstaller && pip install --upgrade dist/*.whl && poetry run pytest {posargs}'
 commands_post:
     bash -c "docker-compose -f tests/resources/docker/docker-compose.yml run openvpn chown -R $UID /project"
     docker-compose -f tests/resources/docker/docker-compose.yml down
 """
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `openvpn-ldap-auth-0.1.6/setup.py` & `openvpn_ldap_auth-0.1.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,167 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: openvpn-ldap-auth
+Version: 0.1.7
+Summary: An auth verify script for OpenVPN to authenticate via LDAP.
+Home-page: https://github.com/phihos/python-openvpn-ldap-auth/
+License: MIT
+Keywords: OpenVPN,LDAP
+Author: Philipp Hossner
+Author-email: philipph@posteo.de
+Requires-Python: >=3.8,<3.13
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Plugins
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
+Requires-Dist: Cerberus (>=1.3.2,<2.0.0)
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
+Requires-Dist: python-ldap (>=3.3.1,<4.0.0)
+Project-URL: Repository, https://github.com/phihos/python-openvpn-ldap-auth/
+Description-Content-Type: text/markdown
 
-packages = \
-['openvpn_ldap_auth']
+# Python OpenVPN LDAP Auth
 
-package_data = \
-{'': ['*']}
+[![PyPI license](https://img.shields.io/pypi/l/openvpn-ldap-auth.svg)](https://pypi.python.org/pypi/openvpn-ldap-auth/)
+[![PyPI status](https://img.shields.io/pypi/status/openvpn-ldap-auth.svg)](https://pypi.python.org/pypi/openvpn-ldap-auth/)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/openvpn-ldap-auth.svg)](https://pypi.python.org/pypi/openvpn-ldap-auth/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/openvpn-ldap-auth.svg)](https://pypi.python.org/pypi/openvpn-ldap-auth/)
+![main build status](https://github.com/phihos/Python-OpenVPN-LDAP-Auth/actions/workflows/test.yml/badge.svg?branch=main)
 
-install_requires = \
-['Cerberus>=1.3.2,<2.0.0', 'PyYAML>=5.4.1,<6.0.0', 'python-ldap>=3.3.1,<4.0.0']
-
-entry_points = \
-{'console_scripts': ['openvpn-ldap-auth = openvpn_ldap_auth.main:main']}
-
-setup_kwargs = {
-    'name': 'openvpn-ldap-auth',
-    'version': '0.1.6',
-    'description': 'An auth verify script for OpenVPN to authenticate via LDAP.',
-    'long_description': '# Python OpenVPN LDAP Auth\n\n[![PyPI license](https://img.shields.io/pypi/l/openvpn-ldap-auth.svg)](https://pypi.python.org/pypi/openvpn-ldap-auth/)\n[![PyPI status](https://img.shields.io/pypi/status/openvpn-ldap-auth.svg)](https://pypi.python.org/pypi/openvpn-ldap-auth/)\n[![PyPI version shields.io](https://img.shields.io/pypi/v/openvpn-ldap-auth.svg)](https://pypi.python.org/pypi/openvpn-ldap-auth/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/openvpn-ldap-auth.svg)](https://pypi.python.org/pypi/openvpn-ldap-auth/)\n![main build status](https://github.com/phihos/Python-OpenVPN-LDAP-Auth/actions/workflows/test.yml/badge.svg?branch=main)\n\nAn auth verify script for [OpenVPN](https://community.openvpn.net) to authenticate via LDAP. Each VPN login is\nforwarded to this script and the script in turn attempts a simple bind against the specified LDAP server. When the bind\nis successful the script returns exit code 0 telling OpenVPN that the credentials are valid.\n\nAlthough there already is the [openvpn-auth-ldap](https://github.com/threerings/openvpn-auth-ldap) plugin I felt the\nneed to write this auth script. First the source code is more accessible due to it being written in Python. Second it\noffers more possibilities regarding\nOpenVPN\'s [`static-challenge`](https://openvpn.net/community-resources/reference-manual-for-openvpn-2-4/) parameter (see\nbelow).\n\nThe downsides of using a script instead of a C-plugin\nare [less performance and slightly reduced security](https://openvpn.net/community-resources/using-alternative-authentication-methods/).\nIf you are fine with that go ahead.\n\n## Quickstart\n\nInstall the package via pip:\n\n```shell\npip install openvpn-ldap-auth\n```\n\nThen create `/etc/openvpn/ldap.yaml`:\n\n```yaml\nldap:\n  url: \'ldaps://first.ldap.tld:636/ ldaps://second.ldap.tld:636/\'\n  bind_dn: \'uid=readonly,dc=example,dc=org\'\n  password: \'somesecurepassword\'\n  timeout: 5 # optional\nauthorization:\n  base_dn: \'ou=people,dc=example,dc=org\'\n  search_filter: \'(uid={})\' # optional, {} will be replaced with the username\n  static_challenge: \'ignore\' # optional, other values are prepend, append \n```\n\nFind out where `openvpn-ldap-auth` lives:\n\n```shell\nwhich openvpn-ldap-auth\n```\n\nAdd the following line to your OpenVPN server configuration:\n\n```\nscript-security 2\nauth-user-pass-verify /path/to/openvpn-ldap-auth via-file\n```\n\nNow you can start your OpenVPN server and try to connect with a client.\n\n## Installation\n\n### Single Executable\n\nFor those who wish to [sacrifice a little more performance](https://pyinstaller.readthedocs.io/en/stable/operating-mode.html#how-the-one-file-program-works) for not having to install or compile a Python interpreter or you just want to quickly try the script out this option might be interesting.\nEach [release](https://github.com/phihos/python-openvpn-ldap-auth/releases) also has executables attached to it: *openvpn-ldap-auth-&lt;distro&gt;-&lt;distro-version&gt;-&lt;arch&gt;*. They are created via [PyInstaller](https://www.pyinstaller.org/) on the respective Linux distro, version and architecture. They might also work on other distros provided they use the same or a later libc version that the distro uses.\n\n**Important: /tmp must not be read only.**\n\n### From Source\n\nDownload or clone this repository, cd into it and run\n\n```shell\npip install poetry\npoetry install --no-dev\npoetry build\npip install --upgrade --find-links=dist openvpn-ldap-auth\n```\n\nExchange `pip` with `pip3` if applicable.\n\n## Configuration\n\n### Static Challenge\n\nIf you want users to provide a normal password combined with a one-time-password OpenVPN\'s\n[`static-challenge`](https://openvpn.net/community-resources/reference-manual-for-openvpn-2-4/) parameter is what you\nare looking for.\n\nIn the client configuration you need to add a line like\n\n```\nstatic-challenge "Enter OTP" 1 # use 0 if the OTP should not be echoed\n```\n\nWhen connecting you will now be prompted for your password and your OTP. By setting `authorization.static_challenge` you\ncan now influence how the OTP is used:\n\n- *ignore (default)*: Just use the password for binding.\n- *prepend*: Prepend the OTP to your password and use that for binding.\n- *append*: Append the OTP to your password and use that for binding.\n\nThe last two options are useful if your LDAP server offers internal 2FA validation \nlike [oath-ldap](https://oath-ldap.stroeder.com/).\n\n### Using `via-env`\n\nIn the server configuration the following alternative setting is also supported but discouraged:\n\n```\nauth-user-pass-verify /path/to/openvpn-ldap-auth via-env\n```\n\nOpenVPN\'s manpage about that topic:\n\n*If method is set to "via-env", OpenVPN will call script with the environmental variables username and password set to \nthe username/password strings provided by the client. Be aware that this method is insecure on some platforms which \nmake the environment of a process publicly visible to other unprivileged processes.*\n\nIf you still want to use `via-env` make sure to set `script-security` to `3`.\n\n## Running Tests\n\nFirst make sure to install [Docker](https://docs.docker.com/engine/install/)\nwith [docker-compose](https://docs.docker.com/compose/install/)\nand [tox](https://tox.readthedocs.io/en/latest/install.html). Then run\n\n```shell\ntox\n```\n\nTo run a specific Python-OpenVPN combination run something like\n\n```shell\ntox -e python38-openvpn25\n```\n\nTo see a full list of current environment see the `tool.tox` section in [pyproject.toml](pyproject.toml).\n',
-    'author': 'Philipp Hossner',
-    'author_email': 'philipph@posteo.de',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/phihos/python-openvpn-ldap-auth/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
-}
+An auth verify script for [OpenVPN](https://community.openvpn.net) to authenticate via LDAP. Each VPN login is
+forwarded to this script and the script in turn attempts a simple bind against the specified LDAP server. When the bind
+is successful the script returns exit code 0 telling OpenVPN that the credentials are valid.
 
+Although there already is the [openvpn-auth-ldap](https://github.com/threerings/openvpn-auth-ldap) plugin I felt the
+need to write this auth script. First the source code is more accessible due to it being written in Python. Second it
+offers more possibilities regarding
+OpenVPN's [`static-challenge`](https://openvpn.net/community-resources/reference-manual-for-openvpn-2-4/) parameter (see
+below).
+
+The downsides of using a script instead of a C-plugin
+are [less performance and slightly reduced security](https://openvpn.net/community-resources/using-alternative-authentication-methods/).
+If you are fine with that go ahead.
+
+## Quickstart
+
+Install the package via pip:
+
+```shell
+pip install openvpn-ldap-auth
+```
+
+Then create `/etc/openvpn/ldap.yaml`:
+
+```yaml
+ldap:
+  url: 'ldaps://first.ldap.tld:636/ ldaps://second.ldap.tld:636/'
+  bind_dn: 'uid=readonly,dc=example,dc=org'
+  password: 'somesecurepassword'
+  timeout: 5 # (optional) wait this many seconds for connection and response
+authorization:
+  base_dn: 'ou=people,dc=example,dc=org'
+  search_filter: '(uid={})' # optional, {} will be replaced with the username
+  static_challenge: 'ignore' # optional, other values are prepend, append 
+```
+
+Find out where `openvpn-ldap-auth` lives:
+
+```shell
+which openvpn-ldap-auth
+```
+
+Add the following line to your OpenVPN server configuration:
+
+```
+script-security 2
+auth-user-pass-verify /path/to/openvpn-ldap-auth via-file
+```
+
+Now you can start your OpenVPN server and try to connect with a client.
+
+## Installation
+
+### Single Executable
+
+For those who wish to [sacrifice a little more performance](https://pyinstaller.readthedocs.io/en/stable/operating-mode.html#how-the-one-file-program-works) for not having to install or compile a Python interpreter or you just want to quickly try the script out this option might be interesting.
+Each [release](https://github.com/phihos/python-openvpn-ldap-auth/releases) also has executables attached to it: *openvpn-ldap-auth-&lt;distro&gt;-&lt;distro-version&gt;-&lt;arch&gt;*. They are created via [PyInstaller](https://www.pyinstaller.org/) on the respective Linux distro, version and architecture. They might also work on other distros provided they use the same or a later libc version that the distro uses.
+
+**Important: /tmp must not be read only.**
+
+### From Source
+
+Download or clone this repository, cd into it and run
+
+```shell
+pip install poetry
+poetry install --no-dev
+poetry build
+pip install --upgrade --find-links=dist openvpn-ldap-auth
+```
+
+Exchange `pip` with `pip3` if applicable.
+
+## Configuration
+
+### Static Challenge
+
+If you want users to provide a normal password combined with a one-time-password OpenVPN's
+[`static-challenge`](https://openvpn.net/community-resources/reference-manual-for-openvpn-2-4/) parameter is what you
+are looking for.
+
+In the client configuration you need to add a line like
+
+```
+static-challenge "Enter OTP" 1 # use 0 if the OTP should not be echoed
+```
+
+When connecting you will now be prompted for your password and your OTP. By setting `authorization.static_challenge` you
+can now influence how the OTP is used:
+
+- *ignore (default)*: Just use the password for binding.
+- *prepend*: Prepend the OTP to your password and use that for binding.
+- *append*: Append the OTP to your password and use that for binding.
+
+The last two options are useful if your LDAP server offers internal 2FA validation 
+like [oath-ldap](https://oath-ldap.stroeder.com/).
+
+### Using `via-env`
+
+In the server configuration the following alternative setting is also supported but discouraged:
+
+```
+auth-user-pass-verify /path/to/openvpn-ldap-auth via-env
+```
+
+OpenVPN's manpage about that topic:
+
+*If method is set to "via-env", OpenVPN will call script with the environmental variables username and password set to 
+the username/password strings provided by the client. Be aware that this method is insecure on some platforms which 
+make the environment of a process publicly visible to other unprivileged processes.*
+
+If you still want to use `via-env` make sure to set `script-security` to `3`.
+
+## Running Tests
+
+First make sure to install [Docker](https://docs.docker.com/engine/install/)
+with [docker-compose](https://docs.docker.com/compose/install/)
+and [tox](https://tox.readthedocs.io/en/latest/install.html). Then run
+
+```shell
+tox
+```
+
+To run a specific Python-OpenVPN combination run something like
+
+```shell
+tox -e python38-openvpn25
+```
+
+To see a full list of current environment see the `tool.tox` section in [pyproject.toml](pyproject.toml).
 
-setup(**setup_kwargs)
```

