# Comparing `tmp/pybomwater-0.1.1.tar.gz` & `tmp/pybomwater-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybomwater-0.1.1.tar", max compression
+gzip compressed data, was "pybomwater-0.1.2.tar", last modified: Thu May 23 01:52:37 2024, max compression
```

## Comparing `pybomwater-0.1.1.tar` & `pybomwater-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,21 @@
--rw-r--r--   0        0        0     3383 2021-12-13 05:55:16.056870 pybomwater-0.1.1/LICENSE
--rw-r--r--   0        0        0       66 2023-10-23 00:23:00.993722 pybomwater-0.1.1/pybomwater/__init__.py
--rw-r--r--   0        0        0      164 2023-10-31 02:09:46.315329 pybomwater-0.1.1/pybomwater/_version.py
--rw-r--r--   0        0        0    28974 2023-10-30 05:39:30.323681 pybomwater-0.1.1/pybomwater/bom_water.py
--rw-r--r--   0        0        0 61581716 2023-10-23 00:23:01.338685 pybomwater-0.1.1/pybomwater/cache/stations.json
--rw-r--r--   0        0        0    24713 2023-10-23 00:23:00.995731 pybomwater-0.1.1/pybomwater/cache/waterML_GetDataAvailability.json
--rw-r--r--   0        0        0     3091 2023-10-24 22:14:31.774046 pybomwater-0.1.1/pybomwater/spatial_util.py
--rw-r--r--   0        0        0      870 2023-10-31 02:29:13.335985 pybomwater-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8860 2023-10-31 02:27:15.605255 pybomwater-0.1.1/README.md
--rw-r--r--   0        0        0    10092 1970-01-01 00:00:00.000000 pybomwater-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 01:52:37.538856 pybomwater-0.1.2/
+-rw-rw-rw-   0        0        0     3383 2021-12-13 05:55:16.000000 pybomwater-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     9708 2024-05-23 01:52:37.532861 pybomwater-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8860 2023-10-31 02:27:15.000000 pybomwater-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 01:52:37.367860 pybomwater-0.1.2/pybomwater/
+-rw-rw-rw-   0        0        0       66 2023-10-23 00:23:00.000000 pybomwater-0.1.2/pybomwater/__init__.py
+-rw-rw-rw-   0        0        0      164 2024-05-23 00:53:35.000000 pybomwater-0.1.2/pybomwater/_version.py
+-rw-rw-rw-   0        0        0    28974 2023-10-30 05:39:30.000000 pybomwater-0.1.2/pybomwater/bom_water.py
+-rw-rw-rw-   0        0        0     3091 2023-10-24 22:14:31.000000 pybomwater-0.1.2/pybomwater/spatial_util.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:52:37.525854 pybomwater-0.1.2/pybomwater.egg-info/
+-rw-rw-rw-   0        0        0     9708 2024-05-23 01:52:36.000000 pybomwater-0.1.2/pybomwater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2024-05-23 01:52:37.000000 pybomwater-0.1.2/pybomwater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 01:52:36.000000 pybomwater-0.1.2/pybomwater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-23 01:52:36.000000 pybomwater-0.1.2/pybomwater.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       67 2024-05-23 01:52:36.000000 pybomwater-0.1.2/pybomwater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-23 01:52:36.000000 pybomwater-0.1.2/pybomwater.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      896 2024-05-23 01:52:19.000000 pybomwater-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 01:52:37.540871 pybomwater-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1910 2023-10-30 22:28:05.000000 pybomwater-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:52:37.515853 pybomwater-0.1.2/test/
+-rw-rw-rw-   0        0        0    16362 2023-10-30 05:39:30.000000 pybomwater-0.1.2/test/test_core.py
```

### Comparing `pybomwater-0.1.1/LICENSE` & `pybomwater-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybomwater-0.1.1/pybomwater/bom_water.py` & `pybomwater-0.1.2/pybomwater/bom_water.py`

 * *Files identical despite different names*

### Comparing `pybomwater-0.1.1/pybomwater/spatial_util.py` & `pybomwater-0.1.2/pybomwater/spatial_util.py`

 * *Files identical despite different names*

### Comparing `pybomwater-0.1.1/pyproject.toml` & `pybomwater-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "pybomwater"
-version = "0.1.1"
+version = "0.1.2"
 description = "A python tool for requesting data from BoM Sensor Observation Service (SOS2, as WaterML 2.0 format)"
 authors = ["Andrew Freebairn <andrew.freebairn@csiro.au>"]
 license = "CSIRO Open Source Software Licence Agreement (variation of the BSD / MIT License)"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = ">=3.10,=3.12.2"
 requests = "^2.31.0"
 iso8601 = "^2.1.0"
 pytz = "^2023.3.post1"
 geojson = "^3.0.1"
 shapely = "^2.0.1"
 pytest = "^7.4.2"
 lxml = "^4.9.3"
