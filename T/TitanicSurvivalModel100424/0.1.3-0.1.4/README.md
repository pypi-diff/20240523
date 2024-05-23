# Comparing `tmp/titanicsurvivalmodel100424-0.1.3.tar.gz` & `tmp/titanicsurvivalmodel100424-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titanicsurvivalmodel100424-0.1.3.tar", last modified: Mon May 20 06:44:04 2024, max compression
+gzip compressed data, was "titanicsurvivalmodel100424-0.1.4.tar", last modified: Thu May 23 18:17:14 2024, max compression
```

## Comparing `titanicsurvivalmodel100424-0.1.3.tar` & `titanicsurvivalmodel100424-0.1.4.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 06:44:04.486437 titanicsurvivalmodel100424-0.1.3/
--rw-r--r--   0 ongzhicong   (501) staff       (20)      443 2024-05-20 06:43:12.000000 titanicsurvivalmodel100424-0.1.3/MANIFEST.in
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-20 06:44:04.485464 titanicsurvivalmodel100424-0.1.3/PKG-INFO
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 06:44:04.484759 titanicsurvivalmodel100424-0.1.3/TitanicSurvivalModel100424.egg-info/
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-20 06:44:04.000000 titanicsurvivalmodel100424-0.1.3/TitanicSurvivalModel100424.egg-info/PKG-INFO
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1070 2024-05-20 06:44:04.000000 titanicsurvivalmodel100424-0.1.3/TitanicSurvivalModel100424.egg-info/SOURCES.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)        1 2024-05-20 06:44:04.000000 titanicsurvivalmodel100424-0.1.3/TitanicSurvivalModel100424.egg-info/dependency_links.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)      188 2024-05-20 06:44:04.000000 titanicsurvivalmodel100424-0.1.3/TitanicSurvivalModel100424.egg-info/requires.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)       21 2024-05-20 06:44:04.000000 titanicsurvivalmodel100424-0.1.3/TitanicSurvivalModel100424.egg-info/top_level.txt
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 06:44:04.477789 titanicsurvivalmodel100424-0.1.3/classification_model/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        6 2024-05-20 06:39:58.000000 titanicsurvivalmodel100424-0.1.3/classification_model/VERSION
--rw-r--r--   0 ongzhicong   (501) staff       (20)      862 2024-05-04 09:04:59.000000 titanicsurvivalmodel100424-0.1.3/classification_model/__init__.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 06:44:04.478255 titanicsurvivalmodel100424-0.1.3/classification_model/config/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:23.000000 titanicsurvivalmodel100424-0.1.3/classification_model/config/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     2129 2024-05-20 00:42:53.000000 titanicsurvivalmodel100424-0.1.3/classification_model/config/core.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)      899 2024-05-17 08:13:51.000000 titanicsurvivalmodel100424-0.1.3/classification_model/config.yml
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 06:44:04.481118 titanicsurvivalmodel100424-0.1.3/classification_model/datasets/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:51.000000 titanicsurvivalmodel100424-0.1.3/classification_model/datasets/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)    61194 2024-05-04 09:08:51.000000 titanicsurvivalmodel100424-0.1.3/classification_model/datasets/titanic_train.csv
--rw-r--r--   0 ongzhicong   (501) staff       (20)     2434 2024-05-17 06:12:30.000000 titanicsurvivalmodel100424-0.1.3/classification_model/pipeline.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1058 2024-05-18 07:00:50.000000 titanicsurvivalmodel100424-0.1.3/classification_model/predict.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 06:44:04.483145 titanicsurvivalmodel100424-0.1.3/classification_model/processing/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:58.000000 titanicsurvivalmodel100424-0.1.3/classification_model/processing/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1751 2024-05-20 06:30:05.000000 titanicsurvivalmodel100424-0.1.3/classification_model/processing/data_manager.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     3575 2024-05-17 06:26:00.000000 titanicsurvivalmodel100424-0.1.3/classification_model/processing/features.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1763 2024-05-18 07:29:10.000000 titanicsurvivalmodel100424-0.1.3/classification_model/processing/validation.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)      831 2024-05-17 06:24:46.000000 titanicsurvivalmodel100424-0.1.3/classification_model/train_pipeline.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 06:44:04.483627 titanicsurvivalmodel100424-0.1.3/classification_model/trained_models/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:09:07.000000 titanicsurvivalmodel100424-0.1.3/classification_model/trained_models/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     4110 2024-05-20 06:42:06.000000 titanicsurvivalmodel100424-0.1.3/classification_model/trained_models/classification_model_output_v0.1.3.pkl
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1914 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.3/pyproject.toml
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 06:44:04.474591 titanicsurvivalmodel100424-0.1.3/requirements/
--rw-r--r--   0 ongzhicong   (501) staff       (20)      225 2024-05-17 09:24:00.000000 titanicsurvivalmodel100424-0.1.3/requirements/requirements.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)       65 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.3/requirements/test_requirements.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)       38 2024-05-20 06:44:04.486586 titanicsurvivalmodel100424-0.1.3/setup.cfg
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1997 2024-05-20 01:46:16.000000 titanicsurvivalmodel100424-0.1.3/setup.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-20 06:44:04.484417 titanicsurvivalmodel100424-0.1.3/tests/
--rw-r--r--   0 ongzhicong   (501) staff       (20)      680 2024-05-14 08:58:22.000000 titanicsurvivalmodel100424-0.1.3/tests/test_features.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)      855 2024-05-14 08:58:29.000000 titanicsurvivalmodel100424-0.1.3/tests/test_prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-23 18:17:14.000000 titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-23 18:17:14.000000 titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:17:14.000000 titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-23 18:17:14.000000 titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 18:17:14.000000 titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.136476 titanicsurvivalmodel100424-0.1.4/classification_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/classification_model/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/config/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/classification_model/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/classification_model/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/processing/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/processing/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/processing/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/train_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/classification_model/trained_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/trained_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/trained_models/classification_model_output_v0.1.1.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.136476 titanicsurvivalmodel100424-0.1.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/requirements/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/tests/test_prediction.py
```

### Comparing `titanicsurvivalmodel100424-0.1.3/PKG-INFO` & `titanicsurvivalmodel100424-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanicSurvivalModel100424
-Version: 0.1.3
+Version: 0.1.4
 Summary: sample Classification model package.
 Home-page: https://github.com/zong006/model_packaging
 Author: sample_author
 Author-email: sample_email@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `titanicsurvivalmodel100424-0.1.3/TitanicSurvivalModel100424.egg-info/PKG-INFO` & `titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanicSurvivalModel100424
-Version: 0.1.3
+Version: 0.1.4
 Summary: sample Classification model package.
 Home-page: https://github.com/zong006/model_packaging
 Author: sample_author
 Author-email: sample_email@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `titanicsurvivalmodel100424-0.1.3/TitanicSurvivalModel100424.egg-info/SOURCES.txt` & `titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 classification_model/config.yml
 classification_model/pipeline.py
 classification_model/predict.py
 classification_model/train_pipeline.py
 classification_model/config/__init__.py
 classification_model/config/core.py
 classification_model/datasets/__init__.py
