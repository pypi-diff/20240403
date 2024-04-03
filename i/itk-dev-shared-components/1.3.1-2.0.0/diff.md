# Comparing `tmp/itk_dev_shared_components-1.3.1.tar.gz` & `tmp/itk_dev_shared_components-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itk_dev_shared_components-1.3.1.tar", last modified: Wed Feb 21 14:08:24 2024, max compression
+gzip compressed data, was "itk_dev_shared_components-2.0.0.tar", last modified: Wed Apr  3 07:55:43 2024, max compression
```

## Comparing `itk_dev_shared_components-1.3.1.tar` & `itk_dev_shared_components-2.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:08:24.050435 itk_dev_shared_components-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-02-21 14:08:24.050435 itk_dev_shared_components-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:08:24.046435 itk_dev_shared_components-1.3.1/itk_dev_shared_components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:08:24.046435 itk_dev_shared_components-1.3.1/itk_dev_shared_components/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/graph/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/graph/mail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:08:24.046435 itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/cpr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/nova_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/nova_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/nova_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/nova_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:08:24.046435 itk_dev_shared_components-1.3.1/itk_dev_shared_components/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/misc/cpr_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:08:24.050435 itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/fmcacov.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/gridview_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/multi_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/opret_kundekontakt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/sap_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/sap_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/tree_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:08:24.050435 itk_dev_shared_components-1.3.1/itk_dev_shared_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-02-21 14:08:24.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-02-21 14:08:24.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 14:08:24.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-21 14:08:24.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-21 14:08:24.000000 itk_dev_shared_components-1.3.1/itk_dev_shared_components.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-21 14:08:15.000000 itk_dev_shared_components-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 14:08:24.050435 itk_dev_shared_components-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:55:43.596047 itk_dev_shared_components-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-03 07:55:43.596047 itk_dev_shared_components-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:55:43.588047 itk_dev_shared_components-2.0.0/itk_dev_shared_components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:55:43.592047 itk_dev_shared_components-2.0.0/itk_dev_shared_components/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/graph/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/graph/mail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:55:43.592047 itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/cpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/nova_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/nova_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/nova_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/nova_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:55:43.592047 itk_dev_shared_components-2.0.0/itk_dev_shared_components/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/misc/cpr_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:55:43.592047 itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/fmcacov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/gridview_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/multi_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/opret_kundekontakt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/sap_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/sap_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/tree_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:55:43.592047 itk_dev_shared_components-2.0.0/itk_dev_shared_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-03 07:55:43.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-03 07:55:43.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:55:43.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 07:55:43.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 07:55:43.000000 itk_dev_shared_components-2.0.0/itk_dev_shared_components.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-03 07:55:39.000000 itk_dev_shared_components-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 07:55:43.596047 itk_dev_shared_components-2.0.0/setup.cfg
```

### Comparing `itk_dev_shared_components-1.3.1/LICENSE` & `itk_dev_shared_components-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/PKG-INFO` & `itk_dev_shared_components-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itk_dev_shared_components
-Version: 1.3.1
+Version: 2.0.0
 Summary: Shared components to use in RPA projects
 Author-email: ITK Development <itk-rpa@mkb.aarhus.dk>
 Project-URL: Homepage, https://github.com/itk-dev-rpa/itk-dev-shared-components
 Project-URL: Bug Tracker, https://github.com/itk-dev-rpa/itk-dev-shared-components/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `itk_dev_shared_components-1.3.1/README.md` & `itk_dev_shared_components-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/graph/authentication.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/graph/authentication.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/graph/mail.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/graph/mail.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/authentication.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/authentication.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/cpr.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/cpr.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/nova_cases.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/nova_cases.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import uuid
 import base64
 import urllib.parse
 
 import requests
 
 from itk_dev_shared_components.kmd_nova.authentication import NovaAccess
