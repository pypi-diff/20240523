# Comparing `tmp/mailck-0.3.1.tar.gz` & `tmp/mailck-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailck-0.3.1.tar", max compression
+gzip compressed data, was "mailck-0.4.0.tar", max compression
```

## Comparing `mailck-0.3.1.tar` & `mailck-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    32471 2023-12-20 14:28:07.561795 mailck-0.3.1/LICENSE
--rw-r--r--   0        0        0     4229 2024-05-03 15:50:48.456584 mailck-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-05-03 15:50:22.009071 mailck-0.3.1/mailck/__init__.py
--rw-r--r--   0        0        0     7273 2024-05-03 15:50:22.005738 mailck-0.3.1/mailck/main.py
--rw-r--r--   0        0        0      645 2024-05-03 15:49:33.404184 mailck-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4905 1970-01-01 00:00:00.000000 mailck-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-12-20 14:28:07.561795 mailck-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4229 2024-05-03 15:50:48.456584 mailck-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 15:50:22.009071 mailck-0.4.0/mailck/__init__.py
+-rw-r--r--   0        0        0     7554 2024-05-23 19:16:18.193075 mailck-0.4.0/mailck/main.py
+-rw-r--r--   0        0        0      645 2024-05-23 19:19:21.832316 mailck-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4905 1970-01-01 00:00:00.000000 mailck-0.4.0/PKG-INFO
```

### Comparing `mailck-0.3.1/LICENSE` & `mailck-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mailck-0.3.1/README.md` & `mailck-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mailck-0.3.1/mailck/main.py` & `mailck-0.4.0/mailck/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,18 @@
 
     logger.debug("checking mail...")
     mail = imaplib.IMAP4_SSL(host=r.server, port=r.port)
     (retcode, capabilities) = mail.login(r.username, r.password)
     mail.list()
     mail.select(r.folder, readonly=True)
 
+    _check_time = ""
+    if r.show_check_time:
+        _check_time = datetime.now().strftime('%Y-%m-%d %H:%M')
+
     n = 0
     (retcode, messages) = mail.search(None, r.message_type)
     if retcode == "OK":
         for num in messages[0].split():
             n = n + 1
             if r.show_messages:
                 resp_code, mail_data = mail.fetch(num, "(RFC822)")
@@ -135,15 +139,15 @@
                     )
                     logger.critical(f"Subject    : {message.get('Subject')}")
                     logger.critical("---------------------------------")
                 else:
                     pass
 
     # the base/normal output which is the # of messages only.
-    logger.critical(f"{r.output_prefix}{n}{r.output_suffix}")
+    logger.critical(f"{r.output_prefix}{n}{r.output_suffix}{_check_time}")
 
     mail.close()
     mail.logout()
 
 
 def app():
     usage = "usage: %prog [options] arg"
@@ -217,14 +221,20 @@
     parser.add_option(
         "--suffix",
         dest="output_suffix",
         default="",
         help="suffix to add to output (e.g. ' (unread)', ' (new)')",
     )
     parser.add_option(
+        "--show-check-time",
+        dest="show_check_time",
+        default=False,
+        help="show check time in results",
+    )
+    parser.add_option(
         "--version",
         action="store_true",
         dest="showVersion",
         help="show script version and exit",
     )
 
     (options, args) = parser.parse_args()
```

### Comparing `mailck-0.3.1/pyproject.toml` & `mailck-0.4.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [internal]
 created = 2023-12-20
-modified = 2024-01-06
+modified = 2024-05-23
 
 
 [tool.poetry]
 name = "mailck"
-version = "0.3.1"
+version = "0.4.0"
 description = "a simple mail check utility, currently supporting IMAP"
 authors = ["drad <sa@adercon.com>"]
 maintainers = ["drad <sa@adercon.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://gitlab.com/drad/mailck"
 repository = "https://gitlab.com/drad/mailck"
```

### Comparing `mailck-0.3.1/PKG-INFO` & `mailck-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailck
-Version: 0.3.1
+Version: 0.4.0
 Summary: a simple mail check utility, currently supporting IMAP
 Home-page: https://gitlab.com/drad/mailck
 License: GPL-3.0-only
 Keywords: mail,imap,check,conky,cron,terminal,email
 Author: drad
 Author-email: sa@adercon.com
 Maintainer: drad
```

