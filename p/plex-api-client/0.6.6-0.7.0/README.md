# Comparing `tmp/plex-api-client-0.6.6.tar.gz` & `tmp/plex-api-client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-api-client-0.6.6.tar", last modified: Wed May  8 18:16:45 2024, max compression
+gzip compressed data, was "plex-api-client-0.7.0.tar", last modified: Thu May 23 15:59:01 2024, max compression
```

## Comparing `plex-api-client-0.6.6.tar` & `plex-api-client-0.7.0.tar`

### file list

```diff
@@ -1,172 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:45.833995 plex-api-client-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 18:16:36.000000 plex-api-client-0.6.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-05-08 18:16:45.833995 plex-api-client-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14178 2024-05-08 18:16:36.000000 plex-api-client-0.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:16:45.833995 plex-api-client-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:45.801995 plex-api-client-0.6.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:45.805995 plex-api-client-0.6.6/src/plex_api/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:45.805995 plex-api-client-0.6.6/src/plex_api/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/hubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42185 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:45.805995 plex-api-client-0.6.6/src/plex_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:45.809995 plex-api-client-0.6.6/src/plex_api/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:45.817995 plex-api-client-0.6.6/src/plex_api/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/errors/uploadplaylist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:45.817995 plex-api-client-0.6.6/src/plex_api/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:45.829995 plex-api-client-0.6.6/src/plex_api/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21445 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getlibraryitems.py
--rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/searchlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/models/operations/uploadplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    33949 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/plex.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    28000 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:45.829995 plex-api-client-0.6.6/src/plex_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-05-08 18:16:37.000000 plex-api-client-0.6.6/src/plex_api/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:45.829995 plex-api-client-0.6.6/src/plex_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-05-08 18:16:45.000000 plex-api-client-0.6.6/src/plex_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-08 18:16:45.000000 plex-api-client-0.6.6/src/plex_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:16:45.000000 plex-api-client-0.6.6/src/plex_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-08 18:16:45.000000 plex-api-client-0.6.6/src/plex_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 18:16:45.000000 plex-api-client-0.6.6/src/plex_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.773991 plex-api-client-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20824 2024-05-23 15:59:01.773991 plex-api-client-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:59:01.773991 plex-api-client-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.749991 plex-api-client-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.753991 plex-api-client-0.7.0/src/plex_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.753991 plex-api-client-0.7.0/src/plex_api/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18356 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/hubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38654 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.753991 plex-api-client-0.7.0/src/plex_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.753991 plex-api-client-0.7.0/src/plex_api/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.761991 plex-api-client-0.7.0/src/plex_api/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/errors/uploadplaylist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.761991 plex-api-client-0.7.0/src/plex_api/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.773991 plex-api-client-0.7.0/src/plex_api/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/searchlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/models/operations/uploadplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34579 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/plex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13494 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28675 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11002 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.773991 plex-api-client-0.7.0/src/plex_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-23 15:58:53.000000 plex-api-client-0.7.0/src/plex_api/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:01.773991 plex-api-client-0.7.0/src/plex_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20824 2024-05-23 15:59:01.000000 plex-api-client-0.7.0/src/plex_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-23 15:59:01.000000 plex-api-client-0.7.0/src/plex_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:59:01.000000 plex-api-client-0.7.0/src/plex_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-23 15:59:01.000000 plex-api-client-0.7.0/src/plex_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 15:59:01.000000 plex-api-client-0.7.0/src/plex_api_client.egg-info/top_level.txt
```

### Comparing `plex-api-client-0.6.6/LICENSE.md` & `plex-api-client-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/PKG-INFO` & `plex-api-client-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.6.6
+Version: 0.7.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/LukeHagar/plexpy.git
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
@@ -31,15 +31,14 @@
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
-        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -97,15 +96,14 @@
         ### [library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md)
         
         * [get_file_hash](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_file_hash) - Get Hash Value
         * [get_recently_added](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_recently_added) - Get Recently Added
         * [get_libraries](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_libraries) - Get All Libraries
         * [get_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_library) - Get Library Details
         * [delete_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#delete_library) - Delete Library Section
-        * [get_library_items](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_library_items) - Get Library Items
         * [refresh_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#refresh_library) - Refresh Library
         * [search_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#search_library) - Search Library
         * [get_metadata](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_metadata) - Get Items Metadata
         * [get_metadata_children](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_metadata_children) - Get Items Children
         * [get_on_deck](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_on_deck) - Get On Deck
         
         ### [log](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/log/README.md)
@@ -171,15 +169,14 @@
         from plex_api.models import errors
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
-        
         res = None
         try:
             res = s.server.get_server_capabilities()
         except errors.GetServerCapabilitiesResponseBody as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
@@ -211,15 +208,14 @@
         
         s = plex_api.PlexAPI(
             server_idx=0,
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
-        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -239,15 +235,14 @@
         
         s = plex_api.PlexAPI(
             server_url="{protocol}://{ip}:{port}",
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
-        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -258,16 +253,15 @@
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             x_plex_client_identifier='Postman',
         )
         
-        
-        res = s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False, x_plex_client_identifier='Postman')
+        res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman', server_url="https://plex.tv/api/v2")
         
         if res.object is not None:
             # handle response
             pass
         
         ```
         <!-- End Server Selection [server] -->
@@ -304,15 +298,14 @@
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
-        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -343,15 +336,14 @@
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             x_plex_client_identifier='Postman',
         )
         
-        
         res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman')
         
         if res.object is not None:
             # handle response
             pass
         
         ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.6 Summary: Python
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.7.0 Summary: Python
 Client SDK Generated by Speakeasy Home-page: https://github.com/LukeHagar/
 plexpy.git Author: LukeHagar License: UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
@@ -71,17 +71,15 @@
 //github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#get_recently_added) - Get Recently Added * [get_libraries](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#get_libraries) - Get All Libraries * [get_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#get_library) - Get Library Details * [delete_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
-README.md#delete_library) - Delete Library Section * [get_library_items](https:
-//github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
-README.md#get_library_items) - Get Library Items * [refresh_library](https://
+README.md#delete_library) - Delete Library Section * [refresh_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#refresh_library) - Refresh Library * [search_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#search_library) - Search Library * [get_metadata](https://github.com/
 LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_metadata) - Get
 Items Metadata * [get_metadata_children](https://github.com/LukeHagar/plexpy/
 blob/master/docs/sdks/library/README.md#get_metadata_children) - Get Items
@@ -172,16 +170,16 @@
 optional parameter when initializing the SDK client instance. For example:
 ```python import plex_api s = plex_api.PlexAPI( server_url="{protocol}://{ip}:
 {port}", access_token="", x_plex_client_identifier='Postman', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
 pass ``` ### Override Server URL Per-Operation The server URL can also be
 overridden on a per-operation basis, provided a server list was specified for
 the operation. For example: ```python import plex_api s = plex_api.PlexAPI
-( x_plex_client_identifier='Postman', ) res = s.plex.get_pin(server_url="https:
-//plex.tv/api/v2", strong=False, x_plex_client_identifier='Postman') if
+( x_plex_client_identifier='Postman', ) res = s.plex.get_pin(strong=False,
+x_plex_client_identifier='Postman', server_url="https://plex.tv/api/v2") if
 res.object is not None: # handle response pass ``` ## Custom HTTP Client The
 Python SDK makes API calls using the [requests](https://pypi.org/project/
 requests/) HTTP library. In order to provide a convenient way to configure
 timeouts, cookies, proxies, custom headers, and other low-level configuration,
 you can initialize the SDK client with a custom `requests.Session` object. For
 example, you could specify a header for every request that this sdk makes as
 follows: ```python import plex_api import requests http_client =
```

### Comparing `plex-api-client-0.6.6/README.md` & `plex-api-client-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 import plex_api
 
 s = plex_api.PlexAPI(
     access_token="<YOUR_API_KEY_HERE>",
     x_plex_client_identifier='Postman',
 )
 
-
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
     pass
 
 ```
@@ -90,15 +89,14 @@
 ### [library](docs/sdks/library/README.md)
 
 * [get_file_hash](docs/sdks/library/README.md#get_file_hash) - Get Hash Value
 * [get_recently_added](docs/sdks/library/README.md#get_recently_added) - Get Recently Added
 * [get_libraries](docs/sdks/library/README.md#get_libraries) - Get All Libraries
 * [get_library](docs/sdks/library/README.md#get_library) - Get Library Details
 * [delete_library](docs/sdks/library/README.md#delete_library) - Delete Library Section
-* [get_library_items](docs/sdks/library/README.md#get_library_items) - Get Library Items
 * [refresh_library](docs/sdks/library/README.md#refresh_library) - Refresh Library
 * [search_library](docs/sdks/library/README.md#search_library) - Search Library
 * [get_metadata](docs/sdks/library/README.md#get_metadata) - Get Items Metadata
 * [get_metadata_children](docs/sdks/library/README.md#get_metadata_children) - Get Items Children
 * [get_on_deck](docs/sdks/library/README.md#get_on_deck) - Get On Deck
 
 ### [log](docs/sdks/log/README.md)
@@ -164,15 +162,14 @@
 from plex_api.models import errors
 
 s = plex_api.PlexAPI(
     access_token="<YOUR_API_KEY_HERE>",
     x_plex_client_identifier='Postman',
 )
 
-
 res = None
 try:
     res = s.server.get_server_capabilities()
 except errors.GetServerCapabilitiesResponseBody as e:
     # handle exception
     raise(e)
 except errors.SDKError as e:
@@ -204,15 +201,14 @@
 
 s = plex_api.PlexAPI(
     server_idx=0,
     access_token="<YOUR_API_KEY_HERE>",
     x_plex_client_identifier='Postman',
 )
 
-
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
     pass
 
 ```
@@ -232,15 +228,14 @@
 
 s = plex_api.PlexAPI(
     server_url="{protocol}://{ip}:{port}",
     access_token="<YOUR_API_KEY_HERE>",
     x_plex_client_identifier='Postman',
 )
 
-
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
     pass
 
 ```
@@ -251,16 +246,15 @@
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
     x_plex_client_identifier='Postman',
 )
 
-
-res = s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False, x_plex_client_identifier='Postman')
+res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman', server_url="https://plex.tv/api/v2")
 
 if res.object is not None:
     # handle response
     pass
 
 ```
 <!-- End Server Selection [server] -->
@@ -297,15 +291,14 @@
 import plex_api
 
 s = plex_api.PlexAPI(
     access_token="<YOUR_API_KEY_HERE>",
     x_plex_client_identifier='Postman',
 )
 
-
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
     pass
 
 ```
@@ -336,15 +329,14 @@
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
     x_plex_client_identifier='Postman',
 )
 
-
 res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman')
 
 if res.object is not None:
     # handle response
     pass
 
 ```
```

#### html2text {}

```diff
@@ -44,35 +44,34 @@
 [get_search_results](docs/sdks/search/README.md#get_search_results) - Get
 Search Results ### [library](docs/sdks/library/README.md) * [get_file_hash]
 (docs/sdks/library/README.md#get_file_hash) - Get Hash Value *
 [get_recently_added](docs/sdks/library/README.md#get_recently_added) - Get
 Recently Added * [get_libraries](docs/sdks/library/README.md#get_libraries) -
 Get All Libraries * [get_library](docs/sdks/library/README.md#get_library) -
 Get Library Details * [delete_library](docs/sdks/library/
-README.md#delete_library) - Delete Library Section * [get_library_items](docs/
-sdks/library/README.md#get_library_items) - Get Library Items *
-[refresh_library](docs/sdks/library/README.md#refresh_library) - Refresh
-Library * [search_library](docs/sdks/library/README.md#search_library) - Search
-Library * [get_metadata](docs/sdks/library/README.md#get_metadata) - Get Items
-Metadata * [get_metadata_children](docs/sdks/library/
-README.md#get_metadata_children) - Get Items Children * [get_on_deck](docs/
-sdks/library/README.md#get_on_deck) - Get On Deck ### [log](docs/sdks/log/
-README.md) * [log_line](docs/sdks/log/README.md#log_line) - Logging a single
-line message. * [log_multi_line](docs/sdks/log/README.md#log_multi_line) -
-Logging a multi-line message * [enable_paper_trail](docs/sdks/log/
-README.md#enable_paper_trail) - Enabling Papertrail ### [plex](docs/sdks/plex/
-README.md) * [get_pin](docs/sdks/plex/README.md#get_pin) - Get a Pin *
-[get_token](docs/sdks/plex/README.md#get_token) - Get Access Token ###
-[playlists](docs/sdks/playlists/README.md) * [create_playlist](docs/sdks/
-playlists/README.md#create_playlist) - Create a Playlist * [get_playlists]
-(docs/sdks/playlists/README.md#get_playlists) - Get All Playlists *
-[get_playlist](docs/sdks/playlists/README.md#get_playlist) - Retrieve Playlist
-* [delete_playlist](docs/sdks/playlists/README.md#delete_playlist) - Deletes a
-Playlist * [update_playlist](docs/sdks/playlists/README.md#update_playlist) -
-Update a Playlist * [get_playlist_contents](docs/sdks/playlists/
+README.md#delete_library) - Delete Library Section * [refresh_library](docs/
+sdks/library/README.md#refresh_library) - Refresh Library * [search_library]
+(docs/sdks/library/README.md#search_library) - Search Library * [get_metadata]
+(docs/sdks/library/README.md#get_metadata) - Get Items Metadata *
+[get_metadata_children](docs/sdks/library/README.md#get_metadata_children) -
+Get Items Children * [get_on_deck](docs/sdks/library/README.md#get_on_deck) -
+Get On Deck ### [log](docs/sdks/log/README.md) * [log_line](docs/sdks/log/
+README.md#log_line) - Logging a single line message. * [log_multi_line](docs/
+sdks/log/README.md#log_multi_line) - Logging a multi-line message *
+[enable_paper_trail](docs/sdks/log/README.md#enable_paper_trail) - Enabling
+Papertrail ### [plex](docs/sdks/plex/README.md) * [get_pin](docs/sdks/plex/
+README.md#get_pin) - Get a Pin * [get_token](docs/sdks/plex/
+README.md#get_token) - Get Access Token ### [playlists](docs/sdks/playlists/
+README.md) * [create_playlist](docs/sdks/playlists/README.md#create_playlist) -
+Create a Playlist * [get_playlists](docs/sdks/playlists/
+README.md#get_playlists) - Get All Playlists * [get_playlist](docs/sdks/
+playlists/README.md#get_playlist) - Retrieve Playlist * [delete_playlist](docs/
+sdks/playlists/README.md#delete_playlist) - Deletes a Playlist *
+[update_playlist](docs/sdks/playlists/README.md#update_playlist) - Update a
+Playlist * [get_playlist_contents](docs/sdks/playlists/
 README.md#get_playlist_contents) - Retrieve Playlist Contents *
 [clear_playlist_contents](docs/sdks/playlists/
 README.md#clear_playlist_contents) - Delete Playlist Contents *
 [add_playlist_contents](docs/sdks/playlists/README.md#add_playlist_contents) -
 Adding to a Playlist * [upload_playlist](docs/sdks/playlists/
 README.md#upload_playlist) - Upload Playlist ### [authentication](docs/sdks/
 authentication/README.md) * [get_transient_token](docs/sdks/authentication/
@@ -123,16 +122,16 @@
 optional parameter when initializing the SDK client instance. For example:
 ```python import plex_api s = plex_api.PlexAPI( server_url="{protocol}://{ip}:
 {port}", access_token="", x_plex_client_identifier='Postman', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
 pass ``` ### Override Server URL Per-Operation The server URL can also be
 overridden on a per-operation basis, provided a server list was specified for
 the operation. For example: ```python import plex_api s = plex_api.PlexAPI
-( x_plex_client_identifier='Postman', ) res = s.plex.get_pin(server_url="https:
-//plex.tv/api/v2", strong=False, x_plex_client_identifier='Postman') if
+( x_plex_client_identifier='Postman', ) res = s.plex.get_pin(strong=False,
+x_plex_client_identifier='Postman', server_url="https://plex.tv/api/v2") if
 res.object is not None: # handle response pass ``` ## Custom HTTP Client The
 Python SDK makes API calls using the [requests](https://pypi.org/project/
 requests/) HTTP library. In order to provide a convenient way to configure
 timeouts, cookies, proxies, custom headers, and other low-level configuration,
 you can initialize the SDK client with a custom `requests.Session` object. For
 example, you could specify a header for every request that this sdk makes as
 follows: ```python import plex_api import requests http_client =
```

### Comparing `plex-api-client-0.6.6/setup.py` & `plex-api-client-0.7.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='plex-api-client',
-    version='0.6.6',
+    version='0.7.0',
     author='LukeHagar',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/LukeHagar/plexpy.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `plex-api-client-0.6.6/src/plex_api/_hooks/registration.py` & `plex-api-client-0.7.0/src/plex_api/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/_hooks/sdkhooks.py` & `plex-api-client-0.7.0/src/plex_api/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/_hooks/types.py` & `plex-api-client-0.7.0/src/plex_api/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/activities.py` & `plex-api-client-0.7.0/src/plex_api/activities.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,23 +60,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetServerActivitiesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetServerActivitiesResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetServerActivitiesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -132,14 +134,15 @@
         res = operations.CancelServerActivitiesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.CancelServerActivitiesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/authentication.py` & `plex-api-client-0.7.0/src/plex_api/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         res = operations.GetTransientTokenResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetTransientTokenResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -127,14 +128,15 @@
         res = operations.GetSourceConnectionInformationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetSourceConnectionInformationResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/butler.py` & `plex-api-client-0.7.0/src/plex_api/butler.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,23 +53,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetButlerTasksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetButlerTasksResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetButlerTasksResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -125,14 +127,15 @@
         res = operations.StartAllTasksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.StartAllTasksResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -184,14 +187,15 @@
         res = operations.StopAllTasksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.StopAllTasksResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -251,14 +255,15 @@
         res = operations.StartTaskResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code in [200, 202]:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.StartTaskResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -314,14 +319,15 @@
         res = operations.StopTaskResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code == 404 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.StopTaskResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/hubs.py` & `plex-api-client-0.7.0/src/plex_api/hubs.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,23 +59,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetGlobalHubsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetGlobalHubsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetGlobalHubsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -130,23 +132,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetLibraryHubsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetLibraryHubsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetLibraryHubsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/library.py` & `plex-api-client-0.7.0/src/plex_api/library.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         res = operations.GetFileHashResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetFileHashResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -118,23 +119,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetRecentlyAddedResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetRecentlyAddedResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetRecentlyAddedResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -187,23 +190,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetLibrariesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetLibrariesResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetLibrariesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -295,23 +300,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetLibraryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetLibraryResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetLibraryResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -367,108 +374,29 @@
         res = operations.DeleteLibraryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.DeleteLibraryResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_library_items(self, section_id: int, tag: operations.Tag) -> operations.GetLibraryItemsResponse:
-        r"""Get Library Items
-        Fetches details from a specific section of the library identified by a section key and a tag. The tag parameter accepts the following values:
-        - `all`: All items in the section.
-        - `unwatched`: Items that have not been played.
-        - `newest`: Items that are recently released.
-        - `recentlyAdded`: Items that are recently added to the library.
-        - `recentlyViewed`: Items that were recently viewed.
-        - `onDeck`: Items to continue watching.
-        - `collection`: Items categorized by collection.
-        - `edition`: Items categorized by edition.
-        - `genre`: Items categorized by genre.
-        - `year`: Items categorized by year of release.
-        - `decade`: Items categorized by decade.
-        - `director`: Items categorized by director.
-        - `actor`: Items categorized by starring actor.
-        - `country`: Items categorized by country of origin.
-        - `contentRating`: Items categorized by content rating.
-        - `rating`: Items categorized by rating.
-        - `resolution`: Items categorized by resolution.
-        - `firstCharacter`: Items categorized by the first letter.
-        - `folder`: Items categorized by folder.
-        """
-        hook_ctx = HookContext(operation_id='getLibraryItems', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetLibraryItemsRequest(
-            section_id=section_id,
-            tag=tag,
-        )
-        
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(base_url, '/library/sections/{sectionId}/{tag}', request)
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        res = operations.GetLibraryItemsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetLibraryItemsResponseBody])
-                res.object = out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-        return res
-
-    
-    
     def refresh_library(self, section_id: float) -> operations.RefreshLibraryResponse:
         r"""Refresh Library
         This endpoint Refreshes the library.
         """
         hook_ctx = HookContext(operation_id='refreshLibrary', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.RefreshLibraryRequest(
             section_id=section_id,
@@ -510,14 +438,15 @@
         res = operations.RefreshLibraryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.RefreshLibraryResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -588,14 +517,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.SearchLibraryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.SearchLibraryResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -648,23 +578,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetMetadataResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetMetadataResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetMetadataResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -716,23 +648,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetMetadataChildrenResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetMetadataChildrenResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetMetadataChildrenResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -780,23 +714,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetOnDeckResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetOnDeckResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetOnDeckResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/log.py` & `plex-api-client-0.7.0/src/plex_api/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         res = operations.LogLineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.LogLineResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -147,14 +148,15 @@
         res = operations.LogMultiLineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.LogMultiLineResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -206,14 +208,15 @@
         res = operations.EnablePaperTrailResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code == 403 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.EnablePaperTrailResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/media.py` & `plex-api-client-0.7.0/src/plex_api/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         res = operations.MarkPlayedResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.MarkPlayedResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -125,14 +126,15 @@
         res = operations.MarkUnplayedResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.MarkUnplayedResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -191,14 +193,15 @@
         res = operations.UpdatePlayProgressResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.UpdatePlayProgressResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/__init__.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/addplaylistcontents.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/applyupdates.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/applyupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/cancelserveractivities.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/checkforupdates.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/checkforupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/clearplaylistcontents.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/createplaylist.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/createplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/deletelibrary.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/deleteplaylist.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/enablepapertrail.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getavailableclients.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getbutlertasks.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getdevices.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getfilehash.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getglobalhubs.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getglobalhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getlibraries.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getlibrary.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getlibraryhubs.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getlibraryhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getmetadata.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getmetadatachildren.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getmyplexaccount.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getondeck.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getondeck.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getpin.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getpin.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getplaylist.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getplaylistcontents.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getplaylists.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getplaylists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getrecentlyadded.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getrecentlyadded.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getresizedphoto.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getresizedphoto.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getsearchresults.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getsearchresults.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getserveractivities.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getservercapabilities.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getservercapabilities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getserveridentity.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getserverlist.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getserverpreferences.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getsessionhistory.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getsessions.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getsourceconnectioninformation.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getstatistics.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/gettimeline.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/gettimeline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/gettoken.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/gettoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/gettranscodesessions.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/gettranscodesessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/gettransienttoken.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/gettransienttoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/getupdatestatus.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/logline.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/logline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/logmultiline.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/markplayed.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/markunplayed.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/performsearch.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/performvoicesearch.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/refreshlibrary.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/sdkerror.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/startalltasks.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/starttask.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/starttask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/startuniversaltranscode.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/stopalltasks.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/stoptask.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/stoptask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/stoptranscodesession.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/updateplaylist.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/updateplayprogress.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/errors/uploadplaylist.py` & `plex-api-client-0.7.0/src/plex_api/models/errors/uploadplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/internal/globals.py` & `plex-api-client-0.7.0/src/plex_api/models/internal/globals.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/__init__.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from .getbutlertasks import *
 from .getdevices import *
 from .getfilehash import *
 from .getglobalhubs import *
 from .getlibraries import *
 from .getlibrary import *
 from .getlibraryhubs import *
-from .getlibraryitems import *
 from .getmetadata import *
 from .getmetadatachildren import *
 from .getmyplexaccount import *
 from .getondeck import *
 from .getpin import *
 from .getplaylist import *
 from .getplaylistcontents import *
@@ -57,8 +56,8 @@
 from .stopalltasks import *
 from .stoptask import *
 from .stoptranscodesession import *
 from .updateplaylist import *
 from .updateplayprogress import *
 from .uploadplaylist import *
 
-__all__ = ["Account","Activity","AddPlaylistContentsMediaContainer","AddPlaylistContentsMetadata","AddPlaylistContentsRequest","AddPlaylistContentsResponse","AddPlaylistContentsResponseBody","ApplyUpdatesRequest","ApplyUpdatesResponse","ButlerTask","ButlerTasks","CancelServerActivitiesRequest","CancelServerActivitiesResponse","CheckForUpdatesRequest","CheckForUpdatesResponse","ClearPlaylistContentsRequest","ClearPlaylistContentsResponse","Context","Country","CreatePlaylistMediaContainer","CreatePlaylistMetadata","CreatePlaylistRequest","CreatePlaylistResponse","CreatePlaylistResponseBody","DeleteLibraryRequest","DeleteLibraryResponse","DeletePlaylistRequest","DeletePlaylistResponse","Device","Director","Directory","Download","EnablePaperTrailResponse","Field","FieldType","Filter","Force","GET_PIN_SERVERS","GET_TOKEN_SERVERS","Genre","GetAvailableClientsMediaContainer","GetAvailableClientsResponse","GetAvailableClientsResponseBody","GetButlerTasksResponse","GetButlerTasksResponseBody","GetDevicesMediaContainer","GetDevicesResponse","GetDevicesResponseBody","GetFileHashRequest","GetFileHashResponse","GetGlobalHubsMediaContainer","GetGlobalHubsMetadata","GetGlobalHubsRequest","GetGlobalHubsResponse","GetGlobalHubsResponseBody","GetLibrariesDirectory","GetLibrariesLocation","GetLibrariesMediaContainer","GetLibrariesResponse","GetLibrariesResponseBody","GetLibraryDirectory","GetLibraryHubsCountry","GetLibraryHubsDirector","GetLibraryHubsGenre","GetLibraryHubsHub","GetLibraryHubsMedia","GetLibraryHubsMediaContainer","GetLibraryHubsMetadata","GetLibraryHubsPart","GetLibraryHubsRequest","GetLibraryHubsResponse","GetLibraryHubsResponseBody","GetLibraryHubsRole","GetLibraryHubsWriter","GetLibraryItemsCountry","GetLibraryItemsDirector","GetLibraryItemsGenre","GetLibraryItemsMedia","GetLibraryItemsMediaContainer","GetLibraryItemsMetadata","GetLibraryItemsPart","GetLibraryItemsRequest","GetLibraryItemsResponse","GetLibraryItemsResponseBody","GetLibraryItemsRole","GetLibraryItemsWriter","GetLibraryMediaContainer","GetLibraryRequest","GetLibraryResponse","GetLibraryResponseBody","GetLibraryType","GetMetadataChildrenDirectory","GetMetadataChildrenMediaContainer","GetMetadataChildrenMetadata","GetMetadataChildrenRequest","GetMetadataChildrenResponse","GetMetadataChildrenResponseBody","GetMetadataCountry","GetMetadataDirector","GetMetadataGenre","GetMetadataMedia","GetMetadataMediaContainer","GetMetadataMetadata","GetMetadataPart","GetMetadataRequest","GetMetadataResponse","GetMetadataResponseBody","GetMetadataRole","GetMetadataWriter","GetMyPlexAccountResponse","GetMyPlexAccountResponseBody","GetOnDeckGuids","GetOnDeckMedia","GetOnDeckMediaContainer","GetOnDeckMetadata","GetOnDeckPart","GetOnDeckResponse","GetOnDeckResponseBody","GetOnDeckStream","GetPinGlobals","GetPinRequest","GetPinResponse","GetPinResponseBody","GetPlaylistContentsCountry","GetPlaylistContentsDirector","GetPlaylistContentsGenre","GetPlaylistContentsMedia","GetPlaylistContentsMediaContainer","GetPlaylistContentsMetadata","GetPlaylistContentsPart","GetPlaylistContentsRequest","GetPlaylistContentsResponse","GetPlaylistContentsResponseBody","GetPlaylistContentsRole","GetPlaylistContentsWriter","GetPlaylistMediaContainer","GetPlaylistMetadata","GetPlaylistRequest","GetPlaylistResponse","GetPlaylistResponseBody","GetPlaylistsMediaContainer","GetPlaylistsMetadata","GetPlaylistsRequest","GetPlaylistsResponse","GetPlaylistsResponseBody","GetRecentlyAddedMediaContainer","GetRecentlyAddedResponse","GetRecentlyAddedResponseBody","GetResizedPhotoRequest","GetResizedPhotoResponse","GetSearchResultsCountry","GetSearchResultsDirector","GetSearchResultsGenre","GetSearchResultsMedia","GetSearchResultsMediaContainer","GetSearchResultsMetadata","GetSearchResultsPart","GetSearchResultsRequest","GetSearchResultsResponse","GetSearchResultsResponseBody","GetSearchResultsRole","GetSearchResultsWriter","GetServerActivitiesMediaContainer","GetServerActivitiesResponse","GetServerActivitiesResponseBody","GetServerCapabilitiesResponse","GetServerCapabilitiesResponseBody","GetServerIdentityMediaContainer","GetServerIdentityResponse","GetServerIdentityResponseBody","GetServerListMediaContainer","GetServerListResponse","GetServerListResponseBody","GetServerListServer","GetServerPreferencesMediaContainer","GetServerPreferencesResponse","GetServerPreferencesResponseBody","GetSessionHistoryMediaContainer","GetSessionHistoryMetadata","GetSessionHistoryResponse","GetSessionHistoryResponseBody","GetSessionsMedia","GetSessionsMediaContainer","GetSessionsMetadata","GetSessionsPart","GetSessionsResponse","GetSessionsResponseBody","GetSessionsStream","GetSourceConnectionInformationRequest","GetSourceConnectionInformationResponse","GetStatisticsDevice","GetStatisticsMediaContainer","GetStatisticsRequest","GetStatisticsResponse","GetStatisticsResponseBody","GetTimelineRequest","GetTimelineResponse","GetTokenGlobals","GetTokenRequest","GetTokenResponse","GetTranscodeSessionsMediaContainer","GetTranscodeSessionsResponse","GetTranscodeSessionsResponseBody","GetTransientTokenQueryParamType","GetTransientTokenRequest","GetTransientTokenResponse","GetUpdateStatusMediaContainer","GetUpdateStatusResponse","GetUpdateStatusResponseBody","Guids","Hub","IncludeDetails","Level","Location","LogLineRequest","LogLineResponse","LogMultiLineResponse","MarkPlayedRequest","MarkPlayedResponse","MarkUnplayedRequest","MarkUnplayedResponse","Media","MediaContainer","Metadata","MinSize","MyPlex","OnlyTransient","Operator","Part","PathParamTaskName","PerformSearchRequest","PerformSearchResponse","PerformVoiceSearchRequest","PerformVoiceSearchResponse","Player","PlaylistType","Producer","Provider","QueryParamOnlyTransient","QueryParamSmart","QueryParamType","Ratings","RefreshLibraryRequest","RefreshLibraryResponse","Release","Role","Scope","SearchLibraryMediaContainer","SearchLibraryMetadata","SearchLibraryRequest","SearchLibraryResponse","SearchLibraryResponseBody","Server","Session","Setting","Skip","Smart","Sort","StartAllTasksResponse","StartTaskRequest","StartTaskResponse","StartUniversalTranscodeRequest","StartUniversalTranscodeResponse","State","StatisticsMedia","StopAllTasksResponse","StopTaskRequest","StopTaskResponse","StopTranscodeSessionRequest","StopTranscodeSessionResponse","Stream","Tag","TaskName","Tonight","TranscodeSession","Type","UpdatePlayProgressRequest","UpdatePlayProgressResponse","UpdatePlaylistRequest","UpdatePlaylistResponse","UploadPlaylistRequest","UploadPlaylistResponse","Upscale","User","Writer"]
+__all__ = ["Account","Activity","AddPlaylistContentsMediaContainer","AddPlaylistContentsMetadata","AddPlaylistContentsRequest","AddPlaylistContentsResponse","AddPlaylistContentsResponseBody","ApplyUpdatesRequest","ApplyUpdatesResponse","ButlerTask","ButlerTasks","CancelServerActivitiesRequest","CancelServerActivitiesResponse","CheckForUpdatesRequest","CheckForUpdatesResponse","ClearPlaylistContentsRequest","ClearPlaylistContentsResponse","Context","Country","CreatePlaylistMediaContainer","CreatePlaylistMetadata","CreatePlaylistRequest","CreatePlaylistResponse","CreatePlaylistResponseBody","DeleteLibraryRequest","DeleteLibraryResponse","DeletePlaylistRequest","DeletePlaylistResponse","Device","Director","Directory","Download","EnablePaperTrailResponse","Field","FieldType","Filter","Force","GET_PIN_SERVERS","GET_TOKEN_SERVERS","Genre","GetAvailableClientsMediaContainer","GetAvailableClientsResponse","GetAvailableClientsResponseBody","GetButlerTasksResponse","GetButlerTasksResponseBody","GetDevicesMediaContainer","GetDevicesResponse","GetDevicesResponseBody","GetFileHashRequest","GetFileHashResponse","GetGlobalHubsMediaContainer","GetGlobalHubsMetadata","GetGlobalHubsRequest","GetGlobalHubsResponse","GetGlobalHubsResponseBody","GetLibrariesDirectory","GetLibrariesLocation","GetLibrariesMediaContainer","GetLibrariesResponse","GetLibrariesResponseBody","GetLibraryDirectory","GetLibraryHubsCountry","GetLibraryHubsDirector","GetLibraryHubsGenre","GetLibraryHubsHub","GetLibraryHubsMedia","GetLibraryHubsMediaContainer","GetLibraryHubsMetadata","GetLibraryHubsPart","GetLibraryHubsRequest","GetLibraryHubsResponse","GetLibraryHubsResponseBody","GetLibraryHubsRole","GetLibraryHubsWriter","GetLibraryMediaContainer","GetLibraryRequest","GetLibraryResponse","GetLibraryResponseBody","GetLibraryType","GetMetadataChildrenDirectory","GetMetadataChildrenMediaContainer","GetMetadataChildrenMetadata","GetMetadataChildrenRequest","GetMetadataChildrenResponse","GetMetadataChildrenResponseBody","GetMetadataCountry","GetMetadataDirector","GetMetadataGenre","GetMetadataMedia","GetMetadataMediaContainer","GetMetadataMetadata","GetMetadataPart","GetMetadataRequest","GetMetadataResponse","GetMetadataResponseBody","GetMetadataRole","GetMetadataWriter","GetMyPlexAccountResponse","GetMyPlexAccountResponseBody","GetOnDeckGuids","GetOnDeckMedia","GetOnDeckMediaContainer","GetOnDeckMetadata","GetOnDeckPart","GetOnDeckResponse","GetOnDeckResponseBody","GetOnDeckStream","GetPinGlobals","GetPinRequest","GetPinResponse","GetPinResponseBody","GetPlaylistContentsCountry","GetPlaylistContentsDirector","GetPlaylistContentsGenre","GetPlaylistContentsMedia","GetPlaylistContentsMediaContainer","GetPlaylistContentsMetadata","GetPlaylistContentsPart","GetPlaylistContentsRequest","GetPlaylistContentsResponse","GetPlaylistContentsResponseBody","GetPlaylistContentsRole","GetPlaylistContentsWriter","GetPlaylistMediaContainer","GetPlaylistMetadata","GetPlaylistRequest","GetPlaylistResponse","GetPlaylistResponseBody","GetPlaylistsMediaContainer","GetPlaylistsMetadata","GetPlaylistsRequest","GetPlaylistsResponse","GetPlaylistsResponseBody","GetRecentlyAddedMediaContainer","GetRecentlyAddedResponse","GetRecentlyAddedResponseBody","GetResizedPhotoRequest","GetResizedPhotoResponse","GetSearchResultsCountry","GetSearchResultsDirector","GetSearchResultsGenre","GetSearchResultsMedia","GetSearchResultsMediaContainer","GetSearchResultsMetadata","GetSearchResultsPart","GetSearchResultsRequest","GetSearchResultsResponse","GetSearchResultsResponseBody","GetSearchResultsRole","GetSearchResultsWriter","GetServerActivitiesMediaContainer","GetServerActivitiesResponse","GetServerActivitiesResponseBody","GetServerCapabilitiesResponse","GetServerCapabilitiesResponseBody","GetServerIdentityMediaContainer","GetServerIdentityResponse","GetServerIdentityResponseBody","GetServerListMediaContainer","GetServerListResponse","GetServerListResponseBody","GetServerListServer","GetServerPreferencesMediaContainer","GetServerPreferencesResponse","GetServerPreferencesResponseBody","GetSessionHistoryMediaContainer","GetSessionHistoryMetadata","GetSessionHistoryResponse","GetSessionHistoryResponseBody","GetSessionsMedia","GetSessionsMediaContainer","GetSessionsMetadata","GetSessionsPart","GetSessionsResponse","GetSessionsResponseBody","GetSessionsStream","GetSourceConnectionInformationRequest","GetSourceConnectionInformationResponse","GetStatisticsDevice","GetStatisticsMediaContainer","GetStatisticsRequest","GetStatisticsResponse","GetStatisticsResponseBody","GetTimelineRequest","GetTimelineResponse","GetTokenGlobals","GetTokenRequest","GetTokenResponse","GetTranscodeSessionsMediaContainer","GetTranscodeSessionsResponse","GetTranscodeSessionsResponseBody","GetTransientTokenQueryParamType","GetTransientTokenRequest","GetTransientTokenResponse","GetUpdateStatusMediaContainer","GetUpdateStatusResponse","GetUpdateStatusResponseBody","Guids","Hub","IncludeDetails","Level","Location","LogLineRequest","LogLineResponse","LogMultiLineResponse","MarkPlayedRequest","MarkPlayedResponse","MarkUnplayedRequest","MarkUnplayedResponse","Media","MediaContainer","Metadata","MinSize","MyPlex","OnlyTransient","Operator","Part","PathParamTaskName","PerformSearchRequest","PerformSearchResponse","PerformVoiceSearchRequest","PerformVoiceSearchResponse","Player","PlaylistType","Producer","Provider","QueryParamOnlyTransient","QueryParamSmart","QueryParamType","Ratings","RefreshLibraryRequest","RefreshLibraryResponse","Release","Role","Scope","SearchLibraryMediaContainer","SearchLibraryMetadata","SearchLibraryRequest","SearchLibraryResponse","SearchLibraryResponseBody","Server","Session","Setting","Skip","Smart","Sort","StartAllTasksResponse","StartTaskRequest","StartTaskResponse","StartUniversalTranscodeRequest","StartUniversalTranscodeResponse","State","StatisticsMedia","StopAllTasksResponse","StopTaskRequest","StopTaskResponse","StopTranscodeSessionRequest","StopTranscodeSessionResponse","Stream","TaskName","Tonight","TranscodeSession","Type","UpdatePlayProgressRequest","UpdatePlayProgressResponse","UpdatePlaylistRequest","UpdatePlaylistResponse","UploadPlaylistRequest","UploadPlaylistResponse","Upscale","User","Writer"]
```

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/addplaylistcontents.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/applyupdates.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/applyupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/cancelserveractivities.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/checkforupdates.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/checkforupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/clearplaylistcontents.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/createplaylist.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/createplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/deletelibrary.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/deleteplaylist.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/enablepapertrail.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getavailableclients.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getbutlertasks.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getdevices.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getfilehash.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getglobalhubs.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getglobalhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getlibraries.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getlibrary.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getlibraryhubs.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getlibraryhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getlibraryitems.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getondeck.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,227 +1,166 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
-from datetime import date
-from enum import Enum
+from datetime import datetime
 from plex_api import utils
 from typing import List, Optional
 
-class Tag(str, Enum):
-    r"""A key representing a specific tag within the section."""
-    ALL = 'all'
-    UNWATCHED = 'unwatched'
-    NEWEST = 'newest'
-    RECENTLY_ADDED = 'recentlyAdded'
-    RECENTLY_VIEWED = 'recentlyViewed'
-    ON_DECK = 'onDeck'
-    COLLECTION = 'collection'
-    EDITION = 'edition'
-    GENRE = 'genre'
-    YEAR = 'year'
-    DECADE = 'decade'
-    DIRECTOR = 'director'
-    ACTOR = 'actor'
-    COUNTRY = 'country'
-    CONTENT_RATING = 'contentRating'
-    RATING = 'rating'
-    RESOLUTION = 'resolution'
-    FIRST_CHARACTER = 'firstCharacter'
-    FOLDER = 'folder'
-
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetLibraryItemsRequest:
-    section_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'sectionId', 'style': 'simple', 'explode': False }})
-    r"""the Id of the library to query"""
-    tag: Tag = dataclasses.field(metadata={'path_param': { 'field_name': 'tag', 'style': 'simple', 'explode': False }})
-    r"""A key representing a specific tag within the section."""
+class GetOnDeckStream:
+    id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    stream_type: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streamType'), 'exclude': lambda f: f is None }})
+    default: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('default'), 'exclude': lambda f: f is None }})
+    codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec'), 'exclude': lambda f: f is None }})
+    index: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('index'), 'exclude': lambda f: f is None }})
+    bitrate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bitrate'), 'exclude': lambda f: f is None }})
+    language: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('language'), 'exclude': lambda f: f is None }})
+    language_tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('languageTag'), 'exclude': lambda f: f is None }})
+    language_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('languageCode'), 'exclude': lambda f: f is None }})
+    bit_depth: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bitDepth'), 'exclude': lambda f: f is None }})
+    chroma_location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('chromaLocation'), 'exclude': lambda f: f is None }})
+    chroma_subsampling: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('chromaSubsampling'), 'exclude': lambda f: f is None }})
+    coded_height: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codedHeight'), 'exclude': lambda f: f is None }})
+    coded_width: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codedWidth'), 'exclude': lambda f: f is None }})
+    color_range: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('colorRange'), 'exclude': lambda f: f is None }})
+    frame_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('frameRate'), 'exclude': lambda f: f is None }})
+    height: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is None }})
+    level: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('level'), 'exclude': lambda f: f is None }})
+    profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('profile'), 'exclude': lambda f: f is None }})
+    ref_frames: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refFrames'), 'exclude': lambda f: f is None }})
+    width: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is None }})
+    display_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('displayTitle'), 'exclude': lambda f: f is None }})
+    extended_display_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extendedDisplayTitle'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetLibraryItemsPart:
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+class GetOnDeckPart:
+    id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
-    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
+    duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
     file: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file'), 'exclude': lambda f: f is None }})
