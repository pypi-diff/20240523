# Comparing `tmp/tablinum-0.1.2.tar.gz` & `tmp/tablinum-0.1.3.tar.gz`

## Comparing `tablinum-0.1.2.tar` & `tablinum-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 tablinum-0.1.2/src/tablinum/__about__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tablinum-0.1.2/src/tablinum/__init__.py
--rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 tablinum-0.1.2/src/tablinum/tab_fun_dates.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 tablinum-0.1.2/src/tablinum/tab_fun_maths.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 tablinum-0.1.2/src/tablinum/tab_fun_useful.py
--rw-r--r--   0        0        0    58701 2020-02-02 00:00:00.000000 tablinum-0.1.2/src/tablinum/tablinum.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test-input.txt
--rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_calculation.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_command_line.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_contingency.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_filter.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_grouping.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_help.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_levels.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_makers.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_parsing.py
--rw-r--r--   0        0        0     9593 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_poppers_and_adders.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_roller.py
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_sort.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_text_manip.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tab_wrangler.py
--rw-r--r--   0        0        0    13743 2020-02-02 00:00:00.000000 tablinum-0.1.2/tests/test_tablinum.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tablinum-0.1.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tablinum-0.1.2/LICENSE
--rw-r--r--   0        0        0    60858 2020-02-02 00:00:00.000000 tablinum-0.1.2/README.md
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 tablinum-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    61746 2020-02-02 00:00:00.000000 tablinum-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tablinum-0.1.3/t
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 tablinum-0.1.3/src/tablinum/__about__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tablinum-0.1.3/src/tablinum/__init__.py
+-rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 tablinum-0.1.3/src/tablinum/tab_fun_dates.py
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 tablinum-0.1.3/src/tablinum/tab_fun_maths.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 tablinum-0.1.3/src/tablinum/tab_fun_useful.py
+-rw-r--r--   0        0        0    59527 2020-02-02 00:00:00.000000 tablinum-0.1.3/src/tablinum/tablinum.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test-input.txt
+-rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_calculation.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_command_line.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_contingency.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_filter.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_grouping.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_help.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_levels.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_makers.py
+-rw-r--r--   0        0        0     9002 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_parsing.py
+-rw-r--r--   0        0        0     9593 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_poppers_and_adders.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_roller.py
+-rw-r--r--   0        0        0     9684 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_sort.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_text_manip.py
+-rw-r--r--   0        0        0     8119 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_wrangler.py
+-rw-r--r--   0        0        0    14125 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tablinum.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tablinum-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tablinum-0.1.3/LICENSE
+-rw-r--r--   0        0        0    60858 2020-02-02 00:00:00.000000 tablinum-0.1.3/README.md
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 tablinum-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    61853 2020-02-02 00:00:00.000000 tablinum-0.1.3/PKG-INFO
```

### Comparing `tablinum-0.1.2/src/tablinum/tab_fun_dates.py` & `tablinum-0.1.3/src/tablinum/tab_fun_dates.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/src/tablinum/tab_fun_maths.py` & `tablinum-0.1.3/src/tablinum/tab_fun_maths.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,43 +224,47 @@
     >>> si('.2 k')
     Decimal('200.0')
     >>> si('Heading')
     'Heading'
 
     """
     sips = ' kMGTPE'
-    m = re.match(rf'([-+]?(?:\d+\.\d*|\.\d+|0|[1-9]\d*))\s*([{sips}])\Z', str(amount))
-    if m is not None:
+    sipat = re.compile(rf'([-+]?(?:\d+\.\d*|\.\d+|0|[1-9]\d*))\s*([{sips}])\Z')
+    if (m := sipat.match(str(amount))) is not None:
         return decimal.Decimal(m.group(1)) * 10 ** (3 * sips.index(m.group(2)))
+
     try:
         n = decimal.Decimal(amount)
     except decimal.InvalidOperation:
         return amount
     else:
         e = min(int(n.log10() / 3), len(sips) - 1)
         return '{:7.3f} {}'.format(n / (10 ** (3 * e)), sips[e]).strip()
 
 
-def ifactors(n):
-    "Iterate through the factors"
+def factors(n):
+    '''find the factors of n and return them in a tuple ... only use this for small numbers
+    >>> factors(12345)
+    (3, 5, 823)
+    >>> factors(128)
+    (2, 2, 2, 2, 2, 2, 2)
+    >>> factors(817)
+    (19, 43)
+    >>> factors(1000038)
+    (2, 3, 13, 12821)
+    >>> factors(1000039)
+    (1000039,)
+    >>> factors(8761591) 
+    (2957, 2963)
+    '''
+    out = []
     f = 2
-    f_cycle = itertools.cycle([4, 2, 4, 2, 4, 6, 2, 6])
-    increments = itertools.chain([1, 2, 2], f_cycle)
-    for incr in increments:
+    for incr in itertools.chain([1, 2, 2], itertools.cycle([4, 2, 4, 2, 4, 6, 2, 6])):
         if f * f > n:
             break
         while n % f == 0:
-            yield f
+            out.append(f)
             n //= f
         f += incr
     if n > 1:
-        yield n
-
-
-def factors(n):
-    '''find the factors of n and return a list... very slowly
-    >>> factors(12345)
-    [3, 5, 823]
-    >>> factors(128)
-    [2, 2, 2, 2, 2, 2, 2]
-    '''
-    return list(ifactors(n))
+        out.append(n)
+    return tuple(out)
```

### Comparing `tablinum-0.1.2/src/tablinum/tab_fun_useful.py` & `tablinum-0.1.3/src/tablinum/tab_fun_useful.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/src/tablinum/tablinum.py` & `tablinum-0.1.3/src/tablinum/tablinum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python3
 '''Tablinum
 
 A module to line up text tables.
-Toby Thurston -- 19 Apr 2024
+Toby Thurston -- 24 Apr 2024
 '''
 
 import argparse
 import builtins
 import collections
 import csv
 import decimal
@@ -21,14 +21,17 @@
 import sys
 import textwrap
 import tokenize
 
 import tablinum.tab_fun_dates as tab_fun_dates
 import tablinum.tab_fun_maths as tab_fun_maths
 import tablinum.tab_fun_useful as tab_fun_useful
+# import tab_fun_dates
+# import tab_fun_maths
+# import tab_fun_useful
 
 
 # Panther is a big cat of functions for column maths, using the Decimal
 # versions.  This is used to limit the scope of the `eval` function when
 # evaluating expressions in DSL options.  So if you are calculating a new
 # column value with arr, or sorting on a calculated value etc, you can only use
 # the functions in this dictionary.  The idea is that the keys are what you the
@@ -141,14 +144,21 @@
     (536.2, '8:56.2')
 
     >>> as_numeric_tuple("13:34:20")
     (48860.0, '13:34:20')
 
     >>> as_numeric_tuple("Monday") < as_numeric_tuple("Friday")
     True
+
+    >>> as_numeric_tuple('192.168.0.1')
+    (3232235521, '192.168.0.1')
+
+    >>> as_numeric_tuple('00:01:E6:2C:42:1D')
+    (8156627485, '00:01:E6:2C:42:1D')
+
     '''
 
     alpha, omega = -1e12, 1e12
     if backwards:
         alpha, omega = omega, alpha
 
     if x is None or x == '':
@@ -163,35 +173,43 @@
 
     try:
         return (tab_fun_dates.parse_date(x).toordinal(), x)   # make parse date return epoch sec string
     except ValueError:
         pass
 
     # is this a time?
-    m = re.match(r'(\d+):([0-5]\d):([0-5]\d(\.\d+)?)', x)
-    if m is not None:
+    if (m := re.match(r'(\d+):([0-5]\d):([0-5]\d(\.\d+)?)\Z', x)) is not None:
         return (int(m.group(1)) * 3600 + int(m.group(2)) * 60 + float(m.group(3)), x)
 
-    m = re.match(r'(\d+):([0-5]\d(\.\d+)?)', x)
-    if m is not None:
+    if (m := re.match(r'(\d+):([0-5]\d(\.\d+)?\Z)', x)) is not None:
         return (int(m.group(1)) * 60 + float(m.group(2)), x)
 
+    # is this an IP4 address?
+    if (m := re.match(r'(\d+)\.(\d+)\.(\d+)\.(\d+)\Z', x)) is not None:
+        a, b, c, d = map(int, m.groups())
+        if all(t < 256 for t in (a, b, c, d)):
+            return (a * 16777216 + b * 65536 + c * 256 + d, x)
+
+    # is this a MAC address
+    if all(t in '0123456789ABCDEF:' for t in x):
+        if x.count(':') == 5:
+            if len(x) == 17:
+                return (int(x.replace(':', ''), 16), x)
+
     # pad trailing numbers with zeros
     # Make A1, A2, A10 etc sortable...
-    m = re.match(r'(\D+)(\d+["\']?)\Z', x)
-    if m is not None:
+    if (m := re.match(r'(\D+)(\d+["\']?)\Z', x)) is not None:
         return (alpha, m.group(1) + m.group(2).zfill(15))
 
     si_values = {
         'B': 1, 'K': 1000, 'M': 1000000, 'G': 1000000000, 'T': 1000000000000,
         'KB': 1024, 'MB': 1048576, 'GB': 1073741824, 'TB': 1099511627776,
         'KIB': 1024, 'MIB': 1048576, 'GIB': 1073741824, 'TIB': 1099511627776,
     }
-    m = re.match(r'(\d+\.\d*|\.?\d+)\s?([BKMGT](I?B)?)', x)
-    if m is not None:
+    if (m := re.match(r'(\d+\.\d*|\.?\d+)\s?([BKMGT](I?B)?)', x)) is not None:
         return (float(m.group(1)) * si_values.get(m.group(2), 1), x)
 
     # remove leading articles (Library sort)
     words = x.split()
     if len(words) > 1 and words.pop(0) in ('A', 'AN', 'THE'):
         return (alpha, ' '.join(words))
 
@@ -262,21 +280,29 @@
         return (True, decimal.Decimal(trial_number))
     except ArithmeticError:
         pass
 
     return (False, sss)
 
 
-def as_decimal(n, na_value=decimal.Decimal('0')):
-    "Make this a decimal"
+def as_decimal(n=0, na_value=decimal.Decimal('0')):
+    '''Make this a decimal
+
+    >>> as_decimal('123.45')
+    Decimal('123.45')
+    >>> as_decimal()
+    Decimal('0')
+    >>> as_decimal('1E234')
+    Decimal('1E+234')
+    >>> as_decimal('1E2341412541245251234534')
+    Decimal('0')
+    '''
     try:
-        return decimal.Decimal(n) + 0
-    except decimal.Overflow:
-        return na_value
-    except decimal.InvalidOperation:
+        return decimal.Decimal(n)
+    except decimal.DecimalException:
         return na_value
 
 
 def siggy(s, n):
     '''Reduce to n sig figs
     >>> siggy('1,234', 2)
     '1200'
@@ -710,26 +736,28 @@
 
     def parse_lines(self, lines_thing, splitter=re.compile(r'\s\s+'), splits=0, append=False):
         "Read lines from an iterable thing, and append to self"
 
         if not append:
             self.clear()
             self.indent = 99
+
         for raw_line in lines_thing:
             raw_line = raw_line.replace("\t", "    ")
             stripped_line = raw_line.strip()
             if not stripped_line:
                 self.add_blank()
             elif set(stripped_line) == {'-'}:
                 self.add_rule()
             elif stripped_line.startswith('#'):
                 self.add_comment(stripped_line)
             else:
                 self.append(splitter.split(stripped_line, maxsplit=splits))
-                self.indent = min(self.indent, len(raw_line) - len(raw_line.lstrip()))
+                if not append:
+                    self.indent = min(self.indent, len(raw_line) - len(raw_line.lstrip()))
         # catch empty tables
         if not self.data:
             self.indent = 0
 
     def parse_lol(self, list_of_iterables, append=False, filler=''):
         "pass lol into self.data"
         if not append:
@@ -783,15 +811,16 @@
         if n < self.cols:
             row.extend([filler] * (self.cols - n))
         elif self.cols < n:
             for r in self.data:
                 r.extend([filler] * (n - self.cols))
             self.cols = n
 
-        # they should all be strings, and normalize space in last column...
+        # if there are any cells in the new row, then insert at "i"
+        # make sure values are strings, and normalize space in last cell
         if n > 0:
             self.data.insert(i, [str(x) for x in row[:-1]] + [' '.join(str(row[-1]).split())])
 
     def copy(self):
         "Implement the standard copy method"
         return self.data[:]
 
@@ -1033,33 +1062,30 @@
     def _fix_sigfigs(self, sf_string):
         "Round to n sig figs all the numeric fields in each row"
         self._apply_formats(sf_string, siggy)
 
     def _generate_new_rows(self, count_or_range):
         "Add some more data on the bottom"
 
-        m = re.match(r'([-+]?\d+)', count_or_range)
-        if m is not None:
+        if (m := re.match(r'([-+]?\d+)', count_or_range)) is not None:
             alpha = int(m.group(1))
 
-            m = re.match(r'(?:[-+]?\d+)(?:\D+?)([-+]?\d+)$', count_or_range)
-            if m is not None:
+            if (m := re.match(r'(?:[-+]?\d+)(?:\D+?)([-+]?\d+)$', count_or_range)) is not None:
                 omega = int(m.group(1))
             else:
                 omega = 1
 
             if alpha > omega:
                 (alpha, omega) = (omega, alpha)
 
             self.parse_lol(list([x] for x in range(alpha, omega + 1)), append=True)
             return
 
         # Labels * Cols...
-        m = re.match(r'([A-Za-z]+)(\d)?$', count_or_range)
-        if m is not None:
+        if (m := re.match(r'([A-Za-z]+)(\d)?$', count_or_range)) is not None:
             labels = m.group(1)
             columns = 1 if m.group(2) is None else int(m.group(2))
             self.parse_lol(list([*x] for x in itertools.product(labels, repeat=columns)), append=True)
             return
 
     def _copy_down(self, marker):
         '''Fix up ditto marks'''
@@ -1229,26 +1255,26 @@
 
         pivot_functions_for = {
             'wide': (builtins.sum, as_decimal),
             'sum': (builtins.sum, as_decimal),
             'count': (builtins.len, as_decimal),
             'mean': (lambda a: statistics.mean(a) if a else 'NA', as_decimal),
             'any': (builtins.any, as_decimal),
-            'first': (lambda a: a[0] if a else '-', str),
-            'string': (lambda a: a[0] if a else '-', str),
-            'last': (lambda a: a[-1] if a else '-', str),
+            'alpha': (lambda a: a[0] if a else '-', str),
+            'omega': (lambda a: a[-1] if a else '-', str),
         }
 
+        shape = shape.lower()
+
         for k in pivot_functions_for:
-            if k.startswith(shape.lower()):
+            if k.startswith(shape):
                 self._wrangle_wide(*pivot_functions_for[k])
                 return
 
-        m = re.match(r'long([1-9a-o])?$', shape)
-        if m is None:
+        if (m := re.match(r'long([1-9a-o])?$', shape)) is None:
             return
 
         if m.group(1) is None:
             last_key_col = 1
         else:
             try:
                 last_key_col = int(m.group(1))
@@ -1731,33 +1757,31 @@
             out = []
             for j, cell in enumerate(row):
                 out.append(f'{cell:{aligns[j]}{widths[j]}}')
 
             yield ' ' * self.indent + separator.join(out).rstrip() + eol_marker  # no trailing blanks
 
 
-def filter(argv=sys.argv[1:]):
+def filter():
     parser = argparse.ArgumentParser()
     parser.add_argument("agenda", nargs='*', help="[delimiter.maxsplit] [verb [option]]...")
     parser.add_argument("--file", help="Source file name, defaults to STDIN")
     args = parser.parse_args()
 
     # Join the agenda args into one string, remove any backslash (for Vim),
     # and split into a list
     agenda = ' '.join(args.agenda).replace('\\', '').split()
 
     # Get the delimiter from the agenda if possible
-    
-
     try:
         delim = agenda.pop(0)
     except IndexError:
         delim = ''
     else:
-        # If the removed delim is starts with alphabetic, put it back and reset delim to None
+        # If the removed delim starts with alphabetic, put it back and reset delim to None
         if re.match(r'^[a-zA-Z]', delim):
             agenda.insert(0, delim)
             delim = ''
 
     table = Table()
     fh = open(args.file) if args.file else io.StringIO("" if sys.stdin.isatty() else sys.stdin.read())
 
@@ -1786,26 +1810,27 @@
             table.parse_lol(csv.reader(fh, dialect), filler='-')
         except csv.Error:
             fh.seek(0)
             table.parse_lol(csv.reader(fh))
 
     else:
         # check for a maxsplit spec ".3", "2.4" etc
-        mm = re.match(r'(\d*)\.(\d+)', delim)
-        if mm is not None:
-            delim = mm.group(1)
+        if (m := re.match(r'(\d*)\.(\d+)', delim)) is not None:
+            delim = m.group(1)
             if delim == '':
                 delim = '2'
-            cell_limit = int(mm.group(2))
+            cell_limit = int(m.group(2))
         else:
             cell_limit = 0
+
         if delim.isdigit():
             in_sep = re.compile(rf'\s{{{delim},}}')
         else:
             in_sep = re.compile(re.escape(delim))
+
         table.parse_lines(fh, splitter=in_sep, splits=cell_limit)
 
     table.do(agenda)
     print(table)
 
     if args.file is not None:
         fh.close()
```

### Comparing `tablinum-0.1.2/tests/test_tab_calculation.py` & `tablinum-0.1.3/tests/test_tab_calculation.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,7 +274,37 @@
         self.assertEqual(str(self.tab), '''
 1   2  0.333333333333
 2   5  0.266666666667
 3   8            0.25
 4  11  0.242424242424
 5  14  0.238095238095
 '''.strip())
+
+
+    def test_shorthand_substitutions(self):
+        self.tab.do("clear gen 1:5 arr a(4214a) arr ab(b mod 23)")
+        self.assertEqual(str(self.tab), '''
+1   4214   5
+2   8428  10
+3  12642  15
+4  16856  20
+5  21070   2
+'''.strip())
+
+        self.tab.do("arr ~(c<>15)")
+        self.assertEqual(str(self.tab), '''
+1   4214   5   True
+2   8428  10   True
+3  12642  15  False
+4  16856  20   True
+5  21070   2   True
+'''.strip())
+
+        self.tab.do("arr a(b mod 100)c arr abc(b++c)")
+        self.assertEqual(str(self.tab), '''
+1  14   5  14.8660687473
+2  28  10  29.7321374946
+3  42  15  44.5982062420
+4  56  20  59.4642749893
+5  70   2  70.0285656000
+'''.strip())
+
```

### Comparing `tablinum-0.1.2/tests/test_tab_command_line.py` & `tablinum-0.1.3/tests/test_tab_command_line.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/tests/test_tab_contingency.py` & `tablinum-0.1.3/tests/test_tab_contingency.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/tests/test_tab_filter.py` & `tablinum-0.1.3/tests/test_tab_filter.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/tests/test_tab_grouping.py` & `tablinum-0.1.3/tests/test_tab_grouping.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/tests/test_tab_help.py` & `tablinum-0.1.3/tests/test_tab_help.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/tests/test_tab_levels.py` & `tablinum-0.1.3/tests/test_tab_levels.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/tests/test_tab_makers.py` & `tablinum-0.1.3/tests/test_tab_makers.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/tests/test_tab_parsing.py` & `tablinum-0.1.3/tests/test_tab_parsing.py`

 * *Files 13% similar despite different names*

```diff
@@ -105,14 +105,40 @@
     2020-05-19  09:20:00  29.8  29.7  28.6  25.5  25.2  25.3  23.9  17.2  1106  37.1
     2020-05-19  09:20:10  29.3  29.7  25.9  25.5  25.3  25.2  23.3  21.0  1189  40.6
     2020-05-19  09:20:20  30.1  29.8  27.1  25.0  25.3  24.1  22.7  21.7  1273  42.3
     2020-05-19  09:20:30  28.3  28.2  29.1  25.3  22.9  24.4  24.3  18.1  1375  48.6
     --------------------------------------------------------------------------------
     2020-05-19  09:20:40  28.3  28.6  22.5  22.3  24.1  23.7  19.7  23.0  1428  50.5''')
 
+        self.tab.parse_lines('''2020-05-19  09:18:00  30.3  30.2  30.1  28.9  29.8  29.6  29.9  30.2   135   4.5
+    2020-05-19  09:20:40  28.3  28.6  22.5  22.3  24.1  23.7  19.7  23.0  1428  50.5'''.splitlines(), append=True)
+
+        self.assertEqual(str(self.tab), '''# data has a long descriptive comment
+    2020-05-19  09:18:00  30.3  30.2  30.1  28.9  29.8  29.6  29.9  30.2   135   4.5
+    2020-05-19  09:18:10  29.2  29.1  29.4  30.5  30.2  30.3  30.0  29.5   132   4.5
+    2020-05-19  09:18:20  29.2  28.8  28.6  29.2  29.2  29.3  29.1  28.8   136   4.7
+    2020-05-19  09:18:30  31.2  31.6  31.2  29.6  29.2  29.1  29.2  29.3   155   5.0
+    2020-05-19  09:18:40  33.1  32.9  31.9  31.1  29.3  29.5  28.6  27.8   208   6.3
+    2020-05-19  09:18:50  29.1  29.2  30.2  31.0  31.8  31.2  31.9  30.2   197   6.8
+    2020-05-19  09:19:00  32.3  30.7  26.8  23.8  25.2  24.6  21.3  19.4   326  10.1
+    2020-05-19  09:19:10  31.4  33.1  26.2  20.2  14.5  15.6  12.9  14.6   494  15.7
+
+    2020-05-19  09:19:20  32.9  33.1  31.5  27.4  32.8  32.8  26.5  15.2   671  20.4
+    2020-05-19  09:19:30  30.9  30.9  26.3  25.0  24.8  24.9  23.9  25.1   729  23.6
+    2020-05-19  09:19:40  34.3  34.0  29.5  23.8  24.0  24.1  22.6  20.3   869  25.3
+    2020-05-19  09:19:50  31.0  30.9  28.2  26.6  26.0  25.8  19.4  19.9   980  31.6
+    2020-05-19  09:20:00  29.8  29.7  28.6  25.5  25.2  25.3  23.9  17.2  1106  37.1
+    2020-05-19  09:20:10  29.3  29.7  25.9  25.5  25.3  25.2  23.3  21.0  1189  40.6
+    2020-05-19  09:20:20  30.1  29.8  27.1  25.0  25.3  24.1  22.7  21.7  1273  42.3
+    2020-05-19  09:20:30  28.3  28.2  29.1  25.3  22.9  24.4  24.3  18.1  1375  48.6
+    --------------------------------------------------------------------------------
+    2020-05-19  09:20:40  28.3  28.6  22.5  22.3  24.1  23.7  19.7  23.0  1428  50.5
+    2020-05-19  09:18:00  30.3  30.2  30.1  28.9  29.8  29.6  29.9  30.2   135   4.5
+    2020-05-19  09:20:40  28.3  28.6  22.5  22.3  24.1  23.7  19.7  23.0  1428  50.5''')
+
     def test_tex(self):
         "parse TeX source"
 
         self.tab.parse_tex(r'''This&3&4\cr
 % ignore this comment
 The other & 34 & 91 \cr
 \noalign{\medskip}
@@ -140,11 +166,31 @@
 This        3    4
 The other  34   91
 The other  34   91
 ------------------
 Total      71  186
 '''.strip())
 
+        self.tab.pop()
+        self.tab.extras.clear()
+
+        self.tab.parse_tex(r'''
+More of it & 42 & 30 \\
+And again\\
+'''.strip().splitlines(), append=True)
+
+        self.tab.do("rule add")
+
+        self.assertEqual(str(self.tab), '''
+This          3    4
+The other    34   91
+The other    34   91
+More of it   42   30
+And again
+--------------------
+Total       113  216
+'''.strip())
+
     def test_nothing(self):
         self.nulltab = tablinum.Table()
         self.nulltab.parse_lines("")
         self.assertEqual(str(self.nulltab), '')
```

### Comparing `tablinum-0.1.2/tests/test_tab_poppers_and_adders.py` & `tablinum-0.1.3/tests/test_tab_poppers_and_adders.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/tests/test_tab_roller.py` & `tablinum-0.1.3/tests/test_tab_roller.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/tests/test_tab_sort.py` & `tablinum-0.1.3/tests/test_tab_sort.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,46 @@
 Wednesday  0.91  0.17
 Thursday   0.22  0.94
 Friday     0.94  0.28
 Saturday   0.62  0.02
 Sunday     0.34  0.25
 '''.strip()
 
+
+        self.addresses = '''
+Mac                IP
+00:01:E6:2C:42:1D  192.168.0.12
+3C:07:54:3D:3F:82  192.168.0.13
+60:C5:47:21:D7:E9  192.168.0.16
+2C:4D:54:74:A4:D8  192.168.0.4
+50:C7:BF:1C:88:66  192.168.0.3
+74:D0:2B:5D:CD:C0  192.168.0.2
+'''.strip()
+
+        self.addresses_by_A = '''
+Mac                IP
+00:01:E6:2C:42:1D  192.168.0.12
+2C:4D:54:74:A4:D8  192.168.0.4
+3C:07:54:3D:3F:82  192.168.0.13
+50:C7:BF:1C:88:66  192.168.0.3
+60:C5:47:21:D7:E9  192.168.0.16
+74:D0:2B:5D:CD:C0  192.168.0.2
+'''.strip()
+
+        self.addresses_by_B = '''
+Mac                IP
+74:D0:2B:5D:CD:C0  192.168.0.2
+50:C7:BF:1C:88:66  192.168.0.3
+2C:4D:54:74:A4:D8  192.168.0.4
+00:01:E6:2C:42:1D  192.168.0.12
+3C:07:54:3D:3F:82  192.168.0.13
+60:C5:47:21:D7:E9  192.168.0.16
+'''.strip()
+        
+
     def test_filter(self):
         "Select matching rows"
         self.tab.parse_lines(self.rain.splitlines())
         self.tab.do('sort')  # missing predicate does nothing because we start sorted
         self.assertEqual(str(self.tab), self.rain)
         self.tab.do('sort j')
         expected = '''
@@ -186,7 +218,15 @@
 Wednesday  0.91  0.17
 Thursday   0.22  0.94
 Friday     0.94  0.28
 Saturday   0.62  0.02
 Sunday     0.34  0.25
 '''.strip())
 
+
+    def test_special_sorts(self):
+        "Smart sorting"
+        self.tab.parse_lines(self.addresses.splitlines())
+        self.tab.do('sort') 
+        self.assertEqual(str(self.tab), self.addresses_by_A)
+        self.tab.do('sort b')
+        self.assertEqual(str(self.tab), self.addresses_by_B)
```

### Comparing `tablinum-0.1.2/tests/test_tab_text_manip.py` & `tablinum-0.1.3/tests/test_tab_text_manip.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/tests/test_tab_wrangler.py` & `tablinum-0.1.3/tests/test_tab_wrangler.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,19 +99,19 @@
         self.assertEqual(str(self.tab), summer)
 
         self.tab.parse_lines(sales.splitlines())
         self.tab.do("pivot mean")
         self.assertEqual(str(self.tab), summer)
 
         self.tab.parse_lines(sales.splitlines())
-        self.tab.do("pivot first")
+        self.tab.do("pivot alpha")
         self.assertEqual(str(self.tab), summer)
 
         self.tab.parse_lines(sales.splitlines())
-        self.tab.do("pivot string")
+        self.tab.do("pivot omega")
         self.assertEqual(str(self.tab), summer)
 
         self.tab.parse_lines(sales.splitlines())
         self.tab.do("pivot count")
         self.assertEqual(str(self.tab), counter)
 
         self.tab.parse_lines(sales.splitlines())
```

### Comparing `tablinum-0.1.2/tests/test_tablinum.py` & `tablinum-0.1.3/tests/test_tablinum.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,25 @@
     2020-05-19  09:18:10  29.4   4.5
     2020-05-19  09:18:20  28.6   4.7
     2020-05-19  09:18:30  31.2   5.0
     2020-05-19  09:18:40  31.9   6.3
     2020-05-19  09:20:30  29.1  48.6
     2020-05-19  09:20:40  22.5  50.5
 ''')
+        self.tab.do("arr -1")
+        self.assertEqual(str(self.tab) + "\n", '''Only lowercase ASCII allowed after -
+
+    2020-05-19  09:18:00  30.1   4.5
+    2020-05-19  09:18:10  29.4   4.5
+    2020-05-19  09:18:20  28.6   4.7
+    2020-05-19  09:18:30  31.2   5.0
+    2020-05-19  09:18:40  31.9   6.3
+    2020-05-19  09:20:30  29.1  48.6
+    2020-05-19  09:20:40  22.5  50.5
+''')
 
     def test_arrange_C(self):
         self.tab.parse_lines('''
     2020-05-19  09:18:00  30.3  30.2  30.1  28.9  29.8  29.6  29.9  30.2   135   4.5
     2020-05-19  09:18:10  29.2  29.1  29.4  30.5  30.2  30.3  30.0  29.5   132   4.5
     2020-05-19  09:18:20  29.2  28.8  28.6  29.2  29.2  29.3  29.1  28.8   136   4.7
     2020-05-19  09:18:30  31.2  31.6  31.2  29.6  29.2  29.1  29.2  29.3   155   5.0
```

### Comparing `tablinum-0.1.2/.gitignore` & `tablinum-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/LICENSE` & `tablinum-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/README.md` & `tablinum-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.2/pyproject.toml` & `tablinum-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tablinum"
 dynamic = ["version"]
-description = ''
+description = 'Tablinum is a Python library to make, manipulate, and neatly print tabular output to the console.'
+long_description = '''Tablinum is an exportable module that will line up tabular material automatically,
+and so save you hours of time faffing about with format and alignment.  As a script
+it provides a filter with a simple DSL (domain-specific language) that can be used
+to make and manipulate tables in editors that support external filters (such as Vim).'''
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Toby Thurston", email = "toby.thurston@gmail.com" },
 ]
@@ -78,7 +82,14 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.pytest.ini_options]
+ addopts = [
+     '--import-mode=importlib',
+     '--doctest-modules',
+     '--pyargs',
+ ]
```

### Comparing `tablinum-0.1.2/PKG-INFO` & `tablinum-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.3
 Name: tablinum
-Version: 0.1.2
+Version: 0.1.3
+Summary: Tablinum is a Python library to make, manipulate, and neatly print tabular output to the console.
 Project-URL: Documentation, https://github.com/unknown/tablinum#readme
 Project-URL: Issues, https://github.com/unknown/tablinum/issues
 Project-URL: Source, https://github.com/unknown/tablinum
 Author-email: Toby Thurston <toby.thurston@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

