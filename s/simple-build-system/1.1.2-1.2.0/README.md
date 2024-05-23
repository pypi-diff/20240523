# Comparing `tmp/simple_build_system-1.1.2.tar.gz` & `tmp/simple_build_system-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_build_system-1.1.2.tar", last modified: Mon May  6 09:51:28 2024, max compression
+gzip compressed data, was "simple_build_system-1.2.0.tar", last modified: Thu May 23 08:02:00 2024, max compression
```

## Comparing `simple_build_system-1.1.2.tar` & `simple_build_system-1.2.0.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.725201 simple_build_system-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14092 2024-05-06 09:51:28.721201 simple_build_system-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:51:28.725201 simple_build_system-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.701201 simple_build_system-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.709200 simple_build_system-1.1.2/src/_simple_build_system/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/_determine_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/_export_jsoncmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/_sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/_sphinxutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20990 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/build_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/cfgbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/cfglocate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/col.py
--rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/cpudetect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.709200 simple_build_system-1.1.2/src/_simple_build_system/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cfgtemplate.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.713200 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/Detect.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/ExtDep_Python.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/ExtDep_pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/ExtractFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/Utils.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/WriteResults.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/extract_flags_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.713200 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_ASE.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_DL.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Fortran.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Garfield.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Geant4.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Gemmi.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_HDF5.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Mantidpython.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_NCrystal.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Numpy.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_OSG.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Pandas.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Pymatgen.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_ROOT.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Scipy.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Spglib.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Threads.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_ZLib.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_matplotlib.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_mpmath.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.713200 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.713200 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.713200 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/app_cmakebuildtype/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/app_cmakebuildtype/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libinc/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libinc/FPE.hh
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libinc/File.hh
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libinc/FindData.hh
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libinc/Python.hh
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libinc/String.hh
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libinc/Types.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/FPE.cc
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/File.cc
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/FindData.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/String.cc
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/static_asserts.cc
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/pkg.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/pycpp_FPE/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/pycpp_FPE/mod.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/pycpp_misc/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/pycpp_misc/mod.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/python/CpuDetect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/python/FindData.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/python/FindData3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/python/System.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/python/find_libpython.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/scripts/extdeps
--rwxr-xr-x   0 runner    (1001) docker     (127)      600 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/scripts/finddata
--rwxr-xr-x   0 runner    (1001) docker     (127)     2825 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/scripts/queryenv
--rwxr-xr-x   0 runner    (1001) docker     (127)     6199 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/scripts/reflogupdate
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/simplebuild.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/app_test/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/app_test/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/libsrc/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/libsrc/sometest.cc
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/pkg.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_build_is_debug/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_build_is_debug/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_forcefpe/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_forcefpe/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.717201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testfile/
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testfile/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.721201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testformat/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testformat/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.721201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testpycpp/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testpycpp/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.721201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testsdk/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testsdk/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.721201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_teststring/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_teststring/main.cc
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/pkg.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.721201 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      691 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testfpe
--rwxr-xr-x   0 runner    (1001) docker     (127)     1279 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testlibsymbols
--rwxr-xr-x   0 runner    (1001) docker     (127)     1180 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testnodostxt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1824 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testpylibsymbols
--rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testpyquery
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/simplebuild.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.721201 simple_build_system-1.1.2/src/_simple_build_system/data/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/resources/shellrc_snippet.sh
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/data/resources/shellrc_snippet_deactivate.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/dirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/dotgen.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/envcfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/envsetup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/extractenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/find.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/findpkgdirs.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/formatlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    18720 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/grep.py
--rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/incinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/includes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/init_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/instsl.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/instsl2.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/langs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/loadpkgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/makefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/mtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/parse_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/pkgfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/pkgutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/replace.py
--rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/singlecfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/target_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/target_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/testlauncher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/testxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/tfact_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/tfact_headerdeps.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/tfact_libavail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/tfact_prepinc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/tfact_pyinit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/tfact_reflogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/tfact_symlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-06 09:51:22.000000 simple_build_system-1.1.2/src/_simple_build_system/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:51:28.721201 simple_build_system-1.1.2/src/simple_build_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14092 2024-05-06 09:51:28.000000 simple_build_system-1.1.2/src/simple_build_system.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-06 09:51:28.000000 simple_build_system-1.1.2/src/simple_build_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:51:28.000000 simple_build_system-1.1.2/src/simple_build_system.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-06 09:51:28.000000 simple_build_system-1.1.2/src/simple_build_system.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-06 09:51:28.000000 simple_build_system-1.1.2/src/simple_build_system.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 09:51:28.000000 simple_build_system-1.1.2/src/simple_build_system.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.767870 simple_build_system-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14092 2024-05-23 08:02:00.767870 simple_build_system-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:02:00.767870 simple_build_system-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.743870 simple_build_system-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.755870 simple_build_system-1.2.0/src/_simple_build_system/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/_determine_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/_export_jsoncmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/_sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/_sphinxutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20990 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/build_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/cfgbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/cfglocate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/col.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/cpudetect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.755870 simple_build_system-1.2.0/src/_simple_build_system/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cfgtemplate.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.755870 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/Detect.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/ExtDep_Python.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/ExtDep_pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/ExtractFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/Utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/WriteResults.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/extract_flags_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.759870 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_ASE.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_DL.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Fortran.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Garfield.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Geant4.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Gemmi.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_HDF5.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Mantidpython.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_NCrystal.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Numpy.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_OSG.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Pandas.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Pymatgen.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_ROOT.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Scipy.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Spglib.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Threads.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_ZLib.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_matplotlib.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_mpmath.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.759870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.759870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.759870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/app_cmakebuildtype/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/app_cmakebuildtype/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.759870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libinc/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libinc/FPE.hh
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libinc/File.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libinc/FindData.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libinc/Python.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libinc/String.hh
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libinc/Types.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.759870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libsrc/
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libsrc/FPE.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libsrc/File.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libsrc/FindData.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libsrc/String.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libsrc/static_asserts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/pkg.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.759870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/pycpp_FPE/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/pycpp_FPE/mod.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.759870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/pycpp_misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/pycpp_misc/mod.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.759870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/python/CpuDetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/python/FindData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/python/FindData3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/python/System.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/python/find_libpython.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/scripts/extdeps
+-rwxr-xr-x   0 runner    (1001) docker     (127)      600 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/scripts/finddata
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2825 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/scripts/queryenv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6199 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/scripts/reflogupdate
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/simplebuild.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/app_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/app_test/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/libsrc/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/libsrc/sometest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreLinkTests/pkg.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_build_is_debug/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_build_is_debug/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_forcefpe/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_forcefpe/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testfile/
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testfile/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testformat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testformat/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testpycpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testpycpp/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testsdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testsdk/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_teststring/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_teststring/main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/pkg.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      691 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testfpe
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1279 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testlibsymbols
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1180 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testnodostxt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1824 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testpylibsymbols
+-rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testpyquery
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/simplebuild.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.763870 simple_build_system-1.2.0/src/_simple_build_system/data/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/resources/shellrc_snippet.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/data/resources/shellrc_snippet_deactivate.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/dotgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/envcfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/envsetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/extractenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/find.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/findpkgdirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/formatlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18720 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/grep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/incinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/includes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/init_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/instsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/instsl2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/langs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16357 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/loadpkgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/mtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/parse_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/pkgfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/pkgutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17097 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/singlecfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/target_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/target_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/testlauncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/testxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/tfact_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/tfact_headerdeps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/tfact_libavail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/tfact_prepinc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/tfact_pyinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/tfact_reflogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/tfact_symlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-23 08:01:54.000000 simple_build_system-1.2.0/src/_simple_build_system/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:02:00.767870 simple_build_system-1.2.0/src/simple_build_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14092 2024-05-23 08:02:00.000000 simple_build_system-1.2.0/src/simple_build_system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-23 08:02:00.000000 simple_build_system-1.2.0/src/simple_build_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:02:00.000000 simple_build_system-1.2.0/src/simple_build_system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-23 08:02:00.000000 simple_build_system-1.2.0/src/simple_build_system.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 08:02:00.000000 simple_build_system-1.2.0/src/simple_build_system.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 08:02:00.000000 simple_build_system-1.2.0/src/simple_build_system.egg-info/top_level.txt
```

### Comparing `simple_build_system-1.1.2/LICENSE` & `simple_build_system-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/MANIFEST.in` & `simple_build_system-1.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/PKG-INFO` & `simple_build_system-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-build-system
-Version: 1.1.2
+Version: 1.2.0
 Summary: A very simple to use build system for projects with primarily C++/Python code, intended for usage by scientific developers without a strong SW-engineering background.
 Author-email: Thomas Kittelmann <thomas.kittelmann@ess.eu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `simple_build_system-1.1.2/pyproject.toml` & `simple_build_system-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/_cli.py` & `simple_build_system-1.2.0/src/_simple_build_system/_cli.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/_export_jsoncmds.py` & `simple_build_system-1.2.0/src/_simple_build_system/_export_jsoncmds.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/_sphinxext.py` & `simple_build_system-1.2.0/src/_simple_build_system/_sphinxext.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/_sphinxutils.py` & `simple_build_system-1.2.0/src/_simple_build_system/_sphinxutils.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/backend.py` & `simple_build_system-1.2.0/src/_simple_build_system/backend.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/build_summary.py` & `simple_build_system-1.2.0/src/_simple_build_system/build_summary.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/cfgbuilder.py` & `simple_build_system-1.2.0/src/_simple_build_system/cfgbuilder.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/cfglocate.py` & `simple_build_system-1.2.0/src/_simple_build_system/cfglocate.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/col.py` & `simple_build_system-1.2.0/src/_simple_build_system/col.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/conf.py` & `simple_build_system-1.2.0/src/_simple_build_system/conf.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/cpudetect.py` & `simple_build_system-1.2.0/src/_simple_build_system/cpudetect.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cfgtemplate.txt` & `simple_build_system-1.2.0/src/_simple_build_system/data/cfgtemplate.txt`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,24 @@
 [build]
   # By default, the cache directory used for build output will be
   # './simplebuild_cache'. If for instance you would like everything to go into
   # /tmp/myname/sbcache you could use:
   #
   #   cachedir = '/scr/myname/mysbcache'
   #
