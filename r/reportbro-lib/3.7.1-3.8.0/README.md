# Comparing `tmp/reportbro_lib-3.7.1.tar.gz` & `tmp/reportbro_lib-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportbro_lib-3.7.1.tar", max compression
+gzip compressed data, was "reportbro_lib-3.8.0.tar", max compression
```

## Comparing `reportbro_lib-3.7.1.tar` & `reportbro_lib-3.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34520 2024-04-09 09:54:48.145967 reportbro_lib-3.7.1/LICENSE
--rw-r--r--   0        0        0     2145 2024-04-09 09:54:48.145967 reportbro_lib-3.7.1/README.rst
--rw-r--r--   0        0        0     1449 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/pyproject.toml
--rw-r--r--   0        0        0      122 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/__init__.py
--rw-r--r--   0        0        0     7046 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/barcode128.py
--rw-r--r--   0        0        0    10788 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/containers.py
--rw-r--r--   0        0        0    20965 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/context.py
--rw-r--r--   0        0        0        0 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/data/__init__.py
--rw-r--r--   0        0        0    10193 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/data/logo_watermark.png
--rw-r--r--   0        0        0     5962 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/docelement.py
--rw-r--r--   0        0        0    89054 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/elements.py
--rw-r--r--   0        0        0     1162 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/enums.py
--rw-r--r--   0        0        0      698 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/errors.py
--rw-r--r--   0        0        0    21437 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/rendering.py
--rw-r--r--   0        0        0    52455 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/reportbro.py
--rw-r--r--   0        0        0    14818 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/structs.py
--rw-r--r--   0        0        0     1590 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/utils.py
--rw-r--r--   0        0        0       22 2024-04-09 09:54:48.149968 reportbro_lib-3.7.1/reportbro/version.py
--rw-r--r--   0        0        0     3548 1970-01-01 00:00:00.000000 reportbro_lib-3.7.1/PKG-INFO
+-rw-r--r--   0        0        0    34520 2024-05-23 11:05:23.951993 reportbro_lib-3.8.0/LICENSE
+-rw-r--r--   0        0        0     2145 2024-05-23 11:05:23.951993 reportbro_lib-3.8.0/README.rst
+-rw-r--r--   0        0        0     1449 2024-05-23 11:05:23.951993 reportbro_lib-3.8.0/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-23 11:05:23.951993 reportbro_lib-3.8.0/reportbro/__init__.py
+-rw-r--r--   0        0        0     7046 2024-05-23 11:05:23.951993 reportbro_lib-3.8.0/reportbro/barcode128.py
+-rw-r--r--   0        0        0    10787 2024-05-23 11:05:23.951993 reportbro_lib-3.8.0/reportbro/containers.py
+-rw-r--r--   0        0        0    21593 2024-05-23 11:05:23.951993 reportbro_lib-3.8.0/reportbro/context.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:05:23.951993 reportbro_lib-3.8.0/reportbro/data/__init__.py
+-rw-r--r--   0        0        0    10193 2024-05-23 11:05:23.951993 reportbro_lib-3.8.0/reportbro/data/logo_watermark.png
+-rw-r--r--   0        0        0     5962 2024-05-23 11:05:23.951993 reportbro_lib-3.8.0/reportbro/docelement.py
+-rw-r--r--   0        0        0    91789 2024-05-23 11:05:23.955993 reportbro_lib-3.8.0/reportbro/elements.py
+-rw-r--r--   0        0        0     1237 2024-05-23 11:05:23.955993 reportbro_lib-3.8.0/reportbro/enums.py
+-rw-r--r--   0        0        0      698 2024-05-23 11:05:23.955993 reportbro_lib-3.8.0/reportbro/errors.py
+-rw-r--r--   0        0        0    21884 2024-05-23 11:05:23.955993 reportbro_lib-3.8.0/reportbro/rendering.py
+-rw-r--r--   0        0        0    52838 2024-05-23 11:05:23.955993 reportbro_lib-3.8.0/reportbro/reportbro.py
+-rw-r--r--   0        0        0    14818 2024-05-23 11:05:23.955993 reportbro_lib-3.8.0/reportbro/structs.py
+-rw-r--r--   0        0        0     1687 2024-05-23 11:05:23.955993 reportbro_lib-3.8.0/reportbro/utils.py
+-rw-r--r--   0        0        0       22 2024-05-23 11:05:23.955993 reportbro_lib-3.8.0/reportbro/version.py
+-rw-r--r--   0        0        0     3548 1970-01-01 00:00:00.000000 reportbro_lib-3.8.0/PKG-INFO
```

### Comparing `reportbro_lib-3.7.1/LICENSE` & `reportbro_lib-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.1/README.rst` & `reportbro_lib-3.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.1/pyproject.toml` & `reportbro_lib-3.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reportbro-lib"
-version = "3.7.1"
+version = "3.8.0"
 description = "Generate PDF and Excel reports from visually designed templates"
 authors = ["jobsta <alex@reportbro.com>"]
 license = "AGPL-3.0"
 readme = "README.rst"
 
 homepage = "https://www.reportbro.com"
 repository = "https://github.com/jobsta/reportbro-lib"
