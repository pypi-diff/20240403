# Comparing `tmp/Flask-SimpleLDAP-1.4.0.tar.gz` & `tmp/Flask-SimpleLDAP-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-SimpleLDAP-1.4.0.tar", last modified: Tue Jul 16 10:16:25 2019, max compression
+gzip compressed data, was "Flask-SimpleLDAP-2.0.0.tar", last modified: Wed Apr  3 19:18:51 2024, max compression
```

## Comparing `Flask-SimpleLDAP-1.4.0.tar` & `Flask-SimpleLDAP-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-07-16 10:16:25.000000 Flask-SimpleLDAP-1.4.0/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-07-16 10:16:25.000000 Flask-SimpleLDAP-1.4.0/Flask_SimpleLDAP.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      797 2019-07-16 10:16:24.000000 Flask-SimpleLDAP-1.4.0/Flask_SimpleLDAP.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      285 2019-07-16 10:16:25.000000 Flask-SimpleLDAP-1.4.0/Flask_SimpleLDAP.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2019-07-16 10:16:24.000000 Flask-SimpleLDAP-1.4.0/Flask_SimpleLDAP.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2019-07-14 23:22:55.000000 Flask-SimpleLDAP-1.4.0/Flask_SimpleLDAP.egg-info/not-zip-safe
--rw-r--r--   0 alex       (501) staff       (20)       33 2019-07-16 10:16:24.000000 Flask-SimpleLDAP-1.4.0/Flask_SimpleLDAP.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       17 2019-07-16 10:16:24.000000 Flask-SimpleLDAP-1.4.0/Flask_SimpleLDAP.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)      797 2019-07-16 10:16:25.000000 Flask-SimpleLDAP-1.4.0/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     2768 2019-07-15 04:16:26.000000 Flask-SimpleLDAP-1.4.0/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-07-16 10:16:25.000000 Flask-SimpleLDAP-1.4.0/flask_simpleldap/
--rw-r--r--   0 alex       (501) staff       (20)    15245 2019-07-16 10:06:02.000000 Flask-SimpleLDAP-1.4.0/flask_simpleldap/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)       38 2019-07-16 10:16:25.000000 Flask-SimpleLDAP-1.4.0/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     1031 2019-07-16 10:13:13.000000 Flask-SimpleLDAP-1.4.0/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-03 19:18:51.788297 Flask-SimpleLDAP-2.0.0/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-03 19:18:51.787977 Flask-SimpleLDAP-2.0.0/Flask_SimpleLDAP.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     9852 2024-04-03 19:18:51.000000 Flask-SimpleLDAP-2.0.0/Flask_SimpleLDAP.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      342 2024-04-03 19:18:51.000000 Flask-SimpleLDAP-2.0.0/Flask_SimpleLDAP.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-03 19:18:51.000000 Flask-SimpleLDAP-2.0.0/Flask_SimpleLDAP.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-03 17:13:16.000000 Flask-SimpleLDAP-2.0.0/Flask_SimpleLDAP.egg-info/not-zip-safe
+-rw-r--r--   0 alex       (501) staff       (20)       32 2024-04-03 19:18:51.000000 Flask-SimpleLDAP-2.0.0/Flask_SimpleLDAP.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       17 2024-04-03 19:18:51.000000 Flask-SimpleLDAP-2.0.0/Flask_SimpleLDAP.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)     1084 2023-10-05 00:04:37.000000 Flask-SimpleLDAP-2.0.0/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)     9852 2024-04-03 19:18:51.788165 Flask-SimpleLDAP-2.0.0/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     8959 2024-04-03 19:16:04.000000 Flask-SimpleLDAP-2.0.0/README.md
+-rw-r--r--   0 alex       (501) staff       (20)        6 2024-04-03 19:16:04.000000 Flask-SimpleLDAP-2.0.0/VERSION
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-03 19:18:51.787683 Flask-SimpleLDAP-2.0.0/flask_simpleldap/
+-rw-r--r--   0 alex       (501) staff       (20)    19542 2024-04-03 19:16:04.000000 Flask-SimpleLDAP-2.0.0/flask_simpleldap/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)       81 2024-04-03 19:16:04.000000 Flask-SimpleLDAP-2.0.0/pyproject.toml
+-rw-r--r--   0 alex       (501) staff       (20)      906 2024-04-03 19:18:51.788573 Flask-SimpleLDAP-2.0.0/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-03 19:18:51.787828 Flask-SimpleLDAP-2.0.0/tests/
+-rw-r--r--   0 alex       (501) staff       (20)      999 2024-04-03 19:16:04.000000 Flask-SimpleLDAP-2.0.0/tests/test_simpleldap.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Flask-SimpleLDAP-1.4.0/flask_simpleldap/__init__.py` & `Flask-SimpleLDAP-2.0.0/flask_simpleldap/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 from functools import wraps
 import ldap
 from ldap import filter as ldap_filter
