# Comparing `tmp/cargo2rpm-0.1.8.tar.gz` & `tmp/cargo2rpm-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cargo2rpm-0.1.8.tar", last modified: Mon Sep 18 16:16:48 2023, max compression
+gzip compressed data, was "cargo2rpm-0.1.9.tar", last modified: Fri Sep 22 13:04:26 2023, max compression
```

## Comparing `cargo2rpm-0.1.8.tar` & `cargo2rpm-0.1.9.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-18 16:16:48.042719 cargo2rpm-0.1.8/
--rw-r--r--   0 deca      (1000) deca      (1000)     2166 2023-09-18 16:15:49.000000 cargo2rpm-0.1.8/CHANGELOG.md
--rw-r--r--   0 deca      (1000) deca      (1000)     1059 2023-02-02 16:39:47.000000 cargo2rpm-0.1.8/LICENSE
--rw-rw-r--   0 deca      (1000) deca      (1000)       71 2023-07-31 10:25:42.000000 cargo2rpm-0.1.8/MANIFEST.in
--rw-r--r--   0 deca      (1000) deca      (1000)     1971 2023-09-18 16:16:48.042719 cargo2rpm-0.1.8/PKG-INFO
--rw-r--r--   0 deca      (1000) deca      (1000)     1142 2023-02-12 23:57:41.000000 cargo2rpm-0.1.8/README.md
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-18 16:16:48.036719 cargo2rpm-0.1.8/cargo2rpm/
--rw-r--r--   0 deca      (1000) deca      (1000)      497 2023-09-18 16:15:17.000000 cargo2rpm-0.1.8/cargo2rpm/__init__.py
--rw-r--r--   0 deca      (1000) deca      (1000)     7941 2023-09-18 16:11:36.000000 cargo2rpm-0.1.8/cargo2rpm/__main__.py
--rw-r--r--   0 deca      (1000) deca      (1000)     5648 2023-09-18 15:36:41.000000 cargo2rpm-0.1.8/cargo2rpm/cli.py
--rw-r--r--   0 deca      (1000) deca      (1000)    24552 2023-03-03 16:38:35.000000 cargo2rpm-0.1.8/cargo2rpm/metadata.py
--rw-r--r--   0 deca      (1000) deca      (1000)    15915 2023-06-12 23:49:45.000000 cargo2rpm-0.1.8/cargo2rpm/rpm.py
--rw-r--r--   0 deca      (1000) deca      (1000)    23295 2023-07-31 09:05:15.000000 cargo2rpm-0.1.8/cargo2rpm/semver.py
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-18 16:16:48.040719 cargo2rpm-0.1.8/cargo2rpm/testdata/
--rw-r--r--   0 deca      (1000) deca      (1000)     6403 2023-02-04 15:25:02.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/ahash-0.8.3.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2134 2023-06-12 20:40:02.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/aho-corasick-1.0.2.json
--rw-r--r--   0 deca      (1000) deca      (1000)     4690 2023-02-04 15:26:13.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/assert_cmd-2.0.8.json
--rw-r--r--   0 deca      (1000) deca      (1000)     3989 2023-02-04 15:27:28.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/assert_fs-1.0.10.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2177 2023-02-04 11:54:43.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/autocfg-1.1.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     4792 2023-02-04 15:28:23.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/bstr-1.2.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2078 2023-02-04 11:53:09.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/cfg-if-1.0.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)    21085 2023-02-04 15:28:56.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/clap-4.1.4.json
--rw-r--r--   0 deca      (1000) deca      (1000)    19710 2023-02-07 16:19:07.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json
--rw-r--r--   0 deca      (1000) deca      (1000)     6679 2023-02-04 15:29:26.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/gstreamer-0.19.7.json
--rw-r--r--   0 deca      (1000) deca      (1000)     3706 2023-02-04 15:30:03.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/human-panic-1.1.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     7484 2023-02-08 15:04:25.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/hyperfine-1.15.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     5189 2023-06-12 20:41:15.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/iri-string-0.7.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     7821 2023-02-07 16:31:01.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/libblkio-1.2.2.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2126 2023-02-04 11:52:04.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/libc-0.2.139.json
--rw-r--r--   0 deca      (1000) deca      (1000)     4674 2023-02-04 15:30:40.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/predicates-2.1.5.json
--rw-r--r--   0 deca      (1000) deca      (1000)     3363 2023-02-04 11:53:39.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/proc-macro2-1.0.50.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2537 2023-02-04 11:52:34.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/quote-1.0.23.json
--rw-r--r--   0 deca      (1000) deca      (1000)     3523 2023-02-04 11:44:15.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/rand-0.8.5.json
--rw-r--r--   0 deca      (1000) deca      (1000)     1963 2023-02-04 11:45:17.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/rand_core-0.6.4.json
--rw-r--r--   0 deca      (1000) deca      (1000)     6593 2023-06-12 20:40:35.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/regex-1.8.4.json
--rw-r--r--   0 deca      (1000) deca      (1000)     1816 2023-06-12 20:40:57.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/regex-syntax-0.7.2.json
--rw-r--r--   0 deca      (1000) deca      (1000)     4188 2023-02-07 16:26:50.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/rpm-sequoia-1.2.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     9928 2023-02-04 15:31:49.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/rust_decimal-1.28.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)    10741 2023-02-08 12:38:58.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/rustix-0.36.8.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2116 2023-02-04 11:54:11.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/serde-1.0.152.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2562 2023-02-10 16:01:12.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/serde_derive-1.0.152.json
--rw-r--r--   0 deca      (1000) deca      (1000)    10844 2023-02-04 11:36:50.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/syn-1.0.107.json
--rw-r--r--   0 deca      (1000) deca      (1000)     6240 2023-02-04 15:32:38.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/time-0.3.17.json
--rw-r--r--   0 deca      (1000) deca      (1000)    32900 2023-02-08 13:03:00.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/tokio-1.25.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2131 2023-02-04 11:55:18.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/unicode-xid-0.2.4.json
--rw-r--r--   0 deca      (1000) deca      (1000)    12152 2023-02-04 15:33:09.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/zbus-3.8.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)    41849 2023-02-04 15:42:40.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/zola-0.16.1.json
--rw-r--r--   0 deca      (1000) deca      (1000)     6485 2023-02-08 15:04:53.000000 cargo2rpm-0.1.8/cargo2rpm/testdata/zoxide-0.9.0.json
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-18 16:16:48.040719 cargo2rpm-0.1.8/cargo2rpm/tests/
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-18 16:16:48.041719 cargo2rpm-0.1.8/cargo2rpm/tests/metadata/
--rw-r--r--   0 deca      (1000) deca      (1000)    14347 2023-07-31 09:21:45.000000 cargo2rpm-0.1.8/cargo2rpm/tests/metadata/test_deps.py
--rw-r--r--   0 deca      (1000) deca      (1000)     7555 2023-07-31 09:17:15.000000 cargo2rpm-0.1.8/cargo2rpm/tests/metadata/test_description.py
--rw-r--r--   0 deca      (1000) deca      (1000)    41281 2023-07-31 09:20:46.000000 cargo2rpm-0.1.8/cargo2rpm/tests/metadata/test_feature_closure.py
--rw-r--r--   0 deca      (1000) deca      (1000)      493 2023-07-31 09:23:50.000000 cargo2rpm-0.1.8/cargo2rpm/tests/metadata/test_feature_flags.py
--rw-r--r--   0 deca      (1000) deca      (1000)     8469 2023-07-31 09:23:24.000000 cargo2rpm-0.1.8/cargo2rpm/tests/metadata/test_package.py
--rw-r--r--   0 deca      (1000) deca      (1000)     6979 2023-07-31 09:22:37.000000 cargo2rpm-0.1.8/cargo2rpm/tests/metadata/test_workspace_features.py
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-18 16:16:48.042719 cargo2rpm-0.1.8/cargo2rpm/tests/rpm/
--rw-r--r--   0 deca      (1000) deca      (1000)    88622 2023-07-31 09:14:05.000000 cargo2rpm-0.1.8/cargo2rpm/tests/rpm/test_buildrequires.py
--rw-r--r--   0 deca      (1000) deca      (1000)     3721 2023-07-31 09:12:00.000000 cargo2rpm-0.1.8/cargo2rpm/tests/rpm/test_provides.py
--rw-r--r--   0 deca      (1000) deca      (1000)    87145 2023-07-31 09:11:57.000000 cargo2rpm-0.1.8/cargo2rpm/tests/rpm/test_requires.py
--rw-r--r--   0 deca      (1000) deca      (1000)     8272 2023-07-31 09:13:08.000000 cargo2rpm-0.1.8/cargo2rpm/tests/rpm/test_subpackages.py
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-18 16:16:48.042719 cargo2rpm-0.1.8/cargo2rpm/tests/semver/
--rw-r--r--   0 deca      (1000) deca      (1000)     3740 2023-07-31 07:29:08.000000 cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_comparator.py
--rw-r--r--   0 deca      (1000) deca      (1000)     1172 2023-07-31 07:44:38.000000 cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_prerelease.py
--rw-r--r--   0 deca      (1000) deca      (1000)     4101 2023-07-31 09:07:21.000000 cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_prerelease_comp.py
--rw-r--r--   0 deca      (1000) deca      (1000)     4999 2023-07-31 07:26:44.000000 cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_regex.py
--rw-r--r--   0 deca      (1000) deca      (1000)     5096 2023-07-31 07:30:24.000000 cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_version.py
--rw-r--r--   0 deca      (1000) deca      (1000)     3716 2023-07-31 08:42:23.000000 cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_version_comp.py
--rw-r--r--   0 deca      (1000) deca      (1000)    10121 2023-07-31 07:29:34.000000 cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_version_req.py
--rw-r--r--   0 deca      (1000) deca      (1000)     3599 2023-02-12 23:55:37.000000 cargo2rpm-0.1.8/cargo2rpm/tests/test_cli.py
--rw-r--r--   0 deca      (1000) deca      (1000)      766 2023-02-12 21:25:39.000000 cargo2rpm-0.1.8/cargo2rpm/utils.py
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-18 16:16:48.037719 cargo2rpm-0.1.8/cargo2rpm.egg-info/
--rw-r--r--   0 deca      (1000) deca      (1000)     1971 2023-09-18 16:16:48.000000 cargo2rpm-0.1.8/cargo2rpm.egg-info/PKG-INFO
--rw-r--r--   0 deca      (1000) deca      (1000)     2460 2023-09-18 16:16:48.000000 cargo2rpm-0.1.8/cargo2rpm.egg-info/SOURCES.txt
--rw-r--r--   0 deca      (1000) deca      (1000)        1 2023-09-18 16:16:48.000000 cargo2rpm-0.1.8/cargo2rpm.egg-info/dependency_links.txt
--rw-r--r--   0 deca      (1000) deca      (1000)       54 2023-09-18 16:16:48.000000 cargo2rpm-0.1.8/cargo2rpm.egg-info/entry_points.txt
--rw-r--r--   0 deca      (1000) deca      (1000)       10 2023-09-18 16:16:48.000000 cargo2rpm-0.1.8/cargo2rpm.egg-info/top_level.txt
--rw-r--r--   0 deca      (1000) deca      (1000)      161 2023-02-02 00:36:19.000000 cargo2rpm-0.1.8/pyproject.toml
--rw-r--r--   0 deca      (1000) deca      (1000)     1023 2023-09-18 16:16:48.043719 cargo2rpm-0.1.8/setup.cfg
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-22 13:04:26.885690 cargo2rpm-0.1.9/
+-rw-r--r--   0 deca      (1000) deca      (1000)     2818 2023-09-22 13:02:17.000000 cargo2rpm-0.1.9/CHANGELOG.md
+-rw-r--r--   0 deca      (1000) deca      (1000)     1059 2023-02-02 16:39:47.000000 cargo2rpm-0.1.9/LICENSE
+-rw-rw-r--   0 deca      (1000) deca      (1000)       71 2023-07-31 10:25:42.000000 cargo2rpm-0.1.9/MANIFEST.in
+-rw-r--r--   0 deca      (1000) deca      (1000)     1971 2023-09-22 13:04:26.885690 cargo2rpm-0.1.9/PKG-INFO
+-rw-r--r--   0 deca      (1000) deca      (1000)     1142 2023-02-12 23:57:41.000000 cargo2rpm-0.1.9/README.md
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-22 13:04:26.878690 cargo2rpm-0.1.9/cargo2rpm/
+-rw-r--r--   0 deca      (1000) deca      (1000)      497 2023-09-22 13:02:21.000000 cargo2rpm-0.1.9/cargo2rpm/__init__.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     7941 2023-09-18 16:11:36.000000 cargo2rpm-0.1.9/cargo2rpm/__main__.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     5648 2023-09-18 15:36:41.000000 cargo2rpm-0.1.9/cargo2rpm/cli.py
+-rw-r--r--   0 deca      (1000) deca      (1000)    25031 2023-09-22 12:52:46.000000 cargo2rpm-0.1.9/cargo2rpm/metadata.py
+-rw-r--r--   0 deca      (1000) deca      (1000)    16170 2023-09-22 12:37:54.000000 cargo2rpm-0.1.9/cargo2rpm/rpm.py
+-rw-r--r--   0 deca      (1000) deca      (1000)    23293 2023-09-22 09:51:15.000000 cargo2rpm-0.1.9/cargo2rpm/semver.py
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-22 13:04:26.883690 cargo2rpm-0.1.9/cargo2rpm/testdata/
+-rw-r--r--   0 deca      (1000) deca      (1000)     6403 2023-02-04 15:25:02.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/ahash-0.8.3.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2134 2023-06-12 20:40:02.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/aho-corasick-1.0.2.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     4690 2023-02-04 15:26:13.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/assert_cmd-2.0.8.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     3989 2023-02-04 15:27:28.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/assert_fs-1.0.10.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2177 2023-02-04 11:54:43.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/autocfg-1.1.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     4792 2023-02-04 15:28:23.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/bstr-1.2.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2078 2023-02-04 11:53:09.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/cfg-if-1.0.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    21085 2023-02-04 15:28:56.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/clap-4.1.4.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    64518 2023-09-22 10:44:32.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/espanso-2.1.8.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    19710 2023-02-07 16:19:07.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     6679 2023-02-04 15:29:26.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/gstreamer-0.19.7.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     3706 2023-02-04 15:30:03.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/human-panic-1.1.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     7484 2023-02-08 15:04:25.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/hyperfine-1.15.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     5189 2023-06-12 20:41:15.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/iri-string-0.7.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     7821 2023-02-07 16:31:01.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/libblkio-1.2.2.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2126 2023-02-04 11:52:04.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/libc-0.2.139.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     4674 2023-02-04 15:30:40.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/predicates-2.1.5.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     3363 2023-02-04 11:53:39.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/proc-macro2-1.0.50.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2537 2023-02-04 11:52:34.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/quote-1.0.23.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     3523 2023-02-04 11:44:15.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/rand-0.8.5.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     1963 2023-02-04 11:45:17.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/rand_core-0.6.4.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     6593 2023-06-12 20:40:35.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/regex-1.8.4.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     1816 2023-06-12 20:40:57.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/regex-syntax-0.7.2.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     4188 2023-02-07 16:26:50.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/rpm-sequoia-1.2.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     9928 2023-02-04 15:31:49.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/rust_decimal-1.28.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    10741 2023-02-08 12:38:58.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/rustix-0.36.8.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2116 2023-02-04 11:54:11.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/serde-1.0.152.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2562 2023-02-10 16:01:12.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/serde_derive-1.0.152.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    10844 2023-02-04 11:36:50.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/syn-1.0.107.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     6240 2023-02-04 15:32:38.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/time-0.3.17.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    32900 2023-02-08 13:03:00.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/tokio-1.25.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2131 2023-02-04 11:55:18.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/unicode-xid-0.2.4.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    12152 2023-02-04 15:33:09.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/zbus-3.8.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    41849 2023-02-04 15:42:40.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/zola-0.16.1.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     6485 2023-02-08 15:04:53.000000 cargo2rpm-0.1.9/cargo2rpm/testdata/zoxide-0.9.0.json
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-22 13:04:26.883690 cargo2rpm-0.1.9/cargo2rpm/tests/
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-22 13:04:26.883690 cargo2rpm-0.1.9/cargo2rpm/tests/metadata/
+-rw-r--r--   0 deca      (1000) deca      (1000)    14347 2023-07-31 09:21:45.000000 cargo2rpm-0.1.9/cargo2rpm/tests/metadata/test_deps.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     7555 2023-07-31 09:17:15.000000 cargo2rpm-0.1.9/cargo2rpm/tests/metadata/test_description.py
+-rw-r--r--   0 deca      (1000) deca      (1000)    41281 2023-07-31 09:20:46.000000 cargo2rpm-0.1.9/cargo2rpm/tests/metadata/test_feature_closure.py
+-rw-r--r--   0 deca      (1000) deca      (1000)      493 2023-07-31 09:23:50.000000 cargo2rpm-0.1.9/cargo2rpm/tests/metadata/test_feature_flags.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     8659 2023-09-22 11:01:20.000000 cargo2rpm-0.1.9/cargo2rpm/tests/metadata/test_package.py
+-rw-r--r--   0 deca      (1000) deca      (1000)    10325 2023-09-22 11:41:03.000000 cargo2rpm-0.1.9/cargo2rpm/tests/metadata/test_workspace_features.py
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-22 13:04:26.884690 cargo2rpm-0.1.9/cargo2rpm/tests/rpm/
+-rw-r--r--   0 deca      (1000) deca      (1000)   102523 2023-09-22 12:39:44.000000 cargo2rpm-0.1.9/cargo2rpm/tests/rpm/test_buildrequires.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     3721 2023-07-31 09:12:00.000000 cargo2rpm-0.1.9/cargo2rpm/tests/rpm/test_provides.py
+-rw-r--r--   0 deca      (1000) deca      (1000)    87780 2023-09-22 10:01:34.000000 cargo2rpm-0.1.9/cargo2rpm/tests/rpm/test_requires.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     8272 2023-07-31 09:13:08.000000 cargo2rpm-0.1.9/cargo2rpm/tests/rpm/test_subpackages.py
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-22 13:04:26.885690 cargo2rpm-0.1.9/cargo2rpm/tests/semver/
+-rw-r--r--   0 deca      (1000) deca      (1000)     3740 2023-07-31 07:29:08.000000 cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_comparator.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     1172 2023-07-31 07:44:38.000000 cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_prerelease.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     4101 2023-07-31 09:07:21.000000 cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_prerelease_comp.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     4999 2023-07-31 07:26:44.000000 cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_regex.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     5096 2023-07-31 07:30:24.000000 cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_version.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     3716 2023-07-31 08:42:23.000000 cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_version_comp.py
+-rw-r--r--   0 deca      (1000) deca      (1000)    10121 2023-07-31 07:29:34.000000 cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_version_req.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     3599 2023-02-12 23:55:37.000000 cargo2rpm-0.1.9/cargo2rpm/tests/test_cli.py
+-rw-r--r--   0 deca      (1000) deca      (1000)      766 2023-02-12 21:25:39.000000 cargo2rpm-0.1.9/cargo2rpm/utils.py
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-09-22 13:04:26.879690 cargo2rpm-0.1.9/cargo2rpm.egg-info/
+-rw-r--r--   0 deca      (1000) deca      (1000)     1971 2023-09-22 13:04:26.000000 cargo2rpm-0.1.9/cargo2rpm.egg-info/PKG-INFO
+-rw-r--r--   0 deca      (1000) deca      (1000)     2498 2023-09-22 13:04:26.000000 cargo2rpm-0.1.9/cargo2rpm.egg-info/SOURCES.txt
+-rw-r--r--   0 deca      (1000) deca      (1000)        1 2023-09-22 13:04:26.000000 cargo2rpm-0.1.9/cargo2rpm.egg-info/dependency_links.txt
+-rw-r--r--   0 deca      (1000) deca      (1000)       54 2023-09-22 13:04:26.000000 cargo2rpm-0.1.9/cargo2rpm.egg-info/entry_points.txt
+-rw-r--r--   0 deca      (1000) deca      (1000)       10 2023-09-22 13:04:26.000000 cargo2rpm-0.1.9/cargo2rpm.egg-info/top_level.txt
+-rw-r--r--   0 deca      (1000) deca      (1000)      161 2023-02-02 00:36:19.000000 cargo2rpm-0.1.9/pyproject.toml
+-rw-r--r--   0 deca      (1000) deca      (1000)     1023 2023-09-22 13:04:26.885690 cargo2rpm-0.1.9/setup.cfg
```

### Comparing `cargo2rpm-0.1.8/CHANGELOG.md` & `cargo2rpm-0.1.9/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+## Release 0.1.9
+
+This release includes a bugfix in the support for cargo workspaces and a
+small (backwards compatible) improvement for the RPM dependency generators:
+
+- Required features of any binary targets in workspace members are now
+  resolved correctly and no longer cause crashes.
+- If crates set a minimum supported Rust version (MSRV) by using the
+  `package.rust-version` setting in `Cargo.toml`, an equivalent dependency
+  on `rust >= MSRV` is now automatically generated for crate `Requires` and
+  `BuildRequires`. This allows builds to fail fast during dependency
+  resolution instead of only failing late during the actual build stage.
+
 ## Release 0.1.8
 
 This release adds another subcommand for the cargo2rpm script, which can be
 used by RPM generators for bundled / vendored crate dependencies.
 
 ## Release 0.1.7
