# Comparing `tmp/pyerualjetwork-1.1.7.tar.gz` & `tmp/pyerualjetwork-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.1.7.tar", last modified: Thu May 23 02:38:13 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.1.8.tar", last modified: Thu May 23 07:56:17 2024, max compression
```

## Comparing `pyerualjetwork-1.1.7.tar` & `pyerualjetwork-1.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 02:38:13.800655 pyerualjetwork-1.1.7/
--rw-rw-rw-   0        0        0      276 2024-05-23 02:38:13.800655 pyerualjetwork-1.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 02:38:13.769407 pyerualjetwork-1.1.7/plan/
--rw-rw-rw-   0        0        0      315 2024-05-23 00:45:27.000000 pyerualjetwork-1.1.7/plan/__init__.py
--rw-rw-rw-   0        0        0    40264 2024-05-23 02:36:06.000000 pyerualjetwork-1.1.7/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-23 02:38:13.785017 pyerualjetwork-1.1.7/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      276 2024-05-23 02:38:13.000000 pyerualjetwork-1.1.7/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-23 02:38:13.000000 pyerualjetwork-1.1.7/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 02:38:13.000000 pyerualjetwork-1.1.7/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-23 02:38:13.000000 pyerualjetwork-1.1.7/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 02:38:13.800655 pyerualjetwork-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-23 02:37:08.000000 pyerualjetwork-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:56:17.818579 pyerualjetwork-1.1.8/
+-rw-rw-rw-   0        0        0      276 2024-05-23 07:56:17.818579 pyerualjetwork-1.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 07:56:17.802960 pyerualjetwork-1.1.8/plan/
+-rw-rw-rw-   0        0        0      315 2024-05-23 00:45:27.000000 pyerualjetwork-1.1.8/plan/__init__.py
+-rw-rw-rw-   0        0        0    40201 2024-05-23 07:55:26.000000 pyerualjetwork-1.1.8/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:56:17.818579 pyerualjetwork-1.1.8/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      276 2024-05-23 07:56:17.000000 pyerualjetwork-1.1.8/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-23 07:56:17.000000 pyerualjetwork-1.1.8/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 07:56:17.000000 pyerualjetwork-1.1.8/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-23 07:56:17.000000 pyerualjetwork-1.1.8/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 07:56:17.818579 pyerualjetwork-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-23 07:55:48.000000 pyerualjetwork-1.1.8/setup.py
```

### Comparing `pyerualjetwork-1.1.7/plan/plan.py` & `pyerualjetwork-1.1.8/plan/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,14 @@
     
     W = WeightIdentification(len(Layers) - 1,ClassCount,Neurons,InputSize)
     Divides = SynapticDividing(ClassCount,W)
     TrainedWs = [1] * len(W)
     print(Fore.GREEN + "Train Started with 0 ERROR" + Style.RESET_ALL,)
     TrainPredictions = [1] * len(Labels)
     true = 0
-    Inputs, Labels = AutoBalancer(Inputs, Labels, ClassCount)
     StartTime = time.time()
     for index, inp in enumerate(Inputs):
         UniStartTime = time.time()
         inp = np.array(inp)
         inp = inp.ravel()
         
         if InputSize != len(inp):
```