-from flask import abort, current_app, g, make_response, redirect, url_for, \
-    request
+from flask import abort, current_app, g, make_response, redirect, url_for, request
 
-__all__ = ['LDAP']
+__all__ = ["LDAP"]
 
 
 class LDAPException(RuntimeError):
     message = None
 
     def __init__(self, message):
         self.message = message
@@ -28,80 +27,88 @@
     def init_app(app):
         """Initialize the `app` for use with this :class:`~LDAP`. This is
         called automatically if `app` is passed to :meth:`~LDAP.__init__`.
 
         :param flask.Flask app: the application to configure for use with
            this :class:`~LDAP`
         """
-        app.config.setdefault('LDAP_HOST', 'localhost')
-        app.config.setdefault('LDAP_PORT', 389)
-        app.config.setdefault('LDAP_SCHEMA', 'ldap')
-        app.config.setdefault('LDAP_USERNAME', None)
-        app.config.setdefault('LDAP_PASSWORD', None)
-        app.config.setdefault('LDAP_TIMEOUT', 10)
-        app.config.setdefault('LDAP_USE_SSL', False)
-        app.config.setdefault('LDAP_USE_TLS', False)
-        app.config.setdefault('LDAP_REQUIRE_CERT', False)
-        app.config.setdefault('LDAP_CERT_PATH', '/path/to/cert')
-        app.config.setdefault('LDAP_BASE_DN', None)
-        app.config.setdefault('LDAP_OBJECTS_DN', 'distinguishedName')
-        app.config.setdefault('LDAP_USER_FIELDS', [])
-        app.config.setdefault('LDAP_USER_OBJECT_FILTER',
-                              '(&(objectclass=Person)(userPrincipalName=%s))')
-        app.config.setdefault('LDAP_USER_GROUPS_FIELD', 'memberOf')
-        app.config.setdefault('LDAP_GROUP_FIELDS', [])
-        app.config.setdefault('LDAP_GROUP_OBJECT_FILTER',
-                              '(&(objectclass=Group)(userPrincipalName=%s))')
-        app.config.setdefault('LDAP_GROUP_MEMBERS_FIELD', 'member')
-        app.config.setdefault('LDAP_LOGIN_VIEW', 'login')
-        app.config.setdefault('LDAP_REALM_NAME', 'LDAP authentication')
-        app.config.setdefault('LDAP_OPENLDAP', False)
-        app.config.setdefault('LDAP_GROUP_MEMBER_FILTER', '*')
-        app.config.setdefault('LDAP_GROUP_MEMBER_FILTER_FIELD', '*')
-        app.config.setdefault('LDAP_CUSTOM_OPTIONS', None)
-
-        if app.config['LDAP_USE_SSL'] or app.config['LDAP_USE_TLS']:
-            ldap.set_option(ldap.OPT_X_TLS_REQUIRE_CERT,
-                            ldap.OPT_X_TLS_NEVER)
-
-        if app.config['LDAP_REQUIRE_CERT']:
-            ldap.set_option(ldap.OPT_X_TLS_REQUIRE_CERT,
-                            ldap.OPT_X_TLS_DEMAND)
-            ldap.set_option(ldap.OPT_X_TLS_CACERTFILE,
-                            current_app.config['LDAP_CERT_PATH'])
-
-        for option in ['USERNAME', 'PASSWORD', 'BASE_DN']:
-            if app.config['LDAP_{0}'.format(option)] is None:
-                raise LDAPException('LDAP_{0} cannot be None!'.format(option))
+        app.config.setdefault("LDAP_HOST", "localhost")
+        app.config.setdefault("LDAP_PORT", 389)
+        app.config.setdefault("LDAP_SCHEMA", "ldap")
+        app.config.setdefault("LDAP_SOCKET_PATH", "/")
+        app.config.setdefault("LDAP_USERNAME", None)
+        app.config.setdefault("LDAP_PASSWORD", None)
+        app.config.setdefault("LDAP_TIMEOUT", 10)
+        app.config.setdefault("LDAP_USE_SSL", False)
+        app.config.setdefault("LDAP_USE_TLS", False)
+        app.config.setdefault("LDAP_REQUIRE_CERT", False)
+        app.config.setdefault("LDAP_CERT_PATH", "/path/to/cert")
+        app.config.setdefault("LDAP_BASE_DN", None)
+        app.config.setdefault("LDAP_OBJECTS_DN", "distinguishedName")
+        app.config.setdefault("LDAP_USER_FIELDS", [])
+        app.config.setdefault("LDAP_USER_GROUPS_FIELD", "memberOf")
+        app.config.setdefault(
+            "LDAP_USER_OBJECT_FILTER", "(&(objectclass=Person)(userPrincipalName=%s))"
+        )
+        app.config.setdefault("LDAP_USERS_OBJECT_FILTER", "objectclass=Person")
+        app.config.setdefault("LDAP_GROUP_FIELDS", [])
+        app.config.setdefault("LDAP_GROUP_MEMBERS_FIELD", "member")
+        app.config.setdefault(
+            "LDAP_GROUP_OBJECT_FILTER", "(&(objectclass=Group)(userPrincipalName=%s))"
+        )
+        app.config.setdefault("LDAP_GROUPS_OBJECT_FILTER", "objectclass=Group")
+        app.config.setdefault("LDAP_LOGIN_VIEW", "login")
+        app.config.setdefault("LDAP_REALM_NAME", "LDAP authentication")
+        app.config.setdefault("LDAP_OPENLDAP", False)
+        app.config.setdefault("LDAP_GROUP_MEMBER_FILTER", "*")
+        app.config.setdefault("LDAP_GROUP_MEMBER_FILTER_FIELD", "*")
+        app.config.setdefault("LDAP_CUSTOM_OPTIONS", None)
+
+        if app.config["LDAP_USE_SSL"] or app.config["LDAP_USE_TLS"]:
+            ldap.set_option(ldap.OPT_X_TLS_REQUIRE_CERT, ldap.OPT_X_TLS_NEVER)
+
+        if app.config["LDAP_REQUIRE_CERT"]:
+            ldap.set_option(ldap.OPT_X_TLS_REQUIRE_CERT, ldap.OPT_X_TLS_DEMAND)
+            ldap.set_option(ldap.OPT_X_TLS_CACERTFILE, app.config["LDAP_CERT_PATH"])
+
+        if app.config["LDAP_BASE_DN"] is None:
+            raise LDAPException("LDAP_BASE_DN cannot be None!")
+
+        if app.config["LDAP_SCHEMA"] != "ldapi":
+            for option in ["USERNAME", "PASSWORD"]:
+                if app.config[f"LDAP_{option}"] is None:
+                    raise LDAPException(f"LDAP_{option} cannot be None!")
 
     @staticmethod
     def _set_custom_options(conn):
