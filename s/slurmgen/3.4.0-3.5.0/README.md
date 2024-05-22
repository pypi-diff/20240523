# Comparing `tmp/slurmgen-3.4.0.tar.gz` & `tmp/slurmgen-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurmgen-3.4.0.tar", last modified: Fri May  3 06:49:15 2024, max compression
+gzip compressed data, was "slurmgen-3.5.0.tar", last modified: Wed May 22 22:39:13 2024, max compression
```

## Comparing `slurmgen-3.4.0.tar` & `slurmgen-3.5.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-03 06:49:15.151745 slurmgen-3.4.0/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      278 2023-11-27 16:21:41.000000 slurmgen-3.4.0/.gitignore
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1303 2023-11-27 14:39:14.000000 slurmgen-3.4.0/LICENSE.txt
--rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-03 06:49:15.151745 slurmgen-3.4.0/PKG-INFO
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     2093 2024-03-30 02:44:17.000000 slurmgen-3.4.0/README.md
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-03 06:49:15.151745 slurmgen-3.4.0/example/
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-03 06:49:15.151745 slurmgen-3.4.0/example/data_output/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-05-03 06:42:15.000000 slurmgen-3.4.0/example/data_output/goodbye.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       55 2024-05-03 06:42:15.000000 slurmgen-3.4.0/example/data_output/hello.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      866 2024-05-03 05:48:33.000000 slurmgen-3.4.0/example/job_def.json
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-03-21 18:33:57.000000 slurmgen-3.4.0/example/job_tmpl.json
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1027 2023-11-27 20:00:16.000000 slurmgen-3.4.0/example/run_slurm.py
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-03 06:49:15.151745 slurmgen-3.4.0/example/slurm_output/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      756 2024-05-03 06:42:15.000000 slurmgen-3.4.0/example/slurm_output/test.log
--rwxrw-r--   0 tguillod  (1000) tguillod  (1000)     1277 2024-05-03 06:42:15.000000 slurmgen-3.4.0/example/slurm_output/test.sh
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1566 2024-05-03 05:50:27.000000 slurmgen-3.4.0/pyproject.toml
--rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     1719 2023-11-27 16:21:41.000000 slurmgen-3.4.0/run_release.sh
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       38 2024-05-03 06:49:15.151745 slurmgen-3.4.0/setup.cfg
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-03 06:49:15.151745 slurmgen-3.4.0/slurmgen/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      176 2024-05-03 05:52:06.000000 slurmgen-3.4.0/slurmgen/__init__.py
--rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     8589 2024-05-03 06:22:59.000000 slurmgen-3.4.0/slurmgen/gen.py
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     2924 2024-05-03 06:38:38.000000 slurmgen-3.4.0/slurmgen/run.py
--rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     7501 2024-05-03 06:42:15.000000 slurmgen-3.4.0/slurmgen/script.py
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        5 2024-05-03 06:49:15.000000 slurmgen-3.4.0/slurmgen/version.txt
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-03 06:49:15.151745 slurmgen-3.4.0/slurmgen.egg-info/
--rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-03 06:49:15.000000 slurmgen-3.4.0/slurmgen.egg-info/PKG-INFO
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      503 2024-05-03 06:49:15.000000 slurmgen-3.4.0/slurmgen.egg-info/SOURCES.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        1 2024-05-03 06:49:15.000000 slurmgen-3.4.0/slurmgen.egg-info/dependency_links.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       45 2024-05-03 06:49:15.000000 slurmgen-3.4.0/slurmgen.egg-info/entry_points.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        9 2024-05-03 06:49:15.000000 slurmgen-3.4.0/slurmgen.egg-info/top_level.txt
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-22 22:39:13.526689 slurmgen-3.5.0/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      278 2023-11-27 16:21:41.000000 slurmgen-3.5.0/.gitignore
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1303 2023-11-27 14:39:14.000000 slurmgen-3.5.0/LICENSE.txt
+-rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-22 22:39:13.526689 slurmgen-3.5.0/PKG-INFO
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     2093 2024-03-30 02:44:17.000000 slurmgen-3.5.0/README.md
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-22 22:39:13.526689 slurmgen-3.5.0/example/
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-22 22:39:13.526689 slurmgen-3.5.0/example/data_output/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-05-22 22:37:06.000000 slurmgen-3.5.0/example/data_output/goodbye.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       55 2024-05-22 22:37:06.000000 slurmgen-3.5.0/example/data_output/hello.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      756 2024-05-22 21:53:10.000000 slurmgen-3.5.0/example/job_def.json
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-05-22 21:27:31.000000 slurmgen-3.5.0/example/job_tmpl.json
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1027 2023-11-27 20:00:16.000000 slurmgen-3.5.0/example/run_slurm.py
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-22 22:39:13.526689 slurmgen-3.5.0/example/slurm_output/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      756 2024-05-22 22:37:20.000000 slurmgen-3.5.0/example/slurm_output/test.log
+-rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     1271 2024-05-22 22:37:20.000000 slurmgen-3.5.0/example/slurm_output/test.sh
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1566 2024-05-03 05:50:27.000000 slurmgen-3.5.0/pyproject.toml
+-rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     1719 2023-11-27 16:21:41.000000 slurmgen-3.5.0/run_release.sh
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       38 2024-05-22 22:39:13.526689 slurmgen-3.5.0/setup.cfg
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-22 22:39:13.526689 slurmgen-3.5.0/slurmgen/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      176 2024-05-03 05:52:06.000000 slurmgen-3.5.0/slurmgen/__init__.py
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      265 2024-05-22 21:17:32.000000 slurmgen-3.5.0/slurmgen/error.py
+-rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     8106 2024-05-22 21:53:34.000000 slurmgen-3.5.0/slurmgen/gen.py
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     2836 2024-05-22 21:17:59.000000 slurmgen-3.5.0/slurmgen/run.py
+-rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     7880 2024-05-22 21:42:13.000000 slurmgen-3.5.0/slurmgen/script.py
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        5 2024-05-22 22:39:13.000000 slurmgen-3.5.0/slurmgen/version.txt
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-22 22:39:13.526689 slurmgen-3.5.0/slurmgen.egg-info/
+-rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-22 22:39:13.000000 slurmgen-3.5.0/slurmgen.egg-info/PKG-INFO
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      521 2024-05-22 22:39:13.000000 slurmgen-3.5.0/slurmgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        1 2024-05-22 22:39:13.000000 slurmgen-3.5.0/slurmgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       45 2024-05-22 22:39:13.000000 slurmgen-3.5.0/slurmgen.egg-info/entry_points.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        9 2024-05-22 22:39:13.000000 slurmgen-3.5.0/slurmgen.egg-info/top_level.txt
```

### Comparing `slurmgen-3.4.0/LICENSE.txt` & `slurmgen-3.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slurmgen-3.4.0/PKG-INFO` & `slurmgen-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmgen
-Version: 3.4.0
+Version: 3.5.0
 Summary: SlurmGen - Simple Slurm Manager
 Author-email: Thomas Guillod <guillod@otvam.ch>
 Maintainer-email: Thomas Guillod <guillod@otvam.ch>
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/otvam/slurmgen
 Project-URL: Repository, https://github.com/otvam/slurmgen
 Project-URL: Releases, https://github.com/otvam/slurmgen/releases
