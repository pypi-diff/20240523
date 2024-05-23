# Comparing `tmp/pmac_motorhome-1.5.tar.gz` & `tmp/pmac_motorhome-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pmac_motorhome/pmac_motorhome/dist/tmp0427lhbo/pmac_motorhome-1.5.tar", last modified: Mon Jan 22 14:24:54 2024, max compression
+gzip compressed data, was "/home/runner/work/pmac_motorhome/pmac_motorhome/dist/tmphs9_q8ay/pmac_motorhome-1.6.tar", last modified: Thu May 23 15:36:04 2024, max compression
```

## Comparing `pmac_motorhome-1.5.tar` & `pmac_motorhome-1.6.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/
--rw-rw-r--   0 runner    (1001) docker     (127)       71 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/MANIFEST.in
--rw-rw-r--   0 runner    (1001) docker     (127)     3170 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     2094 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/converter/
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3044 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/converter.py
--rw-rw-r--   0 runner    (1001) docker     (127)      157 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/indent.py
--rw-rw-r--   0 runner    (1001) docker     (127)    21841 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/motionarea.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/converter/old_motorhome/
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/old_motorhome/__init__.py
--rwxrwxr-x   0 runner    (1001) docker     (127)    43004 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/old_motorhome/motorhome.py
--rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/pipemessage.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/converter/shim/
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/shim/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/shim/controllertype.py
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/shim/functions.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/shim/globals.py
--rw-rw-r--   0 runner    (1001) docker     (127)      753 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/shim/group.py
--rw-rw-r--   0 runner    (1001) docker     (127)      384 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/shim/motor.py
--rw-rw-r--   0 runner    (1001) docker     (127)      915 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/shim/motorhome.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4291 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/converter/shim/plc.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/pmac_motorhome/
--rw-rw-r--   0 runner    (1001) docker     (127)      214 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3850 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/pmac_motorhome/_version_git.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5420 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/commands.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2015 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/constants.py
--rw-rw-r--   0 runner    (1001) docker     (127)    22313 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/group.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6514 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/motor.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1085 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/onlyaxes.py
--rw-rw-r--   0 runner    (1001) docker     (127)    12678 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/plc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      887 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/plcgenerator.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8176 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/sequences.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/
--rw-rw-r--   0 runner    (1001) docker     (127)      315 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/check_homed.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)     1585 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/continue_home_maintain_axes_offset.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      303 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/debug_pause.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      622 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/disable_axis_limits.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/disable_limits.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      780 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_off_home.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      709 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_relative.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      493 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_to_hard_limit.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_to_home.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)       10 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_to_home_if_on_limit.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      783 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_to_hstop.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_to_initial_pos.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      608 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_to_limit.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_to_soft_limit.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/home.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)     1790 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/jog_if_on_limit.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)     5186 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/plc.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/post_home_action.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)       10 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/pre_home_action.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      135 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/restore_limits.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      272 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/store_position_diff.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)     1462 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/wait_for_done.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      291 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/power/zero_encoders.pmc.jinja
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/
--rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/check_homed.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)     1408 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/continue_home_maintain_axes_offset.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/debug_pause.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      608 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/disable_axis_limits.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/disable_limits.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      671 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_off_home.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_relative.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_to_hard_limit.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      722 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_to_home.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)       10 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_to_home_if_on_limit.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_to_hstop.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_to_initial_pos.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      499 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_to_limit.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      607 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_to_soft_limit.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/home.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)     1620 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/jog_if_on_limit.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)     4213 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/plc.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      385 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/post_home_action.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/pre_home_action.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      133 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/restore_limits.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      196 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/store_position_diff.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)     1358 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/wait_for_done.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)      217 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/zero_encoders.pmc.jinja
--rw-rw-r--   0 runner    (1001) docker     (127)    10676 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/snippets.py
--rw-rw-r--   0 runner    (1001) docker     (127)      984 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pmac_motorhome/template.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/pmac_motorhome.egg-info/
--rw-rw-r--   0 runner    (1001) docker     (127)     3170 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/pmac_motorhome.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     3720 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/pmac_motorhome.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1001) docker     (127)        1 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/pmac_motorhome.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       71 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/pmac_motorhome.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       96 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/pmac_motorhome.egg-info/requires.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/pmac_motorhome.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      340 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1121 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/setup.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/setup.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/tests/__init__.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:54.000000 pmac_motorhome-1.5/tests/converter/
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/tests/converter/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      554 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/tests/test_checks.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2669 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/tests/test_converter.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14045 2024-01-22 14:24:31.000000 pmac_motorhome-1.5/tests/test_pmac_motorhome.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/
+-rw-rw-r--   0 runner    (1001) docker     (127)       71 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/MANIFEST.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     3170 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     2094 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/converter/
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3044 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/converter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      157 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/indent.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    21841 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/motionarea.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/converter/old_motorhome/
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/old_motorhome/__init__.py
+-rwxrwxr-x   0 runner    (1001) docker     (127)    43004 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/old_motorhome/motorhome.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/pipemessage.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/converter/shim/
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/shim/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/shim/controllertype.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/shim/functions.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/shim/globals.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      753 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/shim/group.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      384 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/shim/motor.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      915 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/shim/motorhome.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4291 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/converter/shim/plc.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/pmac_motorhome/
+-rw-rw-r--   0 runner    (1001) docker     (127)      214 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3850 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/pmac_motorhome/_version_git.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5420 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/commands.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2015 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/constants.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    22442 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/group.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6514 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/motor.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1085 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/onlyaxes.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    12678 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/plc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      887 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/plcgenerator.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8176 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/sequences.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/
+-rw-rw-r--   0 runner    (1001) docker     (127)      315 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/check_homed.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)     1585 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/continue_home_maintain_axes_offset.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      303 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/debug_pause.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      622 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/disable_axis_limits.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/disable_limits.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      780 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_off_home.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      709 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_relative.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      493 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_to_hard_limit.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_to_home.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)       10 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_to_home_if_on_limit.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      783 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_to_hstop.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_to_initial_pos.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      608 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_to_limit.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_to_soft_limit.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/home.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)     1790 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/jog_if_on_limit.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)     5226 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/plc.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/post_home_action.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)       10 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/pre_home_action.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      135 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/restore_limits.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      272 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/store_position_diff.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)     1462 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/wait_for_done.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      291 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/power/zero_encoders.pmc.jinja
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/
+-rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/check_homed.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)     1408 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/continue_home_maintain_axes_offset.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/debug_pause.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      608 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/disable_axis_limits.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/disable_limits.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      671 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_off_home.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_relative.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_to_hard_limit.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      722 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_to_home.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)       10 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_to_home_if_on_limit.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_to_hstop.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_to_initial_pos.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      499 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_to_limit.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      607 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_to_soft_limit.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/home.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)     1620 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/jog_if_on_limit.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)     4256 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/plc.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      385 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/post_home_action.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/pre_home_action.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      133 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/restore_limits.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      196 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/store_position_diff.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)     1358 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/wait_for_done.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)      217 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/zero_encoders.pmc.jinja
+-rw-rw-r--   0 runner    (1001) docker     (127)    10676 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/snippets.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      984 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pmac_motorhome/template.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/pmac_motorhome.egg-info/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3170 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/pmac_motorhome.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     3720 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/pmac_motorhome.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/pmac_motorhome.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       71 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/pmac_motorhome.egg-info/entry_points.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       96 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/pmac_motorhome.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/pmac_motorhome.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      340 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1121 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/setup.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/setup.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/tests/__init__.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:36:04.000000 pmac_motorhome-1.6/tests/converter/
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/tests/converter/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      554 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/tests/test_checks.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2669 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/tests/test_converter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14045 2024-05-23 15:35:44.000000 pmac_motorhome-1.6/tests/test_pmac_motorhome.py
```

### Comparing `pmac_motorhome-1.5/PKG-INFO` & `pmac_motorhome-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmac_motorhome
-Version: 1.5
+Version: 1.6
 Summary: Generate homing procedures in pmc code for Delta Tau motion controllers
 Home-page: https://github.com/dls-controls/pmac_motorhome
 Author: Arvinder Palaha
 Author-email: arvinder.palaha@diamond.ac.uk
 License: Apache License 2.0
 Description: pmac_motorhome
         ===========================