-        options = current_app.config['LDAP_CUSTOM_OPTIONS']
+        options = current_app.config["LDAP_CUSTOM_OPTIONS"]
         if options:
             for k, v in options.items():
                 conn.set_option(k, v)
         return conn
 
     @property
     def initialize(self):
         """Initialize a connection to the LDAP server.
 
         :return: LDAP connection object.
         """
 
         try:
-            conn = ldap.initialize('{0}://{1}:{2}'.format(
-                current_app.config['LDAP_SCHEMA'],
-                current_app.config['LDAP_HOST'],
-                current_app.config['LDAP_PORT']))
-            conn.set_option(ldap.OPT_NETWORK_TIMEOUT,
-                            current_app.config['LDAP_TIMEOUT'])
+            if current_app.config["LDAP_SCHEMA"] == "ldapi":
+                uri = f"{current_app.config['LDAP_SCHEMA']}://{current_app.config['LDAP_SOCKET_PATH']}"
+            else:
+                uri = f"{current_app.config['LDAP_SCHEMA']}://{current_app.config['LDAP_HOST']}:{current_app.config['LDAP_PORT']}"
+            conn = ldap.initialize(uri)
+            conn.set_option(
+                ldap.OPT_NETWORK_TIMEOUT, current_app.config["LDAP_TIMEOUT"]
+            )
             conn = self._set_custom_options(conn)
             conn.protocol_version = ldap.VERSION3