-  # If you wish to enable debug-symbols in your build, you can use:
+  # If you want to add many more sanity checks to your code (to help debugging
+  # code CORRECTNESS, at the cost of runtime performance), you can use:
   #
   #   mode = 'debug'
   #
+  # If you wish to just enable debug-symbols in your build, but not otherwise
+  # modify compilation options (to help debugging code SPEED), you can use:
+  #
+  #   mode = 'reldbg'
+  #
   # If you have many packages, and would like to only consider a subset of them,
   # you can set one or more package filters. Note that this concerns packages
   # *explicitly* enabled. Any package needed by those, will be *implicitly*
   # enabled. Thus, to build a package 'MyPkg', you only need to add 'MyPkg' to
   # the list, even if 'MyPkg' itself depends on many other packages.
   #
   #   pkg_filter = ['MyPkg','MyOtherPkg']
```

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/CMakeLists.txt` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/CMakeLists.txt`

 * *Files 27% similar despite different names*

```diff
@@ -14,22 +14,30 @@
   endfunction()
 endif()
 
 if( NOT CMAKE_BUILD_TYPE )
   message( FATAL_ERROR "CMAKE_BUILD_TYPE should always be set" )
 endif()
 
+if (NOT "${CMAKE_BUILD_TYPE}" MATCHES "^(Debug|Release)$")
+  message( FATAL_ERROR "For simplicity we require CMAKE_BUILD_TYPE to be exactly Debug or Release." )
+endif()
+
 message( STATUS "Using CMAKE_BUILD_TYPE=${CMAKE_BUILD_TYPE}" )
 
 project( DETECT LANGUAGES C CXX )
 
 set(output_filename "cmakecfg.txt")
 
 set(BUILD_SHARED_LIBS ON)
 
