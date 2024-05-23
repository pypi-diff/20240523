# Comparing `tmp/story_protocol_python_sdk-0.1.9.tar.gz` & `tmp/story_protocol_python_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "story_protocol_python_sdk-0.1.9.tar", last modified: Thu May 23 19:24:15 2024, max compression
+gzip compressed data, was "story_protocol_python_sdk-0.2.0.tar", last modified: Thu May 23 20:41:24 2024, max compression
```

## Comparing `story_protocol_python_sdk-0.1.9.tar` & `story_protocol_python_sdk-0.2.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:15.032739 story_protocol_python_sdk-0.1.9/
--rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      219 2024-05-23 01:32:43.000000 story_protocol_python_sdk-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3429 2024-05-23 19:24:15.032739 story_protocol_python_sdk-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2841 2024-05-23 02:26:36.000000 story_protocol_python_sdk-0.1.9/README.md
--rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.1.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 19:24:15.032739 story_protocol_python_sdk-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      904 2024-05-23 19:24:04.000000 story_protocol_python_sdk-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.534687 story_protocol_python_sdk-0.1.9/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.598690 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/
--rw-rw-rw-   0        0        0      221 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.654693 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.682689 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IPAssetRegistry/
--rw-rw-rw-   0        0        0    13409 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
--rw-rw-rw-   0        0        0     4546 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.690693 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
--rw-rw-rw-   0        0        0    16117 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
--rw-rw-rw-   0        0        0     1761 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.726688 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseRegistry/
--rw-rw-rw-   0        0        0    26905 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
--rw-rw-rw-   0        0        0     4230 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.761889 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseToken/
--rw-rw-rw-   0        0        0    23007 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
--rw-rw-rw-   0        0        0     1159 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.801892 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicensingModule/
--rw-rw-rw-   0        0        0    19697 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
--rw-rw-rw-   0        0        0     5246 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.853891 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/PILicenseTemplate/
--rw-rw-rw-   0        0        0    26246 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
--rw-rw-rw-   0        0        0     4625 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.877888 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyModule/
--rw-rw-rw-   0        0        0    16029 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
--rw-rw-rw-   0        0        0     1489 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.897890 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
--rw-rw-rw-   0        0        0    14037 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
--rw-rw-rw-   0        0        0     1183 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.941888 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/
--rw-rw-rw-   0        0        0     5472 2024-05-23 18:37:04.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/IPAsset.py
--rw-rw-rw-   0        0        0    13588 2024-05-23 18:38:15.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/License.py
--rw-rw-rw-   0        0        0     8542 2024-05-23 19:05:20.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/Royalty.py
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:15.001888 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/__init__.py
--rw-rw-rw-   0        0        0     3539 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/config.json
--rw-rw-rw-   0        0        0      426 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/config_impl.json
--rw-rw-rw-   0        0        0     7361 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/generate_client.py
--rw-rw-rw-   0        0        0     5288 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/generate_client_impl.py
--rw-rw-rw-   0        0        0     1426 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/story_client.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:15.028740 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/utils/
--rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     2444 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/utils/license_terms.py
--rw-rw-rw-   0        0        0     1449 2024-05-23 18:37:10.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/utils/transaction_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:24:14.654693 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/
--rw-rw-rw-   0        0        0     3429 2024-05-23 19:24:14.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2767 2024-05-23 19:24:14.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 19:24:14.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-23 19:24:14.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-23 19:24:14.000000 story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:24.060715 story_protocol_python_sdk-0.2.0/
+-rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      219 2024-05-23 01:32:43.000000 story_protocol_python_sdk-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3430 2024-05-23 20:41:24.059715 story_protocol_python_sdk-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2841 2024-05-23 02:26:36.000000 story_protocol_python_sdk-0.2.0/README.md
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 20:41:24.060715 story_protocol_python_sdk-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      905 2024-05-23 20:41:16.000000 story_protocol_python_sdk-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:23.803715 story_protocol_python_sdk-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:23.817716 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/
+-rw-rw-rw-   0        0        0      221 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:23.891715 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:23.910716 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/IPAssetRegistry/
+-rw-rw-rw-   0        0        0    13409 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
+-rw-rw-rw-   0        0        0     4546 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:23.932717 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
+-rw-rw-rw-   0        0        0    16117 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
+-rw-rw-rw-   0        0        0     1761 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:23.945717 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicenseRegistry/
+-rw-rw-rw-   0        0        0    26905 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
+-rw-rw-rw-   0        0        0     4230 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:23.955714 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicenseToken/
+-rw-rw-rw-   0        0        0    23007 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
+-rw-rw-rw-   0        0        0     1159 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:23.967718 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicensingModule/
+-rw-rw-rw-   0        0        0    19697 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
+-rw-rw-rw-   0        0        0     5246 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:23.989715 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/PILicenseTemplate/
+-rw-rw-rw-   0        0        0    26246 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
+-rw-rw-rw-   0        0        0     4625 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:24.037716 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/RoyaltyModule/
+-rw-rw-rw-   0        0        0    16029 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
+-rw-rw-rw-   0        0        0     1489 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:24.042716 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
+-rw-rw-rw-   0        0        0    14037 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
+-rw-rw-rw-   0        0        0     1183 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:24.047716 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/resources/
+-rw-rw-rw-   0        0        0     5472 2024-05-23 18:37:04.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/resources/IPAsset.py
+-rw-rw-rw-   0        0        0    13588 2024-05-23 18:38:15.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/resources/License.py
+-rw-rw-rw-   0        0        0     8542 2024-05-23 20:29:32.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/resources/Royalty.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:24.053716 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/scripts/
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3539 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/scripts/config.json
+-rw-rw-rw-   0        0        0      426 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/scripts/config_impl.json
+-rw-rw-rw-   0        0        0     7361 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/scripts/generate_client.py
+-rw-rw-rw-   0        0        0     5288 2024-05-23 01:34:07.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/scripts/generate_client_impl.py
+-rw-rw-rw-   0        0        0     1426 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/story_client.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:24.057715 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     2444 2024-05-23 01:21:34.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/utils/license_terms.py
+-rw-rw-rw-   0        0        0     1449 2024-05-23 18:37:10.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/utils/transaction_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:41:23.883715 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0     3430 2024-05-23 20:41:23.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2767 2024-05-23 20:41:23.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 20:41:23.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-23 20:41:23.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-23 20:41:23.000000 story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk.egg-info/top_level.txt
```

### Comparing `story_protocol_python_sdk-0.1.9/LICENSE` & `story_protocol_python_sdk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/PKG-INFO` & `story_protocol_python_sdk-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: story_protocol_python_sdk
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: web3>=5.0.0
 Requires-Dist: pytest
 Requires-Dist: python-dotenv
 
 # Story Protocol SDK
