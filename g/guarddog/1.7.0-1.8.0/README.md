# Comparing `tmp/guarddog-1.7.0.tar.gz` & `tmp/guarddog-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guarddog-1.7.0.tar", max compression
+gzip compressed data, was "guarddog-1.8.0.tar", max compression
```

## Comparing `guarddog-1.7.0.tar` & `guarddog-1.8.0.tar`

### file list

```diff
@@ -1,70 +1,73 @@
--rw-r--r--   0        0        0    11377 2024-05-07 19:22:34.620713 guarddog-1.7.0/LICENSE
--rw-r--r--   0        0        0      314 2024-05-07 19:22:34.620713 guarddog-1.7.0/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0      140 2024-05-07 19:22:34.624713 guarddog-1.7.0/NOTICE
--rw-r--r--   0        0        0      154 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/__init__.py
--rw-r--r--   0        0        0      246 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/__main__.py
--rw-r--r--   0        0        0        0 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/__init__.py
--rw-r--r--   0        0        0     9791 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/analyzer.py
--rw-r--r--   0        0        0      457 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/__init__.py
--rw-r--r--   0        0        0      609 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/detector.py
--rw-r--r--   0        0        0     1166 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/empty_information.py
--rw-r--r--   0        0        0     1126 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/npm/__init__.py
--rw-r--r--   0        0        0     2449 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/npm/direct_url_dependency.py
--rw-r--r--   0        0        0      793 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/npm/empty_information.py
--rw-r--r--   0        0        0     4428 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py
--rw-r--r--   0        0        0     1643 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      578 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/npm/release_zero.py
--rw-r--r--   0        0        0     1732 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/npm/typosquatting.py
--rw-r--r--   0        0        0      899 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/npm/unclaimed_maintainer_email_domain.py
--rw-r--r--   0        0        0      461 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/npm/utils.py
--rw-r--r--   0        0        0     2806 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0     1151 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/pypi/__init__.py
--rw-r--r--   0        0        0      723 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/pypi/empty_information.py
--rw-r--r--   0        0        0     1679 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      716 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/pypi/release_zero.py
--rw-r--r--   0        0        0    11635 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
--rw-r--r--   0        0        0     1369 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/pypi/single_python_file.py
--rw-r--r--   0        0        0     3490 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/pypi/typosquatting.py
--rw-r--r--   0        0        0      406 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/pypi/unclaimed_maintainer_email_domain.py
--rw-r--r--   0        0        0      199 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/pypi/utils.py
--rw-r--r--   0        0        0      438 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/release_zero.py
--rw-r--r--   0        0        0      743 2024-05-07 19:22:34.624713 guarddog-1.7.0/guarddog/analyzer/metadata/repository_integrity_mismatch.py
--rw-r--r--   0        0        0   373303 2024-05-07 19:22:34.628713 guarddog-1.7.0/guarddog/analyzer/metadata/resources/top_npm_packages.json
--rw-r--r--   0        0        0   387251 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/metadata/resources/top_pypi_packages.json
--rw-r--r--   0        0        0     5619 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/metadata/typosquatting.py
--rw-r--r--   0        0        0     2343 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/metadata/unclaimed_maintainer_email_domain.py
--rw-r--r--   0        0        0     1603 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/metadata/utils.py
--rw-r--r--   0        0        0     1043 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/__init__.py
--rw-r--r--   0        0        0      524 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/clipboard-access.yml
--rw-r--r--   0        0        0      682 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/cmd-overwrite.yml
--rw-r--r--   0        0        0     4655 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/code-execution.yml
--rw-r--r--   0        0        0     2855 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/download-executable.yml
--rw-r--r--   0        0        0     2371 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/exec-base64.yml
--rw-r--r--   0        0        0     1815 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
--rw-r--r--   0        0        0      576 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/npm-exec-base64.yml
--rw-r--r--   0        0        0     2692 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/npm-exfiltrate-sensitive-data.yml
--rw-r--r--   0        0        0     1067 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/npm-install-script.yml
--rw-r--r--   0        0        0     2100 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/npm-obfuscation.yml
--rw-r--r--   0        0        0      835 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
--rw-r--r--   0        0        0     3513 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
--rw-r--r--   0        0        0      582 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/obfuscation.yml
--rw-r--r--   0        0        0     1415 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/shady-links.yml
--rw-r--r--   0        0        0      418 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/silent-process-execution.yml
--rw-r--r--   0        0        0      606 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/analyzer/sourcecode/steganography.yml
--rw-r--r--   0        0        0    13215 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/cli.py
--rw-r--r--   0        0        0      315 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/ecosystems.py
--rw-r--r--   0        0        0        0 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/reporters/__init__.py
--rw-r--r--   0        0        0     6189 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/reporters/sarif.py
--rw-r--r--   0        0        0      752 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/scanners/__init__.py
--rw-r--r--   0        0        0     1968 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/scanners/npm_package_scanner.py
--rw-r--r--   0        0        0     2243 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/scanners/npm_project_scanner.py
--rw-r--r--   0        0        0     2512 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/scanners/pypi_package_scanner.py
--rw-r--r--   0        0        0     5491 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/scanners/pypi_project_scanner.py
--rw-r--r--   0        0        0    11170 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/scanners/scanner.py
--rw-r--r--   0        0        0        0 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/utils/__init__.py
--rw-r--r--   0        0        0     1323 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/utils/archives.py
--rw-r--r--   0        0        0       54 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/utils/exceptions.py
--rw-r--r--   0        0        0      953 2024-05-07 19:22:34.632713 guarddog-1.7.0/guarddog/utils/package_info.py
--rw-r--r--   0        0        0       52 2024-05-07 19:22:34.632713 guarddog-1.7.0/pypi.rst
--rw-r--r--   0        0        0     1222 2024-05-07 19:22:42.628758 guarddog-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 guarddog-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11377 2024-05-23 11:15:19.322424 guarddog-1.8.0/LICENSE
+-rw-r--r--   0        0        0      314 2024-05-23 11:15:19.322424 guarddog-1.8.0/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0      140 2024-05-23 11:15:19.322424 guarddog-1.8.0/NOTICE
+-rw-r--r--   0        0        0      154 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/__init__.py
+-rw-r--r--   0        0        0     9791 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/analyzer.py
+-rw-r--r--   0        0        0      457 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/metadata/__init__.py
+-rw-r--r--   0        0        0     1840 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/metadata/bundled_binary.py
+-rw-r--r--   0        0        0      609 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/metadata/detector.py
+-rw-r--r--   0        0        0     1166 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/metadata/empty_information.py
+-rw-r--r--   0        0        0     1223 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/__init__.py
+-rw-r--r--   0        0        0      360 2024-05-23 11:15:19.322424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/bundled_binary.py
+-rw-r--r--   0        0        0     2449 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/direct_url_dependency.py
+-rw-r--r--   0        0        0      793 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/empty_information.py
+-rw-r--r--   0        0        0     4428 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py
+-rw-r--r--   0        0        0     1643 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      578 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/release_zero.py
+-rw-r--r--   0        0        0     1732 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/typosquatting.py
+-rw-r--r--   0        0        0      899 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/unclaimed_maintainer_email_domain.py
+-rw-r--r--   0        0        0      461 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/npm/utils.py
+-rw-r--r--   0        0        0     2806 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0     1251 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/__init__.py
+-rw-r--r--   0        0        0      361 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/bundled_binary.py
+-rw-r--r--   0        0        0      723 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/empty_information.py
+-rw-r--r--   0        0        0     1679 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      716 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/release_zero.py
+-rw-r--r--   0        0        0    11635 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0     1369 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/single_python_file.py
+-rw-r--r--   0        0        0     3490 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/typosquatting.py
+-rw-r--r--   0        0        0      406 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/unclaimed_maintainer_email_domain.py
+-rw-r--r--   0        0        0      199 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/pypi/utils.py
+-rw-r--r--   0        0        0      438 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/release_zero.py
+-rw-r--r--   0        0        0      743 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0   373303 2024-05-23 11:15:19.326424 guarddog-1.8.0/guarddog/analyzer/metadata/resources/top_npm_packages.json
+-rw-r--r--   0        0        0   387251 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/metadata/resources/top_pypi_packages.json
+-rw-r--r--   0        0        0     5619 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/metadata/typosquatting.py
+-rw-r--r--   0        0        0     2343 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/metadata/unclaimed_maintainer_email_domain.py
+-rw-r--r--   0        0        0     1603 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/metadata/utils.py
+-rw-r--r--   0        0        0     1043 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/__init__.py
+-rw-r--r--   0        0        0      524 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/clipboard-access.yml
+-rw-r--r--   0        0        0      682 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/cmd-overwrite.yml
+-rw-r--r--   0        0        0     4655 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/code-execution.yml
+-rw-r--r--   0        0        0     3055 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/download-executable.yml
+-rw-r--r--   0        0        0     2371 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/exec-base64.yml
+-rw-r--r--   0        0        0     1815 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
+-rw-r--r--   0        0        0      576 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-exec-base64.yml
+-rw-r--r--   0        0        0     3011 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-exfiltrate-sensitive-data.yml
+-rw-r--r--   0        0        0     1067 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-install-script.yml
+-rw-r--r--   0        0        0     2100 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-obfuscation.yml
+-rw-r--r--   0        0        0      835 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
+-rw-r--r--   0        0        0     3513 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
+-rw-r--r--   0        0        0      582 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/obfuscation.yml
+-rw-r--r--   0        0        0     1609 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/shady-links.yml
+-rw-r--r--   0        0        0      418 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/silent-process-execution.yml
+-rw-r--r--   0        0        0      606 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/analyzer/sourcecode/steganography.yml
+-rw-r--r--   0        0        0    13215 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/cli.py
+-rw-r--r--   0        0        0      315 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/ecosystems.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/reporters/__init__.py
+-rw-r--r--   0        0        0     6189 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/reporters/sarif.py
+-rw-r--r--   0        0        0      752 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/scanners/__init__.py
+-rw-r--r--   0        0        0     1968 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/scanners/npm_package_scanner.py
+-rw-r--r--   0        0        0     2243 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/scanners/npm_project_scanner.py
+-rw-r--r--   0        0        0     2512 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/scanners/pypi_package_scanner.py
+-rw-r--r--   0        0        0     5491 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/scanners/pypi_project_scanner.py
+-rw-r--r--   0        0        0    11170 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/scanners/scanner.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/utils/__init__.py
+-rw-r--r--   0        0        0     1323 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/utils/archives.py
+-rw-r--r--   0        0        0       54 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/utils/exceptions.py
+-rw-r--r--   0        0        0      953 2024-05-23 11:15:19.330424 guarddog-1.8.0/guarddog/utils/package_info.py
+-rw-r--r--   0        0        0       52 2024-05-23 11:15:19.330424 guarddog-1.8.0/pypi.rst
+-rw-r--r--   0        0        0     1222 2024-05-23 11:15:28.242414 guarddog-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 guarddog-1.8.0/PKG-INFO
```

### Comparing `guarddog-1.7.0/LICENSE` & `guarddog-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/analyzer.py` & `guarddog-1.8.0/guarddog/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/detector.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/detector.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/empty_information.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/npm/__init__.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/npm/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 )
 from guarddog.analyzer.metadata.npm.release_zero import NPMReleaseZeroDetector
 from guarddog.analyzer.metadata.npm.typosquatting import NPMTyposquatDetector
 from guarddog.analyzer.metadata.npm.direct_url_dependency import (
     NPMDirectURLDependencyDetector,
 )
 from guarddog.analyzer.metadata.npm.npm_metadata_mismatch import NPMMetadataMismatch
