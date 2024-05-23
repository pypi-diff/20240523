# Comparing `tmp/oresat_c3-0.3.0.tar.gz` & `tmp/oresat_c3-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_c3-0.3.0.tar", last modified: Sun Apr 28 22:21:11 2024, max compression
+gzip compressed data, was "oresat_c3-0.4.0.tar", last modified: Thu May 23 00:28:11 2024, max compression
```

## Comparing `oresat_c3-0.3.0.tar` & `oresat_c3-0.4.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.473003 oresat_c3-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.461003 oresat_c3-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.461003 oresat_c3-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-28 22:21:11.473003 oresat_c3-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.465003 oresat_c3-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/edl.rst
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/opd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/state.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.465003 oresat_c3-0.3.0/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/static/comms_ipc.drawio
--rw-r--r--   0 runner    (1001) docker     (127)    33084 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/static/comms_ipc.jpg
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    98849 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/static/opd.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.465003 oresat_c3-0.3.0/oresat_c3/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.465003 oresat_c3-0.3.0/oresat_c3/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/drivers/fm24cl64b.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/drivers/max7310.py
--rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/drivers/si41xx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.465003 oresat_c3-0.3.0/oresat_c3/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/protocols/ax25.py
--rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/protocols/edl_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/protocols/edl_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/oresat_c3/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/services/beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)    29640 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/services/edl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/services/node_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/services/radios.py
--rw-r--r--   0 runner    (1001) docker     (127)    11807 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/services/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/oresat_c3/subsystems/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/subsystems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/subsystems/antennas.py
--rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/subsystems/opd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/subsystems/rtc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/oresat_c3/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/templates/beacon.html
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/templates/keys.html
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/templates/node_manager.html
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/templates/state.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.473003 oresat_c3-0.3.0/oresat_c3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)    14200 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/scripts/edl_cmd_shell.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13336 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/scripts/edl_file_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4214 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/scripts/edl_ping_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 22:21:11.473003 oresat_c3-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/tests/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/drivers/test_fm23cl64b.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/drivers/test_max7310.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/tests/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/protocols/test_ax25.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/protocols/test_edl_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/protocols/test_edl_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/services/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/tests/subsystems/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/subsystems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/subsystems/test_opd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.918331 oresat_c3-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.906331 oresat_c3-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.906331 oresat_c3-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-23 00:28:11.918331 oresat_c3-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.910331 oresat_c3-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/edl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/opd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/state.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.910331 oresat_c3-0.4.0/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/static/comms_ipc.drawio
+-rw-r--r--   0 runner    (1001) docker     (127)    33084 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/static/comms_ipc.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    98849 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/docs/static/opd.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.910331 oresat_c3-0.4.0/oresat_c3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.910331 oresat_c3-0.4.0/oresat_c3/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/drivers/fm24cl64b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/drivers/max7310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/drivers/si41xx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.910331 oresat_c3-0.4.0/oresat_c3/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/protocols/ax25.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/protocols/edl_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/protocols/edl_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/oresat_c3/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/services/beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29640 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/services/edl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14657 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/services/node_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/services/radios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/services/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/oresat_c3/subsystems/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/subsystems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/subsystems/antennas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15253 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/subsystems/opd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/subsystems/rtc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/oresat_c3/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/templates/beacon.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/templates/keys.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/templates/node_manager.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/oresat_c3/templates/state.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.918331 oresat_c3-0.4.0/oresat_c3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 00:28:11.000000 oresat_c3-0.4.0/oresat_c3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14219 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/scripts/edl_cmd_shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13336 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/scripts/edl_file_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4214 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/scripts/edl_ping_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 00:28:11.918331 oresat_c3-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/tests/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/drivers/test_fm23cl64b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/drivers/test_max7310.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/protocols/test_ax25.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/protocols/test_edl_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/protocols/test_edl_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.914331 oresat_c3-0.4.0/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/services/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:11.918331 oresat_c3-0.4.0/tests/subsystems/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/subsystems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-23 00:28:02.000000 oresat_c3-0.4.0/tests/subsystems/test_opd.py
```

### Comparing `oresat_c3-0.3.0/.github/workflows/pypi.yaml` & `oresat_c3-0.4.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/.github/workflows/tests.yaml` & `oresat_c3-0.4.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/.gitignore` & `oresat_c3-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/LICENSE` & `oresat_c3-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/PKG-INFO` & `oresat_c3-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-c3
-Version: 0.3.0
+Version: 0.4.0
 Summary: OreSat C3 OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oresat_c3-0.3.0/README.md` & `oresat_c3-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/docs/Makefile` & `oresat_c3-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/docs/conf.py` & `oresat_c3-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/docs/edl.rst` & `oresat_c3-0.4.0/docs/edl.rst`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/docs/make.bat` & `oresat_c3-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/docs/opd.rst` & `oresat_c3-0.4.0/docs/opd.rst`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/docs/state.rst` & `oresat_c3-0.4.0/docs/state.rst`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/docs/static/comms_ipc.drawio` & `oresat_c3-0.4.0/docs/static/comms_ipc.drawio`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/docs/static/comms_ipc.jpg` & `oresat_c3-0.4.0/docs/static/comms_ipc.jpg`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/docs/static/opd.jpg` & `oresat_c3-0.4.0/docs/static/opd.jpg`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/__init__.py` & `oresat_c3-0.4.0/oresat_c3/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/__main__.py` & `oresat_c3-0.4.0/oresat_c3/__main__.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/drivers/fm24cl64b.py` & `oresat_c3-0.4.0/oresat_c3/drivers/fm24cl64b.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/drivers/max7310.py` & `oresat_c3-0.4.0/oresat_c3/drivers/max7310.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/drivers/si41xx.py` & `oresat_c3-0.4.0/oresat_c3/drivers/si41xx.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/protocols/ax25.py` & `oresat_c3-0.4.0/oresat_c3/protocols/ax25.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/protocols/edl_command.py` & `oresat_c3-0.4.0/oresat_c3/protocols/edl_command.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/protocols/edl_packet.py` & `oresat_c3-0.4.0/oresat_c3/protocols/edl_packet.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/services/beacon.py` & `oresat_c3-0.4.0/oresat_c3/services/beacon.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/services/edl.py` & `oresat_c3-0.4.0/oresat_c3/services/edl.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/services/node_manager.py` & `oresat_c3-0.4.0/oresat_c3/services/node_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,35 +19,39 @@
 class NodeState(IntEnum):
     """
     OreSat Node States
 
     .. mermaid
         stateDiagram-v2
             [*] --> OFF
-            OFF--> BOOT : Enable
+            OFF --> BOOT : Enable
+            OFF --> BOOTLOADER : Bootloader (STM32 only)
+            BOOTLOADER --> OFF : Disable
             BOOT --> OFF : Disable
             BOOT --> ON : Heartbeats and no OPD fault
             BOOT --> ERROR : Timeout with no heartbeats or OPD fault
+            ERROR --> DEAD : Multiple resets failed in a row
+            ERROR --> ON : Reset
+            ERROR --> OFF : Disable
             ON --> OFF : Disable
             ON --> ERROR : Timeout with no heartbeats or OPD fault
-            ERROR --> OFF : Disable
-            ERROR --> ON : Reset
-            ERROR --> DEAD : Multiple resets failed in a row
     """
 
     OFF = 0
     """Node is powered off."""
     BOOT = 1
     """Node is booting."""
     ON = 2
     """Node is powered on."""
     ERROR = 3
     """Node is not sending heartbeats or has a OPD fault."""
     NOT_FOUND = 4
     """Node is not found on the OPD."""
