# Comparing `tmp/mcpmark-0.1.tar.gz` & `tmp/mcpmark-1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcpmark-0.1.tar", last modified: Tue Jan 17 21:24:49 2023, max compression
+gzip compressed data, was "mcpmark-1.0a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mcpmark-0.1.tar` & `mcpmark-1.0a2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0      981 2023-01-17 21:19:18.528913 mcpmark-0.1/.github/workflows/testing.yml
--rw-r--r--   0        0        0       38 2022-10-14 16:02:13.312682 mcpmark-0.1/.gitignore
--rw-r--r--   0        0        0     1802 2022-10-14 16:02:13.312814 mcpmark-0.1/.travis.yml
--rw-r--r--   0        0        0     1604 2022-10-14 16:02:13.312964 mcpmark-0.1/LICENSE
--rw-r--r--   0        0        0     6538 2023-01-17 21:06:13.406787 mcpmark-0.1/README.md
--rw-r--r--   0        0        0     2054 2022-10-14 16:02:13.313343 mcpmark-0.1/doc/assign_config.yaml
--rw-r--r--   0        0        0     1283 2022-10-14 16:02:13.313459 mcpmark-0.1/doc/find_nb_components.py
--rw-r--r--   0        0        0     7505 2022-10-14 16:02:13.313625 mcpmark-0.1/doc/marking.md
--rw-r--r--   0        0        0      266 2023-01-17 21:24:24.649566 mcpmark-0.1/mcpmark/__init__.py
--rw-r--r--   0        0        0       22 2022-10-14 16:02:13.313920 mcpmark-0.1/mcpmark/cli/__init__.py
--rw-r--r--   0        0        0     2026 2022-10-14 18:46:43.954871 mcpmark-0.1/mcpmark/cli/check_one.py
--rwxr-xr-x   0        0        0     1575 2022-12-13 10:12:39.956954 mcpmark-0.1/mcpmark/cli/check_unpack.py
--rwxr-xr-x   0        0        0     1211 2022-10-14 16:02:13.314313 mcpmark-0.1/mcpmark/cli/cp_models.py
--rwxr-xr-x   0        0        0      809 2022-10-14 16:02:13.314437 mcpmark-0.1/mcpmark/cli/echo_config.py
--rw-r--r--   0        0        0     1668 2022-10-14 16:02:13.314542 mcpmark-0.1/mcpmark/cli/export_marks.py
--rwxr-xr-x   0        0        0     3000 2022-12-16 15:30:36.875074 mcpmark-0.1/mcpmark/cli/extract_manual.py
--rwxr-xr-x   0        0        0     2337 2022-11-26 20:16:14.814284 mcpmark-0.1/mcpmark/cli/extract_plots.py
--rwxr-xr-x   0        0        0      986 2022-10-14 16:02:13.314981 mcpmark-0.1/mcpmark/cli/find_duplicates.py
--rw-r--r--   0        0        0     5464 2023-01-17 21:06:13.407325 mcpmark-0.1/mcpmark/cli/grade_component.py
--rwxr-xr-x   0        0        0     2451 2022-10-14 16:02:13.315273 mcpmark-0.1/mcpmark/cli/grade_nbs.py
--rwxr-xr-x   0        0        0     4664 2022-10-14 16:02:13.315413 mcpmark-0.1/mcpmark/cli/grade_oknb.py
--rwxr-xr-x   0        0        0    11174 2023-01-16 10:54:44.549452 mcpmark-0.1/mcpmark/cli/make_feedback.py
--rwxr-xr-x   0        0        0     1361 2022-10-14 16:02:13.315523 mcpmark-0.1/mcpmark/cli/merge_marks.py
--rwxr-xr-x   0        0        0     1030 2022-10-14 16:02:13.315642 mcpmark-0.1/mcpmark/cli/mk_minimal_csv.py
--rwxr-xr-x   0        0        0     1243 2022-10-14 16:02:13.315750 mcpmark-0.1/mcpmark/cli/parse_manual_scores.py
--rwxr-xr-x   0        0        0     4088 2023-01-17 21:06:13.407777 mcpmark-0.1/mcpmark/cli/prepare_components.py
--rw-r--r--   0        0        0     1464 2022-10-14 19:18:39.127709 mcpmark-0.1/mcpmark/cli/rename_named_dirs.py
--rw-r--r--   0        0        0     1876 2022-10-14 16:02:13.316121 mcpmark-0.1/mcpmark/cli/run_notebooks.py
--rw-r--r--   0        0        0     1857 2023-01-17 21:06:13.408300 mcpmark-0.1/mcpmark/cli/scale_combine.py
--rw-r--r--   0        0        0    21037 2023-01-14 22:41:11.978481 mcpmark-0.1/mcpmark/mcputils.py
--rw-r--r--   0        0        0     1818 2022-10-14 16:02:13.316707 mcpmark-0.1/mcpmark/tests/data/assign_config.yaml
--rw-r--r--   0        0        0      947 2022-10-14 16:02:13.316825 mcpmark-0.1/mcpmark/tests/data/blank_comp_config.yaml
--rw-r--r--   0        0        0      950 2022-10-14 16:02:13.316935 mcpmark-0.1/mcpmark/tests/data/empty_comp_config.yaml
--rw-r--r--   0        0        0      947 2022-10-14 16:02:13.317023 mcpmark-0.1/mcpmark/tests/data/no_comp_config.yaml
--rw-r--r--   0        0        0     1222 2022-10-14 16:02:13.317121 mcpmark-0.1/mcpmark/tests/data/one_comp_config.yaml
--rw-r--r--   0        0        0     5979 2022-11-01 10:02:03.433657 mcpmark-0.1/mcpmark/tests/test_mcputils.py
--rw-r--r--   0        0        0     1451 2022-10-28 07:11:38.764441 mcpmark-0.1/pyproject.toml
--rw-r--r--   0        0        0       24 2022-10-14 16:02:13.317489 mcpmark-0.1/requirements.txt
--rw-r--r--   0        0        0       27 2022-10-14 16:02:13.317592 mcpmark-0.1/test-requirements.txt
--rw-r--r--   0        0        0     6983 1970-01-01 00:00:00.000000 mcpmark-0.1/PKG-INFO
+-rw-r--r--   0        0        0     6503 2024-01-02 18:05:52.098607 mcpmark-1.0a2/README.md
+-rw-r--r--   0        0        0      268 2024-05-23 14:19:22.029721 mcpmark-1.0a2/mcpmark/__init__.py
+-rw-r--r--   0        0        0       22 2022-10-14 16:02:13.313920 mcpmark-1.0a2/mcpmark/cli/__init__.py
+-rw-r--r--   0        0        0     1758 2024-04-29 21:24:19.342481 mcpmark-1.0a2/mcpmark/cli/allow_raise.py
+-rw-r--r--   0        0        0     3445 2023-08-23 20:40:59.674369 mcpmark-1.0a2/mcpmark/cli/categories.py
+-rw-r--r--   0        0        0     2026 2022-10-14 18:46:43.954871 mcpmark-1.0a2/mcpmark/cli/check_one.py
+-rwxr-xr-x   0        0        0     1575 2022-12-13 10:12:39.956954 mcpmark-1.0a2/mcpmark/cli/check_unpack.py
+-rwxr-xr-x   0        0        0     1211 2022-10-14 16:02:13.314313 mcpmark-1.0a2/mcpmark/cli/cp_models.py
+-rwxr-xr-x   0        0        0      809 2022-10-14 16:02:13.314437 mcpmark-1.0a2/mcpmark/cli/echo_config.py
+-rw-r--r--   0        0        0     1870 2024-01-05 13:55:04.663219 mcpmark-1.0a2/mcpmark/cli/export_marks.py
+-rwxr-xr-x   0        0        0     3000 2022-12-16 15:30:36.875074 mcpmark-1.0a2/mcpmark/cli/extract_manual.py
+-rwxr-xr-x   0        0        0     2337 2022-11-26 20:16:14.814284 mcpmark-1.0a2/mcpmark/cli/extract_plots.py
+-rwxr-xr-x   0        0        0      986 2022-10-14 16:02:13.314981 mcpmark-1.0a2/mcpmark/cli/find_duplicates.py
+-rw-r--r--   0        0        0     4647 2023-03-09 20:10:14.754604 mcpmark-1.0a2/mcpmark/cli/grade_component.py
+-rwxr-xr-x   0        0        0     2652 2024-04-29 21:12:21.768110 mcpmark-1.0a2/mcpmark/cli/grade_nbs.py
+-rwxr-xr-x   0        0        0     4715 2023-12-02 11:09:23.430398 mcpmark-1.0a2/mcpmark/cli/grade_oknb.py
+-rwxr-xr-x   0        0        0    11221 2023-12-13 12:56:02.640316 mcpmark-1.0a2/mcpmark/cli/make_feedback.py
+-rwxr-xr-x   0        0        0     1361 2022-10-14 16:02:13.315523 mcpmark-1.0a2/mcpmark/cli/merge_marks.py
+-rwxr-xr-x   0        0        0     1030 2022-10-14 16:02:13.315642 mcpmark-1.0a2/mcpmark/cli/mk_minimal_csv.py
+-rwxr-xr-x   0        0        0     1243 2022-10-14 16:02:13.315750 mcpmark-1.0a2/mcpmark/cli/parse_manual_scores.py
+-rwxr-xr-x   0        0        0     5438 2024-04-25 11:43:40.984643 mcpmark-1.0a2/mcpmark/cli/prepare_components.py
+-rw-r--r--   0        0        0     1464 2022-10-14 19:18:39.127709 mcpmark-1.0a2/mcpmark/cli/rename_named_dirs.py
+-rw-r--r--   0        0        0     1876 2022-10-14 16:02:13.316121 mcpmark-1.0a2/mcpmark/cli/run_notebooks.py
+-rw-r--r--   0        0        0     2694 2024-01-02 18:05:52.099990 mcpmark-1.0a2/mcpmark/cli/scale_combine.py
+-rw-r--r--   0        0        0      228 2023-03-09 16:39:14.034423 mcpmark-1.0a2/mcpmark/cli/tests/data/autograde.csv
+-rw-r--r--   0        0        0      314 2023-03-09 16:39:14.034833 mcpmark-1.0a2/mcpmark/cli/tests/data/post_1p0_format.csv
+-rw-r--r--   0        0        0       62 2023-03-09 16:39:14.035040 mcpmark-1.0a2/mcpmark/cli/tests/data/pre_1p0_format.csv
+-rw-r--r--   0        0        0     1886 2023-03-09 16:39:14.035226 mcpmark-1.0a2/mcpmark/cli/tests/test_grade_component.py
+-rw-r--r--   0        0        0      683 2023-03-09 16:39:14.035569 mcpmark-1.0a2/mcpmark/cli/tests/test_scale_combine.py
+-rw-r--r--   0        0        0    23621 2024-05-22 16:23:26.771991 mcpmark-1.0a2/mcpmark/mcputils.py
+-rw-r--r--   0        0        0     4732 2023-12-14 10:40:02.163795 mcpmark-1.0a2/mcpmark/rnbconv.py
+-rw-r--r--   0        0        0     1818 2022-10-14 16:02:13.316707 mcpmark-1.0a2/mcpmark/tests/data/assign_config.yaml
+-rw-r--r--   0        0        0      947 2022-10-14 16:02:13.316825 mcpmark-1.0a2/mcpmark/tests/data/blank_comp_config.yaml
+-rw-r--r--   0        0        0    42780 2023-11-26 00:46:37.105437 mcpmark-1.0a2/mcpmark/tests/data/eg_otter.Rmd
+-rw-r--r--   0        0        0      950 2022-10-14 16:02:13.316935 mcpmark-1.0a2/mcpmark/tests/data/empty_comp_config.yaml
+-rw-r--r--   0        0        0      947 2022-10-14 16:02:13.317023 mcpmark-1.0a2/mcpmark/tests/data/no_comp_config.yaml
+-rw-r--r--   0        0        0     1222 2022-10-14 16:02:13.317121 mcpmark-1.0a2/mcpmark/tests/data/one_comp_config.yaml
+-rw-r--r--   0        0        0     5979 2022-11-01 10:02:03.433657 mcpmark-1.0a2/mcpmark/tests/test_mcputils.py
+-rw-r--r--   0        0        0     2267 2023-12-14 10:23:53.964741 mcpmark-1.0a2/mcpmark/tests/test_rnbconv.py
+-rw-r--r--   0        0        0     1810 2024-05-23 14:27:58.853963 mcpmark-1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     6966 1970-01-01 00:00:00.000000 mcpmark-1.0a2/PKG-INFO
```

### Comparing `mcpmark-0.1/README.md` & `mcpmark-1.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,46 @@
+Metadata-Version: 2.1
+Name: mcpmark
+Version: 1.0a2
+Summary: Tools for grading multiple notebook component exercises.
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: gradools
+Requires-Dist: rnbgrader>=0.2
+Requires-Dist: pytest ; extra == "test"
+Project-URL: Home, https://github.com/matthew-brett/project-grader
+Provides-Extra: test
+
 # (Multiple) component marking
 
 Some tools I use when marking homework with with single or multiple Jupyter
 notebook components.
 
 The notebooks may have questions for manual marking, and plots for marking.
 
 They assume some Canvas](https://www.instructure.com/canvas) conventions of
 naming files, and grade output CSV format.
 
-The tools consist primarily command line utilities, with some supporting code
-in a utility library.
+The tools are mainly command line utilities, with some supporting code in
+a utility library.
 
 ## Quickstart
 
 ### For single component submission:
 
 ```
 COMPONENTS_DIR=components
 mcp-check-unpack
 mcp-prepare-components
 mcp-find-duplicates $COMPONENTS_DIR/*/*.Rmd
 mcp-cp-models
 mcp-extract-manual
-rnbg-allow-raise $COMPONENTS_DIR/*/*.Rmd --show-error
+mcp-allow-raise
 mcp-extract-plots
 mcp-grade-nbs
 # Review `<component>/marking/autograde.md`.
 # Rerun after any edits.
 mcp-grade-nbs
 mcp-grade-component
 mcp-scale-combine
@@ -38,21 +52,23 @@
 COMPONENTS_DIR=components
 mcp-check-unpack
 mcp-prepare-components
 mcp-find-duplicates $COMPONENTS_DIR/*/*.Rmd
 mcp-cp-models
 # For each component
     COMPONENT=my_component
-    rnbg-allow-raise $COMPONENTS_DIR/$COMPONENT/*.Rmd --show-error
+    mcp-allow-raise $COMPONENT
     mcp-grade-nbs $COMPONENT
-    # Review `$COMPONENT/marking/autograde.md`.
+    # Review `$COMPONENTS_DIR/$COMPONENT/marking/autograde.md`.
     # Rerun after any edits.
     mcp-grade-nbs $COMPONENT
     mcp-extract-manual $COMPONENT
+    # Mark manual questions in $COMPONENT/marking/*_report.md files
     mcp-extract-plots $COMPONENT
+    # Mark plot questions in $COMPONENT/marking/plot_nb.ipynb file
     mcp-grade-component $COMPONENT
 # Finally
 mcp-scale-combine
 ```
 
 ## Getting set up
 
@@ -133,16 +149,14 @@
     * Test tests with `grade_oknb.py`.
     * Copy tests etc into components directory with `mcp-cp-models`
     * e.g. `mcp-find-duplicates components/my_component/*.Rmd` to analyze
       duplicates, write summary into some file, say `report.md`.
     * Check notebook execution with `mcp-run-notebooks <path_to_notebooks>`.
       Consider running this with e.g. `rerun mcp-run-notebooks
       components/pandering` to continuously test notebooks.
-    * Move any irreparable notebooks to `broken` directory, and mark in
-      `marking/broken.csv` file.
     * `mcp-extract-manual <component_name>` (component name optional for single
       component submissions). Edit notebooks where manual component not found.
       Maybe e.g. `rerun mcp-extract-manual pandering`.
     * Mark generated manual file in `<component>/marking/*_report.md`.
     * Check manual scoring with something like `mcp-manual-scores
       components/lymphoma/dunleavy_plausible_report.md`.  Or you can leave
       that until grading the whole component with `mcp-grade-component`.
@@ -166,7 +180,8 @@
   even when there is only one component (in order to do the rescaling).
 * `mcp-export-marks` to convert the output of `ncp-rescale-combines` to
   a format for import into Canvas.
 
 ## Utilities
 
 * `mcputils` - various utilities for supporting the scripts.
+
```

### Comparing `mcpmark-0.1/doc/assign_config.yaml` & `mcpmark-1.0a2/mcpmark/tests/data/assign_config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 # Configuration for an assignment.
 # An "assignment" is one submitted piece of work.
-# It might have multiple "components".  One component corresponds to one
-# notebook.
+# It might have multiple "components".  These are typically notebooks.
 # All relative paths here are relative to this config file.
 # All path keys should end with "_path" (see mcputils.py).
 
-# Path containing downloaded student submissions as zip files (multiple
-# components) or ipynb files (single component).
-input_submission_path: /some/path/submissions_second
-# Directory to which to unpack / copy checked submission files.
+# Path containing student submissions as zip files.
+input_submission_path: ~/Downloads/submissions_second
+# Directory to which to unpack submission zip files.
 submissions_path: submissions_second
-# Grade export from Canvas (relative to this config file).
-# Used for finding which students should have submitted, and later,
-# for building marks output file for export to Canvas.
+# Grade export from Canvas (relative to this config file)
 canvas_export_path: "2020-03-20T0949_some_course_name.csv"
-# Column name in file above that identifies student.
+# Student identifying column name
 student_id_col: "SIS Login ID"
 # Canvas assignment name
 assignment_name: "An assignment name"
 # Components directory relative to this file.
 components_path: components_second
 component_script_path: find_nb_components.py
 components:
```

### Comparing `mcpmark-0.1/mcpmark/cli/check_one.py` & `mcpmark-1.0a2/mcpmark/cli/check_one.py`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/cli/check_unpack.py` & `mcpmark-1.0a2/mcpmark/cli/check_unpack.py`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/cli/cp_models.py` & `mcpmark-1.0a2/mcpmark/cli/cp_models.py`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/cli/echo_config.py` & `mcpmark-1.0a2/mcpmark/cli/echo_config.py`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/cli/export_marks.py` & `mcpmark-1.0a2/mcpmark/cli/export_marks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 #!/usr/bin/env python
 """ Export marks for upload to Canvas, submission to office.
 """
 
-import os
-import os.path as op
+from pathlib import Path
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 
 import pandas as pd
 
+from gradools import canvastools as ct
+
 from ..mcputils import get_minimal_df, read_config
 
 
 def write_exports(config, out_dir):
     login_fn = config['student_id_col']
-    ass_fn = config['assignment_name']
+    template = ct.to_minimal_df(config['canvas_export_path'])
+    ass_col = config['canvas_assignment_name']
+    out_cols = list(template) + [ass_col]
     in_fname = config['mark_fname']
-    in_df = get_minimal_df(config)
-    df = in_df.set_index(login_fn).drop(ass_fn, axis=1)
+    in_df = get_minimal_df(config)[[login_fn, ct.CANVAS_ID_COL]]
+    df = in_df.merge(template,
+                     on=ct.CANVAS_ID_COL,
+                     how='left').set_index(login_fn)
     mark_df = pd.read_csv(in_fname).set_index(login_fn)
     for out_field in ('Percent', 'Total'):
         final = mark_df.loc[:, [out_field]].copy()
-        ok_final = final.rename(columns={out_field: ass_fn})
-        ffinal = ok_final.join(df)
-        ffinal[login_fn] = ffinal.index
-        export = ffinal.loc[:, list(in_df)]
-        out_fname = op.join(out_dir, f'interim_marks_{out_field.lower()}.csv')
+        ok_final = final.rename(columns={out_field: ass_col})
+        ffinal = df.join(ok_final, how='right')
+        export = ffinal.loc[:, out_cols]
+        out_fname = out_dir / f'interim_marks_{out_field.lower()}.csv'
         export.to_csv(out_fname, index=None)
 
 
 def get_parser():
     parser = ArgumentParser(description=__doc__,  # Usage from docstring
                             formatter_class=RawDescriptionHelpFormatter)
     parser.add_argument('--config-path',
-                        default=op.join(os.getcwd(), 'assign_config.yaml'),
+                        default=Path() / 'assign_config.yaml',
                         help='Path to config file')
     parser.add_argument('--out-dir',
                         help='Directory to which to write files')
     return parser
 
 
 def main():
     parser = get_parser()
     args = parser.parse_args()
     config = read_config(args.config_path)
     out_dir = args.out_dir if args.out_dir else config['base_path']
-    write_exports(config, out_dir)
+    write_exports(config, Path(out_dir))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mcpmark-0.1/mcpmark/cli/extract_manual.py` & `mcpmark-1.0a2/mcpmark/cli/extract_manual.py`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/cli/extract_plots.py` & `mcpmark-1.0a2/mcpmark/cli/extract_plots.py`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/cli/find_duplicates.py` & `mcpmark-1.0a2/mcpmark/cli/find_duplicates.py`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/cli/grade_nbs.py` & `mcpmark-1.0a2/mcpmark/cli/grade_nbs.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,24 @@
 
 def get_parser():
     parser = ArgumentParser(description=__doc__,  # Usage from docstring
                             formatter_class=RawDescriptionHelpFormatter)
     parser.add_argument('--nb-lext', action='append',
                         help='Ordered list of notebook extensions '
                         'to search for (lower case, including . prefix)')
+    parser.add_argument('-v', '--verbose', action='store_true',
+                        help='More verbosity')
     return parser
 
 
-def grade_nbs(nb_fnames, cwd):
+def grade_nbs(nb_fnames, cwd, verbose=False):
     grades = {}
     for nb_fname in nb_fnames:
+        if verbose:
+            print(f'Grading {nb_fname}')
         grades[loginfn2login(nb_fname)] = grade_nb_fname(nb_fname, cwd)
     return grades
 
 
 def write_grade_report(all_grades, out_path):
     lines = []
     for login, grades in all_grades.items():
@@ -55,15 +59,15 @@
     args, config = get_component_config(get_parser())
     nb_path = component_path(config, args.component)
     lexts = args.nb_lext if args.nb_lext else ['.rmd', '.ipynb']
     nb_fnames = get_notebooks(nb_path, lexts, first_only=True)
     if len(nb_fnames) == 0:
         raise RuntimeError(f'No notebooks found in path "{nb_path}" '
                            f'with extensions {lexts}')
-    all_grades = grade_nbs(nb_fnames, nb_path)
+    all_grades = grade_nbs(nb_fnames, nb_path, args.verbose)
     assert len(all_grades) == len(nb_fnames)
     write_grade_report(all_grades, nb_path)
     write_grade_csv(config, all_grades, nb_path)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mcpmark-0.1/mcpmark/cli/grade_oknb.py` & `mcpmark-1.0a2/mcpmark/cli/grade_oknb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 """ Print results of grading notebook
 """
 
+# This should mostly be refactored to use oktools
+
 import os
 import os.path as op
 from glob import glob
 from argparse import ArgumentParser
 
 import numpy as np
```

### Comparing `mcpmark-0.1/mcpmark/cli/make_feedback.py` & `mcpmark-1.0a2/mcpmark/cli/make_feedback.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import jupytext
 
 from rmdex.exerciser import make_solution
 from ..mcputils import (execute_nb_fname, get_notebooks,
                         get_component_config,
                         make_submission_handler,
                         component_path as get_component_path)
+from .scale_combine import read_component
 
 
 def clean_dir(start_path,
               bad_dir_func=lambda d : False,
               bad_fname_func=lambda f : False):
     for dirpath, dirnames, filenames in os.walk(start_path):
         for dn in dirnames:
@@ -204,31 +205,29 @@
         return ''
     if not msg.endswith('\n'):
         msg += '\n\n'
     return msg
 
 
 def summarize_component_marking(config,
-                                component_path,
+                                component,
                                 nbs,
                                 out_nbs,
                                 component_msg=None):
     component_msg = add_nn(component_msg)
-    login_col = config['student_id_col']
-    in_marking = Path(component_path) / 'marking'
-    component_marks = pd.read_csv(in_marking / 'component.csv')
+    component_marks = read_component(component, config)
     for nb, out_nb in zip(nbs, out_nbs):
         _, login, _ = fname2login_ext(nb)
-        row = row4login(component_marks, login_col, login)
+        row = component_marks.loc[login].reset_index()
+        row.columns = ['Question type', 'Question', 'Mark']
         comp_mark_pth = Path(out_nb).parent / 'component_mark.md'
         comp_mark_pth.write_text(f"""\
-# Mark summary for this notebook
+# Mark summary for {component} notebook
 
-{component_msg}Mark: {row['Mark']}
-""")
+""" + row.to_markdown(index=None))
 
 
 def summarize_final_marks(config,
                           pth_maker,
                           final_msg=None):
     final_msg = add_nn(final_msg)
     final_marks = pd.read_csv(config['mark_fname'])
@@ -249,18 +248,20 @@
     if in_path.is_file():
         shutil.copy2(in_path, out_path)
     else:
         warn(f'No file {in_path}')
 
 
 def cp_summaries(config, root_path):
+    root_path = Path(root_path)
     in_path = Path(config['base_path'])
     cp_if(in_path.parent / 'about_marking.md', root_path)
     cp_if(in_path / 'README.md', root_path)
-    cp_if(in_path / 'criteria.md', root_path)
+    for crit_path in in_path.glob('*criteria.md'):
+        cp_if(crit_path, root_path)
     cp_if(in_path / config['mark_fname'], root_path / 'final.csv')
 
 
 def clean_nb_dirs(nb_fnames):
     written_paths = set(op.dirname(fn) for fn in nb_fnames)
     for wp in written_paths:
         clean_dir(wp,
@@ -307,21 +308,21 @@
         nbs = get_notebooks(component_path, lexts=('.rmd',))
         out_nbs = [pth_maker(f) for f in nbs]
         write_component(component_path, nbs, out_nbs)
         clean_nb_dirs(out_nbs)
         out_nb_path = op.dirname(out_nbs[-1])
         if args.type == 'moderation' and out_nbs:
             write_marking(component_path, out_nb_path)
-        else:
-            summarize_component_marking(
-                config,
-                component_path,
-                nbs,
-                out_nbs,
-                args.component_msg)
+            continue
+        summarize_component_marking(
+            config,
+            component,
+            nbs,
+            out_nbs,
+            args.component_msg)
     if args.type == 'moderation':
         cp_summaries(config, root_path)
     elif args.type == 'feedback':
         summarize_final_marks(config,
                               pth_maker,
                               args.final_msg)
```

### Comparing `mcpmark-0.1/mcpmark/cli/merge_marks.py` & `mcpmark-1.0a2/mcpmark/cli/merge_marks.py`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/cli/mk_minimal_csv.py` & `mcpmark-1.0a2/mcpmark/cli/mk_minimal_csv.py`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/cli/parse_manual_scores.py` & `mcpmark-1.0a2/mcpmark/cli/parse_manual_scores.py`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/cli/rename_named_dirs.py` & `mcpmark-1.0a2/mcpmark/cli/rename_named_dirs.py`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/cli/run_notebooks.py` & `mcpmark-1.0a2/mcpmark/cli/run_notebooks.py`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/cli/scale_combine.py` & `mcpmark-1.0a2/mcpmark/cli/scale_combine.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,81 @@
 #!/usr/bin/env python
 """ Scale marks to final totals, combine components (if more than one).
 """
 
-import os
-import os.path as op
+from pathlib import Path
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 
 import pandas as pd
 
-from ..mcputils import (read_config, component_path)
+from ..mcputils import read_config, component_path, MCPError
 
 
-def get_parser():
-    parser = ArgumentParser(description=__doc__,  # Usage from docstring
-                            formatter_class=RawDescriptionHelpFormatter)
-    parser.add_argument('--config-path',
-                        default=op.join(os.getcwd(), 'assign_config.yaml'),
-                        help='Path to config file')
-    return parser
+TINY = 1e-15
+
+
+def read_component(name, config):
+    return read_component_csv(Path(component_path(config, name)) /
+                              'marking' /
+                              'component.csv')
+
+
+def remove_unnamed(seq_of_seq, rep):
+    out = []
+    for seq in seq_of_seq:
+        out.append(tuple([s if not s.startswith('Unnamed: ') else rep
+                          for s in seq]))
+    return tuple(out)
+
+
+def read_component_csv(csv_pth):
+    if not csv_pth.is_file():
+        raise RuntimeError(f'No component csv file at {csv_pth}; '
+                            'Do you need to run mcp-grade-component?')
+    comp_marks = pd.read_csv(csv_pth, header=[0, 1], index_col=0)
+    # Check for old API
+    if list(comp_marks)[0][0] == 'Mark' and len(comp_marks.columns) == 1:
+        raise MCPError(f'{csv_pth} looks like the old component CSV format; '
+                       'use mcpmark < 1.0 to use these files')
+    comp_marks.columns = remove_unnamed(comp_marks.columns, '')
+    return comp_marks
 
 
 def process_components(config):
-    series = {}
-    stid_col = config['student_id_col']
     components = config['components']
     scaled_max = sum([components[c]['scaled_to'] for c in components])
+    final = pd.DataFrame()
     for name, info in components.items():
-        csv_pth = op.join(component_path(config, name),
-                          'marking',
-                          'component.csv')
-        if not op.isfile(csv_pth):
-            raise RuntimeError(f'No component csv file at {csv_pth}; '
-                               'Do you need to run mcp-grade-component?')
-        df = pd.read_csv(csv_pth).set_index(stid_col)
-        series[name] = df['Mark'] * info['scaled_to'] / info['actual_max']
-    final = pd.DataFrame(series)
+        df = read_component(name, config)
+        final[name] = df['Total'] * info['scaled_to'] / info['actual_max']
     total = final.sum(axis=1)
-    if config.get('round_final'):
-        total = round(total)
-    final['Percent'] = total / scaled_max * 100
+    if config.get('round_final') or config.get('round_total'):
+        total = round(total + TINY)
+    percent = total / scaled_max * 100
+    final['Percent'] = (round(percent + TINY) if config.get('round_percent')
+                        else percent)
     final['Total'] = total
-    return final
+    return final.reset_index().rename(
+        columns={'index': config['student_id_col']})
+
+
+def get_parser():
+    parser = ArgumentParser(description=__doc__,  # Usage from docstring
+                            formatter_class=RawDescriptionHelpFormatter)
+    parser.add_argument('--config-path',
+                        default=Path('assign_config.yaml'),
+                        help='Path to config file')
+    return parser
 
 
 def main():
     parser = get_parser()
     args = parser.parse_args()
     config = read_config(args.config_path)
     all_answers = process_components(config)
-    out_csv = op.join(config['base_path'], config['mark_fname'])
-    all_answers.to_csv(out_csv)
+    out_csv = Path(config['base_path']) / config['mark_fname']
+    all_answers.to_csv(out_csv, index=None)
     print(all_answers.describe())
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mcpmark-0.1/mcpmark/mcputils.py` & `mcpmark-1.0a2/mcpmark/mcputils.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import os
 import os.path as op
 from pathlib import Path
 import re
 import shutil
 from fnmatch import fnmatch
+from functools import partial
 from zipfile import ZipFile, BadZipFile
 
 import yaml
 import numpy as np
 import pandas as pd
 import nbformat.v4 as nbf
 from nbconvert.preprocessors import ExecutePreprocessor
@@ -128,46 +129,65 @@
             dirs[:] = ok_dirs
             for fn in files:
                 if fn.startswith('.'):
                     os.unlink(op.join(root, fn))
         return this_out
 
     def login2jh(self, login):
-        return login
+        return login.lower().replace('-', '-2d')
 
     def login2uuid(self, login):
         return login
 
 
 class CanvasHandler(SubmissionHandler):
 
     def get_student_id(self, fname, df=None):
-        if isinstance(df, (None, str)):
+        if self.config.get('anonymous'):
+            name = Path(fname).name
+            return name.split('_')[2 if name.startswith('LATE_') else 1]
+        if isinstance(df, (type(None), str)):
             df = self.read_student_data(df)
         name1, name2, id_no = ct.fname2key(fname)
         assert name2 == ''
         return df.loc[int(id_no), self.config['student_id_col']]
 
     def read_student_data(self, fname=None):
         fname = self.config['canvas_export_path'] if fname is None else fname
         required = ('ID', 'Student', 'SIS User ID', 'SIS Login ID', 'Section')
         dtypes = {'ID': int, 'SIS User ID': int}
         df = ct.to_minimal_df(fname, required, dtypes)
+        df['Email'] = df['SIS Login ID'].str.lower()
+        df['school_user'] = (df['SIS Login ID'].
+                             str.split('@', expand=True)
+                             .iloc[:, 0])
+        if 'github_users_path' in self.config:
+            gh_users = pd.read_csv(self.config['github_users_path'])
+            df = df.merge(gh_users[['gh_user', 'Email']],
+                                   on='Email',
+                                   how='left')
         return df.set_index('ID')
 
 
 def attend_fn2info(fname):
     froot = Path(fname).stem
     match = re.search(r'(.*)\s+\((.+\..+@lis\.ac\.uk)\)',
                         froot)
     if match is None:
         raise ValueError(f'{froot} does not match')
     return match.groups()
 
 
+def astype_apply(val, converter):
+    try:
+        return converter(val)
+    except ValueError:
+        return None
+
+
 class AttendHandler(SubmissionHandler):
 
     def __init__(self, config):
         super().__init__(config)
         if not 'github_users_path' in config:
             raise ValueError('Need `github_users_path` in config')
         df = pd.read_csv(config['github_users_path'])
@@ -183,45 +203,69 @@
         rows = df[df['Email'] == email]
         assert len(rows) == 1
         return rows.iloc[0][self.config['student_id_col']]
 
     def read_student_data(self, fname=None):
         fname = self.config['attendance_export_path'] if fname is None else fname
         required = ['StudentId', 'Forename', 'Surname', 'Email',
-                   'gh_user']
+                    'school_user', 'gh_user']
         df = pd.read_excel(fname)
         dtypes = {'StudentId': int}
         for name, dt in dtypes.items():
-            df[name] = df[name].astype(dt)
+            df[name] = df[name].apply(astype_apply, converter=dt)
+        df['school_user'] = df['Email'].str.split('@').apply(lambda v : v[0])
         df = df.merge(self.gh_users, on='Email', how='left')
         missing = df['gh_user'].isna()
         if np.any(missing):
             raise ValueError('Missing gh_user for ' +
                              ', '.join(df.loc[missing, 'Email']))
         return df[required].set_index('StudentId')
 
-    def login2jh(self, login):
-        return login.lower().replace('-', '-2d')
-
     def login2uuid(self, login):
         df = self._def_student_data
         login_col = self.config['student_id_col']
         rows = df[df[login_col] == login]
         if len(rows) == 0:
             raise ValueError(f'No rows for login {login}')
         if len(rows) > 1:
             raise ValueError(f'More than one row for login {login}')
         return str(rows.iloc[0].name)
 
 
+class CsvHandler(SubmissionHandler):
+
+    def get_student_id(self, fname, df=None):
+        """ Work out student ID from given filename
+        """
+        if isinstance(df, (None, str)):
+            df = self.read_student_data(df)
+        name, email = attend_fn2info(fname)
+        rows = df[df['Email'] == email]
+        assert len(rows) == 1
+        return rows.iloc[0][self.config['student_id_col']]
+
+    def read_student_data(self, fname=None):
+        fname = self.config['user_csv_path'] if fname is None else fname
+        required = ['Name', 'Email', 'school_user', 'gh_user']
+        df = pd.read_csv(fname, comment='#')
+        df['school_user'] = df['Email'].str.split('@').apply(lambda v : v[0])
+        missing = df['gh_user'].isna()
+        if np.any(missing):
+            raise ValueError('Missing gh_user for ' +
+                             ', '.join(df.loc[missing, 'Email']))
+        return df[required].set_index('gh_user', drop=False)
+
+
 def make_submission_handler(config):
     if 'canvas_export_path' in config:
         return CanvasHandler(config)
     elif 'attendance_export_path' in config:
         return AttendHandler(config)
+    elif 'user_csv_path' in config:
+        return CsvHandler(config)
     else:
         raise ValueError('No Canvas or Attendance path')
 
 
 def get_minimal_df(config):
     return make_submission_handler(config).get_minimal_df()
 
@@ -620,7 +664,29 @@
     else:
         to_test = set(args.component) if multi_component else {args.component}
         if to_test.difference(comp_names):
             raise ValueError(
                 f'Component{comp_suff} "{args.component}" must be in ' +
                 ', '.join(comp_names))
     return args, config
+
+
+def has_md_text(nb, cell_regex, flags=None):
+    """ True if notebook `nb` has Markdown text matching `cell_regex`
+    """
+    flags = re.I if flags is None else flags
+    if not hasattr(cell_regex, 'pattern'):
+        cell_regex = re.compile(cell_regex, flags=flags)
+    for cell in nb.cells:
+        if cell['cell_type'] != 'markdown' or not 'source' in cell:
+            continue
+        if cell_regex.search(cell['source'].lower()):
+            return True
+    return False
+
+
+def has_md_text_component(nb, nb_path, cell_regex, flags=None):
+    return nb_path if has_md_text(nb, cell_regex) else None
+
+
+def has_md_checker(cell_regex, flags=None):
+    return partial(has_md_text_component, cell_regex=cell_regex)
```

### Comparing `mcpmark-0.1/mcpmark/tests/data/blank_comp_config.yaml` & `mcpmark-1.0a2/mcpmark/tests/data/blank_comp_config.yaml`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/tests/data/empty_comp_config.yaml` & `mcpmark-1.0a2/mcpmark/tests/data/empty_comp_config.yaml`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/tests/data/no_comp_config.yaml` & `mcpmark-1.0a2/mcpmark/tests/data/no_comp_config.yaml`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/tests/data/one_comp_config.yaml` & `mcpmark-1.0a2/mcpmark/tests/data/one_comp_config.yaml`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/mcpmark/tests/test_mcputils.py` & `mcpmark-1.0a2/mcpmark/tests/test_mcputils.py`

 * *Files identical despite different names*

### Comparing `mcpmark-0.1/PKG-INFO` & `mcpmark-1.0a2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,32 @@
-Metadata-Version: 2.1
-Name: mcpmark
-Version: 0.1
-Summary: Tools for grading multiple notebook component exercises.
-Home-page: https://github.com/matthew-brett/mcpmark
-Author: Matthew Brett
-Author-email: matthew.brett@gmail.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: gradools
-Requires-Dist: rnbgrader>=0.2
-
 # (Multiple) component marking
 
 Some tools I use when marking homework with with single or multiple Jupyter
 notebook components.
 
 The notebooks may have questions for manual marking, and plots for marking.
 
 They assume some Canvas](https://www.instructure.com/canvas) conventions of
 naming files, and grade output CSV format.
 
-The tools consist primarily command line utilities, with some supporting code
-in a utility library.
+The tools are mainly command line utilities, with some supporting code in
+a utility library.
 
 ## Quickstart
 
 ### For single component submission:
 
 ```
 COMPONENTS_DIR=components
 mcp-check-unpack
 mcp-prepare-components
 mcp-find-duplicates $COMPONENTS_DIR/*/*.Rmd
 mcp-cp-models
 mcp-extract-manual
-rnbg-allow-raise $COMPONENTS_DIR/*/*.Rmd --show-error
+mcp-allow-raise
 mcp-extract-plots
 mcp-grade-nbs
 # Review `<component>/marking/autograde.md`.
 # Rerun after any edits.
 mcp-grade-nbs
 mcp-grade-component
 mcp-scale-combine
@@ -52,21 +38,23 @@
 COMPONENTS_DIR=components
 mcp-check-unpack
 mcp-prepare-components
 mcp-find-duplicates $COMPONENTS_DIR/*/*.Rmd
 mcp-cp-models
 # For each component
     COMPONENT=my_component
-    rnbg-allow-raise $COMPONENTS_DIR/$COMPONENT/*.Rmd --show-error
+    mcp-allow-raise $COMPONENT
     mcp-grade-nbs $COMPONENT
-    # Review `$COMPONENT/marking/autograde.md`.
+    # Review `$COMPONENTS_DIR/$COMPONENT/marking/autograde.md`.
     # Rerun after any edits.
     mcp-grade-nbs $COMPONENT
     mcp-extract-manual $COMPONENT
+    # Mark manual questions in $COMPONENT/marking/*_report.md files
     mcp-extract-plots $COMPONENT
+    # Mark plot questions in $COMPONENT/marking/plot_nb.ipynb file
     mcp-grade-component $COMPONENT
 # Finally
 mcp-scale-combine
 ```
 
 ## Getting set up
 
@@ -147,16 +135,14 @@
     * Test tests with `grade_oknb.py`.
     * Copy tests etc into components directory with `mcp-cp-models`
     * e.g. `mcp-find-duplicates components/my_component/*.Rmd` to analyze
       duplicates, write summary into some file, say `report.md`.
     * Check notebook execution with `mcp-run-notebooks <path_to_notebooks>`.
       Consider running this with e.g. `rerun mcp-run-notebooks
       components/pandering` to continuously test notebooks.
-    * Move any irreparable notebooks to `broken` directory, and mark in
-      `marking/broken.csv` file.
     * `mcp-extract-manual <component_name>` (component name optional for single
       component submissions). Edit notebooks where manual component not found.
       Maybe e.g. `rerun mcp-extract-manual pandering`.
     * Mark generated manual file in `<component>/marking/*_report.md`.
     * Check manual scoring with something like `mcp-manual-scores
       components/lymphoma/dunleavy_plausible_report.md`.  Or you can leave
       that until grading the whole component with `mcp-grade-component`.
@@ -180,8 +166,7 @@
   even when there is only one component (in order to do the rescaling).
 * `mcp-export-marks` to convert the output of `ncp-rescale-combines` to
   a format for import into Canvas.
 
 ## Utilities
 
 * `mcputils` - various utilities for supporting the scripts.
-
```

