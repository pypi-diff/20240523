# Comparing `tmp/junit2html-31.0.1-py3-none-any.whl.zip` & `tmp/junit2html-31.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 17441 bytes, number of entries: 21
+Zip file size: 17513 bytes, number of entries: 21
 -rw-r--r--  2.0 unx        0 b- defN 24-May-10 20:15 junit2htmlreport/__init__.py
 -rw-r--r--  2.0 unx      106 b- defN 24-May-10 20:15 junit2htmlreport/__main__.py
 -rw-r--r--  2.0 unx      474 b- defN 24-May-10 20:15 junit2htmlreport/case_result.py
 -rw-r--r--  2.0 unx     1080 b- defN 24-May-10 20:15 junit2htmlreport/common.py
--rw-r--r--  2.0 unx     9496 b- defN 24-May-10 20:15 junit2htmlreport/matrix.py
+-rw-r--r--  2.0 unx     9642 b- defN 24-May-23 12:43 junit2htmlreport/matrix.py
 -rw-r--r--  2.0 unx     2647 b- defN 24-May-10 20:15 junit2htmlreport/merge.py
--rw-r--r--  2.0 unx    15374 b- defN 24-May-10 20:15 junit2htmlreport/parser.py
+-rw-r--r--  2.0 unx    15513 b- defN 24-May-23 12:43 junit2htmlreport/parser.py
 -rw-r--r--  2.0 unx      298 b- defN 24-May-10 20:15 junit2htmlreport/parserimpl.py
 -rw-r--r--  2.0 unx     1953 b- defN 24-May-10 20:15 junit2htmlreport/render.py
 -rw-r--r--  2.0 unx     3929 b- defN 24-May-10 20:15 junit2htmlreport/runner.py
 -rw-r--r--  2.0 unx      302 b- defN 24-May-10 20:15 junit2htmlreport/textutils.py
 -rw-r--r--  2.0 unx      297 b- defN 24-May-10 20:15 junit2htmlreport/templates/base.html
 -rw-r--r--  2.0 unx     2795 b- defN 24-May-10 20:15 junit2htmlreport/templates/matrix.html
 -rw-r--r--  2.0 unx     4859 b- defN 24-May-10 20:15 junit2htmlreport/templates/report.html
 -rw-r--r--  2.0 unx     3491 b- defN 24-May-10 20:15 junit2htmlreport/templates/styles.css
--rw-r--r--  2.0 unx     1067 b- defN 24-May-10 20:16 junit2html-31.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      393 b- defN 24-May-10 20:16 junit2html-31.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-10 20:16 junit2html-31.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-10 20:16 junit2html-31.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 24-May-10 20:16 junit2html-31.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1802 b- defN 24-May-10 20:16 junit2html-31.0.1.dist-info/RECORD
-21 files, 50533 bytes uncompressed, 14477 bytes compressed:  71.4%
+-rw-r--r--  2.0 unx     1067 b- defN 24-May-23 12:44 junit2html-31.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      393 b- defN 24-May-23 12:44 junit2html-31.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-23 12:44 junit2html-31.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-23 12:44 junit2html-31.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-May-23 12:44 junit2html-31.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1802 b- defN 24-May-23 12:44 junit2html-31.0.2.dist-info/RECORD
+21 files, 50818 bytes uncompressed, 14549 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -39,26 +39,26 @@
 
 Filename: junit2htmlreport/templates/report.html
 Comment: 
 
 Filename: junit2htmlreport/templates/styles.css
 Comment: 
 
-Filename: junit2html-31.0.1.dist-info/LICENSE
+Filename: junit2html-31.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: junit2html-31.0.1.dist-info/METADATA
+Filename: junit2html-31.0.2.dist-info/METADATA
 Comment: 
 
-Filename: junit2html-31.0.1.dist-info/WHEEL
+Filename: junit2html-31.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: junit2html-31.0.1.dist-info/entry_points.txt
+Filename: junit2html-31.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: junit2html-31.0.1.dist-info/top_level.txt
+Filename: junit2html-31.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: junit2html-31.0.1.dist-info/RECORD
+Filename: junit2html-31.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## junit2htmlreport/matrix.py

```diff
@@ -7,14 +7,20 @@
 from typing import TYPE_CHECKING
 
 from . import parser
 from .case_result import CaseResult
 from .common import ReportContainer
 from .render import HTMLMatrix
 
+UNTESTED = CaseResult.UNTESTED
+PARTIAL_PASS = CaseResult.PARTIAL_PASS
+PARTIAL_FAIL = CaseResult.PARTIAL_FAIL
+TOTAL_FAIL = CaseResult.TOTAL_FAIL
+
+
 if TYPE_CHECKING: # pragma: no cover
     from .parser import Case, Class
     from typing import Dict, List, Optional, Any, Literal
 
 
 class ReportMatrix(ReportContainer):
     """
```

## junit2htmlreport/parser.py

