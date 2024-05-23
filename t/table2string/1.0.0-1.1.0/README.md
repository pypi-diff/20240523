# Comparing `tmp/table2string-1.0.0.tar.gz` & `tmp/table2string-1.1.0.tar.gz`

## Comparing `table2string-1.0.0.tar` & `table2string-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 table2string-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 table2string-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 table2string-1.0.0/table2string/__init__.py
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 table2string-1.0.0/table2string/table2string.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 table2string-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0    15849 2020-02-02 00:00:00.000000 table2string-1.0.0/tests/test_table2text.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 table2string-1.0.0/.gitignore
--rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 table2string-1.0.0/LICENSE
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 table2string-1.0.0/README.md
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 table2string-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 table2string-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 table2string-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 table2string-1.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 table2string-1.1.0/table2string/__init__.py
+-rw-r--r--   0        0        0    10581 2020-02-02 00:00:00.000000 table2string-1.1.0/table2string/table2string.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 table2string-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    17934 2020-02-02 00:00:00.000000 table2string-1.1.0/tests/test_table2string.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 table2string-1.1.0/.gitignore
+-rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 table2string-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 table2string-1.1.0/README.md
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 table2string-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 table2string-1.1.0/PKG-INFO
```

### Comparing `table2string-1.0.0/.github/workflows/publish.yml` & `table2string-1.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `table2string-1.0.0/.github/workflows/tests.yml` & `table2string-1.1.0/.github/workflows/tests.yml`

 * *Files 19% similar despite different names*

```diff
@@ -23,20 +23,21 @@
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+        pip install black ruff pytest
         pip install .
     - name: Lint with black
       run: |
-        pip install black
         black . --check --diff
     - name: Lint with Ruff
       run: |
-        pip install ruff
         ruff check . --ignore=E501
     - name: Test with pytest
       run: |
-        pip install pytest
         pytest
+    - name: Test README.md with doctest
+      run: |
+        python -m doctest -f README.md
```

### Comparing `table2string-1.0.0/table2string/table2string.py` & `table2string-1.1.0/table2string/table2string.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,77 +5,79 @@
 
 AlignType: TypeAlias = Literal[
     "<", ">", "^", "*", "<<", "<^", "<>", "^<", "^^", "^>", "><", ">^", ">>"
 ]
 
 
 def get_text_width_in_console(text: str) -> int:
-    """Определяет количество позиций, которое займет строка в консоли."""
+    """
+    Calculates the number of positions that a line will occupy in the console.
+    """
     width = 0
     for char in text:
         if unicodedata.east_asian_width(char) in ("W", "F"):
-            width += 2  # Широкие символы
+            width += 2  # Wide characters
         else:
-            width += 1  # Узкие символы
+            width += 1  # Narrow characters
     return width
 
 
 def decrease_numbers(
     row_lengths: list[int], max_width: int = 120, min_value: int = 10
 ) -> list[int]:
     """
 
     :param row_lengths:
     :param max_width:
     :param min_value:
     :return:
     """
-    # Рассчитываем среднее значение
+    # Calculate the average value
     mean_value = sum(row_lengths) / len(row_lengths)
     new_numbers = []
 
     for num in row_lengths:
-        # Определяем насколько это число больше или меньше среднего
+        # Determine how much more or less this number is than the average
         diff_from_mean = num - mean_value
 
         if diff_from_mean > 0:
             reduction_percent = 0.4
         else:
             reduction_percent = 0.01
 
         reduced_num = num - (mean_value * reduction_percent)
 
         new_num = max(int(reduced_num), min_value)
         new_numbers.append(new_num)
 
-    # Если общая сумма новых чисел превышает max_width, уменьшаем наибольшее число на 1
+    # If the total sum of new numbers exceeds max_width, reduce the largest number by 1
     while sum(new_numbers) > max_width:
         new_numbers[new_numbers.index(max(new_numbers))] -= 1
 
-    # Рассчитываем коэффициент для пропорционального увеличения, если сумма меньше max_sum
+    # Calculate the coefficient for proportional increase if the sum is less than max_sum
     if sum(new_numbers) < max_width:
         new_numbers = [int(num * (max_width / sum(new_numbers))) for num in new_numbers]
 
