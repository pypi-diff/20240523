# Comparing `tmp/aiida_gromacs-2.0.7.tar.gz` & `tmp/aiida_gromacs-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_gromacs-2.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_gromacs-2.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_gromacs-2.0.7.tar` & `aiida_gromacs-2.0.8.tar`

### file list

```diff
@@ -1,120 +1,118 @@
--rw-r--r--   0        0        0      570 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/.github/workflows/auto-generate-release.yml
--rw-r--r--   0        0        0     2079 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1050 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/.github/workflows/publish-on-pypi.yml
--rw-r--r--   0        0        0      266 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/.gitignore
--rw-r--r--   0        0        0      820 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      161 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/.readthedocs.yml
--rw-r--r--   0        0        0     1076 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/LICENSE
--rw-r--r--   0        0        0     1697 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/README.md
--rw-r--r--   0        0        0      121 2024-01-23 11:59:23.394197 aiida_gromacs-2.0.7/aiida_gromacs/__init__.py
--rw-r--r--   0        0        0       97 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/aiida_gromacs/calculations/__init__.py
--rw-r--r--   0        0        0     4141 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/aiida_gromacs/calculations/editconf.py
--rw-r--r--   0        0        0     6144 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/aiida_gromacs/calculations/genericMD.py
--rw-r--r--   0        0        0     3839 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/aiida_gromacs/calculations/genion.py
--rw-r--r--   0        0        0     6046 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/aiida_gromacs/calculations/grompp.py
--rw-r--r--   0        0        0     4732 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/aiida_gromacs/calculations/make_ndx.py
--rw-r--r--   0        0        0     7349 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/aiida_gromacs/calculations/mdrun.py
--rw-r--r--   0        0        0     3837 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/aiida_gromacs/calculations/pdb2gmx.py
--rw-r--r--   0        0        0     3438 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/aiida_gromacs/calculations/solvate.py
--rw-r--r--   0        0        0      991 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/aiida_gromacs/cli/createarchive.py
--rwxr-xr-x   0        0        0     5511 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/aiida_gromacs/cli/editconf.py
--rwxr-xr-x   0        0        0     5613 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/aiida_gromacs/cli/genericMD.py
--rw-r--r--   0        0        0     4261 2024-01-23 11:59:14.462143 aiida_gromacs-2.0.7/aiida_gromacs/cli/genion.py
--rw-r--r--   0        0        0     6738 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/cli/grompp.py
--rw-r--r--   0        0        0     3803 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/cli/make_ndx.py
--rw-r--r--   0        0        0     9809 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/cli/mdrun.py
--rw-r--r--   0        0        0     5545 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/cli/pdb2gmx.py
--rw-r--r--   0        0        0     3943 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/cli/solvate.py
--rw-r--r--   0        0        0       97 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/data/__init__.py
--rw-r--r--   0        0        0     3392 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/data/editconf.py
--rw-r--r--   0        0        0     3081 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/data/genion.py
--rw-r--r--   0        0        0     3457 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/data/grompp.py
--rw-r--r--   0        0        0     2677 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/data/make_ndx.py
--rw-r--r--   0        0        0     5065 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/data/mdrun.py
--rw-r--r--   0        0        0     3371 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/data/pdb2gmx.py
--rw-r--r--   0        0        0     2722 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/data/solvate.py
--rw-r--r--   0        0        0     2836 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/helpers.py
--rw-r--r--   0        0        0       96 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/parsers/__init__.py
--rw-r--r--   0        0        0     2848 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/parsers/editconf.py
--rw-r--r--   0        0        0     4231 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/parsers/genericMD.py
--rw-r--r--   0        0        0     2502 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/parsers/genion.py
--rw-r--r--   0        0        0     2898 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/parsers/grompp.py
--rw-r--r--   0        0        0     2809 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/parsers/make_ndx.py
--rw-r--r--   0        0        0     5302 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/parsers/mdrun.py
--rw-r--r--   0        0        0     2948 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/parsers/pdb2gmx.py
--rw-r--r--   0        0        0     2509 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/parsers/solvate.py
--rw-r--r--   0        0        0     9817 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/utils/fileparsers.py
--rwxr-xr-x   0        0        0     3431 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/utils/inspectdb.py
--rwxr-xr-x   0        0        0      824 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/utils/querydb.py
--rw-r--r--   0        0        0     6850 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/utils/searchprevious.py
--rw-r--r--   0        0        0     3587 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/utils/topfile_utils.py
--rw-r--r--   0        0        0       97 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/workflows/__init__.py
--rw-r--r--   0        0        0    11987 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/aiida_gromacs/workflows/simsetup.py
--rw-r--r--   0        0        0      674 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/conftest.py
--rw-r--r--   0        0        0     5414 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/docker/github-actions/Dockerfile
--rw-r--r--   0        0        0     1065 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/docker/github-actions/fix-permissions
--rw-r--r--   0        0        0      163 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/docker/github-actions/initial-condarc
--rw-r--r--   0        0        0        7 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/docs/.gitignore
--rwxr-xr-x   0        0        0     1541 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/docs/Makefile
--rwxr-xr-x   0        0        0    11390 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/docs/source/conf.py
--rw-r--r--   0        0        0     4617 2024-01-23 11:59:14.466143 aiida_gromacs-2.0.7/docs/source/developer_guide/index.rst
--rw-r--r--   0        0        0   847801 2024-01-23 11:59:14.470143 aiida_gromacs-2.0.7/docs/source/images/53.dot.png
--rw-r--r--   0        0        0    76300 2024-01-23 11:59:14.470143 aiida_gromacs-2.0.7/docs/source/images/AiiDA_transparent_logo.png
--rwxr-xr-x   0        0        0     1321 2024-01-23 11:59:14.470143 aiida_gromacs-2.0.7/docs/source/index.rst
--rw-r--r--   0        0        0     5365 2024-01-23 11:59:14.470143 aiida_gromacs-2.0.7/docs/source/tutorials/genericMD.rst
--rw-r--r--   0        0        0      381 2024-01-23 11:59:14.470143 aiida_gromacs-2.0.7/docs/source/tutorials/index.rst
--rw-r--r--   0        0        0     3516 2024-01-23 11:59:14.470143 aiida_gromacs-2.0.7/docs/source/tutorials/lysozyme.rst
--rw-r--r--   0        0        0     2262 2024-01-23 11:59:14.470143 aiida_gromacs-2.0.7/docs/source/user_guide/aiida_cheatsheet.rst
--rw-r--r--   0        0        0     3370 2024-01-23 11:59:14.470143 aiida_gromacs-2.0.7/docs/source/user_guide/aiida_sessions.rst
--rw-r--r--   0        0        0    19315 2024-01-23 11:59:14.470143 aiida_gromacs-2.0.7/docs/source/user_guide/api_interface.rst
--rw-r--r--   0        0        0     8592 2024-01-23 11:59:14.470143 aiida_gromacs-2.0.7/docs/source/user_guide/cli_interface.rst
--rw-r--r--   0        0        0     1045 2024-01-23 11:59:14.470143 aiida_gromacs-2.0.7/docs/source/user_guide/index.rst
--rw-r--r--   0        0        0     2712 2024-01-23 11:59:14.470143 aiida_gromacs-2.0.7/docs/source/user_guide/installation.rst
--rwxr-xr-x   0        0        0     1823 2024-01-23 11:59:14.470143 aiida_gromacs-2.0.7/examples/gromacs-jobs.sh
--rw-r--r--   0        0        0    95531 2024-01-23 11:59:14.474143 aiida_gromacs-2.0.7/examples/gromacs_files/1AKI_clean.pdb
--rw-r--r--   0        0        0     1044 2024-01-23 11:59:14.474143 aiida_gromacs-2.0.7/examples/gromacs_files/ions.mdp
--rw-r--r--   0        0        0     1045 2024-01-23 11:59:14.474143 aiida_gromacs-2.0.7/examples/gromacs_files/min.mdp
--rw-r--r--   0        0        0     2586 2024-01-23 11:59:14.474143 aiida_gromacs-2.0.7/examples/gromacs_files/npt.mdp
--rw-r--r--   0        0        0     2366 2024-01-23 11:59:14.474143 aiida_gromacs-2.0.7/examples/gromacs_files/nvt.mdp
--rw-r--r--   0        0        0     2737 2024-01-23 11:59:14.474143 aiida_gromacs-2.0.7/examples/gromacs_files/prod.mdp
-lrwxr-xr-x   0        0        0        0 2024-01-23 11:59:14.474143 aiida_gromacs-2.0.7/notebooks/gromacs_files -> ../examples/gromacs_files/
--rw-r--r--   0        0        0    16673 2024-01-23 11:59:14.474143 aiida_gromacs-2.0.7/notebooks/lysozyme_tutorial.ipynb
--rw-r--r--   0        0        0     5297 2024-01-23 11:59:14.474143 aiida_gromacs-2.0.7/pyproject.toml
--rw-r--r--   0        0        0      215 2024-01-23 11:59:14.474143 aiida_gromacs-2.0.7/tests/__init__.py
--rw-r--r--   0        0        0    31304 2024-01-23 11:59:14.474143 aiida_gromacs-2.0.7/tests/input_files/1AKI_restraints.itp
--rw-r--r--   0        0        0        0 2024-01-23 11:59:14.474143 aiida_gromacs-2.0.7/tests/input_files/__init__.py
--rw-r--r--   0        0        0    88246 2024-01-23 11:59:14.474143 aiida_gromacs-2.0.7/tests/input_files/editconf_1AKI_forcefield.gro
--rw-r--r--   0        0        0  1266952 2024-01-23 11:59:14.478143 aiida_gromacs-2.0.7/tests/input_files/genion_1AKI_ions.tpr
--rw-r--r--   0        0        0   553082 2024-01-23 11:59:14.482143 aiida_gromacs-2.0.7/tests/input_files/genion_1AKI_topology.top
--rw-r--r--   0        0        0  1527580 2024-01-23 11:59:14.486143 aiida_gromacs-2.0.7/tests/input_files/grompp2_1AKI_solvated_ions.gro
--rw-r--r--   0        0        0   553101 2024-01-23 11:59:14.486143 aiida_gromacs-2.0.7/tests/input_files/grompp2_1AKI_topology.top
--rw-r--r--   0        0        0     1045 2024-01-23 11:59:14.486143 aiida_gromacs-2.0.7/tests/input_files/grompp2_min.mdp
--rw-r--r--   0        0        0  1527580 2024-01-23 11:59:14.494143 aiida_gromacs-2.0.7/tests/input_files/grompp3_1AKI_minimised.gro
--rw-r--r--   0        0        0     2369 2024-01-23 11:59:14.494143 aiida_gromacs-2.0.7/tests/input_files/grompp3_nvt.mdp
--rw-r--r--   0        0        0  1525186 2024-01-23 11:59:14.498143 aiida_gromacs-2.0.7/tests/input_files/grompp_1AKI_solvated.gro
--rw-r--r--   0        0        0   553082 2024-01-23 11:59:14.498143 aiida_gromacs-2.0.7/tests/input_files/grompp_1AKI_topology.top
--rw-r--r--   0        0        0     1045 2024-01-23 11:59:14.498143 aiida_gromacs-2.0.7/tests/input_files/grompp_ions.mdp
--rw-r--r--   0        0        0  1178036 2024-01-23 11:59:14.502143 aiida_gromacs-2.0.7/tests/input_files/make_ndx_index.ndx
--rw-r--r--   0        0        0       34 2024-01-23 11:59:14.502143 aiida_gromacs-2.0.7/tests/input_files/make_ndx_interactive_inputs.txt
--rw-r--r--   0        0        0  1267460 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/input_files/mdrun_1AKI_em.tpr
--rw-r--r--   0        0        0   109917 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/input_files/pdb2gmx_1AKI_clean.pdb
--rw-r--r--   0        0        0    88246 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/input_files/solvate_1AKI_newbox.gro
--rw-r--r--   0        0        0   553051 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/input_files/solvate_1AKI_topology.top
--rw-r--r--   0        0        0     1580 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_calcs_editconf.py
--rw-r--r--   0        0        0     3722 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_calcs_genericMD.py
--rw-r--r--   0        0        0     1905 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_calcs_genion.py
--rw-r--r--   0        0        0     1753 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_calcs_grompp.py
--rw-r--r--   0        0        0     2091 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_calcs_make_gmx.py
--rw-r--r--   0        0        0     2310 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_calcs_mdrun.py
--rw-r--r--   0        0        0     1946 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_calcs_pdb2gmx.py
--rw-r--r--   0        0        0     1843 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_calcs_solvate.py
--rw-r--r--   0        0        0     1016 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_cli_editconf.py
--rw-r--r--   0        0        0     1576 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_cli_genericMD.py
--rw-r--r--   0        0        0     1135 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_cli_genion.py
--rw-r--r--   0        0        0     3118 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_cli_grompp.py
--rw-r--r--   0        0        0     1070 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_cli_make_ndx.py
--rw-r--r--   0        0        0     1201 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_cli_mdrun.py
--rw-r--r--   0        0        0     1079 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_cli_pdb2gmx.py
--rw-r--r--   0        0        0     1060 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_cli_solvate.py
--rw-r--r--   0        0        0     3317 2024-01-23 11:59:14.510143 aiida_gromacs-2.0.7/tests/test_utils_searchprevious.py
--rw-r--r--   0        0        0     3230 1970-01-01 00:00:00.000000 aiida_gromacs-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2621 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/.github/workflows/auto-release.yml
+-rw-r--r--   0        0        0     2579 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      266 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/.gitignore
+-rw-r--r--   0        0        0      820 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      161 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/.readthedocs.yml
+-rw-r--r--   0        0        0     1076 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/LICENSE
+-rw-r--r--   0        0        0     1637 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/README.md
+-rw-r--r--   0        0        0      121 2024-05-23 15:14:55.765488 aiida_gromacs-2.0.8/aiida_gromacs/__init__.py
+-rw-r--r--   0        0        0       97 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/calculations/__init__.py
+-rw-r--r--   0        0        0     4342 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/calculations/editconf.py
+-rw-r--r--   0        0        0     6020 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/calculations/genericMD.py
+-rw-r--r--   0        0        0     4698 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/calculations/genion.py
+-rw-r--r--   0        0        0     6247 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/calculations/grompp.py
+-rw-r--r--   0        0        0     4933 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/calculations/make_ndx.py
+-rw-r--r--   0        0        0     7550 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/calculations/mdrun.py
+-rw-r--r--   0        0        0     4038 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/calculations/pdb2gmx.py
+-rw-r--r--   0        0        0     3639 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/calculations/solvate.py
+-rw-r--r--   0        0        0      991 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/cli/createarchive.py
+-rwxr-xr-x   0        0        0     5778 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/cli/editconf.py
+-rwxr-xr-x   0        0        0     5119 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/cli/genericMD.py
+-rw-r--r--   0        0        0     5249 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/cli/genion.py
+-rw-r--r--   0        0        0     7044 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/cli/grompp.py
+-rw-r--r--   0        0        0     4069 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/cli/make_ndx.py
+-rw-r--r--   0        0        0    10073 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/cli/mdrun.py
+-rw-r--r--   0        0        0     5988 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/cli/pdb2gmx.py
+-rw-r--r--   0        0        0     4246 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/cli/solvate.py
+-rw-r--r--   0        0        0      528 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/commands/provenance.py
+-rw-r--r--   0        0        0       97 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/data/__init__.py
+-rw-r--r--   0        0        0     3392 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/data/editconf.py
+-rw-r--r--   0        0        0     3660 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/data/genion.py
+-rw-r--r--   0        0        0     3457 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/data/grompp.py
+-rw-r--r--   0        0        0     2677 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/data/make_ndx.py
+-rw-r--r--   0        0        0     5065 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/data/mdrun.py
+-rw-r--r--   0        0        0     3371 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/data/pdb2gmx.py
+-rw-r--r--   0        0        0     2722 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/data/solvate.py
+-rw-r--r--   0        0        0     3504 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/helpers.py
+-rw-r--r--   0        0        0       96 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/parsers/__init__.py
+-rw-r--r--   0        0        0     2848 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/parsers/editconf.py
+-rw-r--r--   0        0        0     4163 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/parsers/genericMD.py
+-rw-r--r--   0        0        0     2502 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/parsers/genion.py
+-rw-r--r--   0        0        0     2898 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/parsers/grompp.py
+-rw-r--r--   0        0        0     2809 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/parsers/make_ndx.py
+-rw-r--r--   0        0        0     6599 2024-05-23 15:14:46.461433 aiida_gromacs-2.0.8/aiida_gromacs/parsers/mdrun.py
+-rw-r--r--   0        0        0     2948 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/aiida_gromacs/parsers/pdb2gmx.py
+-rw-r--r--   0        0        0     2509 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/aiida_gromacs/parsers/solvate.py
+-rw-r--r--   0        0        0     2484 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/aiida_gromacs/utils/displayprovenance.py
+-rw-r--r--   0        0        0     9898 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/aiida_gromacs/utils/fileparsers.py
+-rwxr-xr-x   0        0        0     3431 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/aiida_gromacs/utils/inspectdb.py
+-rwxr-xr-x   0        0        0      824 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/aiida_gromacs/utils/querydb.py
+-rw-r--r--   0        0        0     7854 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/aiida_gromacs/utils/searchprevious.py
+-rw-r--r--   0        0        0     3587 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/aiida_gromacs/utils/topfile_utils.py
+-rw-r--r--   0        0        0       97 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/aiida_gromacs/workflows/__init__.py
+-rw-r--r--   0        0        0    11987 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/aiida_gromacs/workflows/simsetup.py
+-rw-r--r--   0        0        0      674 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/conftest.py
+-rw-r--r--   0        0        0        7 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/docs/.gitignore
+-rwxr-xr-x   0        0        0     1541 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/docs/Makefile
+-rwxr-xr-x   0        0        0    11430 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/docs/source/conf.py
+-rw-r--r--   0        0        0     5216 2024-05-23 15:14:46.465433 aiida_gromacs-2.0.8/docs/source/developer_guide/index.rst
+-rw-r--r--   0        0        0   847801 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/docs/source/images/53.dot.png
+-rw-r--r--   0        0        0    76300 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/docs/source/images/AiiDA_transparent_logo.png
+-rwxr-xr-x   0        0        0     1306 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/docs/source/index.rst
+-rw-r--r--   0        0        0     5365 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/docs/source/tutorials/genericMD.rst
+-rw-r--r--   0        0        0      381 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/docs/source/tutorials/index.rst
+-rw-r--r--   0        0        0     3516 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/docs/source/tutorials/lysozyme.rst
+-rw-r--r--   0        0        0     2262 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/docs/source/user_guide/aiida_cheatsheet.rst
+-rw-r--r--   0        0        0     3370 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/docs/source/user_guide/aiida_sessions.rst
+-rw-r--r--   0        0        0    19315 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/docs/source/user_guide/api_interface.rst
+-rw-r--r--   0        0        0     8592 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/docs/source/user_guide/cli_interface.rst
+-rw-r--r--   0        0        0     1045 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/docs/source/user_guide/index.rst
+-rw-r--r--   0        0        0     2712 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/docs/source/user_guide/installation.rst
+-rwxr-xr-x   0        0        0     1823 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/examples/gromacs-jobs.sh
+-rw-r--r--   0        0        0    95531 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/examples/gromacs_files/1AKI_clean.pdb
+-rw-r--r--   0        0        0     1044 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/examples/gromacs_files/ions.mdp
+-rw-r--r--   0        0        0     1045 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/examples/gromacs_files/min.mdp
+-rw-r--r--   0        0        0     2586 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/examples/gromacs_files/npt.mdp
+-rw-r--r--   0        0        0     2366 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/examples/gromacs_files/nvt.mdp
+-rw-r--r--   0        0        0     2737 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/examples/gromacs_files/prod.mdp
+lrwxr-xr-x   0        0        0        0 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/notebooks/gromacs_files -> ../examples/gromacs_files/
+-rw-r--r--   0        0        0    16673 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/notebooks/lysozyme_tutorial.ipynb
+-rw-r--r--   0        0        0     5391 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0      215 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/tests/__init__.py
+-rw-r--r--   0        0        0    31304 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/tests/input_files/1AKI_restraints.itp
+-rw-r--r--   0        0        0        0 2024-05-23 15:14:46.469433 aiida_gromacs-2.0.8/tests/input_files/__init__.py
+-rw-r--r--   0        0        0    88246 2024-05-23 15:14:46.473433 aiida_gromacs-2.0.8/tests/input_files/editconf_1AKI_forcefield.gro
+-rw-r--r--   0        0        0  1266952 2024-05-23 15:14:46.477433 aiida_gromacs-2.0.8/tests/input_files/genion_1AKI_ions.tpr
+-rw-r--r--   0        0        0   553082 2024-05-23 15:14:46.477433 aiida_gromacs-2.0.8/tests/input_files/genion_1AKI_topology.top
+-rw-r--r--   0        0        0  1527580 2024-05-23 15:14:46.485433 aiida_gromacs-2.0.8/tests/input_files/grompp2_1AKI_solvated_ions.gro
+-rw-r--r--   0        0        0   553101 2024-05-23 15:14:46.485433 aiida_gromacs-2.0.8/tests/input_files/grompp2_1AKI_topology.top
+-rw-r--r--   0        0        0     1045 2024-05-23 15:14:46.485433 aiida_gromacs-2.0.8/tests/input_files/grompp2_min.mdp
+-rw-r--r--   0        0        0  1527580 2024-05-23 15:14:46.489433 aiida_gromacs-2.0.8/tests/input_files/grompp3_1AKI_minimised.gro
+-rw-r--r--   0        0        0     2369 2024-05-23 15:14:46.489433 aiida_gromacs-2.0.8/tests/input_files/grompp3_nvt.mdp
+-rw-r--r--   0        0        0  1525186 2024-05-23 15:14:46.497433 aiida_gromacs-2.0.8/tests/input_files/grompp_1AKI_solvated.gro
+-rw-r--r--   0        0        0   553082 2024-05-23 15:14:46.497433 aiida_gromacs-2.0.8/tests/input_files/grompp_1AKI_topology.top
+-rw-r--r--   0        0        0     1045 2024-05-23 15:14:46.497433 aiida_gromacs-2.0.8/tests/input_files/grompp_ions.mdp
+-rw-r--r--   0        0        0  1178036 2024-05-23 15:14:46.501433 aiida_gromacs-2.0.8/tests/input_files/make_ndx_index.ndx
+-rw-r--r--   0        0        0       34 2024-05-23 15:14:46.501433 aiida_gromacs-2.0.8/tests/input_files/make_ndx_interactive_inputs.txt
+-rw-r--r--   0        0        0  1267460 2024-05-23 15:14:46.505433 aiida_gromacs-2.0.8/tests/input_files/mdrun_1AKI_em.tpr
+-rw-r--r--   0        0        0   109917 2024-05-23 15:14:46.505433 aiida_gromacs-2.0.8/tests/input_files/pdb2gmx_1AKI_clean.pdb
+-rw-r--r--   0        0        0    88246 2024-05-23 15:14:46.505433 aiida_gromacs-2.0.8/tests/input_files/solvate_1AKI_newbox.gro
+-rw-r--r--   0        0        0   553051 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/input_files/solvate_1AKI_topology.top
+-rw-r--r--   0        0        0     1580 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_calcs_editconf.py
+-rw-r--r--   0        0        0     3722 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_calcs_genericMD.py
+-rw-r--r--   0        0        0     1905 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_calcs_genion.py
+-rw-r--r--   0        0        0     1753 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_calcs_grompp.py
+-rw-r--r--   0        0        0     2091 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_calcs_make_gmx.py
+-rw-r--r--   0        0        0     2310 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_calcs_mdrun.py
+-rw-r--r--   0        0        0     1946 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_calcs_pdb2gmx.py
+-rw-r--r--   0        0        0     1843 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_calcs_solvate.py
+-rw-r--r--   0        0        0     1016 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_cli_editconf.py
+-rw-r--r--   0        0        0     1576 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_cli_genericMD.py
+-rw-r--r--   0        0        0     1135 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_cli_genion.py
+-rw-r--r--   0        0        0     3118 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_cli_grompp.py
+-rw-r--r--   0        0        0     1070 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_cli_make_ndx.py
+-rw-r--r--   0        0        0     1201 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_cli_mdrun.py
+-rw-r--r--   0        0        0     1079 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_cli_pdb2gmx.py
+-rw-r--r--   0        0        0     1060 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_cli_solvate.py
+-rw-r--r--   0        0        0     3317 2024-05-23 15:14:46.509433 aiida_gromacs-2.0.8/tests/test_utils_searchprevious.py
+-rw-r--r--   0        0        0     3157 1970-01-01 00:00:00.000000 aiida_gromacs-2.0.8/PKG-INFO
```

