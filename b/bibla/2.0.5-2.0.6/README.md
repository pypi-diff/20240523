# Comparing `tmp/bibla-2.0.5.tar.gz` & `tmp/bibla-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibla-2.0.5.tar", last modified: Fri May 17 21:30:29 2024, max compression
+gzip compressed data, was "bibla-2.0.6.tar", last modified: Thu May 23 08:31:52 2024, max compression
```

## Comparing `bibla-2.0.5.tar` & `bibla-2.0.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.496213 bibla-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-17 21:30:22.000000 bibla-2.0.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.484213 bibla-2.0.5/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-17 21:30:22.000000 bibla-2.0.5/.idea/biblint.iml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.484213 bibla-2.0.5/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-17 21:30:22.000000 bibla-2.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-17 21:30:22.000000 bibla-2.0.5/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-17 21:30:22.000000 bibla-2.0.5/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-17 21:30:22.000000 bibla-2.0.5/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-17 21:30:22.000000 bibla-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-17 21:30:22.000000 bibla-2.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-05-17 21:30:29.496213 bibla-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-17 21:30:22.000000 bibla-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.488213 bibla-2.0.5/bibla/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/bibla.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/lint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.492213 bibla-2.0.5/bibla/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rules/database_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rules/entry_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rules/field_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rules/specification_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/rules/text_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-17 21:30:22.000000 bibla-2.0.5/bibla/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.496213 bibla-2.0.5/bibla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-05-17 21:30:29.000000 bibla-2.0.5/bibla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-17 21:30:29.000000 bibla-2.0.5/bibla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:30:29.000000 bibla-2.0.5/bibla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-17 21:30:29.000000 bibla-2.0.5/bibla.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-17 21:30:29.000000 bibla-2.0.5/bibla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 21:30:29.000000 bibla-2.0.5/bibla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 21:30:29.496213 bibla-2.0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1575 2024-05-17 21:30:22.000000 bibla-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.492213 bibla-2.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:22.000000 bibla-2.0.5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-17 21:30:22.000000 bibla-2.0.5/test/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:29.496213 bibla-2.0.5/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/.bibla.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/authorNameFormatting.bib
--rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/bibLaTeX.bib
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/dateFormat.bib
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/emptyEntries.bib
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/mit.bib
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/noHomepages.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/nodirectives.bib
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/nokeys.bib
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/originalOverAlias.bib
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/pages.bib
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/required.bib
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/shouldUseDateInsteadOfYearMonthDay.bib
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/suggestedFields.bib
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/syntax.bib
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/unique.bib
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/wrongDateFormat.bib
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-17 21:30:22.000000 bibla-2.0.5/test_data/wrongFormatKey.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.173184 bibla-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-23 08:31:43.000000 bibla-2.0.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.169184 bibla-2.0.6/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-23 08:31:43.000000 bibla-2.0.6/.idea/biblint.iml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.169184 bibla-2.0.6/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-23 08:31:43.000000 bibla-2.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-23 08:31:43.000000 bibla-2.0.6/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-23 08:31:43.000000 bibla-2.0.6/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-23 08:31:43.000000 bibla-2.0.6/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-23 08:31:43.000000 bibla-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-23 08:31:43.000000 bibla-2.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-23 08:31:52.173184 bibla-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-23 08:31:43.000000 bibla-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.169184 bibla-2.0.6/bibla/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/bibla.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.169184 bibla-2.0.6/bibla/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rules/database_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rules/entry_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rules/field_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rules/specification_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rules/text_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.173184 bibla-2.0.6/bibla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-23 08:31:52.000000 bibla-2.0.6/bibla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-23 08:31:52.000000 bibla-2.0.6/bibla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:31:52.000000 bibla-2.0.6/bibla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 08:31:52.000000 bibla-2.0.6/bibla.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-23 08:31:52.000000 bibla-2.0.6/bibla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 08:31:52.000000 bibla-2.0.6/bibla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:31:52.173184 bibla-2.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1575 2024-05-23 08:31:43.000000 bibla-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.169184 bibla-2.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:43.000000 bibla-2.0.6/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 08:31:43.000000 bibla-2.0.6/test/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.173184 bibla-2.0.6/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/.bibla.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/authorNameFormatting.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/bibLaTeX.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/dateFormat.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/emptyEntries.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/mit.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/noHomepages.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/nodirectives.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/nokeys.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/originalOverAlias.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/pages.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/required.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/shouldUseDateInsteadOfYearMonthDay.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/suggestedFields.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/syntax.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/unique.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/wrongDateFormat.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/wrongFormatKey.bib
```

### Comparing `bibla-2.0.5/.idea/biblint.iml` & `bibla-2.0.6/.idea/biblint.iml`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/LICENSE` & `bibla-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/PKG-INFO` & `bibla-2.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibla
-Version: 2.0.5
+Version: 2.0.6
 Summary: A minimalistic bibLaTeX linter by Tristan Cuvelier.
 Home-page: https://github.com/MrClassicT/bibla
 Author: Tristan Cuvelier
 Author-email: tristan.cuvelier@student.hogent.be
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -40,24 +40,29 @@
 ```shell script
 pip install bibla
 ```
 ## Usage - This still needs to receive an update!
 
 Run bibla on your biblatex files with the following command
 ```shell script
