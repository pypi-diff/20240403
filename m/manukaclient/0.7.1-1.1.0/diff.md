# Comparing `tmp/manukaclient-0.7.1.tar.gz` & `tmp/manukaclient-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/manukaclient-0.7.1.tar", last modified: Mon Jul  6 07:51:30 2020, max compression
+gzip compressed data, was "manukaclient-1.1.0.tar", last modified: Wed Apr  3 03:48:37 2024, max compression
```

## Comparing `manukaclient-0.7.1.tar` & `manukaclient-1.1.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:30.000000 manukaclient-0.7.1/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       61 2020-07-06 07:51:30.000000 manukaclient-0.7.1/setup.cfg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1626 2020-07-06 07:51:26.000000 manukaclient-0.7.1/setup.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:30.000000 manukaclient-0.7.1/manukaclient.egg-info/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       46 2020-07-06 07:51:29.000000 manukaclient-0.7.1/manukaclient.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2020-07-06 07:51:29.000000 manukaclient-0.7.1/manukaclient.egg-info/not-zip-safe
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       13 2020-07-06 07:51:29.000000 manukaclient-0.7.1/manukaclient.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      682 2020-07-06 07:51:29.000000 manukaclient-0.7.1/manukaclient.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2020-07-06 07:51:30.000000 manukaclient-0.7.1/manukaclient.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2020-07-06 07:51:29.000000 manukaclient-0.7.1/manukaclient.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      479 2020-07-06 07:51:29.000000 manukaclient-0.7.1/manukaclient.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       46 2020-07-06 07:51:26.000000 manukaclient-0.7.1/requirements.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      130 2020-07-06 07:51:26.000000 manukaclient-0.7.1/MANIFEST.in
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:30.000000 manukaclient-0.7.1/manukaclient/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5582 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/exceptions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1906 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/client.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:30.000000 manukaclient-0.7.1/manukaclient/v1/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2132 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/v1/users.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1240 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/v1/external_ids.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1461 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/v1/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/v1/__init__.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:30.000000 manukaclient-0.7.1/manukaclient/osc/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:30.000000 manukaclient-0.7.1/manukaclient/osc/v1/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5464 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/osc/v1/users.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2827 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/osc/v1/external_ids.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/osc/v1/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/osc/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1472 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/osc/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2263 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/osc/plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14730 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/__init__.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:30.000000 manukaclient-0.7.1/manukaclient/tests/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:30.000000 manukaclient-0.7.1/manukaclient/tests/unit/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:30.000000 manukaclient-0.7.1/manukaclient/tests/unit/v1/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1378 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/tests/unit/v1/test_external_ids.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3390 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/tests/unit/v1/test_users.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14923 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/tests/unit/v1/fakes.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6359 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/tests/unit/fakes.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/tests/unit/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3119 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/tests/unit/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2020-07-06 07:51:26.000000 manukaclient-0.7.1/manukaclient/tests/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      479 2020-07-06 07:51:30.000000 manukaclient-0.7.1/PKG-INFO
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-03 03:48:37.945533 manukaclient-1.1.0/
+-rw-rw-r--   0 sam       (1000) sam       (1000)    10143 2023-10-31 04:52:20.000000 manukaclient-1.1.0/LICENSE
+-rw-rw-r--   0 sam       (1000) sam       (1000)      130 2023-10-31 04:52:20.000000 manukaclient-1.1.0/MANIFEST.in
+-rw-rw-r--   0 sam       (1000) sam       (1000)      440 2024-04-03 03:48:37.945533 manukaclient-1.1.0/PKG-INFO
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-03 03:48:37.941533 manukaclient-1.1.0/manukaclient/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-10-31 04:52:20.000000 manukaclient-1.1.0/manukaclient/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1909 2024-04-03 00:47:27.000000 manukaclient-1.1.0/manukaclient/client.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-03 03:48:37.941533 manukaclient-1.1.0/manukaclient/osc/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-10-31 04:52:20.000000 manukaclient-1.1.0/manukaclient/osc/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2263 2023-10-31 04:52:20.000000 manukaclient-1.1.0/manukaclient/osc/plugin.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-03 03:48:37.945533 manukaclient-1.1.0/manukaclient/osc/v1/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-10-31 04:52:20.000000 manukaclient-1.1.0/manukaclient/osc/v1/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2830 2024-04-03 00:47:27.000000 manukaclient-1.1.0/manukaclient/osc/v1/external_ids.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2367 2023-11-10 00:02:39.000000 manukaclient-1.1.0/manukaclient/osc/v1/terms.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     5468 2024-04-03 02:28:19.000000 manukaclient-1.1.0/manukaclient/osc/v1/users.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-03 03:48:37.945533 manukaclient-1.1.0/manukaclient/tests/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-10-31 04:52:20.000000 manukaclient-1.1.0/manukaclient/tests/__init__.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-03 03:48:37.945533 manukaclient-1.1.0/manukaclient/tests/unit/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-10-31 04:52:20.000000 manukaclient-1.1.0/manukaclient/tests/unit/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     6359 2023-11-10 00:56:17.000000 manukaclient-1.1.0/manukaclient/tests/unit/fakes.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-03 03:48:37.945533 manukaclient-1.1.0/manukaclient/tests/unit/v1/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-10-31 04:52:20.000000 manukaclient-1.1.0/manukaclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)    15682 2024-04-03 00:47:27.000000 manukaclient-1.1.0/manukaclient/tests/unit/v1/fakes.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1382 2024-04-03 00:47:27.000000 manukaclient-1.1.0/manukaclient/tests/unit/v1/test_external_ids.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1074 2024-04-03 00:47:27.000000 manukaclient-1.1.0/manukaclient/tests/unit/v1/test_keystone_ext.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     3436 2024-04-03 00:47:27.000000 manukaclient-1.1.0/manukaclient/tests/unit/v1/test_users.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-03 03:48:37.945533 manukaclient-1.1.0/manukaclient/v1/
+-rw-rw-r--   0 sam       (1000) sam       (1000)        0 2023-10-31 04:52:20.000000 manukaclient-1.1.0/manukaclient/v1/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1598 2024-04-03 00:47:27.000000 manukaclient-1.1.0/manukaclient/v1/client.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1107 2024-04-03 00:47:27.000000 manukaclient-1.1.0/manukaclient/v1/external_ids.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1086 2024-04-03 00:47:27.000000 manukaclient-1.1.0/manukaclient/v1/keystone_ext.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      899 2023-11-10 00:03:16.000000 manukaclient-1.1.0/manukaclient/v1/terms.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     2018 2024-04-03 00:47:27.000000 manukaclient-1.1.0/manukaclient/v1/users.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2024-04-03 03:48:37.941533 manukaclient-1.1.0/manukaclient.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      440 2024-04-03 03:48:37.000000 manukaclient-1.1.0/manukaclient.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1018 2024-04-03 03:48:37.000000 manukaclient-1.1.0/manukaclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2024-04-03 03:48:37.000000 manukaclient-1.1.0/manukaclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)      682 2024-04-03 03:48:37.000000 manukaclient-1.1.0/manukaclient.egg-info/entry_points.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2020-04-23 05:17:12.000000 manukaclient-1.1.0/manukaclient.egg-info/not-zip-safe
+-rw-rw-r--   0 sam       (1000) sam       (1000)       92 2024-04-03 03:48:37.000000 manukaclient-1.1.0/manukaclient.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       13 2024-04-03 03:48:37.000000 manukaclient-1.1.0/manukaclient.egg-info/top_level.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       92 2024-04-03 00:47:27.000000 manukaclient-1.1.0/requirements.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       61 2024-04-03 03:48:37.945533 manukaclient-1.1.0/setup.cfg
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1577 2024-04-03 00:47:27.000000 manukaclient-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `manukaclient-0.7.1/setup.py` & `manukaclient-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,28 +20,27 @@
         'account external-id delete = manukaclient.osc.v1.external_ids:DeleteExternalId',
     ]
 }
 
 
 setuptools.setup(
     name='manukaclient',
-    version='0.7.1',
+    version='1.1.0',
     description=('Client for the Nectar Account system'),
     author='Sam Morrison',
     author_email='sorrison@gmail.com',
     url='https://github.com/NeCTAR-RC/python-manukaclient',
     packages=[
         'manukaclient',
     ],
     include_package_data=True,
     setup_requires=['pbr>=3.0.0'],
     install_requires=parse_requirements(),
     license="Apache",
     zip_safe=False,
     classifiers=(
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ),
     entry_points=entry_points,
 )
```

