# Comparing `tmp/story_protocol_python_sdk-0.1.5.tar.gz` & `tmp/story_protocol_python_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "story_protocol_python_sdk-0.1.5.tar", last modified: Wed May 22 18:52:02 2024, max compression
+gzip compressed data, was "story_protocol_python_sdk-0.1.6.tar", last modified: Wed May 22 22:43:16 2024, max compression
```

## Comparing `story_protocol_python_sdk-0.1.5.tar` & `story_protocol_python_sdk-0.1.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.752024 story_protocol_python_sdk-0.1.5/
--rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      219 2024-05-21 20:55:29.000000 story_protocol_python_sdk-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      932 2024-05-22 18:52:02.750023 story_protocol_python_sdk-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.5/README.md
--rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.1.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 18:52:02.752024 story_protocol_python_sdk-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      904 2024-05-22 18:50:15.000000 story_protocol_python_sdk-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.376131 story_protocol_python_sdk-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.395128 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/
--rw-rw-rw-   0        0        0      221 2024-05-21 18:30:08.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.418129 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.451129 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IPAssetRegistry/
--rw-rw-rw-   0        0        0    13409 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
--rw-rw-rw-   0        0        0     4546 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.551129 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
--rw-rw-rw-   0        0        0    16117 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
--rw-rw-rw-   0        0        0     1761 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.564131 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseRegistry/
--rw-rw-rw-   0        0        0    26905 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
--rw-rw-rw-   0        0        0     4230 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.590135 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseToken/
--rw-rw-rw-   0        0        0    23007 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
--rw-rw-rw-   0        0        0     1159 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.603130 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicensingModule/
--rw-rw-rw-   0        0        0    19697 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
--rw-rw-rw-   0        0        0     5246 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.616129 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/PILicenseTemplate/
--rw-rw-rw-   0        0        0    26246 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
--rw-rw-rw-   0        0        0     4625 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.635129 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyModule/
--rw-rw-rw-   0        0        0    16029 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
--rw-rw-rw-   0        0        0     1489 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.660133 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
--rw-rw-rw-   0        0        0    14037 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
--rw-rw-rw-   0        0        0     1183 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.682130 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/
--rw-rw-rw-   0        0        0     7087 2024-05-22 18:39:33.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/IPAsset.py
--rw-rw-rw-   0        0        0    16684 2024-05-22 18:40:50.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/License.py
--rw-rw-rw-   0        0        0    12865 2024-05-22 18:41:32.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/Royalty.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.743027 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/__init__.py
--rw-rw-rw-   0        0        0     3539 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/config.json
--rw-rw-rw-   0        0        0      426 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/config_impl.json
--rw-rw-rw-   0        0        0     7361 2024-05-21 21:24:57.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/generate_client.py
--rw-rw-rw-   0        0        0     5288 2024-05-21 21:26:03.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/generate_client_impl.py
--rw-rw-rw-   0        0        0     1561 2024-05-22 18:49:34.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/story_client.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.747027 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/utils/
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     2444 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/utils/license_terms.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:52:02.416128 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/
--rw-rw-rw-   0        0        0      932 2024-05-22 18:52:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2710 2024-05-22 18:52:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 18:52:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-22 18:52:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-22 18:52:02.000000 story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.906950 story_protocol_python_sdk-0.1.6/
+-rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      219 2024-05-21 20:55:29.000000 story_protocol_python_sdk-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      932 2024-05-22 22:43:16.905362 story_protocol_python_sdk-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.6/README.md
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.1.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 22:43:16.906950 story_protocol_python_sdk-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      904 2024-05-22 22:42:33.000000 story_protocol_python_sdk-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.719350 story_protocol_python_sdk-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.737350 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/
+-rw-rw-rw-   0        0        0      221 2024-05-21 18:30:08.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.764349 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.776352 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/
+-rw-rw-rw-   0        0        0    13409 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
+-rw-rw-rw-   0        0        0     4546 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.787350 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
+-rw-rw-rw-   0        0        0    16117 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
+-rw-rw-rw-   0        0        0     1761 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.799350 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseRegistry/
+-rw-rw-rw-   0        0        0    26905 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
+-rw-rw-rw-   0        0        0     4230 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.818349 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseToken/
+-rw-rw-rw-   0        0        0    23007 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
+-rw-rw-rw-   0        0        0     1159 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.831350 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicensingModule/
+-rw-rw-rw-   0        0        0    19697 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
+-rw-rw-rw-   0        0        0     5246 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.843351 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/
+-rw-rw-rw-   0        0        0    26246 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
+-rw-rw-rw-   0        0        0     4625 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.864351 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyModule/
+-rw-rw-rw-   0        0        0    16029 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
+-rw-rw-rw-   0        0        0     1489 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.875352 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
+-rw-rw-rw-   0        0        0    14037 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
+-rw-rw-rw-   0        0        0     1183 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.881353 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/
+-rw-rw-rw-   0        0        0     7242 2024-05-22 22:41:36.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/IPAsset.py
+-rw-rw-rw-   0        0        0    16684 2024-05-22 18:40:50.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/License.py
+-rw-rw-rw-   0        0        0    12865 2024-05-22 18:41:32.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/Royalty.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.902361 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3539 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/config.json
+-rw-rw-rw-   0        0        0      426 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/config_impl.json
+-rw-rw-rw-   0        0        0     7361 2024-05-21 21:24:57.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/generate_client.py
+-rw-rw-rw-   0        0        0     5288 2024-05-21 21:26:03.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/generate_client_impl.py
+-rw-rw-rw-   0        0        0     1561 2024-05-22 18:49:34.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/story_client.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.904362 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     2444 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/utils/license_terms.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:43:16.762349 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0      932 2024-05-22 22:43:16.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2710 2024-05-22 22:43:16.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 22:43:16.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-22 22:43:16.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-22 22:43:16.000000 story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/top_level.txt
```

### Comparing `story_protocol_python_sdk-0.1.5/LICENSE` & `story_protocol_python_sdk-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/PKG-INFO` & `story_protocol_python_sdk-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: story_protocol_python_sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `story_protocol_python_sdk-0.1.5/setup.py` & `story_protocol_python_sdk-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='story_protocol_python_sdk',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(where='src', exclude=["tests"]),
     package_dir={'': 'src'},
     install_requires=[
         'web3>=5.0.0',
         'pytest',
         'python-dotenv'
     ],
```

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/IPAsset.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/IPAsset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #src/resources/IPAsset.py
 