-    size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
+    size: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
+    audio_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioProfile'), 'exclude': lambda f: f is None }})
     container: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('container'), 'exclude': lambda f: f is None }})
     video_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoProfile'), 'exclude': lambda f: f is None }})
+    stream: Optional[List[GetOnDeckStream]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Stream'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetLibraryItemsMedia:
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
-    bitrate: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bitrate'), 'exclude': lambda f: f is None }})
-    width: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is None }})
-    height: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is None }})
+class GetOnDeckMedia:
+    id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
+    bitrate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bitrate'), 'exclude': lambda f: f is None }})
+    width: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is None }})
+    height: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is None }})
     aspect_ratio: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aspectRatio'), 'exclude': lambda f: f is None }})
-    audio_channels: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioChannels'), 'exclude': lambda f: f is None }})
+    audio_channels: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioChannels'), 'exclude': lambda f: f is None }})
     audio_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioCodec'), 'exclude': lambda f: f is None }})
     video_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoCodec'), 'exclude': lambda f: f is None }})
     video_resolution: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoResolution'), 'exclude': lambda f: f is None }})
     container: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('container'), 'exclude': lambda f: f is None }})
     video_frame_rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoFrameRate'), 'exclude': lambda f: f is None }})
+    audio_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioProfile'), 'exclude': lambda f: f is None }})
     video_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoProfile'), 'exclude': lambda f: f is None }})