+if ( NOT DEFINED SBLD_RELDBG_MODE )
+  set(SBLD_RELDBG_MODE OFF)
+endif()
+
 #We compile with -pedantic and -Werror unless SBLD_RELAX is set:
 set(FLAG_PEDANTIC "")
 set(FLAG_WERROR "")
 if (NOT SBLD_RELAX)
   set(FLAG_PEDANTIC "-pedantic ")
   set(FLAG_WERROR "-Werror ")
 endif()
@@ -42,15 +50,14 @@
     set(FLAGS_PLATFORM_CXX " -Wno-reserved-id-macro -Wno-keyword-macro")
   endif()
 endif()
 
 set(SBLD_GLOBAL_COMPILE_FLAGS_CXX "${FLAG_PEDANTIC}-std=c++17 -Wextra ${FLAG_WERROR}-Wall -Woverloaded-virtual -Wno-non-virtual-dtor -Wno-long-long -Wwrite-strings -Wpointer-arith -Wno-variadic-macros -Wshadow${FLAGS_PLATFORM_CXX} ${SBLD_EXTRA_CFLAGS}")
 set(SBLD_GLOBAL_COMPILE_FLAGS_C "${FLAG_PEDANTIC}-std=c99 -Wextra${FLAGS_PLATFORM_C} ${FLAG_WERROR}-Wall ${SBLD_EXTRA_CFLAGS}")
 
