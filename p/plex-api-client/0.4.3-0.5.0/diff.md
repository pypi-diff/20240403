# Comparing `tmp/plex-api-client-0.4.3.tar.gz` & `tmp/plex-api-client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-api-client-0.4.3.tar", last modified: Fri Mar 29 16:38:20 2024, max compression
+gzip compressed data, was "plex-api-client-0.5.0.tar", last modified: Wed Apr  3 01:14:00 2024, max compression
```

## Comparing `plex-api-client-0.4.3.tar` & `plex-api-client-0.5.0.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:38:20.932633 plex-api-client-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    15327 2024-03-29 16:38:20.932633 plex-api-client-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 16:38:20.932633 plex-api-client-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:38:20.908633 plex-api-client-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:38:20.912633 plex-api-client-0.4.3/src/plex_api/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:38:20.912633 plex-api-client-0.4.3/src/plex_api/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    17553 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/hubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    41270 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:38:20.912633 plex-api-client-0.4.3/src/plex_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:38:20.912633 plex-api-client-0.4.3/src/plex_api/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:38:20.920633 plex-api-client-0.4.3/src/plex_api/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/errors/uploadplaylist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:38:20.932633 plex-api-client-0.4.3/src/plex_api/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21445 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getlibraryitems.py
--rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/searchlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/models/operations/uploadplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    33349 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/plex.py
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    27097 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    13857 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:38:20.932633 plex-api-client-0.4.3/src/plex_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-03-29 16:38:08.000000 plex-api-client-0.4.3/src/plex_api/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:38:20.932633 plex-api-client-0.4.3/src/plex_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15327 2024-03-29 16:38:20.000000 plex-api-client-0.4.3/src/plex_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-03-29 16:38:20.000000 plex-api-client-0.4.3/src/plex_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:38:20.000000 plex-api-client-0.4.3/src/plex_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-29 16:38:20.000000 plex-api-client-0.4.3/src/plex_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-29 16:38:20.000000 plex-api-client-0.4.3/src/plex_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.793893 plex-api-client-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17401 2024-04-03 01:14:00.793893 plex-api-client-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14179 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:14:00.793893 plex-api-client-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.773893 plex-api-client-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.773893 plex-api-client-0.5.0/src/plex_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.777893 plex-api-client-0.5.0/src/plex_api/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17617 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/hubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41590 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11615 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.777893 plex-api-client-0.5.0/src/plex_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.777893 plex-api-client-0.5.0/src/plex_api/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.785893 plex-api-client-0.5.0/src/plex_api/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/errors/uploadplaylist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.793893 plex-api-client-0.5.0/src/plex_api/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21445 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getlibraryitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/searchlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/models/operations/uploadplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33733 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/plex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13135 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.793893 plex-api-client-0.5.0/src/plex_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-03 01:13:48.000000 plex-api-client-0.5.0/src/plex_api/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:00.793893 plex-api-client-0.5.0/src/plex_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17401 2024-04-03 01:14:00.000000 plex-api-client-0.5.0/src/plex_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-03 01:14:00.000000 plex-api-client-0.5.0/src/plex_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:14:00.000000 plex-api-client-0.5.0/src/plex_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 01:14:00.000000 plex-api-client-0.5.0/src/plex_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 01:14:00.000000 plex-api-client-0.5.0/src/plex_api_client.egg-info/top_level.txt
```

### Comparing `plex-api-client-0.4.3/LICENSE.md` & `plex-api-client-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/PKG-INFO` & `plex-api-client-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.4.3
+Version: 0.5.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
@@ -28,14 +28,15 @@
         ### Example
         
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
+            x_plex_client_identifier='<value>',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -167,14 +168,15 @@
         
         ```python
         import plex_api
         from plex_api.models import errors
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
+            x_plex_client_identifier='<value>',
         )
         
         
         res = None
         try:
             res = s.server.get_server_capabilities()
         except errors.GetServerCapabilitiesResponseBody as e:
@@ -206,14 +208,15 @@
         
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             server_idx=0,
             access_token="<YOUR_API_KEY_HERE>",
+            x_plex_client_identifier='<value>',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -233,14 +236,15 @@
         The default server can also be overridden globally by passing a URL to the `server_url: str` optional parameter when initializing the SDK client instance. For example:
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             server_url="{protocol}://{ip}:{port}",
             access_token="<YOUR_API_KEY_HERE>",
+            x_plex_client_identifier='<value>',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -250,18 +254,20 @@
         
         ### Override Server URL Per-Operation
         
         The server URL can also be overridden on a per-operation basis, provided a server list was specified for the operation. For example:
         ```python
         import plex_api
         