-            if current_app.config['LDAP_USE_TLS']:
+            if current_app.config["LDAP_USE_TLS"]:
                 conn.start_tls_s()
             return conn
         except ldap.LDAPError as e:
             raise LDAPException(self.error(e.args))
 
     @property
     def bind(self):
@@ -111,16 +118,16 @@
         :return: Bound LDAP connection object if successful or ``None`` if
             unsuccessful.
         """
 
         conn = self.initialize
         try:
             conn.simple_bind_s(
-                current_app.config['LDAP_USERNAME'],
-                current_app.config['LDAP_PASSWORD'])
+                current_app.config["LDAP_USERNAME"], current_app.config["LDAP_PASSWORD"]
+            )
             return conn
         except ldap.LDAPError as e:
             raise LDAPException(self.error(e.args))
 
     def bind_user(self, username, password):
         """Attempts to bind a user to the LDAP server using the credentials
         supplied.
@@ -143,142 +150,245 @@
 
         user_dn = self.get_object_details(user=username, dn_only=True)
 
         if user_dn is None:
             return
         try:
             conn = self.initialize
-            _user_dn = user_dn.decode('utf-8') \
-                if isinstance(user_dn, bytes) else user_dn
+            _user_dn = (
+                user_dn.decode("utf-8") if isinstance(user_dn, bytes) else user_dn
+            )
             conn.simple_bind_s(_user_dn, password)
             return True
         except ldap.LDAPError:
             return
 
-    def get_object_details(self, user=None, group=None, query_filter=None,
-                           dn_only=False):
+    def get_users(self, fields=None, dn_only=False):
+        """Returns a ``list`` with the users in base dn
+        or empty ``list`` if unsuccessful.
+
+        LDAP query setting is ``LDAP_USERS_OBJECT_FILTER``
+
+        :param fields: list of user fields to retrieve.
+         if ``None`` or empty, default user fields
+         ``LDAP_USER_FIELDS`` is used
+        :param bool dn_only: If we should only retrieve the object's
+            distinguished name or not. Default: ``False``.
+        :type fields: list
+        """
+        conn = self.bind
+        try:
+            fields = fields or current_app.config["LDAP_USER_FIELDS"]
+            if current_app.config["LDAP_OPENLDAP"]:
+                records = conn.search_s(
+                    current_app.config["LDAP_BASE_DN"],
+                    ldap.SCOPE_SUBTREE,
+                    current_app.config["LDAP_USERS_OBJECT_FILTER"],
+                    fields,
+                )
+            else:
+                records = conn.search_s(
+                    current_app.config["LDAP_BASE_DN"],
+                    ldap.SCOPE_SUBTREE,
+                    current_app.config["LDAP_USERS_OBJECT_FILTER"],
+                    fields,
+                )
+            conn.unbind_s()
+            if records:
+                if dn_only:
+                    return [r[0] for r in records]
+                else:
+                    return [r[1] for r in records]
+            else:
+                return []
+        except ldap.LDAPError as e:
+            raise LDAPException(self.error(e.args))
+
+    def get_object_details(
+        self, user=None, group=None, query_filter=None, dn_only=False
+    ):
         """Returns a ``dict`` with the object's (user or group) details.
 
         :param str user: Username of the user object you want details for.
         :param str group: Name of the group object you want details for.
         :param str query_filter: If included, will be used to query object.
         :param bool dn_only: If we should only retrieve the object's
             distinguished name or not. Default: ``False``.
         """
         query = None
         fields = None
         if user is not None:
             if not dn_only:
-                fields = current_app.config['LDAP_USER_FIELDS']
-            query_filter = query_filter or \
-                           current_app.config['LDAP_USER_OBJECT_FILTER']
+                fields = current_app.config["LDAP_USER_FIELDS"]
+            query_filter = query_filter or current_app.config["LDAP_USER_OBJECT_FILTER"]
             query = ldap_filter.filter_format(query_filter, (user,))
         elif group is not None:
             if not dn_only:
-                fields = current_app.config['LDAP_GROUP_FIELDS']
-            query_filter = query_filter or \
-                           current_app.config['LDAP_GROUP_OBJECT_FILTER']
+                fields = current_app.config["LDAP_GROUP_FIELDS"]
+            query_filter = (
+                query_filter or current_app.config["LDAP_GROUP_OBJECT_FILTER"]
+            )
             query = ldap_filter.filter_format(query_filter, (group,))
         conn = self.bind
         try:
-            records = conn.search_s(current_app.config['LDAP_BASE_DN'],
-                                    ldap.SCOPE_SUBTREE, query, fields)
+            records = conn.search_s(
+                current_app.config["LDAP_BASE_DN"], ldap.SCOPE_SUBTREE, query, fields
+            )
             conn.unbind_s()
             result = {}
-            if records:
+            if (
+                records
+                and records[0][0] is not None
+                and isinstance(records[0][1], dict)
+            ):
                 if dn_only:
-                    if current_app.config['LDAP_OPENLDAP']:
+                    if current_app.config["LDAP_OPENLDAP"]:
                         if records:
                             return records[0][0]
                     else:
-                        if current_app.config['LDAP_OBJECTS_DN'] \
-                                in records[0][1]:
-                            dn = records[0][1][
-                                current_app.config['LDAP_OBJECTS_DN']]
+                        if current_app.config["LDAP_OBJECTS_DN"] in records[0][1]:
+                            dn = records[0][1][current_app.config["LDAP_OBJECTS_DN"]]
                             return dn[0]
                 for k, v in list(records[0][1].items()):
                     result[k] = v
                 return result
         except ldap.LDAPError as e:
             raise LDAPException(self.error(e.args))
 
+    def get_groups(self, fields=None, dn_only=False):
+        """Returns a ``list`` with the groups in base dn
+        or an empty``list`` if unsuccessful.
+
+        LDAP query setting is ``LDAP_GROUPS_OBJECT_FILTER``
+
+        :param fields: list of group fields to retrieve.
+         if ``None`` or empty, default group fields is used
+        :type fields: list
+        :param bool dn_only: If we should only retrieve the object's
+            distinguished name or not. Default: ``False``.
+        """
+        conn = self.bind
+        try:
+            fields = fields or current_app.config["LDAP_GROUP_FIELDS"]
+            if current_app.config["LDAP_OPENLDAP"]:
+                records = conn.search_s(
+                    current_app.config["LDAP_BASE_DN"],
+                    ldap.SCOPE_SUBTREE,
+                    current_app.config["LDAP_GROUPS_OBJECT_FILTER"],
+                    fields,
+                )
+            else:
+                records = conn.search_s(
+                    current_app.config["LDAP_BASE_DN"],
+                    ldap.SCOPE_SUBTREE,
+                    current_app.config["LDAP_GROUPS_OBJECT_FILTER"],
+                    fields,
+                )
+            conn.unbind_s()
+            if records:
+                if dn_only:
+                    return [r[0] for r in records]
+                else:
+                    return [r[1] for r in records]
+            else:
+                return []
+        except ldap.LDAPError as e:
+            raise LDAPException(self.error(e.args))
+
     def get_user_groups(self, user):
         """Returns a ``list`` with the user's groups or ``None`` if
         unsuccessful.
 
         :param str user: User we want groups for.
         """
 
         conn = self.bind
         try:
-            if current_app.config['LDAP_OPENLDAP']:
-                fields = \
-                    [str(current_app.config['LDAP_GROUP_MEMBER_FILTER_FIELD'])]
+            if current_app.config["LDAP_OPENLDAP"]:
+                fields = [str(current_app.config["LDAP_GROUP_MEMBER_FILTER_FIELD"])]
                 records = conn.search_s(
-                    current_app.config['LDAP_BASE_DN'], ldap.SCOPE_SUBTREE,
+                    current_app.config["LDAP_BASE_DN"],
+                    ldap.SCOPE_SUBTREE,
                     ldap_filter.filter_format(
-                        current_app.config['LDAP_GROUP_MEMBER_FILTER'],
-                        (self.get_object_details(user, dn_only=True),)),
-                    fields)
+                        current_app.config["LDAP_GROUP_MEMBER_FILTER"],
+                        (self.get_object_details(user, dn_only=True),),
+                    ),
+                    fields,
+                )
             else:
                 records = conn.search_s(
-                    current_app.config['LDAP_BASE_DN'], ldap.SCOPE_SUBTREE,
+                    current_app.config["LDAP_BASE_DN"],
+                    ldap.SCOPE_SUBTREE,
                     ldap_filter.filter_format(
-                        current_app.config['LDAP_USER_OBJECT_FILTER'],
-                        (user,)),
-                    [current_app.config['LDAP_USER_GROUPS_FIELD']])
+                        current_app.config["LDAP_USER_OBJECT_FILTER"], (user,)
+                    ),
+                    [current_app.config["LDAP_USER_GROUPS_FIELD"]],
+                )
 
             conn.unbind_s()
             if records:
-                if current_app.config['LDAP_OPENLDAP']:
-                    group_member_filter = \
-                        current_app.config['LDAP_GROUP_MEMBER_FILTER_FIELD']
-                    groups = [record[1][group_member_filter][0] for
-                              record in records]
+                if current_app.config["LDAP_OPENLDAP"]:
+                    group_member_filter = current_app.config[
+                        "LDAP_GROUP_MEMBER_FILTER_FIELD"
+                    ]
+                    record_list = [record[1] for record in records]
+                    record_dicts = [
+                        record for record in record_list if isinstance(record, dict)
+                    ]
+                    groups = [
+                        item.get([group_member_filter][0])[0] for item in record_dicts
+                    ]
                     return groups
                 else:
-                    if current_app.config['LDAP_USER_GROUPS_FIELD'] in \
-                            records[0][1]:
+                    if current_app.config["LDAP_USER_GROUPS_FIELD"] in records[0][1]:
                         groups = records[0][1][
-                            current_app.config['LDAP_USER_GROUPS_FIELD']]
-                        result = [re.findall(b'(?:cn=|CN=)(.*?),', group)[0]
-                                  for group in groups]
+                            current_app.config["LDAP_USER_GROUPS_FIELD"]
+                        ]
+                        result = [
+                            re.findall(b"(?:cn=|CN=)(.*?),", group)[0]
+                            for group in groups
+                        ]
+                        result = [r.decode("utf-8") for r in result]
                         return result
         except ldap.LDAPError as e:
             raise LDAPException(self.error(e.args))
 
     def get_group_members(self, group):
         """Returns a ``list`` with the group's members or ``None`` if
         unsuccessful.
 
         :param str group: Group we want users for.
         """
 
         conn = self.bind
         try:
             records = conn.search_s(
-                current_app.config['LDAP_BASE_DN'], ldap.SCOPE_SUBTREE,
+                current_app.config["LDAP_BASE_DN"],
+                ldap.SCOPE_SUBTREE,
                 ldap_filter.filter_format(
-                    current_app.config['LDAP_GROUP_OBJECT_FILTER'], (group,)),
-                [current_app.config['LDAP_GROUP_MEMBERS_FIELD']])
+                    current_app.config["LDAP_GROUP_OBJECT_FILTER"], (group,)
+                ),
+                [current_app.config["LDAP_GROUP_MEMBERS_FIELD"]],
+            )
             conn.unbind_s()
             if records:
-                if current_app.config['LDAP_GROUP_MEMBERS_FIELD'] in \
-                        records[0][1]:
+                if current_app.config["LDAP_GROUP_MEMBERS_FIELD"] in records[0][1]:
                     members = records[0][1][
-                        current_app.config['LDAP_GROUP_MEMBERS_FIELD']]
+                        current_app.config["LDAP_GROUP_MEMBERS_FIELD"]
+                    ]
+                    members = [m.decode("utf-8") for m in members]
                     return members
         except ldap.LDAPError as e:
             raise LDAPException(self.error(e.args))
 
     @staticmethod
     def error(e):
         e = e[0]
-        if 'desc' in e:
-            return e['desc']
+        if "desc" in e:
+            return e["desc"]
         else:
             return e
 
     @staticmethod
     def login_required(func):
         """When applied to a view function, any unauthenticated requests will
         be redirected to the view named in LDAP_LOGIN_VIEW. Authenticated
@@ -290,16 +400,20 @@
 
         :param func: The view function to decorate.
         """
 
         @wraps(func)
         def wrapped(*args, **kwargs):
             if g.user is None:
-                return redirect(url_for(current_app.config['LDAP_LOGIN_VIEW'],
-                                        next=request.full_path or request.path))
+                next_path = request.full_path or request.path
+                if next_path == "/?":
+                    return redirect(url_for(current_app.config["LDAP_LOGIN_VIEW"]))
+                return redirect(
+                    url_for(current_app.config["LDAP_LOGIN_VIEW"], next=next_path)
+                )
             return func(*args, **kwargs)
 
         return wrapped
 
     @staticmethod
     def group_required(groups=None):
         """When applied to a view function, any unauthenticated requests will
@@ -316,19 +430,22 @@
         """
 
         def wrapper(func):
             @wraps(func)
             def wrapped(*args, **kwargs):
                 if g.user is None:
                     return redirect(
-                        url_for(current_app.config['LDAP_LOGIN_VIEW'],
-                                next=request.full_path or request.path))
+                        url_for(
+                            current_app.config["LDAP_LOGIN_VIEW"],
+                            next=request.full_path or request.path,
+                        )
+                    )
                 match = [group for group in groups if group in g.ldap_groups]
                 if not match:
-                    abort(401)
+                    abort(403)
 
                 return func(*args, **kwargs)
 
             return wrapped
 
         return wrapper
 
@@ -344,38 +461,40 @@
         username is stored in ``flask.g.ldap_username`` and the password in
         ``flask.g.ldap_password``.
 
         :param func: The view function to decorate.
         """
 
         def make_auth_required_response():
-            response = make_response('Unauthorized', 401)
-            response.www_authenticate.set_basic(
-                current_app.config['LDAP_REALM_NAME'])
+            response = make_response("Unauthorized", 401)
+            response.headers["WWW-Authenticate"] = (
+                f'Basic realm="{current_app.config["LDAP_REALM_NAME"]}"'
+            )
             return response
 
         @wraps(func)
         def wrapped(*args, **kwargs):
             if request.authorization is None:
                 req_username = None
                 req_password = None
             else:
                 req_username = request.authorization.username
                 req_password = request.authorization.password
             # Many LDAP servers will grant you anonymous access if you log in
             # with an empty password, even if you supply a non-anonymous user
             # ID, causing .bind_user() to return True. Therefore, only accept
             # non-empty passwords.
-            if req_username in ['', None] or req_password in ['', None]:
-                current_app.logger.debug('Got a request without auth data')
+            if req_username in ["", None] or req_password in ["", None]:
+                current_app.logger.debug("Got a request without auth data")
                 return make_auth_required_response()
 
             if not self.bind_user(req_username, req_password):
-                current_app.logger.debug('User {0!r} gave wrong '
-                                         'password'.format(req_username))
+                current_app.logger.debug(
+                    "User {0!r} gave wrong " "password".format(req_username)
+                )
                 return make_auth_required_response()
 
             g.ldap_username = req_username
             g.ldap_password = req_password
 
             return func(*args, **kwargs)
```