-
 set(SBLD_GLOBAL_COMPILE_FLAGS_Fortran "")
 set(SBLD_GLOBAL_LINK_FLAGS "${SBLD_EXTRA_LDFLAGS}")
 set(SBLD_GLOBAL_LINK_FLAGS_PREPENDED "")
 if ("${CMAKE_CXX_COMPILER_ID}" STREQUAL "GNU")
   #Ubuntu has --as-needed by default and GCC, so we overrule this (prepended, before specific libs appear on the link cmd):
   set(SBLD_GLOBAL_LINK_FLAGS_PREPENDED "-Wl,--no-as-needed")
   #With GCC we can (since v4.6) make sure the compiler stops after after a few
@@ -62,14 +69,46 @@
 if ( APPLE AND DEFINED CMAKE_OSX_SYSROOT AND NOT "x${CMAKE_OSX_SYSROOT}" STREQUAL "x" )
   set(SBLD_GLOBAL_COMPILE_FLAGS_C "${SBLD_GLOBAL_COMPILE_FLAGS_C} -isysroot ${CMAKE_OSX_SYSROOT}")
   set(SBLD_GLOBAL_COMPILE_FLAGS_CXX "${SBLD_GLOBAL_COMPILE_FLAGS_CXX} -isysroot ${CMAKE_OSX_SYSROOT}")
   set(SBLD_GLOBAL_COMPILE_FLAGS_Fortran "${SBLD_GLOBAL_COMPILE_FLAGS_Fortran} -isysroot ${CMAKE_OSX_SYSROOT}")
   set(SBLD_GLOBAL_LINK_FLAGS "${SBLD_GLOBAL_LINK_FLAGS} -isysroot ${CMAKE_OSX_SYSROOT}")
 endif()
 