@@ -30,15 +30,15 @@
 
 include = ["data/logo_watermark.png"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Babel = "^2.14.0"
 python-barcode = "^0.15.1"
-reportbro-fpdf2 = "^2.7.4"
+reportbro-fpdf2 = "^2.7.5"
 # reportbro-fpdf2 = { path = "../fpdf2/", develop = true}
 simpleeval = "^0.9.13"
 Pillow = "^10.2.0"
 qrcode = "^7.4.2"
 XlsxWriter = "^3.0.3"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `reportbro_lib-3.7.1/reportbro/barcode128.py` & `reportbro_lib-3.8.0/reportbro/barcode128.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.1/reportbro/containers.py` & `reportbro_lib-3.8.0/reportbro/containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.container_offset_y = 0
         self.sorted_elements = None  # type: List[DocElementBase]
         self.render_elements = None  # type: List[DocElementBase]
         self.render_elements_created = False
         self.manual_page_break = False
         self.first_element_offset_y = 0
         # maximum bottom value (from element layout coordinates) of currently rendered elements,
-        # this is used the determine if the minimum height of a container
+        # this is used to determine if the minimum height of a container
         # (e.g. table or section band) is reached
         self.max_bottom = 0
         # maximum bottom render value of currently rendered elements, this is the actual container
         # height on the current page
         self.render_bottom = 0
 
     def add(self, doc_element):
```

### Comparing `reportbro_lib-3.7.1/reportbro/context.py` & `reportbro_lib-3.8.0/reportbro/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from collections import namedtuple
 from simpleeval import simple_eval, NameNotDefined, FunctionNotDefined
 from simpleeval import DEFAULT_NAMES as EVAL_DEFAULT_NAMES
 from simpleeval import DEFAULT_FUNCTIONS as EVAL_DEFAULT_FUNCTIONS
 from typing import List, Optional
 import datetime
 import decimal
+import math
 
 from .enums import *
 from .errors import Error, ReportBroError, ReportBroInternalError
 from .structs import Parameter
 
 
 # parameter instance, the data map referenced by the parameter and the data map containing
@@ -21,30 +22,35 @@
 CONTEXT_ENTRY_PARAMETERS = 0
 CONTEXT_ENTRY_DATA = 1
 CONTEXT_ENTRY_DATA_SOURCE = 2
 CONTEXT_ENTRY_PREV_ENTRY = 3
 
 
 class Context:
-    def __init__(self, report, parameters, data):
+    def __init__(self, report, parameters, data, custom_functions):
         self.report = report
         self.pattern_locale = report.document_properties.pattern_locale
         self.pattern_currency_symbol = report.document_properties.pattern_currency_symbol
         data.update(EVAL_DEFAULT_NAMES)
         # each new context (push_context) gets a new unique id
         self.id = 1
         data['__context_id'] = self.id
         self.eval_functions = EVAL_DEFAULT_FUNCTIONS.copy()
         self.eval_functions.update(
             decimal=decimal.Decimal,
             datetime=datetime,
             format_datetime=self.format_datetime_func,
             format_decimal=self.format_decimal_func,
             len=len,
+            abs=abs,
+            floor=math.floor,
+            ceil=math.ceil,
         )
+        if custom_functions:
+            self.eval_functions.update(custom_functions)
         self.root_data = data
         self.root_data['page_number'] = 0
         self.root_data['page_count'] = 0
         self.context_stack: List[ContextEntry] = [
             ContextEntry(parameters=parameters, data=data, data_source=None, prev_entry=None)
         ]
         # a range count is increased inside a table group band (e.g. to show header or sums for grouped rows),
@@ -173,26 +179,28 @@
         if len(self.context_stack) <= 1:
             raise ReportBroInternalError('Context.pop_context failed')
         self.context_stack = self.context_stack[:-1]
 
     def fill_parameters(
             self, expr: str, object_id: int, field: str, pattern: str = None,
             parameter_type: Optional[ParameterType] = None,
-            replaced_parameters: Optional[List[Parameter]] = None) -> str:
+            replaced_parameters: Optional[List[Parameter]] = None, ignore_pattern: bool = False) -> str:
         """
         Return a string where parameter references are replaced with parameter value. A parameter is referenced
         in the format "${parameter_name}".
 
         :param expr: input string which can contain parameter references.
         :param object_id: object id where the expression belongs to, used in case an error is thrown.
         :param field: field name of the expression, used in case an error is thrown.
         :param pattern: optional pattern to format a parameter value. If the pattern is set then it is
         used for all parameter references.
         :param parameter_type: if set then only parameters which match this type are replaced with the parameter value.
         :param replaced_parameters: if set then parameters which are replaced by its value are added to this list.
+        :param ignore_pattern: if True then all patterns (pattern parameter of this method and parameter pattern)
+        are ignored and parameters are replaced with the value of their default string representation.
         :return: string with replaced parameter references.
         """
         if expr.find('${') == -1:
             return expr
         rv = ''
         prev_c = None
         parameter_index = -1
