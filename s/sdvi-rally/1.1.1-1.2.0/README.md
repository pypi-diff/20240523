# Comparing `tmp/sdvi-rally-1.1.1.tar.gz` & `tmp/sdvi_rally-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdvi-rally-1.1.1.tar", last modified: Tue Jan  2 03:56:17 2024, max compression
+gzip compressed data, was "sdvi_rally-1.2.0.tar", last modified: Thu May 23 16:57:46 2024, max compression
```

## Comparing `sdvi-rally-1.1.1.tar` & `sdvi_rally-1.2.0.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.046506 sdvi-rally-1.1.1/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2798 2023-06-20 01:06:24.000000 sdvi-rally-1.1.1/LICENSE
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       58 2023-08-14 15:51:39.000000 sdvi-rally-1.1.1/MANIFEST.in
--rw-r--r--   0 bmarks    (1002) bmarks    (1002)    11593 2024-01-02 03:56:17.046506 sdvi-rally-1.1.1/PKG-INFO
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)    11198 2023-12-11 18:42:19.000000 sdvi-rally-1.1.1/README.md
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:16.986489 sdvi-rally-1.1.1/rally/
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)      715 2023-12-11 18:42:19.000000 sdvi-rally-1.1.1/rally/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     4541 2023-06-20 01:06:24.000000 sdvi-rally-1.1.1/rally/_rate_limit.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3524 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_session.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     1971 2023-06-20 01:06:24.000000 sdvi-rally-1.1.1/rally/_storage.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     1029 2023-06-20 01:06:24.000000 sdvi-rally-1.1.1/rally/_utils.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:16.986489 sdvi-rally-1.1.1/rally/_vendored/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        0 2023-06-20 01:06:24.000000 sdvi-rally-1.1.1/rally/_vendored/__init__.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:16.990490 sdvi-rally-1.1.1/rally/_vendored/__pycache__/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      170 2023-10-30 21:03:36.000000 sdvi-rally-1.1.1/rally/_vendored/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:16.990490 sdvi-rally-1.1.1/rally/_vendored/bin/
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)      253 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/bin/chardetect
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:16.990490 sdvi-rally-1.1.1/rally/_vendored/certifi/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       52 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/certifi/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       41 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/certifi/__main__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)   281457 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/certifi/cacert.pem
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      218 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/certifi/core.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:16.990490 sdvi-rally-1.1.1/rally/_vendored/certifi-2019.11.28.dist-info/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1580 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/certifi-2019.11.28.dist-info/DESCRIPTION.rst
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        4 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/certifi-2019.11.28.dist-info/INSTALLER
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2523 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/certifi-2019.11.28.dist-info/METADATA
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1040 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/certifi-2019.11.28.dist-info/RECORD
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      113 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/certifi-2019.11.28.dist-info/WHEEL
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1023 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/certifi-2019.11.28.dist-info/metadata.json
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        8 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/certifi-2019.11.28.dist-info/top_level.txt
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.010496 sdvi-rally-1.1.1/rally/_vendored/chardet/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1559 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    31254 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/big5freq.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1757 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/big5prober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     9411 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/chardistribution.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3787 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/charsetgroupprober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5110 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/charsetprober.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.014497 sdvi-rally-1.1.1/rally/_vendored/chardet/cli/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        0 2023-12-03 19:05:58.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/cli/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2738 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/cli/chardetect.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3590 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/codingstatemachine.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1134 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/compat.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1855 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/cp949prober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1661 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/enums.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3950 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/escprober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    10510 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/escsm.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3749 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/eucjpprober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    13546 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/euckrfreq.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1748 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/euckrprober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    31621 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/euctwfreq.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1747 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/euctwprober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    20715 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/gb2312freq.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1754 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/gb2312prober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    13838 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/hebrewprober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    25777 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/jisfreq.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    19643 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/jpcntx.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    12839 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/langbulgarianmodel.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    17948 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/langcyrillicmodel.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    12688 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/langgreekmodel.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    11345 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/langhebrewmodel.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    12592 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/langhungarianmodel.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    11290 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/langthaimodel.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    11102 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/langturkishmodel.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5370 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/latin1prober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3413 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/mbcharsetprober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2012 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/mbcsgroupprober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    25481 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/mbcssm.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5657 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/sbcharsetprober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3546 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/sbcsgroupprober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3774 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/sjisprober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    12485 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/universaldetector.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2766 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/utf8prober.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      242 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet/version.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.014497 sdvi-rally-1.1.1/rally/_vendored/chardet-3.0.4.dist-info/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2174 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet-3.0.4.dist-info/DESCRIPTION.rst
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        4 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet-3.0.4.dist-info/INSTALLER
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3239 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet-3.0.4.dist-info/METADATA
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     6073 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet-3.0.4.dist-info/RECORD
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      110 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet-3.0.4.dist-info/WHEEL
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       60 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet-3.0.4.dist-info/entry_points.txt
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1375 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet-3.0.4.dist-info/metadata.json
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        8 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/chardet-3.0.4.dist-info/top_level.txt
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.018498 sdvi-rally-1.1.1/rally/_vendored/idna/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       58 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3299 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna/codec.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      232 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna/compat.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    11733 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna/core.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    40899 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna/idnadata.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1749 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna/intranges.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       21 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna/package_data.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)   198292 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna/uts46data.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.018498 sdvi-rally-1.1.1/rally/_vendored/idna-2.8.dist-info/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        4 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna-2.8.dist-info/INSTALLER
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3947 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna-2.8.dist-info/LICENSE.rst
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     8862 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna-2.8.dist-info/METADATA
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1368 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna-2.8.dist-info/RECORD
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      110 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna-2.8.dist-info/WHEEL
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        5 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/idna-2.8.dist-info/top_level.txt
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.022499 sdvi-rally-1.1.1/rally/_vendored/requests/
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     3995 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      436 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/__version__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1096 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/_internal_utils.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)    21616 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/adapters.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     6271 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/api.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    10206 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/auth.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)      469 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/certs.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     1699 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/compat.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    18430 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/cookies.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     3201 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/exceptions.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     3594 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/help.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      757 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/hooks.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)    34295 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/models.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)      590 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/packages.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    29332 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/sessions.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     4129 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/status_codes.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2981 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/structures.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    30049 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests/utils.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.022499 sdvi-rally-1.1.1/rally/_vendored/requests-2.22.0.dist-info/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        4 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests-2.22.0.dist-info/INSTALLER
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      582 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests-2.22.0.dist-info/LICENSE
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5523 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests-2.22.0.dist-info/METADATA
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2700 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests-2.22.0.dist-info/RECORD
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      110 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests-2.22.0.dist-info/WHEEL
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        9 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/requests-2.22.0.dist-info/top_level.txt
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.022499 sdvi-rally-1.1.1/rally/_vendored/urllib3/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2683 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    10792 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/_collections.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    14026 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/connection.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    36513 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/connectionpool.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.038504 sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        0 2023-10-30 18:14:43.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      957 2023-12-03 19:06:05.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/_appengine_environ.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.042505 sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/_securetransport/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        0 2023-10-30 18:14:43.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/_securetransport/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    16886 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/_securetransport/bindings.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    11956 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/_securetransport/low_level.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    11010 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/appengine.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     4160 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/ntlmpool.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    16423 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/pyopenssl.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    32275 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/securetransport.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     7036 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/socks.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     6607 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/exceptions.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     8553 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/fields.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2440 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/filepost.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.042505 sdvi-rally-1.1.1/rally/_vendored/urllib3/packages/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      108 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/packages/__init__.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.042505 sdvi-rally-1.1.1/rally/_vendored/urllib3/packages/backports/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        0 2023-12-03 19:05:58.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/packages/backports/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1418 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/packages/backports/makefile.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    32536 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/packages/six.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.042505 sdvi-rally-1.1.1/rally/_vendored/urllib3/packages/ssl_match_hostname/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      688 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/packages/ssl_match_hostname/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5679 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    17053 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/poolmanager.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     6018 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/request.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    27833 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/response.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.046506 sdvi-rally-1.1.1/rally/_vendored/urllib3/util/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1038 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/util/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     4637 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/util/connection.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      497 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/util/queue.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3815 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/util/request.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2573 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/util/response.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    15450 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/util/retry.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    14155 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/util/ssl_.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     9871 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/util/timeout.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    13962 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/util/url.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5406 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3/util/wait.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.038504 sdvi-rally-1.1.1/rally/_vendored/urllib3-1.25.8.dist-info/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        4 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3-1.25.8.dist-info/INSTALLER
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1115 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3-1.25.8.dist-info/LICENSE.txt
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    38976 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3-1.25.8.dist-info/METADATA
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5579 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3-1.25.8.dist-info/RECORD
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        0 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3-1.25.8.dist-info/REQUESTED
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      110 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3-1.25.8.dist-info/WHEEL
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        8 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/_vendored/urllib3-1.25.8.dist-info/top_level.txt
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)    19811 2023-12-11 18:42:19.000000 sdvi-rally-1.1.1/rally/asset.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1935 2023-06-20 01:06:40.000000 sdvi-rally-1.1.1/rally/context.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     1460 2023-06-20 01:06:24.000000 sdvi-rally-1.1.1/rally/exceptions.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.046506 sdvi-rally-1.1.1/rally/experimental/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      486 2023-06-20 01:06:24.000000 sdvi-rally-1.1.1/rally/experimental/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      548 2023-06-20 01:06:24.000000 sdvi-rally-1.1.1/rally/experimental/asset_status.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)    26911 2023-12-06 17:25:56.000000 sdvi-rally-1.1.1/rally/files.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     7665 2023-08-07 17:38:43.000000 sdvi-rally-1.1.1/rally/jobs.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     2552 2023-06-20 01:06:40.000000 sdvi-rally-1.1.1/rally/notifications.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     2070 2023-06-20 01:06:24.000000 sdvi-rally-1.1.1/rally/secret.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)    25708 2023-11-28 22:18:25.000000 sdvi-rally-1.1.1/rally/supplyChain.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.046506 sdvi-rally-1.1.1/rally/tools/
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       26 2023-06-20 01:06:24.000000 sdvi-rally-1.1.1/rally/tools/__init__.py
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     4489 2023-12-11 18:42:09.000000 sdvi-rally-1.1.1/rally/tools/cli.py
--rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     4440 2023-06-20 01:06:40.000000 sdvi-rally-1.1.1/rally/userDefinedConnector.py
-drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-01-02 03:56:17.046506 sdvi-rally-1.1.1/sdvi_rally.egg-info/
--rw-r--r--   0 bmarks    (1002) bmarks    (1002)    11593 2024-01-02 03:56:16.000000 sdvi-rally-1.1.1/sdvi_rally.egg-info/PKG-INFO
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     6751 2024-01-02 03:56:16.000000 sdvi-rally-1.1.1/sdvi_rally.egg-info/SOURCES.txt
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        1 2024-01-02 03:56:16.000000 sdvi-rally-1.1.1/sdvi_rally.egg-info/dependency_links.txt
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       42 2024-01-02 03:56:16.000000 sdvi-rally-1.1.1/sdvi_rally.egg-info/entry_points.txt
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       14 2024-01-02 03:56:16.000000 sdvi-rally-1.1.1/sdvi_rally.egg-info/requires.txt
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        6 2024-01-02 03:56:16.000000 sdvi-rally-1.1.1/sdvi_rally.egg-info/top_level.txt
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       38 2024-01-02 03:56:17.046506 sdvi-rally-1.1.1/setup.cfg
--rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1168 2023-08-14 15:51:39.000000 sdvi-rally-1.1.1/setup.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.283540 sdvi_rally-1.2.0/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2798 2023-06-20 01:06:24.000000 sdvi_rally-1.2.0/LICENSE
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       58 2023-08-14 15:51:39.000000 sdvi_rally-1.2.0/MANIFEST.in
+-rw-r--r--   0 bmarks    (1002) bmarks    (1002)    11757 2024-05-23 16:57:46.275536 sdvi_rally-1.2.0/PKG-INFO
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)    11362 2024-03-27 15:01:31.000000 sdvi_rally-1.2.0/README.md
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.239520 sdvi_rally-1.2.0/rally/
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)      715 2024-03-27 15:01:31.000000 sdvi_rally-1.2.0/rally/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     4541 2023-06-20 01:06:24.000000 sdvi_rally-1.2.0/rally/_rate_limit.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3524 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_session.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     1971 2023-06-20 01:06:24.000000 sdvi_rally-1.2.0/rally/_storage.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     1029 2023-06-20 01:06:24.000000 sdvi_rally-1.2.0/rally/_utils.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.239520 sdvi_rally-1.2.0/rally/_vendored/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        0 2023-06-20 01:06:24.000000 sdvi_rally-1.2.0/rally/_vendored/__init__.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.239520 sdvi_rally-1.2.0/rally/_vendored/__pycache__/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      170 2023-10-30 21:03:36.000000 sdvi_rally-1.2.0/rally/_vendored/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.239520 sdvi_rally-1.2.0/rally/_vendored/bin/
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)      253 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/bin/chardetect
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.239520 sdvi_rally-1.2.0/rally/_vendored/certifi/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       52 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/certifi/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       41 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/certifi/__main__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)   281457 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/certifi/cacert.pem
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      218 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/certifi/core.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.239520 sdvi_rally-1.2.0/rally/_vendored/certifi-2019.11.28.dist-info/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1580 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/certifi-2019.11.28.dist-info/DESCRIPTION.rst
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        4 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/certifi-2019.11.28.dist-info/INSTALLER
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2523 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/certifi-2019.11.28.dist-info/METADATA
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1040 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/certifi-2019.11.28.dist-info/RECORD
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      113 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/certifi-2019.11.28.dist-info/WHEEL
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1023 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/certifi-2019.11.28.dist-info/metadata.json
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        8 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/certifi-2019.11.28.dist-info/top_level.txt
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.251526 sdvi_rally-1.2.0/rally/_vendored/chardet/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1559 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    31254 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/big5freq.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1757 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/big5prober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     9411 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/chardistribution.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3787 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/charsetgroupprober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5110 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/charsetprober.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.251526 sdvi_rally-1.2.0/rally/_vendored/chardet/cli/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        0 2023-12-03 19:05:58.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/cli/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2738 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/cli/chardetect.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3590 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/codingstatemachine.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1134 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/compat.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1855 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/cp949prober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1661 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/enums.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3950 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/escprober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    10510 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/escsm.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3749 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/eucjpprober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    13546 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/euckrfreq.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1748 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/euckrprober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    31621 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/euctwfreq.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1747 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/euctwprober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    20715 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/gb2312freq.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1754 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/gb2312prober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    13838 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/hebrewprober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    25777 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/jisfreq.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    19643 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/jpcntx.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    12839 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/langbulgarianmodel.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    17948 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/langcyrillicmodel.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    12688 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/langgreekmodel.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    11345 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/langhebrewmodel.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    12592 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/langhungarianmodel.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    11290 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/langthaimodel.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    11102 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/langturkishmodel.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5370 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/latin1prober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3413 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/mbcharsetprober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2012 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/mbcsgroupprober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    25481 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/mbcssm.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5657 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/sbcharsetprober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3546 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/sbcsgroupprober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3774 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/sjisprober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    12485 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/universaldetector.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2766 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/utf8prober.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      242 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet/version.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.251526 sdvi_rally-1.2.0/rally/_vendored/chardet-3.0.4.dist-info/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2174 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet-3.0.4.dist-info/DESCRIPTION.rst
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        4 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet-3.0.4.dist-info/INSTALLER
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3239 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet-3.0.4.dist-info/METADATA
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     6073 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet-3.0.4.dist-info/RECORD
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      110 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet-3.0.4.dist-info/WHEEL
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       60 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet-3.0.4.dist-info/entry_points.txt
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1375 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet-3.0.4.dist-info/metadata.json
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        8 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/chardet-3.0.4.dist-info/top_level.txt
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.259529 sdvi_rally-1.2.0/rally/_vendored/idna/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       58 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3299 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna/codec.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      232 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna/compat.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    11733 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna/core.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    40899 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna/idnadata.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1749 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna/intranges.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       21 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna/package_data.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)   198292 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna/uts46data.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.259529 sdvi_rally-1.2.0/rally/_vendored/idna-2.8.dist-info/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        4 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna-2.8.dist-info/INSTALLER
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3947 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna-2.8.dist-info/LICENSE.rst
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     8862 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna-2.8.dist-info/METADATA
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1368 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna-2.8.dist-info/RECORD
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      110 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna-2.8.dist-info/WHEEL
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        5 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/idna-2.8.dist-info/top_level.txt
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.267533 sdvi_rally-1.2.0/rally/_vendored/requests/
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     3995 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      436 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/__version__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1096 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/_internal_utils.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)    21616 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/adapters.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     6271 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/api.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    10206 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/auth.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)      469 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/certs.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     1699 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/compat.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    18430 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/cookies.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     3201 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/exceptions.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     3594 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/help.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      757 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/hooks.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)    34295 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/models.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)      590 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/packages.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    29332 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/sessions.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     4129 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/status_codes.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2981 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/structures.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    30049 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests/utils.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.267533 sdvi_rally-1.2.0/rally/_vendored/requests-2.22.0.dist-info/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        4 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests-2.22.0.dist-info/INSTALLER
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      582 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests-2.22.0.dist-info/LICENSE
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5523 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests-2.22.0.dist-info/METADATA
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2700 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests-2.22.0.dist-info/RECORD
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      110 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests-2.22.0.dist-info/WHEEL
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        9 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/requests-2.22.0.dist-info/top_level.txt
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.267533 sdvi_rally-1.2.0/rally/_vendored/urllib3/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2683 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    10792 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/_collections.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    14026 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/connection.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    36513 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/connectionpool.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.275536 sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        0 2023-10-30 18:14:43.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      957 2023-12-03 19:06:05.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/_appengine_environ.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.275536 sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/_securetransport/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        0 2023-10-30 18:14:43.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    16886 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    11956 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    11010 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/appengine.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     4160 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/ntlmpool.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    16423 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/pyopenssl.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    32275 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/securetransport.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     7036 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/socks.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     6607 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/exceptions.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     8553 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/fields.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2440 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/filepost.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.275536 sdvi_rally-1.2.0/rally/_vendored/urllib3/packages/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      108 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/packages/__init__.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.275536 sdvi_rally-1.2.0/rally/_vendored/urllib3/packages/backports/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        0 2023-12-03 19:05:58.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/packages/backports/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1418 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/packages/backports/makefile.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    32536 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/packages/six.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.275536 sdvi_rally-1.2.0/rally/_vendored/urllib3/packages/ssl_match_hostname/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      688 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5679 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/packages/ssl_match_hostname/_implementation.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    17053 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/poolmanager.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     6018 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/request.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    27833 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/response.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.275536 sdvi_rally-1.2.0/rally/_vendored/urllib3/util/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1038 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/util/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     4637 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/util/connection.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      497 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/util/queue.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     3815 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/util/request.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     2573 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/util/response.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    15450 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/util/retry.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    14155 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/util/ssl_.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     9871 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/util/timeout.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    13962 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/util/url.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5406 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3/util/wait.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.275536 sdvi_rally-1.2.0/rally/_vendored/urllib3-1.25.8.dist-info/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        4 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3-1.25.8.dist-info/INSTALLER
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1115 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3-1.25.8.dist-info/LICENSE.txt
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)    38976 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3-1.25.8.dist-info/METADATA
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     5579 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3-1.25.8.dist-info/RECORD
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        0 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3-1.25.8.dist-info/REQUESTED
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      110 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3-1.25.8.dist-info/WHEEL
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        8 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/_vendored/urllib3-1.25.8.dist-info/top_level.txt
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)    19811 2023-12-11 18:42:19.000000 sdvi_rally-1.2.0/rally/asset.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1935 2023-06-20 01:06:40.000000 sdvi_rally-1.2.0/rally/context.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     1460 2023-06-20 01:06:24.000000 sdvi_rally-1.2.0/rally/exceptions.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.275536 sdvi_rally-1.2.0/rally/experimental/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      486 2023-06-20 01:06:24.000000 sdvi_rally-1.2.0/rally/experimental/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)      548 2023-06-20 01:06:24.000000 sdvi_rally-1.2.0/rally/experimental/asset_status.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)    26911 2023-12-06 17:25:56.000000 sdvi_rally-1.2.0/rally/files.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     7665 2023-08-07 17:38:43.000000 sdvi_rally-1.2.0/rally/jobs.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     2908 2024-03-27 15:01:31.000000 sdvi_rally-1.2.0/rally/notifications.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     2070 2023-06-20 01:06:24.000000 sdvi_rally-1.2.0/rally/secret.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)    25708 2023-11-28 22:18:25.000000 sdvi_rally-1.2.0/rally/supplyChain.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.275536 sdvi_rally-1.2.0/rally/tools/
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       26 2023-06-20 01:06:24.000000 sdvi_rally-1.2.0/rally/tools/__init__.py
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     4489 2023-12-11 18:42:09.000000 sdvi_rally-1.2.0/rally/tools/cli.py
+-rwxrwxr-x   0 bmarks    (1002) bmarks    (1002)     4440 2023-06-20 01:06:40.000000 sdvi_rally-1.2.0/rally/userDefinedConnector.py
+drwxrwxr-x   0 bmarks    (1002) bmarks    (1002)        0 2024-05-23 16:57:46.275536 sdvi_rally-1.2.0/sdvi_rally.egg-info/
+-rw-r--r--   0 bmarks    (1002) bmarks    (1002)    11757 2024-05-23 16:57:46.000000 sdvi_rally-1.2.0/sdvi_rally.egg-info/PKG-INFO
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     6751 2024-05-23 16:57:46.000000 sdvi_rally-1.2.0/sdvi_rally.egg-info/SOURCES.txt
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        1 2024-05-23 16:57:46.000000 sdvi_rally-1.2.0/sdvi_rally.egg-info/dependency_links.txt
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       42 2024-05-23 16:57:46.000000 sdvi_rally-1.2.0/sdvi_rally.egg-info/entry_points.txt
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       14 2024-05-23 16:57:46.000000 sdvi_rally-1.2.0/sdvi_rally.egg-info/requires.txt
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)        6 2024-05-23 16:57:46.000000 sdvi_rally-1.2.0/sdvi_rally.egg-info/top_level.txt
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)       38 2024-05-23 16:57:46.283540 sdvi_rally-1.2.0/setup.cfg
+-rw-rw-r--   0 bmarks    (1002) bmarks    (1002)     1168 2023-08-14 15:51:39.000000 sdvi_rally-1.2.0/setup.py
```

### Comparing `sdvi-rally-1.1.1/LICENSE` & `sdvi_rally-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/PKG-INFO` & `sdvi_rally-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdvi-rally
-Version: 1.1.1
+Version: 1.2.0
 Summary: Rally Python SDK
 Author: SDVI Corp
 License: Proprietary
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -15,14 +15,20 @@
 
 # Rally Python SDK
 
 A collection of classes and functions for interacting with SDVI Rally APIs.
 
 Refer to documentation found in your Rally Silo.
 
