# Comparing `tmp/story_protocol_python_sdk-0.1.6.tar.gz` & `tmp/story_protocol_python_sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "story_protocol_python_sdk-0.1.6.tar", last modified: Wed May 22 22:43:16 2024, max compression
+gzip compressed data, was "story_protocol_python_sdk-0.1.7.tar", last modified: Wed May 22 22:50:31 2024, max compression
```

## Comparing `story_protocol_python_sdk-0.1.6.tar` & `story_protocol_python_sdk-0.1.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.906950 story_protocol_python_sdk-0.1.6/
--rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      219 2024-05-21 20:55:29.000000 story_protocol_python_sdk-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      932 2024-05-22 22:43:16.905362 story_protocol_python_sdk-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.6/README.md
--rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.1.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 22:43:16.906950 story_protocol_python_sdk-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      904 2024-05-22 22:42:33.000000 story_protocol_python_sdk-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.719350 story_protocol_python_sdk-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.737350 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/
--rw-rw-rw-   0        0        0      221 2024-05-21 18:30:08.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.764349 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.776352 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/
--rw-rw-rw-   0        0        0    13409 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
--rw-rw-rw-   0        0        0     4546 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.787350 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
--rw-rw-rw-   0        0        0    16117 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
--rw-rw-rw-   0        0        0     1761 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.799350 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseRegistry/
--rw-rw-rw-   0        0        0    26905 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
--rw-rw-rw-   0        0        0     4230 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.818349 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseToken/
--rw-rw-rw-   0        0        0    23007 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
--rw-rw-rw-   0        0        0     1159 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.831350 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicensingModule/
--rw-rw-rw-   0        0        0    19697 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
--rw-rw-rw-   0        0        0     5246 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.843351 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/
--rw-rw-rw-   0        0        0    26246 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
--rw-rw-rw-   0        0        0     4625 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.864351 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyModule/
--rw-rw-rw-   0        0        0    16029 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
--rw-rw-rw-   0        0        0     1489 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.875352 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
--rw-rw-rw-   0        0        0    14037 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
--rw-rw-rw-   0        0        0     1183 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.881353 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/
--rw-rw-rw-   0        0        0     7242 2024-05-22 22:41:36.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/IPAsset.py
--rw-rw-rw-   0        0        0    16684 2024-05-22 18:40:50.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/License.py
--rw-rw-rw-   0        0        0    12865 2024-05-22 18:41:32.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/Royalty.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.902361 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/__init__.py
--rw-rw-rw-   0        0        0     3539 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/config.json
--rw-rw-rw-   0        0        0      426 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/config_impl.json
--rw-rw-rw-   0        0        0     7361 2024-05-21 21:24:57.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/generate_client.py
--rw-rw-rw-   0        0        0     5288 2024-05-21 21:26:03.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/generate_client_impl.py
--rw-rw-rw-   0        0        0     1561 2024-05-22 18:49:34.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/story_client.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.904362 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/utils/
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     2444 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/utils/license_terms.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.762349 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/
--rw-rw-rw-   0        0        0      932 2024-05-22 22:43:16.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2710 2024-05-22 22:43:16.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 22:43:16.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-22 22:43:16.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-22 22:43:16.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.088721 story_protocol_python_sdk-0.1.7/
+-rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      219 2024-05-21 20:55:29.000000 story_protocol_python_sdk-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      932 2024-05-22 22:50:31.087721 story_protocol_python_sdk-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.7/README.md
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.1.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 22:50:31.089723 story_protocol_python_sdk-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      904 2024-05-22 22:50:27.000000 story_protocol_python_sdk-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:30.994707 story_protocol_python_sdk-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.007709 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/
+-rw-rw-rw-   0        0        0      221 2024-05-21 18:30:08.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.038707 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.042707 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/IPAssetRegistry/
+-rw-rw-rw-   0        0        0    13409 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
+-rw-rw-rw-   0        0        0     4546 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.045709 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
+-rw-rw-rw-   0        0        0    16117 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
+-rw-rw-rw-   0        0        0     1761 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.050707 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicenseRegistry/
+-rw-rw-rw-   0        0        0    26905 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
+-rw-rw-rw-   0        0        0     4230 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.054708 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicenseToken/
+-rw-rw-rw-   0        0        0    23007 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
+-rw-rw-rw-   0        0        0     1159 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.059708 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicensingModule/
+-rw-rw-rw-   0        0        0    19697 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
+-rw-rw-rw-   0        0        0     5246 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.064721 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/PILicenseTemplate/
+-rw-rw-rw-   0        0        0    26246 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
+-rw-rw-rw-   0        0        0     4625 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.068721 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/RoyaltyModule/
+-rw-rw-rw-   0        0        0    16029 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
+-rw-rw-rw-   0        0        0     1489 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.072722 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
+-rw-rw-rw-   0        0        0    14037 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
+-rw-rw-rw-   0        0        0     1183 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.077721 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/resources/
+-rw-rw-rw-   0        0        0     7577 2024-05-22 22:50:16.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/resources/IPAsset.py
+-rw-rw-rw-   0        0        0    16745 2024-05-22 22:50:05.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/resources/License.py
+-rw-rw-rw-   0        0        0    12863 2024-05-22 22:49:26.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/resources/Royalty.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.083722 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/scripts/
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3539 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/scripts/config.json
+-rw-rw-rw-   0        0        0      426 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/scripts/config_impl.json
+-rw-rw-rw-   0        0        0     7361 2024-05-21 21:24:57.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/scripts/generate_client.py
+-rw-rw-rw-   0        0        0     5288 2024-05-21 21:26:03.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/scripts/generate_client_impl.py
+-rw-rw-rw-   0        0        0     1561 2024-05-22 18:49:34.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/story_client.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.086721 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     2444 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/utils/license_terms.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:50:31.036707 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0      932 2024-05-22 22:50:30.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2710 2024-05-22 22:50:30.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 22:50:30.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-22 22:50:30.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-22 22:50:30.000000 story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk.egg-info/top_level.txt
```

### Comparing `story_protocol_python_sdk-0.1.6/LICENSE` & `story_protocol_python_sdk-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/PKG-INFO` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: story_protocol_python_sdk
-Version: 0.1.6
+Name: story-protocol-python-sdk
+Version: 0.1.7
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `story_protocol_python_sdk-0.1.6/setup.py` & `story_protocol_python_sdk-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='story_protocol_python_sdk',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(where='src', exclude=["tests"]),
     package_dir={'': 'src'},
     install_requires=[
         'web3>=5.0.0',
         'pytest',
         'python-dotenv'
     ],