+from guarddog.analyzer.metadata.npm.bundled_binary import NPMBundledBinary
 
 NPM_METADATA_RULES = {}
 
 classes = [
     NPMEmptyInfoDetector,
     NPMReleaseZeroDetector,
     NPMPotentiallyCompromisedEmailDomainDetector,
     NPMUnclaimedMaintainerEmailDomainDetector,
     NPMTyposquatDetector,
     NPMDirectURLDependencyDetector,
     NPMMetadataMismatch,
+    NPMBundledBinary,
 ]
 
 for detectorClass in classes:
     detectorInstance = detectorClass()  # type: ignore
     NPM_METADATA_RULES[detectorInstance.get_name()] = detectorInstance
```

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/npm/direct_url_dependency.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/npm/direct_url_dependency.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/npm/empty_information.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/npm/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/npm/release_zero.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/npm/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/npm/typosquatting.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/npm/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/npm/unclaimed_maintainer_email_domain.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/npm/unclaimed_maintainer_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/potentially_compromised_email_domain.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/pypi/__init__.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,24 +3,25 @@
     PypiPotentiallyCompromisedEmailDomainDetector
 from guarddog.analyzer.metadata.pypi.unclaimed_maintainer_email_domain import \
     PypiUnclaimedMaintainerEmailDomainDetector
 from guarddog.analyzer.metadata.pypi.release_zero import PypiReleaseZeroDetector
 from guarddog.analyzer.metadata.pypi.repository_integrity_mismatch import PypiIntegrityMismatchDetector
 from guarddog.analyzer.metadata.pypi.single_python_file import PypiSinglePythonFileDetector
 from guarddog.analyzer.metadata.pypi.typosquatting import PypiTyposquatDetector
+from guarddog.analyzer.metadata.pypi.bundled_binary import PypiBundledBinary
 
 PYPI_METADATA_RULES = {}
 
 classes = [
     PypiEmptyInfoDetector,
     PypiReleaseZeroDetector,
     PypiTyposquatDetector,
     PypiPotentiallyCompromisedEmailDomainDetector,
     PypiUnclaimedMaintainerEmailDomainDetector,
     PypiIntegrityMismatchDetector,
-    PypiSinglePythonFileDetector
-
+    PypiSinglePythonFileDetector,
+    PypiBundledBinary,
 ]
 
 for detectorClass in classes:
     detectorInstance = detectorClass()  # type: ignore
     PYPI_METADATA_RULES[detectorInstance.get_name()] = detectorInstance
```

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/pypi/empty_information.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/pypi/release_zero.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/pypi/single_python_file.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/single_python_file.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/pypi/typosquatting.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/pypi/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/repository_integrity_mismatch.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/resources/top_npm_packages.json` & `guarddog-1.8.0/guarddog/analyzer/metadata/resources/top_npm_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/resources/top_pypi_packages.json` & `guarddog-1.8.0/guarddog/analyzer/metadata/resources/top_pypi_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/typosquatting.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/unclaimed_maintainer_email_domain.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/unclaimed_maintainer_email_domain.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/metadata/utils.py` & `guarddog-1.8.0/guarddog/analyzer/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/__init__.py` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/clipboard-access.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/clipboard-access.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/cmd-overwrite.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/cmd-overwrite.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/code-execution.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/code-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/download-executable.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/download-executable.yml`

 * *Files 23% similar despite different names*