+bibla lint bibliography1.bib
+```
+or
+```shell script
 bibla lint bibliography1.bib bibliography2.bib ... 
 ```
 or as a python module with
 ```shell script
 python -m bibla lint bibliography1.bib bibliography2.bib ... 
 ```
 
 bibla will check these files for a variety of style issues and deviations from the biblatex spec (http://www.biblatex.org/Format/, https://en.wikipedia.org/wiki/biblatex).
 Each possible type of issue is formulated as a rule. Each rule is identified by a unique code. Some examples of rules are 
 
+Everything below this line is mostly a copy/paste of the original and still has to be reviewed/changed!
 Rule ID|Rule description
 -|-
 `D00`|Entry not in alphabetical order by ke
 `T00`|Non-ascii character
 `E00`|Keys of published works should have format AuthorYEARa
 `E06`|Incorrect doi format
 `T01`|Non-standard whitespace at beginning of line (indents should be 4 spaces)
@@ -66,14 +71,15 @@
 
 This link provides a [list of all available rules]() \[TODO\]
 generated with the default configuration (see Configuration section below).
 
 
 The first character of a rule id refers to a rules category, e.g. `E` for issues with entry values, `T` for textual
 issues with the `.bib` file, etc.
+**NOTE: The following does not work yet due to having a fixed set ignore in the general config, this will be fixed!** - May 18th, 2024
 You can specify which rules to check by using `--select` or `--ignore`. Wildcards are allowed. `--select` will only
 enable the specified rules, disabling all other rules, while `--ignore` will disable all rules except the ones specified.
 `--select` and `--ignore` may not be specified simultaneously.
 ```shell script
 bibla --select "D*,E06,T01" lint bibliography.bib
 ```
 will only check all rules starting with D, rule E06 and rule T01
```

