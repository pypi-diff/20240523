# Comparing `tmp/zut-0.9.1-py3-none-any.whl.zip` & `tmp/zut-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 54123 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat    88849 b- defN 24-May-20 08:57 zut/__init__.py
--rw-rw-rw-  2.0 fat      427 b- defN 24-May-20 15:24 zut/_version.py
--rw-rw-rw-  2.0 fat    24764 b- defN 24-Mar-21 02:07 zut/excel.py
--rw-rw-rw-  2.0 fat    12859 b- defN 24-Mar-21 10:49 zut/files.py
+Zip file size: 48922 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat    89190 b- defN 24-May-23 15:47 zut/__init__.py
+-rw-rw-rw-  2.0 fat      427 b- defN 24-May-23 17:07 zut/_version.py
+-rw-rw-rw-  2.0 fat    25956 b- defN 24-May-23 09:45 zut/excel.py
+-rw-rw-rw-  2.0 fat    12923 b- defN 24-May-23 12:12 zut/files.py
 -rw-rw-rw-  2.0 fat     2984 b- defN 24-May-20 14:22 zut/db/__init__.py
--rw-rw-rw-  2.0 fat    27603 b- defN 24-May-20 14:04 zut/db/base.py
--rw-rw-rw-  2.0 fat    11635 b- defN 24-May-20 14:18 zut/db/mssql.py
--rw-rw-rw-  2.0 fat     8390 b- defN 24-May-20 15:01 zut/db/mysql.py
--rw-rw-rw-  2.0 fat    19153 b- defN 24-May-20 13:13 zut/db/pg.py
--rw-rw-rw-  2.0 fat     3808 b- defN 24-Mar-21 09:36 zut/db/pg2.py
+-rw-rw-rw-  2.0 fat    25278 b- defN 24-May-21 12:29 zut/db/base.py
+-rw-rw-rw-  2.0 fat     7700 b- defN 24-May-21 12:29 zut/db/mssql.py
+-rw-rw-rw-  2.0 fat     3265 b- defN 24-May-21 12:29 zut/db/mysql.py
+-rw-rw-rw-  2.0 fat     7151 b- defN 24-May-21 12:29 zut/db/pg.py
+-rw-rw-rw-  2.0 fat     3557 b- defN 24-May-21 12:29 zut/db/pg2.py
 -rw-rw-rw-  2.0 fat     1641 b- defN 24-Jan-24 18:06 zut/db/sql-utils/pg.sql
--rw-rw-rw-  2.0 fat     1103 b- defN 24-May-20 15:24 zut-0.9.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     3872 b- defN 24-May-20 15:24 zut-0.9.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-20 15:24 zut-0.9.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 24-May-20 15:24 zut-0.9.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1165 b- defN 24-May-20 15:24 zut-0.9.1.dist-info/RECORD
-16 files, 208349 bytes uncompressed, 52271 bytes compressed:  74.9%
+-rw-rw-rw-  2.0 fat     1103 b- defN 24-May-23 17:07 zut-0.9.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     3872 b- defN 24-May-23 17:07 zut-0.9.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 17:07 zut-0.9.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 24-May-23 17:07 zut-0.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1163 b- defN 24-May-23 17:07 zut-0.9.2.dist-info/RECORD
+16 files, 186306 bytes uncompressed, 47070 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: zut/db/pg2.py
 Comment: 
 
 Filename: zut/db/sql-utils/pg.sql
 Comment: 
 
-Filename: zut-0.9.1.dist-info/LICENSE.txt
+Filename: zut-0.9.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: zut-0.9.1.dist-info/METADATA
+Filename: zut-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: zut-0.9.1.dist-info/WHEEL
+Filename: zut-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: zut-0.9.1.dist-info/top_level.txt
+Filename: zut-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: zut-0.9.1.dist-info/RECORD
+Filename: zut-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zut/__init__.py

```diff
@@ -845,20 +845,24 @@
     """
     now = datetime.now().astimezone(parse_tz(tz))
     if not ms:
         now = now.replace(microsecond=0)
     return now
 
 
-def make_aware(value: T_WithTime, tz: tzinfo|str = None) -> T_WithTime:
+def make_aware(value: T_WithTime, tz: tzinfo|str = None, after1970: bool = False) -> T_WithTime:
     """
     Make a datetime aware in timezone `tz` (use `tz=None` or `tz='localtime'` for the system local timezone).
     """
     if value is None:
         return None
+
+    if after1970 and value.year <= 1970:
+        return None
+    
     if is_aware(value):
         raise ValueError("make_aware expects a naive datetime, got %s" % value)
     
     tz = parse_tz(tz, explicit_local=True)
     if hasattr(tz, 'localize'):
         # See: https://stackoverflow.com/a/6411149
         return tz.localize(value)
@@ -866,20 +870,24 @@
         return value.replace(tzinfo=tz)
 
 
 def is_naive(value: T_WithTime):
     return not is_aware(value)
 
 
-def make_naive(value: T_WithTime, tz: tzinfo = None) -> T_WithTime:
+def make_naive(value: T_WithTime, tz: tzinfo = None, after1970: bool = False) -> T_WithTime:
     """
     Make a datetime naive and expressed in timezone `tz` (use `tz=None` or `tz='localtime'` for the system local timezone).
     """
     if value is None:
         return None
+
+    if after1970 and value.year <= 1970:
+        return None
+
     if not is_aware(value):
         raise ValueError("make_naive expects an aware datetime, got %s" % value)
     
     value = value.astimezone(parse_tz(tz))
     value = value.replace(tzinfo=None)
     return value
 
@@ -1343,15 +1351,15 @@
         
         if self.title is not False:
             logger.info(f"{'Append' if self._append else 'Export'}{f' {self.title}' if self.title else ''} to {self.out_name}")
 
         return self
             
     
-    def __exit__(self, exc_type = None, exc_val = None, exc_tb = None):        
+    def __exit__(self, exc_type = None, exc_value = None, exc_traceback = None):
         if not self.atexit:
             self.close()
 
 
     @property
     def file(self):
         if self._file is None:
@@ -1433,15 +1441,15 @@
         super().__init__(out, title=title, append=append, encoding=encoding, atexit=atexit)
 
         if self.db:
             self.out_name = self.db.get_url(hide_password=True)
 
         self.headers: list[Header] = headers  # for CSV, not None <=> export started
 
-        if self.db:
+        if self.db: #TODO: adapt zut.db and csv formatting
             if tablefmt and tablefmt != 'csv':
                 raise ValueError(f"Tablefmt \"{tablefmt}\" cannot be used for a database output")
             if csv_decimal_separator and csv_decimal_separator != '.':
                 raise ValueError(f"CSV decimal separator \"{csv_decimal_separator}\" cannot be used for a database output")
             self.tablefmt = 'csv'
             csv_decimal_separator = '.' # only this decimal separator is understood by Pg COPY command
         elif not self.out:
@@ -1789,16 +1797,17 @@
         if self.headers:
             floatfmts = []
             for header in self.headers:
                 floatfmts.append(header._get_tabulate_floatfmt())
             result = tabulate(rows, headers=self.headers, floatfmt=tuple(floatfmts))
         else:
             result = tabulate(rows)
-        
-        print(result, file=self.file)
+
+        for line in result.splitlines():
+            print(line, file=self.file)
 
 
     def _escape_tabulate_value(self, value: str, *, header: Header|None):
         if header and header.max_length is not None:
             if not isinstance(value, str):
                 return value
             
@@ -1910,14 +1919,15 @@
     #endregion
 
 
     #region DB specifics
             
     def _export_db(self):                        
         logger.debug(f"Copy data to table %s.%s", self.db.schema, self.db.table)
+        raise NotImplementedError("TODO")
         self.out.seek(0)
         self.db.load_from_csv(self.out, columns=[header.name for header in self.headers], encoding=self.encoding, csv_delimiter=self.csv_delimiter, csv_quotechar=self.csv_quotechar, csv_nullval=self.csv_nullval)
 
     #endregion
 
 
 class Header:
@@ -1993,15 +2003,15 @@
                     value = human_bytes(value)
         
             elif self.fmt == 'datetime' or self.fmt == 'dateortime' or self.fmt == 'datetime1970' or self.fmt == 'dateortime1970':
                 if not isinstance(value, datetime):
                     value = convert_to_datetime(value)
                 if value.year <= 1970 and (after1970 or self.fmt == 'datetime1970' or self.fmt == 'dateortime1970'):
                     value = None
-                if tablefmt and tablefmt != 'excel' and self.fmt == 'dateortime':
+                if tablefmt and tablefmt != 'excel' and (self.fmt == 'dateortime' or self.fmt == 'dateortime1970'):
                     value = value.strftime('%H:%M:%S') if value.date() == today() else value.strftime('%Y-%m-%d')
 
         elif callable(self.fmt):
             if self.fmt in {bool, int, float, Decimal, datetime, date, time, list}:
                 value = convert(value, self.fmt)
             else:
                 value = self.fmt(value)
```

## zut/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '0.9.1'
-__version_tuple__ = version_tuple = (0, 9, 1)
+__version__ = version = '0.9.2'
+__version_tuple__ = version_tuple = (0, 9, 2)
```

## zut/excel.py

```diff
@@ -1,13 +1,14 @@
 """
 Manipulate Excel tables.
 """
 from __future__ import annotations
 
 import logging