-from itk_dev_shared_components.kmd_nova.nova_objects import NovaCase, CaseParty, JournalNote
+from itk_dev_shared_components.kmd_nova.nova_objects import NovaCase, CaseParty, JournalNote, Caseworker, Department
 from itk_dev_shared_components.kmd_nova.util import datetime_from_iso_string
 
 
 def get_cases(nova_access: NovaAccess, cpr: str = None, case_number: str = None, case_title: str = None, limit: int = 100) -> list[NovaCase]:
     """Search for cases on different search terms.
     Currently supports search on cpr number, case number and case title. At least one search term must be given.
 
@@ -79,49 +79,119 @@
                 },
                 "proceedingFacet": {
                     "code": True
                 }
             },
             "sensitivity": {
                 "sensitivity": True
-            }
+            },
+            "caseworker": {
+                "kspIdentity": {
+                    "novaUserId": True,
+                    "fullName": True,
+                    "racfId": True
+                }
+            },
+            "responsibleDepartment": {
+                "losIdentity": {
+                    "novaUnitId": True,
+                    "administrativeUnitId": True,
+                    "fullName": True,
+                    "userKey": True
+                }
+            },
+            "securityUnit": {
+                "losIdentity": {
+                    "novaUnitId": True,
+                    "administrativeUnitId": True,
+                    "fullName": True,
+                    "userKey": True
+                }
+            },
         }
     }
 
     headers = {'Content-Type': 'application/json', 'Authorization': f"Bearer {nova_access.get_bearer_token()}"}
 
     response = requests.put(url, params=params, headers=headers, json=payload, timeout=60)
     response.raise_for_status()
 
     if response.json()['pagingInformation']['numberOfRows'] == 0:
         return []
 
     # Convert json to NovaCase objects
     cases = []
     for case_dict in response.json()['cases']:
+        security_unit, responsible_department = _extract_departments(case_dict)
         case = NovaCase(
             uuid = case_dict['common']['uuid'],
             title = case_dict['caseAttributes']['title'],
             case_date = datetime_from_iso_string(case_dict['caseAttributes']['caseDate']),
             case_number = case_dict['caseAttributes']['userFriendlyCaseNumber'],
             active_code = case_dict['state']['activeCode'],
             progress_state = case_dict['state']['progressState'],
             case_parties = _extract_case_parties(case_dict),
             document_count = case_dict['numberOfDocuments'],
             note_count = case_dict['numberOfJournalNotes'],
             kle_number = case_dict['caseClassification']['kleNumber']['code'],
             proceeding_facet = case_dict['caseClassification']['proceedingFacet']['code'],
-            sensitivity = case_dict["sensitivity"]["sensitivity"]
+            sensitivity = case_dict["sensitivity"]["sensitivity"],
+            caseworker = _extract_case_worker(case_dict),
+            security_unit=security_unit,
+            responsible_department=responsible_department
         )
 
         cases.append(case)
 
     return cases
 
 
+def _extract_departments(case_dict: dict) -> tuple[Department, Department]:
+    """Extract the departments from a HTTP request response.
+
+    Args:
+        case_dict: The dictionary describing the case.
+
+    Returns:
+        The security unit and the responsible department.
+    """
+    security_unit = Department(
+        id=case_dict['securityUnit']['losIdentity']['administrativeUnitId'],
+        name=case_dict['securityUnit']['losIdentity']['fullName'],
+        user_key=case_dict['securityUnit']['losIdentity']['userKey']
+    )
+
+    responsible_department = Department(
+        id=case_dict['responsibleDepartment']['losIdentity']['administrativeUnitId'],
+        name=case_dict['responsibleDepartment']['losIdentity']['fullName'],
+        user_key=case_dict['responsibleDepartment']['losIdentity']['userKey']
+    )
+
+    return security_unit, responsible_department
+
+
+def _extract_case_worker(case_dict: dict) -> Caseworker | None:
+    """Extract the case worker from a HTTP request response.
+
+    Args:
+        case_dict: The dictionary describing the case.
+
+    Returns:
+        A case worker object describing the case worker if any.
+    """
+    if 'caseworker' in case_dict:
+        return Caseworker(
+            uuid = case_dict['caseworker']['kspIdentity']['novaUserId'],
+            name = case_dict['caseworker']['kspIdentity']['fullName'],
+            ident = case_dict['caseworker']['kspIdentity']['racfId']
+        )
+
+    return None
+
+
 def _extract_case_parties(case_dict: dict) -> list[CaseParty]:
     """Extract the case parties from a HTTP request response.
 
     Args:
         case_dict: The dictionary describing the case party.
 
     Returns:
@@ -160,15 +230,15 @@
             note = base64.b64decode(note_dict['journalNoteAttributes']['note']),
             approved = note_dict['journalNoteAttributes'].get('approved', False)
         )
         notes.append(note)
     return notes
 
 