+if ( "x${CMAKE_CXX_COMPILER_ID}" STREQUAL "xIntelLLVM" )
+  set( SBLD_ISINTEL "ON" )
+else()
+  set( SBLD_ISINTEL "OFF" )
+endif()
+
+set( sbld_extra_ccxx_cflags "")
+if ( NOT "${CMAKE_BUILD_TYPE}" STREQUAL "Debug" )
+  #Aggressively target native platform + a few other optimisations (see also
+  #https://github.com/mctools/simplebuild/issues/73). For now we assume the
+  #compiler understands all of these:
+  set( sbld_extra_ccxx_cflags "${sbld_extra_ccxx_cflags} -O3 -DNDEBUG -fno-math-errno -march=native -mtune=native")
+  if ( NOT SBLD_ISINTEL )
+    #TODO: Do we need to add -flto to link step as well, or use gcc to drive the linking, before it works??
+    #NB: =auto due to https://stackoverflow.com/questions/72218980
+    set( sbld_extra_ccxx_cflags "${sbld_extra_ccxx_cflags} -ftree-vectorize -flto=auto")
+  endif()
+endif()
+if ( SBLD_ISINTEL )
+  #Intel defaults to the equivalent of -ffast-math, revert back to proper math:
+  set( sbld_extra_ccxx_cflags "${sbld_extra_ccxx_cflags} -fp-model=precise")
+endif()
+if ( SBLD_RELDBG_MODE )
+  #NB: Fortran -g is handled in ExtDep_Fortran.cmake
+  set( sbld_extra_ccxx_cflags "${sbld_extra_ccxx_cflags} -g")
+endif()
+
+if ( sbld_extra_ccxx_cflags )
+  set(SBLD_GLOBAL_COMPILE_FLAGS_CXX "${SBLD_GLOBAL_COMPILE_FLAGS_CXX} ${sbld_extra_ccxx_cflags}")
+  set(SBLD_GLOBAL_COMPILE_FLAGS_C     "${SBLD_GLOBAL_COMPILE_FLAGS_C} ${sbld_extra_ccxx_cflags}")
+endif()
+
 #To be filled with versions of global ext deps (Python):
 set(SBLD_GLOBAL_VERSION_DEPS_CXX "")
 set(SBLD_GLOBAL_VERSION_DEPS_C "")
 set(SBLD_GLOBAL_VERSION_DEPS_Fortran "")
 
 include("Utils.cmake")
 include("Detect.cmake")
```

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/Detect.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/Detect.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/ExtDep_Python.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/ExtDep_Python.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/ExtDep_pybind11.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/ExtDep_pybind11.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/ExtractFlags.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/ExtractFlags.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/Utils.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/Utils.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/WriteResults.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/WriteResults.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/extract_flags_helper.py` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/extract_flags_helper.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_DL.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_DL.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Fortran.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Fortran.cmake`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,20 @@
   else()
     set( tmp_abort_fortran "1" )
   endif()
 endif()
 
 if ( NOT tmp_abort_fortran )
   set(HAS_Fortran 1)
-  set(ExtDep_Fortran_COMPILE_FLAGS "")
+  if ( SBLD_RELDBG_MODE )
+    set(ExtDep_Fortran_COMPILE_FLAGS "-g")
+  else()
+    set(ExtDep_Fortran_COMPILE_FLAGS "")
+  endif()
+
   set(ExtDep_Fortran_LINK_FLAGS "")
   list(REMOVE_DUPLICATES CMAKE_Fortran_IMPLICIT_LINK_LIBRARIES)
   set(tmp_fortran_striplgcc OFF)
   if (APPLE AND UNIX AND CMAKE_CXX_COMPILER_ID MATCHES "Clang")
     #In the special case OSX+Clang, we forbid any -lgcc* to creep in via the
     #detected fortran link flags. This is a nasty unmaintainable workaround, but
     #at least works for now (see DGSW-442):
```

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Garfield.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Garfield.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Geant4.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Geant4.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_HDF5.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_HDF5.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_NCrystal.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_NCrystal.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Numpy.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Numpy.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_OSG.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_OSG.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Pandas.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Pandas.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_ROOT.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_ROOT.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_Scipy.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_Scipy.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_ZLib.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_ZLib.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/cmake/optional/ExtDep_matplotlib.cmake` & `simple_build_system-1.2.0/src/_simple_build_system/data/cmake/optional/ExtDep_matplotlib.cmake`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libinc/FPE.hh` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libinc/FPE.hh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libinc/File.hh` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libinc/File.hh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libinc/FindData.hh` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libinc/FindData.hh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libinc/Python.hh` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libinc/Python.hh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libinc/String.hh` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libinc/String.hh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libinc/Types.hh` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libinc/Types.hh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/FPE.cc` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libsrc/FPE.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/File.cc` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libsrc/File.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/FindData.cc` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libsrc/FindData.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/libsrc/String.cc` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/libsrc/String.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/pycpp_FPE/mod.cc` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/pycpp_FPE/mod.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/python/CpuDetect.py` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/python/CpuDetect.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/python/FindData.py` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/python/FindData.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/python/FindData3.py` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/python/FindData3.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/python/System.py` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/python/System.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/python/find_libpython.py` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/python/find_libpython.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/scripts/extdeps` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/scripts/extdeps`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/scripts/finddata` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/scripts/finddata`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/scripts/queryenv` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/scripts/queryenv`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core/Core/scripts/reflogupdate` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core/Core/scripts/reflogupdate`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_forcefpe/main.cc` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_forcefpe/main.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testfile/main.cc` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testfile/main.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testformat/main.cc` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_testformat/main.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_teststring/main.cc` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/app_teststring/main.cc`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testfpe` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testfpe`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testlibsymbols` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testlibsymbols`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testnodostxt` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testnodostxt`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testpylibsymbols` & `simple_build_system-1.2.0/src/_simple_build_system/data/pkgs-core_val/CoreTests/scripts/testpylibsymbols`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/resources/shellrc_snippet.sh` & `simple_build_system-1.2.0/src/_simple_build_system/data/resources/shellrc_snippet.sh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/data/resources/shellrc_snippet_deactivate.sh` & `simple_build_system-1.2.0/src/_simple_build_system/data/resources/shellrc_snippet_deactivate.sh`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/db.py` & `simple_build_system-1.2.0/src/_simple_build_system/db.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/dirs.py` & `simple_build_system-1.2.0/src/_simple_build_system/dirs.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/dotgen.py` & `simple_build_system-1.2.0/src/_simple_build_system/dotgen.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/envcfg.py` & `simple_build_system-1.2.0/src/_simple_build_system/envcfg.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,20 +28,24 @@
 
     cachedir_postfix = ( '' if main_cfg.build_mode=='release'
                            else f'_{main_cfg.build_mode}' )
 
     import shlex
     _cmake_args = shlex.split( _query('CMAKE_ARGS') or '' )
 