-import logging
+import logging, time
 from web3 import Web3
 from story_protocol_python_sdk.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
 from story_protocol_python_sdk.abi.LicensingModule.LicensingModule_client import LicensingModuleClient
 from story_protocol_python_sdk.abi.LicenseToken.LicenseToken_client import LicenseTokenClient
 from story_protocol_python_sdk.abi.LicenseRegistry.LicenseRegistry_client import LicenseRegistryClient
 
 # Configure logging
@@ -38,15 +38,14 @@
             ip_id = self._get_ip_id(token_contract, token_id)
             if self._is_registered(ip_id):
                 return {
                     'txHash': None,
                     'ipId': ip_id
                 }
 
-
             # Fetch the current average gas price from the node plus 10%
             current_gas_price = int(self.web3.eth.gas_price * 1.1)
 
             # Build the transaction
             transaction = self.ip_asset_registry_client.build_register_transaction(
                 self.chain_id, token_contract, token_id, {
                     'from': self.account.address,
@@ -58,14 +57,18 @@
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
             
+            if ip_id != None:
+                while self.ip_asset_registry_client.isRegistered(ip_id) == False:
+                    time.sleep(1)
+
             return {
                 'txHash': tx_hash.hex(),
                 'ipId': ip_id
             }
 
         except Exception as e:
             # logger.error(f"Error interacting with contract: {e}")
```

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/License.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/License.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/resources/Royalty.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/resources/Royalty.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/config.json` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/config.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/generate_client.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/generate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/scripts/generate_client_impl.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/scripts/generate_client_impl.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/story_client.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/story_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk/utils/license_terms.py` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk/utils/license_terms.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/PKG-INFO` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: story-protocol-python-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `story_protocol_python_sdk-0.1.5/src/story_protocol_python_sdk.egg-info/SOURCES.txt` & `story_protocol_python_sdk-0.1.6/src/story_protocol_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

