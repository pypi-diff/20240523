# Comparing `tmp/cryoemservices-0.2.2.tar.gz` & `tmp/cryoemservices-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryoemservices-0.2.2.tar", last modified: Fri May  3 09:55:34 2024, max compression
+gzip compressed data, was "cryoemservices-0.2.4.tar", last modified: Thu May 23 10:03:50 2024, max compression
```

## Comparing `cryoemservices-0.2.2.tar` & `cryoemservices-0.2.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.157049 cryoemservices-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-05-03 09:55:34.157049 cryoemservices-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-03 09:55:34.161049 cryoemservices-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.149048 cryoemservices-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.149048 cryoemservices-0.2.2/src/cryoemservices/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.153049 cryoemservices-0.2.2/src/cryoemservices/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/cli/resubmit_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.153049 cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/combine_star_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/combine_star_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/reextract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.157049 cryoemservices-0.2.2/src/cryoemservices/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/bfactor_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/cluster_submission.py
--rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/cryolo.py
--rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/ctffind.py
--rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/denoise_slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17110 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/extract_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/icebreaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/images_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    46671 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/ispyb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/ispyb_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27301 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/motioncorr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/motioncorr_slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/node_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    21298 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/select_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/select_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)    22125 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/tomo_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/services/tomo_align_slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.157049 cryoemservices-0.2.2/src/cryoemservices/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/util/dispatcher_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/util/slurm_submission.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/util/spa_output_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/util/spa_relion_service_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.157049 cryoemservices-0.2.2/src/cryoemservices/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/wrappers/class2d_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24579 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/wrappers/class3d_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-05-03 09:55:30.000000 cryoemservices-0.2.2/src/cryoemservices/wrappers/refine3d_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:55:34.157049 cryoemservices-0.2.2/src/cryoemservices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-05-03 09:55:34.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-03 09:55:34.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:55:34.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-03 09:55:34.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:55:33.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-03 09:55:34.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 09:55:34.000000 cryoemservices-0.2.2/src/cryoemservices.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:50.772920 cryoemservices-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-05-23 10:03:50.772920 cryoemservices-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-23 10:03:50.772920 cryoemservices-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:50.764921 cryoemservices-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:50.764921 cryoemservices-0.2.4/src/cryoemservices/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:50.768921 cryoemservices-0.2.4/src/cryoemservices/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/cli/resubmit_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:50.768921 cryoemservices-0.2.4/src/cryoemservices/pipeliner_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/pipeliner_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/pipeliner_plugins/combine_star_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/pipeliner_plugins/combine_star_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/pipeliner_plugins/reextract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:50.772920 cryoemservices-0.2.4/src/cryoemservices/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/bfactor_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/cluster_submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/cryolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/ctffind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/denoise_slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17110 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/extract_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/icebreaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/images_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46671 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/ispyb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/ispyb_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27301 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/motioncorr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/motioncorr_slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/node_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25708 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/select_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/select_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22125 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/tomo_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/services/tomo_align_slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:50.772920 cryoemservices-0.2.4/src/cryoemservices/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/util/dispatcher_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/util/slurm_submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/util/spa_output_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/util/spa_relion_service_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:50.772920 cryoemservices-0.2.4/src/cryoemservices/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/wrappers/class2d_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24579 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/wrappers/class3d_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-05-23 10:03:47.000000 cryoemservices-0.2.4/src/cryoemservices/wrappers/refine3d_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:03:50.772920 cryoemservices-0.2.4/src/cryoemservices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-05-23 10:03:50.000000 cryoemservices-0.2.4/src/cryoemservices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-23 10:03:50.000000 cryoemservices-0.2.4/src/cryoemservices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:03:50.000000 cryoemservices-0.2.4/src/cryoemservices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-23 10:03:50.000000 cryoemservices-0.2.4/src/cryoemservices.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:03:50.000000 cryoemservices-0.2.4/src/cryoemservices.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-23 10:03:50.000000 cryoemservices-0.2.4/src/cryoemservices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 10:03:50.000000 cryoemservices-0.2.4/src/cryoemservices.egg-info/top_level.txt
```

### Comparing `cryoemservices-0.2.2/LICENSE` & `cryoemservices-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/PKG-INFO` & `cryoemservices-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryoemservices
-Version: 0.2.2
+Version: 0.2.4
 Summary: Services for CryoEM processing
 Author: Diamond Light Source - Data Analysis et al.
 Author-email: dataanalysis@diamond.ac.uk
 License: BSD 3-Clause
 Project-URL: GitHub, https://github.com/DiamondLightSource/cryoem-services
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/cryoem-services/issues
 Keywords: cryoem-services