### Comparing `aiida_gromacs-2.0.7/.github/workflows/ci.yml` & `aiida_gromacs-2.0.8/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,32 @@
   push:
     branches: [master]
   pull_request:
 
 jobs:
 
   tests:
+    strategy:
+      matrix:
+        container: [py3.11.0]
+        aiida: [2.4.0, 2.4.1, 2.4.2, 2.5.0]
+        gmx: [2023.1=nompi_h76c6bb2_100,
+              2022.4=nompi_hca75aac_100]
     runs-on: ubuntu-latest
     timeout-minutes: 30
     container:
-        image: harbor.stfc.ac.uk/biosimulation-cloud/aiida-testenv:0.2
+        image: harbor.stfc.ac.uk/biosimulation-cloud/aiida-testbase:${{ matrix.container }}
+    name: container = ${{ matrix.container }}, aiida = ${{ matrix.aiida }}, gmx = ${{ matrix.gmx }}
     steps:
     - uses: actions/checkout@v4
 
+    - name: Install conda packages
+      shell: bash
+      run: mamba install gromacs=${{ matrix.gmx }} aiida-core=${{ matrix.aiida }} aiida-core.services=${{ matrix.aiida }} -c conda-forge -yq
+
     - name: Initialise PostGRES DB
       shell: bash
       run: initdb -D /home/aiida/.aiida/aiida_db
 
     - name: Start PostGRES DB
       shell: bash
       run: pg_ctl -D /home/aiida/.aiida/aiida_db -l /home/aiida/.aiida/logfile start