-    # Если общая сумма новых чисел меньше max_width, увеличиваем наименьшее число на 1
+    # If the total sum of new numbers is less than max_width, increase the smallest number by 1
     while sum(new_numbers) < max_width and min(new_numbers) < min_value:
         new_numbers[new_numbers.index(min(new_numbers))] += 1
 
     return new_numbers
 
 
 def transform_align(
     column_count: int, align: tuple[AlignType | str, ...] | AlignType | str = "*"
 ) -> tuple[AlignType]:
     """
+    Convert align to a suitable view
 
     :param column_count:
     :param align:
     :return:
     """
-    # Преобразуем align в подходящий вид
     if isinstance(align, str):
         align = (align, *(align,) * (column_count - 1))
     else:
         align = (*align, *("*",) * (column_count - len(align)))
 
     return align[:column_count]
 
@@ -86,47 +88,54 @@
     """
 
     :param width:
     :param column_count:
     :param row_lengths:
     :return:
     """
-    if width is not None and isinstance(width, tuple):
+    if isinstance(width, (tuple, list)) and column_count == len(width):
+        return width
+
+    if width is not None and isinstance(width, (tuple, list)):
         width: tuple[int]
+
         if len(width) < column_count:
             width: tuple = tuple((*width, *(width[-1],) * (column_count - len(width))))
+
         width: int = sum(width) + (3 * len(width)) + 1
 
     if width is not None and width < column_count + (3 * column_count) + 1:
         width: int = (
             sum(1 if rl > 1 else 0 for rl in row_lengths) + (3 * column_count) + 1
         )
 
-    # Вычисляем ширину каждой колонки
+    # Calculate the width of each column
     if width:
         sum_column_width = width - (3 * column_count) - 1
         max_widths = decrease_numbers(row_lengths, sum_column_width)
     else:
         max_widths = row_lengths
 
     return max_widths
 
 
 def line_spliter(
     text: str,
     width: int = None,
     height: int = None,
     line_break_symbol: str = "↩",
+    cell_break_symbol: str = "…",  # chr(8230)
 ) -> tuple[list[str], list[str]]:
     """
 
     :param text:
     :param width:
     :param height:
     :param line_break_symbol:
+    :param cell_break_symbol:
     :return:
     """
     lines = text.split("\n")
     result_lines = []
     result_breaks = []
     for line in lines:
         if get_text_width_in_console(line) == 0:
@@ -145,15 +154,15 @@
                     result_lines.append(line[:w])
                     result_breaks.append(line_break_symbol)
                     line = line[w:]
 
     if height and len(result_lines) > height:
         result_lines = result_lines[:height]
         result_breaks = result_breaks[:height]