-        s = plex_api.PlexAPI()
+        s = plex_api.PlexAPI(
+            x_plex_client_identifier='<value>',
+        )
         
         
-        res = s.plex.get_pin(server_url="https://plex.tv/api/v2", x_plex_client_identifier='<value>', strong=False)
+        res = s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False, x_plex_client_identifier='<value>')
         
         if res.object is not None:
             # handle response
             pass
         
         ```
         <!-- End Server Selection [server] -->
@@ -295,26 +301,66 @@
         
         To authenticate with the API the `access_token` parameter must be set when initializing the SDK client instance. For example:
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
+            x_plex_client_identifier='<value>',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
         <!-- End Authentication [security] -->
         
+        <!-- Start Global Parameters [global-parameters] -->
+        ## Global Parameters
+        
+        A parameter is configured globally. This parameter must be set on the SDK client instance itself during initialization. When configured as an option during SDK initialization, This global value will be used as the default on the operations that use it. When such operations are called, there is a place in each to override the global value, if needed.
+        
+        For example, you can set `X-Plex-Client-Identifier` to `'<value>'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_pin`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
+        
+        
+        ### Available Globals
+        
+        The following global parameter is available. The required parameter must be set when you initialize the SDK client.
+        
+        | Name | Type | Required | Description |
+        | ---- | ---- |:--------:| ----------- |
+        | x_plex_client_identifier | str | ✔️ | The unique identifier for the client application
+        This is used to track the client application and its usage
+        (UUID, serial number, or other number unique per device)
+         |
+        
+        
+        ### Example
+        
+        ```python
+        import plex_api
+        
+        s = plex_api.PlexAPI(
+            x_plex_client_identifier='<value>',
+        )
+        
+        
+        res = s.plex.get_pin(strong=False, x_plex_client_identifier='<value>')
+        
+        if res.object is not None:
+            # handle response
+            pass
+        
+        ```
+        <!-- End Global Parameters [global-parameters] -->
+        
         <!-- Placeholder for Future Speakeasy SDK Sections -->
         
         # Development
         
         ## Maturity
         
         This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.4.3 Summary: Python
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.5.0 Summary: Python
 Client SDK Generated by Speakeasy Home-page: UNKNOWN Author: LukeHagar License:
 UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
-( access_token="", ) res = s.server.get_server_capabilities() if res.object is
-not None: # handle response pass ``` ## Available Resources and Operations ###
-[server](docs/sdks/server/README.md) * [get_server_capabilities](docs/sdks/
-server/README.md#get_server_capabilities) - Server Capabilities *
+( access_token="", x_plex_client_identifier='', ) res =
+s.server.get_server_capabilities() if res.object is not None: # handle response
+pass ``` ## Available Resources and Operations ### [server](docs/sdks/server/
+README.md) * [get_server_capabilities](docs/sdks/server/
+README.md#get_server_capabilities) - Server Capabilities *
 [get_server_preferences](docs/sdks/server/README.md#get_server_preferences) -
 Get Server Preferences * [get_available_clients](docs/sdks/server/
 README.md#get_available_clients) - Get Available Clients * [get_devices](docs/
 sdks/server/README.md#get_devices) - Get Devices * [get_server_identity](docs/
 sdks/server/README.md#get_server_identity) - Get Server Identity *
 [get_my_plex_account](docs/sdks/server/README.md#get_my_plex_account) - Get
 MyPlex Account * [get_resized_photo](docs/sdks/server/
@@ -96,61 +97,80 @@
 expectations. All operations return a response object or raise an error. If
 Error objects are specified in your OpenAPI Spec, the SDK will raise the
 appropriate Error type. | Error Object | Status Code | Content Type | | -------
 --------------------------------- | ---------------------------------------- |
 ---------------------------------------- | |
 errors.GetServerCapabilitiesResponseBody | 401 | application/json | |
 errors.SDKError | 4x-5xx | */* | ### Example ```python import plex_api from
-plex_api.models import errors s = plex_api.PlexAPI( access_token="", ) res =
-None try: res = s.server.get_server_capabilities() except
+plex_api.models import errors s = plex_api.PlexAPI( access_token="",
+x_plex_client_identifier='', ) res = None try: res =
+s.server.get_server_capabilities() except
 errors.GetServerCapabilitiesResponseBody as e: # handle exception raise(e)
 except errors.SDKError as e: # handle exception raise(e) if res.object is not
 None: # handle response pass ``` ## Server Selection ### Select Server by Index
 You can override the default server globally by passing a server index to the
 `server_idx: int` optional parameter when initializing the SDK client instance.
 The selected server will then be used as the default on the operations that use
 it. This table lists the indexes associated with the available servers: | # |
 Server | Variables | | - | ------ | --------- | | 0 | `{protocol}://{ip}:
 {port}` | `protocol` (default is `http`), `ip` (default is `10.10.10.47`),
 `port` (default is `32400`) | #### Example ```python import plex_api s =
-plex_api.PlexAPI( server_idx=0, access_token="", ) res =
-s.server.get_server_capabilities() if res.object is not None: # handle response
-pass ``` #### Variables Some of the server options above contain variables. If
-you want to set the values of those variables, the following optional
-parameters are available when initializing the SDK client instance: *
+plex_api.PlexAPI( server_idx=0, access_token="", x_plex_client_identifier='', )
+res = s.server.get_server_capabilities() if res.object is not None: # handle
+response pass ``` #### Variables Some of the server options above contain
+variables. If you want to set the values of those variables, the following
+optional parameters are available when initializing the SDK client instance: *
 `protocol: models.ServerProtocol` * `ip: str` * `port: str` ### Override Server
 URL Per-Client The default server can also be overridden globally by passing a
 URL to the `server_url: str` optional parameter when initializing the SDK
 client instance. For example: ```python import plex_api s = plex_api.PlexAPI
-( server_url="{protocol}://{ip}:{port}", access_token="", ) res =
+( server_url="{protocol}://{ip}:{port}", access_token="",
+x_plex_client_identifier='', ) res = s.server.get_server_capabilities() if
+res.object is not None: # handle response pass ``` ### Override Server URL Per-
+Operation The server URL can also be overridden on a per-operation basis,
+provided a server list was specified for the operation. For example: ```python
+import plex_api s = plex_api.PlexAPI( x_plex_client_identifier='', ) res =
+s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False,
+x_plex_client_identifier='') if res.object is not None: # handle response pass
+``` ## Custom HTTP Client The Python SDK makes API calls using the [requests]
+(https://pypi.org/project/requests/) HTTP library. In order to provide a
+convenient way to configure timeouts, cookies, proxies, custom headers, and
+other low-level configuration, you can initialize the SDK client with a custom
+`requests.Session` object. For example, you could specify a header for every
+request that this sdk makes as follows: ```python import plex_api import
+requests http_client = requests.Session() http_client.headers.update({'x-
+custom-header': 'someValue'}) s = plex_api.PlexAPI(client: http_client) ``` ##
+Authentication ### Per-Client Security Schemes This SDK supports the following
+security scheme globally: | Name | Type | Scheme | | -------------- | ---------
+----- | -------------- | | `access_token` | apiKey | API key | To authenticate
+with the API the `access_token` parameter must be set when initializing the SDK
+client instance. For example: ```python import plex_api s = plex_api.PlexAPI
+( access_token="", x_plex_client_identifier='', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
-pass ``` ### Override Server URL Per-Operation The server URL can also be
-overridden on a per-operation basis, provided a server list was specified for
-the operation. For example: ```python import plex_api s = plex_api.PlexAPI()
-res = s.plex.get_pin(server_url="https://plex.tv/api/v2",
-x_plex_client_identifier='', strong=False) if res.object is not None: # handle
-response pass ``` ## Custom HTTP Client The Python SDK makes API calls using
-the [requests](https://pypi.org/project/requests/) HTTP library. In order to
-provide a convenient way to configure timeouts, cookies, proxies, custom
-headers, and other low-level configuration, you can initialize the SDK client
-with a custom `requests.Session` object. For example, you could specify a
-header for every request that this sdk makes as follows: ```python import
-plex_api import requests http_client = requests.Session()
-http_client.headers.update({'x-custom-header': 'someValue'}) s =
-plex_api.PlexAPI(client: http_client) ``` ## Authentication ### Per-Client
-Security Schemes This SDK supports the following security scheme globally: |
-Name | Type | Scheme | | -------------- | -------------- | -------------- | |
-`access_token` | apiKey | API key | To authenticate with the API the
-`access_token` parameter must be set when initializing the SDK client instance.
-For example: ```python import plex_api s = plex_api.PlexAPI( access_token="", )
-res = s.server.get_server_capabilities() if res.object is not None: # handle
-response pass ``` # Development ## Maturity This SDK is in beta, and there may
-be breaking changes between versions without a major version update. Therefore,
-we recommend pinning usage to a specific package version. This way, you can
-install the same version each time without breaking changes unless you are
-intentionally looking for the latest version. ## Contributions While we value
-open-source contributions to this SDK, this library is generated
+pass ``` ## Global Parameters A parameter is configured globally. This
+parameter must be set on the SDK client instance itself during initialization.
+When configured as an option during SDK initialization, This global value will
+be used as the default on the operations that use it. When such operations are
+called, there is a place in each to override the global value, if needed. For
+example, you can set `X-Plex-Client-Identifier` to `''` at SDK initialization
+and then you do not have to pass the same value on calls to operations like
+`get_pin`. But if you want to do so you may, which will locally override the
+global setting. See the example code below for a demonstration. ### Available
+Globals The following global parameter is available. The required parameter
+must be set when you initialize the SDK client. | Name | Type | Required |
+Description | | ---- | ---- |:--------:| ----------- | |
+x_plex_client_identifier | str | âï¸ | The unique identifier for the client
+application This is used to track the client application and its usage (UUID,
+serial number, or other number unique per device) | ### Example ```python
+import plex_api s = plex_api.PlexAPI( x_plex_client_identifier='', ) res =
+s.plex.get_pin(strong=False, x_plex_client_identifier='') if res.object is not
+None: # handle response pass ``` # Development ## Maturity This SDK is in beta,
+and there may be breaking changes between versions without a major version
+update. Therefore, we recommend pinning usage to a specific package version.
+This way, you can install the same version each time without breaking changes
+unless you are intentionally looking for the latest version. ## Contributions
+While we value open-source contributions to this SDK, this library is generated
 programmatically. Feel free to open a PR or a Github issue as a proof of
 concept and we'll do our best to include it in a future release! ### SDK
 Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
 client-sdks) Platform: UNKNOWN Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: dev
```

### Comparing `plex-api-client-0.4.3/README.md` & `plex-api-client-0.5.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 ### Example
 
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
     access_token="<YOUR_API_KEY_HERE>",
+    x_plex_client_identifier='<value>',
 )
 
 
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
@@ -160,14 +161,15 @@
 
 ```python
 import plex_api
 from plex_api.models import errors
 
 s = plex_api.PlexAPI(
     access_token="<YOUR_API_KEY_HERE>",
+    x_plex_client_identifier='<value>',
 )
 
 
 res = None
 try:
     res = s.server.get_server_capabilities()
 except errors.GetServerCapabilitiesResponseBody as e:
@@ -199,14 +201,15 @@
 
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
     server_idx=0,
     access_token="<YOUR_API_KEY_HERE>",
+    x_plex_client_identifier='<value>',
 )
 
 
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
@@ -226,14 +229,15 @@
 The default server can also be overridden globally by passing a URL to the `server_url: str` optional parameter when initializing the SDK client instance. For example:
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
     server_url="{protocol}://{ip}:{port}",
     access_token="<YOUR_API_KEY_HERE>",
+    x_plex_client_identifier='<value>',
 )
 
 
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
@@ -243,18 +247,20 @@
 
 ### Override Server URL Per-Operation
 
 The server URL can also be overridden on a per-operation basis, provided a server list was specified for the operation. For example:
 ```python
 import plex_api
 
-s = plex_api.PlexAPI()
+s = plex_api.PlexAPI(
+    x_plex_client_identifier='<value>',
+)
 
 
-res = s.plex.get_pin(server_url="https://plex.tv/api/v2", x_plex_client_identifier='<value>', strong=False)
+res = s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False, x_plex_client_identifier='<value>')
 
 if res.object is not None:
     # handle response
     pass
 
 ```
 <!-- End Server Selection [server] -->
@@ -288,26 +294,66 @@
 
 To authenticate with the API the `access_token` parameter must be set when initializing the SDK client instance. For example:
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
     access_token="<YOUR_API_KEY_HERE>",
+    x_plex_client_identifier='<value>',
 )
 
 
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
     pass
 
 ```
 <!-- End Authentication [security] -->
 