-    if main_cfg.build_mode=='release':
+    if main_cfg.build_mode in ('release','reldbg'):
         _cmake_args.append('-DCMAKE_BUILD_TYPE=Release')
+        if main_cfg.build_mode == 'reldbg':
+            #not just CMAKE_BUILD_TYPE=RelWithDebInfo since that changes other
+            #flags as well.
+            _cmake_args.append('-DSBLD_RELDBG_MODE=ON')
     else:
         assert main_cfg.build_mode=='debug'
         _cmake_args.append('-DCMAKE_BUILD_TYPE=Debug')
-    _build_mode_summary_string = main_cfg.build_mode.capitalize()
+    _build_mode_summary_string = main_cfg.build_mode#.capitalize()
 
     class EnvCfg:
 
         #These are the basic ones:
         build_dir_resolved = cfg.build_cachedir / f'bld{cachedir_postfix}'
         install_dir_resolved = cfg.build_cachedir / f'install{cachedir_postfix}'
```

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/envsetup.py` & `simple_build_system-1.2.0/src/_simple_build_system/envsetup.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/error.py` & `simple_build_system-1.2.0/src/_simple_build_system/error.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/extractenv.py` & `simple_build_system-1.2.0/src/_simple_build_system/extractenv.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/find.py` & `simple_build_system-1.2.0/src/_simple_build_system/find.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/formatlist.py` & `simple_build_system-1.2.0/src/_simple_build_system/formatlist.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/frontend.py` & `simple_build_system-1.2.0/src/_simple_build_system/frontend.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/grep.py` & `simple_build_system-1.2.0/src/_simple_build_system/grep.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/incinfo.py` & `simple_build_system-1.2.0/src/_simple_build_system/incinfo.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/includes.py` & `simple_build_system-1.2.0/src/_simple_build_system/includes.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/init_project.py` & `simple_build_system-1.2.0/src/_simple_build_system/init_project.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,18 +16,28 @@
                 otherargs.append( e )
         if pick_last:
             optvals = optvals[-1] if optvals else None
         return otherargs, optvals
 
     #Keywords:
     args, debug_mode = has_keyword(args, 'DEBUG')
+    args, release_mode = has_keyword(args, 'RELEASE')
+    args, reldbg_mode = has_keyword(args, 'RELDBG' )
     args, compact = has_keyword(args, 'COMPACT')
     args, build_cachedir = extract_opt_with_args( args, 'CACHEDIR',
                                                   pick_last = True)
 
+    _n_mode_opts=sum(int(e) for e in (debug_mode,release_mode,reldbg_mode))
+    if _n_mode_opts == 0:
+        release_mode=True
+    elif _n_mode_opts > 1:
+        from .error import error
+        error('Do not specify more than one of the DEBUG, '
+              'RELEASE, and RELDBG keywords')
+
     #Remaining args are the dep-bundles, but remove duplicates:
     depbundles = []
     for d in args:
         if d not in depbundles:
             depbundles.append(d)
 
     from .io import print
@@ -35,18 +45,20 @@
     cwd = pathlib.Path.cwd()
     template = ( pathlib.Path(__file__).parent
                  / 'data' / 'cfgtemplate.txt' ).read_text()
     res = ''
     for e in template.splitlines():
         res += e.rstrip()+'\n'
         if e.startswith('[build]'):
-            if debug_mode:
+            if ( debug_mode or reldbg_mode ):
                 #inject mode statement:
                 sbundles = "', '".join(depbundles)
-                res += "\n  mode = 'debug'\n\n"
+                res += "\n  mode = '%s'\n\n"%( 'debug'
+                                               if debug_mode
+                                               else 'reldbg' )
             if build_cachedir:
                 #inject cachedir statement:
                 res += f"\n  cachedir = '{build_cachedir}'\n\n"
         elif e.startswith('[depend]'):
             if depbundles:
                 #inject depend.bundles list:
                 sbundles = "', '".join(depbundles)
```

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/instsl.py` & `simple_build_system-1.2.0/src/_simple_build_system/instsl.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/instsl2.py` & `simple_build_system-1.2.0/src/_simple_build_system/instsl2.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/io.py` & `simple_build_system-1.2.0/src/_simple_build_system/io.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/langs.py` & `simple_build_system-1.2.0/src/_simple_build_system/langs.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/loadpkgs.py` & `simple_build_system-1.2.0/src/_simple_build_system/loadpkgs.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/makefile.py` & `simple_build_system-1.2.0/src/_simple_build_system/makefile.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/mtime.py` & `simple_build_system-1.2.0/src/_simple_build_system/mtime.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/parse_args.py` & `simple_build_system-1.2.0/src/_simple_build_system/parse_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,28 +34,39 @@
                         '--init --help for more options.')
     _p = progname
     initmode_longhelp = f"""
 
 New bundle initialisation mode ("{_p} --init") is used to initialise a new
 simplebuild bundle in the current directory by creating a simplebuild.cfg
 file. Additional arguments can be used to specify bundles which the new bundle
-should depend on, or they can be a special keyword (DEBUG|COMPACT|...). In any
-case, it might be most convenient to edit the simplebuild.cfg file afterwards to
-fine-tune the desired settings.
+should depend on, or they can be a special keyword (DEBUG|RELDBG|COMPACT|...).
+In any case, it might be most convenient to edit the simplebuild.cfg file
+afterwards to fine-tune the desired settings.
 
 Examples of {_p} --init usage:
 
 $> {_p} --init core_val
 
     Set up bundle which depends on the core_val bundle.
 
+$> {_p} --init RELEASE
+
+    Set up bundle with default build options for compilation of binaries
+    (build.mode='release'). This is the default behaviour.
+
 $> {_p} --init DEBUG
 
     Set up bundle with build options for producing debug symbols
-    (build.mode='debug').
+    (build.mode='debug'). Also reduces compiler optimisation levels and enables
+    additional safe checks in code.
+
+$> {_p} --init RELDBG
+
+    Set up bundle with build options for producing debug symbols
+    but otherwise keep all compiler optimisations (build.mode='reldbg').
 
 $> {_p} --init COMPACT
 
     The resulting simplebuild.cfg file will have all comments and empty lines
     stripped.
 
 $> {_p} --init core_val dgcode COMPACT DEBUG
@@ -306,14 +317,19 @@
             if not special_init_opt and not is_valid_bundle_name(a):
                 parser.error(f'Invalid name for dependency bundle: {a}')
             args.init.append( a )
         args_unused = []
     else:
         args.init = None
 
+    if args.init and sum(int(e in args.init)
+                         for e in ('RELEASE','DEBUG','RELDBG')) > 1:
+        parser.error('Do not specify more than one of the DEBUG, RELEASE, and'
+                     ' RELDBG keywords with --init')
+
     if args_unused:
         parser.error("Unrecognised arguments: %s"%' '.join(args_unused))
 
     if return_parser:
         return parser, args
     else:
         return args
```

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/pkgfilter.py` & `simple_build_system-1.2.0/src/_simple_build_system/pkgfilter.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/pkgutils.py` & `simple_build_system-1.2.0/src/_simple_build_system/pkgutils.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/replace.py` & `simple_build_system-1.2.0/src/_simple_build_system/replace.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/singlecfg.py` & `simple_build_system-1.2.0/src/_simple_build_system/singlecfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
     return dict( bundle   = dict( name        = (decode_valid_lowercase_identifier_string,None),
                                   pkg_root      = (decode_dir, '.'),
                                   env_paths   = (decode_is_env_paths,[]),
                                  ),
                  depend    = dict( bundles     = (decode_is_list_of_valid_lowercase_identifier_string,[]),
                                    search_path = (decode_list_of_search_paths,[])
                                   ),
-                 build     = dict( mode = ( lambda a,b : decode_str_enum(a,b,('debug','release')), 'release' ),
+                 build     = dict( mode = ( lambda a,b : decode_str_enum(a,b,('debug','release','reldbg')), 'release' ),
                                    #njobs = (decode_nonneg_int, 0),
                                    cachedir = (decode_dir, './simplebuild_cache'),
                                    pkg_filter = (decode_is_list_of_nonempty_str,[]),
                                    #extdep_ignore = (decode_is_list_of_valid_identifier_string,[]),
                                    #cmake_flags = (decode_is_list_of_nonempty_str,[]),
                                    #extra_cflags = (decode_is_list_of_nonempty_str,[]),
                                    #extra_linkflags = (decode_is_list_of_nonempty_str,[]),
```

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/target_base.py` & `simple_build_system-1.2.0/src/_simple_build_system/target_base.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/target_builder.py` & `simple_build_system-1.2.0/src/_simple_build_system/target_builder.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/testlauncher.py` & `simple_build_system-1.2.0/src/_simple_build_system/testlauncher.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/testxml.py` & `simple_build_system-1.2.0/src/_simple_build_system/testxml.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/tfact_binary.py` & `simple_build_system-1.2.0/src/_simple_build_system/tfact_binary.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/tfact_headerdeps.py` & `simple_build_system-1.2.0/src/_simple_build_system/tfact_headerdeps.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/tfact_libavail.py` & `simple_build_system-1.2.0/src/_simple_build_system/tfact_libavail.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/tfact_prepinc.py` & `simple_build_system-1.2.0/src/_simple_build_system/tfact_prepinc.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/tfact_pyinit.py` & `simple_build_system-1.2.0/src/_simple_build_system/tfact_pyinit.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/tfact_reflogs.py` & `simple_build_system-1.2.0/src/_simple_build_system/tfact_reflogs.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/tfact_symlink.py` & `simple_build_system-1.2.0/src/_simple_build_system/tfact_symlink.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/_simple_build_system/utils.py` & `simple_build_system-1.2.0/src/_simple_build_system/utils.py`

 * *Files identical despite different names*

### Comparing `simple_build_system-1.1.2/src/simple_build_system.egg-info/PKG-INFO` & `simple_build_system-1.2.0/src/simple_build_system.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-build-system
-Version: 1.1.2
+Version: 1.2.0
 Summary: A very simple to use build system for projects with primarily C++/Python code, intended for usage by scientific developers without a strong SW-engineering background.
 Author-email: Thomas Kittelmann <thomas.kittelmann@ess.eu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `simple_build_system-1.1.2/src/simple_build_system.egg-info/SOURCES.txt` & `simple_build_system-1.2.0/src/simple_build_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