+    BOOTLOADER = 5
+    """For STM32s on the OPD only: Bootloader mode (used to reflash the app)."""
     DEAD = 0xFF
     """Node has failed to clear errors after multiple resets."""
 
 
 @dataclass_json
 @dataclass
 class Node(Card):
@@ -128,22 +132,28 @@
         self._nodes_not_found_obj = nodes_mgr_rec["nodes_not_found"]
         self._nodes_with_errors_obj = nodes_mgr_rec["nodes_with_errors"]
         self._nodes_dead_obj = nodes_mgr_rec["nodes_dead"]
         nodes_mgr_rec["total_nodes"].value = len(list(self._data))
 
         self.node.add_sdo_callbacks("node_manager", "status_json", self._get_status_json, None)
         self.node.add_sdo_callbacks("opd", "status", self._get_opd_status, self._set_opd_status)
+        self.node.add_sdo_callbacks(
+            "opd",
+            "uart_node_select",
+            self._get_uart_node_select,
+            self._set_uart_node_select,
+        )
         for name in self._data:
             if self._data[name].node_id == 0:
                 continue  # not a CANopen node
             self.node.add_sdo_callbacks(
                 "node_status",
                 str(name),
                 lambda n=name: self.node_status(n),
-                lambda v, n=name: self.enable(n) if v == NodeState.ON else self.disable(n),
+                lambda v, n=name: self._set_node_status(n, v),
             )
 
     def _check_co_nodes_state(self, name: str) -> NodeState:
         """Get a CANopen node's state."""
 
         next_state = self._data[name].status
         if next_state == NodeState.DEAD:
@@ -202,15 +212,17 @@
             elif status == OpdNodeState.NOT_FOUND:
                 next_state = NodeState.NOT_FOUND
             elif (
                 prev_state == NodeState.ERROR and self._data[name].opd_resets >= self._MAX_CO_RESETS
             ):
                 next_state = NodeState.DEAD
             elif status == OpdNodeState.ENABLED:
-                if self._data[name].node_id != 0:  # aka CANopen nodes
+                if self._data[name].processor == "stm32" and self.opd[name].in_bootloader_mode:
+                    next_state = NodeState.BOOTLOADER
+                elif self._data[name].node_id != 0:  # aka CANopen nodes
                     next_state = self._check_co_nodes_state(name)
                 else:
                     next_state = NodeState.ON
             elif status == OpdNodeState.DISABLED:
                 next_state = NodeState.OFF
 
         return next_state
@@ -266,74 +278,118 @@
 
             if info.opd_always_on and info.status == NodeState.OFF:
                 self.enable(name)
 
             if info.status == NodeState.ERROR:
                 logger.error(f"resetting node {name}, try {info.opd_resets + 1}")
                 self.opd[name].reset(1)
+                self._data[name].last_enable = monotonic()
                 info.opd_resets += 1
             else:
                 info.opd_resets = 0
 
-    def enable(self, name: Union[str, int]):
-        """Enable a OreSat node."""
+    def enable(self, name: Union[str, int], bootloader_mode: bool = False):
+        """
+        Enable a OreSat node.
+
+        Parameters
+        ----------
+        name: str | int
+            Name or node id of the card to enable
+        bootloader_mode: bool
+            Go into bootloader mode instead. Only for STM32 nodes on the OPD, flag will be ignored
+            otherwise.
+        """
 
         if isinstance(name, int):
             name = self.opd_addr_to_name[name]
 
         node = self._data[name]
         child_node = self._data[node.child] if node.child else None
         if node.opd_address == 0:
             logger.warning(f"cannot enable node {name} as it is not on the OPD")
             return  # not on OPD, nothing to do
 
+        if node.status != NodeState.OFF:
+            logger.debug(f"cannot enable node {name} unless it is disabled")
+            return
+
         if node.status == NodeState.DEAD:
             logger.error(f"cannot enable node {name} as it is DEAD")
             return
 
-        self.opd[name].enable()
-        if child_node:
-            self.opd[node.child].enable()
+        if node.processor == "stm32":
+            self.opd[name].enable(bootloader_mode)
+            if child_node:
+                self.opd[node.child].enable(bootloader_mode)
+        else:
+            self.opd[name].enable()
+            if child_node:
+                self.opd[node.child].enable()
         node.last_enable = monotonic()
 
     def disable(self, name: Union[str, int]):