### Comparing `manukaclient-0.7.1/manukaclient.egg-info/entry_points.txt` & `manukaclient-1.1.0/manukaclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `manukaclient-0.7.1/manukaclient.egg-info/SOURCES.txt` & `manukaclient-1.1.0/manukaclient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
+LICENSE
 MANIFEST.in
 requirements.txt
 setup.cfg
 setup.py
 manukaclient/__init__.py
-manukaclient/base.py
 manukaclient/client.py
-manukaclient/exceptions.py
 manukaclient.egg-info/PKG-INFO
 manukaclient.egg-info/SOURCES.txt
 manukaclient.egg-info/dependency_links.txt
 manukaclient.egg-info/entry_points.txt
 manukaclient.egg-info/not-zip-safe
 manukaclient.egg-info/requires.txt
 manukaclient.egg-info/top_level.txt
 manukaclient/osc/__init__.py
 manukaclient/osc/plugin.py
-manukaclient/osc/utils.py
 manukaclient/osc/v1/__init__.py
 manukaclient/osc/v1/external_ids.py
+manukaclient/osc/v1/terms.py
 manukaclient/osc/v1/users.py
 manukaclient/tests/__init__.py
 manukaclient/tests/unit/__init__.py
 manukaclient/tests/unit/fakes.py