-    part: Optional[List[GetLibraryItemsPart]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Part'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetLibraryItemsGenre:
-    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetLibraryItemsCountry:
-    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetLibraryItemsDirector:
-    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
+    part: Optional[List[GetOnDeckPart]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Part'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetLibraryItemsWriter:
-    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
+class GetOnDeckGuids:
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetLibraryItemsRole:
-    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetLibraryItemsMetadata:
-    rating_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingKey'), 'exclude': lambda f: f is None }})
+class GetOnDeckMetadata:
+    allow_sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSync'), 'exclude': lambda f: f is None }})
+    library_section_id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionID'), 'exclude': lambda f: f is None }})
+    library_section_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionTitle'), 'exclude': lambda f: f is None }})
+    library_section_uuid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionUUID'), 'exclude': lambda f: f is None }})
+    rating_key: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingKey'), 'exclude': lambda f: f is None }})
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
+    parent_rating_key: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentRatingKey'), 'exclude': lambda f: f is None }})
+    grandparent_rating_key: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentRatingKey'), 'exclude': lambda f: f is None }})
     guid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('guid'), 'exclude': lambda f: f is None }})
-    studio: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('studio'), 'exclude': lambda f: f is None }})
+    parent_guid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentGuid'), 'exclude': lambda f: f is None }})
+    grandparent_guid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentGuid'), 'exclude': lambda f: f is None }})
     type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
     title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