+import os
 import re
 from configparser import _UNSET
 from pathlib import Path
 from typing import Any
 
 try:
     import openpyxl
@@ -25,37 +26,41 @@
     PatternFill = dict
 
 from . import files
 
 logger = logging.getLogger(__name__)
 
 
-def is_excel_path(path: str|Path, accept_table_suffix = False):
+def is_excel_path(path: str|Path, *, accept_table_suffix = False):
     if isinstance(path, Path):
         path = str(path)
     elif not isinstance(path, str):
-        raise ValueError(f'invalid path type: {type(path)}')
+        raise ValueError(f'Invalid path type: {type(path)}')
     
     return re.search(r'\.xlsx(?:#[^\.]+)?$' if accept_table_suffix else r'\.xlsx$', path, re.IGNORECASE)
 
 
-def split_excel_path(path: str|Path, default_table_name: str = None, **kwargs) -> tuple[Path,str]:
+def split_excel_path(path: str|Path, *, default_table_name: str = None, dir: str|Path = None, **kwargs) -> tuple[Path,str]:
     """ Return (actual path, table name) """
     if isinstance(path, Path):
         path = str(path)
     elif not isinstance(path, str):
-        raise ValueError(f'invalid path type: {type(path)}')
+        raise ValueError(f'Invalid path type: {type(path)}')
         
     path = path.format(**kwargs)
 
     m = re.match(r'^(.+\.xlsx)(?:#([^\.]*))?$', path, re.IGNORECASE)
     if not m:
         return (Path(path), default_table_name)
     
-    return (Path(m[1]), m[2] if m[2] else default_table_name)
+    path = m[1]    
+    if dir and not path.startswith(('./','.\\')):
+        path = os.path.join(dir, path)
+    
+    return (Path(path), m[2] if m[2] else default_table_name)
 
 
 class ExcelWorkbook:
     _workbook_cache: dict[str,ExcelWorkbook] = {}
     """ Workbooks per canonical path """
     
     _defusedxml_alert_emitted = False
@@ -67,20 +72,20 @@
         if not DEFUSEDXML and not self.__class__._defusedxml_alert_emitted:
             logger.warning("Install package `defusedxml` (in addition to `openpyxl`) to guard against quadratic blowup or billion laughs xml attacks")
             self.__class__._defusedxml_alert_emitted = True
 
         self.path = Path(path) if not isinstance(path, Path) else path
 
         if files.exists(self.path):
-            logger.debug("load excel workbook %s", self.path)
+            logger.debug("Load excel workbook %s", self.path)
             with files.open(self.path, 'rb') as fp:
                 self.pyxl_workbook: Workbook = load_workbook(fp) #NOTE: using keep_vba=True causes issues, example on openpyxl 3.1.2: load and save samples/empty-table.xlsx without modification corrupts the file
             self._create_next_table_in_active_sheet = False
         else:
-            logger.debug("create excel workbook for %s", self.path)
+            logger.debug("Create excel workbook for %s", self.path)
             self.pyxl_workbook = Workbook()
             self._create_next_table_in_active_sheet = True
 
         self.tables: dict[str,ExcelTable] = {}
         self.needs_save = False
 
 
@@ -104,49 +109,60 @@
     def close_all_cached(cls):
         for workbook in cls._workbook_cache.values():
             workbook.close()
 
 
     def close(self):
         if not self.needs_save:
-            logger.debug("excel workbook %s not modified", self.path)
+            logger.debug("Excel workbook %s not modified", self.path)
             return
         
         for table in self.tables.values():
             table.redefine()
         
-        logger.debug("save excel workbook %s", self.path)
+        logger.debug("Save excel workbook %s", self.path)
         with files.open(self.path, 'wb') as fp:
             self.pyxl_workbook.save(fp)
 
         self.needs_save = False
         
 
-    def get_table(self, name: str, default = '__raise__') -> ExcelTable:
-        if name in self.tables:
-            return self.tables[name]
-        
-        for sheet_name in self.pyxl_workbook.sheetnames:
-            pyxl_worksheet: Worksheet = self.pyxl_workbook[sheet_name]
-            if name in pyxl_worksheet.tables:
-                pyxl_table = pyxl_worksheet.tables[name]
-                self.tables[name] = ExcelTable(pyxl_table, pyxl_worksheet, self)
+    def get_table(self, name: str|None = None, default = '__raise__') -> ExcelTable:
+        if name is None: # Search the name of the table (if there is only one table in the file)
+            for sheet_name in self.pyxl_workbook.sheetnames:
+                pyxl_worksheet: Worksheet = self.pyxl_workbook[sheet_name]
+                for a_name in pyxl_worksheet.tables:
+                    if name is not None:
+                        raise ValueError(f"Several tables found in workbook \"{self.path}\"")
+                    else:
+                        name = a_name
+
+        if name is not None:
+            if name in self.tables:
                 return self.tables[name]
             
+            for sheet_name in self.pyxl_workbook.sheetnames:
+                pyxl_worksheet: Worksheet = self.pyxl_workbook[sheet_name]
+                if name in pyxl_worksheet.tables:
+                    pyxl_table = pyxl_worksheet.tables[name]
+                    self.tables[name] = ExcelTable(pyxl_table, pyxl_worksheet, self)
+                    return self.tables[name]
+
+        # Case when no table is found            
         if default == '__raise__':
-            raise KeyError(f"no table found with name \"{name}\" in workbook \"{self.path}\"")
+            raise KeyError(f"No table found with name \"{name}\" in workbook \"{self.path}\"")
         else:
             return default
         
 
     def create_table(self, name: str, no_headers: bool = False) -> ExcelTable:
         for sheet_name in self.pyxl_workbook.sheetnames:
             pyxl_worksheet: Worksheet = self.pyxl_workbook[sheet_name]
             if name in pyxl_worksheet.tables:
-                raise ValueError(f"table {name} already exist")
+                raise ValueError(f"Table {name} already exist")
     
         self.needs_save = True
         
         if self._create_next_table_in_active_sheet:
             pyxl_worksheet: Worksheet = self.pyxl_workbook.active
             pyxl_worksheet.title = name
             self._create_next_table_in_active_sheet = False
@@ -158,36 +174,36 @@
 
         
     def get_or_create_table(self, name: str, no_headers: bool = False) -> ExcelTable:
         table = self.get_table(name, default=None)
         if table is None:
             table = self.create_table(name, no_headers)
         return table
-    
-    # defined names
+
 
     def get_global_named_values(self, name: str) -> list:
         defn = self.pyxl_workbook.defined_names[name]
         values = []
         
         for title, coord in defn.destinations:
             worksheet = self.pyxl_workbook[title]
             cell = worksheet[coord]
             value = cell.value
             values.append(value)
 
         return values
 
+
     def get_global_named_value(self, name: str) -> Any:
         values = self.get_global_named_values(name)
         
         if len(values) > 1:
-            raise ValueError(f"more than one cell")
+            raise ValueError(f"More than one cell")
         elif len(values) == 0:
-            raise ValueError(f"global name not found")
+            raise ValueError(f"Global name not found")
         else:
             return values[0]
 
 
 class ExcelTable:
     min_row_index: int
     """ 0-base index of the first data row (excluding headers). """
@@ -233,62 +249,62 @@
             if pyxl_table.headerRowCount == 0:
                 self.has_headers = False
                 self.min_row_index = min_row - 1
             elif pyxl_table.headerRowCount == 1:
                 self.has_headers = True
                 self.min_row_index = min_row
             else:
-                raise ValueError(f'invalid headerRowCount: {pyxl_table.headerRowCount}')
+                raise ValueError(f'Invalid headerRowCount: {pyxl_table.headerRowCount}')
             
             self.row_count = max_row - self.min_row_index
             col_count = max_col - self.min_col_index
         
             self.column_names: list[str] = list(self.pyxl_table.column_names)
             # NOTE: if no headers, default names are returned, example in French: ['Colonne1', 'Colonne2']
             if len(self.column_names) != col_count:
-                raise ValueError(f'invalid column_names length ({len(self.column_names)}, expected {col_count}): {self.column_names}')
+                raise ValueError(f'Invalid column_names length ({len(self.column_names)}, expected {col_count}): {self.column_names}')
             
             self._column_indexes = {}
             for i, name in enumerate(self.column_names):                
                 self._column_indexes[name] = i
 
             if self.row_count == 1 and self.is_row_empty(0):
                 self.row_count = 0
         else:
-            raise ValueError(f"invalid type for pyxl_table: {type(pyxl_table).__name__}")
+            raise ValueError(f"Invalid type for pyxl_table: {type(pyxl_table).__name__}")
 
         self._column_formats: list[dict[str,Any]] = None
     
     @property
     def col_count(self) -> int:
         return len(self.column_names)
     
     @property
     def ref(self) -> str:
         if self.col_count == 0:
-            raise ValueError(f"cannot get table ref: table does not contain any column")
+            raise ValueError(f"Cannot get table ref: table does not contain any column")
         if self.row_count == 0:
-            raise ValueError(f"cannot get table ref: table does not contain any row")
+            raise ValueError(f"Cannot get table ref: table does not contain any row")
                 
         return f"{get_column_letter(self.min_col_index + 1)}{self.min_row_index - (1 if self.has_headers else 0) + 1}:{get_column_letter(self.min_col_index + self.col_count)}{self.min_row_index + self.row_count}"
 
 
     def get_row(self, index: int, *, readonly: bool = False) -> ExcelRow:
         """
         Get row at the given 0-base index.
         """
         if index == -1:
             if self.row_count == 0:
-                raise ValueError(f"cannot get last row: table does not contain any row")
+                raise ValueError(f"Cannot get last row: table does not contain any row")
             index = self.row_count - 1
         elif index < 0:
-            raise ValueError(f"invalid row index: {index}")
+            raise ValueError(f"Invalid row index: {index}")
         
         if index >= self.row_count:
-            raise ValueError(f"cannot get row at index {index}: table contains {self.row_count} rows")
+            raise ValueError(f"Cannot get row at index {index}: table contains {self.row_count} rows")
 
         return ExcelRow(self, index, readonly=readonly)
     
 
     def is_row_empty(self, row_index: int):
         for col_index in range(0, self.col_count):
             cell = self.pyxl_worksheet.cell(self.min_row_index + 1 + row_index, self.min_col_index + 1 + col_index)
@@ -308,36 +324,36 @@
     
 
     def insert_row(self) -> ExcelRow:
         self.workbook.needs_save = True
         row_index = self.row_count
 
         if not self.is_row_empty(row_index):
-            raise ValueError(f'cannot insert row: row at index {row_index} is not empty')
+            raise ValueError(f'Cannot insert row: row at index {row_index} is not empty')
 
         self.row_count += 1
 
         # erase old styles and apply column format
         for col_index in range(0, self.col_count):
             self.erase_cell(row_index, col_index)
             
         return self.get_row(row_index)
     
 
     def insert_col(self, name: str):
         self.workbook.needs_save = True
         if not name:
-            raise ValueError(f'name cannot be empty')
+            raise ValueError(f'Name cannot be empty')
         if name in self.column_names:
-            raise ValueError(f'column name already used: {name}')
+            raise ValueError(f'Column name already used: {name}')
             
         col_index = self.col_count
 
         if not self.is_col_empty(col_index):
-            raise ValueError(f'cannot insert column: column {col_index} is not empty')
+            raise ValueError(f'Cannot insert column: column {col_index} is not empty')
 
         self.column_names.append(name) # implies self.col_count += 1
         self._column_indexes[name] = self.col_count - 1
 
         if self.has_headers:
             cell = self.pyxl_worksheet.cell(self.min_row_index, self.min_col_index + 1 + col_index)
             #logger.debug('set column name to cell %s%s: %s', cell.column_letter, cell.row, name)
@@ -365,15 +381,15 @@
         if self.row_count == 0:
             self.insert_row()
 
         new_ref = self.ref
         if self.pyxl_table is not None and new_ref == self.pyxl_table.ref:
             return
         
-        logger.debug("define table %s: %s => %s", self.name, self.pyxl_table.ref if self.pyxl_table is not None else None, new_ref)
+        logger.debug("Define table %s: %s => %s", self.name, self.pyxl_table.ref if self.pyxl_table is not None else None, new_ref)
 
         newcolumns = []
 
         for i in range(0, self.col_count):
             if self.has_headers:
                 name = self.pyxl_worksheet.cell(self.min_row_index, self.min_col_index + 1 + i).value
             else:
@@ -444,17 +460,17 @@
     def _check_indexes(self, row_index: int, col_index: int):
         if row_index == -1:
             row_index = self.row_count - 1
         if col_index == -1:
             col_index = self.col_count - 1
 
         if row_index < 0 or row_index >= self.row_count:
-            raise ValueError(f"invalid row index: {row_index} (row count: {self.row_count})")
+            raise ValueError(f"Invalid row index: {row_index} (row count: {self.row_count})")
         if col_index < 0 or col_index >= self.col_count:
-            raise ValueError(f"invalid row index: {col_index} (row count: {self.col_count})")
+            raise ValueError(f"Invalid row index: {col_index} (row count: {self.col_count})")
 
 
     def erase_cell(self, row_index: int, col_index: int, allow_outside: bool = False):
         """
         Erase the value of the cell located at the given 0-base indices, and apply the default formatting and formulas of the corresponding table column.
         
         If `allow_outside` is set, the cell may be located outside of the table. In this case, no formatting or formula is applied.
@@ -617,21 +633,34 @@
             self._must_refresh[key] = False
             return value
 
         else:
             return self._values[key]
         
 
+    def get(self, key: str, default = None):
+        if key in self.table.column_names:
+            return self[key]
+        else:
+            return default
+           
+
     def __setitem__(self, key: int|str, value):
         if not isinstance(key, int):
+            if not key in self.table._column_indexes:
+                self.table.insert_col(key)
             key = self.table._column_indexes[key]
 
         if self._values is None:
             self._values = [ _UNSET ] * self.table.col_count
             self._must_refresh = {index: True for index in range(0, self.table.col_count)}
+        else:
+            for index in range(len(self._values), key+1):
+                self._values.append(_UNSET)
+                self._must_refresh[index] = True
 
         self._values[key] = value
         if self._must_refresh is not None:
             self._must_refresh[key] = False
         
         if not self.readonly:
             self.table.set_value(self.index, key, value)
```

## zut/files.py

```diff
@@ -323,22 +323,21 @@
         return shutil.copytree(src, dst, symlinks=symlinks, ignore=ignore, ignore_dangling_symlinks=ignore_dangling_symlinks, dirs_exist_ok=dirs_exist_ok)
 
     if not smbclient_shutil:
         raise ModuleNotFoundError(f'missing package `smbprotocol`')
     return smbclient_shutil.copytree(src, dst, symlinks=symlinks, ignore=ignore, ignore_dangling_symlinks=ignore_dangling_symlinks, dirs_exist_ok=dirs_exist_ok)
 
 
-def archivate(path: str|Path, target: str|Path = None, *, missing_ok: bool = False) -> str:
+def archivate(path: str|Path, target: str|Path = None, *, missing_ok: bool = False, keep: bool = False) -> str:
     """