```

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/IPAsset.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/resources/IPAsset.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,17 +57,16 @@
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
             
-            if ip_id != None:
-                while self.ip_asset_registry_client.isRegistered(ip_id) == False:
-                    time.sleep(1)
+            # Wait for the transaction receipt
+            tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
 
             return {
                 'txHash': tx_hash.hex(),
                 'ipId': ip_id
             }
 
         except Exception as e:
@@ -111,14 +110,17 @@
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
             
+            # Wait for the transaction receipt
+            tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
+
             return {
                 'txHash': tx_hash.hex()
             }
 
         except Exception as e:
             # logger.error(f"Failed to register derivative: {e}")
             raise e
@@ -150,14 +152,17 @@
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
             
+            # Wait for the transaction receipt
+            tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
+
             return {
                 'txHash': tx_hash.hex()
             }
 
         except Exception as e:
             # logger.error(f"Failed to register derivative with license tokens: {e}")
             raise e
```

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/License.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/resources/License.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
             # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for transaction receipt with a longer timeout
 
-            tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)  # 10 minutes timeout
+            tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
             # logger.info(f"Transaction receipt: {tx_receipt}")
 
             # Parse the event logs for LicenseTermsRegistered
             target_logs = self._parse_tx_license_terms_registered_event(tx_receipt)
             return {
                 'txHash': tx_hash.hex(),
                 'licenseTermsId': target_logs
@@ -114,15 +114,15 @@
             # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
             # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for transaction receipt with a longer timeout
-            tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)  # 10 minutes timeout
+            tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
             # logger.info(f"Transaction receipt: {tx_receipt}")
 
             # Parse the event logs for LicenseTermsRegistered
             if not tx_receipt.logs:
                 # logger.error(f"No logs found in transaction receipt: {tx_receipt}")
                 return None
 
@@ -174,15 +174,15 @@
             # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
             # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for transaction receipt with a longer timeout
-            tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)
+            tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
             # logger.info(f"Transaction receipt: {tx_receipt}")
 
             # Parse the event logs for LicenseTermsRegistered
             if not tx_receipt.logs:
                 # logger.error(f"No logs found in transaction receipt: {tx_receipt}")
                 return None
 
@@ -247,15 +247,15 @@
             # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
             # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for the transaction receipt
-            tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)
+            tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
             # logger.info(f"Transaction receipt: {tx_receipt}")
 
             return {'txHash': tx_hash.hex()}
         
         except Exception as e:
             # logger.error(f"Failed to attach license terms: {e}")
             raise e
@@ -306,15 +306,15 @@
             # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
             # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for the transaction receipt
-            tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)
+            tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=300)  # 5 minutes timeout
             # logger.info(f"Transaction receipt: {tx_receipt}")
 
             # Parse the event logs for LicenseTokensMinted
             target_logs = self._parse_tx_license_tokens_minted_event(tx_receipt)
             # print("the license token id is " , target_logs)
             return {
                 'txHash': tx_hash.hex(),
```

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/Royalty.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/resources/Royalty.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,14 @@
             signed_txn = self.account.sign_transaction(transaction)
             # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
             # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
-
             # Wait for transaction receipt with a longer timeout
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)  # 10 minutes timeout
             # logger.info(f"Transaction receipt: {tx_receipt}")
 
             snapshotId =  self._parseTxSnapshotCompletedEvent(tx_receipt)
 
             return {
```

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/config.json` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/scripts/config.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/generate_client.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/scripts/generate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/generate_client_impl.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/scripts/generate_client_impl.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/story_client.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/story_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/utils/license_terms.py` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk/utils/license_terms.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/PKG-INFO` & `story_protocol_python_sdk-0.1.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: story-protocol-python-sdk
-Version: 0.1.6
+Name: story_protocol_python_sdk
+Version: 0.1.7
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/SOURCES.txt` & `story_protocol_python_sdk-0.1.7/src/story_protocol_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

