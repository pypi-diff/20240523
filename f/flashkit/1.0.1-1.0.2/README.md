# Comparing `tmp/flashkit-1.0.1.tar.gz` & `tmp/flashkit-1.0.2.tar.gz`

## Comparing `flashkit-1.0.1.tar` & `flashkit-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 flashkit-1.0.1/lint.sh
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 flashkit-1.0.1/requirements.txt
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 flashkit-1.0.1/flashkit/__init__.py
--rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 flashkit-1.0.1/flashkit/cart.py
--rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 flashkit-1.0.1/flashkit/device.py
--rwxr-xr-x   0        0        0     9230 2020-02-02 00:00:00.000000 flashkit-1.0.1/flashkit/flashkit.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 flashkit-1.0.1/.gitignore
--rw-r--r--   0        0        0    34916 2020-02-02 00:00:00.000000 flashkit-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 flashkit-1.0.1/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 flashkit-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 flashkit-1.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 flashkit-1.0.2/lint.sh
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 flashkit-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 flashkit-1.0.2/flashkit/__init__.py
+-rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 flashkit-1.0.2/flashkit/cart.py
+-rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 flashkit-1.0.2/flashkit/device.py
+-rwxr-xr-x   0        0        0     9521 2020-02-02 00:00:00.000000 flashkit-1.0.2/flashkit/flashkit.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 flashkit-1.0.2/.gitignore
+-rw-r--r--   0        0        0    34916 2020-02-02 00:00:00.000000 flashkit-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 flashkit-1.0.2/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 flashkit-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 flashkit-1.0.2/PKG-INFO
```

### Comparing `flashkit-1.0.1/lint.sh` & `flashkit-1.0.2/lint.sh`

 * *Files identical despite different names*

### Comparing `flashkit-1.0.1/flashkit/cart.py` & `flashkit-1.0.2/flashkit/cart.py`

 * *Files identical despite different names*

### Comparing `flashkit-1.0.1/flashkit/device.py` & `flashkit-1.0.2/flashkit/device.py`

 * *Files identical despite different names*

### Comparing `flashkit-1.0.1/flashkit/flashkit.py` & `flashkit-1.0.2/flashkit/flashkit.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # last sync with upstream C# version:
 #   commit 8194b0d72ee0036447532c277778ec503bd8e4c6
 #   Author: krikzz <biokrik@gmail.com>
 #   Date:   Wed Dec 20 01:37:44 2023 +0100
 
+"""
+Drive the Krikzz FlashKit Programmer MD from the command-line to rewrite Sega
+Genesis / MegaDrive flash carts.
+"""
 
 import argparse
 import datetime
 import hashlib
 
 from .device import FlashKitDevice
 from .cart import Cart, TIME_REGISTER
@@ -281,15 +285,15 @@
       description=__doc__,
       epilog='Use "flashkit <command> --help" to see options for each command.')
   parser.add_argument('-p', '--port',
       help='Serial port device to use; default is to autodetect')
 
   subparsers = parser.add_subparsers(
       title='available commands',
-      metavar='command', dest='command', required=True)
+      metavar='command', dest='command')
 
   check_parser = subparsers.add_parser('check',
       help='Print info about the attached cart')
   check_parser.set_defaults(
       func=lambda args: check(args.port))
 
   read_rom_parser = subparsers.add_parser('read-rom',
@@ -317,13 +321,19 @@
       help='Write the RAM from a file to the cart')
   write_ram_parser.add_argument('-i', '--input', required=True,
       help='Input file; required')
   write_ram_parser.set_defaults(
       func=lambda args: writeRam(args.port, args.input))
 
   args = parser.parse_args()
-  # Run the "func" associated with whichever subcommand was given:
-  args.func(args)
+
+  if args.command:
+    # Run the "func" associated with whichever subcommand was given:
+    args.func(args)
+  else:
+    # Explicitly print help, instead of making command required.
+    # This way, we see the full help instead of the short version
+    parser.print_help()
 
 
 if __name__ == '__main__':
   main()
```

### Comparing `flashkit-1.0.1/LICENSE.md` & `flashkit-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flashkit-1.0.1/README.md` & `flashkit-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flashkit-1.0.1/pyproject.toml` & `flashkit-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flashkit"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Joey Parrish", email="joey.parrish@gmail.com" },
 ]
 description = "Drive the Krikzz FlashKit Programmer MD to flash Sega Genesis carts from the command-line."
 readme = "README.md"
 # This comes from the usage of require=True in argparse's add_subparsers()
 requires-python = ">=3.7"
```

### Comparing `flashkit-1.0.1/PKG-INFO` & `flashkit-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashkit
-Version: 1.0.1
+Version: 1.0.2
 Summary: Drive the Krikzz FlashKit Programmer MD to flash Sega Genesis carts from the command-line.
 Project-URL: Homepage, https://github.com/joeyparrish/flashkit-md-py
 Project-URL: Issues, https://github.com/joeyparrish/flashkit-md-py/issues
 Author-email: Joey Parrish <joey.parrish@gmail.com>
 License-File: LICENSE.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