-manukaclient/tests/unit/utils.py
 manukaclient/tests/unit/v1/__init__.py
 manukaclient/tests/unit/v1/fakes.py
 manukaclient/tests/unit/v1/test_external_ids.py
+manukaclient/tests/unit/v1/test_keystone_ext.py
 manukaclient/tests/unit/v1/test_users.py
 manukaclient/v1/__init__.py
 manukaclient/v1/client.py
 manukaclient/v1/external_ids.py
+manukaclient/v1/keystone_ext.py
+manukaclient/v1/terms.py
 manukaclient/v1/users.py
```

### Comparing `manukaclient-0.7.1/manukaclient/client.py` & `manukaclient-1.1.0/manukaclient/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 #
 from keystoneauth1 import adapter
+from nectarclient_lib import exceptions
 from oslo_utils import importutils
 
-from manukaclient import exceptions
-
 
 def Client(version, *args, **kwargs):
     module = 'manukaclient.v%s.client' % version
     module = importutils.import_module(module)
     client_class = getattr(module, 'Client')
     return client_class(*args, **kwargs)
```

### Comparing `manukaclient-0.7.1/manukaclient/v1/users.py` & `manukaclient-1.1.0/manukaclient/v1/users.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 #
 
-import json
+from nectarclient_lib import base
 
-from manukaclient import base
 from manukaclient.v1 import external_ids
 
 
 class User(base.Resource):
 
     date_fields = ['registered_at', 'terms_accepted_at', 'last_login']
 
@@ -34,17 +33,15 @@
 
 class UserManager(base.BasicManager):
 
     base_url = 'v1/users'
     resource_class = User
 
     def update(self, user_id, **kwargs):