@@ -227,15 +235,19 @@
                             # with p tag we return the parameter value (and thus exclude the surrounding p tag).
                             # this allows rich text parameter content with p tags, otherwise p tags are always
                             # present in the content where the parameter is contained.
                             if param_ref.parameter.type == ParameterType.rich_text and\
                                     value[:2] == '<p' and rv == '<p>' and expr[i + 1:] == '</p>':
                                 return value
                             else:
-                                rv += self.get_formatted_value(value, param_ref.parameter, object_id, pattern=pattern)
+                                if ignore_pattern:
+                                    rv = str(value)
+                                else:
+                                    rv += self.get_formatted_value(
+                                        value, param_ref.parameter, object_id, pattern=pattern)
                     else:
                         # parameter type is set and referenced parameter does not match type -> do not replace parameter
                         rv += '${' + parameter_name + '}'
                     parameter_index = -1
             prev_c = c
         return rv
```

### Comparing `reportbro_lib-3.7.1/reportbro/data/logo_watermark.png` & `reportbro_lib-3.8.0/reportbro/data/logo_watermark.png`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.1/reportbro/docelement.py` & `reportbro_lib-3.8.0/reportbro/docelement.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.1/reportbro/elements.py` & `reportbro_lib-3.8.0/reportbro/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from .context import Context
 from .docelement import DocElementBase, DocElement
 from .enums import *
 from .errors import Error, ReportBroError, ReportBroInternalError
 from .rendering import BarCodeRenderElement, BarcodeSVGWriter, ImageRenderElement, LineRenderElement,\
     TableRenderElement, FrameRenderElement, SectionRenderElement
 from .structs import BorderStyle, Color, ConditionalStyleRule, TextLinePart, TextStyle
-from .utils import get_float_value, get_int_value, get_str_value, to_string, get_image_display_size
+from .utils import get_float_value, get_int_value, get_str_value, to_string, get_image_display_size,\
+    parse_datetime_string, parse_number_string
 
 
 class ImageElement(DocElement):
     def __init__(self, report, data):
         DocElement.__init__(self, report, data)
         self.source = get_str_value(data, 'source')
         self.image = get_str_value(data, 'image')
@@ -364,14 +365,19 @@
             self.remove_empty_element = bool(data.get('removeEmptyElement'))
             self.always_print_on_same_page = bool(data.get('alwaysPrintOnSamePage'))
         self.height = get_int_value(data, 'height')
         self.spreadsheet_hide = bool(data.get('spreadsheet_hide'))
         self.spreadsheet_column = get_int_value(data, 'spreadsheet_column')
         self.spreadsheet_colspan = get_int_value(data, 'spreadsheet_colspan')
         self.spreadsheet_add_empty_row = bool(data.get('spreadsheet_addEmptyRow'))
+        if data.get('spreadsheet_type'):
+            self.spreadsheet_type = SpreadsheetType[data.get('spreadsheet_type')]
+        else:
+            self.spreadsheet_type = SpreadsheetType.default
+        self.spreadsheet_pattern = get_str_value(data, 'spreadsheet_pattern')
         self.spreadsheet_text_wrap = bool(data.get('spreadsheet_textWrap'))
         self.spreadsheet_formats = dict()  # caching of formats for rendering spreadsheet
         self.text_height = 0
         self.line_index = -1
         self.lines_count = 0
         self.text_lines = None
         self.used_style = None
@@ -407,15 +413,20 @@
                         try:
                             content = format_datetime(content, self.pattern, locale=ctx.pattern_locale)
                         except ValueError:
                             raise ReportBroError(
                                 Error('errorMsgInvalidPattern', object_id=self.id, field='pattern', context=self.content))
                 content = to_string(content)
             else:
-                content = self.fill_parameters(ctx)
+                if pdf_doc is None and self.spreadsheet_type != SpreadsheetType.default:
+                    # content is exported to spreadsheet with specific type -> use string representation of
+                    # parameter value so the content can be parsed for the type when spreadsheet is rendered
+                    content = ctx.fill_parameters(self.content, self.id, field='content', ignore_pattern=True)
+                else:
+                    content = self.fill_parameters(ctx)
 
             if self.link:
                 self.prepared_link = ctx.fill_parameters(self.link, self.id, field='link')
                 if not (self.prepared_link.startswith('http://') or self.prepared_link.startswith('https://')):
                     raise ReportBroError(
                         Error('errorMsgInvalidLink', object_id=self.id, field='link'))
         else:
@@ -564,14 +575,28 @@
         self.rendering_complete = rendering_complete
         return text_block_elem, rendering_complete
 
     def is_first_render_element(self):
         return self.first_render_element
 
     def render_spreadsheet(self, row, col, ctx, renderer):
+        content = self.text_lines[0] if self.text_lines else ''
+        if self.spreadsheet_type == SpreadsheetType.date:
+            try:
+                content = parse_datetime_string(content)
+            except (ValueError, TypeError):
+                raise ReportBroError(Error(
+                    msg_key='errorMsgInvalidSpreadsheetDate', object_id=self.id, field='spreadsheet_type'))
+        elif self.spreadsheet_type == SpreadsheetType.number:
+            try:
+                content = parse_number_string(content)
+            except decimal.InvalidOperation:
+                raise ReportBroError(Error(
+                    msg_key='errorMsgInvalidSpreadsheetNumber', object_id=self.id, field='spreadsheet_type'))
+
         cell_format = None
         if self.used_style.id not in self.spreadsheet_formats:
             format_props = dict()
             if self.used_style.bold:
                 format_props['bold'] = True
             if self.used_style.italic:
                 format_props['italic'] = True
@@ -598,25 +623,36 @@
                     format_props['left'] = 1
                 if self.used_style.border_top:
                     format_props['top'] = 1
                 if self.used_style.border_right:
                     format_props['right'] = 1
                 if self.used_style.border_bottom:
                     format_props['bottom'] = 1
+
+            if self.spreadsheet_type != SpreadsheetType.default and self.spreadsheet_pattern:
+                num_format = self.spreadsheet_pattern
+                if '$' in num_format:
+                    num_format = num_format.replace('$', '[$' + ctx.pattern_currency_symbol + ']')
+                format_props['num_format'] = num_format
+            elif self.spreadsheet_type == SpreadsheetType.date:
+                # use iso format as default when no pattern is specified for date parameter, otherwise
+                # date is shown as a number
+                format_props['num_format'] = 'yyyy-mm-dd'
+
             if self.spreadsheet_text_wrap:
                 format_props['text_wrap'] = True
+
             if format_props:
                 cell_format = renderer.add_format(format_props)
                 self.spreadsheet_formats[self.used_style.id] = cell_format
         else:
             # use cached cell format which is already added to renderer
             cell_format = self.spreadsheet_formats[self.used_style.id]
         if self.spreadsheet_column:
             col = self.spreadsheet_column - 1
-        content = self.text_lines[0] if self.text_lines else ''
         renderer.write(row, col, self.spreadsheet_colspan, content, cell_format,
                        self.width, url=self.prepared_link)
         if self.spreadsheet_add_empty_row:
             row += 1
         return row + 1, col + (self.spreadsheet_colspan if self.spreadsheet_colspan else 1)
 
     def set_font_by_style(self, style, pdf_doc):
@@ -1589,14 +1625,19 @@
         from .containers import Container
         assert(isinstance(data, dict))
         self.id = get_int_value(data, 'id')
         self.width = report.document_properties.page_width -\
             report.document_properties.margin_left - report.document_properties.margin_right
         self.height = get_int_value(data, 'height')
         self.band_type = band_type
+        self.background_color = Color(data.get('backgroundColor'))
+        if band_type == BandType.content:
+            self.alternate_background_color = Color(data.get('alternateBackgroundColor'))
+        else:
+            self.alternate_background_color = None
         if band_type == BandType.header:
             self.repeat_header = bool(data.get('repeatHeader'))
             self.always_print_on_same_page = True
         else:
             self.repeat_header = None
             self.always_print_on_same_page = bool(data.get('alwaysPrintOnSamePage'))
         self.shrink_to_content_height = bool(data.get('shrinkToContentHeight'))
@@ -1640,28 +1681,29 @@
                 if remaining_min_height <= available_height:
                     self.prepare_container = True
                     self.container.render_bottom += remaining_min_height
                 else:
                     # minimum height is larger than available space, continue on next page
                     self.rendering_complete = False
                     self.prepare_container = False
-                    self.container.render_bottom += available_height
+                    self.container.render_bottom = available_height
             else:
                 self.prepare_container = True
         else:
             if self.always_print_on_same_page:
                 # band must be printed on same page but available space is not enough,
                 # try to render it on top of next page
                 self.prepare_container = True
                 if offset_y == 0:
                     field = 'size' if self.band_type == BandType.header else 'alwaysPrintOnSamePage'
                     raise ReportBroError(
                         Error('errorMsgSectionBandNotOnSamePage', object_id=self.id, field=field))
             else:
                 self.prepare_container = False
+                self.container.render_bottom = available_height
 
     def get_render_bottom(self):
         return self.container.render_bottom
 
     def get_render_elements(self):
         return self.container.render_elements
 
@@ -1741,27 +1783,31 @@
     def get_next_render_element(self, offset_y, container_top, container_width, container_height, ctx, pdf_doc):
         self.render_y = offset_y
         self.render_bottom = self.render_y
         render_element = SectionRenderElement(self.report, render_y=offset_y)
 
         if self.print_header:
             self.header.create_render_elements(offset_y, container_top, container_height, ctx, pdf_doc)
-            render_element.add_section_band(self.header)
+            render_element.add_section_band(self.header, background_color=self.header.background_color)
             if not self.header.rendering_complete:
                 return render_element, False
             if not self.header.repeat_header:
                 self.print_header = False
 
         while self.row_index < self.row_count:
             # push data context of current row so values of current row can be accessed
             ctx.push_context(self.row_parameters, self.rows[self.row_index], data_source=self.data_source_parameter)
             self.content.create_render_elements(
                 offset_y + render_element.height, container_top, container_height, ctx, pdf_doc)
             ctx.pop_context()
-            render_element.add_section_band(self.content)
+
+            background_color = self.content.background_color
+            if not self.content.alternate_background_color.transparent and self.row_index % 2 == 1:
+                background_color = self.content.alternate_background_color
+            render_element.add_section_band(self.content, background_color=background_color)
             if not self.content.rendering_complete:
                 return render_element, False
             self.row_index += 1
 
             page_break = self.content.container.manual_page_break
             self.content.container.reset()
 
@@ -1769,15 +1815,15 @@
             # we stop rendering and start on new page
             if page_break and self.row_index < self.row_count:
                 return render_element, False
 
         if self.footer:
             self.footer.create_render_elements(
                 offset_y + render_element.height, container_top, container_height, ctx, pdf_doc)
-            render_element.add_section_band(self.footer)
+            render_element.add_section_band(self.footer, background_color=self.footer.background_color)
             if not self.footer.rendering_complete:
                 return render_element, False
 
         # all bands finished
         self.rendering_complete = True
         self.render_bottom += render_element.height
         return render_element, True
```