```

### Comparing `pmac_motorhome-1.5/README.rst` & `pmac_motorhome-1.6/README.rst`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/converter/converter.py` & `pmac_motorhome-1.6/converter/converter.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/converter/motionarea.py` & `pmac_motorhome-1.6/converter/motionarea.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/converter/old_motorhome/motorhome.py` & `pmac_motorhome-1.6/converter/old_motorhome/motorhome.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/converter/pipemessage.py` & `pmac_motorhome-1.6/converter/pipemessage.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/converter/shim/functions.py` & `pmac_motorhome-1.6/converter/shim/functions.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/converter/shim/globals.py` & `pmac_motorhome-1.6/converter/shim/globals.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/converter/shim/group.py` & `pmac_motorhome-1.6/converter/shim/group.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/converter/shim/motorhome.py` & `pmac_motorhome-1.6/converter/shim/motorhome.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/converter/shim/plc.py` & `pmac_motorhome-1.6/converter/shim/plc.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/_version_git.py` & `pmac_motorhome-1.6/pmac_motorhome/_version_git.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # versiongit-1.0 (https://github.com/dls-controls/versiongit)
 import os
 import re
 import sys
 from subprocess import STDOUT, CalledProcessError, check_output
 
 # These will be filled in if git archive is run or by setup.py cmdclasses
-GIT_REFS = 'tag: 1.5'
-GIT_SHA1 = 'a004052'
+GIT_REFS = 'tag: 1.6'
+GIT_SHA1 = '5250bf4'
 
 # Git describe gives us sha1, last version-like tag, and commits since then
 CMD = "git describe --tags --dirty --always --long --match=[0-9]*[-.][0-9]*"
 
 
 def get_version_from_git(path=None):
     """Try to parse version from git describe, fallback to git archive tags"""
```

