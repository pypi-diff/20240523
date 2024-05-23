# Comparing `tmp/dkist_quality-1.0.1.tar.gz` & `tmp/dkist_quality-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_quality-1.0.1.tar", last modified: Thu Apr 25 19:41:27 2024, max compression
+gzip compressed data, was "dkist_quality-1.0.2.tar", last modified: Thu May 23 16:11:43 2024, max compression
```

## Comparing `dkist_quality-1.0.1.tar` & `dkist_quality-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     3104 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      468 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2155 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1229 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2513 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/dkist_quality/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/dkist_quality/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    91676 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/fonts/Oswald-Bold.ttf
--rw-rw-rw-   0 root         (0) root         (0)    91400 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/fonts/Oswald-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      871 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)    34162 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/report.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/dkist_quality/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11169 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/tests/test_report.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/dkist_quality.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2155 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      668 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     2037 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1214 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     3104 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      468 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2513 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 16:11:43.825722 dkist_quality-1.0.2/dkist_quality/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/dkist_quality/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    91676 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/fonts/Oswald-Bold.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    91400 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/fonts/Oswald-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      871 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)    37316 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/report.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/dkist_quality/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11866 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/tests/test_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/dkist_quality/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/dkist_quality.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      668 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-23 16:11:43.000000 dkist_quality-1.0.2/dkist_quality.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2032 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-23 16:11:43.829722 dkist_quality-1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2024-05-23 16:11:31.000000 dkist_quality-1.0.2/tox.ini
```

### Comparing `dkist_quality-1.0.1/.gitignore` & `dkist_quality-1.0.2/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
-.tox/
+.tox*/
 .nox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *.cover
@@ -154,8 +154,8 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+.idea/
```

### Comparing `dkist_quality-1.0.1/.pre-commit-config.yaml` & `dkist_quality-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.1/PKG-INFO` & `dkist_quality-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dkist-quality
-Version: 1.0.1
+Version: 1.0.2
 Summary: DKIST library for generating quality report pdf
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist-quality
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Requires-Dist: reportlab>=4.0.4
-Requires-Dist: matplotlib<3.8,>=3.6
+Requires-Dist: matplotlib>=3.6
 Requires-Dist: seaborn>=0.13.0
 Requires-Dist: dacite>=1.8.0
 Requires-Dist: natsort>=8.0.0
 Requires-Dist: pydantic<2,>=1.10.4
 Provides-Extra: test
 Requires-Dist: tox>=4; extra == "test"
 Requires-Dist: pytest; extra == "test"
```

### Comparing `dkist_quality-1.0.1/README.rst` & `dkist_quality-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.1/bitbucket-pipelines.yml` & `dkist_quality-1.0.2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.1/dkist_quality/fonts/Oswald-Bold.ttf` & `dkist_quality-1.0.2/dkist_quality/fonts/Oswald-Bold.ttf`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.1/dkist_quality/fonts/Oswald-Regular.ttf` & `dkist_quality-1.0.2/dkist_quality/fonts/Oswald-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.1/dkist_quality/json_encoder.py` & `dkist_quality-1.0.2/dkist_quality/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.1/dkist_quality/report.py` & `dkist_quality-1.0.2/dkist_quality/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """
 Report Formatting
 """
 import os
 from datetime import datetime
+from importlib.metadata import version
 from io import BytesIO
 from typing import Any
 
 import dacite
 import matplotlib.dates as mdates
 import numpy as np
 import pandas
 import pkg_resources
 import seaborn as sns
 from cycler import cycler
 from matplotlib import pyplot as plt
 from matplotlib import rc
 from matplotlib import rcdefaults
+from matplotlib import rcParams
+from matplotlib.ticker import _Edge_integer  # noqa
 from matplotlib.ticker import MaxNLocator
+from matplotlib.ticker import scale_range  # noqa
 from natsort import natsorted
+from pkg_resources import packaging  # noqa
 from pydantic import Field
 from pydantic.dataclasses import dataclass as validating_dataclass
 from reportlab.lib import colors
 from reportlab.lib.styles import ParagraphStyle
 from reportlab.pdfbase import pdfmetrics
 from reportlab.pdfbase.ttfonts import TTFont
 from reportlab.platypus import Flowable
@@ -32,14 +37,89 @@
 from reportlab.platypus import SimpleDocTemplate
 from reportlab.platypus import Spacer
 from reportlab.platypus import Table
 from reportlab.platypus import TableStyle
 from reportlab.platypus.tableofcontents import TableOfContents
 
 
+def nso_raw_ticks(self, vmin, vmax):
+    """
+    This overrides the `MaxNLocator._raw_ticks` method in matplotlib, which has a bug.
+    The bug was introduced in matplotlib 3.8.0 and still exists as of 3.9.0.
+    Bug details:   https://github.com/matplotlib/matplotlib/issues/27603
+    """
+    if self._nbins == "auto":
+        if self.axis is not None:
+            nbins = np.clip(self.axis.get_tick_space(), max(1, self._min_n_ticks - 1), 9)
+        else:
+            nbins = 9
+    else:
+        nbins = self._nbins
+
+    scale, offset = scale_range(vmin, vmax, nbins)
+    _vmin = vmin - offset
+    _vmax = vmax - offset
+    steps = self._extended_steps * scale
+    if self._integer:
+        # For steps > 1, keep only integer values.
+        igood = (steps < 1) | (np.abs(steps - np.round(steps)) < 0.001)
+        steps = steps[igood]
+
+    raw_step = (_vmax - _vmin) / nbins
+    large_steps = steps >= raw_step
+
+    # This is the source of the matplotlib error
+    # If all large_steps are False, then
+    #  `np.nonzero(large_steps)[0][0]` results in `IndexError: index 0 is out of bounds for axis 0 with size 0`
+    if rcParams["axes.autolimit_mode"] == "round_numbers":
+        # Classic round_numbers mode may require a larger step.
+        # Get first multiple of steps that are <= _vmin
+        floored_vmins = (_vmin // steps) * steps
+        floored_vmaxs = floored_vmins + steps * nbins
+        large_steps = large_steps & (floored_vmaxs >= _vmax)
+
+    # Find index of smallest large step
+    # istep = np.nonzero(large_steps)[0][0]
+
+    # This is the temporary fix
+    if any(large_steps):
+        istep = np.nonzero(large_steps)[0][0]
+    else:
+        istep = len(steps) - 1
+
+    # Start at smallest of the steps greater than the raw step, and check
+    # if it provides enough ticks. If not, work backwards through
+    # smaller steps until one is found that provides enough ticks.
+    for step in steps[: istep + 1][::-1]:
+
+        if self._integer and np.floor(_vmax) - np.ceil(_vmin) >= self._min_n_ticks - 1:
+            step = max(1, step)
+        best_vmin = (_vmin // step) * step
+
+        # Find tick locations spanning the vmin-vmax range, taking into
+        # account degradation of precision when there is a large offset.
+        # The edge ticks beyond vmin and/or vmax are needed for the
+        # "round_numbers" autolimit mode.
+        edge = _Edge_integer(step, offset)
+        low = edge.le(_vmin - best_vmin)
+        high = edge.ge(_vmax - best_vmin)
+        ticks = np.arange(low, high + 1) * step + best_vmin
+        # Count only the ticks that will be displayed.
+        nticks = ((ticks <= _vmax) & (ticks >= _vmin)).sum()
+        if nticks >= self._min_n_ticks:
+            break
+    return ticks + offset
+
+
+version_loaded = packaging.version.parse(version("matplotlib"))
+version_380 = packaging.version.parse("3.8.0")
+if version_loaded >= version_380:
+    MaxNLocator._raw_ticks = nso_raw_ticks
+
+
 class ReportFormattingException(Exception):
     """
     Error formatting the quality report data into the expected template
     """
 
 
 """
```