```

### Comparing `aiida_gromacs-2.0.7/.pre-commit-config.yaml` & `aiida_gromacs-2.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/LICENSE` & `aiida_gromacs-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/README.md` & `aiida_gromacs-2.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-[![Build Status](https://github.com/PSDI-Biomolecular-team/aiida-gromacs/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/PSDI-Biomolecular-team/aiida-gromacs/actions/workflows/ci.yml)
-[![Coverage Status](https://coveralls.io/repos/github/PSDI-Biomolecular-team/aiida-gromacs/badge.svg?branch=master)](https://coveralls.io/github/PSDI-Biomolecular-team/aiida-gromacs?branch=master)
+[![Build Status](https://github.com/PSDI-UK/aiida-gromacs/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/PSDI-UK/aiida-gromacs/actions/workflows/ci.yml)
+[![Coverage Status](https://coveralls.io/repos/github/PSDI-UK/aiida-gromacs/badge.svg?branch=master)](https://coveralls.io/github/PSDI-UK/aiida-gromacs?branch=master)
 [![Docs status](https://readthedocs.org/projects/aiida-gromacs/badge)](http://aiida-gromacs.readthedocs.io/)
 [![PyPI version](https://badge.fury.io/py/aiida-gromacs.svg)](https://badge.fury.io/py/aiida-gromacs)
 
 # aiida-gromacs
 
 The GROMACS plugin for AiiDA aims to enable the capture and sharing of the full
 provenance of data when parameterising and running molecular dynamics
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/calculations/editconf.py` & `aiida_gromacs-2.0.8/aiida_gromacs/calculations/editconf.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This calculation configures the ability to use the 'gmx editconf' executable.
 """
 import os 
 
 from aiida.common import CalcInfo, CodeInfo
 from aiida.engine import CalcJob
-from aiida.orm import SinglefileData
+from aiida.orm import SinglefileData, Str
 from aiida.plugins import DataFactory
 
 EditconfParameters = DataFactory("gromacs.editconf")
 
 
 class EditconfCalculation(CalcJob):
     """
@@ -22,14 +22,19 @@
 
     @classmethod
     def define(cls, spec):
         """Define inputs and outputs of the calculation."""
         # yapf: disable
         super().define(spec)
 
+        # Define inputs and outputs of the calculation.
+        spec.input('command',
+                valid_type=Str, required=False,
+                help='The command used to execute the job.')
+
         # set default values for AiiDA options
         # TODO: something changed about withmpi in aiida-2.4.0, needs investigation.
         spec.inputs['metadata']['options']['withmpi'].default = False
         spec.inputs['metadata']['options']['resources'].default = {
             'num_machines': 1,
             'num_mpiprocs_per_machine': 1,
         }
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/calculations/genericMD.py` & `aiida_gromacs-2.0.8/aiida_gromacs/calculations/genericMD.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,14 @@
             'input_files',
             valid_type=SinglefileData,
             required=False,
             help='Dictionary of input files.',
             dynamic=True, # can take num of values unknown at time of definition
         )
 
-        spec.output('log', valid_type=SinglefileData, required=False,
-                help='link to the default file.out.')
 
         # set the list of output file names as an input so that it can be
         # iterated over in the parser later.
         spec.input('output_files', valid_type=List, required=False,
                    help='List of output file names.')
 
         # define the schema for metadata.options
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/calculations/genion.py` & `aiida_gromacs-2.0.8/aiida_gromacs/calculations/genion.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This calculation configures the ability to use the 'gmx genion' executable.
 """
 import os
 
 from aiida.common import CalcInfo, CodeInfo
 from aiida.engine import CalcJob
-from aiida.orm import SinglefileData
+from aiida.orm import SinglefileData, Str
 from aiida.plugins import DataFactory
 
 GenionParameters = DataFactory("gromacs.genion")
 
 
 class GenionCalculation(CalcJob):
     """
@@ -22,14 +22,19 @@
 
     @classmethod
     def define(cls, spec):
         """Define inputs and outputs of the calculation."""
         # yapf: disable
         super().define(spec)
 
+        # Define inputs and outputs of the calculation.
+        spec.input('command',
+                valid_type=Str, required=False,
+                help='The command used to execute the job.')
+
         # set default values for AiiDA options
         # TODO: something changed about withmpi in aiida-2.4.0, needs investigation.
         spec.inputs['metadata']['options']['withmpi'].default = False
         spec.inputs['metadata']['options']['resources'].default = {
             'num_machines': 1,
             'num_mpiprocs_per_machine': 1,
         }
@@ -40,14 +45,22 @@
         spec.input('tprfile', valid_type=SinglefileData, help='Input tpr file.')
         spec.input('topfile', valid_type=SinglefileData, help='Input topology file.')
         spec.input('parameters', valid_type=GenionParameters, help='Command line parameters for gmx genion')
         spec.input('metadata.options.output_dir', valid_type=str, default=os.getcwd(),
                 help='Directory where output files will be saved when parsed.')
 
         # Optional inputs.
+        spec.input(
+            'metadata.options.filename_stdin',
+            valid_type=str,
+            required=False,
+            help='Filename that should be redirected to the shell command using the stdin file descriptor.',
+        )
+        spec.input('instructions_file', valid_type=SinglefileData, required=False, help='Instructions for generating index file')
+        spec.input('metadata.options.stdin_filename', valid_type=str, required=False, help='name of file used in stdin.')
         spec.input('n_file', required=False, valid_type=SinglefileData, help='Index file.')
 
         # Default outputs.
         spec.output('stdout', valid_type=SinglefileData, help='stdout')
         spec.output('grofile', valid_type=SinglefileData, help='Output gro file with ions added.')
         spec.output('topfile', valid_type=SinglefileData, help='Output topology with ions added.')
 
@@ -60,15 +73,15 @@
         :param folder: an `aiida.common.folders.Folder` where the plugin should temporarily place all files
             needed by the calculation.
         :return: `aiida.common.datastructures.CalcInfo` instance
         """
         codeinfo = CodeInfo()
 
         # Setup data structures for files.
-        input_options = ["tprfile", "topfile", "n_file"]
+        input_options = ["tprfile", "topfile", "n_file", "instructions_file"]
         cmdline_input_files = {}
         input_files = []
 
         # Map input files to AiiDA plugin data types.
         for item in input_options:
             if item in self.inputs:
                 cmdline_input_files[item] = self.inputs[item].filename
@@ -76,14 +89,17 @@
                         self.inputs[item].uuid,
                         self.inputs[item].filename,
                         self.inputs[item].filename,
                     ))
 
         # Form the commandline.
         codeinfo.cmdline_params = self.inputs.parameters.cmdline_params(cmdline_input_files)
+
+        # Form stdin file for index instructions
+        codeinfo.stdin_name = self.inputs['metadata']['options'].get('stdin_filename', None)
         
         codeinfo.code_uuid = self.inputs.code.uuid
         codeinfo.stdout_name = self.metadata.options.output_filename
         codeinfo.withmpi = self.inputs.metadata.options.withmpi
 
         # Prepare a `CalcInfo` to be returned to the engine
         calcinfo = CalcInfo()
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/calculations/grompp.py` & `aiida_gromacs-2.0.8/aiida_gromacs/calculations/grompp.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This calculation configures the ability to use the 'gmx grompp' executable.
 """
 import os
 
 from aiida.common import CalcInfo, CodeInfo
 from aiida.engine import CalcJob
-from aiida.orm import SinglefileData, FolderData
+from aiida.orm import SinglefileData, FolderData, Str
 from aiida.plugins import DataFactory
 
 GromppParameters = DataFactory("gromacs.grompp")
 
 
 class GromppCalculation(CalcJob):
     """
@@ -22,14 +22,19 @@
 
     @classmethod
     def define(cls, spec):
         """Define inputs and outputs of the calculation."""
         # yapf: disable
         super().define(spec)
 
+        # Define inputs and outputs of the calculation.
+        spec.input('command',
+                valid_type=Str, required=False,
+                help='The command used to execute the job.')
+
         # set default values for AiiDA options
         # TODO: something changed about withmpi in aiida-2.4.0, needs investigation.
         spec.inputs['metadata']['options']['withmpi'].default = False
         spec.inputs['metadata']['options']['resources'].default = {
             'num_machines': 1,
             'num_mpiprocs_per_machine': 1,
         }
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/calculations/make_ndx.py` & `aiida_gromacs-2.0.8/aiida_gromacs/calculations/make_ndx.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This calculation configures the ability to use the 'gmx make_ndx' executable.
 """
 import os
 
 from aiida.common import CalcInfo, CodeInfo
 from aiida.engine import CalcJob
-from aiida.orm import SinglefileData
+from aiida.orm import SinglefileData, Str
 from aiida.plugins import DataFactory
 
 Make_ndxParameters = DataFactory("gromacs.make_ndx")
 
 
 class Make_ndxCalculation(CalcJob):
     """
@@ -22,14 +22,19 @@
 
     @classmethod
     def define(cls, spec):
         """Define inputs and outputs of the calculation."""
         # yapf: disable
         super().define(spec)
 
+        # Define inputs and outputs of the calculation.
+        spec.input('command',
+                valid_type=Str, required=False,
+                help='The command used to execute the job.')
+
         # set default values for AiiDA options
         # TODO: something changed about withmpi in aiida-2.4.0, needs investigation.
         spec.inputs['metadata']['options']['withmpi'].default = False
         # TODO: remove this for production release.
         spec.inputs['metadata']['options']['max_wallclock_seconds'].default = 86400
         spec.inputs['metadata']['options']['resources'].default = {
             'num_machines': 1,
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/calculations/mdrun.py` & `aiida_gromacs-2.0.8/aiida_gromacs/calculations/mdrun.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This calculation configures the ability to use the 'gmx mdrun' executable.
 """
 import os
 
 from aiida.common import CalcInfo, CodeInfo
 from aiida.engine import CalcJob
-from aiida.orm import SinglefileData, Dict
+from aiida.orm import SinglefileData, Dict, Str
 from aiida.plugins import DataFactory
 
 MdrunParameters = DataFactory("gromacs.mdrun")
 
 
 class MdrunCalculation(CalcJob):
     """
@@ -22,14 +22,19 @@
 
     @classmethod
     def define(cls, spec):
         """Define inputs and outputs of the calculation."""
         # yapf: disable
         super().define(spec)
 
+        # Define inputs and outputs of the calculation.
+        spec.input('command',
+                valid_type=Str, required=False,
+                help='The command used to execute the job.')
+
         # set default values for AiiDA options
         # TODO: something changed about withmpi in aiida-2.4.0, needs investigation.
         spec.inputs['metadata']['options']['withmpi'].default = False
         # TODO: remove this for production release.
         spec.inputs['metadata']['options']['max_wallclock_seconds'].default = 86400
         spec.inputs['metadata']['options']['resources'].default = {
             'num_machines': 1,
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/calculations/pdb2gmx.py` & `aiida_gromacs-2.0.8/aiida_gromacs/calculations/pdb2gmx.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This calculation configures the ability to use the 'gmx pdb2gmx' executable.
 """
 import os
 
 from aiida.common import CalcInfo, CodeInfo
 from aiida.engine import CalcJob
-from aiida.orm import SinglefileData
+from aiida.orm import SinglefileData, Str
 from aiida.plugins import DataFactory
 
 Pdb2gmxParameters = DataFactory("gromacs.pdb2gmx")
 
 
 class Pdb2gmxCalculation(CalcJob):
     """
@@ -22,14 +22,19 @@
 
     @classmethod
     def define(cls, spec):
         """Define inputs and outputs of the calculation."""
         # yapf: disable
         super().define(spec)
 
+        # Define inputs and outputs of the calculation.
+        spec.input('command',
+                valid_type=Str, required=False,
+                help='The command used to execute the job.')
+
         # set default values for AiiDA options
         # TODO: something changed about withmpi in aiida-2.4.0, needs investigation.
         spec.inputs['metadata']['options']['withmpi'].default = False
         spec.inputs['metadata']['options']['resources'].default = {
             'num_machines': 1,
             'num_mpiprocs_per_machine': 1,
         }
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/calculations/solvate.py` & `aiida_gromacs-2.0.8/aiida_gromacs/calculations/solvate.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This calculation configures the ability to use the 'gmx solvate' executable.
 """
 import os
 
 from aiida.common import CalcInfo, CodeInfo
 from aiida.engine import CalcJob
-from aiida.orm import SinglefileData
+from aiida.orm import SinglefileData, Str
 from aiida.plugins import DataFactory
 
 SolvateParameters = DataFactory("gromacs.solvate")
 
 
 class SolvateCalculation(CalcJob):
     """
@@ -22,14 +22,19 @@
 
     @classmethod
     def define(cls, spec):
         """Define inputs and outputs of the calculation."""
         # yapf: disable
         super().define(spec)
 
+        # Define inputs and outputs of the calculation.
+        spec.input('command',
+                valid_type=Str, required=False,
+                help='The command used to execute the job.')
+
         # set default values for AiiDA options
         # TODO: something changed about withmpi in aiida-2.4.0, needs investigation.
         spec.inputs['metadata']['options']['withmpi'].default = False
         spec.inputs['metadata']['options']['resources'].default = {
             'num_machines': 1,
             'num_mpiprocs_per_machine': 1,
         }
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/cli/createarchive.py` & `aiida_gromacs-2.0.8/aiida_gromacs/cli/createarchive.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/cli/editconf.py` & `aiida_gromacs-2.0.8/aiida_gromacs/cli/editconf.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Usage: gmx_editconf --help
 """
 
 import os
 
 import click
 
-from aiida import cmdline, engine
+from aiida import cmdline, engine, orm
 from aiida.plugins import CalculationFactory, DataFactory
 
 from aiida_gromacs import helpers
 from aiida_gromacs.utils import searchprevious
 
 
 def launch(params):
@@ -34,29 +34,35 @@
     # If code is not initialised, then setup.
     if "code" in inputs:
         inputs["code"] = params.pop("code")
     else:
         computer = helpers.get_computer()
         inputs["code"] = helpers.get_code(entry_point="gromacs", computer=computer)
 
+    # save the full command as a string in the inputs dict
+    inputs = searchprevious.save_command("gmx editconf", params, inputs)
+
+    input_file_labels = {} # dict used for finding previous nodes
+    input_file_labels[params["f"]] = "grofile"
+
     # Prepare input parameters in AiiDA formats.
     SinglefileData = DataFactory("core.singlefile")
     inputs["grofile"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("f")))
 
     if "n" in params:
         inputs["n_file"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("n")))
 
     if "bf" in params:
         inputs["bf_file"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("bf")))
 
     EditconfParameters = DataFactory("gromacs.editconf")
     inputs["parameters"] = EditconfParameters(params)
 
     # check if inputs are outputs from prev processes
-    inputs = searchprevious.get_prev_inputs(inputs, ["grofile"])
+    inputs = searchprevious.link_previous_file_nodes(input_file_labels, inputs)
 
     # check if a pytest test is running, if so run rather than submit aiida job
     # Note: in order to submit your calculation to the aiida daemon, do:
     # pylint: disable=unused-variable
     if "PYTEST_CURRENT_TEST" in os.environ:
         future = engine.run(CalculationFactory("gromacs.editconf"), **inputs)
     else:
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/cli/genericMD.py` & `aiida_gromacs-2.0.8/aiida_gromacs/cli/genericMD.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,17 @@
 from aiida.common import exceptions
 from aiida.plugins import CalculationFactory
 
 from aiida_gromacs import helpers
 from aiida_gromacs.utils import searchprevious
 
 # set base path for input files.
-INPUT_DIR = os.path.join(os.getcwd())
-profile = load_profile()
+INPUT_DIR = os.getcwd()
+profile = load_profile() # need to load profile first
 computer = helpers.get_computer()
-# code = helpers.get_code(entry_point="gromacs", computer=computer)
-# code = helpers.get_code(entry_point="bash", computer=computer)
 
 
 def launch_genericMD(options):
     """Run genericMD"""
 
     code = options["code"]
     command = options["command"]
@@ -34,50 +32,37 @@
     outputs = options["outputs"]
     output_dir = options["output_dir"]
     submit = options["submit"]
 
     print(f"command: {command}")
     print(f"code: {code}")
 
-    # Create or load code
-    try:
-        code = orm.load_code(code)
-    except exceptions.NotExistent:
-        # Setting up code via python API (or use "verdi code setup")
-        executable = code.split('@')[0]
-        path = helpers.get_path_to_executable(executable)
-        code = orm.InstalledCode(
-            label=executable, computer=computer, 
-            filepath_executable=path, 
-            default_calc_job_plugin='genericMD'
-        )
+    code = helpers.setup_generic_code(code)
 
     if not code:
         raise exceptions.NonExistent("Code has not been set.")
     Path(output_dir).mkdir(parents=True, exist_ok=True)
 
     # MyAppCalculation = CalculationFactory("gromacs.genericMD")
 
     # Check if a previous calculation with the same input parameter
     # value has been stored by loading the QueryBuilder and append
     # all previous jobs ordered by newest first.
     qb = searchprevious.build_query()
-    # qb.append(MyAppCalculation, tag="calcjob")
-    # qb.order_by({MyAppCalculation: {"ctime": "desc"}})
 
     # Wait for previous process to finish if running
     if submit:
         searchprevious.check_prev_process(qb)
 
     # Save list of input files to a dict with keys that are formatted
     # file names and values that are SinglefileData.
     input_files = {}
     for filename in list(inputs):
         file_path = os.path.join(INPUT_DIR, filename)
-        stripped_input = filename.split("/")[-1]
+        stripped_input = searchprevious.strip_path(filename) #.split("/")[-1]
         input_files[searchprevious.format_link_label(stripped_input)] = \
             orm.SinglefileData(file=file_path)
 
     # Keep the output filenames as a list.
     output_files = list(outputs)
 
     # create input dictionary for calculation.
@@ -86,15 +71,15 @@
         "command": orm.Str(command),
         "input_files": input_files,
         "output_files": orm.List(output_files),
         "metadata": {
             "label": "generic-execute",
             "description": "Run CLI job and save input and output file provenance.",
             "options": {
-                "output_filename": "file.out",
+                "output_filename": f"{searchprevious.format_link_label(command.split()[0])}.out",
                 "output_dir": output_dir,
                 "parser_name": "gromacs.genericMD",
             },
         },
     }
 
     # check if previous processes have run and add previous outputs
@@ -106,18 +91,18 @@
     # check if a pytest test is running, if so run rather than submit aiida job
     # Submit your calculation to the aiida daemon
     # pylint: disable=unused-variable
     if "PYTEST_CURRENT_TEST" in os.environ:
         future = engine.run(CalculationFactory("gromacs.genericMD"), 
                                **process_inputs)
     else:
-        if submit:
+        if submit: # submit to deamon and release interpretor
             future = engine.submit(CalculationFactory("gromacs.genericMD"), 
                                 **process_inputs)
-        else:
+        else: # blocking mode
             future = engine.run(CalculationFactory("gromacs.genericMD"), 
                                 **process_inputs)
 
     # future = engine.submit(process)
     print(f"Submitted calculation: {future}\n")
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/cli/genion.py` & `aiida_gromacs-2.0.8/aiida_gromacs/cli/genion.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Usage: gmx_genion --help
 """
 
 import os
 
 import click
 
-from aiida import cmdline, engine
+from aiida import cmdline, engine, orm
 from aiida.plugins import CalculationFactory, DataFactory
 
 from aiida_gromacs import helpers
 from aiida_gromacs.utils import searchprevious
 
 
 def launch(params):
@@ -24,39 +24,53 @@
     # Prune unused CLI parameters from dict.
     params = {k:v for k,v in params.items() if v != None}
 
     # dict to hold our calculation data.
     inputs = {
         "metadata": {
             "description": params.pop("description"),
+            "options": {},
         },
     }
 
     # If code is not initialised, then setup.
     if "code" in inputs:
         inputs["code"] = params.pop("code")
     else:
         computer = helpers.get_computer()
         inputs["code"] = helpers.get_code(entry_point="gromacs", computer=computer)
+        # inputs["code"] = helpers.get_code(entry_point="bash", computer=computer)
+
+    # save the full command as a string in the inputs dict
+    inputs = searchprevious.save_command("gmx genion", params, inputs)
+
+    input_file_labels = {} # dict used for finding previous nodes
+    input_file_labels[params["s"]] = "tprfile"
+    input_file_labels[params["p"]] = "topfile"
+    SinglefileData = DataFactory("core.singlefile")
+    if "instructions" in params:
+        inputs["metadata"]["options"]["stdin_filename"] = str(params["instructions"])
+        inputs["instructions_file"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("instructions")))
+    else:
+        # if no instructions given, then default to hard coded genion input
         inputs["code"] = helpers.get_code(entry_point="bash", computer=computer)
 
 
     # Prepare input parameters in AiiDA formats.
-    SinglefileData = DataFactory("core.singlefile")
     inputs["tprfile"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("s")))
     inputs["topfile"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("p")))
 
     if "n" in params:
         inputs["n_file"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("n")))
 
     GenionParameters = DataFactory("gromacs.genion")
     inputs["parameters"] = GenionParameters(params)
 
     # check if inputs are outputs from prev processes
-    inputs = searchprevious.get_prev_inputs(inputs, ["tprfile", "topfile"])
+    inputs = searchprevious.link_previous_file_nodes(input_file_labels, inputs)
 
 
     # check if a pytest test is running, if so run rather than submit aiida job
     # Note: in order to submit your calculation to the aiida daemon, do:
     # pylint: disable=unused-variable
     if "PYTEST_CURRENT_TEST" in os.environ:
         future = engine.run(CalculationFactory("gromacs.genion"), **inputs)
@@ -69,14 +83,15 @@
 @cmdline.params.options.CODE()
 # Plugin options
 @click.option("--description", default="record genion data provenance via the aiida_gromacs plugin", type=str, help="Short metadata description")
 # Input file options
 @click.option("-s", default="topol.tpr", type=str, help="Input structure file")
 @click.option("-n", type=str, help="Index file")
 @click.option("-p", default="topol.top", type=str, help="Topology file")
+@click.option("--instructions", type=str, help="aiida-gromacs specific option: File containing interactive instructions for genion command, each instruction should be on a new line in the file.")
 # Output file options
 @click.option("-o", default="out.gro", type=str, help="Output structure file")
 # Other parameter options
 @click.option("-np", type=str, help="Number of positive ions")
 @click.option("-pname", default="NA", type=str, help="Name of positive ion")
 @click.option("-pq", type=str, help="Charge of the positive ion")
 @click.option("-nn", type=str, help="Number of negative ions")
@@ -91,20 +106,20 @@
 def cli(*args, **kwargs):
     # pylint: disable=unused-argument
     # pylint: disable=line-too-long
     """Run example.
 
     Example usage:
 
-    $ gmx_genion --code gmx@localhost -s 1AKI_ions.tpr -p 1AKI_topology.top -pname NA -nname CL -neutral true -o 1AKI_solvated_ions.gro
+    $ gmx_genion --code gmx@localhost -s 1AKI_ions.tpr -p 1AKI_topology.top -pname NA -nname CL -neutral true -o 1AKI_solvated_ions.gro --instructions instructions.txt
 
     Alternative (automatically tried to create gmx@localhost code, but requires
     gromacs to be installed and available in your environment path):
 
-    $ gmx_genion -s 1AKI_ions.tpr -p 1AKI_topology.top -pname NA -nname CL -neutral true -o 1AKI_solvated_ions.gro
+    $ gmx_genion -s 1AKI_ions.tpr -p 1AKI_topology.top -pname NA -nname CL -neutral true -o 1AKI_solvated_ions.gro --instructions instuctions.txt
 
     Help: $ gmx_genion --help
     """
 
     launch(kwargs)
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/cli/grompp.py` & `aiida_gromacs-2.0.8/aiida_gromacs/cli/grompp.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 
 Usage: gmx_grompp --help
 """
 
 import click
 import os
 
-from aiida import cmdline, engine
+from aiida import cmdline, engine, orm
 from aiida.plugins import CalculationFactory, DataFactory
 
 from aiida_gromacs import helpers
-from aiida_gromacs.utils import searchprevious
-from aiida_gromacs.utils import topfile_utils
+from aiida_gromacs.utils import searchprevious, topfile_utils
 
 
 def launch(params):
     """Run grompp.
 
     Uses helpers to add gromacs on localhost to AiiDA on the fly.
     """
@@ -34,14 +33,22 @@
     # If code is not initialised, then setup.
     if "code" in inputs:
         inputs["code"] = params.pop("code")
     else:
         computer = helpers.get_computer()
         inputs["code"] = helpers.get_code(entry_point="gromacs", computer=computer)
 
+    # save the full command as a string in the inputs dict
+    inputs = searchprevious.save_command("gmx grompp", params, inputs)
+
+    input_file_labels = {} # dict used for finding previous nodes
+    input_file_labels[params["f"]] = "mdpfile"
+    input_file_labels[params["c"]] = "grofile"
+    input_file_labels[params["p"]] = "topfile"
+
     # Prepare input parameters in AiiDA formats.
     SinglefileData = DataFactory("core.singlefile")
     FolderData = DataFactory("core.folder")
     inputs["mdpfile"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("f")))
     inputs["grofile"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("c")))
     inputs["topfile"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("p")))
 
@@ -101,15 +108,15 @@
     if "ref" in params:
         inputs["ref_file"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("ref")))
 
     GromppParameters = DataFactory("gromacs.grompp")
     inputs["parameters"] = GromppParameters(params)
 
     # check if inputs are outputs from prev processes
-    inputs = searchprevious.get_prev_inputs(inputs, ["grofile", "topfile", "mdpfile"])
+    inputs = searchprevious.link_previous_file_nodes(input_file_labels, inputs)
 
     # check if a pytest test is running, if so run rather than submit aiida job
     # Note: in order to submit your calculation to the aiida daemon, do:
     # pylint: disable=unused-variable
     if "PYTEST_CURRENT_TEST" in os.environ:
         future = engine.run(CalculationFactory("gromacs.grompp"), **inputs)
     else:
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/cli/make_ndx.py` & `aiida_gromacs-2.0.8/aiida_gromacs/cli/make_ndx.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Usage: gmx_make_ndx --help
 """
 
 import os
 
 import click
 
-from aiida import cmdline, engine
+from aiida import cmdline, engine, orm
 from aiida.plugins import CalculationFactory, DataFactory
 
 from aiida_gromacs import helpers
 from aiida_gromacs.utils import searchprevious
 
 
 def launch(params):
@@ -35,30 +35,35 @@
     # If code is not initialised, then setup.
     if "code" in inputs:
         inputs["code"] = params.pop("code")
     else:
         computer = helpers.get_computer()
         inputs["code"] = helpers.get_code(entry_point="gromacs", computer=computer)
 
+    # save the full command as a string in the inputs dict
+    inputs = searchprevious.save_command("gmx make_ndx", params, inputs)
+
     # Prepare input parameters in AiiDA formats.
     SinglefileData = DataFactory("core.singlefile")
 
+    input_file_labels = {} # dict used for finding previous nodes
     if "f" in params:
+        input_file_labels[params["f"]] = "grofile"
         inputs["grofile"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("f")))
     if "n" in params:
         inputs["n_file"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("n")))
     if "instructions" in params:
         inputs["metadata"]["options"]["stdin_filename"] = str(params["instructions"])
         inputs["instructions_file"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("instructions")))
 
     Make_ndxParameters = DataFactory("gromacs.make_ndx")
     inputs["parameters"] = Make_ndxParameters(params)
 
-    # check if inputs are outputs from prev processes
-    inputs = searchprevious.get_prev_inputs(inputs, ["grofile", "n_file"])
+    # check if inputs are outputs from prev gmx_* processes
+    inputs = searchprevious.link_previous_file_nodes(input_file_labels, inputs)
 
     # check if a pytest test is running, if so run rather than submit aiida job
     # Note: in order to submit your calculation to the aiida daemon, do:
     # pylint: disable=unused-variable
     if "PYTEST_CURRENT_TEST" in os.environ:
         future = engine.run(CalculationFactory("gromacs.make_ndx"), **inputs)
     else:
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/cli/mdrun.py` & `aiida_gromacs-2.0.8/aiida_gromacs/cli/mdrun.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Usage: gmx_mdrun --help
 """
 
 import os
 
 import click
 
-from aiida import cmdline, engine
+from aiida import cmdline, engine, orm
 from aiida.plugins import CalculationFactory, DataFactory
 
 from aiida_gromacs import helpers
 from aiida_gromacs.utils import searchprevious
 
 
 def launch(params):
@@ -34,14 +34,20 @@
     # If code is not initialised, then setup.
     if "code" in inputs:
         inputs["code"] = params.pop("code")
     else:
         computer = helpers.get_computer()
         inputs["code"] = helpers.get_code(entry_point="gromacs", computer=computer)
 
+    # save the full command as a string in the inputs dict
+    inputs = searchprevious.save_command("gmx mdrun", params, inputs)
+
+    input_file_labels = {} # dict used for finding previous nodes
+    input_file_labels[params["s"]] = "tprfile"
+
     # Prepare input parameters in AiiDA formats.
     SinglefileData = DataFactory("core.singlefile")
     inputs["tprfile"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("s")))
 
     if "cpi" in params:
         inputs["cpi_file"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("cpi")))
 
@@ -75,15 +81,15 @@
     if "mn" in params:
         inputs["mn_file"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("mn")))
 
     MdrunParameters = DataFactory("gromacs.mdrun")
     inputs["parameters"] = MdrunParameters(params)
 
     # check if inputs are outputs from prev processes