```

### Comparing `cargo2rpm-0.1.8/LICENSE` & `cargo2rpm-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/PKG-INFO` & `cargo2rpm-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cargo2rpm
-Version: 0.1.8
+Version: 0.1.9
 Summary: Translation layer between cargo and RPM
 Home-page: https://pagure.io/fedora-rust/cargo2rpm
 Author: Fedora Rust SIG
 Author-email: rust@lists.fedoraproject.org
 License: MIT
 Keywords: rpm,cargo,rust
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cargo2rpm-0.1.8/README.md` & `cargo2rpm-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/__main__.py` & `cargo2rpm-0.1.9/cargo2rpm/__main__.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/cli.py` & `cargo2rpm-0.1.9/cargo2rpm/cli.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/metadata.py` & `cargo2rpm-0.1.9/cargo2rpm/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,26 @@
     def target(self) -> Optional[str]:
         return self._data["target"]
 
     @property
     def path(self) -> Optional[str]:
         return self._data.get("path")
 
+    @property
+    def source(self) -> Optional[str]:
+        return self._data.get("source")
+
+    def is_path_or_git(self) -> bool:
+        if self.path:
+            return True
+        if source := self.source:
+            if source.startswith("git+"):
+                return True
+        return False
+
     def to_rpm(self, feature: Optional[str]) -> str:
         """
         Formats this crate dependency as an RPM dependency string.
         """
 
         assert self.path is None, "Attempt to generate an RPM dependency for a path dependency!"
 
@@ -610,15 +622,18 @@
             member_features[package.name] = features
 
         # enable required and default features of binary targets
         for package in self.packages:
             for target in package.targets:
                 if ("bin" in target.kind and "bin" in target.crate_types) or ("cdylib" in target.kind and "cdylib" in target.crate_types):
                     if reqs := target.required_features:
-                        required_features[package.name].update(reqs)
+                        if package.name not in required_features.keys():
+                            required_features[package.name] = set(reqs)
+                        else:
+                            required_features[package.name].update(reqs)
                     if not flags.no_default_features:
                         member_defaults[package.name] = True
 
         for package in self.packages:
             for dep in filter(lambda pkg: pkg.path is not None, package.dependencies):
                 features = member_features.get(dep.name) or set()
                 features.update(dep.features)
@@ -627,15 +642,15 @@
                 defaults = member_defaults.get(dep.name) or False
                 defaults = defaults or dep.uses_default_features
                 member_defaults[dep.name] = defaults
 
         # unconditionally add required features to resolved features:
         # "cargo build" skips building targets for which required features are
         # not enabled, but for package builds this behaviour doesn't make sense
-        for (name, required) in required_features.items():
+        for name, required in required_features.items():
             member_features[name].update(required)
 
         # turn on default features for all workspace members that are not
         # explicitly referenced by other workspace members
         for package in self.packages:
             if package.name not in member_defaults.keys():
                 member_defaults[package.name] = True
@@ -647,15 +662,15 @@
             enabled = member_features[package.name].copy()
             if member_defaults[package.name] and "default" in package.get_feature_names():
                 enabled.add("default")
 
             while True:
                 new: set[str] = set()
 
-                for (feature_name, deps) in package.features.items():
+                for feature_name, deps in package.features.items():
                     if feature_name not in enabled:
                         continue
 
                     for dep in deps:
                         # named optional dependency
                         if dep.startswith("dep:"):
                             # cargo builds all workspace members even if they are optional
```

### Comparing `cargo2rpm-0.1.8/cargo2rpm/rpm.py` & `cargo2rpm-0.1.9/cargo2rpm/rpm.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,77 +49,77 @@
     deps_enabled_features: dict[str, set[str]] = dict()
     # - determine whether default features are enabled for all dependencies
     deps_default_features: dict[str, bool] = dict()
     # - determine optional dependencies that need to be enabled as workarounds
     workarounds: dict[str, tuple[set[str], bool]] = dict()
 
     # unconditionally enabled features of normal dependencies
-    for (name, dep) in normal.items():
+    for name, dep in normal.items():
         features = deps_enabled_features.get(name) or set()
         features.update(dep.features)
         deps_enabled_features[name] = features
 
         defaults = deps_default_features.get(name) or False
         defaults = defaults or dep.uses_default_features
         deps_default_features[name] = defaults
 
     # unconditionally enabled features of enabled, optional, normal dependencies