```diff
@@ -58,22 +58,40 @@
                     - patterns:
                         - pattern: os.rename(..., $EXE)
                         - metavariable-pattern:
                             metavariable: $EXE
                             pattern-regex: (?i)^['"].*?\.exe['"]$
 
     pattern-sources:
-      - pattern: (...).send(...)
-      - pattern: send(...)
-      - pattern: (...).request(...)
-      - pattern: request(...)
-      - pattern: (...).urlopen(...)
-      - pattern: urlopen(...)
-      - pattern: (...).getresponse(...)
-      - pattern: getresponse(...)
-      - pattern: requests.$FUNC(...)
-      - pattern: (...).urlretrieve(...)
-      - pattern: urlretrieve(...)
-      - pattern: requests.get(...)
+      - pattern: |
+          (...).request(...)
+          ...
+      - pattern: |
+          request(...)
+          ...
+      - pattern: |
+          (...).urlopen(...)
+          ...
+      - pattern: |
+          urlopen(...)
+          ...
+      - pattern: |
+          (...).getresponse(...)
+          ...
+      - pattern: |
+          getresponse(...)
+          ...
+      - pattern: |
+          requests.$FUNC(...)
+          ...
+      - pattern: |
+          (...).urlretrieve(...)
+          ...
+      - pattern: |
+          urlretrieve(...)
+          ...
+      - pattern: |
+          requests.get(...)
+          ...
     severity: WARNING
     options: 
       symbolic_propagation: true
```

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/exec-base64.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/npm-exec-base64.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/npm-exfiltrate-sensitive-data.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-exfiltrate-sensitive-data.yml`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
       description: Identify when a package reads and exfiltrates sensitive data from
         the local system
     pattern-sources:
       - pattern-either:
           - patterns:              
             - pattern-either:
               - pattern: process.env
-          - patterns:              
-            - pattern-either:
+          - patterns:  
+            - pattern-either: # after defining fs
                 - pattern-inside: |
                     $FS = require('fs')
                     ...
                 - pattern-inside: |
                     $FS = require('fs/promises')
                     ...
                 - pattern-inside: |
@@ -26,24 +26,31 @@
                     ...
                 - pattern-inside: |
                     import * as $FS from 'fs/promises'
                     ...
                 - pattern-inside: |
                     import $FS from 'fs/promises'
                     ...
-            - patterns:
-                - pattern-either:
-                    - pattern: $FS. ... .readFileSync(...,<..."$FILE"...>,...)
-                    - pattern: $FS. ... .readFile(...,<..."$FILE"...>,...)
-                    - pattern: $FS. ... .open(...,<..."$FILE"...>,...)
-                    - pattern: $FS. ... .access(...,<..."$FILE"...>,...)
-                    - pattern: $FS. ... .createReadStream(...,<..."$FILE"...>,...)
-                - metavariable-regex:
-                    metavariable: $FILE
-                    regex: (/etc/passwd|.aws/credentials|.docker/config.json|/.kube/config|/etc/hosts/.ssh/id_rsa)
+            - pattern-either: 
+                # match use of ootb functions
+                - pattern: $FS. ... .homedir()
+                - pattern: $FS. ... .hostname()
+                - pattern: $FS. ... .userInfo()
+
+                # match access to sensitive files
+                - patterns:
+                    - pattern-either:
+                        - pattern: $FS. ... .readFileSync(...,<..."$FILE"...>,...)
+                        - pattern: $FS. ... .readFile(...,<..."$FILE"...>,...)
+                        - pattern: $FS. ... .open(...,<..."$FILE"...>,...)
+                        - pattern: $FS. ... .access(...,<..."$FILE"...>,...)
+                        - pattern: $FS. ... .createReadStream(...,<..."$FILE"...>,...)
+                    - metavariable-regex:
+                        metavariable: $FILE
+                        regex: (/etc/passwd|.aws/credentials|.docker/config.json|/.kube/config|/etc/hosts/.ssh/id_rsa)
         
     pattern-sinks:
       - patterns:
           - pattern-either:
               - pattern-inside: |
                   $HTTP = require('https')
                   ...
```

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/npm-install-script.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-install-script.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/npm-obfuscation.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-obfuscation.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/npm-serialize-environment.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-serialize-environment.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/obfuscation.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/obfuscation.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/analyzer/sourcecode/steganography.yml` & `guarddog-1.8.0/guarddog/analyzer/sourcecode/steganography.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/cli.py` & `guarddog-1.8.0/guarddog/cli.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/reporters/sarif.py` & `guarddog-1.8.0/guarddog/reporters/sarif.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/scanners/__init__.py` & `guarddog-1.8.0/guarddog/scanners/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/scanners/npm_package_scanner.py` & `guarddog-1.8.0/guarddog/scanners/npm_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/scanners/npm_project_scanner.py` & `guarddog-1.8.0/guarddog/scanners/npm_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/scanners/pypi_package_scanner.py` & `guarddog-1.8.0/guarddog/scanners/pypi_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/scanners/pypi_project_scanner.py` & `guarddog-1.8.0/guarddog/scanners/pypi_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/scanners/scanner.py` & `guarddog-1.8.0/guarddog/scanners/scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/utils/archives.py` & `guarddog-1.8.0/guarddog/utils/archives.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/guarddog/utils/package_info.py` & `guarddog-1.8.0/guarddog/utils/package_info.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.7.0/pyproject.toml` & `guarddog-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "guarddog"
 description = "GuardDog is a CLI tool to Identify malicious PyPI packages"
 authors = ["Ellen Wang", "Christophe Tafani-Dereeper"]
 license = "Apache-2.0"
 readme = "pypi.rst"
 repository = "https://github.com/DataDog/guarddog"
