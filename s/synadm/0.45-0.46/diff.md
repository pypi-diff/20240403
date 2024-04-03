# Comparing `tmp/synadm-0.45.tar.gz` & `tmp/synadm-0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synadm-0.45.tar", last modified: Wed Nov 29 16:11:22 2023, max compression
+gzip compressed data, was "synadm-0.46.tar", last modified: Wed Apr  3 07:41:10 2024, max compression
```

## Comparing `synadm-0.45.tar` & `synadm-0.46.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-11-29 16:11:22.029829 synadm-0.45/
--rw-r--r--   0 jojo       (501) staff       (20)    35148 2023-10-18 16:20:47.000000 synadm-0.45/LICENSE
--rw-r--r--   0 jojo       (501) staff       (20)    14717 2023-11-29 16:11:22.028680 synadm-0.45/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)    13498 2023-10-18 16:35:23.000000 synadm-0.45/README.md
--rw-r--r--   0 jojo       (501) staff       (20)       38 2023-11-29 16:11:22.030003 synadm-0.45/setup.cfg
--rwxr-xr-x   0 jojo       (501) staff       (20)     2245 2023-11-29 16:04:04.000000 synadm-0.45/setup.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-11-29 16:11:22.012983 synadm-0.45/synadm/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-10-18 16:20:47.000000 synadm-0.45/synadm/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)    55643 2023-11-29 15:57:24.000000 synadm-0.45/synadm/api.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-11-29 16:11:22.026076 synadm-0.45/synadm/cli/
--rw-r--r--   0 jojo       (501) staff       (20)    10316 2023-11-29 16:03:20.000000 synadm-0.45/synadm/cli/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)     1958 2023-10-18 16:35:42.000000 synadm-0.45/synadm/cli/_common.py
--rw-r--r--   0 jojo       (501) staff       (20)    10973 2023-11-29 16:03:20.000000 synadm-0.45/synadm/cli/_helper.py
--rw-r--r--   0 jojo       (501) staff       (20)     1458 2023-10-18 16:35:23.000000 synadm-0.45/synadm/cli/group.py
--rw-r--r--   0 jojo       (501) staff       (20)     4917 2023-10-18 16:35:23.000000 synadm-0.45/synadm/cli/history.py
--rw-r--r--   0 jojo       (501) staff       (20)     4823 2023-10-18 16:35:42.000000 synadm-0.45/synadm/cli/matrix.py
--rw-r--r--   0 jojo       (501) staff       (20)    10313 2023-10-18 16:35:23.000000 synadm-0.45/synadm/cli/media.py
--rw-r--r--   0 jojo       (501) staff       (20)     5891 2023-10-18 16:35:23.000000 synadm-0.45/synadm/cli/notice.py
--rw-r--r--   0 jojo       (501) staff       (20)     1979 2023-10-18 16:35:42.000000 synadm-0.45/synadm/cli/raw.py
--rw-r--r--   0 jojo       (501) staff       (20)     5438 2023-10-18 16:35:23.000000 synadm-0.45/synadm/cli/regtok.py
--rw-r--r--   0 jojo       (501) staff       (20)    14543 2023-10-18 16:35:42.000000 synadm-0.45/synadm/cli/room.py
--rw-r--r--   0 jojo       (501) staff       (20)    29424 2023-11-29 15:57:24.000000 synadm-0.45/synadm/cli/user.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-11-29 16:11:22.027488 synadm-0.45/synadm.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)    14717 2023-11-29 16:11:21.000000 synadm-0.45/synadm.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      489 2023-11-29 16:11:22.000000 synadm-0.45/synadm.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-11-29 16:11:21.000000 synadm-0.45/synadm.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)       43 2023-11-29 16:11:21.000000 synadm-0.45/synadm.egg-info/entry_points.txt
--rw-r--r--   0 jojo       (501) staff       (20)       77 2023-11-29 16:11:21.000000 synadm-0.45/synadm.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)        7 2023-11-29 16:11:21.000000 synadm-0.45/synadm.egg-info/top_level.txt
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2024-04-03 07:41:10.060047 synadm-0.46/
+-rw-r--r--   0 jackson    (501) staff       (20)    35148 2023-09-10 19:56:27.000000 synadm-0.46/LICENSE
+-rw-r--r--   0 jackson    (501) staff       (20)    14717 2024-04-03 07:41:10.059467 synadm-0.46/PKG-INFO
+-rw-r--r--   0 jackson    (501) staff       (20)    13498 2024-04-03 07:28:27.000000 synadm-0.46/README.md
+-rw-r--r--   0 jackson    (501) staff       (20)       38 2024-04-03 07:41:10.060134 synadm-0.46/setup.cfg
+-rwxr-xr-x   0 jackson    (501) staff       (20)     2245 2024-04-03 07:40:08.000000 synadm-0.46/setup.py
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2024-04-03 07:41:10.046235 synadm-0.46/synadm/
+-rw-r--r--   0 jackson    (501) staff       (20)        0 2023-09-10 19:56:27.000000 synadm-0.46/synadm/__init__.py
+-rw-r--r--   0 jackson    (501) staff       (20)     1046 2024-03-27 12:12:23.000000 synadm-0.46/synadm/__main__.py
+-rw-r--r--   0 jackson    (501) staff       (20)    56756 2024-04-03 07:30:29.000000 synadm-0.46/synadm/api.py
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2024-04-03 07:41:10.057890 synadm-0.46/synadm/cli/
+-rw-r--r--   0 jackson    (501) staff       (20)    10366 2024-04-03 07:28:27.000000 synadm-0.46/synadm/cli/__init__.py
+-rw-r--r--   0 jackson    (501) staff       (20)     1958 2024-03-27 12:12:23.000000 synadm-0.46/synadm/cli/_common.py
+-rw-r--r--   0 jackson    (501) staff       (20)    10973 2024-03-27 12:12:23.000000 synadm-0.46/synadm/cli/_helper.py
+-rw-r--r--   0 jackson    (501) staff       (20)     1458 2024-03-27 12:12:23.000000 synadm-0.46/synadm/cli/group.py
+-rw-r--r--   0 jackson    (501) staff       (20)     4917 2024-03-27 12:12:23.000000 synadm-0.46/synadm/cli/history.py
+-rw-r--r--   0 jackson    (501) staff       (20)     4823 2024-03-27 12:12:23.000000 synadm-0.46/synadm/cli/matrix.py
+-rw-r--r--   0 jackson    (501) staff       (20)    10387 2024-04-03 07:37:21.000000 synadm-0.46/synadm/cli/media.py
+-rw-r--r--   0 jackson    (501) staff       (20)     5891 2024-03-27 12:12:23.000000 synadm-0.46/synadm/cli/notice.py
+-rw-r--r--   0 jackson    (501) staff       (20)     1979 2024-03-27 12:12:23.000000 synadm-0.46/synadm/cli/raw.py
+-rw-r--r--   0 jackson    (501) staff       (20)     5438 2024-03-27 12:12:23.000000 synadm-0.46/synadm/cli/regtok.py
+-rw-r--r--   0 jackson    (501) staff       (20)    18402 2024-04-03 07:29:51.000000 synadm-0.46/synadm/cli/room.py
+-rw-r--r--   0 jackson    (501) staff       (20)    29424 2024-03-27 12:12:23.000000 synadm-0.46/synadm/cli/user.py
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2024-04-03 07:41:10.058948 synadm-0.46/synadm.egg-info/
+-rw-r--r--   0 jackson    (501) staff       (20)    14717 2024-04-03 07:41:10.000000 synadm-0.46/synadm.egg-info/PKG-INFO
+-rw-r--r--   0 jackson    (501) staff       (20)      508 2024-04-03 07:41:10.000000 synadm-0.46/synadm.egg-info/SOURCES.txt
+-rw-r--r--   0 jackson    (501) staff       (20)        1 2024-04-03 07:41:10.000000 synadm-0.46/synadm.egg-info/dependency_links.txt
+-rw-r--r--   0 jackson    (501) staff       (20)       43 2024-04-03 07:41:10.000000 synadm-0.46/synadm.egg-info/entry_points.txt
+-rw-r--r--   0 jackson    (501) staff       (20)       77 2024-04-03 07:41:10.000000 synadm-0.46/synadm.egg-info/requires.txt
+-rw-r--r--   0 jackson    (501) staff       (20)        7 2024-04-03 07:41:10.000000 synadm-0.46/synadm.egg-info/top_level.txt
```

### Comparing `synadm-0.45/LICENSE` & `synadm-0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `synadm-0.45/PKG-INFO` & `synadm-0.46/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synadm
-Version: 0.45
+Version: 0.46
 Summary: Command line admin tool for Synapse (Matrix reference homeserver)
 Home-page: https://github.com/joj0/synadm
 Author: Johannes Tiefenbacher
 Author-email: jt@peek-a-boo.at
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/joj0/synadm/issues
 Project-URL: Documentation, https://github.com/joj0/synadm
@@ -52,26 +52,26 @@
 - [Contributing](#contributing)
 
 
 
 
 ## About
 
-A CLI tool to help admins of [Matrix-Synapse homeservers](https://github.com/matrix-org/synapse) conveniently issue commands available via its [admin API](https://matrix-org.github.io/synapse/develop/usage/administration/admin_api/index.html#the-admin-api).
+A CLI tool to help admins of [Matrix-Synapse homeservers](https://github.com/matrix-org/synapse) conveniently issue commands available via its [Admin API](https://element-hq.github.io/synapse/develop/usage/administration/admin_api/index.html#the-admin-api).
 
 
 
 ## Prerequisites
 
 - Python 3.6+
 - a running Synapse instance
 - an admin-enabled user on the instance
 - the admin user's access token
 
-`synadm` is designed to run either directly on the host running the Synapse instance or on a remote machine able to access Synapse's API port. Synapse's default admin API endpoint address usually is http://localhost:8008/_synapse/admin or https://localhost:8448/_synapse/admin.
+`synadm` is designed to run either directly on the host running the Synapse instance or on a remote machine able to access Synapse's API port. Synapse's default Admin API endpoint address usually is http://localhost:8008/_synapse/admin or https://localhost:8448/_synapse/admin.
 
 
 
 
 ## Installation
 
 ### Install from PyPI
@@ -243,75 +243,75 @@
 
 *Note: If you installed it in [editable mode](CONTRIBUTING.md#4-install-in-editable-mode) (or for development), you can spare the `pip install .` command - just `git pull` and you're done.*
 
 
 
 ## Implementation Status / Commands List
 
-[Follow this link to the official Synapse Admin API docs](https://matrix-org.github.io/synapse/develop/usage/administration/admin_api/index.html) - direct links to the specific API documentation pages are provided in the list below.
+[Follow this link to the official Synapse Admin API docs](https://element-hq.github.io/synapse/develop/usage/administration/admin_api/index.html) - direct links to the specific API documentation pages are provided in the list below.
 
 *Note: Most commands have several optional arguments available. Put -h after any of the below listed commands to view them or have a look at the [Command Line Reference](https://synadm.readthedocs.io/en/latest/index_cli_reference.html).*
 
 
-* [ ] [Account Validity](https://matrix-org.github.io/synapse/develop/admin_api/account_validity.html)
-* [x] [Delete Group](https://matrix-org.github.io/synapse/develop/admin_api/delete_group.html) (delete community)
-* [ ] [Event Reports](https://matrix-org.github.io/synapse/develop/admin_api/event_reports.html)
-* [x] [Media Admin](https://matrix-org.github.io/synapse/develop/admin_api/media_admin_api.html)
+* [ ] [Account Validity](https://element-hq.github.io/synapse/develop/admin_api/account_validity.html)
+* [x] [Delete Group](https://element-hq.github.io/synapse/develop/admin_api/delete_group.html) (delete community)
+* [ ] [Event Reports](https://element-hq.github.io/synapse/develop/admin_api/event_reports.html)
+* [x] [Media Admin](https://element-hq.github.io/synapse/develop/admin_api/media_admin_api.html)
   * [x] `media list -r <room id>`
   * [x] `media list -u <user id>` (alias of `user media <user id>`)
   * [x] `media quarantine -s <server name> -i <media id>`
   * [x] `media quarantine -r <room id>`
   * [x] `media quarantine -u <room id>`
   * [x] `media protect <media id>`
   * [x] `media delete -s <server name> -i <media id>`
   * [x] `media delete -s <server name> --before <date> --size 1024`
   * [x] `media purge --before <date>` (purge remote media API)
-* [x] [Purge History](https://matrix-org.github.io/synapse/develop/admin_api/purge_history_api.html)
+* [x] [Purge History](https://element-hq.github.io/synapse/develop/admin_api/purge_history_api.html)
   * [x] `history purge <room id>`
   * [x] `history purge-status <purge id>`
-* [x] ~~[Purge Rooms](https://matrix-org.github.io/synapse/develop/admin_api/purge_room.html)~~ (DEPRECATED, covered by `room delete`)
-* [ ] [Register Users](https://matrix-org.github.io/synapse/develop/admin_api/register_api.html)
-* [x] [Manipulate Room Membership](https://matrix-org.github.io/synapse/develop/admin_api/room_membership.html)
+* [x] ~~[Purge Rooms](https://element-hq.github.io/synapse/develop/admin_api/purge_room.html)~~ (DEPRECATED, covered by `room delete`)
+* [ ] [Register Users](https://element-hq.github.io/synapse/develop/admin_api/register_api.html)
+* [x] [Manipulate Room Membership](https://element-hq.github.io/synapse/develop/admin_api/room_membership.html)
   * [x] `room join`
-* [x] [Rooms](https://matrix-org.github.io/synapse/develop/admin_api/rooms.html)
+* [x] [Rooms](https://element-hq.github.io/synapse/develop/admin_api/rooms.html)
   * [x] `room list`
   * [x] `room details <room id>`
   * [x] `room members <room id>`
   * [x] `room delete <room id>`
   * [x] `room make-admin <room id> <user id>`
   * [x] `room state <room id>`
   * [ ] Additional commands and aliases around room management
     * [x] `room search <search-term>` (alias of `room list -n <search-term>`)
     * [x] `room resolve <room alias>`
     * [x] `room power-levels`
     * [x] `room block`
     * [x] `room block-status`
-* [x] [Server Notices](https://matrix-org.github.io/synapse/develop/admin_api/server_notices.html)
-* [x] ~~[Shutdown Room](https://matrix-org.github.io/synapse/develop/admin_api/shutdown_room.html)~~ (DEPRECATED, covered by `room delete`)
-* [ ] [Statistics](https://matrix-org.github.io/synapse/develop/admin_api/statistics.html)
+* [x] [Server Notices](https://element-hq.github.io/synapse/develop/admin_api/server_notices.html)
+* [x] ~~[Shutdown Room](https://element-hq.github.io/synapse/develop/admin_api/shutdown_room.html)~~ (DEPRECATED, covered by `room delete`)
+* [ ] [Statistics](https://element-hq.github.io/synapse/develop/admin_api/statistics.html)
   * [ ] `synadm media user-stats`
   * [ ] `synadm room largest`
-* [x] [Users](https://matrix-org.github.io/synapse/develop/admin_api/user_admin_api.html)
+* [x] [Users](https://element-hq.github.io/synapse/develop/admin_api/user_admin_api.html)
   * [x] `user details <user id>`
   * [x] `user modify <user id>` (also used for user creation)
   * [x] `user list`
   * [x] `user deactivate <user id>` (including GDPR erase)
   * [x] `user password <user id>`
   * [x] `user membership <user id>`
   * [x] `user whois <user id>`
   * [x] `user shadow-ban <user id>`
   * [x] `user media -u <user id>` (also available as `media list -u <user id>`)
   * [x] `user login <user id>`
   * [ ] Additional commands and aliases around user management
       * [x] `user search <search-term>` (shortcut to `user list -d -g -n <search-term>`)
       * [ ] `user create <user id>` (alias of `user modify ...`)
       * [x] `user prune-devices <user id>`
-* [x] [Server Version](https://matrix-org.github.io/synapse/develop/admin_api/version_api.html)
+* [x] [Server Version](https://element-hq.github.io/synapse/develop/admin_api/version_api.html)
   * [x] `version`
-* [x] [Registration Tokens](https://matrix-org.github.io/synapse/latest/usage/administration/admin_api/registration_tokens.html)
+* [x] [Registration Tokens](https://element-hq.github.io/synapse/latest/usage/administration/admin_api/registration_tokens.html)
   * [x] `regtok list`
   * [x] `regtok details <registration token>`
   * [x] `regtok new`
   * [x] `regtok update <registration token>`
   * [x] `regtok delete <registration token>`
```