+## v1.2.0 -- released 9 April 2024
+
+### Feature
+
+- Add new `direct` flag to `notification.send_notification` to send notifications immediately instead of queueing
+
 ## v1.1.1 -- released 2 January 2023
 
 ### Fixes
 
 - Change `asset.set_asset_deadline` to allow setting deadline to None to remove deadline
 
 ---
```

### Comparing `sdvi-rally-1.1.1/README.md` & `sdvi_rally-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Rally Python SDK
 
 A collection of classes and functions for interacting with SDVI Rally APIs.
 
 Refer to documentation found in your Rally Silo.
 
+## v1.2.0 -- released 9 April 2024
+
+### Feature
+
+- Add new `direct` flag to `notification.send_notification` to send notifications immediately instead of queueing
+
 ## v1.1.1 -- released 2 January 2023
 
 ### Fixes
 
 - Change `asset.set_asset_deadline` to allow setting deadline to None to remove deadline
 
 ---
```

### Comparing `sdvi-rally-1.1.1/rally/__init__.py` & `sdvi_rally-1.2.0/rally/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 from . import files
 from . import jobs
 from . import notifications
 from . import secret
 from . import supplyChain
 from . import experimental
 
-__version__ = '1.1.1'
+__version__ = '1.2.0'
```

### Comparing `sdvi-rally-1.1.1/rally/_rate_limit.py` & `sdvi_rally-1.2.0/rally/_rate_limit.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_session.py` & `sdvi_rally-1.2.0/rally/_session.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_storage.py` & `sdvi_rally-1.2.0/rally/_storage.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_utils.py` & `sdvi_rally-1.2.0/rally/_utils.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/certifi/cacert.pem` & `sdvi_rally-1.2.0/rally/_vendored/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/certifi-2019.11.28.dist-info/DESCRIPTION.rst` & `sdvi_rally-1.2.0/rally/_vendored/certifi-2019.11.28.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/certifi-2019.11.28.dist-info/METADATA` & `sdvi_rally-1.2.0/rally/_vendored/certifi-2019.11.28.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/certifi-2019.11.28.dist-info/RECORD` & `sdvi_rally-1.2.0/rally/_vendored/certifi-2019.11.28.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/certifi-2019.11.28.dist-info/metadata.json` & `sdvi_rally-1.2.0/rally/_vendored/certifi-2019.11.28.dist-info/metadata.json`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/__init__.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/big5freq.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/big5prober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/chardistribution.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/charsetgroupprober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/charsetprober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/cli/chardetect.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/codingstatemachine.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/compat.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/cp949prober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/enums.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/escprober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/escsm.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/eucjpprober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/euckrfreq.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/euckrprober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/euctwfreq.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/euctwprober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/gb2312freq.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/gb2312prober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/hebrewprober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/jisfreq.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/jpcntx.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/langbulgarianmodel.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/langcyrillicmodel.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/langcyrillicmodel.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/langgreekmodel.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/langhebrewmodel.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/langhungarianmodel.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/langthaimodel.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/langturkishmodel.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/latin1prober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/mbcharsetprober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/mbcsgroupprober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/mbcssm.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/sbcharsetprober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/sbcsgroupprober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/sjisprober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/universaldetector.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet/utf8prober.py` & `sdvi_rally-1.2.0/rally/_vendored/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet-3.0.4.dist-info/DESCRIPTION.rst` & `sdvi_rally-1.2.0/rally/_vendored/chardet-3.0.4.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet-3.0.4.dist-info/METADATA` & `sdvi_rally-1.2.0/rally/_vendored/chardet-3.0.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet-3.0.4.dist-info/RECORD` & `sdvi_rally-1.2.0/rally/_vendored/chardet-3.0.4.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/chardet-3.0.4.dist-info/metadata.json` & `sdvi_rally-1.2.0/rally/_vendored/chardet-3.0.4.dist-info/metadata.json`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/idna/codec.py` & `sdvi_rally-1.2.0/rally/_vendored/idna/codec.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/idna/core.py` & `sdvi_rally-1.2.0/rally/_vendored/idna/core.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/idna/idnadata.py` & `sdvi_rally-1.2.0/rally/_vendored/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/idna/intranges.py` & `sdvi_rally-1.2.0/rally/_vendored/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/idna/uts46data.py` & `sdvi_rally-1.2.0/rally/_vendored/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/idna-2.8.dist-info/LICENSE.rst` & `sdvi_rally-1.2.0/rally/_vendored/idna-2.8.dist-info/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/idna-2.8.dist-info/METADATA` & `sdvi_rally-1.2.0/rally/_vendored/idna-2.8.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/idna-2.8.dist-info/RECORD` & `sdvi_rally-1.2.0/rally/_vendored/idna-2.8.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/__init__.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/_internal_utils.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/adapters.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/api.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/api.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/auth.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/compat.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/cookies.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/exceptions.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/help.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/help.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/hooks.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/models.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/models.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/packages.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/packages.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/sessions.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/status_codes.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/structures.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/structures.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests/utils.py` & `sdvi_rally-1.2.0/rally/_vendored/requests/utils.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests-2.22.0.dist-info/LICENSE` & `sdvi_rally-1.2.0/rally/_vendored/requests-2.22.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests-2.22.0.dist-info/METADATA` & `sdvi_rally-1.2.0/rally/_vendored/requests-2.22.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/requests-2.22.0.dist-info/RECORD` & `sdvi_rally-1.2.0/rally/_vendored/requests-2.22.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/__init__.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/_collections.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/connection.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/connectionpool.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/_appengine_environ.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/_securetransport/bindings.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/_securetransport/low_level.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/appengine.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/ntlmpool.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/pyopenssl.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/securetransport.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/contrib/socks.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/exceptions.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/fields.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/filepost.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/packages/backports/makefile.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/packages/six.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/packages/ssl_match_hostname/__init__.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/packages/ssl_match_hostname/__init__.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/packages/ssl_match_hostname/_implementation.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/packages/ssl_match_hostname/_implementation.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/poolmanager.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/request.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/response.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/util/__init__.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/util/connection.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/util/request.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/util/response.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/util/retry.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/util/ssl_.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/util/timeout.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/util/url.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3/util/wait.py` & `sdvi_rally-1.2.0/rally/_vendored/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3-1.25.8.dist-info/LICENSE.txt` & `sdvi_rally-1.2.0/rally/_vendored/urllib3-1.25.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3-1.25.8.dist-info/METADATA` & `sdvi_rally-1.2.0/rally/_vendored/urllib3-1.25.8.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/_vendored/urllib3-1.25.8.dist-info/RECORD` & `sdvi_rally-1.2.0/rally/_vendored/urllib3-1.25.8.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/asset.py` & `sdvi_rally-1.2.0/rally/asset.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/context.py` & `sdvi_rally-1.2.0/rally/context.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/exceptions.py` & `sdvi_rally-1.2.0/rally/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/experimental/asset_status.py` & `sdvi_rally-1.2.0/rally/experimental/asset_status.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/files.py` & `sdvi_rally-1.2.0/rally/files.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/jobs.py` & `sdvi_rally-1.2.0/rally/jobs.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/notifications.py` & `sdvi_rally-1.2.0/rally/notifications.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,37 +7,40 @@
 
 >>> from rally import notifications
 """
 __all__ = [
     'send_notification'
 ]
 
-from .context import context, JOB_UUID
+from .context import context, JOB_UUID, ASSET_ID
 from ._session import _getSession
 
 
-# TODO this method should bypass the queue
-def send_notification(destination, message, subject='No Subject: Notification from Decision Engine', attributes=None, attachments=None, group_id=None):
-    """ Send a notification or email.  The notification will be queued with Rally's Notification system and sent in the future.
+def send_notification(destination, message, subject='No Subject: Notification from Decision Engine', attributes=None, attachments=None,
+                      group_id=None, direct=False):
+    """ Send a notification or email.  The notification will be queued with Rally's Notification system and sent in the future by default,
+    or sent direct if direct is set true.
 
     :param destination: name of the notification preset, or email address
     :type destination: str
     :param message: notification contents
     :type message: str
-    :param subject: notification subject, defaults to empty string
+    :param subject: notification subject, defaults to 'No Subject: Notification from Decision Engine'
     :type subject: str, optional
     :param attributes: key value pairs to include with the notification, not supported with all notification types,
         defaults to no attributes
     :type attributes: dict, optional
     :param attachments: includes the labeled files as notification attachments, not supported with all notification
         types, defaults to no attachments
     :type attachments: list(str), optional
     :param group_id: the string value of the AWS Message Group Id to use in the notification request if applicable,
         defaults to no group
     :type group_id: str, optional
+    :param direct: flag indicating if notification should be send directly or queued, defaults to false (queued)
+    :type direct: bool, optional
 
     Usage:
 
     >>> notifications.send_notification('Notify Preset', 'Supply Chain is complete!', subject='Asset: Yak Incorporated')
 
     Sending Emails:
 
@@ -53,16 +56,21 @@
     if not isinstance(subject, str):
         raise TypeError(f'invalid subject \'{subject}\' must be of type string')
 
     s = _getSession()
     payload = {
         'destination': destination,
         'text': message,
-        'jobUuid': context(JOB_UUID),
         'subject': subject,
-        'format': 'raw',
         'attributes': attributes,
         'attachments': _attachments if _attachments else None,
-        'messageGroupId': group_id
+        'messageGroupId': group_id,
+        'direct' : direct
     }
+    if direct:
+        payload['assetId'] = context(ASSET_ID)
+    else:
+        payload['jobUuid'] = context(JOB_UUID)
+        payload['format'] =  'raw'
 
     s.post('v1.0/notify/events/new', json=payload)
+
```

### Comparing `sdvi-rally-1.1.1/rally/secret.py` & `sdvi_rally-1.2.0/rally/secret.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/supplyChain.py` & `sdvi_rally-1.2.0/rally/supplyChain.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/tools/cli.py` & `sdvi_rally-1.2.0/rally/tools/cli.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/rally/userDefinedConnector.py` & `sdvi_rally-1.2.0/rally/userDefinedConnector.py`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/sdvi_rally.egg-info/PKG-INFO` & `sdvi_rally-1.2.0/sdvi_rally.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdvi-rally
-Version: 1.1.1
+Version: 1.2.0
 Summary: Rally Python SDK
 Author: SDVI Corp
 License: Proprietary
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -15,14 +15,20 @@
 
 # Rally Python SDK
 
 A collection of classes and functions for interacting with SDVI Rally APIs.
 
 Refer to documentation found in your Rally Silo.
 
+## v1.2.0 -- released 9 April 2024
+
+### Feature
+
+- Add new `direct` flag to `notification.send_notification` to send notifications immediately instead of queueing
+
 ## v1.1.1 -- released 2 January 2023
 
 ### Fixes
 
 - Change `asset.set_asset_deadline` to allow setting deadline to None to remove deadline
 
 ---
```

### Comparing `sdvi-rally-1.1.1/sdvi_rally.egg-info/SOURCES.txt` & `sdvi_rally-1.2.0/sdvi_rally.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdvi-rally-1.1.1/setup.py` & `sdvi_rally-1.2.0/setup.py`

 * *Files identical despite different names*

