# Comparing `tmp/textual-totp-0.9.0.tar.gz` & `tmp/textual_totp-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual-totp-0.9.0.tar", last modified: Tue Dec 12 03:03:52 2023, max compression
+gzip compressed data, was "textual_totp-0.9.1.tar", last modified: Thu May 23 11:45:40 2024, max compression
```

## Comparing `textual-totp-0.9.0.tar` & `textual_totp-0.9.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 03:03:52.531209 textual-totp-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 03:03:52.523209 textual-totp-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 03:03:52.527209 textual-totp-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-12-12 03:03:38.000000 textual-totp-0.9.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      862 2023-12-12 03:03:38.000000 textual-totp-0.9.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-12-12 03:03:38.000000 textual-totp-0.9.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-12 03:03:38.000000 textual-totp-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-12 03:03:38.000000 textual-totp-0.9.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 03:03:52.527209 textual-totp-0.9.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2023-12-12 03:03:38.000000 textual-totp-0.9.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-12 03:03:38.000000 textual-totp-0.9.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-12 03:03:38.000000 textual-totp-0.9.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-12-12 03:03:38.000000 textual-totp-0.9.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2023-12-12 03:03:52.531209 textual-totp-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2023-12-12 03:03:38.000000 textual-totp-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2023-12-12 03:03:38.000000 textual-totp-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-12 03:03:38.000000 textual-totp-0.9.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-12-12 03:03:38.000000 textual-totp-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-12 03:03:52.531209 textual-totp-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 03:03:52.523209 textual-totp-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 03:03:52.527209 textual-totp-0.9.0/src/textual_totp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2023-12-12 03:03:52.000000 textual-totp-0.9.0/src/textual_totp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-12 03:03:52.000000 textual-totp-0.9.0/src/textual_totp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 03:03:52.000000 textual-totp-0.9.0/src/textual_totp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-12 03:03:52.000000 textual-totp-0.9.0/src/textual_totp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-12 03:03:52.000000 textual-totp-0.9.0/src/textual_totp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-12 03:03:52.000000 textual-totp-0.9.0/src/textual_totp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 03:03:52.527209 textual-totp-0.9.0/src/ttotp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 03:03:38.000000 textual-totp-0.9.0/src/ttotp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13692 2023-12-12 03:03:38.000000 textual-totp-0.9.0/src/ttotp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-12 03:03:52.000000 textual-totp-0.9.0/src/ttotp/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44685 2023-12-12 03:03:38.000000 textual-totp-0.9.0/ttotp.png
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-12 03:03:38.000000 textual-totp-0.9.0/ttotp.png.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:45:40.490465 textual_totp-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:45:40.482465 textual_totp-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:45:40.486465 textual_totp-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-23 11:45:29.000000 textual_totp-0.9.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-23 11:45:29.000000 textual_totp-0.9.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-23 11:45:29.000000 textual_totp-0.9.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-23 11:45:29.000000 textual_totp-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-23 11:45:29.000000 textual_totp-0.9.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:45:40.486465 textual_totp-0.9.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-23 11:45:29.000000 textual_totp-0.9.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-23 11:45:29.000000 textual_totp-0.9.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-23 11:45:29.000000 textual_totp-0.9.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-23 11:45:29.000000 textual_totp-0.9.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-23 11:45:40.486465 textual_totp-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-23 11:45:29.000000 textual_totp-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-23 11:45:29.000000 textual_totp-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-23 11:45:29.000000 textual_totp-0.9.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-23 11:45:29.000000 textual_totp-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:45:40.490465 textual_totp-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:45:40.482465 textual_totp-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:45:40.486465 textual_totp-0.9.1/src/textual_totp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-23 11:45:40.000000 textual_totp-0.9.1/src/textual_totp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-23 11:45:40.000000 textual_totp-0.9.1/src/textual_totp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:45:40.000000 textual_totp-0.9.1/src/textual_totp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 11:45:40.000000 textual_totp-0.9.1/src/textual_totp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 11:45:40.000000 textual_totp-0.9.1/src/textual_totp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 11:45:40.000000 textual_totp-0.9.1/src/textual_totp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:45:40.486465 textual_totp-0.9.1/src/ttotp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:45:29.000000 textual_totp-0.9.1/src/ttotp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15988 2024-05-23 11:45:29.000000 textual_totp-0.9.1/src/ttotp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 11:45:40.000000 textual_totp-0.9.1/src/ttotp/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44685 2024-05-23 11:45:29.000000 textual_totp-0.9.1/ttotp.png
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-23 11:45:29.000000 textual_totp-0.9.1/ttotp.png.license
```

### Comparing `textual-totp-0.9.0/.github/workflows/codeql.yml` & `textual_totp-0.9.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `textual-totp-0.9.0/.github/workflows/release.yml` & `textual_totp-0.9.1/.github/workflows/release.yml`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
   release:
     types: [published]
 
 jobs:
   release:
 
     runs-on: ubuntu-22.04