-def add_case(case: NovaCase, nova_access: NovaAccess, security_unit_id: int = 818485, security_unit_name: str = "Borgerservice"):
+def add_case(case: NovaCase, nova_access: NovaAccess):
     """Add a case to KMD Nova. The case will be created as 'Active'.
 
     Args:
         case: The case object describing the case.
         nova_access: The NovaAccess object used to authenticate.
         security_unit_id: The id of the security unit that has access to the case. Defaults to 818485.
         security_unit_name: The name of the security unit that has access to the case. Defaults to "Borgerservice".
@@ -204,25 +274,41 @@
                 "identificationType": party.identification_type,
                 "identification": party.identification,
                 "participantRole": party.role
             } for party in case.case_parties
         ],
         "securityUnit": {
             "losIdentity": {
-                "administrativeUnitId": security_unit_id,
-                "fullName": security_unit_name,
+                "administrativeUnitId": case.security_unit.id,
+                "fullName": case.security_unit.name,
+                "userKey": case.security_unit.user_key
+            }
+        },
+        "responsibleDepartment": {
+            "losIdentity": {
+                "administrativeUnitId": case.responsible_department.id,
+                "fullName": case.responsible_department.name,
+                "userKey": case.responsible_department.user_key
             }
         },
         "SensitivityCtrlBy": "Bruger",
         "SecurityUnitCtrlBy": "Regler",
         "ResponsibleDepartmentCtrlBy": "Regler",
         "caseAvailability": {
             "unit": "År",
             "scale": 5
         },
         "AvailabilityCtrlBy": "Regler"
     }
 
+    if case.caseworker:
+        payload['caseworker'] = {
+            "kspIdentity": {
+                "racfId": case.caseworker.ident,
+                "fullName": case.caseworker.name
+            }
+        }
+
     headers = {'Content-Type': 'application/json', 'Authorization': f"Bearer {nova_access.get_bearer_token()}"}
 
     response = requests.post(url, params=params, headers=headers, json=payload, timeout=60)
     response.raise_for_status()
```

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/nova_documents.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/nova_documents.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/nova_objects.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/nova_objects.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,30 @@
 from datetime import datetime
 
 # All classes in this module are pure dataclasses made to contain data.
 # pylint: disable=too-many-instance-attributes
 
 
 @dataclass(slots=True, kw_only=True)
+class Department:
+    """A dataclass representing a department in a KMD Nova case."""
+    id: int
+    name: str
+    user_key: str
+
+
+@dataclass(slots=True, kw_only=True)
+class Caseworker:
+    """A dataclass representing a caseworker in a KMD Nova case."""
+    uuid: str
+    name: str
+    ident: str
+
+
+@dataclass(slots=True, kw_only=True)
 class CaseParty:
     """A dataclass representing a case party in a KMD Nova case."""
     uuid: Optional[str] = None
     role: Literal["Primær", "Sekundær"]
     identification_type: Literal["CprNummer", "CvrNummer", "Frit", "PNummer", "EsrNummer", "BfeNummer"]
     identification: str
     name: Optional[str] = None
@@ -47,16 +63,15 @@
 
 @dataclass(slots=True, kw_only=True)
 class Task:
     """A dataclass representing a KMD Nova task."""
     uuid: str
     title: str
     description: Optional[str] = None
-    case_worker_ident: Optional[str] = None
-    case_worker_uuid: str
+    caseworker: Caseworker
     status_code: Literal['N', 'S', 'F']  # Not Started, Started, Finished
     deadline: datetime
     created_date: Optional[datetime] = None
     started_date: Optional[datetime] = None
     closed_date: Optional[datetime] = None
 
 
@@ -66,12 +81,15 @@
     uuid: str
     title: str
     case_number: Optional[str] = None
     case_date: datetime
     active_code: Optional[str] = None
     progress_state: Literal["Opstaaet", "Oplyst", "Afgjort", "Bestilt", "Udfoert", "Afsluttet"]
     case_parties: list[CaseParty]
+    caseworker: Optional[Caseworker] = None
     document_count: Optional[int] = 0
     note_count: Optional[int] = 0
     kle_number: str
     proceeding_facet: str
     sensitivity: Literal["Fortrolige", "IkkeFortrolige", "SærligFølsomme", "Følsomme"]
+    responsible_department: Department
+    security_unit: Department
```

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/nova_tasks.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/nova_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 to the KMD Nova api."""
 import uuid
 import urllib.parse
 
 import requests
 
 from itk_dev_shared_components.kmd_nova.authentication import NovaAccess