```

### Comparing `story_protocol_python_sdk-0.1.9/README.md` & `story_protocol_python_sdk-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/setup.py` & `story_protocol_python_sdk-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='story_protocol_python_sdk',
-    version='0.1.9',
+    version='0.2.0',
     packages=find_packages(where='src', exclude=["tests"]),
     package_dir={'': 'src'},
     install_requires=[
         'web3>=5.0.0',
         'pytest',
         'python-dotenv'
     ],
@@ -19,9 +19,9 @@
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.10',
 )
```

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/IPAsset.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/resources/IPAsset.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/License.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/resources/License.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/resources/Royalty.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/resources/Royalty.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/config.json` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/scripts/config.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/generate_client.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/scripts/generate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/scripts/generate_client_impl.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/scripts/generate_client_impl.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/story_client.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/story_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/utils/license_terms.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/utils/license_terms.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk/utils/transaction_utils.py` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/PKG-INFO` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: story-protocol-python-sdk
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: web3>=5.0.0
 Requires-Dist: pytest
 Requires-Dist: python-dotenv
 
 # Story Protocol SDK
```

### Comparing `story_protocol_python_sdk-0.1.9/src/story_protocol_python_sdk.egg-info/SOURCES.txt` & `story_protocol_python_sdk-0.2.0/src/story_protocol_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