@@ -22,12 +22,13 @@
 pytest-cov = "^4.1.0"
 owslib = "^0.29.2"
 geopandas = "^0.14.0"
 xarray = "^2023.9.0"
 scipy = "^1.11.3"
 netcdf4 = "^1.6.4"
 wheel = "^0.41.2"
+setuptools = "^70.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pybomwater-0.1.1/README.md` & `pybomwater-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pybomwater-0.1.1/PKG-INFO` & `pybomwater-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,134 +1,126 @@
-Metadata-Version: 2.1
-Name: pybomwater
-Version: 0.1.1
-Summary: A python tool for requesting data from BoM Sensor Observation Service (SOS2, as WaterML 2.0 format)
-License: CSIRO Open Source Software Licence Agreement (variation of the BSD / MIT License)
-Author: Andrew Freebairn
-Author-email: andrew.freebairn@csiro.au
-Requires-Python: >=3.10,<3.12
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: codecov (>=2.1.13,<3.0.0)
-Requires-Dist: fiona (>=1.9.4.post1,<2.0.0)
-Requires-Dist: geojson (>=3.0.1,<4.0.0)
-Requires-Dist: geopandas (>=0.14.0,<0.15.0)
-Requires-Dist: iso8601 (>=2.1.0,<3.0.0)
-Requires-Dist: lxml (>=4.9.3,<5.0.0)
-Requires-Dist: netcdf4 (>=1.6.4,<2.0.0)
-Requires-Dist: owslib (>=0.29.2,<0.30.0)
-Requires-Dist: pandas (>=2.1.1,<3.0.0)
-Requires-Dist: pytest (>=7.4.2,<8.0.0)
-Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
-Requires-Dist: pytz (>=2023.3.post1,<2024.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: scipy (>=1.11.3,<2.0.0)
-Requires-Dist: shapely (>=2.0.1,<3.0.0)
-Requires-Dist: wheel (>=0.41.2,<0.42.0)
-Requires-Dist: xarray (>=2023.9.0,<2024.0.0)
-Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
-Description-Content-Type: text/markdown
-
-# BoM Water
-A python tool for requesting data from BoM Sensor Observation Service (SOS2, as WaterML 2.0 format)
-
-[![license](http://img.shields.io/badge/license-MIT-blue.svg)]() ![status](https://img.shields.io/badge/status-alpha-blue.svg) [![CI](https://github.com/csiro-hydroinformatics/pybomwater/actions/workflows/main.yml/badge.svg)](https://github.com/csiro-hydroinformatics/pybomwater/actions/workflows/main.yml)   ![pypi](https://img.shields.io/pypi/v/pybomwater.svg?logo=python&logoColor=white) 
-[![codecov](https://codecov.io/gh/csiro-hydroinformatics/pybomwater/branch/main/graph/badge.svg?token=uj1VUQu7dT)](https://codecov.io/gh/csiro-hydroinformatics/pybomwater)
-
-
-This package has been developed to access to the BoM Water Data Sensor Observation Service (SOS). With a goal to easily and efficiently integrate data into scientific workflows  
-
-## License
-MIT-derived (see [License.txt](LICENSE))
-
-## Installation
-From pypi:
-
-`pip install pybomwater`
-
-From source:
-- Using [`poetry`](https://python-poetry.org/docs/)
-  - I like to keep the `.venv` in my project directory so I use `poetry config --local virtualenvs.in-project true`
-  - `poetry install` which will install the dependencies listed in the `poetry.lock`
-  - `poetry shell` which is initialize the environment within your running application (eg cmd), or in VS Code `Cmd+Shift+p` and then type `Python Interpreter` and select the environment you just built.
-
-## Usage
-see [Jupyter Notebook example](https://github.com/csiro-hydroinformatics/bomwater-notebook)
-
----
-**NOTE**
-
-The first time a BomWater object is instantiated (bm = bom_water.BomWater()) a cache of data is created.  This process obtains data from the BoM service and will take a little while to complete.  Once cached this process is not repeated and performance will return to normal.
-
----
-
-## Documentation
-Bureau of Meteorology (BoM) documentation on using their SOS service is available at the following links:
-* [BoM Water Data service ](http://www.bom.gov.au/waterdata/services)
-* [BoM Notes](http://www.bom.gov.au/metadata/catalogue/19115/ANZCW0503900528)
-* [BoM Guide to Sensor Observation Services (SOS2)](https://github.com/csiro-hydroinformatics/bom_water/blob/main/doc/Guide_to_Sensor_Observation_Services_(SOS2)_for_Water_Data_Online_v1.0.1.pdf)
-
-### [The following cells implement requests that access the BoM SOS2 service.](https://github.com/csiro-hydroinformatics/bom_water/blob/main/doc/Guide_to_Sensor_Observation_Services_(SOS2)_for_Water_Data_Online_v1.0.1.pdf#page=14) 
-### GetCapabilties
-Lists services available and the filters that can be used to select data output by those services. It also provides an overview of parameters, time series types and geographic area covered by the services.
-### GetFeatureOfInterest
-Provides details about a set of geographical features or locations at which observations are measured. They can be selected according to the parameter measured, type of time series available, and area or point location.
-### GetDataAvailability
-Lists the type of data available for a ‘feature of interest’ and its coverage. This includes a list of parameters, the time series types available for each of the parameters, and the observed period of record for each time series type.
-### GetObservation
-Returns observations of a specified ‘feature of interest’ and parameter, within a specific time series type. Each observation has a datetime, value, quality and interpolation type.
-
-### [Parameter currently available via SOS2](https://github.com/csiro-hydroinformatics/bom_water/blob/main/doc/Guide_to_Sensor_Observation_Services_(SOS2)_for_Water_Data_Online_v1.0.1.pdf#page=13)
-|Parameter | Water regulation Data Subcategory |
-|:--- |:--- |
-|Dry Air Temperature  |  4f  |
-|Electrical Conductivity @ 25C  | 9a  |
-|Evaporation  | 4c  |
-|Ground Water Level  | 2a  |
-|Rainfall  | 4a  |
-|Relative Humidity  | 4h  |
-|Storage Level  | 3a  |
-|Storage Volume  | 3b  |
-|Turbidity  | 9d  |
-|Water Course Discharge (standard time series types)  | 1b  |
-|Water Course Discharge (flood warning time series types)  | 11b  |
-|Water Course Level (standard time series types)  | 1a  |
-|Water Course Level (flood warning time series types)   | 11a  |
-|Water pH  | 9g  |
-|Water Temperature  | 9h  |
-|Wind Direction  | 4  |
-### [Timeseries pattern and aggreated available](https://github.com/csiro-hydroinformatics/bom_water/blob/main/doc/Guide_to_Sensor_Observation_Services_(SOS2)_for_Water_Data_Online_v1.0.1.pdf#page=37)
-|Time series name | Procedure | Identifier Time series description |
-|:---|:---|:---|
-|DMQaQc.Merged.DailyMean.24HR| Pat1_C_B_1_DailyMean or Pat9_C_B_1_DailyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to daily means, reported from midnight to midnight. |
-|DMQaQc.Merged.DailyMax.24HR | Pat1_C_B_1_DailyMax or Pat9_C_B_1_DailyMax | Maximum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight |
-|DMQaQc.Merged.DailyMin.24HR | Pat1_C_B_1_DailyMin or Pat9_C_B_1_DailyMin | Minimum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.  |
-|DMQaQc.Merged.MonthlyMean.CalMonth| Pat1_C_B_1_MonthlyMean or Pat9_C_B_1_MonthlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to monthly means. |
-|DMQaQc.Merged.YearlyMean.CalYear | Pat1_C_B_1_YearlyMean or Pat9_C_B_1_YearlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to yearly means. |
-|DMQaQc.Merged.DailyTotal.09HR | Pat2_C_B_1_DailyTot09 | DMQaQc.Merged.AsStored.1 timeseries aggregated to daily totals, reported from 9am to 9am. |
-|DMQaQc.Merged.DailyTotal.24HR|Pat2_C_B_1_DailyTot24 | DMQaQc.Merged.AsStored.1 timeseries aggregated to daily totals,reported from midnight to midnight.|
-|DMQaQc.Merged.MonthlyTotal.CalMonth|Pat2_C_B_1_MonthlyTot24 | DMQaQc.Merged.AsStored.1 timeseries aggregated to monthly totals.|
-|DMQaQc.Merged.YearlyTotal.CalYear|Pat2_C_B_1_YearlyTot24 | DMQaQc.Merged.AsStored.1 timeseries aggregated to yearly totals.|
-|DMQaQc.Merged.HourlyMean.HR|Pat3_C_B_1_HourlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to hourly means.|
-|DMQaQc.Merged.DailyMean.24HR|Pat3_C_B_1_DailyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to daily means, reported from midnight to midnight.|
-|DMQaQc.Merged.DailyMax.24HR |Pat3_C_B_1_DailyMax | Maximum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.|
-|DMQaQc.Merged.DailyMin.24HR|Pat3_C_B_1_DailyMin | Minimum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.|
-|DMQaQc.Merged.MonthlyMean.CalMonth|Pat3_C_B_1_MonthlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to monthly means.|
-|DMQaQc.Merged.YearlyMean.CalYear|Pat3_C_B_1_YearlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to yearly means.|
-|DMQaQc.Merged.HourlyMean.HR|Pat4_C_B_1_HourlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to hourly means.|
-|DMQaQc.Merged.DailyMean.09HR| Pat4_C_B_1_DailyMean09 | DMQaQc.Merged.AsStored.1 timeseries aggregated to daily means, reported from 9am to 9am.|
-|DMQaQc.Merged.DailyMax.24HR|Pat4_C_B_1_DailyMax | Maximum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.|
-|DMQaQc.Merged.DailyMin.24HR|Pat4_C_B_1_DailyMin | Minimum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.|
-|DMQaQc.Merged.DailyMean.24HR|Pat4_C_B_1_DailyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to daily means, reported from midnight to midnight.|
-|DMQaQc.Merged.MonthlyMean.CalMonth|Pat4_C_B_1_MonthlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to monthly means.|
-|DMQaQc.Merged.YearlyMean.CalYear|Pat4_C_B_1_YearlyMean| DMQaQc.Merged.AsStored.1 timeseries aggregated to yearly means.|
-|DMQaQc.Merged.HourlyMean.HR|Pat6_C_B_1_HourlyMean or Pat7_C_B_1_HourlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to hourly means.|
-|DMQaQc.Merged.DailyMean.24HR|Pat6_C_B_1_DailyMean or Pat7_C_B_1_DailyMean|DMQaQc.Merged.AsStored.1 timeseries aggregated to daily means, reported from midnight to midnight.|
-|DMQaQc.Merged.DailyMax.24HR|Pat6_C_B_1_DailyMax or Pat7_C_B_1_DailyMax | Maximum of values in theDMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.|
-|DMQaQc.Merged.DailyMin.24HR|Pat6_C_B_1_DailyMin or Pat7_C_B_1_DailyMin | Minimum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.|
-|DMQaQc.Merged.MonthlyMean.CalMonth|Pat6_C_B_1_MonthlyMean or Pat7_C_B_1_MonthlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to monthly means.|
-|DMQaQc.Merged.YearlyMean.CalYear |Pat6_C_B_1_YearlyMean or Pat7_C_B_1_YearlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to yearly means.|
-
-## [Task list](https://github.com/csiro-hydroinformatics/bom_water/blob/main/tasklist.md)
-
+Metadata-Version: 2.1
+Name: pybomwater
+Version: 0.1.2
+Summary: A tool for requesting data from BoM Water Data service.
+Home-page: https://github.com/csiro-hydroinformatics/pybomwater
+Author: Andrew Freebairn
+Author-email: andrew.freebairn@csiro.au
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Hydrology
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: iso8601
+Requires-Dist: wheel
+Requires-Dist: pytz
+Requires-Dist: json5
+Requires-Dist: xmltodict
+Requires-Dist: pandas
+Requires-Dist: geojson
+Requires-Dist: shapely
+
+# BoM Water
+A python tool for requesting data from BoM Sensor Observation Service (SOS2, as WaterML 2.0 format)
+
+[![license](http://img.shields.io/badge/license-MIT-blue.svg)]() ![status](https://img.shields.io/badge/status-alpha-blue.svg) [![CI](https://github.com/csiro-hydroinformatics/pybomwater/actions/workflows/main.yml/badge.svg)](https://github.com/csiro-hydroinformatics/pybomwater/actions/workflows/main.yml)   ![pypi](https://img.shields.io/pypi/v/pybomwater.svg?logo=python&logoColor=white) 
+[![codecov](https://codecov.io/gh/csiro-hydroinformatics/pybomwater/branch/main/graph/badge.svg?token=uj1VUQu7dT)](https://codecov.io/gh/csiro-hydroinformatics/pybomwater)
+
+
+This package has been developed to access to the BoM Water Data Sensor Observation Service (SOS). With a goal to easily and efficiently integrate data into scientific workflows  
+
+## License
+MIT-derived (see [License.txt](LICENSE))
+
+## Installation
+From pypi:
+
+`pip install pybomwater`
+
+From source:
+- Using [`poetry`](https://python-poetry.org/docs/)
+  - I like to keep the `.venv` in my project directory so I use `poetry config --local virtualenvs.in-project true`
+  - `poetry install` which will install the dependencies listed in the `poetry.lock`
+  - `poetry shell` which is initialize the environment within your running application (eg cmd), or in VS Code `Cmd+Shift+p` and then type `Python Interpreter` and select the environment you just built.
+
+## Usage
+see [Jupyter Notebook example](https://github.com/csiro-hydroinformatics/bomwater-notebook)
+
+---
+**NOTE**
+
+The first time a BomWater object is instantiated (bm = bom_water.BomWater()) a cache of data is created.  This process obtains data from the BoM service and will take a little while to complete.  Once cached this process is not repeated and performance will return to normal.
+
+---
+
+## Documentation
+Bureau of Meteorology (BoM) documentation on using their SOS service is available at the following links:
+* [BoM Water Data service ](http://www.bom.gov.au/waterdata/services)
+* [BoM Notes](http://www.bom.gov.au/metadata/catalogue/19115/ANZCW0503900528)
+* [BoM Guide to Sensor Observation Services (SOS2)](https://github.com/csiro-hydroinformatics/bom_water/blob/main/doc/Guide_to_Sensor_Observation_Services_(SOS2)_for_Water_Data_Online_v1.0.1.pdf)
+
+### [The following cells implement requests that access the BoM SOS2 service.](https://github.com/csiro-hydroinformatics/bom_water/blob/main/doc/Guide_to_Sensor_Observation_Services_(SOS2)_for_Water_Data_Online_v1.0.1.pdf#page=14) 
+### GetCapabilties
+Lists services available and the filters that can be used to select data output by those services. It also provides an overview of parameters, time series types and geographic area covered by the services.
+### GetFeatureOfInterest
+Provides details about a set of geographical features or locations at which observations are measured. They can be selected according to the parameter measured, type of time series available, and area or point location.
+### GetDataAvailability
+Lists the type of data available for a â€˜feature of interestâ€™ and its coverage. This includes a list of parameters, the time series types available for each of the parameters, and the observed period of record for each time series type.
+### GetObservation
+Returns observations of a specified â€˜feature of interestâ€™ and parameter, within a specific time series type. Each observation has a datetime, value, quality and interpolation type.
+
+### [Parameter currently available via SOS2](https://github.com/csiro-hydroinformatics/bom_water/blob/main/doc/Guide_to_Sensor_Observation_Services_(SOS2)_for_Water_Data_Online_v1.0.1.pdf#page=13)
+|Parameter | Water regulation Data Subcategory |
+|:--- |:--- |
+|Dry Air Temperature  |  4f  |
+|Electrical Conductivity @ 25C  | 9a  |
+|Evaporation  | 4c  |
+|Ground Water Level  | 2a  |
+|Rainfall  | 4a  |
+|Relative Humidity  | 4h  |
+|Storage Level  | 3a  |
+|Storage Volume  | 3b  |
+|Turbidity  | 9d  |
+|Water Course Discharge (standard time series types)  | 1b  |
+|Water Course Discharge (flood warning time series types)  | 11b  |
+|Water Course Level (standard time series types)  | 1a  |
+|Water Course Level (flood warning time series types)   | 11a  |
+|Water pH  | 9g  |
+|Water Temperature  | 9h  |
+|Wind Direction  | 4  |
+### [Timeseries pattern and aggreated available](https://github.com/csiro-hydroinformatics/bom_water/blob/main/doc/Guide_to_Sensor_Observation_Services_(SOS2)_for_Water_Data_Online_v1.0.1.pdf#page=37)
+|Time series name | Procedure | Identifier Time series description |
+|:---|:---|:---|
+|DMQaQc.Merged.DailyMean.24HR| Pat1_C_B_1_DailyMean or Pat9_C_B_1_DailyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to daily means, reported from midnight to midnight. |
+|DMQaQc.Merged.DailyMax.24HR | Pat1_C_B_1_DailyMax or Pat9_C_B_1_DailyMax | Maximum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight |
+|DMQaQc.Merged.DailyMin.24HR | Pat1_C_B_1_DailyMin or Pat9_C_B_1_DailyMin | Minimum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.  |
+|DMQaQc.Merged.MonthlyMean.CalMonth| Pat1_C_B_1_MonthlyMean or Pat9_C_B_1_MonthlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to monthly means. |
+|DMQaQc.Merged.YearlyMean.CalYear | Pat1_C_B_1_YearlyMean or Pat9_C_B_1_YearlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to yearly means. |
+|DMQaQc.Merged.DailyTotal.09HR | Pat2_C_B_1_DailyTot09 | DMQaQc.Merged.AsStored.1 timeseries aggregated to daily totals, reported from 9am to 9am. |
+|DMQaQc.Merged.DailyTotal.24HR|Pat2_C_B_1_DailyTot24 | DMQaQc.Merged.AsStored.1 timeseries aggregated to daily totals,reported from midnight to midnight.|
+|DMQaQc.Merged.MonthlyTotal.CalMonth|Pat2_C_B_1_MonthlyTot24 | DMQaQc.Merged.AsStored.1 timeseries aggregated to monthly totals.|
+|DMQaQc.Merged.YearlyTotal.CalYear|Pat2_C_B_1_YearlyTot24 | DMQaQc.Merged.AsStored.1 timeseries aggregated to yearly totals.|
+|DMQaQc.Merged.HourlyMean.HR|Pat3_C_B_1_HourlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to hourly means.|
+|DMQaQc.Merged.DailyMean.24HR|Pat3_C_B_1_DailyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to daily means, reported from midnight to midnight.|
+|DMQaQc.Merged.DailyMax.24HR |Pat3_C_B_1_DailyMax | Maximum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.|
+|DMQaQc.Merged.DailyMin.24HR|Pat3_C_B_1_DailyMin | Minimum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.|
+|DMQaQc.Merged.MonthlyMean.CalMonth|Pat3_C_B_1_MonthlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to monthly means.|
+|DMQaQc.Merged.YearlyMean.CalYear|Pat3_C_B_1_YearlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to yearly means.|
+|DMQaQc.Merged.HourlyMean.HR|Pat4_C_B_1_HourlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to hourly means.|
+|DMQaQc.Merged.DailyMean.09HR| Pat4_C_B_1_DailyMean09 | DMQaQc.Merged.AsStored.1 timeseries aggregated to daily means, reported from 9am to 9am.|
+|DMQaQc.Merged.DailyMax.24HR|Pat4_C_B_1_DailyMax | Maximum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.|
+|DMQaQc.Merged.DailyMin.24HR|Pat4_C_B_1_DailyMin | Minimum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.|
+|DMQaQc.Merged.DailyMean.24HR|Pat4_C_B_1_DailyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to daily means, reported from midnight to midnight.|
+|DMQaQc.Merged.MonthlyMean.CalMonth|Pat4_C_B_1_MonthlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to monthly means.|
+|DMQaQc.Merged.YearlyMean.CalYear|Pat4_C_B_1_YearlyMean| DMQaQc.Merged.AsStored.1 timeseries aggregated to yearly means.|
+|DMQaQc.Merged.HourlyMean.HR|Pat6_C_B_1_HourlyMean or Pat7_C_B_1_HourlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to hourly means.|
+|DMQaQc.Merged.DailyMean.24HR|Pat6_C_B_1_DailyMean or Pat7_C_B_1_DailyMean|DMQaQc.Merged.AsStored.1 timeseries aggregated to daily means, reported from midnight to midnight.|
+|DMQaQc.Merged.DailyMax.24HR|Pat6_C_B_1_DailyMax or Pat7_C_B_1_DailyMax | Maximum of values in theDMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.|
+|DMQaQc.Merged.DailyMin.24HR|Pat6_C_B_1_DailyMin or Pat7_C_B_1_DailyMin | Minimum of values in the DMQaQc.Merged.AsStored.1 timeseries - from midnight to midnight.|
+|DMQaQc.Merged.MonthlyMean.CalMonth|Pat6_C_B_1_MonthlyMean or Pat7_C_B_1_MonthlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to monthly means.|
+|DMQaQc.Merged.YearlyMean.CalYear |Pat6_C_B_1_YearlyMean or Pat7_C_B_1_YearlyMean | DMQaQc.Merged.AsStored.1 timeseries aggregated to yearly means.|
+
+## [Task list](https://github.com/csiro-hydroinformatics/bom_water/blob/main/tasklist.md)
```