+<!-- Start Global Parameters [global-parameters] -->
+## Global Parameters
+
+A parameter is configured globally. This parameter must be set on the SDK client instance itself during initialization. When configured as an option during SDK initialization, This global value will be used as the default on the operations that use it. When such operations are called, there is a place in each to override the global value, if needed.
+
+For example, you can set `X-Plex-Client-Identifier` to `'<value>'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_pin`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
+
+
+### Available Globals
+
+The following global parameter is available. The required parameter must be set when you initialize the SDK client.
+
+| Name | Type | Required | Description |
+| ---- | ---- |:--------:| ----------- |
+| x_plex_client_identifier | str | ✔️ | The unique identifier for the client application
+This is used to track the client application and its usage
+(UUID, serial number, or other number unique per device)
+ |
+
+
+### Example
+
+```python
+import plex_api
+
+s = plex_api.PlexAPI(
+    x_plex_client_identifier='<value>',
+)
+
+
+res = s.plex.get_pin(strong=False, x_plex_client_identifier='<value>')
+
+if res.object is not None:
+    # handle response
+    pass
+
+```
+<!-- End Global Parameters [global-parameters] -->
+
 <!-- Placeholder for Future Speakeasy SDK Sections -->
 
 # Development
 
 ## Maturity
 
 This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
 # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