```diff
@@ -15,14 +15,19 @@
 from .render import HTMLReport
 from .textutils import unicode_str
 
 if TYPE_CHECKING:
     from typing import Dict, List, Optional, Union, Any, OrderedDict
 
 NO_CLASSNAME = "no-testclass"
+PASSED = CaseResult.PASSED
+FAILED = CaseResult.FAILED
+SKIPPED = CaseResult.SKIPPED
+ABSENT = CaseResult.ABSENT
+UNKNOWN = CaseResult.UNKNOWN
 
 
 def clean_xml_attribute(element: "ET.Element", attribute: str, default: "Optional[str]"=None):
     """
     Get an XML attribute value and ensure it is legal in XML
     :param element:
     :param attribute:
```

## Comparing `junit2html-31.0.1.dist-info/LICENSE` & `junit2html-31.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `junit2html-31.0.1.dist-info/RECORD` & `junit2html-31.0.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 junit2htmlreport/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 junit2htmlreport/__main__.py,sha256=Pc2x_9ZITfVd9f8zmykZ_JxzC7v0W9OgYYPIRSQNv2s,106
 junit2htmlreport/case_result.py,sha256=Bdh5dNQnDOpgnIKpgw89i--Owo6OibdypuQay4YmuRM,474
 junit2htmlreport/common.py,sha256=uO5m_02Ln6DkbmN1_7IYaRgBnaqQw3z9e41qiOeWaI8,1080
-junit2htmlreport/matrix.py,sha256=zg57QqRoUhbHIiIhmrclfgiWwWphiFSZd-64qwwED7o,9496
+junit2htmlreport/matrix.py,sha256=CYl-X-JGFYt2buIgwyHcjEmXieiutOtbzDuJiDpBwZ8,9642
 junit2htmlreport/merge.py,sha256=F4Ml6VXqMs0S52fxdB6bBU_e5pXaBgFteC-XiHh6BZk,2647
-junit2htmlreport/parser.py,sha256=TSUOWY6OBRFMfSxi0KQIZu7w4FCnjMyaRVhqV15DLYw,15374
+junit2htmlreport/parser.py,sha256=39sEIYpZ9dys3dOcskoqJ3q8rID5KvE8hc-2bEW6GAQ,15513
 junit2htmlreport/parserimpl.py,sha256=PPt2_zzeHwx1HV0MDt228LNE1JjBWH_crspPQsQdpAc,298
 junit2htmlreport/render.py,sha256=cAn4f2hGQInqa7uPG-Poeug-Y81-VmySL-3dz3H7Tlw,1953
 junit2htmlreport/runner.py,sha256=u5D0wtpRr1HU7pAlOE6KrLUQIUMqwR4ZL91bCxNanBY,3929
 junit2htmlreport/textutils.py,sha256=pzYrwfQX2b8V0u6Gaibkh0QGY6yLt8kRYuyVVxvmBMs,302
 junit2htmlreport/templates/base.html,sha256=psEV5nS2H3gyF0fMVuwb4xdzrBt4lpEVeRSdmu7_6Kw,297
 junit2htmlreport/templates/matrix.html,sha256=wm8vJpNckn3RR7gmmeDGTbcdA4qPBHCKy1D2iNPLkFo,2795
 junit2htmlreport/templates/report.html,sha256=nryF11xwS1O_e6Ka5Lzf2FQtMCkkB1PQKGCDwVDT_58,4859
 junit2htmlreport/templates/styles.css,sha256=tH2LNuTQOVH5zCKrnfGwC5lWBKcB-BcijQAB2BkVsaQ,3491
-junit2html-31.0.1.dist-info/LICENSE,sha256=ivuVVcN0m-Z13p4AlvzR1igQOmsKRunaTW0YFrtzKv8,1067
-junit2html-31.0.1.dist-info/METADATA,sha256=AlKsx2CfOBkVY2sPuIrUZDr_JvIs9GRQ-xe7k6iVEFo,393
-junit2html-31.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-junit2html-31.0.1.dist-info/entry_points.txt,sha256=SGCtRQG6bPYBflaA4n9fSC1A07omx-SoOgyti2niMg4,61
-junit2html-31.0.1.dist-info/top_level.txt,sha256=owI63bvIj-v171IWbY9x6W-5vPr0uMP9Hlm9fgjwc4k,17
-junit2html-31.0.1.dist-info/RECORD,,
+junit2html-31.0.2.dist-info/LICENSE,sha256=ivuVVcN0m-Z13p4AlvzR1igQOmsKRunaTW0YFrtzKv8,1067
+junit2html-31.0.2.dist-info/METADATA,sha256=u-uz1eWpKSMgIQHELBGEtOf-3N8lDDH298ysPd5CMj8,393
+junit2html-31.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+junit2html-31.0.2.dist-info/entry_points.txt,sha256=SGCtRQG6bPYBflaA4n9fSC1A07omx-SoOgyti2niMg4,61
+junit2html-31.0.2.dist-info/top_level.txt,sha256=owI63bvIj-v171IWbY9x6W-5vPr0uMP9Hlm9fgjwc4k,17
+junit2html-31.0.2.dist-info/RECORD,,
```