+    grandparent_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentKey'), 'exclude': lambda f: f is None }})
+    parent_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentKey'), 'exclude': lambda f: f is None }})
+    library_section_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionKey'), 'exclude': lambda f: f is None }})
+    grandparent_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentTitle'), 'exclude': lambda f: f is None }})
+    parent_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentTitle'), 'exclude': lambda f: f is None }})
     content_rating: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentRating'), 'exclude': lambda f: f is None }})
     summary: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('summary'), 'exclude': lambda f: f is None }})
-    rating: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rating'), 'exclude': lambda f: f is None }})
-    audience_rating: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audienceRating'), 'exclude': lambda f: f is None }})
-    year: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('year'), 'exclude': lambda f: f is None }})
-    tagline: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tagline'), 'exclude': lambda f: f is None }})
+    index: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('index'), 'exclude': lambda f: f is None }})
+    parent_index: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentIndex'), 'exclude': lambda f: f is None }})
+    last_viewed_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastViewedAt'), 'exclude': lambda f: f is None }})
+    year: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('year'), 'exclude': lambda f: f is None }})
     thumb: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('thumb'), 'exclude': lambda f: f is None }})
     art: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('art'), 'exclude': lambda f: f is None }})
-    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
-    originally_available_at: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('originallyAvailableAt'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'exclude': lambda f: f is None }})
-    added_at: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('addedAt'), 'exclude': lambda f: f is None }})
-    updated_at: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'exclude': lambda f: f is None }})
-    audience_rating_image: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audienceRatingImage'), 'exclude': lambda f: f is None }})
-    chapter_source: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('chapterSource'), 'exclude': lambda f: f is None }})
-    primary_extra_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('primaryExtraKey'), 'exclude': lambda f: f is None }})
-    rating_image: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingImage'), 'exclude': lambda f: f is None }})
-    grandparent_rating_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentRatingKey'), 'exclude': lambda f: f is None }})
-    grandparent_guid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentGuid'), 'exclude': lambda f: f is None }})
-    grandparent_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentKey'), 'exclude': lambda f: f is None }})
-    grandparent_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentTitle'), 'exclude': lambda f: f is None }})
+    parent_thumb: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentThumb'), 'exclude': lambda f: f is None }})
     grandparent_thumb: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentThumb'), 'exclude': lambda f: f is None }})
     grandparent_art: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentArt'), 'exclude': lambda f: f is None }})
     grandparent_theme: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentTheme'), 'exclude': lambda f: f is None }})
-    media: Optional[List[GetLibraryItemsMedia]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Media'), 'exclude': lambda f: f is None }})
-    genre: Optional[List[GetLibraryItemsGenre]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Genre'), 'exclude': lambda f: f is None }})
-    country: Optional[List[GetLibraryItemsCountry]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Country'), 'exclude': lambda f: f is None }})
-    director: Optional[List[GetLibraryItemsDirector]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Director'), 'exclude': lambda f: f is None }})
-    writer: Optional[List[GetLibraryItemsWriter]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Writer'), 'exclude': lambda f: f is None }})
-    role: Optional[List[GetLibraryItemsRole]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Role'), 'exclude': lambda f: f is None }})
-    title_sort: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('titleSort'), 'exclude': lambda f: f is None }})
-    view_count: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('viewCount'), 'exclude': lambda f: f is None }})
-    last_viewed_at: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastViewedAt'), 'exclude': lambda f: f is None }})
-    original_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('originalTitle'), 'exclude': lambda f: f is None }})
-    view_offset: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('viewOffset'), 'exclude': lambda f: f is None }})
-    skip_count: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('skipCount'), 'exclude': lambda f: f is None }})
-    index: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('index'), 'exclude': lambda f: f is None }})
-    theme: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('theme'), 'exclude': lambda f: f is None }})
-    leaf_count: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leafCount'), 'exclude': lambda f: f is None }})
-    viewed_leaf_count: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('viewedLeafCount'), 'exclude': lambda f: f is None }})
-    child_count: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('childCount'), 'exclude': lambda f: f is None }})
-    has_premium_extras: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasPremiumExtras'), 'exclude': lambda f: f is None }})
-    has_premium_primary_extra: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasPremiumPrimaryExtra'), 'exclude': lambda f: f is None }})
-    parent_rating_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentRatingKey'), 'exclude': lambda f: f is None }})
-    parent_guid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentGuid'), 'exclude': lambda f: f is None }})
-    parent_studio: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentStudio'), 'exclude': lambda f: f is None }})
-    parent_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentKey'), 'exclude': lambda f: f is None }})
-    parent_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentTitle'), 'exclude': lambda f: f is None }})
-    parent_index: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentIndex'), 'exclude': lambda f: f is None }})
-    parent_year: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentYear'), 'exclude': lambda f: f is None }})
-    parent_thumb: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentThumb'), 'exclude': lambda f: f is None }})
-    parent_theme: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentTheme'), 'exclude': lambda f: f is None }})
+    duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
+    originally_available_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('originallyAvailableAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
+    added_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('addedAt'), 'exclude': lambda f: f is None }})
+    updated_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'exclude': lambda f: f is None }})
+    media: Optional[List[GetOnDeckMedia]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Media'), 'exclude': lambda f: f is None }})
+    guids: Optional[List[GetOnDeckGuids]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Guid'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetLibraryItemsMediaContainer:
-    size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
+class GetOnDeckMediaContainer:
+    size: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
     allow_sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSync'), 'exclude': lambda f: f is None }})
-    art: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('art'), 'exclude': lambda f: f is None }})
     identifier: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('identifier'), 'exclude': lambda f: f is None }})
-    library_section_id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionID'), 'exclude': lambda f: f is None }})
-    library_section_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionTitle'), 'exclude': lambda f: f is None }})
-    library_section_uuid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionUUID'), 'exclude': lambda f: f is None }})
     media_tag_prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaTagPrefix'), 'exclude': lambda f: f is None }})
-    media_tag_version: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaTagVersion'), 'exclude': lambda f: f is None }})
-    thumb: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('thumb'), 'exclude': lambda f: f is None }})
-    title1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title1'), 'exclude': lambda f: f is None }})
-    title2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title2'), 'exclude': lambda f: f is None }})
-    view_group: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('viewGroup'), 'exclude': lambda f: f is None }})
-    view_mode: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('viewMode'), 'exclude': lambda f: f is None }})
+    media_tag_version: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaTagVersion'), 'exclude': lambda f: f is None }})
     mixed_parents: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mixedParents'), 'exclude': lambda f: f is None }})