-        """Disable a OreSat node."""
+        """
+        Disable a OreSat node.
+
+        Parameters
+        ----------
+        name: str | int
+            Name or node id of the card to enable
+        """
 
         if isinstance(name, int):
             name = self.opd_addr_to_name[name]
 
         node = self._data[name]
         child_node = self._data[node.child] if node.child else None
         if node.opd_address == 0:
             logger.warning(f"cannot disable node {name} as it is not on the OPD")
             return  # not on OPD, nothing to do
 
+        if node.status in [NodeState.OFF, NodeState.DEAD]:
+            logger.debug(f"cannot disable node {name} as it is already disabled or dead")
+            return
+
         if child_node:
             self.opd[node.child].disable()
-
         self.opd[name].disable()
 
     def node_status(self, name: Union[str, int]) -> NodeState:
         """Get the status of a OreSat node."""
 
         if isinstance(name, int):
             name = self.opd_addr_to_name[name]
 
         return self._data[name].status
 
+    def _set_node_status(self, name: Union[str, int], state: int):
+        """Set the status of a OreSat node."""
+
+        if isinstance(name, int):
+            name = self.opd_addr_to_name[name]
+
+        if state == NodeState.ON:
+            self.enable(name)
+        elif state == NodeState.OFF:
+            self.disable(name)
+        elif state == NodeState.BOOTLOADER:
+            self.enable(name, True)
+
     def _get_status_json(self) -> str:
         """SDO read callback to get the status of all data as a JSON."""
 
         data = []
         for name, info in self._data.items():
             data.append(
                 {
                     "name": name,
                     "nice_name": info.nice_name,
                     "node_id": info.node_id,
+                    "processor": info.processor,
                     "opd_addr": info.opd_address,
                     "status": info.status.name,
                 }
             )
         return json.dumps(data)
 
     def _get_opd_status(self) -> int:
@@ -343,7 +399,27 @@
         if value == 0:
             self.opd.disable()
         elif value == 1:
             if self.opd.status == OpdState.DISABLED:
                 for node in self._data.values():
                     node.last_enable = monotonic()
             self.opd.enable()
+
+    def _get_uart_node_select(self) -> int:
+        """SDO write callback to select a node to connect to via UART."""
+
+        return 0 if self.opd.uart_node is None else self._data[self.opd.uart_node].opd_address
+
+    def _set_uart_node_select(self, value: int):
+        """
+        SDO write callback to select a node to connect to via UART.
+
+        Parameters
+        ----------
+        value: int
+            The opd address of the node to connect to UART or 0 for no node.
+        """
+
+        if value == 0:
+            self.opd.uart_node = None
+        elif value in self.opd_addr_to_name:
+            self.opd.uart_node = self.opd_addr_to_name[value]
```

### Comparing `oresat_c3-0.3.0/oresat_c3/services/radios.py` & `oresat_c3-0.4.0/oresat_c3/services/radios.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/services/state.py` & `oresat_c3-0.4.0/oresat_c3/services/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,14 +288,16 @@
 
             if obj.data_type == canopen.objectdictionary.OCTET_STRING:
                 size = len(obj.default)
                 obj.value = self._fram.read(offset, size)
             else:
                 size = len(obj.encode_raw(obj.default))
                 raw = self._fram.read(offset, size)
+                if obj.name == "status":  # case of empty FRAM
+                    raw = raw or C3State.PRE_DEPLOY.value.to_bytes(1, "little")
                 obj.value = obj.decode_raw(raw)
             offset += size
 
     def clear_state(self):
         """Clear the rtc time and state from F-RAM; keys will be stored again after clear."""
 
         self._fram.clear()