-        data = json.dumps(kwargs)
-        return self._update('/%s/%s/' % (self.base_url, user_id), data=data,
-                            headers={"content-type": "application/json"})
+        return self._update('/%s/%s/' % (self.base_url, user_id), data=kwargs)
 
     def refresh_orcid(self, user_id):
         return self._post('/%s/%s/refresh-orcid/' % (self.base_url, user_id),
                           data={})
 
     def projects(self, user_id, role_name):
         return self._get('/%s/%s/projects/%s/' %
```

### Comparing `manukaclient-0.7.1/manukaclient/v1/external_ids.py` & `manukaclient-1.1.0/manukaclient/tests/unit/v1/test_external_ids.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,33 +7,33 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 #
 
+import datetime
 import json
 
-from manukaclient import base
+from nectarclient_lib.tests.unit import utils
 
+from manukaclient.tests.unit.v1 import fakes
+from manukaclient.v1 import external_ids
 
-class ExternalId(base.Resource):
 
-    date_fields = ['last_login']
+class ExternalIdsTest(utils.TestCase):
 
-    def __repr__(self):
-        return "<ExternalId %s>" % self.attributes.get('id')
+    def setUp(self):
+        super(ExternalIdsTest, self).setUp()
+        self.cs = fakes.FakeClient()
 
+    def test_update(self):
+        new_user_id = '234'
+        e = self.cs.external_ids.update(123, user_id=new_user_id)
+        self.cs.assert_called('PATCH', '/v1/external-ids/123/',
+                              json.dumps({'user_id': new_user_id}))
+        self.assertIsInstance(e, external_ids.ExternalId)
+        self.assertIsInstance(e.last_login, datetime.datetime)
 
-class ExternalIdManager(base.Manager):
-
-    base_url = 'v1/external-ids'
-    resource_class = ExternalId
-
-    def update(self, external_id, **kwargs):
-        data = json.dumps(kwargs)
-        return self._update('/%s/%s/' % (self.base_url, external_id),
-                            data=data,
-                            headers={"content-type": "application/json"})
-
-    def delete(self, external_id):
-        return self._delete('/%s/%s/' % (self.base_url, external_id))
+    def test_delete(self):
+        self.cs.external_ids.delete(123)
+        self.cs.assert_called('DELETE', '/v1/external-ids/123/')
```

### Comparing `manukaclient-0.7.1/manukaclient/v1/client.py` & `manukaclient-1.1.0/manukaclient/v1/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 #
 
+from nectarclient_lib import exceptions
+
 from manukaclient import client
-from manukaclient import exceptions
 from manukaclient.v1 import external_ids
+from manukaclient.v1 import keystone_ext
 from manukaclient.v1 import users
 
 
 class Client(object):
     """Client for the Nectar Allocations v1 API
     :param string session: session
     :type session: :py:class:`keystoneauth.adapter.Adapter`
@@ -27,9 +29,11 @@
         """Initialize a new client for the Manuka v1 API."""
         if session is None:
             raise exceptions.ClientException(
                 message='Session is required argument')
         self.http_client = client.SessionClient(
             session, service_type=service_type, **kwargs)
         self.external_ids = external_ids.ExternalIdManager(self.http_client)
+        self.keystone_ext = keystone_ext.KeystoneExtManager(
+            self.http_client)
         self.pending_users = users.PendingUserManager(self.http_client)
         self.users = users.UserManager(self.http_client)
```

### Comparing `manukaclient-0.7.1/manukaclient/osc/v1/users.py` & `manukaclient-1.1.0/manukaclient/osc/v1/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 #
 
 import logging
 
+from nectarclient_lib import exceptions
 from osc_lib.command import command
 from osc_lib import utils as osc_utils
 
-from manukaclient import exceptions
-
 
 class ListUsers(command.Lister):
     """List users."""
 
     log = logging.getLogger(__name__ + '.ListUsers')
 
     def take_action(self, parsed_args):
@@ -76,14 +75,15 @@
     """Show user details."""
 
     log = logging.getLogger(__name__ + '.ShowUser')
 
     def take_action(self, parsed_args):
         self.log.debug('take_action(%s)', parsed_args)
         client = self.app.client_manager.account
+
         try:
             user = client.users.get(parsed_args.id)
         except exceptions.NotFound as ex:
             raise exceptions.CommandError(str(ex))
 
         return self.dict2columns(user.to_dict())
```

### Comparing `manukaclient-0.7.1/manukaclient/osc/v1/external_ids.py` & `manukaclient-1.1.0/manukaclient/osc/v1/external_ids.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 #
 
 import logging
 
+from nectarclient_lib import exceptions
 from osc_lib.command import command
 
-from manukaclient import exceptions
-
 
 class ExternalIdCommand(command.ShowOne):
 
     def get_parser(self, prog_name):
         parser = super(ExternalIdCommand, self).get_parser(prog_name)
         parser.add_argument(
             'id',
```

### Comparing `manukaclient-0.7.1/manukaclient/osc/plugin.py` & `manukaclient-1.1.0/manukaclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `manukaclient-0.7.1/manukaclient/tests/unit/v1/test_users.py` & `manukaclient-1.1.0/manukaclient/tests/unit/v1/test_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 #   License for the specific language governing permissions and limitations
 #   under the License.
 #
 
 import datetime
 import json
 
-from manukaclient.v1 import users
+from nectarclient_lib.tests.unit import utils
 
-from manukaclient.tests.unit import utils
 from manukaclient.tests.unit.v1 import fakes
+from manukaclient.v1 import users
 
 
 class UsersTest(utils.TestCase):
 
     def setUp(self):
         super(UsersTest, self).setUp()
         self.cs = fakes.FakeClient()
@@ -63,15 +63,16 @@
                               json.dumps({'orcid': new_orcid}))
         self.assertIsInstance(u, users.User)
         self.assertEqual(new_orcid, u.orcid)
 
     def test_search(self):
         query = 'needle'
         ul = self.cs.users.search(query)
-        self.cs.assert_called('POST', '/v1/users/search/', {'search': query})
+        self.cs.assert_called('POST', '/v1/users/search/',
+                              json.dumps({'search': query}))
         for u in ul:
             self.assertIsInstance(u, users.User)
 
 
 class PendingUsersTest(utils.TestCase):
 
     def setUp(self):
```

### Comparing `manukaclient-0.7.1/manukaclient/tests/unit/v1/fakes.py` & `manukaclient-1.1.0/manukaclient/tests/unit/v1/fakes.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import re
+from unittest import mock
+from urllib import parse
 
-import mock
-from six.moves.urllib import parse
+from nectarclient_lib.tests.unit import fakes
+from nectarclient_lib.tests.unit import utils
 
 from manukaclient import client as base_client
-from manukaclient.tests.unit import fakes
-from manukaclient.tests.unit import utils
 from manukaclient.v1 import client
 from manukaclient.v1 import external_ids
+from manukaclient.v1 import keystone_ext
 from manukaclient.v1 import users
 
 
 # regex to compare callback to result of get_endpoint()
 # checks version number (vX or vX.X where X is a number)
 # and also checks if the id is on the end
 ENDPOINT_RE = re.compile(
@@ -51,15 +52,15 @@
     "ignore_username_not_email": False,
     "orcid": "sammmee",
     "state": "created",
     "last_login": "2020-04-23T10:23:20",
     "terms_version": "v1",
     "external_ids": [
         {
-            "id": "1233",
+            "id": 1233,
             "last_login": "2020-04-23T10:23:20",
             "idp": "https://idp/idp/shibboleth",
         }
     ],
 }
 
 
@@ -67,14 +68,15 @@
 
     def __init__(self, *args, **kwargs):
         client.Client.__init__(self, session=mock.Mock())
         self.http_client = FakeSessionClient(**kwargs)
         self.users = users.UserManager(self.http_client)
         self.pending_users = users.PendingUserManager(self.http_client)
         self.external_ids = external_ids.ExternalIdManager(self.http_client)
+        self.keystone_ext = keystone_ext.KeystoneExtManager(self.http_client)
 
 
 class FakeSessionClient(base_client.SessionClient):
 
     def __init__(self, *args, **kwargs):
 
         self.callstack = []
@@ -291,15 +293,15 @@
                 "orcid": "sammmee",
                 "state": "created",
                 "last_login": "2020-04-23T10:23:20",
                 "terms_version": "v1"
             }
         ]
 
-        return (200, data, users)
+        return (200, {}, users)
 
     def get_v1_pending_users(self, **kw):
         users = [
             {
                 "first_name": "uEelNrtNg3SPzh50nol5",
                 "affiliation": "staff",
                 "id": 123,
@@ -365,13 +367,28 @@
     def get_v1_pending_users_123(self, **kw):
         return (200, {}, generic_user)
 
     def delete_v1_external_ids_123(self, **kw):
         return (204, {}, {})
 
     def patch_v1_external_ids_123(self, data, **kw):
-        return (202, {'user_id': '234'},
+        return (202, {},
                 {
-                    "id": "134",
+                    "id": 134,
                     "last_login": "2020-04-23T10:23:20",
                     "idp": "F72fIjesixhkTUSzMxdF"
                 })
+
+    def get_v1_keystone_ext_user_by_name_bob(self, **kw):
+        ks_user = {'email': 'email@example.com',
+                   'full_name': 'displayName-lyWtLuxXWxku24cbhgjT',
+                   'inactive': False,
+                   'id': '123456789',
+                   'name': 'email@example.com',
+                   'domain_id': 'default',
+                   'enabled': True,
+                   'default_project_id': '987654321',
+                   'password_expires_at': None,
+                   'options': {},
+                   'links': {'self': 'http://keystone:5000/v3/users/123456789'}
+                   }
+        return (200, {}, ks_user)
```

### Comparing `manukaclient-0.7.1/manukaclient/tests/unit/fakes.py` & `manukaclient-1.1.0/manukaclient/tests/unit/fakes.py`

 * *Files identical despite different names*