-    for (name, dep) in normal_optional.items():
+    for name, dep in normal_optional.items():
         if name in optional_enabled:
             features = deps_enabled_features.get(name) or set()
             features.update(dep.features)
             deps_enabled_features[name] = features
 
             defaults = deps_default_features.get(name) or False
             defaults = defaults or dep.uses_default_features
             deps_default_features[name] = defaults
 
     # unconditionally enabled features of build-dependencies
-    for (name, dep) in build.items():
+    for name, dep in build.items():
         features = deps_enabled_features.get(name) or set()
         features.update(dep.features)
         deps_enabled_features[name] = features
 
         defaults = deps_default_features.get(name) or False
         defaults = defaults or dep.uses_default_features
         deps_default_features[name] = defaults
 
     # unconditionally enabled features of enabled, optional, build-dependencies
-    for (name, dep) in build_optional.items():
+    for name, dep in build_optional.items():
         if name in optional_enabled:
             features = deps_enabled_features.get(name) or set()
             features.update(dep.features)
             deps_enabled_features[name] = features
 
             defaults = deps_default_features.get(name) or False
             defaults = defaults or dep.uses_default_features
             deps_default_features[name] = defaults
 
     # unconditionally enabled features of enabled dev-dependencies
     if with_dev_deps:
-        for (name, dep) in dev.items():
+        for name, dep in dev.items():
             features = deps_enabled_features.get(name) or set()
             features.update(dep.features)
             deps_enabled_features[name] = features
 
             defaults = deps_default_features.get(name) or False
             defaults = defaults or dep.uses_default_features
             deps_default_features[name] = defaults
 
     # features unconditionally enabled by feature dependencies
-    for (name, other_features) in other_enabled.items():
+    for name, other_features in other_enabled.items():
         features = deps_enabled_features.get(name) or set()
         features.update(other_features)
         deps_enabled_features[name] = features
 
         if "default" in features:
             deps_default_features[name] = True
 
     # features conditionally enabled by feature dependencies
-    for (name, other_features) in other_conditional.items():
+    for name, other_features in other_conditional.items():
         if name in enabled or CARGO_BUGGY_RESOLVER:
             features = deps_enabled_features.get(name) or set()
             features.update(other_features)
             deps_enabled_features[name] = features
 
         if name not in enabled and CARGO_BUGGY_RESOLVER:
             defaults = deps_default_features.get(name) or False
@@ -130,79 +130,83 @@
                 defaults = defaults or dep.uses_default_features
                 additional_features = dep.features
             workarounds[name] = (set.union(other_features, additional_features), defaults)
 
     # collect dependencies taking into account which features are enabled
     brs = set()
 
+    # minimum supported Rust version
+    if msrv := package.rust_version:
+        brs.add(f"rust >= {msrv}")
+
     # normal dependencies
-    for (name, dep) in normal.items():
-        if dep.path:
+    for name, dep in normal.items():
+        if dep.is_path_or_git():
             continue
 
         if deps_default_features[name]:
             brs.add(dep.to_rpm("default"))
         else:
             brs.add(dep.to_rpm(None))
         for feature in deps_enabled_features[name]:
             brs.add(dep.to_rpm(feature))
 
     # optional normal dependencies
-    for (name, dep) in normal_optional.items():
-        if dep.path:
+    for name, dep in normal_optional.items():
+        if dep.is_path_or_git():
             continue
 
         if name in optional_enabled:
             if deps_default_features[name]:
                 brs.add(dep.to_rpm("default"))
             else:
                 brs.add(dep.to_rpm(None))
             for feature in deps_enabled_features[name]:
                 brs.add(dep.to_rpm(feature))
 
     # build-dependencies
-    for (name, dep) in build.items():
-        if dep.path:
+    for name, dep in build.items():
+        if dep.is_path_or_git():
             continue
 
         if deps_default_features[name]:
             brs.add(dep.to_rpm("default"))
         else:
             brs.add(dep.to_rpm(None))
         for feature in deps_enabled_features[name]:
             brs.add(dep.to_rpm(feature))
 
     # optional build-dependencies
-    for (name, dep) in build_optional.items():
-        if dep.path:
+    for name, dep in build_optional.items():
+        if dep.is_path_or_git():
             continue
 
         if name in optional_enabled:
             if deps_default_features[name]:
                 brs.add(dep.to_rpm("default"))
             else:
                 brs.add(dep.to_rpm(None))
             for feature in deps_enabled_features[name]:
                 brs.add(dep.to_rpm(feature))
 
     # dev-dependencies
     if with_dev_deps:
-        for (name, dep) in dev.items():
-            if dep.path:
+        for name, dep in dev.items():
+            if dep.is_path_or_git():
                 continue
 
             if deps_default_features[name]:
                 brs.add(dep.to_rpm("default"))
             else:
                 brs.add(dep.to_rpm(None))
             for feature in deps_enabled_features[name]:
                 brs.add(dep.to_rpm(feature))
 
     # workarounds
-    for (name, (features, defaults)) in workarounds.items():
+    for name, (features, defaults) in workarounds.items():
         if dep := normal_optional.get(name):
             if defaults:
                 brs.add(dep.to_rpm("default"))
             else:
                 brs.add(dep.to_rpm(None))
             for feature in features:
                 brs.add(dep.to_rpm(feature))
@@ -274,14 +278,18 @@
     build = package.get_build_dependencies(False)
 
     deps = set()
 
     # dependency on cargo is mandatory
     deps.add("cargo")
 
+    # minimum supported Rust version
+    if msrv := package.rust_version:
+        deps.add(f"rust >= {msrv}")
+
     # normal dependencies
     for dep in normal.values():
         if dep.uses_default_features:
             deps.add(dep.to_rpm("default"))
         else:
             deps.add(dep.to_rpm(None))
         for depf in dep.features:
```

### Comparing `cargo2rpm-0.1.8/cargo2rpm/semver.py` & `cargo2rpm-0.1.9/cargo2rpm/semver.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         """
         Algorithm for determining precedence between pre-releases based on the semver.org spec.
         """
 
         if not isinstance(other, PreRelease):
             return False  # pragma nocover
 
-        for (lpart, rpart) in itertools.zip_longest(self.parts, other.parts):
+        for lpart, rpart in itertools.zip_longest(self.parts, other.parts):
             match lpart, rpart:
                 # all previous parts were equal and the left pre-release has more parts
                 case l, None:
                     return False
 
                 # all previous parts were equal and the right pre-release has more parts
                 case None, r:
```

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/ahash-0.8.3.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/ahash-0.8.3.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/aho-corasick-1.0.2.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/aho-corasick-1.0.2.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/assert_cmd-2.0.8.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/assert_cmd-2.0.8.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/assert_fs-1.0.10.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/assert_fs-1.0.10.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/autocfg-1.1.0.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/autocfg-1.1.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/bstr-1.2.0.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/bstr-1.2.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/cfg-if-1.0.0.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/cfg-if-1.0.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/clap-4.1.4.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/clap-4.1.4.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/gstreamer-0.19.7.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/gstreamer-0.19.7.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/human-panic-1.1.0.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/human-panic-1.1.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/hyperfine-1.15.0.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/hyperfine-1.15.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/iri-string-0.7.0.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/iri-string-0.7.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/libblkio-1.2.2.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/libblkio-1.2.2.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/libc-0.2.139.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/libc-0.2.139.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/predicates-2.1.5.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/predicates-2.1.5.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/proc-macro2-1.0.50.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/proc-macro2-1.0.50.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/quote-1.0.23.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/quote-1.0.23.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/rand-0.8.5.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/rand-0.8.5.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/rand_core-0.6.4.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/rand_core-0.6.4.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/regex-1.8.4.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/regex-1.8.4.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/regex-syntax-0.7.2.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/regex-syntax-0.7.2.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/rpm-sequoia-1.2.0.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/rpm-sequoia-1.2.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/rust_decimal-1.28.0.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/rust_decimal-1.28.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/rustix-0.36.8.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/rustix-0.36.8.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/serde-1.0.152.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/serde-1.0.152.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/serde_derive-1.0.152.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/serde_derive-1.0.152.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/syn-1.0.107.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/syn-1.0.107.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/time-0.3.17.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/time-0.3.17.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/tokio-1.25.0.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/tokio-1.25.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/unicode-xid-0.2.4.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/unicode-xid-0.2.4.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/zbus-3.8.0.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/zbus-3.8.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/zola-0.16.1.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/zola-0.16.1.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/testdata/zoxide-0.9.0.json` & `cargo2rpm-0.1.9/cargo2rpm/testdata/zoxide-0.9.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/metadata/test_deps.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/metadata/test_deps.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/metadata/test_description.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/metadata/test_description.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/metadata/test_feature_closure.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/metadata/test_feature_closure.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/metadata/test_package.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/metadata/test_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         "aho-corasick-1.0.2.json",
         "assert_cmd-2.0.8.json",
         "assert_fs-1.0.10.json",
         "autocfg-1.1.0.json",
         "bstr-1.2.0.json",
         "cfg-if-1.0.0.json",
         "clap-4.1.4.json",
+        "espanso-2.1.8.json",
         "fapolicy-analyzer-0.6.8.json",
         "gstreamer-0.19.7.json",
         "human-panic-1.1.0.json",
         "hyperfine-1.15.0.json",
         "iri-string-0.7.0.json",
         "libblkio-1.2.2.json",
         "libc-0.2.139.json",
@@ -58,14 +59,15 @@
         ("aho-corasick-1.0.2.json", False),
         ("assert_cmd-2.0.8.json", True),
         ("assert_fs-1.0.10.json", False),
         ("autocfg-1.1.0.json", False),
         ("bstr-1.2.0.json", False),
         ("cfg-if-1.0.0.json", False),
         ("clap-4.1.4.json", True),
+        ("espanso-2.1.8.json", True),
         ("fapolicy-analyzer-0.6.8.json", True),
         ("gstreamer-0.19.7.json", False),
         ("human-panic-1.1.0.json", False),
         ("hyperfine-1.15.0.json", True),
         ("iri-string-0.7.0.json", False),
         ("libblkio-1.2.2.json", False),
         ("libc-0.2.139.json", False),
@@ -103,14 +105,15 @@
         ("aho-corasick-1.0.2.json", True),
         ("assert_cmd-2.0.8.json", True),
         ("assert_fs-1.0.10.json", True),
         ("autocfg-1.1.0.json", True),
         ("bstr-1.2.0.json", True),
         ("cfg-if-1.0.0.json", True),
         ("clap-4.1.4.json", True),
+        ("espanso-2.1.8.json", False),
         ("fapolicy-analyzer-0.6.8.json", False),
         ("gstreamer-0.19.7.json", True),
         ("human-panic-1.1.0.json", True),
         ("hyperfine-1.15.0.json", False),
         ("iri-string-0.7.0.json", True),
         ("libblkio-1.2.2.json", False),
         ("libc-0.2.139.json", True),
@@ -148,14 +151,15 @@
         ("aho-corasick-1.0.2.json", False),
         ("assert_cmd-2.0.8.json", False),
         ("assert_fs-1.0.10.json", False),
         ("autocfg-1.1.0.json", False),
         ("bstr-1.2.0.json", False),
         ("cfg-if-1.0.0.json", False),
         ("clap-4.1.4.json", False),
+        ("espanso-2.1.8.json", True),
         ("fapolicy-analyzer-0.6.8.json", True),
         ("gstreamer-0.19.7.json", False),
         ("human-panic-1.1.0.json", False),
         ("hyperfine-1.15.0.json", False),
         ("iri-string-0.7.0.json", False),
         ("libblkio-1.2.2.json", True),
         ("libc-0.2.139.json", False),
@@ -193,14 +197,15 @@
         ("aho-corasick-1.0.2.json", set()),
         ("assert_cmd-2.0.8.json", {"bin_fixture"}),
         ("assert_fs-1.0.10.json", set()),
         ("autocfg-1.1.0.json", set()),
         ("bstr-1.2.0.json", set()),
         ("cfg-if-1.0.0.json", set()),
         ("clap-4.1.4.json", {"stdio-fixture"}),
+        ("espanso-2.1.8.json", {"espanso"}),
         ("fapolicy-analyzer-0.6.8.json", {"tdb", "rulec"}),
         ("gstreamer-0.19.7.json", set()),
         ("human-panic-1.1.0.json", set()),
         ("hyperfine-1.15.0.json", {"hyperfine"}),
         ("iri-string-0.7.0.json", set()),
         ("libblkio-1.2.2.json", set()),
         ("libc-0.2.139.json", set()),
```

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/rpm/test_buildrequires.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/rpm/test_buildrequires.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,33 +49,36 @@
         ),
         # default features with dev-dependencies
         (
             "aho-corasick-1.0.2.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.60.0",
                 "(crate(doc-comment/default) >= 0.3.3 with crate(doc-comment/default) < 0.4.0~)",
                 "(crate(memchr) >= 2.4.0 with crate(memchr) < 3.0.0~)",
             }.union({"(crate(memchr/std) >= 2.4.0 with crate(memchr/std) < 3.0.0~)"} if CARGO_BUGGY_RESOLVER else set()),
         ),
         # default features without dev-dependencies
         (
             "aho-corasick-1.0.2.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.60.0",
                 "(crate(memchr) >= 2.4.0 with crate(memchr) < 3.0.0~)",
             }.union({"(crate(memchr/std) >= 2.4.0 with crate(memchr/std) < 3.0.0~)"} if CARGO_BUGGY_RESOLVER else set()),
         ),
         # default features with dev-dependencies
         (
             "assert_cmd-2.0.8.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.60.0",
                 "(crate(bstr/default) >= 1.0.1 with crate(bstr/default) < 2.0.0~)",
                 "(crate(doc-comment/default) >= 0.3.0 with crate(doc-comment/default) < 0.4.0~)",
                 "(crate(predicates) >= 2.1.0 with crate(predicates) < 3.0.0~)",
                 "(crate(predicates/diff) >= 2.1.0 with crate(predicates/diff) < 3.0.0~)",
                 "(crate(predicates-core/default) >= 1.0.0 with crate(predicates-core/default) < 2.0.0~)",
                 "(crate(predicates-tree/default) >= 1.0.0 with crate(predicates-tree/default) < 2.0.0~)",
                 "(crate(wait-timeout/default) >= 0.2.0 with crate(wait-timeout/default) < 0.3.0~)",
@@ -84,14 +87,15 @@
         ),
         # default features without dev-dependencies
         (
             "assert_cmd-2.0.8.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.60.0",
                 "(crate(bstr/default) >= 1.0.1 with crate(bstr/default) < 2.0.0~)",
                 "(crate(doc-comment/default) >= 0.3.0 with crate(doc-comment/default) < 0.4.0~)",
                 "(crate(predicates) >= 2.1.0 with crate(predicates) < 3.0.0~)",
                 "(crate(predicates/diff) >= 2.1.0 with crate(predicates/diff) < 3.0.0~)",
                 "(crate(predicates-core/default) >= 1.0.0 with crate(predicates-core/default) < 2.0.0~)",
                 "(crate(predicates-tree/default) >= 1.0.0 with crate(predicates-tree/default) < 2.0.0~)",
                 "(crate(wait-timeout/default) >= 0.2.0 with crate(wait-timeout/default) < 0.3.0~)",
@@ -99,14 +103,15 @@
         ),
         # default features with dev-dependencies
         (
             "assert_fs-1.0.10.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.60.0",
                 "(crate(doc-comment/default) >= 0.3.0 with crate(doc-comment/default) < 0.4.0~)",
                 "(crate(globwalk/default) >= 0.8.0 with crate(globwalk/default) < 0.9.0~)",
                 "(crate(predicates) >= 2.0.3 with crate(predicates) < 3.0.0~)",
                 "(crate(predicates/diff) >= 2.0.3 with crate(predicates/diff) < 3.0.0~)",
                 "(crate(predicates-core/default) >= 1.0.0 with crate(predicates-core/default) < 2.0.0~)",
                 "(crate(predicates-tree/default) >= 1.0.0 with crate(predicates-tree/default) < 2.0.0~)",
                 "(crate(tempfile/default) >= 3.0.0 with crate(tempfile/default) < 4.0.0~)",
@@ -114,14 +119,15 @@
         ),
         # default features without dev-dependencies
         (
             "assert_fs-1.0.10.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.60.0",
                 "(crate(doc-comment/default) >= 0.3.0 with crate(doc-comment/default) < 0.4.0~)",
                 "(crate(globwalk/default) >= 0.8.0 with crate(globwalk/default) < 0.9.0~)",
                 "(crate(predicates) >= 2.0.3 with crate(predicates) < 3.0.0~)",
                 "(crate(predicates/diff) >= 2.0.3 with crate(predicates/diff) < 3.0.0~)",
                 "(crate(predicates-core/default) >= 1.0.0 with crate(predicates-core/default) < 2.0.0~)",
                 "(crate(predicates-tree/default) >= 1.0.0 with crate(predicates-tree/default) < 2.0.0~)",
                 "(crate(tempfile/default) >= 3.0.0 with crate(tempfile/default) < 4.0.0~)",
@@ -143,14 +149,15 @@
         ),
         # default features with dev-dependencies
         (
             "bstr-1.2.0.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.60",
                 "(crate(memchr) >= 2.4.0 with crate(memchr) < 3.0.0~)",
                 "(crate(memchr/std) >= 2.4.0 with crate(memchr/std) < 3.0.0~)",
                 "(crate(once_cell/default) >= 1.14.0 with crate(once_cell/default) < 2.0.0~)",
                 "(crate(regex-automata) >= 0.1.5 with crate(regex-automata) < 0.2.0~)",
                 "(crate(quickcheck) >= 1.0.0 with crate(quickcheck) < 2.0.0~)",
                 "(crate(ucd-parse/default) >= 0.1.3 with crate(ucd-parse/default) < 0.2.0~)",
                 "(crate(unicode-segmentation/default) >= 1.2.1 with crate(unicode-segmentation/default) < 2.0.0~)",
@@ -166,14 +173,15 @@
         ),
         # default features without dev-dependencies
         (
             "bstr-1.2.0.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.60",
                 "(crate(memchr) >= 2.4.0 with crate(memchr) < 3.0.0~)",
                 "(crate(memchr/std) >= 2.4.0 with crate(memchr/std) < 3.0.0~)",
                 "(crate(once_cell/default) >= 1.14.0 with crate(once_cell/default) < 2.0.0~)",
                 "(crate(regex-automata) >= 0.1.5 with crate(regex-automata) < 0.2.0~)",
             }.union(
                 {
                     "(crate(serde) >= 1.0.85 with crate(serde) < 2.0.0~)",
@@ -200,14 +208,15 @@
         ),
         # default features with dev-dependencies
         (
             "clap-4.1.4.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.64.0",
                 "(crate(bitflags/default) >= 1.2.0 with crate(bitflags/default) < 2.0.0~)",
                 "(crate(clap_lex/default) >= 0.3.0 with crate(clap_lex/default) < 0.4.0~)",
                 "(crate(is-terminal/default) >= 0.4.1 with crate(is-terminal/default) < 0.5.0~)",
                 "(crate(strsim/default) >= 0.10.0 with crate(strsim/default) < 0.11.0~)",
                 "(crate(termcolor/default) >= 1.1.1 with crate(termcolor/default) < 2.0.0~)",
                 "(crate(humantime/default) >= 2.0.0 with crate(humantime/default) < 3.0.0~)",
                 "(crate(rustversion/default) >= 1.0.0 with crate(rustversion/default) < 2.0.0~)",
@@ -224,27 +233,29 @@
         ),
         # default features without dev-dependencies
         (
             "clap-4.1.4.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.64.0",
                 "(crate(bitflags/default) >= 1.2.0 with crate(bitflags/default) < 2.0.0~)",
                 "(crate(clap_lex/default) >= 0.3.0 with crate(clap_lex/default) < 0.4.0~)",
                 "(crate(is-terminal/default) >= 0.4.1 with crate(is-terminal/default) < 0.5.0~)",
                 "(crate(strsim/default) >= 0.10.0 with crate(strsim/default) < 0.11.0~)",
                 "(crate(termcolor/default) >= 1.1.1 with crate(termcolor/default) < 2.0.0~)",
             },
         ),
         # default features with dev-dependencies
         (
             "gstreamer-0.19.7.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.63",
                 "(crate(bitflags/default) >= 1.0.0 with crate(bitflags/default) < 2.0.0~)",
                 "(crate(cfg-if/default) >= 1.0.0 with crate(cfg-if/default) < 2.0.0~)",
                 "(crate(gstreamer-sys/default) >= 0.19.0 with crate(gstreamer-sys/default) < 0.20.0~)",
                 "(crate(futures-channel/default) >= 0.3.0 with crate(futures-channel/default) < 0.4.0~)",
                 "(crate(futures-core/default) >= 0.3.0 with crate(futures-core/default) < 0.4.0~)",
                 "(crate(futures-util) >= 0.3.0 with crate(futures-util) < 0.4.0~)",
                 "(crate(glib/default) >= 0.16.2 with crate(glib/default) < 0.17.0~)",
@@ -265,14 +276,15 @@
         ),
         # default features without dev-dependencies
         (
             "gstreamer-0.19.7.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.63",
                 "(crate(bitflags/default) >= 1.0.0 with crate(bitflags/default) < 2.0.0~)",
                 "(crate(cfg-if/default) >= 1.0.0 with crate(cfg-if/default) < 2.0.0~)",
                 "(crate(gstreamer-sys/default) >= 0.19.0 with crate(gstreamer-sys/default) < 0.20.0~)",
                 "(crate(futures-channel/default) >= 0.3.0 with crate(futures-channel/default) < 0.4.0~)",
                 "(crate(futures-core/default) >= 0.3.0 with crate(futures-core/default) < 0.4.0~)",
                 "(crate(futures-util) >= 0.3.0 with crate(futures-util) < 0.4.0~)",
                 "(crate(glib/default) >= 0.16.2 with crate(glib/default) < 0.17.0~)",
@@ -289,14 +301,15 @@
         ),
         # default features with dev-dependencies
         (
             "human-panic-1.1.0.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.60.0",
                 "(crate(backtrace/default) >= 0.3.9 with crate(backtrace/default) < 0.4.0~)",
                 "crate(concolor/default) = 0.0.11",
                 "crate(concolor/auto) = 0.0.11",
                 "(crate(os_info/default) >= 2.0.6 with crate(os_info/default) < 3.0.0~)",
                 "(crate(serde/default) >= 1.0.79 with crate(serde/default) < 2.0.0~)",
                 "(crate(serde_derive/default) >= 1.0.79 with crate(serde_derive/default) < 2.0.0~)",
                 "(crate(termcolor/default) >= 1.0.4 with crate(termcolor/default) < 2.0.0~)",
@@ -307,14 +320,15 @@
         ),
         # default features without dev-dependencies
         (
             "human-panic-1.1.0.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.60.0",
                 "(crate(backtrace/default) >= 0.3.9 with crate(backtrace/default) < 0.4.0~)",
                 "crate(concolor/default) = 0.0.11",
                 "crate(concolor/auto) = 0.0.11",
                 "(crate(os_info/default) >= 2.0.6 with crate(os_info/default) < 3.0.0~)",
                 "(crate(serde/default) >= 1.0.79 with crate(serde/default) < 2.0.0~)",
                 "(crate(serde_derive/default) >= 1.0.79 with crate(serde_derive/default) < 2.0.0~)",
                 "(crate(termcolor/default) >= 1.0.4 with crate(termcolor/default) < 2.0.0~)",
@@ -324,53 +338,59 @@
             },
         ),
         # default features with dev-dependencies
         (
             "iri-string-0.7.0.json",
             FeatureFlags(),
             True,
-            {"(crate(serde_test/default) >= 1.0.104 with crate(serde_test/default) < 2.0.0~)"}.union(
+            {
+                "rust >= 1.60",
+                "(crate(serde_test/default) >= 1.0.104 with crate(serde_test/default) < 2.0.0~)",
+            }.union(
                 {
                     "(crate(memchr) >= 2.4.1 with crate(memchr) < 3.0.0~)",
                     "(crate(memchr/std) >= 2.4.1 with crate(memchr/std) < 3.0.0~)",
                     "(crate(serde) >= 1.0.103 with crate(serde) < 2.0.0~)",
                     "(crate(serde/alloc) >= 1.0.103 with crate(serde/alloc) < 2.0.0~)",
                     "(crate(serde/derive) >= 1.0.103 with crate(serde/derive) < 2.0.0~)",
                     "(crate(serde/std) >= 1.0.103 with crate(serde/std) < 2.0.0~)",
                 }
                 if CARGO_BUGGY_RESOLVER
-                else set()
+                else set(),
             ),
         ),
         # default features without dev-dependencies
         (
             "iri-string-0.7.0.json",
             FeatureFlags(),
             False,
-            {
-                "(crate(memchr) >= 2.4.1 with crate(memchr) < 3.0.0~)",
-                "(crate(memchr/std) >= 2.4.1 with crate(memchr/std) < 3.0.0~)",
-                "(crate(serde) >= 1.0.103 with crate(serde) < 2.0.0~)",
-                "(crate(serde/alloc) >= 1.0.103 with crate(serde/alloc) < 2.0.0~)",
-                "(crate(serde/derive) >= 1.0.103 with crate(serde/derive) < 2.0.0~)",
-                "(crate(serde/std) >= 1.0.103 with crate(serde/std) < 2.0.0~)",
-            }
-            if CARGO_BUGGY_RESOLVER
-            else set(),
+            {"rust >= 1.60"}.union(
+                {
+                    "(crate(memchr) >= 2.4.1 with crate(memchr) < 3.0.0~)",
+                    "(crate(memchr/std) >= 2.4.1 with crate(memchr/std) < 3.0.0~)",
+                    "(crate(serde) >= 1.0.103 with crate(serde) < 2.0.0~)",
+                    "(crate(serde/alloc) >= 1.0.103 with crate(serde/alloc) < 2.0.0~)",
+                    "(crate(serde/derive) >= 1.0.103 with crate(serde/derive) < 2.0.0~)",
+                    "(crate(serde/std) >= 1.0.103 with crate(serde/std) < 2.0.0~)",
+                }
+                if CARGO_BUGGY_RESOLVER
+                else set()
+            ),
         ),
         # default features with dev-dependencies
         ("libc-0.2.139.json", FeatureFlags(), True, set()),
         # default features without dev-dependencies
         ("libc-0.2.139.json", FeatureFlags(), False, set()),
         # default features with dev-dependencies
         (
             "predicates-2.1.5.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.60.0",
                 "(crate(difflib/default) >= 0.4.0 with crate(difflib/default) < 0.5.0~)",
                 "(crate(float-cmp/default) >= 0.9.0 with crate(float-cmp/default) < 0.10.0~)",
                 "(crate(itertools/default) >= 0.10.0 with crate(itertools/default) < 0.11.0~)",
                 "(crate(normalize-line-endings/default) >= 0.3.0 with crate(normalize-line-endings/default) < 0.4.0~)",
                 "(crate(predicates-core/default) >= 1.0.0 with crate(predicates-core/default) < 2.0.0~)",
                 "(crate(regex/default) >= 1.0.0 with crate(regex/default) < 2.0.0~)",
                 "(crate(predicates-tree/default) >= 1.0.0 with crate(predicates-tree/default) < 2.0.0~)",
@@ -378,58 +398,65 @@
         ),
         # default features without dev-dependencies
         (
             "predicates-2.1.5.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.60.0",
                 "(crate(difflib/default) >= 0.4.0 with crate(difflib/default) < 0.5.0~)",
                 "(crate(float-cmp/default) >= 0.9.0 with crate(float-cmp/default) < 0.10.0~)",
                 "(crate(itertools/default) >= 0.10.0 with crate(itertools/default) < 0.11.0~)",
                 "(crate(normalize-line-endings/default) >= 0.3.0 with crate(normalize-line-endings/default) < 0.4.0~)",
                 "(crate(predicates-core/default) >= 1.0.0 with crate(predicates-core/default) < 2.0.0~)",
                 "(crate(regex/default) >= 1.0.0 with crate(regex/default) < 2.0.0~)",
             },
         ),
         # default features with dev-dependencies
         (
             "proc-macro2-1.0.50.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.31",
                 "(crate(unicode-ident/default) >= 1.0.0 with crate(unicode-ident/default) < 2.0.0~)",
                 "(crate(quote) >= 1.0.0 with crate(quote) < 2.0.0~)",
             },
         ),
         # default features without dev-dependencies
         (
             "proc-macro2-1.0.50.json",
             FeatureFlags(),
             False,
-            {"(crate(unicode-ident/default) >= 1.0.0 with crate(unicode-ident/default) < 2.0.0~)"},
+            {
+                "rust >= 1.31",
+                "(crate(unicode-ident/default) >= 1.0.0 with crate(unicode-ident/default) < 2.0.0~)",
+            },
         ),
         # default features with dev-dependencies
         (
             "quote-1.0.23.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.31",
                 "(crate(proc-macro2) >= 1.0.40 with crate(proc-macro2) < 2.0.0~)",
                 "(crate(proc-macro2/proc-macro) >= 1.0.40 with crate(proc-macro2/proc-macro) < 2.0.0~)",
                 "(crate(rustversion/default) >= 1.0.0 with crate(rustversion/default) < 2.0.0~)",
                 "(crate(trybuild/default) >= 1.0.66 with crate(trybuild/default) < 2.0.0~)",
                 "(crate(trybuild/diff) >= 1.0.66 with crate(trybuild/diff) < 2.0.0~)",
             },
         ),
         # default features without dev-dependencies
         (
             "quote-1.0.23.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.31",
                 "(crate(proc-macro2) >= 1.0.40 with crate(proc-macro2) < 2.0.0~)",
                 "(crate(proc-macro2/proc-macro) >= 1.0.40 with crate(proc-macro2/proc-macro) < 2.0.0~)",
             },
         ),
         # default features with dev-dependencies
         (
             "rand-0.8.5.json",
@@ -468,14 +495,15 @@
         ("rand_core-0.6.4.json", FeatureFlags(), False, set()),
         # default features with dev-dependencies
         (
             "regex-1.8.4.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.60.0",
                 "(crate(aho-corasick/default) >= 1.0.0 with crate(aho-corasick/default) < 2.0.0~)",
                 "(crate(memchr/default) >= 2.5.0 with crate(memchr/default) < 3.0.0~)",
                 "(crate(regex-syntax/default) >= 0.7.2 with crate(regex-syntax/default) < 0.8.0~)",
                 "(crate(regex-syntax/unicode) >= 0.7.2 with crate(regex-syntax/unicode) < 0.8.0~)",
                 "(crate(regex-syntax/unicode-age) >= 0.7.2 with crate(regex-syntax/unicode-age) < 0.8.0~)",
                 "(crate(regex-syntax/unicode-bool) >= 0.7.2 with crate(regex-syntax/unicode-bool) < 0.8.0~)",
                 "(crate(regex-syntax/unicode-case) >= 0.7.2 with crate(regex-syntax/unicode-case) < 0.8.0~)",
@@ -492,37 +520,39 @@
         ),
         # default features without dev-dependencies
         (
             "regex-1.8.4.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.60.0",
                 "(crate(aho-corasick/default) >= 1.0.0 with crate(aho-corasick/default) < 2.0.0~)",
                 "(crate(memchr/default) >= 2.5.0 with crate(memchr/default) < 3.0.0~)",
                 "(crate(regex-syntax/default) >= 0.7.2 with crate(regex-syntax/default) < 0.8.0~)",
                 "(crate(regex-syntax/unicode) >= 0.7.2 with crate(regex-syntax/unicode) < 0.8.0~)",
                 "(crate(regex-syntax/unicode-age) >= 0.7.2 with crate(regex-syntax/unicode-age) < 0.8.0~)",
                 "(crate(regex-syntax/unicode-bool) >= 0.7.2 with crate(regex-syntax/unicode-bool) < 0.8.0~)",
                 "(crate(regex-syntax/unicode-case) >= 0.7.2 with crate(regex-syntax/unicode-case) < 0.8.0~)",
                 "(crate(regex-syntax/unicode-gencat) >= 0.7.2 with crate(regex-syntax/unicode-gencat) < 0.8.0~)",
                 "(crate(regex-syntax/unicode-perl) >= 0.7.2 with crate(regex-syntax/unicode-perl) < 0.8.0~)",
                 "(crate(regex-syntax/unicode-script) >= 0.7.2 with crate(regex-syntax/unicode-script) < 0.8.0~)",
                 "(crate(regex-syntax/unicode-segment) >= 0.7.2 with crate(regex-syntax/unicode-segment) < 0.8.0~)",
             },
         ),
         # default features with dev-dependencies