-    metadata: Optional[List[GetLibraryItemsMetadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Metadata'), 'exclude': lambda f: f is None }})
+    metadata: Optional[List[GetOnDeckMetadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Metadata'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetLibraryItemsResponseBody:
-    r"""The contents of the library by section and tag"""
-    media_container: Optional[GetLibraryItemsMediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
+class GetOnDeckResponseBody:
+    r"""The on Deck content"""
+    media_container: Optional[GetOnDeckMediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclasses.dataclass
-class GetLibraryItemsResponse:
+class GetOnDeckResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    object: Optional[GetLibraryItemsResponseBody] = dataclasses.field(default=None)
-    r"""The contents of the library by section and tag"""
+    object: Optional[GetOnDeckResponseBody] = dataclasses.field(default=None)
+    r"""The on Deck content"""
```

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getmetadata.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getmetadatachildren.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getmyplexaccount.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getondeck.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getplaylistcontents.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,166 +1,178 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
+from datetime import date
 from plex_api import utils
 from typing import List, Optional
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOnDeckStream:
-    id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    stream_type: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streamType'), 'exclude': lambda f: f is None }})
-    default: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('default'), 'exclude': lambda f: f is None }})
-    codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec'), 'exclude': lambda f: f is None }})
-    index: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('index'), 'exclude': lambda f: f is None }})
-    bitrate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bitrate'), 'exclude': lambda f: f is None }})
-    language: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('language'), 'exclude': lambda f: f is None }})
-    language_tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('languageTag'), 'exclude': lambda f: f is None }})
-    language_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('languageCode'), 'exclude': lambda f: f is None }})
-    bit_depth: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bitDepth'), 'exclude': lambda f: f is None }})
-    chroma_location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('chromaLocation'), 'exclude': lambda f: f is None }})
-    chroma_subsampling: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('chromaSubsampling'), 'exclude': lambda f: f is None }})
-    coded_height: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codedHeight'), 'exclude': lambda f: f is None }})
-    coded_width: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codedWidth'), 'exclude': lambda f: f is None }})
-    color_range: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('colorRange'), 'exclude': lambda f: f is None }})
-    frame_rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('frameRate'), 'exclude': lambda f: f is None }})
-    height: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is None }})
-    level: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('level'), 'exclude': lambda f: f is None }})
-    profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('profile'), 'exclude': lambda f: f is None }})
-    ref_frames: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refFrames'), 'exclude': lambda f: f is None }})
-    width: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is None }})
-    display_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('displayTitle'), 'exclude': lambda f: f is None }})
-    extended_display_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extendedDisplayTitle'), 'exclude': lambda f: f is None }})
+class GetPlaylistContentsRequest:
+    playlist_id: float = dataclasses.field(metadata={'path_param': { 'field_name': 'playlistID', 'style': 'simple', 'explode': False }})
+    r"""the ID of the playlist"""
+    type: float = dataclasses.field(metadata={'query_param': { 'field_name': 'type', 'style': 'form', 'explode': True }})
+    r"""the metadata type of the item to return"""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOnDeckPart:
-    id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+class GetPlaylistContentsPart:
+    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
-    duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
+    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
     file: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file'), 'exclude': lambda f: f is None }})
-    size: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
+    size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
     audio_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioProfile'), 'exclude': lambda f: f is None }})
     container: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('container'), 'exclude': lambda f: f is None }})
+    has64bit_offsets: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has64bitOffsets'), 'exclude': lambda f: f is None }})
+    optimized_for_streaming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('optimizedForStreaming'), 'exclude': lambda f: f is None }})
     video_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoProfile'), 'exclude': lambda f: f is None }})
-    stream: Optional[List[GetOnDeckStream]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Stream'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOnDeckMedia:
-    id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
-    bitrate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bitrate'), 'exclude': lambda f: f is None }})
-    width: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is None }})
-    height: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is None }})
+class GetPlaylistContentsMedia:
+    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
+    bitrate: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bitrate'), 'exclude': lambda f: f is None }})
+    width: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is None }})
+    height: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is None }})
     aspect_ratio: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aspectRatio'), 'exclude': lambda f: f is None }})
-    audio_channels: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioChannels'), 'exclude': lambda f: f is None }})
+    audio_channels: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioChannels'), 'exclude': lambda f: f is None }})
     audio_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioCodec'), 'exclude': lambda f: f is None }})
     video_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoCodec'), 'exclude': lambda f: f is None }})
     video_resolution: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoResolution'), 'exclude': lambda f: f is None }})
     container: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('container'), 'exclude': lambda f: f is None }})
     video_frame_rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoFrameRate'), 'exclude': lambda f: f is None }})
+    optimized_for_streaming: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('optimizedForStreaming'), 'exclude': lambda f: f is None }})
     audio_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioProfile'), 'exclude': lambda f: f is None }})
+    has64bit_offsets: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has64bitOffsets'), 'exclude': lambda f: f is None }})
     video_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoProfile'), 'exclude': lambda f: f is None }})
-    part: Optional[List[GetOnDeckPart]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Part'), 'exclude': lambda f: f is None }})
+    part: Optional[List[GetPlaylistContentsPart]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Part'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOnDeckGuids:
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+class GetPlaylistContentsGenre:
+    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOnDeckMetadata:
-    allow_sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSync'), 'exclude': lambda f: f is None }})
-    library_section_id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionID'), 'exclude': lambda f: f is None }})
-    library_section_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionTitle'), 'exclude': lambda f: f is None }})
-    library_section_uuid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionUUID'), 'exclude': lambda f: f is None }})
-    rating_key: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingKey'), 'exclude': lambda f: f is None }})
+class GetPlaylistContentsCountry:
+    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
+    
+
+
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetPlaylistContentsDirector:
+    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
+    
+
+
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetPlaylistContentsWriter:
+    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
+    
+
+
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetPlaylistContentsRole:
+    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
+    
+
+
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetPlaylistContentsMetadata:
+    rating_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingKey'), 'exclude': lambda f: f is None }})
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
-    parent_rating_key: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentRatingKey'), 'exclude': lambda f: f is None }})
-    grandparent_rating_key: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentRatingKey'), 'exclude': lambda f: f is None }})
     guid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('guid'), 'exclude': lambda f: f is None }})
-    parent_guid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentGuid'), 'exclude': lambda f: f is None }})
-    grandparent_guid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentGuid'), 'exclude': lambda f: f is None }})
+    studio: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('studio'), 'exclude': lambda f: f is None }})
     type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
     title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
-    grandparent_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentKey'), 'exclude': lambda f: f is None }})
-    parent_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentKey'), 'exclude': lambda f: f is None }})
+    title_sort: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('titleSort'), 'exclude': lambda f: f is None }})
+    library_section_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionTitle'), 'exclude': lambda f: f is None }})
+    library_section_id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionID'), 'exclude': lambda f: f is None }})
     library_section_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionKey'), 'exclude': lambda f: f is None }})
-    grandparent_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentTitle'), 'exclude': lambda f: f is None }})
-    parent_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentTitle'), 'exclude': lambda f: f is None }})
     content_rating: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentRating'), 'exclude': lambda f: f is None }})
     summary: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('summary'), 'exclude': lambda f: f is None }})
-    index: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('index'), 'exclude': lambda f: f is None }})
-    parent_index: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentIndex'), 'exclude': lambda f: f is None }})
-    last_viewed_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastViewedAt'), 'exclude': lambda f: f is None }})
-    year: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('year'), 'exclude': lambda f: f is None }})
+    rating: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rating'), 'exclude': lambda f: f is None }})
+    audience_rating: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audienceRating'), 'exclude': lambda f: f is None }})
+    year: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('year'), 'exclude': lambda f: f is None }})
+    tagline: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tagline'), 'exclude': lambda f: f is None }})
     thumb: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('thumb'), 'exclude': lambda f: f is None }})
     art: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('art'), 'exclude': lambda f: f is None }})
-    parent_thumb: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentThumb'), 'exclude': lambda f: f is None }})
-    grandparent_thumb: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentThumb'), 'exclude': lambda f: f is None }})
-    grandparent_art: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentArt'), 'exclude': lambda f: f is None }})
-    grandparent_theme: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grandparentTheme'), 'exclude': lambda f: f is None }})
-    duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
-    originally_available_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('originallyAvailableAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
-    added_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('addedAt'), 'exclude': lambda f: f is None }})
-    updated_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'exclude': lambda f: f is None }})
-    media: Optional[List[GetOnDeckMedia]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Media'), 'exclude': lambda f: f is None }})
-    guids: Optional[List[GetOnDeckGuids]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Guid'), 'exclude': lambda f: f is None }})
+    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
+    originally_available_at: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('originallyAvailableAt'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'exclude': lambda f: f is None }})
+    added_at: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('addedAt'), 'exclude': lambda f: f is None }})
+    updated_at: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'exclude': lambda f: f is None }})
+    audience_rating_image: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audienceRatingImage'), 'exclude': lambda f: f is None }})
+    has_premium_extras: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasPremiumExtras'), 'exclude': lambda f: f is None }})
+    has_premium_primary_extra: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasPremiumPrimaryExtra'), 'exclude': lambda f: f is None }})
+    rating_image: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingImage'), 'exclude': lambda f: f is None }})
+    media: Optional[List[GetPlaylistContentsMedia]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Media'), 'exclude': lambda f: f is None }})
+    genre: Optional[List[GetPlaylistContentsGenre]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Genre'), 'exclude': lambda f: f is None }})
+    country: Optional[List[GetPlaylistContentsCountry]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Country'), 'exclude': lambda f: f is None }})
+    director: Optional[List[GetPlaylistContentsDirector]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Director'), 'exclude': lambda f: f is None }})
+    writer: Optional[List[GetPlaylistContentsWriter]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Writer'), 'exclude': lambda f: f is None }})
+    role: Optional[List[GetPlaylistContentsRole]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Role'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOnDeckMediaContainer:
-    size: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
-    allow_sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSync'), 'exclude': lambda f: f is None }})
-    identifier: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('identifier'), 'exclude': lambda f: f is None }})
-    media_tag_prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaTagPrefix'), 'exclude': lambda f: f is None }})
-    media_tag_version: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaTagVersion'), 'exclude': lambda f: f is None }})
-    mixed_parents: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mixedParents'), 'exclude': lambda f: f is None }})
-    metadata: Optional[List[GetOnDeckMetadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Metadata'), 'exclude': lambda f: f is None }})
+class GetPlaylistContentsMediaContainer:
+    size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
+    composite: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('composite'), 'exclude': lambda f: f is None }})
+    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
+    leaf_count: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leafCount'), 'exclude': lambda f: f is None }})
+    playlist_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('playlistType'), 'exclude': lambda f: f is None }})
+    rating_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingKey'), 'exclude': lambda f: f is None }})
+    smart: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('smart'), 'exclude': lambda f: f is None }})
+    title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
+    metadata: Optional[List[GetPlaylistContentsMetadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Metadata'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOnDeckResponseBody:
-    r"""The on Deck content"""
-    media_container: Optional[GetOnDeckMediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
+class GetPlaylistContentsResponseBody:
+    r"""The playlist contents"""
+    media_container: Optional[GetPlaylistContentsMediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclasses.dataclass
-class GetOnDeckResponse:
+class GetPlaylistContentsResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    object: Optional[GetOnDeckResponseBody] = dataclasses.field(default=None)
-    r"""The on Deck content"""
+    object: Optional[GetPlaylistContentsResponseBody] = dataclasses.field(default=None)
+    r"""The playlist contents"""
```

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getpin.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getpin.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getplaylist.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getplaylistcontents.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getrecentlyadded.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,178 +1,166 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
-from datetime import date
+from datetime import datetime
 from plex_api import utils
 from typing import List, Optional
 
 
-@dataclasses.dataclass
-class GetPlaylistContentsRequest:
-    playlist_id: float = dataclasses.field(metadata={'path_param': { 'field_name': 'playlistID', 'style': 'simple', 'explode': False }})
-    r"""the ID of the playlist"""
-    type: float = dataclasses.field(metadata={'query_param': { 'field_name': 'type', 'style': 'form', 'explode': True }})
-    r"""the metadata type of the item to return"""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetPlaylistContentsPart:
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+class Part:
+    id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
-    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
+    duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
     file: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file'), 'exclude': lambda f: f is None }})
-    size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
-    audio_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioProfile'), 'exclude': lambda f: f is None }})
+    size: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
     container: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('container'), 'exclude': lambda f: f is None }})
     has64bit_offsets: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has64bitOffsets'), 'exclude': lambda f: f is None }})
+    has_thumbnail: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasThumbnail'), 'exclude': lambda f: f is None }})
     optimized_for_streaming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('optimizedForStreaming'), 'exclude': lambda f: f is None }})
     video_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoProfile'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetPlaylistContentsMedia:
-    id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
-    bitrate: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bitrate'), 'exclude': lambda f: f is None }})
-    width: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is None }})
-    height: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is None }})
+class Media:
+    id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
+    bitrate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bitrate'), 'exclude': lambda f: f is None }})
+    width: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is None }})
+    height: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is None }})
     aspect_ratio: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aspectRatio'), 'exclude': lambda f: f is None }})
-    audio_channels: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioChannels'), 'exclude': lambda f: f is None }})
+    audio_channels: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioChannels'), 'exclude': lambda f: f is None }})
     audio_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioCodec'), 'exclude': lambda f: f is None }})
     video_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoCodec'), 'exclude': lambda f: f is None }})
-    video_resolution: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoResolution'), 'exclude': lambda f: f is None }})
+    video_resolution: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoResolution'), 'exclude': lambda f: f is None }})
     container: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('container'), 'exclude': lambda f: f is None }})
     video_frame_rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoFrameRate'), 'exclude': lambda f: f is None }})
-    optimized_for_streaming: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('optimizedForStreaming'), 'exclude': lambda f: f is None }})
-    audio_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioProfile'), 'exclude': lambda f: f is None }})
+    optimized_for_streaming: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('optimizedForStreaming'), 'exclude': lambda f: f is None }})
     has64bit_offsets: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has64bitOffsets'), 'exclude': lambda f: f is None }})
     video_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoProfile'), 'exclude': lambda f: f is None }})
-    part: Optional[List[GetPlaylistContentsPart]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Part'), 'exclude': lambda f: f is None }})
+    part: Optional[List[Part]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Part'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetPlaylistContentsGenre:
+class Genre:
     tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetPlaylistContentsCountry:
+class Director:
     tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetPlaylistContentsDirector:
+class Writer:
     tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetPlaylistContentsWriter:
+class Country:
     tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetPlaylistContentsRole:
+class Role:
     tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetPlaylistContentsMetadata:
-    rating_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingKey'), 'exclude': lambda f: f is None }})
+class Metadata:
+    allow_sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSync'), 'exclude': lambda f: f is None }})
+    library_section_id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionID'), 'exclude': lambda f: f is None }})
+    library_section_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionTitle'), 'exclude': lambda f: f is None }})
+    library_section_uuid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionUUID'), 'exclude': lambda f: f is None }})
+    rating_key: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingKey'), 'exclude': lambda f: f is None }})
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
     guid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('guid'), 'exclude': lambda f: f is None }})
     studio: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('studio'), 'exclude': lambda f: f is None }})
     type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
     title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
-    title_sort: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('titleSort'), 'exclude': lambda f: f is None }})
-    library_section_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionTitle'), 'exclude': lambda f: f is None }})
-    library_section_id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionID'), 'exclude': lambda f: f is None }})
-    library_section_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionKey'), 'exclude': lambda f: f is None }})
     content_rating: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentRating'), 'exclude': lambda f: f is None }})
     summary: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('summary'), 'exclude': lambda f: f is None }})
     rating: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rating'), 'exclude': lambda f: f is None }})
     audience_rating: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audienceRating'), 'exclude': lambda f: f is None }})
-    year: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('year'), 'exclude': lambda f: f is None }})
+    year: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('year'), 'exclude': lambda f: f is None }})
     tagline: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tagline'), 'exclude': lambda f: f is None }})
     thumb: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('thumb'), 'exclude': lambda f: f is None }})
     art: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('art'), 'exclude': lambda f: f is None }})
-    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
-    originally_available_at: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('originallyAvailableAt'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'exclude': lambda f: f is None }})
-    added_at: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('addedAt'), 'exclude': lambda f: f is None }})
-    updated_at: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'exclude': lambda f: f is None }})
+    duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
+    originally_available_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('originallyAvailableAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
+    added_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('addedAt'), 'exclude': lambda f: f is None }})
+    updated_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'exclude': lambda f: f is None }})
     audience_rating_image: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audienceRatingImage'), 'exclude': lambda f: f is None }})
-    has_premium_extras: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasPremiumExtras'), 'exclude': lambda f: f is None }})
-    has_premium_primary_extra: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasPremiumPrimaryExtra'), 'exclude': lambda f: f is None }})
+    chapter_source: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('chapterSource'), 'exclude': lambda f: f is None }})
+    primary_extra_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('primaryExtraKey'), 'exclude': lambda f: f is None }})
     rating_image: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingImage'), 'exclude': lambda f: f is None }})