+    environment: release
     permissions:
       # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
     steps:
     - name: Dump GitHub context
       env:
         GITHUB_CONTEXT: ${{ toJson(github) }}
```

### Comparing `textual-totp-0.9.0/.github/workflows/test.yml` & `textual_totp-0.9.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `textual-totp-0.9.0/.pre-commit-config.yaml` & `textual_totp-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `textual-totp-0.9.0/LICENSES/CC0-1.0.txt` & `textual_totp-0.9.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `textual-totp-0.9.0/LICENSES/MIT.txt` & `textual_totp-0.9.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `textual-totp-0.9.0/LICENSES/Unlicense.txt` & `textual_totp-0.9.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `textual-totp-0.9.0/PKG-INFO` & `textual_totp-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-totp
-Version: 0.9.0
+Version: 0.9.1
 Summary: TOTP (authenticator) application using Python & Textual
 Author-email: Jeff Epler <jepler@gmail.com>
 Project-URL: homepage, https://github.com/jepler/textual-totp
 Project-URL: repository, https://github.com/jepler/textual-totp
 Keywords: otp,totp,2fa,authenticator
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -54,14 +54,38 @@
 If you hate security, you can use an insecure command like `cat`, or just test things with `echo`:
 ```toml
 otp-command = "echo 'otpauth://totp/example?algorithm=SHA1&digits=6&secret=IHACDTJ2TFCSLUJLMSHYDBD74FS7OY5B'"
 ```
 
 If the command is a string, it is interpreted with the shell; otherwise, the list of arguments is used directly.
 
+## Auto-exit on idle
+
+To auto exit after a specified inactivity period, use the `auto-exit` setting:
+```toml
+# Exit after 5 minutes (300 seconds) of inactivity
+auto-exit = 300
+```
+Any key event, mouse click, or mouse scroll counts as "activity" and will reset the auto exit timer.
+
+If `auto-exit` is not specified, or it is 0, there is no inactivity timeout.
+
+## Profiles
+
+textual-totp supports multiple profiles. Profiles are organized as sections of the configuration file; if a setting is not specified within a profile section, the global setting is used.
+
+For example, given
+```
+auto-exit=300
+otp-command = ["..."]
+[trusted-location]
+auto-exit=0
+```
+textual-totp will normally exit after 5 minutes of inactivity, but when you run `ttotp --profile trusted-location` auto-exit will be disabled.
+
 # Obtaining TOTP URIs
 
 There are a couple of ways to obtain your TOTP URIs, which are strings that begin `otpauth://totp/`.
 
  * Scan individual QR codes when signing up for 2FA
    * You can photograph or screen capture and then locally decode QR codes using a compatible tool such as [PyQRCode](https://pypi.org/project/PyQRCode/)
  * Scan the QR code(s) from Google Authenticator's "transfer accounts" feature. These are in the form of an "offline otpauth-migration" URL. Decode these with a compatible tool, such as [otpauth-migration-decode](https://github.com/trewlgns/otpauth-migration-decode)
@@ -94,18 +118,18 @@
 
 Copy a code directly to the operating system's clipboard by pressing "c".
 The code will be cleared from the clipboard after 30 seconds.
 Your Operating System may report that `ttotp` "pasted from the clipboard".
 This is because `ttotp` tries to only clear values that it set,
 by checking that the current clipboard value is equal to the value it pasted earlier.
 
-Search for a key by pressing "/" and then entering a modified case insensitive regular expression.
+Search for a key by pressing "/" and then entering sub-strings to search for.
 Press Ctrl+A to show all keys again.
 
-In this type of regular expression, a space ` ` stands for "zero or more characters, followed by whitespace, followed by zero or more characters"; the sequence backslash-space stands for a literal space.
+Textual's built in [fuzzy match](https://textual.textualize.io/api/fuzzy_matcher/) algorithm is used.
 
 This makes it easy to search for e.g., "Jay Doe / example.com" by entering "ja d ex", while not requiring any sophisticated fuzzy search technology.
 
 Due to the simple way this is implemented, a space character inside a character class does not function as expected.
 Since complicated regular expressions are likely seldom used, this is not likely to be a huge limitation.
 
 Exit the app with Ctrl+C.
```

### Comparing `textual-totp-0.9.0/README.md` & `textual_totp-0.9.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -31,14 +31,38 @@
 If you hate security, you can use an insecure command like `cat`, or just test things with `echo`:
 ```toml
 otp-command = "echo 'otpauth://totp/example?algorithm=SHA1&digits=6&secret=IHACDTJ2TFCSLUJLMSHYDBD74FS7OY5B'"
 ```
 
 If the command is a string, it is interpreted with the shell; otherwise, the list of arguments is used directly.
 
+## Auto-exit on idle
+
+To auto exit after a specified inactivity period, use the `auto-exit` setting:
+```toml
+# Exit after 5 minutes (300 seconds) of inactivity
+auto-exit = 300
+```
+Any key event, mouse click, or mouse scroll counts as "activity" and will reset the auto exit timer.
+
+If `auto-exit` is not specified, or it is 0, there is no inactivity timeout.
+
+## Profiles
+
+textual-totp supports multiple profiles. Profiles are organized as sections of the configuration file; if a setting is not specified within a profile section, the global setting is used.
+
+For example, given
+```
+auto-exit=300
+otp-command = ["..."]
+[trusted-location]
+auto-exit=0
+```
+textual-totp will normally exit after 5 minutes of inactivity, but when you run `ttotp --profile trusted-location` auto-exit will be disabled.
+
 # Obtaining TOTP URIs
 
 There are a couple of ways to obtain your TOTP URIs, which are strings that begin `otpauth://totp/`.
 
  * Scan individual QR codes when signing up for 2FA
    * You can photograph or screen capture and then locally decode QR codes using a compatible tool such as [PyQRCode](https://pypi.org/project/PyQRCode/)
  * Scan the QR code(s) from Google Authenticator's "transfer accounts" feature. These are in the form of an "offline otpauth-migration" URL. Decode these with a compatible tool, such as [otpauth-migration-decode](https://github.com/trewlgns/otpauth-migration-decode)
@@ -71,18 +95,18 @@
 
 Copy a code directly to the operating system's clipboard by pressing "c".
 The code will be cleared from the clipboard after 30 seconds.
 Your Operating System may report that `ttotp` "pasted from the clipboard".
 This is because `ttotp` tries to only clear values that it set,
 by checking that the current clipboard value is equal to the value it pasted earlier.
 
-Search for a key by pressing "/" and then entering a modified case insensitive regular expression.
+Search for a key by pressing "/" and then entering sub-strings to search for.
 Press Ctrl+A to show all keys again.
 
-In this type of regular expression, a space ` ` stands for "zero or more characters, followed by whitespace, followed by zero or more characters"; the sequence backslash-space stands for a literal space.
+Textual's built in [fuzzy match](https://textual.textualize.io/api/fuzzy_matcher/) algorithm is used.
 
 This makes it easy to search for e.g., "Jay Doe / example.com" by entering "ja d ex", while not requiring any sophisticated fuzzy search technology.
 
 Due to the simple way this is implemented, a space character inside a character class does not function as expected.
 Since complicated regular expressions are likely seldom used, this is not likely to be a huge limitation.
 
 Exit the app with Ctrl+C.
```

### Comparing `textual-totp-0.9.0/pyproject.toml` & `textual_totp-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `textual-totp-0.9.0/src/textual_totp.egg-info/PKG-INFO` & `textual_totp-0.9.1/src/textual_totp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-totp
-Version: 0.9.0
+Version: 0.9.1
 Summary: TOTP (authenticator) application using Python & Textual
 Author-email: Jeff Epler <jepler@gmail.com>
 Project-URL: homepage, https://github.com/jepler/textual-totp
 Project-URL: repository, https://github.com/jepler/textual-totp
 Keywords: otp,totp,2fa,authenticator
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -54,14 +54,38 @@
 If you hate security, you can use an insecure command like `cat`, or just test things with `echo`:
 ```toml
 otp-command = "echo 'otpauth://totp/example?algorithm=SHA1&digits=6&secret=IHACDTJ2TFCSLUJLMSHYDBD74FS7OY5B'"
 ```
 
 If the command is a string, it is interpreted with the shell; otherwise, the list of arguments is used directly.
 
+## Auto-exit on idle
+
+To auto exit after a specified inactivity period, use the `auto-exit` setting:
+```toml
+# Exit after 5 minutes (300 seconds) of inactivity
+auto-exit = 300
+```
+Any key event, mouse click, or mouse scroll counts as "activity" and will reset the auto exit timer.
+
+If `auto-exit` is not specified, or it is 0, there is no inactivity timeout.
+
+## Profiles
+
+textual-totp supports multiple profiles. Profiles are organized as sections of the configuration file; if a setting is not specified within a profile section, the global setting is used.
+
+For example, given
+```
+auto-exit=300
+otp-command = ["..."]
+[trusted-location]
+auto-exit=0
+```
+textual-totp will normally exit after 5 minutes of inactivity, but when you run `ttotp --profile trusted-location` auto-exit will be disabled.
+
 # Obtaining TOTP URIs
 
 There are a couple of ways to obtain your TOTP URIs, which are strings that begin `otpauth://totp/`.
 
  * Scan individual QR codes when signing up for 2FA
    * You can photograph or screen capture and then locally decode QR codes using a compatible tool such as [PyQRCode](https://pypi.org/project/PyQRCode/)
  * Scan the QR code(s) from Google Authenticator's "transfer accounts" feature. These are in the form of an "offline otpauth-migration" URL. Decode these with a compatible tool, such as [otpauth-migration-decode](https://github.com/trewlgns/otpauth-migration-decode)
@@ -94,18 +118,18 @@
 
 Copy a code directly to the operating system's clipboard by pressing "c".
 The code will be cleared from the clipboard after 30 seconds.
 Your Operating System may report that `ttotp` "pasted from the clipboard".
 This is because `ttotp` tries to only clear values that it set,
 by checking that the current clipboard value is equal to the value it pasted earlier.
 
-Search for a key by pressing "/" and then entering a modified case insensitive regular expression.
+Search for a key by pressing "/" and then entering sub-strings to search for.
 Press Ctrl+A to show all keys again.
 
-In this type of regular expression, a space ` ` stands for "zero or more characters, followed by whitespace, followed by zero or more characters"; the sequence backslash-space stands for a literal space.
+Textual's built in [fuzzy match](https://textual.textualize.io/api/fuzzy_matcher/) algorithm is used.
 
 This makes it easy to search for e.g., "Jay Doe / example.com" by entering "ja d ex", while not requiring any sophisticated fuzzy search technology.
 
 Due to the simple way this is implemented, a space character inside a character class does not function as expected.
 Since complicated regular expressions are likely seldom used, this is not likely to be a huge limitation.
 
 Exit the app with Ctrl+C.
```

### Comparing `textual-totp-0.9.0/src/textual_totp.egg-info/SOURCES.txt` & `textual_totp-0.9.1/src/textual_totp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `textual-totp-0.9.0/src/ttotp/__main__.py` & `textual_totp-0.9.1/src/ttotp/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,49 +11,59 @@
 import pathlib
 import subprocess
 from urllib.parse import parse_qsl, unquote, urlparse
 import re
 from typing import TYPE_CHECKING, Any, Sequence, cast
 
 import rich.text
+from textual.fuzzy import Matcher
 from textual.app import App, ComposeResult
+from textual.events import Key, MouseDown, MouseUp, MouseScrollDown, MouseScrollUp
 from textual.widget import Widget
 from textual.widgets import Label, Footer, ProgressBar, Button, Input
 from textual.binding import Binding
 from textual.containers import VerticalScroll, Horizontal
 from textual.css.query import DOMQuery
 from textual.timer import Timer
 
 import click
 import pyotp
 import platformdirs
 import tomllib
 
+from textual._ansi_sequences import ANSI_SEQUENCES_KEYS
+from textual.keys import Keys
+from typing import TypeGuard  # use `typing_extensions` for Python 3.9 and below
+
 # workaround for pyperclip being un-typed
 if TYPE_CHECKING:
 
     def pyperclip_paste() -> str:
         ...
 
     def pyperclip_copy(data: str) -> None:
         ...
 else:
     from pyperclip import paste as pyperclip_paste
     from pyperclip import copy as pyperclip_copy
 
-from typing import TypeGuard  # use `typing_extensions` for Python 3.9 and below
-
 
 def is_str_list(val: Any) -> TypeGuard[list[str]]:
     """Determines whether all objects in the list are strings"""
     if not isinstance(val, list):
         return False
     return all(isinstance(x, str) for x in val)
 
 
+# Monkeypatch escape key as meaning "F9", WFM
+# ignore typing here because ANSI_SEQUENCES_KEYS is a Mapping[] which is read-only as
+# far as mypy is concerned.
+ANSI_SEQUENCES_KEYS["\x1b\x1b"] = (Keys.F9,)  # type: ignore
+
+
 # Copied from pyotp with the issuer mismatch check removed and HTOP support removed
 def parse_uri(uri: str) -> pyotp.TOTP:
     """
     Parses the provisioning URI for the TOTP
 
     See also:
         https://github.com/google/google-authenticator/wiki/Key-Uri-Format
@@ -170,14 +180,15 @@
 
 
 class SearchInput(Input, can_focus=False):
     BINDINGS = [
         Binding("up", "focus_previous", show=False),
         Binding("down", "focus_next", show=False),
         Binding("ctrl+a", "clear_search", "Show all", show=True),
+        Binding("F9", "clear_search", show=True),
     ]
 
     def on_focus(self) -> None:
         self.placeholder = "Enter search expression"
 
     def on_blur(self) -> None:
         self.placeholder = "Type / to search"
@@ -274,28 +285,51 @@
     """
 
     BINDINGS = [
         Binding("/", "search"),
         Binding("ctrl+a", "clear_search", "Show all", show=True),
     ]
 
-    def __init__(self, tokens: Sequence[pyotp.TOTP]) -> None:
+    def __init__(
+        self, tokens: Sequence[pyotp.TOTP], timeout: int | float | None
+    ) -> None:
         super().__init__()
         self.tokens = tokens
         self.otp_data: list[TOTPData] = []
         self.timer: Timer | None = None
         self.clear_clipboard_time: Timer | None = None
+        self.exit_time: Timer | None = None
+        self.warn_exit_time: Timer | None = None
+        self.timeout: int | float | None = timeout
         self.copied = ""
 
     def on_mount(self) -> None:
         self.timer_func()
         self.timer = self.set_interval(1, self.timer_func)
         self.clear_clipboard_timer = self.set_timer(
             30, self.clear_clipboard_func, pause=True
         )
+        if self.timeout:
+            self.exit_time = self.set_timer(self.timeout, self.action_quit)
+            warn_timeout = max(self.timeout / 2, self.timeout - 10)
+            self.warn_exit_time = self.set_timer(warn_timeout, self.warn_quit)
+
+    def reset_exit_timers(self) -> None:
+        if self.exit_time:
+            self.exit_time.reset()
+        if self.warn_exit_time:
+            self.warn_exit_time.reset()
+
+    async def on_event(self, event: Any) -> None:
+        if isinstance(event, (Key, MouseDown, MouseUp, MouseScrollDown, MouseScrollUp)):
+            self.reset_exit_timers()
+        await super().on_event(event)
+
+    def warn_quit(self) -> None:
+        self.notify("Will exit soon due to inactivity", title="Auto-exit")
 
     def clear_clipboard_func(self) -> None:
         if pyperclip_paste() == self.copied:
             self.notify("Clipboard cleared", title="")
             pyperclip_copy("")
 
     def timer_func(self) -> None:
@@ -350,28 +384,41 @@
 
     def action_clear_search(self) -> None:
         self.search.clear()
         if self.focused is self.search:
             self.screen.focus_next()
 
     def on_input_changed(self, event: Input.Changed) -> None:
-        haystack = event.value.replace(" ", ".* .*")
-        try:
-            rx = re.compile(haystack, re.I)
-        except re.error:
-            self.search.add_class("error")
-            return
-        self.search.remove_class("error")
-        for otp in self.otp_data:
-            parent = otp.name_widget.parent
-            assert parent is not None
-            if rx.search(otp.name):
-                parent.remove_class("otp-hidden")
-            else:
-                parent.add_class("otp-hidden")
+        with self.batch_update():
+            needle = event.value
+            if not needle:
+                for otp in self.otp_data:
+                    name_widget = otp.name_widget
+                    parent = name_widget.parent
+                    assert parent is not None
+                    parent.remove_class("otp-hidden")
+                    name_widget.update(
+                        rich.text.Text(otp.name, overflow="ellipsis", no_wrap=True)
+                    )
+                return
+
+            matcher = Matcher(needle)
+            for otp in self.otp_data:
+                name_widget = otp.name_widget
+                parent = name_widget.parent
+                assert parent is not None
+                score = matcher.match(otp.name)
+                if score > 0:
+                    highlighted = matcher.highlight(otp.name)
+                    highlighted.overflow = "ellipsis"
+                    highlighted.no_wrap = True
+                    name_widget.update(highlighted)
+                    parent.remove_class("otp-hidden")
+                else:
+                    parent.add_class("otp-hidden")
 
     def on_input_submitted(self, event: Input.Changed) -> None:
         self.screen.focus_next()
 
 
 @click.command
 @click.option(
@@ -414,35 +461,41 @@
     if not config.exists():
         config_hint(f"The configuration file {config} does not exist.")
 
     with open(config, "rb") as f:
         config_data = tomllib.load(f)
 
     if profile:
-        config_data = config_data.get(profile, None)
-        if config_data is None:
+        profile_data = config_data.get(profile, None)
+        if profile_data is None:
             config_hint(f"The profile {profile!r} file does not exist.")
+        config_data.update(profile_data)
 
     otp_command = config_data.get("otp-command")
     if otp_command is None:
         config_hint("The otp-command value is missing.")
 
     if isinstance(otp_command, str) or is_str_list(otp_command):
         c = subprocess.check_output(
             otp_command, shell=isinstance(otp_command, str), text=True
         )
     else:
         config_hint("The otp-command value must be a string or list of strings.")
 
+    timeout = config_data.get("auto-exit", None)
+    if timeout is not None:
+        if not isinstance(timeout, (float, int)):
+            config_hint("If specified, the auto-exit value must be a number.")
+
     tokens: list[pyotp.TOTP] = []
     for row in c.strip().split("\n"):
         if row.startswith("otpauth://"):
             tokens.append(parse_uri(row))
 
     if not tokens:
         config_hint("No tokens were found when running the given command.")
 
-    TTOTP(tokens).run()
+    TTOTP(tokens, timeout).run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `textual-totp-0.9.0/ttotp.png` & `textual_totp-0.9.1/ttotp.png`

 * *Files identical despite different names*