-        ("regex-syntax-0.7.2.json", FeatureFlags(), True, set()),
+        ("regex-syntax-0.7.2.json", FeatureFlags(), True, {"rust >= 1.60.0"}),
         # default features without dev-dependencies
-        ("regex-syntax-0.7.2.json", FeatureFlags(), False, set()),
+        ("regex-syntax-0.7.2.json", FeatureFlags(), False, {"rust >= 1.60.0"}),
         # default features with dev-dependencies
         (
             "rpm-sequoia-1.2.0.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.60",
                 "(crate(anyhow/default) >= 1.0.0 with crate(anyhow/default) < 2.0.0~)",
                 "(crate(buffered-reader) >= 1.0.0 with crate(buffered-reader) < 2.0.0~)",
                 "(crate(chrono) >= 0.4.0 with crate(chrono) < 0.5.0~)",
                 "(crate(chrono/std) >= 0.4.0 with crate(chrono/std) < 0.5.0~)",
                 "(crate(lazy_static/default) >= 1.0.0 with crate(lazy_static/default) < 2.0.0~)",
                 "(crate(libc/default) >= 0.2.0 with crate(libc/default) < 0.3.0~)",
                 "(crate(sequoia-openpgp) >= 1.11.0 with crate(sequoia-openpgp) < 2.0.0~)",
@@ -535,14 +565,15 @@
         ),
         # default features without dev-dependencies
         (
             "rpm-sequoia-1.2.0.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.60",
                 "(crate(anyhow/default) >= 1.0.0 with crate(anyhow/default) < 2.0.0~)",
                 "(crate(buffered-reader) >= 1.0.0 with crate(buffered-reader) < 2.0.0~)",
                 "(crate(chrono) >= 0.4.0 with crate(chrono) < 0.5.0~)",
                 "(crate(chrono/std) >= 0.4.0 with crate(chrono/std) < 0.5.0~)",
                 "(crate(lazy_static/default) >= 1.0.0 with crate(lazy_static/default) < 2.0.0~)",
                 "(crate(libc/default) >= 0.2.0 with crate(libc/default) < 0.3.0~)",
                 "(crate(sequoia-openpgp) >= 1.11.0 with crate(sequoia-openpgp) < 2.0.0~)",
@@ -554,14 +585,15 @@
         ),
         # default features with dev-dependencies
         (
             "rust_decimal-1.28.0.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.60",
                 "(crate(arrayvec) >= 0.7.0 with crate(arrayvec) < 0.8.0~)",
                 "(crate(arrayvec/std) >= 0.7.0 with crate(arrayvec/std) < 0.8.0~)",
                 "(crate(num-traits) >= 0.2.0 with crate(num-traits) < 0.3.0~)",
                 "(crate(num-traits/i128) >= 0.2.0 with crate(num-traits/i128) < 0.3.0~)",
                 "(crate(serde) >= 1.0.0 with crate(serde) < 2.0.0~)",
                 "(crate(serde/derive) >= 1.0.0 with crate(serde/derive) < 2.0.0~)",
                 "(crate(serde/std) >= 1.0.0 with crate(serde/std) < 2.0.0~)",
@@ -601,14 +633,15 @@
         ),
         # default features without dev-dependencies
         (
             "rust_decimal-1.28.0.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.60",
                 "(crate(arrayvec) >= 0.7.0 with crate(arrayvec) < 0.8.0~)",
                 "(crate(arrayvec/std) >= 0.7.0 with crate(arrayvec/std) < 0.8.0~)",
                 "(crate(num-traits) >= 0.2.0 with crate(num-traits) < 0.3.0~)",
                 "(crate(num-traits/i128) >= 0.2.0 with crate(num-traits/i128) < 0.3.0~)",
                 "(crate(serde) >= 1.0.0 with crate(serde) < 2.0.0~)",
                 "(crate(serde/std) >= 1.0.0 with crate(serde/std) < 2.0.0~)",
             }.union(
@@ -635,14 +668,15 @@
         ),
         # default features with dev-dependencies
         (
             "rustix-0.36.8.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.48",
                 "(crate(bitflags/default) >= 1.2.1 with crate(bitflags/default) < 2.0.0~)",
                 "(crate(io-lifetimes) >= 1.0.0 with crate(io-lifetimes) < 2.0.0~)",
                 "(crate(io-lifetimes/close) >= 1.0.0 with crate(io-lifetimes/close) < 2.0.0~)",
                 "(crate(flate2/default) >= 1.0.0 with crate(flate2/default) < 2.0.0~)",
                 "(crate(libc/default) >= 0.2.133 with crate(libc/default) < 0.3.0~)",
                 "(crate(errno) >= 0.2.8 with crate(errno) < 0.3.0~)",
                 "(crate(memoffset/default) >= 0.7.1 with crate(memoffset/default) < 0.8.0~)",
@@ -665,14 +699,15 @@
         ),
         # default features + cc with dev-dependencies
         (
             "rustix-0.36.8.json",
             FeatureFlags(features=["cc"]),
             True,
             {
+                "rust >= 1.48",
                 "(crate(bitflags/default) >= 1.2.1 with crate(bitflags/default) < 2.0.0~)",
                 "(crate(io-lifetimes) >= 1.0.0 with crate(io-lifetimes) < 2.0.0~)",
                 "(crate(io-lifetimes/close) >= 1.0.0 with crate(io-lifetimes/close) < 2.0.0~)",
                 "(crate(flate2/default) >= 1.0.0 with crate(flate2/default) < 2.0.0~)",
                 "(crate(libc/default) >= 0.2.133 with crate(libc/default) < 0.3.0~)",
                 "(crate(errno) >= 0.2.8 with crate(errno) < 0.3.0~)",
                 "(crate(memoffset/default) >= 0.7.1 with crate(memoffset/default) < 0.8.0~)",
@@ -696,14 +731,15 @@
         ),
         # default features without dev-dependencies
         (
             "rustix-0.36.8.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.48",
                 "(crate(bitflags/default) >= 1.2.1 with crate(bitflags/default) < 2.0.0~)",
                 "(crate(io-lifetimes) >= 1.0.0 with crate(io-lifetimes) < 2.0.0~)",
                 "(crate(io-lifetimes/close) >= 1.0.0 with crate(io-lifetimes/close) < 2.0.0~)",
                 "(crate(libc/default) >= 0.2.133 with crate(libc/default) < 0.3.0~)",
                 "(crate(errno) >= 0.2.8 with crate(errno) < 0.3.0~)",
                 "(crate(linux-raw-sys) >= 0.1.2 with crate(linux-raw-sys) < 0.2.0~)",
                 "(crate(linux-raw-sys/general) >= 0.1.2 with crate(linux-raw-sys/general) < 0.2.0~)",
@@ -720,14 +756,15 @@
         ),
         # default features + cc without dev-dependencies
         (
             "rustix-0.36.8.json",
             FeatureFlags(features=["cc"]),
             False,
             {
+                "rust >= 1.48",
                 "(crate(bitflags/default) >= 1.2.1 with crate(bitflags/default) < 2.0.0~)",
                 "(crate(io-lifetimes) >= 1.0.0 with crate(io-lifetimes) < 2.0.0~)",
                 "(crate(io-lifetimes/close) >= 1.0.0 with crate(io-lifetimes/close) < 2.0.0~)",
                 "(crate(libc/default) >= 0.2.133 with crate(libc/default) < 0.3.0~)",
                 "(crate(errno) >= 0.2.8 with crate(errno) < 0.3.0~)",
                 "(crate(cc/default) >= 1.0.68 with crate(cc/default) < 2.0.0~)",
                 "(crate(linux-raw-sys) >= 0.1.2 with crate(linux-raw-sys) < 0.2.0~)",
@@ -745,53 +782,57 @@
         ),
         # default features with dev-dependencies
         (
             "serde-1.0.152.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.13",
                 "(crate(serde_derive/default) >= 1.0.0 with crate(serde_derive/default) < 2.0.0~)",
             },
         ),
         # default features without dev-dependencies
         (
             "serde-1.0.152.json",
             FeatureFlags(),
             False,
-            set(),
+            {"rust >= 1.13"},
         ),
         # default features with dev-dependencies
         (
             "serde_derive-1.0.152.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.31",
                 "(crate(proc-macro2/default) >= 1.0.0 with crate(proc-macro2/default) < 2.0.0~)",
                 "(crate(quote/default) >= 1.0.0 with crate(quote/default) < 2.0.0~)",
                 "(crate(syn/default) >= 1.0.104 with crate(syn/default) < 2.0.0~)",
                 "(crate(serde/default) >= 1.0.0 with crate(serde/default) < 2.0.0~)",
             },
         ),
         # default features without dev-dependencies
         (
             "serde_derive-1.0.152.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.31",
                 "(crate(proc-macro2/default) >= 1.0.0 with crate(proc-macro2/default) < 2.0.0~)",
                 "(crate(quote/default) >= 1.0.0 with crate(quote/default) < 2.0.0~)",
                 "(crate(syn/default) >= 1.0.104 with crate(syn/default) < 2.0.0~)",
             },
         ),
         # default features with dev-dependencies
         (
             "syn-1.0.107.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.31",
                 "(crate(proc-macro2) >= 1.0.46 with crate(proc-macro2) < 2.0.0~)",
                 "(crate(proc-macro2/proc-macro) >= 1.0.46 with crate(proc-macro2/proc-macro) < 2.0.0~)",
                 "(crate(quote) >= 1.0.0 with crate(quote) < 2.0.0~)",
                 "(crate(quote/proc-macro) >= 1.0.0 with crate(quote/proc-macro) < 2.0.0~)",
                 "(crate(unicode-ident/default) >= 1.0.0 with crate(unicode-ident/default) < 2.0.0~)",
                 "(crate(anyhow/default) >= 1.0.0 with crate(anyhow/default) < 2.0.0~)",
                 "(crate(automod/default) >= 1.0.0 with crate(automod/default) < 2.0.0~)",
@@ -810,27 +851,29 @@
         ),
         # default features without dev-dependencies
         (
             "syn-1.0.107.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.31",
                 "(crate(proc-macro2) >= 1.0.46 with crate(proc-macro2) < 2.0.0~)",
                 "(crate(proc-macro2/proc-macro) >= 1.0.46 with crate(proc-macro2/proc-macro) < 2.0.0~)",
                 "(crate(quote) >= 1.0.0 with crate(quote) < 2.0.0~)",
                 "(crate(quote/proc-macro) >= 1.0.0 with crate(quote/proc-macro) < 2.0.0~)",
                 "(crate(unicode-ident/default) >= 1.0.0 with crate(unicode-ident/default) < 2.0.0~)",
             },
         ),
         # default features with dev-dependencies
         (
             "time-0.3.17.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.60.0",
                 "crate(time-core/default) = 0.1.0",
                 "(crate(quickcheck_macros/default) >= 1.0.0 with crate(quickcheck_macros/default) < 2.0.0~)",
                 "(crate(rand) >= 0.8.4 with crate(rand) < 0.9.0~)",
                 "(crate(serde) >= 1.0.126 with crate(serde) < 2.0.0~)",
                 "(crate(serde/derive) >= 1.0.126 with crate(serde/derive) < 2.0.0~)",
                 "(crate(serde_json/default) >= 1.0.68 with crate(serde_json/default) < 2.0.0~)",
                 "(crate(serde_test/default) >= 1.0.126 with crate(serde_test/default) < 2.0.0~)",
@@ -840,29 +883,33 @@
             }.union({"(crate(serde/alloc) >= 1.0.126 with crate(serde/alloc) < 2.0.0~)"} if CARGO_BUGGY_RESOLVER else set()),
         ),
         # default features without dev-dependencies
         (
             "time-0.3.17.json",
             FeatureFlags(),
             False,
-            {"crate(time-core/default) = 0.1.0",}.union(
+            {
+                "rust >= 1.60.0",
+                "crate(time-core/default) = 0.1.0",
+            }.union(
                 {
                     "(crate(serde) >= 1.0.126 with crate(serde) < 2.0.0~)",
                     "(crate(serde/alloc) >= 1.0.126 with crate(serde/alloc) < 2.0.0~)",
                 }
                 if CARGO_BUGGY_RESOLVER
                 else set()
             ),
         ),
         # default features with dev-dependencies
         (
             "tokio-1.25.0.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.49",
                 "(crate(pin-project-lite/default) >= 0.2.0 with crate(pin-project-lite/default) < 0.3.0~)",
                 "(crate(async-stream/default) >= 0.3.0 with crate(async-stream/default) < 0.4.0~)",
                 "(crate(futures/default) >= 0.3.0 with crate(futures/default) < 0.4.0~)",
                 "(crate(futures/async-await) >= 0.3.0 with crate(futures/async-await) < 0.4.0~)",
                 "(crate(mockall/default) >= 0.11.1 with crate(mockall/default) < 0.12.0~)",
                 "(crate(tempfile/default) >= 3.1.0 with crate(tempfile/default) < 4.0.0~)",
                 "(crate(tokio-stream/default) >= 0.1.0 with crate(tokio-stream/default) < 0.2.0~)",
@@ -889,31 +936,38 @@
         ),
         # default features without dev-dependencies
         (
             "tokio-1.25.0.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.49",
                 "(crate(pin-project-lite/default) >= 0.2.0 with crate(pin-project-lite/default) < 0.3.0~)",
                 "(crate(autocfg/default) >= 1.1.0 with crate(autocfg/default) < 2.0.0~)",
                 "(crate(windows-sys/default) >= 0.42.0 with crate(windows-sys/default) < 0.43.0~)",
                 "(crate(windows-sys/Win32_Foundation) >= 0.42.0 with crate(windows-sys/Win32_Foundation) < 0.43.0~)",
                 "(crate(windows-sys/Win32_Security_Authorization) >= 0.42.0 with crate(windows-sys/Win32_Security_Authorization) < 0.43.0~)",
             },
         ),
         # default features with dev-dependencies