-    media: Optional[List[GetPlaylistContentsMedia]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Media'), 'exclude': lambda f: f is None }})
-    genre: Optional[List[GetPlaylistContentsGenre]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Genre'), 'exclude': lambda f: f is None }})
-    country: Optional[List[GetPlaylistContentsCountry]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Country'), 'exclude': lambda f: f is None }})
-    director: Optional[List[GetPlaylistContentsDirector]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Director'), 'exclude': lambda f: f is None }})
-    writer: Optional[List[GetPlaylistContentsWriter]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Writer'), 'exclude': lambda f: f is None }})
-    role: Optional[List[GetPlaylistContentsRole]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Role'), 'exclude': lambda f: f is None }})
+    media: Optional[List[Media]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Media'), 'exclude': lambda f: f is None }})
+    genre: Optional[List[Genre]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Genre'), 'exclude': lambda f: f is None }})
+    director: Optional[List[Director]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Director'), 'exclude': lambda f: f is None }})
+    writer: Optional[List[Writer]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Writer'), 'exclude': lambda f: f is None }})
+    country: Optional[List[Country]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Country'), 'exclude': lambda f: f is None }})
+    role: Optional[List[Role]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Role'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetPlaylistContentsMediaContainer:
-    size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
-    composite: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('composite'), 'exclude': lambda f: f is None }})
-    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
-    leaf_count: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leafCount'), 'exclude': lambda f: f is None }})
-    playlist_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('playlistType'), 'exclude': lambda f: f is None }})
-    rating_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingKey'), 'exclude': lambda f: f is None }})
-    smart: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('smart'), 'exclude': lambda f: f is None }})
-    title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
-    metadata: Optional[List[GetPlaylistContentsMetadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Metadata'), 'exclude': lambda f: f is None }})
+class GetRecentlyAddedMediaContainer:
+    size: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
+    allow_sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSync'), 'exclude': lambda f: f is None }})
+    identifier: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('identifier'), 'exclude': lambda f: f is None }})
+    media_tag_prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaTagPrefix'), 'exclude': lambda f: f is None }})
+    media_tag_version: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaTagVersion'), 'exclude': lambda f: f is None }})
+    mixed_parents: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mixedParents'), 'exclude': lambda f: f is None }})
+    metadata: Optional[List[Metadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Metadata'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetPlaylistContentsResponseBody:
-    r"""The playlist contents"""
-    media_container: Optional[GetPlaylistContentsMediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
+class GetRecentlyAddedResponseBody:
+    r"""The recently added content"""
+    media_container: Optional[GetRecentlyAddedMediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclasses.dataclass
-class GetPlaylistContentsResponse:
+class GetRecentlyAddedResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    object: Optional[GetPlaylistContentsResponseBody] = dataclasses.field(default=None)
-    r"""The playlist contents"""
+    object: Optional[GetRecentlyAddedResponseBody] = dataclasses.field(default=None)
+    r"""The recently added content"""
```

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getplaylists.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getplaylists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getrecentlyadded.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getsearchresults.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,101 +6,108 @@
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from plex_api import utils
 from typing import List, Optional
 
 
+@dataclasses.dataclass
+class GetSearchResultsRequest:
+    query: str = dataclasses.field(metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
+    r"""The search query string to use"""
+    
+
+
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Part:
+class GetSearchResultsPart:
     id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
     duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
     file: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file'), 'exclude': lambda f: f is None }})
     size: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
+    audio_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioProfile'), 'exclude': lambda f: f is None }})
     container: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('container'), 'exclude': lambda f: f is None }})
-    has64bit_offsets: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has64bitOffsets'), 'exclude': lambda f: f is None }})
-    has_thumbnail: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasThumbnail'), 'exclude': lambda f: f is None }})
-    optimized_for_streaming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('optimizedForStreaming'), 'exclude': lambda f: f is None }})
     video_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoProfile'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Media:
+class GetSearchResultsMedia:
     id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
     bitrate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bitrate'), 'exclude': lambda f: f is None }})
     width: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is None }})
     height: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is None }})
     aspect_ratio: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aspectRatio'), 'exclude': lambda f: f is None }})
     audio_channels: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioChannels'), 'exclude': lambda f: f is None }})
     audio_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioCodec'), 'exclude': lambda f: f is None }})
     video_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoCodec'), 'exclude': lambda f: f is None }})
     video_resolution: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoResolution'), 'exclude': lambda f: f is None }})
     container: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('container'), 'exclude': lambda f: f is None }})
     video_frame_rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoFrameRate'), 'exclude': lambda f: f is None }})
-    optimized_for_streaming: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('optimizedForStreaming'), 'exclude': lambda f: f is None }})
-    has64bit_offsets: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has64bitOffsets'), 'exclude': lambda f: f is None }})
+    audio_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioProfile'), 'exclude': lambda f: f is None }})
     video_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoProfile'), 'exclude': lambda f: f is None }})
-    part: Optional[List[Part]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Part'), 'exclude': lambda f: f is None }})
+    part: Optional[List[GetSearchResultsPart]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Part'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Genre:
+class GetSearchResultsGenre:
     tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Director:
+class GetSearchResultsDirector:
     tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Writer:
+class GetSearchResultsWriter:
     tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Country:
+class GetSearchResultsCountry:
     tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Role:
+class GetSearchResultsRole:
     tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Metadata:
+class GetSearchResultsMetadata:
     allow_sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSync'), 'exclude': lambda f: f is None }})
     library_section_id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionID'), 'exclude': lambda f: f is None }})
     library_section_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionTitle'), 'exclude': lambda f: f is None }})
     library_section_uuid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionUUID'), 'exclude': lambda f: f is None }})
+    personal: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('personal'), 'exclude': lambda f: f is None }})
+    source_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceTitle'), 'exclude': lambda f: f is None }})
     rating_key: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingKey'), 'exclude': lambda f: f is None }})
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
     guid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('guid'), 'exclude': lambda f: f is None }})
     studio: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('studio'), 'exclude': lambda f: f is None }})
     type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
     title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
     content_rating: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentRating'), 'exclude': lambda f: f is None }})
@@ -115,52 +122,61 @@
     originally_available_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('originallyAvailableAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     added_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('addedAt'), 'exclude': lambda f: f is None }})
     updated_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'exclude': lambda f: f is None }})
     audience_rating_image: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audienceRatingImage'), 'exclude': lambda f: f is None }})
     chapter_source: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('chapterSource'), 'exclude': lambda f: f is None }})
     primary_extra_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('primaryExtraKey'), 'exclude': lambda f: f is None }})
     rating_image: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingImage'), 'exclude': lambda f: f is None }})
-    media: Optional[List[Media]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Media'), 'exclude': lambda f: f is None }})
-    genre: Optional[List[Genre]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Genre'), 'exclude': lambda f: f is None }})
-    director: Optional[List[Director]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Director'), 'exclude': lambda f: f is None }})
-    writer: Optional[List[Writer]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Writer'), 'exclude': lambda f: f is None }})
-    country: Optional[List[Country]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Country'), 'exclude': lambda f: f is None }})
-    role: Optional[List[Role]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Role'), 'exclude': lambda f: f is None }})
+    media: Optional[List[GetSearchResultsMedia]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Media'), 'exclude': lambda f: f is None }})
+    genre: Optional[List[GetSearchResultsGenre]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Genre'), 'exclude': lambda f: f is None }})
+    director: Optional[List[GetSearchResultsDirector]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Director'), 'exclude': lambda f: f is None }})
+    writer: Optional[List[GetSearchResultsWriter]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Writer'), 'exclude': lambda f: f is None }})
+    country: Optional[List[GetSearchResultsCountry]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Country'), 'exclude': lambda f: f is None }})
+    role: Optional[List[GetSearchResultsRole]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Role'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetRecentlyAddedMediaContainer:
+class Provider:
+    key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
+    title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+    
+
+
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetSearchResultsMediaContainer:
     size: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
-    allow_sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSync'), 'exclude': lambda f: f is None }})
     identifier: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('identifier'), 'exclude': lambda f: f is None }})
     media_tag_prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaTagPrefix'), 'exclude': lambda f: f is None }})
     media_tag_version: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaTagVersion'), 'exclude': lambda f: f is None }})
-    mixed_parents: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mixedParents'), 'exclude': lambda f: f is None }})
-    metadata: Optional[List[Metadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Metadata'), 'exclude': lambda f: f is None }})
+    metadata: Optional[List[GetSearchResultsMetadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Metadata'), 'exclude': lambda f: f is None }})
+    provider: Optional[List[Provider]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Provider'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetRecentlyAddedResponseBody:
-    r"""The recently added content"""
-    media_container: Optional[GetRecentlyAddedMediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
+class GetSearchResultsResponseBody:
+    r"""Search Results"""
+    media_container: Optional[GetSearchResultsMediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclasses.dataclass
-class GetRecentlyAddedResponse:
+class GetSearchResultsResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    object: Optional[GetRecentlyAddedResponseBody] = dataclasses.field(default=None)
-    r"""The recently added content"""
+    object: Optional[GetSearchResultsResponseBody] = dataclasses.field(default=None)
+    r"""Search Results"""
```

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getresizedphoto.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getresizedphoto.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getsearchresults.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getservercapabilities.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,182 +1,99 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
 from plex_api import utils
 from typing import List, Optional
 
 
-@dataclasses.dataclass
-class GetSearchResultsRequest:
-    query: str = dataclasses.field(metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
-    r"""The search query string to use"""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetSearchResultsPart:
-    id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+class Directory:
+    count: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('count'), 'exclude': lambda f: f is None }})
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
-    duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
-    file: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file'), 'exclude': lambda f: f is None }})
-    size: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
-    audio_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioProfile'), 'exclude': lambda f: f is None }})
-    container: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('container'), 'exclude': lambda f: f is None }})
-    video_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoProfile'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetSearchResultsMedia:
-    id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
-    bitrate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bitrate'), 'exclude': lambda f: f is None }})
-    width: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is None }})
-    height: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is None }})
-    aspect_ratio: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aspectRatio'), 'exclude': lambda f: f is None }})
-    audio_channels: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioChannels'), 'exclude': lambda f: f is None }})
-    audio_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioCodec'), 'exclude': lambda f: f is None }})
-    video_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoCodec'), 'exclude': lambda f: f is None }})
-    video_resolution: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoResolution'), 'exclude': lambda f: f is None }})
-    container: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('container'), 'exclude': lambda f: f is None }})
-    video_frame_rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoFrameRate'), 'exclude': lambda f: f is None }})
-    audio_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioProfile'), 'exclude': lambda f: f is None }})
-    video_profile: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoProfile'), 'exclude': lambda f: f is None }})
-    part: Optional[List[GetSearchResultsPart]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Part'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetSearchResultsGenre:
-    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetSearchResultsDirector:
-    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetSearchResultsWriter:
-    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetSearchResultsCountry:
-    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetSearchResultsRole:
-    tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetSearchResultsMetadata:
-    allow_sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSync'), 'exclude': lambda f: f is None }})
-    library_section_id: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionID'), 'exclude': lambda f: f is None }})
-    library_section_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionTitle'), 'exclude': lambda f: f is None }})
-    library_section_uuid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('librarySectionUUID'), 'exclude': lambda f: f is None }})
-    personal: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('personal'), 'exclude': lambda f: f is None }})
-    source_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceTitle'), 'exclude': lambda f: f is None }})
-    rating_key: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingKey'), 'exclude': lambda f: f is None }})
-    key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
-    guid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('guid'), 'exclude': lambda f: f is None }})
-    studio: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('studio'), 'exclude': lambda f: f is None }})
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
     title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