```

### Comparing `cryoemservices-0.2.2/README.md` & `cryoemservices-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/setup.cfg` & `cryoemservices-0.2.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cryoemservices
-version = 0.2.2
+version = 0.2.4
 description = Services for CryoEM processing
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Diamond Light Source - Data Analysis et al.
 author_email = dataanalysis@diamond.ac.uk
 license = BSD 3-Clause
 license_files = LICENSE
```

### Comparing `cryoemservices-0.2.2/src/cryoemservices/cli/resubmit_wrapper.py` & `cryoemservices-0.2.4/src/cryoemservices/cli/resubmit_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/combine_star_files.py` & `cryoemservices-0.2.4/src/cryoemservices/pipeliner_plugins/combine_star_files.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/combine_star_job.py` & `cryoemservices-0.2.4/src/cryoemservices/pipeliner_plugins/combine_star_job.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/pipeliner_plugins/reextract.py` & `cryoemservices-0.2.4/src/cryoemservices/pipeliner_plugins/reextract.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/bfactor_setup.py` & `cryoemservices-0.2.4/src/cryoemservices/services/bfactor_setup.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/cluster_submission.py` & `cryoemservices-0.2.4/src/cryoemservices/services/cluster_submission.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/cryolo.py` & `cryoemservices-0.2.4/src/cryoemservices/services/cryolo.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/ctffind.py` & `cryoemservices-0.2.4/src/cryoemservices/services/ctffind.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/denoise_slurm.py` & `cryoemservices-0.2.4/src/cryoemservices/services/denoise_slurm.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/extract.py` & `cryoemservices-0.2.4/src/cryoemservices/services/extract.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/extract_class.py` & `cryoemservices-0.2.4/src/cryoemservices/services/extract_class.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/icebreaker.py` & `cryoemservices-0.2.4/src/cryoemservices/services/icebreaker.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/images.py` & `cryoemservices-0.2.4/src/cryoemservices/services/images.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/images_plugins.py` & `cryoemservices-0.2.4/src/cryoemservices/services/images_plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 
 def picked_particles(plugin_params):
     basefilename = plugin_params.parameters("file")
     if basefilename.endswith(".jpeg"):
         logger.info(f"Replacing jpeg extension with mrc extension for {basefilename}")
         basefilename = basefilename.replace(".jpeg", ".mrc")
     coords = plugin_params.parameters("coordinates")
+    selected_coords = plugin_params.parameters("selected_coordinates")
     pixel_size = plugin_params.parameters("pixel_size")
     if not pixel_size:
         # Legacy case of zocalo-relion
         pixel_size = plugin_params.parameters("angpix")
     diam = plugin_params.parameters("diameter")
     contrast_factor = plugin_params.parameters("contrast_factor", default=6)
     outfile = plugin_params.parameters("outfile")
@@ -136,25 +137,37 @@
     data = data.astype("uint8")
     with PIL.Image.fromarray(data).convert(mode="RGB") as bim:
         enhancer = ImageEnhance.Contrast(bim)
         enhanced = enhancer.enhance(contrast_factor)
         fim = enhanced.filter(ImageFilter.BLUR)
         dim = ImageDraw.Draw(fim)
         if coords and coords[0]:
+            # Orange circles for all coordinates
             for x, y in coords:
                 dim.ellipse(
                     [
                         (float(x) - radius, float(y) - radius),
                         (float(x) + radius, float(y) + radius),
                     ],
                     width=8,
                     outline="#f58a07",
                 )
         else:
             logger.warning(f"No coordinates provided for {basefilename}")
+        if selected_coords and selected_coords[0]:
+            # Green circles if selected coordinates are provided
+            for x, y in selected_coords:
+                dim.ellipse(
+                    [
+                        (float(x) - radius, float(y) - radius),
+                        (float(x) + radius, float(y) + radius),
+                    ],
+                    width=12,
+                    outline="#98df8a",
+                )
         try:
             fim.save(outfile)
         except FileNotFoundError:
             logger.error(
                 f"Trying to save to file {outfile} but directory does not exist"
             )
             return False
