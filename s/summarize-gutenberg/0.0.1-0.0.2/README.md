# Comparing `tmp/summarize_gutenberg-0.0.1.tar.gz` & `tmp/summarize_gutenberg-0.0.2.tar.gz`

## Comparing `summarize_gutenberg-0.0.1.tar` & `summarize_gutenberg-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/pytest.ini
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/requirements.in
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/src/summarize_gutenberg/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/src/summarize_gutenberg/__main__.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/src/summarize_gutenberg/api.py
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/src/summarize_gutenberg/cli.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/src/summarize_gutenberg/db.py
--rw-r--r--   0        0        0    12311 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/src/summarize_gutenberg/demo.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/src/summarize_gutenberg/get_books.py
--rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/src/summarize_gutenberg/get_text.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/src/summarize_gutenberg/make_summary.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/tests/test_author_parse.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/tests/test_booksdb.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/tests/test_create_filename.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/tests/test_get_books.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/tests/test_models.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/LICENSE
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/README.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    47564 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/pytest.ini
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/requirements.in
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/__main__.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/api.py
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/cli.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/db.py
+-rw-r--r--   0        0        0    12311 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/demo.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/get_books.py
+-rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/get_text.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/src/summarize_gutenberg/make_summary.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/test_author_parse.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/test_booksdb.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/test_create_filename.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/test_get_books.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/tests/test_models.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/README.md
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    47604 2020-02-02 00:00:00.000000 summarize_gutenberg-0.0.2/PKG-INFO
```

### Comparing `summarize_gutenberg-0.0.1/requirements.txt` & `summarize_gutenberg-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/src/summarize_gutenberg/api.py` & `summarize_gutenberg-0.0.2/src/summarize_gutenberg/api.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/src/summarize_gutenberg/cli.py` & `summarize_gutenberg-0.0.2/src/summarize_gutenberg/cli.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/src/summarize_gutenberg/db.py` & `summarize_gutenberg-0.0.2/src/summarize_gutenberg/db.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/src/summarize_gutenberg/demo.py` & `summarize_gutenberg-0.0.2/src/summarize_gutenberg/demo.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/src/summarize_gutenberg/get_books.py` & `summarize_gutenberg-0.0.2/src/summarize_gutenberg/get_books.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/src/summarize_gutenberg/get_text.py` & `summarize_gutenberg-0.0.2/src/summarize_gutenberg/get_text.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/src/summarize_gutenberg/make_summary.py` & `summarize_gutenberg-0.0.2/src/summarize_gutenberg/make_summary.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/tests/test_author_parse.py` & `summarize_gutenberg-0.0.2/tests/test_author_parse.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/tests/test_booksdb.py` & `summarize_gutenberg-0.0.2/tests/test_booksdb.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/tests/test_create_filename.py` & `summarize_gutenberg-0.0.2/tests/test_create_filename.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/tests/test_get_books.py` & `summarize_gutenberg-0.0.2/tests/test_get_books.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/tests/test_models.py` & `summarize_gutenberg-0.0.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/.gitignore` & `summarize_gutenberg-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/LICENSE` & `summarize_gutenberg-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `summarize_gutenberg-0.0.1/README.md` & `summarize_gutenberg-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # Summarize: generate abstractive summaries from Project Gutenberg books
 
 ### About the app
-Summarize is a CLI app written in **Python 3.12.1**. The CLI uses **Typer** and **Rich** for beautiful rich-text output. The app uses the [Gutendex API](https://gutendex.com/) to retrieve books from Project Gutenberg and the pszemraj's [pegasus-x-large-book-summary](https://huggingface.co/pszemraj/pegasus-x-large-book-summary) LLM to generate abstractive summaries. The user can save summaries to a .txt file or print them to stdout for further piping.
+Summarize is a CLI app written in **Python 3.12**. The CLI uses **Typer** and **Rich** for beautiful rich-text output. The app uses the [Gutendex API](https://gutendex.com/) to retrieve books from Project Gutenberg and the pszemraj's [pegasus-x-large-book-summary](https://huggingface.co/pszemraj/pegasus-x-large-book-summary) LLM to generate abstractive summaries. The user can save summaries to a .txt file or print them to stdout for further piping.
 
-### Local installation
-Eventually Summarize will be packaged on pypi, but for now you can install it by cloning from Github. You'll need Python 3.12 or later installed.
-1. [Clone this repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository).
-2. Navigate to the 'summarize' directory.
-3. Create a virtual environment ```python -m venv venv``` (Windows/Linux) or ```python3 -m venv venv``` (Mac).
-4. Activate the virtual environment ```.\venv\Scripts\activate``` (Windows) or ```source venv/bin/activate```
-5. Install the necessary packages: ```pip install -r requirements.txt``` (There is also a requirements.in if you prefer to use pip-tools)
+### Installation
+Summarize is available as a package on PyPI! You'll need Python 3.12 or later installed.
+1. Navigate to the directory where you want to install Summarize.
+2. Create a virtual environment: ```python -m venv venv``` (Windows/Linux) or ```python3 -m venv venv``` (Mac).
+3. Activate the virtual environment: ```.\venv\Scripts\activate``` (Windows) or ```source venv/bin/activate``` (Linux/Mac).
+4. Install summarize: ```pip install summarize-gutenberg```
 
 ### Running the app
 At present the app retrieves the top 32 books from Project Gutenberg and offers the user a choice among them. Here's how to use it:
 1. Make sure your virtual environment is activated.
-2. Run ```python src/summarize/__main__.py```
+2. Type ```summarize```
 3. Follow the onscreen prompts to create your summary!
 
 ### A note on chunks
-Summarize works by breaking the source text into chunks of a given number of lines; you can specify how many lines per chunk the program works on. In theory the LLM should work with very large chunks, but experience has shown that a range of 200-800 works best. Please note that the smaller the chunk size, the longer the program will take to run!
+Summarize works by breaking the source text into chunks of a given number of lines; you can specify how many lines per chunk the program works on. In theory the LLM should work with very large chunks or even entire texts, but experience has shown that a range of 200-800 works best. Please note that the smaller the chunk size, the longer the program will take to run!
 
 ### Sample output
 [Kafka's *The Metamorphosis*](https://en.wikipedia.org/wiki/The_Metamorphosis), 400 lines per chunk:
 
 > One morning, Samsa wakes from a nightmare and finds himself transformed into a "horrid vermin" in his bed. He is a traveling salesman, and his room is small, but it is comfortable. A picture hangs above the table, showing a woman wearing a hat and a boa. Samsa thinks about how hard it is to be a salesman, how he has to travel all over the world, and how he can never be friendly with anyone. He feels a slight itch on his belly, and pushes himself up onto the bed to lift his head. When he touches the bed, he is overcome by a "cold shudder". He thinks about getting up early, but he knows that other salesmen live a "life of luxury" and that he would get kicked out of his job if he did not have his parents to worry about. He decides that he will pay off his parents' debt, and then he will make the big decision to quit his job. He looks over at the clock, which is ticking past six, and wonders if he could have slept peacefully through the furniture-ratting noise.The next morning, the chief clerk tells Gregor that he has to leave immediately. He tells him that he is in debt to his employer and must look after his parents and sister.The chapter opens with a loud "No" from the family. It's five years later, and the family is still broke. They've lost everything, but they're still able to scrape together enough money to send their sister to the conservatory. The narrator tells us that this is the first time that the family has heard anything positive about their financial situation since the business collapsed five years ago. The family is overjoyed, and they've even gotten used to the idea of having to pay for the expenses of the house. But now that the business is gone, the family can't afford to go back to the good old days. So, they'll have to work.The chapter opens with a description of the situation in which the family finds itself. The family is in the middle of a heated argument when an apple flies through the air and lands on the floor. It is an apple that has been thrown at the family, and it is the apple that is lodged in the flesh of Gregor. The apple is a reminder of the family's reaction to the accident, and the family does not treat the apple as an enemy, but rather as a reminder that the family is patient with its son. The chapter ends with a comparison between the family and a hotel room. The hotel room was a place where the family would gather and talk, but now the family has moved to the bedroom, where they can only talk in the dark.The monster is back, and it's not going to stop until they get rid of him. It's going to take a long time, and they're going to have to live with it for the rest of their lives.
 
+### Planned additional features
+There are two major features still to be implemented. The first is a search function allowing you to retrieve any book from Project Gutenberg. The second is a full set of command-line options to control program flow.
+
 ### License
-Summarize is [free software](https://www.fsf.org/about/what-is-free-software), released under version 3.0 of the GPL. Everyone has the right to use, modify, and distribute Summarize subject to the [stipulations](https://github.com/jwjacobson/summarize/blob/main/LICENSE) of that license.
+Summarize is [free software](https://www.fsf.org/about/what-is-free-software), released under version 3.0 of the GPL. Everyone has the right to use, modify, and distribute Summarize subject to the [stipulations](https://github.com/jwjacobson/summarize/blob/main/LICENSE) of that license. Contributions are welcome!
 
 ### Acknowledgments
 The overall structure of the app is inspired by Brian Okken's [cards](https://github.com/okken/cards).
 The UI and (eventual) search functionality are inspired by [pybites-search](https://github.com/PyBites-Open-Source/search).
 The tone of user messages is doubtless inspired by countless hours of [Dungeon Crawl Stone Soup](https://crawl.develz.org/) over the years.
```