### Comparing `reportbro_lib-3.7.1/reportbro/enums.py` & `reportbro_lib-3.8.0/reportbro/enums.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,14 +42,20 @@
     simple_array = 7
     map = 8
     sum = 9
     average = 10
     image = 11
 
 
+class SpreadsheetType(Enum):
+    default = 0
+    number = 1
+    date = 2
+
+
 class BandType(Enum):
     header = 1
     content = 2
     footer = 3
 
 
 class PageFormat(Enum):
```

### Comparing `reportbro_lib-3.7.1/reportbro/errors.py` & `reportbro_lib-3.8.0/reportbro/errors.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.1/reportbro/rendering.py` & `reportbro_lib-3.8.0/reportbro/rendering.py`

 * *Files 2% similar despite different names*

```diff
@@ -465,24 +465,34 @@
         self.height = 0
         self.bands = []
         self.complete = False
 
     def is_empty(self):
         return len(self.bands) == 0
 
-    def add_section_band(self, section_band):
+    def add_section_band(self, section_band, background_color):
         if section_band.rendering_complete or not section_band.always_print_on_same_page:
             band_height = section_band.get_render_bottom()
-            self.bands.append(dict(height=band_height, elements=list(section_band.get_render_elements())))
+            self.bands.append(dict(
+                width=section_band.width,
+                height=band_height,
+                background_color=background_color,
+                elements=list(section_band.get_render_elements())
+            ))
             self.height += band_height
             self.render_bottom += band_height
 
     def render_pdf(self, container_offset_x, container_offset_y, pdf_doc):
         y = self.render_y + container_offset_y
         for band in self.bands:
+            if not band['background_color'].transparent:
+                pdf_doc.set_fill_color(
+                    band['background_color'].r, band['background_color'].g, band['background_color'].b)
+                pdf_doc.rect(container_offset_x, y, band['width'], band['height'], 'F')
+
             for element in band['elements']:
                 element.render_pdf(container_offset_x=container_offset_x, container_offset_y=y, pdf_doc=pdf_doc)
             y += band['height']
 
     def cleanup(self):
         for band in self.bands:
             for element in band['elements']:
```

### Comparing `reportbro_lib-3.7.1/reportbro/reportbro.py` & `reportbro_lib-3.8.0/reportbro/reportbro.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,23 +185,23 @@
     def update_column_width(self, col, width):
         if col >= len(self.column_widths):
             # make sure column_width list contains entries for each column
             self.column_widths.extend([-1] * (col + 1 - len(self.column_widths)))
         if width > self.column_widths[col]:
             self.column_widths[col] = width
 
-    def write(self, row, col, colspan, text, cell_format, width, url=None):
+    def write(self, row, col, colspan, data, cell_format, width, url=None):
         if colspan > 1:
-            self.worksheet.merge_range(row, col, row, col + colspan - 1, text, cell_format)
+            self.worksheet.merge_range(row, col, row, col + colspan - 1, data, cell_format)
         elif not url:
-            self.worksheet.write(row, col, text, cell_format)
+            self.worksheet.write(row, col, data, cell_format)
             self.update_column_width(col, width)
         # url also works combined with colspan, the first cell of the range is simply overwritten
         if url:
-            self.worksheet.write_url(row, col, url, cell_format, text)
+            self.worksheet.write_url(row, col, url, cell_format, data)
 
     def insert_image(self, row, col, image_filename, image_data, width, url=None):
         options = dict()
         if image_data:
             options['image_data'] = image_data
         if url:
             options['url'] = url
@@ -522,15 +522,16 @@
             raise ReportBroError(Error('errorMsgMissingGlyph', object_id=object_id, field=field))
 
 
 class Report:
     def __init__(self, report_definition, data, is_test_data=False, additional_fonts=None,
                  page_limit=10000, request_headers=None, encode_error_handling='strict',
                  core_fonts_encoding='windows-1252', spreadsheet_options=None,
-                 allow_local_image=True, allow_external_image=False):
+                 allow_local_image=True, allow_external_image=False,
+                 custom_functions=None):
         """Create Report instance which can then be used to generate pdf and xlsx reports.
 
         :param report_definition: The report object containg report elements, parameters,
         styles and document properties. This object can be obtained in
         ReportBro Designer by using getReport method.
         :param data: Dictionary containing all data for the report.
         This structure must correspond with the defined parameters
@@ -542,31 +543,35 @@
         :param additional_fonts: In case additional (non-standard) fonts are used they
         must be made available so they can be embedded into the pdf file.
         :param page_limit: maximum number of pages for pdf reports. This can
         be used to avoid reports getting too big or taking too long for generation.
         If set to 0 or None then no page limit is used.
         :param request_headers: request headers used when images are fetched by url
         :param encode_error_handling: defines behaviour when a character cannot
-        be encoded with the encoding used for the core fonts. The following options exist:
+        be encoded with the encoding used for the core fonts or when a character
+        is missing in a TrueType Font (custom font). The following options exist:
         - 'strict': raise a UnicodeDecodeError exception
         - 'ignore': just leave the character out of the result
-        - 'replace': use U+FFFD replacement character
+        - 'replace': use '?' as replacement character
         :param core_fonts_encoding: defines the encoding when using the core fonts.
         Default is 'windows-1252' which is usually the best choice for English and many European
         languages including Spanish, French, and German.
         :param spreadsheet_options: options to change default conversion for string content in spreadsheet.
         The dict parameter can contain the following keys:
         - 'strings_to_numbers': enable converting strings to numbers. Default is False.
         - 'strings_to_formulas': enable converting strings to formulas. Default is True.
         - 'strings_to_urls': enable converting strings to urls. Default is True.
         :param allow_local_image: If set to True an image source can contain a relative path to an image
         file on the local file system. If set to False an error is thrown in case a path is specified for an image.
         :param allow_external_image: If set to True an image source can contain an external url. The image will be
         downloaded on the fly when rendering the spreadsheet. If set to False an error is thrown
         in case an url is specified for an image.
+        :param custom_functions: optional dict containing functions which can be used when an expression
+        is evaluated. The dict key is the function name and the value is a function with an arbitrary number
+        of arguments.
         """
         assert isinstance(report_definition, dict)
         assert isinstance(data, dict)
         assert encode_error_handling in ('strict', 'ignore', 'replace')
 
         self.errors = []
 