-    inputs = searchprevious.get_prev_inputs(inputs, ["tprfile"])
+    inputs = searchprevious.link_previous_file_nodes(input_file_labels, inputs)
 
     # check if a pytest test is running, if so run rather than submit aiida job
     # Note: in order to submit your calculation to the aiida daemon, do:
     # pylint: disable=unused-variable
     if "PYTEST_CURRENT_TEST" in os.environ:
         future = engine.run(CalculationFactory("gromacs.mdrun"), **inputs)
     else:
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/cli/pdb2gmx.py` & `aiida_gromacs-2.0.8/aiida_gromacs/cli/pdb2gmx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python
 """CLI utility to run gmx pdb2gmx with AiiDA.
 
 Usage: gmx_pdb2gmx --help
 """
 
 import os
-
+import sys
 import click
 
-from aiida import cmdline, engine
+from aiida import cmdline, engine, orm
 from aiida.plugins import CalculationFactory, DataFactory
 
 from aiida_gromacs import helpers
+from aiida_gromacs.utils import searchprevious
 
 
 def launch(params):
     """Run pdb2gmx.
 
     Uses helpers to add gromacs on localhost to AiiDA on the fly.
     """
@@ -33,21 +34,30 @@
     # If code is not initialised, then setup.
     if "code" in inputs:
         inputs["code"] = params.pop("code")
     else:
         computer = helpers.get_computer()
         inputs["code"] = helpers.get_code(entry_point="gromacs", computer=computer)
 
