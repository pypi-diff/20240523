# Comparing `tmp/scorify-0.9.3.tar.gz` & `tmp/scorify-2024.5.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scorify-0.9.3.tar", last modified: Thu May 21 15:51:58 2020, max compression
+gzip compressed data, was "scorify-2024.5.23.tar", last modified: Thu May 23 18:45:22 2024, max compression
```

## Comparing `scorify-0.9.3.tar` & `scorify-2024.5.23.tar`

### file list

```diff
@@ -1,37 +1,44 @@
-drwxrwxr-x   0 njvack     (501) staff       (20)        0 2020-05-21 15:51:58.000000 scorify-0.9.3/
--rw-rw-r--   0 njvack     (501) staff       (20)    13669 2020-05-21 15:51:58.000000 scorify-0.9.3/PKG-INFO
--rw-rw-r--   0 njvack     (501) staff       (20)    10498 2020-05-21 15:46:30.000000 scorify-0.9.3/README.md
-drwxrwxr-x   0 njvack     (501) staff       (20)        0 2020-05-21 15:51:58.000000 scorify-0.9.3/scorify/
--rw-rw-r--   0 njvack     (501) staff       (20)       85 2020-05-21 15:19:45.000000 scorify-0.9.3/scorify/__init__.py
--rw-rw-r--   0 njvack     (501) staff       (20)     3468 2020-05-18 21:24:02.000000 scorify-0.9.3/scorify/aggregators.py
--rw-rw-r--   0 njvack     (501) staff       (20)     3009 2020-05-18 21:24:00.000000 scorify-0.9.3/scorify/datafile.py
--rw-rw-r--   0 njvack     (501) staff       (20)     5317 2020-05-18 21:24:00.000000 scorify-0.9.3/scorify/directives.py
--rw-rw-r--   0 njvack     (501) staff       (20)      434 2020-05-18 21:24:00.000000 scorify-0.9.3/scorify/errors.py
--rw-rw-r--   0 njvack     (501) staff       (20)      681 2020-05-18 20:08:54.000000 scorify-0.9.3/scorify/excel_reader.py
--rw-rw-r--   0 njvack     (501) staff       (20)      261 2020-05-21 15:20:15.000000 scorify-0.9.3/scorify/info.py
--rw-rw-r--   0 njvack     (501) staff       (20)     4316 2020-05-18 21:24:00.000000 scorify-0.9.3/scorify/mappings.py
--rwxrwxr-x   0 njvack     (501) staff       (20)     5659 2020-05-18 21:24:00.000000 scorify-0.9.3/scorify/score_data.py
--rw-rw-r--   0 njvack     (501) staff       (20)     4067 2020-05-18 21:24:00.000000 scorify-0.9.3/scorify/scorer.py
--rw-rw-r--   0 njvack     (501) staff       (20)     9402 2020-05-18 21:24:00.000000 scorify-0.9.3/scorify/scoresheet.py
--rw-rw-r--   0 njvack     (501) staff       (20)      715 2020-05-18 21:24:00.000000 scorify-0.9.3/scorify/utils.py
-drwxrwxr-x   0 njvack     (501) staff       (20)        0 2020-05-21 15:51:58.000000 scorify-0.9.3/scorify.egg-info/
--rw-r--r--   0 njvack     (501) staff       (20)    13669 2020-05-21 15:51:57.000000 scorify-0.9.3/scorify.egg-info/PKG-INFO
--rw-r--r--   0 njvack     (501) staff       (20)      709 2020-05-21 15:51:57.000000 scorify-0.9.3/scorify.egg-info/SOURCES.txt
--rw-r--r--   0 njvack     (501) staff       (20)        1 2020-05-21 15:51:57.000000 scorify-0.9.3/scorify.egg-info/dependency_links.txt
--rw-r--r--   0 njvack     (501) staff       (20)       56 2020-05-21 15:51:57.000000 scorify-0.9.3/scorify.egg-info/entry_points.txt
--rw-rw-r--   0 njvack     (501) staff       (20)        1 2020-05-18 21:22:10.000000 scorify-0.9.3/scorify.egg-info/not-zip-safe
--rw-rw-r--   0 njvack     (501) staff       (20)       44 2020-05-21 15:51:57.000000 scorify-0.9.3/scorify.egg-info/requires.txt
--rw-r--r--   0 njvack     (501) staff       (20)       14 2020-05-21 15:51:57.000000 scorify-0.9.3/scorify.egg-info/top_level.txt
--rw-rw-r--   0 njvack     (501) staff       (20)     1136 2020-05-21 15:51:58.000000 scorify-0.9.3/setup.cfg
--rwxrwxr-x   0 njvack     (501) staff       (20)      529 2020-05-18 21:33:32.000000 scorify-0.9.3/setup.py
-drwxrwxr-x   0 njvack     (501) staff       (20)        0 2020-05-21 15:51:58.000000 scorify-0.9.3/tests/
--rw-rw-r--   0 njvack     (501) staff       (20)        0 2019-10-14 20:29:38.000000 scorify-0.9.3/tests/__init__.py
--rw-rw-r--   0 njvack     (501) staff       (20)      240 2019-10-14 20:29:38.000000 scorify-0.9.3/tests/base.py
--rw-r--r--   0 njvack     (501) staff       (20)     3368 2020-05-18 21:23:59.000000 scorify-0.9.3/tests/test_aggregators.py
--rw-rw-r--   0 njvack     (501) staff       (20)     5051 2020-05-18 21:23:59.000000 scorify-0.9.3/tests/test_datafile.py
--rw-rw-r--   0 njvack     (501) staff       (20)     1865 2020-05-18 21:23:59.000000 scorify-0.9.3/tests/test_directives.py
--rw-rw-r--   0 njvack     (501) staff       (20)     2200 2020-05-18 20:08:54.000000 scorify-0.9.3/tests/test_integration.py
--rw-r--r--   0 njvack     (501) staff       (20)     2792 2020-05-18 21:23:59.000000 scorify-0.9.3/tests/test_mappings.py
--rw-rw-r--   0 njvack     (501) staff       (20)     5470 2020-05-18 21:23:59.000000 scorify-0.9.3/tests/test_scorer.py
--rw-rw-r--   0 njvack     (501) staff       (20)     4612 2020-05-18 21:23:59.000000 scorify-0.9.3/tests/test_scoresheet.py
--rw-r--r--   0 njvack     (501) staff       (20)      479 2020-05-18 21:23:59.000000 scorify-0.9.3/tests/test_utils.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-23 18:45:22.894810 scorify-2024.5.23/
+-rw-r--r--   0 njvack     (501) staff       (20)     1121 2017-06-21 17:05:08.000000 scorify-2024.5.23/LICENSE
+-rw-r--r--   0 njvack     (501) staff       (20)    12893 2024-05-23 18:45:22.894680 scorify-2024.5.23/PKG-INFO
+-rw-r--r--   0 njvack     (501) staff       (20)    11776 2024-04-10 20:45:21.000000 scorify-2024.5.23/README.md
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-23 18:45:22.889270 scorify-2024.5.23/scorify/
+-rw-rw-r--   0 njvack     (501) staff       (20)       85 2020-05-21 15:19:45.000000 scorify-2024.5.23/scorify/__init__.py
+-rw-r--r--   0 njvack     (501) staff       (20)     3467 2024-05-15 20:38:47.000000 scorify-2024.5.23/scorify/aggregators.py
+-rw-r--r--   0 njvack     (501) staff       (20)     3167 2024-05-15 20:38:47.000000 scorify-2024.5.23/scorify/datafile.py
+-rw-r--r--   0 njvack     (501) staff       (20)     5302 2024-05-15 20:38:47.000000 scorify-2024.5.23/scorify/directives.py
+-rw-r--r--   0 njvack     (501) staff       (20)      443 2024-05-15 20:38:47.000000 scorify-2024.5.23/scorify/errors.py
+-rw-rw-r--   0 njvack     (501) staff       (20)      681 2020-05-18 20:08:54.000000 scorify-2024.5.23/scorify/excel_reader.py
+-rw-rw-r--   0 njvack     (501) staff       (20)      266 2024-05-23 18:37:00.000000 scorify-2024.5.23/scorify/info.py
+-rw-r--r--   0 njvack     (501) staff       (20)     4457 2024-05-15 20:38:47.000000 scorify-2024.5.23/scorify/mappings.py
+-rwxr-xr-x   0 njvack     (501) staff       (20)     8593 2024-04-10 20:45:21.000000 scorify-2024.5.23/scorify/reliability.py
+-rw-r--r--   0 njvack     (501) staff       (20)     4252 2024-05-15 20:38:47.000000 scorify-2024.5.23/scorify/scorer.py
+-rw-r--r--   0 njvack     (501) staff       (20)    10229 2024-05-15 20:38:47.000000 scorify-2024.5.23/scorify/scoresheet.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-23 18:45:22.891248 scorify-2024.5.23/scorify/scripts/
+-rw-r--r--   0 njvack     (501) staff       (20)        0 2024-04-15 21:35:50.000000 scorify-2024.5.23/scorify/scripts/__init__.py
+-rwxr-xr-x   0 njvack     (501) staff       (20)     5567 2024-05-15 20:38:47.000000 scorify-2024.5.23/scorify/scripts/score_data.py
+-rwxr-xr-x   0 njvack     (501) staff       (20)     5425 2024-05-15 21:14:43.000000 scorify-2024.5.23/scorify/scripts/score_multi.py
+-rw-r--r--   0 njvack     (501) staff       (20)      701 2024-05-15 20:38:47.000000 scorify-2024.5.23/scorify/utils.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-23 18:45:22.894441 scorify-2024.5.23/scorify.egg-info/
+-rw-r--r--   0 njvack     (501) staff       (20)    12893 2024-05-23 18:45:22.000000 scorify-2024.5.23/scorify.egg-info/PKG-INFO
+-rw-r--r--   0 njvack     (501) staff       (20)      859 2024-05-23 18:45:22.000000 scorify-2024.5.23/scorify.egg-info/SOURCES.txt
+-rw-r--r--   0 njvack     (501) staff       (20)        1 2024-05-23 18:45:22.000000 scorify-2024.5.23/scorify.egg-info/dependency_links.txt
+-rw-r--r--   0 njvack     (501) staff       (20)      163 2024-05-23 18:45:22.000000 scorify-2024.5.23/scorify.egg-info/entry_points.txt
+-rw-rw-r--   0 njvack     (501) staff       (20)        1 2020-05-18 21:22:10.000000 scorify-2024.5.23/scorify.egg-info/not-zip-safe
+-rw-rw-r--   0 njvack     (501) staff       (20)       74 2024-05-23 18:45:22.000000 scorify-2024.5.23/scorify.egg-info/requires.txt
+-rw-r--r--   0 njvack     (501) staff       (20)       14 2024-05-23 18:45:22.000000 scorify-2024.5.23/scorify.egg-info/top_level.txt
+-rw-r--r--   0 njvack     (501) staff       (20)     1276 2024-05-23 18:45:22.895086 scorify-2024.5.23/setup.cfg
+-rwxr-xr-x   0 njvack     (501) staff       (20)      530 2024-05-15 20:38:47.000000 scorify-2024.5.23/setup.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2024-05-23 18:45:22.894219 scorify-2024.5.23/tests/
+-rw-rw-r--   0 njvack     (501) staff       (20)        0 2019-10-14 20:29:38.000000 scorify-2024.5.23/tests/__init__.py
+-rw-r--r--   0 njvack     (501) staff       (20)      288 2024-05-15 20:38:47.000000 scorify-2024.5.23/tests/base.py
+-rw-r--r--   0 njvack     (501) staff       (20)     3370 2024-05-15 20:38:47.000000 scorify-2024.5.23/tests/test_aggregators.py
+-rw-r--r--   0 njvack     (501) staff       (20)     4988 2024-05-15 20:38:47.000000 scorify-2024.5.23/tests/test_datafile.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1871 2024-05-15 20:38:47.000000 scorify-2024.5.23/tests/test_directives.py
+-rw-r--r--   0 njvack     (501) staff       (20)     2112 2024-05-15 20:38:47.000000 scorify-2024.5.23/tests/test_integration.py
+-rw-r--r--   0 njvack     (501) staff       (20)     2745 2024-05-15 20:38:47.000000 scorify-2024.5.23/tests/test_mappings.py
+-rw-r--r--   0 njvack     (501) staff       (20)     2444 2024-04-10 20:45:21.000000 scorify-2024.5.23/tests/test_reliability.py
+-rw-r--r--   0 njvack     (501) staff       (20)     1271 2024-05-15 20:48:39.000000 scorify-2024.5.23/tests/test_score_multi.py
+-rw-r--r--   0 njvack     (501) staff       (20)     5485 2024-05-15 20:38:47.000000 scorify-2024.5.23/tests/test_scorer.py
+-rw-r--r--   0 njvack     (501) staff       (20)     4661 2024-05-15 20:38:47.000000 scorify-2024.5.23/tests/test_scoresheet.py
+-rw-r--r--   0 njvack     (501) staff       (20)      479 2024-05-15 20:38:47.000000 scorify-2024.5.23/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scorify-0.9.3/PKG-INFO` & `scorify-2024.5.23/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,302 +1,331 @@
 Metadata-Version: 2.1
 Name: scorify
-Version: 0.9.3
+Version: 2024.5.23
 Summary: Library for scoring questionnaires
 Home-page: https://github.com/uwmadison-chm/scorify
+Download-URL: https://github.com/uwmadison-chm/scorify/releases
 Author: Nate Vack
 Author-email: njvack@wisc.edu
 Maintainer: Nate Vack
 Maintainer-email: njvack@wisc.edu
 License: MIT
