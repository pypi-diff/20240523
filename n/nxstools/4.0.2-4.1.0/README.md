# Comparing `tmp/nxstools-4.0.2.tar.gz` & `tmp/nxstools-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxstools-4.0.2.tar", last modified: Wed May 15 09:37:07 2024, max compression
+gzip compressed data, was "nxstools-4.1.0.tar", last modified: Thu May 23 04:48:28 2024, max compression
```

## Comparing `nxstools-4.0.2.tar` & `nxstools-4.1.0.tar`

### file list

```diff
@@ -1,380 +1,380 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.882289 nxstools-4.0.2/
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.746290 nxstools-4.0.2/.ci/
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.746290 nxstools-4.0.2/.ci/debian10_py2/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3614 2023-01-30 11:59:31.000000 nxstools-4.0.2/.ci/debian10_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.746290 nxstools-4.0.2/.ci/debian10_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3642 2023-01-30 11:59:31.000000 nxstools-4.0.2/.ci/debian10_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.746290 nxstools-4.0.2/.ci/debian11_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2976 2023-01-30 11:59:31.000000 nxstools-4.0.2/.ci/debian11_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.746290 nxstools-4.0.2/.ci/debian9_py2/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3598 2023-01-30 11:59:31.000000 nxstools-4.0.2/.ci/debian9_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.746290 nxstools-4.0.2/.ci/debian9_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3612 2023-01-30 11:59:31.000000 nxstools-4.0.2/.ci/debian9_py3/Dockerfile
--rw-r--r--   0 jkotan   (15949) irc         (39)     5204 2024-04-24 09:15:54.000000 nxstools-4.0.2/.ci/install.sh
--rw-r--r--   0 jkotan   (15949) irc         (39)      677 2023-10-27 08:48:03.000000 nxstools-4.0.2/.ci/run.sh
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.746290 nxstools-4.0.2/.ci/ubuntu18.04_py2/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3191 2023-01-30 11:59:31.000000 nxstools-4.0.2/.ci/ubuntu18.04_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.746290 nxstools-4.0.2/.ci/ubuntu18.04_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3188 2023-01-30 11:59:31.000000 nxstools-4.0.2/.ci/ubuntu18.04_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.746290 nxstools-4.0.2/.ci/ubuntu20.04_py3/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3801 2023-02-06 19:31:51.000000 nxstools-4.0.2/.ci/ubuntu20.04_py3/Dockerfile
--rw-r--r--   0 jkotan   (15949) irc         (39)      185 2022-10-12 15:26:51.000000 nxstools-4.0.2/.flake8
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.738290 nxstools-4.0.2/.github/
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.746290 nxstools-4.0.2/.github/workflows/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2095 2024-05-13 08:57:45.000000 nxstools-4.0.2/.github/workflows/tests.yml
--rw-r--r--   0 jkotan   (15949) irc         (39)       83 2014-03-04 09:18:25.000000 nxstools-4.0.2/.gitignore
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2014-03-04 09:18:25.000000 nxstools-4.0.2/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)    46450 2024-05-15 09:36:56.000000 nxstools-4.0.2/ChangeLog
--rw-r--r--   0 jkotan   (15949) irc         (39)      203 2016-11-17 08:47:01.000000 nxstools-4.0.2/MANIFEST.in
--rw-r--r--   0 jkotan   (15949) irc         (39)     4875 2024-05-15 09:37:07.882289 nxstools-4.0.2/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     3543 2023-11-08 19:31:46.000000 nxstools-4.0.2/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.750290 nxstools-4.0.2/doc/
--rw-r--r--   0 jkotan   (15949) irc         (39)     6770 2016-04-26 12:17:18.000000 nxstools-4.0.2/doc/Makefile
--rw-r--r--   0 jkotan   (15949) irc         (39)    14330 2023-11-09 13:02:28.000000 nxstools-4.0.2/doc/conf.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      484 2023-11-09 13:02:37.000000 nxstools-4.0.2/doc/index.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)     6705 2016-04-26 12:17:18.000000 nxstools-4.0.2/doc/make.bat
--rw-r--r--   0 jkotan   (15949) irc         (39)    11174 2023-11-09 13:02:37.000000 nxstools-4.0.2/doc/nxscollect.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)     3909 2023-11-09 13:02:37.000000 nxstools-4.0.2/doc/nxsconfig.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)    19089 2024-02-21 21:28:01.000000 nxstools-4.0.2/doc/nxscreate.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)     1244 2023-11-09 13:02:37.000000 nxstools-4.0.2/doc/nxsdata.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)     7020 2024-04-12 10:12:47.000000 nxstools-4.0.2/doc/nxsetup.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)    15854 2024-01-04 17:09:29.000000 nxstools-4.0.2/doc/nxsfileinfo.rst
--rw-r--r--   0 jkotan   (15949) irc         (39)     3241 2024-05-13 08:57:45.000000 nxstools-4.0.2/doc/nxstools.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.754289 nxstools-4.0.2/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)    11417 2024-05-13 08:57:45.000000 nxstools-4.0.2/man/nxscollect.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     4989 2024-05-13 08:57:45.000000 nxstools-4.0.2/man/nxsconfig.1
--rw-r--r--   0 jkotan   (15949) irc         (39)    22445 2024-05-13 08:57:45.000000 nxstools-4.0.2/man/nxscreate.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     2288 2024-05-13 08:57:45.000000 nxstools-4.0.2/man/nxsdata.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     8616 2024-05-13 08:57:45.000000 nxstools-4.0.2/man/nxsetup.1
--rw-r--r--   0 jkotan   (15949) irc         (39)    17461 2024-05-13 08:57:45.000000 nxstools-4.0.2/man/nxsfileinfo.1
--rw-r--r--   0 jkotan   (15949) irc         (39)   428821 2024-05-13 08:57:45.000000 nxstools-4.0.2/man/nxstools.1
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       73 2016-03-02 14:46:03.000000 nxstools-4.0.2/nxscollect
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       71 2016-11-02 14:11:38.000000 nxstools-4.0.2/nxsconfig
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       72 2016-11-08 13:51:28.000000 nxstools-4.0.2/nxscreate
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       67 2016-04-21 09:21:42.000000 nxstools-4.0.2/nxsdata
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       67 2019-02-22 09:13:56.000000 nxstools-4.0.2/nxsetup
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       75 2016-11-08 13:51:28.000000 nxstools-4.0.2/nxsfileinfo
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.762290 nxstools-4.0.2/nxstools/
--rw-r--r--   0 jkotan   (15949) irc         (39)      899 2023-11-09 13:02:28.000000 nxstools-4.0.2/nxstools/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3401 2023-11-09 13:02:28.000000 nxstools-4.0.2/nxstools/filenamegenerator.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    31327 2024-05-13 08:57:45.000000 nxstools-4.0.2/nxstools/filewriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    59098 2024-05-13 08:57:45.000000 nxstools-4.0.2/nxstools/h5cppwriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    47629 2023-11-09 13:02:28.000000 nxstools-4.0.2/nxstools/h5pywriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    58193 2024-05-15 09:36:56.000000 nxstools-4.0.2/nxstools/h5rediswriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3241 2023-11-09 13:02:28.000000 nxstools-4.0.2/nxstools/nxsargparser.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    64898 2023-11-09 13:02:28.000000 nxstools-4.0.2/nxstools/nxscollect.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    61440 2023-11-09 13:02:28.000000 nxstools-4.0.2/nxstools/nxsconfig.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    65063 2024-02-21 21:28:01.000000 nxstools-4.0.2/nxstools/nxscreate.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   111677 2024-02-21 21:28:01.000000 nxstools-4.0.2/nxstools/nxscreator.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11170 2023-11-09 13:02:28.000000 nxstools-4.0.2/nxstools/nxsdata.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    14584 2024-05-13 08:57:45.000000 nxstools-4.0.2/nxstools/nxsdevicetools.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    67628 2024-04-12 10:12:47.000000 nxstools-4.0.2/nxstools/nxsetup.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   188157 2024-02-09 08:24:05.000000 nxstools-4.0.2/nxstools/nxsfileinfo.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    27916 2024-05-08 07:07:07.000000 nxstools-4.0.2/nxstools/nxsfileparser.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    35902 2023-11-09 13:02:28.000000 nxstools-4.0.2/nxstools/nxsparser.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    25209 2023-11-09 13:02:28.000000 nxstools-4.0.2/nxstools/nxsxml.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.766290 nxstools-4.0.2/nxstools/ontology/
--rw-r--r--   0 jkotan   (15949) irc         (39)     5583 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/ontology/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   191838 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/ontology/ontology.json
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.774289 nxstools-4.0.2/nxstools/pyeval/
--rw-r--r--   0 jkotan   (15949) irc         (39)      848 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1922 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/absorber.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5617 2022-12-12 11:56:25.000000 nxstools-4.0.2/nxstools/pyeval/beamtimeid.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2119 2022-11-02 12:53:27.000000 nxstools-4.0.2/nxstools/pyeval/cobold.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3836 2022-11-02 07:07:13.000000 nxstools-4.0.2/nxstools/pyeval/common.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2307 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/dalsa.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7272 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/dalsavds.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7304 2023-07-05 09:24:53.000000 nxstools-4.0.2/nxstools/pyeval/datasignal.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2063 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/dcm.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4561 2024-02-19 12:22:32.000000 nxstools-4.0.2/nxstools/pyeval/eigerdectris.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10653 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/lambdavds.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2876 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/limaccd.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3894 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/lmbd.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1722 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/marccd.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1897 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/mssar.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2279 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/mythen.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2629 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/pco.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2975 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/pe.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5841 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/pilatus.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1551 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/qbpm.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7449 2024-01-02 20:17:43.000000 nxstools-4.0.2/nxstools/pyeval/scdataset.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    14955 2024-02-21 21:28:01.000000 nxstools-4.0.2/nxstools/pyeval/secop.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2253 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/tangovimba.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2888 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/pyeval/timestamp.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2502 2024-05-13 08:57:45.000000 nxstools-4.0.2/nxstools/redisutils.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      889 2024-05-15 09:36:56.000000 nxstools-4.0.2/nxstools/release.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.822289 nxstools-4.0.2/nxstools/xmltemplates/
--rw-r--r--   0 jkotan   (15949) irc         (39)    66661 2024-02-21 21:28:01.000000 nxstools-4.0.2/nxstools/xmltemplates/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2183 2022-12-06 15:35:05.000000 nxstools-4.0.2/nxstools/xmltemplates/absorber.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      272 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/absorber_foil.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      287 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/absorber_thickness.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2002 2022-11-25 10:06:49.000000 nxstools-4.0.2/nxstools/xmltemplates/beamstop.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      171 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/beamtime_filename.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-4.0.2/nxstools/xmltemplates/beamtime_id.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      443 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/beamtimefname.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      330 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/beamtimefname.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      436 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/beamtimeid.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      258 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/beamtimeid.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     6163 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/chcut.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      282 2022-11-08 06:33:42.000000 nxstools-4.0.2/nxstools/xmltemplates/chcut_crystal.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      358 2022-11-08 06:33:42.000000 nxstools-4.0.2/nxstools/xmltemplates/chcut_unitcalibration.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      156 2019-09-25 10:15:20.000000 nxstools-4.0.2/nxstools/xmltemplates/chemical_formula.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      216 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/client_start_time.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      732 2022-11-02 12:07:43.000000 nxstools-4.0.2/nxstools/xmltemplates/cobold.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1694 2022-11-02 12:07:43.000000 nxstools-4.0.2/nxstools/xmltemplates/coboldhisto.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      324 2022-11-02 12:07:43.000000 nxstools-4.0.2/nxstools/xmltemplates/coboldhisto_timeofflight.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)       96 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/collect2.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      119 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/collect3.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      143 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/collect4.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      166 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/collect5.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      189 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/collect6.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      214 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/common2_common.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      237 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/common3_common.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3334 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/dalsa.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      438 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/dalsa_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      599 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/dalsa_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3375 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/dalsavds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      342 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/dalsavds_filestartnum_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      354 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/dalsavds_nrexposedframes_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      336 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/dalsavds_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1088 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/dalsavds_triggermode_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      597 2022-11-02 07:59:08.000000 nxstools-4.0.2/nxstools/xmltemplates/dataaxessignal.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      506 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/datasignal.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)    11075 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/dcm.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      230 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/dcm_crystal.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      236 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/dcm_reflection.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      246 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/dcm_unitcalibration.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      189 2019-09-25 14:14:28.000000 nxstools-4.0.2/nxstools/xmltemplates/default.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      502 2023-07-05 09:24:53.000000 nxstools-4.0.2/nxstools/xmltemplates/defaultaxes.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2702 2024-05-13 08:57:45.000000 nxstools-4.0.2/nxstools/xmltemplates/defaultinstrument.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      428 2019-09-25 14:15:25.000000 nxstools-4.0.2/nxstools/xmltemplates/defaultsample.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      441 2023-07-05 09:24:53.000000 nxstools-4.0.2/nxstools/xmltemplates/defaultsignal.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      274 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/description.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      246 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/descriptiontext.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1183 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/detectorlive.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2356 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/eigerdectris.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      320 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/eigerdectris_description_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      370 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/eigerdectris_stepindex.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      555 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/eigerdectris_triggermode_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)       49 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/empty.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      228 2019-09-25 10:15:20.000000 nxstools-4.0.2/nxstools/xmltemplates/end_time.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      168 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/experiment_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      304 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/groupsecop.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      403 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/groupsecop_time.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      909 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/keithley.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4545 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/lambda.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4815 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/lambda2m.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      456 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/lambda2m_m1_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-4.0.2/nxstools/xmltemplates/lambda2m_m1_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      456 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/lambda2m_m2_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-4.0.2/nxstools/xmltemplates/lambda2m_m2_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      456 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/lambda2m_m3_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-4.0.2/nxstools/xmltemplates/lambda2m_m3_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      566 2023-02-14 07:32:53.000000 nxstools-4.0.2/nxstools/xmltemplates/lambda_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      345 2019-09-25 10:15:20.000000 nxstools-4.0.2/nxstools/xmltemplates/lambda_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4643 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/lambdavds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      307 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/lambdavds_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      337 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/lambdavds_framenumbers_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      342 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/lambdavds_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      334 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/lambdavds_savefilename_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      858 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4612 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/lambdavdsnm.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      342 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/lambdavdsnm_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      877 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/lambdavdsnm_triggermode_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4056 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/limaccd.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      413 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/limaccd_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      412 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/limaccd_filestartnum_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      646 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/limaccd_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      295 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/limaccd_xpixelsize.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      295 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/limaccd_ypixelsize.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3223 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/maia.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1313 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/maiadimension.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1170 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/maiaflux.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1502 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/marccd.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      414 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/marccd_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1628 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/mcaxia.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      263 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/msnsar_env.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      262 2023-02-14 17:32:17.000000 nxstools-4.0.2/nxstools/xmltemplates/mssar_env.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3353 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/mythen.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3563 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/mythen2.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      280 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/mythen_filestartnumber.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      410 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/mythen_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      264 2019-09-25 10:15:20.000000 nxstools-4.0.2/nxstools/xmltemplates/nexdatas_configuration.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      236 2022-11-08 06:33:42.000000 nxstools-4.0.2/nxstools/xmltemplates/nexdatas_version.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      301 2022-12-06 18:19:56.000000 nxstools-4.0.2/nxstools/xmltemplates/parametercopymap.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3755 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/pco.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      278 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/pco_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      382 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/pco_filestartnum_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      520 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/pco_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4332 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/perkinelmerdetector.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      271 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/perkinelmerdetector_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      307 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/perkinelmerdetector_fileindex_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      469 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/perkinelmerdetector_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2493 2022-10-26 05:57:42.000000 nxstools-4.0.2/nxstools/xmltemplates/pilatus.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      279 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/pilatus100k_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      277 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/pilatus1m_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      277 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/pilatus2m_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      279 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/pilatus300k_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      277 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/pilatus6m_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      278 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/pilatus_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      391 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/pilatus_filestartnum_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      383 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/pilatus_mxparameters_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      529 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/pilatus_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2028 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/pinhole.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      560 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/pointdet.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2186 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/qbpm.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      265 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/qbpm_foil.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      160 2023-01-12 10:09:54.000000 nxstools-4.0.2/nxstools/xmltemplates/sample_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      327 2024-02-20 16:16:42.000000 nxstools-4.0.2/nxstools/xmltemplates/sample_env_links.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      326 2024-02-20 16:16:42.000000 nxstools-4.0.2/nxstools/xmltemplates/sample_log_links.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      207 2019-09-25 10:15:20.000000 nxstools-4.0.2/nxstools/xmltemplates/sample_name.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      309 2024-02-21 10:18:02.000000 nxstools-4.0.2/nxstools/xmltemplates/sample_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      315 2023-01-12 10:09:54.000000 nxstools-4.0.2/nxstools/xmltemplates/sampledescription.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      296 2023-01-12 10:09:54.000000 nxstools-4.0.2/nxstools/xmltemplates/sampledescriptiontext.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      315 2024-02-21 21:28:01.000000 nxstools-4.0.2/nxstools/xmltemplates/sampleenv_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      596 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/samplehkl.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      311 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/sardanaenvironment.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      271 2024-02-19 15:12:24.000000 nxstools-4.0.2/nxstools/xmltemplates/secop.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      371 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/secop_time.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-4.0.2/nxstools/xmltemplates/signal_axes.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-4.0.2/nxstools/xmltemplates/signal_name.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      384 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/signalname.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      259 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/singlesecop.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      359 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/singlesecop_time.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     5066 2023-02-28 12:36:19.000000 nxstools-4.0.2/nxstools/xmltemplates/slit.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      920 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/source.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      209 2022-10-20 05:49:21.000000 nxstools-4.0.2/nxstools/xmltemplates/start_time.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      247 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/start_timestamp.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      321 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/starttime.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      308 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/starttime.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      274 2022-10-19 07:07:03.000000 nxstools-4.0.2/nxstools/xmltemplates/tango.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1395 2019-09-25 10:30:34.000000 nxstools-4.0.2/nxstools/xmltemplates/tangovimba.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      478 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/tangovimba_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      603 2022-10-25 19:40:52.000000 nxstools-4.0.2/nxstools/xmltemplates/tangovimba_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      134 2019-09-25 10:15:20.000000 nxstools-4.0.2/nxstools/xmltemplates/title.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2369 2022-10-12 15:26:51.000000 nxstools-4.0.2/nxstools/xmltemplates/undulator.xml
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.762290 nxstools-4.0.2/nxstools.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)     4875 2024-05-15 09:37:07.000000 nxstools-4.0.2/nxstools.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)    11755 2024-05-15 09:37:07.000000 nxstools-4.0.2/nxstools.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2024-05-15 09:37:07.000000 nxstools-4.0.2/nxstools.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2019-10-10 18:35:39.000000 nxstools-4.0.2/nxstools.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       41 2024-05-15 09:37:07.000000 nxstools-4.0.2/nxstools.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        9 2024-05-15 09:37:07.000000 nxstools-4.0.2/nxstools.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      201 2024-05-15 09:37:07.882289 nxstools-4.0.2/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     4783 2024-05-14 07:32:44.000000 nxstools-4.0.2/setup.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.862289 nxstools-4.0.2/test/
--rw-r--r--   0 jkotan   (15949) irc         (39)   344154 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/FileWriterH5CppH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   179723 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/FileWriterH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   172755 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/FileWriterH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   215920 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/H5CppWriter_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   181022 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/H5PYWriter_test.py
--rwxr-xr-x   0 jkotan   (15949) irc         (39)    12534 2022-11-15 13:21:44.000000 nxstools-4.0.2/test/MacroServer2
--rwxr-xr-x   0 jkotan   (15949) irc         (39)    12534 2022-11-15 13:21:44.000000 nxstools-4.0.2/test/MacroServer3
--rw-r--r--   0 jkotan   (15949) irc         (39)     6333 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/MacroServerSetUp.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1378 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCollectH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1375 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCollectH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   286941 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCollect_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   312641 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSConfig_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateClientDSDB2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateClientDSDBR2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2513 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateClientDSDBR_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5158 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateClientDSDB_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4692 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateClientDSFS2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateClientDSFS3_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    23938 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateClientDSFS_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1505 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateCompDB2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1512 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateCompDBR2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2469 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateCompDBR_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4986 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateCompDB_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11295 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateCompFS2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1512 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateCompFS3_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   106092 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateCompFS_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    24689 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateCompare_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateDeviceDSDB2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateDeviceDSDBR2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2513 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateDeviceDSDBR_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10662 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateDeviceDSDB_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    12050 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateDeviceDSFS2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateDeviceDSFS3_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    13367 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateDeviceDSFS4_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    52028 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateDeviceDSFS_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2024-03-27 12:55:16.000000 nxstools-4.0.2/test/NXSCreateOnlineCPDB2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineCPDBR2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3140 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineCPDBR_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5112 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineCPDB_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    20755 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineCPFS2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineCPFS3_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   118294 2024-03-27 14:00:23.000000 nxstools-4.0.2/test/NXSCreateOnlineCPFS_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1532 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineDSDB2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1619 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineDSDBE2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1597 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineDSDBE_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineDSDBR2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3282 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineDSDBR_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5193 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineDSDB_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     8102 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineDSFS2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineDSFS3_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    70429 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateOnlineDSFS_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1519 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreatePoolDSDB2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1526 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreatePoolDSDBR2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3178 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreatePoolDSDBR_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5044 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreatePoolDSDB_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     8582 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreatePoolDSFS2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1526 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreatePoolDSFS3_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    43545 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreatePoolDSFS_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   111513 2023-12-18 11:00:31.000000 nxstools-4.0.2/test/NXSCreatePyEvalH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1483 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreatePyEvalH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1526 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateStdCompDB2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1665 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateStdCompDBE2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1642 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateStdCompDBE_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1582 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateStdCompDBR2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3181 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateStdCompDBR_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5116 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateStdCompDB_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    13494 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateStdCompFS2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1589 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateStdCompFS3_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    74098 2024-05-13 08:57:45.000000 nxstools-4.0.2/test/NXSCreateStdCompFS_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1526 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateTangoDSDB2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateTangoDSDBR2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2502 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateTangoDSDBR_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5019 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateTangoDSDB_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6160 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateTangoDSFS2_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateTangoDSFS3_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    51953 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreateTangoDSFS_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7127 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSCreate_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    92377 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSData_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1386 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSFileInfoH5Cpp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1383 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSFileInfoH5PY_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   568895 2024-02-08 19:21:48.000000 nxstools-4.0.2/test/NXSFileInfo_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1147 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/NXSTools_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)   223693 2024-03-27 14:00:23.000000 nxstools-4.0.2/test/NXSetUp_test.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4543 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/ServerSetUp.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10230 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/TestPool.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5183 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/TestPoolSetUp.py
--rwxr-xr-x   0 jkotan   (15949) irc         (39)    55523 2022-11-15 13:21:44.000000 nxstools-4.0.2/test/TestServer2
--rwxr-xr-x   0 jkotan   (15949) irc         (39)    55525 2022-11-15 13:21:44.000000 nxstools-4.0.2/test/TestServer3
--rw-r--r--   0 jkotan   (15949) irc         (39)    11787 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/TestServerSetUp.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4582 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/WriterSetUp.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      937 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/__init__.py
--rwxr-xr-x   0 jkotan   (15949) irc         (39)      945 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/__main__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4476 2023-11-09 13:02:28.000000 nxstools-4.0.2/test/checks.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.878289 nxstools-4.0.2/test/files/
--rw-r--r--   0 jkotan   (15949) irc         (39)   101011 2022-10-12 15:26:51.000000 nxstools-4.0.2/test/files/test_file.cbf
--rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.2/test/files/test_file.tif
--rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.2/test/files/test_file0.tif
--rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.2/test/files/test_file1.tif
--rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.2/test/files/test_file2.tif
--rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.2/test/files/test_file3.tif
--rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.2/test/files/test_file4.tif
--rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.2/test/files/test_file5.tif
--rwxr-xr-x   0 jkotan   (15949) irc         (39)    18658 2024-05-13 08:57:45.000000 nxstools-4.0.2/test/main.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.882289 nxstools-4.0.2/test/nxsextrasp00/
--rw-r--r--   0 jkotan   (15949) irc         (39)     4449 2022-10-12 15:26:51.000000 nxstools-4.0.2/test/nxsextrasp00/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      143 2022-10-12 15:26:51.000000 nxstools-4.0.2/test/nxsextrasp00/collect4.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      258 2022-10-12 15:26:51.000000 nxstools-4.0.2/test/nxsextrasp00/common4_common.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      565 2022-10-12 15:26:51.000000 nxstools-4.0.2/test/nxsextrasp00/mymca.xml
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-15 09:37:07.882289 nxstools-4.0.2/tests/
--rwxr-xr-x   0 jkotan   (15949) irc         (39)     2802 2023-11-09 13:02:28.000000 nxstools-4.0.2/tests/simpleXMLAScan.py
--rwxr-xr-x   0 jkotan   (15949) irc         (39)     2449 2023-11-09 13:02:28.000000 nxstools-4.0.2/tests/simpleXMLCScan.py
--rwxr-xr-x   0 jkotan   (15949) irc         (39)     2411 2023-11-09 13:02:28.000000 nxstools-4.0.2/tests/simpleXMLScan.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     7217 2023-11-09 13:02:28.000000 nxstools-4.0.2/tests/testNXSxml.py
--rwxr-xr-x   0 jkotan   (15949) irc         (39)     5304 2023-11-09 13:02:28.000000 nxstools-4.0.2/tests/testXMLCreator.py
--rwxr-xr-x   0 jkotan   (15949) irc         (39)     7425 2023-11-09 13:02:28.000000 nxstools-4.0.2/tests/testXMLtrigger.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.477767 nxstools-4.1.0/
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.277763 nxstools-4.1.0/.ci/
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.277763 nxstools-4.1.0/.ci/debian10_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3614 2023-01-30 11:59:31.000000 nxstools-4.1.0/.ci/debian10_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.277763 nxstools-4.1.0/.ci/debian10_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3642 2023-01-30 11:59:31.000000 nxstools-4.1.0/.ci/debian10_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.277763 nxstools-4.1.0/.ci/debian11_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2976 2023-01-30 11:59:31.000000 nxstools-4.1.0/.ci/debian11_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.281763 nxstools-4.1.0/.ci/debian9_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3598 2023-01-30 11:59:31.000000 nxstools-4.1.0/.ci/debian9_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.281763 nxstools-4.1.0/.ci/debian9_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3612 2023-01-30 11:59:31.000000 nxstools-4.1.0/.ci/debian9_py3/Dockerfile
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5204 2024-04-24 09:15:54.000000 nxstools-4.1.0/.ci/install.sh
+-rw-r--r--   0 jkotan   (15949) irc         (39)      677 2023-10-27 08:48:03.000000 nxstools-4.1.0/.ci/run.sh
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.281763 nxstools-4.1.0/.ci/ubuntu18.04_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3191 2023-01-30 11:59:31.000000 nxstools-4.1.0/.ci/ubuntu18.04_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.281763 nxstools-4.1.0/.ci/ubuntu18.04_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3188 2023-01-30 11:59:31.000000 nxstools-4.1.0/.ci/ubuntu18.04_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.281763 nxstools-4.1.0/.ci/ubuntu20.04_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3801 2023-02-06 19:31:51.000000 nxstools-4.1.0/.ci/ubuntu20.04_py3/Dockerfile
+-rw-r--r--   0 jkotan   (15949) irc         (39)      185 2022-10-12 15:26:51.000000 nxstools-4.1.0/.flake8
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.269763 nxstools-4.1.0/.github/
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.281763 nxstools-4.1.0/.github/workflows/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2095 2024-05-13 08:57:45.000000 nxstools-4.1.0/.github/workflows/tests.yml
+-rw-r--r--   0 jkotan   (15949) irc         (39)       83 2014-03-04 09:18:25.000000 nxstools-4.1.0/.gitignore
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2014-03-04 09:18:25.000000 nxstools-4.1.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)    46599 2024-05-23 04:47:10.000000 nxstools-4.1.0/ChangeLog
+-rw-r--r--   0 jkotan   (15949) irc         (39)      203 2016-11-17 08:47:01.000000 nxstools-4.1.0/MANIFEST.in
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4875 2024-05-23 04:48:28.477767 nxstools-4.1.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3543 2023-11-08 19:31:46.000000 nxstools-4.1.0/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.289764 nxstools-4.1.0/doc/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6770 2016-04-26 12:17:18.000000 nxstools-4.1.0/doc/Makefile
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14330 2023-11-09 13:02:28.000000 nxstools-4.1.0/doc/conf.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      484 2023-11-09 13:02:37.000000 nxstools-4.1.0/doc/index.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6705 2016-04-26 12:17:18.000000 nxstools-4.1.0/doc/make.bat
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11174 2023-11-09 13:02:37.000000 nxstools-4.1.0/doc/nxscollect.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3909 2023-11-09 13:02:37.000000 nxstools-4.1.0/doc/nxsconfig.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)    19089 2024-02-21 21:28:01.000000 nxstools-4.1.0/doc/nxscreate.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1244 2023-11-09 13:02:37.000000 nxstools-4.1.0/doc/nxsdata.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7020 2024-04-12 10:12:47.000000 nxstools-4.1.0/doc/nxsetup.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)    15854 2024-01-04 17:09:29.000000 nxstools-4.1.0/doc/nxsfileinfo.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3241 2024-05-13 08:57:45.000000 nxstools-4.1.0/doc/nxstools.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.293763 nxstools-4.1.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11417 2024-05-13 08:57:45.000000 nxstools-4.1.0/man/nxscollect.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4989 2024-05-13 08:57:45.000000 nxstools-4.1.0/man/nxsconfig.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)    22445 2024-05-13 08:57:45.000000 nxstools-4.1.0/man/nxscreate.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2288 2024-05-13 08:57:45.000000 nxstools-4.1.0/man/nxsdata.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8616 2024-05-13 08:57:45.000000 nxstools-4.1.0/man/nxsetup.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)    17461 2024-05-13 08:57:45.000000 nxstools-4.1.0/man/nxsfileinfo.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)   428821 2024-05-13 08:57:45.000000 nxstools-4.1.0/man/nxstools.1
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       73 2016-03-02 14:46:03.000000 nxstools-4.1.0/nxscollect
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       71 2016-11-02 14:11:38.000000 nxstools-4.1.0/nxsconfig
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       72 2016-11-08 13:51:28.000000 nxstools-4.1.0/nxscreate
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       67 2016-04-21 09:21:42.000000 nxstools-4.1.0/nxsdata
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       67 2019-02-22 09:13:56.000000 nxstools-4.1.0/nxsetup
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       75 2016-11-08 13:51:28.000000 nxstools-4.1.0/nxsfileinfo
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.305764 nxstools-4.1.0/nxstools/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      899 2023-11-09 13:02:28.000000 nxstools-4.1.0/nxstools/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3401 2023-11-09 13:02:28.000000 nxstools-4.1.0/nxstools/filenamegenerator.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    31327 2024-05-13 08:57:45.000000 nxstools-4.1.0/nxstools/filewriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    59098 2024-05-13 08:57:45.000000 nxstools-4.1.0/nxstools/h5cppwriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    47629 2023-11-09 13:02:28.000000 nxstools-4.1.0/nxstools/h5pywriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    58193 2024-05-22 13:48:36.000000 nxstools-4.1.0/nxstools/h5rediswriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3241 2023-11-09 13:02:28.000000 nxstools-4.1.0/nxstools/nxsargparser.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    64898 2023-11-09 13:02:28.000000 nxstools-4.1.0/nxstools/nxscollect.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    61440 2023-11-09 13:02:28.000000 nxstools-4.1.0/nxstools/nxsconfig.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    65063 2024-02-21 21:28:01.000000 nxstools-4.1.0/nxstools/nxscreate.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   111677 2024-02-21 21:28:01.000000 nxstools-4.1.0/nxstools/nxscreator.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11170 2023-11-09 13:02:28.000000 nxstools-4.1.0/nxstools/nxsdata.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14584 2024-05-13 08:57:45.000000 nxstools-4.1.0/nxstools/nxsdevicetools.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    67628 2024-04-12 10:12:47.000000 nxstools-4.1.0/nxstools/nxsetup.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   188157 2024-02-09 08:24:05.000000 nxstools-4.1.0/nxstools/nxsfileinfo.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    27916 2024-05-08 07:07:07.000000 nxstools-4.1.0/nxstools/nxsfileparser.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35902 2023-11-09 13:02:28.000000 nxstools-4.1.0/nxstools/nxsparser.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    25209 2023-11-09 13:02:28.000000 nxstools-4.1.0/nxstools/nxsxml.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.309764 nxstools-4.1.0/nxstools/ontology/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5583 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/ontology/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   191838 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/ontology/ontology.json
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.317764 nxstools-4.1.0/nxstools/pyeval/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      848 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1922 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/absorber.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5617 2022-12-12 11:56:25.000000 nxstools-4.1.0/nxstools/pyeval/beamtimeid.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2119 2022-11-02 12:53:27.000000 nxstools-4.1.0/nxstools/pyeval/cobold.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3836 2022-11-02 07:07:13.000000 nxstools-4.1.0/nxstools/pyeval/common.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2307 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/dalsa.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7272 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/dalsavds.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7304 2023-07-05 09:24:53.000000 nxstools-4.1.0/nxstools/pyeval/datasignal.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2063 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/dcm.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4561 2024-02-19 12:22:32.000000 nxstools-4.1.0/nxstools/pyeval/eigerdectris.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10653 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/lambdavds.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2876 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/limaccd.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3894 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/lmbd.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1722 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/marccd.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1897 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/mssar.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2279 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/mythen.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2629 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/pco.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2975 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/pe.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5841 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/pilatus.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1551 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/qbpm.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7452 2024-05-23 04:47:10.000000 nxstools-4.1.0/nxstools/pyeval/scdataset.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14955 2024-02-21 21:28:01.000000 nxstools-4.1.0/nxstools/pyeval/secop.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2253 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/tangovimba.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2888 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/pyeval/timestamp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2502 2024-05-13 08:57:45.000000 nxstools-4.1.0/nxstools/redisutils.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      889 2024-05-23 04:47:10.000000 nxstools-4.1.0/nxstools/release.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.373765 nxstools-4.1.0/nxstools/xmltemplates/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    66661 2024-02-21 21:28:01.000000 nxstools-4.1.0/nxstools/xmltemplates/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2183 2022-12-06 15:35:05.000000 nxstools-4.1.0/nxstools/xmltemplates/absorber.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      272 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/absorber_foil.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      287 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/absorber_thickness.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2002 2022-11-25 10:06:49.000000 nxstools-4.1.0/nxstools/xmltemplates/beamstop.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      171 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/beamtime_filename.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-4.1.0/nxstools/xmltemplates/beamtime_id.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      443 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/beamtimefname.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      330 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/beamtimefname.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      436 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/beamtimeid.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      258 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/beamtimeid.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6163 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/chcut.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      282 2022-11-08 06:33:42.000000 nxstools-4.1.0/nxstools/xmltemplates/chcut_crystal.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      358 2022-11-08 06:33:42.000000 nxstools-4.1.0/nxstools/xmltemplates/chcut_unitcalibration.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      156 2019-09-25 10:15:20.000000 nxstools-4.1.0/nxstools/xmltemplates/chemical_formula.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      216 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/client_start_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      732 2022-11-02 12:07:43.000000 nxstools-4.1.0/nxstools/xmltemplates/cobold.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1694 2022-11-02 12:07:43.000000 nxstools-4.1.0/nxstools/xmltemplates/coboldhisto.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      324 2022-11-02 12:07:43.000000 nxstools-4.1.0/nxstools/xmltemplates/coboldhisto_timeofflight.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)       96 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/collect2.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      119 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/collect3.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      143 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/collect4.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      166 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/collect5.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      189 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/collect6.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      214 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/common2_common.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      237 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/common3_common.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3334 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/dalsa.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      438 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/dalsa_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      599 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/dalsa_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3375 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/dalsavds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      342 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/dalsavds_filestartnum_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      354 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/dalsavds_nrexposedframes_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      336 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/dalsavds_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1088 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/dalsavds_triggermode_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      597 2022-11-02 07:59:08.000000 nxstools-4.1.0/nxstools/xmltemplates/dataaxessignal.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      506 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/datasignal.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11075 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/dcm.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      230 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/dcm_crystal.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      236 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/dcm_reflection.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      246 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/dcm_unitcalibration.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      189 2019-09-25 14:14:28.000000 nxstools-4.1.0/nxstools/xmltemplates/default.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      502 2023-07-05 09:24:53.000000 nxstools-4.1.0/nxstools/xmltemplates/defaultaxes.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2702 2024-05-13 08:57:45.000000 nxstools-4.1.0/nxstools/xmltemplates/defaultinstrument.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      428 2019-09-25 14:15:25.000000 nxstools-4.1.0/nxstools/xmltemplates/defaultsample.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      441 2023-07-05 09:24:53.000000 nxstools-4.1.0/nxstools/xmltemplates/defaultsignal.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      274 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/description.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      246 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/descriptiontext.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1183 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/detectorlive.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2356 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/eigerdectris.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      320 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/eigerdectris_description_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      370 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/eigerdectris_stepindex.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      555 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/eigerdectris_triggermode_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)       49 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/empty.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      228 2019-09-25 10:15:20.000000 nxstools-4.1.0/nxstools/xmltemplates/end_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      168 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/experiment_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      304 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/groupsecop.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      403 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/groupsecop_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      909 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/keithley.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4545 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/lambda.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4815 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/lambda2m.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      456 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/lambda2m_m1_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-4.1.0/nxstools/xmltemplates/lambda2m_m1_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      456 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/lambda2m_m2_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-4.1.0/nxstools/xmltemplates/lambda2m_m2_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      456 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/lambda2m_m3_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-4.1.0/nxstools/xmltemplates/lambda2m_m3_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      566 2023-02-14 07:32:53.000000 nxstools-4.1.0/nxstools/xmltemplates/lambda_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      345 2019-09-25 10:15:20.000000 nxstools-4.1.0/nxstools/xmltemplates/lambda_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4643 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/lambdavds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      307 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/lambdavds_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      337 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/lambdavds_framenumbers_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      342 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/lambdavds_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      334 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/lambdavds_savefilename_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      858 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4612 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/lambdavdsnm.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      342 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/lambdavdsnm_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      877 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/lambdavdsnm_triggermode_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4056 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/limaccd.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      413 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/limaccd_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      412 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/limaccd_filestartnum_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      646 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/limaccd_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      295 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/limaccd_xpixelsize.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      295 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/limaccd_ypixelsize.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3223 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/maia.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1313 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/maiadimension.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1170 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/maiaflux.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1502 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/marccd.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      414 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/marccd_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1628 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/mcaxia.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      263 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/msnsar_env.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      262 2023-02-14 17:32:17.000000 nxstools-4.1.0/nxstools/xmltemplates/mssar_env.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3353 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/mythen.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3563 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/mythen2.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      280 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/mythen_filestartnumber.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      410 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/mythen_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      264 2019-09-25 10:15:20.000000 nxstools-4.1.0/nxstools/xmltemplates/nexdatas_configuration.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      236 2022-11-08 06:33:42.000000 nxstools-4.1.0/nxstools/xmltemplates/nexdatas_version.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      301 2022-12-06 18:19:56.000000 nxstools-4.1.0/nxstools/xmltemplates/parametercopymap.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3755 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/pco.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      278 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/pco_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      382 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/pco_filestartnum_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      520 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/pco_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4332 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/perkinelmerdetector.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      271 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/perkinelmerdetector_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      307 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/perkinelmerdetector_fileindex_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      469 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/perkinelmerdetector_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2493 2022-10-26 05:57:42.000000 nxstools-4.1.0/nxstools/xmltemplates/pilatus.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      279 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/pilatus100k_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      277 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/pilatus1m_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      277 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/pilatus2m_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      279 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/pilatus300k_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      277 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/pilatus6m_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      278 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/pilatus_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      391 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/pilatus_filestartnum_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      383 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/pilatus_mxparameters_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      529 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/pilatus_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2028 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/pinhole.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      560 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/pointdet.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2186 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/qbpm.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      265 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/qbpm_foil.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      160 2023-01-12 10:09:54.000000 nxstools-4.1.0/nxstools/xmltemplates/sample_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      327 2024-02-20 16:16:42.000000 nxstools-4.1.0/nxstools/xmltemplates/sample_env_links.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      326 2024-02-20 16:16:42.000000 nxstools-4.1.0/nxstools/xmltemplates/sample_log_links.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      207 2019-09-25 10:15:20.000000 nxstools-4.1.0/nxstools/xmltemplates/sample_name.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      309 2024-02-21 10:18:02.000000 nxstools-4.1.0/nxstools/xmltemplates/sample_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      315 2023-01-12 10:09:54.000000 nxstools-4.1.0/nxstools/xmltemplates/sampledescription.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      296 2023-01-12 10:09:54.000000 nxstools-4.1.0/nxstools/xmltemplates/sampledescriptiontext.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      315 2024-02-21 21:28:01.000000 nxstools-4.1.0/nxstools/xmltemplates/sampleenv_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      596 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/samplehkl.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      311 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/sardanaenvironment.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      271 2024-02-19 15:12:24.000000 nxstools-4.1.0/nxstools/xmltemplates/secop.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      371 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/secop_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-4.1.0/nxstools/xmltemplates/signal_axes.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-4.1.0/nxstools/xmltemplates/signal_name.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      384 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/signalname.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      259 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/singlesecop.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      359 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/singlesecop_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5066 2023-02-28 12:36:19.000000 nxstools-4.1.0/nxstools/xmltemplates/slit.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      920 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/source.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      209 2022-10-20 05:49:21.000000 nxstools-4.1.0/nxstools/xmltemplates/start_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      247 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/start_timestamp.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      321 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/starttime.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      308 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/starttime.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      274 2022-10-19 07:07:03.000000 nxstools-4.1.0/nxstools/xmltemplates/tango.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1395 2019-09-25 10:30:34.000000 nxstools-4.1.0/nxstools/xmltemplates/tangovimba.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      478 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/tangovimba_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      603 2022-10-25 19:40:52.000000 nxstools-4.1.0/nxstools/xmltemplates/tangovimba_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      134 2019-09-25 10:15:20.000000 nxstools-4.1.0/nxstools/xmltemplates/title.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2369 2022-10-12 15:26:51.000000 nxstools-4.1.0/nxstools/xmltemplates/undulator.xml
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.305764 nxstools-4.1.0/nxstools.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4875 2024-05-23 04:48:27.000000 nxstools-4.1.0/nxstools.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11755 2024-05-23 04:48:28.000000 nxstools-4.1.0/nxstools.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2024-05-23 04:48:27.000000 nxstools-4.1.0/nxstools.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2019-10-10 18:35:39.000000 nxstools-4.1.0/nxstools.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       41 2024-05-23 04:48:27.000000 nxstools-4.1.0/nxstools.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        9 2024-05-23 04:48:27.000000 nxstools-4.1.0/nxstools.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      201 2024-05-23 04:48:28.477767 nxstools-4.1.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4783 2024-05-14 07:32:44.000000 nxstools-4.1.0/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.449766 nxstools-4.1.0/test/
+-rw-r--r--   0 jkotan   (15949) irc         (39)   344154 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/FileWriterH5CppH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   179723 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/FileWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   172755 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/FileWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   215920 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/H5CppWriter_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   181022 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/H5PYWriter_test.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)    12534 2022-11-15 13:21:44.000000 nxstools-4.1.0/test/MacroServer2
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)    12534 2022-11-15 13:21:44.000000 nxstools-4.1.0/test/MacroServer3
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6333 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/MacroServerSetUp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1378 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCollectH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1375 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCollectH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   286941 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCollect_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   312641 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSConfig_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateClientDSDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateClientDSDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2513 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateClientDSDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5158 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateClientDSDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4692 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateClientDSFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateClientDSFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    23938 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateClientDSFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1505 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateCompDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1512 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateCompDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2469 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateCompDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4986 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateCompDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11295 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateCompFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1512 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateCompFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   106092 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateCompFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    24689 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateCompare_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateDeviceDSDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateDeviceDSDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2513 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateDeviceDSDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10662 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateDeviceDSDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    12050 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateDeviceDSFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateDeviceDSFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    13367 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateDeviceDSFS4_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    52028 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateDeviceDSFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2024-03-27 12:55:16.000000 nxstools-4.1.0/test/NXSCreateOnlineCPDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineCPDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3140 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineCPDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5112 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineCPDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    20755 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineCPFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineCPFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   118294 2024-03-27 14:00:23.000000 nxstools-4.1.0/test/NXSCreateOnlineCPFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1532 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineDSDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1619 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineDSDBE2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1597 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineDSDBE_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineDSDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3282 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineDSDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5193 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineDSDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8102 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineDSFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineDSFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    70429 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateOnlineDSFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1519 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreatePoolDSDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1526 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreatePoolDSDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3178 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreatePoolDSDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5044 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreatePoolDSDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8582 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreatePoolDSFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1526 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreatePoolDSFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    43545 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreatePoolDSFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   111513 2023-12-18 11:00:31.000000 nxstools-4.1.0/test/NXSCreatePyEvalH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1483 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreatePyEvalH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1526 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateStdCompDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1665 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateStdCompDBE2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1642 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateStdCompDBE_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1582 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateStdCompDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3181 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateStdCompDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5116 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateStdCompDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    13494 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateStdCompFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1589 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateStdCompFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    74098 2024-05-13 08:57:45.000000 nxstools-4.1.0/test/NXSCreateStdCompFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1526 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateTangoDSDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateTangoDSDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2502 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateTangoDSDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5019 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateTangoDSDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6160 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateTangoDSFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateTangoDSFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    51953 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreateTangoDSFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7127 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSCreate_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    92377 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSData_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1386 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSFileInfoH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1383 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSFileInfoH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   568895 2024-02-08 19:21:48.000000 nxstools-4.1.0/test/NXSFileInfo_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1147 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/NXSTools_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   223693 2024-03-27 14:00:23.000000 nxstools-4.1.0/test/NXSetUp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4543 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/ServerSetUp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10230 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/TestPool.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5183 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/TestPoolSetUp.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)    55523 2022-11-15 13:21:44.000000 nxstools-4.1.0/test/TestServer2
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)    55525 2022-11-15 13:21:44.000000 nxstools-4.1.0/test/TestServer3
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11787 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/TestServerSetUp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4582 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/WriterSetUp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      937 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/__init__.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      945 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/__main__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4476 2023-11-09 13:02:28.000000 nxstools-4.1.0/test/checks.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.469767 nxstools-4.1.0/test/files/
+-rw-r--r--   0 jkotan   (15949) irc         (39)   101011 2022-10-12 15:26:51.000000 nxstools-4.1.0/test/files/test_file.cbf
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.1.0/test/files/test_file.tif
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.1.0/test/files/test_file0.tif
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.1.0/test/files/test_file1.tif
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.1.0/test/files/test_file2.tif
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.1.0/test/files/test_file3.tif
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.1.0/test/files/test_file4.tif
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.1.0/test/files/test_file5.tif
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)    18658 2024-05-13 08:57:45.000000 nxstools-4.1.0/test/main.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.473767 nxstools-4.1.0/test/nxsextrasp00/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4449 2022-10-12 15:26:51.000000 nxstools-4.1.0/test/nxsextrasp00/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      143 2022-10-12 15:26:51.000000 nxstools-4.1.0/test/nxsextrasp00/collect4.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      258 2022-10-12 15:26:51.000000 nxstools-4.1.0/test/nxsextrasp00/common4_common.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      565 2022-10-12 15:26:51.000000 nxstools-4.1.0/test/nxsextrasp00/mymca.xml
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-23 04:48:28.477767 nxstools-4.1.0/tests/
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     2802 2023-11-09 13:02:28.000000 nxstools-4.1.0/tests/simpleXMLAScan.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     2449 2023-11-09 13:02:28.000000 nxstools-4.1.0/tests/simpleXMLCScan.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     2411 2023-11-09 13:02:28.000000 nxstools-4.1.0/tests/simpleXMLScan.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7217 2023-11-09 13:02:28.000000 nxstools-4.1.0/tests/testNXSxml.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     5304 2023-11-09 13:02:28.000000 nxstools-4.1.0/tests/testXMLCreator.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     7425 2023-11-09 13:02:28.000000 nxstools-4.1.0/tests/testXMLtrigger.py
```

### Comparing `nxstools-4.0.2/.ci/debian10_py2/Dockerfile` & `nxstools-4.1.0/.ci/debian10_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/.ci/debian10_py3/Dockerfile` & `nxstools-4.1.0/.ci/debian10_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/.ci/debian11_py3/Dockerfile` & `nxstools-4.1.0/.ci/debian11_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/.ci/debian9_py2/Dockerfile` & `nxstools-4.1.0/.ci/debian9_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/.ci/debian9_py3/Dockerfile` & `nxstools-4.1.0/.ci/debian9_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/.ci/install.sh` & `nxstools-4.1.0/.ci/install.sh`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/.ci/run.sh` & `nxstools-4.1.0/.ci/run.sh`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/.ci/ubuntu18.04_py2/Dockerfile` & `nxstools-4.1.0/.ci/ubuntu18.04_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/.ci/ubuntu18.04_py3/Dockerfile` & `nxstools-4.1.0/.ci/ubuntu18.04_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/.ci/ubuntu20.04_py3/Dockerfile` & `nxstools-4.1.0/.ci/ubuntu20.04_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/.github/workflows/tests.yml` & `nxstools-4.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/COPYRIGHT` & `nxstools-4.1.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/ChangeLog` & `nxstools-4.1.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-05-22 Jan Kotanski <jankotan@gmail.com>
+	* adapt the entry name in the appendentry mode to NXS_FileRecorder v3.21.0 (#637)
+	* tagged as v4.1.0
+
 2024-05-15 Jan Kotanski <jankotan@gmail.com>
 	* reduce number of plots in h5redis writer (#635)
 	* tagged as v4.0.2
 
 2024-05-12 Jan Kotanski <jankotan@gmail.com>
 	* add finish for h5redis writer
 	* tagged as v4.0.1
```

### Comparing `nxstools-4.0.2/PKG-INFO` & `nxstools-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxstools
-Version: 4.0.2
+Version: 4.1.0
 Summary: Configuration tools for NeXDaTaS Tango Servers
 Home-page: http://github.com/nexdatas/nxstools
 Author: Jan Kotanski, Eugen Wintersberger , Halil Pasic
 Author-email: jankotan@gmail.com, eugen.wintersberger@gmail.com, halil.pasic@gmail.com
 Maintainer: Jan Kotanski, Eugen Wintersberger , Halil Pasic
 Maintainer-email: jankotan@gmail.com, eugen.wintersberger@gmail.com, halil.pasic@gmail.com
 License: GNU GENERAL PUBLIC LICENSE version 3
```

### Comparing `nxstools-4.0.2/README.rst` & `nxstools-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/doc/Makefile` & `nxstools-4.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/doc/conf.py` & `nxstools-4.1.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/doc/make.bat` & `nxstools-4.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/doc/nxscollect.rst` & `nxstools-4.1.0/doc/nxscollect.rst`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/doc/nxsconfig.rst` & `nxstools-4.1.0/doc/nxsconfig.rst`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/doc/nxscreate.rst` & `nxstools-4.1.0/doc/nxscreate.rst`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/doc/nxsdata.rst` & `nxstools-4.1.0/doc/nxsdata.rst`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/doc/nxsetup.rst` & `nxstools-4.1.0/doc/nxsetup.rst`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/doc/nxsfileinfo.rst` & `nxstools-4.1.0/doc/nxsfileinfo.rst`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/doc/nxstools.rst` & `nxstools-4.1.0/doc/nxstools.rst`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/man/nxscollect.1` & `nxstools-4.1.0/man/nxscollect.1`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/man/nxsconfig.1` & `nxstools-4.1.0/man/nxsconfig.1`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/man/nxscreate.1` & `nxstools-4.1.0/man/nxscreate.1`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/man/nxsdata.1` & `nxstools-4.1.0/man/nxsdata.1`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/man/nxsetup.1` & `nxstools-4.1.0/man/nxsetup.1`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/man/nxsfileinfo.1` & `nxstools-4.1.0/man/nxsfileinfo.1`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/man/nxstools.1` & `nxstools-4.1.0/man/nxstools.1`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/__init__.py` & `nxstools-4.1.0/nxstools/__init__.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/filenamegenerator.py` & `nxstools-4.1.0/nxstools/filenamegenerator.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/filewriter.py` & `nxstools-4.1.0/nxstools/filewriter.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/h5cppwriter.py` & `nxstools-4.1.0/nxstools/h5cppwriter.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/h5pywriter.py` & `nxstools-4.1.0/nxstools/h5pywriter.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/h5rediswriter.py` & `nxstools-4.1.0/nxstools/h5rediswriter.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/nxsargparser.py` & `nxstools-4.1.0/nxstools/nxsargparser.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/nxscollect.py` & `nxstools-4.1.0/nxstools/nxscollect.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/nxsconfig.py` & `nxstools-4.1.0/nxstools/nxsconfig.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/nxscreate.py` & `nxstools-4.1.0/nxstools/nxscreate.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/nxscreator.py` & `nxstools-4.1.0/nxstools/nxscreator.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/nxsdata.py` & `nxstools-4.1.0/nxstools/nxsdata.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/nxsdevicetools.py` & `nxstools-4.1.0/nxstools/nxsdevicetools.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/nxsetup.py` & `nxstools-4.1.0/nxstools/nxsetup.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/nxsfileinfo.py` & `nxstools-4.1.0/nxstools/nxsfileinfo.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/nxsfileparser.py` & `nxstools-4.1.0/nxstools/nxsfileparser.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/nxsparser.py` & `nxstools-4.1.0/nxstools/nxsparser.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/nxsxml.py` & `nxstools-4.1.0/nxstools/nxsxml.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/ontology/__init__.py` & `nxstools-4.1.0/nxstools/ontology/__init__.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/ontology/ontology.json` & `nxstools-4.1.0/nxstools/ontology/ontology.json`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/__init__.py` & `nxstools-4.1.0/nxstools/pyeval/__init__.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/absorber.py` & `nxstools-4.1.0/nxstools/pyeval/absorber.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/beamtimeid.py` & `nxstools-4.1.0/nxstools/pyeval/beamtimeid.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/cobold.py` & `nxstools-4.1.0/nxstools/pyeval/cobold.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/common.py` & `nxstools-4.1.0/nxstools/pyeval/common.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/dalsa.py` & `nxstools-4.1.0/nxstools/pyeval/dalsa.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/dalsavds.py` & `nxstools-4.1.0/nxstools/pyeval/dalsavds.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/datasignal.py` & `nxstools-4.1.0/nxstools/pyeval/datasignal.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/dcm.py` & `nxstools-4.1.0/nxstools/pyeval/dcm.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/eigerdectris.py` & `nxstools-4.1.0/nxstools/pyeval/eigerdectris.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/lambdavds.py` & `nxstools-4.1.0/nxstools/pyeval/lambdavds.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/limaccd.py` & `nxstools-4.1.0/nxstools/pyeval/limaccd.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/lmbd.py` & `nxstools-4.1.0/nxstools/pyeval/lmbd.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/marccd.py` & `nxstools-4.1.0/nxstools/pyeval/marccd.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/mssar.py` & `nxstools-4.1.0/nxstools/pyeval/mssar.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/mythen.py` & `nxstools-4.1.0/nxstools/pyeval/mythen.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/pco.py` & `nxstools-4.1.0/nxstools/pyeval/pco.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/pe.py` & `nxstools-4.1.0/nxstools/pyeval/pe.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/pilatus.py` & `nxstools-4.1.0/nxstools/pyeval/pilatus.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/qbpm.py` & `nxstools-4.1.0/nxstools/pyeval/qbpm.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/scdataset.py` & `nxstools-4.1.0/nxstools/pyeval/scdataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 if isinstance(variables, dict) and "entryname" in variables:
                     entryname = variables["entryname"]
         except Exception:
             macro.warning("NeXusSelectorDevice is not available")
         if not nexus or appendentry is False:
             sname = "%s_%05i" % (scanname, sid)
         else:
-            sname = "%s::/%s%i;%s_%05i" % (
+            sname = "%s::/%s_%05i;%s_%05i" % (
                 scanname, entryname, sid, scanname, sid)
         if reingest:
             sname = "%s:%s" % (sname, time.time())
 
         # auto grouping
         grouping = bool(get_env_var(macro, 'SciCatAutoGrouping', False))
         if grouping:
```

### Comparing `nxstools-4.0.2/nxstools/pyeval/secop.py` & `nxstools-4.1.0/nxstools/pyeval/secop.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/tangovimba.py` & `nxstools-4.1.0/nxstools/pyeval/tangovimba.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/pyeval/timestamp.py` & `nxstools-4.1.0/nxstools/pyeval/timestamp.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/redisutils.py` & `nxstools-4.1.0/nxstools/redisutils.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/release.py` & `nxstools-4.1.0/nxstools/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """  NXS tools release version"""
 
 #: (:obj:`str`) package version
-__version__ = "4.0.2"
+__version__ = "4.1.0"
```

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/__init__.py` & `nxstools-4.1.0/nxstools/xmltemplates/__init__.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/absorber.xml` & `nxstools-4.1.0/nxstools/xmltemplates/absorber.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/beamstop.xml` & `nxstools-4.1.0/nxstools/xmltemplates/beamstop.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/chcut.xml` & `nxstools-4.1.0/nxstools/xmltemplates/chcut.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/cobold.xml` & `nxstools-4.1.0/nxstools/xmltemplates/cobold.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/coboldhisto.xml` & `nxstools-4.1.0/nxstools/xmltemplates/coboldhisto.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/dalsa.xml` & `nxstools-4.1.0/nxstools/xmltemplates/dalsa.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/dalsa_nxdata.ds.xml` & `nxstools-4.1.0/nxstools/xmltemplates/dalsa_nxdata.ds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/dalsavds.xml` & `nxstools-4.1.0/nxstools/xmltemplates/dalsavds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/dalsavds_triggermode_cb.ds.xml` & `nxstools-4.1.0/nxstools/xmltemplates/dalsavds_triggermode_cb.ds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/dataaxessignal.xml` & `nxstools-4.1.0/nxstools/xmltemplates/dataaxessignal.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/dcm.xml` & `nxstools-4.1.0/nxstools/xmltemplates/dcm.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/defaultinstrument.xml` & `nxstools-4.1.0/nxstools/xmltemplates/defaultinstrument.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/detectorlive.xml` & `nxstools-4.1.0/nxstools/xmltemplates/detectorlive.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/eigerdectris.xml` & `nxstools-4.1.0/nxstools/xmltemplates/eigerdectris.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/eigerdectris_triggermode_cb.ds.xml` & `nxstools-4.1.0/nxstools/xmltemplates/eigerdectris_triggermode_cb.ds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/keithley.xml` & `nxstools-4.1.0/nxstools/xmltemplates/keithley.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/lambda.xml` & `nxstools-4.1.0/nxstools/xmltemplates/lambda.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/lambda2m.xml` & `nxstools-4.1.0/nxstools/xmltemplates/lambda2m.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/lambda_external_data.ds.xml` & `nxstools-4.1.0/nxstools/xmltemplates/lambda_external_data.ds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/lambdavds.xml` & `nxstools-4.1.0/nxstools/xmltemplates/lambdavds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml` & `nxstools-4.1.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/lambdavdsnm.xml` & `nxstools-4.1.0/nxstools/xmltemplates/lambdavdsnm.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/lambdavdsnm_triggermode_cb.ds.xml` & `nxstools-4.1.0/nxstools/xmltemplates/lambdavdsnm_triggermode_cb.ds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/limaccd.xml` & `nxstools-4.1.0/nxstools/xmltemplates/limaccd.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/limaccd_postrun.ds.xml` & `nxstools-4.1.0/nxstools/xmltemplates/limaccd_postrun.ds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/maia.xml` & `nxstools-4.1.0/nxstools/xmltemplates/maia.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/maiadimension.xml` & `nxstools-4.1.0/nxstools/xmltemplates/maiadimension.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/maiaflux.xml` & `nxstools-4.1.0/nxstools/xmltemplates/maiaflux.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/marccd.xml` & `nxstools-4.1.0/nxstools/xmltemplates/marccd.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/mcaxia.xml` & `nxstools-4.1.0/nxstools/xmltemplates/mcaxia.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/mythen.xml` & `nxstools-4.1.0/nxstools/xmltemplates/mythen.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/mythen2.xml` & `nxstools-4.1.0/nxstools/xmltemplates/mythen2.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/pco.xml` & `nxstools-4.1.0/nxstools/xmltemplates/pco.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/pco_postrun.ds.xml` & `nxstools-4.1.0/nxstools/xmltemplates/pco_postrun.ds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/perkinelmerdetector.xml` & `nxstools-4.1.0/nxstools/xmltemplates/perkinelmerdetector.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/pilatus.xml` & `nxstools-4.1.0/nxstools/xmltemplates/pilatus.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/pilatus_postrun.ds.xml` & `nxstools-4.1.0/nxstools/xmltemplates/pilatus_postrun.ds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/pinhole.xml` & `nxstools-4.1.0/nxstools/xmltemplates/pinhole.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/pointdet.xml` & `nxstools-4.1.0/nxstools/xmltemplates/pointdet.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/qbpm.xml` & `nxstools-4.1.0/nxstools/xmltemplates/qbpm.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/samplehkl.xml` & `nxstools-4.1.0/nxstools/xmltemplates/samplehkl.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/slit.xml` & `nxstools-4.1.0/nxstools/xmltemplates/slit.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/source.xml` & `nxstools-4.1.0/nxstools/xmltemplates/source.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/tangovimba.xml` & `nxstools-4.1.0/nxstools/xmltemplates/tangovimba.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/tangovimba_nxdata.ds.xml` & `nxstools-4.1.0/nxstools/xmltemplates/tangovimba_nxdata.ds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools/xmltemplates/undulator.xml` & `nxstools-4.1.0/nxstools/xmltemplates/undulator.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/nxstools.egg-info/PKG-INFO` & `nxstools-4.1.0/nxstools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxstools
-Version: 4.0.2
+Version: 4.1.0
 Summary: Configuration tools for NeXDaTaS Tango Servers
 Home-page: http://github.com/nexdatas/nxstools
 Author: Jan Kotanski, Eugen Wintersberger , Halil Pasic
 Author-email: jankotan@gmail.com, eugen.wintersberger@gmail.com, halil.pasic@gmail.com
 Maintainer: Jan Kotanski, Eugen Wintersberger , Halil Pasic
 Maintainer-email: jankotan@gmail.com, eugen.wintersberger@gmail.com, halil.pasic@gmail.com
 License: GNU GENERAL PUBLIC LICENSE version 3
```

### Comparing `nxstools-4.0.2/nxstools.egg-info/SOURCES.txt` & `nxstools-4.1.0/nxstools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/setup.py` & `nxstools-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/FileWriterH5CppH5PY_test.py` & `nxstools-4.1.0/test/FileWriterH5CppH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/FileWriterH5Cpp_test.py` & `nxstools-4.1.0/test/FileWriterH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/FileWriterH5PY_test.py` & `nxstools-4.1.0/test/FileWriterH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/H5CppWriter_test.py` & `nxstools-4.1.0/test/H5CppWriter_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/H5PYWriter_test.py` & `nxstools-4.1.0/test/H5PYWriter_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/MacroServer2` & `nxstools-4.1.0/test/MacroServer2`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/MacroServer3` & `nxstools-4.1.0/test/MacroServer3`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/MacroServerSetUp.py` & `nxstools-4.1.0/test/MacroServerSetUp.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCollectH5Cpp_test.py` & `nxstools-4.1.0/test/NXSCollectH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCollectH5PY_test.py` & `nxstools-4.1.0/test/NXSCollectH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCollect_test.py` & `nxstools-4.1.0/test/NXSCollect_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSConfig_test.py` & `nxstools-4.1.0/test/NXSConfig_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateClientDSDB2_test.py` & `nxstools-4.1.0/test/NXSCreateClientDSDB2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateClientDSDBR2_test.py` & `nxstools-4.1.0/test/NXSCreateClientDSDBR2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateClientDSDBR_test.py` & `nxstools-4.1.0/test/NXSCreateClientDSDBR_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateClientDSDB_test.py` & `nxstools-4.1.0/test/NXSCreateClientDSDB_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateClientDSFS2_test.py` & `nxstools-4.1.0/test/NXSCreateClientDSFS2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateClientDSFS3_test.py` & `nxstools-4.1.0/test/NXSCreateClientDSFS3_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateClientDSFS_test.py` & `nxstools-4.1.0/test/NXSCreateClientDSFS_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateCompDB2_test.py` & `nxstools-4.1.0/test/NXSCreateCompDB2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateCompDBR2_test.py` & `nxstools-4.1.0/test/NXSCreateCompDBR2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateCompDBR_test.py` & `nxstools-4.1.0/test/NXSCreateCompDBR_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateCompDB_test.py` & `nxstools-4.1.0/test/NXSCreateCompDB_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateCompFS2_test.py` & `nxstools-4.1.0/test/NXSCreateCompFS2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateCompFS3_test.py` & `nxstools-4.1.0/test/NXSCreateCompFS3_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateCompFS_test.py` & `nxstools-4.1.0/test/NXSCreateCompFS_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateCompare_test.py` & `nxstools-4.1.0/test/NXSCreateCompare_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateDeviceDSDB2_test.py` & `nxstools-4.1.0/test/NXSCreateDeviceDSDB2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateDeviceDSDBR2_test.py` & `nxstools-4.1.0/test/NXSCreateDeviceDSDBR2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateDeviceDSDBR_test.py` & `nxstools-4.1.0/test/NXSCreateDeviceDSDBR_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateDeviceDSDB_test.py` & `nxstools-4.1.0/test/NXSCreateDeviceDSDB_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateDeviceDSFS2_test.py` & `nxstools-4.1.0/test/NXSCreateDeviceDSFS2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateDeviceDSFS3_test.py` & `nxstools-4.1.0/test/NXSCreateDeviceDSFS3_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateDeviceDSFS4_test.py` & `nxstools-4.1.0/test/NXSCreateDeviceDSFS4_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateDeviceDSFS_test.py` & `nxstools-4.1.0/test/NXSCreateDeviceDSFS_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineCPDB2_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineCPDB2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineCPDBR2_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineCPDBR2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineCPDBR_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineCPDBR_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineCPDB_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineCPDB_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineCPFS2_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineCPFS2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineCPFS3_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineCPFS3_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineCPFS_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineCPFS_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineDSDB2_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineDSDB2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineDSDBE2_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineDSDBE2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineDSDBE_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineDSDBE_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineDSDBR2_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineDSDBR2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineDSDBR_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineDSDBR_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineDSDB_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineDSDB_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineDSFS2_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineDSFS2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineDSFS3_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineDSFS3_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateOnlineDSFS_test.py` & `nxstools-4.1.0/test/NXSCreateOnlineDSFS_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreatePoolDSDB2_test.py` & `nxstools-4.1.0/test/NXSCreatePoolDSDB2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreatePoolDSDBR2_test.py` & `nxstools-4.1.0/test/NXSCreatePoolDSDBR2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreatePoolDSDBR_test.py` & `nxstools-4.1.0/test/NXSCreatePoolDSDBR_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreatePoolDSDB_test.py` & `nxstools-4.1.0/test/NXSCreatePoolDSDB_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreatePoolDSFS2_test.py` & `nxstools-4.1.0/test/NXSCreatePoolDSFS2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreatePoolDSFS3_test.py` & `nxstools-4.1.0/test/NXSCreatePoolDSFS3_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreatePoolDSFS_test.py` & `nxstools-4.1.0/test/NXSCreatePoolDSFS_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreatePyEvalH5Cpp_test.py` & `nxstools-4.1.0/test/NXSCreatePyEvalH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreatePyEvalH5PY_test.py` & `nxstools-4.1.0/test/NXSCreatePyEvalH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateStdCompDB2_test.py` & `nxstools-4.1.0/test/NXSCreateStdCompDB2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateStdCompDBE2_test.py` & `nxstools-4.1.0/test/NXSCreateStdCompDBE2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateStdCompDBE_test.py` & `nxstools-4.1.0/test/NXSCreateStdCompDBE_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateStdCompDBR2_test.py` & `nxstools-4.1.0/test/NXSCreateStdCompDBR2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateStdCompDBR_test.py` & `nxstools-4.1.0/test/NXSCreateStdCompDBR_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateStdCompDB_test.py` & `nxstools-4.1.0/test/NXSCreateStdCompDB_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateStdCompFS2_test.py` & `nxstools-4.1.0/test/NXSCreateStdCompFS2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateStdCompFS3_test.py` & `nxstools-4.1.0/test/NXSCreateStdCompFS3_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateStdCompFS_test.py` & `nxstools-4.1.0/test/NXSCreateStdCompFS_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateTangoDSDB2_test.py` & `nxstools-4.1.0/test/NXSCreateTangoDSDB2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateTangoDSDBR2_test.py` & `nxstools-4.1.0/test/NXSCreateTangoDSDBR2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateTangoDSDBR_test.py` & `nxstools-4.1.0/test/NXSCreateTangoDSDBR_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateTangoDSDB_test.py` & `nxstools-4.1.0/test/NXSCreateTangoDSDB_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateTangoDSFS2_test.py` & `nxstools-4.1.0/test/NXSCreateTangoDSFS2_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateTangoDSFS3_test.py` & `nxstools-4.1.0/test/NXSCreateTangoDSFS3_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreateTangoDSFS_test.py` & `nxstools-4.1.0/test/NXSCreateTangoDSFS_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSCreate_test.py` & `nxstools-4.1.0/test/NXSCreate_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSData_test.py` & `nxstools-4.1.0/test/NXSData_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSFileInfoH5Cpp_test.py` & `nxstools-4.1.0/test/NXSFileInfoH5Cpp_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSFileInfoH5PY_test.py` & `nxstools-4.1.0/test/NXSFileInfoH5PY_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSFileInfo_test.py` & `nxstools-4.1.0/test/NXSFileInfo_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSTools_test.py` & `nxstools-4.1.0/test/NXSTools_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/NXSetUp_test.py` & `nxstools-4.1.0/test/NXSetUp_test.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/ServerSetUp.py` & `nxstools-4.1.0/test/ServerSetUp.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/TestPool.py` & `nxstools-4.1.0/test/TestPool.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/TestPoolSetUp.py` & `nxstools-4.1.0/test/TestPoolSetUp.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/TestServer2` & `nxstools-4.1.0/test/TestServer2`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/TestServer3` & `nxstools-4.1.0/test/TestServer3`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/TestServerSetUp.py` & `nxstools-4.1.0/test/TestServerSetUp.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/WriterSetUp.py` & `nxstools-4.1.0/test/WriterSetUp.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/__init__.py` & `nxstools-4.1.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/__main__.py` & `nxstools-4.1.0/test/__main__.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/checks.py` & `nxstools-4.1.0/test/checks.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/files/test_file.cbf` & `nxstools-4.1.0/test/files/test_file.cbf`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/files/test_file.tif` & `nxstools-4.1.0/test/files/test_file.tif`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/files/test_file0.tif` & `nxstools-4.1.0/test/files/test_file0.tif`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/files/test_file1.tif` & `nxstools-4.1.0/test/files/test_file1.tif`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/files/test_file2.tif` & `nxstools-4.1.0/test/files/test_file2.tif`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/files/test_file3.tif` & `nxstools-4.1.0/test/files/test_file3.tif`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/files/test_file4.tif` & `nxstools-4.1.0/test/files/test_file4.tif`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/files/test_file5.tif` & `nxstools-4.1.0/test/files/test_file5.tif`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/main.py` & `nxstools-4.1.0/test/main.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/nxsextrasp00/__init__.py` & `nxstools-4.1.0/test/nxsextrasp00/__init__.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/test/nxsextrasp00/mymca.xml` & `nxstools-4.1.0/test/nxsextrasp00/mymca.xml`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/tests/simpleXMLAScan.py` & `nxstools-4.1.0/tests/simpleXMLAScan.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/tests/simpleXMLCScan.py` & `nxstools-4.1.0/tests/simpleXMLCScan.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/tests/simpleXMLScan.py` & `nxstools-4.1.0/tests/simpleXMLScan.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/tests/testNXSxml.py` & `nxstools-4.1.0/tests/testNXSxml.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/tests/testXMLCreator.py` & `nxstools-4.1.0/tests/testXMLCreator.py`

 * *Files identical despite different names*

### Comparing `nxstools-4.0.2/tests/testXMLtrigger.py` & `nxstools-4.1.0/tests/testXMLtrigger.py`

 * *Files identical despite different names*

