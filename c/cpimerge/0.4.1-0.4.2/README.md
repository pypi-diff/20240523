# Comparing `tmp/cpimerge-0.4.1-py3-none-any.whl.zip` & `tmp/cpimerge-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 11223 bytes, number of entries: 14
+Zip file size: 11235 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 cpimerge/__init__.py
 -rw-r--r--  2.0 unx      249 b- defN 20-Feb-02 00:00 cpimerge/__main__.py
 -rw-r--r--  2.0 unx     1218 b- defN 20-Feb-02 00:00 cpimerge/config.py
 -rw-r--r--  2.0 unx      987 b- defN 20-Feb-02 00:00 cpimerge/descriptions.py
 -rw-r--r--  2.0 unx     1007 b- defN 20-Feb-02 00:00 cpimerge/exclusions.py
--rw-r--r--  2.0 unx    18619 b- defN 20-Feb-02 00:00 cpimerge/gui.py
+-rw-r--r--  2.0 unx    18624 b- defN 20-Feb-02 00:00 cpimerge/gui.py
 -rw-r--r--  2.0 unx      951 b- defN 20-Feb-02 00:00 cpimerge/ical.py
 -rw-r--r--  2.0 unx     3532 b- defN 20-Feb-02 00:00 cpimerge/load.py
 -rw-r--r--  2.0 unx     4910 b- defN 20-Feb-02 00:00 cpimerge/merge.py
-?rw-r--r--  2.0 unx      446 b- defN 20-Feb-02 00:00 cpimerge-0.4.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 cpimerge-0.4.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx       48 b- defN 20-Feb-02 00:00 cpimerge-0.4.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1073 b- defN 20-Feb-02 00:00 cpimerge-0.4.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1078 b- defN 20-Feb-02 00:00 cpimerge-0.4.1.dist-info/RECORD
-14 files, 34205 bytes uncompressed, 9449 bytes compressed:  72.4%
+?rw-r--r--  2.0 unx      446 b- defN 20-Feb-02 00:00 cpimerge-0.4.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 cpimerge-0.4.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx       48 b- defN 20-Feb-02 00:00 cpimerge-0.4.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1073 b- defN 20-Feb-02 00:00 cpimerge-0.4.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1078 b- defN 20-Feb-02 00:00 cpimerge-0.4.2.dist-info/RECORD
+14 files, 34210 bytes uncompressed, 9461 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: cpimerge/load.py
 Comment: 
 
 Filename: cpimerge/merge.py
 Comment: 
 
-Filename: cpimerge-0.4.1.dist-info/METADATA
+Filename: cpimerge-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: cpimerge-0.4.1.dist-info/WHEEL
+Filename: cpimerge-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: cpimerge-0.4.1.dist-info/entry_points.txt
+Filename: cpimerge-0.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cpimerge-0.4.1.dist-info/licenses/LICENSE
+Filename: cpimerge-0.4.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: cpimerge-0.4.1.dist-info/RECORD
+Filename: cpimerge-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cpimerge/gui.py

```diff
@@ -180,15 +180,15 @@
     save_config(config, config_path)
     messagebox.showinfo("Success", "Configuration saved successfully.")
 
 # Open the OUT file in the default application
 def open_output_file(file_path):
     try:
         if platform.system() == 'Windows':
-            subprocess.call(['start', file_path], shell=True)
+            subprocess.call(f'start "" "{file_path}"', shell=True)
         elif platform.system() == 'Darwin':  # macOS
             subprocess.call(['open', file_path])
         elif platform.system() == 'Linux':
             subprocess.call(['xdg-open', file_path])
         else:
             messagebox.showerror("Unsupported OS", "Your operating system is not supported for this operation.")
     except Exception as e:
```

## Comparing `cpimerge-0.4.1.dist-info/licenses/LICENSE` & `cpimerge-0.4.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `cpimerge-0.4.1.dist-info/RECORD` & `cpimerge-0.4.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 cpimerge/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cpimerge/__main__.py,sha256=bMK3PJQeTpKJWgYPAS9SZvsXzQWJaF0lY96pkf6B5A4,249
 cpimerge/config.py,sha256=c3m7eKmyOOfa_f9QbRRG54XhywjGybT8sQiuXJIoc2o,1218
 cpimerge/descriptions.py,sha256=SoJXM7g_e84Nm19jbF4h1rEwsLwXYvfaR-NsSmJCwFU,987
 cpimerge/exclusions.py,sha256=PjlDXcfONogTUBdFW_aSDEGDFRfo0uZ7lve0F4dlA-g,1007
-cpimerge/gui.py,sha256=uVaxTsLzPlFwD65AL3XydhRoEp22c9NVnIKTg_wPfZ0,18619
+cpimerge/gui.py,sha256=30kkHid1YmeXdDsejDVqJQZHSogtQtmXy23oNIxN8xY,18624
 cpimerge/ical.py,sha256=0KNQ40nKe8qkYexvOPM_WLq26qo3Kgu2tZ8MCVhzA_8,951
 cpimerge/load.py,sha256=eSUqs5i3a1viLfBQC2YS3nNUWgRee5dLEC_nLbJAE0c,3532
 cpimerge/merge.py,sha256=K9i59H0iKh3Bc9HTSm3HESSYdEFbRYugvhkIJxfsJLc,4910
-cpimerge-0.4.1.dist-info/METADATA,sha256=YioU2kNBdJRuHsR3QteivYbrs4T8oSGyiOfUCeTQxVQ,446
-cpimerge-0.4.1.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-cpimerge-0.4.1.dist-info/entry_points.txt,sha256=7o9gpwVzU9DJoA91AOZEgWlKyj-8tq3zFfMTvUvs4YI,48
-cpimerge-0.4.1.dist-info/licenses/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
-cpimerge-0.4.1.dist-info/RECORD,,
+cpimerge-0.4.2.dist-info/METADATA,sha256=YKawPluFfKVkxIG-DG0o5hBAks5xd4Ci35E-6UuN6rA,446
+cpimerge-0.4.2.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+cpimerge-0.4.2.dist-info/entry_points.txt,sha256=7o9gpwVzU9DJoA91AOZEgWlKyj-8tq3zFfMTvUvs4YI,48
+cpimerge-0.4.2.dist-info/licenses/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
+cpimerge-0.4.2.dist-info/RECORD,,
```