### Comparing `pmac_motorhome-1.5/pmac_motorhome/commands.py` & `pmac_motorhome-1.6/pmac_motorhome/commands.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/constants.py` & `pmac_motorhome-1.6/pmac_motorhome/constants.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/group.py` & `pmac_motorhome-1.6/pmac_motorhome/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,21 +124,25 @@
         for htype
 
         Args:
             htype (str): Homing sequence type e.g. RLIM HSW etc.
         """
         group = Group.instance()
         enc_axes = ""
+        if group.controller is ControllerType.pbrick:
+            line_start = "//"
+        else:
+            line_start = ";"
         if len(group.encoders)> 0:
             enc_axes = ", enc_axes = {enc}".format(enc=group.encoders)
 
             
         group.comment = "\n".join(
             [
-                f";  Axis {ax.axis}: htype = {htype}, "
+                f"{line_start}  Axis {ax.axis}: htype = {htype}, "
                 f"jdist = {ax.jdist}, post = {ax.post_home_with_distance}" 
                 f"{enc_axes}"
                 for ax in group.motors
             ]
         )
 
     @classmethod
@@ -346,15 +350,15 @@
         Generate a command string for all group axes: check in postiion
         relOperator (relationalOperator) is required for power pmac based
         controllers as each variable needs to be evaluated separately
         """
 
         if self.controller is ControllerType.pbrick:
             pbrickVar = "Motor[{axis}].InPos"