-    Copy `path` to `target` directory, ensuring unique subdir name.
+    Archivate `path` to `target` directory, ensuring unique archive name.
     """
     if isinstance(path, Path):
         path = str(path)
 
-
     if missing_ok:
         if not path or not exists(path):
             return
 
     if isinstance(target, Path):
         target = str(target)
     
@@ -360,8 +359,10 @@
         archive = mainpart + (f"-{i}" if i > 1 else '') + ext
         if not exists(archive):
             break
         i += 1
 
     logger.info(f"Archivate {path} to {archive}")
     copy2(path, archive)
+    if not keep:
+        remove(path)
     return archive
```

## zut/db/base.py

```diff
@@ -29,19 +29,17 @@
     pass
 
 
 logger = logging.getLogger(__name__)
 
 T_Connection = TypeVar('T_Connection')
 T_Cursor = TypeVar('T_Cursor')
-T_Composable = TypeVar('T_Composable')
-T_Composed = TypeVar('T_Composed')
 
 
-class DbAdapter(Generic[T_Connection, T_Cursor, T_Composable, T_Composed]):
+class DbAdapter(Generic[T_Connection, T_Cursor]):
     """
     Base class for database adapters.
     """
     URL_SCHEME: str
     _ALT_SCHEMES: set[str] = set()
     DEFAULT_SCHEMA = None
     ONLY_POSITIONAL_PARAMS = False
@@ -320,42 +318,37 @@
         if limit is not None:
             result += f" LIMIT {limit}"
         if offset is not None:
             result += f" OFFSET {offset}"
         return result
     
 
-    def get_select_table_query(self, table: str|tuple = None, *, schema_only = False) -> T_Composed:
+    def get_select_table_query(self, table: str|tuple = None, *, schema_only = False) -> str:
         """
         Build a query on the given table.
 
         If `schema_only` is given, no row will be returned (this is used to get information on the table).
         Otherwise, all rows will be returned.
 
         The return type of this function depends on the database engine.
         It is passed directly to the cursor's execute function for this engine.
         """
         raise NotImplementedError()
+                
 
+    def escape_identifier(self, value: str) -> str:
+        raise NotImplementedError()
+        
 
-    def _get_composable_param(self, value) -> T_Composable:
+    def escape_literal(self, value) -> str:
         if value is None:
             return "null"
-        elif value == '__now__':
-            return "CURRENT_DATETIME()"
         else:
-            return self.escape_literal(value)
-                
-
-    def escape_identifier(self, value) -> T_Composable:
-        raise NotImplementedError()
-                
-
-    def escape_literal(self, value) -> T_Composable:
-        raise NotImplementedError()
+            return f"'" + str(value).replace("'", "''") + "'"
+    
     
     #endregion
     
 
     #region Execution
 
     def execute_query(self, query: str, params: list|tuple|dict = None, *, cursor: T_Cursor = None, results: bool|Literal['warning']|TextIOWrapper|OutTable|str|Path = False, tz: tzinfo = None, limit: int = None, offset: int = None, query_id: str = None):
@@ -396,15 +389,15 @@
             
             # Handle results
             if results == 'warning':
                 if _cursor.description:
                     rows = [row for row in _cursor]                    
                     row_count = len(rows)
                     if row_count > 0:
-                        columns = self.get_cursor_column_names(_cursor)
+                        columns = self.get_columns(_cursor)
 
                         if tabulate:
                             text_rows = tabulate(rows[0:10], headers=columns)
                         else:
                             fp = StringIO()
                             with out_table(fp, headers=columns) as o:
                                 for row in rows[0:10]:
@@ -414,15 +407,15 @@
                         if row_count > 10:
                             text_rows += "\n…"
                         logger.warning("query%s returned %d row%s:\n%s", f" {query_id}" if query_id else "", row_count, "s" if row_count > 1 else "", text_rows)
                 return None
             
             elif isinstance(results, (OutTable,IOBase,str,Path)):
                 # Write results as CSV to the given stream
-                columns = self.get_cursor_column_names(_cursor)
+                columns = self.get_columns(_cursor)
 
                 if isinstance(results, OutTable):
                     o = results
                     o.headers = columns
                 else:
                     o = out_table(results, headers=columns, title=False, tablefmt='csv')
                 
@@ -431,15 +424,15 @@
                         o.append(format_row(row))
                     
                     o.file.seek(0)
                     return columns, o.row_count
 
             elif results:
                 # Return results as a dict list
-                columns = self.get_cursor_column_names(_cursor)
+                columns = self.get_columns(_cursor)
                 return [{columns[i]: value for i, value in enumerate(format_row(row))} for row in _cursor]
             
             else:
                 return None
 
 
     def _log_execute_messages(self, cursor: T_Cursor):
@@ -507,28 +500,29 @@
 
             try:
                 next(iterator)
                 raise SeveralFoundError()
             except StopIteration:
                 pass
 
-            columns = self.get_cursor_column_names(cursor)
+            columns = self.get_columns(cursor)
             return {columns[i]: value for i, value in enumerate(row)}
     
 
+    # TODO: default of execute_query()?
     def get_result(self, query: str, params: list|tuple|dict = None, *, limit: int = None, offset: int = None):
         cursor = self.cursor()
         self.execute_query(query, params, limit=limit, offset=offset, cursor=cursor)
         return CursorResult(self, cursor)
     
 
     def iter_dicts(self, query: str, params: list|tuple|dict = None, *, limit: int = None, offset: int = None):        
         with self.cursor() as cursor:
             self.execute_query(query, params, limit=limit, offset=offset, cursor=cursor)
-            columns = self.get_cursor_column_names(cursor)
+            columns = self.get_columns(cursor)
             for row in cursor:
                 yield {columns[i]: value for i, value in enumerate(row)}
                 
     
     def get_dicts(self, query: str, params: list|tuple|dict = None, *, limit: int = None, offset: int = None):        
         return [row for row in self.iter_dicts(query, params, limit=limit, offset=offset)]
     
@@ -561,89 +555,42 @@
         except ValueError:
             schema = self.DEFAULT_SCHEMA
             name = name
 
         return (schema, name)
     
 
-    def schema_exists(self, schema: str) -> bool:
-        raise NotImplementedError()
-    
-
-    def create_schema(self, schema: str):
-        raise NotImplementedError()
-    
-
-    def drop_schema(self, schema: str, cascade: bool = False):
-        raise NotImplementedError()
-    
-
     def table_exists(self, table: str|tuple = None) -> bool:
         raise NotImplementedError()
 
 
-    def get_cursor_column_names(self, cursor: T_Cursor) -> list[str]:
-        if not cursor.description:
-            raise ValueError("No cursor description available")
-        return [info[0] for info in cursor.description]
-
-
-    def get_cursor_columns(self, cursor: T_Cursor) -> list[ColumnInfo]:
-        if not cursor.description:
-            raise ValueError("No cursor description available")
-        return [ColumnInfo(self, cursor, index) for index in range(len(cursor.description))]
-        
-
-    def get_table_column_names(self, table: str|tuple = None) -> list[str]:
-        query = self.get_select_table_query(table, schema_only=True)
-        with self.cursor() as cursor:
-            self.execute_query(query, cursor=cursor)
-            return self.get_cursor_column_names(cursor)
-        
-
-    def get_table_columns(self, table: str|tuple = None) -> list[ColumnInfo]:
-        query = self.get_select_table_query(table, schema_only=True)
-        with self.cursor() as cursor:
-            self.execute_query(query, cursor=cursor)
-            return self.get_cursor_columns(cursor)
-        
-
-    def _update_column_info(self, info: ColumnInfo, cursor: T_Cursor, index: int):
-        info.name = cursor.description[index][0]
-    
-
-    def drop_table(self, table: str|tuple = None):
-        schema, table = self.split_name(table)
-        
-        query = "DROP TABLE "
-            
-        if schema:    
-            query += f"{self.escape_identifier(schema)}."
-        query += f"{self.escape_identifier(table)}"
-
-        self.execute_query(query)
+    def get_columns(self, table_or_cursor: str|tuple|T_Cursor = None) -> list[str]:
+        if table_or_cursor is None or isinstance(table_or_cursor, (str,tuple)):
+            # table_or_cursor is assumed to be a table name (use self.table if None) 
+            query = self.get_select_table_query(table_or_cursor, schema_only=True)
+            with self.cursor() as cursor:
+                self.execute_query(query, cursor=cursor)
+                return self.get_columns(cursor)
+        else:
+            # table_or_cursor is assumed to be a cursor
+            if not table_or_cursor.description:
+                raise ValueError("No cursor description available")
+            return [info[0] for info in table_or_cursor.description]
 
 
-    def truncate_table(self, table: str|tuple = None, *, cascade: bool = False):
+    def truncate_table(self, table: str|tuple = None):
         schema, table = self.split_name(table)
         
         query = "TRUNCATE TABLE "
             
         if schema:    
             query += f"{self.escape_identifier(schema)}."
         query += f"{self.escape_identifier(table)}"
 
-        if cascade:
-            query += " CASCADE"
-
         self.execute_query(query)
-
-
-    def load_from_csv(self, file: os.PathLike|IOBase, table: str|tuple = None, *, columns: list[str] = None, encoding: str = 'utf-8', merge: Literal['truncate', 'truncate-cascade', 'upsert'] = None, noheaders: bool = False, csv_delimiter: str = None, csv_quotechar: str = None, csv_nullval: str = None) -> int:
-        raise NotImplementedError()
    
 
     # endregion
 
 
 def _get_connection_from_wrapper(origin):    
     if type(origin).__module__.startswith(('django.db.backends.', 'django.utils.connection')):
@@ -652,34 +599,18 @@
         return origin.connection()
     elif type(origin).__module__.startswith(('psycopg2.pool',)):
         return origin.getconn()
     else:
         return origin
 
 
-class ColumnInfo:
-    def __init__(self, db: DbAdapter, cursor: T_Cursor, index: int):
-        self.name = None
-        self.python_type: type = None
-        self.sql_type: str = None
-        self.sql_typecode: int = None
-        self.nullable: bool = None
-        db._update_column_info(self, cursor, index)
-
-    def __str__(self):
-        return self.name
-    
-    def __repr__(self):
-        return self.name
-
-
 class CursorResult(Generic[T_Cursor]):
     def __init__(self, db: DbAdapter, cursor: T_Cursor):
         self.cursor = cursor
-        self.columns = db.get_cursor_column_names(cursor)
+        self.columns = db.get_columns(cursor)
         self._column_indexes: dict[str, int] = None
 
     def __enter__(self):
         return self
     
     def __exit__(self, exc_type = None, exc_val = None, exc_tb = None):
         self.close()
```

## zut/db/mssql.py

```diff
@@ -5,24 +5,24 @@
 import re
 from contextlib import nullcontext
 from datetime import tzinfo
 from io import IOBase, TextIOWrapper
 from pathlib import Path
 from urllib.parse import unquote, urlparse
 
-from .. import OutTable, Literal, build_url, skip_utf8_bom, _get_csv_params
-from .base import ColumnInfo, DbAdapter
+from .. import OutTable, build_url, skip_utf8_bom
+from .base import DbAdapter
 
 logger = logging.getLogger(__name__)
 notice_logger = logging.getLogger("mssql")
 
 try:
     from pyodbc import Connection, Cursor, connect, drivers
 
-    class MssqlAdapter(DbAdapter[Connection, Cursor, str, str]):
+    class MssqlAdapter(DbAdapter[Connection, Cursor]):
         """
         Database adapter for Microsoft SQL Server (using `pyodbc` driver).
         """
         URL_SCHEME = 'mssql' # or mssqls (if encrypted)
         DEFAULT_SCHEMA = 'dbo'
         ONLY_POSITIONAL_PARAMS = True
         EXPECTED_CONNECTION_TYPES = ['pyodbc.Connection']
@@ -68,18 +68,14 @@
 
         def _get_url_from_connection(self):
             with self.cursor() as cursor:
                 cursor.execute("SELECT @@SERVERNAME, local_tcp_port, SUSER_NAME(), DB_NAME() FROM sys.dm_exec_connections WHERE session_id = @@spid")
                 host, port, user, dbname = next(iter(cursor))
             return build_url(scheme=self.URL_SCHEME, username=user, hostname=host, port=port, path='/'+dbname)
         
-
-        # -------------------------------------------------------------------------
-        # Execution
-        #
         
         def execute_file(self, path: str|Path, params: list|tuple|dict = None, *, cursor: Cursor = None, results: bool|TextIOWrapper|OutTable|str|Path = False, tz: tzinfo = None, limit: int = None, offset: int = None, encoding: str = 'utf-8') -> None:
             import sqlparse  # not at the top because the enduser might not need this feature
 
             # Read file
             with open(path, 'r', encoding=encoding) as fp:
                 skip_utf8_bom(fp)
@@ -104,18 +100,14 @@
                         self.execute_query(query, params, cursor=_cursor, results='warning', tz=tz, query_id=query_id, limit=limit, offset=offset)
 
                     else:
                         # Last query
                         return self.execute_query(query, params, cursor=_cursor, results=results, tz=tz, query_id=query_id, limit=limit, offset=offset)
 
 
-        # -------------------------------------------------------------------------
-        # Queries
-        #
-            
         def _paginate_parsed_query(self, selectpart: str, orderpart: str, *, limit: int|None, offset: int|None) -> str:
             if orderpart:
                 result = f"{selectpart} {orderpart} OFFSET {offset or 0} ROWS"
                 if limit is not None:
                     result += f" FETCH NEXT {limit} ROWS ONLY"
                 return result
             elif limit is not None:
@@ -132,20 +124,18 @@
             query = f'SELECT * FROM {self.escape_identifier(schema)}.{self.escape_identifier(table)}'
             if schema_only:
                 query += ' WHERE 1 = 0'
 
             return query
             
 
-        def escape_identifier(self, value: str) -> str:
+        def escape_identifier(self, value: str):
+            if not isinstance(value, str):
+                raise TypeError(f"Invalid identifier: {value} (type: {type(value)})")
             return f"[{value.replace(']', ']]')}]"
-        
-
-        def escape_literal(self, value: str) -> str:
-            return f"'" + value.replace("'", "''") + "'"
 
 
         def _log_execute_messages(self, cursor: Cursor):
             if cursor.messages:
                 for msg_type, msg_text in cursor.messages:
                     m = re.match(r"^\[Microsoft\]\[ODBC Driver \d+ for SQL Server\]\[SQL Server\](.+)$", msg_text)
                     if m:
@@ -158,103 +148,25 @@
                         if msg_type == "[01003] (8153)": # Avertissement : la valeur NULL est éliminée par un agrégat ou par une autre opération SET.
                             level = logging.INFO
                         else:
                             level = logging.WARNING
 
                     notice_logger.log(level, f"{msg_text}")
 
-        # -------------------------------------------------------------------------
-        # Tables and columns
-        #    
 
         def table_exists(self, table: str|tuple = None) -> bool:        
             schema, table = self.split_name(table)
 
             query = "SELECT CASE WHEN EXISTS(SELECT 1 FROM information_schema.tables WHERE table_schema = ? AND table_name = ?) THEN 1 ELSE 0 END"
             params = [schema, table]
 
             return self.get_scalar(query, params) == 1
 
-            
-        def truncate_table(self, table: str|tuple = None, *, cascade: bool = False):
-            if cascade:
-                raise ValueError("Cascade truncate is not supported by mssql.")
-            super().truncate_table(table)
-            
-
-        def _update_column_info(self, info: ColumnInfo, cursor: Cursor, index: int):
-            info.name, info.python_type, display_size, internal_size, precision, scale, info.nullable = cursor.description[index]
-
-        #endregion
-
-
-        def load_from_csv(self, file: os.PathLike, table: str|tuple = None, *, columns: list[str] = None, encoding: str = 'utf-8', merge: Literal['truncate', 'truncate-cascade', 'upsert'] = None, noheaders: bool = False, csv_delimiter: str = None, csv_quotechar: str = None, csv_nullval: str = None) -> int:
-            if isinstance(file, IOBase):
-                # TODO: use named pipes?
-                raise NotImplementedError("Cannot use IOBase file with mssql.")
-            if columns or not noheaders:
-                # TODO: compare CSV headers with columns (check consistency) + use named pipes?
-                raise NotImplementedError("Arguments 'columns' or 'noheaders' cannot be used yet.")
-
-            sche, tab = self.split_name(table)
-            tmp_tab: str = None
-            key_columns: list[str] = []
-            nonkey_target_columns: list[str] = []
-
-            _, csv_delimiter, csv_quotechar, csv_nullval = _get_csv_params(None, csv_delimiter, csv_quotechar, csv_nullval, context=file)
-            if csv_nullval != '':
-                raise ValueError(f"Invalid csv nullval for mssql: \"{csv_nullval}\"")
-
-            try:
-                if merge in ['truncate', 'truncate-cascade']:                
-                    self.truncate_table((sche, tab), cascade=merge == 'truncate-cascade')
-
-                elif merge == 'upsert':
-                    raise NotImplementedError("Cannot use 'upsert' yet") #TODO
-
-                # Prepare actual copy operation
-                sql = f"BULK INSERT "
-                    
-                if tmp_tab:
-                    sql += f"{self.escape_identifier(tmp_tab)}"
-                else:    
-                    if sche:    
-                        sql +=f"{self.escape_identifier(sche)}."
-                    sql += f"{self.escape_identifier(tab)}"
-
-                sql += f" FROM {self.escape_literal(os.path.abspath(file))}"
-                sql += f' WITH ('
-                sql += f' CODEPAGE = {self.escape_literal('utf-8' if encoding == 'utf-8-sig' else encoding)}'
-                sql += f', FIELDTERMINATOR = {self.escape_literal(csv_delimiter)}'
-                sql += f', FIELDQUOTE = {self.escape_literal(csv_quotechar)}'
-                if csv_nullval == '':
-                    sql += f', KEEPNULLS'
-                sql += ")"
-
-                if tmp_tab:
-                    logger.debug("Actual copy from %s to %s", file, tmp_tab)
-                
-                #TODO: skip_utf8_bom(fp)
-                with self.cursor() as cursor:
-                    self.execute_query(sql)
-                    result_count = cursor.rowcount
-                
-                # Upsert from tmp table if necessary
-                if tmp_tab:
-                    pass #TODO
-
-                return result_count
-
-            finally:
-                if tmp_tab:
-                    self.execute_query(f"DROP TABLE IF EXISTS {self.escape_identifier(tmp_tab)}")
-
-
 
-except ImportError:  
+except ImportError:
 
     class MssqlAdapter(DbAdapter):
         """
         Database adapter for Microsoft SQL Server (using `pyodbc` driver).
         """
                 
         URL_SCHEME = 'mssql' # or mssqls (if encrypted)
```

## zut/db/mysql.py

```diff
@@ -1,33 +1,24 @@
 from __future__ import annotations
 
-from decimal import Decimal
 import logging
-import os
-import re
-from contextlib import nullcontext
-from datetime import date, datetime, timedelta, tzinfo
-from io import IOBase, TextIOWrapper
-from pathlib import Path
-from urllib.parse import unquote, urlparse
+from urllib.parse import urlparse
 
-from .. import OutTable, Literal, build_url, skip_utf8_bom, _get_csv_params
-from .base import ColumnInfo, DbAdapter
+from .base import DbAdapter
 
 logger = logging.getLogger(__name__)
 notice_logger = logging.getLogger("mysql")
 
 try:
     from MySQLdb import connect
     from MySQLdb.connections import Connection
     from MySQLdb.cursors import Cursor
-    from MySQLdb.constants import FIELD_TYPE
 
     # TODO: cursor/procedure messages (_log_execute_messages?)
-    class MysqlAdapter(DbAdapter[Connection, Cursor, str, str]):
+    class MysqlAdapter(DbAdapter[Connection, Cursor]):
         """
         Database adapter for Microsoft SQL Server (using `pyodbc` driver).
         """
         URL_SCHEME = 'mysql'
         EXPECTED_CONNECTION_TYPES = ['MySQLdb.connections.Connection'] # Compatible with the Python DB API interface version 2 (not "_mysql.connection")
 
         @classmethod
@@ -51,41 +42,31 @@
             return connect(**kwargs, sql_mode='STRICT_ALL_TABLES', autocommit=self.autocommit)
 
 
         def _get_url_from_connection(self):
             raise NotImplementedError() # TODO
         
 
-        # -------------------------------------------------------------------------
-        # Queries
-        #
-
         def get_select_table_query(self, table: str|tuple = None, *, schema_only = False) -> str:
             _, table = self.split_name(table)
             
             query = f'SELECT * FROM {self.escape_identifier(table)}'
             if schema_only:
                 query += ' WHERE 1 = 0'
 
             return query
             
 
-        def escape_identifier(self, value: str) -> str:
+        def escape_identifier(self, value: str):
+            if not isinstance(value, str):
+                raise TypeError(f"Invalid identifier: {value} (type: {type(value)})")
             if '`' in value:
-                raise ValueError(f"Identifier cannot contain back ticks.")
+                raise ValueError(f"Identifier cannot contain back ticks")
             return f"`" + value + "`"
-        
-
-        def escape_literal(self, value: str) -> str:
-            return f"'" + value.replace("'", "''") + "'"
 
-
-        # -------------------------------------------------------------------------
-        # Tables and columns
-        #    
     
         def split_name(self, name: str|tuple = None) -> tuple[str,str]:
             schema, name = super().split_name(name)
             if schema is not None:
                 raise ValueError(f"Cannot use schema (\"{schema}\") with mysql.")
             return None, name
 
@@ -93,115 +74,15 @@
         def table_exists(self, table: str|tuple = None) -> bool:        
             _, table = self.split_name(table)
 
             query = "SELECT EXISTS(SELECT 1 FROM information_schema.tables WHERE table_name = %s)"
             params = [table]
 
             return self.get_scalar(query, params) == 1
-
-            
-        def truncate_table(self, table: str|tuple = None, *, cascade: bool = False):
-            if cascade:
-                raise ValueError("Cascade truncate is not supported by mssql.")
-            super().truncate_table(table)
-            
-
-        def _update_column_info(self, info: ColumnInfo, cursor: Cursor, index: int):
-            info.name, info.sql_typecode, _display_size, _internal_size, _precision, _scale, nullok = cursor.description[index]
-
-            info.nullable = nullok == 1
-            
-            if info.sql_typecode == FIELD_TYPE.TINY:
-                info.sql_type = 'TINY'
-            elif info.sql_typecode == FIELD_TYPE.ENUM:
-                info.sql_type = 'ENUM'
-            else:
-                for name in dir(FIELD_TYPE):
-                    if name.startswith('_'):
-                        continue
-                    code = getattr(FIELD_TYPE, name)
-                    if code == info.sql_typecode:
-                        info.sql_type = name
-                        break
-            
-            info.python_type = PYTHON_TYPES.get(info.sql_typecode)
-
-
-        def load_from_csv(self, file: os.PathLike|IOBase, table: str|tuple = None, *, columns: list[str] = None, encoding: str = 'utf-8', merge: Literal['truncate', 'truncate-cascade', 'upsert'] = None, noheaders: bool = False, csv_delimiter: str = None, csv_quotechar: str = None, csv_nullval: str = None) -> int:
-            if isinstance(file, IOBase):
-                # TODO: use named pipes?
-                raise NotImplementedError("Cannot use IOBase file with mssql.")
-            
-            # TODO: end-of-line of CSV input should be verified. Windows end-of-lines does not work as of now.
-            # (e.g. on Windows, tests/samples/mixed-mysql.csv is forced to LF. If not, "test_load_csv_ordered" results in last column being 0 instead of NULL, and "test_load_csv_upsert" fails)
-
-            _, tab = self.split_name(table)
-            _, csv_delimiter, csv_quotechar, csv_nullval = _get_csv_params(None, csv_delimiter, csv_quotechar, csv_nullval, context=file)
-
-            if merge in ['truncate', 'truncate-cascade']:                
-                self.truncate_table((None, tab), cascade=merge == 'truncate-cascade')
-
-            sql = f"LOAD DATA LOCAL INFILE {self.escape_literal(str(os.path.abspath(file)).replace('\\', '\\\\'))}"
-            if merge == 'upsert':
-                sql += " REPLACE"
-            sql += f" INTO TABLE {self.escape_identifier(tab)}"
-
-            sql += f' CHARACTER SET {self.escape_literal('utf8' if encoding in ['utf-8', 'utf-8-sig'] else encoding)}'
-            sql += f' FIELDS TERMINATED BY {self.escape_literal(csv_delimiter)}'
-            sql += f' ENCLOSED BY {self.escape_literal(csv_quotechar)}'
-            sql += f' ESCAPED BY {self.escape_literal(csv_quotechar)}'
-            #TODO: csv_nullval handling?
             
-            if not noheaders:
-                #TODO: check that file headers match given columns
-                sql += " IGNORE 1 LINES"
-            
-            if columns:
-                sql += " ("
-                for i, colinfo in enumerate(columns):
-                    sql += (", " if i > 0 else "") + f"{self.escape_identifier(colinfo)}"
-                sql += ")"
-            
-            #TODO skip_utf8_bom(fp)
-            with self.cursor() as cursor:
-                self.execute_query(sql)
-                result_count = cursor.rowcount
-            
-            return result_count
-
-
-    PYTHON_TYPES = {
-        FIELD_TYPE.DECIMAL: Decimal,
-        FIELD_TYPE.TINY: int,
-        FIELD_TYPE.SHORT: int,
-        FIELD_TYPE.LONG: int,
-        FIELD_TYPE.FLOAT: float,
-        FIELD_TYPE.DOUBLE: float,
-        FIELD_TYPE.NULL: None,
-        FIELD_TYPE.TIMESTAMP: datetime,
-        FIELD_TYPE.LONGLONG: int,
-        FIELD_TYPE.INT24: int,
-        FIELD_TYPE.DATE: date,
-        FIELD_TYPE.TIME: timedelta,
-        FIELD_TYPE.DATETIME: datetime,
-        FIELD_TYPE.YEAR: int,
-        FIELD_TYPE.VARCHAR: str,
-        FIELD_TYPE.BIT: bytes,
-        FIELD_TYPE.JSON: None,
-        FIELD_TYPE.NEWDECIMAL: Decimal,
-        FIELD_TYPE.ENUM: None,
-        FIELD_TYPE.SET: None,
-        FIELD_TYPE.TINY_BLOB: str,
-        FIELD_TYPE.MEDIUM_BLOB: str,
-        FIELD_TYPE.LONG_BLOB: str,
-        FIELD_TYPE.BLOB: str,
-        FIELD_TYPE.VAR_STRING: str,
-        FIELD_TYPE.STRING: str,
-        FIELD_TYPE.GEOMETRY: None,
-    }
 
 except ImportError:  
 
     class MysqlAdapter(DbAdapter):
         """
         Database adapter for Microsoft SQL Server (using `pyodbc` driver).
         """
```

## zut/db/pg.py

```diff
@@ -1,22 +1,16 @@
 from __future__ import annotations
 
 import logging
-import os
 import re
 from contextlib import nullcontext
-from datetime import date, datetime, time
-from decimal import Decimal
-from io import IOBase
-from secrets import token_hex
 from typing import Any
-from uuid import UUID
 
-from .. import Literal, build_url, skip_utf8_bom, _get_csv_params
-from .base import ColumnInfo, DbAdapter, T_Connection, T_Cursor, T_Composable, T_Composed
+from .. import build_url
+from .base import DbAdapter, T_Connection, T_Cursor
 
 logger = logging.getLogger(__name__)
 
 
 def pg_notice_handler(diag: Diagnostic, logger: logging.Logger = None):
     """
     Handler required by psycopg 3 `connection.add_notice_handler()`.
