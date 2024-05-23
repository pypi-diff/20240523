# Comparing `tmp/summarize_gutenberg-0.0.2.tar.gz` & `tmp/summarize_gutenberg-0.0.3.tar.gz`

## Comparing `summarize_gutenberg-0.0.2.tar` & `summarize_gutenberg-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/pytest.ini
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/requirements.in
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/__main__.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/api.py
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/cli.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/db.py
--rw-r--r--   0        0        0    12311 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/demo.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/get_books.py
--rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/get_text.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/make_summary.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/test_author_parse.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/test_booksdb.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/test_create_filename.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/test_get_books.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/test_models.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/LICENSE
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/README.md
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    47604 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/pytest.ini
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/requirements.in
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/src/summarize_gutenberg/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/src/summarize_gutenberg/__main__.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/src/summarize_gutenberg/api.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/src/summarize_gutenberg/cli.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/src/summarize_gutenberg/db.py
+-rw-r--r--   0        0        0    12311 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/src/summarize_gutenberg/demo.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/src/summarize_gutenberg/get_books.py
+-rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/src/summarize_gutenberg/get_text.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/src/summarize_gutenberg/make_summary.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/tests/test_author_parse.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/tests/test_booksdb.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/tests/test_create_filename.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/tests/test_get_books.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/tests/test_models.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/README.md
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    47604 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.3/PKG-INFO
```

### Comparing `summarize_gutenberg-0.0.2/requirements.txt` & `summarize_gutenberg-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/src/summarize_gutenberg/api.py` & `summarize_gutenberg-0.0.3/src/summarize_gutenberg/api.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/src/summarize_gutenberg/cli.py` & `summarize_gutenberg-0.0.3/src/summarize_gutenberg/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,22 @@
 from summarize_gutenberg.get_text import write_text_to_file
 from summarize_gutenberg.make_summary import save_summary, print_summary
 from summarize_gutenberg.api import Book, BooksDB
 
 FILE_DIR = Path("./files/")
 SUMMARY_DIR = FILE_DIR / "summaries"
 
-app = typer.Typer()
+def dir_check():
+    """Make sure the directories for saving files exist"""
+    FILE_DIR.mkdir(parents=True, exist_ok=True)
+    SUMMARY_DIR.mkdir(parents=True, exist_ok=True)
+
+dir_check()
 
+app = typer.Typer()
 
 
 def get_default_books():
     """
     Get the default book info then populate the database with corresponding Book objects
     """
     print("\n[italic yellow]Retrieving default book data...")
```

### Comparing `summarize_gutenberg-0.0.2/src/summarize_gutenberg/db.py` & `summarize_gutenberg-0.0.3/src/summarize_gutenberg/db.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/src/summarize_gutenberg/demo.py` & `summarize_gutenberg-0.0.3/src/summarize_gutenberg/demo.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/src/summarize_gutenberg/get_books.py` & `summarize_gutenberg-0.0.3/src/summarize_gutenberg/get_books.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/src/summarize_gutenberg/get_text.py` & `summarize_gutenberg-0.0.3/src/summarize_gutenberg/get_text.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/src/summarize_gutenberg/make_summary.py` & `summarize_gutenberg-0.0.3/src/summarize_gutenberg/make_summary.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/tests/test_author_parse.py` & `summarize_gutenberg-0.0.3/tests/test_author_parse.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/tests/test_booksdb.py` & `summarize_gutenberg-0.0.3/tests/test_booksdb.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/tests/test_create_filename.py` & `summarize_gutenberg-0.0.3/tests/test_create_filename.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/tests/test_get_books.py` & `summarize_gutenberg-0.0.3/tests/test_get_books.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/tests/test_models.py` & `summarize_gutenberg-0.0.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/.gitignore` & `summarize_gutenberg-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/LICENSE` & `summarize_gutenberg-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/README.md` & `summarize_gutenberg-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.2/pyproject.toml` & `summarize_gutenberg-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "summarize_gutenberg"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
     "tinydb",
     "requests",
     "rich",
     "typer",
     "transformers",
     "torch",
```

### Comparing `summarize_gutenberg-0.0.2/PKG-INFO` & `summarize_gutenberg-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: summarize_gutenberg
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate abstractive summaries of Project Gutenberg tests
 Project-URL: Homepage, https://github.com/jwjacobson/summarize
 Project-URL: Issues, https://github.com/jwjacobson/summarize/issues
 Author-email: Jeff Jacobson <jeffjacobsonhimself@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