```

### Comparing `slurmgen-3.4.0/README.md` & `slurmgen-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `slurmgen-3.4.0/example/job_def.json` & `slurmgen-3.5.0/example/job_def.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6607142857142857%*

 * *Differences: {"'commands'": "{0: {'cmd': 'python3 --version', delete: ['executable', 'arguments']}, 1: {'cmd': "*

 * *               '\'python3 run_slurm.py "hello" "hello world!"\', delete: [\'executable\', '*

 * *               '\'arguments\']}, 2: {\'cmd\': \'python3 run_slurm.py "goodbye" "goodbye world!"\', '*

 * *               "delete: ['executable', 'arguments']}}",*

 * * "'envs'": "OrderedDict([('PYTHONUNBUFFERED', '1'), ('VARWORLD', '$var')])",*

 * * 'delete': "['vars']"}*

```diff
@@ -1,35 +1,26 @@
 {
     "commands": [
         {
-            "arguments": [
-                "--version"
-            ],
-            "executable": "python3",
+            "cmd": "python3 --version",
             "tag": "version"
         },
         {
-            "arguments": [
-                "run_slurm.py",
-                "hello",
-                "hello world!"
-            ],
-            "executable": "python3",
+            "cmd": "python3 run_slurm.py \"hello\" \"hello world!\"",
             "tag": "hello"
         },
         {
-            "arguments": [
-                "run_slurm.py",
-                "goodbye",
-                "goodbye world!"
-            ],
-            "executable": "python3",
+            "cmd": "python3 run_slurm.py \"goodbye\" \"goodbye world!\"",
             "tag": "goodbye"
         }
     ],
+    "envs": {
+        "PYTHONUNBUFFERED": "1",
+        "VARWORLD": "$var"
+    },
     "folder": {
         "folder_create": [
             "data_output"
         ],
         "folder_delete": [
             "data_output"
         ],
@@ -38,13 +29,9 @@
     "overwrite": true,
     "pragmas": {
         "mem": "8G",
         "nodes": "1",
         "ntasks-per-node": "2",
         "time": "4:00:00"
     },
-    "tag": "$title",
-    "vars": {
-        "PYTHONUNBUFFERED": "1",
-        "VARWORLD": "$var"
-    }
+    "tag": "$title"
 }
```

### Comparing `slurmgen-3.4.0/example/run_slurm.py` & `slurmgen-3.5.0/example/run_slurm.py`

 * *Files identical despite different names*

### Comparing `slurmgen-3.4.0/example/slurm_output/test.log` & `slurmgen-3.5.0/example/slurm_output/test.log`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-================================== test - 05/03/24 06:42:15
+================================== test - 05/22/24 21:55:45
 ==================== PARAM
 JOB TAG      : test
 LOG FILE     : slurm_output/test.log
 SCRIPT FILE  : slurm_output/test.sh
 ==================== TIME
-DATE GEN     : 05/03/24 06:42:15
-DATE RUN     : 05/03/24 06:42:15
+DATE GEN     : 05/22/24 21:55:45
+DATE RUN     : 05/22/24 21:55:45
 ==================== SLURM
 JOB ID       : NOT SLURM
 JOB NAME     : NOT SLURM
 JOB NODE     : NOT SLURM
 ==================== ENV VAR
 ==================== RUN: version
 Python 3.10.12
@@ -19,8 +19,8 @@
     VARWORLD = Welcome to everyone
 exit script
 ==================== RUN: goodbye
 enter script
     ARGUMENT = goodbye world!
     VARWORLD = Welcome to everyone
 exit script
-================================== test - 05/03/24 06:42:15
+================================== test - 05/22/24 21:55:45
```

### Comparing `slurmgen-3.4.0/example/slurm_output/test.sh` & `slurmgen-3.5.0/example/slurm_output/test.sh`

 * *Files 10% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 
 echo "==================== PARAM"
 echo "JOB TAG      : test"
 echo "LOG FILE     : slurm_output/test.log"
 echo "SCRIPT FILE  : slurm_output/test.sh"
 
 echo "==================== TIME"
-echo "DATE GEN     : 05/03/24 06:42:15"
+echo "DATE GEN     : 05/22/24 21:55:45"
 echo "DATE RUN     : `date -u +"%D %H:%M:%S"`"
 
 echo "==================== SLURM"
 echo "JOB ID       : $SLURM_JOB_ID"
 echo "JOB NAME     : $SLURM_JOB_NAME"
 echo "JOB NODE     : $SLURM_JOB_NODELIST"
 
 echo "==================== ENV VAR"
 export PYTHONUNBUFFERED="1"
 export VARWORLD="Welcome to everyone"
 
 echo "==================== RUN: version"
-python3 "--version"
+python3 --version
 ret=$(( ret || $? ))
 
 echo "==================== RUN: hello"
-python3 "run_slurm.py" "hello" "hello world!"
+python3 run_slurm.py "hello" "hello world!"
 ret=$(( ret || $? ))
 
 echo "==================== RUN: goodbye"
-python3 "run_slurm.py" "goodbye" "goodbye world!"
+python3 run_slurm.py "goodbye" "goodbye world!"
 ret=$(( ret || $? ))
 
 echo "================================== test - `date -u +"%D %H:%M:%S"`"
 
 # ############### exit with status
 exit $ret
```

### Comparing `slurmgen-3.4.0/pyproject.toml` & `slurmgen-3.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slurmgen-3.4.0/run_release.sh` & `slurmgen-3.5.0/run_release.sh`

 * *Files identical despite different names*

### Comparing `slurmgen-3.4.0/slurmgen/gen.py` & `slurmgen-3.5.0/slurmgen/gen.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Module for creating a Slurm script.
 """
 
 __author__ = "Thomas Guillod"
 __copyright__ = "Thomas Guillod - Dartmouth College"
 __license__ = "BSD License"
 
-import sys
 import os.path
 import shutil
 import datetime
+from slurmgen.error import SlurmGenError
 
 
 def _write_title(fid, tag):
     """
     Write simulation header.
 
     Parameters
@@ -46,22 +46,19 @@
         Path of the log file created by during the Slurm job.
     pragmas : dict
         Dictionary with the pragmas controlling the Slurm job.
     """
 
     # check pragmas
     if "job-name" in pragmas:
-        print("error: job name is already set by the script", file=sys.stderr)
-        raise ValueError("invalid data")
+        raise SlurmGenError("error: job name is already set by the script")
     if "output" in pragmas:
-        print("error: job log is already set by the script", file=sys.stderr)
-        raise ValueError("invalid data")
+        raise SlurmGenError("error: job log is already set by the script")
     if "error" in pragmas:
-        print("error: job log is already set by the script", file=sys.stderr)
-        raise ValueError("invalid data")
+        raise SlurmGenError("error: job log is already set by the script")
 
     fid.write('#!/bin/bash\n')
     fid.write('\n')
     fid.write('# ############### define Slurm commands\n')
     fid.write('#SBATCH --job-name="%s"\n' % tag)
     fid.write('#SBATCH --output="%s"\n' % filename_log)
     for tag, val in pragmas.items():
@@ -110,29 +107,29 @@
     fid.write('echo "==================== SLURM"\n')
     fid.write('echo "JOB ID       : $SLURM_JOB_ID"\n')
     fid.write('echo "JOB NAME     : $SLURM_JOB_NAME"\n')
     fid.write('echo "JOB NODE     : $SLURM_JOB_NODELIST"\n')
     fid.write('\n')
 
 
-def _write_vars(fid, var):
+def _write_envs(fid, envs):
     """
     Handling of the folders and the environment variables.
 
     Parameters
     ----------
     fid : file
         File descriptor for the script.
-    vars : dict
+    envs : dict
         Dictionary of environment variable to be set and exported.
     """
 
-    if var:
+    if envs:
         fid.write('echo "==================== ENV VAR"\n')
-        for var, val in var.items():
+        for var, val in envs.items():
             if (var is not None) and (val is not None):
                 fid.write('export %s="%s"\n' % (var, val))
         fid.write('\n')
 
 
 def _write_commands(fid, commands):
     """
@@ -145,46 +142,40 @@
     commands : list
         List of commands to be executed by the job.
     """
 
     for tmp in commands:
         # extract data
         tag = tmp["tag"]
-        executable = tmp["executable"]
-        arguments = tmp["arguments"]
+        cmd = tmp["cmd"]
 
         # write command
         fid.write('echo "==================== RUN: %s"\n' % tag)
-        if arguments:
-            arg_all = ['"' + tmp + '"' for tmp in arguments]
-            arg_all = " ".join(arg_all)
-            fid.write('%s %s\n' % (executable, arg_all))
-        else:
-            fid.write('%s\n' % executable)
+        fid.write('%s\n' % cmd)
 
         # update status
         fid.write('ret=$(( ret || $? ))\n')
         fid.write('\n')
 
 
-def _generate_file(tag, filename_script, filename_log, pragmas, vars, commands):
+def _generate_file(tag, filename_script, filename_log, pragmas, envs, commands):
     """
     Generate and write a Slurm script or a Shell script.
 
     Parameters
     ----------
     tag : string
         Name of the job to be created.
     filename_script : string
         Path of the script controlling the simulation.
     filename_log : string
         Path of the log file created by during the Slurm job.
     pragmas : dict
         Dictionary with the pragmas controlling the Slurm job.
-    vars : dict
+    envs : dict
         Dictionary of environment variable to be set and exported.
     commands : list
         List of commands to be executed by the job.
     """
 
     # write the data
     with open(filename_script, "w") as fid:
@@ -194,44 +185,44 @@
         # write script header
         _write_title(fid, tag)
 
         # write summary of the variables
         _write_summary(fid, tag, filename_script, filename_log)
 
         # write environment variables
-        _write_vars(fid, vars)
+        _write_envs(fid, envs)
 
         # write the commands to be executed
         _write_commands(fid, commands)
 
         # end script footer
         _write_title(fid, tag)
 
         # end script footer
         fid.write('# ############### exit with status\n')
         fid.write('exit $ret\n')
         
 
-def run_data(tag, overwrite, folder, pragmas, vars, commands):
+def run_data(tag, overwrite, folder, pragmas, envs, commands):
     """
     Generate a Slurm script.
 
     Parameters
     ----------
     tag : string
         Name of the job to be created.
-    tag : bool
+    overwrite : bool
         Switch controlling if previous script and log should be replaced.
     folder : dict
         Name of the output folder for the script and log files.
         Name of the folders that should be deleted at the start of the job.
         Name of the folders that should be created at the start of the job.
     pragmas : dict
         Dictionary with the pragmas controlling the Slurm job.
-    vars : dict
+    vaenvsrs : dict
         Dictionary of environment variable to be set and exported.
     commands : list
         List of commands to be executed by the job.
     """
 
     # extract data
     folder_output = folder["folder_output"]
@@ -257,22 +248,19 @@
             os.makedirs(folder_output)
         except FileExistsError:
             pass
 
     # check that the output files are not existing
     print("info: check files")
     if os.path.isfile(filename_script):
-        print("error: Slurm file already exists", file=sys.stderr)
-        raise RuntimeError("invalid data")
+        raise SlurmGenError("error: Slurm file already exists")
     if os.path.isfile(filename_log):
-        print("error: log file already exists", file=sys.stderr)
-        raise RuntimeError("invalid data")
+        raise SlurmGenError("error: log file already exists")
     if not os.path.isdir(folder_output):
-        print("error: output folder does not exist", file=sys.stderr)
-        raise RuntimeError("invalid data")
+        raise SlurmGenError("error: output folder does not exist")
 
     # remove folders
     print("info: remove folders")
     for folder in folder_delete:
         try:
             shutil.rmtree(folder)
         except FileNotFoundError:
@@ -283,10 +271,10 @@
         try:
             os.makedirs(folder)
         except FileExistsError:
             pass
 
     # create the script
     print("info: generate Slurm file")
-    _generate_file(tag, filename_script, filename_log, pragmas, vars, commands)
+    _generate_file(tag, filename_script, filename_log, pragmas, envs, commands)
 
     return filename_script, filename_log
```

### Comparing `slurmgen-3.4.0/slurmgen/run.py` & `slurmgen-3.5.0/slurmgen/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Module for running a Slurm script.
 """
 
 __author__ = "Thomas Guillod"
 __copyright__ = "Thomas Guillod - Dartmouth College"
 __license__ = "BSD License"
 
-import sys
 import stat
 import os.path
 import subprocess
+from slurmgen.error import SlurmGenError
 
 
 def _run_cmd_raw(command, env):
     """
     Run a Slurm script.
 
     Parameters
@@ -27,23 +27,21 @@
     # run the command
     try:
         process = subprocess.run(
             command,
             env=env,
         )
     except OSError as ex:
-        print("error: command not found", file=sys.stderr)
-        raise ex
+        raise SlurmGenError("error: command error: %s" % str(ex))
 
     # check return code
     if process.returncode == 0:
         print("info: valid return code")
     else:
-        print("error: invalid return code", file=sys.stderr)
-        raise RuntimeError("invalid process")
+        raise SlurmGenError("error: invalid return code")
 
 
 def _run_cmd_log(command, filename_log, env):
     """
     Run a Slurm script.
 
     Parameters
@@ -62,23 +60,21 @@
             process = subprocess.run(
                 command,
                 env=env,
                 stderr=fid,
                 stdout=fid,
             )
     except OSError as ex:
-        print("error: command not found", file=sys.stderr)
-        raise ex
+        raise SlurmGenError("error: command error: %s" % str(ex))
 
     # check return code
     if process.returncode == 0:
         print("info: valid return code")
     else:
-        print("error: invalid return code", file=sys.stderr)
-        raise RuntimeError("invalid process")
+        raise SlurmGenError("error: invalid return code")
 
 
 def run_data(filename_script, filename_log, local, cluster):
     """
     Run a Slurm script.
 
     Parameters
```

### Comparing `slurmgen-3.4.0/slurmgen.egg-info/PKG-INFO` & `slurmgen-3.5.0/slurmgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmgen
-Version: 3.4.0
+Version: 3.5.0
 Summary: SlurmGen - Simple Slurm Manager
 Author-email: Thomas Guillod <guillod@otvam.ch>
 Maintainer-email: Thomas Guillod <guillod@otvam.ch>
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/otvam/slurmgen
 Project-URL: Repository, https://github.com/otvam/slurmgen
 Project-URL: Releases, https://github.com/otvam/slurmgen/releases
```