### Comparing `summarize_gutenberg-0.0.1/pyproject.toml` & `summarize_gutenberg-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "summarize_gutenberg"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
     "tinydb",
     "requests",
     "rich",
     "typer",
     "transformers",
     "torch",
 ]
 requires-python = ">=3.12"
 authors = [
   { name="Jeff Jacobson", email="jeffjacobsonhimself@gmail.com" },
 ]
-description = "A jazz repertoire management app"
+description = "Generate abstractive summaries of Project Gutenberg tests"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["abstractive summary", "literature", "books", "LLM", "Pegasus"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
-    "Framework :: Pytest",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
```

### Comparing `summarize_gutenberg-0.0.1/PKG-INFO` & `summarize_gutenberg-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: summarize_gutenberg
-Version: 0.0.1
-Summary: A jazz repertoire management app
+Version: 0.0.2
+Summary: Generate abstractive summaries of Project Gutenberg tests
 Project-URL: Homepage, https://github.com/jwjacobson/summarize
 Project-URL: Issues, https://github.com/jwjacobson/summarize/issues
 Author-email: Jeff Jacobson <jeffjacobsonhimself@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -679,15 +679,14 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 License-File: LICENSE
 Keywords: LLM,Pegasus,abstractive summary,books,literature
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
-Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -713,38 +712,40 @@
 Requires-Dist: pre-commit; extra == 'tools'
 Requires-Dist: ruff; extra == 'tools'
 Description-Content-Type: text/markdown
 
 # Summarize: generate abstractive summaries from Project Gutenberg books
 
 ### About the app
-Summarize is a CLI app written in **Python 3.12.1**. The CLI uses **Typer** and **Rich** for beautiful rich-text output. The app uses the [Gutendex API](https://gutendex.com/) to retrieve books from Project Gutenberg and the pszemraj's [pegasus-x-large-book-summary](https://huggingface.co/pszemraj/pegasus-x-large-book-summary) LLM to generate abstractive summaries. The user can save summaries to a .txt file or print them to stdout for further piping.
+Summarize is a CLI app written in **Python 3.12**. The CLI uses **Typer** and **Rich** for beautiful rich-text output. The app uses the [Gutendex API](https://gutendex.com/) to retrieve books from Project Gutenberg and the pszemraj's [pegasus-x-large-book-summary](https://huggingface.co/pszemraj/pegasus-x-large-book-summary) LLM to generate abstractive summaries. The user can save summaries to a .txt file or print them to stdout for further piping.
 
-### Local installation
-Eventually Summarize will be packaged on pypi, but for now you can install it by cloning from Github. You'll need Python 3.12 or later installed.
-1. [Clone this repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository).
-2. Navigate to the 'summarize' directory.
-3. Create a virtual environment ```python -m venv venv``` (Windows/Linux) or ```python3 -m venv venv``` (Mac).
-4. Activate the virtual environment ```.\venv\Scripts\activate``` (Windows) or ```source venv/bin/activate```
-5. Install the necessary packages: ```pip install -r requirements.txt``` (There is also a requirements.in if you prefer to use pip-tools)
+### Installation
+Summarize is available as a package on PyPI! You'll need Python 3.12 or later installed.
+1. Navigate to the directory where you want to install Summarize.
+2. Create a virtual environment: ```python -m venv venv``` (Windows/Linux) or ```python3 -m venv venv``` (Mac).
+3. Activate the virtual environment: ```.\venv\Scripts\activate``` (Windows) or ```source venv/bin/activate``` (Linux/Mac).
+4. Install summarize: ```pip install summarize-gutenberg```
 
 ### Running the app
 At present the app retrieves the top 32 books from Project Gutenberg and offers the user a choice among them. Here's how to use it:
 1. Make sure your virtual environment is activated.
-2. Run ```python src/summarize/__main__.py```
+2. Type ```summarize```
 3. Follow the onscreen prompts to create your summary!
 
 ### A note on chunks
-Summarize works by breaking the source text into chunks of a given number of lines; you can specify how many lines per chunk the program works on. In theory the LLM should work with very large chunks, but experience has shown that a range of 200-800 works best. Please note that the smaller the chunk size, the longer the program will take to run!
+Summarize works by breaking the source text into chunks of a given number of lines; you can specify how many lines per chunk the program works on. In theory the LLM should work with very large chunks or even entire texts, but experience has shown that a range of 200-800 works best. Please note that the smaller the chunk size, the longer the program will take to run!
 
 ### Sample output
 [Kafka's *The Metamorphosis*](https://en.wikipedia.org/wiki/The_Metamorphosis), 400 lines per chunk:
 
 > One morning, Samsa wakes from a nightmare and finds himself transformed into a "horrid vermin" in his bed. He is a traveling salesman, and his room is small, but it is comfortable. A picture hangs above the table, showing a woman wearing a hat and a boa. Samsa thinks about how hard it is to be a salesman, how he has to travel all over the world, and how he can never be friendly with anyone. He feels a slight itch on his belly, and pushes himself up onto the bed to lift his head. When he touches the bed, he is overcome by a "cold shudder". He thinks about getting up early, but he knows that other salesmen live a "life of luxury" and that he would get kicked out of his job if he did not have his parents to worry about. He decides that he will pay off his parents' debt, and then he will make the big decision to quit his job. He looks over at the clock, which is ticking past six, and wonders if he could have slept peacefully through the furniture-ratting noise.The next morning, the chief clerk tells Gregor that he has to leave immediately. He tells him that he is in debt to his employer and must look after his parents and sister.The chapter opens with a loud "No" from the family. It's five years later, and the family is still broke. They've lost everything, but they're still able to scrape together enough money to send their sister to the conservatory. The narrator tells us that this is the first time that the family has heard anything positive about their financial situation since the business collapsed five years ago. The family is overjoyed, and they've even gotten used to the idea of having to pay for the expenses of the house. But now that the business is gone, the family can't afford to go back to the good old days. So, they'll have to work.The chapter opens with a description of the situation in which the family finds itself. The family is in the middle of a heated argument when an apple flies through the air and lands on the floor. It is an apple that has been thrown at the family, and it is the apple that is lodged in the flesh of Gregor. The apple is a reminder of the family's reaction to the accident, and the family does not treat the apple as an enemy, but rather as a reminder that the family is patient with its son. The chapter ends with a comparison between the family and a hotel room. The hotel room was a place where the family would gather and talk, but now the family has moved to the bedroom, where they can only talk in the dark.The monster is back, and it's not going to stop until they get rid of him. It's going to take a long time, and they're going to have to live with it for the rest of their lives.
 
+### Planned additional features
+There are two major features still to be implemented. The first is a search function allowing you to retrieve any book from Project Gutenberg. The second is a full set of command-line options to control program flow.
+
 ### License
-Summarize is [free software](https://www.fsf.org/about/what-is-free-software), released under version 3.0 of the GPL. Everyone has the right to use, modify, and distribute Summarize subject to the [stipulations](https://github.com/jwjacobson/summarize/blob/main/LICENSE) of that license.
+Summarize is [free software](https://www.fsf.org/about/what-is-free-software), released under version 3.0 of the GPL. Everyone has the right to use, modify, and distribute Summarize subject to the [stipulations](https://github.com/jwjacobson/summarize/blob/main/LICENSE) of that license. Contributions are welcome!
 
 ### Acknowledgments
 The overall structure of the app is inspired by Brian Okken's [cards](https://github.com/okken/cards).
 The UI and (eventual) search functionality are inspired by [pybites-search](https://github.com/PyBites-Open-Source/search).
 The tone of user messages is doubtless inspired by countless hours of [Dungeon Crawl Stone Soup](https://crawl.develz.org/) over the years.
```

