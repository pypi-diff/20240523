# Comparing `tmp/pyerualjetwork-1.1.6.tar.gz` & `tmp/pyerualjetwork-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.1.6.tar", last modified: Thu May 23 00:46:13 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.1.7.tar", last modified: Thu May 23 02:38:13 2024, max compression
```

## Comparing `pyerualjetwork-1.1.6.tar` & `pyerualjetwork-1.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 00:46:13.330536 pyerualjetwork-1.1.6/
--rw-rw-rw-   0        0        0      276 2024-05-23 00:46:13.330536 pyerualjetwork-1.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 00:46:13.314911 pyerualjetwork-1.1.6/plan/
--rw-rw-rw-   0        0        0      315 2024-05-23 00:45:27.000000 pyerualjetwork-1.1.6/plan/__init__.py
--rw-rw-rw-   0        0        0    40246 2024-05-23 00:44:58.000000 pyerualjetwork-1.1.6/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-23 00:46:13.330536 pyerualjetwork-1.1.6/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      276 2024-05-23 00:46:12.000000 pyerualjetwork-1.1.6/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-23 00:46:13.000000 pyerualjetwork-1.1.6/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 00:46:12.000000 pyerualjetwork-1.1.6/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-23 00:46:12.000000 pyerualjetwork-1.1.6/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 00:46:13.330536 pyerualjetwork-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-23 00:46:02.000000 pyerualjetwork-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:38:13.800655 pyerualjetwork-1.1.7/
+-rw-rw-rw-   0        0        0      276 2024-05-23 02:38:13.800655 pyerualjetwork-1.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 02:38:13.769407 pyerualjetwork-1.1.7/plan/
+-rw-rw-rw-   0        0        0      315 2024-05-23 00:45:27.000000 pyerualjetwork-1.1.7/plan/__init__.py
+-rw-rw-rw-   0        0        0    40264 2024-05-23 02:36:06.000000 pyerualjetwork-1.1.7/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:38:13.785017 pyerualjetwork-1.1.7/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      276 2024-05-23 02:38:13.000000 pyerualjetwork-1.1.7/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-23 02:38:13.000000 pyerualjetwork-1.1.7/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 02:38:13.000000 pyerualjetwork-1.1.7/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-23 02:38:13.000000 pyerualjetwork-1.1.7/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 02:38:13.800655 pyerualjetwork-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-23 02:37:08.000000 pyerualjetwork-1.1.7/setup.py
```

### Comparing `pyerualjetwork-1.1.6/plan/plan.py` & `pyerualjetwork-1.1.7/plan/plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1041,14 +1041,14 @@
             else:
                 SelectedIndices = ClassIndices[i]
             BalancedIndices.extend(SelectedIndices)
         
         BalancedInputs = [TrainInputs[idx] for idx in BalancedIndices]
         BalancedLabels = [TrainLabels[idx] for idx in BalancedIndices]
         
-        print(Fore.GREEN + "All Training Data Succesfully Balanced from: " + str(len(TrainInputs)) + " to: " + str(len(BalancedInputs)) + ". from: AutoBalancer ")
+        print(Fore.GREEN + "All Training Data Succesfully Balanced from: " + str(len(TrainInputs)) + " to: " + str(len(BalancedInputs)) + ". from: AutoBalancer " + Style.RESET_ALL)
         time.sleep(1.5)
    except:
         print(Fore.RED + "ERROR: Inputs and labels must be same length check parameters" + infoAutoBalancer)
         return 'e'
         
    return BalancedInputs, BalancedLabels
```