+    # save the full command as a string in the inputs dict
+    inputs = searchprevious.save_command("gmx pdb2gmx", params, inputs)
+
+    input_file_labels = {} # dict used for finding previous nodes
+    input_file_labels[params["f"]] = "pdbfile"
+
     # Prepare input parameters in AiiDA formats.
     SinglefileData = DataFactory("core.singlefile")
     inputs["pdbfile"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("f")))
 
     Pdb2gmxParameters = DataFactory("gromacs.pdb2gmx")
     inputs["parameters"] = Pdb2gmxParameters(params)
 
+    # check if inputs are outputs from prev processes
+    inputs = searchprevious.link_previous_file_nodes(input_file_labels, inputs)
+
     # check if a pytest test is running, if so run rather than submit aiida job
     # Note: in order to submit your calculation to the aiida daemon, do:
     # pylint: disable=unused-variable
     if "PYTEST_CURRENT_TEST" in os.environ:
         future = engine.run(CalculationFactory("gromacs.pdb2gmx"), **inputs)
     else:
         future = engine.submit(CalculationFactory("gromacs.pdb2gmx"), **inputs)
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/cli/solvate.py` & `aiida_gromacs-2.0.8/aiida_gromacs/cli/solvate.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Usage: gmx_solvate --help
 """
 
 import os
 
 import click
 
-from aiida import cmdline, engine
+from aiida import cmdline, engine, orm
 from aiida.plugins import CalculationFactory, DataFactory
 
 from aiida_gromacs import helpers
 from aiida_gromacs.utils import searchprevious
 
 
 def launch(params):
@@ -34,28 +34,35 @@
     # If code is not initialised, then setup.
     if "code" in inputs:
         inputs["code"] = params.pop("code")
     else:
         computer = helpers.get_computer()
         inputs["code"] = helpers.get_code(entry_point="gromacs", computer=computer)
 
+    # save the full command as a string in the inputs dict
+    inputs = searchprevious.save_command("gmx solvate", params, inputs)
+
+    input_file_labels = {} # dict used for finding previous nodes
+    input_file_labels[params["cp"]] = "grofile"
+    input_file_labels[params["p"]] = "topfile"
+
     # Prepare input parameters in AiiDA formats.
     SinglefileData = DataFactory("core.singlefile")
     inputs["grofile"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("cp")))
     inputs["topfile"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("p")))
 
     if "cs" in params:
         if params["cs"] != "spc216.gro": # needs fixing
             inputs["cs_file"] = SinglefileData(file=os.path.join(os.getcwd(), params.pop("cs")))
 
     SolvateParameters = DataFactory("gromacs.solvate")
     inputs["parameters"] = SolvateParameters(params)
 
     # check if inputs are outputs from prev processes
-    inputs = searchprevious.get_prev_inputs(inputs, ["grofile", "topfile"])
+    inputs = searchprevious.link_previous_file_nodes(input_file_labels, inputs)
 
     # check if a pytest test is running, if so run rather than submit aiida job
     # Note: in order to submit your calculation to the aiida daemon, do:
     # pylint: disable=unused-variable
     if "PYTEST_CURRENT_TEST" in os.environ:
         future = engine.run(CalculationFactory("gromacs.solvate"), **inputs)
     else:
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/data/editconf.py` & `aiida_gromacs-2.0.8/aiida_gromacs/data/editconf.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/data/genion.py` & `aiida_gromacs-2.0.8/aiida_gromacs/data/genion.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,29 +69,41 @@
 
         e.g. [ '--ignore-case', 'filename1', 'filename2']
 
         :param pdbfile: Name of input pdb file
         :param type pdbfile: str
 
         """
