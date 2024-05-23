# Comparing `tmp/story_protocol_python_sdk-0.1.8.tar.gz` & `tmp/story_protocol_python_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "story_protocol_python_sdk-0.1.8.tar", last modified: Wed May 22 22:54:31 2024, max compression
+gzip compressed data, was "story_protocol_python_sdk-0.1.9.tar", last modified: Thu May 23 19:24:15 2024, max compression
```

## Comparing `story_protocol_python_sdk-0.1.8.tar` & `story_protocol_python_sdk-0.1.9.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.411681 story_protocol_python_sdk-0.1.8/
--rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      219 2024-05-21 20:55:29.000000 story_protocol_python_sdk-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      932 2024-05-22 22:54:31.410681 story_protocol_python_sdk-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.8/README.md
--rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.1.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 22:54:31.411681 story_protocol_python_sdk-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      904 2024-05-22 22:54:29.000000 story_protocol_python_sdk-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.340166 story_protocol_python_sdk-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.353166 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/
--rw-rw-rw-   0        0        0      221 2024-05-21 18:30:08.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.369681 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.373681 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/IPAssetRegistry/
--rw-rw-rw-   0        0        0    13409 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
--rw-rw-rw-   0        0        0     4546 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.377682 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
--rw-rw-rw-   0        0        0    16117 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
--rw-rw-rw-   0        0        0     1761 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.381680 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicenseRegistry/
--rw-rw-rw-   0        0        0    26905 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
--rw-rw-rw-   0        0        0     4230 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.384681 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicenseToken/
--rw-rw-rw-   0        0        0    23007 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
--rw-rw-rw-   0        0        0     1159 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.388682 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicensingModule/
--rw-rw-rw-   0        0        0    19697 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
--rw-rw-rw-   0        0        0     5246 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.391681 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/PILicenseTemplate/
--rw-rw-rw-   0        0        0    26246 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
--rw-rw-rw-   0        0        0     4625 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.394685 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/RoyaltyModule/
--rw-rw-rw-   0        0        0    16029 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
--rw-rw-rw-   0        0        0     1489 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.397681 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
--rw-rw-rw-   0        0        0    14037 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
--rw-rw-rw-   0        0        0     1183 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.401683 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/resources/
--rw-rw-rw-   0        0        0     7577 2024-05-22 22:50:16.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/resources/IPAsset.py
--rw-rw-rw-   0        0        0    16745 2024-05-22 22:50:05.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/resources/License.py
--rw-rw-rw-   0        0        0    12865 2024-05-22 22:54:20.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/resources/Royalty.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.406680 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/scripts/
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/scripts/__init__.py
--rw-rw-rw-   0        0        0     3539 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/scripts/config.json
--rw-rw-rw-   0        0        0      426 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/scripts/config_impl.json
--rw-rw-rw-   0        0        0     7361 2024-05-21 21:24:57.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/scripts/generate_client.py
--rw-rw-rw-   0        0        0     5288 2024-05-21 21:26:03.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/scripts/generate_client_impl.py
--rw-rw-rw-   0        0        0     1561 2024-05-22 18:49:34.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/story_client.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.408681 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/utils/
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     2444 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/utils/license_terms.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:54:31.368680 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk.egg-info/
--rw-rw-rw-   0        0        0      932 2024-05-22 22:54:31.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2710 2024-05-22 22:54:31.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 22:54:31.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-22 22:54:31.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-22 22:54:31.000000 story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:15.032739 story_protocol_python_sdk-0.1.9/
+-rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      219 2024-05-23 01:32:43.000000 story_protocol_python_sdk-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3429 2024-05-23 19:24:15.032739 story_protocol_python_sdk-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2841 2024-05-23 02:26:36.000000 story_protocol_python_sdk-0.1.9/README.md
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.1.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 19:24:15.032739 story_protocol_python_sdk-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      904 2024-05-23 19:24:04.000000 story_protocol_python_sdk-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.534687 story_protocol_python_sdk-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.598690 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/
+-rw-rw-rw-   0        0        0      221 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.654693 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.682689 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IPAssetRegistry/
+-rw-rw-rw-   0        0        0    13409 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
+-rw-rw-rw-   0        0        0     4546 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.690693 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
+-rw-rw-rw-   0        0        0    16117 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
+-rw-rw-rw-   0        0        0     1761 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.726688 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseRegistry/
+-rw-rw-rw-   0        0        0    26905 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
+-rw-rw-rw-   0        0        0     4230 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.761889 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseToken/
+-rw-rw-rw-   0        0        0    23007 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
+-rw-rw-rw-   0        0        0     1159 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.801892 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicensingModule/
+-rw-rw-rw-   0        0        0    19697 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
+-rw-rw-rw-   0        0        0     5246 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.853891 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/PILicenseTemplate/
+-rw-rw-rw-   0        0        0    26246 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
+-rw-rw-rw-   0        0        0     4625 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.877888 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyModule/
+-rw-rw-rw-   0        0        0    16029 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
+-rw-rw-rw-   0        0        0     1489 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.897890 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
+-rw-rw-rw-   0        0        0    14037 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
+-rw-rw-rw-   0        0        0     1183 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.941888 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/
+-rw-rw-rw-   0        0        0     5472 2024-05-23 18:37:04.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/IPAsset.py
+-rw-rw-rw-   0        0        0    13588 2024-05-23 18:38:15.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/License.py
+-rw-rw-rw-   0        0        0     8542 2024-05-23 19:05:20.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/Royalty.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:15.001888 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3539 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/config.json
+-rw-rw-rw-   0        0        0      426 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/config_impl.json
+-rw-rw-rw-   0        0        0     7361 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/generate_client.py
+-rw-rw-rw-   0        0        0     5288 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/generate_client_impl.py
+-rw-rw-rw-   0        0        0     1426 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/story_client.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:15.028740 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     2444 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/utils/license_terms.py
+-rw-rw-rw-   0        0        0     1449 2024-05-23 18:37:10.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/utils/transaction_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.654693 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0     3429 2024-05-23 19:24:14.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2767 2024-05-23 19:24:14.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 19:24:14.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-23 19:24:14.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-23 19:24:14.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/top_level.txt
```

### Comparing `story_protocol_python_sdk-0.1.8/LICENSE` & `story_protocol_python_sdk-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/setup.py` & `story_protocol_python_sdk-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='story_protocol_python_sdk',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(where='src', exclude=["tests"]),
     package_dir={'': 'src'},
     install_requires=[
         'web3>=5.0.0',
         'pytest',
         'python-dotenv'
     ],