@@ -57,57 +51,15 @@
         return logging.ERROR
     elif severity_nonlocalized in 'PANIC': # sent to client
         return logging.CRITICAL
     else:
         return logging.ERROR
 
 
-OID_CATALOG = {
-    16: ('bool', bool),
-    17: ('bytea', bytes),
-    18: ('char', str),
-    19: ('name', str),
-    20: ('int8', int),
-    21: ('int2', int),
-    23: ('int4', int),
-    25: ('text', str),
-    26: ('oid', int),
-    114: ('json', None),
-    650: ('cidr', None),
-    700: ('float4', float),
-    701: ('float8', float),
-    869: ('inet', None),
-    1042: ('bpchar', str),
-    1043: ('varchar', str),
-    1082: ('date', date),
-    1083: ('time', time),
-    1114: ('timestamp', datetime),
-    1184: ('timestamptz', datetime),
-    1186: ('interval', None),
-    1266: ('timetz', time),
-    1700: ('numeric', Decimal),
-    2249: ('record', None),
-    2950: ('uuid', UUID),
-    3802: ('jsonb', None),
-    3904: ('int4range', None),
-    3906: ('numrange', None),
-    3908: ('tsrange', None),
-    3910: ('tstzrange', None),
-    3912: ('daterange', None),
-    3926: ('int8range', None),
-    4451: ('int4multirange', None),
-    4532: ('nummultirange', None),
-    4533: ('tsmultirange', None),
-    4534: ('tstzmultirange', None),
-    4535: ('datemultirange', None),
-    4536: ('int8multirange', None),
-}
-
-
-class BasePgAdapter(DbAdapter[T_Connection, T_Cursor, T_Composable, T_Composed]):
+class BasePgAdapter(DbAdapter[T_Connection, T_Cursor]):
     """
     Base class for PostgreSql database adapters (:class:`PgAdapter` using `psycopg` (v3) driver or :class:`Pg2Adapter` using `psycopg2` driver).
     """
     URL_SCHEME = 'postgresql' # See: https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-CONNSTRING
     _ALT_SCHEMES = {'pg', 'postgres'}
     DEFAULT_SCHEMA = 'public'    
     EXPECTED_CONNECTION_TYPES = ['psycopg.Connection']