```

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/ispyb.py` & `cryoemservices-0.2.4/src/cryoemservices/services/ispyb.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/ispyb_buffer.py` & `cryoemservices-0.2.4/src/cryoemservices/services/ispyb_buffer.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/motioncorr.py` & `cryoemservices-0.2.4/src/cryoemservices/services/motioncorr.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/motioncorr_slurm.py` & `cryoemservices-0.2.4/src/cryoemservices/services/motioncorr_slurm.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/node_creator.py` & `cryoemservices-0.2.4/src/cryoemservices/services/node_creator.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/postprocess.py` & `cryoemservices-0.2.4/src/cryoemservices/services/postprocess.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/select_classes.py` & `cryoemservices-0.2.4/src/cryoemservices/services/select_classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 import re
 import shutil
 import subprocess
 from contextlib import redirect_stdout
 from pathlib import Path
 
+import mrcfile
 import numpy as np
 import workflows.recipe
 from gemmi import cif
 from pydantic import BaseModel, Field, ValidationError
 from workflows.services.common_service import CommonService
 
 from cryoemservices.pipeliner_plugins.combine_star_files import (
@@ -20,14 +21,15 @@
 )
 from cryoemservices.util.spa_relion_service_options import RelionServiceOptions
 
 
 class SelectClassesParameters(BaseModel):
     input_file: str = Field(..., min_length=1)
     combine_star_job_number: int
+    particle_diameter: float
     class2d_fraction_of_classes_to_remove: float = 0.9
     particles_file: str = "particles.star"
     classes_file: str = "class_averages.star"
     python_exe: str = "python"
     autoselect_min_score: float = 0
     min_particles: int = 500
     class3d_batch_size: int = 50000
@@ -135,14 +137,17 @@
         # Update the relion options
         autoselect_params.relion_options.class2d_fraction_of_classes_to_remove = (
             autoselect_params.class2d_fraction_of_classes_to_remove
         )
         autoselect_params.relion_options.autoselect_min_score = (
             autoselect_params.autoselect_min_score
         )
+        autoselect_params.relion_options.particle_diameter = (
+            autoselect_params.particle_diameter
+        )
 
         self.log.info(f"Inputs: {autoselect_params.input_file}")
 
         class2d_job_dir = Path(
             re.search(".+/job[0-9]{3}/", autoselect_params.input_file)[0]
         )
         project_dir = class2d_job_dir.parent.parent
@@ -480,14 +485,109 @@
 
         # End here if the command failed
         if not split_node_creator_params["success"]:
             self.log.error("Star file splitting failed")
             rw.transport.nack(header)
             return
 
+        # Request selected particles image from images service
+        self.log.info("Sending to images service")
+        files_selected_from = []
+        (combine_star_dir / "Movies").mkdir(exist_ok=True)
+        with open(
+            select_dir / autoselect_params.particles_file, "r"
+        ) as selected_particles:
+            while True:
+                line = selected_particles.readline()
+                if not line:
+                    break
+                if not line.strip():
+                    continue
+                if line.strip()[0].isnumeric():
+                    # Second entry is particle files in the form 001@Extract/file.star
+                    particle_x = line.split()[0]
+                    particle_y = line.split()[1]
+                    extracted_file = line.split()[2].split("@")[1]
+                    motioncorr_file = line.split()[3]
+                    if [extracted_file, motioncorr_file] not in files_selected_from:
+                        # Make a list of all files
+                        files_selected_from.append([extracted_file, motioncorr_file])
+                    # Append any newly selected particles to a file
+                    with open(
+                        combine_star_dir / f"Movies/{Path(extracted_file).stem}.star",
+                        "a",
+                    ) as selected_file:
+                        selected_file.write(f"{particle_x} {particle_y}\n")
+
+        original_pixel_size = None
+        for extracted_file, motioncorr_file in files_selected_from:
+            # Get the selected picks for each file
+            extract_job_number = int(extracted_file.split("job")[1][:3])
+            try:
+                with open(
+                    combine_star_dir / f"Movies/{Path(extracted_file).stem}.star", "r"
+                ) as selected_file:
+                    selected_coords = [line.split() for line in selected_file]
+            except FileNotFoundError:
+                selected_coords = []
+
+            if not Path(motioncorr_file).is_relative_to(project_dir):
+                motioncorr_file = project_dir / motioncorr_file
+
+            if not original_pixel_size:
+                with mrcfile.open(motioncorr_file) as mrc:
+                    original_pixel_size = float(mrc.header.cella.z)
+
+            # Get the name of the  picking image file
+            cryolo_output_path = (
+                Path(
+                    re.sub(
+                        "MotionCorr/job002/.+",
+                        f"AutoPick/job{extract_job_number - 1:03}/STAR/",
+                        str(motioncorr_file),
+                    )
+                )
+                / Path(motioncorr_file).with_suffix(".star").name
+            )
+
+            # Get all the picks
+            try:
+                with open(cryolo_output_path, "r") as coords_file:
+                    coords = [line.split() for line in coords_file][6:]
+            except FileNotFoundError:
+                coords = []
+
+            # Generate image of selected and non-selected picks
+            if isinstance(rw, MockRW):
+                rw.transport.send(
+                    destination="images",
+                    message={
+                        "image_command": "picked_particles",
+                        "file": str(motioncorr_file),
+                        "coordinates": coords,
+                        "selected_coordinates": selected_coords,
+                        "pixel_size": original_pixel_size,
+                        "diameter": autoselect_params.particle_diameter,
+                        "outfile": str(Path(cryolo_output_path).with_suffix(".jpeg")),
+                    },
+                )
+            else:
+                rw.send_to(
+                    "images",
+                    {
+                        "image_command": "picked_particles",
+                        "file": str(motioncorr_file),
+                        "coordinates": coords,
+                        "selected_coordinates": selected_coords,
+                        "pixel_size": original_pixel_size,
+                        "diameter": autoselect_params.particle_diameter,
+                        "outfile": str(Path(cryolo_output_path).with_suffix(".jpeg")),
+                    },
+                )
+
         # Create 3D classification jobs
         if send_to_3d_classification:
             # Only send to 3D if a new multiple of the batch threshold is crossed
             # and the count has not passed the maximum
             self.log.info("Sending to Murfey for Class3D")
 
             # Copy the particle batch file
```

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/select_particles.py` & `cryoemservices-0.2.4/src/cryoemservices/services/select_particles.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/tomo_align.py` & `cryoemservices-0.2.4/src/cryoemservices/services/tomo_align.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/services/tomo_align_slurm.py` & `cryoemservices-0.2.4/src/cryoemservices/services/tomo_align_slurm.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/util/dispatcher_tools.py` & `cryoemservices-0.2.4/src/cryoemservices/util/dispatcher_tools.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/util/slurm_submission.py` & `cryoemservices-0.2.4/src/cryoemservices/util/slurm_submission.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/util/spa_output_files.py` & `cryoemservices-0.2.4/src/cryoemservices/util/spa_output_files.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/util/spa_relion_service_options.py` & `cryoemservices-0.2.4/src/cryoemservices/util/spa_relion_service_options.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/wrappers/class2d_wrapper.py` & `cryoemservices-0.2.4/src/cryoemservices/wrappers/class2d_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/wrappers/class3d_wrapper.py` & `cryoemservices-0.2.4/src/cryoemservices/wrappers/class3d_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices/wrappers/refine3d_wrapper.py` & `cryoemservices-0.2.4/src/cryoemservices/wrappers/refine3d_wrapper.py`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices.egg-info/PKG-INFO` & `cryoemservices-0.2.4/src/cryoemservices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryoemservices
-Version: 0.2.2
+Version: 0.2.4
 Summary: Services for CryoEM processing
 Author: Diamond Light Source - Data Analysis et al.
 Author-email: dataanalysis@diamond.ac.uk
 License: BSD 3-Clause
 Project-URL: GitHub, https://github.com/DiamondLightSource/cryoem-services
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/cryoem-services/issues
 Keywords: cryoem-services
```

### Comparing `cryoemservices-0.2.2/src/cryoemservices.egg-info/SOURCES.txt` & `cryoemservices-0.2.4/src/cryoemservices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryoemservices-0.2.2/src/cryoemservices.egg-info/entry_points.txt` & `cryoemservices-0.2.4/src/cryoemservices.egg-info/entry_points.txt`

 * *Files identical despite different names*