```

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/resources/License.py` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/License.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,40 @@
-import logging
+#src/story_protcol_python_sdk/resources/License.py
+
 from web3 import Web3
-from web3.exceptions import LogTopicError
 
 from story_protocol_python_sdk.abi.PILicenseTemplate.PILicenseTemplate_client import PILicenseTemplateClient
 from story_protocol_python_sdk.abi.LicenseRegistry.LicenseRegistry_client import LicenseRegistryClient
 from story_protocol_python_sdk.abi.LicensingModule.LicensingModule_client import LicensingModuleClient
 from story_protocol_python_sdk.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
-from story_protocol_python_sdk.utils.license_terms import get_license_term_by_type, PIL_TYPE
 
-# Configure logging
-# logging.basicConfig(level=logging.DEBUG)  # Set to DEBUG to capture all log messages
-# logger = logging.getLogger(__name__)
+from story_protocol_python_sdk.utils.license_terms import get_license_term_by_type, PIL_TYPE
+from story_protocol_python_sdk.utils.transaction_utils import build_and_send_transaction
 
 class License:
     def __init__(self, web3: Web3, account, chain_id):
         self.web3 = web3
         self.account = account
         self.chain_id = chain_id
 
         self.license_template_client = PILicenseTemplateClient(web3)
         self.license_registry_client = LicenseRegistryClient(web3)
         self.licensing_module_client  = LicensingModuleClient(web3)
         self.ip_asset_registry_client = IPAssetRegistryClient(web3)
 
     def _get_license_terms_id(self, license_terms):
-        # logger.info(f"Getting license terms ID for: {license_terms}")
         return self.license_template_client.getLicenseTermsId(license_terms)
 
     def registerNonComSocialRemixingPIL(self):
         try:
             # Get the license terms for non-commercial social remixing PIL
             license_terms = get_license_term_by_type(PIL_TYPE['NON_COMMERCIAL_REMIX'])
-            # logger.info(f"License terms: {license_terms}")
 
             # Check if the license terms are already registered
             license_terms_id = self._get_license_terms_id(license_terms)
-            # logger.info(f"License terms ID: {license_terms_id}")
             if (license_terms_id is not None) and (license_terms_id != 0):
                 return {'licenseTermsId': license_terms_id}
 
             # Fetch the current average gas price from the node plus 10%
             current_gas_price = int(self.web3.eth.gas_price * 1.1)
 
             # Build the transaction
@@ -47,55 +42,45 @@
                 license_terms, {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
                     'gasPrice': current_gas_price
                 }
             )