-        cmdline = "echo"
-        cmdline = cmdline + " " + "SOL"
-        cmdline = cmdline + " " + "| gmx genion"
-        cmdline = cmdline + " " + " -s " + input_files["tprfile"]
-        cmdline = cmdline + " " + " -p " + input_files["topfile"]
-        if "n_file" in input_files: cmdline = cmdline + " " + " -n " + input_files["n_file"]
-
         parameters = []
+        if "instructions_file" in input_files:
+            parameters.append("genion")
+            parameters.extend(["-s", input_files["tprfile"]])
+            parameters.extend(["-p", input_files["topfile"]])
+            if "n_file" in input_files: parameters.extend(["-n", input_files["n_file"]])
+
+            parm_dict = self.get_dict()
+
+            for key, value in parm_dict.items():
+                parameters.extend(["-" + key, value])
+
+        else:
+            # if no instructions given, then default to hard coded genion input
+            cmdline = "echo"
+            cmdline = cmdline + " " + "SOL"
+            cmdline = cmdline + " " + "| gmx genion"
+            cmdline = cmdline + " " + " -s " + input_files["tprfile"]
+            cmdline = cmdline + " " + " -p " + input_files["topfile"]
+            if "n_file" in input_files: cmdline = cmdline + " " + " -n " + input_files["n_file"]
 
-        parm_dict = self.get_dict()
+            parm_dict = self.get_dict()
 
-        for key, value in parm_dict.items():
-            cmdline = cmdline + " -" + key + " " + value
+            for key, value in parm_dict.items():
+                cmdline = cmdline + " -" + key + " " + value
 
-        parameters.extend(["-c", cmdline])
+            parameters.extend(["-c", cmdline])
 
         return [str(p) for p in parameters]
 
     def __str__(self):
         """String representation of node.
 
         Append values of dictionary to usual representation. E.g.::
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/data/grompp.py` & `aiida_gromacs-2.0.8/aiida_gromacs/data/grompp.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/data/make_ndx.py` & `aiida_gromacs-2.0.8/aiida_gromacs/data/make_ndx.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/data/mdrun.py` & `aiida_gromacs-2.0.8/aiida_gromacs/data/mdrun.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/data/pdb2gmx.py` & `aiida_gromacs-2.0.8/aiida_gromacs/data/pdb2gmx.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/data/solvate.py` & `aiida_gromacs-2.0.8/aiida_gromacs/data/solvate.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/helpers.py` & `aiida_gromacs-2.0.8/aiida_gromacs/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 Note: Point 2 is made possible by the fact that the ``diff`` executable is
 available in the PATH on almost any UNIX system.
 """
 import shutil
 import tempfile
 
 from aiida.common.exceptions import NotExistent
-from aiida.orm import InstalledCode, Computer
+from aiida.common import exceptions
+from aiida.orm import InstalledCode, Computer, load_code
 
 LOCALHOST_NAME = "localhost"
 
 executables = {
     "gromacs": "gmx",
     "bash": "bash",
 }
@@ -96,7 +97,27 @@
         label = executable,
         default_calc_job_plugin=entry_point,
         computer=computer,
         filepath_executable=path,
     )
 
     return code.store()
+
+
+def setup_generic_code(code):
+    """Try to set up any code for running a genericMD process
+
+    :param code: executable@computer of the code being run
+    """
+    # Create or load code
+    try:
+        code = load_code(code)
+    except exceptions.NotExistent:
+        # Setting up code via python API (or use "verdi code setup")
+        executable = code.split('@')[0]
+        path = get_path_to_executable(executable)
+        code = InstalledCode(
+            label=executable, computer= get_computer(), 
+            filepath_executable=path, 
+            default_calc_job_plugin='genericMD'
+        )
+    return code
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/parsers/editconf.py` & `aiida_gromacs-2.0.8/aiida_gromacs/parsers/editconf.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/parsers/genericMD.py` & `aiida_gromacs-2.0.8/aiida_gromacs/parsers/genericMD.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,17 +72,14 @@
                 return self.exit_codes.ERROR_UNTRACKED_OUTPUT_FILES
 
         # passing along the std output file as a SinglefileData node.
         self.logger.info(f"Parsing '{output_filename}'")
         with self.retrieved.open(output_filename, "rb") as handle:
             output_node = SinglefileData(file=handle)
 
-        # return stdout file 
-        self.out("log", output_node)
-
         # passing along all expected output file as SinglefileData nodes.
         for thing in files_expected:
             self.logger.info(f"Parsing '{thing}'")
             with self.retrieved.open(thing, "rb") as handle:
                 output_node = SinglefileData(file=handle, filename=thing)
             self.out(self.format_link_label(thing), output_node)
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/parsers/genion.py` & `aiida_gromacs-2.0.8/aiida_gromacs/parsers/genion.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/parsers/grompp.py` & `aiida_gromacs-2.0.8/aiida_gromacs/parsers/grompp.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/parsers/make_ndx.py` & `aiida_gromacs-2.0.8/aiida_gromacs/parsers/make_ndx.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/parsers/mdrun.py` & `aiida_gromacs-2.0.8/aiida_gromacs/parsers/mdrun.py`

 * *Files 17% similar despite different names*

```diff
@@ -73,14 +73,18 @@
 
         # Grab list of retrieved files.
         files_retrieved = self.retrieved.base.repository.list_object_names()
 
         # Grab list of files expected and remove the scheduler stdout and stderr files.
         files_expected = [files for files in self.node.get_option("retrieve_list") if files not in ["_scheduler-stdout.txt", "_scheduler-stderr.txt"]]
 
+        # check if any trajectory file is in files_retrieved
+        files_retrieved, files_expected = MdrunParser.check_trajectory_format(
+                files_retrieved, files_expected)
+
         # Check if the expected files are a subset of retrieved.
         if not set(files_expected) <= set(files_retrieved):
             self.logger.error(
                 f"Found files '{files_retrieved}', expected to find '{files_expected}'"
             )
             return self.exit_codes.ERROR_MISSING_OUTPUT_FILES
 
@@ -130,8 +134,31 @@
         :param metadata_dict: the aiida dictionary containing metadata
         """
         # If not in testing mode, then copy back dict as json file.
         if "PYTEST_CURRENT_TEST" not in os.environ:
             f_prefix = f.split(".")[0]
             file_path = os.path.join(output_dir, f"{f_prefix}_metadata.json")
             with open(file_path, 'w', encoding='utf-8') as f:
-                json.dump(metadata_dict, f, ensure_ascii=False, indent=4)
+                json.dump(metadata_dict, f, ensure_ascii=False, indent=4)
+
+    
+    def check_trajectory_format(files_retrieved: list, files_expected: list):
+        """
+        In the case where nstxout-compressed = >0, gromacs should produce a 
+        xtc file instead of what is requested for -o flag in mdrun. Check 
+        if an unexpected xtc file is produced, if so, add this to 
+        files_expected, and if a file defined from the -o file is not in the 
+        files_retrieved list, then remove it as we have the xtc file instead.
+
+        :param files_retrieved: list of file names returned from calc
+        :param files_expected: list of file names expected to be returned 
+            from calc
+        """
+        for file in files_retrieved:
+            if file.split(".")[-1] == "xtc":
+                if file not in files_expected:
+                    files_expected.append(file)
+                for file2 in files_expected:
+                    if (file2.split(".")[-1] in ["trr", "cpt", "tng"] and 
+                            file2 not in files_retrieved):
+                        files_expected.remove(file2)
+        return files_retrieved, files_expected
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/parsers/pdb2gmx.py` & `aiida_gromacs-2.0.8/aiida_gromacs/parsers/pdb2gmx.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/parsers/solvate.py` & `aiida_gromacs-2.0.8/aiida_gromacs/parsers/solvate.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/utils/fileparsers.py` & `aiida_gromacs-2.0.8/aiida_gromacs/utils/fileparsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,20 +184,21 @@
                             if len(numbers) == len(header):
                                 for hn in range(len(header)):
                                     averages[header[hn].strip()] = numbers[hn]
             if "Time:" in line:
                 averages["Time"] = {}
                 l = line.strip().split()[1:]
                 head = list(filter(None, lines[i-1].strip().split("  ")))
-                for hn in range(len(header)):
+                for hn in range(len(head)):
                     averages["Time"][head[hn]] = l[hn]
             if "Performance:" in line:
                 averages["Performance"] = {}
                 l = line.strip().split()[1:]
-                head = list(filter(None, lines[i-1].strip().split("  ")))
-                for hn in range(len(header)):
+                # head = list(filter(None, lines[i-1].strip().split("  ")))
+                head = list(filter(None, re.split(r'\s{2,}', lines[i-1].strip())))
+                for hn in range(len(head)):
                     averages["Performance"][head[hn]] = l[hn]
                         
     averages = {"Summary": averages}
     # merge dicts
     all_dict = input_params | averages
     return all_dict
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/utils/inspectdb.py` & `aiida_gromacs-2.0.8/aiida_gromacs/utils/inspectdb.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/utils/querydb.py` & `aiida_gromacs-2.0.8/aiida_gromacs/utils/querydb.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/utils/searchprevious.py` & `aiida_gromacs-2.0.8/aiida_gromacs/utils/searchprevious.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,52 +25,36 @@
     """
     alphanumeric = re.sub("[^0-9a-zA-Z_]+", "_", filename)
     link_label = re.sub("_[_]+", "_", alphanumeric)
 
     return link_label
 
 
+def strip_path(input: str) -> str:
+    """For a given input, strip the path from the filename
+
+    :param input: path+filename of an input used for an aiida-gromacs input
+    """
+    return input.split("/")[-1]
+
+
 def build_query():
     """
-    Uses AiiDA querybuilder to find previously run processes
+    Uses AiiDA querybuilder to find previously run processes and order from
+    newest to oldest
 
     :returns: the query entries
     :rtype: :py:class:`aiida.orm.querybuilder.QueryBuilder`
     """
     qb = orm.QueryBuilder()
     qb.append(orm.ProcessNode, tag='process')
     qb.order_by({orm.ProcessNode: {"ctime": "desc"}})
     return qb
 
 
