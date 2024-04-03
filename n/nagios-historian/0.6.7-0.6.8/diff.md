# Comparing `tmp/nagios_historian-0.6.7.tar.gz` & `tmp/nagios_historian-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nagios_historian-0.6.7.tar", last modified: Tue Oct  1 19:39:09 2019, max compression
+gzip compressed data, was "nagios_historian-0.6.8.tar", last modified: Wed Apr  3 19:18:32 2024, max compression
```

## Comparing `nagios_historian-0.6.7.tar` & `nagios_historian-0.6.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 v759329   (1005) v759329   (1005)        0 2019-10-01 19:39:09.000000 nagios_historian-0.6.7/
-drwxrwxr-x   0 v759329   (1005) v759329   (1005)        0 2019-10-01 19:39:09.000000 nagios_historian-0.6.7/nagios_historian.egg-info/
--rw-rw-r--   0 v759329   (1005) v759329   (1005)        1 2019-10-01 19:39:09.000000 nagios_historian-0.6.7/nagios_historian.egg-info/dependency_links.txt
--rw-rw-r--   0 v759329   (1005) v759329   (1005)      485 2019-10-01 19:39:09.000000 nagios_historian-0.6.7/nagios_historian.egg-info/SOURCES.txt
--rw-rw-r--   0 v759329   (1005) v759329   (1005)       26 2019-10-01 19:39:09.000000 nagios_historian-0.6.7/nagios_historian.egg-info/requires.txt
--rw-rw-r--   0 v759329   (1005) v759329   (1005)     3722 2019-10-01 19:39:09.000000 nagios_historian-0.6.7/nagios_historian.egg-info/PKG-INFO
--rw-rw-r--   0 v759329   (1005) v759329   (1005)        1 2019-08-13 15:05:39.000000 nagios_historian-0.6.7/nagios_historian.egg-info/not-zip-safe
--rw-rw-r--   0 v759329   (1005) v759329   (1005)       69 2019-10-01 19:39:09.000000 nagios_historian-0.6.7/nagios_historian.egg-info/entry_points.txt
--rw-rw-r--   0 v759329   (1005) v759329   (1005)       17 2019-10-01 19:39:09.000000 nagios_historian-0.6.7/nagios_historian.egg-info/top_level.txt
--rw-rw-r--   0 v759329   (1005) v759329   (1005)       38 2019-10-01 19:39:09.000000 nagios_historian-0.6.7/setup.cfg
--rw-rw-r--   0 v759329   (1005) v759329   (1005)     2461 2019-08-13 15:17:24.000000 nagios_historian-0.6.7/README.rst
--rw-rw-r--   0 v759329   (1005) v759329   (1005)     3722 2019-10-01 19:39:09.000000 nagios_historian-0.6.7/PKG-INFO
-drwxrwxr-x   0 v759329   (1005) v759329   (1005)        0 2019-10-01 19:39:09.000000 nagios_historian-0.6.7/nagios_historian/
--rw-rw-r--   0 v759329   (1005) v759329   (1005)      156 2019-08-13 15:02:24.000000 nagios_historian-0.6.7/nagios_historian/__init__.py
--rw-rw-r--   0 v759329   (1005) v759329   (1005)     3215 2019-08-13 15:02:24.000000 nagios_historian-0.6.7/nagios_historian/oauth2_token.py
--rw-rw-r--   0 v759329   (1005) v759329   (1005)        6 2019-10-01 19:36:25.000000 nagios_historian-0.6.7/nagios_historian/VERSION
--rw-rw-r--   0 v759329   (1005) v759329   (1005)     8566 2019-10-01 19:07:51.000000 nagios_historian-0.6.7/nagios_historian/historian_check.py
--rw-rw-r--   0 v759329   (1005) v759329   (1005)     6003 2019-10-01 15:36:36.000000 nagios_historian-0.6.7/nagios_historian/__main__.py
--rw-rw-r--   0 v759329   (1005) v759329   (1005)     1998 2019-08-13 15:02:24.000000 nagios_historian-0.6.7/nagios_historian/plugin_check.py
--rw-rw-r--   0 v759329   (1005) v759329   (1005)     3234 2019-09-13 18:18:47.000000 nagios_historian-0.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:18:32.696434 nagios_historian-0.6.8/
+-rw-rw-rw-   0        0        0     1089 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/LICENSE
+-rw-rw-rw-   0        0        0     3099 2024-04-03 19:18:32.696434 nagios_historian-0.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2527 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-03 19:18:32.696434 nagios_historian-0.6.8/nagios_historian/
+-rw-rw-rw-   0        0        0        7 2024-04-03 19:14:19.000000 nagios_historian-0.6.8/nagios_historian/VERSION
+-rw-rw-rw-   0        0        0      163 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/nagios_historian/__init__.py
+-rw-rw-rw-   0        0        0     6139 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/nagios_historian/__main__.py
+-rw-rw-rw-   0        0        0     4832 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/nagios_historian/historian_check.py
+-rw-rw-rw-   0        0        0     3288 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/nagios_historian/oauth2_token.py
+-rw-rw-rw-   0        0        0     2055 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/nagios_historian/plugin_check.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:18:32.696434 nagios_historian-0.6.8/nagios_historian.egg-info/
+-rw-rw-rw-   0        0        0     3099 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 19:18:32.696434 nagios_historian-0.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     3328 2024-04-03 19:18:30.000000 nagios_historian-0.6.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nagios_historian-0.6.7/nagios_historian.egg-info/PKG-INFO` & `nagios_historian-0.6.8/nagios_historian.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-Metadata-Version: 1.1
-Name: nagios-historian
-Version: 0.6.7
-Summary: nagios historian plugin
-Home-page: https://github.com/matiasgrana/nagios_historian
-Author: Matias Graña
-Author-email: maicolmatiasg@gmail.com
-License: MIT
-Description: Title1
-        ======
-        
-        Checks historian tags and samples.
-        
-        `VERSION  <nagios_historian/VERSION>`__
-        
-        Install
-        =======
-        
-        Linux::
-        
-            sudo pip3 install nagios_historian --upgrade
-        
-        Also is possible to use::
-        
-            sudo python3 -m pip install nagios_historian --upgrade
-        
-        On windows with python3.5::
-        
-            pip install nagios_historian --upgrade
-        
-        For proxies add::
-        
-            --proxy='http://user:passw@server:port'
-        
-        Usage
-        =====
-        
-        Use the command line::
-        
-            > nagios_historian --help
-              usage: nagios_historian [-h] [-u [URL]] [-e [EXTRA_ARGS]]
-        
-                optional arguments:
-                -h, --help            show this help message and exit
-                -u [URL], --url [URL]
-                                      url to check 
-        		--client_id
-                                      oauth2 client_id example client id: user01
-        		--client_secret
-                                      oauth2 client_secret client password
-        		--auth_url
-                                      oauth2 auth_url example: https://login.microsoftonline.com/company.onmicrosoft.com/oauth2/v2.0/token
-        		--instance
-                                      instance name of historian
-        		--oauth2
-                                      Flag to use or not token for oauth2 before creating the request, used to check published services that uses azure oauth2
-                -e [EXTRA_ARGS], --extra_args [EXTRA_ARGS]
-                                      extra args
-        
-        
-        Example usage
-        =============
-        
-        Example use:
-        
-            > nagios_historian -u "https://xxx/yyy/currentvalue?tagNames=" --client_id "admin1234" --client_secret "pass1234" --auth_url "https://xxxx/oauth/token" --oauth2 --instance "instancename"
-        
-        
-        Nagios config
-        =============
-        
-        Example command::
-        
-            define command{
-                command_name  check_nagios_historian
-                command_line  /usr/local/bin/nagios_historian -u "$ARG1$" --client_id "$ARG2$" --client_secret "$ARG3$" --auth_url "$ARG4$" --oauth2 --instance "$ARG5$" --extra_args='$ARG6$'
-            }
-        
-        Example service::
-        
-            define service {
-                    host_name                       SERVERX
-                    service_description             service_name
-                    check_command                   check_nagios_historian!http://url/path!admin123!pass1234!http://authurl/oauth2!instancename
-                    use				                generic-service
-                    notes                           some useful notes
-            }
-        
-        You can use ansible role that already has the installation and command: https://github.com/CoffeeITWorks/ansible_nagios4_server_plugins
-        
-        TODO
-        ====
-        
-        * Use hash passwords
-        * Add Unit tests?
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: System :: Monitoring
+Metadata-Version: 2.1
+Name: nagios-historian
+Version: 0.6.8
+Summary: nagios historian plugin
+Home-page: https://github.com/matiasgrana/nagios_historian
+Author: Matias Graña
+Author-email: maicolmatiasg@gmail.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: System :: Monitoring
+License-File: LICENSE
+
+Title1
+======
+
+Checks historian tags and samples.
+
+`VERSION  <nagios_historian/VERSION>`__
+
+Install
+=======
+
+Linux::
+
+    sudo pip3 install nagios_historian --upgrade
+
+Also is possible to use::
+
+    sudo python3 -m pip install nagios_historian --upgrade
+
+On windows with python3.5::
+
+    pip install nagios_historian --upgrade
+
+For proxies add::
+
+    --proxy='http://user:passw@server:port'
+
+Usage
+=====
+
+Use the command line::
+
+    > nagios_historian --help
+      usage: nagios_historian [-h] [-u [URL]] [-e [EXTRA_ARGS]]
+
+        optional arguments:
+        -h, --help            show this help message and exit
+        -u [URL], --url [URL]
+                              url to check 
+		--client_id
+                              oauth2 client_id example client id: user01
+		--client_secret
+                              oauth2 client_secret client password
+		--auth_url
+                              oauth2 auth_url example: https://login.microsoftonline.com/company.onmicrosoft.com/oauth2/v2.0/token
+		--tags
+                              tags names of historian
+		--oauth2
+                              Flag to use or not token for oauth2 before creating the request, used to check published services that uses azure oauth2
+        -e [EXTRA_ARGS], --extra_args [EXTRA_ARGS]
+                              extra args
+
+
+Example usage
+=============
+
+Example use:
+
+    > nagios_historian -u "https://xxx/yyy/currentvalue?tagNames=" --client_id "admin1234" --client_secret "pass1234" --auth_url "https://xxxx/oauth/token" --oauth2 --tags "TAG1;TAG2;TAG3"
+
+
+Nagios config
+=============
+
+Example command::
+
+    define command{
+        command_name  check_nagios_historian
+        command_line  /usr/local/bin/nagios_historian -u "$ARG1$" --client_id "$ARG2$" --client_secret "$ARG3$" --auth_url "$ARG4$" --oauth2 --tags "$ARG5$" --extra_args='$ARG6$'
+    }
+
+Example service::
+
+    define service {
+            host_name                       SERVERX
+            service_description             service_name
+            check_command                   check_nagios_historian!http://url/path!admin123!pass1234!http://authurl/oauth2!Tags
+            use				                generic-service
+            notes                           some useful notes
+    }
+
+You can use ansible role that already has the installation and command: https://github.com/CoffeeITWorks/ansible_nagios4_server_plugins
+
+TODO
+====
+
+* Use hash passwords
+* Add Unit tests?
```

### Comparing `nagios_historian-0.6.7/README.rst` & `nagios_historian-0.6.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,103 @@
-Title1
-======
-
-Checks historian tags and samples.
-
-`VERSION  <nagios_historian/VERSION>`__
-
-Install
-=======
-
-Linux::
-
-    sudo pip3 install nagios_historian --upgrade
-
-Also is possible to use::
-
-    sudo python3 -m pip install nagios_historian --upgrade
-
-On windows with python3.5::
-
-    pip install nagios_historian --upgrade
-
-For proxies add::
-
-    --proxy='http://user:passw@server:port'
-
-Usage
-=====
-
-Use the command line::
-
-    > nagios_historian --help
-      usage: nagios_historian [-h] [-u [URL]] [-e [EXTRA_ARGS]]
-
-        optional arguments:
-        -h, --help            show this help message and exit
-        -u [URL], --url [URL]
-                              url to check 
-		--client_id
-                              oauth2 client_id example client id: user01
-		--client_secret
-                              oauth2 client_secret client password
-		--auth_url
-                              oauth2 auth_url example: https://login.microsoftonline.com/company.onmicrosoft.com/oauth2/v2.0/token
-		--instance
-                              instance name of historian
-		--oauth2
-                              Flag to use or not token for oauth2 before creating the request, used to check published services that uses azure oauth2
-        -e [EXTRA_ARGS], --extra_args [EXTRA_ARGS]
-                              extra args
-
-
-Example usage
-=============
-
-Example use:
-
-    > nagios_historian -u "https://xxx/yyy/currentvalue?tagNames=" --client_id "admin1234" --client_secret "pass1234" --auth_url "https://xxxx/oauth/token" --oauth2 --instance "instancename"
-
-
-Nagios config
-=============
-
-Example command::
-
-    define command{
-        command_name  check_nagios_historian
-        command_line  /usr/local/bin/nagios_historian -u "$ARG1$" --client_id "$ARG2$" --client_secret "$ARG3$" --auth_url "$ARG4$" --oauth2 --instance "$ARG5$" --extra_args='$ARG6$'
-    }
-
-Example service::
-
-    define service {
-            host_name                       SERVERX
-            service_description             service_name
-            check_command                   check_nagios_historian!http://url/path!admin123!pass1234!http://authurl/oauth2!instancename
-            use				                generic-service
-            notes                           some useful notes
-    }
-
-You can use ansible role that already has the installation and command: https://github.com/CoffeeITWorks/ansible_nagios4_server_plugins
-
-TODO
-====
-
-* Use hash passwords
-* Add Unit tests?
+Metadata-Version: 2.1
+Name: nagios_historian
+Version: 0.6.8
+Summary: nagios historian plugin
+Home-page: https://github.com/matiasgrana/nagios_historian
+Author: Matias Graña
+Author-email: maicolmatiasg@gmail.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: System :: Monitoring
+License-File: LICENSE
+
+Title1
+======
+
+Checks historian tags and samples.
+
+`VERSION  <nagios_historian/VERSION>`__
+
+Install
+=======
+
+Linux::
+
+    sudo pip3 install nagios_historian --upgrade
+
+Also is possible to use::
+
+    sudo python3 -m pip install nagios_historian --upgrade
+
+On windows with python3.5::
+
+    pip install nagios_historian --upgrade
+
+For proxies add::
+
+    --proxy='http://user:passw@server:port'
+
+Usage
+=====
+
+Use the command line::
+
+    > nagios_historian --help
+      usage: nagios_historian [-h] [-u [URL]] [-e [EXTRA_ARGS]]
+
+        optional arguments:
+        -h, --help            show this help message and exit
+        -u [URL], --url [URL]
+                              url to check 
+		--client_id
+                              oauth2 client_id example client id: user01
+		--client_secret
+                              oauth2 client_secret client password
+		--auth_url
+                              oauth2 auth_url example: https://login.microsoftonline.com/company.onmicrosoft.com/oauth2/v2.0/token
+		--tags
+                              tags names of historian
+		--oauth2
+                              Flag to use or not token for oauth2 before creating the request, used to check published services that uses azure oauth2
+        -e [EXTRA_ARGS], --extra_args [EXTRA_ARGS]
+                              extra args
+
+
+Example usage
+=============
+
+Example use:
+
+    > nagios_historian -u "https://xxx/yyy/currentvalue?tagNames=" --client_id "admin1234" --client_secret "pass1234" --auth_url "https://xxxx/oauth/token" --oauth2 --tags "TAG1;TAG2;TAG3"
+
+
+Nagios config
+=============
+
+Example command::
+
+    define command{
+        command_name  check_nagios_historian
+        command_line  /usr/local/bin/nagios_historian -u "$ARG1$" --client_id "$ARG2$" --client_secret "$ARG3$" --auth_url "$ARG4$" --oauth2 --tags "$ARG5$" --extra_args='$ARG6$'
+    }
+
+Example service::
+
+    define service {
+            host_name                       SERVERX
+            service_description             service_name
+            check_command                   check_nagios_historian!http://url/path!admin123!pass1234!http://authurl/oauth2!Tags
+            use				                generic-service
+            notes                           some useful notes
+    }
+
+You can use ansible role that already has the installation and command: https://github.com/CoffeeITWorks/ansible_nagios4_server_plugins
+
+TODO
+====
+
+* Use hash passwords
+* Add Unit tests?
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nagios_historian-0.6.7/nagios_historian/oauth2_token.py` & `nagios_historian-0.6.8/nagios_historian/oauth2_token.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-#
-# documentation:
-# https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow
-import requests
-import json
-
-# Will support with access token
-
-class GetOauth2Token:
-    def __init__(self, client_id, client_secret, auth_url,
-                 grant_type = 'client_credentials'):
-        """
-        reference: https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#request-an-access-token
-        The Authority configured on the client MUST match the one configured on the server. 
-        The Scope configured on the client MUST match the one configured on the server, followed by the .default suffix. 
-        The Client Id is the ApplicationId of the client application configured on the Microsoft Application Registration Portal. 
-        The Client Key is the Password generated on the client. 
-
-        param client_id: example client id: 6731de76-14a6-49ae-97bc-6eba6914391e
-        param scope: example: https://company.onmicrosoft.com/some-unique-number-for-scope/.default
-        param client_secret: "client password secret here"
-        param grant_type: default is "client_credentials"
-        param auth_url: use the correct one for your organization and application server, default example
-                        https://login.microsoftonline.com/company.onmicrosoft.com/oauth2/v2.0/token
-        """
-        self.client_id = client_id
-        self.client_secret = client_secret
-        self.grant_type = grant_type
-        self.auth_url = auth_url
-    
-    def get_token(self):
-        """
-
-        return: tuple dict with access_token, status_code
-            {'access_token': 'tokenid'
-            'expires_in': 3600,
-            'ext_expires_in': 0,
-            'token_type': 'Bearer'}, 200
-        """
-        # Request access token:
-        # https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#request-an-access-token
-
-        headers = {'Content-Type': 'application/x-www-form-urlencoded'}
-        url = self.auth_url
-        data = { "client_id": self.client_id,
-                "client_secret": self.client_secret,
-                "grant_type": self.grant_type
-            }
-
-        # requests doc http://docs.python-requests.org/en/v0.10.7/user/quickstart/#custom-headers
-        r = requests.post(url=url, data=data, headers=headers, verify=False)
-
-        return r.json(), r.status_code
-
-    def url_check(self, url_check):
-        """
-        Just example howto proceed with the token got
-
-        param url_check: url to check with authenticated token
-
-        """
-        # Use the access token:
-        # https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-access-token
-        
-        get_token = self.get_token()
-        access_token = get_token[0]['access_token']
-        header_token = {"Authorization": "Bearer {}".format(access_token)}
-        rt = requests.get(url=url_check, headers=header_token)
-
-        return rt.json(), rt.status_code
-
-# Refresh? will need to check if we are going to do it (don't think so)
-# https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token
+#
+# documentation:
+# https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow
+import requests
+import json
+
+# Will support with access token
+
+class GetOauth2Token:
+    def __init__(self, client_id, client_secret, auth_url,
+                 grant_type = 'client_credentials'):
+        """
+        reference: https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#request-an-access-token
+        The Authority configured on the client MUST match the one configured on the server. 
+        The Scope configured on the client MUST match the one configured on the server, followed by the .default suffix. 
+        The Client Id is the ApplicationId of the client application configured on the Microsoft Application Registration Portal. 
+        The Client Key is the Password generated on the client. 
+
+        param client_id: example client id: 6731de76-14a6-49ae-97bc-6eba6914391e
+        param scope: example: https://company.onmicrosoft.com/some-unique-number-for-scope/.default
+        param client_secret: "client password secret here"
+        param grant_type: default is "client_credentials"
+        param auth_url: use the correct one for your organization and application server, default example
+                        https://login.microsoftonline.com/company.onmicrosoft.com/oauth2/v2.0/token
+        """
+        self.client_id = client_id
+        self.client_secret = client_secret
+        self.grant_type = grant_type
+        self.auth_url = auth_url
+    
+    def get_token(self):
+        """
+
+        return: tuple dict with access_token, status_code
+            {'access_token': 'tokenid'
+            'expires_in': 3600,
+            'ext_expires_in': 0,
+            'token_type': 'Bearer'}, 200
+        """
+        # Request access token:
+        # https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#request-an-access-token
+
+        headers = {'Content-Type': 'application/x-www-form-urlencoded'}
+        url = self.auth_url
+        data = { "client_id": self.client_id,
+                "client_secret": self.client_secret,
+                "grant_type": self.grant_type
+            }
+
+        # requests doc http://docs.python-requests.org/en/v0.10.7/user/quickstart/#custom-headers
+        r = requests.post(url=url, data=data, headers=headers, verify=False)
+
+        return r.json(), r.status_code
+
+    def url_check(self, url_check):
+        """
+        Just example howto proceed with the token got
+
+        param url_check: url to check with authenticated token
+
+        """
+        # Use the access token:
+        # https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-access-token
+        
+        get_token = self.get_token()
+        access_token = get_token[0]['access_token']
+        header_token = {"Authorization": "Bearer {}".format(access_token)}
+        rt = requests.get(url=url_check, headers=header_token)
+
+        return rt.json(), rt.status_code
+
+# Refresh? will need to check if we are going to do it (don't think so)
+# https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token
```

### Comparing `nagios_historian-0.6.7/nagios_historian/__main__.py` & `nagios_historian-0.6.8/nagios_historian/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-#!python3
-# https://nagios-plugins.org/doc/guidelines.html
-
-# Import required libs
-from .plugin_check import curlCheck
-from .oauth2_token import GetOauth2Token 
-from .historian_check import HistorianChecks
-import argparse
-import sys
-
-
-# Return codes expected by Nagios
-OK = 0
-WARNING = 1
-CRITICAL = 2
-UNKNOWN = 3
-
-# Return message
-message = {
-    'status': OK,
-    'summary': 'Example summary',
-    'perfdata': 'label1=0;;;; '  # 'label'=value[UOM];[warn];[crit];[min];[max] 
-}
-
-# For multiple perdata, ensure to add space after each perfdata
-# message['perfdata'] = 'label1=x;;;; '
-# message['perfdata'] += 'label2=x;;;; '
-
-# Function to parse arguments
-def parse_args(args):
-    """
-    Information extracted from: https://mkaz.com/2014/07/26/python-argparse-cookbook/
-     https://docs.python.org/3/library/argparse.html
-    :return: parse.parse_args(args) object
-    You can use obj.option, example:
-    options = parse_args(args)
-    options.user # to read username
-    """
-    parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter, 
-                                     description='nagios plugin to check some url using curl and some other code')
-
-    parser.add_argument('-u', '--url', dest='url', nargs='?', default=None, const=None,
-                        help='url to check \n')
-    parser.add_argument('-e', '--extra_args', dest='extra_args', nargs='?', default='', const=None,
-                            help='extra args to add to curl, see curl manpage  \n')
-    
-    # Arguments to check using OAuth2
-    parser.add_argument('--client_id', dest='client_id', nargs='?', default=None, const=None,
-                            help='oauth2 client_id example client id: user01 \n')
-    parser.add_argument('--client_secret', dest='client_secret', nargs='?', default=None, const=None,
-                            help='oauth2 client_secret client password \n')
-    parser.add_argument('--grant_type', dest='grant_type', nargs='?', default='client_credentials', const=None,
-                            help='oauth2 grant_type \n')
-    parser.add_argument('--auth_url', dest='auth_url', nargs='?', default=None, const=None,
-                            help='oauth2 auth_url example: https://login.microsoftonline.com/company.onmicrosoft.com/oauth2/v2.0/token \n')
-    parser.add_argument('--instance', dest='instance', nargs='?', default=None, const=None,
-                        help='instance name of historian \n')
-    parser.add_argument('--oauth2', action='store_true',
-                            help='''Flag to use or not token for oauth2 before creating the request, used to check published services that uses azure oauth2 \n
-                                    See https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token \n''')
-
-    if not args:
-        raise SystemExit(parser.print_help())
-
-    return parser.parse_args(args)
-
-# Function to execute cli commands
-def cli_execution(options):
-    """
-    : param: options: arguments from parse.parse_args(args) (see parse_args function)
-    """
-    auth_args = ''
-    # Creating access_token to authenticate with azure oauth2
-    if options.oauth2:
-        if not options.client_id:
-            sys.exit('param client_id is required  when using oauth2')
-        if not options.client_secret:
-            sys.exit('param client_secret is required  when using oauth2')
-        if not options.auth_url:
-            sys.exit('param auth_url is required  when using oauth2')
-        
-        #Define oauth object
-        oauth_obj = GetOauth2Token(client_id = options.client_id,                              
-                               client_secret = options.client_secret,
-                               grant_type = options.grant_type,
-                               auth_url = options.auth_url)
-        
-        #Get tuple with http_code and token
-        auth_tuple = oauth_obj.get_token()
-
-        #Vaildate http_code
-        auth_http_code = auth_tuple[1]
-        if auth_http_code != 200:
-            sys.exit('Error getting access_token, http_code != 200, http_code: {}'.format(auth_http_code))
-        
-        #Extract from tuple the token
-        access_token = auth_tuple[0]['access_token']      
-        header_token = {"Authorization": "Bearer {}".format(access_token)}
-        # https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-access-token
-        auth_args = "--header 'Authorization: {}'".format(header_token['Authorization'])
-
-    #Create historian object    
-    historianobj = HistorianChecks(url=options.url,
-                              access_token=access_token,
-                              instance=options.instance)
-
-    def collect_data():        
-        retrcode, msgdata = historianobj.check_tags_data()
-        return retrcode, msgdata
-    
-    def check(retrcode):
-        if retrcode >= 2:
-            status = CRITICAL
-            message['summary'] = 'CRITICAL: '            
-        elif retrcode == 1:
-            status = WARNING
-            message['summary'] = 'WARNING: '
-        else:
-            status = OK
-            message['summary'] = 'OK: '
-        return status
-        
-   
-    # Check logic starts here
-    data = collect_data()
-    message['status'] = check(data[0])
-    # Add summary       
-    message['summary'] += data[1]
-    # Add perfdata
-    # total = len(data)
-    #message['perfdata'] = curlnagiosobj.format_perfdata()    
-    # Print the message
-    # Print the message
-    
-    print("{summary}".format(
-        summary=message.get('summary')
-    ))
-    # Exit with status code
-    raise SystemExit(message['status'])
-
-# Argument parser
-# https://docs.python.org/3.5/library/argparse.html
-
-def main():
-    """
-    Main function
-    """
-    # Get options with argparse
-    options = parse_args(sys.argv[1:])
-    # Execute program functions passing the options collected
-    cli_execution(options)
-
-
-if __name__ == "__main__":
-    main()
+#!python3
+# https://nagios-plugins.org/doc/guidelines.html
+
+# Import required libs
+from .plugin_check import curlCheck
+from .oauth2_token import GetOauth2Token 
+from .historian_check import HistorianChecks
+import argparse
+import sys
+
+
+# Return codes expected by Nagios
+OK = 0
+WARNING = 1
+CRITICAL = 2
+UNKNOWN = 3
+
+# Return message
+message = {
+    'status': OK,
+    'summary': 'Example summary',
+    'perfdata': 'label1=0;;;; '  # 'label'=value[UOM];[warn];[crit];[min];[max] 
+}
+
+# For multiple perdata, ensure to add space after each perfdata
+# message['perfdata'] = 'label1=x;;;; '
+# message['perfdata'] += 'label2=x;;;; '
+
+# Function to parse arguments
+def parse_args(args):
+    """
+    Information extracted from: https://mkaz.com/2014/07/26/python-argparse-cookbook/
+     https://docs.python.org/3/library/argparse.html
+    :return: parse.parse_args(args) object
+    You can use obj.option, example:
+    options = parse_args(args)
+    options.user # to read username
+    """
+    parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter, 
+                                     description='nagios plugin to check some url using curl and some other code')
+
+    parser.add_argument('-u', '--url', dest='url', nargs='?', default=None, const=None,
+                        help='url to check \n')
+    parser.add_argument('-e', '--extra_args', dest='extra_args', nargs='?', default='', const=None,
+                            help='extra args to add to curl, see curl manpage  \n')
+    
+    # Arguments to check using OAuth2
+    parser.add_argument('--client_id', dest='client_id', nargs='?', default=None, const=None,
+                            help='oauth2 client_id example client id: user01 \n')
+    parser.add_argument('--client_secret', dest='client_secret', nargs='?', default=None, const=None,
+                            help='oauth2 client_secret client password \n')
+    parser.add_argument('--grant_type', dest='grant_type', nargs='?', default='client_credentials', const=None,
+                            help='oauth2 grant_type \n')
+    parser.add_argument('--auth_url', dest='auth_url', nargs='?', default=None, const=None,
+                            help='oauth2 auth_url example: https://login.microsoftonline.com/company.onmicrosoft.com/oauth2/v2.0/token \n')
+    parser.add_argument('--tags', dest='tags', nargs='?', default=None, const=None,
+                        help='tags names of historian \n')
+    parser.add_argument('--oauth2', action='store_true',
+                            help='''Flag to use or not token for oauth2 before creating the request, used to check published services that uses azure oauth2 \n
+                                    See https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token \n''')
+
+    if not args:
+        raise SystemExit(parser.print_help())
+
+    return parser.parse_args(args)
+
+# Function to execute cli commands
+def cli_execution(options):
+    """
+    : param: options: arguments from parse.parse_args(args) (see parse_args function)
+    """
+    auth_args = ''
+    # Creating access_token to authenticate with azure oauth2
+    if options.oauth2:
+        if not options.client_id:
+            sys.exit('param client_id is required  when using oauth2')
+        if not options.client_secret:
+            sys.exit('param client_secret is required  when using oauth2')
+        if not options.auth_url:
+            sys.exit('param auth_url is required  when using oauth2')
+        
+        #Define oauth object
+        oauth_obj = GetOauth2Token(client_id = options.client_id,                              
+                               client_secret = options.client_secret,
+                               grant_type = options.grant_type,
+                               auth_url = options.auth_url)
+        
+        #Get tuple with http_code and token
+        auth_tuple = oauth_obj.get_token()
+
+        #Vaildate http_code
+        auth_http_code = auth_tuple[1]
+        if auth_http_code != 200:
+            sys.exit('Error getting access_token, http_code != 200, http_code: {}'.format(auth_http_code))
+        
+        #Extract from tuple the token
+        access_token = auth_tuple[0]['access_token']      
+        header_token = {"Authorization": "Bearer {}".format(access_token)}
+        # https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-access-token
+        auth_args = "--header 'Authorization: {}'".format(header_token['Authorization'])
+
+    #Create historian object    
+    historianobj = HistorianChecks(url=options.url,
+                              access_token=access_token,
+                              tags=options.tags)
+
+    def collect_data():        
+        retrcode, msgdata = historianobj.check_tags_data()
+        return retrcode, msgdata
+    
+    def check(retrcode):
+        if retrcode >= 2:
+            status = CRITICAL
+            message['summary'] = 'CRITICAL: '            
+        elif retrcode == 1:
+            status = WARNING
+            message['summary'] = 'WARNING: '
+        else:
+            status = OK
+            message['summary'] = 'OK: '
+        return status
+        
+   
+    # Check logic starts here
+    data = collect_data()
+    message['status'] = check(data[0])
+    # Add summary       
+    message['summary'] += data[1]
+    # Add perfdata
+    # total = len(data)
+    #message['perfdata'] = curlnagiosobj.format_perfdata()    
+    # Print the message
+    # Print the message
+    
+    print("{summary}".format(
+        summary=message.get('summary')
+    ))
+    # Exit with status code
+    raise SystemExit(message['status'])
+
+# Argument parser
+# https://docs.python.org/3.5/library/argparse.html
+
+def main():
+    """
+    Main function
+    """
+    # Get options with argparse
+    options = parse_args(sys.argv[1:])
+    # Execute program functions passing the options collected
+    cli_execution(options)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `nagios_historian-0.6.7/nagios_historian/plugin_check.py` & `nagios_historian-0.6.8/nagios_historian/plugin_check.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-# plugin_check.py file with classes or functions to collect data or format messages
-# This is just an example class from healthMonitor
-import json
-import subprocess
-
-class curlCheck:
-    def __init__(self, URL, extra_args='', auth_args=''):
-        """
-        :param URL: provide url to get/put data.
-        :param extra_args: any argument for curl command
-        :param auth_args: normally used internally by the code to add HEADERS with authentication args.
-        """
-        self.url = URL
-        self.extra_args = extra_args
-        self.auth_args = auth_args
-        
-        self.std_args = '''" {\\"response_code\\": \\"%{http_code}\\",
-        \\"dns_time\\": \\"%{time_namelookup}\\",
-        \\"connect_time\\": \\"%{time_connect}\\",
-        \\"pretransfer_time\\": \\"%{time_pretransfer}\\",
-        \\"starttransfer_time\\": \\"%{time_starttransfer}\\",
-        \\"total_time\\": \\"%{time_total}\\"
-        "} '''
-
-    def collect_data(self):
-        """
-
-        return: tuple
-        returncode, return output, dict output with info ex:
-        {'pretransfer_time': '0.000', 
-        'response_code': '200', 
-        'starttransfer_time': '0.182', 
-        'dns_time': '0.000', 
-        'connect_time': '0.000', 
-        'total_time': '0.249'}
-        """
-        ### some code here
-        ### or calling external modules
-        cmdline = "curl {} -k --fail -s -o /dev/null {} -w \\ {}  {}".format(self.url, self.extra_args, self.std_args, self.auth_args)
-
-        retrcode, retroutput = subprocess.getstatusoutput(cmdline)  
-
-        jsonoutput = json.loads(retroutput)
-
-        return retrcode, retroutput, jsonoutput
-    
-    def format_perfdata(self):
-
-        perfdata = ''
-        returntuple = self.collect_data()
-
-        for k, v in returntuple[2].items():
-            # Simple format once we implement  warn;crit;min;max
-            # 'label'=value[UOM];[warn];[crit];[min];[max] 
-            perfdata += '{}={};;;; '.format(k, v)
-        
-        return perfdata
+# plugin_check.py file with classes or functions to collect data or format messages
+# This is just an example class from healthMonitor
+import json
+import subprocess
+
+class curlCheck:
+    def __init__(self, URL, extra_args='', auth_args=''):
+        """
+        :param URL: provide url to get/put data.
+        :param extra_args: any argument for curl command
+        :param auth_args: normally used internally by the code to add HEADERS with authentication args.
+        """
+        self.url = URL
+        self.extra_args = extra_args
+        self.auth_args = auth_args
+        
+        self.std_args = '''" {\\"response_code\\": \\"%{http_code}\\",
+        \\"dns_time\\": \\"%{time_namelookup}\\",
+        \\"connect_time\\": \\"%{time_connect}\\",
+        \\"pretransfer_time\\": \\"%{time_pretransfer}\\",
+        \\"starttransfer_time\\": \\"%{time_starttransfer}\\",
+        \\"total_time\\": \\"%{time_total}\\"
+        "} '''
+
+    def collect_data(self):
+        """
+
+        return: tuple
+        returncode, return output, dict output with info ex:
+        {'pretransfer_time': '0.000', 
+        'response_code': '200', 
+        'starttransfer_time': '0.182', 
+        'dns_time': '0.000', 
+        'connect_time': '0.000', 
+        'total_time': '0.249'}
+        """
+        ### some code here
+        ### or calling external modules
+        cmdline = "curl {} -k --fail -s -o /dev/null {} -w \\ {}  {}".format(self.url, self.extra_args, self.std_args, self.auth_args)
+
+        retrcode, retroutput = subprocess.getstatusoutput(cmdline)  
+
+        jsonoutput = json.loads(retroutput)
+
+        return retrcode, retroutput, jsonoutput
+    
+    def format_perfdata(self):
+
+        perfdata = ''
+        returntuple = self.collect_data()
+
+        for k, v in returntuple[2].items():
+            # Simple format once we implement  warn;crit;min;max
+            # 'label'=value[UOM];[warn];[crit];[min];[max] 
+            perfdata += '{}={};;;; '.format(k, v)
+        
+        return perfdata
```