-( access_token="", ) res = s.server.get_server_capabilities() if res.object is
-not None: # handle response pass ``` ## Available Resources and Operations ###
-[server](docs/sdks/server/README.md) * [get_server_capabilities](docs/sdks/
-server/README.md#get_server_capabilities) - Server Capabilities *
+( access_token="", x_plex_client_identifier='', ) res =
+s.server.get_server_capabilities() if res.object is not None: # handle response
+pass ``` ## Available Resources and Operations ### [server](docs/sdks/server/
+README.md) * [get_server_capabilities](docs/sdks/server/
+README.md#get_server_capabilities) - Server Capabilities *
 [get_server_preferences](docs/sdks/server/README.md#get_server_preferences) -
 Get Server Preferences * [get_available_clients](docs/sdks/server/
 README.md#get_available_clients) - Get Available Clients * [get_devices](docs/
 sdks/server/README.md#get_devices) - Get Devices * [get_server_identity](docs/
 sdks/server/README.md#get_server_identity) - Get Server Identity *
 [get_my_plex_account](docs/sdks/server/README.md#get_my_plex_account) - Get
 MyPlex Account * [get_resized_photo](docs/sdks/server/
@@ -94,60 +95,79 @@
 expectations. All operations return a response object or raise an error. If
 Error objects are specified in your OpenAPI Spec, the SDK will raise the
 appropriate Error type. | Error Object | Status Code | Content Type | | -------
 --------------------------------- | ---------------------------------------- |
 ---------------------------------------- | |
 errors.GetServerCapabilitiesResponseBody | 401 | application/json | |
 errors.SDKError | 4x-5xx | */* | ### Example ```python import plex_api from
-plex_api.models import errors s = plex_api.PlexAPI( access_token="", ) res =
-None try: res = s.server.get_server_capabilities() except
+plex_api.models import errors s = plex_api.PlexAPI( access_token="",
+x_plex_client_identifier='', ) res = None try: res =
+s.server.get_server_capabilities() except
 errors.GetServerCapabilitiesResponseBody as e: # handle exception raise(e)
 except errors.SDKError as e: # handle exception raise(e) if res.object is not
 None: # handle response pass ``` ## Server Selection ### Select Server by Index
 You can override the default server globally by passing a server index to the
 `server_idx: int` optional parameter when initializing the SDK client instance.
 The selected server will then be used as the default on the operations that use
 it. This table lists the indexes associated with the available servers: | # |
 Server | Variables | | - | ------ | --------- | | 0 | `{protocol}://{ip}:
 {port}` | `protocol` (default is `http`), `ip` (default is `10.10.10.47`),
 `port` (default is `32400`) | #### Example ```python import plex_api s =
-plex_api.PlexAPI( server_idx=0, access_token="", ) res =
-s.server.get_server_capabilities() if res.object is not None: # handle response
-pass ``` #### Variables Some of the server options above contain variables. If
-you want to set the values of those variables, the following optional
-parameters are available when initializing the SDK client instance: *
+plex_api.PlexAPI( server_idx=0, access_token="", x_plex_client_identifier='', )
+res = s.server.get_server_capabilities() if res.object is not None: # handle
+response pass ``` #### Variables Some of the server options above contain
+variables. If you want to set the values of those variables, the following
+optional parameters are available when initializing the SDK client instance: *
 `protocol: models.ServerProtocol` * `ip: str` * `port: str` ### Override Server
 URL Per-Client The default server can also be overridden globally by passing a
 URL to the `server_url: str` optional parameter when initializing the SDK
 client instance. For example: ```python import plex_api s = plex_api.PlexAPI
-( server_url="{protocol}://{ip}:{port}", access_token="", ) res =
+( server_url="{protocol}://{ip}:{port}", access_token="",
+x_plex_client_identifier='', ) res = s.server.get_server_capabilities() if
+res.object is not None: # handle response pass ``` ### Override Server URL Per-
+Operation The server URL can also be overridden on a per-operation basis,
+provided a server list was specified for the operation. For example: ```python
+import plex_api s = plex_api.PlexAPI( x_plex_client_identifier='', ) res =
+s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False,
+x_plex_client_identifier='') if res.object is not None: # handle response pass
+``` ## Custom HTTP Client The Python SDK makes API calls using the [requests]
+(https://pypi.org/project/requests/) HTTP library. In order to provide a
+convenient way to configure timeouts, cookies, proxies, custom headers, and
+other low-level configuration, you can initialize the SDK client with a custom
+`requests.Session` object. For example, you could specify a header for every
+request that this sdk makes as follows: ```python import plex_api import
+requests http_client = requests.Session() http_client.headers.update({'x-
+custom-header': 'someValue'}) s = plex_api.PlexAPI(client: http_client) ``` ##
+Authentication ### Per-Client Security Schemes This SDK supports the following
+security scheme globally: | Name | Type | Scheme | | -------------- | ---------
+----- | -------------- | | `access_token` | apiKey | API key | To authenticate
+with the API the `access_token` parameter must be set when initializing the SDK
+client instance. For example: ```python import plex_api s = plex_api.PlexAPI
+( access_token="", x_plex_client_identifier='', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
-pass ``` ### Override Server URL Per-Operation The server URL can also be
-overridden on a per-operation basis, provided a server list was specified for
-the operation. For example: ```python import plex_api s = plex_api.PlexAPI()
-res = s.plex.get_pin(server_url="https://plex.tv/api/v2",
-x_plex_client_identifier='', strong=False) if res.object is not None: # handle
-response pass ``` ## Custom HTTP Client The Python SDK makes API calls using
-the [requests](https://pypi.org/project/requests/) HTTP library. In order to
-provide a convenient way to configure timeouts, cookies, proxies, custom
-headers, and other low-level configuration, you can initialize the SDK client
-with a custom `requests.Session` object. For example, you could specify a
-header for every request that this sdk makes as follows: ```python import
-plex_api import requests http_client = requests.Session()
-http_client.headers.update({'x-custom-header': 'someValue'}) s =
-plex_api.PlexAPI(client: http_client) ``` ## Authentication ### Per-Client
-Security Schemes This SDK supports the following security scheme globally: |
-Name | Type | Scheme | | -------------- | -------------- | -------------- | |
-`access_token` | apiKey | API key | To authenticate with the API the
-`access_token` parameter must be set when initializing the SDK client instance.
-For example: ```python import plex_api s = plex_api.PlexAPI( access_token="", )
-res = s.server.get_server_capabilities() if res.object is not None: # handle
-response pass ``` # Development ## Maturity This SDK is in beta, and there may
-be breaking changes between versions without a major version update. Therefore,
-we recommend pinning usage to a specific package version. This way, you can
-install the same version each time without breaking changes unless you are
-intentionally looking for the latest version. ## Contributions While we value
-open-source contributions to this SDK, this library is generated
+pass ``` ## Global Parameters A parameter is configured globally. This
+parameter must be set on the SDK client instance itself during initialization.
+When configured as an option during SDK initialization, This global value will
+be used as the default on the operations that use it. When such operations are
+called, there is a place in each to override the global value, if needed. For
+example, you can set `X-Plex-Client-Identifier` to `''` at SDK initialization
+and then you do not have to pass the same value on calls to operations like
+`get_pin`. But if you want to do so you may, which will locally override the
+global setting. See the example code below for a demonstration. ### Available
+Globals The following global parameter is available. The required parameter
+must be set when you initialize the SDK client. | Name | Type | Required |
+Description | | ---- | ---- |:--------:| ----------- | |
+x_plex_client_identifier | str | âï¸ | The unique identifier for the client
+application This is used to track the client application and its usage (UUID,
+serial number, or other number unique per device) | ### Example ```python
+import plex_api s = plex_api.PlexAPI( x_plex_client_identifier='', ) res =
+s.plex.get_pin(strong=False, x_plex_client_identifier='') if res.object is not
+None: # handle response pass ``` # Development ## Maturity This SDK is in beta,
+and there may be breaking changes between versions without a major version
+update. Therefore, we recommend pinning usage to a specific package version.
+This way, you can install the same version each time without breaking changes
+unless you are intentionally looking for the latest version. ## Contributions
+While we value open-source contributions to this SDK, this library is generated
 programmatically. Feel free to open a PR or a Github issue as a proof of
 concept and we'll do our best to include it in a future release! ### SDK
 Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
 client-sdks)
```

### Comparing `plex-api-client-0.4.3/setup.py` & `plex-api-client-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="plex-api-client",
-    version="0.4.3",
+    version="0.5.0",
     author="LukeHagar",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2023.7.22",
```

### Comparing `plex-api-client-0.4.3/src/plex_api/_hooks/registration.py` & `plex-api-client-0.5.0/src/plex_api/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/_hooks/sdkhooks.py` & `plex-api-client-0.5.0/src/plex_api/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/_hooks/types.py` & `plex-api-client-0.5.0/src/plex_api/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/activities.py` & `plex-api-client-0.5.0/src/plex_api/activities.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         hook_ctx = HookContext(operation_id='cancelServerActivities', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CancelServerActivitiesRequest(
             activity_uuid=activity_uuid,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CancelServerActivitiesRequest, base_url, '/activities/{activityUUID}', request)
+        url = utils.generate_url(operations.CancelServerActivitiesRequest, base_url, '/activities/{activityUUID}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
```

### Comparing `plex-api-client-0.4.3/src/plex_api/authentication.py` & `plex-api-client-0.5.0/src/plex_api/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         url = base_url + '/security/token'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetTransientTokenRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetTransientTokenRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -96,15 +96,15 @@
         url = base_url + '/security/resources'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetSourceConnectionInformationRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetSourceConnectionInformationRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx,
```

### Comparing `plex-api-client-0.4.3/src/plex_api/butler.py` & `plex-api-client-0.5.0/src/plex_api/butler.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         hook_ctx = HookContext(operation_id='startTask', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.StartTaskRequest(
             task_name=task_name,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.StartTaskRequest, base_url, '/butler/{taskName}', request)
+        url = utils.generate_url(operations.StartTaskRequest, base_url, '/butler/{taskName}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -280,15 +280,15 @@
         hook_ctx = HookContext(operation_id='stopTask', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.StopTaskRequest(
             task_name=task_name,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.StopTaskRequest, base_url, '/butler/{taskName}', request)
+        url = utils.generate_url(operations.StopTaskRequest, base_url, '/butler/{taskName}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
```

### Comparing `plex-api-client-0.4.3/src/plex_api/hubs.py` & `plex-api-client-0.5.0/src/plex_api/hubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         url = base_url + '/hubs'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetGlobalHubsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetGlobalHubsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -96,22 +96,22 @@
             section_id=section_id,
             count=count,
             only_transient=only_transient,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetLibraryHubsRequest, base_url, '/hubs/sections/{sectionId}', request)
+        url = utils.generate_url(operations.GetLibraryHubsRequest, base_url, '/hubs/sections/{sectionId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetLibraryHubsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetLibraryHubsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx,
```

### Comparing `plex-api-client-0.4.3/src/plex_api/library.py` & `plex-api-client-0.5.0/src/plex_api/library.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         url = base_url + '/library/hashes'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetFileHashRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetFileHashRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -263,22 +263,22 @@
         request = operations.GetLibraryRequest(
             section_id=section_id,
             include_details=include_details,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetLibraryRequest, base_url, '/library/sections/{sectionId}', request)
+        url = utils.generate_url(operations.GetLibraryRequest, base_url, '/library/sections/{sectionId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetLibraryRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetLibraryRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -333,15 +333,15 @@
         hook_ctx = HookContext(operation_id='deleteLibrary', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.DeleteLibraryRequest(
             section_id=section_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteLibraryRequest, base_url, '/library/sections/{sectionId}', request)
+        url = utils.generate_url(operations.DeleteLibraryRequest, base_url, '/library/sections/{sectionId}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -417,15 +417,15 @@
         request = operations.GetLibraryItemsRequest(
             section_id=section_id,
             tag=tag,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetLibraryItemsRequest, base_url, '/library/sections/{sectionId}/{tag}', request)
+        url = utils.generate_url(operations.GetLibraryItemsRequest, base_url, '/library/sections/{sectionId}/{tag}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -478,15 +478,15 @@
         hook_ctx = HookContext(operation_id='refreshLibrary', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.RefreshLibraryRequest(
             section_id=section_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RefreshLibraryRequest, base_url, '/library/sections/{sectionId}/refresh', request)
+        url = utils.generate_url(operations.RefreshLibraryRequest, base_url, '/library/sections/{sectionId}/refresh', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -560,22 +560,22 @@
         request = operations.SearchLibraryRequest(
             section_id=section_id,
             type=type_,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.SearchLibraryRequest, base_url, '/library/sections/{sectionId}/search', request)
+        url = utils.generate_url(operations.SearchLibraryRequest, base_url, '/library/sections/{sectionId}/search', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.SearchLibraryRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.SearchLibraryRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -622,15 +622,15 @@
         hook_ctx = HookContext(operation_id='getMetadata', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetMetadataRequest(
             rating_key=rating_key,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetMetadataRequest, base_url, '/library/metadata/{ratingKey}', request)
+        url = utils.generate_url(operations.GetMetadataRequest, base_url, '/library/metadata/{ratingKey}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -691,15 +691,15 @@
         hook_ctx = HookContext(operation_id='getMetadataChildren', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetMetadataChildrenRequest(
             rating_key=rating_key,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetMetadataChildrenRequest, base_url, '/library/metadata/{ratingKey}/children', request)
+        url = utils.generate_url(operations.GetMetadataChildrenRequest, base_url, '/library/metadata/{ratingKey}/children', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
```

### Comparing `plex-api-client-0.4.3/src/plex_api/log.py` & `plex-api-client-0.5.0/src/plex_api/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         url = base_url + '/log'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.LogLineRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.LogLineRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx,
```

### Comparing `plex-api-client-0.4.3/src/plex_api/media.py` & `plex-api-client-0.5.0/src/plex_api/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         url = base_url + '/:/scrobble'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.MarkPlayedRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.MarkPlayedRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -94,15 +94,15 @@
         url = base_url + '/:/unscrobble'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.MarkUnplayedRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.MarkUnplayedRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -161,15 +161,15 @@
         url = base_url + '/:/progress'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.UpdatePlayProgressRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.UpdatePlayProgressRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx,
```

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/__init__.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/addplaylistcontents.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/applyupdates.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/applyupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/cancelserveractivities.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/checkforupdates.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/checkforupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/clearplaylistcontents.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/createplaylist.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/createplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/deletelibrary.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/deleteplaylist.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/enablepapertrail.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getavailableclients.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getbutlertasks.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getdevices.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getfilehash.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getglobalhubs.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getglobalhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getlibraries.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getlibrary.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getlibraryhubs.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getlibraryhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getmetadata.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getmetadatachildren.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getmyplexaccount.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getondeck.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getondeck.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getpin.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getpin.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getplaylist.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getplaylistcontents.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getplaylists.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getplaylists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getrecentlyadded.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getrecentlyadded.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getresizedphoto.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getresizedphoto.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getsearchresults.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getsearchresults.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getserveractivities.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getservercapabilities.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getservercapabilities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getserveridentity.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getserverlist.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getserverpreferences.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getsessionhistory.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getsessions.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getsourceconnectioninformation.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getstatistics.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/gettimeline.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/gettimeline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/gettoken.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/gettoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/gettranscodesessions.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/gettranscodesessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/gettransienttoken.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/gettransienttoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/getupdatestatus.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/logline.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/logline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/logmultiline.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/markplayed.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/markunplayed.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/performsearch.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/performvoicesearch.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/refreshlibrary.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/sdkerror.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/startalltasks.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/starttask.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/starttask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/startuniversaltranscode.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/stopalltasks.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/stoptask.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/stoptask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/stoptranscodesession.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/updateplaylist.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/updateplayprogress.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/errors/uploadplaylist.py` & `plex-api-client-0.5.0/src/plex_api/models/errors/uploadplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/__init__.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/addplaylistcontents.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/applyupdates.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/applyupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/cancelserveractivities.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/checkforupdates.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/checkforupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/clearplaylistcontents.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/createplaylist.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/createplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/deletelibrary.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/deleteplaylist.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/enablepapertrail.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getavailableclients.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getbutlertasks.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getdevices.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getfilehash.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getglobalhubs.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getglobalhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getlibraries.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getlibrary.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getlibraryhubs.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getlibraryhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getlibraryitems.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getlibraryitems.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getmetadata.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getmetadatachildren.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getmyplexaccount.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getondeck.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getondeck.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getpin.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getpin.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 GET_PIN_SERVERS = [
 	"https://plex.tv/api/v2",
 ]
 
 
 @dataclasses.dataclass
 class GetPinRequest:
-    x_plex_client_identifier: str = dataclasses.field(metadata={'header': { 'field_name': 'X-Plex-Client-Identifier', 'style': 'simple', 'explode': False }})
-    r"""The unique identifier for the client application
-    This is used to track the client application and its usage
-    (UUID, serial number, or other number unique per device)
-    """
     strong: Optional[bool] = dataclasses.field(default=False, metadata={'query_param': { 'field_name': 'strong', 'style': 'form', 'explode': True }})
     r"""Determines the kind of code returned by the API call
     Strong codes are used for Pin authentication flows
     Non-Strong codes are used for `Plex.tv/link`
     """
+    x_plex_client_identifier: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Plex-Client-Identifier', 'style': 'simple', 'explode': False }})
+    r"""The unique identifier for the client application
+    This is used to track the client application and its usage
+    (UUID, serial number, or other number unique per device)
+    """
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Location:
```

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getplaylist.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getplaylistcontents.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getplaylists.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getplaylists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getrecentlyadded.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getrecentlyadded.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getresizedphoto.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getresizedphoto.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getsearchresults.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getsearchresults.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getserveractivities.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getservercapabilities.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getservercapabilities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getserveridentity.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getserverlist.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getserverpreferences.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getsessionhistory.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getsessions.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getsourceconnectioninformation.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getstatistics.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/gettimeline.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/gettimeline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/gettoken.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/gettoken.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from typing import Optional
 
 GET_TOKEN_SERVERS = [
 	"https://plex.tv/api/v2",
 ]
 
 
 @dataclasses.dataclass
 class GetTokenRequest:
     pin_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'pinID', 'style': 'simple', 'explode': False }})
     r"""The PinID to retrieve an access token for"""
-    x_plex_client_identifier: str = dataclasses.field(metadata={'header': { 'field_name': 'X-Plex-Client-Identifier', 'style': 'simple', 'explode': False }})
+    x_plex_client_identifier: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'X-Plex-Client-Identifier', 'style': 'simple', 'explode': False }})
     r"""The unique identifier for the client application
     This is used to track the client application and its usage
     (UUID, serial number, or other number unique per device)
     """
```

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/gettranscodesessions.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/gettranscodesessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/gettransienttoken.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/gettransienttoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/getupdatestatus.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/logline.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/logline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/logmultiline.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/markplayed.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/markunplayed.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/performsearch.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/performvoicesearch.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/refreshlibrary.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/searchlibrary.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/searchlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/startalltasks.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/starttask.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/starttask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/startuniversaltranscode.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/stopalltasks.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/stoptask.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/stoptask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/stoptranscodesession.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/updateplaylist.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/updateplayprogress.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/models/operations/uploadplaylist.py` & `plex-api-client-0.5.0/src/plex_api/models/operations/uploadplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/playlists.py` & `plex-api-client-0.5.0/src/plex_api/playlists.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         url = base_url + '/playlists'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.CreatePlaylistRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.CreatePlaylistRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -103,15 +103,15 @@
         url = base_url + '/playlists'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetPlaylistsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetPlaylistsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -167,15 +167,15 @@
         hook_ctx = HookContext(operation_id='getPlaylist', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetPlaylistRequest(
             playlist_id=playlist_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPlaylistRequest, base_url, '/playlists/{playlistID}', request)
+        url = utils.generate_url(operations.GetPlaylistRequest, base_url, '/playlists/{playlistID}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -236,15 +236,15 @@
         hook_ctx = HookContext(operation_id='deletePlaylist', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.DeletePlaylistRequest(
             playlist_id=playlist_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeletePlaylistRequest, base_url, '/playlists/{playlistID}', request)
+        url = utils.generate_url(operations.DeletePlaylistRequest, base_url, '/playlists/{playlistID}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -302,22 +302,22 @@
             playlist_id=playlist_id,
             title=title,
             summary=summary,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdatePlaylistRequest, base_url, '/playlists/{playlistID}', request)
+        url = utils.generate_url(operations.UpdatePlaylistRequest, base_url, '/playlists/{playlistID}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.UpdatePlaylistRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.UpdatePlaylistRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -371,22 +371,22 @@
         request = operations.GetPlaylistContentsRequest(
             playlist_id=playlist_id,
             type=type_,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPlaylistContentsRequest, base_url, '/playlists/{playlistID}/items', request)
+        url = utils.generate_url(operations.GetPlaylistContentsRequest, base_url, '/playlists/{playlistID}/items', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetPlaylistContentsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetPlaylistContentsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -441,15 +441,15 @@
         hook_ctx = HookContext(operation_id='clearPlaylistContents', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ClearPlaylistContentsRequest(
             playlist_id=playlist_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ClearPlaylistContentsRequest, base_url, '/playlists/{playlistID}/items', request)
+        url = utils.generate_url(operations.ClearPlaylistContentsRequest, base_url, '/playlists/{playlistID}/items', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -508,22 +508,22 @@
             playlist_id=playlist_id,
             uri=uri,
             play_queue_id=play_queue_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.AddPlaylistContentsRequest, base_url, '/playlists/{playlistID}/items', request)
+        url = utils.generate_url(operations.AddPlaylistContentsRequest, base_url, '/playlists/{playlistID}/items', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.AddPlaylistContentsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.AddPlaylistContentsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -586,15 +586,15 @@
         url = base_url + '/playlists/upload'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.UploadPlaylistRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.UploadPlaylistRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx,
```

### Comparing `plex-api-client-0.4.3/src/plex_api/plex.py` & `plex-api-client-0.5.0/src/plex_api/plex.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,36 +12,36 @@
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def get_pin(self, x_plex_client_identifier: str, strong: Optional[bool] = None, server_url: Optional[str] = None) -> operations.GetPinResponse:
+    def get_pin(self, strong: Optional[bool] = None, x_plex_client_identifier: Optional[str] = None, server_url: Optional[str] = None) -> operations.GetPinResponse:
         r"""Get a Pin
         Retrieve a Pin from Plex.tv for authentication flows
         """
         hook_ctx = HookContext(operation_id='getPin', oauth2_scopes=[], security_source=None)
         request = operations.GetPinRequest(
-            x_plex_client_identifier=x_plex_client_identifier,
             strong=strong,
+            x_plex_client_identifier=x_plex_client_identifier,
         )
         
         base_url = utils.template_url(operations.GET_PIN_SERVERS[0], {
         })
         if server_url is not None:
             base_url = server_url
         
         url = base_url + '/pins'
         
         headers = {}
         query_params = {}
         
-        headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.GetPinRequest, request), **query_params }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        query_params = { **utils.get_query_params(operations.GetPinRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -85,34 +85,34 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_token(self, pin_id: str, x_plex_client_identifier: str, server_url: Optional[str] = None) -> operations.GetTokenResponse:
+    def get_token(self, pin_id: str, x_plex_client_identifier: Optional[str] = None, server_url: Optional[str] = None) -> operations.GetTokenResponse:
         r"""Get Access Token
         Retrieve an Access Token from Plex.tv after the Pin has already been authenticated
         """
         hook_ctx = HookContext(operation_id='getToken', oauth2_scopes=[], security_source=None)
         request = operations.GetTokenRequest(
             pin_id=pin_id,
             x_plex_client_identifier=x_plex_client_identifier,
         )
         
         base_url = utils.template_url(operations.GET_TOKEN_SERVERS[0], {
         })
         if server_url is not None:
             base_url = server_url
         
-        url = utils.generate_url(operations.GetTokenRequest, base_url, '/pins/{pinID}', request)
+        url = utils.generate_url(operations.GetTokenRequest, base_url, '/pins/{pinID}', request, self.sdk_configuration.globals)
         
         headers = {}
         
-        headers = { **utils.get_headers(request), **headers }
+        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx,
```

### Comparing `plex-api-client-0.4.3/src/plex_api/sdk.py` & `plex-api-client-0.5.0/src/plex_api/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,27 +70,30 @@
     Updates to the status can be observed via the Event API.
     """
 
     sdk_configuration: SDKConfiguration
 
     def __init__(self,
                  access_token: Union[str, Callable[[], str]],
+                 x_plex_client_identifier: str = None,
                  protocol: ServerProtocol = None,
                  ip: str = None,
                  port: str = None,
                  server_idx: Optional[int] = None,
                  server_url: Optional[str] = None,
                  url_params: Optional[Dict[str, str]] = None,
                  client: Optional[requests_http.Session] = None,
                  retry_config: Optional[utils.RetryConfig] = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
 
         :param access_token: The access_token required for authentication
         :type access_token: Union[str, Callable[[], str]]
+        :param x_plex_client_identifier: Configures the x_plex_client_identifier parameter for all supported operations
+        :type x_plex_client_identifier: str
         :param protocol: Allows setting the protocol variable for url substitution
         :type protocol: ServerProtocol
         :param ip: Allows setting the ip variable for url substitution
         :type ip: str
         :param port: Allows setting the port variable for url substitution
         :type port: str
         :param server_idx: The index of the server to use for all operations
@@ -119,21 +122,33 @@
         server_defaults = [
             {
                 'protocol': protocol or 'http',
                 'ip': ip or '10.10.10.47',
                 'port': port or '32400',
             },
         ]
+        global_params = {
+            'parameters': {
+                'queryParam': {
+                },
+                'pathParam': {
+                },
+                'header': {
+                    'x_plex_client_identifier': x_plex_client_identifier,
+                },
+            },
+        }
 
         self.sdk_configuration = SDKConfiguration(
             client,
             security,
             server_url,
             server_idx,
             server_defaults,
+            global_params,
             retry_config=retry_config
         )
 
         hooks = SDKHooks()
 
         current_server_url, *_ = self.sdk_configuration.get_server_details()
         server_url, self.sdk_configuration.client = hooks.sdk_init(current_server_url, self.sdk_configuration.client)
```

### Comparing `plex-api-client-0.4.3/src/plex_api/sdkconfiguration.py` & `plex-api-client-0.5.0/src/plex_api/sdkconfiguration.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
 from dataclasses import dataclass, field
 from enum import Enum
 from plex_api.models import components
-from typing import Callable, Dict, List, Tuple, Union
+from typing import Any, Callable, Dict, List, Tuple, Union
 
 
 SERVERS = [
     '{protocol}://{ip}:{port}',
     # The full address of your Plex Server
 ]
 """Contains the list of servers available to the SDK"""
@@ -26,19 +26,20 @@
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: str = ''
     server_idx: int = 0
     server_defaults: List[Dict[str, str]] = field(default_factory=List)
+    globals: Dict[str, Dict[str, Dict[str, Any]]] = field(default_factory=Dict)
     language: str = 'python'
     openapi_doc_version: str = '0.0.3'
-    sdk_version: str = '0.4.3'
-    gen_version: str = '2.291.0'
-    user_agent: str = 'speakeasy-sdk/python 0.4.3 2.291.0 0.0.3 plex-api-client'
+    sdk_version: str = '0.5.0'
+    gen_version: str = '2.292.0'
+    user_agent: str = 'speakeasy-sdk/python 0.5.0 2.292.0 0.0.3 plex-api-client'
     retry_config: RetryConfig = None
     _hooks: SDKHooks = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url:
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
```

### Comparing `plex-api-client-0.4.3/src/plex_api/search.py` & `plex-api-client-0.5.0/src/plex_api/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         url = base_url + '/hubs/search'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.PerformSearchRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.PerformSearchRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -113,15 +113,15 @@
         url = base_url + '/hubs/search/voice'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.PerformVoiceSearchRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.PerformVoiceSearchRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -178,15 +178,15 @@
         url = base_url + '/search'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetSearchResultsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetSearchResultsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx,
```

### Comparing `plex-api-client-0.4.3/src/plex_api/server.py` & `plex-api-client-0.5.0/src/plex_api/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -416,15 +416,15 @@
         url = base_url + '/photo/:/transcode'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetResizedPhotoRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetResizedPhotoRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx,
```

### Comparing `plex-api-client-0.4.3/src/plex_api/sessions.py` & `plex-api-client-0.5.0/src/plex_api/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         hook_ctx = HookContext(operation_id='stopTranscodeSession', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.StopTranscodeSessionRequest(
             session_key=session_key,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.StopTranscodeSessionRequest, base_url, '/transcode/sessions/{sessionKey}', request)
+        url = utils.generate_url(operations.StopTranscodeSessionRequest, base_url, '/transcode/sessions/{sessionKey}', request, self.sdk_configuration.globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
```

### Comparing `plex-api-client-0.4.3/src/plex_api/statistics.py` & `plex-api-client-0.5.0/src/plex_api/statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         url = base_url + '/statistics/media'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetStatisticsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetStatisticsRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx,
```

### Comparing `plex-api-client-0.4.3/src/plex_api/updater.py` & `plex-api-client-0.5.0/src/plex_api/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         url = base_url + '/updater/check'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.CheckForUpdatesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.CheckForUpdatesRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -163,15 +163,15 @@
         url = base_url + '/updater/apply'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ApplyUpdatesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.ApplyUpdatesRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx,
```

### Comparing `plex-api-client-0.4.3/src/plex_api/utils/retries.py` & `plex-api-client-0.5.0/src/plex_api/utils/retries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/utils/utils.py` & `plex-api-client-0.5.0/src/plex_api/utils/utils.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.4.3/src/plex_api/video.py` & `plex-api-client-0.5.0/src/plex_api/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         url = base_url + '/:/timeline'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetTimelineRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetTimelineRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx, 
@@ -86,15 +86,15 @@
         url = base_url + '/video/:/transcode/universal/start.mpd'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.StartUniversalTranscodeRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.StartUniversalTranscodeRequest, request, self.sdk_configuration.globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = self.sdk_configuration.get_hooks().before_request(
                 hook_ctx,
```

### Comparing `plex-api-client-0.4.3/src/plex_api_client.egg-info/PKG-INFO` & `plex-api-client-0.5.0/src/plex_api_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.4.3
+Version: 0.5.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
@@ -28,14 +28,15 @@
         ### Example
         
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
+            x_plex_client_identifier='<value>',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -167,14 +168,15 @@
         
         ```python
         import plex_api
         from plex_api.models import errors
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
+            x_plex_client_identifier='<value>',
         )
         
         
         res = None
         try:
             res = s.server.get_server_capabilities()
         except errors.GetServerCapabilitiesResponseBody as e:
@@ -206,14 +208,15 @@
         
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             server_idx=0,
             access_token="<YOUR_API_KEY_HERE>",
+            x_plex_client_identifier='<value>',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -233,14 +236,15 @@
         The default server can also be overridden globally by passing a URL to the `server_url: str` optional parameter when initializing the SDK client instance. For example:
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             server_url="{protocol}://{ip}:{port}",
             access_token="<YOUR_API_KEY_HERE>",
+            x_plex_client_identifier='<value>',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -250,18 +254,20 @@
         
         ### Override Server URL Per-Operation
         
         The server URL can also be overridden on a per-operation basis, provided a server list was specified for the operation. For example:
         ```python
         import plex_api
         
-        s = plex_api.PlexAPI()
+        s = plex_api.PlexAPI(
+            x_plex_client_identifier='<value>',
+        )
         
         
-        res = s.plex.get_pin(server_url="https://plex.tv/api/v2", x_plex_client_identifier='<value>', strong=False)
+        res = s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False, x_plex_client_identifier='<value>')
         
         if res.object is not None:
             # handle response
             pass
         
         ```
         <!-- End Server Selection [server] -->
@@ -295,26 +301,66 @@
         
         To authenticate with the API the `access_token` parameter must be set when initializing the SDK client instance. For example:
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
+            x_plex_client_identifier='<value>',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
         <!-- End Authentication [security] -->
         
+        <!-- Start Global Parameters [global-parameters] -->
+        ## Global Parameters
+        
+        A parameter is configured globally. This parameter must be set on the SDK client instance itself during initialization. When configured as an option during SDK initialization, This global value will be used as the default on the operations that use it. When such operations are called, there is a place in each to override the global value, if needed.
+        
+        For example, you can set `X-Plex-Client-Identifier` to `'<value>'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_pin`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
+        
+        
+        ### Available Globals
+        
+        The following global parameter is available. The required parameter must be set when you initialize the SDK client.
+        
+        | Name | Type | Required | Description |
+        | ---- | ---- |:--------:| ----------- |
+        | x_plex_client_identifier | str | ✔️ | The unique identifier for the client application
+        This is used to track the client application and its usage
+        (UUID, serial number, or other number unique per device)
+         |
+        
+        
+        ### Example
+        
+        ```python
+        import plex_api
+        
+        s = plex_api.PlexAPI(
+            x_plex_client_identifier='<value>',
+        )
+        
+        
+        res = s.plex.get_pin(strong=False, x_plex_client_identifier='<value>')
+        
+        if res.object is not None:
+            # handle response
+            pass
+        
+        ```
+        <!-- End Global Parameters [global-parameters] -->
+        
         <!-- Placeholder for Future Speakeasy SDK Sections -->
         
         # Development
         
         ## Maturity
         
         This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.4.3 Summary: Python
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.5.0 Summary: Python
 Client SDK Generated by Speakeasy Home-page: UNKNOWN Author: LukeHagar License:
 UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
-( access_token="", ) res = s.server.get_server_capabilities() if res.object is
-not None: # handle response pass ``` ## Available Resources and Operations ###
-[server](docs/sdks/server/README.md) * [get_server_capabilities](docs/sdks/
-server/README.md#get_server_capabilities) - Server Capabilities *
+( access_token="", x_plex_client_identifier='', ) res =
+s.server.get_server_capabilities() if res.object is not None: # handle response
+pass ``` ## Available Resources and Operations ### [server](docs/sdks/server/
+README.md) * [get_server_capabilities](docs/sdks/server/
+README.md#get_server_capabilities) - Server Capabilities *
 [get_server_preferences](docs/sdks/server/README.md#get_server_preferences) -
 Get Server Preferences * [get_available_clients](docs/sdks/server/
 README.md#get_available_clients) - Get Available Clients * [get_devices](docs/
 sdks/server/README.md#get_devices) - Get Devices * [get_server_identity](docs/
 sdks/server/README.md#get_server_identity) - Get Server Identity *
 [get_my_plex_account](docs/sdks/server/README.md#get_my_plex_account) - Get
 MyPlex Account * [get_resized_photo](docs/sdks/server/
@@ -96,61 +97,80 @@
 expectations. All operations return a response object or raise an error. If
 Error objects are specified in your OpenAPI Spec, the SDK will raise the
 appropriate Error type. | Error Object | Status Code | Content Type | | -------
 --------------------------------- | ---------------------------------------- |
 ---------------------------------------- | |
 errors.GetServerCapabilitiesResponseBody | 401 | application/json | |
 errors.SDKError | 4x-5xx | */* | ### Example ```python import plex_api from
-plex_api.models import errors s = plex_api.PlexAPI( access_token="", ) res =
-None try: res = s.server.get_server_capabilities() except
+plex_api.models import errors s = plex_api.PlexAPI( access_token="",
+x_plex_client_identifier='', ) res = None try: res =
+s.server.get_server_capabilities() except
 errors.GetServerCapabilitiesResponseBody as e: # handle exception raise(e)
 except errors.SDKError as e: # handle exception raise(e) if res.object is not
 None: # handle response pass ``` ## Server Selection ### Select Server by Index
 You can override the default server globally by passing a server index to the
 `server_idx: int` optional parameter when initializing the SDK client instance.
 The selected server will then be used as the default on the operations that use
 it. This table lists the indexes associated with the available servers: | # |
 Server | Variables | | - | ------ | --------- | | 0 | `{protocol}://{ip}:
 {port}` | `protocol` (default is `http`), `ip` (default is `10.10.10.47`),
 `port` (default is `32400`) | #### Example ```python import plex_api s =
-plex_api.PlexAPI( server_idx=0, access_token="", ) res =
-s.server.get_server_capabilities() if res.object is not None: # handle response
-pass ``` #### Variables Some of the server options above contain variables. If
-you want to set the values of those variables, the following optional
-parameters are available when initializing the SDK client instance: *
+plex_api.PlexAPI( server_idx=0, access_token="", x_plex_client_identifier='', )
+res = s.server.get_server_capabilities() if res.object is not None: # handle
+response pass ``` #### Variables Some of the server options above contain
+variables. If you want to set the values of those variables, the following
+optional parameters are available when initializing the SDK client instance: *
 `protocol: models.ServerProtocol` * `ip: str` * `port: str` ### Override Server
 URL Per-Client The default server can also be overridden globally by passing a
 URL to the `server_url: str` optional parameter when initializing the SDK
 client instance. For example: ```python import plex_api s = plex_api.PlexAPI
-( server_url="{protocol}://{ip}:{port}", access_token="", ) res =
+( server_url="{protocol}://{ip}:{port}", access_token="",
+x_plex_client_identifier='', ) res = s.server.get_server_capabilities() if
+res.object is not None: # handle response pass ``` ### Override Server URL Per-
+Operation The server URL can also be overridden on a per-operation basis,
+provided a server list was specified for the operation. For example: ```python
+import plex_api s = plex_api.PlexAPI( x_plex_client_identifier='', ) res =
+s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False,
+x_plex_client_identifier='') if res.object is not None: # handle response pass
+``` ## Custom HTTP Client The Python SDK makes API calls using the [requests]
+(https://pypi.org/project/requests/) HTTP library. In order to provide a
+convenient way to configure timeouts, cookies, proxies, custom headers, and
+other low-level configuration, you can initialize the SDK client with a custom
+`requests.Session` object. For example, you could specify a header for every
+request that this sdk makes as follows: ```python import plex_api import
+requests http_client = requests.Session() http_client.headers.update({'x-
+custom-header': 'someValue'}) s = plex_api.PlexAPI(client: http_client) ``` ##
+Authentication ### Per-Client Security Schemes This SDK supports the following
+security scheme globally: | Name | Type | Scheme | | -------------- | ---------
+----- | -------------- | | `access_token` | apiKey | API key | To authenticate
+with the API the `access_token` parameter must be set when initializing the SDK
+client instance. For example: ```python import plex_api s = plex_api.PlexAPI
+( access_token="", x_plex_client_identifier='', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
-pass ``` ### Override Server URL Per-Operation The server URL can also be
-overridden on a per-operation basis, provided a server list was specified for
-the operation. For example: ```python import plex_api s = plex_api.PlexAPI()
-res = s.plex.get_pin(server_url="https://plex.tv/api/v2",
-x_plex_client_identifier='', strong=False) if res.object is not None: # handle
-response pass ``` ## Custom HTTP Client The Python SDK makes API calls using
-the [requests](https://pypi.org/project/requests/) HTTP library. In order to
-provide a convenient way to configure timeouts, cookies, proxies, custom
-headers, and other low-level configuration, you can initialize the SDK client
-with a custom `requests.Session` object. For example, you could specify a
-header for every request that this sdk makes as follows: ```python import
-plex_api import requests http_client = requests.Session()
-http_client.headers.update({'x-custom-header': 'someValue'}) s =
-plex_api.PlexAPI(client: http_client) ``` ## Authentication ### Per-Client
-Security Schemes This SDK supports the following security scheme globally: |
-Name | Type | Scheme | | -------------- | -------------- | -------------- | |
-`access_token` | apiKey | API key | To authenticate with the API the
-`access_token` parameter must be set when initializing the SDK client instance.
-For example: ```python import plex_api s = plex_api.PlexAPI( access_token="", )
-res = s.server.get_server_capabilities() if res.object is not None: # handle
-response pass ``` # Development ## Maturity This SDK is in beta, and there may
-be breaking changes between versions without a major version update. Therefore,
-we recommend pinning usage to a specific package version. This way, you can
-install the same version each time without breaking changes unless you are
-intentionally looking for the latest version. ## Contributions While we value
-open-source contributions to this SDK, this library is generated
+pass ``` ## Global Parameters A parameter is configured globally. This
+parameter must be set on the SDK client instance itself during initialization.
+When configured as an option during SDK initialization, This global value will
+be used as the default on the operations that use it. When such operations are
+called, there is a place in each to override the global value, if needed. For
+example, you can set `X-Plex-Client-Identifier` to `''` at SDK initialization
+and then you do not have to pass the same value on calls to operations like
+`get_pin`. But if you want to do so you may, which will locally override the
+global setting. See the example code below for a demonstration. ### Available
+Globals The following global parameter is available. The required parameter
+must be set when you initialize the SDK client. | Name | Type | Required |
+Description | | ---- | ---- |:--------:| ----------- | |
+x_plex_client_identifier | str | âï¸ | The unique identifier for the client
+application This is used to track the client application and its usage (UUID,
+serial number, or other number unique per device) | ### Example ```python
+import plex_api s = plex_api.PlexAPI( x_plex_client_identifier='', ) res =
+s.plex.get_pin(strong=False, x_plex_client_identifier='') if res.object is not
+None: # handle response pass ``` # Development ## Maturity This SDK is in beta,
+and there may be breaking changes between versions without a major version
+update. Therefore, we recommend pinning usage to a specific package version.
+This way, you can install the same version each time without breaking changes
+unless you are intentionally looking for the latest version. ## Contributions
+While we value open-source contributions to this SDK, this library is generated
 programmatically. Feel free to open a PR or a Github issue as a proof of
 concept and we'll do our best to include it in a future release! ### SDK
 Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
 client-sdks) Platform: UNKNOWN Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: dev
```

### Comparing `plex-api-client-0.4.3/src/plex_api_client.egg-info/SOURCES.txt` & `plex-api-client-0.5.0/src/plex_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