-def get_prev_inputs(inputs, input_labels):
-    """Checks if input labels are output labels in previous processes
-    and if so, adds most recent previous nodes to the new process inputs
-
-    :param inputs: all inputs for the current process
-    :type inputs: dict
-    :param input_labels: input labels of the current process to search for in
-        previous processes.
-    :returns: updated inputs with links to previous nodes if applicable
-    :rtype: dict
-    """
-    qb = build_query()
-    added_files = []
-    if qb.count() > 0:
-        for entry in qb.all():
-            previous_calculation = entry[0]
-            for label in previous_calculation.outputs:
-                if label in input_labels and label not in added_files:
-                    added_files.append(label)
-                    previous_output_node = \
-                        previous_calculation.outputs[f"{label}"]
-                    inputs[label] = previous_output_node
-    return inputs
-
-
 def check_prev_process(qb):
     """Wait for a previous process to finish if it is still running. The
     process state is checked every 10 seconds for up to 5 minutes and stops 
     when the process state is set to finished. If a previous processes takes 
     longer than 5 minutes, the latest submitted process is exited.
 
     :param qb: The queries of previous processes in the AiiDA database
@@ -88,15 +72,36 @@
                 time.sleep(10)
                 if time.time() > timeout:
                     sys.exit("Wait time exceeded for previous "
                              "process to complete")
         else:
             sys.exit("Previous process did not complete successfully, "
                      "please check")
+            
 
+def find_previous_file_nodes(qb):
+    """
+    For any previous processes, store nodes that are files into a list
+
+    :param qb: The queries of previous processes in the AiiDA database
+    :type qb: :py:class:`aiida.orm.querybuilder.QueryBuilder`
+    """
+    file_nodes = []
+    if qb.count() > 0:
+        for entry in qb.all():
+            # A previous calculation exists - use its output as input for the
+            # current calculation.
+            previous_calculation = entry[0]
+            for label in previous_calculation.outputs:
+                # Get the outputs from a previous process.
+                previous_output_node = previous_calculation.outputs[f"{label}"]
+                # check if the output node is a file.
+                if isinstance(previous_output_node, orm.SinglefileData):
+                    file_nodes.append(previous_output_node)
+    return file_nodes
 
 
 def append_prev_nodes(qb, inputs, process_inputs, INPUT_DIR):
     """Checks if previous processes exists for genericMD calcs and links the 
     most recent SinglefileData type output nodes from previous processs as 
     inputs to the new process if the file names match.
 