### Comparing `dkist_quality-1.0.1/dkist_quality/tests/test_report.py` & `dkist_quality-1.0.2/dkist_quality/tests/test_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,7 +301,25 @@
             f.write(report_bytes)
 
 
 def test_format_invalid_report(dataset_id):
     bad_report_data = {"NotTheKeyYouAreLookingFor": "value"}
     with pytest.raises(ReportFormattingException):
         report_bytes = format_report(bad_report_data, dataset_id)
+
+
+def test_temp_raw_ticks():
+    """
+    There is a matplotlib bug that causes an IndexError when `rcParams["axes.autolimit_mode"] = "round_numbers"`.
+    A temporary fix has been implemented to address the bug.
+    This test tests that temporary fix.
+    """
+    import matplotlib as mpl
+
+    # valid values:  data | round_numbers
+    mpl.rcParams["axes.autolimit_mode"] = "round_numbers"
+    mnl = mpl.ticker.MaxNLocator()
+    mnl._nbins = 1
+    mnl._extended_steps = np.array([0.1, 0.2, 0.5, 1.0, 2.0, 5.0, 10.0, 20.0])
+    actual_raw_ticks = mnl._raw_ticks(-9.4, 18.9)
+    expected_raw_ticks = np.array([-10.0, 0.0, 10.0, 20.0])
+    assert np.array_equal(actual_raw_ticks, expected_raw_ticks)
```

### Comparing `dkist_quality-1.0.1/dkist_quality.egg-info/PKG-INFO` & `dkist_quality-1.0.2/dkist_quality.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dkist-quality
-Version: 1.0.1
+Version: 1.0.2
 Summary: DKIST library for generating quality report pdf
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist-quality
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Requires-Dist: reportlab>=4.0.4
-Requires-Dist: matplotlib<3.8,>=3.6
+Requires-Dist: matplotlib>=3.6
 Requires-Dist: seaborn>=0.13.0
 Requires-Dist: dacite>=1.8.0
 Requires-Dist: natsort>=8.0.0
 Requires-Dist: pydantic<2,>=1.10.4
 Provides-Extra: test
 Requires-Dist: tox>=4; extra == "test"
 Requires-Dist: pytest; extra == "test"
```

### Comparing `dkist_quality-1.0.1/dkist_quality.egg-info/SOURCES.txt` & `dkist_quality-1.0.2/dkist_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.1/licenses/LICENSE.rst` & `dkist_quality-1.0.2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.1/licenses/TEMPLATE_LICENSE.rst` & `dkist_quality-1.0.2/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.1/pyproject.toml` & `dkist_quality-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 license = { text = "BSD 3-Clause" }
 authors = [
   { name = "NSO / AURA", email = "dkistdc@nso.edu" },
 ]
 # the current version of Airflow does not support pydantic v2
 dependencies = [
     "reportlab>=4.0.4",
-    "matplotlib>=3.6,<3.8",
+    "matplotlib>=3.6",
     "seaborn>=0.13.0",
     "dacite>=1.8.0",
     "natsort>=8.0.0",
     "pydantic>=1.10.4,<2",
 ]
 dynamic = ["version"]
```

### Comparing `dkist_quality-1.0.1/tox.ini` & `dkist_quality-1.0.2/tox.ini`

 * *Files identical despite different names*

