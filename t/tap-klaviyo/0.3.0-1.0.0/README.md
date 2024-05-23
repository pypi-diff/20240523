# Comparing `tmp/tap-klaviyo-0.3.0.tar.gz` & `tmp/tap_klaviyo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-klaviyo-0.3.0.tar", last modified: Mon Jun 13 20:33:26 2022, max compression
+gzip compressed data, was "tap_klaviyo-1.0.0.tar", last modified: Thu May 23 11:25:03 2024, max compression
```

## Comparing `tap-klaviyo-0.3.0.tar` & `tap_klaviyo-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,50 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-06-13 20:33:26.525933 tap-klaviyo-0.3.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34520 2021-10-08 20:12:44.000000 tap-klaviyo-0.3.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2022-06-13 20:33:26.525933 tap-klaviyo-0.3.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2907 2021-12-01 22:41:40.000000 tap-klaviyo-0.3.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-06-13 20:33:26.525933 tap-klaviyo-0.3.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      750 2022-06-13 20:32:15.000000 tap-klaviyo-0.3.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-06-13 20:33:26.509933 tap-klaviyo-0.3.0/tap_klaviyo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6280 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-06-13 20:33:26.521933 tap-klaviyo-0.3.0/tap_klaviyo/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/bounce.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3176 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/campaigns.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/click.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/clicked_sms.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/consented_to_receive.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/dropped_email.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/failed_to_deliver.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/failed_to_deliver_automated_response.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      389 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/global_exclusions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      717 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/lists.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/mark_as_spam.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/open.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/receive.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/received_automated_response.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/received_sms.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/sent_sms.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-06-13 20:33:26.521933 tap-klaviyo-0.3.0/tap_klaviyo/schemas/shared/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      983 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/shared/event.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/subscribe_list.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/unsub_list.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/unsubscribe.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/unsubscribed_from_sms.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/schemas/update_email_preferences.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8291 2022-06-08 22:01:06.000000 tap-klaviyo-0.3.0/tap_klaviyo/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-06-13 20:33:26.513933 tap-klaviyo-0.3.0/tap_klaviyo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2022-06-13 20:33:26.000000 tap-klaviyo-0.3.0/tap_klaviyo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1168 2022-06-13 20:33:26.000000 tap-klaviyo-0.3.0/tap_klaviyo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-06-13 20:33:26.000000 tap-klaviyo-0.3.0/tap_klaviyo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2022-06-13 20:33:26.000000 tap-klaviyo-0.3.0/tap_klaviyo.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-06-13 20:33:26.000000 tap-klaviyo-0.3.0/tap_klaviyo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-06-13 20:33:26.000000 tap-klaviyo-0.3.0/tap_klaviyo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:25:03.067510 tap_klaviyo-1.0.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34520 2022-05-26 07:48:47.000000 tap_klaviyo-1.0.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      308 2024-05-23 11:25:03.067510 tap_klaviyo-1.0.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2923 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 11:25:03.067510 tap_klaviyo-1.0.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      750 2024-05-23 11:18:39.000000 tap_klaviyo-1.0.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:25:03.059509 tap_klaviyo-1.0.0/tap_klaviyo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6591 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tap_klaviyo/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:25:03.067510 tap_klaviyo-1.0.0/tap_klaviyo/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/bounce.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5918 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/campaigns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/click.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/clicked_sms.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/dropped_email.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/failed_to_deliver.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/failed_to_deliver_automated_response.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1662 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/global_exclusions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1148 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/lists.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/mark_as_spam.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/open.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/receive.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/received_automated_response.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/received_sms.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/sent_sms.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:25:03.067510 tap_klaviyo-1.0.0/tap_klaviyo/schemas/shared/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3719 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/shared/event.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/subscribe_list.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/subscribed_to_email.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/subscribed_to_sms.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/unsub_list.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/unsubscribe.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/unsubscribed_from_sms.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2022-09-11 20:52:24.000000 tap_klaviyo-1.0.0/tap_klaviyo/schemas/update_email_preferences.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11371 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tap_klaviyo/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:25:03.067510 tap_klaviyo-1.0.0/tap_klaviyo.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      308 2024-05-23 11:25:02.000000 tap_klaviyo-1.0.0/tap_klaviyo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1445 2024-05-23 11:25:03.000000 tap_klaviyo-1.0.0/tap_klaviyo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 11:25:02.000000 tap_klaviyo-1.0.0/tap_klaviyo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2024-05-23 11:25:02.000000 tap_klaviyo-1.0.0/tap_klaviyo.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 11:25:02.000000 tap_klaviyo-1.0.0/tap_klaviyo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2024-05-23 11:25:02.000000 tap_klaviyo-1.0.0/tap_klaviyo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:25:03.067510 tap_klaviyo-1.0.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3948 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tests/test_klaviyo_all_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3450 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tests/test_klaviyo_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9538 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tests/test_klaviyo_bookmark.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6315 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tests/test_klaviyo_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3097 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tests/test_klaviyo_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7815 2024-05-23 10:46:08.000000 tap_klaviyo-1.0.0/tests/test_klaviyo_start_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      881 2022-05-26 07:48:47.000000 tap_klaviyo-1.0.0/tests/test_klaviyo_sync_canary.py
```

### Comparing `tap-klaviyo-0.3.0/LICENSE` & `tap_klaviyo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-klaviyo-0.3.0/README.md` & `tap_klaviyo-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # tap-klaviyo
 
 This is a [Singer](https://singer.io) tap that produces JSON-formatted
 data from the Klaviyo API following the [Singer
 spec](https://github.com/singer-io/getting-started/blob/master/SPEC.md).
 
 This tap:
-- Pulls raw data from the [Klaviyo metrics API](https://www.klaviyo.com/docs/api/metrics)
+- Pulls raw data from the [Klaviyo metrics API](https://developers.klaviyo.com/en/reference/api_overview)
 - Outputs the schema for each resource
 - Incrementally pulls data based on the input state for incremental endpoints
 - Updates full tables for global exclusions and lists endpoints
 
 Singer taps function in two modes: [discovery mode](https://github.com/singer-io/getting-started/blob/master/docs/DISCOVERY_MODE.md) and [sync mode](https://github.com/singer-io/getting-started/blob/master/docs/SYNC_MODE.md). Before running the tap in sync mode, you should run the tap in discovery mode and direct the output to a file called catalog.json, which can be used as an input to run the tap in sync mode and to specify which streams should be synced (see Step 4).
 
 ## Quick start
```

### Comparing `tap-klaviyo-0.3.0/tap_klaviyo/__init__.py` & `tap_klaviyo-1.0.0/tap_klaviyo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 #!/usr/bin/env/python
 
 import json
 import os
 import sys
 import singer
 from singer import metadata
-from tap_klaviyo.utils import get_incremental_pull, get_full_pulls, get_all_pages
+from tap_klaviyo.utils import get_incremental_pull, get_full_pulls, get_all_using_next
 
 LOGGER = singer.get_logger()
 
+API_VERSION = "2024-02-15"
+
+# For stream global_exclusions, data related to suppressed users can be found in the /api/profiles endpoint
 ENDPOINTS = {
-    'global_exclusions': 'https://a.klaviyo.com/api/v1/people/exclusions',
-    'lists': 'https://a.klaviyo.com/api/v1/lists',
-    'metrics': 'https://a.klaviyo.com/api/v1/metrics',
-    'metric': 'https://a.klaviyo.com/api/v1/metric/',
-    'campaigns': 'https://a.klaviyo.com/api/v1/campaigns'
+    'global_exclusions': 'https://a.klaviyo.com/api/profiles',
+    'lists': 'https://a.klaviyo.com/api/lists',
+    'metrics': 'https://a.klaviyo.com/api/metrics',
+    'events': 'https://a.klaviyo.com/api/events',
+    'campaigns': 'https://a.klaviyo.com/api/campaigns'
 }
 
 EVENT_MAPPINGS = {
     "Received Email": "receive",
     "Clicked Email": "click",
     "Opened Email": "open",
     "Bounced Email": "bounce",
-    "Unsubscribed": "unsubscribe",
+    "Unsubscribed from Email Marketing": "unsubscribe",
     "Marked Email as Spam": "mark_as_spam",
     "Unsubscribed from List": "unsub_list",
+    "Subscribed to Email Marketing": "subscribed_to_email",
     "Subscribed to List": "subscribe_list",
     "Updated Email Preferences": "update_email_preferences",
     "Dropped Email": "dropped_email",
     "Clicked SMS": "clicked_sms",
-    "Consented to Receive SMS": "consented_to_receive",
+    "Subscribed to SMS Marketing": "subscribed_to_sms",
     "Failed to Deliver SMS": "failed_to_deliver",
     "Failed to deliver Automated Response SMS": "failed_to_deliver_automated_response",
     "Received Automated Response SMS": "received_automated_response",
     "Received SMS": "received_sms",
     "Sent SMS": "sent_sms",
-    "Unsubscribed from SMS": "unsubscribed_from_sms"
+    "Unsubscribed from SMS Marketing": "unsubscribed_from_sms"
 }
 
 
 class Stream(object):
     def __init__(self, stream, tap_stream_id, key_properties, replication_method, replication_keys=None):
         self.stream = stream
         self.tap_stream_id = tap_stream_id
@@ -79,15 +83,15 @@
 
 CREDENTIALS_KEYS = ["api_key"]
 REQUIRED_CONFIG_KEYS = ["start_date"] + CREDENTIALS_KEYS
 
 GLOBAL_EXCLUSIONS = Stream(
     'global_exclusions',
     'global_exclusions',
-    'email',
+    'id',
     'FULL_TABLE'
 )
 
 LISTS = Stream(
     'lists',
     'lists',
     'id',
@@ -122,16 +126,15 @@
     shared_schema_refs = {}
     for shared_file in shared_file_names:
         with open(os.path.join(shared_schemas_path, shared_file)) as data_file:
             shared_schema_refs['shared/' + shared_file] = json.load(data_file)
 
     return shared_schema_refs
 
-def do_sync(config, state, catalog):
-    api_key = config['api_key']
+def do_sync(config, state, catalog, headers):
     start_date = config['start_date'] if 'start_date' in config else None
 
     stream_ids_to_sync = set()
 
     for stream in catalog.get('streams'):
         mdata = metadata.to_map(stream['metadata'])
         if metadata.get(mdata, (), 'selected'):
@@ -143,58 +146,61 @@
         singer.write_schema(
             stream['stream'],
             stream['schema'],
             stream['key_properties']
         )
 
         if stream['stream'] in EVENT_MAPPINGS.values():
-            get_incremental_pull(stream, ENDPOINTS['metric'], state,
-                                 api_key, start_date)
+            get_incremental_pull(stream, ENDPOINTS['events'], state,
+                                 headers, start_date)
         else:
-            get_full_pulls(stream, ENDPOINTS[stream['stream']], api_key)
+            get_full_pulls(stream, ENDPOINTS[stream['stream']], headers)
 
 
-def get_available_metrics(api_key):
+def get_available_metrics(headers):
     metric_streams = []
-    for response in get_all_pages('metric_list',
-                                  ENDPOINTS['metrics'], api_key):
+    for response in get_all_using_next('metric_list',
+                                  ENDPOINTS['metrics'], headers, {}):
         for metric in response.json().get('data'):
-            if metric['name'] in EVENT_MAPPINGS:
+            if metric['attributes']['name'] in EVENT_MAPPINGS:
                 metric_streams.append(
                     Stream(
-                        stream=EVENT_MAPPINGS[metric['name']],
+                        stream=EVENT_MAPPINGS[metric['attributes']['name']],
                         tap_stream_id=metric['id'],
                         key_properties="id",
                         replication_method='INCREMENTAL',
                         replication_keys=["timestamp"]
                     )
                 )
 
     return metric_streams
 
 
-def discover(api_key):
-    metric_streams = get_available_metrics(api_key)
+def discover(headers):
+    metric_streams = get_available_metrics(headers)
     return {"streams": [a.to_catalog_dict()
                         for a in metric_streams + FULL_STREAMS]}
 
 
-def do_discover(api_key):
-    print(json.dumps(discover(api_key), indent=2))
+def do_discover(headers):
+    print(json.dumps(discover(headers), indent=2))
 
 @singer.utils.handle_top_exception(LOGGER)
 def main():
 
     args = singer.utils.parse_args(REQUIRED_CONFIG_KEYS)
+    headers = {
+        "Authorization": f"Klaviyo-API-Key {args.config.get('api_key')}",
+        "revision": API_VERSION
+    }
 
     if args.discover:
-        do_discover(args.config['api_key'])
+        do_discover(headers)
 
     else:
-        catalog = args.catalog.to_dict() if args.catalog else discover(
-             args.config['api_key'])
+        catalog = args.catalog.to_dict() if args.catalog else discover(headers)
 
         state = args.state if args.state else {"bookmarks": {}}
-        do_sync(args.config, state, catalog)
+        do_sync(args.config, state, catalog, headers)
 
 if __name__ == '__main__':
     main()
```

### Comparing `tap-klaviyo-0.3.0/tap_klaviyo/schemas/lists.json` & `tap_klaviyo-1.0.0/tap_klaviyo/schemas/lists.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8295454545454546%*

 * *Differences: {"'properties'": "{'created': {'format': 'date-time'}, 'updated': {'format': 'date-time'}, 'type': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'tags': OrderedDict([('type', "*

 * *                 "['null', 'array']), ('items', OrderedDict([('type', ['null', 'object']), "*

 * *                 "('properties', OrderedDict([('type', OrderedDict([('type', ['null', "*

 * *                 "'string'])])), ('id', OrderedDict([('type', ['null', 'string'])])), ('name', "*

 * *                 "OrderedDict([('type' […]*

```diff
@@ -1,52 +1,74 @@
 {
     "properties": {
         "created": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "folder": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "list_type": {
+        "name": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "name": {
+        "opt_in_process": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "object": {
+        "tags": {
+            "items": {
+                "properties": {
+                    "id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "type": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "person_count": {
+        "type": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "updated": {
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": [
```

### Comparing `tap-klaviyo-0.3.0/tap_klaviyo/utils.py` & `tap_klaviyo-1.0.0/tap_klaviyo/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,47 @@
 
 # set default timeout of 300 seconds
 REQUEST_TIMEOUT = 300
 
 session = requests.Session()
 logger = singer.get_logger()
 
+STREAM_PARAMS_MAP = {
+    "campaigns": [
+        {
+            "filter": "equals(messages.channel,'email')",
+            "include": "tags,campaign-messages"
+        }
+    ],
+    "global_exclusions": [
+        {
+            "filter": "equals(subscriptions.email.marketing.suppression.reason,'HARD_BOUNCE')",
+            "additional-fields[profile]": "subscriptions,predictive_analytics"
+        },
+        {
+            "filter": "equals(subscriptions.email.marketing.suppression.reason,'USER_SUPPRESSED')",
+            "additional-fields[profile]": "subscriptions,predictive_analytics"
+        },
+        {
+            "filter": "equals(subscriptions.email.marketing.suppression.reason,'UNSUBSCRIBE')",
+            "additional-fields[profile]": "subscriptions,predictive_analytics"
+        },
+        {
+            "filter": "equals(subscriptions.email.marketing.suppression.reason,'INVALID_EMAIL')",
+            "additional-fields[profile]": "subscriptions,predictive_analytics"
+        }
+    ],
+    "lists": [
+        {
+            "include": "tags"
+        }
+    ]
+
+}
+
 class KlaviyoError(Exception):
     pass
 
 class KlaviyoBackoffError(KlaviyoError):
     pass
 
 class KlaviyoNotFoundError(KlaviyoError):
@@ -164,87 +197,101 @@
 def get_latest_event_time(events):
     return ts_to_dt(int(events[-1]['timestamp']) - 1) if len(events) else None
 
 # during 'Timeout' error there is also possibility of 'ConnectionError',
 # hence added backoff for 'ConnectionError' too.
 @backoff.on_exception(backoff.expo, (requests.Timeout, requests.ConnectionError), max_tries=5, factor=2)
 @backoff.on_exception(backoff.expo, (simplejson.scanner.JSONDecodeError, KlaviyoBackoffError), max_tries=3)
-def authed_get(source, url, params):
+def authed_get(source, url, params, headers):
     with metrics.http_request_timer(source) as timer:
-        resp = session.request(method='get', url=url, params=params, timeout=get_request_timeout())
+        resp = requests.get(url=url, params=params, headers=headers, timeout=get_request_timeout())
         
         if resp.status_code != 200:
             raise_for_error(resp)
         else:
             resp.json()
             timer.tags[metrics.Tag.http_status_code] = resp.status_code
             return resp
 
-
-def get_all_using_next(stream, url, api_key, since=None):
-    while True:
-        r = authed_get(stream, url, {'api_key': api_key,
-                                     'since': since,
-                                     'sort': 'asc'})
-        yield r
-        if 'next' in r.json() and r.json()['next']:
-            since = r.json()['next']
-        else:
-            break
-
-
-def get_all_pages(source, url, api_key):
-    page = 0
-    while True:
-        r = authed_get(source, url, {'page': page, 'api_key': api_key})
+def get_all_using_next(stream, url, headers, params):
+    # Paginate till there is a url or next url.
+    while url:
+        r = authed_get(stream, url, params, headers)
+        # Re-initializing params to {} as next url contains all necessary params.
+        params = {}
         yield r
-        if r.json()['end'] < r.json()['total'] - 1:
-            page += 1
-        else:
-            break
+        url = r.json()['links'].get('next', None)
 
-def get_incremental_pull(stream, endpoint, state, api_key, start_date):
+def get_incremental_pull(stream, endpoint, state, headers, start_date):
     latest_event_time = get_starting_point(stream, state, start_date)
 
     with metrics.record_counter(stream['stream']) as counter:
-        url = '{}{}/timeline'.format(
-            endpoint,
-            stream['tap_stream_id']
-        )
-        for response in get_all_using_next(
-                stream['stream'], url, api_key,
-                latest_event_time):
+        params = {
+            "filter": f"equals(metric_id,\"{stream['tap_stream_id']}\"),greater-or-equal(timestamp,{latest_event_time})",
+            "include": "profile,metric",
+            "sort": "datetime"
+        }
+        for response in get_all_using_next(stream['stream'], endpoint, headers, params):
             events = response.json().get('data')
 
             if events:
+                included_list = response.json().get('included', [])
+                # Creating a dict/map of included relationships to optimize computations
+                included = {}
+                for included_relationship in included_list:
+                    included[included_relationship['id']] = included_relationship
                 counter.increment(len(events))
-                transfrom_and_write_records(events, stream)
+                transfrom_and_write_records(events, stream, included, params.get("include","").split(","))
                 update_state(state, stream['stream'], get_latest_event_time(events))
                 singer.write_state(state)
 
     return state
 
-def get_full_pulls(resource, endpoint, api_key):
+def get_full_pulls(resource, endpoint, headers):
 
     with metrics.record_counter(resource['stream']) as counter:
-
-        for response in get_all_pages(resource['stream'], endpoint, api_key):
-            
-            records = response.json().get('data')
-            counter.increment(len(records))
-            transfrom_and_write_records(records, resource)
+        for params in STREAM_PARAMS_MAP.get(resource['stream'],[]):
+            for response in get_all_using_next(resource['stream'], endpoint, headers, params):
+                records = response.json().get('data')
+                included_list = response.json().get('included', [])
+                # Creating a dict/map of included relationships to optimize computations
+                included = {}
+                for included_relationship in included_list:
+                    included[included_relationship['id']] = included_relationship
+                counter.increment(len(records))
+                transfrom_and_write_records(records, resource, included, params.get("include","").split(","))
 
 
-def transfrom_and_write_records(events, stream):
+def transfrom_and_write_records(events, stream, included, valid_relationships):
     event_stream = stream['stream']
     event_schema = stream['schema']
     event_mdata = metadata.to_map(stream['metadata'])
 
     with Transformer() as transformer:
         for event in events:
+            # Flatten the event dict with attributes
+            event.update(event['attributes'])
+            for relationship_key, relationship_value in event.get('relationships',{}).items():
+                if not relationship_key in valid_relationships:
+                    continue
+                relationship_data = relationship_value['data']
+                # Generalizing relationship data to list of dicts for all streams
+                # This is due to the fact that, for Full table streams, data is returned as a list
+                # And, for incremental streams, data is return as a dict in API response
+                if isinstance(relationship_data, dict):
+                    relationship_data = [relationship_data]
+                for relationship in relationship_data:
+                    included_relationship = included.get(relationship['id'], None)
+                    # Check if current relationship is present in included relationship dict
+                    if included_relationship is not None:
+                        # Flatten the included_relationship dict with attributes
+                        included_relationship.update(included_relationship['attributes'])
+                        relationship.update(included_relationship)
+                event.update({relationship_key: relationship_data})
+            # write record
             singer.write_record(
                 event_stream, 
                 transformer.transform(
                     event, event_schema, event_mdata
             ))
 
 # return the 'timeout'
```