@@ -106,59 +111,85 @@
     :type inputs: list
     :param process_inputs: All inputs for the current process to be submitted
     :type process_inputs: dict
     :param INPUT_DIR: base directory where outputted files are stored.
     :returns: Updated inputs for the current process
     :rtype: dict
     """
-
-    # if previous processes exist then check if input files are stored as
-    # previous nodes and use these nodes as inputs for new process.
-    if qb.count() > 0:
-        # get just the name of the file from the filepath.
+    file_nodes = find_previous_file_nodes(qb)
+    if file_nodes:
         stripped_inputs = []
-        for inp in inputs:  # strip input file names of any paths.
-            stripped_inputs.append(inp.split("/")[-1])
-
-        prev = {}
         prev_files = []  # list of previous files already saved.
-        wait_for = []
-        for entry in qb.all():
-            # A previous calculation exists - use its output as input for the
-            # current calculation.
-            previous_calculation = entry[0]
-            wait_for.append(previous_calculation)
-            for label in previous_calculation.outputs:
-                # Get the outputs from a previous process.
-                previous_output_node = previous_calculation.outputs[f"{label}"]
-                # (below 2 lines does the same as above)
-                # previous_output_node = orm.load_node(
-                #         previous_calculation.outputs[f"{label}"].pk)
-
-                # check if the output node is a file.
-                if isinstance(previous_output_node, orm.SinglefileData):
-                    prev_output_filename = previous_output_node.base.attributes.get(
-                        "filename"
-                    ) # get filename of the node
-                    # check if output file is an input for new process and
-                    # hasn't already been included as an input.
-                    if (
-                        prev_output_filename in stripped_inputs
-                        and prev_output_filename not in prev_files
-                    ):
-                        prev_files.append(prev_output_filename)
-                        prev[
-                            format_link_label(prev_output_filename)
-                        ] = previous_output_node
+        prev = {} # dict for genericMD inputs
+        for inp in inputs:  # strip input file names of any paths.
+            stripped_inputs.append(strip_path(inp))
+        for prev_file_node in file_nodes:
+            prev_output_filename = prev_file_node.base.attributes.get(
+                            "filename") # get filename of the node
+            # check if output file is an input for new process and
+            # hasn't already been included as an input.
+            if (
+                prev_output_filename in stripped_inputs
+                and prev_output_filename not in prev_files
+            ):
+                prev_files.append(prev_output_filename)
+                prev[
+                    format_link_label(prev_output_filename)
+                ] = prev_file_node
 
         # save input files not found in previous nodes too.
         for filename in list(inputs):
-            stripped_input = filename.split("/")[-1]
+            stripped_input = strip_path(filename)
             if stripped_input not in prev_files:
                 prev[format_link_label(stripped_input)] = orm.SinglefileData(
                     file=os.path.join(INPUT_DIR, filename)
                 )
 
         # update the calculation inputs dict with new dictionary of
         # input files including nodes from previous processes.
         process_inputs["input_files"] = prev
     return process_inputs
+
+
+def link_previous_file_nodes(input_file_labels: dict, inputs: dict):
+    """
+    For an incoming process, check if an input file is an output of a previous
+    process. If this is the case, then rename the node with the new label
+
+    :param input_file_labels: dictionary with keys of filenames and values the
+        label for the node
+    :param inputs: dictionary used for all inputs for 
+    """
+    qb = build_query()
+    # if previous processes exist then check if input files are stored as
+    # previous nodes and use these nodes as inputs for new process.
+    file_nodes = find_previous_file_nodes(qb)
+    prev_files = []  # list of previous files already saved.
+    if file_nodes:
+        for prev_file_node in file_nodes:
+            prev_output_filename = prev_file_node.base.attributes.get(
+                            "filename") # get filename of the node
+            # save previous file nodes if the filenames match with current process
+            # input files
+            if (prev_output_filename in input_file_labels.keys() and 
+                    prev_output_filename not in prev_files):
+                prev_files.append(prev_output_filename)
+                label = input_file_labels[prev_output_filename]
+                inputs[label] = prev_file_node
+    return inputs
+
+
+
+def save_command(executable: str, params: dict, inputs: dict):
+    """
+    For a given cli command run via aiida-gromacs, save this as a string 
+    and use this as an attribute for the given process
+    """
+
+    # save the full command as a string in the inputs dict
+    str_params = ""
+    for k, v in params.items():
+        v_stripped = strip_path(v)
+        str_params += f"-{k} {v_stripped} "
+    command = f"{executable} {str_params}"
+    inputs["command"] = orm.Str(command)
+    return inputs
```

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/utils/topfile_utils.py` & `aiida_gromacs-2.0.8/aiida_gromacs/utils/topfile_utils.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/aiida_gromacs/workflows/simsetup.py` & `aiida_gromacs-2.0.8/aiida_gromacs/workflows/simsetup.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/conftest.py` & `aiida_gromacs-2.0.8/conftest.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/docs/Makefile` & `aiida_gromacs-2.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/docs/source/conf.py` & `aiida_gromacs-2.0.8/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 import aiida_gromacs
 
 # -- AiiDA-related setup --------------------------------------------------
 
 # If we are not on READTHEDOCS load the Sphinx theme manually
 if not os.environ.get("READTHEDOCS", None):
-    import sphinx_rtd_theme
+    # import sphinx_rtd_theme
 
-    html_theme = "sphinx_rtd_theme"
-    html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
+    html_theme = "furo"  # "sphinx_rtd_theme"
+    # html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 
 # -- General configuration ------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 
@@ -135,18 +135,19 @@
 # a list of builtin themes.
 # ~ html_theme = 'basicstrap'
 ## SET BELOW
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-html_theme_options = {
-    "display_version": True,
-}
+# html_theme_options = {
+#     "display_version": True,
+# }
 
+html_theme = "furo"
 # Add any paths that contain custom themes here, relative to this directory.
 # ~ html_theme_path = ["."]
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
```

### Comparing `aiida_gromacs-2.0.7/docs/source/developer_guide/index.rst` & `aiida_gromacs-2.0.8/docs/source/developer_guide/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 Clone the repository
 ++++++++++++++++++++
 
 The first step in getting going as a developer is to clone our git repository by either
 
 #. HTTPS::
 
-        git clone https://github.com/PSDI-Biomolecular-team/aiida-gromacs.git
+        git clone https://github.com/PSDI-UK/aiida-gromacs.git
 
 #. SSH::
 
-        git clone git@github.com:PSDI-Biomolecular-team/aiida-gromacs.git
+        git clone git@github.com:PSDI-UK/aiida-gromacs.git
 
 Running the tests
 +++++++++++++++++
 
 To run our test suite, in addition to having AiiDA installed, you should also have the daemon running, which will include the full AiiDA startup steps for the database and an initial user profile to be setup.
 
 The following will discover and run all unit test::
@@ -50,17 +50,17 @@
 
 
 Continuous integration
 ++++++++++++++++++++++
 
 ``aiida-gromacs`` comes with a ``.github`` folder that contains continuous integration tests on every commit using `GitHub Actions <https://github.com/features/actions>`_. It will:
 
-#. run all tests
-#. build the documentation
-#. check coding style and version number (not required to pass by default)
+#. run all tests including against several package dependencies and their versions.
+#. build the documentation.
+#. check coding style and version number (not required to pass by default).
 
 We have these activated on github via the github actions platform. When version numbers are tagged, we will also automatically push a version to pypi.
 
 Building the documentation
 ++++++++++++++++++++++++++
 
  #. Install the ``docs`` extra::
@@ -81,15 +81,15 @@
 Check the result by opening ``build/html/index.html`` in your browser.
 
 Putting it all together
 +++++++++++++++++++++++
 
 Putting all of the above together into the following install commands::
 
-        git clone git@github.com:PSDI-Biomolecular-team/aiida-gromacs.git
+        git clone git@github.com:PSDI-UK/aiida-gromacs.git
         cd aiida-gromacs
         pip install -e .[docs,pre-commit,testing]
         pre-commit install
 
 Will install the plugin from the git repository with all of the above features activated.
 
 Sending code contributions
@@ -98,12 +98,14 @@
 We will always welcome code contributions for new features, but these should always be via the submission of a pull request. Upon receiving a PR, the CI workflow will automatically run our test suite, buld the docs and run the pre-commit checks. One of the core developers will review the code submitted and make a decision based upon the fit of the PR with the project goals and make an assessment of the quality of the contribution.
 
 We would always recommend reporting problems/bugs via the issue tracker even if you intend to attempt a fix, likewise we would recommend contacting a member of the core team if developing features of your own so they can advise on the direction of the project.
 
 Version Numbering
 +++++++++++++++++
 
-We will align our version numbering against the AiiDA major series that the plugin release supports. So our first release will be 2.0.0, where the x in x.y.z corresponds to the AiiDA major series that the plugin is supporting. So 2.0.0 will support AiiDA 2.x.x. The remaining two numbers in our versioning will represent major and minor changes to the plugin respectively. A minor release can be expected to be version compatible with no breaking changes, whilst a major release will be expected to cause changes that are breaking in nature.
+We will align our version numbering against the AiiDA major series that the plugin release supports. So our first release will be v2.0.0, where the X in vX.Y.Z corresponds to the AiiDA major series that the plugin is supporting. So v2.0.0 will support AiiDA 2.x.x. The remaining two numbers in our versioning will represent major and minor changes to the plugin respectively. A minor release can be expected to be version compatible with no breaking changes, whilst a major release will be expected to cause changes that are breaking in nature.
+
+To make and release a new version, the procedure is triggered by pushing a new tag onto the master branch. This should be done after all relevant PRs for a particular release have been reviewed and merged to master and all the CI tests have completed and passed. You should make sure the tag contains the following format vX.Y.Z, the "v" is important for CI automation. Upon pushing a new tag, actions will be triggered to auto make a github release with a full changelog, tests will run against the tag and then a new version will be sent to PYPI for users to download.
 
 Happy coding!
 
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
```

### Comparing `aiida_gromacs-2.0.7/docs/source/images/53.dot.png` & `aiida_gromacs-2.0.8/docs/source/images/53.dot.png`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/docs/source/images/AiiDA_transparent_logo.png` & `aiida_gromacs-2.0.8/docs/source/images/AiiDA_transparent_logo.png`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/docs/source/index.rst` & `aiida_gromacs-2.0.8/docs/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. figure:: images/AiiDA_transparent_logo.png
     :width: 250px
     :align: center
 
 The aiida-gromacs plugin for `AiiDA`_
 =====================================================
 
-``aiida-gromacs`` is available at http://github.com/PSDI-Biomolecular-team/aiida-gromacs
+``aiida-gromacs`` is available at http://github.com/PSDI-UK/aiida-gromacs
 
 
 .. toctree::
    :maxdepth: 2
 
    user_guide/index
    tutorials/index
```

### Comparing `aiida_gromacs-2.0.7/docs/source/tutorials/genericMD.rst` & `aiida_gromacs-2.0.8/docs/source/tutorials/genericMD.rst`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/docs/source/tutorials/lysozyme.rst` & `aiida_gromacs-2.0.8/docs/source/tutorials/lysozyme.rst`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/docs/source/user_guide/aiida_cheatsheet.rst` & `aiida_gromacs-2.0.8/docs/source/user_guide/aiida_cheatsheet.rst`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/docs/source/user_guide/aiida_sessions.rst` & `aiida_gromacs-2.0.8/docs/source/user_guide/aiida_sessions.rst`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/docs/source/user_guide/api_interface.rst` & `aiida_gromacs-2.0.8/docs/source/user_guide/api_interface.rst`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/docs/source/user_guide/cli_interface.rst` & `aiida_gromacs-2.0.8/docs/source/user_guide/cli_interface.rst`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/docs/source/user_guide/index.rst` & `aiida_gromacs-2.0.8/docs/source/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/docs/source/user_guide/installation.rst` & `aiida_gromacs-2.0.8/docs/source/user_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/examples/gromacs-jobs.sh` & `aiida_gromacs-2.0.8/examples/gromacs-jobs.sh`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/examples/gromacs_files/1AKI_clean.pdb` & `aiida_gromacs-2.0.8/examples/gromacs_files/1AKI_clean.pdb`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/examples/gromacs_files/ions.mdp` & `aiida_gromacs-2.0.8/examples/gromacs_files/ions.mdp`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/examples/gromacs_files/min.mdp` & `aiida_gromacs-2.0.8/examples/gromacs_files/min.mdp`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/examples/gromacs_files/npt.mdp` & `aiida_gromacs-2.0.8/examples/gromacs_files/npt.mdp`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/examples/gromacs_files/nvt.mdp` & `aiida_gromacs-2.0.8/examples/gromacs_files/nvt.mdp`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/examples/gromacs_files/prod.mdp` & `aiida_gromacs-2.0.8/examples/gromacs_files/prod.mdp`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/notebooks/lysozyme_tutorial.ipynb` & `aiida_gromacs-2.0.8/notebooks/lysozyme_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/pyproject.toml` & `aiida_gromacs-2.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
     "Natural Language :: English",
     "Development Status :: 5 - Production/Stable",
     "Framework :: AiiDA"
 ]
 keywords = ["aiida", "plugin", "gromacs", "aiida-gromacs"]
 requires-python = ">=3.8"
 dependencies = [
-    "aiida-core>=2.0,<3",
+    "aiida-core>=2.4.0,<3",
     "voluptuous"
 ]
 
 [project.urls]
-Source = "https://github.com/PSDI-Biomolecular-team/aiida-gromacs"
+Source = "https://github.com/PSDI-UK/aiida-gromacs"
 
 [project.optional-dependencies]
 testing = [
     "pgtest~=1.3",
     "wheel~=0.40",
     "coverage[toml]",
     "pytest~=7.3",
@@ -91,14 +91,17 @@
 "gromacs.solvate" = "aiida_gromacs.parsers.solvate:SolvateParser"
 "gromacs.make_ndx" = "aiida_gromacs.parsers.make_ndx:Make_ndxParser"
 "gromacs.genericMD" = "aiida_gromacs.parsers.genericMD:GenericParser"
 
 [project.entry-points."aiida.workflows"]
 "gromacs.setup" = "aiida_gromacs.workflows.simsetup:SetupWorkChain"
 
+[project.entry-points."aiida.cmdline.data"]
+"provenance" = "aiida_gromacs.commands.provenance:provenance"
+
 [tool.flit.module]
 name = "aiida_gromacs"
 
 [tool.pylint.format]
 max-line-length = 125
 
 [tool.pylint.messages_control]
```

### Comparing `aiida_gromacs-2.0.7/tests/input_files/1AKI_restraints.itp` & `aiida_gromacs-2.0.8/tests/input_files/1AKI_restraints.itp`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/editconf_1AKI_forcefield.gro` & `aiida_gromacs-2.0.8/tests/input_files/editconf_1AKI_forcefield.gro`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/genion_1AKI_ions.tpr` & `aiida_gromacs-2.0.8/tests/input_files/genion_1AKI_ions.tpr`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/genion_1AKI_topology.top` & `aiida_gromacs-2.0.8/tests/input_files/genion_1AKI_topology.top`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/grompp2_1AKI_solvated_ions.gro` & `aiida_gromacs-2.0.8/tests/input_files/grompp2_1AKI_solvated_ions.gro`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/grompp2_1AKI_topology.top` & `aiida_gromacs-2.0.8/tests/input_files/grompp2_1AKI_topology.top`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/grompp2_min.mdp` & `aiida_gromacs-2.0.8/tests/input_files/grompp2_min.mdp`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/grompp3_1AKI_minimised.gro` & `aiida_gromacs-2.0.8/tests/input_files/grompp3_1AKI_minimised.gro`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/grompp3_nvt.mdp` & `aiida_gromacs-2.0.8/tests/input_files/grompp3_nvt.mdp`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/grompp_1AKI_solvated.gro` & `aiida_gromacs-2.0.8/tests/input_files/grompp_1AKI_solvated.gro`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/grompp_1AKI_topology.top` & `aiida_gromacs-2.0.8/tests/input_files/grompp_1AKI_topology.top`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/grompp_ions.mdp` & `aiida_gromacs-2.0.8/tests/input_files/grompp_ions.mdp`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/make_ndx_index.ndx` & `aiida_gromacs-2.0.8/tests/input_files/make_ndx_index.ndx`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/mdrun_1AKI_em.tpr` & `aiida_gromacs-2.0.8/tests/input_files/mdrun_1AKI_em.tpr`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/pdb2gmx_1AKI_clean.pdb` & `aiida_gromacs-2.0.8/tests/input_files/pdb2gmx_1AKI_clean.pdb`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/solvate_1AKI_newbox.gro` & `aiida_gromacs-2.0.8/tests/input_files/solvate_1AKI_newbox.gro`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/input_files/solvate_1AKI_topology.top` & `aiida_gromacs-2.0.8/tests/input_files/solvate_1AKI_topology.top`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_calcs_editconf.py` & `aiida_gromacs-2.0.8/tests/test_calcs_editconf.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_calcs_genericMD.py` & `aiida_gromacs-2.0.8/tests/test_calcs_genericMD.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_calcs_genion.py` & `aiida_gromacs-2.0.8/tests/test_calcs_genion.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_calcs_grompp.py` & `aiida_gromacs-2.0.8/tests/test_calcs_grompp.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_calcs_make_gmx.py` & `aiida_gromacs-2.0.8/tests/test_calcs_make_gmx.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_calcs_mdrun.py` & `aiida_gromacs-2.0.8/tests/test_calcs_mdrun.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_calcs_pdb2gmx.py` & `aiida_gromacs-2.0.8/tests/test_calcs_pdb2gmx.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_calcs_solvate.py` & `aiida_gromacs-2.0.8/tests/test_calcs_solvate.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_cli_editconf.py` & `aiida_gromacs-2.0.8/tests/test_cli_editconf.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_cli_genericMD.py` & `aiida_gromacs-2.0.8/tests/test_cli_genericMD.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_cli_genion.py` & `aiida_gromacs-2.0.8/tests/test_cli_genion.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_cli_grompp.py` & `aiida_gromacs-2.0.8/tests/test_cli_grompp.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_cli_make_ndx.py` & `aiida_gromacs-2.0.8/tests/test_cli_make_ndx.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_cli_mdrun.py` & `aiida_gromacs-2.0.8/tests/test_cli_mdrun.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_cli_pdb2gmx.py` & `aiida_gromacs-2.0.8/tests/test_cli_pdb2gmx.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_cli_solvate.py` & `aiida_gromacs-2.0.8/tests/test_cli_solvate.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/tests/test_utils_searchprevious.py` & `aiida_gromacs-2.0.8/tests/test_utils_searchprevious.py`

 * *Files identical despite different names*

### Comparing `aiida_gromacs-2.0.7/PKG-INFO` & `aiida_gromacs-2.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: aiida-gromacs
-Version: 2.0.7
+Version: 2.0.8
 Summary: A plugin for using GROMACS with AiiDA for molecular dymanics simulations.
 Keywords: aiida,plugin,gromacs,aiida-gromacs
 Author-email: James Gebbie-Rayet <james.gebbie@stfc.ac.uk>, Jas Kalayan <jas.kalayan@stfc.ac.uk>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
-Requires-Dist: aiida-core>=2.0,<3
+Requires-Dist: aiida-core>=2.4.0,<3
 Requires-Dist: voluptuous
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx_rtd_theme ; extra == "docs"
 Requires-Dist: sphinxcontrib-contentui ; extra == "docs"
 Requires-Dist: sphinxcontrib-details-directive ; extra == "docs"
 Requires-Dist: furo ; extra == "docs"
 Requires-Dist: markupsafe<2.1 ; extra == "docs"
@@ -24,21 +24,21 @@
 Requires-Dist: pylint~=2.17 ; extra == "pre-commit"
 Requires-Dist: pgtest~=1.3 ; extra == "testing"
 Requires-Dist: wheel~=0.40 ; extra == "testing"
 Requires-Dist: coverage[toml] ; extra == "testing"
 Requires-Dist: pytest~=7.3 ; extra == "testing"
 Requires-Dist: pytest-cov~=4.0 ; extra == "testing"
 Requires-Dist: pytest-sugar~=0.9 ; extra == "testing"
-Project-URL: Source, https://github.com/PSDI-Biomolecular-team/aiida-gromacs
+Project-URL: Source, https://github.com/PSDI-UK/aiida-gromacs
 Provides-Extra: docs
 Provides-Extra: pre-commit
 Provides-Extra: testing
 
-[![Build Status](https://github.com/PSDI-Biomolecular-team/aiida-gromacs/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/PSDI-Biomolecular-team/aiida-gromacs/actions/workflows/ci.yml)
-[![Coverage Status](https://coveralls.io/repos/github/PSDI-Biomolecular-team/aiida-gromacs/badge.svg?branch=master)](https://coveralls.io/github/PSDI-Biomolecular-team/aiida-gromacs?branch=master)
+[![Build Status](https://github.com/PSDI-UK/aiida-gromacs/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/PSDI-UK/aiida-gromacs/actions/workflows/ci.yml)
+[![Coverage Status](https://coveralls.io/repos/github/PSDI-UK/aiida-gromacs/badge.svg?branch=master)](https://coveralls.io/github/PSDI-UK/aiida-gromacs?branch=master)
 [![Docs status](https://readthedocs.org/projects/aiida-gromacs/badge)](http://aiida-gromacs.readthedocs.io/)
 [![PyPI version](https://badge.fury.io/py/aiida-gromacs.svg)](https://badge.fury.io/py/aiida-gromacs)
 
 # aiida-gromacs
 
 The GROMACS plugin for AiiDA aims to enable the capture and sharing of the full
 provenance of data when parameterising and running molecular dynamics
```

