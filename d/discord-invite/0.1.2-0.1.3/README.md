# Comparing `tmp/discord_invite-0.1.2.tar.gz` & `tmp/discord_invite-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_invite-0.1.2.tar", last modified: Wed May 22 12:42:57 2024, max compression
+gzip compressed data, was "discord_invite-0.1.3.tar", last modified: Thu May 23 02:34:45 2024, max compression
```

## Comparing `discord_invite-0.1.2.tar` & `discord_invite-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 12:42:57.274047 discord_invite-0.1.2/
--rw-rw-rw-   0        0        0      608 2024-05-22 12:42:57.273056 discord_invite-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-05-22 11:55:50.000000 discord_invite-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 12:42:57.272543 discord_invite-0.1.2/discord_invite.egg-info/
--rw-rw-rw-   0        0        0      608 2024-05-22 12:42:57.000000 discord_invite-0.1.2/discord_invite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-05-22 12:42:57.000000 discord_invite-0.1.2/discord_invite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 12:42:57.000000 discord_invite-0.1.2/discord_invite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-22 12:42:57.000000 discord_invite-0.1.2/discord_invite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 12:42:57.000000 discord_invite-0.1.2/discord_invite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 12:42:57.274047 discord_invite-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      669 2024-05-22 12:29:48.000000 discord_invite-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:34:45.493356 discord_invite-0.1.3/
+-rw-rw-rw-   0        0        0      608 2024-05-23 02:34:45.492357 discord_invite-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-22 11:55:50.000000 discord_invite-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 02:34:45.492357 discord_invite-0.1.3/discord_invite.egg-info/
+-rw-rw-rw-   0        0        0      608 2024-05-23 02:34:45.000000 discord_invite-0.1.3/discord_invite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-05-23 02:34:45.000000 discord_invite-0.1.3/discord_invite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 02:34:45.000000 discord_invite-0.1.3/discord_invite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-23 02:34:45.000000 discord_invite-0.1.3/discord_invite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 02:34:45.000000 discord_invite-0.1.3/discord_invite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 02:34:45.493356 discord_invite-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      669 2024-05-23 02:34:23.000000 discord_invite-0.1.3/setup.py
```

### Comparing `discord_invite-0.1.2/PKG-INFO` & `discord_invite-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord_invite
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python of discord joiner
 Home-page: https://github.com/LaciaHax/discord_joiner
 Author: Lacia Hax
 Author-email: yuitanmiruku@outlook.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `discord_invite-0.1.2/discord_invite.egg-info/PKG-INFO` & `discord_invite-0.1.3/discord_invite.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-invite
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python of discord joiner
 Home-page: https://github.com/LaciaHax/discord_joiner
 Author: Lacia Hax
 Author-email: yuitanmiruku@outlook.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `discord_invite-0.1.2/setup.py` & `discord_invite-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='discord_invite',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'tls-client',
     ],
     author='Lacia Hax',
     author_email='yuitanmiruku@outlook.jp',
     description='A python of discord joiner',
```