-    content_rating: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentRating'), 'exclude': lambda f: f is None }})
-    summary: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('summary'), 'exclude': lambda f: f is None }})
-    rating: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rating'), 'exclude': lambda f: f is None }})
-    audience_rating: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audienceRating'), 'exclude': lambda f: f is None }})
-    year: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('year'), 'exclude': lambda f: f is None }})
-    tagline: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tagline'), 'exclude': lambda f: f is None }})
-    thumb: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('thumb'), 'exclude': lambda f: f is None }})
-    art: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('art'), 'exclude': lambda f: f is None }})
-    duration: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
-    originally_available_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('originallyAvailableAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
-    added_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('addedAt'), 'exclude': lambda f: f is None }})
-    updated_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'exclude': lambda f: f is None }})
-    audience_rating_image: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audienceRatingImage'), 'exclude': lambda f: f is None }})
-    chapter_source: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('chapterSource'), 'exclude': lambda f: f is None }})
-    primary_extra_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('primaryExtraKey'), 'exclude': lambda f: f is None }})
-    rating_image: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingImage'), 'exclude': lambda f: f is None }})
-    media: Optional[List[GetSearchResultsMedia]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Media'), 'exclude': lambda f: f is None }})
-    genre: Optional[List[GetSearchResultsGenre]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Genre'), 'exclude': lambda f: f is None }})
-    director: Optional[List[GetSearchResultsDirector]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Director'), 'exclude': lambda f: f is None }})
-    writer: Optional[List[GetSearchResultsWriter]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Writer'), 'exclude': lambda f: f is None }})
-    country: Optional[List[GetSearchResultsCountry]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Country'), 'exclude': lambda f: f is None }})
-    role: Optional[List[GetSearchResultsRole]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Role'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Provider:
-    key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
-    title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetSearchResultsMediaContainer:
+class MediaContainer:
     size: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
-    identifier: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('identifier'), 'exclude': lambda f: f is None }})
-    media_tag_prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaTagPrefix'), 'exclude': lambda f: f is None }})
-    media_tag_version: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaTagVersion'), 'exclude': lambda f: f is None }})
-    metadata: Optional[List[GetSearchResultsMetadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Metadata'), 'exclude': lambda f: f is None }})
-    provider: Optional[List[Provider]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Provider'), 'exclude': lambda f: f is None }})
+    allow_camera_upload: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowCameraUpload'), 'exclude': lambda f: f is None }})
+    allow_channel_access: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowChannelAccess'), 'exclude': lambda f: f is None }})
+    allow_media_deletion: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowMediaDeletion'), 'exclude': lambda f: f is None }})
+    allow_sharing: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSharing'), 'exclude': lambda f: f is None }})
+    allow_sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSync'), 'exclude': lambda f: f is None }})
+    allow_tuners: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowTuners'), 'exclude': lambda f: f is None }})
+    background_processing: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('backgroundProcessing'), 'exclude': lambda f: f is None }})
+    certificate: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('certificate'), 'exclude': lambda f: f is None }})
+    companion_proxy: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companionProxy'), 'exclude': lambda f: f is None }})
+    country_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('countryCode'), 'exclude': lambda f: f is None }})
+    diagnostics: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('diagnostics'), 'exclude': lambda f: f is None }})
+    event_stream: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventStream'), 'exclude': lambda f: f is None }})
+    friendly_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('friendlyName'), 'exclude': lambda f: f is None }})
+    hub_search: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hubSearch'), 'exclude': lambda f: f is None }})
+    item_clusters: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemClusters'), 'exclude': lambda f: f is None }})
+    livetv: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('livetv'), 'exclude': lambda f: f is None }})
+    machine_identifier: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('machineIdentifier'), 'exclude': lambda f: f is None }})
+    media_providers: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaProviders'), 'exclude': lambda f: f is None }})
+    multiuser: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('multiuser'), 'exclude': lambda f: f is None }})
+    music_analysis: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('musicAnalysis'), 'exclude': lambda f: f is None }})
+    my_plex: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('myPlex'), 'exclude': lambda f: f is None }})
+    my_plex_mapping_state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('myPlexMappingState'), 'exclude': lambda f: f is None }})
+    my_plex_signin_state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('myPlexSigninState'), 'exclude': lambda f: f is None }})
+    my_plex_subscription: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('myPlexSubscription'), 'exclude': lambda f: f is None }})
+    my_plex_username: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('myPlexUsername'), 'exclude': lambda f: f is None }})
+    offline_transcode: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('offlineTranscode'), 'exclude': lambda f: f is None }})
+    owner_features: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerFeatures'), 'exclude': lambda f: f is None }})
+    photo_auto_tag: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoAutoTag'), 'exclude': lambda f: f is None }})
+    platform: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platform'), 'exclude': lambda f: f is None }})
+    platform_version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platformVersion'), 'exclude': lambda f: f is None }})
+    plugin_host: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pluginHost'), 'exclude': lambda f: f is None }})
+    push_notifications: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pushNotifications'), 'exclude': lambda f: f is None }})
+    read_only_libraries: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('readOnlyLibraries'), 'exclude': lambda f: f is None }})
+    streaming_brain_abr_version: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streamingBrainABRVersion'), 'exclude': lambda f: f is None }})
+    streaming_brain_version: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streamingBrainVersion'), 'exclude': lambda f: f is None }})
+    sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sync'), 'exclude': lambda f: f is None }})
+    transcoder_active_video_sessions: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderActiveVideoSessions'), 'exclude': lambda f: f is None }})
+    transcoder_audio: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderAudio'), 'exclude': lambda f: f is None }})
+    transcoder_lyrics: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderLyrics'), 'exclude': lambda f: f is None }})
+    transcoder_photo: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderPhoto'), 'exclude': lambda f: f is None }})
+    transcoder_subtitles: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderSubtitles'), 'exclude': lambda f: f is None }})
+    transcoder_video: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderVideo'), 'exclude': lambda f: f is None }})
+    transcoder_video_bitrates: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderVideoBitrates'), 'exclude': lambda f: f is None }})
+    transcoder_video_qualities: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderVideoQualities'), 'exclude': lambda f: f is None }})
+    transcoder_video_resolutions: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderVideoResolutions'), 'exclude': lambda f: f is None }})
+    updated_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'exclude': lambda f: f is None }})
+    updater: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updater'), 'exclude': lambda f: f is None }})
+    version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('version'), 'exclude': lambda f: f is None }})
+    voice_search: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('voiceSearch'), 'exclude': lambda f: f is None }})
+    directory: Optional[List[Directory]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Directory'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetSearchResultsResponseBody:
-    r"""Search Results"""
-    media_container: Optional[GetSearchResultsMediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
+class GetServerCapabilitiesResponseBody:
+    r"""The Server Capabilities"""
+    media_container: Optional[MediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclasses.dataclass
-class GetSearchResultsResponse:
+class GetServerCapabilitiesResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    object: Optional[GetSearchResultsResponseBody] = dataclasses.field(default=None)
-    r"""Search Results"""
+    object: Optional[GetServerCapabilitiesResponseBody] = dataclasses.field(default=None)
+    r"""The Server Capabilities"""
```

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getserveractivities.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getservercapabilities.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/gettranscodesessions.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,94 +6,66 @@
 from dataclasses_json import Undefined, dataclass_json
 from plex_api import utils
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Directory:
-    count: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('count'), 'exclude': lambda f: f is None }})
+class TranscodeSession:
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
-    title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
+    throttled: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('throttled'), 'exclude': lambda f: f is None }})
+    complete: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('complete'), 'exclude': lambda f: f is None }})
+    progress: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('progress'), 'exclude': lambda f: f is None }})
+    size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
+    speed: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('speed'), 'exclude': lambda f: f is None }})
+    error: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
+    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
+    remaining: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('remaining'), 'exclude': lambda f: f is None }})
+    context: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('context'), 'exclude': lambda f: f is None }})
+    source_video_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceVideoCodec'), 'exclude': lambda f: f is None }})
+    source_audio_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceAudioCodec'), 'exclude': lambda f: f is None }})
+    video_decision: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoDecision'), 'exclude': lambda f: f is None }})
+    audio_decision: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioDecision'), 'exclude': lambda f: f is None }})
+    subtitle_decision: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtitleDecision'), 'exclude': lambda f: f is None }})
+    protocol: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('protocol'), 'exclude': lambda f: f is None }})
+    container: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('container'), 'exclude': lambda f: f is None }})
+    video_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoCodec'), 'exclude': lambda f: f is None }})
+    audio_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioCodec'), 'exclude': lambda f: f is None }})
+    audio_channels: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioChannels'), 'exclude': lambda f: f is None }})
+    transcode_hw_requested: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcodeHwRequested'), 'exclude': lambda f: f is None }})
+    time_stamp: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeStamp'), 'exclude': lambda f: f is None }})
+    max_offset_available: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maxOffsetAvailable'), 'exclude': lambda f: f is None }})
+    min_offset_available: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minOffsetAvailable'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class MediaContainer:
-    size: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
-    allow_camera_upload: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowCameraUpload'), 'exclude': lambda f: f is None }})
-    allow_channel_access: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowChannelAccess'), 'exclude': lambda f: f is None }})
-    allow_media_deletion: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowMediaDeletion'), 'exclude': lambda f: f is None }})
-    allow_sharing: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSharing'), 'exclude': lambda f: f is None }})
-    allow_sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSync'), 'exclude': lambda f: f is None }})
-    allow_tuners: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowTuners'), 'exclude': lambda f: f is None }})
-    background_processing: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('backgroundProcessing'), 'exclude': lambda f: f is None }})
-    certificate: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('certificate'), 'exclude': lambda f: f is None }})
-    companion_proxy: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companionProxy'), 'exclude': lambda f: f is None }})
-    country_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('countryCode'), 'exclude': lambda f: f is None }})
-    diagnostics: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('diagnostics'), 'exclude': lambda f: f is None }})
-    event_stream: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventStream'), 'exclude': lambda f: f is None }})
-    friendly_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('friendlyName'), 'exclude': lambda f: f is None }})
-    hub_search: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hubSearch'), 'exclude': lambda f: f is None }})
-    item_clusters: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemClusters'), 'exclude': lambda f: f is None }})
-    livetv: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('livetv'), 'exclude': lambda f: f is None }})
-    machine_identifier: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('machineIdentifier'), 'exclude': lambda f: f is None }})
-    media_providers: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaProviders'), 'exclude': lambda f: f is None }})
-    multiuser: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('multiuser'), 'exclude': lambda f: f is None }})
-    music_analysis: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('musicAnalysis'), 'exclude': lambda f: f is None }})
-    my_plex: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('myPlex'), 'exclude': lambda f: f is None }})
-    my_plex_mapping_state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('myPlexMappingState'), 'exclude': lambda f: f is None }})
-    my_plex_signin_state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('myPlexSigninState'), 'exclude': lambda f: f is None }})
-    my_plex_subscription: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('myPlexSubscription'), 'exclude': lambda f: f is None }})
-    my_plex_username: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('myPlexUsername'), 'exclude': lambda f: f is None }})
-    offline_transcode: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('offlineTranscode'), 'exclude': lambda f: f is None }})
-    owner_features: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerFeatures'), 'exclude': lambda f: f is None }})
-    photo_auto_tag: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoAutoTag'), 'exclude': lambda f: f is None }})
-    platform: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platform'), 'exclude': lambda f: f is None }})
-    platform_version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('platformVersion'), 'exclude': lambda f: f is None }})
-    plugin_host: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pluginHost'), 'exclude': lambda f: f is None }})
-    push_notifications: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pushNotifications'), 'exclude': lambda f: f is None }})
-    read_only_libraries: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('readOnlyLibraries'), 'exclude': lambda f: f is None }})
-    streaming_brain_abr_version: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streamingBrainABRVersion'), 'exclude': lambda f: f is None }})
-    streaming_brain_version: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streamingBrainVersion'), 'exclude': lambda f: f is None }})
-    sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sync'), 'exclude': lambda f: f is None }})
-    transcoder_active_video_sessions: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderActiveVideoSessions'), 'exclude': lambda f: f is None }})
-    transcoder_audio: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderAudio'), 'exclude': lambda f: f is None }})
-    transcoder_lyrics: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderLyrics'), 'exclude': lambda f: f is None }})
-    transcoder_photo: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderPhoto'), 'exclude': lambda f: f is None }})
-    transcoder_subtitles: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderSubtitles'), 'exclude': lambda f: f is None }})
-    transcoder_video: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderVideo'), 'exclude': lambda f: f is None }})
-    transcoder_video_bitrates: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderVideoBitrates'), 'exclude': lambda f: f is None }})
-    transcoder_video_qualities: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderVideoQualities'), 'exclude': lambda f: f is None }})
-    transcoder_video_resolutions: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcoderVideoResolutions'), 'exclude': lambda f: f is None }})
-    updated_at: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'exclude': lambda f: f is None }})
-    updater: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updater'), 'exclude': lambda f: f is None }})
-    version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('version'), 'exclude': lambda f: f is None }})
-    voice_search: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('voiceSearch'), 'exclude': lambda f: f is None }})
-    directory: Optional[List[Directory]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Directory'), 'exclude': lambda f: f is None }})
+class GetTranscodeSessionsMediaContainer:
+    size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
+    transcode_session: Optional[List[TranscodeSession]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('TranscodeSession'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetServerCapabilitiesResponseBody:
-    r"""The Server Capabilities"""
-    media_container: Optional[MediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
+class GetTranscodeSessionsResponseBody:
+    r"""The Transcode Sessions"""
+    media_container: Optional[GetTranscodeSessionsMediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclasses.dataclass
-class GetServerCapabilitiesResponse:
+class GetTranscodeSessionsResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    object: Optional[GetServerCapabilitiesResponseBody] = dataclasses.field(default=None)
-    r"""The Server Capabilities"""
+    object: Optional[GetTranscodeSessionsResponseBody] = dataclasses.field(default=None)
+    r"""The Transcode Sessions"""
```

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getserveridentity.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getserverlist.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getserverpreferences.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getsessionhistory.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getsessions.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getsourceconnectioninformation.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getstatistics.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/gettimeline.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/gettimeline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/gettoken.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/gettoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/gettranscodesessions.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/searchlibrary.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,96 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
 from plex_api import utils
 from typing import List, Optional
 
+class Type(int, Enum):
+    r"""Plex content type to search for"""
+    ONE = 1
+    TWO = 2
+    THREE = 3
+    FOUR = 4
+
+
+@dataclasses.dataclass
+class SearchLibraryRequest:
+    section_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'sectionId', 'style': 'simple', 'explode': False }})
+    r"""the Id of the library to query"""
+    type: Type = dataclasses.field(metadata={'query_param': { 'field_name': 'type', 'style': 'form', 'explode': True }})
+    r"""Plex content type to search for"""
+    
+
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class TranscodeSession:
+class SearchLibraryMetadata:
+    rating_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ratingKey'), 'exclude': lambda f: f is None }})
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
-    throttled: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('throttled'), 'exclude': lambda f: f is None }})
-    complete: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('complete'), 'exclude': lambda f: f is None }})
-    progress: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('progress'), 'exclude': lambda f: f is None }})
-    size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
-    speed: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('speed'), 'exclude': lambda f: f is None }})
-    error: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
-    remaining: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('remaining'), 'exclude': lambda f: f is None }})
-    context: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('context'), 'exclude': lambda f: f is None }})
-    source_video_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceVideoCodec'), 'exclude': lambda f: f is None }})
-    source_audio_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceAudioCodec'), 'exclude': lambda f: f is None }})
-    video_decision: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoDecision'), 'exclude': lambda f: f is None }})
-    audio_decision: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioDecision'), 'exclude': lambda f: f is None }})
-    subtitle_decision: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtitleDecision'), 'exclude': lambda f: f is None }})
-    protocol: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('protocol'), 'exclude': lambda f: f is None }})
-    container: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('container'), 'exclude': lambda f: f is None }})
-    video_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('videoCodec'), 'exclude': lambda f: f is None }})
-    audio_codec: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioCodec'), 'exclude': lambda f: f is None }})
-    audio_channels: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audioChannels'), 'exclude': lambda f: f is None }})
-    transcode_hw_requested: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transcodeHwRequested'), 'exclude': lambda f: f is None }})
-    time_stamp: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeStamp'), 'exclude': lambda f: f is None }})
-    max_offset_available: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maxOffsetAvailable'), 'exclude': lambda f: f is None }})
-    min_offset_available: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minOffsetAvailable'), 'exclude': lambda f: f is None }})
+    parent_rating_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentRatingKey'), 'exclude': lambda f: f is None }})
+    guid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('guid'), 'exclude': lambda f: f is None }})
+    parent_guid: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentGuid'), 'exclude': lambda f: f is None }})
+    parent_studio: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentStudio'), 'exclude': lambda f: f is None }})
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+    title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
+    parent_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentKey'), 'exclude': lambda f: f is None }})
+    parent_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentTitle'), 'exclude': lambda f: f is None }})
+    summary: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('summary'), 'exclude': lambda f: f is None }})
+    index: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('index'), 'exclude': lambda f: f is None }})
+    parent_index: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentIndex'), 'exclude': lambda f: f is None }})
+    parent_year: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentYear'), 'exclude': lambda f: f is None }})
+    thumb: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('thumb'), 'exclude': lambda f: f is None }})
+    art: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('art'), 'exclude': lambda f: f is None }})
+    parent_thumb: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentThumb'), 'exclude': lambda f: f is None }})
+    parent_theme: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentTheme'), 'exclude': lambda f: f is None }})
+    added_at: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('addedAt'), 'exclude': lambda f: f is None }})
+    updated_at: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetTranscodeSessionsMediaContainer:
+class SearchLibraryMediaContainer:
     size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