```

### Comparing `oresat_c3-0.3.0/oresat_c3/subsystems/antennas.py` & `oresat_c3-0.4.0/oresat_c3/subsystems/antennas.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/subsystems/opd.py` & `oresat_c3-0.4.0/oresat_c3/subsystems/opd.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Everything todo with the OPD (OreSat Power Domain) functionality.
 
 Every card, other than the solar cards, has a MAX7310 that can be used to turn the card or off.
 """
 
 from enum import IntEnum
 from time import sleep
+from typing import Union
 
 from olaf import Adc, Gpio, logger
 
 from ..drivers.max7310 import Max7310, Max7310Error
 
 
 class OpdError(Exception):
@@ -274,39 +275,62 @@
                 self._max7310.output_clear(self._BOOT_PIN)
         except Max7310Error:
             self._status = OpdNodeState.FAULT
             return self._status
 
         return super().enable()
 
+    def disable(self):
+        """
+        Disable the OPD node.
+
+        Returns
+        -------
+        OpdNodeState
+            The node state after disabling the node.
+        """
+        try:
+            self._max7310.output_clear(self._BOOT_PIN)
+        except Max7310Error:
+            pass
+        return super().disable()
+
     def configure(self):
         """Configure the MAX7310 for the OPD node."""
 
         inputs = 1 << self._I2C_SCL_PIN | 1 << self._I2C_SDA_PIN | 1 << self._NOT_FAULT_PIN
         self._max7310.configure(0, 0, inputs, self._TIMEOUT_CONFIG)
         if self._mock:
             self._max7310._mock_input_set(self._NOT_FAULT_PIN)  # pylint: disable=W0212
         self._status = OpdNodeState.DISABLED
 
     def enable_uart(self):
         """Connect the node the C3's UART"""
 
         self._max7310.output_set(self._UART_PIN)
+        logger.info(f"OPD node {self.name} (0x{self.addr:02X}) was connected to UART")
 
     def disable_uart(self):
         """Disconnect the node from the C3's UART"""
 
         self._max7310.output_clear(self._UART_PIN)
+        logger.info(f"OPD node {self.name} (0x{self.addr:02X}) was disconnected from UART")
 
     @property
     def is_uart_enabled(self) -> bool:
         """bool: Check if the UART pin is connected"""
 
         return self._max7310.output_status(self._UART_PIN)
 
+    @property
+    def in_bootloader_mode(self) -> bool:
+        """bool: Check if the card is in bootloader mode."""
+
+        return self._max7310.output_status(self._BOOT_PIN)
+
 
 class OpdOctavoNode(OpdNode):
     """A Octavo A8-based OPD Node"""
 
     _SYS_BOOT2 = 0
     _UART_PIN = 7  # connect to C3 UART
 
@@ -316,19 +340,21 @@
         self._max7310.output_set(self._SYS_BOOT2)
         return super().enable()
 
     def enable_uart(self):
         """Connect the node the C3's UART"""
 
         self._max7310.output_set(self._UART_PIN)
+        logger.info(f"OPD node {self.name} (0x{self.addr:02X}) was connected to UART")
 
     def disable_uart(self):
         """Disconnect the node the C3's UART"""
 
         self._max7310.output_clear(self._UART_PIN)
+        logger.info(f"OPD node {self.name} (0x{self.addr:02X}) was disconnected from UART")
 
     @property
     def is_uart_enabled(self) -> bool:
         """bool: Check if the UART pin is connected"""
 
         return self._max7310.output_status(self._UART_PIN)
 
@@ -347,15 +373,15 @@
 
 
 class Opd:
     """OreSat Power Domain."""
 
     # values for getting opd current value from ADC pin
     _R_SET = 23_700  # ohms