-            # logger.info(f"Transaction: {transaction}")
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
-            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for transaction receipt with a longer timeout
-
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
-            # logger.info(f"Transaction receipt: {tx_receipt}")
 
             # Parse the event logs for LicenseTermsRegistered
             target_logs = self._parse_tx_license_terms_registered_event(tx_receipt)
             return {
                 'txHash': tx_hash.hex(),
                 'licenseTermsId': target_logs
             }
 
         except Exception as e:
-            # logger.error(f"Error interacting with contract: {e}")
             raise e
         
     def registerCommercialUsePIL(self, minting_fee, currency, royalty_policy, tx_options=None):
         try:
-            # logger.info(f"Starting registerCommercialUsePIL with minting_fee: {minting_fee}, currency: {currency}, royalty_policy: {royalty_policy}")
-
             # Construct complete license terms
             complete_license_terms = get_license_term_by_type(PIL_TYPE['COMMERCIAL_USE'], {
                 'mintingFee': minting_fee,
                 'currency': currency,
                 'royaltyPolicy': royalty_policy,
             })
-            # logger.info(f"Complete license terms: {complete_license_terms}")
 
             # Check if the license terms are already registered
             license_terms_id = self._get_license_terms_id(complete_license_terms)
-            # logger.info(f"License terms ID: {license_terms_id}")
             if (license_terms_id is not None) and (license_terms_id != 0):
                 return {'licenseTermsId': license_terms_id}
 
             # Fetch the current average gas price from the node plus 10%
             current_gas_price = int(self.web3.eth.gas_price * 1.1)
 
             # Build the transaction
@@ -103,59 +88,48 @@
                 complete_license_terms, {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
                     'gasPrice': current_gas_price
                 }
             )
-            # logger.info(f"Built transaction: {transaction}")
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
-            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for transaction receipt with a longer timeout
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
-            # logger.info(f"Transaction receipt: {tx_receipt}")
 
             # Parse the event logs for LicenseTermsRegistered
             if not tx_receipt.logs:
-                # logger.error(f"No logs found in transaction receipt: {tx_receipt}")
                 return None
 
             target_logs = self._parse_tx_license_terms_registered_event(tx_receipt)
             return {
                 'txHash': tx_hash.hex(),
                 'licenseTermsId': target_logs
             }
 
         except Exception as e:
-            # logger.error(f"Error interacting with contract: {e}")
             raise e
 
     def registerCommercialRemixPIL(self, minting_fee, currency, commercial_rev_share, royalty_policy, tx_options=None):
         try:
-            # logger.info(f"Starting registerCommercialRemixPIL with minting_fee: {minting_fee}, currency: {currency}, commercial_rev_share: {commercial_rev_share}, royalty_policy: {royalty_policy}")
-
             # Construct complete license terms
             complete_license_terms = get_license_term_by_type(PIL_TYPE['COMMERCIAL_REMIX'], {
                 'mintingFee': minting_fee,
                 'currency': currency,
                 'commercialRevShare': commercial_rev_share,
                 'royaltyPolicy': royalty_policy,
             })
-            # logger.info(f"Complete license terms: {complete_license_terms}")
-
             # Check if the license terms are already registered
             license_terms_id = self._get_license_terms_id(complete_license_terms)
-            # logger.info(f"License terms ID: {license_terms_id}")
             if license_terms_id and license_terms_id != 0:
                 return {'licenseTermsId': license_terms_id}
 
             # Fetch the current average gas price from the node plus 10%
             current_gas_price = int(self.web3.eth.gas_price * 1.1)
 
             # Build the transaction
@@ -163,56 +137,48 @@
                 complete_license_terms, {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
                     'gasPrice': current_gas_price
                 }
             )
-            # logger.info(f"Built transaction: {transaction}")
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
-            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for transaction receipt with a longer timeout
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
-            # logger.info(f"Transaction receipt: {tx_receipt}")
 
             # Parse the event logs for LicenseTermsRegistered
             if not tx_receipt.logs:
-                # logger.error(f"No logs found in transaction receipt: {tx_receipt}")
                 return None
 
             target_logs = self._parse_tx_license_terms_registered_event(tx_receipt)
             return {
                 'txHash': tx_hash.hex(),
                 'licenseTermsId': target_logs
             }
 
         except Exception as e:
-            # logger.error(f"Error interacting with contract: {e}")
             raise e
 
     def _parse_tx_license_terms_registered_event(self, tx_receipt):
         event_signature = self.web3.keccak(text="LicenseTermsRegistered(uint256,address,bytes)").hex()
 
         for log in tx_receipt['logs']:
             if log['topics'][0].hex() == event_signature:
                 return int(log['topics'][1].hex(), 16)
 
         return None
     
     def attachLicenseTerms(self, ip_id, license_template, license_terms_id):
         try:
-            # logger.info(f"Starting attachLicenseTerms with ip_id: {ip_id}, license_template: {license_template}, license_terms_id: {license_terms_id}")
-
             # Validate the license template address
             if not Web3.is_address(license_template):
                 raise ValueError(f'Address "{license_template}" is invalid.')
 
             # Check if the IP is registered
             is_registered = self.ip_asset_registry_client.isRegistered(ip_id)
             if not is_registered:
@@ -236,38 +202,31 @@
                 ip_id, license_template, license_terms_id, {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
                     'gasPrice': current_gas_price
                 }
             )
-            # logger.info(f"Built transaction: {transaction}")
 
             # Sign the transaction
             signed_txn = self.account.sign_transaction(transaction)
-            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for the transaction receipt
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
-            # logger.info(f"Transaction receipt: {tx_receipt}")
 
             return {'txHash': tx_hash.hex()}
         
         except Exception as e:
-            # logger.error(f"Failed to attach license terms: {e}")
             raise e
         
     def mintLicenseTokens(self, licensor_ip_id, license_template, license_terms_id, amount, receiver):
         try:
-            # logger.info(f"Starting mintLicenseTokens with licensor_ip_id: {licensor_ip_id}, license_template: {license_template}, license_terms_id: {license_terms_id}, amount: {amount}, receiver: {receiver}")
-
             # Validate the license template address
             if not Web3.is_address(license_template):
                 raise ValueError(f'Address "{license_template}" is invalid.')
             
             # Validate the license template address
             if not Web3.is_address(receiver):
                 raise ValueError(f'Address "{receiver}" is invalid.')
@@ -295,38 +254,33 @@
                 licensor_ip_id, license_template, license_terms_id, amount, receiver, '0x0000000000000000000000000000000000000000', {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
                     'gasPrice': current_gas_price
                 }
             )
-            # logger.info(f"Built transaction: {transaction}")
 
             # Sign the transaction
             signed_txn = self.account.sign_transaction(transaction)
-            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for the transaction receipt
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
-            # logger.info(f"Transaction receipt: {tx_receipt}")
 
             # Parse the event logs for LicenseTokensMinted
             target_logs = self._parse_tx_license_tokens_minted_event(tx_receipt)
-            # print("the license token id is " , target_logs)
+
             return {
                 'txHash': tx_hash.hex(),
                 'licenseTokenIds': target_logs
             }
 
         except Exception as e:
-            # logger.error(f"Failed to mint license tokens: {e}")
             raise e
 
     def _parse_tx_license_tokens_minted_event(self, tx_receipt):
         event_signature = self.web3.keccak(text="LicenseTokenMinted(address,address,uint256)").hex()
         token_ids = []
 
         for log in tx_receipt['logs']:
```

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/scripts/config.json` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/config.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/scripts/generate_client.py` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/generate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/scripts/generate_client_impl.py` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/generate_client_impl.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/story_client.py` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/story_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 # src/story_client.py
 
 import os
-import json
 import sys
-import logging
 
 # Ensure the src directory is in the Python path
 current_dir = os.path.dirname(__file__)
 src_path = os.path.abspath(os.path.join(current_dir, '..'))
 if src_path not in sys.path:
     sys.path.append(src_path)
 
 from story_protocol_python_sdk.resources.IPAsset import IPAsset
 from story_protocol_python_sdk.resources.License import License
 from story_protocol_python_sdk.resources.Royalty import Royalty
 
-# Configure logging
-# logging.basicConfig(level=logging.INFO)
-# logger = logging.getLogger(__name__)
-
 class StoryClient:
     def __init__(self, web3, account, chain_id):
         if not web3 or not account:
             raise ValueError("web3 and account must be provided")
 
         self.web3 = web3
         self.account = account
```

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk/utils/license_terms.py` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/utils/license_terms.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.8/src/story_protocol_python_sdk.egg-info/SOURCES.txt` & `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,8 +41,9 @@
 src/story_protocol_python_sdk/resources/__init__.py
 src/story_protocol_python_sdk/scripts/__init__.py
 src/story_protocol_python_sdk/scripts/config.json
 src/story_protocol_python_sdk/scripts/config_impl.json
 src/story_protocol_python_sdk/scripts/generate_client.py
 src/story_protocol_python_sdk/scripts/generate_client_impl.py
 src/story_protocol_python_sdk/utils/__init__.py
-src/story_protocol_python_sdk/utils/license_terms.py
+src/story_protocol_python_sdk/utils/license_terms.py
+src/story_protocol_python_sdk/utils/transaction_utils.py
```