-classification_model/datasets/titanic_train.csv
 classification_model/processing/__init__.py
 classification_model/processing/data_manager.py
 classification_model/processing/features.py
 classification_model/processing/validation.py
 classification_model/trained_models/__init__.py
-classification_model/trained_models/classification_model_output_v0.1.3.pkl
+classification_model/trained_models/classification_model_output_v0.1.1.pkl
 tests/test_features.py
 tests/test_prediction.py
```

### Comparing `titanicsurvivalmodel100424-0.1.3/classification_model/__init__.py` & `titanicsurvivalmodel100424-0.1.4/classification_model/__init__.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.3/classification_model/config/core.py` & `titanicsurvivalmodel100424-0.1.4/classification_model/config/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import List, Optional
 
 from pydantic import BaseModel
 from strictyaml import YAML, load
 
-script_path = Path(__file__).resolve().parent 
+script_path = Path(__file__).resolve().parent
 
 PACKAGE_ROOT = script_path.parent
 ROOT = PACKAGE_ROOT.parent
 CONFIG_FILE_PATH = PACKAGE_ROOT / "config.yml"
 DATASET_DIR = PACKAGE_ROOT / "datasets"
 TRAINED_MODEL_DIR = PACKAGE_ROOT / "trained_models"
```

### Comparing `titanicsurvivalmodel100424-0.1.3/classification_model/config.yml` & `titanicsurvivalmodel100424-0.1.4/classification_model/config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Package Overview
 package_name: classification_model
 
 # Data Files