-    transcode_session: Optional[List[TranscodeSession]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('TranscodeSession'), 'exclude': lambda f: f is None }})
+    allow_sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allowSync'), 'exclude': lambda f: f is None }})
+    art: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('art'), 'exclude': lambda f: f is None }})
+    identifier: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('identifier'), 'exclude': lambda f: f is None }})
+    media_tag_prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaTagPrefix'), 'exclude': lambda f: f is None }})
+    media_tag_version: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mediaTagVersion'), 'exclude': lambda f: f is None }})
+    nocache: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nocache'), 'exclude': lambda f: f is None }})
+    thumb: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('thumb'), 'exclude': lambda f: f is None }})
+    title1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title1'), 'exclude': lambda f: f is None }})
+    title2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title2'), 'exclude': lambda f: f is None }})
+    view_group: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('viewGroup'), 'exclude': lambda f: f is None }})
+    view_mode: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('viewMode'), 'exclude': lambda f: f is None }})
+    metadata: Optional[List[SearchLibraryMetadata]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('Metadata'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetTranscodeSessionsResponseBody:
-    r"""The Transcode Sessions"""
-    media_container: Optional[GetTranscodeSessionsMediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
+class SearchLibraryResponseBody:
+    r"""The contents of the library by section and type"""
+    media_container: Optional[SearchLibraryMediaContainer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MediaContainer'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclasses.dataclass
-class GetTranscodeSessionsResponse:
+class SearchLibraryResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    object: Optional[GetTranscodeSessionsResponseBody] = dataclasses.field(default=None)
-    r"""The Transcode Sessions"""
+    object: Optional[SearchLibraryResponseBody] = dataclasses.field(default=None)
+    r"""The contents of the library by section and type"""
```

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/gettransienttoken.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/gettransienttoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/getupdatestatus.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/logline.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/logline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/logmultiline.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/markplayed.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/markunplayed.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/performsearch.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/performvoicesearch.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/refreshlibrary.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/startalltasks.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/starttask.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/starttask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/startuniversaltranscode.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/stopalltasks.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/stoptask.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/stoptask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/stoptranscodesession.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/updateplaylist.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/updateplayprogress.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/models/operations/uploadplaylist.py` & `plex-api-client-0.7.0/src/plex_api/models/operations/uploadplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/playlists.py` & `plex-api-client-0.7.0/src/plex_api/playlists.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,23 +60,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreatePlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreatePlaylistResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.CreatePlaylistResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -130,23 +132,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPlaylistsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetPlaylistsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetPlaylistsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -199,23 +203,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetPlaylistResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetPlaylistResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -271,14 +277,15 @@
         res = operations.DeletePlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.DeletePlaylistResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -337,14 +344,15 @@
         res = operations.UpdatePlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.UpdatePlaylistResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -401,23 +409,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPlaylistContentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetPlaylistContentsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetPlaylistContentsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -473,14 +483,15 @@
         res = operations.ClearPlaylistContentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ClearPlaylistContentsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -536,23 +547,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.AddPlaylistContentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.AddPlaylistContentsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.AddPlaylistContentsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -610,14 +623,15 @@
         res = operations.UploadPlaylistResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.UploadPlaylistResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/plex.py` & `plex-api-client-0.7.0/src/plex_api/plex.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,21 +65,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPinResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetPinResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetPinResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -143,14 +145,15 @@
         
         
         res = operations.GetTokenResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetTokenResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/sdk.py` & `plex-api-client-0.7.0/src/plex_api/sdk.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/sdkconfiguration.py` & `plex-api-client-0.7.0/src/plex_api/sdkconfiguration.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     server_defaults: List[Dict[str, str]] = field(default_factory=List)
     language: str = 'python'
     openapi_doc_version: str = '0.0.3'
-    sdk_version: str = '0.6.6'
-    gen_version: str = '2.319.10'
-    user_agent: str = 'speakeasy-sdk/python 0.6.6 2.319.10 0.0.3 plex-api-client'
+    sdk_version: str = '0.7.0'
+    gen_version: str = '2.326.3'
+    user_agent: str = 'speakeasy-sdk/python 0.7.0 2.326.3 0.0.3 plex-api-client'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `plex-api-client-0.6.6/src/plex_api/search.py` & `plex-api-client-0.7.0/src/plex_api/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         res = operations.PerformSearchResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.PerformSearchResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -144,14 +145,15 @@
         res = operations.PerformVoiceSearchResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.PerformVoiceSearchResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -204,23 +206,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetSearchResultsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetSearchResultsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetSearchResultsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/server.py` & `plex-api-client-0.7.0/src/plex_api/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,23 +53,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetServerCapabilitiesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetServerCapabilitiesResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetServerCapabilitiesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -117,23 +119,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetServerPreferencesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetServerPreferencesResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetServerPreferencesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -181,23 +185,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAvailableClientsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetAvailableClientsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetAvailableClientsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -245,23 +251,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetDevicesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDevicesResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetDevicesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -309,23 +317,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetServerIdentityResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetServerIdentityResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetServerIdentityResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -373,23 +383,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetMyPlexAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetMyPlexAccountResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetMyPlexAccountResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -442,14 +454,15 @@
         res = operations.GetResizedPhotoResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetResizedPhotoResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -497,23 +510,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetServerListResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetServerListResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetServerListResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/sessions.py` & `plex-api-client-0.7.0/src/plex_api/sessions.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,23 +53,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetSessionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetSessionsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetSessionsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -117,23 +119,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetSessionHistoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetSessionHistoryResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetSessionHistoryResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -181,23 +185,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetTranscodeSessionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetTranscodeSessionsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetTranscodeSessionsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -253,14 +259,15 @@
         res = operations.StopTranscodeSessionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.StopTranscodeSessionResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/statistics.py` & `plex-api-client-0.7.0/src/plex_api/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,23 +58,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetStatisticsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetStatisticsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetStatisticsResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/updater.py` & `plex-api-client-0.7.0/src/plex_api/updater.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,23 +55,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUpdateStatusResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetUpdateStatusResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetUpdateStatusResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -128,14 +130,15 @@
         res = operations.CheckForUpdatesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.CheckForUpdatesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -193,14 +196,15 @@
         res = operations.ApplyUpdatesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code == 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ApplyUpdatesResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api/utils/retries.py` & `plex-api-client-0.7.0/src/plex_api/utils/retries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.6/src/plex_api/utils/utils.py` & `plex-api-client-0.7.0/src/plex_api/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -904,14 +904,41 @@
 
 
 def bigintdecoder(val):
     if isinstance(val, float):
         raise ValueError(f"{val} is a float")
     return int(val)
 
+def integerstrencoder(optional: bool):
+    def integerstrencode(val: int):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return integerstrencode
+
+
+def integerstrdecoder(val):
+    if isinstance(val, float):
+        raise ValueError(f"{val} is a float")
+    return int(val)
+
+
+def numberstrencoder(optional: bool):
+    def numberstrencode(val: float):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return numberstrencode
+
+
+def numberstrdecoder(val):
+    return float(val)
+
 
 def decimalencoder(optional: bool, as_str: bool):
     def decimalencode(val: Decimal):
         if optional and val is None:
             return None
 
         if as_str:
```

### Comparing `plex-api-client-0.6.6/src/plex_api/video.py` & `plex-api-client-0.7.0/src/plex_api/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         res = operations.GetTimelineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.GetTimelineResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
@@ -117,14 +118,15 @@
         res = operations.StartUniversalTranscodeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.StartUniversalTranscodeResponseBody)
                 out.raw_response = http_res
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `plex-api-client-0.6.6/src/plex_api_client.egg-info/PKG-INFO` & `plex-api-client-0.7.0/src/plex_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.6.6
+Version: 0.7.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/LukeHagar/plexpy.git
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
@@ -31,15 +31,14 @@
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
-        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -97,15 +96,14 @@
         ### [library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md)
         
         * [get_file_hash](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_file_hash) - Get Hash Value
         * [get_recently_added](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_recently_added) - Get Recently Added
         * [get_libraries](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_libraries) - Get All Libraries
         * [get_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_library) - Get Library Details
         * [delete_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#delete_library) - Delete Library Section
-        * [get_library_items](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_library_items) - Get Library Items
         * [refresh_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#refresh_library) - Refresh Library
         * [search_library](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#search_library) - Search Library
         * [get_metadata](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_metadata) - Get Items Metadata
         * [get_metadata_children](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_metadata_children) - Get Items Children
         * [get_on_deck](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_on_deck) - Get On Deck
         
         ### [log](https://github.com/LukeHagar/plexpy/blob/master/docs/sdks/log/README.md)
@@ -171,15 +169,14 @@
         from plex_api.models import errors
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
-        
         res = None
         try:
             res = s.server.get_server_capabilities()
         except errors.GetServerCapabilitiesResponseBody as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
@@ -211,15 +208,14 @@
         
         s = plex_api.PlexAPI(
             server_idx=0,
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
-        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -239,15 +235,14 @@
         
         s = plex_api.PlexAPI(
             server_url="{protocol}://{ip}:{port}",
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
-        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -258,16 +253,15 @@
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             x_plex_client_identifier='Postman',
         )
         
-        
-        res = s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False, x_plex_client_identifier='Postman')
+        res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman', server_url="https://plex.tv/api/v2")
         
         if res.object is not None:
             # handle response
             pass
         
         ```
         <!-- End Server Selection [server] -->
@@ -304,15 +298,14 @@
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
             x_plex_client_identifier='Postman',
         )
         
-        
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
             pass
         
         ```
@@ -343,15 +336,14 @@
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             x_plex_client_identifier='Postman',
         )
         
-        
         res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman')
         
         if res.object is not None:
             # handle response
             pass
         
         ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.6 Summary: Python
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.7.0 Summary: Python
 Client SDK Generated by Speakeasy Home-page: https://github.com/LukeHagar/
 plexpy.git Author: LukeHagar License: UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
@@ -71,17 +71,15 @@
 //github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#get_recently_added) - Get Recently Added * [get_libraries](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#get_libraries) - Get All Libraries * [get_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#get_library) - Get Library Details * [delete_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
-README.md#delete_library) - Delete Library Section * [get_library_items](https:
-//github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
-README.md#get_library_items) - Get Library Items * [refresh_library](https://
+README.md#delete_library) - Delete Library Section * [refresh_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#refresh_library) - Refresh Library * [search_library](https://
 github.com/LukeHagar/plexpy/blob/master/docs/sdks/library/
 README.md#search_library) - Search Library * [get_metadata](https://github.com/
 LukeHagar/plexpy/blob/master/docs/sdks/library/README.md#get_metadata) - Get
 Items Metadata * [get_metadata_children](https://github.com/LukeHagar/plexpy/
 blob/master/docs/sdks/library/README.md#get_metadata_children) - Get Items
@@ -172,16 +170,16 @@
 optional parameter when initializing the SDK client instance. For example:
 ```python import plex_api s = plex_api.PlexAPI( server_url="{protocol}://{ip}:
 {port}", access_token="", x_plex_client_identifier='Postman', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
 pass ``` ### Override Server URL Per-Operation The server URL can also be
 overridden on a per-operation basis, provided a server list was specified for
 the operation. For example: ```python import plex_api s = plex_api.PlexAPI
-( x_plex_client_identifier='Postman', ) res = s.plex.get_pin(server_url="https:
-//plex.tv/api/v2", strong=False, x_plex_client_identifier='Postman') if
+( x_plex_client_identifier='Postman', ) res = s.plex.get_pin(strong=False,
+x_plex_client_identifier='Postman', server_url="https://plex.tv/api/v2") if
 res.object is not None: # handle response pass ``` ## Custom HTTP Client The
 Python SDK makes API calls using the [requests](https://pypi.org/project/
 requests/) HTTP library. In order to provide a convenient way to configure
 timeouts, cookies, proxies, custom headers, and other low-level configuration,
 you can initialize the SDK client with a custom `requests.Session` object. For
 example, you could specify a header for every request that this sdk makes as
 follows: ```python import plex_api import requests http_client =
```

### Comparing `plex-api-client-0.6.6/src/plex_api_client.egg-info/SOURCES.txt` & `plex-api-client-0.7.0/src/plex_api_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,14 @@
 src/plex_api/models/operations/getbutlertasks.py
 src/plex_api/models/operations/getdevices.py
 src/plex_api/models/operations/getfilehash.py
 src/plex_api/models/operations/getglobalhubs.py
 src/plex_api/models/operations/getlibraries.py
 src/plex_api/models/operations/getlibrary.py
 src/plex_api/models/operations/getlibraryhubs.py
-src/plex_api/models/operations/getlibraryitems.py
 src/plex_api/models/operations/getmetadata.py
 src/plex_api/models/operations/getmetadatachildren.py
 src/plex_api/models/operations/getmyplexaccount.py
 src/plex_api/models/operations/getondeck.py
 src/plex_api/models/operations/getpin.py
 src/plex_api/models/operations/getplaylist.py
 src/plex_api/models/operations/getplaylistcontents.py
```