@@ -120,59 +72,53 @@
     
     def _get_url_from_connection(self):
         with self.cursor() as cursor:
             cursor.execute("SELECT session_user, inet_server_addr(), inet_server_port(), current_database()")
             user, host, port, dbname = next(iter(cursor))
         return build_url(scheme=self.URL_SCHEME, username=user, hostname=host, port=port, path='/'+dbname)
 
-
-    #region Execute utils
     
     def execute_procedure(self, name: str|tuple, *args):
         schema, name = self.split_name(name)
         
         query = "CALL "
         params = []
             
         if schema:    
             query +="{}."
-            params += [self.escape_identifier(schema)]
+            params += [self._sql.Identifier(schema)]
 
         query += "{}"
-        params += [self.escape_identifier(name)]
+        params += [self._sql.Identifier(name)]
 
         query += "(" + ", ".join(['{}'] * len(args)) + ")"
         params += [self._get_composable_param(arg) for arg in args]
 
         with self.cursor() as cursor:
             with self.register_notice_handler(if_exists=None, logprefix=f"pg:{schema + '.' if schema and schema != self.DEFAULT_SCHEMA else ''}{name}"):
                 cursor.execute(self._sql.SQL(query).format(*params))
                 return cursor
             
 
     def register_notice_handler(self, if_exists = '__raise__', logprefix = 'pg'):
         raise NotImplementedError()
     
