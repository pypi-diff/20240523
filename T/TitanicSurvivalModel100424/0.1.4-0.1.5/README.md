# Comparing `tmp/titanicsurvivalmodel100424-0.1.4.tar.gz` & `tmp/titanicsurvivalmodel100424-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titanicsurvivalmodel100424-0.1.4.tar", last modified: Thu May 23 18:17:14 2024, max compression
+gzip compressed data, was "titanicsurvivalmodel100424-0.1.5.tar", last modified: Thu May 23 18:48:59 2024, max compression
```

## Comparing `titanicsurvivalmodel100424-0.1.4.tar` & `titanicsurvivalmodel100424-0.1.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-23 18:17:14.000000 titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-23 18:17:14.000000 titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:17:14.000000 titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-23 18:17:14.000000 titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 18:17:14.000000 titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.136476 titanicsurvivalmodel100424-0.1.4/classification_model/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/classification_model/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/config/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/classification_model/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/classification_model/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/processing/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/processing/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/processing/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/train_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/classification_model/trained_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/trained_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/classification_model/trained_models/classification_model_output_v0.1.1.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.136476 titanicsurvivalmodel100424-0.1.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/requirements/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:17:14.140476 titanicsurvivalmodel100424-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-23 18:17:01.000000 titanicsurvivalmodel100424-0.1.4/tests/test_prediction.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.121671 titanicsurvivalmodel100424-0.1.5/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      443 2024-05-20 06:43:12.000000 titanicsurvivalmodel100424-0.1.5/MANIFEST.in
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-23 18:48:59.120746 titanicsurvivalmodel100424-0.1.5/PKG-INFO
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.119709 titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-23 18:48:59.000000 titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/PKG-INFO
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1022 2024-05-23 18:48:59.000000 titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/SOURCES.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        1 2024-05-23 18:48:59.000000 titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/dependency_links.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      188 2024-05-23 18:48:59.000000 titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/requires.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)       21 2024-05-23 18:48:59.000000 titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/top_level.txt
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.113671 titanicsurvivalmodel100424-0.1.5/classification_model/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        6 2024-05-23 18:45:26.000000 titanicsurvivalmodel100424-0.1.5/classification_model/VERSION
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      862 2024-05-04 09:04:59.000000 titanicsurvivalmodel100424-0.1.5/classification_model/__init__.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.114469 titanicsurvivalmodel100424-0.1.5/classification_model/config/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:23.000000 titanicsurvivalmodel100424-0.1.5/classification_model/config/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     2129 2024-05-20 00:42:53.000000 titanicsurvivalmodel100424-0.1.5/classification_model/config/core.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      891 2024-05-23 10:57:47.000000 titanicsurvivalmodel100424-0.1.5/classification_model/config.yml
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.115014 titanicsurvivalmodel100424-0.1.5/classification_model/datasets/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:51.000000 titanicsurvivalmodel100424-0.1.5/classification_model/datasets/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     2434 2024-05-17 06:12:30.000000 titanicsurvivalmodel100424-0.1.5/classification_model/pipeline.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1058 2024-05-18 07:00:50.000000 titanicsurvivalmodel100424-0.1.5/classification_model/predict.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.116620 titanicsurvivalmodel100424-0.1.5/classification_model/processing/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:58.000000 titanicsurvivalmodel100424-0.1.5/classification_model/processing/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1751 2024-05-20 06:30:05.000000 titanicsurvivalmodel100424-0.1.5/classification_model/processing/data_manager.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     3575 2024-05-17 06:26:00.000000 titanicsurvivalmodel100424-0.1.5/classification_model/processing/features.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1763 2024-05-18 07:29:10.000000 titanicsurvivalmodel100424-0.1.5/classification_model/processing/validation.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      831 2024-05-17 06:24:46.000000 titanicsurvivalmodel100424-0.1.5/classification_model/train_pipeline.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.117382 titanicsurvivalmodel100424-0.1.5/classification_model/trained_models/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:09:07.000000 titanicsurvivalmodel100424-0.1.5/classification_model/trained_models/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     4110 2024-05-23 18:47:07.000000 titanicsurvivalmodel100424-0.1.5/classification_model/trained_models/classification_model_output_v0.1.5.pkl
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1914 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.5/pyproject.toml
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.107426 titanicsurvivalmodel100424-0.1.5/requirements/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      225 2024-05-17 09:24:00.000000 titanicsurvivalmodel100424-0.1.5/requirements/requirements.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)       65 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.5/requirements/test_requirements.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)       38 2024-05-23 18:48:59.122265 titanicsurvivalmodel100424-0.1.5/setup.cfg
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1996 2024-05-23 17:39:04.000000 titanicsurvivalmodel100424-0.1.5/setup.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-23 18:48:59.118325 titanicsurvivalmodel100424-0.1.5/tests/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      680 2024-05-14 08:58:22.000000 titanicsurvivalmodel100424-0.1.5/tests/test_features.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      855 2024-05-14 08:58:29.000000 titanicsurvivalmodel100424-0.1.5/tests/test_prediction.py
```

### Comparing `titanicsurvivalmodel100424-0.1.4/PKG-INFO` & `titanicsurvivalmodel100424-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanicSurvivalModel100424
-Version: 0.1.4
+Version: 0.1.5
 Summary: sample Classification model package.
 Home-page: https://github.com/zong006/model_packaging
 Author: sample_author
 Author-email: sample_email@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/PKG-INFO` & `titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanicSurvivalModel100424