-from itk_dev_shared_components.kmd_nova.nova_objects import Task
+from itk_dev_shared_components.kmd_nova.nova_objects import Task, Caseworker
 from itk_dev_shared_components.kmd_nova.util import datetime_from_iso_string, datetime_to_iso_string
 
 
 def attach_task_to_case(case_uuid: str, task: Task, nova_access: NovaAccess) -> None:
     """Attach a Task object to a case in Nova.
 
     The Task object must have the following values set:
@@ -31,15 +31,15 @@
         "common": {
             "transactionId": str(uuid.uuid4()),
             "uuid": task.uuid
         },
         "caseUuid": case_uuid,
         "title": task.title,
         "description": task.description,  # Optional
-        "caseworkerPersonId": task.case_worker_uuid,  # Optional
+        "caseworkerPersonId": task.caseworker.uuid,  # Optional
         "statusCode": task.status_code,
         "deadline": datetime_to_iso_string(task.deadline),
         "startDate": datetime_to_iso_string(task.started_date),  # Optional
         "closeDate": datetime_to_iso_string(task.closed_date),  # Optional
         "taskTypeName": "Aktivitet"
     }
 
@@ -85,27 +85,45 @@
 
     tasks = []
     for task_dict in response.json()['taskList']:
         task = Task(
             uuid = task_dict['taskUuid'],
             title = task_dict['taskTitle'],
             description = task_dict.get('taskDescription'),
-            case_worker_ident = task_dict['caseWorker']['ident'] if 'caseWorker' in task_dict else None,
-            case_worker_uuid = task_dict['caseWorker']['id'] if 'caseWorker' in task_dict else None,
+            caseworker = _extract_caseworker(task_dict),
             status_code = task_dict['taskStatusCode'],
             deadline = datetime_from_iso_string(task_dict.get('taskDeadline')),
             created_date = datetime_from_iso_string(task_dict.get('taskCreateDate')),
             started_date = datetime_from_iso_string(task_dict.get('taskStartDate')),
             closed_date = datetime_from_iso_string(task_dict.get('taskCloseDate'))
         )
         tasks.append(task)
 
     return tasks
 
 
+def _extract_caseworker(task_dict: dict) -> Caseworker | None:
+    """Extract the case worker from a HTTP request response.
+
+    Args:
+        case_dict: The dictionary describing the task.
+
+    Returns:
+        A case worker object describing the case worker if any.
+    """
+    if 'caseWorker' in task_dict:
+        return Caseworker(
+            uuid = task_dict['caseWorker']['id'],
+            ident = task_dict['caseWorker']['ident'],
+            name = task_dict['caseWorker']['name']
+        )
+
+    return None
+
+
 def update_task(task: Task, case_uuid: str, nova_access: NovaAccess):
     """Update a task that already exists in KMD Nova with new
     information.
 
     Args:
         task: The Task object describing the updated task.
         case_uuid: The id of the case the task belongs to.
@@ -121,15 +139,15 @@
         "common": {
             "transactionId": str(uuid.uuid4())
         },
         "uuid": task.uuid,
         "caseUuid": case_uuid,
         "title": task.title,
         "description": task.description,
-        "caseworkerPersonId": task.case_worker_uuid,
+        "caseworkerPersonId": task.caseworker.uuid,
         "statusCode": task.status_code,
         "deadline": datetime_to_iso_string(task.deadline),
         "startDate": datetime_to_iso_string(task.started_date),
         "closeDate": datetime_to_iso_string(task.closed_date),
         "taskType": "Aktivitet"
     }
```

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/kmd_nova/util.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/kmd_nova/util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/misc/cpr_util.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/misc/cpr_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/fmcacov.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/fmcacov.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/gridview_util.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/gridview_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/multi_session.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/multi_session.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/opret_kundekontakt.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/opret_kundekontakt.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/sap_login.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/sap_login.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/sap_util.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/sap_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components/sap/tree_util.py` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components/sap/tree_util.py`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components.egg-info/PKG-INFO` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itk_dev_shared_components
-Version: 1.3.1
+Version: 2.0.0
 Summary: Shared components to use in RPA projects
 Author-email: ITK Development <itk-rpa@mkb.aarhus.dk>
 Project-URL: Homepage, https://github.com/itk-dev-rpa/itk-dev-shared-components
 Project-URL: Bug Tracker, https://github.com/itk-dev-rpa/itk-dev-shared-components/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `itk_dev_shared_components-1.3.1/itk_dev_shared_components.egg-info/SOURCES.txt` & `itk_dev_shared_components-2.0.0/itk_dev_shared_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itk_dev_shared_components-1.3.1/pyproject.toml` & `itk_dev_shared_components-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "itk_dev_shared_components"
-version = "1.3.1"
+version = "2.0.0"
 authors = [
   { name="ITK Development", email="itk-rpa@mkb.aarhus.dk" },
 ]
 description = "Shared components to use in RPA projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