-    #endregion
-
-
-    #region Queries
     
     def get_select_table_query(self, table: str|tuple = None, *, schema_only = False):
         schema, table = self.split_name(table)
 
         query = "SELECT * FROM "
         params = []
             
         if schema:    
             query +="{}."
-            params += [self.escape_identifier(schema)]
+            params += [self._sql.Identifier(schema)]
 
         query += "{}"
-        params += [self.escape_identifier(table)]
+        params += [self._sql.Identifier(table)]
         
         if schema_only:
             query += ' WHERE false'
 
         return self._sql.SQL(query).format(*params)
 
 
@@ -180,273 +126,40 @@
         if value is None:
             return self._sql.SQL("null")
         elif value == '__now__':
             return self._sql.SQL("NOW()")
         elif isinstance(value, self._sql.Composable):
             return value
         else:
-            return self.escape_literal(value)
+            return self._sql.Literal(value)
         
 
-    def escape_identifier(self, value):
-        return self._sql.Identifier(value)
-    
-
-    def escape_literal(self, value):
-        return self._sql.Literal(value)
-    
-    #endregion
-    
-
-    #region Schemas, tables and columns  
-
-    def schema_exists(self, schema: str) -> bool:
-        query = "SELECT EXISTS (SELECT FROM pg_namespace WHERE nspname = %s)"
-        params = [schema]
-
-        return self.get_scalar(query, params)
-    
-
-    def create_schema(self, schema: str):
-        query = "CREATE SCHEMA {}"
-        params = [self._sql.Identifier(schema)]
-
-        return self.execute_query(self._sql.SQL(query).format(*params))
-    
-
-    def drop_schema(self, schema: str, cascade: bool = False):
-        query = "DROP SCHEMA {}"
-        params = [self._sql.Identifier(schema)]
-
-        if cascade:
-            query += " CASCADE"
-
-        return self.execute_query(self._sql.SQL(query).format(*params))
+    def escape_identifier(self, value: str):
+        if not isinstance(value, str):
+            raise TypeError(f"Invalid identifier: {value} (type: {type(value)})")
+        if '"' in value:
+            raise ValueError(f"Identifier cannot contain double quotes")
+        return '"' + value + '"'
     
 
     def table_exists(self, table: str|tuple = None) -> bool:
         schema, table = self.split_name(table)
 
         query = "SELECT EXISTS (SELECT FROM pg_tables WHERE schemaname = %s AND tablename = %s)"
         params = [schema, table]
 
         return self.get_scalar(query, params)
-    
-
-    def drop_table(self, table: str|tuple = None):
-        schema, table = self.split_name(table)
-        
-        query = "DROP TABLE "
-        params = []
-            
-        if schema:    
-            query +="{}."
-            params += [self.escape_identifier(schema)]
-
-        query += "{}"
-        params += [self.escape_identifier(table)]
-
-        self.execute_query(self._sql.SQL(query).format(*params))
-        
-
-    def truncate_table(self, table: str|tuple = None, *, cascade: bool = False):
-        schema, table = self.split_name(table)
-        
-        query = "TRUNCATE TABLE "
-        params = []
-            
-        if schema:    
-            query +="{}."
-            params += [self.escape_identifier(schema)]
-
-        query += "{}"
-        params += [self.escape_identifier(table)]
-
-        if cascade:
-            query += " CASCADE"
-
-        self.execute_query(self._sql.SQL(query).format(*params))
-
-
-    def _update_column_info(self, info: ColumnInfo, cursor, index: int):
-        info.name, info.sql_typecode, _display_size, _internal_size, _precision, _scale, _nullok_alwaysnone = cursor.description[index]
-        type_info = OID_CATALOG.get(info.sql_typecode)
-        if type_info:
-            info.sql_type, info.python_type = type_info
-    
-    #endregion
-
-
-    #region Copy
-
-    def load_from_csv(self, file: os.PathLike|IOBase, table: str|tuple = None, *, columns: list[str] = None, encoding: str = 'utf-8', merge: Literal['truncate', 'truncate-cascade', 'upsert'] = None, noheaders: bool = False, csv_delimiter: str = None, csv_quotechar: str = None, csv_nullval: str = None) -> int:
-        sche, tab = self.split_name(table)
-        tmp_tab: str = None
-        key_columns: list[str] = []
-        nonkey_target_columns: list[str] = []
-
-        _, csv_delimiter, csv_quotechar, csv_nullval = _get_csv_params(None, csv_delimiter, csv_quotechar, csv_nullval, context=file)
-
-        try:
-            if merge in ['truncate', 'truncate-cascade']:                
-                self.truncate_table((sche, tab), cascade=merge == 'truncate-cascade')
-
-            elif merge == 'upsert':
-                with self.cursor() as cursor:
-                    # Retrieve information about the columns
-                    sql = """
-                    WITH pk_columns AS (
-                        SELECT c.column_name
-                        FROM information_schema.table_constraints tc 
-                        LEFT OUTER JOIN information_schema.constraint_column_usage AS ccu USING (constraint_schema, constraint_name) 
-                        LEFT OUTER JOIN information_schema.columns AS c ON c.table_schema = tc.constraint_schema AND tc.table_name = c.table_name AND ccu.column_name = c.column_name
-                        WHERE tc.constraint_type = 'PRIMARY KEY' AND tc.constraint_schema = %(schema)s and tc.table_name = %(table)s
-                    )
-                    SELECT
-                        c.ordinal_position AS position
-                        ,c.column_name AS name
-                        ,c.udt_name AS sql_type
-                        ,c.is_nullable = 'YES' AS is_nullable
-                        ,p.column_name IS NOT NULL AS is_primary_key
-                    FROM information_schema.columns c
-                    LEFT OUTER JOIN pk_columns p ON p.column_name = c.column_name
-                    WHERE table_schema = %(schema)s AND table_name = %(table)s
-                    """
-                    logger.debug("Retrieve %s.%s columns", sche, tab)
-                    target_colinfos = self.execute_query(sql, {'schema': sche, 'table': tab}, cursor=cursor, results=True)
-
-                    # Build a temporary table
-                    tmp_tab = f"tmp_{tab}_{token_hex(4)}"
-                    params = []                
-                    sql = "CREATE TEMPORARY TABLE {} ("; params += [self._sql.Identifier(tmp_tab)]
-                    pk = []
-                    target_colnames = set()
-
-                    for i, colinfo in enumerate(target_colinfos):
-                        name = colinfo['name']
-                        
-                        is_primary_key = colinfo['is_primary_key']
-                        if columns and not name in columns:
-                            if is_primary_key:
-                                raise ValueError(f"Primary key column '{name}' must be included in the list of copied columns")
-                            continue
-
-                        sql += ("," if i > 0 else " ") + "{} {} {}"; params += [self._sql.Identifier(name), self._sql.Identifier(colinfo['sql_type']), self._sql.SQL('NULL' if colinfo['is_nullable'] else 'NOT NULL')]
-                        target_colnames.add(name)
-                        if is_primary_key:
-                            pk.append(name)
-                            key_columns.append(name)
-                        else:
-                            nonkey_target_columns.append(name)
-
-                    # Additional columns if any ('COPY FROM' cannot discard some columns so we have to import them anyway)
-                    if columns:
-                        for name in columns:
-                            if not name in target_colnames:
-                                sql += ',{} text NULL'; params += [self._sql.Identifier(name)]
-                    
-                    if pk:
-                        sql += ", PRIMARY KEY ("
-                        for i, name in enumerate(pk):
-                            sql += (", " if i > 0 else " ") + "{}"; params += [self._sql.Identifier(name)]
-                        sql += ")"
-                    
-                    sql += ")"
-                    
-                    if logger.isEnabledFor(logging.DEBUG):
-                        logger.debug("columns (for COPY operation): %s", columns)
-                        logger.debug("key_columns: %s", key_columns)
-                        logger.debug("nonkey_target_columns: %s", nonkey_target_columns)
-
-                    logger.debug("Create temp table %s", tmp_tab)
-                    self.execute_query(self._sql.SQL(sql).format(*params), cursor=cursor)
-
-            # Prepare actual copy operation
-            sql = "COPY "; params = []
-                
-            if tmp_tab:
-                sql += "{}"; params += [self.escape_identifier(tmp_tab)]
-            else:    
-                if sche:    
-                    sql +="{}."; params += [self.escape_identifier(sche)]
-                sql += "{}"; params += [self.escape_identifier(tab)]
-
-            if columns:
-                sql += " ("
-                for i, colinfo in enumerate(columns):
-                    sql += (", " if i > 0 else "") + "{}"; params += [self.escape_identifier(colinfo)]
-                sql += ")"
-
-            sql += " FROM STDIN (FORMAT csv"
-            sql += ', ENCODING {}'; params.append('utf-8' if encoding == 'utf-8-sig' else self.escape_literal(encoding))
-            sql += ', DELIMITER {}'; params.append(self.escape_literal(csv_delimiter))
-            sql += ', QUOTE {}'; params.append(self.escape_literal(csv_quotechar))            
-            sql += ', ESCAPE {}'; params.append(self.escape_literal(csv_quotechar))
-            sql += ', NULL {}'; params.append(self.escape_literal(csv_nullval))
-                
-            if not noheaders:
-                sql += ", HEADER match"
-            sql += ")"
-
-            with nullcontext(file) if isinstance(file, IOBase) else open(file, "rb") as fp:
-                skip_utf8_bom(fp)
-                if tmp_tab:
-                    logger.debug("Actual copy from %s to %s", file, tmp_tab)
-                result_count = self._actual_copy(self._sql.SQL(sql).format(*params), fp)
-            
-            # Upsert from tmp table if necessary
-            if tmp_tab:
-                params = []
-                sql = "INSERT INTO {}.{} ("; params += [self._sql.Identifier(sche), self._sql.Identifier(tab)]
-                for i, colinfo in enumerate([*key_columns, *nonkey_target_columns]):
-                    sql += ("," if i > 0 else "") + "{}"; params += [self._sql.Identifier(colinfo)]
-                sql += ") SELECT "
-                for i, colinfo in enumerate([*key_columns, *nonkey_target_columns]):
-                    sql += ("," if i > 0 else "") + "{}"; params += [self._sql.Identifier(colinfo)]
-                sql += " FROM {}"; params += [self._sql.Identifier(tmp_tab)]
-                sql += " ON CONFLICT ("
-                for i, colinfo in enumerate(key_columns):
-                    sql += ("," if i > 0 else "") + "{}"; params += [self._sql.Identifier(colinfo)]
-                sql += ") DO UPDATE SET "
-                for i, colinfo in enumerate(nonkey_target_columns):
-                    sql += ("," if i > 0 else "") + "{}=EXCLUDED.{}"; params += [self._sql.Identifier(colinfo), self._sql.Identifier(colinfo)]
-                
-                logger.debug("upsert from %s to %s.%s", tmp_tab, sche, tab)
-                self.execute_query(self._sql.SQL(sql).format(*params))
-
-            return result_count
-
-        finally:
-            if tmp_tab:
-                self.execute_query(self._sql.SQL("DROP TABLE IF EXISTS {}").format(self._sql.Identifier(tmp_tab)))
-
-    
-
-    def _actual_copy(self, query, fp):
-        BUFFER_SIZE = 65536
-
-        with self.cursor() as cursor:
-            with cursor.copy(query) as copy:
-                while True:
-                    data = fp.read(BUFFER_SIZE)
-                    if not data:
-                        break
-                    copy.write(data)
-            return cursor.rowcount
-        
-    #endregion
 
 
 try:
     from psycopg import Connection, Cursor, connect, sql
     from psycopg.errors import Diagnostic