@@ -655,15 +660,15 @@
                             self.errors.append(Error('errorMsgInvalidSize', object_id=elem.id, field='width'))
                         if elem.y < 0:
                             self.errors.append(Error('errorMsgInvalidPosition', object_id=elem.id, field='y'))
                         elif elem.y + elem.height > container.height:
                             self.errors.append(Error('errorMsgInvalidSize', object_id=elem.id, field='height'))
                     container.add(elem)
 
-            self.context = Context(self, self.parameters, self.data)
+            self.context = Context(self, self.parameters, self.data, custom_functions=custom_functions)
             self.process_data(dest_data=self.data, src_data=data, parameters=parameter_list,
                               is_test_data=is_test_data, parents=[])
 
         try:
             if not self.errors:
                 self.evaluate_parameters(parameter_list, self.data)
         except ReportBroError as err:
```

### Comparing `reportbro_lib-3.7.1/reportbro/structs.py` & `reportbro_lib-3.8.0/reportbro/structs.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.7.1/reportbro/utils.py` & `reportbro_lib-3.8.0/reportbro/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import decimal
 
 current_datetime_str = datetime.datetime.now().strftime('%Y-%m-%d %H:%M')
 
 
 def get_int_value(data, key):
     value = data.get(key)
     return int(value) if value else 0