-            return self._all_axes(f"{pbrickVar} {relOperator} {value} ", f"{operator} ")
+            return self._all_axes(f"{pbrickVar} {relOperator} {value} ", "|| ")
         else:
             return self._all_axes("m{axis}40", operator)
 
     def limits(self, relOperator="!=", value=0) -> str:
         """
         Generate a command string for all group axes: check limits
         relOperator (relationalOperator) is required for power pmac based
```

### Comparing `pmac_motorhome-1.5/pmac_motorhome/motor.py` & `pmac_motorhome-1.6/pmac_motorhome/motor.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/onlyaxes.py` & `pmac_motorhome-1.6/pmac_motorhome/onlyaxes.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/plc.py` & `pmac_motorhome-1.6/pmac_motorhome/plc.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/plcgenerator.py` & `pmac_motorhome-1.6/pmac_motorhome/plcgenerator.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/sequences.py` & `pmac_motorhome-1.6/pmac_motorhome/sequences.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/power/continue_home_maintain_axes_offset.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/power/continue_home_maintain_axes_offset.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/power/disable_axis_limits.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/power/disable_axis_limits.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/power/disable_limits.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/power/disable_limits.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_off_home.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_off_home.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_relative.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_relative.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_to_home.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_to_home.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_to_hstop.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_to_hstop.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_to_limit.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_to_limit.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/power/drive_to_soft_limit.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/power/drive_to_soft_limit.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/power/jog_if_on_limit.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/power/jog_if_on_limit.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/power/plc.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/power/plc.pmc.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 CLOSE
 
 //#################################################################
 // Autogenerated Homing PLC for {{plc.controller.value}}, DO NOT MODIFY
 {% for group in plc.groups -%}
 // Group {{ group.group_num }}:
-// {{ group.comment }}
+{% if group.comment != None %}
+{{ group.comment }}
+{% endif %}
 {% endfor -%}
 //
 // Manual homing instructions:
 // Run homing for group GROUP_NUM: P{{plc.plc_num}}02 = GROUP_NUM enable PLC{{plc.plc_num}}
 // Run homing: enable PLC{{plc.plc_num}}
 // Run homing in debug mode: P{{plc.plc_num}}01 = 9 enable PLC{{plc.plc_num}}
 // Pause homing: P{{plc.plc_num}}01 = 8
```

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/power/post_home_action.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/power/post_home_action.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/power/wait_for_done.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/power/wait_for_done.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/continue_home_maintain_axes_offset.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/continue_home_maintain_axes_offset.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/disable_axis_limits.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/disable_axis_limits.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_off_home.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_off_home.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_relative.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_relative.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_to_hard_limit.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_to_hard_limit.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_to_home.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_to_home.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_to_hstop.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_to_hstop.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_to_initial_pos.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_to_initial_pos.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/drive_to_soft_limit.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/drive_to_soft_limit.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/jog_if_on_limit.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/jog_if_on_limit.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/plc.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/plc.pmc.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 CLOSE
 
 ;####################################################
 ; Autogenerated Homing PLC for {{plc.controller.value}}, DO NOT MODIFY
 {% for group in plc.groups -%}
 ; Group {{ group.group_num }}:
+{% if group.comment != None %}
 {{ group.comment }}
+{% endif %}
 {% endfor -%}
 ;####################################################
 
 ; Use a different timer for each PLC
 #define timer             i(5111+({{plc.plc_num}}&30)*50+{{plc.plc_num}}%2)
 ; Make timer more readable
 #define MilliSeconds      * 8388608/i10
```

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets/turbo/wait_for_done.pmc.jinja` & `pmac_motorhome-1.6/pmac_motorhome/snippets/turbo/wait_for_done.pmc.jinja`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/snippets.py` & `pmac_motorhome-1.6/pmac_motorhome/snippets.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome/template.py` & `pmac_motorhome-1.6/pmac_motorhome/template.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/pmac_motorhome.egg-info/PKG-INFO` & `pmac_motorhome-1.6/pmac_motorhome.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmac-motorhome
-Version: 1.5
+Version: 1.6
 Summary: Generate homing procedures in pmc code for Delta Tau motion controllers
 Home-page: https://github.com/dls-controls/pmac_motorhome
 Author: Arvinder Palaha
 Author-email: arvinder.palaha@diamond.ac.uk
 License: Apache License 2.0
 Description: pmac_motorhome
         ===========================
```

### Comparing `pmac_motorhome-1.5/pmac_motorhome.egg-info/SOURCES.txt` & `pmac_motorhome-1.6/pmac_motorhome.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/setup.cfg` & `pmac_motorhome-1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/tests/test_checks.py` & `pmac_motorhome-1.6/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/tests/test_converter.py` & `pmac_motorhome-1.6/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `pmac_motorhome-1.5/tests/test_pmac_motorhome.py` & `pmac_motorhome-1.6/tests/test_pmac_motorhome.py`

 * *Files identical despite different names*