-        result_breaks[-1] = chr(8230)  # "…"
+        result_breaks[-1] = cell_break_symbol
 
     return result_lines, result_breaks
 
 
 def fill_line(
     rows: list[list[str]],
     symbols: list[list[str]],
@@ -172,15 +181,15 @@
     align_left, align_right = map(
         list, zip(*(a * 2 if len(a) == 1 else a for a in align))
     )
 
     if isinstance(rows[0], tuple):
         rows = list(map(list, rows))  # noqa
 
-    # Делаем каждый элемент одинаковой ширины по максимальному элементу
+    # Make each element the same width according to the maximum element
     for n, row in enumerate(rows):
         if align_left[n] == "^" and align_right[n] in ("<", ">") and len(row) > 1:
             max_width = len(max(row, key=len))
             row[:] = [f"{r:{align_right[n]}{max_width}}" for _n, r in enumerate(row)]
             align_right[n] = "^"
 
         if align_left[n] == "*" or align_right[n] == "*":
@@ -217,30 +226,43 @@
 
 def print_table(
     table: list[tuple[str, ...]],
     align: tuple[AlignType | str] | AlignType | str = "*",
     name: str = None,
     name_align: Literal["<", ">", "^"] | str = None,
     max_width: int | tuple[int, ...] = None,
-    max_height: int | tuple[int, ...] = None,
+    max_height: int = None,
     file: StringIO = None,
     line_break_symbol: str = "↩",
+    cell_break_symbol: str = "…",
+    sep: bool | range | tuple = True,
+    end: str | None = "\n",
 ) -> None:
     """
 
     :param table:
     :param align:
     :param name:
     :param name_align:
     :param max_width:
     :param max_height:
     :param file:
     :param line_break_symbol:
+    :param cell_break_symbol:
+    :param sep:
+    :param end:
     :return:
     """
+
+    if len(line_break_symbol) != 1:
+        raise ValueError("length of line_break_symbol must be 1")
+
+    if len(cell_break_symbol) != 1:
+        raise ValueError("length of cell_break_symbol must be 1")
+
     row_lengths: list[int] = []
 
     for column in zip(*table):
         cell_widths = []
         for cell in column:
             if cell:
                 lines = str(cell).splitlines() or [""]
@@ -252,48 +274,98 @@
                 cell_widths.append(1)
 
         row_lengths.append(max(cell_widths))
 
     column_count = max(map(len, table))
     align = transform_align(column_count, align)
     max_widths = transform_width(max_width, column_count, row_lengths)
-
-    # Обрезаем длинные строки
-    table = [
-        [
-            line_spliter(column, max_widths[n], max_height, line_break_symbol)
-            for n, column in enumerate(map(str, row))
-        ]
-        for row in table
-    ]
-
-    # Разделитель строк
-    sep = "+" + "".join(("-" * (i + 2)) + "+" for i in max_widths)
+    line_separator = "+" + "".join(("-" * (i + 2)) + "+" for i in max_widths)
 
     if name:
         # noinspection PyTypeChecker
         name_align = transform_align(1, name_align or "^")
-        print("+" + sep.replace("+", "-")[1:-1] + "+", file=file)
+        print("+" + line_separator.replace("+", "-")[1:-1] + "+", file=file)
 
-        if not max_width:
-            max_width: int = sum(row_lengths) + (3 * column_count) + 1
+        if not max_widths:
+            max_name_width: int = sum(row_lengths) + (3 * column_count) + 1 - 4
+        else:
+            max_name_width = sum(max_widths) + (3 * column_count) + 1 - 4
 
         rows, symbols = zip(
-            line_spliter(name, max_width - 4, max_height, line_break_symbol)
+            line_spliter(
+                name, max_name_width, max_height, line_break_symbol, cell_break_symbol
+            )
         )
-        line = fill_line(rows, symbols, [max_width - 4], name_align)
+        line = fill_line(rows, symbols, [max_name_width], name_align)
         print(line, file=file)
 
+    # Trimming long lines
+    table = (
+        [
+            line_spliter(
+                column, max_widths[n], max_height, line_break_symbol, cell_break_symbol
+            )
+            for n, column in enumerate(map(str, row))
+        ]
+        for row in table
+    )
+
     for n, row in enumerate(table):
-        print(sep, file=file)
+        if (sep is True or n == 0) or (isinstance(sep, (range, tuple)) and n in sep):
+            print(line_separator, file=file)
+
         max_row_height = max(map(len, tuple(zip(*row))[0]))
 
         for column in row:
             extend_data = (" ",) * (max_row_height - len(column[0]))
             column[0].extend(extend_data)
             column[1].extend(extend_data)
 
         rows, symbols = zip(*row)
         line = fill_line(rows, symbols, max_widths, align)
         print(line, file=file)
 
-    print(sep.rstrip("\n"), file=file)
+    print(line_separator.rstrip("\n"), file=file, end=end)
+
+
+def stringify_table(
+    table: list[tuple[str, ...]],
+    align: tuple[AlignType | str] | AlignType | str = "*",
+    name: str = None,
+    name_align: Literal["<", ">", "^"] | str = None,
+    max_width: int | tuple[int, ...] = None,
+    max_height: int = None,
+    line_break_symbol: str = "↩",
+    cell_break_symbol: str = "…",
+    sep: bool | range | tuple = True,
+    end: str | None = "",
+) -> str:
+    """
+
+    :param table:
+    :param align:
+    :param name:
+    :param name_align:
+    :param max_width:
+    :param max_height:
+    :param line_break_symbol:
+    :param cell_break_symbol:
+    :param sep:
+    :param end:
+    :return:
+    """
+    file = StringIO()
+    print_table(
+        table=table,
+        align=align,
+        name=name,
+        name_align=name_align,
+        max_width=max_width,
+        max_height=max_height,
+        file=file,
+        line_break_symbol=line_break_symbol,
+        cell_break_symbol=cell_break_symbol,
+        sep=sep,
+        end=end,
+    )
+    file.seek(0)
+    return file.read()
```

### Comparing `table2string-1.0.0/tests/test_table2text.py` & `table2string-1.1.0/tests/test_table2string.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from io import StringIO
-from typing import Callable
-
 from table2string.table2string import (
     decrease_numbers,
     transform_align,
     transform_width,
+    stringify_table,
     line_spliter,
-    print_table,
     fill_line,
 )
 
 
 def test_decrease_numbers():
     assert decrease_numbers([2, 2, 3], 10) == [3, 3, 4]
     assert decrease_numbers([2, 2, 3], 11) == [3, 4, 4]
@@ -28,15 +25,16 @@
     assert transform_align(3, ("<", "<", "<")) == ("<", "<", "<")
 
 
 def test_transform_width():
     assert transform_width(1, 1, [1]) == [0]
     assert transform_width(1, 2, [2, 2]) == [1, 1]
     assert transform_width((1, 2), 1, [1]) == [6]
-    assert transform_width((1, 2), 2, [2, 2]) == [1, 2]
+    assert transform_width((1, 2), 2, [2, 2]) == (1, 2)
+    assert transform_width((3, 2), 2, [2, 2]) == (3, 2)  # FIXME
 
 
 def test_line_spliter():
     assert line_spliter("", 1) == ([" "], [" "])
     assert line_spliter("1", 1) == (["1"], [" "])
     assert line_spliter("123\n456", 1) == (
         ["1", "2", "3", "4", "5", "6"],
@@ -184,279 +182,269 @@
 |        34    |
 |   1234567    |
 |    787878    |
 """.strip()
     )
 
 
-def test_print_table():
-    def decorator(func: Callable):
-        def wrapper(*args, **kwargs):
-            file = StringIO()
-            func(*args, **kwargs, file=file)
-            file.seek(0)
-            return file.read()
-
-        return wrapper
-
-    get_table = decorator(print_table)
+def test_stringify_table():
     table_1 = [(1, 2, 3), ("123", "456\n567", "")]
     assert (
-        get_table(table_1)
+        stringify_table(table_1)
         == """
 +-----+-----+---+
 |   1 |   2 | 3 |
 +-----+-----+---+
 | 123 | 456 |   |
 |     | 567 |   |
 +-----+-----+---+
-""".lstrip()
+""".strip()
     )
     table_2 = [(1, 2, 3), ("12345", "456\n\n567", ""), ("q", "NULL", "NULL")]
     assert (
-        get_table(table_2)
+        stringify_table(table_2)
         == """
 +-------+------+------+
 |     1 |    2 |    3 |
 +-------+------+------+
 | 12345 | 456  |      |
 |       |      |      |
 |       | 567  |      |
 +-------+------+------+
 | q     | NULL | NULL |
 +-------+------+------+
-""".lstrip()
+""".strip()
     )
     assert (
-        get_table(table_2, align="<", name="Table Name")
+        stringify_table(table_2, align="<", name="Table Name")
         == """
 +---------------------+
 |     Table Name      |
 +-------+------+------+
 | 1     | 2    | 3    |
 +-------+------+------+
 | 12345 | 456  |      |
 |       |      |      |
 |       | 567  |      |
 +-------+------+------+
 | q     | NULL | NULL |
 +-------+------+------+
-""".lstrip()
+""".strip()
     )
     assert (
-        get_table(table_2, align=">", name="Table Name")
+        stringify_table(table_2, align=">", name="Table Name")
         == """
 +---------------------+
 |     Table Name      |
 +-------+------+------+
 |     1 |    2 |    3 |
 +-------+------+------+
 | 12345 |  456 |      |
 |       |      |      |
 |       |  567 |      |
 +-------+------+------+
 |     q | NULL | NULL |
 +-------+------+------+
-""".lstrip()
+""".strip()
     )
     table_3 = [("coll 1", "coll 2")]
     assert (
-        get_table(table_3, name="Table\nName", name_align="<")
+        stringify_table(table_3, name="Table\nName", name_align="<")
         == """
 +-----------------+
 | Table           |
 | Name            |
 +--------+--------+
 | coll 1 | coll 2 |
 +--------+--------+
-""".lstrip()
+""".strip()
     )
     assert (
-        get_table(table_3, name="Table\nName", name_align="^")
+        stringify_table(table_3, name="Table\nName", name_align="^")
         == """
 +-----------------+
 |      Table      |
 |      Name       |
 +--------+--------+
 | coll 1 | coll 2 |
 +--------+--------+
-""".lstrip()
+""".strip()
     )
     assert (
-        get_table(table_3, name="Table\nName", name_align=">")
+        stringify_table(table_3, name="Table\nName", name_align=">")
         == """
 +-----------------+
 |           Table |
 |            Name |
 +--------+--------+
 | coll 1 | coll 2 |
 +--------+--------+
-""".lstrip()
+""".strip()
     )
     assert (
-        get_table(table_3, name="Table\nName", name_align="<<")
+        stringify_table(table_3, name="Table\nName", name_align="<<")
         == """
 +-----------------+
 | Table           |
 | Name            |
 +--------+--------+
 | coll 1 | coll 2 |
 +--------+--------+
-""".lstrip()
+""".strip()
     )
     assert (
-        get_table(table_3, name="Table\nName", name_align=">>")
+        stringify_table(table_3, name="Table\nName", name_align=">>")
         == """
 +-----------------+
 |           Table |
 |            Name |
 +--------+--------+
 | coll 1 | coll 2 |
 +--------+--------+
-""".lstrip()
+""".strip()
     )
     assert (
-        get_table(table_3, name="Table\nName", name_align="<>")
+        stringify_table(table_3, name="Table\nName", name_align="<>")
         == """
 +-----------------+
 | Table           |
 |            Name |
 +--------+--------+
 | coll 1 | coll 2 |
 +--------+--------+
-""".lstrip()
+""".strip()
     )
     assert (
-        get_table(table_3, name="Table\nName", name_align="><")
+        stringify_table(table_3, name="Table\nName", name_align="><")
         == """
 +-----------------+
 |           Table |
 | Name            |
 +--------+--------+
 | coll 1 | coll 2 |
 +--------+--------+
-""".lstrip()
+""".strip()
     )
     table_4 = [("",)]
     assert (
-        get_table(table_4)
+        stringify_table(table_4)
         == """
 +---+
 |   |
 +---+
-""".lstrip()
+""".strip()
     )
     table_5 = [("\n1",)]
     assert (
-        get_table(table_5)
+        stringify_table(table_5)
         == """
 +---+
 |   |
 | 1 |
 +---+
-""".lstrip()
+""".strip()
     )
     table_6 = [("123",)]
     assert (
-        get_table(table_6, max_width=1)
+        stringify_table(table_6, max_width=1)
         == """
 +---+
 | 1↩|
 | 2↩|
 | 3 |
 +---+
-""".lstrip()
+""".strip()
     )
     table_7 = [("123",)]
     assert (
-        get_table(table_7, max_width=(2,))
+        stringify_table(table_7, max_width=(2,))
         == """
 +----+
 | 12↩|
 | 3  |
 +----+
-""".lstrip()
+""".strip()
     )
     table_7 = [("123",)]
     assert (
-        get_table(table_7, max_width=(1,), max_height=2)
+        stringify_table(table_7, max_width=(1,), max_height=2)
         == """
 +---+
 | 1↩|
 | 2…|
 +---+
-""".lstrip()
+""".strip()
     )
     table_8 = [("1",), ("q",), ("👍",)]
     assert (
-        get_table(table_8)
+        stringify_table(table_8)
         == """
 +----+
 |  1 |
 +----+
 | q  |
 +----+
 | 👍 |
 +----+
-""".lstrip()
+""".strip()
     )
     table_9 = [("123456\n\n789000",)]
     assert (
-        get_table(table_9, max_width=(3,), max_height=4)
+        stringify_table(table_9, max_width=(3,), max_height=4)
         == """
 +-----+
 | 123↩|
 | 456 |
 |     |
 | 789…|
 +-----+
-""".lstrip()
+""".strip()
     )
     table_10 = [("1234567\n\n891\n234",)]
     assert (
-        get_table(table_10, max_width=(2,), max_height=7)
+        stringify_table(table_10, max_width=(2,), max_height=7)
         == """
 +----+
 | 12↩|
 | 34↩|
 | 56↩|
 | 7  |
 |    |
 | 89↩|
 | 1 …|
 +----+
-""".lstrip()
+""".strip()
     )
     table_11 = [("1234567\n\n891\n234", "qwe" * 20)]
     assert (
-        get_table(table_11, max_width=(2,), max_height=7)
+        stringify_table(table_11, max_width=(2,), max_height=7)
         == """
 +----+----+
 | 12↩| qw↩|
 | 34↩| eq↩|
 | 56↩| we↩|
 | 7  | qw↩|
 |    | eq↩|
 | 89↩| we↩|
 | 1 …| qw…|
 +----+----+
-""".lstrip()
+""".strip()
     )
     table_12 = [("long string",), ("1234567\n34\n787878",)]
     assert (
-        get_table(table_12, align="^<")
+        stringify_table(table_12, align="^<")
         == """
 +-------------+
 | long string |
 +-------------+
 |   1234567   |
 |   34        |
 |   787878    |
 +-------------+
-""".lstrip()
+""".strip()
     )
     table_13 = [
         ("filler " * 10,),
         (
             """
 We're no strangers to love
 You know the rules and so do I (do I)
@@ -472,15 +460,15 @@
 Never gonna make you cry
 Never gonna say goodbye
 Never gonna tell a lie and hurt you
 """.strip(),
         ),
     ]
     assert (
-        get_table(table_13, align="^<")
+        stringify_table(table_13, align="^<")
         == """
 +------------------------------------------------------------------------+
 | filler filler filler filler filler filler filler filler filler filler  |
 +------------------------------------------------------------------------+
 |                We're no strangers to love                              |
 |                You know the rules and so do I (do I)                   |
 |                A full commitment's what I'm thinking of                |
@@ -492,18 +480,18 @@
 |                Never gonna give you up                                 |
 |                Never gonna let you down                                |
 |                Never gonna run around and desert you                   |
 |                Never gonna make you cry                                |
 |                Never gonna say goodbye                                 |
 |                Never gonna tell a lie and hurt you                     |
 +------------------------------------------------------------------------+
-""".lstrip()
+""".strip()
     )
     assert (
-        get_table(table_13, align="^>")
+        stringify_table(table_13, align="^>")
         == """
 +------------------------------------------------------------------------+
 | filler filler filler filler filler filler filler filler filler filler  |
 +------------------------------------------------------------------------+
 |                              We're no strangers to love                |
 |                   You know the rules and so do I (do I)                |
 |                A full commitment's what I'm thinking of                |
@@ -515,18 +503,18 @@
 |                                 Never gonna give you up                |
 |                                Never gonna let you down                |
 |                   Never gonna run around and desert you                |
 |                                Never gonna make you cry                |
 |                                 Never gonna say goodbye                |
 |                     Never gonna tell a lie and hurt you                |
 +------------------------------------------------------------------------+
-""".lstrip()
+""".strip()
     )
     assert (
-        get_table(table_13, align="^>", max_width=20)
+        stringify_table(table_13, align="^>", max_width=20)
         == """
 +------------------+
 | filler filler fi↩|
 | ller filler fill↩|
 | er filler filler↩|
 |  filler filler f↩|
 |           iller  |
@@ -560,18 +548,18 @@
 |          you cry |
 | Never gonna say ↩|
 |          goodbye |
 | Never gonna tell↩|
 |  a lie and hurt ↩|
 |              you |
 +------------------+
-""".lstrip()
+""".strip()
     )
     assert (
-        get_table(table_13[:1], name=table_13[1][0], name_align="^<")
+        stringify_table(table_13[:1], name=table_13[1][0], name_align="^<")
         == """
 +------------------------------------------------------------------------+
 |                We're no strangers to love                              |
 |                You know the rules and so do I (do I)                   |
 |                A full commitment's what I'm thinking of                |
 |                You wouldn't get this from any other guy                |
 |                                                                        |
@@ -583,32 +571,171 @@
 |                Never gonna run around and desert you                   |
 |                Never gonna make you cry                                |
 |                Never gonna say goodbye                                 |
 |                Never gonna tell a lie and hurt you                     |
 +------------------------------------------------------------------------+
 | filler filler filler filler filler filler filler filler filler filler  |
 +------------------------------------------------------------------------+
-""".lstrip()
+""".strip()
     )
     table_14 = [("filler" * 2,), ("12345\n67890",)]
     assert (
-        get_table(table_14, align="<>")
+        stringify_table(table_14, align="<>")
         == """
 +--------------+
 | fillerfiller |
 +--------------+
 | 12345        |
 |        67890 |
 +--------------+
-""".lstrip()
+""".strip()
     )
     assert (
-        get_table(table_14, align="><")
+        stringify_table(table_14, align="><")
         == """
 +--------------+
 | fillerfiller |
 +--------------+
 |        12345 |
 | 67890        |
 +--------------+
-""".lstrip()
+""".strip()
+    )
+    table_15 = [("qwe", "rty\nuio"), ("123456\n\n789000", "example")]
+    kwargs = {
+        "max_width": (3, 4),
+        "max_height": 4,
+        "line_break_symbol": "\\",
+        "cell_break_symbol": "/",
+    }
+    assert (
+        stringify_table(table_15, **kwargs, sep=True)
+        == """
++-----+------+
+| qwe | rty  |
+|     | uio  |
++-----+------+
+| 123\\| exam\\|
+| 456 | ple  |
+|     |      |
+| 789/|      |
++-----+------+
+""".strip()
+    )
+    assert (
+        stringify_table(table_15, **kwargs, sep=False)
+        == """
++-----+------+
+| qwe | rty  |
+|     | uio  |
+| 123\\| exam\\|
+| 456 | ple  |
+|     |      |
+| 789/|      |
++-----+------+
+""".strip()
+    )
+    table_16 = [("1", "2"), ("3", "4")]
+    assert (
+        stringify_table(table_16, sep=True, name="Name")
+        == """
++-------+
+| Name  |
++---+---+
+| 1 | 2 |
++---+---+
+| 3 | 4 |
++---+---+
+""".strip()
+    )
+    assert (
+        stringify_table(table_16, sep=False, name="Name")
+        == """
++-------+
+| Name  |
++---+---+
+| 1 | 2 |
+| 3 | 4 |
++---+---+
+""".strip()
+    )
+    table_17 = [("1", "2"), ("3", "4"), ("5", "6"), ("7", "8")]
+    assert (
+        stringify_table(table_17, sep=(1,))
+        == """
++---+---+
+| 1 | 2 |
++---+---+
+| 3 | 4 |
+| 5 | 6 |
+| 7 | 8 |
++---+---+
+""".strip()
+    )
+    assert (
+        stringify_table(table_17, sep=(2,))
+        == """
++---+---+
+| 1 | 2 |
+| 3 | 4 |
++---+---+
+| 5 | 6 |
+| 7 | 8 |
++---+---+
+""".strip()
+    )
+    assert (
+        stringify_table(table_17, sep=(1, 3))
+        == """
++---+---+
+| 1 | 2 |
++---+---+
+| 3 | 4 |
+| 5 | 6 |
++---+---+
+| 7 | 8 |
++---+---+
+""".strip()
+    )
+    assert (
+        stringify_table(table_17, sep=(1,), name="Name")
+        == """
++-------+
+| Name  |
++---+---+
+| 1 | 2 |
++---+---+
+| 3 | 4 |
+| 5 | 6 |
+| 7 | 8 |
++---+---+
+""".strip()
+    )
+    assert (
+        stringify_table(table_17, sep=(2,), name="Name")
+        == """
++-------+
+| Name  |
++---+---+
+| 1 | 2 |
+| 3 | 4 |
++---+---+
+| 5 | 6 |
+| 7 | 8 |
++---+---+
+""".strip()
+    )
+    assert (
+        stringify_table(table_17, sep=(1, 3), name="Name")
+        == """
++-------+
+| Name  |
++---+---+
+| 1 | 2 |
++---+---+
+| 3 | 4 |
+| 5 | 6 |
++---+---+
+| 7 | 8 |
++---+---+
+""".strip()
     )
```

### Comparing `table2string-1.0.0/LICENSE` & `table2string-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `table2string-1.0.0/pyproject.toml` & `table2string-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "table2string"
-version = "1.0.0"
+version = "1.1.0"
 description = "A library to convert tables to string with full support for line breaks and formatting"
 authors = [{name = "EgorKhabarov", email = "not.a.fan.of.broccoli@gmail.com"}]
 license = {text = "GPL2"}
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["table", "string", "tools"]
 classifiers = [
```