-    from psycopg.sql import Composable, Composed
 
 
-    class PgAdapter(BasePgAdapter[Connection, Cursor, Composable, Composed]):
+    class PgAdapter(BasePgAdapter[Connection, Cursor]):
         """
         Database adapter for PostgreSQL (using `psycopg` (v3) driver).
         """
         _sql = sql
 
         @classmethod
         def is_available(cls):
```

## zut/db/pg2.py

```diff
@@ -7,17 +7,16 @@
 
 from .. import build_url
 from .pg import BasePgAdapter, pg_get_logging_level
 
 try:
     from psycopg2 import connect, sql
     from psycopg2.extensions import connection, cursor
-    from psycopg2.sql import Composable, Composed
 
-    class Pg2Adapter(BasePgAdapter[connection, cursor, Composable, Composed]):
+    class Pg2Adapter(BasePgAdapter[connection, cursor]):
         """
         Database adapter for PostgreSQL (using `psycopg2` driver).
         """
 
         EXPECTED_CONNECTION_TYPES = ['psycopg2.extensions.connection']
         _sql = sql
 
@@ -55,21 +54,15 @@
                 scheme=self.URL_SCHEME,
                 path='/' + params.get('dbname', None),
                 hostname=params.get('host', None),
                 port=params.get('port', None),
                 username=params.get('user', None),
                 password=params.get('password', None),
             )
-        
-
-        def _actual_copy(self, query, fp):
-            with self.cursor() as cursor:
-                cursor.copy_expert(query, fp)
-                return cursor.rowcount
-        
+                
 
         def register_notice_handler(self, logprefix = None, if_exists = '__raise__'):
             if self.connection.notices:
                 if if_exists != '__raise__':
                     return nullcontext(if_exists)
                 raise ValueError(f"notice handler already registered: {self.connection.notices}")
```

## Comparing `zut-0.9.1.dist-info/LICENSE.txt` & `zut-0.9.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `zut-0.9.1.dist-info/METADATA` & `zut-0.9.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zut
-Version: 0.9.1
+Version: 0.9.2
 Summary: Reusable Python utilities.
 Author-email: Sébastien Hocquet <dev@ipamo.net>
 Project-URL: Homepage, https://github.com/ipamo/zut
 Project-URL: Bug Tracker, https://github.com/ipamo/zut/issues
 Keywords: reusable,util,utils,common,commons,base,flexout,csv,excel,tabulate,smb,samba,share,out_table,out_file,db,DbAdapter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `zut-0.9.1.dist-info/RECORD` & `zut-0.9.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-zut/__init__.py,sha256=KJjWBTrzy0CAQihi99qUQP-84H6PXrTdpKFhD6dxkxQ,88849
-zut/_version.py,sha256=LJQMiDNP_yOQKZid2FYGwd5_O1rhbIq51L82OGb52hE,427
-zut/excel.py,sha256=BYlAmVhhu5Wx8p50ncdJcSHr1QzxVw-tkFMdkQd_3iY,24764
-zut/files.py,sha256=ttNuGPaI7EdvijMoYxqvDQ9j2copfcvH_RnoGXF1UL0,12859
+zut/__init__.py,sha256=zdPqZrqtjPxlmDL0JUkx21Y-CI7qZk_ba4cDBNKEikk,89190
+zut/_version.py,sha256=kf5P3B7rwrwCFjPGDgU8SMAYD27mDNFGKu1xYp5aJx8,427
+zut/excel.py,sha256=Tudw8Rzt-DrR8_n6rRpX4InJ2espLXwzFTz9cc5Ele4,25956
+zut/files.py,sha256=PhJNKPdaO6wI58ciHr1P_hwCavJ8pZhU-hK2a3k5rd4,12923
 zut/db/__init__.py,sha256=q22yE2ezKoXt1nNK_Yrjnt9qyao2g2DrAQWoDIgOwjQ,2984
-zut/db/base.py,sha256=xjEkEe3xxk9pL20RBnmj_rAvLGQ8UGQ2JNq9pKJ1cJc,27603
-zut/db/mssql.py,sha256=MGXV98dJiNX0QJTPYmsOro_lRjrfHVPbCLSHHWQLSis,11635
-zut/db/mysql.py,sha256=COqhAlx0izCR7W33HXae2OnpK9-znjHmdEZnXZd9h0A,8390
-zut/db/pg.py,sha256=XVaX_W5YgymOLuj9fCOSTOzLYiRPNKFa5HgG3Zyg4tA,19153
-zut/db/pg2.py,sha256=qyTLy-Eaw8100qpR3W0BREE-Pn8dcom3XyIJZhFPkeA,3808
+zut/db/base.py,sha256=NMjuyBULQA1YQxg7e0Mm4SsM0PFQxllbp5Yfmf45oEU,25278
+zut/db/mssql.py,sha256=FuS-d25WFzps6OTCI6HbAMkhm__N65cn8F-7jbyieHs,7700
+zut/db/mysql.py,sha256=M6fqDPcDbYlK4XE5fUJ5mDvJT8dTdfHrmMhbVEGoR2g,3265
+zut/db/pg.py,sha256=9qpserJkVziTLvvpKIv-5e2F9YSmco0650p04Q1FlIA,7151
+zut/db/pg2.py,sha256=iNkaIsNyozF7sp5LdlbfmGS8iGVXrKKop66H_cH82BA,3557
 zut/db/sql-utils/pg.sql,sha256=_CfoOZeIXJROCZcEHzrtBdjDBzloMyrGAObUzR2BmMU,1641
-zut-0.9.1.dist-info/LICENSE.txt,sha256=YTk_lGVv3UxRgzQTkxwYdikccg_bow2NGaId-s45n-I,1103
-zut-0.9.1.dist-info/METADATA,sha256=YQCL5hqKc8G9r5DJakJPf-TXXZgfpPuBJNKIO1vWmJo,3872
-zut-0.9.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-zut-0.9.1.dist-info/top_level.txt,sha256=0b5rfbMHLPzpcwBifEaAzzfyv1gZPGT7RXa2myDnXXs,4
-zut-0.9.1.dist-info/RECORD,,
+zut-0.9.2.dist-info/LICENSE.txt,sha256=YTk_lGVv3UxRgzQTkxwYdikccg_bow2NGaId-s45n-I,1103
+zut-0.9.2.dist-info/METADATA,sha256=-y_-MgbxKrEUQ_j6GTA8rYUmJGsbHRwnCmnA2acoRJc,3872
+zut-0.9.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+zut-0.9.2.dist-info/top_level.txt,sha256=0b5rfbMHLPzpcwBifEaAzzfyv1gZPGT7RXa2myDnXXs,4
+zut-0.9.2.dist-info/RECORD,,
```

