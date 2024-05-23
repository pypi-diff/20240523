# Comparing `tmp/muFFT-0.9.3.tar.gz` & `tmp/mufft-0.90.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/muFFT-0.9.3.tar", last modified: Sun Jun 28 18:55:45 2020, max compression
+gzip compressed data, was "mufft-0.90.0.tar", last modified: Thu May 23 06:34:41 2024, max compression
```

## Comparing `muFFT-0.9.3.tar` & `mufft-0.90.0.tar`

### file list

```diff
@@ -1,463 +1,100 @@
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.827956 muFFT-0.9.3/
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)      166 2020-04-11 19:32:05.000000 muFFT-0.9.3/.clang-format
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)      393 2020-04-11 19:32:05.000000 muFFT-0.9.3/.dir-locals.el
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)       54 2020-06-15 10:42:08.000000 muFFT-0.9.3/.gitignore
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     3016 2020-06-17 08:16:35.000000 muFFT-0.9.3/.gitlab-ci.yml
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)      867 2020-06-28 18:46:06.000000 muFFT-0.9.3/CHANGELOG.md
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5806 2020-06-15 10:42:08.000000 muFFT-0.9.3/CMakeLists.txt
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)      210 2020-04-11 19:32:05.000000 muFFT-0.9.3/CPPLINT.cfg
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)    32005 2020-04-11 19:32:05.000000 muFFT-0.9.3/GLPv3
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     7652 2020-04-11 19:32:05.000000 muFFT-0.9.3/LICENSE
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)      346 2020-06-17 10:28:12.000000 muFFT-0.9.3/MANIFEST.in
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)      302 2020-06-28 18:55:45.827956 muFFT-0.9.3/PKG-INFO
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3852 2020-05-22 20:07:18.000000 muFFT-0.9.3/README.md
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.730956 muFFT-0.9.3/cmake/
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     1551 2020-04-11 19:32:05.000000 muFFT-0.9.3/cmake/Eigen3.cmake
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5002 2020-05-22 20:07:18.000000 muFFT-0.9.3/cmake/FindFFTW3.cmake
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     1931 2020-04-11 19:32:05.000000 muFFT-0.9.3/cmake/FindPFFT.cmake
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     8113 2020-04-11 19:32:05.000000 muFFT-0.9.3/cmake/FindPythonLibsNew.cmake
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)      307 2020-04-11 19:32:05.000000 muFFT-0.9.3/cmake/FindSphinx.cmake
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)      400 2020-04-11 19:32:05.000000 muFFT-0.9.3/cmake/Findcorkpp.cmake
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     1483 2020-04-11 19:32:05.000000 muFFT-0.9.3/cmake/Findgmp.cmake
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3796 2020-06-15 10:42:08.000000 muFFT-0.9.3/cmake/cpplint.cmake
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9760 2020-06-15 10:42:08.000000 muFFT-0.9.3/cmake/git_watcher.cmake
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6007 2020-05-22 20:07:18.000000 muFFT-0.9.3/cmake/muTools.cmake
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7165 2020-05-22 20:07:18.000000 muFFT-0.9.3/cmake/muspectreTools.cmake
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)      692 2020-04-11 19:32:05.000000 muFFT-0.9.3/cmake/pybind11.cmake
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.730956 muFFT-0.9.3/doc/
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     2548 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/CMakeLists.txt
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.732956 muFFT-0.9.3/doc/dev-docs/
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)    94508 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/MainSchema.png
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)      608 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/Makefile
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)    58298 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/logo_flat.png
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)    37122 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/logo_square.png
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)       71 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/requirements.txt
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.738956 muFFT-0.9.3/doc/dev-docs/source/
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     3962 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/CellSplit.rst
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)   175672 2020-05-22 20:07:18.000000 muFFT-0.9.3/doc/dev-docs/source/CodingConvention.rst
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     4357 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/ConstitutiveLaws.rst
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)      858 2020-05-22 20:07:18.000000 muFFT-0.9.3/doc/dev-docs/source/Doxyfile
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4833 2020-05-22 20:07:18.000000 muFFT-0.9.3/doc/dev-docs/source/GettingStarted.rst
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)    41053 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/License.rst
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     5181 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/MaterialLaminate.rst
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     2515 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/MaterialLinearElasticGeneric.rst
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)    10554 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/NewMaterial.rst
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     1011 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/OrganisationOfCode.rst
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)       78 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/Reference.rst
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     3708 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/Summary.rst
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)      154 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/Tutorials.rst
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     6793 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/conf.py
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     1126 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/index.rst
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)       30 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/input_def
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)       30 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/input_def.in
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    17602 2020-05-22 20:07:18.000000 muFFT-0.9.3/doc/dev-docs/source/muGrid.rst
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)       30 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/xml_output_def
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)       50 2020-04-11 19:32:05.000000 muFFT-0.9.3/doc/dev-docs/source/xml_output_def.in
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3453 2020-05-22 20:07:18.000000 muFFT-0.9.3/doc/summary.rmk
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.739956 muFFT-0.9.3/dockerfiles/
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)      137 2020-04-11 19:32:05.000000 muFFT-0.9.3/dockerfiles/README
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.739956 muFFT-0.9.3/dockerfiles/debian:stable/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1138 2020-05-22 20:07:18.000000 muFFT-0.9.3/dockerfiles/debian:stable/Dockerfile
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.739956 muFFT-0.9.3/dockerfiles/debian:testing/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1949 2020-05-22 20:07:18.000000 muFFT-0.9.3/dockerfiles/debian:testing/Dockerfile
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)      675 2020-05-22 20:07:18.000000 muFFT-0.9.3/dockerfiles/docker_debian_stable
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)      754 2020-05-22 20:07:18.000000 muFFT-0.9.3/dockerfiles/docker_debian_testing
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.739956 muFFT-0.9.3/dockerfiles/ubuntu:16.04/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)      870 2020-05-22 20:07:18.000000 muFFT-0.9.3/dockerfiles/ubuntu:16.04/Dockerfile
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.739956 muFFT-0.9.3/dockerfiles/ubuntu:18.04/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)      898 2020-05-22 20:07:18.000000 muFFT-0.9.3/dockerfiles/ubuntu:18.04/Dockerfile
--rwxrwxr-x   0 pastewka  (1000) pastewka  (1000)      654 2020-04-11 19:32:05.000000 muFFT-0.9.3/dockerfiles/update_dockers.sh
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.747956 muFFT-0.9.3/examples/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4697 2020-06-15 10:42:08.000000 muFFT-0.9.3/examples/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    13926 2020-06-15 10:42:20.000000 muFFT-0.9.3/examples/circle_gibbs_ringing_simple_split_laminate.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8748 2020-05-22 20:07:18.000000 muFFT-0.9.3/examples/comparison_small_strain.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5359 2020-05-22 20:07:18.000000 muFFT-0.9.3/examples/crack.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5127 2020-06-15 10:42:08.000000 muFFT-0.9.3/examples/demonstrator_dynamic_solve.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5648 2020-06-15 10:42:08.000000 muFFT-0.9.3/examples/demonstrator_mpi.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3487 2020-06-15 10:42:08.000000 muFFT-0.9.3/examples/elasto_plastic_comparison.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2947 2020-06-15 10:42:08.000000 muFFT-0.9.3/examples/hyper-elasticity.cc
--rwxr-xr-x   0 pastewka  (1000) pastewka  (1000)     3061 2020-05-22 20:07:18.000000 muFFT-0.9.3/examples/hyper-elasticity.py
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)  1556044 2020-04-11 19:32:05.000000 muFFT-0.9.3/examples/odd_image.npz
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6616 2020-06-15 10:42:20.000000 muFFT-0.9.3/examples/projection_comparison.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4578 2020-06-15 10:42:08.000000 muFFT-0.9.3/examples/projection_comparison.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2128 2020-05-22 20:07:18.000000 muFFT-0.9.3/examples/python_example_imports.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2487 2020-06-28 18:44:41.000000 muFFT-0.9.3/examples/small_case.cc
--rwxr-xr-x   0 pastewka  (1000) pastewka  (1000)     3706 2020-05-22 20:07:18.000000 muFFT-0.9.3/examples/small_case.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2978 2020-06-15 10:42:08.000000 muFFT-0.9.3/examples/small_elasto_plastic_case.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2899 2020-06-15 10:42:08.000000 muFFT-0.9.3/examples/small_elasto_plastic_case.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3956 2020-06-15 10:42:08.000000 muFFT-0.9.3/examples/tutorial_example.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7024 2020-06-15 10:42:08.000000 muFFT-0.9.3/examples/visco_example.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8268 2020-06-28 18:44:41.000000 muFFT-0.9.3/examples/visco_example_damage.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6988 2020-05-22 20:07:18.000000 muFFT-0.9.3/examples/visualisation_example_finite_strain.py
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.749956 muFFT-0.9.3/external/
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)      293 2020-04-11 19:32:05.000000 muFFT-0.9.3/external/CMakeLists.txt
--rwxrwxr-x   0 pastewka  (1000) pastewka  (1000)   249206 2020-04-11 19:32:05.000000 muFFT-0.9.3/external/cpplint.py
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)    27652 2020-04-11 19:32:05.000000 muFFT-0.9.3/external/cxxopts.hpp
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.750956 muFFT-0.9.3/language_bindings/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1518 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/CMakeLists.txt
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.750956 muFFT-0.9.3/language_bindings/libmufft/
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     1463 2020-04-11 19:32:05.000000 muFFT-0.9.3/language_bindings/libmufft/CMakeLists.txt
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.754956 muFFT-0.9.3/language_bindings/libmufft/python/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3367 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/libmufft/python/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4838 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/libmufft/python/bind_py_common.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2974 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/libmufft/python/bind_py_communicator.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1745 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/libmufft/python/bind_py_declarations.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7820 2020-06-28 18:44:41.000000 muFFT-0.9.3/language_bindings/libmufft/python/bind_py_derivatives.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    22155 2020-06-28 18:44:41.000000 muFFT-0.9.3/language_bindings/libmufft/python/bind_py_fftengine.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1538 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/libmufft/python/bind_py_module.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1357 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/libmufft/python/bind_py_version.cc.skeleton
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.755956 muFFT-0.9.3/language_bindings/libmufft/python/muFFT/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3239 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/libmufft/python/muFFT/Communicator.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    17601 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/libmufft/python/muFFT/NetCDF.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2379 2020-06-15 10:42:20.000000 muFFT-0.9.3/language_bindings/libmufft/python/muFFT/Stencils2D.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3418 2020-06-15 10:42:20.000000 muFFT-0.9.3/language_bindings/libmufft/python/muFFT/Stencils3D.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4433 2020-06-28 18:44:41.000000 muFFT-0.9.3/language_bindings/libmufft/python/muFFT/__init__.py
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.755956 muFFT-0.9.3/language_bindings/libmugrid/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1488 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/libmugrid/CMakeLists.txt
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.757956 muFFT-0.9.3/language_bindings/libmugrid/python/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3133 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/libmugrid/python/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6564 2020-06-28 18:44:41.000000 muFFT-0.9.3/language_bindings/libmugrid/python/bind_py_common.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1746 2020-06-28 18:44:41.000000 muFFT-0.9.3/language_bindings/libmugrid/python/bind_py_declarations.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7912 2020-06-28 18:44:41.000000 muFFT-0.9.3/language_bindings/libmugrid/python/bind_py_field.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9287 2020-06-28 18:44:41.000000 muFFT-0.9.3/language_bindings/libmugrid/python/bind_py_field_collection.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1555 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/libmugrid/python/bind_py_module.cc
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.757956 muFFT-0.9.3/language_bindings/libmugrid/python/muGrid/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1524 2020-06-28 18:44:41.000000 muFFT-0.9.3/language_bindings/libmugrid/python/muGrid/__init__.py
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.762956 muFFT-0.9.3/language_bindings/python/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4360 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/python/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    19296 2020-06-28 18:44:41.000000 muFFT-0.9.3/language_bindings/python/bind_py_cell.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4507 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/python/bind_py_common.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1845 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/python/bind_py_declarations.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    11833 2020-06-15 10:42:20.000000 muFFT-0.9.3/language_bindings/python/bind_py_material.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3114 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_hyper_elasto_plastic1.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3185 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_hyper_elasto_plastic2.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3444 2020-06-15 10:42:20.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_laminate.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2850 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_linear_anisotropic.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3365 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_linear_elastic1.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3102 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_linear_elastic2.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2904 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_linear_elastic3.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2922 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_linear_elastic4.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5981 2020-06-28 18:44:41.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_linear_elastic_generic.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2652 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_linear_orthotropic.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3333 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_neo_hookean_elastic.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5147 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_stochastic_plasticity.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3522 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_visco_elastic_damage_ss.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3239 2020-06-15 10:42:08.000000 muFFT-0.9.3/language_bindings/python/bind_py_material_visco_elastic_ss.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1571 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/python/bind_py_module.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10286 2020-06-28 18:44:41.000000 muFFT-0.9.3/language_bindings/python/bind_py_projections.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6014 2020-06-28 18:44:41.000000 muFFT-0.9.3/language_bindings/python/bind_py_solvers.cc
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.764956 muFFT-0.9.3/language_bindings/python/muSpectre/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6709 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/python/muSpectre/__init__.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    41217 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/python/muSpectre/eshelby_slow.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    24682 2020-06-28 18:44:41.000000 muFFT-0.9.3/language_bindings/python/muSpectre/gradient_integration.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    29274 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/python/muSpectre/stochastic_plasticity_search.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6279 2020-05-22 20:07:18.000000 muFFT-0.9.3/language_bindings/python/muSpectre/vtk_export.py
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.766956 muFFT-0.9.3/muFFT.egg-info/
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)      302 2020-06-28 18:55:45.000000 muFFT-0.9.3/muFFT.egg-info/PKG-INFO
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)    15537 2020-06-28 18:55:45.000000 muFFT-0.9.3/muFFT.egg-info/SOURCES.txt
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)        1 2020-06-28 18:55:45.000000 muFFT-0.9.3/muFFT.egg-info/dependency_links.txt
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)        1 2020-05-07 14:28:20.000000 muFFT-0.9.3/muFFT.egg-info/not-zip-safe
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)        6 2020-06-28 18:55:45.000000 muFFT-0.9.3/muFFT.egg-info/requires.txt
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)       28 2020-06-28 18:55:45.000000 muFFT-0.9.3/muFFT.egg-info/top_level.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)       26 2020-05-22 20:07:18.000000 muFFT-0.9.3/requirements.txt
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)       38 2020-06-28 18:55:45.827956 muFFT-0.9.3/setup.cfg
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)    22299 2020-06-28 18:54:46.000000 muFFT-0.9.3/setup.py
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.766956 muFFT-0.9.3/snippets/
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     1566 2020-04-11 19:32:05.000000 muFFT-0.9.3/snippets/µSpectre_cmake_header
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1504 2020-05-22 20:07:18.000000 muFFT-0.9.3/snippets/µSpectre_cpp_header
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     1428 2020-04-11 19:32:05.000000 muFFT-0.9.3/snippets/µSpectre_py_header
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.767956 muFFT-0.9.3/src/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4294 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/CMakeLists.txt
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.768956 muFFT-0.9.3/src/cell/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1657 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/cell/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    39867 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/cell/cell.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    16035 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/cell/cell.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4722 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/cell/cell_adaptor.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9620 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/cell/cell_factory.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    12929 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/cell/cell_split.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6755 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/cell/cell_split.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3098 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/cell/cell_split_factory.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1976 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/cell/cell_traits.hh
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.771956 muFFT-0.9.3/src/common/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1761 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/common/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4180 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/common/common.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    19782 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/common/geometry.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9760 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/common/git_watcher.cmake
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    15061 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/common/intersection_octree.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    11831 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/common/intersection_octree.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6057 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/common/intersection_volume_calculator_corkpp.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10052 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/common/muSpectre_common.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2653 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/common/version.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4537 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/common/voigt_conversion.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10780 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/common/voigt_conversion.hh
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.775956 muFFT-0.9.3/src/libmufft/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5284 2020-06-15 10:50:28.000000 muFFT-0.9.3/src/libmufft/CMakeLists.txt
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     4500 2020-06-17 08:16:35.000000 muFFT-0.9.3/src/libmufft/communicator.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5827 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/libmufft/communicator.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7182 2020-06-16 18:39:01.000000 muFFT-0.9.3/src/libmufft/derivative.cc
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)    12921 2020-06-17 08:16:35.000000 muFFT-0.9.3/src/libmufft/derivative.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5068 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmufft/fft_engine_base.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10169 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmufft/fft_engine_base.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1997 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/libmufft/fft_utils.cc
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     7278 2020-06-17 08:16:35.000000 muFFT-0.9.3/src/libmufft/fft_utils.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10584 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmufft/fftw_engine.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3406 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmufft/fftw_engine.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    19415 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmufft/fftwmpi_engine.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4754 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmufft/fftwmpi_engine.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9760 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/libmufft/git_watcher.cmake
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     3085 2020-06-17 08:16:35.000000 muFFT-0.9.3/src/libmufft/mufft_common.hh
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     9901 2020-06-17 08:16:35.000000 muFFT-0.9.3/src/libmufft/pfft_engine.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3521 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/libmufft/pfft_engine.hh
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     2477 2020-06-28 18:55:15.000000 muFFT-0.9.3/src/libmufft/version.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2477 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/libmufft/version.cc.skeleton
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.784956 muFFT-0.9.3/src/libmugrid/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3839 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4386 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/libmugrid/T4_map_proxy.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10705 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/ccoord_operations.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    29204 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/ccoord_operations.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7000 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/cpp_compliance.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    17276 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/libmugrid/eigen_tools.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3156 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/libmugrid/exception.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4559 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/libmugrid/exception.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9811 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/field.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9836 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/field.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    21183 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/field_collection.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    24105 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/field_collection.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4937 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/field_collection_global.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7016 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/field_collection_global.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2979 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/field_collection_local.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3900 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/field_collection_local.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8540 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/field_map.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10890 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/libmugrid/field_map.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    22706 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/libmugrid/field_map_static.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    21124 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/field_typed.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    14698 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/field_typed.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2561 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/grid_common.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    17221 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/grid_common.hh
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)    11626 2020-04-11 19:32:05.000000 muFFT-0.9.3/src/libmugrid/iterators.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10258 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/libmugrid/mapped_field.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9579 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/libmugrid/mapped_state_field.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    20294 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/numpy_tools.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3636 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/libmugrid/optional_mapped_field.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6178 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/raw_memory_operations.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2591 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/raw_memory_operations.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3458 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/libmugrid/ref_array.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3363 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/libmugrid/ref_vector.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6296 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/state_field.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8114 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/state_field.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7282 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/libmugrid/state_field_map.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8806 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/libmugrid/state_field_map.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    19060 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/libmugrid/state_field_map_static.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    20111 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/libmugrid/tensor_algebra.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    16052 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/libmugrid/units.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9219 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/libmugrid/units.hh
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.796956 muFFT-0.9.3/src/materials/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2676 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/materials/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    11881 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/iterable_proxy.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    30325 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/materials/laminate_homogenisation.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    17939 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/materials/laminate_homogenisation.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8865 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/materials/material_base.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10069 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_base.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    11329 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_evaluator.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9896 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_hyper_elasto_plastic1.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9976 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_hyper_elasto_plastic1.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5868 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_hyper_elasto_plastic2.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9025 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_hyper_elasto_plastic2.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7487 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_laminate.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7159 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_laminate.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3863 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/materials/material_linear_anisotropic.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6694 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_linear_anisotropic.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2386 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/materials/material_linear_elastic1.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7300 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_linear_elastic1.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2866 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_linear_elastic2.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6078 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_linear_elastic2.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3088 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_linear_elastic3.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7445 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_linear_elastic3.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3394 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_linear_elastic4.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8122 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_linear_elastic4.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2243 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/materials/material_linear_elastic_generic1.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8382 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_linear_elastic_generic1.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3083 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_linear_elastic_generic2.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7579 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_linear_elastic_generic2.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3977 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/materials/material_linear_orthotropic.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4698 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_linear_orthotropic.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    33731 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_muSpectre_base.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2358 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/materials/material_neo_hookean_elastic.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10657 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_neo_hookean_elastic.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7118 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_stochastic_plasticity.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    16040 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_stochastic_plasticity.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6872 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_visco_elastic_damage_ss.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10466 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_visco_elastic_damage_ss.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6052 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_visco_elastic_ss.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10804 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/material_visco_elastic_ss.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    38058 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/materials/materials_toolbox.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4469 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/materials/s_t_material_linear_elastic_generic1.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    11375 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/materials/s_t_material_linear_elastic_generic1.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5781 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/materials/stress_transformations.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1685 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/materials/stress_transformations_Kirchhoff.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6507 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/materials/stress_transformations_Kirchhoff_impl.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1651 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/materials/stress_transformations_PK1.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6374 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/materials/stress_transformations_PK1_impl.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1652 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/materials/stress_transformations_PK2.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8510 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/materials/stress_transformations_PK2_impl.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7350 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/materials/stress_transformations_default_case.hh
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.800956 muFFT-0.9.3/src/projection/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1860 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/projection/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5717 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/projection/projection_approx_Green_operator.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4410 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/projection/projection_approx_Green_operator.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4634 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/projection/projection_base.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7372 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/projection/projection_base.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3750 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/projection/projection_default.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4923 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/projection/projection_default.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4876 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/projection/projection_finite_strain.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3911 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/projection/projection_finite_strain.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7832 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/projection/projection_finite_strain_fast.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5617 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/projection/projection_finite_strain_fast.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4238 2020-06-15 10:42:08.000000 muFFT-0.9.3/src/projection/projection_small_strain.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4169 2020-06-15 10:42:20.000000 muFFT-0.9.3/src/projection/projection_small_strain.hh
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.803956 muFFT-0.9.3/src/solver/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1742 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/solver/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2462 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/solver/krylov_solver_base.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4021 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/solver/krylov_solver_base.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4234 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/solver/krylov_solver_cg.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3584 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/solver/krylov_solver_cg.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3681 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/solver/krylov_solver_eigen.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6791 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/solver/krylov_solver_eigen.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1735 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/solver/solver_common.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3141 2020-05-22 20:07:18.000000 muFFT-0.9.3/src/solver/solver_common.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    27325 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/solver/solvers.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4188 2020-06-28 18:44:41.000000 muFFT-0.9.3/src/solver/solvers.hh
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.816956 muFFT-0.9.3/tests/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4898 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    12917 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/elasto-plasticity.py
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.819956 muFFT-0.9.3/tests/libmufft/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2985 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/libmufft/CMakeLists.txt
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.819956 muFFT-0.9.3/tests/libmufft/license/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1947 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmufft/license/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1481 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmufft/main_test_suite.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2246 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/libmufft/mpi_context.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1550 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmufft/mpi_main_test_suite.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9464 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/libmufft/mpi_test_fft_engine.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1615 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmufft/python_binding_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2039 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmufft/python_communicator_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    29731 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/libmufft/python_derivative_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    22172 2020-06-28 18:44:41.000000 muFFT-0.9.3/tests/libmufft/python_fft_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1564 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/libmufft/python_mpi_binding_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5682 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmufft/python_muFFT_license_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6851 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmufft/python_netcdf_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2145 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmufft/python_test_imports.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3653 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/libmufft/test_fft_utils.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5969 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/libmufft/test_fftw_engine.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1811 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmufft/tests.hh
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.825956 muFFT-0.9.3/tests/libmugrid/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2635 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/libmugrid/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1654 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/libmugrid/field_test_fixtures.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5268 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/libmugrid/field_test_fixtures.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5123 2020-06-28 18:44:41.000000 muFFT-0.9.3/tests/libmugrid/header_test_ccoord_operations.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4610 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmugrid/header_test_eigen_tools.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1702 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmugrid/header_test_ref_array.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7334 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmugrid/header_test_t4_map.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    11181 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmugrid/header_test_tensor_algebra.cc
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.825956 muFFT-0.9.3/tests/libmugrid/license/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1959 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmugrid/license/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1484 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmugrid/main_test_suite.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1471 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmugrid/python_binding_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1689 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmugrid/python_common_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4158 2020-06-28 18:44:41.000000 muFFT-0.9.3/tests/libmugrid/python_field_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5587 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmugrid/python_muGrid_license_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1914 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmugrid/python_test_imports.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4833 2020-06-28 18:44:41.000000 muFFT-0.9.3/tests/libmugrid/test_ccoord_operations.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8831 2020-06-28 18:44:41.000000 muFFT-0.9.3/tests/libmugrid/test_field.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    14651 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/libmugrid/test_field_collection.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    11108 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/libmugrid/test_field_map.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2439 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmugrid/test_goodies.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10158 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/libmugrid/test_goodies.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    11503 2020-06-28 18:44:41.000000 muFFT-0.9.3/tests/libmugrid/test_mapped_fields.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4100 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/libmugrid/test_mapped_state_fields.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4775 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/libmugrid/test_raw_memory_operations.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10851 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/libmugrid/test_state_field_maps.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3274 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/libmugrid/test_state_fields.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6831 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmugrid/test_units.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1677 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/libmugrid/tests.hh
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.825956 muFFT-0.9.3/tests/license/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2409 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/license/CMakeLists.txt
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.826956 muFFT-0.9.3/tests/lint/
--rw-rw-r--   0 pastewka  (1000) pastewka  (1000)     1962 2020-04-11 19:32:05.000000 muFFT-0.9.3/tests/lint/CMakeLists.txt
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1493 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/main_test_suite.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2231 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/mpi_context.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1562 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/mpi_main_test_suite.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3481 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/mpi_test_projection.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8136 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/mpi_test_projection_finite.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7112 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/mpi_test_projection_small.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8320 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/mpi_test_solver_newton_cg.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2768 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_binding_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1936 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_cell_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6020 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_comparison_test_material_linear_elastic1.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5240 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_eigen_strain_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    35361 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_eshelby_slow_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    12148 2020-06-28 18:44:41.000000 muFFT-0.9.3/tests/python_exact_reference_elastic_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    30142 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_exact_reference_plastic_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3031 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_field_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    11145 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_goose_ref.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    39461 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/python_gradient_integration_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    13332 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/python_license_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3204 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_material_evaluator_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8766 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_material_hyper_elasto_plastic2_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1861 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_material_linear_elastic1_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3052 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/python_material_linear_elastic3_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4552 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_material_linear_elastic4_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4116 2020-06-28 18:44:41.000000 muFFT-0.9.3/tests/python_material_linear_elastic_generic1_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4214 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_material_linear_elastic_generic2_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4120 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_material_linear_elastic_generic_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1679 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_mpi_binding_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3834 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_mpi_material_linear_elastic4_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7148 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_mpi_projection_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    26361 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_mpi_stochastic_plasticity_search_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6094 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_muSpectre_license_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3512 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_muSpectre_vtk_export_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6539 2020-06-28 18:44:41.000000 muFFT-0.9.3/tests/python_projection_tests.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2632 2020-06-28 18:44:41.000000 muFFT-0.9.3/tests/python_solver_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    25799 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_stochastic_plasticity_search_test.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1951 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/python_test_imports.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    12010 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/python_vtk_export_test.py
-drwxrwxr-x   0 pastewka  (1000) pastewka  (1000)        0 2020-06-28 18:55:45.827956 muFFT-0.9.3/tests/reference_computations/
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2254 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/reference_computations/Esh3D_h5_to_npz.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2804 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/reference_computations/eshelby_inclusion.ref.npz
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4311 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/reference_computations/eshelby_inclusion_Esh3D.py
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     2804 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/reference_computations/eshelby_inhomogeneity.ref.npz
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5338 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/reference_computations/vtk_export_2D_test.ref.vtr
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    49064 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/reference_computations/vtk_export_3D_test.ref.vtr
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5388 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/split_test_corkpp.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8440 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/split_test_intersection_error_induced.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    23990 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/split_test_laminate_solver.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    20132 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/split_test_material_laminate.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     4742 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/split_test_patch_split_cell.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1450 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/test_base.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    18663 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/test_cell_base.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    13548 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/test_geometry.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    11412 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/test_material_evaluator.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    19052 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/test_material_hyper_elasto_plastic1.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    19884 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/test_material_hyper_elasto_plastic2.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10435 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/test_material_linear_elastic1.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3955 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/test_material_linear_elastic1.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    11209 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/test_material_linear_elastic2.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3465 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/test_material_linear_elastic3.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3534 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/test_material_linear_elastic4.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3403 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/test_material_linear_elastic_generic.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7855 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/test_material_linear_orthotropic.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     8049 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/test_material_neo_hookean.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    10812 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/test_material_visco_elastic_damage_ss.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    12030 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/test_material_visco_elastic_ss.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    15108 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/test_materials_toolbox.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5317 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/test_native_stress_storage.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6318 2020-06-15 10:42:08.000000 muFFT-0.9.3/tests/test_projection.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     9231 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/test_projection_finite.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    20695 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/test_projection_finite_discrete.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     7199 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/test_projection_small.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     3913 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/test_s_t_material_linear_elastic_generic1.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    13548 2020-06-15 10:42:20.000000 muFFT-0.9.3/tests/test_solver_newton_cg.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     6308 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/test_stress_transformation.hh
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5758 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/test_stress_transformation_Kirchhoff_Gradient.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     5471 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/test_stress_transformation_Kirchhoff_GreenLagrange.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)    11902 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/test_stress_transformation_PK2_GreenLagrange.cc
--rw-r--r--   0 pastewka  (1000) pastewka  (1000)     1632 2020-05-22 20:07:18.000000 muFFT-0.9.3/tests/tests.hh
+-rw-r--r--   0        0        0      195 2024-05-23 06:28:29.000000 mufft-0.90.0/.clang-format
+-rw-r--r--   0        0        0      148 2024-05-23 06:28:29.000000 mufft-0.90.0/.gitattributes
+-rw-r--r--   0        0        0      224 2024-05-23 06:28:29.000000 mufft-0.90.0/.github/.install_netcdf.sh
+-rw-r--r--   0        0        0      666 2024-05-23 06:28:29.000000 mufft-0.90.0/.github/install_netcdf4.sh
+-rw-r--r--   0        0        0     1091 2024-05-23 06:28:29.000000 mufft-0.90.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2563 2024-05-23 06:28:29.000000 mufft-0.90.0/.github/workflows/ubuntu.yml
+-rw-r--r--   0        0        0     2171 2024-05-23 06:28:29.000000 mufft-0.90.0/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       93 2024-05-23 06:28:29.000000 mufft-0.90.0/.gitignore
+-rw-r--r--   0        0        0      324 2024-05-23 06:28:29.000000 mufft-0.90.0/.gitmodules
+-rw-r--r--   0        0        0     7056 2024-05-23 06:28:29.000000 mufft-0.90.0/CHANGELOG.md
+-rw-r--r--   0        0        0      210 2024-05-23 06:28:29.000000 mufft-0.90.0/CPPLINT.cfg
+-rw-r--r--   0        0        0    35149 2024-05-23 06:28:29.000000 mufft-0.90.0/LICENSE
+-rw-r--r--   0        0        0     2526 2024-05-23 06:28:29.000000 mufft-0.90.0/README.md
+-rw-r--r--   0        0        0     5765 2024-05-23 06:28:29.000000 mufft-0.90.0/discover_version.py
+-rw-r--r--   0        0        0     2548 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/CMakeLists.txt
+-rw-r--r--   0        0        0    94508 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/MainSchema.png
+-rw-r--r--   0        0        0      608 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/Makefile
+-rw-r--r--   0        0        0    58298 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/logo_flat.png
+-rw-r--r--   0        0        0    37122 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/logo_square.png
+-rw-r--r--   0        0        0       86 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/requirements.txt
+-rw-r--r--   0        0        0     3962 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/CellSplit.rst
+-rw-r--r--   0        0        0   175727 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/CodingConvention.rst
+-rw-r--r--   0        0        0     4357 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/ConstitutiveLaws.rst
+-rw-r--r--   0        0        0      858 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/Doxyfile
+-rw-r--r--   0        0        0     5836 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/GettingStarted.rst
+-rw-r--r--   0        0        0    41053 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/License.rst
+-rw-r--r--   0        0        0     5181 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/MaterialLaminate.rst
+-rw-r--r--   0        0        0     2515 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/MaterialLinearElasticGeneric.rst
+-rw-r--r--   0        0        0    10554 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/NewMaterial.rst
+-rw-r--r--   0        0        0     1011 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/OrganisationOfCode.rst
+-rw-r--r--   0        0        0       78 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/Reference.rst
+-rw-r--r--   0        0        0     3871 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/Summary.rst
+-rw-r--r--   0        0        0      154 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/Tutorials.rst
+-rw-r--r--   0        0        0     6793 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/conf.py
+-rw-r--r--   0        0        0     1126 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/index.rst
+-rw-r--r--   0        0        0       30 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/input_def
+-rw-r--r--   0        0        0       30 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/input_def.in
+-rw-r--r--   0        0        0     1934 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/macosx14_bash_profile
+-rw-r--r--   0        0        0    19363 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/muGrid.rst
+-rw-r--r--   0        0        0       30 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/xml_output_def
+-rw-r--r--   0        0        0       50 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/xml_output_def.in
+-rw-r--r--   0        0        0     3327 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/summary.rmk
+-rw-r--r--   0        0        0       16 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/meson.build
+-rw-r--r--   0        0        0     4849 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/bind_py_common_mufft.cc
+-rw-r--r--   0        0        0     1710 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/bind_py_declarations.hh
+-rw-r--r--   0        0        0     9806 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/bind_py_derivatives.cc
+-rw-r--r--   0        0        0    22658 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/bind_py_fftengine.cc
+-rw-r--r--   0        0        0     1519 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/bind_py_module.cc
+-rw-r--r--   0        0        0     1357 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/bind_py_version.cc.skeleton
+-rw-r--r--   0        0        0      389 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/meson.build
+-rw-r--r--   0        0        0    17601 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/muFFT/NetCDF.py
+-rw-r--r--   0        0        0     1746 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/muFFT/Stencils1D.py
+-rw-r--r--   0        0        0     4275 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/muFFT/Stencils2D.py
+-rw-r--r--   0        0        0    11152 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/muFFT/Stencils3D.py
+-rw-r--r--   0        0        0     6841 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/muFFT/__init__.py
+-rw-r--r--   0        0        0      230 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/muFFT/meson.build
+-rw-r--r--   0        0        0     2845 2024-05-23 06:28:29.000000 mufft-0.90.0/meson.build
+-rw-r--r--   0        0        0     1909 2024-05-23 06:28:29.000000 mufft-0.90.0/pyproject.toml
+-rw-r--r--   0        0        0      114 2024-05-23 06:28:29.000000 mufft-0.90.0/renovate.json
+-rw-r--r--   0        0        0     7182 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/derivative.cc
+-rw-r--r--   0        0        0    13170 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/derivative.hh
+-rw-r--r--   0        0        0    38967 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fft_engine_base.cc
+-rw-r--r--   0        0        0    17691 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fft_engine_base.hh
+-rw-r--r--   0        0        0     1997 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fft_utils.cc
+-rw-r--r--   0        0        0     7278 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fft_utils.hh
+-rw-r--r--   0        0        0     9608 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fftw_engine.cc
+-rw-r--r--   0        0        0     5130 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fftw_engine.hh
+-rw-r--r--   0        0        0    15704 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fftwmpi_engine.cc
+-rw-r--r--   0        0        0     5950 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fftwmpi_engine.hh
+-rw-r--r--   0        0        0      601 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/meson.build
+-rw-r--r--   0        0        0     3138 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/mufft_common.hh
+-rw-r--r--   0        0        0    14560 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/pfft_engine.cc
+-rw-r--r--   0        0        0     5595 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/pfft_engine.hh
+-rw-r--r--   0        0        0    14089 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/pocketfft_engine.cc
+-rw-r--r--   0        0        0     4559 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/pocketfft_engine.hh
+-rw-r--r--   0        0        0     2631 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/version.cc
+-rw-r--r--   0        0        0      163 2024-05-23 06:28:29.000000 mufft-0.90.0/src/meson.build
+-rw-r--r--   0        0        0      590 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/eigen.wrap
+-rw-r--r--   0        0        0      139 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/mugrid.wrap
+-rw-r--r--   0        0        0     1498 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/pocketfft/LICENSE.md
+-rw-r--r--   0        0        0      265 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/pocketfft/POCKETFFT.md
+-rw-r--r--   0        0        0    10843 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/pocketfft/README.md
+-rw-r--r--   0        0        0      116 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/pocketfft/meson.build
+-rw-r--r--   0        0        0   110573 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/pocketfft/pocketfft_hdronly.h
+-rw-r--r--   0        0        0      616 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/pybind11.wrap
+-rw-r--r--   0        0        0     1564 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/main_test_suite.cc
+-rw-r--r--   0        0        0     2404 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/meson.build
+-rw-r--r--   0        0        0     2329 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/mpi_context.hh
+-rw-r--r--   0        0        0     1633 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/mpi_main_test_suite.cc
+-rw-r--r--   0        0        0     8189 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/mpi_test_fft_engine.cc
+-rw-r--r--   0        0        0     1657 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/python_binding_tests.py
+-rw-r--r--   0        0        0    47442 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/python_derivative_tests.py
+-rw-r--r--   0        0        0    36055 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/python_fft_tests.py
+-rw-r--r--   0        0        0     1482 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/python_mpi_binding_tests.py
+-rw-r--r--   0        0        0     5682 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/python_muFFT_license_test.py
+-rw-r--r--   0        0        0     7223 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/python_netcdf_tests.py
+-rw-r--r--   0        0        0     3653 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/test_fft_utils.cc
+-rw-r--r--   0        0        0     7651 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/test_serial_fft_engines.cc
+-rw-r--r--   0        0        0     1880 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/tests.hh
+-rw-r--r--   0        0        0    43893 2024-05-23 06:34:41.621605 mufft-0.90.0/PKG-INFO
```

### Comparing `muFFT-0.9.3/GLPv3` & `mufft-0.90.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,189 +1,674 @@
-GNU GENERAL PUBLIC LICENSE
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
 
-Version 3, 29 June 2007
-
-Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>
-
-Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
-Preamble
-
-The GNU General Public License is a free, copyleft license for software and other kinds of works.
-
-The licenses for most software and other practical works are designed to take away your freedom to share and change the works. By contrast, the GNU General Public License is intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users. We, the Free Software Foundation, use the GNU General Public License for most of our software; it applies also to any other work released this way by its authors. You can apply it to your programs, too.
-
-When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for them if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs, and that you know you can do these things.
-
-To protect your rights, we need to prevent others from denying you these rights or asking you to surrender the rights. Therefore, you have certain responsibilities if you distribute copies of the software, or if you modify it: responsibilities to respect the freedom of others.
-
-For example, if you distribute copies of such a program, whether gratis or for a fee, you must pass on to the recipients the same freedoms that you received. You must make sure that they, too, receive or can get the source code. And you must show them these terms so they know their rights.
-
-Developers that use the GNU GPL protect your rights with two steps: (1) assert copyright on the software, and (2) offer you this License giving you legal permission to copy, distribute and/or modify it.
-
-For the developers' and authors' protection, the GPL clearly explains that there is no warranty for this free software. For both users' and authors' sake, the GPL requires that modified versions be marked as changed, so that their problems will not be attributed erroneously to authors of previous versions.
-
-Some devices are designed to deny users access to install or run modified versions of the software inside them, although the manufacturer can do so. This is fundamentally incompatible with the aim of protecting users' freedom to change the software. The systematic pattern of such abuse occurs in the area of products for individuals to use, which is precisely where it is most unacceptable. Therefore, we have designed this version of the GPL to prohibit the practice for those products. If such problems arise substantially in other domains, we stand ready to extend this provision to those domains in future versions of the GPL, as needed to protect the freedom of users.
-
-Finally, every program is threatened constantly by software patents. States should not allow patents to restrict development and use of software on general-purpose computers, but in those that do, we wish to avoid the special danger that patents applied to a free program could make it effectively proprietary. To prevent this, the GPL assures that patents cannot be used to render the program non-free.
-
-The precise terms and conditions for copying, distribution and modification follow.
-TERMS AND CONDITIONS
-0. Definitions.
-
-“This License” refers to version 3 of the GNU General Public License.
-
-“Copyright” also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
-
-“The Program” refers to any copyrightable work licensed under this License. Each licensee is addressed as “you”. “Licensees” and “recipients” may be individuals or organizations.
-
-To “modify” a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a “modified version” of the earlier work or a work “based on” the earlier work.
-
-A “covered work” means either the unmodified Program or a work based on the Program.
-
-To “propagate” a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
-
-To “convey” a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
-
-An interactive user interface displays “Appropriate Legal Notices” to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
-1. Source Code.
-
-The “source code” for a work means the preferred form of the work for making modifications to it. “Object code” means any non-source form of a work.
-
-A “Standard Interface” means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
-
-The “System Libraries” of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A “Major Component”, in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
-
-The “Corresponding Source” for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
-
-The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
-
-The Corresponding Source for a work in source code form is that same work.
-2. Basic Permissions.
-
-All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
-
-You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
-
-Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
-3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
-
-When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
-4. Conveying Verbatim Copies.
-
-You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
-
-You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
-5. Conveying Modified Source Versions.
-
-You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
-    b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to “keep intact all notices”.
-    c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
-    d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
-
-A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an “aggregate” if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
-6. Conveying Non-Source Forms.
-
-You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
-    b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
-    c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
-    d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
-    e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
-
-A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
-
-A “User Product” is either (1) a “consumer product”, which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, “normally used” refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
-
-“Installation Information” for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
-
-If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
-
-The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
-
-Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
-7. Additional Terms.
-
-“Additional permissions” are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
-
-When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
-
-Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
-    b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
-    c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
-    d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
-    e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
-    f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
-
-All other non-permissive additional terms are considered “further restrictions” within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
-
-If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
-
-Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
-8. Termination.
-
-You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
-
-However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
-
-Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
-
-Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
-9. Acceptance Not Required for Having Copies.
-
-You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
-10. Automatic Licensing of Downstream Recipients.
-
-Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
-
-An “entity transaction” is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
-
-You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
-11. Patents.
-
-A “contributor” is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's “contributor version”.
-
-A contributor's “essential patent claims” are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, “control” includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
-
-Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
-
-In the following three paragraphs, a “patent license” is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To “grant” such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
-
-If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. “Knowingly relying” means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
-
-If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
-
-A patent license is “discriminatory” if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
-
-Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
-12. No Surrender of Others' Freedom.
-
-If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
-13. Use with the GNU Affero General Public License.
-
-Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU Affero General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the special requirements of the GNU Affero General Public License, section 13, concerning interaction through a network will apply to the combination as such.
-14. Revised Versions of this License.
-
-The Free Software Foundation may publish revised and/or new versions of the GNU General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU General Public License “or any later version” applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU General Public License, you may choose any version ever published by the Free Software Foundation.
-
-If the Program specifies that a proxy can decide which future versions of the GNU General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
-
-Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
-15. Disclaimer of Warranty.
-
-THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM “AS IS” WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-16. Limitation of Liability.
-
-IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
-17. Interpretation of Sections 15 and 16.
-
-If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
-
-END OF TERMS AND CONDITIONS
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `muFFT-0.9.3/doc/CMakeLists.txt` & `mufft-0.90.0/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/MainSchema.png` & `mufft-0.90.0/doc/dev-docs/MainSchema.png`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/Makefile` & `mufft-0.90.0/doc/dev-docs/Makefile`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/logo_flat.png` & `mufft-0.90.0/doc/dev-docs/logo_flat.png`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/logo_square.png` & `mufft-0.90.0/doc/dev-docs/logo_square.png`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/source/CellSplit.rst` & `mufft-0.90.0/doc/dev-docs/source/CellSplit.rst`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/source/CodingConvention.rst` & `mufft-0.90.0/doc/dev-docs/source/CodingConvention.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1223,15 +1223,17 @@
 
 Definition:
   RTTI allows a programmer to query the C++ class of an object at run time. This is done by use of ``typeid`` or ``dynamic_cast``.
 
 Cons:
   Querying the type of an object at run-time frequently means a design problem. Needing to know the type of an object at runtime is often an indication that the design of your class hierarchy is flawed.
 
-  Undisciplined use of RTTI makes code hard to maintain. It can lead to type-based decision trees or switch statements scattered throughout the code, all of which must be examined when making further changes.
+  Undisciplined use of RTTI makes code hard to maintain. It can lead to type-based decision trees or switch statements scattered throughout the code, all of which must be examined when making further changes
+
+  RTTI is unreliable across shared library boundaries.
 
 Pros:
   RTTI can be very useful when interacting with duck-typed languages (like python) and when implementing efficient containers with polymorphic interfaces, see, e.g., *µ*\Spectre's ``FieldMap`` implementation.
 
   RTTI can be useful in some unit tests. For example, it is useful in tests of factory classes where the test has to verify that a newly created object has the expected dynamic type. It is also useful in managing the relationship between objects and their mocks.
 
   RTTI is useful when considering multiple abstract objects. Consider
```

### Comparing `muFFT-0.9.3/doc/dev-docs/source/ConstitutiveLaws.rst` & `mufft-0.90.0/doc/dev-docs/source/ConstitutiveLaws.rst`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/source/Doxyfile` & `mufft-0.90.0/doc/dev-docs/source/Doxyfile`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/source/GettingStarted.rst` & `mufft-0.90.0/doc/dev-docs/source/GettingStarted.rst`

 * *Files 13% similar despite different names*

```diff
@@ -15,45 +15,53 @@
 .. code-block:: bash
 
    $ git clone git@gitlab.com:muspectre/muspectre.git
 
 The latter option requires you to have a user account on gitlab (`create
 <https://gitlab.com/users/sign_in#register-pane>`_).
 
+Note that *µ*\Spectre uses submodules that need to be initialized with
+
+.. code-block:: bash
+
+   $ git submodule update --init
 
 .. _gitlab: https://gitlab.com
 
 
 Building *µ*\Spectre
 ********************
-You can compile *µ*\Spectre using `CMake <https://cmake.org/>`_ (3.5.0 or
-higher). 
+You can compile *µ*\Spectre using `Meson <https://mesonbuild.com/>`_
+(0.42.0 or higher) or `CMake <https://cmake.org/>`_ (3.5.0 or
+higher).
 
-Dependencies of *µ*\Spectre
- The current (and possibly incomplete list of) dependencies are
+The current (and possibly incomplete list of) dependencies are
 
-- `CMake <https://cmake.org/>`_ (3.5.0 or higher)
-- `Boost unit test framework <http://www.boost.org/doc/libs/1_66_0/libs/test/doc/html/index.html>`_
-- `FFTW <http://www.fftw.org>`_
+- `Meson <https://mesonbuild.com/>`_ (0.42.0 or higher) or `CMake <https://cmake.org/>`_ (3.5.0 or higher)
 - `git <https://git-scm.com/>`_
 - `Python3 <https://www.python.org/>`_ including the header files
 - `numpy <http://www.numpy.org/>`_ and `scipy <https://scipy.org/>`_
-- `UVW <https://c4science.ch/source/uvw/>`_ for the visualization
+- `UVW <https://c4science.ch/source/uvw/>`_ (0.3.1 or higher) for the visualization
+
+The following dependencies are included as submodules:
+
 - `pybind11 <https://pybind11.readthedocs.io/en/stable/>`_ (2.2.4 or higher)
-- `NetCDF4 <https://unidata.github.io/netcdf4-python/netCDF4/index.html>`_ 
+- `Eigen <http://eigen.tuxfamily.org/>`_ (3.3.0 or higher)
+
+The following dependencies are optional:
+
+- `Boost unit test framework <http://www.boost.org/doc/libs/1_66_0/libs/test/doc/html/index.html>`_
+- `FFTW <http://www.fftw.org>`_
+- `NetCDF4 <https://unidata.github.io/netcdf4-python/netCDF4/index.html>`_
 
 Recommended:
 
 - `Sphinx <http://www.sphinx-doc.org>`_ and `Breathe
   <https://breathe.readthedocs.io>`_ (necessary if you want to build the
   documentation (turned off by default)
-- `Eigen <http://eigen.tuxfamily.org/>`_ (3.3.0 or higher). If you do not
-  install this, it will be downloaded automatically at configuration time, so
-  this is not strictly necessary. The download can be slow, though, so we
-  recommend installing it on your system.
 - The CMake curses graphical user interface (``ccmake``).
 
 Possible compilers
  *µ*\Spectre requires a relatively modern compiler as it makes heavy use of C++14
  features. It has successfully been compiled and tested using the following
  compilers under Linux
 
@@ -62,22 +70,51 @@
 - gcc-5.4
 - clang-6.0
 - clang-5.0
 - clang-4.0
 
 and using clang-4.0 under MacOS.
 
+Under MacOS 14, it has been successfully compiled using gcc-6.5 shipped with homebrew along with the
+CommandLineTools 11.3.
+:download:`Here <macosx14_bash_profile>` is an example commented bash_profile that lead to the successful installation.
+
 It does *not* compile on Intel's most recent compiler, as it is still lacking
 some C++14 support. Work-arounds are planned, but will have to wait for someone
 to pick up the `task <https://gitlab.com/muspectre/muspectre/issues/93>`_.
 
-Instructions for compiling *µ*\Spectre
- To compile, go into the build folder and configure the CMake project. If you do
- this in the folder you cloned in the previous step, it can look for instance
- like this:
+Instructions for compiling *µ*\Spectre with Meson
+*************************************************
+
+To compile for *development*, i.e. with debug options turned on, first setup
+the build folder:
+
+.. code-block:: sh
+
+   $ meson setup meson-build-debug
+
+To compile for *production*, i.e. with code optimizations turned on, setup the
+build folder while specifying the `release` build type.
+
+.. code-block:: sh
+
+   $ meson setup --buildtype release meson-build-release
+
+The compilation is handled with `ninja`. Navigate to the build folder and run:
+
+.. code-block:: sh
+
+   $ ninja
+
+Instructions for compiling *µ*\Spectre with CMake
+*************************************************
+
+To compile, go into the build folder and configure the CMake project. If you do
+this in the folder you cloned in the previous step, it can look for instance
+like this:
 
 .. code-block:: sh
 
    $ cd build
    $ ccmake ..
 
 Then, set the build type to ``Release`` to produce optimised code. *µ*\Spectre
```

### Comparing `muFFT-0.9.3/doc/dev-docs/source/License.rst` & `mufft-0.90.0/doc/dev-docs/source/License.rst`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/source/MaterialLaminate.rst` & `mufft-0.90.0/doc/dev-docs/source/MaterialLaminate.rst`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/source/MaterialLinearElasticGeneric.rst` & `mufft-0.90.0/doc/dev-docs/source/MaterialLinearElasticGeneric.rst`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/source/NewMaterial.rst` & `mufft-0.90.0/doc/dev-docs/source/NewMaterial.rst`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/source/OrganisationOfCode.rst` & `mufft-0.90.0/doc/dev-docs/source/OrganisationOfCode.rst`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/source/Summary.rst` & `mufft-0.90.0/doc/summary.rmk`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,19 @@
-.. _Summary:
+Project µSpectre aims at providing an **open-source platform for efficient FFT-based continuum mesoscale modelling**. Please find the documentation on [[https://muspectre.gitlab.io/muspectre | gitlab pages]].
 
-Summary
--------
-
-Project *µ*\Spectre aims at providing an open-source platform for efficient FFT-based continuum mesoscale modelling. It's development is funded by the `Swiss National Science Foundation <snf.ch>`_ within an Ambizione Project.
-
-Computational continuum mesoscale modelling (or computational homogenisation) involves computing the overall response of a periodic unit cell of material, a so-called representative volume element (RVE), to a given average (i.e., macroscale) strain. Typically, this is done using the finite-element method, even though it is neither able to leverage its main strength, the trivial handling of complex geometries, nor otherwise particularly well suited for periodic problems. An alternative method for modelling periodic RVE, developed by `Moulinec and Suquet`_, is based on the fast Fourier transform (FFT). This method has evolved substantially over the last two decades, with particularly important and currently underused improvements in the last two years, see `Zeman et al`_, `de Geus et al`_.
+Computational continuum mesoscale modelling (or computational homogenisation) involves computing the overall response of a periodic unit cell of material, a so-called representative volume element (RVE), to a given average (i.e., macroscale) strain. Typically, this is done using the finite-element method, even though it is neither able to leverage its main strength, the trivial handling of complex geometries, nor otherwise particularly well suited for periodic problems. An alternative method for modelling periodic RVE, developed by Moulinec and Suquet [1], is based on the fast Fourier transform (FFT). This method has evolved substantially over the last two decades, with particularly important and currently underused improvements in the last two years, see Zeman et al [2].
 
 This new method for the solution of the core problem of computational homogenisation is significantly  superior to the FEM  in terms of computational cost and memory footprint for most applications, but has not been exploited to its full potential. One major obstacle to the wide adoption of the method is the lack of a robust, validated, open-source code. Hence, researchers choose the well-known and tested FEM that has numerous commercial, open-source or legacy in-house FEM codes.
 
-The goal of this project is to develop *µ*\Spectre, an open-source platform for efficient FFT-based continuum mesoscale modelling, which will overcome this obstacle. The project is designed to
+The goal of this project is to develop µSpectre, an open-source platform for efficient FFT-based continuum mesoscale modelling, which will overcome this obstacle. The project is designed to
 i)
 propose a de facto standard implementation for the spectral RVE method that subsequent implementations can be compared to, in order to concentrate the development effort of all interested parties in the field,
 ii)
-make *µ*\Spectre widely accessible for users by providing language bindings for virtually all relevant popular computing platforms and comprehensive user's manuals in order to help widespread adoption, and, finally
+make µSpectre widely accessible for users by providing language bindings for virtually all relevant popular computing platforms and comprehensive user's manuals in order to help widespread adoption, and, finally
 iv)
-make *µ*\Spectre eminently modifiable for developers by developing it in the open, with a clean architecture and extensive developer's documentation in order to maximise outside contributions.
-
-Furthermore, this project places great importance on truly reproducible and verifiable science with a credible open data strategy in the firm belief that these qualifiers help to reach and guarantee a high level of scientific quality, difficult to reach otherwise, and to attract outside collaborations and contributions that help boost the scientific output beyond what can be achieved by a single team.
-
-
-.. _`Moulinec and_Suquet` :
-
-`H. Moulinec and P. Suquet <https://doi.org/10.1016/S0045-7825(97)00218-1>`_. A numerical method for computing the overall response of nonlinear composites with complex microstructure. *Computer Methods in Applied Mechanics and Engineering*, 157(1):69–94, 1998. doi: 10.1016/S0045-7825(97) 00218-1.
-
-.. _`Zeman et al` :
-
-`J. Zeman, T. W. J. de Geus, J. Vondřejc, R. H. J. Peerlings, and M. G. D. Geers <https://dx.doi.org/10.1002/nme.5481>`_. A finite element perspective on non- linear FFT-based micromechanical simulations. *International Journal for Numerical Methods in Engineering*, 2017. doi: 10.1002/nme.5481.
+make µSpectre eminently modifiable for developers by developing it in the open, with a clean architecture and extensive developer's documentation in order to maximise outside contributions.
 
+Furthermore, this project places great importance on //truly reproducible and verifiable// science with a //credible open data strategy// in the firm belief that these qualifiers help to reach and guarantee a high level of scientific quality, difficult to reach otherwise, and to attract outside collaborations and contributions that help boost the scientific output beyond what can be achieved by a single team.
 
-.. _`de Geus et al` :
 
-`T.W.J. de Geus, J. Vondřejc, J. Zeman, R.H.J. Peerlings, M.G.D. Geers <https://doi.org/10.1016/j.cma.2016.12.032>`_. Finite strain FFT-based non-linear solvers made simple, *Computer Methods in Applied Mechanics and Engineering* (318, pp. 412-430), 2017
+[1] [[ https://doi.org/10.1016/S0045-7825(97)00218-1 | H. Moulinec and P. Suquet. A numerical method for computing the overall response of nonlinear composites with complex microstructure. //Computer Methods in Applied Mechanics and Engineering//, 157(1):69–94, 1998. doi: 10.1016/S0045-7825(97) 00218-1.]]
+[2] [[ https://dx.doi.org/10.1002/nme.5481 | J. Zeman, T. W. J. de Geus, J. Vondřejc, R. H. J. Peerlings, and M. G. D. Geers. A finite element perspective on non- linear FFT-based micromechanical simulations. //International Journal for Numerical Methods in Engineering//, 2017. doi: 10.1002/nme.5481. ]]
```

### Comparing `muFFT-0.9.3/doc/dev-docs/source/conf.py` & `mufft-0.90.0/doc/dev-docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/source/index.rst` & `mufft-0.90.0/doc/dev-docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/doc/dev-docs/source/muGrid.rst` & `mufft-0.90.0/doc/dev-docs/source/muGrid.rst`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,60 @@
 
 .. _mugrid:
 
 
 *µ*\Grid
 ########
 
-As the lowest-level component of *µ*\Spectre, *µ*\Grid defines all the commonly used type aliases and data structures used througout the project. The most common aliases are described below, but it is worth having a look at the file `grid_common.hh <https://gitlab.com/muspectre/muspectre/blob/master/src/libmugrid/grid_common.hh>`_ for the details.
+The *µ*\Grid library handles field quantities, i.e. scalar, vectors or tensors,
+that vary in space. It supports only a uniform discretization of space. In the
+language of *µ*\Grid, we call the discrete coordinates **pixels**. Each pixel
+can be subdivided into logical elements, for example into a number of
+support points for numerical quadrature. These subdivisions are called
+**sub-points**. Note that while *µ*\Grid can understand the physical location of
+each *pixel*, the *sub-points* are logical subdivisions and not associated
+with any position within the pixel. Each *sub-point* carries the field quantity,
+which can be a scalar, vector or any type of tensor. The field quantity is
+called the **component**.
+
+Each *µ*\Grid field has a representation in a multidimensional array. This
+representation is used when accessing a field with Python via *numpy* or when
+writing the field to a file. The default representation has the shape
+
+.. code-block:: Python
+
+    (components, sub-points, pixels)
+
+As a concrete example, a second-rank tensor (for example the deformation
+gradient) living on two quadrature points in three dimensions with a spatial
+discretization of 11 x 12 x 13 grid points would have the following shape:
+
+.. code-block:: Python
+
+    (3, 3, 2, 11, 12, 13)
+
+Note that the components are omitted if there is only a single component (i.e.
+a scalar value), but the sub-points are always included even if there is only
+a single sub-point. The default storage order of that representation is
+column-major.
+
+Throughout the code, we call the field quantities **entries**. For example,
+`nb_pixels` refers to the number of pixels while `nb_sub_pts` refers to the
+number of sub-points per pixel. `nb_entries` is then the product of the two.
 
 Common Type Aliases
 %%%%%%%%%%%%%%%%%%%
-All mathematical calculations should use the types.
+As the lowest-level component of *µ*\Spectre, *µ*\Grid defines all the commonly used type aliases and data structures used throuhgout the project. The most common aliases are described below, but it is worth having a look at the file `grid_common.hh <https://gitlab.com/muspectre/muspectre/blob/master/src/libmugrid/grid_common.hh>`_ for the details.
+
+All mathematical calculations should use these types.
 
 .. doxygengroup:: Scalars
    :members:
 
-While it is possible to use other types in principle, these are the ones for which all datastructures are tested and which are known to work. Also, other *µ*\Spectre developpers will expect and understand these types.
+While it is possible to use other types in principle, these are the ones for which all data structures are tested and which are known to work. Also, other *µ*\Spectre developers will expect and understand these types.
 
 Dimensions are counted using the signed integer type :cpp:type:`muGrid::Dim_t`. This is necessary because `Eigen <eigen.tuxfamily.org>`_ uses -1 to signify a dynamic number of dimensions.
 
 The types :cpp:type:`muGrid::Rcoord_t` and :cpp:type:`muGrid::Ccoord_t`  are used to represent real-valued coordinates and integer-valued coordinates (i.e., pixel- or cell-coordinates).
 
 .. doxygengroup:: Coordinates
    :members:
```

### Comparing `muFFT-0.9.3/doc/summary.rmk` & `mufft-0.90.0/doc/dev-docs/source/Summary.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,33 @@
-Project µSpectre aims at providing an **open-source platform for efficient FFT-based continuum mesoscale modelling**. It's development is funded by the [[ http://www.snf.ch/en | Swiss National Science Foundation ]] within an Ambizione Project. Please find the documentation on [[https://muspectre.gitlab.io/muspectre | gitlab pages]].
+.. _Summary:
 
-Computational continuum mesoscale modelling (or computational homogenisation) involves computing the overall response of a periodic unit cell of material, a so-called representative volume element (RVE), to a given average (i.e., macroscale) strain. Typically, this is done using the finite-element method, even though it is neither able to leverage its main strength, the trivial handling of complex geometries, nor otherwise particularly well suited for periodic problems. An alternative method for modelling periodic RVE, developed by Moulinec and Suquet [1], is based on the fast Fourier transform (FFT). This method has evolved substantially over the last two decades, with particularly important and currently underused improvements in the last two years, see Zeman et al [2].
+Summary
+-------
+
+Project *µ*\Spectre aims at providing an open-source platform for efficient FFT-based continuum mesoscale modelling. Its development is funded by the `Swiss National Science Foundation <https://snf.ch>`_ within an Ambizione Project and by the `European Research Council <https://erc.europa.eu>`_ within `Starting Grant 757343 <https://cordis.europa.eu/project/id/757343>`_.
+
+Computational continuum mesoscale modelling (or computational micromechanical homogenisation) involves computing the overall response of a periodic unit cell of material, a so-called representative volume element (RVE), to a given average (i.e., macroscale) strain. Typically, this is done using the finite-element method, even though it is neither able to leverage its main strength, the trivial handling of complex geometries, nor otherwise particularly well suited for periodic problems. An alternative method for modelling periodic RVE, developed by `Moulinec and Suquet`_, is based on the fast Fourier transform (FFT). This method has evolved substantially over the last two decades, with particularly important and currently underused improvements in the last two years, see `Zeman et al`_, `de Geus et al`_.
 
 This new method for the solution of the core problem of computational homogenisation is significantly  superior to the FEM  in terms of computational cost and memory footprint for most applications, but has not been exploited to its full potential. One major obstacle to the wide adoption of the method is the lack of a robust, validated, open-source code. Hence, researchers choose the well-known and tested FEM that has numerous commercial, open-source or legacy in-house FEM codes.
 
-The goal of this project is to develop µSpectre, an open-source platform for efficient FFT-based continuum mesoscale modelling, which will overcome this obstacle. The project is designed to
+The goal of this project is to develop *µ*\Spectre, an open-source platform for efficient FFT-based continuum mesoscale modelling, which will overcome this obstacle. The project is designed to
 i)
 propose a de facto standard implementation for the spectral RVE method that subsequent implementations can be compared to, in order to concentrate the development effort of all interested parties in the field,
 ii)
-make µSpectre widely accessible for users by providing language bindings for virtually all relevant popular computing platforms and comprehensive user's manuals in order to help widespread adoption, and, finally
+make *µ*\Spectre widely accessible for users by providing language bindings for virtually all relevant popular computing platforms and comprehensive user's manuals in order to help widespread adoption, and, finally
 iv)
-make µSpectre eminently modifiable for developers by developing it in the open, with a clean architecture and extensive developer's documentation in order to maximise outside contributions.
+make *µ*\Spectre eminently modifiable for developers by developing it in the open, with a clean architecture and extensive developer's documentation in order to maximise outside contributions.
+
+Furthermore, this project places great importance on truly reproducible and verifiable science with a credible open data strategy in the firm belief that these qualifiers help to reach and guarantee a high level of scientific quality, difficult to reach otherwise, and to attract outside collaborations and contributions that help boost the scientific output beyond what can be achieved by a single team.
+
+
+.. _`Moulinec and Suquet` :
+
+`H. Moulinec and P. Suquet <https://doi.org/10.1016/S0045-7825(97)00218-1>`_. A numerical method for computing the overall response of nonlinear composites with complex microstructure. *Computer Methods in Applied Mechanics and Engineering*, 157(1):69–94, 1998. doi: 10.1016/S0045-7825(97) 00218-1.
+
+.. _`Zeman et al` :
 
-Furthermore, this project places great importance on //truly reproducible and verifiable// science with a //credible open data strategy// in the firm belief that these qualifiers help to reach and guarantee a high level of scientific quality, difficult to reach otherwise, and to attract outside collaborations and contributions that help boost the scientific output beyond what can be achieved by a single team.
+`J. Zeman, T. W. J. de Geus, J. Vondřejc, R. H. J. Peerlings, and M. G. D. Geers <https://dx.doi.org/10.1002/nme.5481>`_. A finite element perspective on non- linear FFT-based micromechanical simulations. *International Journal for Numerical Methods in Engineering*, 2017. doi: 10.1002/nme.5481.
 
+.. _`de Geus et al` :
 
-[1] [[ https://doi.org/10.1016/S0045-7825(97)00218-1 | H. Moulinec and P. Suquet. A numerical method for computing the overall response of nonlinear composites with complex microstructure. //Computer Methods in Applied Mechanics and Engineering//, 157(1):69–94, 1998. doi: 10.1016/S0045-7825(97) 00218-1.]]
-[2] [[ https://dx.doi.org/10.1002/nme.5481 | J. Zeman, T. W. J. de Geus, J. Vondřejc, R. H. J. Peerlings, and M. G. D. Geers. A finite element perspective on non- linear FFT-based micromechanical simulations. //International Journal for Numerical Methods in Engineering//, 2017. doi: 10.1002/nme.5481. ]]
+`T.W.J. de Geus, J. Vondřejc, J. Zeman, R.H.J. Peerlings, M.G.D. Geers <https://doi.org/10.1016/j.cma.2016.12.032>`_. Finite strain FFT-based non-linear solvers made simple, *Computer Methods in Applied Mechanics and Engineering* (318, pp. 412-430), 2017
```

### Comparing `muFFT-0.9.3/language_bindings/CMakeLists.txt` & `mufft-0.90.0/tests/python_mpi_binding_tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,46 @@
-#==============================================================================
-# file   CMakeLists.txt
-#
-# @author Till Junge <till.junge@epfl.ch>
-#
-# @date   08 Jan 2018
-#
-# @brief  configuration for language bindings
-#
-# @section LICENSE
-#
-# Copyright © 2018 Till Junge
-#
-# µSpectre is free software; you can redistribute it and/or
-# modify it under the terms of the GNU Lesser General Public License as
-# published by the Free Software Foundation, either version 3, or (at
-# your option) any later version.
-#
-# µSpectre is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
-# General Public License for more details.
-#
-# You should have received a copy of the GNU Lesser General Public License
-# along with µSpectre; see the file COPYING. If not, write to the
-# Free Software Foundation, Inc., 59 Temple Place - Suite 330,
-# Boston, MA 02111-1307, USA.
-#
-# Additional permission under GNU GPL version 3 section 7
-#
-# If you modify this Program, or any covered work, by linking or combining it
-# with proprietary FFT implementations or numerical libraries, containing parts
-# covered by the terms of those libraries' licenses, the licensors of this
-# Program grant you additional permission to convey the resulting work.
-# =============================================================================
-
-add_subdirectory(libmugrid)
-add_subdirectory(libmufft)
-add_subdirectory(python)
+#!/usr/bin/env python3
+# -*- coding:utf-8 -*-
+"""
+@file   python_mpi_binding_tests.py
+
+@author Till Junge <till.junge@epfl.ch>
+
+@date   28 Feb 2019
+
+@brief  Unit tests for python bindings with MPI support
+
+Copyright © 2019 Till Junge
+
+µFFT is free software; you can redistribute it and/or
+modify it under the terms of the GNU Lesser General Public License as
+published by the Free Software Foundation, either version 3, or (at
+your option) any later version.
+
+µFFT is distributed in the hope that it will be useful, but
+WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License
+along with µFFT; see the file COPYING. If not, write to the
+Free Software Foundation, Inc., 59 Temple Place - Suite 330,
+Boston, MA 02111-1307, USA.
+
+Additional permission under GNU GPL version 3 section 7
+
+If you modify this Program, or any covered work, by linking or combining it
+with proprietary FFT implementations or numerical libraries, containing parts
+covered by the terms of those libraries' licenses, the licensors of this
+Program grant you additional permission to convey the resulting work.
+"""
+
+import unittest
+import numpy as np
+
+import muFFT
+
+from python_fft_tests import FFT_Check
+#from python_netcdf_tests import NetCDF_Check_2d, NetCDF_Check_3d
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `muFFT-0.9.3/language_bindings/libmufft/CMakeLists.txt` & `mufft-0.90.0/tests/mpi_main_test_suite.cc`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,44 @@
-#==============================================================================
-# file   CMakeLists.txt
-#
-# @author Till Junge <till.junge@epfl.ch>
-#
-# @date   08 Jan 2018
-#
-# @brief  configuration for language bindings
-#
-# @section LICENSE
-#
-# Copyright © 2018 Till Junge
-#
-# µSpectre is free software; you can redistribute it and/or
-# modify it under the terms of the GNU Lesser General Public License as
-# published by the Free Software Foundation, either version 3, or (at
-# your option) any later version.
-#
-# µSpectre is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
-# General Public License for more details.
-#
-# You should have received a copy of the GNU Lesser General Public License
-# along with µSpectre; see the file COPYING. If not, write to the
-# Free Software Foundation, Inc., 59 Temple Place - Suite 330,
-# Boston, MA 02111-1307, USA.
-#
-# Additional permission under GNU GPL version 3 section 7
-#
-# If you modify this Program, or any covered work, by linking or combining it
-# with proprietary FFT implementations or numerical libraries, containing parts
-# covered by the terms of those libraries' licenses, the licensors of this
-# Program grant you additional permission to convey the resulting work.
-# =============================================================================
+/**
+ * @file   mpi_main_test_suite.cc
+ *
+ * @author Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
+ *
+ * @date   07 Mar 2018
+ *
+ * @brief  Main test suite for MPI specific modules. Running this suite tests
+ *         all available tests for µSpectre that depend on MPI.
+ *
+ * Copyright © 2017 Till Junge
+ *
+ * µFFT is free software; you can redistribute it and/or
+ * modify it under the terms of the GNU Lesser General Public License as
+ * published by the Free Software Foundation, either version 3, or (at
+ * your option) any later version.
+ *
+ * µFFT is distributed in the hope that it will be useful, but
+ * WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+ * Lesser General Public License for more details.
+ *
+ * You should have received a copy of the GNU Lesser General Public License
+ * along with µFFT; see the file COPYING. If not, write to the
+ * Free Software Foundation, Inc., 59 Temple Place - Suite 330,
+ * * Boston, MA 02111-1307, USA.
+ *
+ * Additional permission under GNU GPL version 3 section 7
+ *
+ * If you modify this Program, or any covered work, by linking or combining it
+ * with proprietary FFT implementations or numerical libraries, containing parts
+ * covered by the terms of those libraries' licenses, the licensors of this
+ * Program grant you additional permission to convey the resulting work.
+ *
+ */
+#define BOOST_TEST_MODULE base_test test
+#define BOOST_TEST_MAIN
 
-add_subdirectory(python)
+// Meson defines this properly, CMake does not
+#ifndef BOOST_TEST_DYN_LINK
+#define BOOST_TEST_DYN_LINK
+#endif
+
+#include <boost/test/unit_test.hpp>
```

### Comparing `muFFT-0.9.3/language_bindings/libmufft/python/bind_py_common.cc` & `mufft-0.90.0/language_bindings/python/bind_py_common_mufft.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * @file   bind_py_common.cc
+ * @file   bind_py_common_mufft.cc
  *
  * @author Till Junge <till.junge@epfl.ch>
  *
  * @date   08 Jan 2018
  *
  * @brief  Python bindings for the common part of µFFT
  *
@@ -29,24 +29,23 @@
  * If you modify this Program, or any covered work, by linking or combining it
  * with proprietary FFT implementations or numerical libraries, containing parts
  * covered by the terms of those libraries' licenses, the licensors of this
  * Program grant you additional permission to convey the resulting work.
  *
  */
 
-#include "libmufft/fft_utils.hh"
-#include "libmufft/mufft_common.hh"
+#include <libmufft/fft_utils.hh>
+#include <libmufft/mufft_common.hh>
 
 #include <libmugrid/ccoord_operations.hh>
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/eigen.h>
 
-
 namespace py = pybind11;
 using pybind11::literals::operator""_a;
 
 void add_version(py::module & mod) {
   auto version{mod.def_submodule("version")};
 
   version.doc() = "version information";
@@ -127,15 +126,15 @@
 
 void add_fft_freqs(py::module & mod) {
   add_fft_freqs_helper<muGrid::oneD>(mod);
   add_fft_freqs_helper<muGrid::twoD>(mod);
   add_fft_freqs_helper<muGrid::threeD>(mod);
 }
 
-void add_common(py::module & mod) {
+void add_common_mufft(py::module & mod) {
   add_version(mod);
   py::enum_<muFFT::FFT_PlanFlags>(mod, "FFT_PlanFlags")
       .value("estimate", muFFT::FFT_PlanFlags::estimate)
       .value("measure", muFFT::FFT_PlanFlags::measure)
       .value("patient", muFFT::FFT_PlanFlags::patient);
 
   add_get_nb_hermitian(mod);
```

### Comparing `muFFT-0.9.3/language_bindings/libmufft/python/bind_py_declarations.hh` & `mufft-0.90.0/language_bindings/python/bind_py_declarations.hh`

 * *Files 9% similar despite different names*

```diff
@@ -35,13 +35,12 @@
 
 #ifndef LANGUAGE_BINDINGS_LIBMUFFT_PYTHON_BIND_PY_DECLARATIONS_HH_
 #define LANGUAGE_BINDINGS_LIBMUFFT_PYTHON_BIND_PY_DECLARATIONS_HH_
 
 #include <pybind11/pybind11.h>
 namespace py = pybind11;
 
-void add_common(py::module & mod);
-void add_communicator(py::module & mod);
+void add_common_mufft(py::module & mod);
 void add_derivatives(py::module & mod);
 void add_fft_engines(py::module & mod);
 
 #endif  // LANGUAGE_BINDINGS_LIBMUFFT_PYTHON_BIND_PY_DECLARATIONS_HH_
```

### Comparing `muFFT-0.9.3/language_bindings/libmufft/python/bind_py_derivatives.cc` & `mufft-0.90.0/language_bindings/python/bind_py_derivatives.cc`

 * *Files 23% similar despite different names*

```diff
@@ -36,25 +36,31 @@
 #include <memory>
 #include <sstream>
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/eigen.h>
 
-#include "libmufft/derivative.hh"
+#include <libmugrid/ccoord_operations.hh>
+#include <libmugrid/numpy_tools.hh>
+
+#include <libmufft/derivative.hh>
+#include <libmufft/fft_engine_base.hh>
 
 using muFFT::DerivativeBase;
 using muFFT::DiscreteDerivative;
 using muFFT::FourierDerivative;
 using muGrid::Complex;
 using muGrid::DynCcoord_t;
 using muGrid::Index_t;
 using muGrid::Real;
 using muGrid::threeD;
 using muGrid::twoD;
+using muGrid::NumpyProxy;
+using muFFT::FFTEngineBase;
 using pybind11::literals::operator""_a;
 namespace py = pybind11;
 
 /**
  * "Trampoline" class for handling the pure virtual methods, see
  * [http://pybind11.readthedocs.io/en/stable/advanced/classes.html#overriding-virtual-functions-in-python]
  * for details
@@ -87,15 +93,15 @@
           "fourier",
           [](DerivativeBase & derivative,
              py::array_t<Real, py::array::f_style> wavevectors) {
             py::buffer_info wavevectors_buffer = wavevectors.request();
             std::vector<ssize_t> output_shape;
             // The first dimension contains the components of The wavevector.
             // This is equal to the dimension of space.
-            ssize_t nb_dof_per_sub_pt{wavevectors_buffer.shape[0]};
+            ssize_t nb_components{wavevectors_buffer.shape[0]};
             // The next dimensions simply hold entries and we don't care about
             // the shape. The return array should have the same shape, minus
             // the first dimension.
             ssize_t nb_entries = 1;
             for (int i = 1; i < wavevectors_buffer.ndim; ++i) {
               output_shape.push_back(wavevectors_buffer.shape[i]);
               nb_entries *= wavevectors_buffer.shape[i];
@@ -104,16 +110,16 @@
             py::array_t<Complex, py::array::f_style> factors(output_shape);
             py::buffer_info factors_buffer = factors.request();
             // Loop over all entries and call fourier method.
             auto wavevector = static_cast<const Real *>(wavevectors_buffer.ptr);
             for (ssize_t i = 0; i < nb_entries; ++i) {
               static_cast<Complex *>(factors_buffer.ptr)[i] =
                   derivative.fourier(Eigen::Map<const DerivativeBase::Vector>(
-                      wavevector, nb_dof_per_sub_pt));
-              wavevector += nb_dof_per_sub_pt;
+                      wavevector, nb_components));
+              wavevector += nb_components;
             }
             return factors;
           },
           "wavevectors"_a,
           "return Fourier representation of the derivative operator for a "
           "certain wavevector");
 }
@@ -166,16 +172,53 @@
                nb_pts[i] = info.shape[i];
              }
              return new DiscreteDerivative(
                  nb_pts, lbounds,
                  Eigen::Map<Eigen::ArrayXd>(static_cast<double *>(info.ptr),
                                             info.size));
            }),
-           "lbounds"_a, "stencil"_a)
+           "lbounds"_a, "stencil"_a,
+           "Constructor with raw stencil information\n"
+           "nb_pts: stencil size\n"
+           "lbounds: relative starting point of stencil, e.g. (-2,) means\n"
+           "         that the stencil start two pixels to the left of where\n"
+           "         the derivative should be computed\n"
+           "stencil: stencil coefficients")
       .def("rollaxes", &DiscreteDerivative::rollaxes, "distance"_a = 1)
+      .def("apply", &DiscreteDerivative::apply<Real>, "in_field"_a, "in_dof"_a,
+           "out_field"_a, "out_dof"_a, "fac"_a = 1.0)
+    .def_property_readonly("lbounds", &DiscreteDerivative::get_lbounds)
+    .def(
+         "apply",
+         [](const DiscreteDerivative & self,
+            py::array_t<Real, py::array::f_style> & input_array) {
+           const py::buffer_info & info = input_array.request();
+           if (info.ndim != self.get_dim()) {
+             std::stringstream s;
+             s << "Stencil is " << self.get_dim() << "-dimensional, "
+               << "but the input array is " << input_array.ndim()
+               << "-dimensional.";
+             throw muGrid::RuntimeError(s.str());
+           }
+           py::array_t<double, py::array::f_style> output_array(info.shape);
+           DynCcoord_t nb_domain_grid_pts{info.shape};
+           DynCcoord_t subdomain_locations(info.ndim);
+           NumpyProxy<Real, py::array::f_style> input_proxy(
+                nb_domain_grid_pts, nb_domain_grid_pts,
+                subdomain_locations, 1, input_array);
+           NumpyProxy<Real, py::array::f_style> output_proxy(
+               nb_domain_grid_pts, nb_domain_grid_pts,
+               subdomain_locations, 1, output_array);
+
+           self.apply(input_proxy.get_field(), 0, output_proxy.get_field(), 0);
+           return output_array;
+         },
+         "input_array"_a,
+         "Apply the discrete derivative stencil to the input array.")
+
       .def_property_readonly("stencil", [](const DiscreteDerivative & self) {
         const Eigen::ArrayXd & stencil = self.get_stencil();
         return py::array_t<double, py::array::f_style>(self.get_nb_pts(),
                                                        stencil.data());
       });
 }
```

### Comparing `muFFT-0.9.3/language_bindings/libmufft/python/bind_py_module.cc` & `mufft-0.90.0/language_bindings/python/bind_py_module.cc`

 * *Files 4% similar despite different names*

```diff
@@ -36,12 +36,11 @@
 #include "bind_py_declarations.hh"
 
 #include <pybind11/pybind11.h>
 
 PYBIND11_MODULE(_muFFT, mod) {
   mod.doc() = "Python bindings to the µFFT library";
 
-  add_common(mod);
-  add_communicator(mod);
+  add_common_mufft(mod);
   add_derivatives(mod);
   add_fft_engines(mod);
 }
```

### Comparing `muFFT-0.9.3/language_bindings/libmufft/python/bind_py_version.cc.skeleton` & `mufft-0.90.0/language_bindings/python/bind_py_version.cc.skeleton`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/language_bindings/libmufft/python/muFFT/NetCDF.py` & `mufft-0.90.0/language_bindings/python/muFFT/NetCDF.py`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/language_bindings/libmufft/python/muFFT/Stencils2D.py` & `mufft-0.90.0/language_bindings/python/muFFT/Stencils1D.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 """
-@file   Stencils2D.py
+@file   Stencils1D.py
 
 @author Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
 
-@date   15 May 2020
+@date   15 Nov 2020
 
-@brief  Library of some common stencils for 2D problems
+@brief  Library of some common stencils for 1D problems
 
 Copyright © 2018 Till Junge
 
 µFFT is free software; you can redistribute it and/or
 modify it under the terms of the GNU Lesser General Public License as
 published by the Free Software Foundation, either version 3, or (at
 your option) any later version.
@@ -33,30 +33,18 @@
 covered by the terms of those libraries' licenses, the licensors of this
 Program grant you additional permission to convey the resulting work.
 """
 
 import muFFT
 
 # First order upwind differences
-upwind_x = muFFT.DiscreteDerivative([0, 0], [[-1], [1]])
-upwind_y = muFFT.DiscreteDerivative([0, 0], [[-1, 1]])
-upwind = (upwind_x, upwind_y)
-
-# d-stencil label the corners used for the derivative
-d_10_00 = upwind_x
-d_01_00 = upwind_y
-d_11_01 = muFFT.DiscreteDerivative([0, 0], [[0, -1],
-                                            [0,  1]])
-d_11_10 = muFFT.DiscreteDerivative([0, 0], [[ 0, 0],
-                                            [-1, 1]])
-
-# First order upwind differences, averaged over neighboring pixels
-averaged_upwind_x = muFFT.DiscreteDerivative([0, 0], [[-0.5, -0.5],
-                                                      [ 0.5,  0.5]])
-averaged_upwind_y = muFFT.DiscreteDerivative([0, 0], [[-0.5, 0.5],
-                                                      [-0.5, 0.5]])
-averaged_upwind = (averaged_upwind_x, averaged_upwind_y)
+upwind = muFFT.DiscreteDerivative([0], [-1, 1])
 
 # Second order central differences
-central_x = muFFT.DiscreteDerivative([-1, 0], [[-0.5], [0], [0.5]])
-central_y = muFFT.DiscreteDerivative([0, -1], [[-0.5, 0, 0.5]])
-central = (central_x, central_y)
+central = muFFT.DiscreteDerivative([-1], [-0.5, 0, 0.5])
+
+# Sixth order central differences
+central6 = muFFT.DiscreteDerivative([-3],
+                                    [-1/60, 3/20, -3/4, 0, 3/4, -3/20, 1/60])
+
+# Fourth order central differences of the second derivative
+central_2nd = muFFT.DiscreteDerivative([-1], [1, -2, 1])
```

### Comparing `muFFT-0.9.3/language_bindings/libmugrid/CMakeLists.txt` & `mufft-0.90.0/tests/tests.hh`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,60 @@
-#==============================================================================
-# file     CMakeLists.txt
-#
-# @author  Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
-#
-# @date    10 Oct 2019
-#
-# @brief   configuration for language bindings
-#
-# @section LICENSE
-#
-# Copyright © 2018 Till Junge
-#
-# µSpectre is free software; you can redistribute it and/or
-# modify it under the terms of the GNU Lesser General Public License as
-# published by the Free Software Foundation, either version 3, or (at
-# your option) any later version.
-#
-# µSpectre is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
-# General Public License for more details.
-#
-# You should have received a copy of the GNU Lesser General Public License
-# along with µSpectre; see the file COPYING. If not, write to the
-# Free Software Foundation, Inc., 59 Temple Place - Suite 330,
-# Boston, MA 02111-1307, USA.
-#
-# Additional permission under GNU GPL version 3 section 7
-#
-# If you modify this Program, or any covered work, by linking or combining it
-# with proprietary FFT implementations or numerical libraries, containing parts
-# covered by the terms of those libraries' licenses, the licensors of this
-# Program grant you additional permission to convey the resulting work.
-# =============================================================================
+/**
+ * @file   tests.hh
+ *
+ * @author Till Junge <till.junge@epfl.ch>
+ *
+ * @date   10 May 2017
+ *
+ * @brief  common defs for tests
+ *
+ * Copyright © 2017 Till Junge
+ *
+ * µFFT is free software; you can redistribute it and/or
+ * modify it under the terms of the GNU Lesser General Public License as
+ * published by the Free Software Foundation, either version 3, or (at
+ * your option) any later version.
+ *
+ * µFFT is distributed in the hope that it will be useful, but
+ * WITHOUT ANY WARRANTY; without even the implied warranty of
+ * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
+ * Lesser General Public License for more details.
+ *
+ * You should have received a copy of the GNU Lesser General Public License
+ * along with µFFT; see the file COPYING. If not, write to the
+ * Free Software Foundation, Inc., 59 Temple Place - Suite 330,
+ * * Boston, MA 02111-1307, USA.
+ *
+ * Additional permission under GNU GPL version 3 section 7
+ *
+ * If you modify this Program, or any covered work, by linking or combining it
+ * with proprietary FFT implementations or numerical libraries, containing parts
+ * covered by the terms of those libraries' licenses, the licensors of this
+ * Program grant you additional permission to convey the resulting work.
+ *
+ */
 
-add_subdirectory(python)
+#include <libmufft/mufft_common.hh>
+
+#include <boost/test/unit_test.hpp>
+#include <boost/mpl/list.hpp>
+
+#ifndef TESTS_LIBMUFFT_TESTS_HH_
+#define TESTS_LIBMUFFT_TESTS_HH_
+
+namespace muFFT {
+
+  constexpr Real tol = 1e-14 * 100;       // it's in percent
+  constexpr Real finite_diff_tol = 1e-7;  // it's in percent
+
+}  // namespace muFFT
+
+template <muFFT::Dim_t Dim>
+struct dimFixture {
+  constexpr static muFFT::Dim_t dim{Dim};
+};
+
+using dimlist =
+    boost::mpl::list<dimFixture<muFFT::oneD>, dimFixture<muFFT::twoD>,
+                     dimFixture<muFFT::threeD>>;
+
+#endif  // TESTS_LIBMUFFT_TESTS_HH_
```

### Comparing `muFFT-0.9.3/language_bindings/libmugrid/python/bind_py_declarations.hh` & `mufft-0.90.0/tests/main_test_suite.cc`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 /**
- * @file   bind_py_declarations.hh
+ * @file   main_test_suite.cc
  *
- * @author Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
+ * @author Till Junge <till.junge@epfl.ch>
  *
- * @date   10 Oct 2019
+ * @date   01 May 2017
  *
- * @brief  header for python bindings for the common part of µGrid
+ * @brief  Main test suite. Running this suite tests all available tests for
+ *         µSpectre
  *
- * Copyright © 2018 Till Junge
+ * Copyright © 2017 Till Junge
  *
- * µGrid is free software; you can redistribute it and/or
+ * µFFT is free software; you can redistribute it and/or
  * modify it under the terms of the GNU Lesser General Public License as
  * published by the Free Software Foundation, either version 3, or (at
  * your option) any later version.
  *
- * µGrid is distributed in the hope that it will be useful, but
+ * µFFT is distributed in the hope that it will be useful, but
  * WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
  * Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with µGrid; see the file COPYING. If not, write to the
+ * along with µFFT; see the file COPYING. If not, write to the
  * Free Software Foundation, Inc., 59 Temple Place - Suite 330,
  * * Boston, MA 02111-1307, USA.
  *
  * Additional permission under GNU GPL version 3 section 7
  *
  * If you modify this Program, or any covered work, by linking or combining it
  * with proprietary FFT implementations or numerical libraries, containing parts
  * covered by the terms of those libraries' licenses, the licensors of this
  * Program grant you additional permission to convey the resulting work.
  *
  */
+#define BOOST_TEST_MODULE base_test test
+#define BOOST_TEST_MAIN
 
-#ifndef LANGUAGE_BINDINGS_LIBMUGRID_PYTHON_BIND_PY_DECLARATIONS_HH_
-#define LANGUAGE_BINDINGS_LIBMUGRID_PYTHON_BIND_PY_DECLARATIONS_HH_
+// Meson defines this properly, CMake does not
+#ifndef BOOST_TEST_DYN_LINK
+#define BOOST_TEST_DYN_LINK
+#endif
 
-#include <pybind11/pybind11.h>
-namespace py = pybind11;
-
-void add_common(py::module & mod);
-void add_field_classes(py::module & mod);
-void add_field_collection_classes(py::module & mod);
-
-#endif  // LANGUAGE_BINDINGS_LIBMUGRID_PYTHON_BIND_PY_DECLARATIONS_HH_
+#include <boost/test/unit_test.hpp>
```

### Comparing `muFFT-0.9.3/language_bindings/libmugrid/python/muGrid/__init__.py` & `mufft-0.90.0/tests/python_binding_tests.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 """
-@file   __init__.py
+@file   python_binding_tests.py
 
-@author Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
+@author Till Junge <till.junge@epfl.ch>
 
-@date   10 Oct 2019
+@date   09 Jan 2018
 
-@brief  Main entry point for muGrid Python module
+@brief  Unit tests for python bindings
 
 Copyright © 2018 Till Junge
 
-µGrid is free software; you can redistribute it and/or
+µFFT is free software; you can redistribute it and/or
 modify it under the terms of the GNU Lesser General Public License as
 published by the Free Software Foundation, either version 3, or (at
 your option) any later version.
 
-µGrid is distributed in the hope that it will be useful, but
+µFFT is distributed in the hope that it will be useful, but
 WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
-along with µGrid; see the file COPYING. If not, write to the
+along with µFFT; see the file COPYING. If not, write to the
 Free Software Foundation, Inc., 59 Temple Place - Suite 330,
 Boston, MA 02111-1307, USA.
 
 Additional permission under GNU GPL version 3 section 7
 
 If you modify this Program, or any covered work, by linking or combining it
 with proprietary FFT implementations or numerical libraries, containing parts
 covered by the terms of those libraries' licenses, the licensors of this
 Program grant you additional permission to convey the resulting work.
 """
 
+import unittest
 import numpy as np
 
-import _muGrid
-from _muGrid import (get_domain_ccoord, get_domain_index, Pixel, SubPt,
-                     DynCcoord, DynRcoord, IterUnit, Verbosity,
-                     GlobalFieldCollection, LocalFieldCollection, Unit)
+import muFFT
 
+from python_derivative_tests import DerivativeCheck2d, DerivativeCheck3d
+from python_fft_tests import FFT_Check
+try:  # netCDF became unmaintanable in ubuntu 16.04, but the tests stay until IO is replaced
+    from python_netcdf_tests import NetCDF_Check_2d, NetCDF_Check_3d
+except Exception:
+    pass
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `muFFT-0.9.3/language_bindings/python/bind_py_material_hyper_elasto_plastic1.cc` & `mufft-0.90.0/src/libmufft/version.cc`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,74 @@
 /**
- * @file   bind_py_material_hyper_elasto_plastic1.cc
+ * @file   version.cc
  *
- * @author Till Junge <till.junge@altermail.ch>
+ * @author Till Junge <till.junge@epfl.ch>
  *
- * @date   29 Oct 2018
+ * @date   04 Feb 2020
  *
- * @brief  python binding for MaterialHyperElastoPlastic1
+ * @brief  File written at compile time containing git state
  *
- * Copyright © 2018 Till Junge
+ * Copyright © 2020 Till Junge
  *
- * µSpectre is free software; you can redistribute it and/or
+ * µFFT is free software; you can redistribute it and/or
  * modify it under the terms of the GNU Lesser General Public License as
  * published by the Free Software Foundation, either version 3, or (at
  * your option) any later version.
  *
- * µSpectre is distributed in the hope that it will be useful, but
+ * µFFT is distributed in the hope that it will be useful, but
  * WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
  * Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with µSpectre; see the file COPYING. If not, write to the
+ * along with µFFT; see the file COPYING. If not, write to the
  * Free Software Foundation, Inc., 59 Temple Place - Suite 330,
  * Boston, MA 02111-1307, USA.
  *
  * Additional permission under GNU GPL version 3 section 7
  *
  * If you modify this Program, or any covered work, by linking or combining it
  * with proprietary FFT implementations or numerical libraries, containing parts
  * covered by the terms of those libraries' licenses, the licensors of this
  * Program grant you additional permission to convey the resulting work.
  *
  */
 
-#include "common/muSpectre_common.hh"
-#include "materials/stress_transformations_Kirchhoff.hh"
-#include "materials/material_hyper_elasto_plastic1.hh"
-#include "cell/cell.hh"
-
-#include <pybind11/pybind11.h>
-#include <pybind11/stl.h>
-#include <pybind11/eigen.h>
 
-#include <sstream>
 #include <string>
+#include <sstream>
 
-using muSpectre::Index_t;
-using muSpectre::Real;
-using pybind11::literals::operator""_a;
-namespace py = pybind11;
+#include "libmugrid/grid_common.hh"
 
-/**
- * python binding for the optionally objective form of Hooke's law
- * with per-pixel elastic properties
- */
-template <Index_t Dim>
-void add_material_hyper_elasto_plastic1_helper(py::module & mod) {
-  std::stringstream name_stream{};
-  name_stream << "MaterialHyperElastoPlastic1_" << Dim << "d";
-  const auto name{name_stream.str()};
-
-  using Mat_t = muSpectre::MaterialHyperElastoPlastic1<Dim>;
-  using Cell_t = muSpectre::Cell;
-
-  py::class_<Mat_t, muSpectre::MaterialBase, std::shared_ptr<Mat_t>>(
-      mod, name.c_str())
-      .def_static(
-          "make",
-          [](Cell_t & cell, std::string name, Real Young, Real Poisson,
-             Real tau_y0, Real h) -> Mat_t & {
-            return Mat_t::make(cell, name, Young, Poisson, tau_y0, h);
-          },
-          "cell"_a, "name"_a, "YoungModulus"_a, "PoissonRatio"_a, "τ_y₀"_a,
-          "h"_a, py::return_value_policy::reference_internal)
-      .def_static(
-          "make_evaluator",
-          [](Real Young, Real Poisson, Real tau_y0, Real h) {
-            return Mat_t::make_evaluator(Young, Poisson, tau_y0, h);
-          },
-          "YoungModulus"_a, "PoissonRatio"_a, "τ_y₀"_a, "h"_a);
-}
-
-template void
-add_material_hyper_elasto_plastic1_helper<muSpectre::twoD>(py::module &);
-template void
-add_material_hyper_elasto_plastic1_helper<muSpectre::threeD>(py::module &);
+namespace muFFT {
+  namespace version {
+
+    /* Presently, version informations is inherited from muGrid. If the
+     * repositories are split sometime in the future, this need to be created
+     * via CMake. */
+
+    //------------------------------------------------------------------------//
+    std::string info() {
+      std::stringstream info_str{};
+      info_str << "µFFT version: " << muGrid::version::description()
+               << std::endl;
+      if (muGrid::version::is_dirty()) {
+        info_str << "WARNING: state is dirty, you will not be able to recover "
+                    "the state of the µFFT sources used to compile me from "
+                    "this info!"
+                 << std::endl;
+      }
+      return info_str.str();
+    }
+
+    //------------------------------------------------------------------------//
+    const char * hash() { return muGrid::version::hash(); }
+
+    //------------------------------------------------------------------------//
+    const char * description() { return muGrid::version::description(); }
+
+    //------------------------------------------------------------------------//
+    bool is_dirty() { return muGrid::version::is_dirty(); }
+
+  }  // namespace version
+
+}  // namespace muFFT
```

### Comparing `muFFT-0.9.3/src/cell/cell_split.hh` & `mufft-0.90.0/src/libmufft/fftwmpi_engine.hh`

 * *Files 24% similar despite different names*

```diff
@@ -1,221 +1,161 @@
 /**
- * @file   cell_split.hh
+ * @file   fftwmpi_engine.hh
  *
- * @author Ali Falsafi <ali.falsafi@epfl.ch>
+ * @author Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
  *
- * @date   10 Dec 2019
+ * @date   06 Mar 2017
  *
- * @brief Base class representing a unit cell able to handle
- *        split material assignments
+ * @brief  FFT engine using MPI-parallel FFTW
  *
  * Copyright © 2017 Till Junge
  *
- * µSpectre is free software; you can redistribute it and/or
+ * µFFT is free software; you can redistribute it and/or
  * modify it under the terms of the GNU Lesser General Public License as
  * published by the Free Software Foundation, either version 3, or (at
  * your option) any later version.
  *
- * µSpectre is distributed in the hope that it will be useful, but
+ * µFFT is distributed in the hope that it will be useful, but
  * WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
  * Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with µSpectre; see the file COPYING. If not, write to the
+ * along with µFFT; see the file COPYING. If not, write to the
  * Free Software Foundation, Inc., 59 Temple Place - Suite 330,
- * Boston, MA 02111-1307, USA.
+ * * Boston, MA 02111-1307, USA.
  *
  * Additional permission under GNU GPL version 3 section 7
  *
  * If you modify this Program, or any covered work, by linking or combining it
  * with proprietary FFT implementations or numerical libraries, containing parts
  * covered by the terms of those libraries' licenses, the licensors of this
  * Program grant you additional permission to convey the resulting work.
  *
  */
 
-#ifndef SRC_CELL_CELL_SPLIT_HH_
-#define SRC_CELL_CELL_SPLIT_HH_
+#ifndef SRC_LIBMUFFT_FFTWMPI_ENGINE_HH_
+#define SRC_LIBMUFFT_FFTWMPI_ENGINE_HH_
 
-#include "cell/cell.hh"
+#include "fft_engine_base.hh"
 
-#include "common/muSpectre_common.hh"
-#include "common/intersection_octree.hh"
-#include "materials/material_base.hh"
-#include "projection/projection_base.hh"
-
-#include "libmugrid/ccoord_operations.hh"
-#include "libmugrid/field.hh"
-
-#include <vector>
-#include <memory>
-#include <tuple>
-#include <functional>
-#include <sstream>
-#include <algorithm>
-
-namespace muSpectre {
-
-  //! DimS spatial dimension (dimension of problem
-  //! DimM material_dimension (dimension of constitutive law)
-  /* This class handles the cells that has
-     splitly assigned material to their pixels */
-  class CellSplit : public Cell {
-    friend class Cell;
+#include <fftw3-mpi.h>
 
-   public:
-    using Parent = Cell;  //!< base class
-
-    //! projections handled through `std::unique_ptr`s
-    using Projection_ptr = std::unique_ptr<ProjectionBase>;
-
-    //! combined stress and tangent field
-    using FullResponse_t =
-        std::tuple<const muGrid::RealField &, const muGrid::RealField &>;
+namespace muFFT {
 
+  /**
+   * implements the `muFFT::FFTEngineBase` interface using the
+   * FFTW library
+   */
+  class FFTWMPIEngine : public FFTEngineBase {
+   public:
+    using Parent = FFTEngineBase;  //!< base class
+    //! field for Fourier transform of second-order tensor
+    using FourierField_t = typename Parent::FourierField_t;
+    //! real-valued second-order tensor
+    using RealField_t = typename Parent::RealField_t;
     //! Default constructor
-    CellSplit() = delete;
+    FFTWMPIEngine() = delete;
 
-    //! constructor using sizes and resolution
-    explicit CellSplit(Projection_ptr projection);
+    /**
+     * Constructor with the domain's number of grid points in each direction and
+     * the communicator
+     * @param nb_grid_pts number of grid points of the global grid
+     * @param comm MPI communicator object
+     * @param plan_flags MPI planner flags
+     * @param allow_temporary_buffer allow the creation of temporary buffers
+     *        if the input buffer has the wrong memory layout
+     * @param allow_destroy_input allow that the input buffers are invalidated
+     *        during the FFT
+     */
+    FFTWMPIEngine(const DynCcoord_t & nb_grid_pts,
+                  Communicator comm = Communicator(),
+                  const FFT_PlanFlags & plan_flags = FFT_PlanFlags::estimate,
+                  bool allow_temporary_buffer = true,
+                  bool allow_destroy_input = false);
 
     //! Copy constructor
-    CellSplit(const CellSplit & other) = delete;
+    FFTWMPIEngine(const FFTWMPIEngine & other) = delete;
 
     //! Move constructor
-    CellSplit(CellSplit && other) = default;
+    FFTWMPIEngine(FFTWMPIEngine && other) = delete;
 
     //! Destructor
-    virtual ~CellSplit() = default;
+    virtual ~FFTWMPIEngine() noexcept;
 
     //! Copy assignment operator
-    CellSplit & operator=(const CellSplit & other) = delete;
+    FFTWMPIEngine & operator=(const FFTWMPIEngine & other) = delete;
 
     //! Move assignment operator
-    CellSplit & operator=(CellSplit && other) = delete;
+    FFTWMPIEngine & operator=(FFTWMPIEngine && other) = delete;
 
-    /**
-     * add a new material to the cell
-     */
-    MaterialBase & add_material(Material_ptr mat) final;
+    // compute the plan, etc
+    void create_plan(const Index_t & nb_dof_per_pixel) override;
 
     /**
-     *completes the assignmnet of material with a specific material so
-     *all the under-assigned pixels would be assigned to a material.
+     * return whether this engine is active (an engine is active if it has more
+     * than zero grid points. FFTWMPI sometimes assigns zero grid points)
      */
+    bool has_grid_pts() const override { return this->active; }
 
-    void complete_material_assignment(MaterialBase & material);
-
-    // returns the assigend ratios to each pixel
-    std::vector<Real> get_assigned_ratios();
-
-    // Assigns pixels according to the coordiantes of the
-    // precipitate
-    void make_automatic_precipitate_split_pixels(
-        const std::vector<DynRcoord_t> & preciptiate_vertices,
-        MaterialBase & material);
-
-    // Returns the unassigend portion of the pixels whose material
-    // assignemnt are not complete
-    std::vector<Real> get_unassigned_ratios_incomplete_pixels() const;
-
-    // This function returns the index of the pixels whose material
-    // assignemnt are not complete
-    std::vector<Index_t> get_index_incomplete_pixels() const;
-
-    // This function returns the Ccoord of the pixels whose material
-    // assignemnt are not complete
-    std::vector<DynCcoord_t> get_unassigned_pixels();
-
-    // this class is designed to handle the pixels with incomplete material
-    // assignment and itereating over them
-    class IncompletePixels {
-     public:
-      //! constructor
-      explicit IncompletePixels(const CellSplit & cell);
-      //! copy constructor
-      IncompletePixels(const IncompletePixels & other) = default;
-      //! move constructor
-      IncompletePixels(IncompletePixels & other) = default;
-      // Deconstructor
-      virtual ~IncompletePixels() = default;
-
-      //! iterator type over all incompletetedly assigned pixel's
-      class iterator {
-       public:
-        using value_type = std::tuple<DynCcoord_t, Real>;  //!< stl conformance
-
-        //! constructor
-        iterator(const IncompletePixels & pixels, Index_t dim,
-                 bool begin = true);
-
-        // deconstructor
-        virtual ~iterator() = default;
-
-        //! dereferencing
-        value_type operator*() const;
-
-        template <Index_t DimS>
-        value_type deref_helper() const;
+    //! perform a deep copy of the engine (this should never be necessary in
+    //! c++)
+    std::unique_ptr<FFTEngineBase> clone() const final;
 
-        //! pre-increment
-        iterator & operator++();
-
-        //! inequality
-        bool operator!=(const iterator & other);
-
-        //! equality
-        inline bool operator==(const iterator & other) const;
-
-       protected:
-        const IncompletePixels & incomplete_pixels;
-        Index_t dim;
-        size_t index;
-      };
-
-      //! stl conformance
-      inline iterator begin() const {
-        return iterator(*this, this->cell.get_spatial_dim());
-      }
-
-      //! stl conformance
-      inline iterator end() const {
-        return iterator(*this, this->cell.get_spatial_dim(), false);
-      }
-
-      //! stl conformance
-      inline size_t size() const {
-        return muGrid::CcoordOps::get_size(
-            this->cell.projection->get_nb_subdomain_grid_pts());
-      }
-
-     protected:
-      const CellSplit & cell;
-      std::vector<Real> incomplete_assigned_ratios;
-      std::vector<Index_t> index_incomplete_pixels;
-    };
-
-    IncompletePixels make_incomplete_pixels();
+    /**
+     * need to override this method here, since FFTWMPI requires field padding
+     */
+    RealField_t &
+    register_real_space_field(const std::string & unique_name,
+                              const Index_t & nb_dof_per_pixel) final;
 
-    //! makes sure every pixel has been assigned to materials whose ratios add
-    //! up to 1.0
-    void check_material_coverage() const final;
+    /**
+     * need to override this method here, since FFTWMPI requires field padding
+     */
+    RealField_t &
+    register_real_space_field(const std::string & unique_name,
+                              const Shape_t & shape) final;
 
-    // full resppnse is composed of the stresses and tangent matrix
-    const muGrid::RealField & evaluate_stress() final;
+    /**
+     * need to override this method here, since FFTWMPI requires field padding
+     */
+    muGrid::ComplexField &
+    register_fourier_space_field(const std::string & unique_name,
+                                 const Index_t & nb_dof_per_pixel) final;
 
-    // stress and the tangent of the response of the cell_split
-    std::tuple<const muGrid::RealField &, const muGrid::RealField &>
-    evaluate_stress_tangent() final;
+    /**
+     * need to override this method here, since FFTWMPI requires field padding
+     */
+    muGrid::ComplexField &
+    register_fourier_space_field(const std::string & unique_name,
+                                 const Shape_t & shape) final;
 
    protected:
-    // this function make the initial magnitude of the
-    // stress and stiffness tensors to zero
-    void set_p_k_zero();
-
-   private:
+    //! forward transform
+    void compute_fft(const RealField_t & field,
+                     FourierField_t & output_field) override;
+
+    //! inverse transform
+    void compute_ifft(const FourierField_t & input_field,
+                      RealField_t & output_field) override;
+
+    //! check whether real-space buffer has the correct memory layout
+    bool check_real_space_field(const RealField_t & field) const final;
+
+    //! check whether Fourier-space buffer has the correct memory layout
+    bool check_fourier_space_field(const FourierField_t & field) const final;
+
+    static int nb_engines;  //!< number of times this engine has
+                            //!< been instantiated
+    //! holds the plans for forward fourier transforms
+    std::map<Index_t, fftw_plan> fft_plans{};
+    //! holds the plans for inversefourier transforms
+    std::map<Index_t, fftw_plan> ifft_plans{};
+    //! holds the fourier field sizes including padding for different transforms
+    std::map<Index_t, Index_t> required_workspace_sizes{};
+    bool active{true};  //!< FFTWMPI sometimes assigns zero grid points
+    //! Input to local_size_many_transposed
+    std::vector<ptrdiff_t> nb_fourier_non_transposed{};
   };
+}  // namespace muFFT
 
-}  // namespace muSpectre
-
-#endif  // SRC_CELL_CELL_SPLIT_HH_
+#endif  // SRC_LIBMUFFT_FFTWMPI_ENGINE_HH_
```

### Comparing `muFFT-0.9.3/src/libmufft/derivative.cc` & `mufft-0.90.0/src/libmufft/derivative.cc`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/src/libmufft/derivative.hh` & `mufft-0.90.0/src/libmufft/derivative.hh`

 * *Files 5% similar despite different names*

```diff
@@ -35,19 +35,19 @@
  */
 
 #ifndef SRC_LIBMUFFT_DERIVATIVE_HH_
 #define SRC_LIBMUFFT_DERIVATIVE_HH_
 
 #include <memory>
 
-#include <libmugrid/ccoord_operations.hh>
-#include <libmugrid/exception.hh>
-#include <libmugrid/field_map.hh>
-#include <libmugrid/field_typed.hh>
-#include <libmugrid/field_collection_global.hh>
+#include "libmugrid/ccoord_operations.hh"
+#include "libmugrid/exception.hh"
+#include "libmugrid/field_map.hh"
+#include "libmugrid/field_typed.hh"
+#include "libmugrid/field_collection_global.hh"
 
 #include "mufft_common.hh"
 
 namespace muFFT {
   /**
    * base class for projection related exceptions
    */
@@ -166,15 +166,17 @@
 
     //! Default constructor
     DiscreteDerivative() = delete;
 
     /**
      * Constructor with raw stencil information
      * @param nb_pts: stencil size
-     * @param lbounds: relative starting point of stencil
+     * @param lbounds: relative starting point of stencil, e.g. (-2,) means
+     * that the stencil start two pixels to the left of where the derivative
+     * should be computed
      * @param stencil: stencil coefficients
      */
     DiscreteDerivative(DynCcoord_t nb_pts, DynCcoord_t lbounds,
                        const std::vector<Real> & stencil);
 
     //! Constructor with raw stencil information
     DiscreteDerivative(DynCcoord_t nb_pts, DynCcoord_t lbounds,
@@ -196,14 +198,19 @@
     DiscreteDerivative & operator=(DiscreteDerivative && other) = delete;
 
     //! Return stencil value
     Real operator()(const DynCcoord_t & dcoord) const {
       return this->stencil[this->pixels.get_index(dcoord)];
     }
 
+    //! Return dimension of the stencil
+    const Dim_t & get_dim() const {
+      return this->pixels.get_dim();
+    }
+
     //! Return number of grid points in stencil
     const DynCcoord_t & get_nb_pts() const {
       return this->pixels.get_nb_subdomain_grid_pts();
     }
 
     //! Return lower stencil bound
     const DynCcoord_t & get_lbounds() const {
@@ -221,16 +228,16 @@
      * compiler should have opportunity to inline this function to optimize
      * loops over DOFs.
      * TODO: This presently only works *without* MPI parallelization! If you
      * need parallelization, apply the stencil in Fourier space using the
      * `fourier` method. Currently this method is only used in the serial tests.
      */
     template <typename T>
-    void apply(const muGrid::TypedField<T> & in_field, Index_t in_dof,
-               muGrid::TypedField<T> & out_field, Index_t out_dof,
+    void apply(const muGrid::TypedFieldBase<T> & in_field, Index_t in_dof,
+               muGrid::TypedFieldBase<T> & out_field, Index_t out_dof,
                Real fac = 1.0) const {
       // check whether fields are global
       if (!in_field.is_global()) {
         throw DerivativeError("Input field must be a global field.");
       }
       if (!out_field.is_global()) {
         throw DerivativeError("Output field must be a global field.");
```

### Comparing `muFFT-0.9.3/src/libmufft/fft_utils.cc` & `mufft-0.90.0/src/libmufft/fft_utils.cc`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/src/libmufft/fft_utils.hh` & `mufft-0.90.0/src/libmufft/fft_utils.hh`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
  * Program grant you additional permission to convey the resulting work.
  *
  */
 
 #ifndef SRC_LIBMUFFT_FFT_UTILS_HH_
 #define SRC_LIBMUFFT_FFT_UTILS_HH_
 
-#include <libmugrid/exception.hh>
+#include "libmugrid/exception.hh"
 
 #include "mufft_common.hh"
 
-#include <Eigen/Dense>
+#include "Eigen/Dense"
 
 #include <array>
 #include <valarray>
 
 namespace muFFT {
 
   namespace internal {
```

### Comparing `muFFT-0.9.3/src/libmufft/fftw_engine.cc` & `mufft-0.90.0/src/libmufft/fftw_engine.cc`

 * *Files 17% similar despite different names*

```diff
@@ -31,31 +31,41 @@
  * covered by the terms of those libraries' licenses, the licensors of this
  * Program grant you additional permission to convey the resulting work.
  *
  */
 
 #include <sstream>
 
-#include <libmugrid/ccoord_operations.hh>
-#include <libmugrid/exception.hh>
+#include "libmugrid/ccoord_operations.hh"
+#include "libmugrid/exception.hh"
 
 #include "fftw_engine.hh"
 
 namespace muFFT {
 
-  FFTWEngine::FFTWEngine(const DynCcoord_t & nb_grid_pts, Communicator comm)
-      : Parent{nb_grid_pts, comm} {
-    this->fourier_field_collection.initialise(this->nb_fourier_grid_pts,
-                                              this->fourier_locations,
-                                              this->fourier_strides);
+  FFTWEngine::FFTWEngine(const DynCcoord_t & nb_grid_pts, Communicator comm,
+                         const FFT_PlanFlags & plan_flags,
+                         bool allow_temporary_buffer, bool allow_destroy_input)
+      : Parent{nb_grid_pts, comm, plan_flags, allow_temporary_buffer,
+               allow_destroy_input} {
+    this->initialise_field_collections();
+    ++this->nb_engines;
   }
 
   /* ---------------------------------------------------------------------- */
-  void FFTWEngine::initialise(const Index_t & nb_dof_per_pixel,
-                              const FFT_PlanFlags & plan_flags) {
+  FFTWEngine::FFTWEngine(const DynCcoord_t & nb_grid_pts,
+                         const FFT_PlanFlags & plan_flags,
+                         bool allow_temporary_buffer, bool allow_destroy_input)
+      : FFTWEngine{nb_grid_pts, Communicator(), plan_flags,
+                   allow_temporary_buffer, allow_destroy_input} {
+    ++this->nb_engines;
+  }
+
+  /* ---------------------------------------------------------------------- */
+  void FFTWEngine::create_plan(const Index_t & nb_dof_per_pixel) {
     if (this->has_plan_for(nb_dof_per_pixel)) {
       // plan already exists, we can bail
       return;
     }
     if (this->comm.size() > 1) {
       std::stringstream error;
       error << "FFTW engine does not support MPI parallel execution, but a "
@@ -73,33 +83,39 @@
     }
     const int * const n{&narr[0]};
     int howmany{static_cast<int>(nb_dof_per_pixel)};
     // temporary buffer for plan
     size_t alloc_size{muGrid::CcoordOps::get_size(this->nb_subdomain_grid_pts) *
                       howmany};
     Real * r_work_space{fftw_alloc_real(alloc_size)};
+    if (r_work_space == nullptr) {
+      throw FFTEngineError("'r_work_space' allocation failed");
+    }
     Real * in{r_work_space};
     // nembed are tricky: they refer to physical layout
     const int * const inembed{nullptr};
     int istride{howmany};
     int idist{1};
     auto && nb_fft_pts{[](const DynCcoord_t & grid_pts) {
       int retval{1};
       for (auto && nb : grid_pts) {
         retval *= nb;
       }
       return retval;
     }(this->get_nb_fourier_grid_pts())};
     fftw_complex * out{fftw_alloc_complex(howmany * nb_fft_pts)};
+    if (out == nullptr) {
+      throw FFTEngineError("'out' allocation failed");
+    }
     const int * const onembed{nullptr};
     int ostride{istride};
     int odist{idist};
 
     unsigned int flags;
-    switch (plan_flags) {
+    switch (this->plan_flags) {
     case FFT_PlanFlags::estimate: {
       flags = FFTW_ESTIMATE;
       break;
     }
     case FFT_PlanFlags::measure: {
       flags = FFTW_MEASURE;
       break;
@@ -111,142 +127,139 @@
     default:
       throw FFTEngineError("unknown planner flag type");
       break;
     }
 
     this->fft_plans[nb_dof_per_pixel] = fftw_plan_many_dft_r2c(
         rank, n, howmany, in, inembed, istride, idist, out, onembed, ostride,
-        odist, FFTW_PRESERVE_INPUT | flags);
+        odist,
+        (this->allow_destroy_input ? FFTW_DESTROY_INPUT : FFTW_PRESERVE_INPUT) |
+            flags);
     if (this->fft_plans.at(nb_dof_per_pixel) == nullptr) {
       throw FFTEngineError("Plan failed");
     }
 
-    fftw_complex * i_in {out};
-    Real * i_out {r_work_space};
+    fftw_complex * i_in{out};
+    Real * i_out{r_work_space};
 
     this->ifft_plans[nb_dof_per_pixel] =
         fftw_plan_many_dft_c2r(rank, n, howmany, i_in, inembed, istride, idist,
                                i_out, onembed, ostride, odist, flags);
 
     if (this->ifft_plans.at(nb_dof_per_pixel) == nullptr) {
       throw FFTEngineError("Plan failed");
     }
+
+    // r2hc_plans
+
+    Real * r_work_space_2{fftw_alloc_real(alloc_size)};
+    if (r_work_space_2 == nullptr) {
+      throw FFTEngineError("'r_work_space_2' allocation failed");
+    }
+    Real * r2hc_out{r_work_space_2};
+
+    std::vector<fftw_r2r_kind> fft_kinds(rank);
+    for (auto && k : fft_kinds) {
+      k = FFTW_R2HC;
+    }
+    std::vector<fftw_r2r_kind> ifft_kinds(rank);
+    for (auto && k : ifft_kinds) {
+      k = FFTW_HC2R;
+    }
+
+    this->hcfft_plans[nb_dof_per_pixel] = fftw_plan_many_r2r(
+        rank, n, howmany, in, inembed, istride, idist, r2hc_out, onembed,
+        ostride, odist, fft_kinds.data(),
+        (this->allow_destroy_input ? FFTW_DESTROY_INPUT : FFTW_PRESERVE_INPUT) |
+            flags);
+    if (this->hcfft_plans.at(nb_dof_per_pixel) == nullptr) {
+      throw FFTEngineError("Plan failed");
+    }
+
+    Real * ir2hc_in{r_work_space_2};
+    this->ihcfft_plans[nb_dof_per_pixel] = fftw_plan_many_r2r(
+        rank, n, howmany, ir2hc_in, inembed, istride, idist, i_out, onembed,
+        ostride, odist, ifft_kinds.data(), flags);
+
+    if (this->ihcfft_plans.at(nb_dof_per_pixel) == nullptr) {
+      throw FFTEngineError("Plan failed");
+    }
+
     fftw_free(r_work_space);
+    fftw_free(r_work_space_2);
     fftw_free(out);
     this->planned_nb_dofs.insert(nb_dof_per_pixel);
   }
 
   /* ---------------------------------------------------------------------- */
   FFTWEngine::~FFTWEngine() noexcept {
     for (auto && nb_dof_per_pixel : this->planned_nb_dofs) {
       auto && fft_plan{this->fft_plans.at(nb_dof_per_pixel)};
-      if (fft_plan != nullptr)
+      if (fft_plan != nullptr) {
         fftw_destroy_plan(fft_plan);
+      }
       auto && ifft_plan{this->ifft_plans.at(nb_dof_per_pixel)};
-      if (ifft_plan != nullptr)
+      if (ifft_plan != nullptr) {
         fftw_destroy_plan(ifft_plan);
+      }
+      auto && hcfft_plan{this->hcfft_plans.at(nb_dof_per_pixel)};
+      if (hcfft_plan != nullptr) {
+        fftw_destroy_plan(hcfft_plan);
+      }
+      auto && ihcfft_plan{this->ihcfft_plans.at(nb_dof_per_pixel)};
+      if (ihcfft_plan != nullptr) {
+        fftw_destroy_plan(ihcfft_plan);
+      }
+    }
+    --this->nb_engines;
+    if (this->nb_engines == 0) {
+      // TODO(Pastewka): Check with Lars why this crashes the sequential(!) MPI
+      // tests
+#ifndef WITH_MPI
+       fftw_cleanup();
+#endif
     }
-    // TODO(Till): We cannot run fftw_cleanup since subsequent FFTW calls will
-    // fail but multiple FFT engines can be active at the same time.
-    // fftw_cleanup();
   }
 
   /* ---------------------------------------------------------------------- */
-  void FFTWEngine::fft(const RealField_t & input_field,
-                       FourierField_t & output_field) const {
-    auto && nb_dofs_per_pixel{input_field.get_nb_dof_per_pixel()};
-    if (not this->has_plan_for(nb_dofs_per_pixel)) {
-      std::stringstream message{};
-      message << "No plan has been created for " << nb_dofs_per_pixel
-              << " degrees of freedom per pixel. Use "
-                 "`muFFT::FFTEngineBase::initialise` to prepare a plan.";
-      throw FFTEngineError{message.str()};
-    }
-    if (static_cast<size_t>(input_field.get_nb_pixels()) !=
-        muGrid::CcoordOps::get_size(this->nb_subdomain_grid_pts)) {
-      std::stringstream error{};
-      error << "The number of pixels of the field '" << input_field.get_name()
-            << "' passed to the forward FFT is " << input_field.get_nb_pixels()
-            << " and does not match the size "
-            << muGrid::CcoordOps::get_size(this->nb_subdomain_grid_pts)
-            << " of the (sub)domain handled by FFTWEngine.";
-      throw FFTEngineError(error.str());
-    }
-    if (static_cast<size_t>(output_field.get_nb_pixels()) !=
-        muGrid::CcoordOps::get_size(this->nb_fourier_grid_pts)) {
-      std::stringstream error{};
-      error << "The number of pixels of the field '" << output_field.get_name()
-            << "' passed to the forward FFT is " << output_field.get_nb_pixels()
-            << " and does not match the size "
-            << muGrid::CcoordOps::get_size(this->nb_fourier_grid_pts)
-            << " of the (sub)domain handled by FFTWEngine.";
-      throw FFTEngineError(error.str());
-    }
-    if (input_field.get_nb_dof_per_sub_pt() * input_field.get_nb_sub_pts() !=
-        input_field.get_nb_dof_per_sub_pt() * input_field.get_nb_sub_pts()) {
-      std::stringstream error;
-      error << "The input field reports " << input_field.get_nb_dof_per_sub_pt()
-            << " components per sub-point and " << input_field.get_nb_sub_pts()
-            << " sub-points, while the output field reports "
-            << output_field.get_nb_dof_per_sub_pt()
-            << " components per sub-point and " << output_field.get_nb_sub_pts()
-            << " sub-points.";
-      throw FFTEngineError(error.str());
-    }
-    fftw_execute_dft_r2c(this->fft_plans.at(nb_dofs_per_pixel),
+  void FFTWEngine::compute_fft(const RealField_t & input_field,
+                               FourierField_t & output_field) {
+    fftw_execute_dft_r2c(this->fft_plans.at(input_field.get_nb_dof_per_pixel()),
                          input_field.data(),
                          reinterpret_cast<fftw_complex *>(output_field.data()));
   }
 
   /* ---------------------------------------------------------------------- */
-  void FFTWEngine::ifft(const FourierField_t & input_field,
-                        RealField_t & output_field) const {
-    auto && nb_dofs_per_pixel{input_field.get_nb_dof_per_pixel()};
-    if (not this->has_plan_for(nb_dofs_per_pixel)) {
-      std::stringstream message{};
-      message << "No plan has been created for " << nb_dofs_per_pixel
-              << " degrees of freedom per pixel. Use "
-                 "`muFFT::FFTEngineBase::initialise` to prepare a plan.";
-      throw FFTEngineError{message.str()};
-    }
-    if (static_cast<size_t>(input_field.get_nb_pixels()) !=
-        muGrid::CcoordOps::get_size(this->nb_fourier_grid_pts)) {
-      std::stringstream error;
-      error << "The number of pixels of the field '" << input_field.get_name()
-            << "' passed to the inverse FFT is " << input_field.get_nb_pixels()
-            << " and does not match the size "
-            << muGrid::CcoordOps::get_size(this->nb_fourier_grid_pts)
-            << " of the (sub)domain handled by FFTWEngine.";
-      throw FFTEngineError(error.str());
-    }
-    if (static_cast<size_t>(output_field.get_nb_pixels()) !=
-        muGrid::CcoordOps::get_size(this->nb_subdomain_grid_pts)) {
-      std::stringstream error;
-      error << "The number of pixels of the field '" << output_field.get_name()
-            << "' passed to the inverse FFT is " << output_field.get_nb_pixels()
-            << " and does not match the size "
-            << muGrid::CcoordOps::get_size(this->nb_subdomain_grid_pts)
-            << " of the (sub)domain handled by FFTWEngine.";
-      throw FFTEngineError(error.str());
-    }
-    if (input_field.get_nb_dof_per_sub_pt() * input_field.get_nb_sub_pts() !=
-        output_field.get_nb_dof_per_sub_pt() * output_field.get_nb_sub_pts()) {
-      std::stringstream error;
-      error << "The input field reports " << input_field.get_nb_dof_per_sub_pt()
-            << " components per sub-point and " << input_field.get_nb_sub_pts()
-            << " sub-points, while the output field reports "
-            << output_field.get_nb_dof_per_sub_pt()
-            << " components per sub-point and " << output_field.get_nb_sub_pts()
-            << " sub-points.";
-      throw FFTEngineError(error.str());
-    }
-    fftw_execute_dft_c2r(this->ifft_plans.at(nb_dofs_per_pixel),
-                         reinterpret_cast<fftw_complex *>(input_field.data()),
-                         output_field.data());
+  void FFTWEngine::compute_ifft(const FourierField_t & input_field,
+                                RealField_t & output_field) {
+    fftw_execute_dft_c2r(
+        this->ifft_plans.at(input_field.get_nb_dof_per_pixel()),
+        reinterpret_cast<fftw_complex *>(input_field.data()),
+        output_field.data());
+  }
+
+  /* ---------------------------------------------------------------------- */
+  void FFTWEngine::compute_hcfft(const RealField_t & input_field,
+                                 RealField_t & output_field) {
+    fftw_execute_r2r(this->hcfft_plans.at(input_field.get_nb_dof_per_pixel()),
+                     input_field.data(), output_field.data());
   }
 
+  /* ---------------------------------------------------------------------- */
+  void FFTWEngine::compute_ihcfft(const RealField_t & input_field,
+                                  RealField_t & output_field) {
+    fftw_execute_r2r(this->ihcfft_plans.at(input_field.get_nb_dof_per_pixel()),
+                     input_field.data(), output_field.data());
+  }
+
+  /* ---------------------------------------------------------------------- */
   std::unique_ptr<FFTEngineBase> FFTWEngine::clone() const {
-    return std::make_unique<FFTWEngine>(this->get_nb_domain_grid_pts(),
-                                        this->get_communicator());
+    return std::make_unique<FFTWEngine>(
+        this->get_nb_domain_grid_pts(), this->get_communicator(),
+        this->plan_flags, this->allow_temporary_buffer,
+        this->allow_destroy_input);
   }
 
+  /* ---------------------------------------------------------------------- */
+  Index_t FFTWEngine::nb_engines{0};
+
 }  // namespace muFFT
```

### Comparing `muFFT-0.9.3/src/libmufft/fftw_engine.hh` & `mufft-0.90.0/src/libmufft/fftw_engine.hh`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 /**
  * @file   fftw_engine.hh
  *
  * @author Till Junge <till.junge@altermail.ch>
  *
  * @date   03 Dec 2017
  *
@@ -53,19 +54,42 @@
     using FourierField_t = typename Parent::FourierField_t;
     //! real-valued second-order tensor
     using RealField_t = typename Parent::RealField_t;
     //! Default constructor
     FFTWEngine() = delete;
 
     /**
-     * Constructor with the domain's number of grid points in each direciton,
-     * the number of components to transform, and the communicator
+     * Constructor with the domain's number of grid points in each direction,
+     * the communicator, and fft planner flags
+     * @param nb_grid_pts number of grid points of the global grid
+     * @param allow_temporary_buffer allow the creation of temporary buffers
+     *        if the input buffer has the wrong memory layout
+     * @param allow_destroy_input allow that the input buffers are invalidated
+     *        during the FFT
+     * @comm MPI communicator object
+     */
+    FFTWEngine(const DynCcoord_t & nb_grid_pts,
+               Communicator comm = Communicator(),
+               const FFT_PlanFlags & plan_flags = FFT_PlanFlags::estimate,
+               bool allow_temporary_buffer = true,
+               bool allow_destroy_input = false);
+    /**
+     * Constructor with the domain's number of grid points in each direction and
+     * the fft planner flags
+     * @param nb_grid_pts number of grid points of the global grid
+     * @param allow_temporary_buffer allow the creation of temporary buffers
+     *        if the input buffer has the wrong memory layout
+     * @param allow_destroy_input allow that the input buffers are invalidated
+     *        during the FFT
+     * @comm MPI communicator object
      */
     FFTWEngine(const DynCcoord_t & nb_grid_pts,
-               Communicator comm = Communicator());
+               const FFT_PlanFlags & plan_flags,
+               bool allow_temporary_buffer = true,
+               bool allow_destroy_input = false);
 
     //! Copy constructor
     FFTWEngine(const FFTWEngine & other) = delete;
 
     //! Move constructor
     FFTWEngine(FFTWEngine && other) = delete;
 
@@ -75,32 +99,47 @@
     //! Copy assignment operator
     FFTWEngine & operator=(const FFTWEngine & other) = delete;
 
     //! Move assignment operator
     FFTWEngine & operator=(FFTWEngine && other) = delete;
 
     // compute the plan, etc
-    void initialise(const Index_t & nb_dof_per_pixel,
-                    const FFT_PlanFlags & plan_flags) override;
-
-    //! forward transform
-    void fft(const RealField_t & input_field,
-             FourierField_t & output_field) const override;
-
-    //! inverse transform
-    void ifft(const FourierField_t & input_field,
-              RealField_t & output_field) const override;
+    void create_plan(const Index_t & nb_dof_per_pixel) override;
 
     //! perform a deep copy of the engine (this should never be necessary in
     //! c++)
     std::unique_ptr<FFTEngineBase> clone() const final;
 
    protected:
+    //! forward transform
+    void compute_fft(const RealField_t & input_field,
+                     FourierField_t & output_field) override;
+
+    //! inverse transform
+    void compute_ifft(const FourierField_t & input_field,
+                      RealField_t & output_field) override;
+
+    //! forward half complex transform
+    void compute_hcfft(const RealField_t & input_field,
+                 RealField_t & output_field) override;
+
+    //! inverse half complex transform
+    void compute_ihcfft(const RealField_t & input_field,
+                      RealField_t & output_field) override;
+
     //! holds the plans for forward fourier transforms
     std::map<Index_t, fftw_plan> fft_plans{};
     //! holds the plans for inversefourier transforms
     std::map<Index_t, fftw_plan> ifft_plans{};
+
+    //! holds the plans for forward half-complex fourier transforms
+    std::map<Index_t, fftw_plan> hcfft_plans{};
+
+    //! holds the plans for inverse half-complex fourier transforms
+    std::map<Index_t, fftw_plan> ihcfft_plans{};
+
+    static Index_t nb_engines;
   };
 
 }  // namespace muFFT
 
 #endif  // SRC_LIBMUFFT_FFTW_ENGINE_HH_
```

### Comparing `muFFT-0.9.3/src/libmufft/fftwmpi_engine.cc` & `mufft-0.90.0/src/libmufft/pfft_engine.cc`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /**
- * @file   fftwmpi_engine.cc
+ * @file   pfft_engine.cc
  *
  * @author Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
  *
  * @date   06 Mar 2017
  *
- * @brief  implements the MPI-parallel fftw engine
+ * @brief  implements the MPI-parallel pfft engine
  *
  * Copyright © 2017 Till Junge
  *
  * µFFT is free software; you can redistribute it and/or
  * modify it under the terms of the GNU Lesser General Public License as
  * published by the Free Software Foundation, either version 3, or (at
  * your option) any later version.
@@ -29,435 +29,338 @@
  * If you modify this Program, or any covered work, by linking or combining it
  * with proprietary FFT implementations or numerical libraries, containing parts
  * covered by the terms of those libraries' licenses, the licensors of this
  * Program grant you additional permission to convey the resulting work.
  *
  */
 
-#include <libmugrid/ccoord_operations.hh>
-#include <libmugrid/exception.hh>
+#include "libmugrid/ccoord_operations.hh"
+#include "libmugrid/exception.hh"
 
-#include "fftwmpi_engine.hh"
+#include "pfft_engine.hh"
 
-#include "fft_utils.hh"
+using muGrid::CcoordOps::get_col_major_strides;
 
 namespace muFFT {
 
-  int FFTWMPIEngine::nb_engines{0};
+  int PFFTEngine::nb_engines{0};
 
-  FFTWMPIEngine::FFTWMPIEngine(const DynCcoord_t & nb_grid_pts,
-                               Communicator comm)
-      : Parent{nb_grid_pts, comm} {
-    if (!this->nb_engines) {
-      fftw_mpi_init();
-    }
+  PFFTEngine::PFFTEngine(const DynCcoord_t & nb_grid_pts,
+                         Communicator comm,
+                         const FFT_PlanFlags & plan_flags,
+                         bool allow_temporary_buffer,
+                         bool allow_destroy_input)
+      : Parent{nb_grid_pts, comm, plan_flags, allow_temporary_buffer,
+               allow_destroy_input}, mpi_comm{comm.get_mpi_comm()} {
+    if (!this->nb_engines)
+      pfft_init();
     this->nb_engines++;
 
+    int size{comm.size()};
+    int dim_x{size};
+    int dim_y{1};
     const int dim{this->nb_fourier_grid_pts.get_dim()};
-    this->nb_fourier_non_transposed.resize(dim);
-    for (Index_t i = 0; i < dim; ++i) {
-      this->nb_fourier_non_transposed[i] =
-          this->nb_fourier_grid_pts[dim - 1 - i];
+
+    // Determine process mesh for pencil decomposition.
+    if (dim > 2) {
+      dim_y = static_cast<int>(sqrt(size));
+      while ((size / dim_y) * dim_y != size)
+        dim_y--;
+      dim_x = size / dim_y;
     }
-    // Reverse the order of the array dimensions, because FFTW expects a
-    // row-major array and the arrays used in muSpectre are column-major
-    const int nb_dof{1};
-    ptrdiff_t res0{}, loc0{}, res1{}, loc1{};
-    this->workspace_size = fftw_mpi_local_size_many_transposed(
-        dim, this->nb_fourier_non_transposed.data(), nb_dof,
-        FFTW_MPI_DEFAULT_BLOCK, FFTW_MPI_DEFAULT_BLOCK,
-        this->comm.get_mpi_comm(), &res0, &loc0, &res1, &loc1);
-    // A factor of two is required because we are using the c2r/r2c DFTs.
-    // See:
-    // http://www.fftw.org/fftw3_doc/Multi_002ddimensional-MPI-DFTs-of-Real-Data.html
-    this->workspace_size *= 2;
-    // Allocate workspace buffer.
-    this->real_workspace = fftw_alloc_real(this->workspace_size);
-    if (this->real_workspace == nullptr) {
-      throw FFTEngineError("allocation of workspace buffer failed");
-    }
-    // res0, loc0 describe the decomposition of the first dimension of the input
-    // data. Since FFTW expect row-major grid but muFFT uses column-major grids,
-    // this is actually the last dimension.
-    this->nb_subdomain_grid_pts[dim - 1] = res0;
-    this->subdomain_locations[dim - 1] = loc0;
-    // res1, loc1 describe the decomposition of the second dimension of the
-    // output data. (Second since we are using transposed output.)
-    if (dim > 1) {
-      this->nb_fourier_grid_pts[dim - 2] = res1;
-      this->fourier_locations[dim - 2] = loc1;
-    } else {
-      this->nb_fourier_grid_pts[dim - 1] = res1;
-      this->fourier_locations[dim - 1] = loc1;
-    }
-    // Set the strides for the real space domain. The real space data needs to
-    // contain an additional padding region if the size if odd numbered. See
-    // http://www.fftw.org/fftw3_doc/Multi_002ddimensional-MPI-DFTs-of-Real-Data.html
-    // Note: This information is presently not used
-    if (dim > 1) {
-      this->subdomain_strides[1] = 2 * this->nb_fourier_grid_pts[0];
-      for (Index_t i = 2; i < dim; ++i) {
-        this->subdomain_strides[i] =
-            this->subdomain_strides[i - 1] * this->nb_subdomain_grid_pts[i - 1];
+
+    if (dim > 2) {
+      if (pfft_create_procmesh_2d(this->comm.get_mpi_comm(), dim_x, dim_y,
+                                  &this->mpi_comm)) {
+        throw FFTEngineError("Failed to create 2d PFFT process mesh.");
       }
     }
-    // Set the strides for the Fourier domain. Since we are omitted the last
-    // transpose, these strides reflect that the grid in the Fourier domain is
-    // transposed. This transpose operation is transparently handled by the
-    // Pixels class, which iterates consecutively of grid locations but returns
-    // the proper (transposed or untransposed) coordinates.
+
+    std::vector<ptrdiff_t> narr(dim);
+    for (Dim_t i = 0; i < dim; ++i) {
+      narr[i] = this->nb_domain_grid_pts[dim - 1 - i];
+    }
+    const int nb_dof{1};
+    std::vector<ptrdiff_t> res(dim), loc(dim), fres(dim), floc(dim);
+    pfft_local_size_many_dft_r2c(
+        dim, narr.data(), narr.data(), narr.data(), nb_dof,
+        PFFT_DEFAULT_BLOCKS, PFFT_DEFAULT_BLOCKS, this->mpi_comm,
+        PFFT_PADDED_R2C | PFFT_TRANSPOSED_OUT, res.data(), loc.data(),
+        fres.data(), floc.data());
+    for (Dim_t i = 0; i < dim; ++i) {
+      this->nb_subdomain_grid_pts[dim-1-i] = res[i];
+      this->subdomain_locations[dim-1-i] = loc[i];
+      this->nb_fourier_grid_pts[dim-1-i] = fres[i];
+      this->fourier_locations[dim-1-i] = floc[i];
+    }
+
+    // Set the strides for the real domain which is padded.
+    this->subdomain_strides = get_col_major_strides(
+        this->nb_subdomain_grid_pts);
+
+    // Set the strides for the Fourier domain (which is not padded but
+    // transposed). Since we are omitting the last transpose, these strides
+    // reflect that the grid in the Fourier domain is transposed. This
+    // transpose operation is transparently handled by the Pixels class, which
+    // iterates consecutively of grid locations but returns the proper
+    // (transposed or untransposed) coordinates.
     if (dim > 1) {
       // cumulative strides over first dimensions
-      Index_t s = this->fourier_strides[dim - 2];
-      this->fourier_strides[dim - 1] = s;
-      this->fourier_strides[dim - 2] = this->nb_fourier_grid_pts[dim - 1] * s;
+      this->fourier_strides[dim - 1] = 1;
+      this->fourier_strides[0] = this->nb_fourier_grid_pts[dim - 1];
+      for (Dim_t i = 1; i < dim - 1; ++i) {
+        this->fourier_strides[i] = this->fourier_strides[i - 1] *
+                                   this->nb_fourier_grid_pts[i - 1];
+      }
     }
 
+    // pfft_local_size_many_dft_r2c returns the *padded* size, not the real size
+    this->nb_subdomain_grid_pts[0] = this->nb_domain_grid_pts[0];
+
     for (auto & n : this->nb_subdomain_grid_pts) {
       if (n == 0) {
         this->active = false;
       }
     }
     for (auto & n : this->nb_fourier_grid_pts) {
       if (n == 0) {
         this->active = false;
       }
     }
-    this->fourier_field_collection.initialise(this->nb_fourier_grid_pts,
-                                              this->fourier_locations,
-                                              this->fourier_strides);
+    this->real_field_collection.initialise(
+        this->nb_domain_grid_pts, this->nb_subdomain_grid_pts,
+        this->subdomain_locations, this->subdomain_strides);
+    this->fourier_field_collection.initialise(
+        this->nb_domain_grid_pts, this->nb_fourier_grid_pts,
+        this->fourier_locations, this->fourier_strides);
   }
 
   /* ---------------------------------------------------------------------- */
-  void FFTWMPIEngine::initialise(const Index_t & nb_dof_per_pixel,
-                                 const FFT_PlanFlags & plan_flags) {
+  void PFFTEngine::create_plan(const Index_t & nb_dof_per_pixel) {
     if (this->has_plan_for(nb_dof_per_pixel)) {
       // plan already exists, we can bail
       return;
     }
 
     const int dim{this->nb_fourier_grid_pts.get_dim()};
 
-
-    if (not this->is_active()) {
-      return;
+    // Reverse the order of the array dimensions, because FFTW expects a
+    // row-major array and the arrays used in muSpectre are column-major
+    std::vector<ptrdiff_t> narr(dim);
+    for (Dim_t i = 0; i < dim; ++i) {
+      narr[i] = this->nb_domain_grid_pts[dim - 1 - i];
     }
-
     int howmany{static_cast<int>(nb_dof_per_pixel)};
-    ptrdiff_t res0{}, loc0{}, res1{}, loc1{};
-    // find how large a workspace this transform needs
-    // this needs the fourier grid points as input
-    auto required_workspace_size{fftw_mpi_local_size_many_transposed(
-        dim, this->nb_fourier_non_transposed.data(), nb_dof_per_pixel,
-        FFTW_MPI_DEFAULT_BLOCK, FFTW_MPI_DEFAULT_BLOCK,
-        this->comm.get_mpi_comm(), &res0, &loc0, &res1, &loc1)};
-    // A factor of two is required because we are using the c2r/r2c DFTs.
-    // See:
-    // http://www.fftw.org/fftw3_doc/Multi_002ddimensional-MPI-DFTs-of-Real-Data.html
-
+    std::vector<ptrdiff_t> res(dim), loc(dim), fres(dim), floc(dim);
+    auto required_workspace_size{pfft_local_size_many_dft_r2c(
+        dim, narr.data(), narr.data(), narr.data(), howmany,
+        PFFT_DEFAULT_BLOCKS, PFFT_DEFAULT_BLOCKS, this->mpi_comm,
+        PFFT_PADDED_R2C | PFFT_TRANSPOSED_OUT, res.data(), loc.data(),
+        fres.data(), floc.data())};
 
     required_workspace_size *= 2;
 
     this->required_workspace_sizes[nb_dof_per_pixel] = required_workspace_size;
 
-    // check whether the current workspace is large enough
-    if (this->workspace_size < required_workspace_size) {
-      if (this->real_workspace != nullptr) {
-        fftw_free(this->real_workspace);
-      }
-      this->real_workspace = fftw_alloc_real(required_workspace_size);
-      if (this->real_workspace == nullptr) {
-        throw FFTEngineError("allocation of workspace buffer failed");
-      }
-      this->workspace_size = required_workspace_size;
-    }
-
     unsigned int flags;
     switch (plan_flags) {
     case FFT_PlanFlags::estimate: {
-      flags = FFTW_ESTIMATE;
+      flags = PFFT_ESTIMATE;
       break;
     }
     case FFT_PlanFlags::measure: {
-      flags = FFTW_MEASURE;
+      flags = PFFT_MEASURE;
       break;
     }
     case FFT_PlanFlags::patient: {
-      flags = FFTW_PATIENT;
+      flags = PFFT_PATIENT;
       break;
     }
     default:
-      throw RuntimeError("unknown planner flag type");
+      throw FFTEngineError("unknown planner flag type");
       break;
     }
 
-    Real * in{this->real_workspace};
-    fftw_complex * out{fftw_alloc_complex(required_workspace_size/2)};
-
-    // Reverse the order of the array dimensions, because FFTW expects a
-    // row-major array and the arrays used in muSpectre are column-major
-    std::vector<ptrdiff_t> narr(dim);
-    for (Index_t i = 0; i < dim; ++i) {
-      narr[i] = this->nb_domain_grid_pts[dim - 1 - i];
+    Real * in{pfft_alloc_real(required_workspace_size)};
+    if (in == nullptr) {
+      throw FFTEngineError("'in' allocation failed");
+    }
+    pfft_complex * out{pfft_alloc_complex(required_workspace_size / 2)};
+    if (out == nullptr) {
+      throw FFTEngineError("'out' allocation failed");
     }
-    // this needs the domain grid points as input narr
-    this->fft_plans[nb_dof_per_pixel] = fftw_mpi_plan_many_dft_r2c(
-        dim, narr.data(), howmany, FFTW_MPI_DEFAULT_BLOCK,
-        FFTW_MPI_DEFAULT_BLOCK, in, out, this->comm.get_mpi_comm(),
-        FFTW_MPI_TRANSPOSED_OUT | flags);
 
+    this->fft_plans[nb_dof_per_pixel] = pfft_plan_many_dft_r2c(
+        dim, narr.data(), narr.data(), narr.data(), howmany,
+        PFFT_DEFAULT_BLOCKS, PFFT_DEFAULT_BLOCKS, in, out, this->mpi_comm,
+        PFFT_FORWARD, PFFT_PADDED_R2C | PFFT_TRANSPOSED_OUT | flags);
     if (this->fft_plans[nb_dof_per_pixel] == nullptr) {
-      if (dim == 1) {
-        throw FFTEngineError("r2c plan failed; MPI parallel FFTW does not "
-                             "support 1D r2c FFTs");
-      } else {
-         std::stringstream message{};
-        message << "Rank " << this->comm.rank() << ": r2c plan failed. "
-                << "nb_subdomain_grid_pts = "
-                << this->get_nb_subdomain_grid_pts()
-                << ", nb_domain_grid_pts = " << this->get_nb_domain_grid_pts();
-        throw RuntimeError{message.str()};
-      }
+      throw FFTEngineError("r2c plan failed");
     }
 
-    fftw_complex * i_in{out};
-    Real * i_out{this->real_workspace};
+    pfft_complex * i_in{out};
+    Real * i_out{in};
 
-    this->ifft_plans[nb_dof_per_pixel] = fftw_mpi_plan_many_dft_c2r(
-        dim, narr.data(), howmany, FFTW_MPI_DEFAULT_BLOCK,
-        FFTW_MPI_DEFAULT_BLOCK, i_in, i_out, this->comm.get_mpi_comm(),
-        FFTW_MPI_TRANSPOSED_IN | flags);
+    this->ifft_plans[nb_dof_per_pixel] = pfft_plan_many_dft_c2r(
+        dim, narr.data(), narr.data(), narr.data(), howmany,
+        PFFT_DEFAULT_BLOCKS, PFFT_DEFAULT_BLOCKS, i_in, i_out, this->mpi_comm,
+        PFFT_BACKWARD, PFFT_PADDED_R2C | PFFT_TRANSPOSED_IN | flags);
     if (this->ifft_plans[nb_dof_per_pixel] == nullptr) {
-      if (dim == 1)
-        throw FFTEngineError("c2r plan failed; MPI parallel FFTW does not "
-                             "support 1D c2r FFTs");
-      else
-        throw FFTEngineError("c2r plan failed");
+      throw FFTEngineError("c2r plan failed");
     }
-    fftw_free(out);
+
+    pfft_free(in);
+    pfft_free(out);
     this->planned_nb_dofs.insert(nb_dof_per_pixel);
   }
 
   /* ---------------------------------------------------------------------- */
-  FFTWMPIEngine::~FFTWMPIEngine() noexcept {
-    if (this->real_workspace != nullptr)
-      fftw_free(this->real_workspace);
+  PFFTEngine::~PFFTEngine() noexcept {
     for (auto && nb_dof_per_pixel : this->planned_nb_dofs) {
       if (this->fft_plans[nb_dof_per_pixel] != nullptr)
-        fftw_destroy_plan(this->fft_plans[nb_dof_per_pixel]);
+        pfft_destroy_plan(this->fft_plans[nb_dof_per_pixel]);
       if (this->ifft_plans[nb_dof_per_pixel] != nullptr)
-        fftw_destroy_plan(this->ifft_plans[nb_dof_per_pixel]);
+        pfft_destroy_plan(this->ifft_plans[nb_dof_per_pixel]);
+    }
+    if (this->mpi_comm != this->comm.get_mpi_comm()) {
+      MPI_Comm_free(&this->mpi_comm);
     }
-    // TODO(junge): We cannot run fftw_mpi_cleanup since also calls fftw_cleanup
-    // and any running FFTWEngine will fail afterwards.
+    // TODO(Till): We cannot run fftw_mpi_cleanup since also calls fftw_cleanup
+    // and any running PFFTEngine will fail afterwards.
     // this->nb_engines--;
-    // if (!this->nb_engines) fftw_mpi_cleanup();
+    // if (!this->nb_engines) pfft_cleanup();
   }
 
   /* ---------------------------------------------------------------------- */
-  void FFTWMPIEngine::fft(const RealField_t & input_field,
-                          FourierField_t & output_field) const {
-    if (not this->is_active()) {
-      return;
-    }
-    auto && nb_dof_per_pixel{input_field.get_nb_dof_per_pixel()};
-    if (nb_dof_per_pixel != output_field.get_nb_dof_per_pixel()) {
-      std::stringstream message{};
-      message << "The input and output fields are not compatible: the input "
-                 "field has  "
-              << nb_dof_per_pixel
-              << " degrees of freedom per pixel, while the output field has "
-              << output_field.get_nb_dof_per_pixel();
-      throw FFTEngineError{message.str()};
-    }
-    if (not this->has_plan_for(nb_dof_per_pixel)) {
-      std::stringstream message{};
-      message << "No plan has been created for " << nb_dof_per_pixel
-              << " degrees of freedom per pixel. Use "
-                 "`muFFT::FFTEngineBase::initialise` to prepare a plan.";
-      throw FFTEngineError{message.str()};
-    }
-    if (static_cast<size_t>(input_field.get_nb_pixels()) !=
-        muGrid::CcoordOps::get_size(this->nb_subdomain_grid_pts)) {
-      std::stringstream error{};
-      error << std::endl
-            << "rank " << this->get_communicator().rank()
-            << ": The number of pixels of the input field '"
-            << input_field.get_name() << "' passed to the forward FFT is "
-            << input_field.get_nb_pixels() << " and does not match the size "
-            << muGrid::CcoordOps::get_size(this->nb_subdomain_grid_pts)
-            << " of the (sub)domain handled by FFTWMPIEngine.";
-      throw RuntimeError(error.str());
-    }
-    if (static_cast<size_t>(output_field.get_nb_pixels()) !=
-        muGrid::CcoordOps::get_size(this->nb_fourier_grid_pts)) {
-      std::stringstream error{};
-      error << std::endl
-            << "rank " << this->get_communicator().rank()
-            << ": The number of pixels of the Fourier space output field '"
-            << output_field.get_name() << "' passed to the forward FFT is "
-            << output_field.get_nb_pixels() << " and doesn't match the size "
-            << muGrid::CcoordOps::get_size(this->nb_fourier_grid_pts)
-            << " of the (sub)domain handled by this FFTWMPIEngine." << std::endl
-            << "Domain shape:         " << this->nb_domain_grid_pts << ","
-            << std::endl
-            << "Subdomain shape:      " << this->nb_subdomain_grid_pts
-            << ", locations: " << this->subdomain_locations << std::endl
-            << "Fourier domain shape: " << this->nb_fourier_grid_pts
-            << ", locations: " << this->fourier_locations;
-      throw RuntimeError(error.str());
-    }
+  void PFFTEngine::compute_fft(const RealField_t & input_field,
+                               FourierField_t & output_field) {
+    // Compute FFT
+    pfft_execute_dft_r2c(
+        this->fft_plans.at(input_field.get_nb_dof_per_pixel()),
+        input_field.data(),
+        reinterpret_cast<pfft_complex *>(output_field.data()));
+  }
+
+  /* ---------------------------------------------------------------------- */
+  void PFFTEngine::compute_ifft(const FourierField_t & input_field,
+                                   RealField_t & output_field) {
+    pfft_execute_dft_c2r(
+        this->ifft_plans.at(input_field.get_nb_dof_per_pixel()),
+        reinterpret_cast<pfft_complex *>(input_field.data()),
+        output_field.data());
+  }
+
+  /* ---------------------------------------------------------------------- */
+  std::unique_ptr<FFTEngineBase> PFFTEngine::clone() const {
+    return std::make_unique<PFFTEngine>(
+        this->get_nb_domain_grid_pts(), this->get_communicator(),
+        this->plan_flags, this->allow_temporary_buffer,
+        this->allow_destroy_input);
+  }
+
+  /* ---------------------------------------------------------------------- */
+  auto
+  PFFTEngine::register_real_space_field(const std::string & unique_name,
+                                           const Index_t & nb_dof_per_pixel)
+  -> RealField_t & {
+    this->create_plan(nb_dof_per_pixel);
+    auto & field{
+        Parent::register_real_space_field(unique_name, nb_dof_per_pixel)};
     /*
      * We need to check whether the fourier field provided is large
      * enough. MPI parallel FFTW may request a workspace size larger than the
      * nominal size of the complex buffer.
      */
     auto && required_workspace_size{
-        this->required_workspace_sizes.at(nb_dof_per_pixel)};
-    if (static_cast<int>(output_field.size() * nb_dof_per_pixel) <
-        required_workspace_size) {
-      output_field.set_pad_size(this->get_required_pad_size(nb_dof_per_pixel));
-    }
-    // Copy non-padded field to padded real_workspace.
-    // Transposed output of M x N x L transform for >= 3 dimensions is padded
-    // M x N x 2*(L/2+1).
-    ptrdiff_t fstride = (nb_dof_per_pixel * this->nb_subdomain_grid_pts[0]);
-    ptrdiff_t wstride =
-        (nb_dof_per_pixel * 2 * (this->nb_subdomain_grid_pts[0] / 2 + 1));
-    ptrdiff_t n = input_field.size() / this->nb_subdomain_grid_pts[0];
-
-    auto fdata{input_field.data()};
-    auto wdata{this->real_workspace};
-    for (int i = 0; i < n; i++) {
-      std::copy(fdata, fdata + fstride, wdata);
-      fdata += fstride;
-      wdata += wstride;
-    }
-
-    // Compute FFT
-    fftw_mpi_execute_dft_r2c(
-        this->fft_plans.at(nb_dof_per_pixel), this->real_workspace,
-        reinterpret_cast<fftw_complex *>(output_field.data()));
+        2 * this->required_workspace_sizes.at(nb_dof_per_pixel)};
+    field.set_pad_size(required_workspace_size -
+                       nb_dof_per_pixel * field.get_nb_buffer_pixels());
+    return field;
   }
 
   /* ---------------------------------------------------------------------- */
-  void FFTWMPIEngine::ifft(const FourierField_t & input_field,
-                           RealField_t & output_field) const {
-    if (not this->is_active()) {
-      return;
-    }
-    auto && nb_dof_per_pixel{input_field.get_nb_dof_per_pixel()};
-    if (nb_dof_per_pixel != output_field.get_nb_dof_per_pixel()) {
-      std::stringstream message{};
-      message << "The input and output fields are not compatible: the input "
-                 "field has  "
-              << nb_dof_per_pixel
-              << " degrees of freedom per pixel, while the output field has "
-              << output_field.get_nb_dof_per_pixel();
-      throw FFTEngineError{message.str()};
-    }
-    if (not this->has_plan_for(nb_dof_per_pixel)) {
-      std::stringstream message{};
-      message << "No plan has been created for " << nb_dof_per_pixel
-              << " degrees of freedom per pixel. Use "
-                 "`muFFT::FFTEngineBase::initialise` to prepare a plan.";
-      throw FFTEngineError{message.str()};
-    }
-
-    if (static_cast<size_t>(output_field.get_nb_pixels()) !=
-        muGrid::CcoordOps::get_size(this->nb_subdomain_grid_pts)) {
-      std::stringstream error;
-      error << std::endl
-            << "rank " << this->get_communicator().rank()
-            << ": The number of pixels of the output_field '"
-            << output_field.get_name() << "' passed to the inverse FFT is "
-            << output_field.get_nb_pixels() << " and does not match the size "
-            << muGrid::CcoordOps::get_size(this->nb_subdomain_grid_pts)
-            << " of the (sub)domain handled by FFTWEngine.";
-      throw RuntimeError(error.str());
-    }
-
-    if (static_cast<size_t>(input_field.get_nb_pixels()) !=
-        muGrid::CcoordOps::get_size(this->nb_fourier_grid_pts)) {
-      std::stringstream error;
-      error << std::endl
-            << "rank " << this->get_communicator().rank()
-            << ": The number of pixels of the Fourier space input_field '"
-            << input_field.get_name() << "' passed to the inverse FFT is "
-            << input_field.get_nb_pixels() << " and does not match the size "
-            << muGrid::CcoordOps::get_size(this->nb_subdomain_grid_pts)
-            << " of the (sub)domain handled by this FFTWEngine." << std::endl
-            << "Domain shape:         " << this->nb_domain_grid_pts << ","
-            << std::endl
-            << "Subdomain shape:      " << this->nb_subdomain_grid_pts
-            << ", locations: " << this->subdomain_locations << std::endl
-            << "Fourier domain shape: " << this->nb_fourier_grid_pts
-            << ", locations: " << this->fourier_locations;
-      throw RuntimeError(error.str());
-    }
-
-    // Compute inverse FFT
-    fftw_mpi_execute_dft_c2r(
-        this->ifft_plans.at(nb_dof_per_pixel),
-        reinterpret_cast<fftw_complex *>(input_field.data()),
-        this->real_workspace);
-    // Copy non-padded field to padded real_workspace.
-    // Transposed output of M x N x L transform for >= 3 dimensions is padded
-    // M x N x 2*(L/2+1).
-    ptrdiff_t fstride{nb_dof_per_pixel * this->nb_subdomain_grid_pts[0]};
-    ptrdiff_t wstride{nb_dof_per_pixel * 2 *
-                      (this->nb_subdomain_grid_pts[0] / 2 + 1)};
-    ptrdiff_t n(output_field.size() / this->nb_subdomain_grid_pts[0]);
-
-    auto fdata{output_field.data()};
-    auto wdata{this->real_workspace};
-    for (int i = 0; i < n; i++) {
-      std::copy(wdata, wdata + fstride, fdata);
-      fdata += fstride;
-      wdata += wstride;
-    }
-  }
-
-  /* ---------------------------------------------------------------------- */
-  std::unique_ptr<FFTEngineBase> FFTWMPIEngine::clone() const {
-    return std::make_unique<FFTWMPIEngine>(this->get_nb_domain_grid_pts(),
-                                           this->get_communicator());
+  auto PFFTEngine::register_real_space_field(const std::string & unique_name,
+                                                const Shape_t & shape)
+  -> RealField_t & {
+    auto & field{Parent::register_real_space_field(unique_name, shape)};
+    /*
+     * We need to check whether the fourier field provided is large
+     * enough. MPI parallel FFTW may request a workspace size larger than the
+     * nominal size of the complex buffer.
+     */
+    auto nb_dof_per_pixel{std::accumulate(shape.begin(), shape.end(), 1,
+                                          std::multiplies<Index_t>())};
+    auto && required_workspace_size{
+        2 * this->required_workspace_sizes.at(nb_dof_per_pixel)};
+    field.set_pad_size(required_workspace_size -
+                       nb_dof_per_pixel * field.get_nb_buffer_pixels());
+    return field;
   }
 
   /* ---------------------------------------------------------------------- */
-  auto
-  FFTWMPIEngine::register_fourier_space_field(const std::string & unique_name,
-                                              const Index_t & nb_dof_per_pixel)
-      -> FourierField_t & {
-    if (not this->has_plan_for(nb_dof_per_pixel)) {
-      std::stringstream message{};
-      message << "No plan has been created for " << nb_dof_per_pixel
-              << " degrees of freedom per pixel. Use "
-                 "`muFFT::FFTEngineBase::initialise` to prepare a plan.";
-      throw FFTEngineError{message.str()};
-    }
+  muGrid::ComplexField & PFFTEngine::register_fourier_space_field(
+      const std::string & unique_name, const Index_t & nb_dof_per_pixel) {
     auto & field{
         Parent::register_fourier_space_field(unique_name, nb_dof_per_pixel)};
     /*
      * We need to check whether the fourier field provided is large
      * enough. MPI parallel FFTW may request a workspace size larger than the
      * nominal size of the complex buffer.
      */
     auto && required_workspace_size{
         this->required_workspace_sizes.at(nb_dof_per_pixel)};
-    if (static_cast<int>(field.size() * nb_dof_per_pixel) <
+    if (static_cast<int>(field.get_nb_entries() * nb_dof_per_pixel) <
         required_workspace_size) {
-      field.set_pad_size(required_workspace_size -
-                         nb_dof_per_pixel * field.size());
+      auto pad_size{required_workspace_size -
+                    nb_dof_per_pixel * field.get_nb_buffer_pixels()};
+      field.set_pad_size(std::max(0L, pad_size));
     }
     return field;
   }
 
   /* ---------------------------------------------------------------------- */
-  Index_t
-  FFTWMPIEngine::get_required_pad_size(const Index_t & nb_dof_per_pixel) const {
+  muGrid::ComplexField &
+  PFFTEngine::register_fourier_space_field(const std::string & unique_name,
+                                              const Shape_t & shape) {
+    auto & field{Parent::register_fourier_space_field(unique_name, shape)};
+    /*
+     * We need to check whether the fourier field provided is large
+     * enough. MPI parallel FFTW may request a workspace size larger than the
+     * nominal size of the complex buffer.
+     */
+    auto nb_dof_per_pixel{std::accumulate(shape.begin(), shape.end(), 1,
+                                          std::multiplies<Index_t>())};
+    auto && required_workspace_size{
+        this->required_workspace_sizes.at(nb_dof_per_pixel)};
+    if (static_cast<int>(field.get_nb_entries() * nb_dof_per_pixel) <
+        required_workspace_size) {
+      auto pad_size{required_workspace_size -
+                    nb_dof_per_pixel * field.get_nb_buffer_pixels()};
+      field.set_pad_size(std::max(0L, pad_size));
+    }
+    return field;
+  }
+
+  /* ---------------------------------------------------------------------- */
+  bool PFFTEngine::check_real_space_field(const RealField_t & field) const {
+    auto nb_dof_per_pixel{field.get_nb_dof_per_pixel()};
+    auto && required_workspace_size{
+        2 * this->required_workspace_sizes.at(nb_dof_per_pixel)};
+    auto required_pad_size{required_workspace_size -
+                           nb_dof_per_pixel * field.get_nb_buffer_pixels()};
+    return Parent::check_real_space_field(field) and
+           static_cast<Index_t>(field.get_pad_size()) >= required_pad_size;
+  }
+
+  /* ---------------------------------------------------------------------- */
+  bool
+  PFFTEngine::check_fourier_space_field(const FourierField_t & field) const {
+    auto nb_dof_per_pixel{field.get_nb_dof_per_pixel()};
     auto && required_workspace_size{
         this->required_workspace_sizes.at(nb_dof_per_pixel)};
-    return required_workspace_size - nb_dof_per_pixel * this->fourier_size();
+    auto required_pad_size{required_workspace_size -
+                           nb_dof_per_pixel * field.get_nb_buffer_pixels()};
+    return Parent::check_fourier_space_field(field) and
+           static_cast<Index_t>(field.get_pad_size()) >= required_pad_size;
   }
 
 }  // namespace muFFT
```

### Comparing `muFFT-0.9.3/src/libmufft/fftwmpi_engine.hh` & `mufft-0.90.0/src/libmufft/pfft_engine.hh`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /**
- * @file   fftwmpi_engine.hh
+ * @file   pfft_engine.hh
  *
  * @author Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
  *
  * @date   06 Mar 2017
  *
- * @brief  FFT engine using MPI-parallel FFTW
+ * @brief  FFT engine using MPI-parallel PFFT
  *
  * Copyright © 2017 Till Junge
  *
  * µFFT is free software; you can redistribute it and/or
  * modify it under the terms of the GNU Lesser General Public License as
  * published by the Free Software Foundation, either version 3, or (at
  * your option) any later version.
@@ -29,107 +29,127 @@
  * If you modify this Program, or any covered work, by linking or combining it
  * with proprietary FFT implementations or numerical libraries, containing parts
  * covered by the terms of those libraries' licenses, the licensors of this
  * Program grant you additional permission to convey the resulting work.
  *
  */
 
-#ifndef SRC_LIBMUFFT_FFTWMPI_ENGINE_HH_
-#define SRC_LIBMUFFT_FFTWMPI_ENGINE_HH_
+#ifndef SRC_LIBMUFFT_PFFT_ENGINE_HH_
+#define SRC_LIBMUFFT_PFFT_ENGINE_HH_
 
 #include "fft_engine_base.hh"
 
-#include <fftw3-mpi.h>
+#include <pfft.h>
 
 namespace muFFT {
 
   /**
    * implements the `muFFT::FFTEngineBase` interface using the
    * FFTW library
    */
-  class FFTWMPIEngine : public FFTEngineBase {
+  class PFFTEngine : public FFTEngineBase {
    public:
     using Parent = FFTEngineBase;  //!< base class
     //! field for Fourier transform of second-order tensor
     using FourierField_t = typename Parent::FourierField_t;
     //! real-valued second-order tensor
     using RealField_t = typename Parent::RealField_t;
     //! Default constructor
-    FFTWMPIEngine() = delete;
+    PFFTEngine() = delete;
 
     /**
      * Constructor with the domain's number of grid points in each direction and
      * the communicator
+     * @param nb_grid_pts number of grid points of the global grid
+     * @param comm MPI communicator object
+     * @param plan_flags MPI planner flags
+     * @param allow_temporary_buffer allow the creation of temporary buffers
+     *        if the input buffer has the wrong memory layout
+     * @param allow_destroy_input allow that the input buffers are invalidated
+     *        during the FFT
      */
-    FFTWMPIEngine(const DynCcoord_t & nb_grid_pts,
-                  Communicator comm = Communicator());
+    PFFTEngine(const DynCcoord_t & nb_grid_pts,
+               Communicator comm = Communicator(),
+               const FFT_PlanFlags & plan_flags = FFT_PlanFlags::estimate,
+               bool allow_temporary_buffer = true,
+               bool allow_destroy_input = false);
 
     //! Copy constructor
-    FFTWMPIEngine(const FFTWMPIEngine & other) = delete;
+    PFFTEngine(const PFFTEngine & other) = delete;
 
     //! Move constructor
-    FFTWMPIEngine(FFTWMPIEngine && other) = delete;
+    PFFTEngine(PFFTEngine && other) = delete;
 
     //! Destructor
-    virtual ~FFTWMPIEngine() noexcept;
+    virtual ~PFFTEngine() noexcept;
 
     //! Copy assignment operator
-    FFTWMPIEngine & operator=(const FFTWMPIEngine & other) = delete;
+    PFFTEngine & operator=(const PFFTEngine & other) = delete;
 
     //! Move assignment operator
-    FFTWMPIEngine & operator=(FFTWMPIEngine && other) = delete;
+    PFFTEngine & operator=(PFFTEngine && other) = default;
 
     // compute the plan, etc
-    void initialise(const Index_t & nb_dof_per_pixel,
-                    const FFT_PlanFlags & plan_flags) override;
+    void create_plan(const Index_t & nb_dof_per_pixel) override;
 
-    //! forward transform
-    void fft(const RealField_t & field,
-             FourierField_t & output_field) const override;
-
-    //! inverse transform
-    void ifft(const FourierField_t & input_field,
-              RealField_t & output_field) const override;
+    //! perform a deep copy of the engine (this should never be necessary in
+    //! c++)
+    std::unique_ptr<FFTEngineBase> clone() const final;
 
     /**
-     * return whether this engine is active (an engine is active if it has more
-     * than zero grid points. FFTWMPI sometimes assigns zero grid points)
+     * need to override this method here, since FFTWMPI requires field padding
      */
-    bool is_active() const override { return this->active; }
+    RealField_t &
+    register_real_space_field(const std::string & unique_name,
+                              const Index_t & nb_dof_per_pixel) final;
 
-    //! perform a deep copy of the engine (this should never be necessary in
-    //! c++)
-    std::unique_ptr<FFTEngineBase> clone() const final;
+    /**
+     * need to override this method here, since FFTWMPI requires field padding
+     */
+    RealField_t &
+    register_real_space_field(const std::string & unique_name,
+                              const Shape_t & shape) final;
 
     /**
      * need to override this method here, since FFTWMPI requires field padding
      */
-    FourierField_t &
+    muGrid::ComplexField &
     register_fourier_space_field(const std::string & unique_name,
                                  const Index_t & nb_dof_per_pixel) final;
 
     /**
-     * Returns the required pad size. Helpful when calling fftwmpi with wrapped
-     * fields
+     * need to override this method here, since FFTWMPI requires field padding
      */
-    Index_t get_required_pad_size(const Index_t & nb_dof_per_pixel) const final;
+    muGrid::ComplexField &
+    register_fourier_space_field(const std::string & unique_name,
+                                 const Shape_t & shape) final;
 
    protected:
+    //! forward transform
+    void compute_fft(const RealField_t & field,
+                     FourierField_t & output_field) override;
+
+    //! inverse transform
+    void compute_ifft(const FourierField_t & input_field,
+                      RealField_t & output_field) override;
+
+    //! check whether real-space buffer has the correct memory layout
+    bool check_real_space_field(const RealField_t & field) const final;
+
+    //! check whether Fourier-space buffer has the correct memory layout
+    bool check_fourier_space_field(const FourierField_t & field) const final;
+
     static int nb_engines;  //!< number of times this engine has
-                            //!< been instatiated
+                            //!< been instantiated
+    MPI_Comm mpi_comm;  //!< MPI communicator
     //! holds the plans for forward fourier transforms
-    std::map<Index_t, fftw_plan> fft_plans{};
+    std::map<Index_t, pfft_plan> fft_plans{};
     //! holds the plans for inversefourier transforms
-    std::map<Index_t, fftw_plan> ifft_plans{};
+    std::map<Index_t, pfft_plan> ifft_plans{};
     //! holds the fourier field sizes including padding for different transforms
     std::map<Index_t, Index_t> required_workspace_sizes{};
-    //! maximum size of workspace buffer (returned by planner)
-    ptrdiff_t workspace_size{0};
-    //! temporary real workspace for correctly padded copy of real input
-    Real * real_workspace{nullptr};
-    bool active{true};  //!< FFTWMPI sometimes assigns zero grid points
-    //! Input to local_size_many_transposed
-    std::vector<ptrdiff_t> nb_fourier_non_transposed{};
+    bool active{true};  //!< PFFT sometimes assigns zero grid points
   };
+
 }  // namespace muFFT
 
-#endif  // SRC_LIBMUFFT_FFTWMPI_ENGINE_HH_
+#endif  // SRC_LIBMUFFT_PFFT_ENGINE_HH_
```

### Comparing `muFFT-0.9.3/src/libmufft/mufft_common.hh` & `mufft-0.90.0/src/libmufft/mufft_common.hh`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  * If you modify this Program, or any covered work, by linking or combining it
  * with proprietary FFT implementations or numerical libraries, containing parts
  * covered by the terms of those libraries' licenses, the licensors of this
  * Program grant you additional permission to convey the resulting work.
  *
  */
 
-#include <libmugrid/grid_common.hh>
+#include "libmugrid/grid_common.hh"
 
 #ifndef SRC_LIBMUFFT_MUFFT_COMMON_HH_
 #define SRC_LIBMUFFT_MUFFT_COMMON_HH_
 
 namespace muFFT {
   using muGrid::Dim_t;
   using muGrid::Index_t;
@@ -49,24 +49,26 @@
 
   using muGrid::RuntimeError;
 
   using muGrid::Ccoord_t;
   using muGrid::DynCcoord_t;
   using muGrid::DynRcoord_t;
   using muGrid::Rcoord_t;
+  using muGrid::Shape_t;
 
   using muGrid::optional;
 
   using muGrid::oneD;
   using muGrid::threeD;
   using muGrid::twoD;
 
   using muGrid::OneQuadPt;
   using muGrid::TwoQuadPts;
   using muGrid::FourQuadPts;
+  using muGrid::SixQuadPts;
   using muGrid::OneNode;
 
   using muGrid::Mapping;
   using muGrid::IterUnit;
 
   /**
    * Planner flags for FFT (follows FFTW, hopefully this choice will
```

### Comparing `muFFT-0.9.3/src/projection/projection_approx_Green_operator.hh` & `mufft-0.90.0/src/libmufft/pocketfft_engine.hh`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,122 @@
 /**
- * @file   projection_approx_Green_operator.hh
+ * @file   pocketfft_engine.hh
  *
- * @author Martin Ladecký <m.ladecky@gmail.com>
+ * @author Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
  *
- * @date   01 Feb 2020
+ * @date   20 Nov 2022
  *
- * @brief  Discrete Green's function for constant material properties
+ * @brief  FFT engine using PocketFFT
  *
- * Copyright © 2020 Martin Ladecký
+ * Copyright © 2017 Till Junge
  *
- * µSpectre is free software; you can redistribute it and/or
+ * µFFT is free software; you can redistribute it and/or
  * modify it under the terms of the GNU Lesser General Public License as
  * published by the Free Software Foundation, either version 3, or (at
  * your option) any later version.
  *
- * µSpectre is distributed in the hope that it will be useful, but
+ * µFFT is distributed in the hope that it will be useful, but
  * WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
  * Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with µSpectre; see the file COPYING. If not, write to the
+ * along with µFFT; see the file COPYING. If not, write to the
  * Free Software Foundation, Inc., 59 Temple Place - Suite 330,
- * Boston, MA 02111-1307, USA.
+ * * Boston, MA 02111-1307, USA.
  *
  * Additional permission under GNU GPL version 3 section 7
  *
  * If you modify this Program, or any covered work, by linking or combining it
  * with proprietary FFT implementations or numerical libraries, containing parts
  * covered by the terms of those libraries' licenses, the licensors of this
  * Program grant you additional permission to convey the resulting work.
  *
  */
 
-#ifndef SRC_PROJECTION_PROJECTION_APPROX_GREEN_OPERATOR_HH_
-#define SRC_PROJECTION_PROJECTION_APPROX_GREEN_OPERATOR_HH_
+#ifndef SRC_LIBMUFFT_POCKETFFT_ENGINE_HH_
+#define SRC_LIBMUFFT_POCKETFFT_ENGINE_HH_
 
-#include "projection/projection_default.hh"
+#include "fft_engine_base.hh"
 
-namespace muSpectre {
+namespace muFFT {
 
-  template <Index_t DimS>
-  class ProjectionApproxGreenOperator : public ProjectionDefault<DimS> {
+  /**
+   * implements the `muFFT::FftEngine_Base` interface using
+   * PocketFFT (that is shipped as part of this code).
+   * See pocketfft/LICENSE.md for PocketFFT's license.
+   */
+  class PocketFFTEngine : public FFTEngineBase {
    public:
-    using Parent = ProjectionDefault<DimS>;  //!< base class
-    //! gradient, i.e. derivatives in each Cartesian direction
-    using Gradient_t = typename Parent::Gradient_t;
-    using Ccoord = typename Parent::Ccoord;  //!< cell coordinates type
-    using Rcoord = typename Parent::Rcoord;  //!< spatial coordinates type
-    //! Fourier-space field containing the projection operator itself
-    using Proj_t = muGrid::RealField;
-    //! iterable operator
-    using Proj_map =
-        muGrid::T4FieldMap<Real, Mapping::Mut, DimS, IterUnit::SubPt>;
-    //! iterable vectorised version of the Fourier-space tensor field
-    using Vector_map =
-        muGrid::MatrixFieldMap<Complex, Mapping::Mut, DimS * DimS, 1,
-                               IterUnit::SubPt>;
-
+    using Parent = FFTEngineBase;  //!< base class
+    //! field for Fourier transform of second-order tensor
+    using FourierField_t = typename Parent::FourierField_t;
+    //! real-valued second-order tensor
+    using RealField_t = typename Parent::RealField_t;
     //! Default constructor
-    ProjectionApproxGreenOperator() = delete;
+    PocketFFTEngine() = delete;
 
-    //! Constructor with fft_engine
-    ProjectionApproxGreenOperator(
-        muFFT::FFTEngine_ptr engine, const DynRcoord_t & lengths,
-        const Eigen::Ref<Eigen::Matrix<Real, Eigen::Dynamic, Eigen::Dynamic>> &
-            C_ref,
-        Gradient_t gradient);
-
-    //! Constructor with fft_engine and default (Fourier) gradient
-    ProjectionApproxGreenOperator(
-        muFFT::FFTEngine_ptr engine, const DynRcoord_t & lengths,
-        const Eigen::Ref<Eigen::Matrix<Real, Eigen::Dynamic, Eigen::Dynamic>> &
-            C_ref);
+    /**
+     * Constructor with the domain's number of grid points in each direction,
+     * the communicator, and fft planner flags
+     * @param nb_grid_pts number of grid points of the global grid
+     * @param allow_temporary_buffer allow the creation of temporary buffers
+     *        if the input buffer has the wrong memory layout
+     * @param allow_destroy_input allow that the input buffers are invalidated
+     *        during the FFT
+     * @comm MPI communicator object
+     */
+    PocketFFTEngine(const DynCcoord_t & nb_grid_pts,
+                    Communicator comm = Communicator(),
+                    const FFT_PlanFlags & plan_flags = FFT_PlanFlags::estimate,
+                    bool allow_temporary_buffer = true,
+                    bool allow_destroy_input = false);
+    /**
+     * Constructor with the domain's number of grid points in each direction and
+     * the fft planner flags
+     * @param nb_grid_pts number of grid points of the global grid
+     * @param allow_temporary_buffer allow the creation of temporary buffers
+     *        if the input buffer has the wrong memory layout
+     * @param allow_destroy_input allow that the input buffers are invalidated
+     *        during the FFT
+     * @comm MPI communicator object
+     */
+    PocketFFTEngine(const DynCcoord_t & nb_grid_pts,
+                    const FFT_PlanFlags & plan_flags,
+                    bool allow_temporary_buffer = true,
+                    bool allow_destroy_input = false);
 
     //! Copy constructor
-    ProjectionApproxGreenOperator(const ProjectionApproxGreenOperator & other) =
-        delete;
+    PocketFFTEngine(const PocketFFTEngine & other) = delete;
 
     //! Move constructor
-    ProjectionApproxGreenOperator(ProjectionApproxGreenOperator && other) =
-        default;
+    PocketFFTEngine(PocketFFTEngine && other) = delete;
 
     //! Destructor
-    virtual ~ProjectionApproxGreenOperator() = default;
+    virtual ~PocketFFTEngine() noexcept;
 
     //! Copy assignment operator
-    ProjectionApproxGreenOperator &
-    operator=(const ProjectionApproxGreenOperator & other) = delete;
+    PocketFFTEngine & operator=(const PocketFFTEngine & other) = delete;
 
     //! Move assignment operator
-    ProjectionApproxGreenOperator &
-    operator=(ProjectionApproxGreenOperator && other) = delete;
+    PocketFFTEngine & operator=(PocketFFTEngine && other) = delete;
 
-    //! initialises the fft engine (plan the transform)
-    void initialise(const muFFT::FFT_PlanFlags & flags =
-                        muFFT::FFT_PlanFlags::estimate) final;
-    //! initialises the fft engine (plan the transform)
-    void reinitialise(
-        const Eigen::Ref<Eigen::Matrix<Real, Eigen::Dynamic, Eigen::Dynamic>> &
-            C_ref_new);
+    // compute the plan, etc
+    void create_plan(const Index_t & nb_dof_per_pixel) override;
 
-    //! perform a deep copy of the projector (this should never be necessary in
+    //! perform a deep copy of the engine (this should never be necessary in
     //! c++)
-    std::unique_ptr<ProjectionBase> clone() const final;
+    std::unique_ptr<FFTEngineBase> clone() const final;
 
    protected:
-    //! Elastic tensor of reference material
-    using C_t = Eigen::Matrix<Real, DimS * DimS, DimS * DimS>;
-    std::unique_ptr<C_t> C_ref_holder;
-    C_t & C_ref;
+    //! forward transform
+    void compute_fft(const RealField_t & input_field,
+                     FourierField_t & output_field) override;
+
+    //! inverse transform
+    void compute_ifft(const FourierField_t & input_field,
+                      RealField_t & output_field) override;
   };
 
-}  // namespace muSpectre
+}  // namespace muFFT
 
-#endif  // SRC_PROJECTION_PROJECTION_APPROX_GREEN_OPERATOR_HH_
+#endif  // SRC_LIBMUFFT_POCKETFFT_ENGINE_HH_
```

### Comparing `muFFT-0.9.3/tests/libmufft/mpi_context.hh` & `mufft-0.90.0/tests/mpi_context.hh`

 * *Files 8% similar despite different names*

```diff
@@ -32,31 +32,35 @@
  * Program grant you additional permission to convey the resulting work.
  *
  */
 
 #ifndef TESTS_LIBMUFFT_MPI_CONTEXT_HH_
 #define TESTS_LIBMUFFT_MPI_CONTEXT_HH_
 
-#include <libmufft/communicator.hh>
+#include <boost/test/unit_test.hpp>
+
+#include <libmugrid/communicator.hh>
+
+using muGrid::Communicator;
 
 namespace muFFT {
 
   /*!
    * MPI context singleton. Initialize MPI once when needed.
    */
   class MPIContext {
    public:
-    Communicator comm;
+    muGrid::Communicator comm;
     static MPIContext & get_context() {
       static MPIContext context;
       return context;
     }
 
    private:
-    MPIContext() : comm(Communicator(MPI_COMM_WORLD)) {
+    MPIContext() : comm(muGrid::Communicator(MPI_COMM_WORLD)) {
       MPI_Init(&boost::unit_test::framework::master_test_suite().argc,
                &boost::unit_test::framework::master_test_suite().argv);
     }
     ~MPIContext() {
       // Wait for all processes to finish before calling finalize.
       MPI_Barrier(comm.get_mpi_comm());
       MPI_Finalize();
```

### Comparing `muFFT-0.9.3/tests/libmufft/mpi_test_fft_engine.cc` & `mufft-0.90.0/tests/mpi_test_fft_engine.cc`

 * *Files 14% similar despite different names*

```diff
@@ -36,22 +36,27 @@
 #define BOOST_MPL_CFG_NO_PREPROCESSED_HEADERS
 #define BOOST_MPL_LIMIT_LIST_SIZE 50
 
 #include <boost/mpl/list.hpp>
 
 #include "tests.hh"
 #include "mpi_context.hh"
+#include <libmufft/pocketfft_engine.hh>
+#ifdef WITH_FFTW
 #include <libmufft/fftw_engine.hh>
+#endif
 #ifdef WITH_FFTWMPI
 #include <libmufft/fftwmpi_engine.hh>
 #endif
 #ifdef WITH_PFFT
 #include <libmufft/pfft_engine.hh>
 #endif
 
+#include "mpi_context.hh"
+
 #include <libmugrid/ccoord_operations.hh>
 #include <libmugrid/field_collection.hh>
 #include <libmugrid/field_map_static.hh>
 #include <libmugrid/iterators.hh>
 
 namespace muFFT {
   using muFFT::tol;
@@ -106,44 +111,48 @@
       FFTW_fixture_python_segfault<FFTWMPIEngine>,
 #endif
 #ifdef WITH_PFFT
       FFTW_fixture<PFFTEngine, twoD, 3>, FFTW_fixture<PFFTEngine, threeD, 3>,
       FFTW_fixture<PFFTEngine, twoD, 4>, FFTW_fixture<PFFTEngine, threeD, 4>,
       FFTW_fixture_python_segfault<PFFTEngine>,
 #endif
-      FFTW_fixture<FFTWEngine, twoD, 3, true>>;
+#ifdef WITH_FFTW
+      FFTW_fixture<FFTWEngine, twoD, 3, true>,
+#endif
+      FFTW_fixture<PocketFFTEngine, twoD, 3, true>>;
 
   /* ---------------------------------------------------------------------- */
   BOOST_FIXTURE_TEST_CASE_TEMPLATE(Constructor_test, Fix, fixlist, Fix) {
     Communicator & comm = MPIContext::get_context().comm;
     if (Fix::serial_engine && comm.size() > 1) {
       return;
     } else {
       BOOST_CHECK_NO_THROW(
-          Fix::engine.initialise(Fix::NbComponents, FFT_PlanFlags::estimate));
+          Fix::engine.create_plan(Fix::NbComponents));
     }
     BOOST_CHECK_EQUAL(comm.sum(Fix::engine.size()),
                       muGrid::CcoordOps::get_size(Fix::res()));
   }
 
   /* ---------------------------------------------------------------------- */
   BOOST_FIXTURE_TEST_CASE_TEMPLATE(fft_test, Fix, fixlist, Fix) {
     if (Fix::serial_engine && Fix::engine.get_communicator().size() > 1) {
       // dont test serial engies in parallel
       return;
     } else {
-      Fix::engine.initialise(Fix::NbComponents, FFT_PlanFlags::estimate);
+      Fix::engine.create_plan(Fix::NbComponents);
     }
     using FC_t = muGrid::GlobalFieldCollection;
     FC_t fc{Fix::sdim};
     auto & input{fc.register_real_field("input", Fix::sdim * Fix::sdim)};
     auto & ref{fc.register_real_field("reference", Fix::sdim * Fix::sdim)};
     auto & result{fc.register_real_field("result", Fix::sdim * Fix::sdim)};
 
-    fc.initialise(Fix::engine.get_nb_subdomain_grid_pts(),
+    fc.initialise(Fix::engine.get_nb_domain_grid_pts(),
+                  Fix::engine.get_nb_subdomain_grid_pts(),
                   Fix::engine.get_subdomain_locations());
 
     using map_t = muGrid::MatrixFieldMap<Real, Mapping::Mut, Fix::sdim,
                                          Fix::sdim, IterUnit::Pixel>;
     map_t inmap{input};
     auto refmap{map_t{ref}};
     auto resultmap{map_t{result}};
@@ -199,52 +208,10 @@
       if (error > tol) {
         std::cout << result.array() / reference.array() << std::endl
                   << std::endl;
       }
     }
   }
 
-  /* ---------------------------------------------------------------------- */
-  BOOST_AUTO_TEST_CASE(gather_test) {
-    auto & comm{MPIContext::get_context().comm};
-    auto rank{comm.rank()};
-    const Dim_t nb_cols = rank + 1;
-    Eigen::Matrix<Real, Eigen::Dynamic, Eigen::Dynamic> send_mat(2, nb_cols);
-
-    for (int col{0}; col < nb_cols; ++col) {
-      send_mat.col(col) = send_mat.col(col).Ones(2, 1) * (rank + col);
-    }
-
-    auto res{comm.template gather<Real>(send_mat)};
-    int counter{0};
-    for (int lrank{0}; lrank < comm.size(); ++lrank) {
-      for (int col{0}; col < lrank + 1; ++col) {
-        BOOST_CHECK_EQUAL(res(0, counter), lrank + col);
-        counter++;
-      }
-    }
-  }
-
-  /* ---------------------------------------------------------------------- */
-  BOOST_AUTO_TEST_CASE(sum_mat_test) {
-    auto & comm{MPIContext::get_context().comm};
-    auto nb_cores{comm.size()};
-    Eigen::Matrix<Real, Eigen::Dynamic, Eigen::Dynamic> send_mat(2, 3);
-    send_mat(0, 0) = 1.;
-    send_mat(0, 1) = 2.;
-    send_mat(0, 2) = 3.;
-    send_mat(1, 0) = 4.;
-    send_mat(1, 1) = 5.;
-    send_mat(1, 2) = 6.;
-    auto res{comm.template sum_mat<Real>(send_mat)};
-    const auto nb_cols{send_mat.cols()};
-    const auto nb_rows{send_mat.rows()};
-    for (int row{0}; row < nb_rows; row++) {
-      for (int col{0}; col < nb_cols; col++) {
-        BOOST_CHECK_EQUAL(res(row, col), (row * nb_cols + col + 1) * nb_cores);
-      }
-    }
-  }
-
   BOOST_AUTO_TEST_SUITE_END();
 
 }  // namespace muFFT
```

### Comparing `muFFT-0.9.3/tests/libmufft/python_derivative_tests.py` & `mufft-0.90.0/tests/python_derivative_tests.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,42 +32,123 @@
 with proprietary FFT implementations or numerical libraries, containing parts
 covered by the terms of those libraries' licenses, the licensors of this
 Program grant you additional permission to convey the resulting work.
 """
 
 import unittest
 import numpy as np
+import itertools
+
+import muFFT
+
+
+class DerivativeCheck1d(unittest.TestCase):
+    def setUp(self):
+        self.nb_pts = [23]
+        np.random.seed(7)
+        self.field = np.empty(self.nb_pts, order='f')
+        self.field[:] = np.random.random(self.nb_pts)
+        self.fft = muFFT.FFT(self.nb_pts)
+        self.nb_dof = 1
+        self.fft.create_plan(self.nb_dof)
+        self.fourier_field = self.fft.register_fourier_space_field(
+            "fft_workspace", self.nb_dof)
+        self.fft.fft(self.field, self.fourier_field)
+
+    def test_upwind_differences(self):
+        diffop = muFFT.Stencils1D.upwind
+        q = self.fft.fftfreq
+        d = diffop.fourier(q)
+        diff_field = np.zeros_like(self.field, order='f')
+        self.fft.ifft(d * self.fourier_field, diff_field)
+        diff_field *= self.fft.normalisation
+        nx, = self.nb_pts
+        diff_field = np.squeeze(diff_field)
+        for x in range(nx):
+            ndiff = self.field[(x+1) % nx] - self.field[x]
+            ndiff = np.squeeze(ndiff)
+            self.assertAlmostEqual(diff_field[x], ndiff)
+
+    def test_central_differences(self):
+        diffop = muFFT.Stencils1D.central
+        q = self.fft.fftfreq
+        d = diffop.fourier(q)
+        diff_field = np.zeros_like(self.field, order='f')
+        self.fft.ifft(d * self.fourier_field, diff_field)
+        diff_field *= self.fft.normalisation
+        nx, = self.nb_pts
+        diff_field = np.squeeze(diff_field)
+        for x in range(nx):
+            ndiff = (self.field[(x+1) % nx] - self.field[(x-1) % nx])/2
+            ndiff = np.squeeze(ndiff)
+            self.assertAlmostEqual(diff_field[x], ndiff)
+
+    def test_central_2nd_differences(self):
+        diffop = muFFT.Stencils1D.central_2nd
+        q = self.fft.fftfreq
+        d = diffop.fourier(q)
+        diff_field = np.zeros_like(self.field, order='f')
+        self.fft.ifft(d * self.fourier_field, diff_field)
+        diff_field *= self.fft.normalisation
+        nx, = self.nb_pts
+        diff_field = np.squeeze(diff_field)
+        for x in range(nx):
+            ndiff = self.field[(x+1) % nx] - 2*self.field[x] \
+                + self.field[(x-1) % nx]
+            ndiff = np.squeeze(ndiff)
+            self.assertAlmostEqual(diff_field[x], ndiff)
+
+    def test_sixth_order_central_differences(self):
+        diffop = muFFT.Stencil1D.central6
+        q = self.fft.fftfreq
+        d = diffop.fourier(q)
+        diff_field = np.zeros_like(self.field, order='f')
+        self.fft.ifft(d * self.fourier_field, diff_field)
+        diff_field *= self.fft.normalisation
+        nx, = self.nb_pts
+        diff_field = np.squeeze(diff_field)
+        for x in range(nx):
+            ndiff = - 1/60*self.field[(x-3) % nx] \
+                    + 3/20*self.field[(x-2) % nx] \
+                    - 3/4*self.field[(x-1) % nx] \
+                    + 3/4*self.field[(x+1) % nx] \
+                    - 3/20*self.field[(x+2) % nx] \
+                    + 1/60*self.field[(x+3) % nx]
+            ndiff = np.squeeze(ndiff)
+            self.assertAlmostEqual(diff_field[x], ndiff)
 
-from python_test_imports import muFFT
 
 class DerivativeCheck2d(unittest.TestCase):
     def setUp(self):
         self.nb_pts = [23, 27]
         np.random.seed(7)
         self.field = np.empty(self.nb_pts, order='f')
         self.field[:] = np.random.random(self.nb_pts)
         self.fft = muFFT.FFT(self.nb_pts)
         self.nb_dof = 1
-        self.fft.initialise(self.nb_dof)
+        self.fft.create_plan(self.nb_dof)
         self.fourier_field = self.fft.register_fourier_space_field(
             "fft_workspace", self.nb_dof)
         self.fft.fft(self.field, self.fourier_field)
 
     def test_rollaxis(self):
         dz = muFFT.DiscreteDerivative([0, 0, 0], [[[-1, 1]]])
         self.assertTrue(dz.stencil.flags.owndata)
         self.assertTrue(np.allclose(dz.stencil[0, 0, :], [-1, 1]))
+        self.assertTrue(np.allclose(dz.lbounds, [0, 0, 0]))
 
         dy = dz.rollaxes(-1)
         self.assertTrue(np.allclose(dy.stencil[0, :, 0], [-1, 1]))
         self.assertTrue(np.allclose(dy.stencil, [[[-1], [1]]]))
+        self.assertTrue(np.allclose(dy.lbounds, [0, 0, 0]))
 
         dx = dy.rollaxes(-1)
         self.assertTrue(np.allclose(dx.stencil[:, 0, 0], [-1, 1]))
         self.assertTrue(np.allclose(dx.stencil, [[[-1]], [[1]]]))
+        self.assertTrue(np.allclose(dx.lbounds, [0, 0, 0]))
 
         dx = muFFT.DiscreteDerivative([0, 0], [[-0.5, 0.5],
                                                [-0.5, 0.5]])
         dy = dx.rollaxes(-1)
         self.assertTrue(np.allclose(dy.stencil.reshape((2, 2)),
                                     [[-0.5, -0.5],
                                      [ 0.5,  0.5]]))
@@ -93,50 +174,50 @@
         d = diffop.fourier(q)
         fourier_field_copy = np.copy(self.fourier_field)
         diff_field = np.zeros_like(self.field, order='f')
         ndiff = np.zeros_like(self.field, order='f')
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         self.fft.ifft(1j*2*np.pi*q[0] * fourier_field_copy, ndiff)
-        ndiff *=  self.fft.normalisation
+        ndiff *= self.fft.normalisation
         nx, ny = self.nb_pts
         diff_field = np.squeeze(diff_field)
         ndiff = np.squeeze(ndiff)
         for x in range(nx):
             for y in range(ny):
-                self.assertAlmostEqual(diff_field[x,y], ndiff[x,y])
+                self.assertAlmostEqual(diff_field[x, y], ndiff[x, y])
 
     def test_fourier_derivative_2_corner(self):
-        #shift the fourier derivative into the lower left shift=[-1/6, -1/6]
-        #corner. (Here the grid spacing is 1 in each direction, otherwise one
-        #should consider it to give the real space shift correct.)
+        # shift the fourier derivative into the lower left shift=[-1/6, -1/6]
+        # corner. (Here the grid spacing is 1 in each direction, otherwise one
+        # should consider it to give the real space shift correct.)
         shift = np.array([-1/6, -1/6])
         diffop = muFFT.FourierDerivative(2, 0, shift)
         q = self.fft.fftfreq
         d = diffop.fourier(q)
         fourier_field_copy = np.copy(self.fourier_field)
         diff_field = np.zeros_like(self.field, order='f')
         ndiff = np.zeros_like(self.field, order='f')
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         self.fft.ifft(1j*2*np.pi*q[0] *
-                              np.exp(1j*2*np.pi*np.einsum("i,i...->...", shift, q)) *
-                              fourier_field_copy, ndiff)
+                      np.exp(1j*2*np.pi*np.einsum("i,i...->...", shift, q)) *
+                      fourier_field_copy, ndiff)
         ndiff *= self.fft.normalisation
         nx, ny = self.nb_pts
         diff_field = np.squeeze(diff_field)
         ndiff = np.squeeze(ndiff)
         for x in range(nx):
             for y in range(ny):
-                self.assertAlmostEqual(diff_field[x,y], ndiff[x,y])
+                self.assertAlmostEqual(diff_field[x, y], ndiff[x, y])
 
     def test_fourier_derivative_2_full(self):
-        #shift the fourier derivative by one grid point in x- and y-direction
-        #shift=[1, 1]. (Here the grid spacing is 1 in each direction, otherwise
-        #one should consider it to give the real space shift correct.)
+        # shift the fourier derivative by one grid point in x- and y-direction
+        # shift=[1, 1]. (Here the grid spacing is 1 in each direction, other-
+        # wise one should consider it to give the real space shift correct.)
         shift = np.array([1, 1])
         diffop = muFFT.FourierDerivative(2, 0, shift)
         q = self.fft.fftfreq
         d = diffop.fourier(q)
         fourier_field_copy = np.copy(self.fourier_field)
         diff_field = np.zeros_like(self.field, order='f')
         ndiff = np.zeros_like(self.field, order='f')
@@ -145,121 +226,126 @@
         self.fft.ifft(1j*2*np.pi*q[0] * fourier_field_copy, ndiff)
         ndiff *= self.fft.normalisation
         nx, ny = self.nb_pts
         diff_field = np.squeeze(diff_field)
         ndiff = np.squeeze(ndiff)
         for x in range(nx):
             for y in range(ny):
-                self.assertAlmostEqual(diff_field[x,y], ndiff[(x+1)%nx, (y+1)%ny])
+                self.assertAlmostEqual(diff_field[x, y],
+                                       ndiff[(x+1) % nx, (y+1) % ny])
 
     def test_upwind_differences_x(self):
         diffop = muFFT.Stencils2D.upwind_x
         q = self.fft.fftfreq
         d = diffop.fourier(q)
         diff_field = np.zeros_like(self.field, order='f')
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
-                ndiff = self.field[(x+1)%nx, y] - self.field[x, y]
+                ndiff = self.field[(x+1) % nx, y] - self.field[x, y]
                 ndiff = np.squeeze(ndiff)
                 self.assertAlmostEqual(diff_field[x, y], ndiff)
 
     def test_upwind_differences_y(self):
         diffop = muFFT.Stencils2D.upwind_y
         q = self.fft.fftfreq
         d = diffop.fourier(q)
         diff_field = np.zeros_like(self.field, order='f')
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
-                ndiff = self.field[x, (y+1)%ny] - self.field[x, y]
+                ndiff = self.field[x, (y+1) % ny] - self.field[x, y]
                 ndiff = np.squeeze(ndiff)
                 self.assertAlmostEqual(diff_field[x, y], ndiff)
 
     def test_d_11_01(self):
         diffop = muFFT.Stencils2D.d_11_01
         q = self.fft.fftfreq
         d = diffop.fourier(q)
         diff_field = np.zeros_like(self.field, order='f')
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
-                ndiff = self.field[(x+1)%nx, (y+1)%ny] - self.field[x, (y+1)%ny]
+                ndiff = self.field[(x+1) % nx, (y+1) % ny] \
+                    - self.field[x, (y+1) % ny]
                 ndiff = np.squeeze(ndiff)
                 self.assertAlmostEqual(diff_field[x, y], ndiff)
 
     def test_d_11_10(self):
         diffop = muFFT.Stencils2D.d_11_10
         q = self.fft.fftfreq
         d = diffop.fourier(q)
         diff_field = np.zeros_like(self.field, order='f')
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
-                ndiff = self.field[(x+1)%nx, (y+1)%ny] - self.field[(x+1)%nx, y]
+                ndiff = self.field[(x+1) % nx, (y+1) % ny] \
+                    - self.field[(x+1) % nx, y]
                 ndiff = np.squeeze(ndiff)
                 self.assertAlmostEqual(diff_field[x, y], ndiff)
 
     def test_upwind_differences_y2(self):
         diffop = muFFT.DiscreteDerivative([0, 0], [[-1, 1],
-                                                   [ 0, 0]])
+                                                   [0,  0]])
         q = self.fft.fftfreq
         d = diffop.fourier(q)
         diff_field = np.zeros_like(self.field, order='f')
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
-                ndiff = self.field[x, (y+1)%ny] - self.field[x, y]
+                ndiff = self.field[x, (y+1) % ny] - self.field[x, y]
                 ndiff = np.squeeze(ndiff)
                 self.assertAlmostEqual(diff_field[x, y], ndiff)
 
     def test_shifted_upwind_differences_y(self):
-        diffop = muFFT.DiscreteDerivative([0, 0], [[ 0, 0],
+        diffop = muFFT.DiscreteDerivative([0, 0], [[0,  0],
                                                    [-1, 1]])
         q = self.fft.fftfreq
         d = diffop.fourier(q)
         diff_field = np.zeros_like(self.field, order='f')
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
-                ndiff = self.field[(x+1)%nx, (y+1)%ny] - self.field[(x+1)%nx, y]
+                ndiff = self.field[(x+1) % nx, (y+1) % ny] \
+                    - self.field[(x+1) % nx, y]
                 ndiff = np.squeeze(ndiff)
                 self.assertAlmostEqual(diff_field[x, y], ndiff)
 
     def test_averaged_upwind_differences_x(self):
         diffop = muFFT.Stencils2D.averaged_upwind_x
         q = self.fft.fftfreq
         d = diffop.fourier(q)
         diff_field = np.zeros_like(self.field, order='f')
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
-                ndiff = (self.field[(x+1)%nx, y] - self.field[x, y] \
-                         + self.field[(x+1)%nx, (y+1)%ny] - self.field[x, (y+1)%ny])/2
+                ndiff = (self.field[(x+1) % nx, y] - self.field[x, y]
+                         + self.field[(x+1) % nx, (y+1) % ny]
+                         - self.field[x, (y+1) % ny])/2
                 ndiff = np.squeeze(ndiff)
                 self.assertAlmostEqual(diff_field[x, y], ndiff)
 
     def test_averaged_upwind_differences_y(self):
         diffop = muFFT.Stencils2D.averaged_upwind_y
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -267,78 +353,188 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
 
         nx, ny = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
-                ndiff = (self.field[x, (y+1)%ny] - self.field[x, y] \
-                         + self.field[(x+1)%nx, (y+1)%ny] - self.field[(x+1)%nx, y])/2
+                ndiff = (self.field[x, (y+1) % ny] - self.field[x, y]
+                         + self.field[(x+1) % nx, (y+1) % ny]
+                         - self.field[(x+1) % nx, y])/2
                 ndiff = np.squeeze(ndiff)
                 self.assertAlmostEqual(diff_field[x, y], ndiff)
 
     def test_central_differences_x(self):
         diffop = muFFT.Stencils2D.central_x
         q = self.fft.fftfreq
         d = diffop.fourier(q)
         diff_field = np.zeros_like(self.field, order='f')
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
-                ndiff = (self.field[(x+1)%nx, y] - self.field[(x-1)%nx, y])/2
+                ndiff = (self.field[(x+1) % nx, y]
+                         - self.field[(x-1) % nx, y])/2
                 ndiff = np.squeeze(ndiff)
                 self.assertAlmostEqual(diff_field[x, y], ndiff)
 
     def test_central_differences_y(self):
         diffop = muFFT.Stencils2D.central_y
         q = self.fft.fftfreq
         d = diffop.fourier(q)
         diff_field = np.zeros_like(self.field, order='f')
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
-                ndiff = (self.field[x, (y+1)%ny] - self.field[x, (y-1)%ny])/2
+                ndiff = (self.field[x, (y+1) % ny]
+                         - self.field[x, (y-1) % ny])/2
                 ndiff = np.squeeze(ndiff)
                 self.assertAlmostEqual(diff_field[x, y], ndiff)
 
     def test_sixth_order_central_differences(self):
         diffop = muFFT.DiscreteDerivative([0, -3],
                                           [[-1/60, 3/20, -3/4, 0,
                                             3/4, -3/20, 1/60]])
+        self.assertTrue(np.allclose(diffop.lbounds, [0, -3]))
+        q = self.fft.fftfreq
+        d = diffop.fourier(q)
+        diff_field = np.zeros_like(self.field, order='f')
+        self.fft.ifft(d * self.fourier_field, diff_field)
+        diff_field *= self.fft.normalisation
+        nx, ny = self.nb_pts
+        diff_field = np.squeeze(diff_field)
+        for x in range(nx):
+            for y in range(ny):
+                ndiff = -1/60*self.field[x, (y-3) % ny] \
+                    + 3/20*self.field[x, (y-2) % ny] \
+                    - 3/4*self.field[x, (y-1) % ny] \
+                    + 3/4*self.field[x, (y+1) % ny] \
+                    - 3/20*self.field[x, (y+2) % ny] \
+                    + 1/60*self.field[x, (y+3) % ny]
+                ndiff = np.squeeze(ndiff)
+                self.assertAlmostEqual(diff_field[x, y], ndiff)
+
+    def test_central_2nd_differences_x(self):
+        diffop = muFFT.Stencils2D.central_2nd_x
         q = self.fft.fftfreq
         d = diffop.fourier(q)
         diff_field = np.zeros_like(self.field, order='f')
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny = self.nb_pts
+
+    def test_convenience_interface_discrete_deriv(self):
+        assert self.nb_dof == 1
+        diffop = muFFT.Stencils2D.upwind_x
+        field = self.field.reshape(self.nb_pts, order='F')
+        diff_field = diffop.apply(field)
+        print('diff_field[0, 0] (python):', diff_field[0, 0])
         diff_field = np.squeeze(diff_field)
+        nx, ny = self.nb_pts
         for x in range(nx):
             for y in range(ny):
-                ndiff = -1/60*self.field[x, (y-3)%ny] \
-                    +3/20*self.field[x, (y-2)%ny] \
-                    -3/4*self.field[x, (y-1)%ny] \
-                    +3/4*self.field[x, (y+1)%ny] \
-                    -3/20*self.field[x, (y+2)%ny] \
-                    +1/60*self.field[x, (y+3)%ny]
+                ndiff = self.field[(x+1) % nx, y] - self.field[x, y]
+                if x == 0 and y == 0:
+                    print('ndiff:', ndiff)
                 ndiff = np.squeeze(ndiff)
                 self.assertAlmostEqual(diff_field[x, y], ndiff)
 
+    def test_central_2nd_differences_y(self):
+        diffop = muFFT.Stencils2D.central_2nd_y
+        q = self.fft.fftfreq
+        d = diffop.fourier(q)
+        diff_field = np.zeros_like(self.field, order='f')
+        self.fft.ifft(d * self.fourier_field, diff_field)
+        diff_field *= self.fft.normalisation
+        nx, ny = self.nb_pts
+        diff_field = np.squeeze(diff_field)
+        for x in range(nx):
+            for y in range(ny):
+                ndiff = self.field[x, (y+1) % ny] - 2*self.field[x, y] \
+                    + self.field[x, (y-1) % ny]
+                ndiff = np.squeeze(ndiff)
+                self.assertAlmostEqual(diff_field[x, y], ndiff)
+
+    def test_hexagonal_T1_dx(self):
+        diffop = muFFT.Stencils2D.hexagonal_T1_dx
+        q = self.fft.fftfreq
+        d = diffop.fourier(q)
+        diff_field = np.zeros_like(self.field, order='f')
+        self.fft.ifft(d * self.fourier_field, diff_field)
+        diff_field *= self.fft.normalisation
+        nx, ny = self.nb_pts
+        diff_field = np.squeeze(diff_field)
+        for x in range(nx):
+            for y in range(ny):
+                ndiff = self.field[(x+1) % nx, y] - self.field[x, y]
+                ndiff = np.squeeze(ndiff)
+                self.assertAlmostEqual(diff_field[x, y], ndiff)
+
+    def test_hexagonal_T1_dy(self):
+        diffop = muFFT.Stencils2D.hexagonal_T1_dy
+        q = self.fft.fftfreq
+        d = diffop.fourier(q)
+        diff_field = np.zeros_like(self.field, order='f')
+        self.fft.ifft(d * self.fourier_field, diff_field)
+        diff_field *= self.fft.normalisation
+        nx, ny = self.nb_pts
+        diff_field = np.squeeze(diff_field)
+        for x in range(nx):
+            for y in range(ny):
+                ndiff = 1/2*(2*self.field[x, (y+1) % ny] - self.field[x, y]
+                             - self.field[(x+1) % nx, y])
+                ndiff = np.squeeze(ndiff)
+                self.assertAlmostEqual(diff_field[x, y], ndiff)
+
+    def test_hexagonal_T2_dx(self):
+        diffop = muFFT.Stencils2D.hexagonal_T2_dx
+        q = self.fft.fftfreq
+        d = diffop.fourier(q)
+        diff_field = np.zeros_like(self.field, order='f')
+        self.fft.ifft(d * self.fourier_field, diff_field)
+        diff_field *= self.fft.normalisation
+        nx, ny = self.nb_pts
+        diff_field = np.squeeze(diff_field)
+        for x in range(nx):
+            for y in range(ny):
+                ndiff = self.field[(x+1) % nx, (y+1) % ny] \
+                    - self.field[x, (y+1) % ny]
+                ndiff = np.squeeze(ndiff)
+                self.assertAlmostEqual(diff_field[x, y], ndiff)
+
+    def test_hexagonal_T2_dy(self):
+        diffop = muFFT.Stencils2D.hexagonal_T2_dy
+        q = self.fft.fftfreq
+        d = diffop.fourier(q)
+        diff_field = np.zeros_like(self.field, order='f')
+        self.fft.ifft(d * self.fourier_field, diff_field)
+        diff_field *= self.fft.normalisation
+        nx, ny = self.nb_pts
+        diff_field = np.squeeze(diff_field)
+        for x in range(nx):
+            for y in range(ny):
+                ndiff = 1/2*(-2*self.field[(x+1) % nx, y]
+                             + self.field[x, (y+1) % ny]
+                             + self.field[(x+1) % nx, (y+1) % ny])
+                ndiff = np.squeeze(ndiff)
+                self.assertAlmostEqual(diff_field[x, y], ndiff)
+
+
 class DerivativeCheck3d(unittest.TestCase):
     def setUp(self):
         self.nb_pts = [23, 23, 17]
         self.field = np.random.random(self.nb_pts)
         self.fft = muFFT.FFT(self.nb_pts)
         self.nb_dof = 1
-        self.fft.initialise(self.nb_dof)
+        self.fft.create_plan(self.nb_dof)
         self.fourier_field = self.fft.register_fourier_space_field(
             "fft_workspace", self.nb_dof)
         self.fft.fft(self.field, self.fourier_field)
 
     def test_upwind_differences_x(self):
         diffop = muFFT.Stencils3D.upwind_x
         q = self.fft.fftfreq
@@ -347,15 +543,15 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[(x+1)%nx, y, z] - self.field[x, y, z]
+                    ndiff = self.field[(x+1) % nx, y, z] - self.field[x, y, z]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_upwind_differences_y(self):
         diffop = muFFT.Stencils3D.upwind_y
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -363,15 +559,15 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[x, (y+1)%ny, z] - self.field[x, y, z]
+                    ndiff = self.field[x, (y+1) % ny, z] - self.field[x, y, z]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_upwind_differences_z(self):
         diffop = muFFT.Stencils3D.upwind_z
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -379,15 +575,15 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[x, y, (z+1)%nz] - self.field[x, y, z]
+                    ndiff = self.field[x, y, (z+1) % nz] - self.field[x, y, z]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_d_100_000(self):
         diffop = muFFT.Stencils3D.d_100_000
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -395,15 +591,15 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[(x+1)%nx, y, z] - self.field[x, y, z]
+                    ndiff = self.field[(x+1) % nx, y, z] - self.field[x, y, z]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_d_110_010(self):
         diffop = muFFT.Stencils3D.d_110_010
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -411,15 +607,16 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[(x+1)%nx, (y+1)%ny, z] - self.field[x, (y+1)%ny, z]
+                    ndiff = self.field[(x+1) % nx, (y+1) % ny, z] \
+                        - self.field[x, (y+1) % ny, z]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_d_111_011(self):
         diffop = muFFT.Stencils3D.d_111_011
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -427,15 +624,16 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[(x+1)%nx, (y+1)%ny, (z+1)%nz] - self.field[x, (y+1)%ny, (z+1)%nz]
+                    ndiff = self.field[(x+1) % nx, (y+1) % ny, (z+1) % nz] \
+                        - self.field[x, (y+1) % ny, (z+1) % nz]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_d_101_001(self):
         diffop = muFFT.Stencils3D.d_101_001
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -443,15 +641,16 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[(x+1)%nx, y, (z+1)%nz] - self.field[x, y, (z+1)%nz]
+                    ndiff = self.field[(x+1) % nx, y, (z+1) % nz] \
+                        - self.field[x, y, (z+1) % nz]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_d_010_000(self):
         diffop = muFFT.Stencils3D.d_010_000
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -459,15 +658,15 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[x, (y+1)%ny, z] - self.field[x, y, z]
+                    ndiff = self.field[x, (y+1) % ny, z] - self.field[x, y, z]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_d_110_100(self):
         diffop = muFFT.Stencils3D.d_110_100
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -475,32 +674,33 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[(x+1)%nx, (y+1)%ny, z] - self.field[(x+1)%nx, y, z]
+                    ndiff = self.field[(x+1) % nx, (y+1) % ny, z] \
+                        - self.field[(x+1) % nx, y, z]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
-
     def test_d_111_101(self):
         diffop = muFFT.Stencils3D.d_111_101
         q = self.fft.fftfreq
         d = diffop.fourier(q)
         diff_field = np.zeros_like(self.field, order='f')
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[(x+1)%nx, (y+1)%ny, (z+1)%nz] - self.field[(x+1)%nx, y, (z+1)%nz]
+                    ndiff = self.field[(x+1) % nx, (y+1) % ny, (z+1) % nz] \
+                        - self.field[(x+1) % nx, y, (z+1) % nz]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_d_011_001(self):
         diffop = muFFT.Stencils3D.d_011_001
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -508,15 +708,16 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[x, (y+1)%ny, (z+1)%nz] - self.field[x, y, (z+1)%nz]
+                    ndiff = self.field[x, (y+1) % ny, (z+1) % nz] \
+                        - self.field[x, y, (z+1) % nz]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_d_001_000(self):
         diffop = muFFT.Stencils3D.d_001_000
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -524,15 +725,15 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[x, y, (z+1)%nz] - self.field[x, y, z]
+                    ndiff = self.field[x, y, (z+1) % nz] - self.field[x, y, z]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_d_101_100(self):
         diffop = muFFT.Stencils3D.d_101_100
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -540,15 +741,16 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[(x+1)%nx, y, (z+1)%nz] - self.field[(x+1)%nx, y, z]
+                    ndiff = self.field[(x+1) % nx, y, (z+1) % nz] \
+                        - self.field[(x+1) % nx, y, z]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_d_111_110(self):
         diffop = muFFT.Stencils3D.d_111_110
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -556,15 +758,16 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[(x+1)%nx, (y+1)%ny, (z+1)%nz] - self.field[(x+1)%nx, (y+1)%ny, z]
+                    ndiff = self.field[(x+1) % nx, (y+1) % ny, (z+1) % nz] \
+                        - self.field[(x+1) % nx, (y+1) % ny, z]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_d_011_010(self):
         diffop = muFFT.Stencils3D.d_011_010
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -572,15 +775,16 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = self.field[x, (y+1)%ny, (z+1)%nz] - self.field[x, (y+1)%ny, z]
+                    ndiff = self.field[x, (y+1) % ny, (z+1) % nz] \
+                        - self.field[x, (y+1) % ny, z]
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_averaged_upwind_differences_x(self):
         diffop = muFFT.Stencils3D.averaged_upwind_x
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -588,18 +792,21 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = (self.field[(x+1)%nx, y, z] - self.field[x, y, z] \
-                             + self.field[(x+1)%nx, (y+1)%ny, z] - self.field[x, (y+1)%ny, z] \
-                             + self.field[(x+1)%nx, y, (z+1)%nz] - self.field[x, y, (z+1)%nz] \
-                             + self.field[(x+1)%nx, (y+1)%ny, (z+1)%nz] - self.field[x, (y+1)%ny, (z+1)%nz])/4
+                    ndiff = (self.field[(x+1) % nx, y, z] - self.field[x, y, z]
+                             + self.field[(x+1) % nx, (y+1) % ny, z]
+                             - self.field[x, (y+1) % ny, z]
+                             + self.field[(x+1) % nx, y, (z+1) % nz]
+                             - self.field[x, y, (z+1) % nz]
+                             + self.field[(x+1) % nx, (y+1) % ny, (z+1) % nz]
+                             - self.field[x, (y+1) % ny, (z+1) % nz])/4
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_averaged_upwind_differences_y(self):
         diffop = muFFT.Stencils3D.averaged_upwind_y
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -607,18 +814,22 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = (self.field[x, (y+1)%ny, z] - self.field[x, y, z] \
-                             + self.field[(x+1)%nx, (y+1)%ny, z] - self.field[(x+1)%nx, y, z] \
-                             + self.field[x, (y+1)%ny, (z+1)%nz] - self.field[x, y, (z+1)%nz] \
-                             + self.field[(x+1)%nx, (y+1)%ny, (z+1)%nz] - self.field[(x+1)%nx, y, (z+1)%nz])/4
+                    ndiff = (self.field[x, (y+1) % ny, z]
+                             - self.field[x, y, z]
+                             + self.field[(x+1) % nx, (y+1) % ny, z]
+                             - self.field[(x+1) % nx, y, z]
+                             + self.field[x, (y+1) % ny, (z+1) % nz]
+                             - self.field[x, y, (z+1) % nz]
+                             + self.field[(x+1) % nx, (y+1) % ny, (z+1) % nz]
+                             - self.field[(x+1) % nx, y, (z+1) % nz])/4
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_averaged_upwind_differences_z(self):
         diffop = muFFT.Stencils3D.averaged_upwind_z
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -626,18 +837,22 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = (self.field[x, y, (z+1)%nz] - self.field[x, y, z] \
-                             + self.field[(x+1)%nx, y, (z+1)%nz] - self.field[(x+1)%nx, y, z] \
-                             + self.field[x, (y+1)%ny, (z+1)%nz] - self.field[x, (y+1)%ny, z] \
-                             + self.field[(x+1)%nx, (y+1)%ny, (z+1)%nz] - self.field[(x+1)%nx, (y+1)%ny, z])/4
+                    ndiff = (self.field[x, y, (z+1) % nz]
+                             - self.field[x, y, z]
+                             + self.field[(x+1) % nx, y, (z+1) % nz]
+                             - self.field[(x+1) % nx, y, z]
+                             + self.field[x, (y+1) % ny, (z+1) % nz]
+                             - self.field[x, (y+1) % ny, z]
+                             + self.field[(x+1) % nx, (y+1) % ny, (z+1) % nz]
+                             - self.field[(x+1) % nx, (y+1) % ny, z])/4
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_central_differences_x(self):
         diffop = muFFT.Stencils3D.central_x
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -645,15 +860,16 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = (self.field[(x+1)%nx, y, z] - self.field[(x-1)%nx, y, z])/2
+                    ndiff = (self.field[(x+1) % nx, y, z]
+                             - self.field[(x-1) % nx, y, z])/2
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_central_differences_y(self):
         diffop = muFFT.Stencils3D.central_y
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -661,15 +877,16 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = (self.field[x, (y+1)%ny, z] - self.field[x, (y-1)%ny, z])/2
+                    ndiff = (self.field[x, (y+1) % ny, z]
+                             - self.field[x, (y-1) % ny, z])/2
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
     def test_central_differences_z(self):
         diffop = muFFT.Stencils3D.central_z
         q = self.fft.fftfreq
         d = diffop.fourier(q)
@@ -677,13 +894,198 @@
         self.fft.ifft(d * self.fourier_field, diff_field)
         diff_field *= self.fft.normalisation
         nx, ny, nz = self.nb_pts
         diff_field = np.squeeze(diff_field)
         for x in range(nx):
             for y in range(ny):
                 for z in range(nz):
-                    ndiff = (self.field[x, y, (z+1)%nz] - self.field[x, y, (z-1)%nz])/2
+                    ndiff = (self.field[x, y, (z+1) % nz]
+                             - self.field[x, y, (z-1) % nz])/2
                     ndiff = np.squeeze(ndiff)
                     self.assertAlmostEqual(diff_field[x, y, z], ndiff)
 
+    def test_convenience_interface_discrete_deriv(self):
+        assert self.nb_dof == 1
+        diffop = muFFT.Stencils3D.central_z
+        field = self.field.reshape([*self.nb_pts], order='F')
+        diff_field = diffop.apply(field)
+        diff_field = np.squeeze(diff_field)
+        nx, ny, nz = self.nb_pts
+        for x in range(nx):
+            for y in range(ny):
+                for z in range(nz):
+                    ndiff = (self.field[x, y, (z+1) % nz]
+                             - self.field[x, y, (z-1) % nz])/2
+                    ndiff = np.squeeze(ndiff)
+                    self.assertAlmostEqual(diff_field[x, y, z], ndiff)
+
+    def test_five_tetraheda_T0_derivative_x(self):
+        diffop = muFFT.Stencils3D.linear_finite_elements_5[0]
+        q = self.fft.fftfreq
+        d = diffop.fourier(q)
+        diff_field = np.zeros_like(self.field, order='f')
+        self.fft.ifft(d * self.fourier_field, diff_field)
+        diff_field *= self.fft.normalisation
+        nx, ny, nz = self.nb_pts
+        diff_field = np.squeeze(diff_field)
+        for x in range(nx):
+            for y in range(ny):
+                for z in range(nz):
+                    ndiff = (self.field[(x+1) % nx, (y+1) % ny, (z+1) % nz]
+                             + self.field[(x+1) % nx, y, z]
+                             - self.field[x, (y+1) % ny, z]
+                             - self.field[x, y, (z+1) % nz])/2
+                    ndiff = np.squeeze(ndiff)
+                    self.assertAlmostEqual(diff_field[x, y, z], ndiff)
+
+    def test_five_tetraheda_T0_derivative_y(self):
+        diffop = muFFT.Stencils3D.linear_finite_elements_5[1]
+        q = self.fft.fftfreq
+        d = diffop.fourier(q)
+        diff_field = np.zeros_like(self.field, order='f')
+        self.fft.ifft(d * self.fourier_field, diff_field)
+        diff_field *= self.fft.normalisation
+        nx, ny, nz = self.nb_pts
+        diff_field = np.squeeze(diff_field)
+        for x in range(nx):
+            for y in range(ny):
+                for z in range(nz):
+                    ndiff = (self.field[(x+1) % nx, (y+1) % ny, (z+1) % nz]
+                             - self.field[(x+1) % nx, y, z]
+                             + self.field[x, (y+1) % ny, z]
+                             - self.field[x, y, (z+1) % nz])/2
+                    ndiff = np.squeeze(ndiff)
+                    self.assertAlmostEqual(diff_field[x, y, z], ndiff)
+
+    def test_five_tetraheda_T0_derivative_z(self):
+        diffop = muFFT.Stencils3D.linear_finite_elements_5[2]
+        q = self.fft.fftfreq
+        d = diffop.fourier(q)
+        diff_field = np.zeros_like(self.field, order='f')
+        self.fft.ifft(d * self.fourier_field, diff_field)
+        diff_field *= self.fft.normalisation
+        nx, ny, nz = self.nb_pts
+        diff_field = np.squeeze(diff_field)
+        for x in range(nx):
+            for y in range(ny):
+                for z in range(nz):
+                    ndiff = (self.field[(x+1) % nx, (y+1) % ny, (z+1) % nz]
+                             - self.field[(x+1) % nx, y, z]
+                             - self.field[x, (y+1) % ny, z]
+                             + self.field[x, y, (z+1) % nz])/2
+                    ndiff = np.squeeze(ndiff)
+                    self.assertAlmostEqual(diff_field[x, y, z], ndiff)
+
+    def test_six_regular_tetraheda(self):
+        def get_diff_field(element, direction):
+            deriv_n = 3*element + direction
+            diffop = muFFT.Stencils3D.linear_finite_elements_6_regular[deriv_n]
+            q = self.fft.fftfreq
+            d = diffop.fourier(q)
+            diff_field = np.zeros_like(self.field, order='f')
+            self.fft.ifft(d * self.fourier_field, diff_field)
+            diff_field *= self.fft.normalisation
+            diff_field = np.squeeze(diff_field)
+
+            return diff_field
+
+        direction_str = {"0": "x",
+                         "1": "y",
+                         "2": "z"}
+
+        def error_message(element, direction):
+            print(f"Derivative test for tetrahedra {element} fails in "
+                  f"{direction_str[str(direction)]}-direction.")
+
+        def test_derivative(diff_field, element, direction):
+            s = stencils[str(element)+str(direction)]
+
+            # derivative in x-direction
+            if direction == 0:
+                for x, y, z in itertools.product(
+                        range(nx), range(ny), range(nz)):
+                    ndiff = self.field[(x+s[0, 0]) % nx,
+                                       (y+s[0, 1]) % ny,
+                                       (z+s[0, 2]) % nz]
+                    ndiff -= self.field[(x+s[1, 0]) % nx,
+                                        (y+s[1, 1]) % ny,
+                                        (z+s[1, 2]) % nz]
+                    ndiff += 1/2*self.field[(x+s[2, 0]) % nx,
+                                            (y+s[2, 1]) % ny,
+                                            (z+s[2, 2]) % nz]
+                    ndiff -= 1/2*self.field[(x+s[3, 0]) % nx,
+                                            (y+s[3, 1]) % ny,
+                                            (z+s[3, 2]) % nz]
+
+                    ndiff = np.squeeze(ndiff)
+                    if round(diff_field[x, y, z], 7) - round(ndiff, 7) != 0:
+                        error_message(element, direction)
+                        self.assertAlmostEqual(diff_field[x, y, z], ndiff)
+                        continue  # skipp test for other field values
+            # derivative in y-direction
+            elif direction == 1:
+                for x, y, z in itertools.product(
+                        range(nx), range(ny), range(nz)):
+                    ndiff = self.field[(x+s[0, 0]) % nx,
+                                       (y+s[0, 1]) % ny,
+                                       (z+s[0, 2]) % nz]
+                    ndiff -= self.field[(x+s[1, 0]) % nx,
+                                        (y+s[1, 1]) % ny,
+                                        (z+s[1, 2]) % nz]
+                    ndiff += 2/3*self.field[(x+s[2, 0]) % nx,
+                                            (y+s[2, 1]) % ny,
+                                            (z+s[2, 2]) % nz]
+                    ndiff -= 2/3*self.field[(x+s[3, 0]) % nx,
+                                            (y+s[3, 1]) % ny,
+                                            (z+s[3, 2]) % nz]
+
+                    ndiff = np.squeeze(ndiff)
+                    if round(diff_field[x, y, z], 7) - round(ndiff, 7) != 0:
+                        error_message(element, direction)
+                        self.assertAlmostEqual(diff_field[x, y, z], ndiff)
+                        continue  # skipp test for other field values
+            # derivative in z-direction
+            elif direction == 2:
+                for x, y, z in itertools.product(
+                        range(nx), range(ny), range(nz)):
+                    ndiff = self.field[(x+s[0, 0]) % nx,
+                                       (y+s[0, 1]) % ny,
+                                       (z+s[0, 2]) % nz]
+                    ndiff -= self.field[(x+s[1, 0]) % nx,
+                                        (y+s[1, 1]) % ny,
+                                        (z+s[1, 2]) % nz]
+
+                    ndiff = np.squeeze(ndiff)
+                    if round(diff_field[x, y, z], 7) - round(ndiff, 7) != 0:
+                        error_message(element, direction)
+                        self.assertAlmostEqual(diff_field[x, y, z], ndiff)
+                        continue  # skipp test for other field values
+
+        nx, ny, nz = self.nb_pts
+        stencils = {
+            "00": np.array([[1, 0, 0], [0, 0, 0], [1, 0, 0], [1, 1, 0]]),
+            "01": np.array([[1, 1, 0], [1, 0, 0], [1, 1, 0], [1, 1, 1]]),
+            "02": np.array([[1, 1, 1], [1, 1, 0]]),
+            "10": np.array([[1, 0, 0], [0, 0, 0], [1, 0, 1], [1, 1, 1]]),
+            "11": np.array([[1, 1, 1], [1, 0, 1], [1, 0, 0], [1, 0, 1]]),
+            "12": np.array([[1, 0, 1], [1, 0, 0]]),
+            "20": np.array([[1, 1, 0], [0, 1, 0], [0, 0, 0], [0, 1, 0]]),
+            "21": np.array([[0, 1, 0], [0, 0, 0], [1, 1, 0], [1, 1, 1]]),
+            "22": np.array([[1, 1, 1], [1, 1, 0]]),
+            "30": np.array([[1, 1, 1], [0, 1, 1], [0, 0, 0], [0, 1, 0]]),
+            "31": np.array([[0, 1, 0], [0, 0, 0], [0, 1, 0], [0, 1, 1]]),
+            "32": np.array([[0, 1, 1], [0, 1, 0]]),
+            "40": np.array([[1, 0, 1], [0, 0, 1], [1, 0, 1], [1, 1, 1]]),
+            "41": np.array([[1, 1, 1], [1, 0, 1], [0, 0, 0], [0, 0, 1]]),
+            "42": np.array([[0, 0, 1], [0, 0, 0]]),
+            "50": np.array([[1, 1, 1], [0, 1, 1], [0, 0, 1], [0, 1, 1]]),
+            "51": np.array([[0, 1, 1], [0, 0, 1], [0, 0, 0], [0, 0, 1]]),
+            "52": np.array([[0, 0, 1], [0, 0, 0]])
+        }
+
+        for element, direction in itertools.product(range(6), range(3)):
+            diff_field = get_diff_field(element, direction)
+            test_derivative(diff_field, element, direction)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `muFFT-0.9.3/tests/libmufft/python_muFFT_license_test.py` & `mufft-0.90.0/tests/python_muFFT_license_test.py`

 * *Files identical despite different names*

### Comparing `muFFT-0.9.3/tests/libmufft/python_netcdf_tests.py` & `mufft-0.90.0/tests/python_netcdf_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,116 +33,120 @@
 covered by the terms of those libraries' licenses, the licensors of this
 Program grant you additional permission to convey the resulting work.
 """
 
 import unittest
 import numpy as np
 
-from netCDF4 import Dataset
+try:
+    from netCDF4 import Dataset
 
-from python_test_imports import muFFT
-from muFFT.NetCDF import NCStructuredGrid
+    import muFFT
+    from muFFT.NetCDF import NCStructuredGrid
 
-def build_test_classes(nb_grid_pts):
-    class NetCDF_Check(unittest.TestCase):
-        def setUp(self):
-            self.nb_grid_pts = nb_grid_pts
-            self.tensor_shape = tuple(list(self.nb_grid_pts) + [3, 3])
-            self.scalar_grid = np.arange(np.prod(self.nb_grid_pts)).reshape(self.nb_grid_pts)
-            self.tensor_grid = np.arange(np.prod(self.tensor_shape)) \
-                .reshape(self.tensor_shape)
-    
-            if muFFT.has_mpi:
-                from mpi4py import MPI
-                self.communicator = MPI.COMM_WORLD
-            else:
-                self.communicator = None
-            self.fft = muFFT.FFT(self.nb_grid_pts, fft='mpi',
-                                 communicator=self.communicator)
-
-        def test_write_read_domain(self):
-            if self.communicator is None:
-                nc = NCStructuredGrid('test_{}d.nc'.format(len(self.nb_grid_pts)), mode='w',
-                                      nb_domain_grid_pts=self.nb_grid_pts)
-            else:
-                nc = NCStructuredGrid('test_{}d.nc'.format(len(self.nb_grid_pts)), mode='w',
-                                      nb_domain_grid_pts=self.nb_grid_pts,
-                                      decomposition='domain',
-                                      subdomain_locations=self.fft.subdomain_locations,
-                                      nb_subdomain_grid_pts=self.fft.nb_subdomain_grid_pts,
-                                      communicator=self.communicator)
-            nc.scalar = self.scalar_grid
-            nc.tensor = self.tensor_grid
-            nc[3].per_frame_tensor = self.tensor_grid
-            nc.close()
-    
-            # Check that the file structure is correct
-            nc = Dataset('test_{}d.nc'.format(len(self.nb_grid_pts)), 'r')
-            dimensions = ['frame', 'grid_x', 'grid_y', 'tensor_3']
-            if len(self.nb_grid_pts) == 3:
-                dimensions += ['grid_z']
-            self.assertEqual(set(nc.dimensions), set(dimensions))
-            self.assertEqual(len(nc.dimensions['frame']), 4)
-            self.assertEqual(len(nc.dimensions['grid_x']), self.nb_grid_pts[0])
-            self.assertEqual(len(nc.dimensions['grid_y']), self.nb_grid_pts[1])
-            if len(self.nb_grid_pts) == 3:
-                self.assertEqual(len(nc.dimensions['grid_z']), self.nb_grid_pts[2])
-            self.assertEqual(len(nc.dimensions['tensor_3']), 3)
-            nc.close()
-    
-            # Read file and check data
-            nc = NCStructuredGrid('test_{}d.nc'.format(len(self.nb_grid_pts)), mode='r')
-            self.assertEqual(tuple(nc.nb_domain_grid_pts), tuple(self.nb_grid_pts))
-            self.assertTrue(np.equal(nc.scalar, self.scalar_grid).all())
-            self.assertTrue(np.equal(nc.tensor, self.tensor_grid).all())
-            self.assertTrue(np.equal(nc[3].per_frame_tensor, self.tensor_grid).all())
-            nc.close()
-
-        def test_write_read_subdomain(self):
-            scalar_grid = self.scalar_grid[self.fft.subdomain_slices]
-            tensor_grid = self.tensor_grid[self.fft.subdomain_slices]
-
-            if self.communicator is None:
-                nc = NCStructuredGrid('test_{}d.nc'.format(len(self.nb_grid_pts)), mode='w',
-                                      nb_domain_grid_pts=self.nb_grid_pts)
-            else:
-                nc = NCStructuredGrid('test_{}d.nc'.format(len(self.nb_grid_pts)), mode='w',
-                                      nb_domain_grid_pts=self.nb_grid_pts,
-                                      decomposition='subdomain',
-                                      subdomain_locations=self.fft.subdomain_locations,
-                                      nb_subdomain_grid_pts=self.fft.nb_subdomain_grid_pts,
-                                      communicator=self.communicator)
-            nc.scalar = scalar_grid
-            nc.tensor = tensor_grid
-            nc[3].per_frame_tensor = tensor_grid
-            nc.close()
-
-            # Check that the file structure is correct
-            nc = Dataset('test_{}d.nc'.format(len(self.nb_grid_pts)), 'r')
-            dimensions = ['frame', 'grid_x', 'grid_y', 'tensor_3']
-            if len(self.nb_grid_pts) == 3:
-                dimensions += ['grid_z']
-            self.assertEqual(set(nc.dimensions), set(dimensions))
-            self.assertEqual(len(nc.dimensions['frame']), 4)
-            self.assertEqual(len(nc.dimensions['grid_x']), self.nb_grid_pts[0])
-            self.assertEqual(len(nc.dimensions['grid_y']), self.nb_grid_pts[1])
-            if len(self.nb_grid_pts) == 3:
-                self.assertEqual(len(nc.dimensions['grid_z']), self.nb_grid_pts[2])
-            self.assertEqual(len(nc.dimensions['tensor_3']), 3)
-            nc.close()
-
-            # Read file and check data
-            nc = NCStructuredGrid('test_{}d.nc'.format(len(self.nb_grid_pts)), mode='r')
-            self.assertEqual(tuple(nc.nb_domain_grid_pts), tuple(self.nb_grid_pts))
-            self.assertTrue(np.equal(nc.scalar, self.scalar_grid).all())
-            self.assertTrue(np.equal(nc.tensor, self.tensor_grid).all())
-            self.assertTrue(np.equal(nc[3].per_frame_tensor, self.tensor_grid).all())
-            nc.close()
-
-    return NetCDF_Check
-
-# Check that it works with tuples or lists
-NetCDF_Check_2d = build_test_classes((11, 23))
-NetCDF_Check_3d = build_test_classes([11, 23, 7])
+    def build_test_classes(nb_grid_pts):
+        class NetCDF_Check(unittest.TestCase):
+            def setUp(self):
+                self.nb_grid_pts = nb_grid_pts
+                self.tensor_shape = tuple(list(self.nb_grid_pts) + [3, 3])
+                self.scalar_grid = np.arange(np.prod(self.nb_grid_pts)).reshape(self.nb_grid_pts)
+                self.tensor_grid = np.arange(np.prod(self.tensor_shape)) \
+                    .reshape(self.tensor_shape)
+
+                if muFFT.has_mpi:
+                    from mpi4py import MPI
+                    self.communicator = MPI.COMM_WORLD
+                else:
+                    self.communicator = None
+                self.fft = muFFT.FFT(self.nb_grid_pts, fft='mpi',
+                                     communicator=self.communicator)
+
+            def test_write_read_domain(self):
+                if self.communicator is None:
+                    nc = NCStructuredGrid('test_{}d.nc'.format(len(self.nb_grid_pts)), mode='w',
+                                          nb_domain_grid_pts=self.nb_grid_pts)
+                else:
+                    nc = NCStructuredGrid('test_{}d.nc'.format(len(self.nb_grid_pts)), mode='w',
+                                          nb_domain_grid_pts=self.nb_grid_pts,
+                                          decomposition='domain',
+                                          subdomain_locations=self.fft.subdomain_locations,
+                                          nb_subdomain_grid_pts=self.fft.nb_subdomain_grid_pts,
+                                          communicator=self.communicator)
+                nc.scalar = self.scalar_grid
+                nc.tensor = self.tensor_grid
+                nc[3].per_frame_tensor = self.tensor_grid
+                nc.close()
+
+                # Check that the file structure is correct
+                nc = Dataset('test_{}d.nc'.format(len(self.nb_grid_pts)), 'r')
+                dimensions = ['frame', 'grid_x', 'grid_y', 'tensor_3']
+                if len(self.nb_grid_pts) == 3:
+                    dimensions += ['grid_z']
+                self.assertEqual(set(nc.dimensions), set(dimensions))
+                self.assertEqual(len(nc.dimensions['frame']), 4)
+                self.assertEqual(len(nc.dimensions['grid_x']), self.nb_grid_pts[0])
+                self.assertEqual(len(nc.dimensions['grid_y']), self.nb_grid_pts[1])
+                if len(self.nb_grid_pts) == 3:
+                    self.assertEqual(len(nc.dimensions['grid_z']), self.nb_grid_pts[2])
+                self.assertEqual(len(nc.dimensions['tensor_3']), 3)
+                nc.close()
+
+                # Read file and check data
+                nc = NCStructuredGrid('test_{}d.nc'.format(len(self.nb_grid_pts)), mode='r')
+                self.assertEqual(tuple(nc.nb_domain_grid_pts), tuple(self.nb_grid_pts))
+                self.assertTrue(np.equal(nc.scalar, self.scalar_grid).all())
+                self.assertTrue(np.equal(nc.tensor, self.tensor_grid).all())
+                self.assertTrue(np.equal(nc[3].per_frame_tensor, self.tensor_grid).all())
+                nc.close()
+
+            def test_write_read_subdomain(self):
+                scalar_grid = self.scalar_grid[self.fft.subdomain_slices]
+                tensor_grid = self.tensor_grid[self.fft.subdomain_slices]
+
+                if self.communicator is None:
+                    nc = NCStructuredGrid('test_{}d.nc'.format(len(self.nb_grid_pts)), mode='w',
+                                          nb_domain_grid_pts=self.nb_grid_pts)
+                else:
+                    nc = NCStructuredGrid('test_{}d.nc'.format(len(self.nb_grid_pts)), mode='w',
+                                          nb_domain_grid_pts=self.nb_grid_pts,
+                                          decomposition='subdomain',
+                                          subdomain_locations=self.fft.subdomain_locations,
+                                          nb_subdomain_grid_pts=self.fft.nb_subdomain_grid_pts,
+                                          communicator=self.communicator)
+                nc.scalar = scalar_grid
+                nc.tensor = tensor_grid
+                nc[3].per_frame_tensor = tensor_grid
+                nc.close()
+
+                # Check that the file structure is correct
+                nc = Dataset('test_{}d.nc'.format(len(self.nb_grid_pts)), 'r')
+                dimensions = ['frame', 'grid_x', 'grid_y', 'tensor_3']
+                if len(self.nb_grid_pts) == 3:
+                    dimensions += ['grid_z']
+                self.assertEqual(set(nc.dimensions), set(dimensions))
+                self.assertEqual(len(nc.dimensions['frame']), 4)
+                self.assertEqual(len(nc.dimensions['grid_x']), self.nb_grid_pts[0])
+                self.assertEqual(len(nc.dimensions['grid_y']), self.nb_grid_pts[1])
+                if len(self.nb_grid_pts) == 3:
+                    self.assertEqual(len(nc.dimensions['grid_z']), self.nb_grid_pts[2])
+                self.assertEqual(len(nc.dimensions['tensor_3']), 3)
+                nc.close()
+
+                # Read file and check data
+                nc = NCStructuredGrid('test_{}d.nc'.format(len(self.nb_grid_pts)), mode='r')
+                self.assertEqual(tuple(nc.nb_domain_grid_pts), tuple(self.nb_grid_pts))
+                self.assertTrue(np.equal(nc.scalar, self.scalar_grid).all())
+                self.assertTrue(np.equal(nc.tensor, self.tensor_grid).all())
+                self.assertTrue(np.equal(nc[3].per_frame_tensor, self.tensor_grid).all())
+                nc.close()
+
+        return NetCDF_Check
+
+    # Check that it works with tuples or lists
+    NetCDF_Check_2d = build_test_classes((11, 23))
+    NetCDF_Check_3d = build_test_classes([11, 23, 7])
+
+except Exception:
+    pass
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `muFFT-0.9.3/tests/libmufft/test_fft_utils.cc` & `mufft-0.90.0/tests/test_fft_utils.cc`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,20 @@
  *
  * If you modify this Program, or any covered work, by linking or combining it
  * with proprietary FFT implementations or numerical libraries, containing parts
  * covered by the terms of those libraries' licenses, the licensors of this
  * Program grant you additional permission to convey the resulting work.
  *
  */
-#include <boost/mpl/list.hpp>
-
 #include "tests.hh"
 #include <libmugrid/ccoord_operations.hh>
 #include <libmufft/fft_utils.hh>
 
+#include <boost/mpl/list.hpp>
+
 namespace muFFT {
 
   BOOST_AUTO_TEST_SUITE(fft_utils);
 
   BOOST_FIXTURE_TEST_CASE_TEMPLATE(test_hermitian, Fix, dimlist, Fix) {
     constexpr auto dim{Fix::dim};
     using Ccoord = Ccoord_t<dim>;
```

### Comparing `muFFT-0.9.3/tests/libmufft/test_fftw_engine.cc` & `mufft-0.90.0/tests/test_serial_fft_engines.cc`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * @file   test_fftw_engine.cc
+ * @file   test_serial_fft_engines.cc
  *
  * @author Till Junge <till.junge@epfl.ch>
  *
  * @date   05 Dec 2017
  *
  * @brief  tests for the fftw fft engine implementation
  *
@@ -29,87 +29,124 @@
  * If you modify this Program, or any covered work, by linking or combining it
  * with proprietary FFT implementations or numerical libraries, containing parts
  * covered by the terms of those libraries' licenses, the licensors of this
  * Program grant you additional permission to convey the resulting work.
  *
  */
 
-#include "tests.hh"
+#include <iostream>
+
+#include <boost/mpl/list.hpp>
 
-#include <libmufft/fftw_engine.hh>
 #include <libmugrid/ccoord_operations.hh>
 #include <libmugrid/field_collection.hh>
 #include <libmugrid/field_map_static.hh>
 #include <libmugrid/iterators.hh>
 
-#include <boost/mpl/list.hpp>
-#include <iostream>
+#include <libmufft/pocketfft_engine.hh>
+#ifdef WITH_FFTW
+#include <libmufft/fftw_engine.hh>
+#endif
+
+#include "tests.hh"
 
 namespace muFFT {
-  BOOST_AUTO_TEST_SUITE(fftw_engine);
+  BOOST_AUTO_TEST_SUITE(serial_fft_engines);
 
   /* ---------------------------------------------------------------------- */
-  template <Index_t DimS, Index_t DimM, Index_t NbGridPts>
-  struct FFTW_fixture {
-    constexpr static Index_t BoxNbGridPts{NbGridPts};
+  template <class Engine, Index_t DimS, Index_t DimM, Index_t NbSubPts,
+            Index_t NbGridPts>
+  struct FFT_fixture {
+    constexpr static Index_t nb_grid_pts{NbGridPts};
     constexpr static Real Boxlength{4.5};
     constexpr static Index_t sdim{DimS};
     constexpr static Index_t mdim{DimM};
+    constexpr static Index_t nb_sub_pts{NbSubPts};
     constexpr static Ccoord_t<sdim> res() {
-      return muGrid::CcoordOps::get_cube<DimS>(BoxNbGridPts);
+      return muGrid::CcoordOps::get_cube<DimS>(nb_grid_pts);
     }
     constexpr static Ccoord_t<sdim> loc() {
       return muGrid::CcoordOps::get_cube<DimS>(Index_t{0});
     }
-    FFTW_fixture() : engine{DynCcoord_t(res())} {}
-    FFTWEngine engine;
+    FFT_fixture() : engine{DynCcoord_t(res())} {}
+    Engine engine;
   };
-  template <Index_t DimS, Index_t DimM, Index_t NbGridPts>
-  constexpr Index_t FFTW_fixture<DimS, DimM, NbGridPts>::sdim;
-  template <Index_t DimS, Index_t DimM, Index_t NbGridPts>
-  constexpr Index_t FFTW_fixture<DimS, DimM, NbGridPts>::mdim;
+  template <class Engine, Index_t DimS, Index_t DimM, Index_t NbSubPts,
+            Index_t NbGridPts>
+  constexpr Index_t FFT_fixture<Engine, DimS, DimM, NbSubPts, NbGridPts>::sdim;
+  template <class Engine, Index_t DimS, Index_t DimM, Index_t NbSubPts,
+            Index_t NbGridPts>
+  constexpr Index_t FFT_fixture<Engine, DimS, DimM, NbSubPts, NbGridPts>::mdim;
+  template <class Engine, Index_t DimS, Index_t DimM, Index_t NbSubPts,
+            Index_t NbGridPts>
+  constexpr Index_t FFT_fixture<Engine, DimS, DimM, NbSubPts,
+                                NbGridPts>::nb_sub_pts;
 
-  struct FFTW_fixture_python_segfault {
+  template<class Engine>
+  struct FFT_fixture_python_segfault {
     constexpr static Index_t dim{twoD};
     constexpr static Index_t sdim{twoD};
     constexpr static Index_t mdim{twoD};
+    constexpr static Index_t nb_sub_pts{1};
     constexpr static Ccoord_t<sdim> res() { return {6, 4}; }
     constexpr static Ccoord_t<sdim> loc() { return {0, 0}; }
-    FFTW_fixture_python_segfault() : engine{DynCcoord_t(res())} {}
-    FFTWEngine engine;
+    FFT_fixture_python_segfault() : engine{DynCcoord_t(res())} {}
+    Engine engine;
   };
-  constexpr Index_t FFTW_fixture_python_segfault::sdim;
-  constexpr Index_t FFTW_fixture_python_segfault::mdim;
+  template<class Engine>
+  constexpr Index_t FFT_fixture_python_segfault<Engine>::sdim;
+  template<class Engine>
+  constexpr Index_t FFT_fixture_python_segfault<Engine>::mdim;
+  template<class Engine>
+  constexpr Index_t FFT_fixture_python_segfault<Engine>::nb_sub_pts;
 
   using fixlist = boost::mpl::list<
-      FFTW_fixture<twoD, twoD, 3>, FFTW_fixture<twoD, threeD, 3>,
-      FFTW_fixture<threeD, threeD, 3>, FFTW_fixture<twoD, twoD, 4>,
-      FFTW_fixture<twoD, threeD, 4>, FFTW_fixture<threeD, threeD, 4>,
-      FFTW_fixture_python_segfault>;
+#ifdef WITH_FFTW
+      FFT_fixture<FFTWEngine, oneD, oneD, OneQuadPt, 3>,
+      FFT_fixture<FFTWEngine, oneD, twoD, OneQuadPt, 3>,
+      FFT_fixture<FFTWEngine, oneD, threeD, OneQuadPt, 3>,
+      FFT_fixture<FFTWEngine, twoD, twoD, OneQuadPt, 3>,
+      FFT_fixture<FFTWEngine, twoD, twoD, TwoQuadPts, 3>,
+      FFT_fixture<FFTWEngine, twoD, threeD, OneQuadPt, 3>,
+      FFT_fixture<FFTWEngine, threeD, threeD, OneQuadPt, 3>,
+      FFT_fixture<FFTWEngine, twoD, threeD, OneQuadPt, 4>,
+      FFT_fixture<FFTWEngine, threeD, threeD, OneQuadPt, 4>,
+      FFT_fixture_python_segfault<FFTWEngine>,
+#endif
+      FFT_fixture<PocketFFTEngine, oneD, oneD, OneQuadPt, 3>,
+      FFT_fixture<PocketFFTEngine, oneD, twoD, OneQuadPt, 3>,
+      FFT_fixture<PocketFFTEngine, oneD, threeD, OneQuadPt, 3>,
+      FFT_fixture<PocketFFTEngine, twoD, twoD, OneQuadPt, 3>,
+      FFT_fixture<PocketFFTEngine, twoD, twoD, TwoQuadPts, 3>,
+      FFT_fixture<PocketFFTEngine, twoD, threeD, OneQuadPt, 3>,
+      FFT_fixture<PocketFFTEngine, threeD, threeD, OneQuadPt, 3>,
+      FFT_fixture<PocketFFTEngine, twoD, threeD, OneQuadPt, 4>,
+      FFT_fixture<PocketFFTEngine, threeD, threeD, OneQuadPt, 4>,
+      FFT_fixture_python_segfault<PocketFFTEngine>
+      >;
 
   /* ---------------------------------------------------------------------- */
   BOOST_FIXTURE_TEST_CASE_TEMPLATE(Constructor_test, Fix, fixlist, Fix) {
-    BOOST_CHECK_NO_THROW(Fix::engine.initialise(this->mdim * this->mdim,
-                                                FFT_PlanFlags::estimate));
+    BOOST_CHECK_NO_THROW(Fix::engine.create_plan(this->mdim * this->mdim));
     BOOST_CHECK_EQUAL(Fix::engine.size(),
                       muGrid::CcoordOps::get_size(Fix::res()));
   }
 
   /* ---------------------------------------------------------------------- */
   BOOST_FIXTURE_TEST_CASE_TEMPLATE(fft_test, Fix, fixlist, Fix) {
-    Fix::engine.initialise(this->mdim * this->mdim, FFT_PlanFlags::estimate);
+    Fix::engine.create_plan(this->mdim * this->mdim);
     using FC_t = muGrid::GlobalFieldCollection;
-    FC_t fc(Fix::sdim);
+    FC_t fc(Fix::sdim, FC_t::SubPtMap_t{{"test", Fix::nb_sub_pts}});
     auto & input{fc.register_real_field("input", Fix::mdim * Fix::mdim)};
     auto & ref{fc.register_real_field("reference", Fix::mdim * Fix::mdim)};
     auto & result{fc.register_real_field("result", Fix::mdim * Fix::mdim)};
-    fc.initialise(Fix::res(), Fix::loc());
+    fc.initialise(Fix::res(), Fix::res(), Fix::loc());
 
     using map_t = muGrid::MatrixFieldMap<Real, Mapping::Mut, Fix::mdim,
-                                         Fix::mdim, IterUnit::Pixel>;
+                                         Fix::mdim, IterUnit::SubPt>;
     map_t inmap{input};
     auto refmap{map_t{ref}};
     auto resultmap{map_t{result}};
     size_t cntr{0};
     for (auto tup : akantu::zip(inmap, refmap)) {
       cntr++;
       auto & in_{std::get<0>(tup)};
@@ -117,17 +154,17 @@
       in_.setRandom();
       ref_ = in_;
     }
     auto & complex_field{Fix::engine.register_fourier_space_field(
         "fourier work space", Fix::mdim * Fix::mdim)};
     Fix::engine.fft(input, complex_field);
     using cmap_t = muGrid::MatrixFieldMap<Complex, Mapping::Mut, Fix::mdim,
-                                          Fix::mdim, IterUnit::Pixel>;
+                                          Fix::mdim, IterUnit::SubPt>;
     cmap_t complex_map(complex_field);
-    Real error = complex_map[0].imag().norm();
+    Real error{complex_map[0].imag().norm()};
     BOOST_CHECK_LT(error, tol);
 
     /* make sure, the engine has not modified input (which is
        unfortunately const-casted internally, hence this test) */
     for (auto && tup : akantu::zip(inmap, refmap)) {
       Real error{(std::get<0>(tup) - std::get<1>(tup)).norm()};
       BOOST_CHECK_LT(error, tol);
```

### Comparing `muFFT-0.9.3/tests/python_gradient_integration_test.py` & `mufft-0.90.0/tests/python_fft_tests.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,908 +1,840 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 """
-@file   python_gradient_integration_test.py
+@file   python_fft_tests.py
 
-@author Richard Leute <richard.leute@imtek.uni-freiburg.de>
+@author Till Junge <till.junge@altermail.ch>
 
-@date   23 Nov 2018
+@date   17 Jan 2018
 
-@brief  test the functionality of gradient_integration.py
+@brief  Compare µSpectre's fft implementations to numpy reference
 
 Copyright © 2018 Till Junge
 
-µSpectre is free software; you can redistribute it and/or
+µFFT is free software; you can redistribute it and/or
 modify it under the terms of the GNU Lesser General Public License as
 published by the Free Software Foundation, either version 3, or (at
 your option) any later version.
 
-µSpectre is distributed in the hope that it will be useful, but
+µFFT is distributed in the hope that it will be useful, but
 WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
-along with µSpectre; see the file COPYING. If not, write to the
+along with µFFT; see the file COPYING. If not, write to the
 Free Software Foundation, Inc., 59 Temple Place - Suite 330,
 Boston, MA 02111-1307, USA.
 
 Additional permission under GNU GPL version 3 section 7
 
 If you modify this Program, or any covered work, by linking or combining it
 with proprietary FFT implementations or numerical libraries, containing parts
 covered by the terms of those libraries' licenses, the licensors of this
 Program grant you additional permission to convey the resulting work.
 """
 
-from python_test_imports import µ
-import muFFT
+import gc
 
 import unittest
 import numpy as np
-import scipy.misc as sm
-import itertools
-import time
-# np.set_printoptions(precision=2)
-# np.set_printoptions(suppress=True)
-### Helper functions
-def init_X_F_Chi(lens, res, rank=2):
-    """
-    Setup all the needed parameters for initialization of the deformation
-    gradient F and the corresponding deformation map/field Chi_X.
-
-    Keyword Arguments:
-    lens -- list [Lx, Ly, ...] of box lengths in each direction (dtype=float)
-    res  -- list [Nx, Ny, ...] of grid resoultions (dtype = int)
-    rank -- int (default=2), rank of the deformation gradient tensor F.
-            (dtype = int)
-
-    Returns:
-    delta_x : np.array of grid spacing for each spatial direction (dtype = float)
-    dim  : int dimension of the structure, derived from len(res).
-    x_n  : np.ndarray shape=(res.shape+1, dim) initial nodal/corner positions
-           as created by gradient_integration.compute_grid (dtype = float)
-    x_c  : np.ndarray shape=(res.shape+1, dim) initial cell center positions
-           as created by gradient_integration.compute_grid (dtype = float)
-    F    : np.zeros shape=(res.shape, dim*rank) initialise deformation gradient
-           (dtype = float)
-    Chi_n: np.zeros shape=((res+1).shape, dim) initialise deformation field
-           (dtype = float)
-    freqs: np.ndarray as returned by compute_wave_vectors(). (dtype = float)
-    """
-    lens = np.array(lens)
-    res = np.array(res)
-    delta_x = lens / res
-    dim = len(res)
-    x_n, x_c = µ.gradient_integration.make_grid(lens, res)
-    F = np.zeros((dim,)*(rank) + x_c.shape[1:])
-    Chi_n = np.zeros(x_n.shape)
-
-    return delta_x, dim, x_n, x_c, F, Chi_n
-
-class GradientIntegration_Check(unittest.TestCase):
-    """
-    Check the implementation of all muSpectre.gradient_integration functions.
-    """
-
-    def setUp(self):
-        self.lengths = np.array([2.4, 3.7, 4.1])
-        self.nb_grid_pts = np.array([5, 3, 5])
-        self.norm_tol = 1e-8
-
-        # set timing = True for timing information
-        self.timing = False
-        self.startTime = time.time()
-
-    def tearDown(self):
-        if self.timing:
-            t = time.time() - self.startTime
-            print("{}:\n{:.3f} seconds".format(self.id(), t))
-
-    def test_make_grid(self):
-        """
-        Test the function compute_grid which creates an orthogonal
-        equally spaced grid of the given number of grid points in each dimension
-        and the corresponding  lengths.
-        """
-        lens = self.lengths
-        res = self.nb_grid_pts
-        d = np.array(lens)/np.array(res)
-        grid_n = np.zeros((len(res),) + tuple(res+1))
-        Nx, Ny, Nz = res+1
-        for i, j, k in itertools.product(range(Nx), range(Ny), range(Nz)):
-            grid_n[:, i, j, k] = np.array([i*d[0], j*d[1], k*d[2]])
-        grid_c = (grid_n - d.reshape((3, 1, 1, 1))/2)[:, 1:, 1:, 1:]
-        for n in range(1, 4):
-            x_n, x_c = µ.gradient_integration.make_grid(lens[:n], res[:n])
-            s = (np.s_[:n],) + (np.s_[:],)*n + (0,)*(3-n)
-            self.assertLess(np.linalg.norm(x_c - grid_c[s]), self.norm_tol)
-            self.assertLess(np.linalg.norm(x_n - grid_n[s]), self.norm_tol)
-
-    def test_reshape_gradient(self):
-        """
-        Test if reshape gradient transforms a flattend second order tensor in
-        the right way to a shape [dim, dim] + nb_grid_pts.
-        """
-        lens = list(self.lengths)
-        res = list(self.nb_grid_pts)
-        tol = 1e-5
-        formulation = µ.Formulation.finite_strain
-        DelF = np.array([[0   , 0.01, 0.02],
-                         [0.03, 0   , 0.04],
-                         [0.05, 0.06, 0   ]])
-        one  = np.eye(3, 3)
-        for n in range(2, 4):
-            cell = µ.Cell(res[:n], lens[:n], formulation)
-            if n == 2:
-                mat = µ.material.MaterialLinearElastic1_2d.make(
-                    cell, "material", 10, 0.3)
-            if n == 3:
-                mat = µ.material.MaterialLinearElastic1_3d.make(
-                    cell, "material", 10, 0.3)
-            for pixel in cell.pixel_indices:
-                mat.add_pixel(pixel)
-            solver = µ.solvers.KrylovSolverCG(cell, tol, maxiter=100,
-                                              verbose=µ.Verbosity.Silent)
-            r = µ.solvers.newton_cg(cell, DelF[:n, :n], solver,
-                                    tol, tol, verbose=µ.Verbosity.Silent)
-            grad = µ.gradient_integration.reshape_gradient(r.grad, list(res[:n]))
-            grad_theo = (DelF[:n, :n] + one[:n, :n]).reshape((n, n,) + (1,)*n)
-            self.assertEqual(grad.shape, (n, n,) + tuple(res[:n]))
-            self.assertLess(np.linalg.norm(grad - grad_theo), self.norm_tol)
-
-    def test_complement_periodically(self):
-        """
-        Test the periodic reconstruction of an array. Lower left entries are
-        added into the upper right part of the array.
-        """
-        # 1D grid scalars
-        x_test = np.array([0, 1, 2, 3])
-        x_test_p = np.array([0, 1, 2, 3, 0])
-        x_p = µ.gradient_integration.complement_periodically(x_test, 1)
-        self.assertLess(np.linalg.norm(x_p-x_test_p), self.norm_tol)
-
-        # 2D grid scalars
-        x_test = np.array([[1, 2, 3, 4],
-                           [5, 6, 7, 8]])
-        x_test_p = np.array([[1, 2, 3, 4, 1],
-                             [5, 6, 7, 8, 5],
-                             [1, 2, 3, 4, 1]])
-        x_p = µ.gradient_integration.complement_periodically(x_test, 2)
-        self.assertLess(np.linalg.norm(x_p-x_test_p), self.norm_tol)
-
-        # 2D grid vectors
-        x_test = np.array([[[1, 2, 3], [3, 4, 5]],
-                           [[6, 7, 8], [9, 10, 11]],
-                           [[12, 13, 14], [15, 6, 17]]])
-        x_test_p = np.array([[[1, 2, 3], [3, 4, 5], [1, 2, 3]],
-                             [[6, 7, 8], [9, 10, 11], [6, 7, 8]],
-                             [[12, 13, 14], [15, 6, 17], [12, 13, 14]],
-                             [[1, 2, 3], [3, 4, 5], [1, 2, 3]]])
-        x_p = µ.gradient_integration.complement_periodically(
-            np.moveaxis(x_test, -1, 0), 2)
-        self.assertLess(np.linalg.norm(x_p - np.moveaxis(x_test_p, -1, 0)),
-                        self.norm_tol)
-
-    def test_get_integrator(self):
-        """
-        Test if the right integrator is computed.
-        """
-        # Init:
-        # even grid
-        lens_e = np.array([1, 1, 1])
-        res_e = np.array([2, 2, 2])
-        delta_x_e = lens_e/res_e
-        x_n_e, x_c_e = µ.gradient_integration.make_grid(lens_e, res_e)
-        # odd grid
-        lens_o = np.array([1, 1])
-        res_o = np.array([3, 3])
-        delta_x_o = lens_o/res_o
-        x_n_o, x_c_o = µ.gradient_integration.make_grid(lens_o, res_o)
-
-        # Fourier Derivative:
-        # even grid
-        dim = len(res_e)
-        fourier_gradient = [µ.FourierDerivative(dim, i) for i in range(dim)]
-        fft_engine = muFFT.FFT(list(res_e))
-
-        #freqs = fft_engine.wavevectors(lens_e)
-        freqs = fft_engine.fftfreq * res_e.reshape((dim,)+(1,)*dim)
-        shift = np.exp(-1j*2*np.pi *
-                       np.einsum("i...,i->...", freqs, delta_x_e/2))
-        # analytic solution -i*q/|q|^2 * shift
-        int_ana = 1j/(2*np.pi)*np.array([[[[0,   0,   0], [0,   0,   1]],
-                                          [[0,   1,   0], [0, 1/2, 1/2]]],
-                                         [[[1,   0,   0], [1/2,   0, 1/2]],
-                                          [[1/2, 1/2,   0], [1/3, 1/3, 1/3]]]])\
-            .transpose((3, 0, 1, 2)) * shift
-        integrator = µ.gradient_integration.get_integrator(
-            fft_engine, fourier_gradient, delta_x_e)
-        self.assertLess(np.linalg.norm(integrator-int_ana), self.norm_tol)
-
-        # odd grid
-        dim = len(res_o)
-        fourier_gradient = [µ.FourierDerivative(dim, i) for i in range(dim)]
-        fft_engine = muFFT.FFT(list(res_o))
-        freqs = fft_engine.fftfreq * res_o.reshape((dim,)+(1,)*dim)
-        shift = np.exp(-1j*2*np.pi *
-                       np.einsum("i...,i->...", freqs, delta_x_o/2))
-        # analytic solution -i*q/|q|^2 * shift
-        int_ana = -1j/(2*np.pi) *\
-            np.array([[[0, 0, 0], [1, 1/2, 1/2]],
-                      [[0, 1, -1], [0, 1/2, -1/2]]]) * shift[np.newaxis, :, :]
-        integrator = µ.gradient_integration.get_integrator(
-            fft_engine, fourier_gradient, delta_x_o)
-        self.assertLess(np.linalg.norm(integrator-int_ana), self.norm_tol)
-
-        # Discrete Derivatives:
-        # odd grid
-        dim = len(res_o)
-        dy = muFFT.DiscreteDerivative([0, 0], [[-0.5, 0.5],
-                                               [-0.5, 0.5]])
-        dx = dy.rollaxes(-1)
-        discrete_gradient = [dx, dy]
-        fft_engine = muFFT.FFT(list(res_o))
-        integrator = µ.gradient_integration.get_integrator(fft_engine,
-                                                           discrete_gradient,
-                                                           delta_x_o)
-        int_ana = np.array(
-            [[[0. + 0.j,  0. - 0.j,  0. - 0.j],
-              [-0.16666667-0.09622504j, -0.16666667+0.09622504j,  0. - 0.19245009j]],
-             [[0. + 0.j, -0.16666667-0.09622504j, -0.16666667+0.09622504j],
-              [0. - 0.j, -0.16666667+0.09622504j,  0. + 0.19245009j]]])
-        self.assertLess(np.linalg.norm(integrator-int_ana), 1e-7)
 
+import muFFT, muGrid
 
-    def test_fourier_integrate_tensor_2(self):
-        """
-        Test the correct integration of a second-rank tensor gradient field,
-        like the deformation gradient, using fourier integration.
-        """
-        # cosinus, diagonal deformation gradient 2D
-        res = np.array([36, 14])
-        lens = np.array([7, 1.4])
-        delta_x, dim, x_n, x_c, F, u_n = init_X_F_Chi(lens, res)
-        for i in range(dim):
-            F[i, i, :, :] = 0.8*np.pi/lens[i]*np.cos(2*np.pi * x_c[i]/lens[i])
-        Chi_n = 0.4 * np.sin(2*np.pi*x_n/lens.reshape((dim,)+(1,)*dim))
-
-        # Fourier Derivative
-        fourier_gradient = [µ.FourierDerivative(dim, i) for i in range(dim)]
-        fft_engine = muFFT.FFT(list(res))
-        fft_engine.initialise(dim)
-        fft_engine.initialise(dim * dim)
-        placement_n = µ.gradient_integration.integrate_tensor_2(
-            F, fft_engine, fourier_gradient, delta_x)
-
-        self.assertLess(np.linalg.norm(Chi_n - placement_n), self.norm_tol)
-
-
-        # cosinus, diagonal deformation gradient 3D
-        res = np.array([36, 14, 15])
-        fft_engine = muFFT.FFT(list(res)) # new engine is now 3d
-        lens = np.array([7, 1.4, 3])
-        delta_x, dim, x_n, x_c, F, _ = init_X_F_Chi(lens, res)
-        for i in range(dim):
-            F[i, i, :, :, :] = 0.8*np.pi/lens[i] * \
-                np.cos(2*np.pi * x_c[i]/lens[i])
-        Chi_n = 0.4 * np.sin(2*np.pi*x_n/lens.reshape((dim,)+(1,)*dim))
-
-        # Fourier Derivative
-        fourier_gradient = [µ.FourierDerivative(dim, i) for i in range(dim)]
-
-        fft_engine.initialise(dim)
-        fft_engine.initialise(dim * dim)
-        placement_n = µ.gradient_integration.integrate_tensor_2(
-            F, fft_engine, fourier_gradient, delta_x)
-
-        self.assertLess(np.linalg.norm(Chi_n - placement_n), self.norm_tol)
-
-        # cosinus, non diagonal deformation gradient
-        res = [31, 19, 13]
-        lens = [7, 1.4, 3]
-        delta_x, dim, x_n, x_c, F, Chi_n = init_X_F_Chi(lens, res)
-
-        F[0, 0, :, :, :] = 4*np.pi/lens[0]*np.cos(2*np.pi/lens[0]*x_c[0])
-        F[1, 1, :, :, :] = 2*np.pi/lens[1]*np.cos(2*np.pi/lens[1]*x_c[1])
-        F[2, 2, :, :, :] = 2*np.pi/lens[2]*np.cos(2*np.pi/lens[2]*x_c[2])
-        F[1, 0, :, :, :] = 2*np.pi/lens[0]*np.cos(2*np.pi/lens[0]*x_c[0])
-        F[2, 0, :, :, :] = 2*np.pi/lens[0]*np.cos(2*np.pi/lens[0]*x_c[0])
-        for i in range(dim):
-            Chi_n[i, :, :, :] = np.sin(2*np.pi*x_n[i]/lens[i])  \
-                + np.sin(2*np.pi*x_n[0]/lens[0])
-
-        # Fourier Derivative
-        fourier_gradient = [µ.FourierDerivative(dim, i) for i in range(dim)]
-
-        fft_engine = muFFT.FFT(res)
-        fft_engine.initialise(dim)
-        fft_engine.initialise(dim * dim)
-        placement_n = µ.gradient_integration.integrate_tensor_2(
-            F, fft_engine, fourier_gradient, delta_x)
-        self.assertLess(np.linalg.norm(Chi_n - placement_n), self.norm_tol)
-
-    def test_shear_composite(self):
-        # Realistic test:
-        #   shear of a two dimensional material with two different Young moduli.
-        # initialize material structure
-        res = [9, 21]  # nb_grid_pts
-        lens = [9, 21]  # lengths
-        delta_x, dim, x_n, x_c, _, _ = init_X_F_Chi(lens, res)
-        formulation = µ.Formulation.finite_strain
-        Young = [10, 20]  # Youngs modulus for each phase (soft, hard)
-        Poisson = [0.3, 0.3]  # Poissons ratio for each phase
-
-        # geometry (two slabs stacked in y-direction with,
-        # hight h (soft material) and hight res[1]-h (hard material))
-        h = res[1]//2
-        phase = np.zeros(tuple(res), dtype=int)
-        phase[:, h:] = 1
-        phase = phase.T.flatten()
-        cell = µ.Cell(res, lens, formulation)
-        mat = µ.material.MaterialLinearElastic4_2d.make(cell, "material")
-        for i, pixel in enumerate(cell.pixels):
-            mat.add_pixel(i, Young[phase[i]], Poisson[phase[i]])
-        cell.initialise()
-        DelF = np.array([[0, 0.01],
-                         [0, 0   ]])
-
-        # µSpectre solution
-        solver = µ.solvers.KrylovSolverCG(cell, tol=1e-6, maxiter=100,
-                                          verbose=µ.Verbosity.Silent)
-        result = µ.solvers.newton_cg(cell, DelF, solver,
-                                     newton_tol=1e-6, equil_tol=1e-6,
-                                     verbose=µ.Verbosity.Silent)
-        F = µ.gradient_integration.reshape_gradient(result.grad, res)
-
-        # muSpectre Fourier integration
-        fourier_gradient = [µ.FourierDerivative(dim, i) for i in range(dim)]
-        fft_engine = muFFT.FFT(res)
-        fft_engine.initialise(dim)
-        fft_engine.initialise(dim * dim)
-
-        placement_n = µ.gradient_integration.integrate_tensor_2(
-            F, fft_engine, fourier_gradient, delta_x)
-        # muSpectre "discrete" integration (forward upwind scheme)
-        dy = muFFT.DiscreteDerivative([0, 0], [[-0.5, 0.5],
-                                               [-0.5, 0.5]])
-        dx = dy.rollaxes(-1)
-        discrete_gradient = [dx, dy]
-        placement_n_disc = µ.gradient_integration.integrate_tensor_2(
-            F, fft_engine, discrete_gradient, delta_x)
-
-        # analytic solution, "placement_ana" (node and center)
-        l_soft = delta_x[1] * h  # height soft material
-        l_hard = delta_x[1] * (res[1]-h)  # height hard material
-        Shear_modulus = np.array(Young) / (2 * (1+np.array(Poisson)))
-        mean_shear_strain = 2*DelF[0, 1]
-        shear_strain_soft = (lens[1]*mean_shear_strain) / (l_soft
-                            + l_hard * Shear_modulus[0]/Shear_modulus[1])
-        shear_strain_hard = (lens[1]*mean_shear_strain) / (l_soft
-                            * Shear_modulus[1]/Shear_modulus[0] + l_hard)
-        placement_ana_n = np.zeros(x_n.shape)
-        placement_ana_c = np.zeros(x_c.shape)
-
-        # x-coordinate
-        # soft material
-        placement_ana_n[0, :, :h+1] = shear_strain_soft/2 * x_n[1, :, :h+1]
-        placement_ana_c[0, :, :h] = shear_strain_soft/2 * x_c[1, :, :h]
-        # hard material
-        placement_ana_n[0, :, h+1:] =\
-            (shear_strain_hard/2 * (x_n[1, :, h+1:]-l_soft) +
-             shear_strain_soft/2 * l_soft)
-        placement_ana_c[0, :, h:] = \
-            (shear_strain_hard/2 * (x_c[1, :, h:]-l_soft) +
-             shear_strain_soft/2 * l_soft)
-        # y-coordinate
-        placement_ana_n[1, :, :] = 0
-        placement_ana_c[1, :, :] = 0
-
-        # shift the analytic solution such that the average nonaffine deformation
-        # is zero (integral of the nonaffine deformation gradient + N*const != 0)
-        F_homo = (1./(np.prod(res)) * F.sum(axis=tuple(-(np.arange(dim)+1))
-                                            )).reshape((dim,)*2 + (1,)*dim)
-        # integration constant = integral of the nonaffine deformation gradient/N
-        int_const =\
-            - ((placement_ana_c[0, :, :] - F_homo[0, 1, :, :] * x_c[1, :, :])
-                       .sum(axis=1))[0] / res[1]
-        ana_sol_n = placement_ana_n + x_n + \
-            np.array([int_const, 0]).reshape((dim,) + (1,)*dim)
-
-        # check the numeric vs the analytic solution
-        norm_n = \
-            (np.linalg.norm(placement_n - ana_sol_n)/
-             np.prod(np.array(res)))
-        self.assertLess(norm_n, 1.17e-5)
-        norm_n_disc = \
-            (np.linalg.norm(placement_n_disc - ana_sol_n)/
-             np.prod(np.array(res)))
-        self.assertLess(norm_n_disc, 3.89e-6)
+if muFFT.has_mpi:
+    from mpi4py import MPI
 
+    communicator = muFFT.Communicator(MPI.COMM_WORLD)
+else:
+    communicator = muFFT.Communicator()
 
 
-    def test_fourier_integrate_tensor_2_small_strain(self):
-        """
-        Test the correct integration of a second-rank tensor gradient field,
-        like the deformation gradient, using fourier integration.
-        """
-        strain_amp = 1e-4
-        # cosinus, diagonal deformation gradient 2D
-        res = np.array([35, 19])
-        lens = np.array([0.53, 1.42])
-        delta_x, dim, x_n, x_c, E, _ = init_X_F_Chi(lens, res)
-        for i in range(dim):
-            E[i, i, :, :] = \
-                (strain_amp * (2*np.pi/lens[i])
-                 * np.cos(2*np.pi * x_c[i]/lens[i]))
-            u_n =\
-                strain_amp * np.sin(2*np.pi*x_n/(lens.reshape((dim,)+(1,)*dim)))
-        fft_engine = muFFT.FFT(list(res))
-        fft_engine.initialise(dim)
-        fft_engine.initialise(dim * dim)
-        u_integrated_n = µ.gradient_integration.integrate_tensor_2_small_strain(
-            E, fft_engine, delta_x)
-        self.assertLess(np.linalg.norm(u_n - u_integrated_n), self.norm_tol)
-
-        #### Non Diagonal 2D:
-        delta_x, dim, x_n, x_c, E, u_n = init_X_F_Chi(lens, res)
-        for i in range(dim):
-            u_n[i, :, :] = strain_amp * (np.sin(2*np.pi*x_n[i]/lens[i]) +
-                                         np.sin(2*np.pi*x_n[0]/lens[0]))
-        E[0, 0, :, :] = \
-            strain_amp * 4 * np.pi/lens[0]*np.cos(2*np.pi/lens[0]*x_c[0])
-        E[1, 1, :, :] =\
-            strain_amp * 2 * np.pi/lens[1]*np.cos(2*np.pi/lens[1]*x_c[1])
-        E[1, 0, :, :] =\
-            strain_amp * np.pi/lens[0]*np.cos(2*np.pi/lens[0]*x_c[0])
-        E[0, 1, :, :] =\
-            strain_amp * np.pi/lens[0]*np.cos(2*np.pi/lens[0]*x_c[0])
-
-        u_integrated_n = µ.gradient_integration.integrate_tensor_2_small_strain(
-            E, fft_engine, delta_x)
-        self.assertLess(np.linalg.norm(u_n - u_integrated_n), self.norm_tol)
-
-        # cosinus, diagonal deformation gradient 3D
-        res = np.array([37, 13, 15])
-        lens = np.array([7, 1.4, 3])
-        delta_x, dim, x_n, x_c, E, _ = init_X_F_Chi(lens, res)
-        for i in range(dim):
-            E[i, i, :, :] = \
-                (strain_amp * (2*np.pi/lens[i])
-                 *np.cos(2*np.pi * x_c[i]/lens[i]))
-            u_n = \
-                strain_amp * np.sin(2*np.pi*x_n/(lens.reshape((dim,)+(1,)*dim)))
-        fft_engine = muFFT.FFT(list(res))
-        fft_engine.initialise(dim)
-        fft_engine.initialise(dim*dim)
-        u_integrated_n = µ.gradient_integration.integrate_tensor_2_small_strain(
-            E, fft_engine, delta_x)
-        self.assertLess(np.linalg.norm(u_n - u_integrated_n), self.norm_tol)
-
-        #### Non Diagonal 2D:
-        delta_x, dim, x_n, x_c, E, u_n = init_X_F_Chi(lens, res)
-        for i in range(dim):
-            u_n[i, :, :] = strain_amp * (np.sin(2*np.pi*x_n[i]/lens[i]) +
-                                         np.sin(2*np.pi*x_n[0]/lens[0]))
-        E[0, 0, :, :] = \
-            strain_amp * 4 * np.pi/lens[0]*np.cos(2*np.pi/lens[0]*x_c[0])
-        E[1, 1, :, :] =\
-            strain_amp * 2 * np.pi/lens[1]*np.cos(2*np.pi/lens[1]*x_c[1])
-        E[2, 2, :, :] =\
-            strain_amp * 2 * np.pi/lens[2]*np.cos(2*np.pi/lens[2]*x_c[2])
-        E[1, 0, :, :] =\
-            strain_amp * np.pi/lens[0]*np.cos(2*np.pi/lens[0]*x_c[0])
-        E[0, 1, :, :] =\
-            strain_amp * np.pi/lens[0]*np.cos(2*np.pi/lens[0]*x_c[0])
-        E[0, 2, :, :] =\
-            strain_amp * np.pi/lens[0]*np.cos(2*np.pi/lens[0]*x_c[0])
-        E[2, 0, :, :] =\
-            strain_amp * np.pi/lens[0]*np.cos(2*np.pi/lens[0]*x_c[0])
-
-        u_integrated_n = µ.gradient_integration.integrate_tensor_2_small_strain(
-            E, fft_engine, delta_x)
-        self.assertLess(np.linalg.norm(u_n - u_integrated_n), self.norm_tol)
+class FFT_Check(unittest.TestCase):
+    def setUp(self):
+        #               v- grid
+        #                      v-components
+        self.grids = [([8, 4], (2, 3)),
+                      ([6, 4], (1,)),
+                      ([6, 4, 5], (2, 3)),
+                      ([6, 4, 4], (1,))]
+
+        self.communicator = communicator
+
+        self.engines = []
+        if muFFT.has_mpi:
+            self.engines = ['fftwmpi', 'pfft']
+        if self.communicator.size == 1:
+            self.engines += ['pocketfft', 'fftw']
+
+    def test_constructor(self):
+        """Check that engines can be initialized with either bare MPI
+        communicator or muFFT communicators"""
+        for engine_str in self.engines:
+            if muFFT.has_mpi:
+                # Check initialization with bare MPI communicator
+                from mpi4py import MPI
+                s = MPI.COMM_WORLD.Get_size()
+                try:
+                    nb_dof = 6
+                    engine = muFFT.FFT([6 * s, 4 * s], fft=engine_str,
+                                       communicator=MPI.COMM_WORLD)
+                    engine.create_plan(nb_dof)
+                except muFFT.UnknownFFTEngineError:
+                    # This FFT engine has not been compiled into the code. Skip
+                    # test.
+                    continue
+
+            s = self.communicator.size
+            nb_dof = 6
+            try:
+                engine = muFFT.FFT([6 * s, 4 * s],
+                                   fft=engine_str,
+                                   communicator=self.communicator)
+                engine.create_plan(nb_dof)
+            except muFFT.UnknownFFTEngineError:
+                # This FFT engine has not been compiled into the code. Skip
+                # test.
+                continue
+
+            self.assertEqual(
+                self.communicator.sum(np.prod(engine.nb_subdomain_grid_pts)),
+                np.prod(engine.nb_domain_grid_pts),
+                msg='{} engine'.format(engine_str))
+
+            comm = engine.communicator
+            self.assertEqual(comm.sum(comm.rank + 4),
+                             comm.size * (comm.size + 1) / 2 + 3 * comm.size,
+                             msg='{} engine'.format(engine_str))
+
+    # Disable this test for now because it requires a lot of memory. This is
+    # because it initializes the pixel_indices array, which is large.
+    # def test_large_transform(self):
+    #     for engine_str in self.engines:
+    #         muFFT.FFT([65536, 65536], fft=engine_str,
+    #                   communicator=self.communicator)
+
+    def test_forward_transform_numpy_interface(self):
+        for engine_str in self.engines:
+            for nb_grid_pts, dims in self.grids:
+                s = self.communicator.size
+                nb_grid_pts = s * np.array(nb_grid_pts)
+                try:
+                    engine = muFFT.FFT(nb_grid_pts,
+                                       fft=engine_str,
+                                       communicator=self.communicator)
+                    engine.create_plan(np.prod(dims))
+                except muFFT.UnknownFFTEngineError:
+                    # This FFT engine has not been compiled into the code. Skip
+                    # test.
+                    continue
+
+                if len(nb_grid_pts) == 2:
+                    axes = (0, 1)
+                elif len(nb_grid_pts) == 3:
+                    axes = (0, 1, 2)
+                else:
+                    raise RuntimeError('Cannot handle {}-dim transforms'
+                                       .format(len(nb_grid_pts)))
 
+                # We need to transpose the input to np.fft because muFFT
+                # uses column-major while np.fft uses row-major storage
+                np.random.seed(1)
+                global_in_arr = np.random.random([*dims, *nb_grid_pts])
+                global_out_ref = np.fft.fftn(global_in_arr.T, axes=axes).T
+                out_ref = global_out_ref[(..., *engine.fourier_slices)]
+                in_arr = global_in_arr[(..., *engine.subdomain_slices)]
+
+                tol = 1e-14 * np.prod(nb_grid_pts)
+
+                # Separately test convenience interface
+                out_msp = np.empty([*dims, *engine.nb_fourier_grid_pts],
+                                   dtype=complex, order='f')
+                engine.fft(in_arr, out_msp)
+                err = np.linalg.norm(out_ref - out_msp)
+                self.assertLess(err, tol, msg='{} engine'.format(engine_str))
+
+    def test_reverse_transform_numpy_interface(self):
+        for engine_str in self.engines:
+            for nb_grid_pts, dims in self.grids:
+                s = self.communicator.size
+                nb_grid_pts = list(s * np.array(nb_grid_pts))
+
+                try:
+                    engine = muFFT.FFT(nb_grid_pts,
+                                       fft=engine_str,
+                                       communicator=self.communicator)
+                    engine.create_plan(np.prod(dims))
+                except muFFT.UnknownFFTEngineError:
+                    # This FFT engine has not been compiled into the code. Skip
+                    # test.
+                    continue
+
+                if len(nb_grid_pts) == 2:
+                    axes = (0, 1)
+                elif len(nb_grid_pts) == 3:
+                    axes = (0, 1, 2)
+                else:
+                    raise RuntimeError('Cannot handle {}-dim transforms'
+                                       .format(len(nb_grid_pts)))
 
-    def test_discrete_integrate_tensor_2(self):
-        """
-        Test the correct integration of a second-rank tensor gradient field,
-        like the deformation gradient, using discrete integration.
-        """
-        F0 = np.array([[1.1, 0.2, 0.0],
-                       [0.3, 1.2, 0.1],
-                       [0.1, 0.0, 0.9]])
-        res = [23, 45, 11]
-        lens = [1.4, 2.3, 1.1]
-        dim = len(res)
-        delta_x = [l/r for l, r in zip(lens, res)]
-        # Create a random displacement field
-        x = (((np.random.random([len(res)]+res)).T-0.5)*delta_x).T
-        for i in range(dim):
-            x[i] -= x[i].mean()  # mean of random field should be zero
-        x = µ.gradient_integration.complement_periodically(x, 3)
-        # Create grid positions
-        nodal_positions, center_positions = \
-            µ.gradient_integration.make_grid(np.array(lens), np.array(res))
-        # The displacement field lives on the corners
-        x += np.einsum('ij,jxyz->ixyz', F0, nodal_positions)
-        # Deformation gradient
-        F = np.zeros(2*[dim] + res)
-        for i in range(dim):
-            for j in range(dim):
-                F[j, i, :, :, :] = (
-                    np.roll(x[j], -1, axis=i) - x[j])[:-1, :-1, :-1]/delta_x[i]
-
-        self.assertTrue(np.allclose(np.mean(F, axis=(2, 3, 4)), F0))
-
-        fft_engine = muFFT.FFT(res)
-        fft_engine.initialise(dim)
-        fft_engine.initialise(dim * dim)
-        dz = muFFT.DiscreteDerivative([0, 0, 0], [[[-1, 1]]])
-        dy = dz.rollaxes(-1)
-        dx = dy.rollaxes(-1)
-        discrete_gradient = [dx, dy, dz]
-        placement_c = µ.gradient_integration.integrate_tensor_2(
-            F, fft_engine, discrete_gradient, delta_x)
+                # We need to transpose the input to np.fft because muFFT
+                # uses column-major while np.fft uses row-major storage
+                np.random.seed(1)
+                complex_res = list(engine.nb_domain_grid_pts)
+                complex_res[0] = complex_res[0] // 2 + 1
+                global_in_arr = np.zeros([*dims, *complex_res], dtype=complex)
+                global_in_arr.real = np.random.random(global_in_arr.shape)
+                global_in_arr.imag = np.random.random(global_in_arr.shape)
+                in_arr = global_in_arr[(..., *engine.fourier_slices)]
+                in_arr.shape = (*dims, *engine.nb_fourier_grid_pts)
+                global_out_ref = np.fft.irfftn(global_in_arr.T, axes=axes).T
+                out_ref = global_out_ref[(..., *engine.subdomain_slices)]
+
+                tol = 1e-14 * np.prod(nb_grid_pts)
+
+                # Separately test convenience interface
+                out_msp = np.empty([*dims, *engine.nb_subdomain_grid_pts],
+                                   dtype=float)
+                engine.ifft(in_arr, out_msp)
+
+                out_msp *= engine.normalisation
+                err = np.linalg.norm(out_ref - out_msp)
+                self.assertLess(err, tol, msg='{} engine'.format(engine_str))
+
+    def test_forward_transform_field_interface(self):
+        for engine_str in self.engines:
+            for nb_grid_pts, dims in self.grids:
+                s = self.communicator.size
+                nb_grid_pts = s * np.array(nb_grid_pts)
+
+                try:
+                    engine = muFFT.FFT(nb_grid_pts,
+                                       fft=engine_str,
+                                       communicator=self.communicator)
+                    engine.create_plan(np.prod(dims))
+                except muFFT.UnknownFFTEngineError:
+                    # This FFT engine has not been compiled into the code. Skip
+                    # test.
+                    continue
+
+                if len(nb_grid_pts) == 2:
+                    axes = (0, 1)
+                elif len(nb_grid_pts) == 3:
+                    axes = (0, 1, 2)
+                else:
+                    raise RuntimeError('Cannot handle {}-dim transforms'
+                                       .format(len(nb_grid_pts)))
 
-        for i in range(dim):
-            self.assertTrue(np.allclose(x[i], placement_c[i, :, :, :]))
+                # We need to transpose the input to np.fft because muFFT
+                # uses column-major while np.fft uses row-major storage
+                np.random.seed(1)
+                global_in_arr = np.random.random([*dims, *nb_grid_pts])
+                global_out_ref = np.fft.fftn(global_in_arr.T, axes=axes).T
+                out_ref = global_out_ref[(..., *engine.fourier_slices)]
+
+                fc = muGrid.GlobalFieldCollection(len(nb_grid_pts))
+                fc.initialise(tuple(engine.nb_domain_grid_pts),
+                              tuple(engine.nb_subdomain_grid_pts))
+                in_field = fc.register_real_field('in_field', dims)
+                self.assertFalse(in_field.array().flags.owndata)
+                in_field.array(muGrid.Pixel)[...] = global_in_arr[
+                    (..., *engine.subdomain_slices)]
+
+                tol = 1e-14 * np.prod(nb_grid_pts)
+
+                # Separately test convenience interface
+                out_field = engine.register_fourier_space_field("out_field",
+                                                                dims)
+                self.assertFalse(out_field.array().flags.owndata)
+                engine.fft(in_field, out_field)
+                err = np.linalg.norm(out_ref -
+                                     out_field.array(muGrid.Pixel))
+                self.assertLess(err, tol, msg='{} engine'.format(engine_str))
+
+    def test_reverse_transform_field_interface(self):
+        for engine_str in self.engines:
+            for nb_grid_pts, dims in self.grids:
+                s = self.communicator.size
+                nb_grid_pts = list(s * np.array(nb_grid_pts))
+
+                try:
+                    engine = muFFT.FFT(nb_grid_pts,
+                                       fft=engine_str,
+                                       communicator=self.communicator)
+                    engine.create_plan(np.prod(dims))
+                except muFFT.UnknownFFTEngineError:
+                    # This FFT engine has not been compiled into the code. Skip
+                    # test.
+                    continue
+
+                if len(nb_grid_pts) == 2:
+                    axes = (0, 1)
+                elif len(nb_grid_pts) == 3:
+                    axes = (0, 1, 2)
+                else:
+                    raise RuntimeError('Cannot handle {}-dim transforms'
+                                       .format(len(nb_grid_pts)))
 
-    def test_discrete_integrate_vector_2d_no_homogeneous(self):
-        """
-        Test the correct integration of a first-rank tensor gradient field,
-        like the electrostatic field, using discrete integration. The mean
-        gradient for this test is zero.
-        """
-        res = [23, 45]
-        lens = [1.4, 2.3]
-        dim = len(res)
-        delta_x = [l/r for l, r in zip(lens, res)]
-        # Create a random displacement field
-        x = np.random.random(res)-0.5
-        x -= x.mean()
-        # Create grid positions
-        x_n, x_c = \
-            µ.gradient_integration.make_grid(np.array(lens), np.array(res))
-        # Gradient
-        g = np.zeros([dim] + res)
-        for i in range(dim):
-            g[i, :, :] = (np.roll(x, -1, axis=i) - x)/delta_x[i]
-
-        fft_engine = muFFT.FFT(res)
-        fft_engine.initialise(dim**0)
-        fft_engine.initialise(dim**1)
-        dy = muFFT.DiscreteDerivative([0, 0], [[-1, 1]])
-        dx = dy.rollaxes(-1)
-        discrete_gradient = [dx, dy]
-        int_x = µ.gradient_integration.integrate_vector(
-            g, fft_engine, discrete_gradient, delta_x)
+                # We need to transpose the input to np.fft because muFFT
+                # uses column-major while np.fft uses row-major storage
+                np.random.seed(1)
+                complex_res = list(engine.nb_domain_grid_pts)
+                complex_res[0] = complex_res[0] // 2 + 1
+                global_in_arr = np.zeros([*dims, *complex_res], dtype=complex)
+                global_in_arr.real = np.random.random(global_in_arr.shape)
+                global_in_arr.imag = np.random.random(global_in_arr.shape)
+                global_out_ref = np.fft.irfftn(global_in_arr.T, axes=axes).T
+                out_ref = global_out_ref[(..., *engine.subdomain_slices)]
+
+                tol = 1e-14 * np.prod(nb_grid_pts)
+
+                fourier_field = engine.register_fourier_space_field(
+                    "fourier_field", dims)
+                self.assertFalse(fourier_field.array().flags.owndata)
+                fourier_field.array(muGrid.Pixel)[...] = \
+                    global_in_arr[(..., *engine.fourier_slices)]
+
+                out_field = engine.register_real_space_field('out_field', dims)
+                self.assertFalse(out_field.array().flags.owndata)
+
+                # Separately test convenience interface
+                engine.ifft(fourier_field, out_field)
+                err = np.linalg.norm(
+                    out_ref -
+                    out_field.array(muGrid.Pixel) * engine.normalisation)
+                self.assertLess(err, tol, msg='{} engine'.format(engine_str))
+
+    def test_nb_components1_forward_transform(self):
+        for engine_str in self.engines:
+            for nb_grid_pts, dims in self.grids:
+                if np.prod(dims) != 1:
+                    continue
+
+                try:
+                    engine = muFFT.FFT(nb_grid_pts,
+                                       fft=engine_str,
+                                       communicator=self.communicator)
+                    engine.create_plan(np.prod(dims))
+                except muFFT.UnknownFFTEngineError:
+                    # This FFT engine has not been compiled into the code. Skip
+                    # test.
+                    continue
+
+                np.random.seed(1)
+                global_in_arr = np.random.random(nb_grid_pts)
+                global_out_ref = np.fft.rfftn(global_in_arr)
+                out_ref = global_out_ref[(*engine.fourier_slices, ...)]
+                in_arr = global_in_arr[(*engine.subdomain_slices, ...)]
+
+                # Separately test convenience interface
+                out_msp = engine.register_fourier_space_field("out_msp",
+                                                              dims)
+                self.assertFalse(out_msp.array().flags.owndata)
+                engine.fft(in_arr, out_msp)
+
+                # Check that the output array does not have a unit first dimension
+                assert np.squeeze(out_msp).shape == engine.nb_fourier_grid_pts, \
+                    "{} not equal to {}".format(out_msp.shape,
+                                                engine.nb_fourier_grid_pts)
+
+    def test_nb_components1_forward_transform(self):
+        for engine_str in self.engines:
+            for nb_grid_pts, dims in self.grids:
+                if np.prod(dims) != 1:
+                    continue
+
+                try:
+                    engine = muFFT.FFT(nb_grid_pts,
+                                       fft=engine_str,
+                                       communicator=self.communicator)
+                    engine.create_plan(np.prod(dims))
+                except muFFT.UnknownFFTEngineError:
+                    # This FFT engine has not been compiled into the code. Skip
+                    # test.
+                    continue
+
+                np.random.seed(1)
+                global_in_arr = np.random.random(nb_grid_pts)
+                global_out_ref = np.fft.rfftn(global_in_arr)
+                out_ref = global_out_ref[(*engine.fourier_slices, ...)]
+                in_arr = global_in_arr[(*engine.subdomain_slices, ...)]
+
+                # Separately test convenience interface
+                out_msp = engine.register_fourier_space_field('out_msp',
+                                                              dims)
+                self.assertFalse(out_msp.array().flags.owndata)
+                engine.fft(in_arr, out_msp)
+
+                # Check that the output array does not have a unit first dimension
+                self.assertEqual(tuple(out_msp.shape), engine.nb_fourier_grid_pts),  # \
+                #                "{} not equal to {}".format(out_msp.shape,
+                #                                            engine.nb_fourier_grid_pts)
+                # TODO(pastewka): I think this test is out of date. the numpy
+                # rfftn shortens a different dimension, and therefore gets a
+                # different shape. can we ditch this?
+                # self.assertEqual(out_msp.shape, global_out_ref.shape)
+                # self.assertEqual(len(out_msp.shape), len(global_out_ref.shape))
+
+                # Convenience interface that returns an array
+                out_msp = engine.fft(in_arr)
+                # Check that the output array does not have a unit first dimension
+                self.assertEqual(tuple(out_msp.shape), engine.nb_fourier_grid_pts),  # \
+
+                # Convenience interface with flattened array (should not give a
+                # segmentation fault)
+                self.assertRaises(RuntimeError,
+                                  lambda: engine.fft(in_arr.ravel()))
+
+    def test_nb_components1_reverse_transform(self):
+        """
+        asserts that the output is of shape ( , ) and not ( , , 1)
+        """
+        for engine_str in self.engines:
+            for nb_grid_pts, dims in self.grids:
+                if np.prod(dims) != 1:
+                    continue
+
+                try:
+                    engine = muFFT.FFT(nb_grid_pts,
+                                       fft=engine_str,
+                                       communicator=self.communicator)
+                    engine.create_plan(np.prod(dims))
+                except muFFT.UnknownFFTEngineError:
+                    # This FFT engine has not been compiled into the code. Skip
+                    # test.
+                    continue
+
+                complex_res = list(engine.nb_domain_grid_pts)
+                complex_res[0] = complex_res[0] // 2 + 1
+                global_in_arr = np.zeros(complex_res, dtype=complex)
+                np.random.seed(1)
+                global_in_arr.real = np.random.random(global_in_arr.shape)
+                global_in_arr.imag = np.random.random(global_in_arr.shape)
+
+                in_arr = global_in_arr[engine.fourier_slices]
+                in_arr.shape = (*dims, *engine.nb_fourier_grid_pts)
+                out_msp = np.empty((1, *engine.nb_subdomain_grid_pts),
+                                   order="f")
+                engine.ifft(in_arr, out_msp)
+                assert out_msp.shape == (1, *engine.nb_subdomain_grid_pts), \
+                    "{} not equal to {}".format(out_msp.shape,
+                                                engine.nb_subdomain_grid_pts)
+
+                # Convenience interface with flattened array (should not give a
+                # segmentation fault)
+                self.assertRaises(RuntimeError,
+                                  lambda: engine.ifft(in_arr.ravel()))
+
+    @unittest.skipIf(communicator.size > 1,
+                     'MPI parallel FFTs do not support 1D transforms')
+    def test_1d_transform(self):
+        for fft in ['pocketfft', 'fftw']:
+            nb_grid_pts = [128, ]
+
+            # Only serial engines support 1d transforms
+            try:
+                engine = muFFT.FFT(nb_grid_pts, fft=fft)
+            except muFFT.UnknownFFTEngineError:
+                # This FFT engine has not been compiled into the code. Skip
+                # test.
+                continue
+
+            nb_dof = 1
+            engine.create_plan(nb_dof)
+            arr = np.random.random(nb_grid_pts * nb_dof)
+
+            fft_arr_ref = np.fft.rfft(arr)
+            fft_arr = engine.register_fourier_space_field("fourier work space",
+                                                          nb_dof)
+            self.assertFalse(fft_arr.array().flags.owndata)
+            self.assertEqual(fft_arr.shape, [nb_grid_pts[0] // 2 + 1])
+            engine.fft(arr, fft_arr)
+            self.assertTrue(np.allclose(fft_arr_ref, fft_arr))
+
+            out_arr = np.empty_like(arr)
+            engine.ifft(fft_arr, out_arr)
+            out_arr *= engine.normalisation
+            self.assertTrue(np.allclose(out_arr, arr))
+
+    def test_fftfreq_numpy(self):
+        for engine_str in self.engines:
+            for nb_grid_pts, dims in self.grids:
+                if np.prod(dims) == 1:
+                    continue
+
+                s = self.communicator.size
+                nb_grid_pts = list(s * np.array(nb_grid_pts))
+
+                try:
+                    engine = muFFT.FFT(nb_grid_pts,
+                                       fft=engine_str,
+                                       communicator=self.communicator)
+                except muFFT.UnknownFFTEngineError:
+                    # This FFT engine has not been compiled into the code. Skip
+                    # test.
+                    continue
+
+                freq = np.array(
+                    np.meshgrid(*(np.fft.fftfreq(n) for n in nb_grid_pts),
+                                indexing='ij'))
+
+                freq = freq[(..., *engine.fourier_slices)]
+                assert np.allclose(engine.fftfreq, freq)
+
+    def test_fftfreq(self):
+        # Check that x and y directions are correct
+        nb_grid_pts = [7, 4]
+        nx, ny = nb_grid_pts
+        nb_dof = 1
+        engine = muFFT.FFT(nb_grid_pts, fft='serial')
+        engine.create_plan(nb_dof)
+        qx, qy = engine.fftfreq
+
+        qarr = np.zeros(engine.nb_fourier_grid_pts, dtype=complex)
+        qarr[np.logical_and(np.abs(np.abs(qx) * nx - 1) < 1e-6,
+                            np.abs(np.abs(qy) * ny - 0) < 1e-6)] = 0.5
+
+        rarr = np.zeros(nb_grid_pts, order='f')
+        engine.ifft(qarr, rarr)
+        assert np.allclose(rarr, rarr[:, 0].reshape(-1, 1))
+        assert np.allclose(rarr[:, 0], np.cos(np.arange(nx) * 2 * np.pi / nx))
+
+        qarr = np.zeros(engine.nb_fourier_grid_pts, dtype=complex)
+        qarr[np.logical_and(np.abs(np.abs(qx) * nx - 0) < 1e-6,
+                            np.abs(np.abs(qy) * ny - 1) < 1e-6)] = 0.5
+        engine.ifft(qarr, rarr)
+        assert np.allclose(rarr, rarr[0, :].reshape(1, -1))
+        assert np.allclose(rarr[0, :], np.cos(np.arange(ny) * 2 * np.pi / ny))
+
+    def test_buffer_lifetime(self):
+        res = [2, 3]
+        data = np.random.random(res)
+        ref = np.fft.rfftn(data.T).T
+        # Python will attempt to remove the muFFT.FFT temporary object here
+        # right after the call to fft. However, since fft returns a pointer
+        # to an *internal* buffer of the object, garbage collection should
+        # be deferred until `tested` is destroyed.
+        engine = muFFT.FFT(res, fft="serial")
+        engine.create_plan(1)
+        f_data = engine.register_fourier_space_field("fourier work space", 1)
+        self.assertFalse(f_data.array().flags.owndata)
+        engine.fft(data, f_data)
+        tested = f_data.array()
+        gc.collect()
+        # It should not own the data, because it reference an internal buffer
+        assert not tested.flags.owndata
+        assert np.allclose(ref.real, tested.real)
+        assert np.allclose(ref.imag, tested.imag)
+
+    @unittest.skipIf(communicator.size > 1,
+                     'This test only works on a single MPI process')
+    def test_strides(self):
+        for engine_str in self.engines:
+            try:
+                engine = muFFT.FFT([3, 5, 7], fft=engine_str,
+                                   communicator=self.communicator)
+                engine.create_plan(1)
+            except muFFT.UnknownFFTEngineError:
+                # This FFT engine has not been compiled into the code. Skip
+                # test.
+                continue
+
+            if engine_str == 'fftwmpi':
+                assert engine.subdomain_strides == (1, 4, 20), \
+                    '{} - {}'.format(engine_str, engine.subdomain_strides)  # padding in first dimension
+                assert engine.fourier_strides == (1, 14, 2), \
+                    '{} - {}'.format(engine_str, engine.fourier_strides)  # transposed output
+            elif engine_str == 'pfft':
+                assert engine.subdomain_strides == (1, 4, 20), \
+                    '{} - {}'.format(engine_str, engine.subdomain_strides)  # padding in first dimension
+                assert engine.fourier_strides == (7, 14, 1), \
+                    '{} - {}'.format(engine_str, engine.fourier_strides)  # transposed output
+            else:
+                assert engine.subdomain_strides == (1, 3, 15), \
+                    '{} - {}'.format(engine_str, engine.subdomain_strides)  # column-major
+                assert engine.fourier_strides == (1, 2, 10), \
+                    '{} - {}'.format(engine_str, engine.fourier_strides)  # column-major
+
+    @unittest.skipIf(communicator.size > 1,
+                     'This test only works on a single MPI process')
+    def test_raises_incompatible_buffer(self):
+        """
+        checks for exception of buffer has incompatible memory layout
+        (FFTW only since PocketFFT can deal with any layout)
+        """
+        for fft in ['fftw']:
+            try:
+                engine = muFFT.FFT([3, 2],
+                                   fft=fft, allow_temporary_buffer=False)
+            except muFFT.UnknownFFTEngineError:
+                # This FFT engine has not been compiled into the code. Skip
+                # test.
+                continue
+
+            engine.create_plan(1)
+
+            in_data = np.random.random(engine.nb_subdomain_grid_pts)
+            out_data = np.zeros(engine.nb_fourier_grid_pts, dtype=complex)
+            with self.assertRaises(RuntimeError):
+                engine.fft(in_data, out_data)
+
+    def test_zero_grid_pts(self):
+        nb_grid_pts = [3, 3]  # Gives one CPU with zero points on 4 processes
+        axes = (0, 1)
+
+        try:
+            engine = muFFT.FFT(nb_grid_pts,
+                               fft='fftwmpi',
+                               communicator=self.communicator)
+            engine.create_plan(1)
+        except muFFT.UnknownFFTEngineError:
+            # This FFT engine has not been compiled into the code. Skip
+            # test.
+            return
+
+        # We need to transpose the input to np.fft because muFFT
+        # uses column-major while np.fft uses row-major storage
+        np.random.seed(1)
+        global_in_arr = np.random.random(nb_grid_pts)
+        global_out_ref = np.fft.fftn(global_in_arr.T, axes=axes).T
+        out_ref = global_out_ref[(..., *engine.fourier_slices)]
+        in_arr = global_in_arr[(..., *engine.subdomain_slices)]
+
+        tol = 1e-14 * np.prod(nb_grid_pts)
+
+        # Separately test convenience interface
+        out_msp = np.empty(engine.nb_fourier_grid_pts,
+                           dtype=complex, order='f')
+        engine.fft(in_arr, out_msp)
+        err = np.linalg.norm(out_ref - out_msp)
+        self.assertLess(err, tol)
 
-        self.assertTrue(np.allclose(x, int_x[0,:-1, :-1]))
 
-    def test_discrete_integrate_vector_3d(self):
-        """
-        Test the correct integration of a first-rank tensor gradient field,
-        like the electrostatic field, using discrete integration.
-        """
-        F0 = np.array([1.1, 0.2, 0.7])
-        res = [23, 45, 17]
-        lens = [1.4, 2.3, 1.7]
-        res1 = [r+1 for r in res]
-        dim = len(res)
-        delta_x = [l/r for l, r in zip(lens, res)]
-        # Create a random displacement field
-        x = np.random.random(res)-0.5
-        x -= x.mean()  # mean of random field should be zero
-        x = µ.gradient_integration.complement_periodically(x, 3)
-        # Create grid positions
-        nodal_positions, center_positions = \
-            µ.gradient_integration.make_grid(np.array(lens), np.array(res))
-        x += np.einsum('j,jxyz->xyz', F0, nodal_positions)
-        # Gradient
-        g = np.zeros([dim] + res)
-        for i in range(dim):
-            g[i, :, :, :] = (np.roll(x, -1, axis=i) -
-                             x)[:-1, :-1, :-1]/delta_x[i]
-
-        fft_engine = muFFT.FFT(res)
-        fft_engine.initialise(dim**0)
-        fft_engine.initialise(dim**1)
-        dz = muFFT.DiscreteDerivative([0, 0, 0], [[[-1, 1]]])
-        dy = dz.rollaxes(-1)
-        dx = dy.rollaxes(-1)
-        discrete_gradient = [dx, dy, dz]
-        int_x = µ.gradient_integration.integrate_vector(
-            g, fft_engine, discrete_gradient, delta_x)
-
-        self.assertTrue(np.allclose(x, int_x))
-
-    def test_compute_placement(self):
-        """Test the computation of placements and the original positions."""
-        ### shear of a homogeneous material ###
-        res = [3, 11]  # nb_grid_pts
-        lens = [10, 10]  # lengths
-        dim = len(res)  # dimension
-        x_n = µ.gradient_integration.make_grid(np.array(lens), np.array(res))[0]
-
-        # finite strain
-        formulation = µ.Formulation.finite_strain
-        cell = µ.Cell(res, lens, formulation)
-        mat = µ.material.MaterialLinearElastic1_2d.make(cell, "material",
-                                                        Young=10, Poisson=0.3)
-        for pixel_id in cell.pixel_indices:
-            mat.add_pixel(pixel_id)
-        cell.initialise()
-        DelF = np.array([[0, 0.05],
-                         [0, 0   ]])
-        # analytic
-        placement_ana = np.copy(x_n)
-        placement_ana[0, :, :] += DelF[0, 1]*x_n[1, :, :]
-
-        # µSpectre solution
-        fourier_gradient = [µ.FourierDerivative(dim, i) for i in range(dim)]
-        solver = µ.solvers.KrylovSolverCG(cell, tol=1e-6, maxiter=100,
-                                          verbose=µ.Verbosity.Silent)
-        result = µ.solvers.newton_cg(cell, DelF, solver, newton_tol=1e-6,
-                                     equil_tol=1e-6,
-                                     verbose=µ.Verbosity.Silent)
-        result_reshaped = µ.gradient_integration.reshape_gradient(
-            result.grad, res).flatten()
-        for r in [result, result_reshaped]:
-            # check input of result=OptimiseResult and result=np.ndarray
-            placement, x = µ.gradient_integration.compute_placement(
-                r, lens, res, fourier_gradient,
-                formulation=µ.Formulation.finite_strain)
-            self.assertLess(np.linalg.norm(placement_ana -
-                                           placement), 1e-12)
-            self.assertTrue((x_n == x).all())
-
-
-    def test_compute_placement_small_strain(self):
-        """Test the computation of placements and the original positions."""
-        ### shear of a homogeneous material ###
-        res = [3, 11]  # nb_grid_pts
-        lens = [10, 12]  # lengths
-        dim = len(res)  # dimension
-        x_n = µ.gradient_integration.make_grid(np.array(lens), np.array(res))[0]
-
-        # finite strain
-        formulation = µ.Formulation.small_strain
-        cell = µ.Cell(res, lens, formulation)
-        mat = µ.material.MaterialLinearElastic1_2d.make(cell, "material",
-                                                        Young=10, Poisson=0.3)
-        for pixel_id in cell.pixel_indices:
-            mat.add_pixel(pixel_id)
-        cell.initialise()
-        DelE = 1e-4 * np.array([[0   , 0.05],
-                                [0.05, 0   ]])
-
-        # analytic
-        placement_ana = np.copy(x_n)
-        placement_ana[0, :, :] += DelE[0, 1] * x_n[1, :, :]
-        placement_ana[1, :, :] += DelE[1, 0] * x_n[0, :, :]
-
-        # µSpectre solution
-        fourier_gradient = [µ.FourierDerivative(dim, i) for i in range(dim)]
-        solver = \
-            µ.solvers.KrylovSolverCG(cell, tol=1e-6, maxiter=100,
-                                     verbose=µ.Verbosity.Silent)
-        result = µ.solvers.newton_cg(cell, DelE, solver,
-                                     newton_tol=1e-6, equil_tol=1e-6,
-                                     verbose=µ.Verbosity.Silent)
-        result_reshaped = µ.gradient_integration.reshape_gradient(
-            result.grad, res).flatten()
-        for r in [result, result_reshaped]:
-            # check input of result=OptimiseResult and result=np.ndarray
-            u_n, x = µ.gradient_integration.compute_placement(
-                r, lens, res, fourier_gradient,
-                formulation=µ.Formulation.small_strain)
-            self.assertLess(np.linalg.norm(placement_ana -
-                                           u_n), 1e-12)
-            self.assertTrue((x_n == x).all())
-
-
-    def test_compare_small_strain_finite_strain(self):
-        """Tests the equality of the displacement field obtained from
-        integration of small strain field Vs. finite strain field of a cell."""
-        F_amp = 1e-4
-        lengths = [1.0, 1.0, 1.0]
-        nb_grid_pts = [11, 11, 3]
-        dim = len(nb_grid_pts)
-        Nx, Ny, Nz = nb_grid_pts
-        formulation = µ.Formulation.small_strain
-        Young = [10, 20]  # Youngs modulus for each phase
-        Poisson = [0.3, 0.4]  # Poissons ratio for each phase
-
-        # solver
-        newton_tol = 1e-8  # tolerance for newton algo
-        cg_tol = 1e-10  # tolerance for cg algo
-        equil_tol = 1e-8  # tolerance for equilibrium
-        maxiter = 1000
-        verbose = verbose=µ.Verbosity.Silent
-
-        # sinusoidal bump
-        d = int(nb_grid_pts[1]*0.2)
-        l = Nx//3  # length of bump
-        h = Ny//5  # height of bump
-        low_y = (Ny-d)//2  # lower y-boundary of phase
-        high_y = low_y+d  # upper y-boundary of phase
-        left_x = (Nx-l)//2  # boundaries in x direction left
-        right_x = left_x + l  # boundaries in x direction right
-        x = np.arange(l)
-        p_y = h*np.sin(np.pi/(l-1)*x)  # bump function
-        xy_bump = np.ones((l, h, Nz))  # grid representing bumpx
-
-        for i, threshold in enumerate(np.round(p_y)):
-            xy_bump[i, int(threshold):, :] = 0
-
-        phase = np.zeros(nb_grid_pts, dtype=int)  # 0 for surrounding matrix
-        phase[:, low_y:high_y, :] = 1
-        phase[left_x:right_x, high_y:high_y+h, :] = xy_bump
-
-        ### Run muSpectre ###
-        #-------------------#
-        fourier_gradient =\
-            [µ.FourierDerivative(dim , i) for i in range(dim)]
-        ######finite strain:
-        DelF = F_amp * np.array([[+0.50, +0.20, +0.00],
-                                 [+0.00, -0.03, +0.15],
-                                 [+0.00, +0.15, +0.40]])
-        F = np.identity(DelF.shape[0]) + DelF
-
-        cell_finite =\
-            µ.Cell(nb_grid_pts, lengths, µ.Formulation.finite_strain,
-                   fourier_gradient)
-        mat_finite =\
-            µ.material.MaterialLinearElastic4_3d.make(cell_finite,
-                                                      "material_finite")
-        for pixel_id, pixel in cell_finite.pixels.enumerate():
-            # add Young and Poisson depending on the material index
-            m_i = phase.flatten(order='F')[pixel_id]
-            mat_finite.add_pixel(pixel_id, Young[m_i], Poisson[m_i])
-
-        cell_finite.initialise()  # initialization of fft to make faster fft
-
-        solver_newton_finite = \
-            µ.solvers.KrylovSolverCG(cell_finite, cg_tol, maxiter, verbose)
-        result_finite = µ.solvers.newton_cg(cell_finite, DelF,
-                                            solver_newton_finite,
-                                            newton_tol, equil_tol, verbose)
-        ######small strain:
-        DelE = 0.5 * ((F.T).dot(F) - np.identity(DelF.shape[0]))
-
-        cell_small =\
-            µ.Cell(nb_grid_pts, lengths, µ.Formulation.small_strain,
-                   fourier_gradient)
-        mat_small =\
-            µ.material.MaterialLinearElastic4_3d.make(cell_small,
-                                                      "material_small")
-        for pixel_id, pixel in cell_small.pixels.enumerate():
-            # add Young and Poisson depending on the material index
-            m_i = phase.flatten(order='F')[pixel_id]
-            mat_small.add_pixel(pixel_id, Young[m_i], Poisson[m_i])
-
-        cell_small.initialise()  # initialization of fft to make faster fft
-        solver_newton_small = \
-            µ.solvers.KrylovSolverCG(cell_small, cg_tol, maxiter, verbose)
-        result_small = µ.solvers.newton_cg(cell_small, DelE,
-                                           solver_newton_small,
-                                           newton_tol, equil_tol, verbose)
-
-        #-------------------#
-        # integration of the deformation gradient field
-        placement_n_finite, x = \
-            µ.gradient_integration.compute_placement(
-                result_finite, lengths, nb_grid_pts, fourier_gradient,
-                formulation = result_finite.formulation)
-
-        placement_n_small, x = \
-            µ.gradient_integration.compute_placement(
-                result_small, lengths, nb_grid_pts, fourier_gradient,
-                formulation = result_small.formulation)
-
-        err_norm = np.linalg.norm(placement_n_small - placement_n_finite)
-        self.assertLess(err_norm, F_amp * 5)
-
-
-    def test_vacuum(self):
-        form = µ.Formulation.finite_strain
-        Poisson = 0.3
-        nb_pts = 9
-
-        for dim in [2, 3]:
-            if dim == 2:
-                dy = muFFT.DiscreteDerivative([0, 0], [[-0.5, 0.5],
-                                                       [-0.5, 0.5]])
-                dx = dy.rollaxes(-1)
-                discrete_gradient = [dx, dy]
-                # We are compressing 10% in lateral and 50% in normal direction
-                DelF = np.array([[-0.10, 0.0],
-                                 [0.0,  0.50]])
-                mat = µ.material.MaterialLinearElastic1_2d
+class FFTCheckSerialOnly(unittest.TestCase):
+    def setUp(self):
+        #               v- grid
+        #                      v-components
+        self.grids = [([8, 4], (2, 3)),
+                      ([6, 4], (1,)),
+                      ([6, 4, 5], (2, 3)),
+                      ([6, 4, 4], (1,))]
+
+        if muFFT.has_mpi:
+            from mpi4py import MPI
+            self.communicator = muFFT.Communicator(MPI.COMM_WORLD)
+        else:
+            self.communicator = muFFT.Communicator()
+
+        self.engines = []
+        if muFFT.has_mpi:
+            self.engines = ['fftwmpi', 'pfft']
+        if self.communicator.size == 1:
+            self.engines += ['pocketfft', 'fftw']
+
+    @unittest.skipIf(communicator.size > 1,
+                     'fftw only')
+    def test_rffth2c_2d_sin(self):
+
+        try:
+            engine = muFFT.FFT([5, 5], fft="fftw",
+                               allow_temporary_buffer=False,
+                               allow_destroy_input=True)
+        except muFFT.UnkownFFTEngineError:
+            return
+
+        in_data = np.cos(np.pi * 2 * np.arange(5) / 5).reshape(1, -1) * np.ones((5, 1))
+        out_data = np.zeros((5, 5), dtype=float)
+
+        # Allocate buffers and create plan for one degree of freedom
+        real_buffer = engine.register_halfcomplex_field(
+            "real-space", 1)
+        fourier_buffer = engine.register_halfcomplex_field(
+            "fourier-space", 1)
+
+        real_buffer.array()[...] = np.cos(np.pi * 2 * np.arange(5) / 5).reshape(1, -1) * np.ones((5, 1))
+
+        engine.hcfft(real_buffer, fourier_buffer)
+
+        expected = np.zeros((5, 5))
+        expected[0, 1] = 1 / 2 / engine.normalisation
+        np.testing.assert_allclose(fourier_buffer, expected, atol=1e-14)
+
+        real_buffer.array()[...] = np.sin(np.pi * 2 * np.arange(5) / 5).reshape(1, -1) * np.ones((5, 1))
+
+        engine.hcfft(real_buffer, fourier_buffer)
+
+        expected = np.zeros((5, 5))
+
+        # The halfcomplex array is:     
+        # r0, r1, r2, ..., rn/2, i(n+1)/2-1, ..., i2, i1
+        # with r, i the real and imaginary parts of the first half of the complex spectrum
+        # Euler formula: 
+        # sin = - i * 1/2 * (e^qx - e^-qx ) 
+        expected[0, -1] = - 1 / 2 / engine.normalisation
+        np.testing.assert_allclose(fourier_buffer, expected, atol=1e-14)
+
+    @unittest.skipIf(communicator.size > 1,
+                     'fftw only')
+    def test_rffth2c_2d_roundtrip(self):
+
+        for nb_grid_pts in [(5, 5), (4, 4), (4, 5), (5, 4)]:
+            nx, ny = nb_grid_pts
+
+            try:
+                engine = muFFT.FFT(nb_grid_pts, fft="fftw",
+                                   allow_temporary_buffer=False,
+                                   allow_destroy_input=True)
+            except muFFT.UnkownFFTEngineError:
+                return
+
+            # Allocate buffers and create plan for one degree of freedom
+            real_buffer = engine.register_halfcomplex_field(
+                "real-space", 1)
+            fourier_buffer = engine.register_halfcomplex_field(
+                "fourier-space", 1)
+
+            original = np.random.normal(size=nb_grid_pts)
+            real_buffer.array()[...] = original.copy()
+
+            engine.hcfft(real_buffer, fourier_buffer)
+            engine.ihcfft(fourier_buffer, real_buffer)
+            real_buffer.array()[...] *= engine.normalisation
+            np.testing.assert_allclose(real_buffer, original, atol=1e-14)
+
+    @unittest.skipIf(communicator.size > 1, 'fftw only')
+    def test_rffth2c_2d_convenience_interface(self):
+
+        nb_grid_pts = (5, 5)
+        nx, ny = nb_grid_pts
+
+        try:
+            engine = muFFT.FFT(nb_grid_pts, fft="fftw")
+        except muFFT.UnkownFFTEngineError:
+            return
+        engine.create_plan(1)
+
+        original = np.random.normal(size=nb_grid_pts)
+        original_backup = original.copy()
+        result_real = np.empty(nb_grid_pts,
+                               dtype=float, order='f')
+        result_fourier = result_real.copy()
+
+        engine.hcfft(original, result_fourier)
+        engine.ihcfft(result_fourier, result_real)
+
+        result_real *= engine.normalisation
+
+        np.testing.assert_allclose(original_backup, original, atol=1e-14)
+        np.testing.assert_allclose(result_real, original, atol=1e-14)
+
+    @unittest.skipIf(communicator.size > 1, 'fftw only')
+    def test_rffth2c_multiple_dofs(self):
+        for nb_grid_pts, dims in self.grids:
+            s = self.communicator.size
+            nb_grid_pts = s * np.array(nb_grid_pts)
+            try:
+                engine = muFFT.FFT(nb_grid_pts,
+                                   fft="fftw",
+                                   communicator=self.communicator)
+                engine.create_plan(np.prod(dims))
+            except muFFT.UnknownFFTEngineError:
+                # This FFT engine has not been compiled into the code. Skip
+                # test.
+                continue
+
+            if len(nb_grid_pts) == 2:
+                axes = (0, 1)
+            elif len(nb_grid_pts) == 3:
+                axes = (0, 1, 2)
             else:
-                dz = muFFT.DiscreteDerivative([0, 0, 0],
-                                              [[[-0.25, 0.25], [-0.25, 0.25]],
-                                               [[-0.25, 0.25], [-0.25, 0.25]]])
-                dy = dz.rollaxes(-1)
-                dx = dy.rollaxes(-1)
-                discrete_gradient = [dx, dy, dz]
-                # We are compressing 10% in lateral and 50% in normal direction
-                DelF = np.array([[-0.10,  0.0,  0.0],
-                                 [0.0,  -0.10,  0.0],
-                                 [0.0,  0.0,   0.50]])
-                mat = µ.material.MaterialLinearElastic1_3d
-
-            fourier_gradient = [µ.FourierDerivative(dim, d) for d in range(dim)]
-
-            lengths = [1.]*dim
-            nb_grid_pts = [nb_pts]*dim
-
-            for k, gradient_op in enumerate([fourier_gradient,
-                                             discrete_gradient]):
-                cell = µ.Cell(nb_grid_pts, lengths, form, gradient_op)
-
-                mat_vac = mat.make(cell, "vacuum", 0, 0)
-                mat_sol = mat.make(cell, "el", 1, Poisson)
-
-                for i, pixel in enumerate(cell.pixels):
-                    if np.array(pixel)[-1] == nb_grid_pts[-1]-1:
-                        mat_vac.add_pixel(i)
-                    else:
-                        mat_sol.add_pixel(i)
-
-                # Solver
-                newton_tol = 1e-8  # tolerance for newton algo
-                cg_tol = 1e-8  # tolerance for cg algo
-                equil_tol = 1e-8  # tolerance for equilibrium
-                maxiter = 1000
-                verbose = µ.Verbosity.Silent
-
-                solver = µ.solvers.KrylovSolverCG(cell, cg_tol, maxiter,
-                                            verbose)
-                cell.initialise()
-
-                result = µ.solvers.newton_cg(cell, DelF, solver,
-                                             newton_tol, equil_tol, verbose)
-
-                F = µ.gradient_integration.reshape_gradient(
-                    result.grad, list(cell.nb_subdomain_grid_pts))
-                PK1 = µ.gradient_integration.reshape_gradient(
-                    result.stress, list(cell.nb_subdomain_grid_pts))
-                displ, r = µ.gradient_integration.compute_placement(
-                    F, lengths, nb_grid_pts, gradient_op,
-                    formulation=µ.Formulation.finite_strain)
-
-                if dim == 2:
-                    x, y = displ
-                    if k == 0:
-                        # Fourier gradient
-                        self.assertAlmostEqual(
-                            y[0, -1] - y[0, -2],
-                            1.5-(nb_pts-1)/nb_pts*(1 + Poisson*0.1*dim),
-                            delta=0.05)
-                    else:
-                        # discrete gradient
-                        self.assertAlmostEqual(
-                            y[0, -1] - y[0, -2],
-                            1.5-(nb_pts-1)/nb_pts*(1 + Poisson*0.1*dim),
-                            delta=0.03)
-                else:
-                    x, y, z = displ
-                    if k == 0:
-                        # Fourier gradient
-                        self.assertAlmostEqual(
-                            z[0, 0, -1] - z[0, 0, -2],
-                            1.5-(nb_pts-1)/nb_pts*(1 + Poisson*0.1*dim),
-                            delta=0.05)
-                    else:
-                        # discrete gradient
-                        self.assertAlmostEqual(
-                            z[0, 0, -1] - z[0, 0, -2],
-                            1.5-(nb_pts-1)/nb_pts*(1 + Poisson*0.1*dim),
-                            delta=0.015)
+                raise RuntimeError('Cannot handle {}-dim transforms'
+                                   .format(len(nb_grid_pts)))
 
+            # We need to transpose the input to np.fft because muFFT
+            # uses column-major while np.fft uses row-major storage
+            np.random.seed(1)
+            global_in_arr = np.random.random([*dims, *nb_grid_pts])
+
+            in_arr = global_in_arr[(..., *engine.subdomain_slices)]
+
+            tol = 1e-14 * np.prod(nb_grid_pts)
+
+            # Separately test convenience interface
+            out_msp = global_in_arr.copy()
+            result_real = global_in_arr.copy()
+
+            engine.hcfft(in_arr, out_msp)
+            engine.ihcfft(out_msp, result_real)
+            result_real *= engine.normalisation
+
+            np.testing.assert_allclose(result_real, in_arr, atol=1e-14)
+
+    @unittest.skipIf(communicator.size > 1, 'fftw only')
+    def test_rffth2c_1d_roundtrip(self):
+
+        for nb_grid_pts in [(5,), (4,)]:
+            nx, = nb_grid_pts
+
+            engine = muFFT.FFT(nb_grid_pts, fft="fftw",
+                               allow_temporary_buffer=False,
+                               allow_destroy_input=True)
+
+            # Allocate buffers and create plan for one degree of freedom
+            real_buffer = engine.register_halfcomplex_field(
+                "real-space", 1)
+            fourier_buffer = engine.register_halfcomplex_field(
+                "fourier-space", 1)
+
+            original = np.random.normal(size=nb_grid_pts)
+            real_buffer.array()[...] = original.copy()
+
+            engine.hcfft(real_buffer, fourier_buffer)
+            engine.ihcfft(fourier_buffer, real_buffer)
+            real_buffer.array()[...] *= engine.normalisation
+            np.testing.assert_allclose(real_buffer, original, atol=1e-14)
+
+    @unittest.skipIf(communicator.size > 1, 'fftw only')
+    def test_rffth2c_3d_roundtrip(self):
+
+        for nb_grid_pts in [(5, 4, 5), (4, 5, 4), (4, 4, 5), (5, 5, 5), (4, 4, 4)]:
+            engine = muFFT.FFT(nb_grid_pts, fft="fftw",
+                               allow_temporary_buffer=False,
+                               allow_destroy_input=True)
+
+            # Allocate buffers and create plan for one degree of freedom
+            real_buffer = engine.register_halfcomplex_field(
+                "real-space", 1)
+            fourier_buffer = engine.register_halfcomplex_field(
+                "fourier-space", 1)
+
+            original = np.random.normal(size=nb_grid_pts)
+            real_buffer.array()[...] = original.copy()
+
+            engine.hcfft(real_buffer, fourier_buffer)
+            engine.ihcfft(fourier_buffer, real_buffer)
+            real_buffer.array()[...] *= engine.normalisation
+            np.testing.assert_allclose(real_buffer, original, atol=1e-14)
+
+    @unittest.skipIf(communicator.size > 1,
+                     'This test only works on a single MPI process')
+    def test_r2hc_incompatible_engines_raise(self):
+        for engine in self.engines:
+            try:
+                engine = muFFT.FFT([3, 5], fft=engine,
+                                   allow_temporary_buffer=False,
+                                   allow_destroy_input=True)
+            except muFFT.UnknownFFTEngineError:  # One of the engines is not installed, skip it
+                continue
+            # Allocate buffers and create plan for one degree of freedom
+            real_buffer = engine.register_halfcomplex_field(
+                "real-space", 1)
+            fourier_buffer = engine.register_halfcomplex_field(
+                "fourier-space", 1)
+            with self.assertRaises(RuntimeError) as context:
+                engine.hcfft(real_buffer, fourier_buffer)
 
+            self.assertTrue("not implemented " in str(context.exception), str(context.exception))
 
 
 if __name__ == '__main__':
     unittest.main()
```