-        ("unicode-xid-0.2.4.json", FeatureFlags(), True, {"(crate(criterion/default) >= 0.3.0 with crate(criterion/default) < 0.4.0~)"}),
+        (
+            "unicode-xid-0.2.4.json",
+            FeatureFlags(),
+            True,
+            {"rust >= 1.17", "(crate(criterion/default) >= 0.3.0 with crate(criterion/default) < 0.4.0~)"},
+        ),
         # default features without dev-dependencies
-        ("unicode-xid-0.2.4.json", FeatureFlags(), False, set()),
+        ("unicode-xid-0.2.4.json", FeatureFlags(), False, {"rust >= 1.17"}),
         # default features with dev-dependencies
         (
             "zbus-3.8.0.json",
             FeatureFlags(),
             True,
             {
+                "rust >= 1.60",
                 "(crate(async-broadcast/default) >= 0.5.0 with crate(async-broadcast/default) < 0.6.0~)",
                 "(crate(async-executor/default) >= 1.5.0 with crate(async-executor/default) < 2.0.0~)",
                 "(crate(async-io/default) >= 1.12.0 with crate(async-io/default) < 2.0.0~)",
                 "(crate(async-lock/default) >= 2.6.0 with crate(async-lock/default) < 3.0.0~)",
                 "(crate(async-recursion/default) >= 1.0.0 with crate(async-recursion/default) < 2.0.0~)",
                 "(crate(async-task/default) >= 4.3.0 with crate(async-task/default) < 5.0.0~)",
                 "(crate(async-trait/default) >= 0.1.58 with crate(async-trait/default) < 0.2.0~)",
@@ -978,14 +1032,15 @@
         ),
         # default features without dev-dependencies
         (
             "zbus-3.8.0.json",
             FeatureFlags(),
             False,
             {
+                "rust >= 1.60",
                 "(crate(async-broadcast/default) >= 0.5.0 with crate(async-broadcast/default) < 0.6.0~)",
                 "(crate(async-executor/default) >= 1.5.0 with crate(async-executor/default) < 2.0.0~)",
                 "(crate(async-io/default) >= 1.12.0 with crate(async-io/default) < 2.0.0~)",
                 "(crate(async-lock/default) >= 2.6.0 with crate(async-lock/default) < 3.0.0~)",
                 "(crate(async-recursion/default) >= 1.0.0 with crate(async-recursion/default) < 2.0.0~)",
                 "(crate(async-task/default) >= 4.3.0 with crate(async-task/default) < 5.0.0~)",
                 "(crate(async-trait/default) >= 0.1.58 with crate(async-trait/default) < 0.2.0~)",
@@ -1040,14 +1095,160 @@
 
 
 @pytest.mark.parametrize(
     "filename,flags,with_dev_deps,expected",
     [
         # default features with dev-dependencies
         (
+            "espanso-2.1.8.json",
+            FeatureFlags(),
+            True,
+            {
+                "(crate(anyhow/default) >= 1.0.38 with crate(anyhow/default) < 2.0.0~)",
+                "(crate(caps/default) >= 0.5.2 with crate(caps/default) < 0.6.0~)",
+                "(crate(cc/default) >= 1.0.73 with crate(cc/default) < 2.0.0~)",
+                "(crate(chrono/default) >= 0.4.19 with crate(chrono/default) < 0.5.0~)",
+                "(crate(chrono/unstable-locales) >= 0.4.19 with crate(chrono/unstable-locales) < 0.5.0~)",
+                "(crate(clap/default) >= 2.33.3 with crate(clap/default) < 3.0.0~)",
+                "(crate(colored/default) >= 2.0.0 with crate(colored/default) < 3.0.0~)",
+                "(crate(const_format/default) >= 0.2.14 with crate(const_format/default) < 0.3.0~)",
+                "(crate(crossbeam/default) >= 0.8.0 with crate(crossbeam/default) < 0.9.0~)",
+                "(crate(dialoguer/default) >= 0.8.0 with crate(dialoguer/default) < 0.9.0~)",
+                "(crate(dirs/default) >= 3.0.1 with crate(dirs/default) < 4.0.0~)",
+                "(crate(dunce/default) >= 1.0.1 with crate(dunce/default) < 2.0.0~)",
+                "(crate(enum-as-inner/default) >= 0.3.3 with crate(enum-as-inner/default) < 0.4.0~)",
+                "(crate(fs_extra/default) >= 1.2.0 with crate(fs_extra/default) < 2.0.0~)",
+                "(crate(fs2/default) >= 0.4.3 with crate(fs2/default) < 0.5.0~)",
+                "(crate(glob/default) >= 0.3.0 with crate(glob/default) < 0.4.0~)",
+                "(crate(hex/default) >= 0.4.3 with crate(hex/default) < 0.5.0~)",
+                "(crate(html2text/default) >= 0.2.1 with crate(html2text/default) < 0.3.0~)",
+                "(crate(include_dir/default) >= 0.6.0 with crate(include_dir/default) < 0.7.0~)",
+                "(crate(include_dir/search) >= 0.6.0 with crate(include_dir/search) < 0.7.0~)",
+                "(crate(indoc/default) >= 1.0.3 with crate(indoc/default) < 2.0.0~)",
+                "(crate(itertools/default) >= 0.10.0 with crate(itertools/default) < 0.11.0~)",
+                "(crate(lazycell/default) >= 1.3.0 with crate(lazycell/default) < 2.0.0~)",
+                "(crate(lazy_static/default) >= 1.4.0 with crate(lazy_static/default) < 2.0.0~)",
+                "(crate(libc/default) >= 0.2.85 with crate(libc/default) < 0.3.0~)",
+                "(crate(libc/default) >= 0.2.98 with crate(libc/default) < 0.3.0~)",
+                "(crate(log/default) >= 0.4.14 with crate(log/default) < 0.5.0~)",
+                "(crate(log-panics/default) >= 2.0.0 with crate(log-panics/default) < 3.0.0~)",
+                "(crate(maplit/default) >= 1.0.2 with crate(maplit/default) < 2.0.0~)",
+                "(crate(markdown/default) >= 0.3.0 with crate(markdown/default) < 0.4.0~)",
+                "(crate(mockall/default) >= 0.9.1 with crate(mockall/default) < 0.10.0~)",
+                "(crate(named_pipe/default) >= 0.4.1 with crate(named_pipe/default) < 0.5.0~)",
+                "(crate(natord/default) >= 1.0.9 with crate(natord/default) < 2.0.0~)",
+                "(crate(notify/default) >= 4.0.17 with crate(notify/default) < 5.0.0~)",
+                "(crate(notify-rust/default) >= 4.2.2 with crate(notify-rust/default) < 5.0.0~)",
+                "(crate(opener/default) >= 0.5.0 with crate(opener/default) < 0.6.0~)",
+                "(crate(ordered-float/default) >= 2.0.0 with crate(ordered-float/default) < 3.0.0~)",
+                "(crate(path-slash/default) >= 0.1.4 with crate(path-slash/default) < 0.2.0~)",
+                "(crate(pretty_assertions/default) >= 0.7.2 with crate(pretty_assertions/default) < 0.8.0~)",
+                "(crate(rand/default) >= 0.8.3 with crate(rand/default) < 0.9.0~)",
+                "(crate(regex/default) >= 1.5.5 with crate(regex/default) < 2.0.0~)",
+                "(crate(reqwest) >= 0.11.4 with crate(reqwest) < 0.12.0~)",
+                "(crate(reqwest/blocking) >= 0.11.4 with crate(reqwest/blocking) < 0.12.0~)",
+                "(crate(reqwest/default-tls) >= 0.11.4 with crate(reqwest/default-tls) < 0.12.0~)",
+                "(crate(scopeguard/default) >= 1.1.0 with crate(scopeguard/default) < 2.0.0~)",
+                "(crate(serde/default) >= 1.0.123 with crate(serde/default) < 2.0.0~)",
+                "(crate(serde/derive) >= 1.0.123 with crate(serde/derive) < 2.0.0~)",
+                "(crate(serde_json/default) >= 1.0.61 with crate(serde_json/default) < 2.0.0~)",
+                "(crate(serde_json/default) >= 1.0.62 with crate(serde_json/default) < 2.0.0~)",
+                "(crate(serde_yaml/default) >= 0.8.17 with crate(serde_yaml/default) < 0.9.0~)",
+                "(crate(sha2/default) >= 0.9.6 with crate(sha2/default) < 0.10.0~)",
+                "(crate(simplelog/default) >= 0.9.0 with crate(simplelog/default) < 0.10.0~)",
+                "(crate(sys-locale/default) >= 0.1.0 with crate(sys-locale/default) < 0.2.0~)",
+                "(crate(sysinfo/default) >= 0.24.5 with crate(sysinfo/default) < 0.25.0~)",
+                "(crate(tempdir/default) >= 0.3.7 with crate(tempdir/default) < 0.4.0~)",
+                "(crate(tempfile/default) >= 3.2.0 with crate(tempfile/default) < 4.0.0~)",
+                "(crate(test-case/default) >= 1.1.0 with crate(test-case/default) < 2.0.0~)",
+                "(crate(thiserror/default) >= 1.0.23 with crate(thiserror/default) < 2.0.0~)",
+                "(crate(unicase/default) >= 2.6.0 with crate(unicase/default) < 3.0.0~)",
+                "(crate(walkdir/default) >= 2.3.1 with crate(walkdir/default) < 3.0.0~)",
+                "(crate(widestring/default) >= 0.4.3 with crate(widestring/default) < 0.5.0~)",
+                "(crate(winapi/default) >= 0.3.9 with crate(winapi/default) < 0.4.0~)",
+                "(crate(winapi/wincon) >= 0.3.9 with crate(winapi/wincon) < 0.4.0~)",
+                "(crate(winreg/default) >= 0.9.0 with crate(winreg/default) < 0.10.0~)",
+                "(crate(winrt-notification/default) >= 0.3.1 with crate(winrt-notification/default) < 0.4.0~)",
+                "(crate(winres/default) >= 0.1.11 with crate(winres/default) < 0.2.0~)",
+                "(crate(zip/default) >= 0.5.12 with crate(zip/default) < 0.6.0~)",
+                "(crate(zip/default) >= 0.5.13 with crate(zip/default) < 0.6.0~)",
+            },
+        ),
+        # default features without dev-dependencies
+        (
+            "espanso-2.1.8.json",
+            FeatureFlags(),
+            False,
+            {
+                "(crate(anyhow/default) >= 1.0.38 with crate(anyhow/default) < 2.0.0~)",
+                "(crate(caps/default) >= 0.5.2 with crate(caps/default) < 0.6.0~)",
+                "(crate(cc/default) >= 1.0.73 with crate(cc/default) < 2.0.0~)",
+                "(crate(chrono/default) >= 0.4.19 with crate(chrono/default) < 0.5.0~)",
+                "(crate(chrono/unstable-locales) >= 0.4.19 with crate(chrono/unstable-locales) < 0.5.0~)",
+                "(crate(clap/default) >= 2.33.3 with crate(clap/default) < 3.0.0~)",
+                "(crate(colored/default) >= 2.0.0 with crate(colored/default) < 3.0.0~)",
+                "(crate(const_format/default) >= 0.2.14 with crate(const_format/default) < 0.3.0~)",
+                "(crate(crossbeam/default) >= 0.8.0 with crate(crossbeam/default) < 0.9.0~)",
+                "(crate(dialoguer/default) >= 0.8.0 with crate(dialoguer/default) < 0.9.0~)",
+                "(crate(dirs/default) >= 3.0.1 with crate(dirs/default) < 4.0.0~)",
+                "(crate(dunce/default) >= 1.0.1 with crate(dunce/default) < 2.0.0~)",
+                "(crate(enum-as-inner/default) >= 0.3.3 with crate(enum-as-inner/default) < 0.4.0~)",
+                "(crate(fs_extra/default) >= 1.2.0 with crate(fs_extra/default) < 2.0.0~)",
+                "(crate(fs2/default) >= 0.4.3 with crate(fs2/default) < 0.5.0~)",
+                "(crate(glob/default) >= 0.3.0 with crate(glob/default) < 0.4.0~)",
+                "(crate(hex/default) >= 0.4.3 with crate(hex/default) < 0.5.0~)",
+                "(crate(html2text/default) >= 0.2.1 with crate(html2text/default) < 0.3.0~)",
+                "(crate(indoc/default) >= 1.0.3 with crate(indoc/default) < 2.0.0~)",
+                "(crate(itertools/default) >= 0.10.0 with crate(itertools/default) < 0.11.0~)",
+                "(crate(lazycell/default) >= 1.3.0 with crate(lazycell/default) < 2.0.0~)",
+                "(crate(lazy_static/default) >= 1.4.0 with crate(lazy_static/default) < 2.0.0~)",
+                "(crate(libc/default) >= 0.2.85 with crate(libc/default) < 0.3.0~)",
+                "(crate(libc/default) >= 0.2.98 with crate(libc/default) < 0.3.0~)",
+                "(crate(log/default) >= 0.4.14 with crate(log/default) < 0.5.0~)",
+                "(crate(log-panics/default) >= 2.0.0 with crate(log-panics/default) < 3.0.0~)",
+                "(crate(maplit/default) >= 1.0.2 with crate(maplit/default) < 2.0.0~)",
+                "(crate(markdown/default) >= 0.3.0 with crate(markdown/default) < 0.4.0~)",
+                "(crate(named_pipe/default) >= 0.4.1 with crate(named_pipe/default) < 0.5.0~)",
+                "(crate(natord/default) >= 1.0.9 with crate(natord/default) < 2.0.0~)",
+                "(crate(notify/default) >= 4.0.17 with crate(notify/default) < 5.0.0~)",
+                "(crate(notify-rust/default) >= 4.2.2 with crate(notify-rust/default) < 5.0.0~)",
+                "(crate(opener/default) >= 0.5.0 with crate(opener/default) < 0.6.0~)",
+                "(crate(ordered-float/default) >= 2.0.0 with crate(ordered-float/default) < 3.0.0~)",
+                "(crate(path-slash/default) >= 0.1.4 with crate(path-slash/default) < 0.2.0~)",
+                "(crate(rand/default) >= 0.8.3 with crate(rand/default) < 0.9.0~)",
+                "(crate(regex/default) >= 1.5.5 with crate(regex/default) < 2.0.0~)",
+                "(crate(reqwest) >= 0.11.4 with crate(reqwest) < 0.12.0~)",
+                "(crate(reqwest/blocking) >= 0.11.4 with crate(reqwest/blocking) < 0.12.0~)",
+                "(crate(reqwest/default-tls) >= 0.11.4 with crate(reqwest/default-tls) < 0.12.0~)",
+                "(crate(scopeguard/default) >= 1.1.0 with crate(scopeguard/default) < 2.0.0~)",
+                "(crate(serde/default) >= 1.0.123 with crate(serde/default) < 2.0.0~)",
+                "(crate(serde/derive) >= 1.0.123 with crate(serde/derive) < 2.0.0~)",
+                "(crate(serde_json/default) >= 1.0.61 with crate(serde_json/default) < 2.0.0~)",
+                "(crate(serde_json/default) >= 1.0.62 with crate(serde_json/default) < 2.0.0~)",
+                "(crate(serde_yaml/default) >= 0.8.17 with crate(serde_yaml/default) < 0.9.0~)",
+                "(crate(sha2/default) >= 0.9.6 with crate(sha2/default) < 0.10.0~)",
+                "(crate(simplelog/default) >= 0.9.0 with crate(simplelog/default) < 0.10.0~)",
+                "(crate(sys-locale/default) >= 0.1.0 with crate(sys-locale/default) < 0.2.0~)",
+                "(crate(sysinfo/default) >= 0.24.5 with crate(sysinfo/default) < 0.25.0~)",
+                "(crate(tempdir/default) >= 0.3.7 with crate(tempdir/default) < 0.4.0~)",
+                "(crate(thiserror/default) >= 1.0.23 with crate(thiserror/default) < 2.0.0~)",
+                "(crate(unicase/default) >= 2.6.0 with crate(unicase/default) < 3.0.0~)",
+                "(crate(walkdir/default) >= 2.3.1 with crate(walkdir/default) < 3.0.0~)",
+                "(crate(widestring/default) >= 0.4.3 with crate(widestring/default) < 0.5.0~)",
+                "(crate(winapi/default) >= 0.3.9 with crate(winapi/default) < 0.4.0~)",
+                "(crate(winapi/wincon) >= 0.3.9 with crate(winapi/wincon) < 0.4.0~)",
+                "(crate(winreg/default) >= 0.9.0 with crate(winreg/default) < 0.10.0~)",
+                "(crate(winrt-notification/default) >= 0.3.1 with crate(winrt-notification/default) < 0.4.0~)",
+                "(crate(winres/default) >= 0.1.11 with crate(winres/default) < 0.2.0~)",
+                "(crate(zip/default) >= 0.5.12 with crate(zip/default) < 0.6.0~)",
+                "(crate(zip/default) >= 0.5.13 with crate(zip/default) < 0.6.0~)",
+            },
+        ),
+        # default features with dev-dependencies
+        (
             "fapolicy-analyzer-0.6.8.json",
             FeatureFlags(),
             True,
             {
                 "(crate(chrono/default) >= 0.4.22 with crate(chrono/default) < 0.5.0~)",
                 "(crate(nom/default) >= 7.1.0 with crate(nom/default) < 8.0.0~)",
                 "(crate(serde/default) >= 1.0.0 with crate(serde/default) < 2.0.0~)",
```

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/rpm/test_provides.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/rpm/test_provides.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/rpm/test_requires.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/rpm/test_requires.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,27 +19,29 @@
                 "(crate(version_check/default) >= 0.9.4 with crate(version_check/default) < 0.10.0~)",
             },
         ),
         (
             "assert_cmd-2.0.8.json",
             {
                 "cargo",
+                "rust >= 1.60.0",
                 "(crate(bstr/default) >= 1.0.1 with crate(bstr/default) < 2.0.0~)",
                 "(crate(doc-comment/default) >= 0.3.0 with crate(doc-comment/default) < 0.4.0~)",
                 "(crate(predicates) >= 2.1.0 with crate(predicates) < 3.0.0~)",
                 "(crate(predicates/diff) >= 2.1.0 with crate(predicates/diff) < 3.0.0~)",
                 "(crate(predicates-core/default) >= 1.0.0 with crate(predicates-core/default) < 2.0.0~)",
                 "(crate(predicates-tree/default) >= 1.0.0 with crate(predicates-tree/default) < 2.0.0~)",
                 "(crate(wait-timeout/default) >= 0.2.0 with crate(wait-timeout/default) < 0.3.0~)",
             },
         ),
         (
             "assert_fs-1.0.10.json",
             {
                 "cargo",
+                "rust >= 1.60.0",
                 "(crate(doc-comment/default) >= 0.3.0 with crate(doc-comment/default) < 0.4.0~)",
                 "(crate(globwalk/default) >= 0.8.0 with crate(globwalk/default) < 0.9.0~)",
                 "(crate(predicates) >= 2.0.3 with crate(predicates) < 3.0.0~)",
                 "(crate(predicates/diff) >= 2.0.3 with crate(predicates/diff) < 3.0.0~)",
                 "(crate(predicates-core/default) >= 1.0.0 with crate(predicates-core/default) < 2.0.0~)",
                 "(crate(predicates-tree/default) >= 1.0.0 with crate(predicates-tree/default) < 2.0.0~)",
                 "(crate(tempfile/default) >= 3.0.0 with crate(tempfile/default) < 4.0.0~)",
@@ -49,34 +51,40 @@
             "autocfg-1.1.0.json",
             {
                 "cargo",
             },
         ),
         (
             "bstr-1.2.0.json",
-            {"cargo", "(crate(memchr) >= 2.4.0 with crate(memchr) < 3.0.0~)"},
+            {
+                "cargo",
+                "rust >= 1.60",
+                "(crate(memchr) >= 2.4.0 with crate(memchr) < 3.0.0~)",
+            },
         ),
         (
             "cfg-if-1.0.0.json",
             {
                 "cargo",
             },
         ),
         (
             "clap-4.1.4.json",
             {
                 "cargo",
+                "rust >= 1.64.0",
                 "(crate(bitflags/default) >= 1.2.0 with crate(bitflags/default) < 2.0.0~)",
                 "(crate(clap_lex/default) >= 0.3.0 with crate(clap_lex/default) < 0.4.0~)",
             },
         ),
         (
             "gstreamer-0.19.7.json",
             {
                 "cargo",
+                "rust >= 1.63",
                 "(crate(bitflags/default) >= 1.0.0 with crate(bitflags/default) < 2.0.0~)",
                 "(crate(cfg-if/default) >= 1.0.0 with crate(cfg-if/default) < 2.0.0~)",
                 "(crate(gstreamer-sys/default) >= 0.19.0 with crate(gstreamer-sys/default) < 0.20.0~)",
                 "(crate(futures-channel/default) >= 0.3.0 with crate(futures-channel/default) < 0.4.0~)",
                 "(crate(futures-core/default) >= 0.3.0 with crate(futures-core/default) < 0.4.0~)",
                 "(crate(futures-util) >= 0.3.0 with crate(futures-util) < 0.4.0~)",
                 "(crate(glib/default) >= 0.16.2 with crate(glib/default) < 0.17.0~)",
@@ -91,14 +99,15 @@
                 "(crate(thiserror/default) >= 1.0.0 with crate(thiserror/default) < 2.0.0~)",
             },
         ),
         (
             "human-panic-1.1.0.json",
             {
                 "cargo",
+                "rust >= 1.60.0",
                 "(crate(backtrace/default) >= 0.3.9 with crate(backtrace/default) < 0.4.0~)",
                 "(crate(os_info/default) >= 2.0.6 with crate(os_info/default) < 3.0.0~)",
                 "(crate(serde/default) >= 1.0.79 with crate(serde/default) < 2.0.0~)",
                 "(crate(serde_derive/default) >= 1.0.79 with crate(serde_derive/default) < 2.0.0~)",
                 "(crate(toml/default) >= 0.5.0 with crate(toml/default) < 0.6.0~)",
                 "(crate(uuid) >= 0.8.0 with crate(uuid) < 0.9.0~)",
                 "(crate(uuid/v4) >= 0.8.0 with crate(uuid/v4) < 0.9.0~)",
@@ -110,29 +119,32 @@
                 "cargo",
             },
         ),
         (
             "predicates-2.1.5.json",
             {
                 "cargo",
+                "rust >= 1.60.0",
                 "(crate(itertools/default) >= 0.10.0 with crate(itertools/default) < 0.11.0~)",
                 "(crate(predicates-core/default) >= 1.0.0 with crate(predicates-core/default) < 2.0.0~)",
             },
         ),
         (
             "proc-macro2-1.0.50.json",
             {
                 "cargo",
+                "rust >= 1.31",
                 "(crate(unicode-ident/default) >= 1.0.0 with crate(unicode-ident/default) < 2.0.0~)",
             },
         ),
         (
             "quote-1.0.23.json",
             {
                 "cargo",
+                "rust >= 1.31",
                 "(crate(proc-macro2) >= 1.0.40 with crate(proc-macro2) < 2.0.0~)",
             },
         ),
         (
             "rand-0.8.5.json",
             {
                 "cargo",
@@ -145,23 +157,25 @@
                 "cargo",
             },
         ),
         (
             "rust_decimal-1.28.0.json",
             {
                 "cargo",
+                "rust >= 1.60",
                 "(crate(arrayvec) >= 0.7.0 with crate(arrayvec) < 0.8.0~)",
                 "(crate(num-traits) >= 0.2.0 with crate(num-traits) < 0.3.0~)",
                 "(crate(num-traits/i128) >= 0.2.0 with crate(num-traits/i128) < 0.3.0~)",
             },
         ),
         (
             "rustix-0.36.8.json",
             {
                 "cargo",
+                "rust >= 1.48",
                 "(crate(bitflags/default) >= 1.2.1 with crate(bitflags/default) < 2.0.0~)",
                 "(crate(linux-raw-sys) >= 0.1.2 with crate(linux-raw-sys) < 0.2.0~)",
                 "(crate(linux-raw-sys/errno) >= 0.1.2 with crate(linux-raw-sys/errno) < 0.2.0~)",
                 "(crate(linux-raw-sys/general) >= 0.1.2 with crate(linux-raw-sys/general) < 0.2.0~)",
                 "(crate(linux-raw-sys/ioctl) >= 0.1.2 with crate(linux-raw-sys/ioctl) < 0.2.0~)",
                 "(crate(linux-raw-sys/no_std) >= 0.1.2 with crate(linux-raw-sys/no_std) < 0.2.0~)",
                 "(crate(libc/default) >= 0.2.133 with crate(libc/default) < 0.3.0~)",
@@ -174,61 +188,68 @@
                 "(crate(windows-sys/Win32_System_Threading) >= 0.45.0 with crate(windows-sys/Win32_System_Threading) < 0.46.0~)",
             },
         ),
         (
             "serde-1.0.152.json",
             {
                 "cargo",
+                "rust >= 1.13",
             },
         ),
         (
             "serde_derive-1.0.152.json",
             {
                 "cargo",
+                "rust >= 1.31",
                 "(crate(proc-macro2/default) >= 1.0.0 with crate(proc-macro2/default) < 2.0.0~)",
                 "(crate(quote/default) >= 1.0.0 with crate(quote/default) < 2.0.0~)",
                 "(crate(syn/default) >= 1.0.104 with crate(syn/default) < 2.0.0~)",
             },
         ),
         (
             "syn-1.0.107.json",
             {
                 "cargo",
+                "rust >= 1.31",
                 "(crate(proc-macro2) >= 1.0.46 with crate(proc-macro2) < 2.0.0~)",
                 "(crate(unicode-ident/default) >= 1.0.0 with crate(unicode-ident/default) < 2.0.0~)",
             },
         ),
         (
             "time-0.3.17.json",
             {
                 "cargo",
+                "rust >= 1.60.0",
                 "crate(time-core/default) = 0.1.0",
             },
         ),
         (
             "tokio-1.25.0.json",
             {
                 "cargo",
+                "rust >= 1.49",
                 "(crate(pin-project-lite/default) >= 0.2.0 with crate(pin-project-lite/default) < 0.3.0~)",
                 "(crate(autocfg/default) >= 1.1.0 with crate(autocfg/default) < 2.0.0~)",
                 "(crate(windows-sys/default) >= 0.42.0 with crate(windows-sys/default) < 0.43.0~)",
                 "(crate(windows-sys/Win32_Foundation) >= 0.42.0 with crate(windows-sys/Win32_Foundation) < 0.43.0~)",
                 "(crate(windows-sys/Win32_Security_Authorization) >= 0.42.0 with crate(windows-sys/Win32_Security_Authorization) < 0.43.0~)",
             },
         ),
         (
             "unicode-xid-0.2.4.json",
             {
                 "cargo",
+                "rust >= 1.17",
             },
         ),
         (
             "zbus-3.8.0.json",
             {
                 "cargo",
+                "rust >= 1.60",
                 "(crate(async-broadcast/default) >= 0.5.0 with crate(async-broadcast/default) < 0.6.0~)",
                 "(crate(async-recursion/default) >= 1.0.0 with crate(async-recursion/default) < 2.0.0~)",
                 "(crate(async-trait/default) >= 0.1.58 with crate(async-trait/default) < 0.2.0~)",
                 "(crate(byteorder/default) >= 1.4.3 with crate(byteorder/default) < 2.0.0~)",
                 "(crate(derivative/default) >= 2.2.0 with crate(derivative/default) < 3.0.0~)",
                 "(crate(dirs/default) >= 4.0.0 with crate(dirs/default) < 5.0.0~)",
                 "(crate(enumflags2/default) >= 0.7.5 with crate(enumflags2/default) < 0.8.0~)",
```

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/rpm/test_subpackages.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/rpm/test_subpackages.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_comparator.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_comparator.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_prerelease.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_prerelease.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_prerelease_comp.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_prerelease_comp.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_regex.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_regex.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_version.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_version.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_version_comp.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_version_comp.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/semver/test_version_req.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/semver/test_version_req.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/tests/test_cli.py` & `cargo2rpm-0.1.9/cargo2rpm/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm/utils.py` & `cargo2rpm-0.1.9/cargo2rpm/utils.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.8/cargo2rpm.egg-info/PKG-INFO` & `cargo2rpm-0.1.9/cargo2rpm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cargo2rpm
-Version: 0.1.8
+Version: 0.1.9
 Summary: Translation layer between cargo and RPM
 Home-page: https://pagure.io/fedora-rust/cargo2rpm
 Author: Fedora Rust SIG
 Author-email: rust@lists.fedoraproject.org
 License: MIT
 Keywords: rpm,cargo,rust
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cargo2rpm-0.1.8/cargo2rpm.egg-info/SOURCES.txt` & `cargo2rpm-0.1.9/cargo2rpm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 cargo2rpm/testdata/aho-corasick-1.0.2.json
 cargo2rpm/testdata/assert_cmd-2.0.8.json
 cargo2rpm/testdata/assert_fs-1.0.10.json
 cargo2rpm/testdata/autocfg-1.1.0.json
 cargo2rpm/testdata/bstr-1.2.0.json
 cargo2rpm/testdata/cfg-if-1.0.0.json
 cargo2rpm/testdata/clap-4.1.4.json
+cargo2rpm/testdata/espanso-2.1.8.json
 cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json
 cargo2rpm/testdata/gstreamer-0.19.7.json
 cargo2rpm/testdata/human-panic-1.1.0.json
 cargo2rpm/testdata/hyperfine-1.15.0.json
 cargo2rpm/testdata/iri-string-0.7.0.json
 cargo2rpm/testdata/libblkio-1.2.2.json
 cargo2rpm/testdata/libc-0.2.139.json
```

### Comparing `cargo2rpm-0.1.8/setup.cfg` & `cargo2rpm-0.1.9/setup.cfg`

 * *Files identical despite different names*