### Comparing `synadm-0.45/README.md` & `synadm-0.46/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 - [Contributing](#contributing)
 
 
 
 
 ## About
 
-A CLI tool to help admins of [Matrix-Synapse homeservers](https://github.com/matrix-org/synapse) conveniently issue commands available via its [admin API](https://matrix-org.github.io/synapse/develop/usage/administration/admin_api/index.html#the-admin-api).
+A CLI tool to help admins of [Matrix-Synapse homeservers](https://github.com/matrix-org/synapse) conveniently issue commands available via its [Admin API](https://element-hq.github.io/synapse/develop/usage/administration/admin_api/index.html#the-admin-api).
 
 
 
 ## Prerequisites
 
 - Python 3.6+
 - a running Synapse instance
 - an admin-enabled user on the instance
 - the admin user's access token
 
-`synadm` is designed to run either directly on the host running the Synapse instance or on a remote machine able to access Synapse's API port. Synapse's default admin API endpoint address usually is http://localhost:8008/_synapse/admin or https://localhost:8448/_synapse/admin.
+`synadm` is designed to run either directly on the host running the Synapse instance or on a remote machine able to access Synapse's API port. Synapse's default Admin API endpoint address usually is http://localhost:8008/_synapse/admin or https://localhost:8448/_synapse/admin.
 
 
 
 
 ## Installation
 
 ### Install from PyPI
@@ -212,75 +212,75 @@
 
 *Note: If you installed it in [editable mode](CONTRIBUTING.md#4-install-in-editable-mode) (or for development), you can spare the `pip install .` command - just `git pull` and you're done.*
 
 
 
 ## Implementation Status / Commands List
 
-[Follow this link to the official Synapse Admin API docs](https://matrix-org.github.io/synapse/develop/usage/administration/admin_api/index.html) - direct links to the specific API documentation pages are provided in the list below.
+[Follow this link to the official Synapse Admin API docs](https://element-hq.github.io/synapse/develop/usage/administration/admin_api/index.html) - direct links to the specific API documentation pages are provided in the list below.
 
 *Note: Most commands have several optional arguments available. Put -h after any of the below listed commands to view them or have a look at the [Command Line Reference](https://synadm.readthedocs.io/en/latest/index_cli_reference.html).*
 
 
-* [ ] [Account Validity](https://matrix-org.github.io/synapse/develop/admin_api/account_validity.html)
-* [x] [Delete Group](https://matrix-org.github.io/synapse/develop/admin_api/delete_group.html) (delete community)
-* [ ] [Event Reports](https://matrix-org.github.io/synapse/develop/admin_api/event_reports.html)
-* [x] [Media Admin](https://matrix-org.github.io/synapse/develop/admin_api/media_admin_api.html)
+* [ ] [Account Validity](https://element-hq.github.io/synapse/develop/admin_api/account_validity.html)
+* [x] [Delete Group](https://element-hq.github.io/synapse/develop/admin_api/delete_group.html) (delete community)
+* [ ] [Event Reports](https://element-hq.github.io/synapse/develop/admin_api/event_reports.html)
+* [x] [Media Admin](https://element-hq.github.io/synapse/develop/admin_api/media_admin_api.html)
   * [x] `media list -r <room id>`
   * [x] `media list -u <user id>` (alias of `user media <user id>`)
   * [x] `media quarantine -s <server name> -i <media id>`
   * [x] `media quarantine -r <room id>`
   * [x] `media quarantine -u <room id>`
   * [x] `media protect <media id>`
   * [x] `media delete -s <server name> -i <media id>`
   * [x] `media delete -s <server name> --before <date> --size 1024`
   * [x] `media purge --before <date>` (purge remote media API)
-* [x] [Purge History](https://matrix-org.github.io/synapse/develop/admin_api/purge_history_api.html)
+* [x] [Purge History](https://element-hq.github.io/synapse/develop/admin_api/purge_history_api.html)
   * [x] `history purge <room id>`
   * [x] `history purge-status <purge id>`
-* [x] ~~[Purge Rooms](https://matrix-org.github.io/synapse/develop/admin_api/purge_room.html)~~ (DEPRECATED, covered by `room delete`)
-* [ ] [Register Users](https://matrix-org.github.io/synapse/develop/admin_api/register_api.html)
-* [x] [Manipulate Room Membership](https://matrix-org.github.io/synapse/develop/admin_api/room_membership.html)
+* [x] ~~[Purge Rooms](https://element-hq.github.io/synapse/develop/admin_api/purge_room.html)~~ (DEPRECATED, covered by `room delete`)
+* [ ] [Register Users](https://element-hq.github.io/synapse/develop/admin_api/register_api.html)
+* [x] [Manipulate Room Membership](https://element-hq.github.io/synapse/develop/admin_api/room_membership.html)
   * [x] `room join`
-* [x] [Rooms](https://matrix-org.github.io/synapse/develop/admin_api/rooms.html)
+* [x] [Rooms](https://element-hq.github.io/synapse/develop/admin_api/rooms.html)
   * [x] `room list`
   * [x] `room details <room id>`
   * [x] `room members <room id>`
   * [x] `room delete <room id>`
   * [x] `room make-admin <room id> <user id>`
   * [x] `room state <room id>`
   * [ ] Additional commands and aliases around room management
     * [x] `room search <search-term>` (alias of `room list -n <search-term>`)
     * [x] `room resolve <room alias>`
     * [x] `room power-levels`
     * [x] `room block`
     * [x] `room block-status`
-* [x] [Server Notices](https://matrix-org.github.io/synapse/develop/admin_api/server_notices.html)
-* [x] ~~[Shutdown Room](https://matrix-org.github.io/synapse/develop/admin_api/shutdown_room.html)~~ (DEPRECATED, covered by `room delete`)
-* [ ] [Statistics](https://matrix-org.github.io/synapse/develop/admin_api/statistics.html)
+* [x] [Server Notices](https://element-hq.github.io/synapse/develop/admin_api/server_notices.html)
+* [x] ~~[Shutdown Room](https://element-hq.github.io/synapse/develop/admin_api/shutdown_room.html)~~ (DEPRECATED, covered by `room delete`)
+* [ ] [Statistics](https://element-hq.github.io/synapse/develop/admin_api/statistics.html)
   * [ ] `synadm media user-stats`
   * [ ] `synadm room largest`
-* [x] [Users](https://matrix-org.github.io/synapse/develop/admin_api/user_admin_api.html)
+* [x] [Users](https://element-hq.github.io/synapse/develop/admin_api/user_admin_api.html)
   * [x] `user details <user id>`
   * [x] `user modify <user id>` (also used for user creation)
   * [x] `user list`
   * [x] `user deactivate <user id>` (including GDPR erase)
   * [x] `user password <user id>`
   * [x] `user membership <user id>`
   * [x] `user whois <user id>`
   * [x] `user shadow-ban <user id>`
   * [x] `user media -u <user id>` (also available as `media list -u <user id>`)
   * [x] `user login <user id>`
   * [ ] Additional commands and aliases around user management
       * [x] `user search <search-term>` (shortcut to `user list -d -g -n <search-term>`)
       * [ ] `user create <user id>` (alias of `user modify ...`)
       * [x] `user prune-devices <user id>`
-* [x] [Server Version](https://matrix-org.github.io/synapse/develop/admin_api/version_api.html)
+* [x] [Server Version](https://element-hq.github.io/synapse/develop/admin_api/version_api.html)
   * [x] `version`
-* [x] [Registration Tokens](https://matrix-org.github.io/synapse/latest/usage/administration/admin_api/registration_tokens.html)
+* [x] [Registration Tokens](https://element-hq.github.io/synapse/latest/usage/administration/admin_api/registration_tokens.html)
   * [x] `regtok list`
   * [x] `regtok details <registration token>`
   * [x] `regtok new`
   * [x] `regtok update <registration token>`
   * [x] `regtok delete <registration token>`
```

### Comparing `synadm-0.45/setup.py` & `synadm-0.46/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from setuptools import setup, find_packages
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="synadm",
-    version="0.45",
+    version="0.46",
     author="Johannes Tiefenbacher",
     author_email="jt@peek-a-boo.at",
     description="Command line admin tool for Synapse (Matrix reference homeserver)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/joj0/synadm",
     project_urls={
```

### Comparing `synadm-0.45/synadm/api.py` & `synadm-0.46/synadm/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Synapse admin API and regular Matrix API clients
+"""Synapse Admin API and regular Matrix API clients
 
 Most API calls defined in this module respect the API's defaults and only pass
 what's necessary in the request body.
 
 A fully qualified Matrix user ID looks like this: @user:server, where server
 often is a domain name only, e.g @user@example.org
 
 See https://github.com/matrix-org/synapse/tree/master/docs/admin_api for
-documentation of the Synapse admin APIs and the Matrix spec at
+documentation of the Synapse Admin APIs and the Matrix spec at
 https://matrix.org/docs/spec/#matrix-apis.
 """
 
 import requests
 from http.client import HTTPConnection
 import datetime
 import json
@@ -378,15 +378,15 @@
             self.log.error("The homeserver name could not be fetched via the "
                            "federation API key/v2/server.")
             return None
         return resp['server_name']
 
 
 class SynapseAdmin(ApiRequest):
-    """Synapse admin API client
+    """Synapse Admin API client
 
     Inheritance:
         ApiRequest (object): parent class containing general properties and
             methods for requesting REST API's
     """
     def __init__(self, log, user, token, base_url, admin_path, timeout, debug,
                  verify):
@@ -420,15 +420,15 @@
 
         Args:
             _from (int): offsets user list by this number, used for pagination
             _limit (int): maximum number of users returned, used for pagination
             _guests (bool): enable/disable fetching of guest users
             _deactivated (bool): enable/disable fetching of deactivated users
             _name (string): user name localpart to search for, see Synapse
-                admin API docs for details
+                Admin API docs for details
             _user_id (string): fully qualified Matrix user ID to search for
             _admin (bool or None): whether to filter for admins. a None
                 does not filter.
 
         Returns:
             string: JSON string containing the found users
         """
@@ -453,22 +453,22 @@
         Args:
             _limit (int): Maximum number of users returned, used for
                 pagination.
             _guests (bool): Enable/disable fetching of guest users.
             _deactivated (bool): Enable/disable fetching of deactivated
                 users.
             _name (string): User name localpart to search for, see Synapse
-                admin API docs for details.
+                Admin API docs for details.
             _user_id (string): Fully qualified Matrix user ID to search for.
             _from (string): Offsets user list by this number, used for
                 pagination.
 
         Yields:
-            dict: The admin API response for listing accounts.
-                https://matrix-org.github.io/synapse/latest/admin_api/user_admin_api.html#list-accounts
+            dict: The Admin API response for listing accounts.
+                https://element-hq.github.io/synapse/latest/admin_api/user_admin_api.html#list-accounts
         """
         while _from is not None:
             response = self.user_list(_from, _limit, _guests, _deactivated,
                                       _name, _user_id, admin)
             yield response
             _from = response.get("next_token", None)
 
@@ -479,16 +479,16 @@
             user_id (string): Fully qualified Matrix user ID
             room_aliases (bool): Return human readable room aliases instead of
                 room ID's if applicable.
             matrix_api (object): An initialized Matrix object needs to be
                 passes as we need some Matrix API functionality here.
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-                an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+                an exception occured. See Synapse Admin API docs for details.
         """
 
         rooms = self.query("get", "v1/users/{user_id}/joined_rooms",
                            user_id=user_id)
         # Translate room ID's into aliases if requested.
         if return_aliases and rooms is not None and "joined_rooms" in rooms:
             for i, room_id in enumerate(rooms["joined_rooms"]):
@@ -499,56 +499,56 @@
 
     def user_deactivate(self, user_id, gdpr_erase):
         """Delete a given user
 
         Args:
             user_id (string): fully qualified Matrix user ID
             gdpr_erase (bool): enable/disable gdpr-erasing the user, see
-                Synapse admin API docs for details.
+                Synapse Admin API docs for details.
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-                an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+                an exception occured. See Synapse Admin API docs for details.
         """
         return self.query("post", "v1/deactivate/{user_id}", data={
             "erase": gdpr_erase
         }, user_id=user_id)
 
     def user_password(self, user_id, password, no_logout):
         """Set the user password, and log the user out if requested
 
         Args:
             user_id (string): fully qualified Matrix user ID
             password (string): new password that should be set
             no_logout (bool): the API defaults to logging out the user after
-                password reset via the admin API, this option can be used to
+                password reset via the Admin API, this option can be used to
                 disable this behaviour.
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-            an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+            an exception occured. See Synapse Admin API docs for details.
         """
         data = {"new_password": password}
         if no_logout:
             data.update({"logout_devices": False})
         return self.query("post", "v1/reset_password/{user_id}", data=data,
                           user_id=user_id)
 
     def user_details(self, user_id):
         """Get information about a given user
 
-        Note that the admin API docs describe this function as "Query User
+        Note that the Admin API docs describe this function as "Query User
         Account".
 
         Args:
             user_id (string): fully qualified Matrix user ID
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-                an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+                an exception occured. See Synapse Admin API docs for details.
 
         """
         return self.query("get", "v2/users/{user_id}", user_id=user_id)
 
     def user_login(self, user_id, expire_days, expire, _expire_ts):
         """Get an access token that can be used to authenticate as that user.
 
@@ -565,16 +565,16 @@
             user_id (string): fully qualified Matrix user ID
             expire_days (int): token should expire after this number of days
             expire (datetime): token should expire after this date/time - a
                 datetime object (e.g. as generated by Click.DateTime())
             _expire_ts (int):  token should expire after this date/time - a
                 unix timestamp in ms.
         Returns:
-            string: JSON string containing the admin API's response or None if
-            an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+            an exception occured. See Synapse Admin API docs for details.
         """
         expire_ts = None
         if expire_days:
             self.log.debug("Received expire_days: %s", expire_days)
             expire_ts = self._timestamp_from_days_ahead(expire_days)
         elif expire:
             self.log.debug("Received expire: %s", expire)
@@ -642,16 +642,16 @@
     def user_devices(self, user_id):
         """ Return information about all devices for a specific user.
 
         Args:
             user_id (string): Fully qualified Matrix user ID.
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-                an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+                an exception occured. See Synapse Admin API docs for details.
         """
         return self.query("get", "v2/users/{user_id}/devices",
                           user_id=user_id)
 
     def user_devices_get_todelete(self, devices_data, min_days, min_surviving,
                                   device_id, readable_seen):
         """ Gather a list of devices that possibly could be deleted.
@@ -770,14 +770,42 @@
             "from": _from,
             "limit": limit,
             "search_term": name,
             "order_by": order_by,
             "dir": "b" if reverse else None
         })
 
+    def room_list_paginate(self, limit, name, order_by, reverse, _from=0):
+        """ Yields API responses for room listing.
+
+        Args:
+            limit (int): Maximum number of rooms returned per pagination.
+            name (string or None): Search for a room by name. Passed as
+                `search_term` in the room list API. Use Python None to avoid
+                searching.
+            order_by (string): Synapse Room list API specific argument.
+            reverse (bool): Whether the results should be
+            _from (int): Initial offset in pagination.
+
+        Yields:
+            dict: The Admin API response for listing accounts.
+                https://element-hq.github.io/synapse/latest/admin_api/rooms.html#list-room-api
+        """
+        while _from is not None:
+            response = self.query("get", "v1/rooms", params={
+                "from": _from,
+                "limit": limit,
+                "search_term": name,
+                "order_by": order_by,
+                "dir": "b" if reverse else None
+            })
+            yield response
+            _from = response.get("next_batch", None)
+            self.log.debug(f"room_list_paginate: next from value = {_from}")
+
     def room_details(self, room_id):
         """ Get details about a room
         """
         return self.query("get", "v1/rooms/{room_id}", room_id=room_id)
 
     def room_members(self, room_id):
         """ Get a list of room members
@@ -787,32 +815,32 @@
     def room_state(self, room_id):
         """ Get a list of all state events in a room.
 
         Args:
             room_id (string)
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-                an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+                an exception occured. See Synapse Admin API docs for details.
         """
         return self.query("get", "v1/rooms/{room_id}/state", room_id=room_id)
 
     def room_power_levels(self, from_, limit, name, order_by, reverse,
                           room_id=None, all_details=True,
                           output_format="json"):
         """ Get a list of configured power_levels in all rooms.
 
         or a single room.
 
         Args:
             room_id (string): If left out, all rooms are fetched.
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-                an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+                an exception occured. See Synapse Admin API docs for details.
         """
         if room_id:
             # We use the "name search" possibility of the room list API to get
             # a single room via it's ID.
             rooms = self.room_list(from_, limit, room_id, order_by, reverse)
         else:
             rooms = self.room_list(from_, limit, name, order_by, reverse)
@@ -898,16 +926,16 @@
         """ Block or unblock a room.
 
         Args:
             room_id (string): Required.
             block (boolean): Whether to block or unblock a room.
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-                an exception occurred. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+                an exception occurred. See Synapse Admin API docs for details.
         """
         # TODO prevent usage on versions before 1.48
         data = {
             "block": block
         }
         return self.query("put", "v1/rooms/{room_id}/block", data=data,
                           room_id=room_id)
@@ -915,16 +943,16 @@
     def room_block_status(self, room_id):
         """ Returns if the room is blocked or not, and who blocked it.
 
         Args:
             room_id (string): Fully qualified Matrix room ID.
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-                an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+                an exception occured. See Synapse Admin API docs for details.
         """
         # TODO prevent usage on versions before 1.48
         return self.query("get", "v1/rooms/{room_id}/block", room_id=room_id)
 
     def room_make_admin(self, room_id, user_id):
         """ Grant a user room admin permission. If the user is not in the room,
         and it is not publicly joinable, then invite the user.
@@ -999,16 +1027,16 @@
         """ Delete a specific (local) media_id
         """
         return self.query(
             "delete", "v1/media/{server_name}/{media_id}", data={},
             server_name=server_name, media_id=media_id
         )
 
-    def media_delete_by_date_or_size(self, server_name, before_days, before,
-                                     _before_ts, _size_gt, delete_profiles):
+    def media_delete_by_date_or_size(self, before_days, before, _before_ts,
+                                     _size_gt, delete_profiles):
         """ Delete local media by date and/or size FIXME and/or?
         """
         if before_days:
             self.log.debug("Received --before-days: %s", before_days)
             before_ts = self._timestamp_from_days_ago(before_days)
         elif before:
             self.log.debug("Received --before: %s", before)
@@ -1021,15 +1049,14 @@
             self.log.debug("Something wrong in click FIXME")
 
         self.log.info("Deleting local media older than timestamp: %d,",
                       before_ts)
         self.log.info("which is the date: %s",
                       self._datetime_from_timestamp(before_ts))
         params = {
-            "server_name": server_name,
         }
         if before_ts is not None:
             params.update({
                 "before_ts": before_ts,
             })
         if _size_gt:
             size_gt = _size_gt * 1024
@@ -1039,16 +1066,15 @@
                 "size_gt": size_gt
             })
         if delete_profiles:
             params.update({
                 "keep_profiles": "false"
             })
         return self.query(
-            "post", "v1/media/{server_name}/delete", data={}, params=params,
-            server_name=server_name
+            "post", "v1/media/delete", data={}, params=params
         )
 
     def media_protect(self, media_id):
         """ Protect a single piece of local or remote media
 
         from being quarantined
         """
@@ -1148,16 +1174,16 @@
             valid (bool): List only valid (if True) or invalid (if False)
                 tokens. Default is to list all tokens regardless of validity.
             readable_expiry (bool): If True, replace the expiry_time field with
                 a human readable datetime. If False, expiry_time will be a unix
                 timestamp.
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-                an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+                an exception occured. See Synapse Admin API docs for details.
 
         """
         result = self.query("get", "v1/registration_tokens", params={
             "valid": (str(valid).lower() if isinstance(valid, bool) else None)
         })
 
         # Change expiry_time to a human readable format if requested
@@ -1181,16 +1207,16 @@
         Args:
             token (string): The registration token in question
             readable_expiry (bool): If True, replace the expiry_time field with
                 a human readable datetime. If False, expiry_time will be a unix
                 timestamp.
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-                an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+                an exception occured. See Synapse Admin API docs for details.
 
         """
         result = self.query("get", "v1/registration_tokens/{t}",
                             t=token)
 
         # Change expiry_time to a human readable format if requested
         if (
@@ -1217,16 +1243,16 @@
             expiry_ts (int): The latest time the registration token is valid.
                 Given as the number of milliseconds since
                 1970-01-01 00:00:00 UTC.
             expire_at (click.DateTime): The latest time the registration token
                 is valid.
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-                an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+                an exception occured. See Synapse Admin API docs for details.
 
         """
         data = {
             "length": length,
             "uses_allowed": uses_allowed,
         }
 
@@ -1255,16 +1281,16 @@
             expiry_ts (int): The latest time the registration token is valid.
                 Given as the number of milliseconds since
                 1970-01-01 00:00:00 UTC. -1 indicates no expiry.
             expire_at (click.DateTime): The latest time the registration token
                 is valid.
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-                an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+                an exception occured. See Synapse Admin API docs for details.
 
         """
         # If uses_allowed or expiry time were not provided by the user,
         # do not add the corresponding parameter to the request so that
         # the server will not modify its value.
         data = {}
 
@@ -1291,16 +1317,16 @@
     def regtok_delete(self, token):
         """ Delete a registration token
 
         Args:
             token (string): The registration token to delete
 
         Returns:
-            string: JSON string containing the admin API's response or None if
-                an exception occured. See Synapse admin API docs for details.
+            string: JSON string containing the Admin API's response or None if
+                an exception occured. See Synapse Admin API docs for details.
 
         """
         # t because query also accepts token when we want it for the
         # request
         # https://github.com/JOJ0/synadm/issues/110#issuecomment-1590032158
         return self.query("delete", "v1/registration_tokens/{t}",
                           t=token)
@@ -1332,16 +1358,16 @@
                 once.  Users are fetched with the user_list method and using
                 its pagination capabilities.
             to_regex (bool): Selects whether receivers should be interpreted as
                 a regular expression or a single recipient.
 
         Returns:
             list: A list of dictionaries, each containing the response of
-                what a single notice admin API call returned. Usually that is
-                an event ID or an error. See Synapse admin API docs for
+                what a single notice Admin API call returned. Usually that is
+                an event ID or an error. See Synapse Admin API docs for
                 details.
         """
         data = {
             "user_id": "",
             "content": {
                 "msgtype": "m.text",
                 "body": content_plain,
```

### Comparing `synadm-0.45/synadm/cli/__init__.py` & `synadm-0.46/synadm/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,27 +71,27 @@
         else:
             ctx.invoke(config_cmd)
 
 
 @root.command(name="config")
 @click.option(
     "--user", "-u", "user_", type=str,
-    help="Admin user allowed to access the Synapse admin API's.")
+    help="Admin user allowed to access the Synapse Admin API's.")
 @click.option(
     "--token", "-t", type=str,
     help="The Admin user's access token.")
 @click.option(
     "--base-url", "-b", type=str,
     help="""The base URL Synapse is running on. Typically this is
     https://localhost:8008 or https://localhost:8448. If Synapse is
-    configured to expose its admin API's to the outside world it might as
+    configured to expose its Admin API's to the outside world it might as
     well be something like this: https://example.org:8448""")
 @click.option(
     "--admin-path", "-p", type=str,
-    help="""The path Synapse provides its admin API's, usually the default fits
+    help="""The path Synapse provides its Admin API's, usually the default fits
     most installations.""")
 @click.option(
     "--matrix-path", "-m", type=str,
     help="""The path Synapse provides the regular Matrix API's, usually the
     default fits most installations.""")
 @click.option(
     "--timeout", "-w", type=int,
@@ -180,21 +180,21 @@
     helper.write_config({
         "user": click.prompt(
             "Synapse admin user name",
             default=user_ if user_ else helper.config.get("user", user_)),
         "token": click.prompt(
             get_redacted_token_prompt(token),
             default=token if token else helper.config.get("token", token),
-            show_default=False,),
+            show_default=False, hide_input=True),
         "base_url": click.prompt(
             "Synapse base URL",
             default=base_url if base_url else helper.config.get(
                 "base_url", base_url)),
         "admin_path": click.prompt(
-            "Synapse admin API path",
+            "Synapse Admin API path",
             default=admin_path if admin_path else helper.config.get(
                 "admin_path", admin_path)),
         "matrix_path": click.prompt(
             "Matrix API path",
             default=matrix_path if matrix_path else helper.config.get(
                 "matrix_path", matrix_path)),
         "format": click.prompt(
@@ -203,15 +203,16 @@
             type=click.Choice([
                 "yaml", "json", "minified", "human", "pprint"])),
         "timeout": click.prompt(
             "Default http timeout",
             default=timeout if timeout else helper.config.get(
                 "timeout", timeout)),
         "homeserver": click.prompt(
-            "Homeserver name (auto-retrieval or matrix.DOMAIN)",
+            "Homeserver name (\"auto-retrieval\" or the domain part in your "
+            "MXID)",
             default=homeserver if homeserver else helper.config.get(
                 "homeserver", homeserver)),
         "ssl_verify": click.prompt(
             "Verify certificate",
             type=bool,
             default=ssl_verify if ssl_verify else helper.config.get(
                 "ssl_verify", ssl_verify)),
```

### Comparing `synadm-0.45/synadm/cli/_common.py` & `synadm-0.46/synadm/cli/_common.py`

 * *Files identical despite different names*

### Comparing `synadm-0.45/synadm/cli/_helper.py` & `synadm-0.46/synadm/cli/_helper.py`

 * *Files identical despite different names*

### Comparing `synadm-0.45/synadm/cli/group.py` & `synadm-0.46/synadm/cli/group.py`

 * *Files identical despite different names*

### Comparing `synadm-0.45/synadm/cli/history.py` & `synadm-0.46/synadm/cli/history.py`

 * *Files identical despite different names*

### Comparing `synadm-0.45/synadm/cli/matrix.py` & `synadm-0.46/synadm/cli/matrix.py`

 * *Files identical despite different names*

### Comparing `synadm-0.45/synadm/cli/media.py` & `synadm-0.46/synadm/cli/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,16 @@
     "--before-ts", "-t", type=int,
     help="""Purge all media that was last accessed before this unix
     timestamp in ms.
     """)
 @click.pass_obj
 def media_purge_cmd(helper, before_days, before, before_ts):
     """ Purge old cached remote media
+
+    To delete local media, use `synadm media delete`
     """
     media_purged = helper.api.purge_media_cache(before_days, before, before_ts)
     if media_purged is None:
         click.echo("Media cache could not be purged.")
         raise SystemExit(1)
     helper.output(media_purged)
 
@@ -256,30 +258,31 @@
     help="""Also delete files that are still used in image data
     (e.g user profile, room avatar). If set, these files will be
     deleted too. Not valid when a specific media is being deleted
     (--media-id)""")
 @click.pass_obj
 def media_delete_cmd(helper, media_id, before_days, before, before_ts,
                      size, delete_profiles):
-    """ Delete media by ID, size or age
+    """ Delete local media by ID, size or age
+
+    To delete cached remote media, use `synadm media purge`
     """
-    server_name = helper.retrieve_homeserver_name(helper.config["base_url"])
-    if not server_name:
-        media_deleted = None
-    elif media_id and delete_profiles:
+    if media_id and delete_profiles:
         click.echo("Combination of --media-id and --delete-profiles not "
                    "valid.")
         media_deleted = None
     elif media_id and size:
         click.echo("Combination of --media-id and --size not valid.")
         media_deleted = None
     elif media_id:
+        server_name = helper.retrieve_homeserver_name(
+                helper.config["base_url"])
         media_deleted = helper.api.media_delete(server_name, media_id)
     else:
         media_deleted = helper.api.media_delete_by_date_or_size(
-            server_name, before_days, before, before_ts, size, delete_profiles
+            before_days, before, before_ts, size, delete_profiles
         )
 
     if media_deleted is None:
         click.echo("Media could not be deleted.")
         raise SystemExit(1)
     helper.output(media_deleted)
```

### Comparing `synadm-0.45/synadm/cli/notice.py` & `synadm-0.46/synadm/cli/notice.py`

 * *Files identical despite different names*

### Comparing `synadm-0.45/synadm/cli/raw.py` & `synadm-0.46/synadm/cli/raw.py`

 * *Files identical despite different names*

### Comparing `synadm-0.45/synadm/cli/regtok.py` & `synadm-0.46/synadm/cli/regtok.py`

 * *Files identical despite different names*

### Comparing `synadm-0.45/synadm/cli/room.py` & `synadm-0.46/synadm/cli/room.py`

 * *Files 12% similar despite different names*

```diff
@@ -292,14 +292,109 @@
             click.echo("Room not deleted.")
             raise SystemExit(1)
         helper.output(room_del)
     else:
         click.echo("Abort.")
 
 
+@room.command(name="purge-empty")
+@click.option(
+    "--no-purge", is_flag=True, default=False, show_default=True,
+    help="""Prevent removing of all traces of the room from your
+    database.""")
+@click.option(
+    "--force-purge", is_flag=True, default=False, show_default=True,
+    help="""Force a purge to go ahead even if there are local users still
+    in the room. Do not use this unless a regular purge operation fails,
+    as it could leave those users' clients in a confused state.""")
+@click.option(
+    "--v1", is_flag=True, default=False, show_default=True,
+    help="""Use version 1 of the room delete API instead of version 2""")
+@click.option(
+    "--dry-run", is_flag=True, default=False,
+    help="""Only show the rooms IDs that will be deleted""")
+@click.option(
+    "--batch-size", "--paginate", "-p", type=int, default=100,
+    show_default=True,
+    help="""How many rooms should be requested from the API one at a time.
+    This option has no effect on how many empty rooms will be deleted.
+
+    Increasing this is not necessary in most cases but useful if you have a
+    lot of rooms on your homeserver.""")
+@click.pass_obj
+def purge_empty(helper, no_purge, force_purge, v1, dry_run, batch_size):
+    """ Delete empty rooms (where 0 local members are currently in a room).
+    """
+    if no_purge and force_purge:
+        click.echo("--force-purge will be ignored as --no-purge is set")
+
+    empty_rooms_ids = []
+    for room_list_response in helper.api.room_list_paginate(
+            batch_size, None, "joined_local_members", True):
+        found_empty_rooms = False
+
+        if "rooms" not in room_list_response.keys():
+            helper.log.warn("\"rooms\" key is missing from room list"
+                            "response.")
+
+        for room in room_list_response["rooms"]:
+            room_id = room["room_id"]
+            joined_local_members = room["joined_local_members"]
+            if joined_local_members == 0:
+                helper.log.debug(f"Added {room_id} to delete "
+                                 f"(joined local members is "
+                                 f"{joined_local_members})")
+                empty_rooms_ids.append(room_id)
+                found_empty_rooms = True
+            else:
+                helper.log.debug(f"Skipping {room_id} (joined local "
+                                 f"members is {joined_local_members}, "
+                                 f"not 0)")
+                # very early cut off, hopefully always works and is never
+                # wrong
+                found_empty_rooms = False
+                break
+
+        # list is sorted by joined_local_members from smallest to biggest,
+        # if there's no more where joined_local_members == 0 then just stop
+        # early
+        if not found_empty_rooms:
+            helper.log.debug("No more empty rooms, stopping room list "
+                             "fetching early.")
+            break
+
+    helper.output(empty_rooms_ids)
+    if dry_run:
+        click.echo("Empty room purge dry run. Rooms will not be deleted "
+                   "is listed.", err=True)
+        return
+
+    sure = (
+        helper.no_confirm or
+        click.prompt("Are you sure you want to delete the listed empty "
+                     "rooms? (y/N)", type=bool, default=False,
+                     show_default=False)
+    )
+    if not sure:
+        click.echo("Abort.", err=True)
+        raise SystemExit(1)
+
+    for room_id in empty_rooms_ids:
+        if v1:
+            result = helper.api.room_delete(
+                    room_id, None, None, None, False, not no_purge,
+                    force_purge)
+            helper.output(result)
+        else:
+            result = helper.api.room_delete_v2(
+                    room_id, None, None, None, False, not no_purge,
+                    force_purge)
+            helper.output(result)
+
+
 @room.command(name="delete-status")
 @optgroup.group(
         "Query type", cls=RequiredMutuallyExclusiveOptionGroup,
         help="Query room deletion status via either Room ID or Deletion ID"
 )
 @optgroup.option(
         "--room-id", "-r", type=str,
```

### Comparing `synadm-0.45/synadm/cli/user.py` & `synadm-0.46/synadm/cli/user.py`

 * *Files identical despite different names*

### Comparing `synadm-0.45/synadm.egg-info/PKG-INFO` & `synadm-0.46/synadm.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synadm
-Version: 0.45
+Version: 0.46
 Summary: Command line admin tool for Synapse (Matrix reference homeserver)
 Home-page: https://github.com/joj0/synadm
 Author: Johannes Tiefenbacher
 Author-email: jt@peek-a-boo.at
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/joj0/synadm/issues
 Project-URL: Documentation, https://github.com/joj0/synadm
@@ -52,26 +52,26 @@
 - [Contributing](#contributing)
 
 
 
 
 ## About
 
-A CLI tool to help admins of [Matrix-Synapse homeservers](https://github.com/matrix-org/synapse) conveniently issue commands available via its [admin API](https://matrix-org.github.io/synapse/develop/usage/administration/admin_api/index.html#the-admin-api).
+A CLI tool to help admins of [Matrix-Synapse homeservers](https://github.com/matrix-org/synapse) conveniently issue commands available via its [Admin API](https://element-hq.github.io/synapse/develop/usage/administration/admin_api/index.html#the-admin-api).
 
 
 
 ## Prerequisites
 
 - Python 3.6+
 - a running Synapse instance
 - an admin-enabled user on the instance
 - the admin user's access token
 
-`synadm` is designed to run either directly on the host running the Synapse instance or on a remote machine able to access Synapse's API port. Synapse's default admin API endpoint address usually is http://localhost:8008/_synapse/admin or https://localhost:8448/_synapse/admin.
+`synadm` is designed to run either directly on the host running the Synapse instance or on a remote machine able to access Synapse's API port. Synapse's default Admin API endpoint address usually is http://localhost:8008/_synapse/admin or https://localhost:8448/_synapse/admin.
 
 
 
 
 ## Installation
 
 ### Install from PyPI
@@ -243,75 +243,75 @@
 
 *Note: If you installed it in [editable mode](CONTRIBUTING.md#4-install-in-editable-mode) (or for development), you can spare the `pip install .` command - just `git pull` and you're done.*
 
 
 
 ## Implementation Status / Commands List
 
-[Follow this link to the official Synapse Admin API docs](https://matrix-org.github.io/synapse/develop/usage/administration/admin_api/index.html) - direct links to the specific API documentation pages are provided in the list below.
+[Follow this link to the official Synapse Admin API docs](https://element-hq.github.io/synapse/develop/usage/administration/admin_api/index.html) - direct links to the specific API documentation pages are provided in the list below.
 
 *Note: Most commands have several optional arguments available. Put -h after any of the below listed commands to view them or have a look at the [Command Line Reference](https://synadm.readthedocs.io/en/latest/index_cli_reference.html).*
 
 
-* [ ] [Account Validity](https://matrix-org.github.io/synapse/develop/admin_api/account_validity.html)
-* [x] [Delete Group](https://matrix-org.github.io/synapse/develop/admin_api/delete_group.html) (delete community)
-* [ ] [Event Reports](https://matrix-org.github.io/synapse/develop/admin_api/event_reports.html)
-* [x] [Media Admin](https://matrix-org.github.io/synapse/develop/admin_api/media_admin_api.html)
+* [ ] [Account Validity](https://element-hq.github.io/synapse/develop/admin_api/account_validity.html)
+* [x] [Delete Group](https://element-hq.github.io/synapse/develop/admin_api/delete_group.html) (delete community)
+* [ ] [Event Reports](https://element-hq.github.io/synapse/develop/admin_api/event_reports.html)
+* [x] [Media Admin](https://element-hq.github.io/synapse/develop/admin_api/media_admin_api.html)
   * [x] `media list -r <room id>`
   * [x] `media list -u <user id>` (alias of `user media <user id>`)
   * [x] `media quarantine -s <server name> -i <media id>`
   * [x] `media quarantine -r <room id>`
   * [x] `media quarantine -u <room id>`
   * [x] `media protect <media id>`
   * [x] `media delete -s <server name> -i <media id>`
   * [x] `media delete -s <server name> --before <date> --size 1024`
   * [x] `media purge --before <date>` (purge remote media API)
-* [x] [Purge History](https://matrix-org.github.io/synapse/develop/admin_api/purge_history_api.html)
+* [x] [Purge History](https://element-hq.github.io/synapse/develop/admin_api/purge_history_api.html)
   * [x] `history purge <room id>`
   * [x] `history purge-status <purge id>`
-* [x] ~~[Purge Rooms](https://matrix-org.github.io/synapse/develop/admin_api/purge_room.html)~~ (DEPRECATED, covered by `room delete`)
-* [ ] [Register Users](https://matrix-org.github.io/synapse/develop/admin_api/register_api.html)
-* [x] [Manipulate Room Membership](https://matrix-org.github.io/synapse/develop/admin_api/room_membership.html)
+* [x] ~~[Purge Rooms](https://element-hq.github.io/synapse/develop/admin_api/purge_room.html)~~ (DEPRECATED, covered by `room delete`)
+* [ ] [Register Users](https://element-hq.github.io/synapse/develop/admin_api/register_api.html)
+* [x] [Manipulate Room Membership](https://element-hq.github.io/synapse/develop/admin_api/room_membership.html)
   * [x] `room join`
-* [x] [Rooms](https://matrix-org.github.io/synapse/develop/admin_api/rooms.html)
+* [x] [Rooms](https://element-hq.github.io/synapse/develop/admin_api/rooms.html)
   * [x] `room list`
   * [x] `room details <room id>`
   * [x] `room members <room id>`
   * [x] `room delete <room id>`
   * [x] `room make-admin <room id> <user id>`
   * [x] `room state <room id>`
   * [ ] Additional commands and aliases around room management
     * [x] `room search <search-term>` (alias of `room list -n <search-term>`)
     * [x] `room resolve <room alias>`
     * [x] `room power-levels`
     * [x] `room block`
     * [x] `room block-status`
-* [x] [Server Notices](https://matrix-org.github.io/synapse/develop/admin_api/server_notices.html)
-* [x] ~~[Shutdown Room](https://matrix-org.github.io/synapse/develop/admin_api/shutdown_room.html)~~ (DEPRECATED, covered by `room delete`)
-* [ ] [Statistics](https://matrix-org.github.io/synapse/develop/admin_api/statistics.html)
+* [x] [Server Notices](https://element-hq.github.io/synapse/develop/admin_api/server_notices.html)
+* [x] ~~[Shutdown Room](https://element-hq.github.io/synapse/develop/admin_api/shutdown_room.html)~~ (DEPRECATED, covered by `room delete`)
+* [ ] [Statistics](https://element-hq.github.io/synapse/develop/admin_api/statistics.html)
   * [ ] `synadm media user-stats`
   * [ ] `synadm room largest`
-* [x] [Users](https://matrix-org.github.io/synapse/develop/admin_api/user_admin_api.html)
+* [x] [Users](https://element-hq.github.io/synapse/develop/admin_api/user_admin_api.html)
   * [x] `user details <user id>`
   * [x] `user modify <user id>` (also used for user creation)
   * [x] `user list`
   * [x] `user deactivate <user id>` (including GDPR erase)
   * [x] `user password <user id>`
   * [x] `user membership <user id>`
   * [x] `user whois <user id>`
   * [x] `user shadow-ban <user id>`
   * [x] `user media -u <user id>` (also available as `media list -u <user id>`)
   * [x] `user login <user id>`
   * [ ] Additional commands and aliases around user management
       * [x] `user search <search-term>` (shortcut to `user list -d -g -n <search-term>`)
       * [ ] `user create <user id>` (alias of `user modify ...`)
       * [x] `user prune-devices <user id>`
-* [x] [Server Version](https://matrix-org.github.io/synapse/develop/admin_api/version_api.html)
+* [x] [Server Version](https://element-hq.github.io/synapse/develop/admin_api/version_api.html)
   * [x] `version`
-* [x] [Registration Tokens](https://matrix-org.github.io/synapse/latest/usage/administration/admin_api/registration_tokens.html)
+* [x] [Registration Tokens](https://element-hq.github.io/synapse/latest/usage/administration/admin_api/registration_tokens.html)
   * [x] `regtok list`
   * [x] `regtok details <registration token>`
   * [x] `regtok new`
   * [x] `regtok update <registration token>`
   * [x] `regtok delete <registration token>`
```