-version = "v1.7.0"
+version = "v1.8.0"
 
 [tool.poetry.scripts]
 guarddog = "guarddog.cli:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 semgrep = "1.67.0"
@@ -21,15 +21,15 @@
 urllib3 = "2.2.1"
 python-whois = ">=0.8,<0.10"
 termcolor = "^2.1.0"
 tarsafe = "^0.0.5"
 semantic-version = "^2.10.0"
 pyyaml = "^6.0"
 # 1.12+ requires new version of libgit2 which is not avaiable in Alpine
-pygit2 = ">=1.11,<1.15"
+pygit2 = ">=1.11,<1.16"
 configparser = ">=5.3,<8.0"
 prettytable="^3.6.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.4.1"
 coverage = "^7.2.7"
 flake8 = ">=5.0.4,<8.0.0"
```

### Comparing `guarddog-1.7.0/PKG-INFO` & `guarddog-1.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guarddog
-Version: 1.7.0
+Version: 1.8.0
 Summary: GuardDog is a CLI tool to Identify malicious PyPI packages
 Home-page: https://github.com/DataDog/guarddog
 License: Apache-2.0
 Author: Ellen Wang
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-option-group (>=0.5.5,<0.6.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: configparser (>=5.3,<8.0)
 Requires-Dist: prettytable (>=3.6.0,<4.0.0)
-Requires-Dist: pygit2 (>=1.11,<1.15)
+Requires-Dist: pygit2 (>=1.11,<1.16)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-whois (>=0.8,<0.10)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
 Requires-Dist: semgrep (==1.67.0)
 Requires-Dist: tarsafe (>=0.0.5,<0.0.6)
```