-    _MAX982L_CUR_RATIO = 965  # curret ratio
+    _MAX982L_CUR_RATIO = 965  # current ratio
 
     def __init__(
         self,
         not_enable_pin: str,
         not_fault_pin: str,
         current_pin: int,
         mock: bool = False,
@@ -377,15 +403,15 @@
         self._not_fault_pin = Gpio(not_fault_pin, mock)
         self._not_fault_pin._mock_value = 1  # fix default for mocking
         self._adc = Adc(current_pin, mock)
         self._not_enable_pin.high()  # make sure OPD disable initially
 
         self._nodes = {}  # type: ignore
         self._status = OpdState.DISABLED
-        self.stop_loop = True
+        self._uart_node: Union[str, None] = None
         self._resets = 0
 
     def __getitem__(self, name: str) -> OpdNode:
         return self._nodes[name]
 
     def __setitem__(self, name: str, node: OpdNode):
         self._nodes[name] = node
@@ -412,14 +438,15 @@
 
         logger.info("stopping OPD subsystem")
 
         for node in self:
             if node.status != OpdNodeState.NOT_FOUND:
                 node.disable()
 
+        self._uart_disconnect()
         self._not_enable_pin.high()
         self._status = OpdState.DISABLED
         self._resets = 0
 
     def reset(self, tries: int = 3, disable_delay: float = 10):
         """
         Restart the OPD subsystem with a delay between stop and start.
@@ -485,7 +512,31 @@
         return int(self._adc.value * self._MAX982L_CUR_RATIO / self._R_SET * 1000)
 
     @property
     def status(self) -> OpdState:
         """OpdState: OPD subsystem status."""
 
         return self._status
+
+    def _uart_disconnect(self):
+        if self._uart_node is not None:
+            self._nodes[self._uart_node].disable_uart()
+            self._uart_node = None
+
+    @property
+    def uart_node(self) -> Union[str, None]:
+        """str: The selected UART node name or an empty string for no node."""
+        if (
+            self._uart_node is not None
+            and self._nodes[self._uart_node].status == OpdNodeState.NOT_FOUND
+        ):
+            self._uart_disconnect()
+        return self._uart_node
+
+    @uart_node.setter
+    def uart_node(self, name: Union[str, None]):
+
+        self._uart_disconnect()
+        if name is None or self._nodes[name].status == OpdNodeState.NOT_FOUND:
+            return
+        self._nodes[name].enable_uart()
+        self._uart_node = name
```

### Comparing `oresat_c3-0.3.0/oresat_c3/subsystems/rtc.py` & `oresat_c3-0.4.0/oresat_c3/subsystems/rtc.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/templates/keys.html` & `oresat_c3-0.4.0/oresat_c3/templates/keys.html`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3/templates/state.html` & `oresat_c3-0.4.0/oresat_c3/templates/state.html`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/oresat_c3.egg-info/PKG-INFO` & `oresat_c3-0.4.0/oresat_c3.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-c3
-Version: 0.3.0
+Version: 0.4.0
 Summary: OreSat C3 OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oresat_c3-0.3.0/oresat_c3.egg-info/SOURCES.txt` & `oresat_c3-0.4.0/oresat_c3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/pyproject.toml` & `oresat_c3-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/scripts/edl_cmd_shell.py` & `oresat_c3-0.4.0/scripts/edl_cmd_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
                 # parse respone
                 res_packet = EdlPacket.unpack(res_packet_raw, self._hmac_key)
             self._seq_num += 1
         except Exception as e:  # pylint: disable=W0718
             print(e)
             return tuple()
 
+        ret = None
         if res_packet and res_packet.payload.values:
             ret = res_packet.payload.values
             print(f"Response {code.name}: {ret}")
 
         return ret
 
     def help_tx_control(self):
```

### Comparing `oresat_c3-0.3.0/scripts/edl_file_upload.py` & `oresat_c3-0.4.0/scripts/edl_file_upload.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/scripts/edl_ping_loop.py` & `oresat_c3-0.4.0/scripts/edl_ping_loop.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/tests/drivers/test_fm23cl64b.py` & `oresat_c3-0.4.0/tests/drivers/test_fm23cl64b.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/tests/drivers/test_max7310.py` & `oresat_c3-0.4.0/tests/drivers/test_max7310.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/tests/protocols/test_ax25.py` & `oresat_c3-0.4.0/tests/protocols/test_ax25.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/tests/protocols/test_edl_command.py` & `oresat_c3-0.4.0/tests/protocols/test_edl_command.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/tests/protocols/test_edl_packet.py` & `oresat_c3-0.4.0/tests/protocols/test_edl_packet.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/tests/services/test_state.py` & `oresat_c3-0.4.0/tests/services/test_state.py`

 * *Files identical despite different names*

### Comparing `oresat_c3-0.3.0/tests/subsystems/test_opd.py` & `oresat_c3-0.4.0/tests/subsystems/test_opd.py`

 * *Files identical despite different names*