-Version: 0.1.4
+Version: 0.1.5
 Summary: sample Classification model package.
 Home-page: https://github.com/zong006/model_packaging
 Author: sample_author
 Author-email: sample_email@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `titanicsurvivalmodel100424-0.1.4/TitanicSurvivalModel100424.egg-info/SOURCES.txt` & `titanicsurvivalmodel100424-0.1.5/TitanicSurvivalModel100424.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 classification_model/config/core.py
 classification_model/datasets/__init__.py
 classification_model/processing/__init__.py
 classification_model/processing/data_manager.py
 classification_model/processing/features.py
 classification_model/processing/validation.py
 classification_model/trained_models/__init__.py
-classification_model/trained_models/classification_model_output_v0.1.1.pkl
+classification_model/trained_models/classification_model_output_v0.1.5.pkl
 tests/test_features.py
 tests/test_prediction.py
```

### Comparing `titanicsurvivalmodel100424-0.1.4/classification_model/__init__.py` & `titanicsurvivalmodel100424-0.1.5/classification_model/__init__.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.4/classification_model/config/core.py` & `titanicsurvivalmodel100424-0.1.5/classification_model/config/core.py`

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

### Comparing `titanicsurvivalmodel100424-0.1.4/classification_model/config.yml` & `titanicsurvivalmodel100424-0.1.5/classification_model/config.yml`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.4/classification_model/pipeline.py` & `titanicsurvivalmodel100424-0.1.5/classification_model/pipeline.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.4/classification_model/predict.py` & `titanicsurvivalmodel100424-0.1.5/classification_model/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import typing as t
-
-import numpy as np
 import pandas as pd
 
 from classification_model import __version__ as _version
 from classification_model.config.core import config
 from classification_model.processing.data_manager import load_pipeline
 from classification_model.processing.validation import validate_inputs
```

### Comparing `titanicsurvivalmodel100424-0.1.4/classification_model/processing/data_manager.py` & `titanicsurvivalmodel100424-0.1.5/classification_model/processing/data_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import typing as t
-import re
 from pathlib import Path
-from typing import Union
 
 import joblib
 import pandas as pd
-import numpy as np
 from sklearn.pipeline import Pipeline
 
 from classification_model import __version__ as _version
 from classification_model.config.core import DATASET_DIR, TRAINED_MODEL_DIR, config
 
 
 def load_dataset(*, file_name: str) -> pd.DataFrame:
@@ -52,7 +49,8 @@
     mapping between the package version and the model
     version to be imported and used by other applications.
     """
     do_not_delete = files_to_keep + ["__init__.py"]
     for model_file in TRAINED_MODEL_DIR.iterdir():
         if model_file.name not in do_not_delete:
             model_file.unlink()
+
```

### Comparing `titanicsurvivalmodel100424-0.1.4/classification_model/processing/features.py` & `titanicsurvivalmodel100424-0.1.5/classification_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.4/classification_model/processing/validation.py` & `titanicsurvivalmodel100424-0.1.5/classification_model/processing/validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     except ValidationError as error:
         errors = error.json()
 
     return validated_data, errors
 
 
 class PassengerDataInputSchema(BaseModel):
+    PassengerId: Optional[int]
     Age: Optional[float]
     Fare: Optional[float]
     Pclass: Optional[int]
     Sex: Optional[str]
     Name: Optional[str]
     SibSp: Optional[int]
     Parch: Optional[int]
```

### Comparing `titanicsurvivalmodel100424-0.1.4/classification_model/train_pipeline.py` & `titanicsurvivalmodel100424-0.1.5/classification_model/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.4/classification_model/trained_models/classification_model_output_v0.1.1.pkl` & `titanicsurvivalmodel100424-0.1.5/classification_model/trained_models/classification_model_output_v0.1.5.pkl`

 * *Files 3% similar despite different names*

```diff
@@ -201,38 +201,38 @@
 00000c80: a5ca 07e5 9a3d f23f 080c 2442 eb43 ea3f  .....=.?..$B.C.?
 00000c90: d9c0 33be cf0c 4940 9e59 b663 5081 d93f  ..3...I@.Y.cP..?
 00000ca0: 3dce 3106 abe3 da3f cc02 c2ea 22d2 ce3f  =.1....?...."..?
 00000cb0: c105 2e70 810b cc3f a54d d4bd 93a6 d83f  ...p...?.M.....?
 00000cc0: 1dec 1e6e 628a dc3f e024 1cda 294e d23f  ...nb..?.$..)N.?
 00000cd0: 2cec ad56 aa3c d63f 96b5 9694 887a df3f  ,..V.<.?.....z.?
 00000ce0: e062 a4af eea3 d93f e82e 1492 9176 de3f  .b.....?.....v.?
-00000cf0: 956f 0100 0000 0000 008c 105f 736b 6c65  .o........._skle
+00000cf0: 9575 0100 0000 0000 008c 105f 736b 6c65  .u........._skle
 00000d00: 6172 6e5f 7665 7273 696f 6e94 8c05 312e  arn_version...1.
-00000d10: 342e 3294 7562 8694 8c05 4c6f 6769 7494  4.2.ub....Logit.
+00000d10: 352e 3094 7562 8694 8c05 4c6f 6769 7494  5.0.ub....Logit.
 00000d20: 8c1e 736b 6c65 6172 6e2e 6c69 6e65 6172  ..sklearn.linear
 00000d30: 5f6d 6f64 656c 2e5f 6c6f 6769 7374 6963  _model._logistic
 00000d40: 948c 124c 6f67 6973 7469 6352 6567 7265  ...LogisticRegre
 00000d50: 7373 696f 6e94 9394 2981 947d 9428 8c07  ssion...)..}.(..
 00000d60: 7065 6e61 6c74 7994 8c02 6c32 948c 0464  penalty...l2...d
 00000d70: 7561 6c94 8968 7d47 3f1a 36e2 eb1c 432d  ual..h}G?.6...C-
 00000d80: 6886 473f f000 0000 0000 008c 0d66 6974  h.G?.........fit
 00000d90: 5f69 6e74 6572 6365 7074 9488 8c11 696e  _intercept....in
 00000da0: 7465 7263 6570 745f 7363 616c 696e 6794  tercept_scaling.
 00000db0: 4b01 8c0c 636c 6173 735f 7765 6967 6874  K...class_weight
 00000dc0: 944e 8c0c 7261 6e64 6f6d 5f73 7461 7465  .N..random_state
 00000dd0: 944b 008c 0673 6f6c 7665 7294 8c05 6c62  .K...solver...lb
 00000de0: 6667 7394 8c08 6d61 785f 6974 6572 944b  fgs...max_iter.K
 00000df0: 648c 0b6d 756c 7469 5f63 6c61 7373 948c  d..multi_class..
-00000e00: 0461 7574 6f94 8c07 7665 7262 6f73 6594  .auto...verbose.
-00000e10: 4b00 8c0a 7761 726d 5f73 7461 7274 9489  K...warm_start..
-00000e20: 8c06 6e5f 6a6f 6273 944e 8c08 6c31 5f72  ..n_jobs.N..l1_r
-00000e30: 6174 696f 944e 6852 4b10 8c08 636c 6173  atio.NhRK...clas
-00000e40: 7365 735f 9468 b129 8194 7d94 2868 b468  ses_.h.)..}.(h.h
-00000e50: b768 b84b 0285 9468 ba68 8668 bb68 cb68  .h.K...h.h.h.h.h
-00000e60: c388 68c4 4b10 7562 07ff ffff ffff ffff  ..h.K.ub........
+00000e00: 0a64 6570 7265 6361 7465 6494 8c07 7665  .deprecated...ve
+00000e10: 7262 6f73 6594 4b00 8c0a 7761 726d 5f73  rbose.K...warm_s
+00000e20: 7461 7274 9489 8c06 6e5f 6a6f 6273 944e  tart....n_jobs.N
+00000e30: 8c08 6c31 5f72 6174 696f 944e 6852 4b10  ..l1_ratio.NhRK.
+00000e40: 8c08 636c 6173 7365 735f 9468 b129 8194  ..classes_.h.)..
+00000e50: 7d94 2868 b468 b768 b84b 0285 9468 ba68  }.(h.h.h.K...h.h
+00000e60: 8668 bb68 cb68 c388 68c4 4b10 7562 01ff  .h.h.h..h.K.ub..
 00000e70: 0000 0000 0000 0000 0100 0000 0000 0000  ................
 00000e80: 954f 0000 0000 0000 008c 076e 5f69 7465  .O.........n_ite
 00000e90: 725f 9468 b129 8194 7d94 2868 b468 b768  r_.h.)..}.(h.h.h
 00000ea0: b84b 0185 9468 ba68 8668 bb68 bd8c 0269  .K...h.h.h.h...i
 00000eb0: 3494 8988 8794 5294 284b 0368 cc4e 4e4e  4.....R.(K.h.NNN
 00000ec0: 4aff ffff ff4a ffff ffff 4b00 7494 6268  J....J....K.t.bh
 00000ed0: c388 68c4 4b10 7562 07ff ffff ffff ffff  ..h.K.ub........
```

### Comparing `titanicsurvivalmodel100424-0.1.4/pyproject.toml` & `titanicsurvivalmodel100424-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.4/setup.py` & `titanicsurvivalmodel100424-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.4/tests/test_features.py` & `titanicsurvivalmodel100424-0.1.5/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `titanicsurvivalmodel100424-0.1.4/tests/test_prediction.py` & `titanicsurvivalmodel100424-0.1.5/tests/test_prediction.py`

 * *Files identical despite different names*

