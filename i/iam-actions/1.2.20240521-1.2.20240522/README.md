# Comparing `tmp/iam_actions-1.2.20240521.tar.gz` & `tmp/iam_actions-1.2.20240522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240521.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240522.tar", max compression
```

## Comparing `iam_actions-1.2.20240521.tar` & `iam_actions-1.2.20240522.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-21 02:25:45.754466 iam_actions-1.2.20240521/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-21 02:25:45.754466 iam_actions-1.2.20240521/README.md
--rw-r--r--   0        0        0      228 2024-05-21 02:25:45.754466 iam_actions-1.2.20240521/iam_actions/__init__.py
--rw-r--r--   0        0        0  4837649 2024-05-21 02:27:29.174227 iam_actions-1.2.20240521/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-21 02:25:45.754466 iam_actions-1.2.20240521/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-21 02:25:45.754466 iam_actions-1.2.20240521/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-21 02:25:45.754466 iam_actions-1.2.20240521/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-21 02:25:45.754466 iam_actions-1.2.20240521/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-21 02:25:45.754466 iam_actions-1.2.20240521/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-21 02:25:45.754466 iam_actions-1.2.20240521/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-21 02:25:45.754466 iam_actions-1.2.20240521/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-21 02:25:45.754466 iam_actions-1.2.20240521/iam_actions/generate/services.py
--rw-r--r--   0        0        0   629289 2024-05-21 02:27:29.174227 iam_actions-1.2.20240521/iam_actions/policies.json
--rw-r--r--   0        0        0   209717 2024-05-21 02:27:29.174227 iam_actions-1.2.20240521/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   610673 2024-05-21 02:27:29.174227 iam_actions-1.2.20240521/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-21 02:27:29.874225 iam_actions-1.2.20240521/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240521/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240521/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-22 02:22:51.069751 iam_actions-1.2.20240522/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-22 02:22:51.069751 iam_actions-1.2.20240522/README.md
+-rw-r--r--   0        0        0      228 2024-05-22 02:22:51.069751 iam_actions-1.2.20240522/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4847700 2024-05-22 02:25:07.903173 iam_actions-1.2.20240522/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-22 02:22:51.069751 iam_actions-1.2.20240522/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-22 02:22:51.069751 iam_actions-1.2.20240522/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-22 02:22:51.069751 iam_actions-1.2.20240522/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-22 02:22:51.073751 iam_actions-1.2.20240522/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-22 02:22:51.073751 iam_actions-1.2.20240522/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-22 02:22:51.073751 iam_actions-1.2.20240522/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-22 02:22:51.073751 iam_actions-1.2.20240522/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-22 02:22:51.073751 iam_actions-1.2.20240522/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   631317 2024-05-22 02:25:07.903173 iam_actions-1.2.20240522/iam_actions/policies.json
+-rw-r--r--   0        0        0   209717 2024-05-22 02:25:07.903173 iam_actions-1.2.20240522/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   612218 2024-05-22 02:25:07.903173 iam_actions-1.2.20240522/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-22 02:25:08.587180 iam_actions-1.2.20240522/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240522/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240522/PKG-INFO
```

### Comparing `iam_actions-1.2.20240521/LICENSE` & `iam_actions-1.2.20240522/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240521/README.md` & `iam_actions-1.2.20240522/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240521/iam_actions/actions.json` & `iam_actions-1.2.20240522/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991802427758875%*

 * *Differences: {"'controltower'": "{'ListControlOperations': {'access_level': 'List', 'description': 'Grants "*

 * *                   "permission to list all control operations'}}",*

 * * "'payments'": "{'ListPaymentInstruments': OrderedDict([('access_level', 'Undocumented'), "*

 * *               "('action', 'ListPaymentInstruments'), ('condition_keys', []), ('description', 'Not "*

 * *               "Documented by AWS'), ('orphan', False), ('resources', [])]), 'UntagResource': "*

 * *               "OrderedDict([('access_level', 'Undocumented' […]*

```diff
@@ -38125,18 +38125,18 @@
             "action": "ListBaselines",
             "condition_keys": [],
             "description": "Grants permission to list Baselines",
             "orphan": false,
             "resources": []
         },
         "ListControlOperations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListControlOperations",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all control operations",
             "orphan": false,
             "resources": []
         },
         "ListDirectoryGroups": {
             "access_level": "List",
             "action": "ListDirectoryGroups",
             "condition_keys": [],
@@ -119979,30 +119979,70 @@
             "access_level": "Undocumented",
             "action": "GetPaymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "ListPaymentInstruments": {
+            "access_level": "Undocumented",
+            "action": "ListPaymentInstruments",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListPaymentPreferences": {
             "access_level": "Undocumented",
             "action": "ListPaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "MakePayment": {
             "access_level": "Undocumented",
             "action": "MakePayment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdatePaymentInstrument": {
+            "access_level": "Undocumented",
+            "action": "UpdatePaymentInstrument",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdatePaymentPreferences": {
             "access_level": "Undocumented",
             "action": "UpdatePaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -149538,14 +149578,38 @@
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to create a receipt rule set by cloning an existing one",
             "orphan": false,
             "resources": []
         },
+        "CreateAddonInstance": {
+            "access_level": "Undocumented",
+            "action": "CreateAddonInstance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateAddonSubscription": {
+            "access_level": "Undocumented",
+            "action": "CreateAddonSubscription",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateArchive": {
+            "access_level": "Undocumented",
+            "action": "CreateArchive",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateConfigurationSet": {
             "access_level": "Write",
             "action": "CreateConfigurationSet",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to create a new configuration set",
@@ -149689,14 +149753,22 @@
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to creates an import job for a data destination",
             "orphan": false,
             "resources": []
         },
+        "CreateIngressPoint": {
+            "access_level": "Undocumented",
+            "action": "CreateIngressPoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateReceiptFilter": {
             "access_level": "Write",
             "action": "CreateReceiptFilter",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to create a new IP address filter",
@@ -149719,24 +149791,72 @@
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to create an empty receipt rule set",
             "orphan": false,
             "resources": []
         },
+        "CreateRelay": {
+            "access_level": "Undocumented",
+            "action": "CreateRelay",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateRuleSet": {
+            "access_level": "Undocumented",
+            "action": "CreateRuleSet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateTemplate": {
             "access_level": "Write",
             "action": "CreateTemplate",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to creates an email template",
             "orphan": false,
             "resources": []
         },
+        "CreateTrafficPolicy": {
+            "access_level": "Undocumented",
+            "action": "CreateTrafficPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteAddonInstance": {
+            "access_level": "Undocumented",
+            "action": "DeleteAddonInstance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteAddonSubscription": {
+            "access_level": "Undocumented",
+            "action": "DeleteAddonSubscription",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteArchive": {
+            "access_level": "Undocumented",
+            "action": "DeleteArchive",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteConfigurationSet": {
             "access_level": "Write",
             "action": "DeleteConfigurationSet",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to delete an existing configuration set",
@@ -149866,14 +149986,22 @@
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to delete the specified sending authorization policy for the given identity (an email address or a domain)",
             "orphan": false,
             "resources": []
         },
+        "DeleteIngressPoint": {
+            "access_level": "Undocumented",
+            "action": "DeleteIngressPoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteReceiptFilter": {
             "access_level": "Write",
             "action": "DeleteReceiptFilter",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to delete the specified IP address filter",
@@ -149896,14 +150024,30 @@
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to delete the specified receipt rule set and all of the receipt rules it contains",
             "orphan": false,
             "resources": []
         },
+        "DeleteRelay": {
+            "access_level": "Undocumented",
+            "action": "DeleteRelay",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteRuleSet": {
+            "access_level": "Undocumented",
+            "action": "DeleteRuleSet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteSuppressedDestination": {
             "access_level": "Write",
             "action": "DeleteSuppressedDestination",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to remove an email address from the suppression list for your account",
@@ -149916,14 +150060,22 @@
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to delete an email template",
             "orphan": false,
             "resources": []
         },
+        "DeleteTrafficPolicy": {
+            "access_level": "Undocumented",
+            "action": "DeleteTrafficPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteVerifiedEmailAddress": {
             "access_level": "Write",
             "action": "DeleteVerifiedEmailAddress",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to delete the specified email address from the list of verified addresses",
@@ -149986,14 +150138,78 @@
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to return the email sending status of your account",
             "orphan": false,
             "resources": []
         },
+        "GetAddonInstance": {
+            "access_level": "Undocumented",
+            "action": "GetAddonInstance",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetAddonSubscription": {
+            "access_level": "Undocumented",
+            "action": "GetAddonSubscription",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetArchive": {
+            "access_level": "Undocumented",
+            "action": "GetArchive",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetArchiveExport": {
+            "access_level": "Undocumented",
+            "action": "GetArchiveExport",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetArchiveMessage": {
+            "access_level": "Undocumented",
+            "action": "GetArchiveMessage",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetArchiveMessageContent": {
+            "access_level": "Undocumented",
+            "action": "GetArchiveMessageContent",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetArchiveSearch": {
+            "access_level": "Undocumented",
+            "action": "GetArchiveSearch",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetArchiveSearchResults": {
+            "access_level": "Undocumented",
+            "action": "GetArchiveSearchResults",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetBlacklistReports": {
             "access_level": "Read",
             "action": "GetBlacklistReports",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to retrieve a list of the deny lists on which your dedicated IP addresses appear",
@@ -150252,24 +150468,48 @@
             ],
             "description": "Grants permission to provide information about an import job",
             "orphan": false,
             "resources": [
                 "import-job"
             ]
         },
+        "GetIngressPoint": {
+            "access_level": "Undocumented",
+            "action": "GetIngressPoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetMessageInsights": {
             "access_level": "Read",
             "action": "GetMessageInsights",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to provide insights about a message",
             "orphan": false,
             "resources": []
         },
+        "GetRelay": {
+            "access_level": "Undocumented",
+            "action": "GetRelay",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetRuleSet": {
+            "access_level": "Undocumented",
+            "action": "GetRuleSet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetSendQuota": {
             "access_level": "Read",
             "action": "GetSendQuota",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to return the user's current sending limits",
@@ -150302,14 +150542,62 @@
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to return the template object, which includes the subject line, HTML par, and text part for the template you specify",
             "orphan": false,
             "resources": []
         },
+        "GetTrafficPolicy": {
+            "access_level": "Undocumented",
+            "action": "GetTrafficPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListAddonInstances": {
+            "access_level": "Undocumented",
+            "action": "ListAddonInstances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListAddonSubscriptions": {
+            "access_level": "Undocumented",
+            "action": "ListAddonSubscriptions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListArchiveExports": {
+            "access_level": "Undocumented",
+            "action": "ListArchiveExports",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListArchiveSearches": {
+            "access_level": "Undocumented",
+            "action": "ListArchiveSearches",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListArchives": {
+            "access_level": "Undocumented",
+            "action": "ListArchives",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListConfigurationSets": {
             "access_level": "List",
             "action": "ListConfigurationSets",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to list all of the configuration sets for your account",
@@ -150435,14 +150723,22 @@
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to list all of the import jobs for your account",
             "orphan": false,
             "resources": []
         },
+        "ListIngressPoints": {
+            "access_level": "Undocumented",
+            "action": "ListIngressPoints",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListReceiptFilters": {
             "access_level": "Read",
             "action": "ListReceiptFilters",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to list the IP address filters associated with your account",
@@ -150468,14 +150764,30 @@
             ],
             "description": "Grants permission to list recommendations for your account",
             "orphan": false,
             "resources": [
                 "identity"
             ]
         },
+        "ListRelays": {
+            "access_level": "Undocumented",
+            "action": "ListRelays",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListRuleSets": {
+            "access_level": "Undocumented",
+            "action": "ListRuleSets",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListSuppressedDestinations": {
             "access_level": "Read",
             "action": "ListSuppressedDestinations",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to list email addresses that are on the suppression list for your account",
@@ -150503,14 +150815,22 @@
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to list the email templates present in your account",
             "orphan": false,
             "resources": []
         },
+        "ListTrafficPolicies": {
+            "access_level": "Undocumented",
+            "action": "ListTrafficPolicies",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListVerifiedEmailAddresses": {
             "access_level": "Read",
             "action": "ListVerifiedEmailAddresses",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to list all of the email addresses that have been verified in your account",
@@ -150963,14 +151283,46 @@
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to set the position of the specified receipt rule in the receipt rule set",
             "orphan": false,
             "resources": []
         },
+        "StartArchiveExport": {
+            "access_level": "Undocumented",
+            "action": "StartArchiveExport",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StartArchiveSearch": {
+            "access_level": "Undocumented",
+            "action": "StartArchiveSearch",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StopArchiveExport": {
+            "access_level": "Undocumented",
+            "action": "StopArchiveExport",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StopArchiveSearch": {
+            "access_level": "Undocumented",
+            "action": "StopArchiveSearch",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
                 "ses:ApiVersion"
@@ -151028,14 +151380,22 @@
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to enable or disable email sending for your account",
             "orphan": false,
             "resources": []
         },
+        "UpdateArchive": {
+            "access_level": "Undocumented",
+            "action": "UpdateArchive",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateConfigurationSetEventDestination": {
             "access_level": "Write",
             "action": "UpdateConfigurationSetEventDestination",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to update the event destination of a configuration set",
@@ -151129,34 +151489,66 @@
             ],
             "description": "Grants permission to update an email template",
             "orphan": false,
             "resources": [
                 "template"
             ]
         },
+        "UpdateIngressPoint": {
+            "access_level": "Undocumented",
+            "action": "UpdateIngressPoint",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateReceiptRule": {
             "access_level": "Write",
             "action": "UpdateReceiptRule",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to update a receipt rule",
             "orphan": false,
             "resources": []
         },
+        "UpdateRelay": {
+            "access_level": "Undocumented",
+            "action": "UpdateRelay",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateRuleSet": {
+            "access_level": "Undocumented",
+            "action": "UpdateRuleSet",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateTemplate": {
             "access_level": "Write",
             "action": "UpdateTemplate",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to update an email template",
             "orphan": false,
             "resources": []
         },
+        "UpdateTrafficPolicy": {
+            "access_level": "Undocumented",
+            "action": "UpdateTrafficPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "VerifyDomainDkim": {
             "access_level": "Write",
             "action": "VerifyDomainDkim",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to return a set of DKIM tokens for a domain",
```

### Comparing `iam_actions-1.2.20240521/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240522/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240521/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240522/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240521/iam_actions/generate/generate.py` & `iam_actions-1.2.20240522/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240521/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240522/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240521/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240522/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240521/iam_actions/generate/services.py` & `iam_actions-1.2.20240522/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240521/iam_actions/policies.json` & `iam_actions-1.2.20240522/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996805219262846%*

 * *Differences: {"'serviceMap'": "{'AWS Payments': {'Actions': {insert: [(4, 'ListPaymentInstruments'), (6, "*

 * *                 "'ListTagsForResource'), (8, 'TagResource'), (9, 'UntagResource'), (10, "*

 * *                 "'UpdatePaymentInstrument')]}, 'HasResource': True, 'ARNFormat': "*

 * *                 "'arn:aws:payments::${Account}:${ResourceType}:${ResourceId}', 'ARNRegex': "*

 * *                 "'^arn:aws:payments::[0-9]{12}:.+:.+', 'conditionKeys': "*

 * *                 "['aws:RequestTag/${TagKey}', 'aws:ResourceTag/${TagKey}' […]*

```diff
@@ -8364,25 +8364,37 @@
                 "payment-cryptography:KeyUsage",
                 "payment-cryptography:RequestAlias",
                 "payment-cryptography:ResourceAliases",
                 "payment-cryptography:WrappingKeyIdentifier"
             ]
         },
         "AWS Payments": {
+            "ARNFormat": "arn:aws:payments::${Account}:${ResourceType}:${ResourceId}",
+            "ARNRegex": "^arn:aws:payments::[0-9]{12}:.+:.+",
             "Actions": [
                 "CreatePaymentInstrument",
                 "DeletePaymentInstrument",
                 "GetPaymentInstrument",
                 "GetPaymentStatus",
+                "ListPaymentInstruments",
                 "ListPaymentPreferences",
+                "ListTagsForResource",
                 "MakePayment",
+                "TagResource",
+                "UntagResource",
+                "UpdatePaymentInstrument",
                 "UpdatePaymentPreferences"
             ],
-            "HasResource": false,
-            "StringPrefix": "payments"
+            "HasResource": true,
+            "StringPrefix": "payments",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
         },
         "AWS Performance Insights": {
             "ARNFormat": "arn:aws:pi:${Region}:${Account}:${ResourceType}/${RelativeId}",
             "ARNRegex": "^arn:aws:pi:.+",
             "Actions": [
                 "CreatePerformanceAnalysisReport",
                 "DeletePerformanceAnalysisReport",
@@ -8399,15 +8411,16 @@
                 "UntagResource"
             ],
             "HasResource": true,
             "StringPrefix": "pi",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:TagKeys",
+                "pi:Dimensions"
             ]
         },
         "AWS Price List": {
             "Actions": [
                 "DescribeServices",
                 "GetAttributeValues",
                 "GetPriceListFileUrl",
@@ -21387,14 +21400,78 @@
             "StringPrefix": "securitylake",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
+        "Amazon Simple Email Service - Mail Manager": {
+            "ARNFormat": "arn:aws:ses:${Region}:${Account}:${ResourceType}/${ResourceId}",
+            "ARNRegex": "^arn:aws:ses:.+:[0-9]+:.+",
+            "Actions": [
+                "CreateAddonInstance",
+                "CreateAddonSubscription",
+                "CreateArchive",
+                "CreateIngressPoint",
+                "CreateRelay",
+                "CreateRuleSet",
+                "CreateTrafficPolicy",
+                "DeleteAddonInstance",
+                "DeleteAddonSubscription",
+                "DeleteArchive",
+                "DeleteIngressPoint",
+                "DeleteRelay",
+                "DeleteRuleSet",
+                "DeleteTrafficPolicy",
+                "GetAddonInstance",
+                "GetAddonSubscription",
+                "GetArchive",
+                "GetArchiveExport",
+                "GetArchiveMessage",
+                "GetArchiveMessageContent",
+                "GetArchiveSearch",
+                "GetArchiveSearchResults",
+                "GetIngressPoint",
+                "GetRelay",
+                "GetRuleSet",
+                "GetTrafficPolicy",
+                "ListAddonInstances",
+                "ListAddonSubscriptions",
+                "ListArchiveExports",
+                "ListArchiveSearches",
+                "ListArchives",
+                "ListIngressPoints",
+                "ListRelays",
+                "ListRuleSets",
+                "ListTagsForResource",
+                "ListTrafficPolicies",
+                "StartArchiveExport",
+                "StartArchiveSearch",
+                "StopArchiveExport",
+                "StopArchiveSearch",
+                "TagResource",
+                "UntagResource",
+                "UpdateArchive",
+                "UpdateIngressPoint",
+                "UpdateRelay",
+                "UpdateRuleSet",
+                "UpdateTrafficPolicy"
+            ],
+            "HasResource": true,
+            "StringPrefix": "ses",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "ses:AddonSubscriptionArn",
+                "ses:MailManagerIngressPointType",
+                "ses:MailManagerRuleSetArn",
+                "ses:MailManagerTrafficPolicyArn"
+            ]
+        },
         "Amazon Simple Email Service v2": {
             "ARNFormat": "arn:aws:ses:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:ses:.+:[0-9]+:.+",
             "Actions": [
                 "BatchGetMetricData",
                 "CancelExportJob",
                 "CreateConfigurationSet",
```

### Comparing `iam_actions-1.2.20240521/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240522/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240521/iam_actions/services.json` & `iam_actions-1.2.20240522/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994233990853458%*

 * *Differences: {"'payments'": "{'Actions': {insert: [(4, 'ListPaymentInstruments'), (6, 'ListTagsForResource'), "*

 * *               "(8, 'TagResource'), (9, 'UntagResource'), (10, 'UpdatePaymentInstrument')]}, "*

 * *               "'ARNFormats': ['arn:aws:payments::${Account}:${ResourceType}:${ResourceId}'], "*

 * *               "'ARNRegexes': ['^arn:aws:payments::[0-9]{12}:.+:.+'], 'ConditionKeys': "*

 * *               "['aws:RequestTag/${TagKey}', 'aws:ResourceTag/${TagKey}', 'aws:TagKeys'], "*

 * *               "'HasResource': True}",*

 * * " […]*

```diff
@@ -16831,27 +16831,40 @@
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Payment Cryptography"
         ]
     },
     "payments": {
-        "ARNFormats": [],
-        "ARNRegexes": [],
+        "ARNFormats": [
+            "arn:aws:payments::${Account}:${ResourceType}:${ResourceId}"
+        ],
+        "ARNRegexes": [
+            "^arn:aws:payments::[0-9]{12}:.+:.+"
+        ],
         "Actions": [
             "CreatePaymentInstrument",
             "DeletePaymentInstrument",
             "GetPaymentInstrument",
             "GetPaymentStatus",
+            "ListPaymentInstruments",
             "ListPaymentPreferences",
+            "ListTagsForResource",
             "MakePayment",
+            "TagResource",
+            "UntagResource",
+            "UpdatePaymentInstrument",
             "UpdatePaymentPreferences"
         ],
-        "ConditionKeys": [],
-        "HasResource": false,
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys"
+        ],
+        "HasResource": true,
         "ServiceNames": [
             "AWS Payments"
         ]
     },
     "pca-connector-ad": {
         "ARNFormats": [
             "arn:aws:pca-connector-ad:${Region}:${Account}:${ResourceType}"
@@ -17014,15 +17027,16 @@
             "ListTagsForResource",
             "TagResource",
             "UntagResource"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
-            "aws:TagKeys"
+            "aws:TagKeys",
+            "pi:Dimensions"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Performance Insights"
         ]
     },
     "pipes": {
@@ -20864,55 +20878,77 @@
         "ARNRegexes": [
             "^arn:aws:ses:.+:[0-9]+:.+"
         ],
         "Actions": [
             "BatchGetMetricData",
             "CancelExportJob",
             "CloneReceiptRuleSet",
+            "CreateAddonInstance",
+            "CreateAddonSubscription",
+            "CreateArchive",
             "CreateConfigurationSet",
             "CreateConfigurationSetEventDestination",
             "CreateConfigurationSetTrackingOptions",
             "CreateContact",
             "CreateContactList",
             "CreateCustomVerificationEmailTemplate",
             "CreateDedicatedIpPool",
             "CreateDeliverabilityTestReport",
             "CreateEmailIdentity",
             "CreateEmailIdentityPolicy",
             "CreateEmailTemplate",
             "CreateExportJob",
             "CreateImportJob",
+            "CreateIngressPoint",
             "CreateReceiptFilter",
             "CreateReceiptRule",
             "CreateReceiptRuleSet",
+            "CreateRelay",
+            "CreateRuleSet",
             "CreateTemplate",
+            "CreateTrafficPolicy",
+            "DeleteAddonInstance",
+            "DeleteAddonSubscription",
+            "DeleteArchive",
             "DeleteConfigurationSet",
             "DeleteConfigurationSetEventDestination",
             "DeleteConfigurationSetTrackingOptions",
             "DeleteContact",
             "DeleteContactList",
             "DeleteCustomVerificationEmailTemplate",
             "DeleteDedicatedIpPool",
             "DeleteEmailIdentity",
             "DeleteEmailIdentityPolicy",
             "DeleteEmailTemplate",
             "DeleteIdentity",
             "DeleteIdentityPolicy",
+            "DeleteIngressPoint",
             "DeleteReceiptFilter",
             "DeleteReceiptRule",
             "DeleteReceiptRuleSet",
+            "DeleteRelay",
+            "DeleteRuleSet",
             "DeleteSuppressedDestination",
             "DeleteTemplate",
+            "DeleteTrafficPolicy",
             "DeleteVerifiedEmailAddress",
             "DescribeActiveReceiptRuleSet",
             "DescribeConfigurationSet",
             "DescribeReceiptRule",
             "DescribeReceiptRuleSet",
             "GetAccount",
             "GetAccountSendingEnabled",
+            "GetAddonInstance",
+            "GetAddonSubscription",
+            "GetArchive",
+            "GetArchiveExport",
+            "GetArchiveMessage",
+            "GetArchiveMessageContent",
+            "GetArchiveSearch",
+            "GetArchiveSearchResults",
             "GetBlacklistReports",
             "GetConfigurationSet",
             "GetConfigurationSetEventDestinations",
             "GetContact",
             "GetContactList",
             "GetCustomVerificationEmailTemplate",
             "GetDedicatedIp",
@@ -20928,38 +20964,51 @@
             "GetExportJob",
             "GetIdentityDkimAttributes",
             "GetIdentityMailFromDomainAttributes",
             "GetIdentityNotificationAttributes",
             "GetIdentityPolicies",
             "GetIdentityVerificationAttributes",
             "GetImportJob",
+            "GetIngressPoint",
             "GetMessageInsights",
+            "GetRelay",
+            "GetRuleSet",
             "GetSendQuota",
             "GetSendStatistics",
             "GetSuppressedDestination",
             "GetTemplate",
+            "GetTrafficPolicy",
+            "ListAddonInstances",
+            "ListAddonSubscriptions",
+            "ListArchiveExports",
+            "ListArchiveSearches",
+            "ListArchives",
             "ListConfigurationSets",
             "ListContactLists",
             "ListContacts",
             "ListCustomVerificationEmailTemplates",
             "ListDedicatedIpPools",
             "ListDeliverabilityTestReports",
             "ListDomainDeliverabilityCampaigns",
             "ListEmailIdentities",
             "ListEmailTemplates",
             "ListExportJobs",
             "ListIdentities",
             "ListIdentityPolicies",
             "ListImportJobs",
+            "ListIngressPoints",
             "ListReceiptFilters",
             "ListReceiptRuleSets",
             "ListRecommendations",
+            "ListRelays",
+            "ListRuleSets",
             "ListSuppressedDestinations",
             "ListTagsForResource",
             "ListTemplates",
+            "ListTrafficPolicies",
             "ListVerifiedEmailAddresses",
             "PutAccountDedicatedIpWarmupAttributes",
             "PutAccountDetails",
             "PutAccountSendingAttributes",
             "PutAccountSuppressionAttributes",
             "PutAccountVdmAttributes",
             "PutConfigurationSetDeliveryOptions",
@@ -20990,50 +21039,64 @@
             "SetActiveReceiptRuleSet",
             "SetIdentityDkimEnabled",
             "SetIdentityFeedbackForwardingEnabled",
             "SetIdentityHeadersInNotificationsEnabled",
             "SetIdentityMailFromDomain",
             "SetIdentityNotificationTopic",
             "SetReceiptRulePosition",
+            "StartArchiveExport",
+            "StartArchiveSearch",
+            "StopArchiveExport",
+            "StopArchiveSearch",
             "TagResource",
             "TestRenderEmailTemplate",
             "TestRenderTemplate",
             "UntagResource",
             "UpdateAccountSendingEnabled",
+            "UpdateArchive",
             "UpdateConfigurationSetEventDestination",
             "UpdateConfigurationSetReputationMetricsEnabled",
             "UpdateConfigurationSetSendingEnabled",
             "UpdateConfigurationSetTrackingOptions",
             "UpdateContact",
             "UpdateContactList",
             "UpdateCustomVerificationEmailTemplate",
             "UpdateEmailIdentityPolicy",
             "UpdateEmailTemplate",
+            "UpdateIngressPoint",
             "UpdateReceiptRule",
+            "UpdateRelay",
+            "UpdateRuleSet",
             "UpdateTemplate",
+            "UpdateTrafficPolicy",
             "VerifyDomainDkim",
             "VerifyDomainIdentity",
             "VerifyEmailAddress",
             "VerifyEmailIdentity"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys",
+            "ses:AddonSubscriptionArn",
             "ses:ApiVersion",
             "ses:ExportSourceType",
             "ses:FeedbackAddress",
             "ses:FromAddress",
             "ses:FromDisplayName",
+            "ses:MailManagerIngressPointType",
+            "ses:MailManagerRuleSetArn",
+            "ses:MailManagerTrafficPolicyArn",
             "ses:Recipients"
         ],
         "HasResource": true,
         "ServiceNames": [
             "Amazon Pinpoint Email Service",
             "Amazon SES",
+            "Amazon Simple Email Service - Mail Manager",
             "Amazon Simple Email Service v2"
         ]
     },
     "shield": {
         "ARNFormats": [
             "arn:aws:shield::${Account}:${Resource}/${ResourceId}"
         ],
```

### Comparing `iam_actions-1.2.20240521/pyproject.toml` & `iam_actions-1.2.20240522/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240521"
+version = "1.2.20240522"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240521/setup.py` & `iam_actions-1.2.20240522/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240521',
+    'version': '1.2.20240522',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240521/PKG-INFO` & `iam_actions-1.2.20240522/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240521
+Version: 1.2.20240522
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