-Download-URL: https://github.com/uwmadison-chm/scorify/releases
-Description: # Scorify: A simple tool for scoring psychological self-report questionnaires.
-        
-        [![DOI](https://zenodo.org/badge/16382827.svg)](https://zenodo.org/badge/latestdoi/16382827)
-        
-        ## Background
-        
-        Many psychology studies use one or more self-report questionnaires to understand their participants. These responses go into CSV files with one question per column, one participant per row.
-        
-        Scoring these files is a bunch of work. Oftentimes, many questionnaires (or sub-scales) are included in one CSV file. Often, half of the questions are "reverse-scored" to combat the tendancy people have to agree with questions. Scoring these files usually means spending a whole bunch of time in Excel, and no one likes doing that.
-        
-        Scorify aims to fix this.
-        
-        ## Installation
-        
-        scorify requires Python 3.5.
-        
-            pip install scorify
-        
-        should have you set up.
-        
-        ## Examples
-        
-        See [examples/](examples/) for some test files. To run the neurohack data and
-        scoresheet, do something like:
-        
-            score_data neurohack_scoresheet.csv neurohack_April+2,+2019_11.05.csv
-        
-        ## Getting started
-        
-        Given an example CSV file, let's say you want to score 5 columns, the answers
-        can be 1 to 5, where the third and fifth are reversed.
-        
-        | ppt  | happy1 | happy2 | happy3 | happy4 | happy5 |
-        | 3001 | 1      | 2      | 1      | 3      | 4      |
-        | 3002 | 4      | 1      | 5      | 1      | 2      |
-        | 3003 | 1      | 3      | 2      | 3      | 1      |
-        | ...  |
-        
-        Create a scoresheet that looks like:
-        
-        | A         | B       | C            | D       |
-        | ---       | ---     | ---          | ---     |
-        | layout    | header  |              |         |
-        | layout    | data    |              |         |
-        |           |         |              |         |
-        | transform | normal  | map(1:5,1:5) |         |
-        | transform | reverse | map(1:5,5:1) |         |
-        |           |         |              |         |
-        | score     | ppt     |              |         |
-        | score     | happy1  | happy        | normal  |
-        | score     | happy2  | happy        | normal  |
-        | score     | happy3  | happy        | reverse |
-        | score     | happy4  | happy        | normal  |
-        | score     | happy5  | happy        | reverse |
-        |           |         |              |         |
-        | measure   | happy   | mean(happy)  |         |
-        
-        Then you call `score_data` with that scoresheet and datafile, like:
-        
-            score_data scoresheet.csv datafile.csv
-        
-        Your output just goes to STDOUT, and you should see it renaming columns.
-        To save the output if it looks good, just pipe it to a file:
-        
-            score_data scoresheet.csv datafile.csv > output.csv
-        
-        ### Other common operations
-        
-        #### Excluding participants
-        
-        If some participant data is particularly messy, you can exclude it using your
-        scoresheet like this:
-        
-        | A       | B                  | C    |
-        | ---     | ---                | ---  |
-        | exclude | ppt_id_column_name | 3001 |
-        
-        #### Keeping second row headers
-        
-        If your question headers have a second row with verbose question text in them,
-        you can keep that in the scored data by adding a `layout keep` instruction:
-        
-            layout header
-            layout keep
-            layout data
-        
-        Repeat the layout keep instruction if you want to keep more than one row.
-        
-        ## Scoresheet reference
-        
-        The main input to scorify is a comma or tab-delimited "scoresheet" that has many rows and four columns. The first column tells what kind of command the row will be, and will be one of: `layout`, `exclude`, `transform`, `score`, or `measure`.
-        
-        ### layout
-        
-        The layout section tells scorify what your input data looks like. It must contain a `header` and `data`, but `skip` and `keep` are also valid. `data` tells scorify that the rest of your input file is data. So:
-        
-            layout header
-            layout skip
-            layout data
-        
-        would tell scorify to expect a header row, skip a line, and then read the rest of the file as data.
-        
-            layout header
-            layout keep
-            layout data
-        
-        would result in scorify expecting a header row, keeping the next line as-is,
-        and reading the rest of the file as data.
-        
-        ### rename
-        
-        The rename section renames a header column, and looks like:
-        
-            rename original_name new_name
-        
-        Columns can only be renamed once, and must use a new, unique name. You must use the column's new name everywhere in the scoresheet.
-        
-        ### exclude
-        
-        The format of an exclude line is:
-        
-            exclude column value
-        
-        which will, as you might expect, exclude rows where `column` == `value`.
-        
-        ### transform
-        
-        Sometimes, you'll want to reverse-score a column or otherwise change its value for scoring. And you'll want to give that some kind of sane name. Transforms let you do this. They look like:
-        
-            transform name mapper
-        
-        Right now, you can apply two transformations.
-        
-        #### `map()`
-        
-        A linear mapping. Example:
-        
-            transform reverse map(1:5,5:1)
-        
-        which will map the values 1,2,3,4,5 to 5,4,3,2,1. This will happily map values outside its input domain.
-        
-        #### `discrete_map()`
-        
-        A mapping for discrete values. Useful to map a numbers to human-meaningful values.
-        
-            transform score_gender discrete_map("1":"f", "2":"m")
-        
-        Unmapped values will return a blank.
-        
-        This transform can be useful when combined with `join()` (below) to combine an array of checkboxes into one column.
-        
-        #### `passthrough_map()`
-        
-        Like `discrete_map()`, though unmapped values will be unchanged. So, if you have:
-        
-            transform score_gender passthrough_map("1":"f", "2":"m")
-        
-        a value of "999" will still be "999".
-        
-        ### score
-        
-        The score section is where you tell scorify which columns you want in your output, what measure (if any) they belong to, and what transform (again, if any) you want to apply. These look like
-        
-            score column measure_name transform
-        
-        `measure_name` and `transform` are both optional. So, to reverse score (using the `reverse` we defined up above) a column called `happy_1` and add it to the `happy` measure, use:
-        
-            score happy_1 happy reverse
-        
-        You can optionally pass a 5th value, which will define the output column name:
-        
-            score happy_1 happy reverse ReverseHappy1
-        
-        ### measure
-        
-        The measure section computes aggregate measures of your scored data. These lines look like:
-        
-            measure final_name aggregator(measure_1, measure_2, ..., measure_n)
-        
-        We support the following aggregators:
-        
-        #### `mean()`
-        
-        As you might expect, this calculates the mean of the measure or measures listed. Example:
-        
-            measure happy mean(happy)
-        
-        If any values in the measures are non-numeric, returns NaN.
-        
-        #### `mean_imputed()`
-        
-        Computes the mean of the measure. However, if any of the values in the measures are non-numeric, this fills in the mean of the numeric values. For example, `mean_imputed(1, '', 3, 5)` is `3`.
-        
-        #### `sum()`
-        
-        Computes the sum fo the listed measures. Example:
-        
-            measure sad sum(sad)
-        
-        If any values in the measures are non-numeric, returns NaN.
-        
-        #### `sum_imputed()`
-        
-        Computes the sum of the measure. However, if any of the values in the measures are non-numeric, this fills in the mean of the numeric values. For example, `sum_imputed(1, '', 3, 5)` is `12`.
-        
-        #### `imputed_fraction()`
-        
-        The fraction of the data that is non-zero and would have a value imputed for it. `imputed_fraction(1, '', 3, 5)` is 0.25.
-        
-        #### `join()`
-        
-        `join()` is a little trickier. It collects all the non-blank values in the listed measures, and joins them with the `|` character. Useful if you have a set of values selected by checkbox. For example, if you had three measures that would either be blank or not for things participants might endorse, you could collate them into one column with:
-        
-            measure liked_pets join(likes_cats, likes_dogs, likes_horses)
-        
-        If a participant had `cats` for `likes_cats` and `horses` for `likes_horses`, you'd get:
-        
-            cats|horses
-        
-        #### `ratio()`
-        
-        `ratio(a, b)` will compute the ratio of two columns; in other words: `a / b`. Notably, this works on other measures, so you can take the ratio of sums or means. In those cases, the ratio line needs to come after the other measures' lines do.
-        
-        #### `min()`
-        
-        `min(measure_1, measure_2)` will output the minimum numeric value in the given measures. Non-numeric values will cause NaN.
-        
-        #### `max()`
-        
-        `max(measure_1, measure_2)` will output the maximum numeric value in the given measures. Non-numeric values will cause NaN.
-        
-        ## Complete example
-        
-        If you take a scoresheet that looks like:
-        
-        | A         | B               | C                             | D       |
-        | ---       | ---             | ---                           | ---     |
-        | layout    | header          |                               |         |
-        | layout    | data            |                               |         |
-        |           |                 |                               |         |
-        | exclude   | PPT_COL         | bad_ppt1                      |         |
-        | exclude   | PPT_COL         | bad_ppt2                      |         |
-        |           |                 |                               |         |
-        | transform | normal          | map(1:5,1:5)                  |         |
-        | transform | reverse         | map(1:5,5:1)                  |         |
-        |           |                 |                               |         |
-        | score     | PPT_COL         |                               |         |
-        | score     | HAPPY_Q1        | happy                         | normal  |
-        | score     | SAD_Q1          | happy                         | normal  |
-        | score     | HAPPY_Q2        | happy                         | reverse |
-        |           |                 |                               |         |
-        | measure   | happy_score     | mean(happy)                   |         |
-        | measure   | sad_score       | mean(sad)                     |         |
-        | measure   | happiness_ratio | ratio(happy_score, sad_score) |         |
-        
-        and run it on data that looks like:
-        
-        | PPT_COL | EXTRA | HAPPY_Q1 | SAD_Q1 | HAPPY_Q2 |
-        | ---     | ---   | ---      | ---    | ---      |
-        | ppt1    | foo   | 4        | 2      | 2        |
-        | ppt2    | bar   | 2        | 5      | 5        |
-        
-        ... you'll get output like:
-        
-        | PPT_COL | HAPPY_Q1: happy | SAD_Q1: sad | HAPPY_Q2: happy | happy_score | sad_score | happiness_ratio |
-        | ---     | ---             | ---         | ---             | ---         | ---       | ---             |
-        | ppt1    | 4               | 2           | 3               | 3.5         | 2         | 1.75            |
-        | ppt2    | 2               | 5           | 1               | 1.5         | 5         | 0.3             |
-        
-        ## Credits
-        
-        Scorify uses several excellent libraries:
-        
-        * [docopt](https://github.com/docopt/docopt)
-        * [schema](https://github.com/halst/schema)
-        * [openpyxl](https://openpyxl.readthedocs.io/)
-        
-        
 Platform: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Provides: bioread
+Provides: scorify
 Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+Requires-Dist: schema>=0.7.0
+Requires-Dist: openpyxl>=3.0.0
+Requires-Dist: docopt-ng>=0.9.0
+Requires-Dist: pandas>=1.3.5
+Requires-Dist: scipy>=1.7.3
+
+# Scorify: A simple tool for scoring psychological self-report questionnaires.
+
+[![DOI](https://zenodo.org/badge/16382827.svg)](https://zenodo.org/badge/latestdoi/16382827)
+
+## Background
+
+Many psychology studies use one or more self-report questionnaires to understand their participants. These responses go into CSV files with one question per column, one participant per row.
+
+Scoring these files is a bunch of work. Oftentimes, many questionnaires (or sub-scales) are included in one CSV file. Often, half of the questions are "reverse-scored" to combat the tendancy people have to agree with questions. Scoring these files usually means spending a whole bunch of time in Excel, and no one likes doing that.
+
+Scorify aims to fix this.
+
+## Try scorify on the web!
+
+If you want to build an automatic pipeline to score your data, you'll want the python version of the tool. But if you just want to give it a try in your browser, [try our web-based tool!](http://scorify-web.glitch.me)
+
+## Installation
+
+scorify requires Python 3.5.
+
+    pip install scorify
+
+should have you set up.
+
+## Examples
+
+See [examples/](examples/) for some test files. To run the neurohack data and
+scoresheet, do something like:
+
+    score_data neurohack_scoresheet.csv neurohack_April+2,+2019_11.05.csv
+
+## Getting started
+
+Given an example CSV file, let's say you want to score 5 columns, the answers
+can be 1 to 5, where the third and fifth are reversed.
+
+| ppt  | happy1 | happy2 | happy3 | happy4 | happy5 |
+| ---  | ---    | ---    | ---    | ---    | ---    |
+| 3001 | 1      | 2      | 1      | 3      | 4      |
+| 3002 | 4      | 1      | 5      | 1      | 2      |
+| 3003 | 1      | 3      | 2      | 3      | 1      |
+| ...  | ...    | ...    | ...    | ...    | ...    |
+
+Create a scoresheet that looks like:
+
+| A         | B       | C            | D       |
+| ---       | ---     | ---          | ---     |
+| layout    | header  |              |         |
+| layout    | data    |              |         |
+|           |         |              |         |
+| transform | normal  | map(1:5,1:5) |         |
+| transform | reverse | map(1:5,5:1) |         |
+|           |         |              |         |
+| score     | ppt     |              |         |
+| score     | happy1  | happy        | normal  |
+| score     | happy2  | happy        | normal  |
+| score     | happy3  | happy        | reverse |
+| score     | happy4  | happy        | normal  |
+| score     | happy5  | happy        | reverse |
+|           |         |              |         |
+| measure   | happy   | mean(happy)  |         |
+
+Then you call `score_data` with that scoresheet and datafile, like:
+
+    score_data scoresheet.csv datafile.csv
+
+Your output just goes to STDOUT, and you should see it renaming columns.
+To save the output if it looks good, just pipe it to a file:
+
+    score_data scoresheet.csv datafile.csv > output.csv
+
+### Other common operations
+
+#### Excluding participants
+
+If some participant data is particularly messy, you can exclude it using your
+scoresheet like this:
+
+| A       | B                  | C    |
+| ---     | ---                | ---  |
+| exclude | ppt_id_column_name | 3001 |
+
+#### Keeping second row headers
+
+If your question headers have a second row with verbose question text in them,
+you can keep that in the scored data by adding a `layout keep` instruction:
+
+    layout header
+    layout keep
+    layout data
+
+Repeat the layout keep instruction if you want to keep more than one row.
+
+## Scoresheet reference
+
+The main input to scorify is a comma or tab-delimited "scoresheet" that has many rows and four columns. The first column tells what kind of command the row will be, and will be one of: `layout`, `exclude`, `transform`, `score`, or `measure`.
+
+### layout
+
+The layout section tells scorify what your input data looks like. It must contain a `header` and `data`, but `skip` and `keep` are also valid. `data` tells scorify that the rest of your input file is data. So:
+
+    layout header
+    layout skip
+    layout data
+
+would tell scorify to expect a header row, skip a line, and then read the rest of the file as data.
+
+    layout header
+    layout keep
+    layout data
+
+would result in scorify expecting a header row, keeping the next line as-is,
+and reading the rest of the file as data.
+
+### rename
+
+The rename section renames a header column, and looks like:
+
+    rename original_name new_name
+
+Columns can only be renamed once, and must use a new, unique name. You must use the column's new name everywhere in the scoresheet.
+
+### exclude
+
+The format of an exclude line is:
+
+    exclude column value
+
+which will, as you might expect, exclude rows where `column` == `value`.
+
+### transform
+
+Sometimes, you'll want to reverse-score a column or otherwise change its value for scoring. And you'll want to give that some kind of sane name. Transforms let you do this. They look like:
+
+    transform name mapper
+
+Right now, you can apply two transformations.
+
+#### `map()`
+
+A linear mapping. Example:
+
+    transform reverse map(1:5,5:1)
+
+which will map the values 1,2,3,4,5 to 5,4,3,2,1. This will happily map values outside its input domain.
+
+#### `discrete_map()`
+
+A mapping for discrete values. Useful to map a numbers to human-meaningful values.
+
+    transform score_gender discrete_map("1":"f", "2":"m")
+
+Unmapped values will return a blank.
+
+This transform can be useful when combined with `join()` (below) to combine an array of checkboxes into one column.
+
+#### `passthrough_map()`
+
+Like `discrete_map()`, though unmapped values will be unchanged. So, if you have:
+
+    transform score_gender passthrough_map("1":"f", "2":"m")
+
+a value of "999" will still be "999".
+
+### score
+
+The score section is where you tell scorify which columns you want in your output, what measure (if any) they belong to, and what transform (again, if any) you want to apply. These look like
+
+    score column measure_name transform
+
+`measure_name` and `transform` are both optional. So, to reverse score (using the `reverse` we defined up above) a column called `happy_1` and add it to the `happy` measure, use:
+
+    score happy_1 happy reverse
+
+You can optionally pass a 5th value, which will define the output column name:
+
+    score happy_1 happy reverse ReverseHappy1
+
+### measure
+
+The measure section computes aggregate measures of your scored data. These lines look like:
+
+    measure final_name aggregator(measure_1, measure_2, ..., measure_n)
+
+We support the following aggregators:
+
+#### `mean()`
+
+As you might expect, this calculates the mean of the measure or measures listed. Example:
+
+    measure happy mean(happy)
+
+If any values in the measures are non-numeric, returns NaN.
+
+#### `mean_imputed()`
+
+Computes the mean of the measure. However, if any of the values in the measures are non-numeric, this fills in the mean of the numeric values. For example, `mean_imputed(1, '', 3, 5)` is `3`.
+
+#### `sum()`
+
+Computes the sum fo the listed measures. Example:
+
+    measure sad sum(sad)
+
+If any values in the measures are non-numeric, returns NaN.
+
+#### `sum_imputed()`
+
+Computes the sum of the measure. However, if any of the values in the measures are non-numeric, this fills in the mean of the numeric values. For example, `sum_imputed(1, '', 3, 5)` is `12`.
+
+#### `imputed_fraction()`
+
+The fraction of the data that is non-zero and would have a value imputed for it. `imputed_fraction(1, '', 3, 5)` is 0.25.
+
+#### `join()`
+
+`join()` is a little trickier. It collects all the non-blank values in the listed measures, and joins them with the `|` character. Useful if you have a set of values selected by checkbox. For example, if you had three measures that would either be blank or not for things participants might endorse, you could collate them into one column with:
+
+    measure liked_pets join(likes_cats, likes_dogs, likes_horses)
+
+If a participant had `cats` for `likes_cats` and `horses` for `likes_horses`, you'd get:
+
+    cats|horses
+
+#### `ratio()`
+
+`ratio(a, b)` will compute the ratio of two columns; in other words: `a / b`. Notably, this works on other measures, so you can take the ratio of sums or means. In those cases, the ratio line needs to come after the other measures' lines do.
+
+#### `min()`
+
+`min(measure_1, measure_2)` will output the minimum numeric value in the given measures. Non-numeric values will cause NaN.
+
+#### `max()`
+
+`max(measure_1, measure_2)` will output the maximum numeric value in the given measures. Non-numeric values will cause NaN.
+
+## Complete example
+
+If you take a scoresheet that looks like:
+
+| A         | B               | C                             | D       |
+| ---       | ---             | ---                           | ---     |
+| layout    | header          |                               |         |
+| layout    | data            |                               |         |
+|           |                 |                               |         |
+| exclude   | PPT_COL         | bad_ppt1                      |         |
+| exclude   | PPT_COL         | bad_ppt2                      |         |
+|           |                 |                               |         |
+| transform | normal          | map(1:5,1:5)                  |         |
+| transform | reverse         | map(1:5,5:1)                  |         |
+|           |                 |                               |         |
+| score     | PPT_COL         |                               |         |
+| score     | HAPPY_Q1        | happy                         | normal  |
+| score     | SAD_Q1          | happy                         | normal  |
+| score     | HAPPY_Q2        | happy                         | reverse |
+|           |                 |                               |         |
+| measure   | happy_score     | mean(happy)                   |         |
+| measure   | sad_score       | mean(sad)                     |         |
+| measure   | happiness_ratio | ratio(happy_score, sad_score) |         |
+
+and run it on data that looks like:
+
+| PPT_COL | EXTRA | HAPPY_Q1 | SAD_Q1 | HAPPY_Q2 |
+| ---     | ---   | ---      | ---    | ---      |
+| ppt1    | foo   | 4        | 2      | 2        |
+| ppt2    | bar   | 2        | 5      | 5        |
+
+... you'll get output like:
+
+| PPT_COL | HAPPY_Q1: happy | SAD_Q1: sad | HAPPY_Q2: happy | happy_score | sad_score | happiness_ratio |
+| ---     | ---             | ---         | ---             | ---         | ---       | ---             |
+| ppt1    | 4               | 2           | 3               | 3.5         | 2         | 1.75            |
+| ppt2    | 2               | 5           | 1               | 1.5         | 5         | 0.3             |
+
+
+## Reliability tool
+
+The `reliability` command reads a scoresheet and a datafile and outputs
+Cronbach's alpha for each measure, Cronbach's alpha for each measure omitting each
+question for that measure, the Mahalanobis distance for each participant, and the
+p value for each Mahalanobis distance.
+
+    $ reliability examples/test_alpha_scoresheet.csv examples/test_alpha_data.csv
+
+By default, any missing answers are handled by ignoring all of that participant's data
+(list-wise deletion). Give the `--imputation` flag to instead fill in any missing response 
+with the average (across participants) response to the question. If you get NaNs for the
+Mahalanobis distance, it's probably because numpy failed to compute an inverse for the
+covariance matrix.
+
+## Credits
+
+Scorify was written by Nate Vack <njvack@wisc.edu> and Dan Fitch <dfitch@wisce.du>. Scorify is copyright 2023 by the Boards of Regents of the University of Wisconsin System.
+
+Scorify uses several excellent libraries:
+
+* [docopt](https://github.com/docopt/docopt)
+* [schema](https://github.com/halst/schema)
+* [openpyxl](https://openpyxl.readthedocs.io/)
+
```

### Comparing `scorify-0.9.3/README.md` & `scorify-2024.5.23/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 
 Many psychology studies use one or more self-report questionnaires to understand their participants. These responses go into CSV files with one question per column, one participant per row.
 
 Scoring these files is a bunch of work. Oftentimes, many questionnaires (or sub-scales) are included in one CSV file. Often, half of the questions are "reverse-scored" to combat the tendancy people have to agree with questions. Scoring these files usually means spending a whole bunch of time in Excel, and no one likes doing that.
 
 Scorify aims to fix this.
 
+## Try scorify on the web!
+
+If you want to build an automatic pipeline to score your data, you'll want the python version of the tool. But if you just want to give it a try in your browser, [try our web-based tool!](http://scorify-web.glitch.me)
+
 ## Installation
 
 scorify requires Python 3.5.
 
     pip install scorify
 
 should have you set up.
@@ -27,18 +31,19 @@
 
 ## Getting started
 
 Given an example CSV file, let's say you want to score 5 columns, the answers
 can be 1 to 5, where the third and fifth are reversed.
 
 | ppt  | happy1 | happy2 | happy3 | happy4 | happy5 |
+| ---  | ---    | ---    | ---    | ---    | ---    |
 | 3001 | 1      | 2      | 1      | 3      | 4      |
 | 3002 | 4      | 1      | 5      | 1      | 2      |
 | 3003 | 1      | 3      | 2      | 3      | 1      |
-| ...  |
+| ...  | ...    | ...    | ...    | ...    | ...    |
 
 Create a scoresheet that looks like:
 
 | A         | B       | C            | D       |
 | ---       | ---     | ---          | ---     |
 | layout    | header  |              |         |
 | layout    | data    |              |         |
@@ -263,15 +268,33 @@
 ... you'll get output like:
 
 | PPT_COL | HAPPY_Q1: happy | SAD_Q1: sad | HAPPY_Q2: happy | happy_score | sad_score | happiness_ratio |
 | ---     | ---             | ---         | ---             | ---         | ---       | ---             |
 | ppt1    | 4               | 2           | 3               | 3.5         | 2         | 1.75            |
 | ppt2    | 2               | 5           | 1               | 1.5         | 5         | 0.3             |
 
+
+## Reliability tool
+
+The `reliability` command reads a scoresheet and a datafile and outputs
+Cronbach's alpha for each measure, Cronbach's alpha for each measure omitting each
+question for that measure, the Mahalanobis distance for each participant, and the
+p value for each Mahalanobis distance.
+
+    $ reliability examples/test_alpha_scoresheet.csv examples/test_alpha_data.csv
+
+By default, any missing answers are handled by ignoring all of that participant's data
+(list-wise deletion). Give the `--imputation` flag to instead fill in any missing response 
+with the average (across participants) response to the question. If you get NaNs for the
+Mahalanobis distance, it's probably because numpy failed to compute an inverse for the
+covariance matrix.
+
 ## Credits
 
+Scorify was written by Nate Vack <njvack@wisc.edu> and Dan Fitch <dfitch@wisce.du>. Scorify is copyright 2023 by the Boards of Regents of the University of Wisconsin System.
+
 Scorify uses several excellent libraries:
 
 * [docopt](https://github.com/docopt/docopt)
 * [schema](https://github.com/halst/schema)
 * [openpyxl](https://openpyxl.readthedocs.io/)
```

### Comparing `scorify-0.9.3/scorify/aggregators.py` & `scorify-2024.5.23/scorify/aggregators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 # -*- coding: utf-8 -*-
 # Part of the scorify package
-# Copyright (c) 2020 Board of Regents of the University of Wisconsin System
+# Copyright (c) 2024 Board of Regents of the University of Wisconsin System
 
 """
-Aggregators are functions that consense sets of numbers into single ones.
+Aggregators are functions that condense sets of numbers into single ones.
 They're used by measure directives.
 """
+
 from __future__ import absolute_import, division
 
 import math
 import re
 import logging
 
-NaN = float('nan')
+NaN = float("nan")
 
-expr_re = re.compile(r"""
+expr_re = re.compile(
+    r"""
     (\w+)  # Function name
     \(
     ([^)]+) # Yup, you can put anything in the parens
     \)
-""", re.VERBOSE | re.IGNORECASE)
+""",
+    re.VERBOSE | re.IGNORECASE,
+)
 
 
 def parse_expr(expr):
     fx_map = {
-        'sum': ag_sum,
-        'sum_imputed': ag_sum_imputed,
-        'mean': ag_mean,
-        'mean_imputed': ag_mean_imputed,
-        'imputed_fraction': ag_imputed_fraction,
-        'join': ag_join,
-        'ratio': ag_ratio,
-        'max': ag_max,
-        'min': ag_min,
+        "sum": ag_sum,
+        "sum_imputed": ag_sum_imputed,
+        "mean": ag_mean,
+        "mean_imputed": ag_mean_imputed,
+        "imputed_fraction": ag_imputed_fraction,
+        "join": ag_join,
+        "ratio": ag_ratio,
+        "max": ag_max,
+        "min": ag_min,
     }
     try:
         fx_name, measure_names = expr_re.match(expr).groups()
         fx_name = fx_name.lower()
         measure_names = [m.strip() for m in measure_names.split(",")]
     except AttributeError as err:
-        raise AggregatorError(
-            "I don't understand {0!r}: {1}".format(expr, err))
+        raise AggregatorError("I don't understand {0!r}: {1}".format(expr, err))
     try:
         fx = fx_map[fx_name]
     except KeyError:
         raise AggregatorError("I don't know {0}".format(fx_name))
     return (fx_name, fx, measure_names)
 
 
@@ -82,15 +85,15 @@
 
 # sum is a reserved word in python because goddammt
 def ag_sum(values):
     return math.fsum([float(v) for v in values])
 
 
 def ag_mean(values):
-    return ag_sum(values)/(len(values))
+    return ag_sum(values) / (len(values))
 
 
 def ag_mean_imputed(values):
     try:
         with_imputed = impute_mean(values)
         mean_val = ag_mean(with_imputed)
         logging.debug("mean({}): {}".format(with_imputed, mean_val))
@@ -106,23 +109,23 @@
         logging.debug("sum({}): {}".format(with_imputed, sum_val))
         return sum_val
     except ZeroDivisionError:
         return NaN
 
 
 def ag_imputed_fraction(values):
-    """ The fraction of non-float-able items in values """
+    """The fraction of non-float-able items in values"""
     imputed_count = len(values) - len(numeric_only(values))
     return imputed_count / len(values)
 
 
 def ag_join(values):
     # Filters out empty values.
     values = [str(v) for v in values if len(str(v).strip()) > 0]
-    return '|'.join([str(v) for v in values])
+    return "|".join([str(v) for v in values])
 
 
 def ag_ratio(values):
     if len(values) != 2:
         raise AggregatorError("ratio() needs two values")
     try:
         return float(values[0] / float(values[1]))
```

### Comparing `scorify-0.9.3/scorify/datafile.py` & `scorify-2024.5.23/scorify/datafile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Part of the scorify package
-# Copyright (c) 2020 Board of Regents of the University of Wisconsin System
+# Copyright (c) 2024 Board of Regents of the University of Wisconsin System
 
 """
 Reads data files (or CSV objects) into datafile objects.
 
 Datafiles are iterable and indexable by column name. When reading, you pass
 in a scoresheet.LayoutSection, which tells you where data and header sections
 are.
@@ -28,36 +28,40 @@
     def read(self):
         self.header = []
         self.data = []
         self.keep = []
         for line_num, line in enumerate(self.lines):
             # Since we assume layout_section is valid, we only care about
             # header and skip and keep lines -- everything else must be data.
-            line_type = ''
+            line_type = ""
             if line_num < len(self.layout_section.directives):
                 line_type = self.layout_section.directives[line_num].info
-            if line_type == 'skip':
+            if line_type == "skip":
                 continue
-            if line_type == 'header':
-                self.header = [
-                    self.rename_section.map_name(h.strip()) for h in line]
+            if line_type == "header":
+                self.header = [self.rename_section.map_name(h.strip()) for h in line]
                 # Warn if header contains duplicates
-                seen_set = set()
-                duplicates = set(x for x in self.header if x in seen_set or seen_set.add(x))
+                # Don't warn if there's a duplicate blank header, which we see from Excel input sometimes
+                seen = set()
+                duplicates = set(
+                    x for x in self.header if x in seen or (x != "" and seen.add(x))
+                )
                 if len(duplicates) > 0:
-                    warnings.warn("Duplicates in header: " + str(duplicates), UserWarning)
-            elif line_type == 'keep':
+                    warnings.warn(
+                        f"Duplicates {duplicates} in header {self.header}", UserWarning
+                    )
+            elif line_type == "keep":
                 self.append_keep(line)
             else:
                 self.append_data(line)
 
     def pad_data(self, data):
         # Force lines of funny length to be the header's length
         len_diff = len(self.header) - len(data)
-        padding = [''] * len_diff
+        padding = [""] * len_diff
         return data + padding
 
     def append_data(self, data):
         full_line = self.pad_data(data)
         self.data.append(dict(zip(self.header, full_line)))
 
     def append_keep(self, data):
@@ -66,16 +70,15 @@
 
     def apply_exclusions(self, exclusion_section):
         new_data = []
         for row in self.data:
             try:
                 exclude = any([e.excludes(row) for e in exclusion_section])
             except KeyError as exc:
-                raise ExclusionError(
-                    "data columns", str(exc), self.data.header)
+                raise ExclusionError("data columns", str(exc), self.data.header)
             if not exclude:
                 new_data.append(row)
         self.data = new_data
 
     def __len__(self):
         return len(self.data)
```

### Comparing `scorify-0.9.3/scorify/directives.py` & `scorify-2024.5.23/scorify/directives.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Part of the scorify package
-# Copyright (c) 2020 Board of Regents of the University of Wisconsin System
+# Copyright (c) 2024 Board of Regents of the University of Wisconsin System
 from __future__ import absolute_import
 
 from scorify import mappings
 from scorify import aggregators
 
 """
 Directives define operations we'll be performing on our input data files.
@@ -15,15 +15,15 @@
 
 exclude: Defines any rows we'll want to exclude from processing
 
 transform: Shortcut names that define mappings
 
 score: A column, a classification for the column, and the transform to run
 
-measure: How to aggregate scored columns into directly-usable measurements
+aggregator: How to aggregate scored columns into directly-usable measurements
 """
 
 
 class Layout(object):
     """
     Informs us about the layout of the data. They're processed in order; each
     layout directive corresponds to one line in your data file, except for a
@@ -41,48 +41,48 @@
     layout header
     layout skip
     layout data
     """
 
     def __init__(self, info):
         info_lower = info.strip().lower()
-        if info_lower not in set(['header', 'data', 'skip', 'keep']):
-            raise DirectiveError(
-                "Didn't understand layout {0!r}".format(info))
+        if info_lower not in set(["header", "data", "skip", "keep"]):
+            raise DirectiveError("Didn't understand layout {0!r}".format(info))
 
         self.info = info_lower
         super(Layout, self).__init__()
 
 
 class Rename(object):
     """
     Renames a column. Renamed columns must be referred to by the new name.
     Does not allow giving a 0-length name. Empty names or names will be
     rejected, too. Sorry if your column names are blank.
 
     All logic for this is in the datafile, since that's the only place where
     we know column names.
     """
+
     def __init__(self, original_name, new_name):
         self.original_name = str(original_name)
         self.new_name = str(new_name)
         if len(self.original_name) == 0:
             raise DirectiveError("Can't rename a blank column.")
         if len(self.new_name) == 0:
             raise DirectiveError("Can't give a column a blank name.")
         if self.original_name == self.new_name:
-            raise DirectiveError(
-                "Can't rename a column to its original name.")
+            raise DirectiveError("Can't rename a column to its original name.")
 
     def conflicts_with(self, other):
         return (
-            self.original_name == other.original_name or
-            self.original_name == other.new_name or
-            self.new_name == other.new_name or
-            self.new_name == other.original_name)
+            self.original_name == other.original_name
+            or self.original_name == other.new_name
+            or self.new_name == other.new_name
+            or self.new_name == other.original_name
+        )
 
     def __str__(self):
         return "rename %s %s" % (self.original_name, self.new_name)
 
 
 class Exclude(object):
     """
@@ -145,15 +145,15 @@
         self.column = column
         self.measure_name = measure_name
         self.transform = transform
         self.output_name = output_name
         super(Score, self).__init__()
 
 
-class Measure(object):
+class Aggregator(object):
     """
     Defines an aggregation (usually sum or mean or maybe count?) of scored
     columns. Examples:
 
     measure MEASURE_1_MEAN mean(MEASURE_1)
     """
 
@@ -164,12 +164,12 @@
             fname, fx, to_use = aggregators.parse_expr(aggregation_expr)
             self.agg_fx = fx
             self.to_use = to_use
 
         except aggregators.AggregatorError as exc:
             raise DirectiveError(str(exc))
 
-        super(Measure, self).__init__()
+        super(Aggregator, self).__init__()
 
 
 class DirectiveError(ValueError):
     pass
```

### Comparing `scorify-0.9.3/scorify/excel_reader.py` & `scorify-2024.5.23/scorify/excel_reader.py`

 * *Files identical despite different names*

### Comparing `scorify-0.9.3/scorify/mappings.py` & `scorify-2024.5.23/scorify/mappings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Part of the scorify package
-# Copyright (c) 2020 Board of Regents of the University of Wisconsin System
+# Copyright (c) 2024 Board of Regents of the University of Wisconsin System
 
 from __future__ import division, absolute_import
 import re
 
 """
 A set (right now, just two) of functions that can transform cells in input
 files.
@@ -22,16 +22,16 @@
     def __init__(self):
         super(Mapping, self).__init__()
 
     def transform(self, value):
         return None
 
     @classmethod
-    def from_string(kls, fx_string=''):
-        if fx_string == '' or fx_string.find('i') == 0:
+    def from_string(kls, fx_string=""):
+        if fx_string == "" or fx_string.find("i") == 0:
             return Identity()
         if fx_string.find("map(") == 0:
             return LinearMapping.from_string(fx_string)
         if fx_string.find("discrete_map(") == 0:
             return DiscreteMapping.from_string(fx_string)
         if fx_string.find("passthrough_map(") == 0:
             return PassthroughMapping.from_string(fx_string)
@@ -42,94 +42,109 @@
     def __init__(self):
         super(Identity, self).__init__()
 
     def transform(self, value):
         return value
 
 
-linear_mapping_re = re.compile(r""" # example: map(1:3,2:4)
+linear_mapping_re = re.compile(
+    r""" # example: map(1:3,2:4)
 map\(\s*
     (-?\d+\.?\d*)\s*:\s*(-?\d+\.?\d*) # 1:5 or -1:5 or 2.5 : -6.3
     \s*,\s*
     (-?\d+\.?\d*)\s*:\s*(-?\d+\.?\d*)
 \s*\)
-""", re.VERBOSE | re.IGNORECASE)
+""",
+    re.VERBOSE | re.IGNORECASE,
+)
 
 
 class LinearMapping(Mapping):
 
     def __init__(self, input_domain, output_domain):
         super(LinearMapping, self).__init__()
         self.input_domain = input_domain
         self.output_domain = output_domain
         try:
             irange = input_domain[1] - input_domain[0]
         except TypeError:
-            raise MappingError("{0} and {1} must both be numbers".format(
-                input_domain[1], input_domain[0]))
+            raise MappingError(
+                "{0} and {1} must both be numbers".format(
+                    input_domain[1], input_domain[0]
+                )
+            )
         if irange == 0:
             raise MappingError("Input domain numbers can't be the same")
         try:
             output_domain[1] - output_domain[0]
         except TypeError:
-            raise MappingError("{0} and {1} must both be numbers".format(
-                input_domain[1], input_domain[0]))
+            raise MappingError(
+                "{0} and {1} must both be numbers".format(
+                    input_domain[1], input_domain[0]
+                )
+            )
 
     def transform(self, value):
         val_float = float(value)
         in_range = self.input_domain[1] - self.input_domain[0]
         out_range = self.output_domain[1] - self.output_domain[0]
         in_first = self.input_domain[0]
         out_first = self.output_domain[0]
-        return (val_float - in_first) * (out_range/in_range) + out_first
+        return (val_float - in_first) * (out_range / in_range) + out_first
 
     @classmethod
     def from_string(kls, fx_string):
         result = linear_mapping_re.match(fx_string)
         if result is None:
-            raise MappingError("I don't understand {0!r}".format(
-                fx_string))
+            raise MappingError("I don't understand {0!r}".format(fx_string))
         params = result.groups()
         pn = [float(param) for param in params]
         return LinearMapping((pn[0], pn[1]), (pn[2], pn[3]))
 
     def __repr__(self):
-        return "LinearMapping({0}, {1})".format(
-            self.input_domain, self.output_domain)
+        return "LinearMapping({0}, {1})".format(self.input_domain, self.output_domain)
+
 
 # Example: string_map("1":"f", "2":"m")
 # We'll use this as an iterator to get all the "1":"f" maps
-discrete_mapping_re = re.compile(r"""
+discrete_mapping_re = re.compile(
+    r"""
     "((?:[^"\\]|\\.)*)"
     \s*:\s*
     "((?:[^"\\]|\\.)*)"
-""", re.VERBOSE)
+""",
+    re.VERBOSE,
+)
 
 
 class DiscreteMapping(Mapping):
 
     def __init__(self, map_dict):
         super(DiscreteMapping, self).__init__()
         self.map_dict = map_dict
 
     def transform(self, value):
         # In the case where there's no match, it's probably best to return an
         # empty string. They'll always see the original value in the output
         # anyhow.
-        return self.map_dict.get(value, '')
+        return self.map_dict.get(value, "")
 
     @classmethod
     def from_string(kls, fx_string):
         def ues(s):
             # Unescapes strings -- will turn '\"' into '"'
-            return bytes(s, 'utf-8').decode('unicode_escape')
+            return bytes(s, "utf-8").decode("unicode_escape")
+
         # Python 2.7 has a sweet dict comprehension, but I'll keep 2.5 compat
-        result = dict((
-            (ues(match.group(1)), ues(match.group(2)))
-            for match in re.finditer(discrete_mapping_re, fx_string)))
+        result = dict(
+            (
+                (ues(match.group(1)), ues(match.group(2)))
+                for match in re.finditer(discrete_mapping_re, fx_string)
+            )
+        )
         return kls(result)
 
 
 class PassthroughMapping(DiscreteMapping):
     def __init__(self, map_dict):
         super(PassthroughMapping, self).__init__(map_dict)
```

### Comparing `scorify-0.9.3/scorify/score_data.py` & `scorify-2024.5.23/scorify/scripts/score_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Part of the scorify package
-# Copyright (c) 2020 Board of Regents of the University of Wisconsin System
+# Copyright (c) 2024 Board of Regents of the University of Wisconsin System
 
 """Score questionnaire responses.
 
 Usage:
   score_data [options] <scoresheet> <datafile>
   score_data -h | --help
 
@@ -14,15 +14,15 @@
   --version            Show version
   --exclusions=<file>  A scoresheet with additional exclude commands
   --sheet=<num>        If using an Excel datafile as input, what sheet
                        should we use? Indexed from 0. [default: 0]
   --nans-as=<string>   Print NaNs as this [default: NaN]
   --dialect=<dialect>  The dialect for CSV files; options are 'excel' or
                        'excel-tab' [default: excel]
-  --output=<file>      An output file to write to [default: STDOUT]
+  --output=<file>      An output file to write to (if blank, writes to STDOUT)
   -q --quiet           Don't print errors
   -v, --verbose        Print extra debugging output
 """
 
 import os
 import io
 import sys
@@ -33,142 +33,141 @@
 import scorify
 from docopt import docopt
 from schema import Schema, Use, Or, And, SchemaError
 from scorify import scoresheet, datafile, scorer
 from scorify.utils import pp
 from scorify.excel_reader import ExcelReader
 
+logging.basicConfig(format="%(message)s")
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
+
 
 def open_for_read(fname):
-    return io.open(os.path.expanduser(fname), 'r', encoding='utf-8-sig')
+    return io.open(os.path.expanduser(fname), "r", encoding="utf-8-sig")
 
 
 def validate_arguments(arguments):
-    s = Schema({
-        '<scoresheet>': Use(open_for_read, error="Can't open scoresheet"),
-        '<datafile>': Use(open_for_read, error="Can't open datafile"),
-        '--sheet': Use(int),
-        '--output': str,
-        '--exclusions': Or(
-            None, Use(open_for_read, error="Can't open exclusions")),
-        '--dialect': And(
-            Use(str.lower),
-            lambda s: s in ['excel', 'excel-tab'],
-            error="Dialect must be excel or excel-tab"),
-        '--nans-as': str,
-        str: object  # Ignore extras
-    })
+    s = Schema(
+        {
+            "<scoresheet>": Use(open_for_read, error="Can't open scoresheet"),
+            "<datafile>": Use(open_for_read, error="Can't open datafile"),
+            "--sheet": Use(int),
+            "--output": str,
+            "--exclusions": Or(None, Use(open_for_read, error="Can't open exclusions")),
+            "--dialect": And(
+                Use(str.lower),
+                lambda s: s in ["excel", "excel-tab"],
+                error="Dialect must be excel or excel-tab",
+            ),
+            "--nans-as": str,
+            str: object,  # Ignore extras
+        }
+    )
     try:
         validated = s.validate(arguments)
     except SchemaError as e:
-        logging.error("Error: " + str(e))
+        logger.error("Error: " + str(e))
         sys.exit(1)
-    if validated['--quiet']:
-        logging.root.setLevel(logging.CRITICAL)
-    if validated['--verbose']:
-        logging.root.setLevel(logging.DEBUG)
     return validated
 
-def parse_arguments(argv=None):
-    return docopt(
-        __doc__,
-        argv,
-        version="Scorify {0}".format(scorify.__version__))
-
-def main():
-    logging.basicConfig(
-        format="%(message)s", stream=sys.stderr, level=logging.INFO)
-    score_data(parse_arguments())
-
-def main_test(test_args):
-    score_data(parse_arguments(test_args))
-
 
 def read_data(thing, dialect, sheet_number=0):
     if thing.name.endswith("xls") or thing.name.endswith("xlsx"):
         wb = openpyxl.load_workbook(thing.name)
         s = wb[wb.sheetnames[sheet_number]]
         return ExcelReader(s)
 
     else:
         return csv.reader(thing, dialect=dialect)
 
-def score_data(arguments):
+
+def score_data(scoresheet_file, data_file, exclusions, dialect, sheet):
     # This method is way too long, I know.
-    validated = validate_arguments(arguments)
-    logging.debug(validated)
-    dialect = validated['--dialect']
-    scoresheet_data = read_data(validated['<scoresheet>'], dialect=dialect)
+    scoresheet_data = read_data(scoresheet_file, dialect=dialect)
 
     # First, read the scoresheet
     ss = scoresheet.Reader(scoresheet_data).read_into_scoresheet()
     if ss.has_errors():
-        logging.error("Errors in {0}:".format(arguments['<scoresheet>']))
+        logger.error("Errors in {0}:".format(scoresheet_file))
         for err in ss.errors:
-            logging.error(err)
+            logger.error(err)
         sys.exit(1)
 
     # Load the data
-    datafile_data = read_data(validated['<datafile>'], dialect=dialect, sheet_number=validated['--sheet'])
-    df = datafile.Datafile(
-        datafile_data, ss.layout_section, ss.rename_section)
+    datafile_data = read_data(data_file, dialect=dialect, sheet_number=sheet)
+    df = datafile.Datafile(datafile_data, ss.layout_section, ss.rename_section)
     df.read()
 
     # Load and apply exclusions file
-    if validated['--exclusions'] is not None:
-        exclusions_data = read_data(
-            validated['--exclusions'],
-            dialect=dialect)
+    if exclusions is not None:
+        exclusions_data = read_data(exclusions, dialect=dialect)
         exc_ss = scoresheet.Reader(exclusions_data).read_into_scoresheet()
         exc = exc_ss.exclude_section
-        try:
-            df.apply_exclusions(exc)
-        except datafile.ExclusionError as err:
-            logging.critical("Error in exclusions of {0}:".format(
-                arguments['--exclusions']))
-            logging.critical(err)
-            sys.exit(1)
+        df.apply_exclusions(exc)
+
+    # Apply exclusions from scoresheet
+    df.apply_exclusions(ss.exclude_section)
+    # Actual scoring!
+    scored = scorer.Scorer.score(df, ss.transform_section, ss.score_section)
+    scorer.Scorer.add_measures(scored, ss.aggregator_section)
+    return scored
 
-    try:
-        # Apply exclusions from scoresheet
-        df.apply_exclusions(ss.exclude_section)
-        # Actual scoring!
-        scored = scorer.Scorer.score(
-            df, ss.transform_section, ss.score_section)
-        scorer.Scorer.add_measures(scored, ss.measure_section)
-        print_data(arguments['--output'], scored, validated['--nans-as'], dialect)
 
+def print_data(scored_data, output, nans_as, dialect, header_map=None):
+    if output is None:
+        out = csv.writer(sys.stdout, dialect=dialect)
+    else:
+        outfile = open(output, "w")
+        out = csv.writer(outfile, dialect=dialect)
+
+    headers_mapped = [h.format_map(header_map) for h in scored_data.header]
+    logger.debug(f"Mapped headers to {headers_mapped}")
+    logger.info(f"Writing to {output}")
+    out.writerow(headers_mapped)
+    for row in scored_data.keep:
+        rk = [row.get(h, "") for h in scored_data.header]
+        out.writerow(rk)
+    for row in scored_data:
+        rl = [pp(row[h], none_val=nans_as) for h in scored_data.header]
+        out.writerow(rl)
+
+
+def main(argv):
+    args = docopt(__doc__, argv, version=f"Scorify {scorify.__version__}")
+    val = validate_arguments(args)
+    if val["--verbose"]:
+        logger.setLevel(logging.DEBUG)
+    elif val["--quiet"]:
+        logger.setLevel(logging.CRITICAL)
+    logger.debug(val)
+
+    try:
+        scored = score_data(
+            val["<scoresheet>"],
+            val["<datafile>"],
+            val["--exclusions"],
+            val["--dialect"],
+            val["--sheet"],
+        )
     except datafile.ExclusionError as err:
-        logging.critical("Error in exclusions of {0}:".format(
-            arguments['<scoresheet>']))
-        logging.critical(err)
+        logger.critical("Error in exclusions")
+        logger.critical(err)
         sys.exit(1)
     except (scorer.ScoringError, scorer.TransformError) as err:
-        logging.critical("Error in score of {0}:".format(
-            arguments['<scoresheet>']))
-        logging.critical(err)
+        logger.critical("Error in score of {0}:".format(val["<scoresheet>"]))
+        logger.critical(err)
         sys.exit(1)
     except scorer.AggregationError as err:
-        logging.critical("Error in measures of {0}:".format(
-            arguments['<scoresheet>']))
-        logging.critical(err)
+        logger.critical("Error in measures of {0}:".format(val["<scoresheet>"]))
+        logger.critical(err)
         sys.exit(1)
 
+    print_data(scored, val["--output"], val["--nans-as"], val["--dialect"])
 
-def print_data(output, sd, nans_as, dialect):
-    if output == "STDOUT":
-        out = csv.writer(sys.stdout, dialect=dialect)
-    else:
-        outfile = open(output, 'w')
-        out = csv.writer(outfile, dialect=dialect)
 
-    out.writerow(sd.header)
-    for row in sd.keep:
-        rk = [row.get(h, '') for h in sd.header]
-        out.writerow(rk)
-    for row in sd:
-        rl = [pp(row[h], none_val=nans_as) for h in sd.header]
-        out.writerow(rl)
+def entry_point():
+    main(sys.argv[1:])
 
 
-if __name__ == '__main__':
-    main()
+if __name__ == "__main__":
+    entry_point()
```

### Comparing `scorify-0.9.3/scorify/scorer.py` & `scorify-2024.5.23/scorify/scorer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 # Part of the scorify package
-# Copyright (c) 2020 Board of Regents of the University of Wisconsin System
+# Copyright (c) 2024 Board of Regents of the University of Wisconsin System
 from __future__ import absolute_import
 
 from collections import defaultdict
 from scorify.errors import HaystackError
 
-NaN = float('nan')
+NaN = float("nan")
 
 
 class ScoredData(object):
     def __init__(self, header=None, keep=None, data=None, measure_columns=None):
         self.header = header or []
         self.data = data or []
         self.keep = keep or []
@@ -40,79 +40,83 @@
 class Scorer(object):
     @classmethod
     def score_name(kls, directive):
         if directive.output_name:
             return directive.output_name
         name = directive.column
         if directive.measure_name != "None" and len(directive.measure_name) > 0:
-            name += ': ' + directive.measure_name
+            name += ": " + directive.measure_name
         if len(directive.transform) > 0:
-            name += ': ' + directive.transform
+            name += ": " + directive.transform
         return name
 
     @classmethod
     def make_measure_columns(kls, score_section):
         mc = defaultdict(list)
         for d in score_section.directives:
             mc[d.measure_name].append(kls.score_name(d))
         return mc
 
     @classmethod
-    def score(kls, datafile, transform_section, score_section):
+    def score(kls, datafile, transform_section, score_section, ignore_missing=False):
         out = ScoredData()
         out.header = [kls.score_name(d) for d in score_section.directives]
         out.measure_columns = kls.make_measure_columns(score_section)
 
         for k in datafile.keep:
             kept = {}
             for d in score_section.directives:
                 name = kls.score_name(d)
                 try:
                     kept[name] = k[d.column]
                 except KeyError as err:
                     # No kept data for this column? No worries, just blank is fine
-                    kept[name] = ''
+                    kept[name] = ""
 
             out.keep.append(kept)
 
         for r in datafile.data:
             scored = {}
             for s in score_section.directives:
                 try:
                     tx = transform_section[s.transform]
                 except KeyError as exc:
                     raise TransformError(
-                        "transforms", "Key not found: " + s.transform,
-                        transform_section.known_transforms())
+                        "transforms",
+                        "Key not found: " + s.transform,
+                        transform_section.known_transforms(),
+                    )
 
                 name = kls.score_name(s)
-                try:
-                    sval = tx.transform(r[s.column])
-                except KeyError as err:
-                    raise ScoringError(
-                        "data columns", str(err),
-                        datafile.header)
-                except ValueError:
-                    sval = NaN
+                if ignore_missing and s.column not in r:
+                    sval = ""
+                else:
+                    try:
+                        sval = tx.transform(r[s.column])
+                    except KeyError as err:
+                        raise ScoringError("data columns", str(err), datafile.header)
+                    except ValueError:
+                        sval = NaN
                 scored[name] = sval
             out.data.append(scored)
 
         return out
 
     @classmethod
-    def add_measures(kls, scored_data, measure_section):
-        for m in measure_section.directives:
+    def add_measures(kls, scored_data, aggregatror_section):
+        for m in aggregatror_section.directives:
             scored_data.header.append(m.name)
         for row in scored_data.data:
-            for m in measure_section.directives:
+            for m in aggregatror_section.directives:
                 try:
                     cols = scored_data.columns_for(m.to_use)
                 except KeyError as exc:
                     raise AggregationError(
-                        "measures", str(exc), scored_data.known_measures())
+                        "measures", str(exc), scored_data.known_measures()
+                    )
                 vals = [row[col] for col in cols]
                 try:
                     row[m.name] = m.agg_fx(vals)
                 except ValueError:
                     row[m.name] = NaN
```

### Comparing `scorify-0.9.3/scorify/scoresheet.py` & `scorify-2024.5.23/scorify/scoresheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Part of the scorify package
-# Copyright (c) 2020 Board of Regents of the University of Wisconsin System
+# Copyright (c) 2024 Board of Regents of the University of Wisconsin System
 from __future__ import absolute_import
 
 from scorify import directives
 from scorify import mappings
 
 
 class Scoresheet(object):
     def __init__(self):
         self.errors = []
         self.layout_section = LayoutSection()
         self.rename_section = RenameSection()
         self.exclude_section = ExcludeSection()
         self.transform_section = TransformSection()
         self.score_section = ScoreSection()
-        self.measure_section = MeasureSection()
+        self.aggregator_section = AggregatorSection()
 
     def add_error(self, message):
         self.errors.append(message)
 
     def has_errors(self):
         return len(self.errors) > 0
 
@@ -41,42 +41,43 @@
             pass  # Obvs not a comment
         return len(content_parts) < 2 or is_comment
 
     def read_into_scoresheet(self, sheet=None):
         if sheet is None:
             sheet = Scoresheet()
         section_map = {
-            'layout': sheet.layout_section,
-            'rename': sheet.rename_section,
-            'exclude': sheet.exclude_section,
-            'transform': sheet.transform_section,
-            'score': sheet.score_section,
-            'measure': sheet.measure_section
+            "layout": sheet.layout_section,
+            "rename": sheet.rename_section,
+            "exclude": sheet.exclude_section,
+            "transform": sheet.transform_section,
+            "score": sheet.score_section,
+            "measure": sheet.aggregator_section,
         }
 
         for line in self.data:
             stripped_parts = [str(p).strip() for p in line]
             if self.ignorable_line(stripped_parts):
                 continue
             line_type = stripped_parts[0]
             line_params = stripped_parts[1:]
             try:
                 sect = section_map[line_type]
                 sect.append_from_strings(line_params)
             except KeyError:
                 sheet.add_error(
                     "Line {0}: I don't understand {1}".format(
-                        self.data.line_num, line_type))
+                        self.data.line_num, line_type
+                    )
+                )
             except (
                 SectionError,
                 directives.DirectiveError,
-                mappings.MappingError
+                mappings.MappingError,
             ) as exc:
-                sheet.add_error("Line {0}: {1}".format(
-                    self.data.line_num, str(exc)))
+                sheet.add_error("Line {0}: {1}".format(self.data.line_num, str(exc)))
         if not sheet.layout_section.is_valid():
             for err in sheet.layout_section.errors:
                 sheet.add_error(err)
         return sheet
 
 
 class SectionError(ValueError):
@@ -109,166 +110,187 @@
 
 class LayoutSection(Section):
     def __init__(self, directives=None):
         super(LayoutSection, self).__init__(directives)
 
     def is_valid(self):
         self.errors = []
-        headers = [d for d in self.directives if d.info == 'header']
+        headers = [d for d in self.directives if d.info == "header"]
         if len(headers) > 1:
-            self.errors.append('You can only have one header in your layout')
+            self.errors.append("You can only have one header in your layout")
         if len(headers) < 1:
-            self.errors.append('You must have one header in your layout')
+            self.errors.append("You must have one header in your layout")
 
-        datas = [d for d in self.directives if d.info == 'data']
+        datas = [d for d in self.directives if d.info == "data"]
         if len(datas) > 1:
-            self.errors.append('You can only have one data in your layout')
+            self.errors.append("You can only have one data in your layout")
         if len(datas) < 1:
-            self.errors.append('You must have one data in your layout')
+            self.errors.append("You must have one data in your layout")
 
         last_entry = self.directives[-1]
-        if not last_entry.info == 'data':
+        if not last_entry.info == "data":
             self.errors.append("Data needs to come last in your layout")
 
         return len(self.errors) == 0
 
     def append_from_strings(self, string_list):
         """
         string_list will have the "layout" stripped off already; it should
         be one of ["header", "data", "skip"] but we'll let directives.Layout
         figure that out.
         """
         if len(string_list) < 1:
             raise directives.DirectiveError(
-                "layout must be 'header', 'data', or 'skip'")
+                "layout must be 'header', 'data', or 'skip'"
+            )
         self.append_directive(directives.Layout(string_list[0]))
 
 
 class RenameSection(Section):
     def __init__(self, directives=None):
         self.mapper = {}
         super(RenameSection, self).__init__(directives)
 
     def append_from_strings(self, string_list):
         if len(string_list) < 2:
             raise directives.DirectiveError(
-                "rename needs an original and new column name")
-        self.append_directive(
-            directives.Rename(string_list[0], string_list[1]))
+                "rename needs an original and new column name"
+            )
+        self.append_directive(directives.Rename(string_list[0], string_list[1]))
 
     def append_directive(self, directive):
         self.__raise_on_conflict(directive)
         self.mapper[directive.original_name] = directive.new_name
         super(RenameSection, self).append_directive(directive)
 
     def map_name(self, name):
         # Default to the original.
         return self.mapper.get(name, name)
 
     def __raise_on_conflict(self, directive):
         conflict = next(
-            (d for d in self.directives if directive.conflicts_with(d)),
-            None)
+            (d for d in self.directives if directive.conflicts_with(d)), None
+        )
         if conflict:
-            raise SectionError(
-                "%s conflicts with %s" % (directive, conflict))
+            raise SectionError("%s conflicts with %s" % (directive, conflict))
 
 
 class ExcludeSection(Section):
     def __init__(self, directives=None):
         super(ExcludeSection, self).__init__(directives)
 
     def append_from_strings(self, string_list):
         if len(string_list) < 1:
-            raise directives.DirectiveError(
-                "exclude must have a column name")
+            raise directives.DirectiveError("exclude must have a column name")
         exclude_col = string_list[0]
-        exclude_val = ''
+        exclude_val = ""
         if len(string_list) > 1:
             exclude_val = string_list[1]
         self.append_directive(directives.Exclude(exclude_col, exclude_val))
 
 
 class TransformSection(Section):
     def __init__(self, directive_list=None):
         super(TransformSection, self).__init__(directive_list)
         self.transform_dict = {}
-        self.identity_transform = directives.Transform('', '')
+        self.identity_transform = directives.Transform("", "")
 
     def append_from_strings(self, string_list):
         if len(string_list) < 2:
             raise directives.DirectiveError(
-                "transform must have a name and transformation")
+                "transform must have a name and transformation"
+            )
         name, xform = string_list[0], string_list[1]
         self.append_directive(directives.Transform(name, xform))
 
     def append_directive(self, directive):
         name = directive.name
         dupes = [d for d in self.directives if d.name == name]
         if len(dupes) > 0:
-            raise SectionError(
-                "there's already a transform called {0}".format(name))
+            raise SectionError("there's already a transform called {0}".format(name))
         self.transform_dict[name] = directive
         super(TransformSection, self).append_directive(directive)
 
     def known_transforms(self):
         return self.transform_dict.keys()
 
     def __getitem__(self, name):
-        if str(name).strip() == '':
+        if str(name).strip() == "":
             return self.identity_transform
         return self.transform_dict[name]
 
 
 class ScoreSection(Section):
     def __init__(self, directives=None):
         super(ScoreSection, self).__init__(directives)
+        self.questions_by_measure = dict()
+        self.all_questions = []
+        self.participant_id_column_name = None
+
+    def get_measures(self):
+        return self.questions_by_measure.keys()
 
     def append_from_strings(self, string_list):
         if len(string_list) < 1:
-            raise directives.DirectiveError(
-                "score must have a column name")
+            raise directives.DirectiveError("score must have a column name")
         col_name = string_list[0]
-        measure_name = ''
-        transform = ''
+        measure_name = ""
+        transform = ""
         output_name = None
+        if self.participant_id_column_name is None:
+            if len(string_list) != 1:
+                self.errors.append(
+                    "first score row should contain only the name of the participant id column"
+                )
+            self.participant_id_column_name = string_list[0]
         if len(string_list) > 1:
             measure_name = string_list[1]
         if len(string_list) > 2:
             transform = string_list[2]
         if len(string_list) > 3:
             output_name = string_list[3]
 
+        if measure_name:
+            if measure_name not in self.questions_by_measure:
+                self.questions_by_measure[measure_name] = []
+            self.questions_by_measure[measure_name].append(col_name)
+            self.all_questions.append(col_name)
+
         self.append_directive(
-            directives.Score(col_name, measure_name, transform, output_name))
+            directives.Score(col_name, measure_name, transform, output_name)
+        )
 
     def append_directive(self, directive):
         column = directive.column
         measure_name = directive.measure_name
         dupes = [
-            d for d in self.directives if
-            d.column == column and d.measure_name == measure_name]
+            d
+            for d in self.directives
+            if d.column == column and d.measure_name == measure_name
+        ]
         if len(dupes) > 0:
-            raise SectionError("{0} is already part of {1}".format(
-                column, measure_name))
+            raise SectionError(
+                "{0} is already part of {1}".format(column, measure_name)
+            )
         super(ScoreSection, self).append_directive(directive)
 
 
-class MeasureSection(Section):
+class AggregatorSection(Section):
     def __init__(self, directives=None):
-        super(MeasureSection, self).__init__(directives)
+        super(AggregatorSection, self).__init__(directives)
 
     def append_from_strings(self, string_list):
         if len(string_list) < 2:
             raise directives.DirectiveError(
-                "measures must have a name and aggregator function")
+                "aggregators must have a name and aggregator function"
+            )
         name = string_list[0]
         agg_fx = string_list[1]
-        d = directives.Measure(name, agg_fx)
-        super(MeasureSection, self).append_directive(d)
+        d = directives.Aggregator(name, agg_fx)
+        super(AggregatorSection, self).append_directive(d)
 
     def append_directive(self, directive):
         name = directive.name
         dupes = [d for d in self.directives if d.name == name]
         if len(dupes) > 0:
-            raise SectionError("{0} is already a measure name".format(name))
-        super(MeasureSection, self).append_directive(directive)
+            raise SectionError("{0} is already an aggregator name".format(name))
+        super(AggregatorSection, self).append_directive(directive)
```

### Comparing `scorify-0.9.3/scorify/utils.py` & `scorify-2024.5.23/scorify/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # -*- coding: utf-8 -*-
 # Part of the scorify package
-# Copyright (c) 2020 Board of Regents of the University of Wisconsin System
+# Copyright (c) 2024 Board of Regents of the University of Wisconsin System
 from __future__ import absolute_import
 
 import re
 import math
 
 float_stripper = re.compile(r"\.0*$")
 
 
-def pp(val, float_places=2, none_val='NaN'):
-    mapping = {
-        float: float_pp
-    }
+def pp(val, float_places=2, none_val="NaN"):
+    mapping = {float: float_pp}
     mapper = mapping.get(type(val))
     if mapper:
         return mapper(val, float_places, none_val)
     else:
         if val is None:
             return none_val
     return str(val)
 
 
-def float_pp(num, float_places=2, none_val='NaN'):
+def float_pp(num, float_places=2, none_val="NaN"):
     if math.isnan(num) or math.isinf(num):
         return none_val
     rounded = str(round(num, float_places))
     return float_stripper.sub("", rounded)
```

### Comparing `scorify-0.9.3/scorify.egg-info/PKG-INFO` & `scorify-2024.5.23/scorify.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,302 +1,331 @@
 Metadata-Version: 2.1
 Name: scorify
-Version: 0.9.3
+Version: 2024.5.23
 Summary: Library for scoring questionnaires
 Home-page: https://github.com/uwmadison-chm/scorify
+Download-URL: https://github.com/uwmadison-chm/scorify/releases
 Author: Nate Vack
 Author-email: njvack@wisc.edu
 Maintainer: Nate Vack
 Maintainer-email: njvack@wisc.edu
 License: MIT
-Download-URL: https://github.com/uwmadison-chm/scorify/releases
-Description: # Scorify: A simple tool for scoring psychological self-report questionnaires.
-        
-        [![DOI](https://zenodo.org/badge/16382827.svg)](https://zenodo.org/badge/latestdoi/16382827)
-        
-        ## Background
-        
-        Many psychology studies use one or more self-report questionnaires to understand their participants. These responses go into CSV files with one question per column, one participant per row.
-        
-        Scoring these files is a bunch of work. Oftentimes, many questionnaires (or sub-scales) are included in one CSV file. Often, half of the questions are "reverse-scored" to combat the tendancy people have to agree with questions. Scoring these files usually means spending a whole bunch of time in Excel, and no one likes doing that.
-        
-        Scorify aims to fix this.
-        
-        ## Installation
-        
-        scorify requires Python 3.5.
-        
-            pip install scorify
-        
-        should have you set up.
-        
-        ## Examples
-        
-        See [examples/](examples/) for some test files. To run the neurohack data and
-        scoresheet, do something like:
-        
-            score_data neurohack_scoresheet.csv neurohack_April+2,+2019_11.05.csv
-        
-        ## Getting started
-        
-        Given an example CSV file, let's say you want to score 5 columns, the answers
-        can be 1 to 5, where the third and fifth are reversed.
-        
-        | ppt  | happy1 | happy2 | happy3 | happy4 | happy5 |
-        | 3001 | 1      | 2      | 1      | 3      | 4      |
-        | 3002 | 4      | 1      | 5      | 1      | 2      |
-        | 3003 | 1      | 3      | 2      | 3      | 1      |
-        | ...  |
-        
-        Create a scoresheet that looks like:
-        
-        | A         | B       | C            | D       |
-        | ---       | ---     | ---          | ---     |
-        | layout    | header  |              |         |
-        | layout    | data    |              |         |
-        |           |         |              |         |
-        | transform | normal  | map(1:5,1:5) |         |
-        | transform | reverse | map(1:5,5:1) |         |
-        |           |         |              |         |
-        | score     | ppt     |              |         |
-        | score     | happy1  | happy        | normal  |
-        | score     | happy2  | happy        | normal  |
-        | score     | happy3  | happy        | reverse |
-        | score     | happy4  | happy        | normal  |
-        | score     | happy5  | happy        | reverse |
-        |           |         |              |         |
-        | measure   | happy   | mean(happy)  |         |
-        
-        Then you call `score_data` with that scoresheet and datafile, like:
-        
-            score_data scoresheet.csv datafile.csv
-        
-        Your output just goes to STDOUT, and you should see it renaming columns.
-        To save the output if it looks good, just pipe it to a file:
-        
-            score_data scoresheet.csv datafile.csv > output.csv
-        
-        ### Other common operations
-        
-        #### Excluding participants
-        
-        If some participant data is particularly messy, you can exclude it using your
-        scoresheet like this:
-        
-        | A       | B                  | C    |
-        | ---     | ---                | ---  |
-        | exclude | ppt_id_column_name | 3001 |
-        
-        #### Keeping second row headers
-        
-        If your question headers have a second row with verbose question text in them,
-        you can keep that in the scored data by adding a `layout keep` instruction:
-        
-            layout header
-            layout keep
-            layout data
-        
-        Repeat the layout keep instruction if you want to keep more than one row.
-        
-        ## Scoresheet reference
-        
-        The main input to scorify is a comma or tab-delimited "scoresheet" that has many rows and four columns. The first column tells what kind of command the row will be, and will be one of: `layout`, `exclude`, `transform`, `score`, or `measure`.
-        
-        ### layout
-        
-        The layout section tells scorify what your input data looks like. It must contain a `header` and `data`, but `skip` and `keep` are also valid. `data` tells scorify that the rest of your input file is data. So:
-        
-            layout header
-            layout skip
-            layout data
-        
-        would tell scorify to expect a header row, skip a line, and then read the rest of the file as data.
-        
-            layout header
-            layout keep
-            layout data
-        
-        would result in scorify expecting a header row, keeping the next line as-is,
-        and reading the rest of the file as data.
-        
-        ### rename
-        
-        The rename section renames a header column, and looks like:
-        
-            rename original_name new_name
-        
-        Columns can only be renamed once, and must use a new, unique name. You must use the column's new name everywhere in the scoresheet.
-        
-        ### exclude
-        
-        The format of an exclude line is:
-        
-            exclude column value
-        
-        which will, as you might expect, exclude rows where `column` == `value`.
-        
-        ### transform
-        
-        Sometimes, you'll want to reverse-score a column or otherwise change its value for scoring. And you'll want to give that some kind of sane name. Transforms let you do this. They look like:
-        
-            transform name mapper
-        
-        Right now, you can apply two transformations.
-        
-        #### `map()`
-        
-        A linear mapping. Example:
-        
-            transform reverse map(1:5,5:1)
-        
-        which will map the values 1,2,3,4,5 to 5,4,3,2,1. This will happily map values outside its input domain.
-        
-        #### `discrete_map()`
-        
-        A mapping for discrete values. Useful to map a numbers to human-meaningful values.
-        
-            transform score_gender discrete_map("1":"f", "2":"m")
-        
-        Unmapped values will return a blank.
-        
-        This transform can be useful when combined with `join()` (below) to combine an array of checkboxes into one column.
-        
-        #### `passthrough_map()`
-        
-        Like `discrete_map()`, though unmapped values will be unchanged. So, if you have:
-        
-            transform score_gender passthrough_map("1":"f", "2":"m")
-        
-        a value of "999" will still be "999".
-        
-        ### score
-        
-        The score section is where you tell scorify which columns you want in your output, what measure (if any) they belong to, and what transform (again, if any) you want to apply. These look like
-        
-            score column measure_name transform
-        
-        `measure_name` and `transform` are both optional. So, to reverse score (using the `reverse` we defined up above) a column called `happy_1` and add it to the `happy` measure, use:
-        
-            score happy_1 happy reverse
-        
-        You can optionally pass a 5th value, which will define the output column name:
-        
-            score happy_1 happy reverse ReverseHappy1
-        
-        ### measure
-        
-        The measure section computes aggregate measures of your scored data. These lines look like:
-        
-            measure final_name aggregator(measure_1, measure_2, ..., measure_n)
-        
-        We support the following aggregators:
-        
-        #### `mean()`
-        
-        As you might expect, this calculates the mean of the measure or measures listed. Example:
-        
-            measure happy mean(happy)
-        
-        If any values in the measures are non-numeric, returns NaN.
-        
-        #### `mean_imputed()`
-        
-        Computes the mean of the measure. However, if any of the values in the measures are non-numeric, this fills in the mean of the numeric values. For example, `mean_imputed(1, '', 3, 5)` is `3`.
-        
-        #### `sum()`
-        
-        Computes the sum fo the listed measures. Example:
-        
-            measure sad sum(sad)
-        
-        If any values in the measures are non-numeric, returns NaN.
-        
-        #### `sum_imputed()`
-        
-        Computes the sum of the measure. However, if any of the values in the measures are non-numeric, this fills in the mean of the numeric values. For example, `sum_imputed(1, '', 3, 5)` is `12`.
-        
-        #### `imputed_fraction()`
-        
-        The fraction of the data that is non-zero and would have a value imputed for it. `imputed_fraction(1, '', 3, 5)` is 0.25.
-        
-        #### `join()`
-        
-        `join()` is a little trickier. It collects all the non-blank values in the listed measures, and joins them with the `|` character. Useful if you have a set of values selected by checkbox. For example, if you had three measures that would either be blank or not for things participants might endorse, you could collate them into one column with:
-        
-            measure liked_pets join(likes_cats, likes_dogs, likes_horses)
-        
-        If a participant had `cats` for `likes_cats` and `horses` for `likes_horses`, you'd get:
-        
-            cats|horses
-        
-        #### `ratio()`
-        
-        `ratio(a, b)` will compute the ratio of two columns; in other words: `a / b`. Notably, this works on other measures, so you can take the ratio of sums or means. In those cases, the ratio line needs to come after the other measures' lines do.
-        
-        #### `min()`
-        
-        `min(measure_1, measure_2)` will output the minimum numeric value in the given measures. Non-numeric values will cause NaN.
-        
-        #### `max()`
-        
-        `max(measure_1, measure_2)` will output the maximum numeric value in the given measures. Non-numeric values will cause NaN.
-        
-        ## Complete example
-        
-        If you take a scoresheet that looks like:
-        
-        | A         | B               | C                             | D       |
-        | ---       | ---             | ---                           | ---     |
-        | layout    | header          |                               |         |
-        | layout    | data            |                               |         |
-        |           |                 |                               |         |
-        | exclude   | PPT_COL         | bad_ppt1                      |         |
-        | exclude   | PPT_COL         | bad_ppt2                      |         |
-        |           |                 |                               |         |
-        | transform | normal          | map(1:5,1:5)                  |         |
-        | transform | reverse         | map(1:5,5:1)                  |         |
-        |           |                 |                               |         |
-        | score     | PPT_COL         |                               |         |
-        | score     | HAPPY_Q1        | happy                         | normal  |
-        | score     | SAD_Q1          | happy                         | normal  |
-        | score     | HAPPY_Q2        | happy                         | reverse |
-        |           |                 |                               |         |
-        | measure   | happy_score     | mean(happy)                   |         |
-        | measure   | sad_score       | mean(sad)                     |         |
-        | measure   | happiness_ratio | ratio(happy_score, sad_score) |         |
-        
-        and run it on data that looks like:
-        
-        | PPT_COL | EXTRA | HAPPY_Q1 | SAD_Q1 | HAPPY_Q2 |
-        | ---     | ---   | ---      | ---    | ---      |
-        | ppt1    | foo   | 4        | 2      | 2        |
-        | ppt2    | bar   | 2        | 5      | 5        |
-        
-        ... you'll get output like:
-        
-        | PPT_COL | HAPPY_Q1: happy | SAD_Q1: sad | HAPPY_Q2: happy | happy_score | sad_score | happiness_ratio |
-        | ---     | ---             | ---         | ---             | ---         | ---       | ---             |
-        | ppt1    | 4               | 2           | 3               | 3.5         | 2         | 1.75            |
-        | ppt2    | 2               | 5           | 1               | 1.5         | 5         | 0.3             |
-        
-        ## Credits
-        
-        Scorify uses several excellent libraries:
-        
-        * [docopt](https://github.com/docopt/docopt)
-        * [schema](https://github.com/halst/schema)
-        * [openpyxl](https://openpyxl.readthedocs.io/)
-        
-        
 Platform: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Provides: bioread
+Provides: scorify
 Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE
+Requires-Dist: schema>=0.7.0
+Requires-Dist: openpyxl>=3.0.0
+Requires-Dist: docopt-ng>=0.9.0
+Requires-Dist: pandas>=1.3.5
+Requires-Dist: scipy>=1.7.3
+
+# Scorify: A simple tool for scoring psychological self-report questionnaires.
+
+[![DOI](https://zenodo.org/badge/16382827.svg)](https://zenodo.org/badge/latestdoi/16382827)
+
+## Background
+
+Many psychology studies use one or more self-report questionnaires to understand their participants. These responses go into CSV files with one question per column, one participant per row.
+
+Scoring these files is a bunch of work. Oftentimes, many questionnaires (or sub-scales) are included in one CSV file. Often, half of the questions are "reverse-scored" to combat the tendancy people have to agree with questions. Scoring these files usually means spending a whole bunch of time in Excel, and no one likes doing that.
+
+Scorify aims to fix this.
+
+## Try scorify on the web!
+
+If you want to build an automatic pipeline to score your data, you'll want the python version of the tool. But if you just want to give it a try in your browser, [try our web-based tool!](http://scorify-web.glitch.me)
+
+## Installation
+
+scorify requires Python 3.5.
+
+    pip install scorify
+
+should have you set up.
+
+## Examples
+
+See [examples/](examples/) for some test files. To run the neurohack data and
+scoresheet, do something like:
+
+    score_data neurohack_scoresheet.csv neurohack_April+2,+2019_11.05.csv
+
+## Getting started
+
+Given an example CSV file, let's say you want to score 5 columns, the answers
+can be 1 to 5, where the third and fifth are reversed.
+
+| ppt  | happy1 | happy2 | happy3 | happy4 | happy5 |
+| ---  | ---    | ---    | ---    | ---    | ---    |
+| 3001 | 1      | 2      | 1      | 3      | 4      |
+| 3002 | 4      | 1      | 5      | 1      | 2      |
+| 3003 | 1      | 3      | 2      | 3      | 1      |
+| ...  | ...    | ...    | ...    | ...    | ...    |
+
+Create a scoresheet that looks like:
+
+| A         | B       | C            | D       |
+| ---       | ---     | ---          | ---     |
+| layout    | header  |              |         |
+| layout    | data    |              |         |
+|           |         |              |         |
+| transform | normal  | map(1:5,1:5) |         |
+| transform | reverse | map(1:5,5:1) |         |
+|           |         |              |         |
+| score     | ppt     |              |         |
+| score     | happy1  | happy        | normal  |
+| score     | happy2  | happy        | normal  |
+| score     | happy3  | happy        | reverse |
+| score     | happy4  | happy        | normal  |
+| score     | happy5  | happy        | reverse |
+|           |         |              |         |
+| measure   | happy   | mean(happy)  |         |
+
+Then you call `score_data` with that scoresheet and datafile, like:
+
+    score_data scoresheet.csv datafile.csv
+
+Your output just goes to STDOUT, and you should see it renaming columns.
+To save the output if it looks good, just pipe it to a file:
+
+    score_data scoresheet.csv datafile.csv > output.csv
+
+### Other common operations
+
+#### Excluding participants
+
+If some participant data is particularly messy, you can exclude it using your
+scoresheet like this:
+
+| A       | B                  | C    |
+| ---     | ---                | ---  |
+| exclude | ppt_id_column_name | 3001 |
+
+#### Keeping second row headers
+
+If your question headers have a second row with verbose question text in them,
+you can keep that in the scored data by adding a `layout keep` instruction:
+
+    layout header
+    layout keep
+    layout data
+
+Repeat the layout keep instruction if you want to keep more than one row.
+
+## Scoresheet reference
+
+The main input to scorify is a comma or tab-delimited "scoresheet" that has many rows and four columns. The first column tells what kind of command the row will be, and will be one of: `layout`, `exclude`, `transform`, `score`, or `measure`.
+
+### layout
+
+The layout section tells scorify what your input data looks like. It must contain a `header` and `data`, but `skip` and `keep` are also valid. `data` tells scorify that the rest of your input file is data. So:
+
+    layout header
+    layout skip
+    layout data
+
+would tell scorify to expect a header row, skip a line, and then read the rest of the file as data.
+
+    layout header
+    layout keep
+    layout data
+
+would result in scorify expecting a header row, keeping the next line as-is,
+and reading the rest of the file as data.
+
+### rename
+
+The rename section renames a header column, and looks like:
+
+    rename original_name new_name
+
+Columns can only be renamed once, and must use a new, unique name. You must use the column's new name everywhere in the scoresheet.
+
+### exclude
+
+The format of an exclude line is:
+
+    exclude column value
+
+which will, as you might expect, exclude rows where `column` == `value`.
+
+### transform
+
+Sometimes, you'll want to reverse-score a column or otherwise change its value for scoring. And you'll want to give that some kind of sane name. Transforms let you do this. They look like:
+
+    transform name mapper
+
+Right now, you can apply two transformations.
+
+#### `map()`
+
+A linear mapping. Example:
+
+    transform reverse map(1:5,5:1)
+
+which will map the values 1,2,3,4,5 to 5,4,3,2,1. This will happily map values outside its input domain.
+
+#### `discrete_map()`
+
+A mapping for discrete values. Useful to map a numbers to human-meaningful values.
+
+    transform score_gender discrete_map("1":"f", "2":"m")
+
+Unmapped values will return a blank.
+
+This transform can be useful when combined with `join()` (below) to combine an array of checkboxes into one column.
+
+#### `passthrough_map()`
+
+Like `discrete_map()`, though unmapped values will be unchanged. So, if you have:
+
+    transform score_gender passthrough_map("1":"f", "2":"m")
+
+a value of "999" will still be "999".
+
+### score
+
+The score section is where you tell scorify which columns you want in your output, what measure (if any) they belong to, and what transform (again, if any) you want to apply. These look like
+
+    score column measure_name transform
+
+`measure_name` and `transform` are both optional. So, to reverse score (using the `reverse` we defined up above) a column called `happy_1` and add it to the `happy` measure, use:
+
+    score happy_1 happy reverse
+
+You can optionally pass a 5th value, which will define the output column name:
+
+    score happy_1 happy reverse ReverseHappy1
+
+### measure
+
+The measure section computes aggregate measures of your scored data. These lines look like:
+
+    measure final_name aggregator(measure_1, measure_2, ..., measure_n)
+
+We support the following aggregators:
+
+#### `mean()`
+
+As you might expect, this calculates the mean of the measure or measures listed. Example:
+
+    measure happy mean(happy)
+
+If any values in the measures are non-numeric, returns NaN.
+
+#### `mean_imputed()`
+
+Computes the mean of the measure. However, if any of the values in the measures are non-numeric, this fills in the mean of the numeric values. For example, `mean_imputed(1, '', 3, 5)` is `3`.
+
+#### `sum()`
+
+Computes the sum fo the listed measures. Example:
+
+    measure sad sum(sad)
+
+If any values in the measures are non-numeric, returns NaN.
+
+#### `sum_imputed()`
+
+Computes the sum of the measure. However, if any of the values in the measures are non-numeric, this fills in the mean of the numeric values. For example, `sum_imputed(1, '', 3, 5)` is `12`.
+
+#### `imputed_fraction()`
+
+The fraction of the data that is non-zero and would have a value imputed for it. `imputed_fraction(1, '', 3, 5)` is 0.25.
+
+#### `join()`
+
+`join()` is a little trickier. It collects all the non-blank values in the listed measures, and joins them with the `|` character. Useful if you have a set of values selected by checkbox. For example, if you had three measures that would either be blank or not for things participants might endorse, you could collate them into one column with:
+
+    measure liked_pets join(likes_cats, likes_dogs, likes_horses)
+
+If a participant had `cats` for `likes_cats` and `horses` for `likes_horses`, you'd get:
+
+    cats|horses
+
+#### `ratio()`
+
+`ratio(a, b)` will compute the ratio of two columns; in other words: `a / b`. Notably, this works on other measures, so you can take the ratio of sums or means. In those cases, the ratio line needs to come after the other measures' lines do.
+
+#### `min()`
+
+`min(measure_1, measure_2)` will output the minimum numeric value in the given measures. Non-numeric values will cause NaN.
+
+#### `max()`
+
+`max(measure_1, measure_2)` will output the maximum numeric value in the given measures. Non-numeric values will cause NaN.
+
+## Complete example
+
+If you take a scoresheet that looks like:
+
+| A         | B               | C                             | D       |
+| ---       | ---             | ---                           | ---     |
+| layout    | header          |                               |         |
+| layout    | data            |                               |         |
+|           |                 |                               |         |
+| exclude   | PPT_COL         | bad_ppt1                      |         |
+| exclude   | PPT_COL         | bad_ppt2                      |         |
+|           |                 |                               |         |
+| transform | normal          | map(1:5,1:5)                  |         |
+| transform | reverse         | map(1:5,5:1)                  |         |
+|           |                 |                               |         |
+| score     | PPT_COL         |                               |         |
+| score     | HAPPY_Q1        | happy                         | normal  |
+| score     | SAD_Q1          | happy                         | normal  |
+| score     | HAPPY_Q2        | happy                         | reverse |
+|           |                 |                               |         |
+| measure   | happy_score     | mean(happy)                   |         |
+| measure   | sad_score       | mean(sad)                     |         |
+| measure   | happiness_ratio | ratio(happy_score, sad_score) |         |
+
+and run it on data that looks like:
+
+| PPT_COL | EXTRA | HAPPY_Q1 | SAD_Q1 | HAPPY_Q2 |
+| ---     | ---   | ---      | ---    | ---      |
+| ppt1    | foo   | 4        | 2      | 2        |
+| ppt2    | bar   | 2        | 5      | 5        |
+
+... you'll get output like:
+
+| PPT_COL | HAPPY_Q1: happy | SAD_Q1: sad | HAPPY_Q2: happy | happy_score | sad_score | happiness_ratio |
+| ---     | ---             | ---         | ---             | ---         | ---       | ---             |
+| ppt1    | 4               | 2           | 3               | 3.5         | 2         | 1.75            |
+| ppt2    | 2               | 5           | 1               | 1.5         | 5         | 0.3             |
+
+
+## Reliability tool
+
+The `reliability` command reads a scoresheet and a datafile and outputs
+Cronbach's alpha for each measure, Cronbach's alpha for each measure omitting each
+question for that measure, the Mahalanobis distance for each participant, and the
+p value for each Mahalanobis distance.
+
+    $ reliability examples/test_alpha_scoresheet.csv examples/test_alpha_data.csv
+
+By default, any missing answers are handled by ignoring all of that participant's data
+(list-wise deletion). Give the `--imputation` flag to instead fill in any missing response 
+with the average (across participants) response to the question. If you get NaNs for the
+Mahalanobis distance, it's probably because numpy failed to compute an inverse for the
+covariance matrix.
+
+## Credits
+
+Scorify was written by Nate Vack <njvack@wisc.edu> and Dan Fitch <dfitch@wisce.du>. Scorify is copyright 2023 by the Boards of Regents of the University of Wisconsin System.
+
+Scorify uses several excellent libraries:
+
+* [docopt](https://github.com/docopt/docopt)
+* [schema](https://github.com/halst/schema)
+* [openpyxl](https://openpyxl.readthedocs.io/)
+
```

### Comparing `scorify-0.9.3/scorify.egg-info/SOURCES.txt` & `scorify-2024.5.23/scorify.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,38 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 scorify/__init__.py
 scorify/aggregators.py
 scorify/datafile.py
 scorify/directives.py
 scorify/errors.py
 scorify/excel_reader.py
 scorify/info.py
 scorify/mappings.py
-scorify/score_data.py
+scorify/reliability.py
 scorify/scorer.py
 scorify/scoresheet.py
 scorify/utils.py
 scorify.egg-info/PKG-INFO
 scorify.egg-info/SOURCES.txt
 scorify.egg-info/dependency_links.txt
 scorify.egg-info/entry_points.txt
 scorify.egg-info/not-zip-safe
 scorify.egg-info/requires.txt
 scorify.egg-info/top_level.txt
+scorify/scripts/__init__.py
+scorify/scripts/score_data.py
+scorify/scripts/score_multi.py
 tests/__init__.py
 tests/base.py
 tests/test_aggregators.py
 tests/test_datafile.py
 tests/test_directives.py
 tests/test_integration.py
 tests/test_mappings.py
+tests/test_reliability.py
+tests/test_score_multi.py
 tests/test_scorer.py
 tests/test_scoresheet.py
 tests/test_utils.py
```

### Comparing `scorify-0.9.3/setup.py` & `scorify-2024.5.23/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 import sys
 from os import path
 
-SETUP_REQUIRES = ['setuptools >= 30.3.0']
-SETUP_REQUIRES += ['wheel'] if 'bdist_wheel' in sys.argv else []
+SETUP_REQUIRES = ["setuptools >= 30.3.0"]
+SETUP_REQUIRES += ["wheel"] if "bdist_wheel" in sys.argv else []
 
 
 def get_locals(filename):
     local_vars = {}
-    exec(open(filename, 'r').read(), {}, local_vars)
+    exec(open(filename, "r").read(), {}, local_vars)
     return local_vars
 
 
-info = get_locals(path.join('scorify', 'info.py'))
+info = get_locals(path.join("scorify", "info.py"))
 
 setup(
     name="scorify",
     setup_requires=SETUP_REQUIRES,
-    version=info['version'],
-    packages=find_packages()
+    version=info["version"],
+    packages=find_packages(),
 )
```

### Comparing `scorify-0.9.3/tests/test_aggregators.py` & `scorify-2024.5.23/tests/test_aggregators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 # -*- coding: utf-8 -*-
 # Part of the scorify package
-# Copyright (c) 2020 Board of Regents of the University of Wisconsin System
+# Copyright (c) 2024 Board of Regents of the University of Wisconsin System
 
 from __future__ import absolute_import, division
 
 import pytest
 
 import math
 
 from scorify import aggregators
 
 
 def test_good_parsing():
     n, fx, measures = aggregators.parse_expr("sum(foo)")
-    assert n == 'sum'
+    assert n == "sum"
     assert fx == aggregators.ag_sum
-    assert measures == ['foo']
+    assert measures == ["foo"]
     n, fx, measures = aggregators.parse_expr("MEAN(foo, bar)")
-    assert n == 'mean'
+    assert n == "mean"
     assert fx == aggregators.ag_mean
-    assert measures == ['foo', 'bar']
-    n, fx, measures = aggregators.parse_expr('join(foo, bar)')
-    assert n == 'join'
+    assert measures == ["foo", "bar"]
+    n, fx, measures = aggregators.parse_expr("join(foo, bar)")
+    assert n == "join"
     assert fx == aggregators.ag_join
-    assert measures == ['foo', 'bar']
-    n, fx, measures = aggregators.parse_expr('ratio(foo, bar)')
-    assert n == 'ratio'
+    assert measures == ["foo", "bar"]
+    n, fx, measures = aggregators.parse_expr("ratio(foo, bar)")
+    assert n == "ratio"
     assert fx == aggregators.ag_ratio
-    assert measures == ['foo', 'bar']
-    n, fx, measures = aggregators.parse_expr('max(foo, bar)')
+    assert measures == ["foo", "bar"]
+    n, fx, measures = aggregators.parse_expr("max(foo, bar)")
     assert fx == aggregators.ag_max
-    assert measures == ['foo', 'bar']
-    n, fx, measures = aggregators.parse_expr('min(foo, bar)')
+    assert measures == ["foo", "bar"]
+    n, fx, measures = aggregators.parse_expr("min(foo, bar)")
     assert fx == aggregators.ag_min
-    assert measures == ['foo', 'bar']
-    n, fx, measures = aggregators.parse_expr('sum_imputed(foo)')
-    assert n == 'sum_imputed'
+    assert measures == ["foo", "bar"]
+    n, fx, measures = aggregators.parse_expr("sum_imputed(foo)")
+    assert n == "sum_imputed"
     assert fx == aggregators.ag_sum_imputed
-    assert measures == ['foo']
-    n, fx, measures = aggregators.parse_expr('mean_imputed(foo)')
-    assert n == 'mean_imputed'
+    assert measures == ["foo"]
+    n, fx, measures = aggregators.parse_expr("mean_imputed(foo)")
+    assert n == "mean_imputed"
     assert fx == aggregators.ag_mean_imputed
-    assert measures == ['foo']
-    n, fx, measures = aggregators.parse_expr('imputed_fraction(foo)')
-    assert n == 'imputed_fraction'
+    assert measures == ["foo"]
+    n, fx, measures = aggregators.parse_expr("imputed_fraction(foo)")
+    assert n == "imputed_fraction"
     assert fx == aggregators.ag_imputed_fraction
-    assert measures == ['foo']
+    assert measures == ["foo"]
 
 
 def test_bad_parses():
     with pytest.raises(aggregators.AggregatorError):
         aggregators.parse_expr("dkjaskdj")
     with pytest.raises(aggregators.AggregatorError):
         aggregators.parse_expr("bogus(foo)")
@@ -57,30 +57,30 @@
 
 def test_sum_with_nums():
     ar = [1, 2, 3]
     assert aggregators.ag_sum(ar) == 6
 
 
 def test_sum_with_strings():
-    ar = ['1', '2', '3']
+    ar = ["1", "2", "3"]
     assert aggregators.ag_sum(ar) == 6
 
 
 def test_mean():
     ar = [1, 2, 3]
     assert aggregators.ag_mean(ar) == 2
 
 
 def test_join():
-    ar = ['foo', 'bar', 'baz']
-    assert aggregators.ag_join(ar) == 'foo|bar|baz'
+    ar = ["foo", "bar", "baz"]
+    assert aggregators.ag_join(ar) == "foo|bar|baz"
     ar = [1, 2, 3]
-    assert aggregators.ag_join(ar) == '1|2|3'
-    ar = ['foo', '', ' ', 'bar']
-    assert aggregators.ag_join(ar) == 'foo|bar'
+    assert aggregators.ag_join(ar) == "1|2|3"
+    ar = ["foo", "", " ", "bar"]
+    assert aggregators.ag_join(ar) == "foo|bar"
 
 
 def test_ratio():
     ar = [1, 2]
     assert aggregators.ag_ratio(ar) == 0.5
 
 
@@ -99,21 +99,21 @@
     assert aggregators.ag_min(ar) == 1
 
 
 def test_mean_imputed():
     ar = [1, None, 3, 5]
     imputed_mean = aggregators.ag_mean([1, 3, 3, 5])
     assert aggregators.ag_mean_imputed(ar) == imputed_mean
-    ar_nan = [1, float('nan'), 3, 5]
+    ar_nan = [1, float("nan"), 3, 5]
     assert aggregators.ag_mean_imputed(ar_nan) == imputed_mean
     assert math.isnan(aggregators.ag_mean_imputed([None, None]))
 
 
 def test_sum_imputed():
     ar = [1, None, 3, 5]
     assert aggregators.ag_sum_imputed(ar) == (1 + 3 + 3 + 5)
     assert math.isnan(aggregators.ag_sum_imputed([None, None]))
 
 
 def test_imputed_fraction():
     ar = [1, None, 3, 5]
-    assert aggregators.ag_imputed_fraction(ar) == (1/4)
+    assert aggregators.ag_imputed_fraction(ar) == (1 / 4)
```

### Comparing `scorify-0.9.3/tests/test_directives.py` & `scorify-2024.5.23/tests/test_directives.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # -*- coding: utf-8 -*-
 # Part of the scorify package
-# Copyright (c) 2020 Board of Regents of the University of Wisconsin System
+# Copyright (c) 2024 Board of Regents of the University of Wisconsin System
 
 from __future__ import with_statement
 
 import pytest
 
 from scorify import directives
 
 
 def test_layout_accepts_header_skip_data():
     with pytest.raises(directives.DirectiveError):
-        directives.Layout('foo')
-    assert directives.Layout('header')
-    assert directives.Layout('data')
-    assert directives.Layout('skip')
-    assert directives.Layout(' skip ')
-    assert directives.Layout('SKIP')
+        directives.Layout("foo")
+    assert directives.Layout("header")
+    assert directives.Layout("data")
+    assert directives.Layout("skip")
+    assert directives.Layout(" skip ")
+    assert directives.Layout("SKIP")
 
 
 def test_layout_accepts_header_keep():
-    assert directives.Layout('keep')
+    assert directives.Layout("keep")
 
 
 def test_transforming_works():
-    tx = directives.Transform('', '')
+    tx = directives.Transform("", "")
     assert tx.transform(1) == 1
-    tx = directives.Transform('', 'map(1:5,2:6)')
+    tx = directives.Transform("", "map(1:5,2:6)")
     assert tx.transform(1) == 2
 
 
 def test_creating_rename():
     # Just verify it exists; this directive doesn't do anything.
     directives.Rename("foo", "bar")
     # You need a new name
@@ -49,12 +49,12 @@
     assert d.conflicts_with(directives.Rename("bar", "baz"))
     assert d.conflicts_with(directives.Rename("baz", "foo"))
     assert d.conflicts_with(directives.Rename("baz", "bar"))
     assert not d.conflicts_with(directives.Rename("baz", "corge"))
 
 
 def test_measure():
-    m = directives.Measure('foo', 'mean(c_foo)')
+    m = directives.Aggregator("foo", "mean(c_foo)")
     assert m.agg_fx
-    assert m.to_use == ['c_foo']
+    assert m.to_use == ["c_foo"]
     with pytest.raises(directives.DirectiveError):
-        directives.Measure('foo', 'bar')
+        directives.Aggregator("foo", "bar")
```

### Comparing `scorify-0.9.3/tests/test_integration.py` & `scorify-2024.5.23/tests/test_integration.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from __future__ import absolute_import, division
 
 import pytest
-import os
-import openpyxl
 import csv
-import warnings
 
-from .base import *
-from scorify.score_data import main_test
-from scorify.scoresheet import SectionError
-from scorify.aggregators import AggregatorError
+from .base import from_subdir
+from scorify.scripts import score_data
+
 
 def run_score_data(scoresheet, data, output, sheet=None):
     args = [
         "--output=" + from_subdir("output", output),
         from_subdir("input", scoresheet),
-        from_subdir("input", data)
-        ]
+        from_subdir("input", data),
+    ]
     if sheet:
         args.append("--sheet={0}".format(sheet))
-    main_test(args)
+    score_data.main(args)
+
 
 def run_test(scoresheet, data, expected):
     run_score_data(scoresheet, data, expected)
 
     expected_content = open(from_subdir("input", expected)).read()
     actual_content = open(from_subdir("output", expected)).read()
     assert actual_content == expected_content
 
+
 def run_excel_test(scoresheet, data, expected, sheet=None):
     run_score_data(scoresheet, data, expected, sheet=sheet)
 
     with open(from_subdir("input", expected)) as ecsv:
         e = csv.reader(ecsv)
         elist = list(e)
 
@@ -41,31 +39,38 @@
 
     # Compare length
     assert len(elist) == len(alist)
     # Compare content
     assert elist == alist
 
 
-
 def test_basic_integration():
     run_test("001_scoresheet.csv", "001_data.csv", "001_expected.csv")
 
+
 def test_scoresheet_error():
     with pytest.raises(SystemExit) as e:
         run_test("002_broken_scoresheet.csv", "001_data.csv", "001_expected.csv")
         assert e.value.code == 1
 
+
 def test_excel_integration():
     run_excel_test("003_scoresheet.xlsx", "003_data.xlsx", "003_expected.csv")
 
+
 def test_excel_specific_sheet():
     run_excel_test("003_scoresheet.xlsx", "003_data.xlsx", "004_expected.csv", 1)
 
+
 def test_excel_integration_error():
     pytest.skip
-    # Need to confirm that input with errors gets correctly handled in excel land
+    # Need to confirm that input with errors gets correctly handled in excel
+    # land
     with pytest.raises(SystemExit) as e:
-        run_excel_test("004_broken_scoresheet.xlsx", "003_data.xlsx", "003_expected.csv")
+        run_excel_test(
+            "004_broken_scoresheet.xlsx", "003_data.xlsx", "003_expected.csv"
+        )
         assert e.value.code == 1
 
+
 def test_score_column_names():
     run_test("005_scoresheet.csv", "005_data.csv", "005_expected.csv")
```

### Comparing `scorify-0.9.3/tests/test_mappings.py` & `scorify-2024.5.23/tests/test_mappings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # -*- coding: utf-8 -*-
 # Part of the scorify package
-# Copyright (c) 2020 Board of Regents of the University of Wisconsin System
+# Copyright (c) 2024 Board of Regents of the University of Wisconsin System
 
 from __future__ import with_statement
 
 import pytest
 
 from scorify.mappings import (
-    Mapping, Identity, LinearMapping, DiscreteMapping, MappingError,
-    PassthroughMapping)
+    Mapping,
+    Identity,
+    LinearMapping,
+    DiscreteMapping,
+    MappingError,
+    PassthroughMapping,
+)
 
 
 def test_identity():
     i = Identity()
-    test_vals = (0, 'foo')
+    test_vals = (0, "foo")
     for v in test_vals:
         assert v == i.transform(v)
 
 
 def test_good_mappings():
-    sets = [
-        ((1, 5), (1, 5)),
-        ((1, 5), (5, 1)),
-        ((1, 5), (2, 6)),
-        ((1, 5), (0, 10))
-    ]
+    sets = [((1, 5), (1, 5)), ((1, 5), (5, 1)), ((1, 5), (2, 6)), ((1, 5), (0, 10))]
     for inrange, outrange in sets:
         m = LinearMapping(inrange, outrange)
         assert m.transform(inrange[0]) == outrange[0]
         assert m.transform(inrange[1]) == outrange[1]
 
 
 def test_linear_mapping_strings():
     m = LinearMapping((1, 5), (2, 6))
-    assert m.transform('1') == 2
+    assert m.transform("1") == 2
 
 
 def test_mapping_fails_with_small_inrange():
     with pytest.raises(MappingError):
         LinearMapping((1, 1), (2, 3))
 
 
 def test_mapping_fails_with_letter_ranges():
     with pytest.raises(MappingError):
-        LinearMapping(('a', 1), (1, 5))
+        LinearMapping(("a", 1), (1, 5))
 
     with pytest.raises(MappingError):
-        LinearMapping((1, 5), ('a', 1))
+        LinearMapping((1, 5), ("a", 1))
 
 
 def test_linear_mapping_from_string():
     m = LinearMapping.from_string("map( -1:3,2.5: 4)")
     assert m.input_domain == (-1.0, 3.0)
     assert m.output_domain == (2.5, 4.0)
     with pytest.raises(MappingError):
@@ -59,16 +59,15 @@
         LinearMapping.from_string("map(a:b,3:4)")
 
 
 def test_discrete_mapping_from_string():
     m = DiscreteMapping.from_string('discrete_map("1":"f","2":"m")')
     assert m.map_dict == {"1": "f", "2": "m"}
     # And let's get trickier
-    m = DiscreteMapping.from_string(
-        r'discrete_map("1\"": "f" , "2" :"m")')
+    m = DiscreteMapping.from_string(r'discrete_map("1\"": "f" , "2" :"m")')
     assert m.map_dict == {r'1"': "f", "2": "m"}
 
 
 def test_discrete_mapping_transform():
     m = DiscreteMapping({"1": "f", "2": "m"})
     assert m.transform("1") == "f"
     assert m.transform("2") == "m"
@@ -83,15 +82,13 @@
 def test_passthrough_mapping_transform():
     m = PassthroughMapping({"1": "f", "2": "m"})
     assert m.transform("1") == "f"
     assert m.transform("3") == "3"
 
 
 def test_mapping_types():
-    assert type(Mapping.from_string('')) == Identity
-    assert type(Mapping.from_string('i')) == Identity
-    assert type(Mapping.from_string('map(1:3,2:4)')) == LinearMapping
-    assert type(
-        Mapping.from_string('discrete_map("a":"b")')) == DiscreteMapping
+    assert type(Mapping.from_string("")) == Identity
+    assert type(Mapping.from_string("i")) == Identity
+    assert type(Mapping.from_string("map(1:3,2:4)")) == LinearMapping
+    assert type(Mapping.from_string('discrete_map("a":"b")')) == DiscreteMapping
 
-    assert type(
-        Mapping.from_string('passthrough_map("a":"b")')) == PassthroughMapping
+    assert type(Mapping.from_string('passthrough_map("a":"b")')) == PassthroughMapping
```

### Comparing `scorify-0.9.3/tests/test_scorer.py` & `scorify-2024.5.23/tests/test_scorer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,115 +1,115 @@
 # -*- coding: utf-8 -*-
 # Part of the scorify package
-# Copyright (c) 2020 Board of Regents of the University of Wisconsin System
+# Copyright (c) 2024 Board of Regents of the University of Wisconsin System
 
 import pytest
 
 import math
 from scorify import datafile, scoresheet, scorer
 
 
 @pytest.fixture
 def transforms():
     ts = scoresheet.TransformSection()
-    ts.append_from_strings(['reverse', 'map(1:5,5:1)'])
-    ts.append_from_strings(['gmap', 'discrete_map("1": "f", "2": "m")'])
+    ts.append_from_strings(["reverse", "map(1:5,5:1)"])
+    ts.append_from_strings(["gmap", 'discrete_map("1": "f", "2": "m")'])
     return ts
 
 
 @pytest.fixture
 def scores_1():
     ss = scoresheet.ScoreSection()
-    ss.append_from_strings(['happy1', 'happy'])
-    ss.append_from_strings(['happy2', 'happy', 'reverse'])
+    ss.append_from_strings(["happy1", "happy"])
+    ss.append_from_strings(["happy2", "happy", "reverse"])
     return ss
 
 
 @pytest.fixture
 def scores_2():
     ss = scoresheet.ScoreSection()
-    ss.append_from_strings(['happy1', 'happy'])
-    ss.append_from_strings(['happy2', 'happy', 'reverse'])
-    ss.append_from_strings(['sad1', 'sad'])
-    ss.append_from_strings(['sad2', 'sad', 'reverse'])
+    ss.append_from_strings(["happy1", "happy"])
+    ss.append_from_strings(["happy2", "happy", "reverse"])
+    ss.append_from_strings(["sad1", "sad"])
+    ss.append_from_strings(["sad2", "sad", "reverse"])
     return ss
 
 
 @pytest.fixture
 def scores_3():
     ss = scoresheet.ScoreSection()
-    ss.append_from_strings(['happy1', 'happy', '', 'KINDA HAPPY'])
-    ss.append_from_strings(['happy2', 'happy', 'reverse', 'VERY HAPPY'])
+    ss.append_from_strings(["happy1", "happy", "", "KINDA HAPPY"])
+    ss.append_from_strings(["happy2", "happy", "reverse", "VERY HAPPY"])
     return ss
 
 
 @pytest.fixture
 def gender_score():
     ss = scoresheet.ScoreSection()
-    ss.append_from_strings(['gender1', 'gender', 'gmap'])
+    ss.append_from_strings(["gender1", "gender", "gmap"])
     return ss
 
 
 @pytest.fixture
 def data_1():
     df = datafile.Datafile(None, None, None)
-    df.header = ['ppt', 'happy1', 'sad1', 'happy2', 'sad2', 'gender1']
-    df.append_data(['a', '5', '2', '2', '4', '1'])
-    df.append_data(['b', '2', '3', '4', '1', '3'])
+    df.header = ["ppt", "happy1", "sad1", "happy2", "sad2", "gender1"]
+    df.append_data(["a", "5", "2", "2", "4", "1"])
+    df.append_data(["b", "2", "3", "4", "1", "3"])
     return df
 
 
 @pytest.fixture
 def data_with_bad():
     df = datafile.Datafile(None, None, None)
-    df.header = ['ppt', 'happy1', 'sad1', 'happy2', 'sad2']
-    df.append_data(['a', 'bad', '2', 'bad', '4'])
+    df.header = ["ppt", "happy1", "sad1", "happy2", "sad2"]
+    df.append_data(["a", "bad", "2", "bad", "4"])
     return df
 
 
 @pytest.fixture
 def bad_scored(data_with_bad, transforms, scores_1):
     return scorer.Scorer.score(data_with_bad, transforms, scores_1)
 
 
 @pytest.fixture
 def measures_1():
-    ms = scoresheet.MeasureSection()
-    ms.append_from_strings(['happy', 'mean(happy)'])
+    ms = scoresheet.AggregatorSection()
+    ms.append_from_strings(["happy", "mean(happy)"])
     return ms
 
 
 @pytest.fixture
 def measures_2():
-    ms = scoresheet.MeasureSection()
-    ms.append_from_strings(['affect', 'sum(happy, sad)'])
+    ms = scoresheet.AggregatorSection()
+    ms.append_from_strings(["affect", "sum(happy, sad)"])
     return ms
 
 
 @pytest.fixture
 def measures_with_ratio():
-    ms = scoresheet.MeasureSection()
-    ms.append_from_strings(['sum_happy', 'sum(happy)'])
-    ms.append_from_strings(['sum_sad', 'sum(sad)'])
-    ms.append_from_strings(['ratio_happy', 'ratio(sum_happy, sum_sad)'])
+    ms = scoresheet.AggregatorSection()
+    ms.append_from_strings(["sum_happy", "sum(happy)"])
+    ms.append_from_strings(["sum_sad", "sum(sad)"])
+    ms.append_from_strings(["ratio_happy", "ratio(sum_happy, sum_sad)"])
     return ms
 
 
 @pytest.fixture
 def measures_with_minmax():
-    ms = scoresheet.MeasureSection()
-    ms.append_from_strings(['min_emo', 'min(happy, sad)'])
-    ms.append_from_strings(['max_happy', 'max(happy)'])
+    ms = scoresheet.AggregatorSection()
+    ms.append_from_strings(["min_emo", "min(happy, sad)"])
+    ms.append_from_strings(["max_happy", "max(happy)"])
     return ms
 
 
 @pytest.fixture
 def measures_bad():
-    ms = scoresheet.MeasureSection()
-    ms.append_from_strings(['happy', 'sum(badness)'])
+    ms = scoresheet.AggregatorSection()
+    ms.append_from_strings(["happy", "sum(badness)"])
     return ms
 
 
 @pytest.fixture
 def scored_data_1(data_1, transforms, scores_1):
     return scorer.Scorer.score(data_1, transforms, scores_1)
 
@@ -117,68 +117,68 @@
 @pytest.fixture
 def scored_data_2(data_1, transforms, scores_2):
     return scorer.Scorer.score(data_1, transforms, scores_2)
 
 
 def test_scorer_scores(data_1, transforms, scores_1):
     res = scorer.Scorer.score(data_1, transforms, scores_1)
-    assert res.header == ['happy1: happy', 'happy2: happy: reverse']
+    assert res.header == ["happy1: happy", "happy2: happy: reverse"]
     d = res.data[0]
-    assert d['happy1: happy'] == '5'
-    assert d['happy2: happy: reverse'] == 4
+    assert d["happy1: happy"] == "5"
+    assert d["happy2: happy: reverse"] == 4
 
 
 def test_scorer_renames(data_1, transforms, scores_3):
     res = scorer.Scorer.score(data_1, transforms, scores_3)
-    assert res.header == ['KINDA HAPPY', 'VERY HAPPY']
+    assert res.header == ["KINDA HAPPY", "VERY HAPPY"]
     d = res.data[0]
-    assert d['KINDA HAPPY'] == '5'
-    assert d['VERY HAPPY'] == 4
+    assert d["KINDA HAPPY"] == "5"
+    assert d["VERY HAPPY"] == 4
 
 
 def test_scorer_assigns_nan_on_bad_score(data_with_bad, transforms, scores_1):
     res = scorer.Scorer.score(data_with_bad, transforms, scores_1)
     d = res.data[0]
-    assert math.isnan(d['happy2: happy: reverse'])
+    assert math.isnan(d["happy2: happy: reverse"])
 
 
 def test_scorer_measures(scored_data_1, measures_1):
-    assert scored_data_1.header == ['happy1: happy', 'happy2: happy: reverse']
+    assert scored_data_1.header == ["happy1: happy", "happy2: happy: reverse"]
     scorer.Scorer.add_measures(scored_data_1, measures_1)
-    assert scored_data_1.header == ['happy1: happy', 'happy2: happy: reverse', 'happy']
-    assert scored_data_1.data[0]['happy'] == 4.5
+    assert scored_data_1.header == ["happy1: happy", "happy2: happy: reverse", "happy"]
+    assert scored_data_1.data[0]["happy"] == 4.5
 
 
 def test_scorer_does_ratio(scored_data_2, measures_with_ratio):
     scorer.Scorer.add_measures(scored_data_2, measures_with_ratio)
-    assert scored_data_2.data[0]['ratio_happy'] == 9.0 / 4.0
+    assert scored_data_2.data[0]["ratio_happy"] == 9.0 / 4.0
 
 
 def test_scorer_minmax(scored_data_2, measures_with_minmax):
     scorer.Scorer.add_measures(scored_data_2, measures_with_minmax)
-    assert scored_data_2.data[0]['min_emo'] == 2
-    assert scored_data_2.data[0]['max_happy'] == 5
-    assert scored_data_2.data[1]['min_emo'] == 2
-    assert scored_data_2.data[1]['max_happy'] == 2
+    assert scored_data_2.data[0]["min_emo"] == 2
+    assert scored_data_2.data[0]["max_happy"] == 5
+    assert scored_data_2.data[1]["min_emo"] == 2
+    assert scored_data_2.data[1]["max_happy"] == 2
 
 
 def test_measures_fail_with_bad_name(scored_data_1, measures_bad):
     with pytest.raises(scorer.AggregationError):
         scorer.Scorer.add_measures(scored_data_1, measures_bad)
 
 
 def test_scorer_assigns_nan_on_bad_measure(bad_scored, measures_1):
     scorer.Scorer.add_measures(bad_scored, measures_1)
-    assert math.isnan(bad_scored.data[0]['happy'])
+    assert math.isnan(bad_scored.data[0]["happy"])
 
 
 def test_scorer_does_discrete_mappings(data_1, transforms, gender_score):
     res = scorer.Scorer.score(data_1, transforms, gender_score)
 
-    assert res.data[0]['gender1: gender: gmap'] == 'f'
-    assert res.data[1]['gender1: gender: gmap'] == ''
+    assert res.data[0]["gender1: gender: gmap"] == "f"
+    assert res.data[1]["gender1: gender: gmap"] == ""
 
 
 def test_measures_multi_names(scored_data_2, measures_2):
     scorer.Scorer.add_measures(scored_data_2, measures_2)
     d = scored_data_2.data[0]
-    assert d['affect'] == 5 + 4 + 2 + 2
+    assert d["affect"] == 5 + 4 + 2 + 2
```

### Comparing `scorify-0.9.3/tests/test_scoresheet.py` & `scorify-2024.5.23/tests/test_scoresheet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # -*- coding: utf-8 -*-
 # Part of the scorify package
-# Copyright (c) 2020 Board of Regents of the University of Wisconsin System
+# Copyright (c) 2024 Board of Regents of the University of Wisconsin System
 
 import pytest
 
 from scorify import scoresheet, directives
 
 
 @pytest.fixture
 def good_sample_csv():
     import io
     import csv
-    return csv.reader(io.StringIO("""
+
+    return csv.reader(
+        io.StringIO(
+            """
 layout,header
 layout,skip
  layout,data
 
 rename,happy_1,happy
 
 # This is a comment
@@ -34,43 +37,45 @@
 
 measure,mean_happy,mean(happy)
 measure,mean_sad,mean(sad)
 measure,emo_vals,"join(happy, sad)"
 measure,happy_ratio,"ratio(mean_happy,mean_sad)"
 measure,min_emo,"min(happy, sad)"
 measure,max_happy,max(happy)
-"""))
+"""
+        )
+    )
 
 
 def test_successful_read(good_sample_csv):
     reader = scoresheet.Reader(good_sample_csv)
     ss = reader.read_into_scoresheet()
     assert type(ss) == scoresheet.Scoresheet
     assert ss.errors == []
     assert len(ss.layout_section) == 3
     assert len(ss.rename_section) == 1
     assert len(ss.transform_section) == 3
     assert len(ss.score_section) == 5
-    assert len(ss.measure_section) == 6
+    assert len(ss.aggregator_section) == 6
 
 
 def test_section_iterates():
-    skip = directives.Layout('skip')
-    header = directives.Layout('header')
-    data = directives.Layout('data')
+    skip = directives.Layout("skip")
+    header = directives.Layout("header")
+    data = directives.Layout("data")
 
     ls = scoresheet.LayoutSection([header, skip, data])
     for directive in ls:
         assert directive
 
 
 def test_layout_section():
-    skip = directives.Layout('skip')
-    header = directives.Layout('header')
-    data = directives.Layout('data')
+    skip = directives.Layout("skip")
+    header = directives.Layout("header")
+    data = directives.Layout("data")
 
     ls = scoresheet.LayoutSection([header, data])
     assert ls.is_valid()
 
     ls = scoresheet.LayoutSection([header, skip, data])
     assert ls.is_valid()
 
@@ -91,28 +96,28 @@
 
     ls = scoresheet.LayoutSection([data, header])
     assert not ls.is_valid()
 
 
 def test_layout_section_with_string_ary():
     ls = scoresheet.LayoutSection()
-    ls.append_from_strings(['header'])
+    ls.append_from_strings(["header"])
     assert len(ls) == 1
     with pytest.raises(directives.DirectiveError):
         ls.append_from_strings([])
     with pytest.raises(directives.DirectiveError):
-        ls.append_from_strings(['foo'])
+        ls.append_from_strings(["foo"])
 
 
 def test_rename_section_with_string_list():
     s = scoresheet.RenameSection()
-    s.append_from_strings(['foo', 'bar'])
+    s.append_from_strings(["foo", "bar"])
     assert len(s) == 1
-    assert s.map_name('foo') == 'bar'
-    assert s.map_name('baz') == 'baz'
+    assert s.map_name("foo") == "bar"
+    assert s.map_name("baz") == "baz"
 
 
 def test_rename_section_dupes():
     s = scoresheet.RenameSection()
     s.append_from_strings(["foo", "bar"])
     # "foo" and "bar" are off-limits for any other renames
     with pytest.raises(scoresheet.SectionError):
@@ -134,33 +139,33 @@
     assert len(s.directives) == 1
 
 
 def test_transform_section_getitem():
     s = scoresheet.TransformSection()
     d = directives.Transform("foo", "map(1:5, 1:5)")
     s.append_directive(d)
-    assert s['foo'] == d
+    assert s["foo"] == d
 
 
 def test_transform_section_getitem_with_blank():
     s = scoresheet.TransformSection()
-    assert type(s['']) == directives.Transform
+    assert type(s[""]) == directives.Transform
 
 
 def test_score_section_dupes():
     s = scoresheet.ScoreSection()
     d = directives.Score("col", "measure")
     s.append_directive(d)
     with pytest.raises(scoresheet.SectionError):
         s.append_directive(d)
     s.append_directive(directives.Score("col", "measure2"))
     s.append_directive(directives.Score("col2", "measure"))
     assert len(s.directives) == 3
 
 
-def test_measure_section_dupes():
-    s = scoresheet.MeasureSection()
-    d = directives.Measure('foo', 'mean(bar)')
+def test_aggregator_section_dupes():
+    s = scoresheet.AggregatorSection()
+    d = directives.Aggregator("foo", "mean(bar)")
     s.append_directive(d)
     with pytest.raises(scoresheet.SectionError):
         s.append_directive(d)
     assert len(s.directives) == 1
```