### Comparing `bibla-2.0.5/README.md` & `bibla-2.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,24 +12,29 @@
 ```shell script
 pip install bibla
 ```
 ## Usage - This still needs to receive an update!
 
 Run bibla on your biblatex files with the following command
 ```shell script
+bibla lint bibliography1.bib
+```
+or
+```shell script
 bibla lint bibliography1.bib bibliography2.bib ... 
 ```
 or as a python module with
 ```shell script
 python -m bibla lint bibliography1.bib bibliography2.bib ... 
 ```
 
 bibla will check these files for a variety of style issues and deviations from the biblatex spec (http://www.biblatex.org/Format/, https://en.wikipedia.org/wiki/biblatex).
 Each possible type of issue is formulated as a rule. Each rule is identified by a unique code. Some examples of rules are 
 
+Everything below this line is mostly a copy/paste of the original and still has to be reviewed/changed!
 Rule ID|Rule description
 -|-
 `D00`|Entry not in alphabetical order by ke
 `T00`|Non-ascii character
 `E00`|Keys of published works should have format AuthorYEARa
 `E06`|Incorrect doi format
 `T01`|Non-standard whitespace at beginning of line (indents should be 4 spaces)
@@ -38,14 +43,15 @@
 
 This link provides a [list of all available rules]() \[TODO\]
 generated with the default configuration (see Configuration section below).
 
 
 The first character of a rule id refers to a rules category, e.g. `E` for issues with entry values, `T` for textual
 issues with the `.bib` file, etc.
+**NOTE: The following does not work yet due to having a fixed set ignore in the general config, this will be fixed!** - May 18th, 2024
 You can specify which rules to check by using `--select` or `--ignore`. Wildcards are allowed. `--select` will only
 enable the specified rules, disabling all other rules, while `--ignore` will disable all rules except the ones specified.
 `--select` and `--ignore` may not be specified simultaneously.
 ```shell script
 bibla --select "D*,E06,T01" lint bibliography.bib
 ```
 will only check all rules starting with D, rule E06 and rule T01
```

### Comparing `bibla-2.0.5/bibla/__main__.py` & `bibla-2.0.6/bibla/__main__.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/bibla/bibla.yml` & `bibla-2.0.6/bibla/bibla.yml`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/bibla/config.py` & `bibla-2.0.6/bibla/config.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/bibla/lint.py` & `bibla-2.0.6/bibla/lint.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         print(f"E00: {e}")
         return []
     except Exception as e:
         print(f"Error: {e}")
         return []
 
     bib_data.file = bibliography
-    with open(bibliography, 'r') as bib_file:
+    with open(bibliography, 'r', encoding='utf-8') as bib_file:
         bib_text = bib_file.read()
 
     rules = load_rules()
 
     text_warnings = _apply_text_rules(bibliography, bib_text,
                                       rules.enabled_text_rules)
     entry_warnings = _apply_entry_rules(bibliography, bib_data, bib_text,
```

### Comparing `bibla-2.0.5/bibla/rule.py` & `bibla-2.0.6/bibla/rule.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/bibla/rules/database_rules.py` & `bibla-2.0.6/bibla/rules/database_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/bibla/rules/entry_rules.py` & `bibla-2.0.6/bibla/rules/entry_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/bibla/rules/field_rules.py` & `bibla-2.0.6/bibla/rules/field_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/bibla/rules/specification_rules.py` & `bibla-2.0.6/bibla/rules/specification_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/bibla/rules/text_rules.py` & `bibla-2.0.6/bibla/rules/text_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/bibla/text_utils.py` & `bibla-2.0.6/bibla/text_utils.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/bibla.egg-info/PKG-INFO` & `bibla-2.0.6/bibla.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibla
-Version: 2.0.5
+Version: 2.0.6
 Summary: A minimalistic bibLaTeX linter by Tristan Cuvelier.
 Home-page: https://github.com/MrClassicT/bibla
 Author: Tristan Cuvelier
 Author-email: tristan.cuvelier@student.hogent.be
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -40,24 +40,29 @@
 ```shell script
 pip install bibla
 ```
 ## Usage - This still needs to receive an update!
 
 Run bibla on your biblatex files with the following command
 ```shell script
+bibla lint bibliography1.bib
+```
+or
+```shell script
 bibla lint bibliography1.bib bibliography2.bib ... 
 ```
 or as a python module with
 ```shell script
 python -m bibla lint bibliography1.bib bibliography2.bib ... 
 ```
 
 bibla will check these files for a variety of style issues and deviations from the biblatex spec (http://www.biblatex.org/Format/, https://en.wikipedia.org/wiki/biblatex).
 Each possible type of issue is formulated as a rule. Each rule is identified by a unique code. Some examples of rules are 
 
+Everything below this line is mostly a copy/paste of the original and still has to be reviewed/changed!
 Rule ID|Rule description
 -|-
 `D00`|Entry not in alphabetical order by ke
 `T00`|Non-ascii character
 `E00`|Keys of published works should have format AuthorYEARa
 `E06`|Incorrect doi format
 `T01`|Non-standard whitespace at beginning of line (indents should be 4 spaces)
@@ -66,14 +71,15 @@
 
 This link provides a [list of all available rules]() \[TODO\]
 generated with the default configuration (see Configuration section below).
 
 
 The first character of a rule id refers to a rules category, e.g. `E` for issues with entry values, `T` for textual
 issues with the `.bib` file, etc.
+**NOTE: The following does not work yet due to having a fixed set ignore in the general config, this will be fixed!** - May 18th, 2024
 You can specify which rules to check by using `--select` or `--ignore`. Wildcards are allowed. `--select` will only
 enable the specified rules, disabling all other rules, while `--ignore` will disable all rules except the ones specified.
 `--select` and `--ignore` may not be specified simultaneously.
 ```shell script
 bibla --select "D*,E06,T01" lint bibliography.bib
 ```
 will only check all rules starting with D, rule E06 and rule T01
```

### Comparing `bibla-2.0.5/bibla.egg-info/SOURCES.txt` & `bibla-2.0.6/bibla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/setup.py` & `bibla-2.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/test_data/bibLaTeX.bib` & `bibla-2.0.6/test_data/bibLaTeX.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/test_data/mit.bib` & `bibla-2.0.6/test_data/mit.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/test_data/nodirectives.bib` & `bibla-2.0.6/test_data/nodirectives.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/test_data/originalOverAlias.bib` & `bibla-2.0.6/test_data/originalOverAlias.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.5/test_data/wrongDateFormat.bib` & `bibla-2.0.6/test_data/wrongDateFormat.bib`

 * *Files identical despite different names*