-training_data_file: titanic_train.csv
+training_data_file: train.csv
 
 pipeline_name: classification_model
 pipeline_save_file: classification_model_output_v
 
 # Variables
 target: Survived
```

### Comparing `titanicsurvivalmodel100424-0.1.3/classification_model/pipeline.py` & `titanicsurvivalmodel100424-0.1.4/classification_model/pipeline.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.3/classification_model/predict.py` & `titanicsurvivalmodel100424-0.1.4/classification_model/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import typing as t
+
+import numpy as np
 import pandas as pd
 
 from classification_model import __version__ as _version
 from classification_model.config.core import config
 from classification_model.processing.data_manager import load_pipeline
 from classification_model.processing.validation import validate_inputs
```

### Comparing `titanicsurvivalmodel100424-0.1.3/classification_model/processing/data_manager.py` & `titanicsurvivalmodel100424-0.1.4/classification_model/processing/data_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import typing as t
+import re
 from pathlib import Path
+from typing import Union
 
 import joblib
 import pandas as pd
+import numpy as np
 from sklearn.pipeline import Pipeline
 
 from classification_model import __version__ as _version
 from classification_model.config.core import DATASET_DIR, TRAINED_MODEL_DIR, config
 
 
 def load_dataset(*, file_name: str) -> pd.DataFrame:
@@ -49,8 +52,7 @@
     mapping between the package version and the model
     version to be imported and used by other applications.
     """
     do_not_delete = files_to_keep + ["__init__.py"]
     for model_file in TRAINED_MODEL_DIR.iterdir():
         if model_file.name not in do_not_delete:
             model_file.unlink()
-
```

### Comparing `titanicsurvivalmodel100424-0.1.3/classification_model/processing/features.py` & `titanicsurvivalmodel100424-0.1.4/classification_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.3/classification_model/processing/validation.py` & `titanicsurvivalmodel100424-0.1.4/classification_model/processing/validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     except ValidationError as error:
         errors = error.json()
 
     return validated_data, errors
 
 
 class PassengerDataInputSchema(BaseModel):
-    PassengerId: Optional[int]
     Age: Optional[float]
     Fare: Optional[float]
     Pclass: Optional[int]
     Sex: Optional[str]
     Name: Optional[str]
     SibSp: Optional[int]
     Parch: Optional[int]
```

### Comparing `titanicsurvivalmodel100424-0.1.3/classification_model/train_pipeline.py` & `titanicsurvivalmodel100424-0.1.4/classification_model/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.3/classification_model/trained_models/classification_model_output_v0.1.3.pkl` & `titanicsurvivalmodel100424-0.1.4/classification_model/trained_models/classification_model_output_v0.1.1.pkl`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.3/pyproject.toml` & `titanicsurvivalmodel100424-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.3/setup.py` & `titanicsurvivalmodel100424-0.1.4/setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,8 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
-)
+)
```

### Comparing `titanicsurvivalmodel100424-0.1.3/tests/test_features.py` & `titanicsurvivalmodel100424-0.1.4/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.3/tests/test_prediction.py` & `titanicsurvivalmodel100424-0.1.4/tests/test_prediction.py`

 * *Files identical despite different names*