@@ -37,14 +38,18 @@
     if colon_count == 1:
         date_format = '%Y-%m-%d %H:%M'
     elif colon_count == 2:
         date_format = '%Y-%m-%d %H:%M:%S'
     return datetime.datetime.strptime(val, date_format)
 
 
+def parse_number_string(val):
+    return decimal.Decimal(val.replace(',', '.'))
+
+
 # return image size so image fits into configured width/height and keep aspect ratio
 def get_image_display_size(width, height, image_width, image_height):
     if image_width <= width and image_height <= height:
         image_display_width, image_display_height = image_width, image_height
     else:
         size_ratio = image_width / image_height
         tmp = width / size_ratio
```

### Comparing `reportbro_lib-3.7.1/PKG-INFO` & `reportbro_lib-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reportbro-lib
-Version: 3.7.1
+Version: 3.8.0
 Summary: Generate PDF and Excel reports from visually designed templates
 Home-page: https://www.reportbro.com
 License: AGPL-3.0
 Keywords: pdf,excel,report,generate,create,web,template,layout
 Author: jobsta
 Author-email: alex@reportbro.com
 Requires-Python: >=3.8,<4.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Babel (>=2.14.0,<3.0.0)
 Requires-Dist: Pillow (>=10.2.0,<11.0.0)
 Requires-Dist: XlsxWriter (>=3.0.3,<4.0.0)
 Requires-Dist: python-barcode (>=0.15.1,<0.16.0)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
-Requires-Dist: reportbro-fpdf2 (>=2.7.4,<3.0.0)
+Requires-Dist: reportbro-fpdf2 (>=2.7.5,<3.0.0)
 Requires-Dist: simpleeval (>=0.9.13,<0.10.0)
 Project-URL: Documentation, https://www.reportbro.com/doc/installation
 Project-URL: Repository, https://github.com/jobsta/reportbro-lib
 Description-Content-Type: text/x-rst
 
 ReportBro Lib
 =================
```