### Comparing `nagios_historian-0.6.7/setup.py` & `nagios_historian-0.6.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-# http://python-packaging.readthedocs.io/en/latest/minimal.html
-# Help from: http://www.scotttorborg.com/python-packaging/minimal.html
-# https://pypi.python.org/pypi?%3Aaction=list_classifiers
-import os
-from os import path
-from setuptools import setup, find_packages
-import rstcheck
-
-
-mypackage_root_dir = 'nagios_historian'
-
-# function to check a readme file
-def check_readme(file='README.rst'):
-    """
-    Checks readme rst file, to ensure it will upload to pypi and be formatted
-    correctly.
-    :param file:
-    :return:
-    """
-    # Get the long description from the relevant file
-    with open(file, encoding='utf-8') as f_object:
-        readme_content = f_object.read()
-
-    errors = list(rstcheck.check(readme_content))
-    if errors:
-        msg = 'There_path are errors in {}, errors \n {}'.format(file,
-                                                            errors[0].message)
-        raise SystemExit(msg)
-    else:
-        msg = 'No errors in {}'.format(file)
-        print(msg)
-
-# Get requirements for this package
-here_path = path.abspath(path.dirname(__file__))
-with open(os.path.join(here_path, 'requirements.txt')) as f:
-    requires = [x.strip() for x in f if x.strip()]
-
-# Get the version from VERSION file
-with open(os.path.join(mypackage_root_dir, 'VERSION')) as version_file:
-    version = version_file.read().strip()
-
-readme_path = path.join(here_path, 'README.rst')
-# Get the long description from the relevant file
-with open(readme_path, encoding='utf-8') as f:
-    long_description = f.read()
-
-# Check the readme
-# when checking rst file you ensure it will be healthy to publish on pypi.org
-check_readme(readme_path)
-
-# Define setuptools specifications
-setup(name='nagios_historian',
-      version=version,
-      description='nagios historian plugin',
-      long_description=long_description,  # this is the file README.rst
-      classifiers=[
-          'Development Status :: 5 - Production/Stable',
-          'Intended Audience :: System Administrators',
-          'License :: OSI Approved :: MIT License',
-          'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3 :: Only',
-          'Topic :: System :: Monitoring',
-      ],
-      url='https://github.com/matiasgrana/nagios_historian',
-      author='Matias Graña',
-      author_email='maicolmatiasg@gmail.com',
-      license='MIT', # Choose your license
-      # http://setuptools.readthedocs.io/en/latest/setuptools.html#using-find-packages
-      packages=find_packages(),
-      include_package_data=True,
-      # use package_data if you want to include more files in the package
-      #package_data={
-      #    'data': 'src/data/*',  
-      #},
-      data_files=[('VERSION', ['{}/VERSION'.format(mypackage_root_dir)])],
-      entry_points={
-          'console_scripts': [
-              # http://python-packaging.readthedocs.io/en/latest/command-line-scripts.html
-              'nagios_historian = nagios_historian.__main__:main'
-          ]
-      },
-      install_requires=requires, # we have already readed requirements.txt in line 30
-      # Use test_require  to add pytest requirements when using unit tests
-      #tests_require=['pytest',
-      #               'pytest-cov'],
-      zip_safe=False)
+# http://python-packaging.readthedocs.io/en/latest/minimal.html
+# Help from: http://www.scotttorborg.com/python-packaging/minimal.html
+# https://pypi.python.org/pypi?%3Aaction=list_classifiers
+import os
+from os import path
+from setuptools import setup, find_packages
+import rstcheck
+
+
+mypackage_root_dir = 'nagios_historian'
+
+# function to check a readme file
+def check_readme(file='README.rst'):
+    """
+    Checks readme rst file, to ensure it will upload to pypi and be formatted
+    correctly.
+    :param file:
+    :return:
+    """
+    # Get the long description from the relevant file
+    with open(file, encoding='utf-8') as f_object:
+        readme_content = f_object.read()
+
+    #errors = list(rstcheck.check(readme_content))
+    #if errors:
+     #   msg = 'There_path are errors in {}, errors \n {}'.format(file,
+      #                                                      errors[0].message)
+       # raise SystemExit(msg)
+    #else:
+     #   msg = 'No errors in {}'.format(file)
+     #   print(msg)
+
+# Get requirements for this package
+here_path = path.abspath(path.dirname(__file__))
+with open(os.path.join(here_path, 'requirements.txt')) as f:
+    requires = [x.strip() for x in f if x.strip()]
+
+# Get the version from VERSION file
+with open(os.path.join(mypackage_root_dir, 'VERSION')) as version_file:
+    version = version_file.read().strip()
+
+readme_path = path.join(here_path, 'README.rst')
+# Get the long description from the relevant file
+with open(readme_path, encoding='utf-8') as f:
+    long_description = f.read()
+
+# Check the readme
+# when checking rst file you ensure it will be healthy to publish on pypi.org
+check_readme(readme_path)
+
+# Define setuptools specifications
+setup(name='nagios_historian',
+      version=version,
+      description='nagios historian plugin',
+      long_description=long_description,  # this is the file README.rst
+      classifiers=[
+          'Development Status :: 5 - Production/Stable',
+          'Intended Audience :: System Administrators',
+          'License :: OSI Approved :: MIT License',
+          'Programming Language :: Python :: 3',
+          'Programming Language :: Python :: 3 :: Only',
+          'Topic :: System :: Monitoring',
+      ],
+      url='https://github.com/matiasgrana/nagios_historian',
+      author='Matias Graña',
+      author_email='maicolmatiasg@gmail.com',
+      license='MIT', # Choose your license
+      # http://setuptools.readthedocs.io/en/latest/setuptools.html#using-find-packages
+      packages=find_packages(),
+      include_package_data=True,
+      # use package_data if you want to include more files in the package
+      #package_data={
+      #    'data': 'src/data/*',  
+      #},
+      data_files=[('VERSION', ['{}/VERSION'.format(mypackage_root_dir)])],
+      entry_points={
+          'console_scripts': [
+              # http://python-packaging.readthedocs.io/en/latest/command-line-scripts.html
+              'nagios_historian = nagios_historian.__main__:main'
+          ]
+      },
+      install_requires=requires, # we have already readed requirements.txt in line 30
+      # Use test_require  to add pytest requirements when using unit tests
+      #tests_require=['pytest',
+      #               'pytest-cov'],
+      zip_safe=False)
```

