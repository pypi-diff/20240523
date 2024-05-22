# Comparing `tmp/uv-0.2.0.tar.gz` & `tmp/uv-0.2.1.tar.gz`

## Comparing `uv-0.2.0.tar` & `uv-0.2.1.tar`

### file list

```diff
@@ -1,391 +1,391 @@
--rw-r--r--   0     1001      127      284 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-normalize/Cargo.toml
--rw-r--r--   0     1001      127     1620 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-normalize/src/extra_name.rs
--rw-r--r--   0     1001      127     5633 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-normalize/src/lib.rs
--rw-r--r--   0     1001      127     2847 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-normalize/src/package_name.rs
--rw-r--r--   0     1001      127     2046 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/Cargo.toml
--rw-r--r--   0     1001      127        1 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/bare.rs
--rw-r--r--   0     1001      127    17958 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/candidate_selector.rs
--rw-r--r--   0     1001      127      610 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/dependency_mode.rs
--rw-r--r--   0     1001      127     1140 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/dependency_provider.rs
--rw-r--r--   0     1001      127     1378 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/editables.rs
--rw-r--r--   0     1001      127    13709 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/error.rs
--rw-r--r--   0     1001      127     2743 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/exclude_newer.rs
--rw-r--r--   0     1001      127     1551 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/exclusions.rs
--rw-r--r--   0     1001      127     8000 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/flat_index.rs
--rw-r--r--   0     1001      127     1260 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/lib.rs
--rw-r--r--   0     1001      127    54297 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/lock.rs
--rw-r--r--   0     1001      127     8769 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/manifest.rs
--rw-r--r--   0     1001      127    12444 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/marker.rs
--rw-r--r--   0     1001      127     2149 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/options.rs
--rw-r--r--   0     1001      127     1122 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/pins.rs
--rw-r--r--   0     1001      127     6368 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/preferences.rs
--rw-r--r--   0     1001      127     4046 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/prerelease_mode.rs
--rw-r--r--   0     1001      127    12211 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/pubgrub/dependencies.rs
--rw-r--r--   0     1001      127     1088 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/pubgrub/distribution.rs
--rw-r--r--   0     1001      127      541 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/pubgrub/mod.rs
--rw-r--r--   0     1001      127     7814 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/pubgrub/package.rs
--rw-r--r--   0     1001      127     5707 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/pubgrub/priority.rs
--rw-r--r--   0     1001      127    40255 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/pubgrub/report.rs
--rw-r--r--   0     1001      127     4890 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/pubgrub/specifier.rs
--rw-r--r--   0     1001      127     1163 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/python_requirement.rs
--rw-r--r--   0     1001      127     4971 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/redirect.rs
--rw-r--r--   0     1001      127    11323 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/resolution/display.rs
--rw-r--r--   0     1001      127    24688 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/resolution/graph.rs
--rw-r--r--   0     1001      127     4444 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/resolution/mod.rs
--rw-r--r--   0     1001      127     1878 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/resolution_mode.rs
--rw-r--r--   0     1001      127     8210 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/resolver/batch_prefetch.rs
--rw-r--r--   0     1001      127     1172 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/resolver/index.rs
--rw-r--r--   0     1001      127    14010 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/resolver/locals.rs
--rw-r--r--   0     1001      127    66870 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/resolver/mod.rs
--rw-r--r--   0     1001      127     8756 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/resolver/provider.rs
--rw-r--r--   0     1001      127     1673 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/resolver/reporter.rs
--rw-r--r--   0     1001      127     8952 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/resolver/urls.rs
--rw-r--r--   0     1001      127     3280 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_optional_missing.snap
--rw-r--r--   0     1001      127      437 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_required_present.snap
--rw-r--r--   0     1001      127    23582 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/version_map.rs
--rw-r--r--   0     1001      127     1752 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/src/yanks.rs
--rw-r--r--   0     1001      127    22764 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-resolver/tests/resolver.rs
--rw-r--r--   0     1001      127      507 2024-05-22 18:48:21.000000 uv-0.2.0/crates/cache-key/Cargo.toml
--rw-r--r--   0     1001      127     8335 2024-05-22 18:48:21.000000 uv-0.2.0/crates/cache-key/src/cache_key.rs
--rw-r--r--   0     1001      127    12317 2024-05-22 18:48:21.000000 uv-0.2.0/crates/cache-key/src/canonical_url.rs
--rw-r--r--   0     1001      127      620 2024-05-22 18:48:21.000000 uv-0.2.0/crates/cache-key/src/digest.rs
--rw-r--r--   0     1001      127      191 2024-05-22 18:48:21.000000 uv-0.2.0/crates/cache-key/src/lib.rs
--rw-r--r--   0     1001      127     1986 2024-05-22 18:48:21.000000 uv-0.2.0/crates/cache-key/src/stable_hash.rs
--rw-r--r--   0     1001      127     2085 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep508-rs/Cargo.toml
--rw-r--r--   0     1001      127    10173 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep508-rs/License-Apache
--rw-r--r--   0     1001      127     1293 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep508-rs/License-BSD
--rw-r--r--   0     1001      127     3039 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep508-rs/Readme.md
--rw-r--r--   0     1001      127     4301 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep508-rs/src/cursor.rs
--rw-r--r--   0     1001      127    62005 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep508-rs/src/lib.rs
--rw-r--r--   0     1001      127    94653 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep508-rs/src/marker.rs
--rw-r--r--   0     1001      127      743 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep508-rs/src/origin.rs
--rw-r--r--   0     1001      127    12553 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep508-rs/src/unnamed.rs
--rw-r--r--   0     1001      127    18647 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep508-rs/src/verbatim_url.rs
--rw-r--r--   0     1001      127      752 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-auth/Cargo.toml
--rw-r--r--   0     1001      127     9542 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-auth/src/cache.rs
--rw-r--r--   0     1001      127    11219 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-auth/src/credentials.rs
--rw-r--r--   0     1001      127     9340 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-auth/src/keyring.rs
--rw-r--r--   0     1001      127      992 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-auth/src/lib.rs
--rw-r--r--   0     1001      127    45581 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-auth/src/middleware.rs
--rw-r--r--   0     1001      127     4661 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-auth/src/realm.rs
--rw-r--r--   0     1001      127      456 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-warnings/Cargo.toml
--rw-r--r--   0     1001      127     1701 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-warnings/src/lib.rs
--rw-r--r--   0     1001      127     1025 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-cache/Cargo.toml
--rw-r--r--   0     1001      127      509 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-cache/src/archive.rs
--rw-r--r--   0     1001      127      195 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-cache/src/by_timestamp.rs
--rw-r--r--   0     1001      127     1768 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-cache/src/cli.rs
--rw-r--r--   0     1001      127    35224 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-cache/src/lib.rs
--rw-r--r--   0     1001      127     6138 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-cache/src/removal.rs
--rw-r--r--   0     1001      127     1663 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-cache/src/timestamp.rs
--rw-r--r--   0     1001      127     2538 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-cache/src/wheel.rs
--rw-r--r--   0     1001      127      411 2024-05-22 18:48:21.000000 uv-0.2.0/crates/once-map/Cargo.toml
--rw-r--r--   0     1001      127     3940 2024-05-22 18:48:21.000000 uv-0.2.0/crates/once-map/src/lib.rs
--rw-r--r--   0     1001      127     1654 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-requirements/Cargo.toml
--rw-r--r--   0     1001      127     2206 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-requirements/src/confirm.rs
--rw-r--r--   0     1001      127      318 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-requirements/src/lib.rs
--rw-r--r--   0     1001      127    10108 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-requirements/src/lookahead.rs
--rw-r--r--   0     1001      127    31011 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-requirements/src/pyproject.rs
--rw-r--r--   0     1001      127     6877 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-requirements/src/source_tree.rs
--rw-r--r--   0     1001      127     7083 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-requirements/src/sources.rs
--rw-r--r--   0     1001      127    14908 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-requirements/src/specification.rs
--rw-r--r--   0     1001      127    13090 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-requirements/src/unnamed.rs
--rw-r--r--   0     1001      127     1638 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-requirements/src/upgrade.rs
--rw-r--r--   0     1001      127    25085 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-requirements/src/workspace.rs
--rw-r--r--   0     1001      127      608 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-filename/Cargo.toml
--rw-r--r--   0     1001      127     2291 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-filename/src/lib.rs
--rw-r--r--   0     1001      127      420 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_build_tag.snap
--rw-r--r--   0     1001      127      539 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap
--rw-r--r--   0     1001      127      398 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_single_tags.snap
--rw-r--r--   0     1001      127     7565 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-filename/src/source_dist.rs
--rw-r--r--   0     1001      127    10961 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-filename/src/wheel.rs
--rw-r--r--   0     1001      127      322 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-version/Cargo.toml
--rw-r--r--   0     1001      127      355 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-version/src/lib.rs
--rw-r--r--   0     1001      127     1004 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep440-rs/Cargo.toml
--rw-r--r--   0     1001      127    10173 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep440-rs/License-Apache
--rw-r--r--   0     1001      127     1293 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep440-rs/License-BSD
--rw-r--r--   0     1001      127     2947 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep440-rs/Readme.md
--rw-r--r--   0     1001      127     2105 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep440-rs/python/Readme.md
--rw-r--r--   0     1001      127     2922 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep440-rs/src/lib.rs
--rw-r--r--   0     1001      127   131052 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep440-rs/src/version.rs
--rw-r--r--   0     1001      127    56892 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pep440-rs/src/version_specifier.rs
--rw-r--r--   0     1001      127     1504 2024-05-22 18:48:21.000000 uv-0.2.0/crates/install-wheel-rs/Cargo.toml
--rw-r--r--   0     1001      127      515 2024-05-22 18:48:21.000000 uv-0.2.0/crates/install-wheel-rs/Readme.md
--rw-r--r--   0     1001      127     4332 2024-05-22 18:48:21.000000 uv-0.2.0/crates/install-wheel-rs/src/lib.rs
--rw-r--r--   0     1001      127    20181 2024-05-22 18:48:21.000000 uv-0.2.0/crates/install-wheel-rs/src/linker.rs
--rw-r--r--   0     1001      127     7104 2024-05-22 18:48:21.000000 uv-0.2.0/crates/install-wheel-rs/src/metadata.rs
--rw-r--r--   0     1001      127      474 2024-05-22 18:48:21.000000 uv-0.2.0/crates/install-wheel-rs/src/record.rs
--rw-r--r--   0     1001      127     5550 2024-05-22 18:48:21.000000 uv-0.2.0/crates/install-wheel-rs/src/script.rs
--rw-r--r--   0     1001      127    11211 2024-05-22 18:48:21.000000 uv-0.2.0/crates/install-wheel-rs/src/uninstall.rs
--rw-r--r--   0     1001      127    34841 2024-05-22 18:48:21.000000 uv-0.2.0/crates/install-wheel-rs/src/wheel.rs
--rw-r--r--   0     1001      127      847 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-fs/Cargo.toml
--rw-r--r--   0     1001      127     1397 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-fs/src/cachedir.rs
--rw-r--r--   0     1001      127    11067 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-fs/src/lib.rs
--rw-r--r--   0     1001      127    10859 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-fs/src/path.rs
--rw-r--r--   0     1001      127     1807 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/Cargo.toml
--rw-r--r--   0     1001      127      112 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/README.md
--rw-r--r--   0     1001      127     7109 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/src/base_client.rs
--rw-r--r--   0     1001      127    30512 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/src/cached_client.rs
--rw-r--r--   0     1001      127    10417 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/src/error.rs
--rw-r--r--   0     1001      127     9211 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/src/flat_index.rs
--rw-r--r--   0     1001      127    46032 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/src/html.rs
--rw-r--r--   0     1001      127    29250 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/src/httpcache/control.rs
--rw-r--r--   0     1001      127    60607 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/src/httpcache/mod.rs
--rw-r--r--   0     1001      127      648 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/src/lib.rs
--rw-r--r--   0     1001      127     5110 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/src/linehaul.rs
--rw-r--r--   0     1001      127     1228 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/src/middleware.rs
--rw-r--r--   0     1001      127    35668 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/src/registry_client.rs
--rw-r--r--   0     1001      127     4579 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/src/remote_metadata.rs
--rw-r--r--   0     1001      127    12019 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/src/rkyvutil.rs
--rw-r--r--   0     1001      127     1146 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/tests/remote_metadata.rs
--rw-r--r--   0     1001      127     8183 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-client/tests/user_agent_version.rs
--rw-r--r--   0     1001      127     1183 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/Cargo.toml
--rw-r--r--   0     1001      127     2511 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/annotation.rs
--rw-r--r--   0     1001      127     1048 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/any.rs
--rw-r--r--   0     1001      127     4711 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/buildable.rs
--rw-r--r--   0     1001      127     6718 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/cached.rs
--rw-r--r--   0     1001      127     2474 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/editable.rs
--rw-r--r--   0     1001      127      985 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/error.rs
--rw-r--r--   0     1001      127     7205 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/file.rs
--rw-r--r--   0     1001      127     2831 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/hash.rs
--rw-r--r--   0     1001      127     3845 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/id.rs
--rw-r--r--   0     1001      127    14472 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/index_url.rs
--rw-r--r--   0     1001      127    12536 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/installed.rs
--rw-r--r--   0     1001      127    35260 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/lib.rs
--rw-r--r--   0     1001      127    10788 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/parsed_url.rs
--rw-r--r--   0     1001      127    20821 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/prioritized_distribution.rs
--rw-r--r--   0     1001      127     8302 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/requirement.rs
--rw-r--r--   0     1001      127     1228 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/requirements.rs
--rw-r--r--   0     1001      127     6611 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/resolution.rs
--rw-r--r--   0     1001      127     6410 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/resolved.rs
--rw-r--r--   0     1001      127     3233 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/specified_requirement.rs
--rw-r--r--   0     1001      127     8193 2024-05-22 18:48:21.000000 uv-0.2.0/crates/distribution-types/src/traits.rs
--rw-r--r--   0     1001      127      897 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-extract/Cargo.toml
--rw-r--r--   0     1001      127     1078 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-extract/src/error.rs
--rw-r--r--   0     1001      127     4113 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-extract/src/hash.rs
--rw-r--r--   0     1001      127      112 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-extract/src/lib.rs
--rw-r--r--   0     1001      127     9419 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-extract/src/stream.rs
--rw-r--r--   0     1001      127     3565 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-extract/src/sync.rs
--rw-r--r--   0     1001      127     1489 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-extract/src/tar.rs
--rw-r--r--   0     1001      127     5685 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs
--rw-r--r--   0     1001      127      112 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-extract/src/vendor/mod.rs
--rw-r--r--   0     1001      127      841 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-configuration/Cargo.toml
--rw-r--r--   0     1001      127     1014 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-configuration/src/authentication.rs
--rw-r--r--   0     1001      127    10722 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-configuration/src/build_options.rs
--rw-r--r--   0     1001      127     1054 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-configuration/src/concurrency.rs
--rw-r--r--   0     1001      127     9254 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-configuration/src/config_settings.rs
--rw-r--r--   0     1001      127     1698 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-configuration/src/constraints.rs
--rw-r--r--   0     1001      127      437 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-configuration/src/lib.rs
--rw-r--r--   0     1001      127     4059 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-configuration/src/name_specifiers.rs
--rw-r--r--   0     1001      127     1706 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-configuration/src/overrides.rs
--rw-r--r--   0     1001      127     2339 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-configuration/src/package_options.rs
--rw-r--r--   0     1001      127      782 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-configuration/src/preview.rs
--rw-r--r--   0     1001      127    11893 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-configuration/src/target_triple.rs
--rw-r--r--   0     1001      127      970 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-dispatch/Cargo.toml
--rw-r--r--   0     1001      127    10815 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-dispatch/src/lib.rs
--rw-r--r--   0     1001      127      774 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/Cargo.toml
--rw-r--r--   0     1001      127      109 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/README.md
--rw-r--r--   0     1001      127     4375 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/src/_virtualenv.py
--rw-r--r--   0     1001      127       20 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/src/activator/.gitattributes
--rw-r--r--   0     1001      127     3388 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/src/activator/activate
--rw-r--r--   0     1001      127     2259 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/src/activator/activate.bat
--rw-r--r--   0     1001      127     2655 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/src/activator/activate.csh
--rw-r--r--   0     1001      127     4219 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/src/activator/activate.fish
--rw-r--r--   0     1001      127     3903 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/src/activator/activate.nu
--rw-r--r--   0     1001      127     2826 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/src/activator/activate.ps1
--rw-r--r--   0     1001      127     2411 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/src/activator/activate_this.py
--rw-r--r--   0     1001      127     1728 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/src/activator/deactivate.bat
--rw-r--r--   0     1001      127     1215 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/src/activator/pydoc.bat
--rw-r--r--   0     1001      127    16565 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/src/bare.rs
--rw-r--r--   0     1001      127     2090 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-virtualenv/src/lib.rs
--rw-r--r--   0     1001      127     1464 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-installer/Cargo.toml
--rw-r--r--   0     1001      127    12444 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-installer/src/compile.rs
--rw-r--r--   0     1001      127     9352 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-installer/src/downloader.rs
--rw-r--r--   0     1001      127     4349 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-installer/src/editable.rs
--rw-r--r--   0     1001      127     2833 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-installer/src/installer.rs
--rw-r--r--   0     1001      127      521 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-installer/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-installer/src/pip_compileall.py
--rw-r--r--   0     1001      127    22428 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-installer/src/plan.rs
--rw-r--r--   0     1001      127     7565 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-installer/src/satisfies.rs
--rw-r--r--   0     1001      127    22636 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-installer/src/site_packages.rs
--rw-r--r--   0     1001      127      978 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-installer/src/uninstall.rs
--rw-r--r--   0     1001      127     1145 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-build/Cargo.toml
--rw-r--r--   0     1001      127       17 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-build/.gitignore
--rw-r--r--   0     1001      127    48655 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-build/src/lib.rs
--rw-r--r--   0     1001      127      472 2024-05-22 18:48:21.000000 uv-0.2.0/crates/platform-tags/Cargo.toml
--rw-r--r--   0     1001      127      161 2024-05-22 18:48:21.000000 uv-0.2.0/crates/platform-tags/src/lib.rs
--rw-r--r--   0     1001      127     3507 2024-05-22 18:48:21.000000 uv-0.2.0/crates/platform-tags/src/platform.rs
--rw-r--r--   0     1001      127    76059 2024-05-22 18:48:21.000000 uv-0.2.0/crates/platform-tags/src/tags.rs
--rw-r--r--   0     1001      127      822 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pypi-types/Cargo.toml
--rw-r--r--   0     1001      127     1609 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pypi-types/src/base_url.rs
--rw-r--r--   0     1001      127     4643 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pypi-types/src/direct_url.rs
--rw-r--r--   0     1001      127    15738 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pypi-types/src/lenient_requirement.rs
--rw-r--r--   0     1001      127      239 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pypi-types/src/lib.rs
--rw-r--r--   0     1001      127    19433 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pypi-types/src/metadata.rs
--rw-r--r--   0     1001      127      575 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pypi-types/src/scheme.rs
--rw-r--r--   0     1001      127    12178 2024-05-22 18:48:21.000000 uv-0.2.0/crates/pypi-types/src/simple_json.rs
--rw-r--r--   0     1001      127     1808 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/Cargo.toml
--rwxr-xr-x   0     1001      127     7922 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/fetch-version-metadata.py
--rw-r--r--   0     1001      127        0 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/python/__init__.py
--rw-r--r--   0     1001      127    21931 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/python/get_interpreter_info.py
--rw-r--r--   0     1001      127    10174 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/python/packaging/LICENSE.APACHE
--rw-r--r--   0     1001      127     1344 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/python/packaging/LICENSE.BSD
--rw-r--r--   0     1001      127      316 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/python/packaging/README.md
--rw-r--r--   0     1001      127      501 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/python/packaging/__init__.py
--rw-r--r--   0     1001      127     3282 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/python/packaging/_elffile.py
--rw-r--r--   0     1001      127     9588 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/python/packaging/_manylinux.py
--rw-r--r--   0     1001      127     2696 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/python/packaging/_musllinux.py
--rw-r--r--   0     1001      127   182247 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/python-version-metadata.json
--rw-r--r--   0     1001      127    53798 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/discovery.rs
--rw-r--r--   0     1001      127     8765 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/environment.rs
--rw-r--r--   0     1001      127     1314 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/implementation.rs
--rw-r--r--   0     1001      127    27969 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/interpreter.rs
--rw-r--r--   0     1001      127    74107 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/lib.rs
--rw-r--r--   0     1001      127     8104 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/managed/downloads.rs
--rw-r--r--   0     1001      127     5960 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/managed/find.rs
--rw-r--r--   0     1001      127      253 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/managed/mod.rs
--rw-r--r--   0     1001      127   224411 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/managed/python_versions.inc
--rw-r--r--   0     1001      127      691 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/managed/python_versions.inc.mustache
--rw-r--r--   0     1001      127     4389 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/platform.rs
--rw-r--r--   0     1001      127      430 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/pointer_size.rs
--rw-r--r--   0     1001      127     3234 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/py_launcher.rs
--rw-r--r--   0     1001      127     7736 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/python_version.rs
--rw-r--r--   0     1001      127      950 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/target.rs
--rw-r--r--   0     1001      127     5511 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/src/virtualenv.rs
--rw-r--r--   0     1001      127     2708 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-interpreter/template-version-metadata.py
--rw-r--r--   0     1001      127     1002 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-workspace/Cargo.toml
--rw-r--r--   0     1001      127     7241 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-workspace/src/combine.rs
--rw-r--r--   0     1001      127      127 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-workspace/src/lib.rs
--rw-r--r--   0     1001      127     3296 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-workspace/src/settings.rs
--rw-r--r--   0     1001      127     5558 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-workspace/src/workspace.rs
--rw-r--r--   0     1001      127     1528 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/Cargo.toml
--rw-r--r--   0     1001      127      684 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/archive.rs
--rw-r--r--   0     1001      127    34434 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/distribution_database.rs
--rw-r--r--   0     1001      127     2185 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/download.rs
--rw-r--r--   0     1001      127     7053 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/error.rs
--rw-r--r--   0     1001      127    10371 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/git.rs
--rw-r--r--   0     1001      127     7145 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/index/built_wheel_index.rs
--rw-r--r--   0     1001      127     3435 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/index/cached_wheel.rs
--rw-r--r--   0     1001      127      162 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/index/mod.rs
--rw-r--r--   0     1001      127     8729 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/index/registry_wheel_index.rs
--rw-r--r--   0     1001      127      965 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/lib.rs
--rw-r--r--   0     1001      127      600 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/locks.rs
--rw-r--r--   0     1001      127     1225 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/reporter.rs
--rw-r--r--   0     1001      127     2029 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/source/built_wheel_metadata.rs
--rw-r--r--   0     1001      127    60426 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/source/mod.rs
--rw-r--r--   0     1001      127     1998 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-distribution/src/source/revision.rs
--rw-r--r--   0     1001      127     1223 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/Cargo.toml
--rw-r--r--   0     1001      127    88063 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/lib.rs
--rw-r--r--   0     1001      127     2237 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/requirement.rs
--rw-r--r--   0     1001      127     6200 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap
--rw-r--r--   0     1001      127     2683 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap
--rw-r--r--   0     1001      127     2273 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap
--rw-r--r--   0     1001      127      284 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-empty.txt.snap
--rw-r--r--   0     1001      127     4140 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap
--rw-r--r--   0     1001      127     1816 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap
--rw-r--r--   0     1001      127      828 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap
--rw-r--r--   0     1001      127    11863 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap
--rw-r--r--   0     1001      127     2257 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap
--rw-r--r--   0     1001      127     2544 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap
--rw-r--r--   0     1001      127     6200 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap
--rw-r--r--   0     1001      127     2683 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap
--rw-r--r--   0     1001      127     2273 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap
--rw-r--r--   0     1001      127      284 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-empty.txt.snap
--rw-r--r--   0     1001      127     4140 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap
--rw-r--r--   0     1001      127     1816 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap
--rw-r--r--   0     1001      127      828 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap
--rw-r--r--   0     1001      127    11863 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap
--rw-r--r--   0     1001      127     2257 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap
--rw-r--r--   0     1001      127     3692 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-bare-url.txt.snap
--rw-r--r--   0     1001      127     8155 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-editable.txt.snap
--rw-r--r--   0     1001      127     2544 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap
--rw-r--r--   0     1001      127     3713 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-bare-url.txt.snap
--rw-r--r--   0     1001      127     8161 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-editable.txt.snap
--rw-r--r--   0     1001      127      113 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/test-data/requirements-txt/bare-url.txt
--rw-r--r--   0     1001      127       90 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/test-data/requirements-txt/basic.txt
--rw-r--r--   0     1001      127       45 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/test-data/requirements-txt/constraints-a.txt
--rw-r--r--   0     1001      127       27 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/test-data/requirements-txt/constraints-b.txt
--rw-r--r--   0     1001      127      491 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/test-data/requirements-txt/editable.txt
--rw-r--r--   0     1001      127        0 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/test-data/requirements-txt/empty.txt
--rw-r--r--   0     1001      127      101 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/test-data/requirements-txt/for-poetry.txt
--rw-r--r--   0     1001      127       43 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/test-data/requirements-txt/include-a.txt
--rw-r--r--   0     1001      127        5 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/test-data/requirements-txt/include-b.txt
--rw-r--r--   0     1001      127     1183 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt
--rw-r--r--   0     1001      127       66 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/test-data/requirements-txt/small.txt
--rw-r--r--   0     1001      127      183 2024-05-22 18:48:21.000000 uv-0.2.0/crates/requirements-txt/test-data/requirements-txt/whitespace.txt
--rw-r--r--   0     1001      127      918 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-git/Cargo.toml
--rw-r--r--   0     1001      127    63247 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-git/src/git.rs
--rw-r--r--   0     1001      127    37494 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-git/src/known_hosts.rs
--rw-r--r--   0     1001      127     3843 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-git/src/lib.rs
--rw-r--r--   0     1001      127      940 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-git/src/sha.rs
--rw-r--r--   0     1001      127     5058 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-git/src/source.rs
--rw-r--r--   0     1001      127     1362 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-git/src/util/errors.rs
--rw-r--r--   0     1001      127      733 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-git/src/util/mod.rs
--rw-r--r--   0     1001      127     7295 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-git/src/util/retry.rs
--rw-r--r--   0     1001      127      790 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-types/Cargo.toml
--rw-r--r--   0     1001      127      423 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-types/src/builds.rs
--rw-r--r--   0     1001      127      239 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-types/src/downloads.rs
--rw-r--r--   0     1001      127     6228 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-types/src/hash.rs
--rw-r--r--   0     1001      127      219 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-types/src/lib.rs
--rw-r--r--   0     1001      127     1478 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-types/src/requirements.rs
--rw-r--r--   0     1001      127     6912 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv-types/src/traits.rs
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 uv-0.2.0/crates/uv/Cargo.toml
--rw-r--r--   0     1001      127     3065 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/build.rs
--rw-r--r--   0     1001      127    79305 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/cli.rs
--rw-r--r--   0     1001      127     4158 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/cache_clean.rs
--rw-r--r--   0     1001      127      213 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/cache_dir.rs
--rw-r--r--   0     1001      127     1955 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/cache_prune.rs
--rw-r--r--   0     1001      127     4868 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/mod.rs
--rw-r--r--   0     1001      127     2316 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/pip/check.rs
--rw-r--r--   0     1001      127    28556 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/pip/compile.rs
--rw-r--r--   0     1001      127     2462 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/pip/freeze.rs
--rw-r--r--   0     1001      127    16730 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/pip/install.rs
--rw-r--r--   0     1001      127     6301 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/pip/list.rs
--rw-r--r--   0     1001      127      198 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/pip/mod.rs
--rw-r--r--   0     1001      127    24504 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/pip/operations.rs
--rw-r--r--   0     1001      127     6601 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/pip/show.rs
--rw-r--r--   0     1001      127    14121 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/pip/sync.rs
--rw-r--r--   0     1001      127     7279 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/pip/uninstall.rs
--rw-r--r--   0     1001      127     5135 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/project/lock.rs
--rw-r--r--   0     1001      127    19397 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/project/mod.rs
--rw-r--r--   0     1001      127     5914 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/project/run.rs
--rw-r--r--   0     1001      127     3663 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/project/sync.rs
--rw-r--r--   0     1001      127    10251 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/reporters.rs
--rw-r--r--   0     1001      127     3965 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/self_update.rs
--rw-r--r--   0     1001      127       20 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/tool/mod.rs
--rw-r--r--   0     1001      127     4227 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/tool/run.rs
--rw-r--r--   0     1001      127    10652 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/venv.rs
--rw-r--r--   0     1001      127      570 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/commands/version.rs
--rw-r--r--   0     1001      127    11263 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/compat/mod.rs
--rw-r--r--   0     1001      127     7723 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/editables.rs
--rw-r--r--   0     1001      127     7604 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/logging.rs
--rw-r--r--   0     1001      127    24207 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/main.rs
--rw-r--r--   0     1001      127     2326 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/printer.rs
--rw-r--r--   0     1001      127    38621 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/settings.rs
--rw-r--r--   0     1001      127     2844 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/shell.rs
--rw-r--r--   0     1001      127     4816 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/src/version.rs
--rw-r--r--   0     1001      127     4437 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/cache_prune.rs
--rw-r--r--   0     1001      127    21602 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/common/mod.rs
--rw-r--r--   0     1001      127    27008 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/lock.rs
--rw-r--r--   0     1001      127     6060 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/pip_check.rs
--rw-r--r--   0     1001      127   305128 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/pip_compile.rs
--rw-r--r--   0     1001      127    19016 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/pip_compile_scenarios.rs
--rw-r--r--   0     1001      127     8341 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/pip_freeze.rs
--rw-r--r--   0     1001      127   151838 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/pip_install.rs
--rw-r--r--   0     1001      127   159295 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/pip_install_scenarios.rs
--rw-r--r--   0     1001      127    18430 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/pip_list.rs
--rw-r--r--   0     1001      127    13190 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/pip_show.rs
--rw-r--r--   0     1001      127   162257 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/pip_sync.rs
--rw-r--r--   0     1001      127    14234 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/pip_uninstall.rs
--rw-r--r--   0     1001      127     1254 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/self_update.rs
--rw-r--r--   0     1001      127    18144 2024-05-22 18:48:21.000000 uv-0.2.0/crates/uv/tests/venv.rs
--rw-r--r--   0     1001      127   134744 2024-05-22 18:48:21.000000 uv-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     8871 1970-01-01 00:00:00.000000 uv-0.2.0/Cargo.toml
--rw-r--r--   0     1001      127     2366 2024-05-22 18:48:21.000000 uv-0.2.0/pyproject.toml
--rw-r--r--   0     1001      127     1055 2024-05-22 18:48:21.000000 uv-0.2.0/python/uv/__main__.py
--rw-r--r--   0     1001      127      806 2024-05-22 18:48:21.000000 uv-0.2.0/python/uv/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-22 18:48:21.000000 uv-0.2.0/python/uv/py.typed
--rw-r--r--   0     1001      127    31568 2024-05-22 18:48:21.000000 uv-0.2.0/README.md
--rw-r--r--   0     1001      127       29 2024-05-22 18:48:21.000000 uv-0.2.0/rust-toolchain.toml
--rw-r--r--   0     1001      127    11356 2024-05-22 18:48:21.000000 uv-0.2.0/LICENSE-APACHE
--rw-r--r--   0     1001      127     1077 2024-05-22 18:48:21.000000 uv-0.2.0/LICENSE-MIT
--rw-r--r--   0        0        0    32935 1970-01-01 00:00:00.000000 uv-0.2.0/PKG-INFO
+-rw-r--r--   0     1001      127     1149 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/Cargo.toml
+-rw-r--r--   0     1001      127     2511 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/annotation.rs
+-rw-r--r--   0     1001      127     1048 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/any.rs
+-rw-r--r--   0     1001      127     4711 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/buildable.rs
+-rw-r--r--   0     1001      127     6718 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/cached.rs
+-rw-r--r--   0     1001      127     2474 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/editable.rs
+-rw-r--r--   0     1001      127      985 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/error.rs
+-rw-r--r--   0     1001      127     7205 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/file.rs
+-rw-r--r--   0     1001      127     2831 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/hash.rs
+-rw-r--r--   0     1001      127     3845 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/id.rs
+-rw-r--r--   0     1001      127    14472 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/index_url.rs
+-rw-r--r--   0     1001      127    12536 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/installed.rs
+-rw-r--r--   0     1001      127    35260 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/lib.rs
+-rw-r--r--   0     1001      127    10788 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/parsed_url.rs
+-rw-r--r--   0     1001      127    20821 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/prioritized_distribution.rs
+-rw-r--r--   0     1001      127     8302 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/requirement.rs
+-rw-r--r--   0     1001      127     1228 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/requirements.rs
+-rw-r--r--   0     1001      127     6132 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/resolution.rs
+-rw-r--r--   0     1001      127     6410 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/resolved.rs
+-rw-r--r--   0     1001      127     3233 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/specified_requirement.rs
+-rw-r--r--   0     1001      127     8193 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-types/src/traits.rs
+-rw-r--r--   0     1001      127      608 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-filename/Cargo.toml
+-rw-r--r--   0     1001      127     2291 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-filename/src/lib.rs
+-rw-r--r--   0     1001      127      420 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_build_tag.snap
+-rw-r--r--   0     1001      127      539 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap
+-rw-r--r--   0     1001      127      398 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_single_tags.snap
+-rw-r--r--   0     1001      127     7565 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-filename/src/source_dist.rs
+-rw-r--r--   0     1001      127    10961 2024-05-22 20:09:33.000000 uv-0.2.1/crates/distribution-filename/src/wheel.rs
+-rw-r--r--   0     1001      127     1654 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-requirements/Cargo.toml
+-rw-r--r--   0     1001      127     2206 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-requirements/src/confirm.rs
+-rw-r--r--   0     1001      127      318 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-requirements/src/lib.rs
+-rw-r--r--   0     1001      127    10108 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-requirements/src/lookahead.rs
+-rw-r--r--   0     1001      127    31011 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-requirements/src/pyproject.rs
+-rw-r--r--   0     1001      127     6877 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-requirements/src/source_tree.rs
+-rw-r--r--   0     1001      127     7083 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-requirements/src/sources.rs
+-rw-r--r--   0     1001      127    14908 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-requirements/src/specification.rs
+-rw-r--r--   0     1001      127    13090 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-requirements/src/unnamed.rs
+-rw-r--r--   0     1001      127     1638 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-requirements/src/upgrade.rs
+-rw-r--r--   0     1001      127    25085 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-requirements/src/workspace.rs
+-rw-r--r--   0     1001      127     1145 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-build/Cargo.toml
+-rw-r--r--   0     1001      127       17 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-build/.gitignore
+-rw-r--r--   0     1001      127    48655 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-build/src/lib.rs
+-rw-r--r--   0     1001      127      322 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-version/Cargo.toml
+-rw-r--r--   0     1001      127      355 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-version/src/lib.rs
+-rw-r--r--   0     1001      127     1002 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-workspace/Cargo.toml
+-rw-r--r--   0     1001      127     7241 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-workspace/src/combine.rs
+-rw-r--r--   0     1001      127      127 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-workspace/src/lib.rs
+-rw-r--r--   0     1001      127     3296 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-workspace/src/settings.rs
+-rw-r--r--   0     1001      127     5558 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-workspace/src/workspace.rs
+-rw-r--r--   0     1001      127      456 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-warnings/Cargo.toml
+-rw-r--r--   0     1001      127     1701 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-warnings/src/lib.rs
+-rw-r--r--   0     1001      127     1223 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/Cargo.toml
+-rw-r--r--   0     1001      127    88063 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/lib.rs
+-rw-r--r--   0     1001      127     2237 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/requirement.rs
+-rw-r--r--   0     1001      127     6200 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap
+-rw-r--r--   0     1001      127     2683 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap
+-rw-r--r--   0     1001      127     2273 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap
+-rw-r--r--   0     1001      127      284 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-empty.txt.snap
+-rw-r--r--   0     1001      127     4140 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap
+-rw-r--r--   0     1001      127     1816 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap
+-rw-r--r--   0     1001      127      828 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap
+-rw-r--r--   0     1001      127    11863 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap
+-rw-r--r--   0     1001      127     2257 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap
+-rw-r--r--   0     1001      127     2544 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap
+-rw-r--r--   0     1001      127     6200 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap
+-rw-r--r--   0     1001      127     2683 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap
+-rw-r--r--   0     1001      127     2273 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap
+-rw-r--r--   0     1001      127      284 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-empty.txt.snap
+-rw-r--r--   0     1001      127     4140 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap
+-rw-r--r--   0     1001      127     1816 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap
+-rw-r--r--   0     1001      127      828 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap
+-rw-r--r--   0     1001      127    11863 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap
+-rw-r--r--   0     1001      127     2257 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap
+-rw-r--r--   0     1001      127     3692 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-bare-url.txt.snap
+-rw-r--r--   0     1001      127     8155 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-editable.txt.snap
+-rw-r--r--   0     1001      127     2544 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap
+-rw-r--r--   0     1001      127     3713 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-bare-url.txt.snap
+-rw-r--r--   0     1001      127     8161 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-editable.txt.snap
+-rw-r--r--   0     1001      127      113 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/test-data/requirements-txt/bare-url.txt
+-rw-r--r--   0     1001      127       90 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/test-data/requirements-txt/basic.txt
+-rw-r--r--   0     1001      127       45 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/test-data/requirements-txt/constraints-a.txt
+-rw-r--r--   0     1001      127       27 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/test-data/requirements-txt/constraints-b.txt
+-rw-r--r--   0     1001      127      491 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/test-data/requirements-txt/editable.txt
+-rw-r--r--   0     1001      127        0 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/test-data/requirements-txt/empty.txt
+-rw-r--r--   0     1001      127      101 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/test-data/requirements-txt/for-poetry.txt
+-rw-r--r--   0     1001      127       43 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/test-data/requirements-txt/include-a.txt
+-rw-r--r--   0     1001      127        5 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/test-data/requirements-txt/include-b.txt
+-rw-r--r--   0     1001      127     1183 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt
+-rw-r--r--   0     1001      127       66 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/test-data/requirements-txt/small.txt
+-rw-r--r--   0     1001      127      183 2024-05-22 20:09:33.000000 uv-0.2.1/crates/requirements-txt/test-data/requirements-txt/whitespace.txt
+-rw-r--r--   0     1001      127     2046 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/Cargo.toml
+-rw-r--r--   0     1001      127        1 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/bare.rs
+-rw-r--r--   0     1001      127    17958 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/candidate_selector.rs
+-rw-r--r--   0     1001      127      610 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/dependency_mode.rs
+-rw-r--r--   0     1001      127     1140 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/dependency_provider.rs
+-rw-r--r--   0     1001      127     1378 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/editables.rs
+-rw-r--r--   0     1001      127    13709 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/error.rs
+-rw-r--r--   0     1001      127     2743 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/exclude_newer.rs
+-rw-r--r--   0     1001      127     1551 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/exclusions.rs
+-rw-r--r--   0     1001      127     8000 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/flat_index.rs
+-rw-r--r--   0     1001      127     1260 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/lib.rs
+-rw-r--r--   0     1001      127    54308 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/lock.rs
+-rw-r--r--   0     1001      127     8769 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/manifest.rs
+-rw-r--r--   0     1001      127    12444 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/marker.rs
+-rw-r--r--   0     1001      127     2149 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/options.rs
+-rw-r--r--   0     1001      127     1122 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/pins.rs
+-rw-r--r--   0     1001      127     6368 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/preferences.rs
+-rw-r--r--   0     1001      127     4046 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/prerelease_mode.rs
+-rw-r--r--   0     1001      127    12211 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/pubgrub/dependencies.rs
+-rw-r--r--   0     1001      127     1088 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/pubgrub/distribution.rs
+-rw-r--r--   0     1001      127      541 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/pubgrub/mod.rs
+-rw-r--r--   0     1001      127     7814 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/pubgrub/package.rs
+-rw-r--r--   0     1001      127     5707 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/pubgrub/priority.rs
+-rw-r--r--   0     1001      127    40255 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/pubgrub/report.rs
+-rw-r--r--   0     1001      127     4890 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/pubgrub/specifier.rs
+-rw-r--r--   0     1001      127     1163 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/python_requirement.rs
+-rw-r--r--   0     1001      127     4971 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/redirect.rs
+-rw-r--r--   0     1001      127    11323 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/resolution/display.rs
+-rw-r--r--   0     1001      127    24688 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/resolution/graph.rs
+-rw-r--r--   0     1001      127     4444 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/resolution/mod.rs
+-rw-r--r--   0     1001      127     1878 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/resolution_mode.rs
+-rw-r--r--   0     1001      127     8210 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/resolver/batch_prefetch.rs
+-rw-r--r--   0     1001      127     1172 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/resolver/index.rs
+-rw-r--r--   0     1001      127    14010 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/resolver/locals.rs
+-rw-r--r--   0     1001      127    66870 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/resolver/mod.rs
+-rw-r--r--   0     1001      127     8756 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/resolver/provider.rs
+-rw-r--r--   0     1001      127     1673 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/resolver/reporter.rs
+-rw-r--r--   0     1001      127     8952 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/resolver/urls.rs
+-rw-r--r--   0     1001      127     3280 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_optional_missing.snap
+-rw-r--r--   0     1001      127      437 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_required_present.snap
+-rw-r--r--   0     1001      127    23582 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/version_map.rs
+-rw-r--r--   0     1001      127     1752 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/src/yanks.rs
+-rw-r--r--   0     1001      127    22820 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-resolver/tests/resolver.rs
+-rw-r--r--   0     1001      127      897 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-extract/Cargo.toml
+-rw-r--r--   0     1001      127     1078 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-extract/src/error.rs
+-rw-r--r--   0     1001      127     4113 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-extract/src/hash.rs
+-rw-r--r--   0     1001      127      112 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-extract/src/lib.rs
+-rw-r--r--   0     1001      127     9419 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-extract/src/stream.rs
+-rw-r--r--   0     1001      127     3565 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-extract/src/sync.rs
+-rw-r--r--   0     1001      127     1489 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-extract/src/tar.rs
+-rw-r--r--   0     1001      127     5685 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs
+-rw-r--r--   0     1001      127      112 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-extract/src/vendor/mod.rs
+-rw-r--r--   0     1001      127     1004 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep440-rs/Cargo.toml
+-rw-r--r--   0     1001      127    10173 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep440-rs/License-Apache
+-rw-r--r--   0     1001      127     1293 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep440-rs/License-BSD
+-rw-r--r--   0     1001      127     2947 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep440-rs/Readme.md
+-rw-r--r--   0     1001      127     2105 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep440-rs/python/Readme.md
+-rw-r--r--   0     1001      127     2922 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep440-rs/src/lib.rs
+-rw-r--r--   0     1001      127   131052 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep440-rs/src/version.rs
+-rw-r--r--   0     1001      127    56892 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep440-rs/src/version_specifier.rs
+-rw-r--r--   0     1001      127      284 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-normalize/Cargo.toml
+-rw-r--r--   0     1001      127     1620 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-normalize/src/extra_name.rs
+-rw-r--r--   0     1001      127     5633 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-normalize/src/lib.rs
+-rw-r--r--   0     1001      127     2847 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-normalize/src/package_name.rs
+-rw-r--r--   0     1001      127     1464 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-installer/Cargo.toml
+-rw-r--r--   0     1001      127    12444 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-installer/src/compile.rs
+-rw-r--r--   0     1001      127     9352 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-installer/src/downloader.rs
+-rw-r--r--   0     1001      127     4349 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-installer/src/editable.rs
+-rw-r--r--   0     1001      127     2833 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-installer/src/installer.rs
+-rw-r--r--   0     1001      127      521 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-installer/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-installer/src/pip_compileall.py
+-rw-r--r--   0     1001      127    22428 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-installer/src/plan.rs
+-rw-r--r--   0     1001      127     7565 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-installer/src/satisfies.rs
+-rw-r--r--   0     1001      127    22636 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-installer/src/site_packages.rs
+-rw-r--r--   0     1001      127      978 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-installer/src/uninstall.rs
+-rw-r--r--   0     1001      127     1808 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/Cargo.toml
+-rwxr-xr-x   0     1001      127     7922 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/fetch-version-metadata.py
+-rw-r--r--   0     1001      127        0 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/python/__init__.py
+-rw-r--r--   0     1001      127    21931 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/python/get_interpreter_info.py
+-rw-r--r--   0     1001      127    10174 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/python/packaging/LICENSE.APACHE
+-rw-r--r--   0     1001      127     1344 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/python/packaging/LICENSE.BSD
+-rw-r--r--   0     1001      127      316 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/python/packaging/README.md
+-rw-r--r--   0     1001      127      501 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/python/packaging/__init__.py
+-rw-r--r--   0     1001      127     3282 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/python/packaging/_elffile.py
+-rw-r--r--   0     1001      127     9588 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/python/packaging/_manylinux.py
+-rw-r--r--   0     1001      127     2696 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/python/packaging/_musllinux.py
+-rw-r--r--   0     1001      127   182247 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/python-version-metadata.json
+-rw-r--r--   0     1001      127    53798 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/discovery.rs
+-rw-r--r--   0     1001      127     8765 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/environment.rs
+-rw-r--r--   0     1001      127     1314 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/implementation.rs
+-rw-r--r--   0     1001      127    27969 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/interpreter.rs
+-rw-r--r--   0     1001      127    74107 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/lib.rs
+-rw-r--r--   0     1001      127     8104 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/managed/downloads.rs
+-rw-r--r--   0     1001      127     5960 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/managed/find.rs
+-rw-r--r--   0     1001      127      253 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/managed/mod.rs
+-rw-r--r--   0     1001      127   224411 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/managed/python_versions.inc
+-rw-r--r--   0     1001      127      691 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/managed/python_versions.inc.mustache
+-rw-r--r--   0     1001      127     4389 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/platform.rs
+-rw-r--r--   0     1001      127      430 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/pointer_size.rs
+-rw-r--r--   0     1001      127     3234 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/py_launcher.rs
+-rw-r--r--   0     1001      127     7736 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/python_version.rs
+-rw-r--r--   0     1001      127      950 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/target.rs
+-rw-r--r--   0     1001      127     5511 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/src/virtualenv.rs
+-rw-r--r--   0     1001      127     2708 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-interpreter/template-version-metadata.py
+-rw-r--r--   0     1001      127      507 2024-05-22 20:09:33.000000 uv-0.2.1/crates/cache-key/Cargo.toml
+-rw-r--r--   0     1001      127     8335 2024-05-22 20:09:33.000000 uv-0.2.1/crates/cache-key/src/cache_key.rs
+-rw-r--r--   0     1001      127    12317 2024-05-22 20:09:33.000000 uv-0.2.1/crates/cache-key/src/canonical_url.rs
+-rw-r--r--   0     1001      127      620 2024-05-22 20:09:33.000000 uv-0.2.1/crates/cache-key/src/digest.rs
+-rw-r--r--   0     1001      127      191 2024-05-22 20:09:33.000000 uv-0.2.1/crates/cache-key/src/lib.rs
+-rw-r--r--   0     1001      127     1986 2024-05-22 20:09:33.000000 uv-0.2.1/crates/cache-key/src/stable_hash.rs
+-rw-r--r--   0     1001      127      970 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-dispatch/Cargo.toml
+-rw-r--r--   0     1001      127    10910 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-dispatch/src/lib.rs
+-rw-r--r--   0     1001      127      918 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-git/Cargo.toml
+-rw-r--r--   0     1001      127    63247 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-git/src/git.rs
+-rw-r--r--   0     1001      127    37494 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-git/src/known_hosts.rs
+-rw-r--r--   0     1001      127     3843 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-git/src/lib.rs
+-rw-r--r--   0     1001      127      940 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-git/src/sha.rs
+-rw-r--r--   0     1001      127     5058 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-git/src/source.rs
+-rw-r--r--   0     1001      127     1362 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-git/src/util/errors.rs
+-rw-r--r--   0     1001      127      733 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-git/src/util/mod.rs
+-rw-r--r--   0     1001      127     7295 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-git/src/util/retry.rs
+-rw-r--r--   0     1001      127     1807 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/Cargo.toml
+-rw-r--r--   0     1001      127      112 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/README.md
+-rw-r--r--   0     1001      127     7109 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/src/base_client.rs
+-rw-r--r--   0     1001      127    30512 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/src/cached_client.rs
+-rw-r--r--   0     1001      127    10417 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/src/error.rs
+-rw-r--r--   0     1001      127     9211 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/src/flat_index.rs
+-rw-r--r--   0     1001      127    46032 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/src/html.rs
+-rw-r--r--   0     1001      127    29250 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/src/httpcache/control.rs
+-rw-r--r--   0     1001      127    60607 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/src/httpcache/mod.rs
+-rw-r--r--   0     1001      127      648 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/src/lib.rs
+-rw-r--r--   0     1001      127     5110 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/src/linehaul.rs
+-rw-r--r--   0     1001      127     1228 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/src/middleware.rs
+-rw-r--r--   0     1001      127    35668 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/src/registry_client.rs
+-rw-r--r--   0     1001      127     4579 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/src/remote_metadata.rs
+-rw-r--r--   0     1001      127    12019 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/src/rkyvutil.rs
+-rw-r--r--   0     1001      127     1146 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/tests/remote_metadata.rs
+-rw-r--r--   0     1001      127     8183 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-client/tests/user_agent_version.rs
+-rw-r--r--   0     1001      127     2085 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep508-rs/Cargo.toml
+-rw-r--r--   0     1001      127    10173 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep508-rs/License-Apache
+-rw-r--r--   0     1001      127     1293 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep508-rs/License-BSD
+-rw-r--r--   0     1001      127     3039 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep508-rs/Readme.md
+-rw-r--r--   0     1001      127     4301 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep508-rs/src/cursor.rs
+-rw-r--r--   0     1001      127    62005 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep508-rs/src/lib.rs
+-rw-r--r--   0     1001      127    94653 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep508-rs/src/marker.rs
+-rw-r--r--   0     1001      127      743 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep508-rs/src/origin.rs
+-rw-r--r--   0     1001      127    12553 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep508-rs/src/unnamed.rs
+-rw-r--r--   0     1001      127    18647 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pep508-rs/src/verbatim_url.rs
+-rw-r--r--   0     1001      127      774 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/Cargo.toml
+-rw-r--r--   0     1001      127      109 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/README.md
+-rw-r--r--   0     1001      127     4375 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/src/_virtualenv.py
+-rw-r--r--   0     1001      127       20 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/src/activator/.gitattributes
+-rw-r--r--   0     1001      127     3388 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/src/activator/activate
+-rw-r--r--   0     1001      127     2259 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/src/activator/activate.bat
+-rw-r--r--   0     1001      127     2655 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/src/activator/activate.csh
+-rw-r--r--   0     1001      127     4219 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/src/activator/activate.fish
+-rw-r--r--   0     1001      127     3903 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/src/activator/activate.nu
+-rw-r--r--   0     1001      127     2826 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/src/activator/activate.ps1
+-rw-r--r--   0     1001      127     2411 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/src/activator/activate_this.py
+-rw-r--r--   0     1001      127     1728 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/src/activator/deactivate.bat
+-rw-r--r--   0     1001      127     1215 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/src/activator/pydoc.bat
+-rw-r--r--   0     1001      127    16565 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/src/bare.rs
+-rw-r--r--   0     1001      127     2090 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-virtualenv/src/lib.rs
+-rw-r--r--   0     1001      127      822 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pypi-types/Cargo.toml
+-rw-r--r--   0     1001      127     1609 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pypi-types/src/base_url.rs
+-rw-r--r--   0     1001      127     4643 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pypi-types/src/direct_url.rs
+-rw-r--r--   0     1001      127    15738 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pypi-types/src/lenient_requirement.rs
+-rw-r--r--   0     1001      127      239 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pypi-types/src/lib.rs
+-rw-r--r--   0     1001      127    19433 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pypi-types/src/metadata.rs
+-rw-r--r--   0     1001      127      575 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pypi-types/src/scheme.rs
+-rw-r--r--   0     1001      127    12178 2024-05-22 20:09:33.000000 uv-0.2.1/crates/pypi-types/src/simple_json.rs
+-rw-r--r--   0     1001      127      847 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-fs/Cargo.toml
+-rw-r--r--   0     1001      127     1397 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-fs/src/cachedir.rs
+-rw-r--r--   0     1001      127    11067 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-fs/src/lib.rs
+-rw-r--r--   0     1001      127    10859 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-fs/src/path.rs
+-rw-r--r--   0     1001      127     1025 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-cache/Cargo.toml
+-rw-r--r--   0     1001      127      509 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-cache/src/archive.rs
+-rw-r--r--   0     1001      127      195 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-cache/src/by_timestamp.rs
+-rw-r--r--   0     1001      127     1768 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-cache/src/cli.rs
+-rw-r--r--   0     1001      127    35224 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-cache/src/lib.rs
+-rw-r--r--   0     1001      127     6138 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-cache/src/removal.rs
+-rw-r--r--   0     1001      127     1663 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-cache/src/timestamp.rs
+-rw-r--r--   0     1001      127     2538 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-cache/src/wheel.rs
+-rw-r--r--   0     1001      127      411 2024-05-22 20:09:33.000000 uv-0.2.1/crates/once-map/Cargo.toml
+-rw-r--r--   0     1001      127     3940 2024-05-22 20:09:33.000000 uv-0.2.1/crates/once-map/src/lib.rs
+-rw-r--r--   0     1001      127     1528 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/Cargo.toml
+-rw-r--r--   0     1001      127      684 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/archive.rs
+-rw-r--r--   0     1001      127    34434 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/distribution_database.rs
+-rw-r--r--   0     1001      127     2185 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/download.rs
+-rw-r--r--   0     1001      127     7053 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/error.rs
+-rw-r--r--   0     1001      127    10371 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/git.rs
+-rw-r--r--   0     1001      127     7145 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/index/built_wheel_index.rs
+-rw-r--r--   0     1001      127     3435 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/index/cached_wheel.rs
+-rw-r--r--   0     1001      127      162 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/index/mod.rs
+-rw-r--r--   0     1001      127     8729 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/index/registry_wheel_index.rs
+-rw-r--r--   0     1001      127      965 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/lib.rs
+-rw-r--r--   0     1001      127      600 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/locks.rs
+-rw-r--r--   0     1001      127     1225 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/reporter.rs
+-rw-r--r--   0     1001      127     2029 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/source/built_wheel_metadata.rs
+-rw-r--r--   0     1001      127    60426 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/source/mod.rs
+-rw-r--r--   0     1001      127     1998 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-distribution/src/source/revision.rs
+-rw-r--r--   0     1001      127      841 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-configuration/Cargo.toml
+-rw-r--r--   0     1001      127     1014 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-configuration/src/authentication.rs
+-rw-r--r--   0     1001      127    10722 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-configuration/src/build_options.rs
+-rw-r--r--   0     1001      127     1054 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-configuration/src/concurrency.rs
+-rw-r--r--   0     1001      127     9254 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-configuration/src/config_settings.rs
+-rw-r--r--   0     1001      127     1698 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-configuration/src/constraints.rs
+-rw-r--r--   0     1001      127      437 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-configuration/src/lib.rs
+-rw-r--r--   0     1001      127     4059 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-configuration/src/name_specifiers.rs
+-rw-r--r--   0     1001      127     1706 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-configuration/src/overrides.rs
+-rw-r--r--   0     1001      127     2339 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-configuration/src/package_options.rs
+-rw-r--r--   0     1001      127      782 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-configuration/src/preview.rs
+-rw-r--r--   0     1001      127    11893 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-configuration/src/target_triple.rs
+-rw-r--r--   0     1001      127      790 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-types/Cargo.toml
+-rw-r--r--   0     1001      127      423 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-types/src/builds.rs
+-rw-r--r--   0     1001      127      239 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-types/src/downloads.rs
+-rw-r--r--   0     1001      127     6228 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-types/src/hash.rs
+-rw-r--r--   0     1001      127      219 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-types/src/lib.rs
+-rw-r--r--   0     1001      127     1478 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-types/src/requirements.rs
+-rw-r--r--   0     1001      127     6944 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-types/src/traits.rs
+-rw-r--r--   0     1001      127     1504 2024-05-22 20:09:33.000000 uv-0.2.1/crates/install-wheel-rs/Cargo.toml
+-rw-r--r--   0     1001      127      515 2024-05-22 20:09:33.000000 uv-0.2.1/crates/install-wheel-rs/Readme.md
+-rw-r--r--   0     1001      127     4332 2024-05-22 20:09:33.000000 uv-0.2.1/crates/install-wheel-rs/src/lib.rs
+-rw-r--r--   0     1001      127    20181 2024-05-22 20:09:33.000000 uv-0.2.1/crates/install-wheel-rs/src/linker.rs
+-rw-r--r--   0     1001      127     7104 2024-05-22 20:09:33.000000 uv-0.2.1/crates/install-wheel-rs/src/metadata.rs
+-rw-r--r--   0     1001      127      474 2024-05-22 20:09:33.000000 uv-0.2.1/crates/install-wheel-rs/src/record.rs
+-rw-r--r--   0     1001      127     5550 2024-05-22 20:09:33.000000 uv-0.2.1/crates/install-wheel-rs/src/script.rs
+-rw-r--r--   0     1001      127    11211 2024-05-22 20:09:33.000000 uv-0.2.1/crates/install-wheel-rs/src/uninstall.rs
+-rw-r--r--   0     1001      127    34841 2024-05-22 20:09:33.000000 uv-0.2.1/crates/install-wheel-rs/src/wheel.rs
+-rw-r--r--   0     1001      127      752 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-auth/Cargo.toml
+-rw-r--r--   0     1001      127     9542 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-auth/src/cache.rs
+-rw-r--r--   0     1001      127    11219 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-auth/src/credentials.rs
+-rw-r--r--   0     1001      127     9340 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-auth/src/keyring.rs
+-rw-r--r--   0     1001      127      992 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-auth/src/lib.rs
+-rw-r--r--   0     1001      127    45581 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-auth/src/middleware.rs
+-rw-r--r--   0     1001      127     4661 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv-auth/src/realm.rs
+-rw-r--r--   0     1001      127      472 2024-05-22 20:09:33.000000 uv-0.2.1/crates/platform-tags/Cargo.toml
+-rw-r--r--   0     1001      127      161 2024-05-22 20:09:33.000000 uv-0.2.1/crates/platform-tags/src/lib.rs
+-rw-r--r--   0     1001      127     3507 2024-05-22 20:09:33.000000 uv-0.2.1/crates/platform-tags/src/platform.rs
+-rw-r--r--   0     1001      127    76059 2024-05-22 20:09:33.000000 uv-0.2.1/crates/platform-tags/src/tags.rs
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 uv-0.2.1/crates/uv/Cargo.toml
+-rw-r--r--   0     1001      127     3065 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/build.rs
+-rw-r--r--   0     1001      127    79497 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/cli.rs
+-rw-r--r--   0     1001      127     4158 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/cache_clean.rs
+-rw-r--r--   0     1001      127      213 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/cache_dir.rs
+-rw-r--r--   0     1001      127     1955 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/cache_prune.rs
+-rw-r--r--   0     1001      127     4868 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/mod.rs
+-rw-r--r--   0     1001      127     2316 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/pip/check.rs
+-rw-r--r--   0     1001      127    28556 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/pip/compile.rs
+-rw-r--r--   0     1001      127     2462 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/pip/freeze.rs
+-rw-r--r--   0     1001      127    14990 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/pip/install.rs
+-rw-r--r--   0     1001      127     6301 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/pip/list.rs
+-rw-r--r--   0     1001      127      209 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/pip/mod.rs
+-rw-r--r--   0     1001      127    26156 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/pip/operations.rs
+-rw-r--r--   0     1001      127     6601 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/pip/show.rs
+-rw-r--r--   0     1001      127    12640 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/pip/sync.rs
+-rw-r--r--   0     1001      127     7279 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/pip/uninstall.rs
+-rw-r--r--   0     1001      127     5158 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/project/lock.rs
+-rw-r--r--   0     1001      127     8824 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/project/mod.rs
+-rw-r--r--   0     1001      127     5926 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/project/run.rs
+-rw-r--r--   0     1001      127     3881 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/project/sync.rs
+-rw-r--r--   0     1001      127    10251 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/reporters.rs
+-rw-r--r--   0     1001      127     3965 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/self_update.rs
+-rw-r--r--   0     1001      127       20 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/tool/mod.rs
+-rw-r--r--   0     1001      127     4223 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/tool/run.rs
+-rw-r--r--   0     1001      127    10353 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/venv.rs
+-rw-r--r--   0     1001      127      570 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/commands/version.rs
+-rw-r--r--   0     1001      127    11263 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/compat/mod.rs
+-rw-r--r--   0     1001      127     7723 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/editables.rs
+-rw-r--r--   0     1001      127     7604 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/logging.rs
+-rw-r--r--   0     1001      127    24234 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/main.rs
+-rw-r--r--   0     1001      127     2326 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/printer.rs
+-rw-r--r--   0     1001      127    38621 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/settings.rs
+-rw-r--r--   0     1001      127     2844 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/shell.rs
+-rw-r--r--   0     1001      127     4816 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/src/version.rs
+-rw-r--r--   0     1001      127     4437 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/cache_prune.rs
+-rw-r--r--   0     1001      127    21602 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/common/mod.rs
+-rw-r--r--   0     1001      127    27008 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/lock.rs
+-rw-r--r--   0     1001      127     6060 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/pip_check.rs
+-rw-r--r--   0     1001      127   305128 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/pip_compile.rs
+-rw-r--r--   0     1001      127    19016 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/pip_compile_scenarios.rs
+-rw-r--r--   0     1001      127     8341 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/pip_freeze.rs
+-rw-r--r--   0     1001      127   151838 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/pip_install.rs
+-rw-r--r--   0     1001      127   159295 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/pip_install_scenarios.rs
+-rw-r--r--   0     1001      127    18430 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/pip_list.rs
+-rw-r--r--   0     1001      127    13190 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/pip_show.rs
+-rw-r--r--   0     1001      127   162257 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/pip_sync.rs
+-rw-r--r--   0     1001      127    14234 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/pip_uninstall.rs
+-rw-r--r--   0     1001      127     1254 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/self_update.rs
+-rw-r--r--   0     1001      127    18144 2024-05-22 20:09:33.000000 uv-0.2.1/crates/uv/tests/venv.rs
+-rw-r--r--   0     1001      127   134729 2024-05-22 20:09:33.000000 uv-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     8871 1970-01-01 00:00:00.000000 uv-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      127     2366 2024-05-22 20:09:33.000000 uv-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      127     1055 2024-05-22 20:09:33.000000 uv-0.2.1/python/uv/__main__.py
+-rw-r--r--   0     1001      127      806 2024-05-22 20:09:33.000000 uv-0.2.1/python/uv/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-22 20:09:33.000000 uv-0.2.1/python/uv/py.typed
+-rw-r--r--   0     1001      127    31568 2024-05-22 20:09:33.000000 uv-0.2.1/README.md
+-rw-r--r--   0     1001      127       29 2024-05-22 20:09:33.000000 uv-0.2.1/rust-toolchain.toml
+-rw-r--r--   0     1001      127    11356 2024-05-22 20:09:33.000000 uv-0.2.1/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1077 2024-05-22 20:09:33.000000 uv-0.2.1/LICENSE-MIT
+-rw-r--r--   0        0        0    32935 1970-01-01 00:00:00.000000 uv-0.2.1/PKG-INFO
```

### Comparing `uv-0.2.0/crates/uv-normalize/src/extra_name.rs` & `uv-0.2.1/crates/uv-normalize/src/extra_name.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-normalize/src/lib.rs` & `uv-0.2.1/crates/uv-normalize/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-normalize/src/package_name.rs` & `uv-0.2.1/crates/uv-normalize/src/package_name.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/Cargo.toml` & `uv-0.2.1/crates/uv-resolver/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/candidate_selector.rs` & `uv-0.2.1/crates/uv-resolver/src/candidate_selector.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/dependency_mode.rs` & `uv-0.2.1/crates/uv-resolver/src/dependency_mode.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/dependency_provider.rs` & `uv-0.2.1/crates/uv-resolver/src/dependency_provider.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/editables.rs` & `uv-0.2.1/crates/uv-resolver/src/editables.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/error.rs` & `uv-0.2.1/crates/uv-resolver/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/exclude_newer.rs` & `uv-0.2.1/crates/uv-resolver/src/exclude_newer.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/exclusions.rs` & `uv-0.2.1/crates/uv-resolver/src/exclusions.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/flat_index.rs` & `uv-0.2.1/crates/uv-resolver/src/flat_index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/lib.rs` & `uv-0.2.1/crates/uv-resolver/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/lock.rs` & `uv-0.2.1/crates/uv-resolver/src/lock.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Temporarily allowed because this module is still in a state of flux
 // as we build out universal locking.
 #![allow(dead_code, unreachable_code, unused_variables)]
 
-use std::collections::VecDeque;
+use std::collections::{BTreeMap, VecDeque};
 use std::path::{Path, PathBuf};
 use std::str::FromStr;
 
 use rustc_hash::FxHashMap;
 use url::Url;
 
 use distribution_filename::WheelFilename;
@@ -67,15 +67,15 @@
             // the root package name explicitly, and we assume here that it is
             // correct.
             .expect("found too many distributions matching root")
             .expect("could not find root");
         let mut queue: VecDeque<&Distribution> = VecDeque::new();
         queue.push_back(root);
 
-        let mut map = FxHashMap::default();
+        let mut map = BTreeMap::default();
         while let Some(dist) = queue.pop_front() {
             for dep in &dist.dependencies {
                 let dep_dist = self.find_by_id(&dep.id);
                 queue.push_back(dep_dist);
             }
             let name = dist.id.name.clone();
             let resolved_dist = ResolvedDist::Installable(dist.to_dist(marker_env, tags));
```

### Comparing `uv-0.2.0/crates/uv-resolver/src/manifest.rs` & `uv-0.2.1/crates/uv-resolver/src/manifest.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/marker.rs` & `uv-0.2.1/crates/uv-resolver/src/marker.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/options.rs` & `uv-0.2.1/crates/uv-resolver/src/options.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/pins.rs` & `uv-0.2.1/crates/uv-resolver/src/pins.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/preferences.rs` & `uv-0.2.1/crates/uv-resolver/src/preferences.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/prerelease_mode.rs` & `uv-0.2.1/crates/uv-resolver/src/prerelease_mode.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/pubgrub/dependencies.rs` & `uv-0.2.1/crates/uv-resolver/src/pubgrub/dependencies.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/pubgrub/distribution.rs` & `uv-0.2.1/crates/uv-resolver/src/pubgrub/distribution.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/pubgrub/mod.rs` & `uv-0.2.1/crates/uv-resolver/src/pubgrub/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/pubgrub/package.rs` & `uv-0.2.1/crates/uv-resolver/src/pubgrub/package.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/pubgrub/priority.rs` & `uv-0.2.1/crates/uv-resolver/src/pubgrub/priority.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/pubgrub/report.rs` & `uv-0.2.1/crates/uv-resolver/src/pubgrub/report.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/pubgrub/specifier.rs` & `uv-0.2.1/crates/uv-resolver/src/pubgrub/specifier.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/python_requirement.rs` & `uv-0.2.1/crates/uv-resolver/src/python_requirement.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/redirect.rs` & `uv-0.2.1/crates/uv-resolver/src/redirect.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/resolution/display.rs` & `uv-0.2.1/crates/uv-resolver/src/resolution/display.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/resolution/graph.rs` & `uv-0.2.1/crates/uv-resolver/src/resolution/graph.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/resolution/mod.rs` & `uv-0.2.1/crates/uv-resolver/src/resolution/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/resolution_mode.rs` & `uv-0.2.1/crates/uv-resolver/src/resolution_mode.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/resolver/batch_prefetch.rs` & `uv-0.2.1/crates/uv-resolver/src/resolver/batch_prefetch.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/resolver/index.rs` & `uv-0.2.1/crates/uv-resolver/src/resolver/index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/resolver/locals.rs` & `uv-0.2.1/crates/uv-resolver/src/resolver/locals.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/resolver/mod.rs` & `uv-0.2.1/crates/uv-resolver/src/resolver/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/resolver/provider.rs` & `uv-0.2.1/crates/uv-resolver/src/resolver/provider.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/resolver/reporter.rs` & `uv-0.2.1/crates/uv-resolver/src/resolver/reporter.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/resolver/urls.rs` & `uv-0.2.1/crates/uv-resolver/src/resolver/urls.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_optional_missing.snap` & `uv-0.2.1/crates/uv-resolver/src/snapshots/uv_resolver__lock__tests__hash_optional_missing.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/version_map.rs` & `uv-0.2.1/crates/uv-resolver/src/version_map.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/src/yanks.rs` & `uv-0.2.1/crates/uv-resolver/src/yanks.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-resolver/tests/resolver.rs` & `uv-0.2.1/crates/uv-resolver/tests/resolver.rs`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 use std::path::{Path, PathBuf};
 use std::str::FromStr;
 
 use anyhow::Result;
 use chrono::{DateTime, Utc};
 use once_cell::sync::Lazy;
 
-use distribution_types::{IndexLocations, Requirement, Resolution, SourceDist};
+use distribution_types::{CachedDist, IndexLocations, Requirement, Resolution, SourceDist};
 use pep508_rs::{MarkerEnvironment, MarkerEnvironmentBuilder};
 use platform_tags::{Arch, Os, Platform, Tags};
 use uv_cache::Cache;
 use uv_client::RegistryClientBuilder;
 use uv_configuration::{
     BuildKind, Concurrency, Constraints, NoBinary, NoBuild, Overrides, SetupPyStrategy,
 };
@@ -85,15 +85,19 @@
         &self.index_locations
     }
 
     async fn resolve<'a>(&'a self, _: &'a [Requirement]) -> Result<Resolution> {
         panic!("The test should not need to build source distributions")
     }
 
-    async fn install<'a>(&'a self, _: &'a Resolution, _: &'a PythonEnvironment) -> Result<()> {
+    async fn install<'a>(
+        &'a self,
+        _: &'a Resolution,
+        _: &'a PythonEnvironment,
+    ) -> Result<Vec<CachedDist>> {
         panic!("The test should not need to build source distributions")
     }
 
     async fn setup_build<'a>(
         &'a self,
         _: &'a Path,
         _: Option<&'a Path>,
```

### Comparing `uv-0.2.0/crates/cache-key/src/cache_key.rs` & `uv-0.2.1/crates/cache-key/src/cache_key.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/cache-key/src/canonical_url.rs` & `uv-0.2.1/crates/cache-key/src/canonical_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/cache-key/src/digest.rs` & `uv-0.2.1/crates/cache-key/src/digest.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/cache-key/src/stable_hash.rs` & `uv-0.2.1/crates/cache-key/src/stable_hash.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep508-rs/Cargo.toml` & `uv-0.2.1/crates/pep508-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep508-rs/License-Apache` & `uv-0.2.1/crates/pep440-rs/License-Apache`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep508-rs/License-BSD` & `uv-0.2.1/crates/pep440-rs/License-BSD`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep508-rs/Readme.md` & `uv-0.2.1/crates/pep508-rs/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep508-rs/src/cursor.rs` & `uv-0.2.1/crates/pep508-rs/src/cursor.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep508-rs/src/lib.rs` & `uv-0.2.1/crates/pep508-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep508-rs/src/marker.rs` & `uv-0.2.1/crates/pep508-rs/src/marker.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep508-rs/src/origin.rs` & `uv-0.2.1/crates/pep508-rs/src/origin.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep508-rs/src/unnamed.rs` & `uv-0.2.1/crates/pep508-rs/src/unnamed.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep508-rs/src/verbatim_url.rs` & `uv-0.2.1/crates/pep508-rs/src/verbatim_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-auth/Cargo.toml` & `uv-0.2.1/crates/uv-auth/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-auth/src/cache.rs` & `uv-0.2.1/crates/uv-auth/src/cache.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-auth/src/credentials.rs` & `uv-0.2.1/crates/uv-auth/src/credentials.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-auth/src/keyring.rs` & `uv-0.2.1/crates/uv-auth/src/keyring.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-auth/src/lib.rs` & `uv-0.2.1/crates/uv-auth/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-auth/src/middleware.rs` & `uv-0.2.1/crates/uv-auth/src/middleware.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-auth/src/realm.rs` & `uv-0.2.1/crates/uv-auth/src/realm.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-warnings/src/lib.rs` & `uv-0.2.1/crates/uv-warnings/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-cache/Cargo.toml` & `uv-0.2.1/crates/uv-cache/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-cache/src/cli.rs` & `uv-0.2.1/crates/uv-cache/src/cli.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-cache/src/lib.rs` & `uv-0.2.1/crates/uv-cache/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-cache/src/removal.rs` & `uv-0.2.1/crates/uv-cache/src/removal.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-cache/src/timestamp.rs` & `uv-0.2.1/crates/uv-cache/src/timestamp.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-cache/src/wheel.rs` & `uv-0.2.1/crates/uv-cache/src/wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/once-map/src/lib.rs` & `uv-0.2.1/crates/once-map/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-requirements/Cargo.toml` & `uv-0.2.1/crates/uv-requirements/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-requirements/src/confirm.rs` & `uv-0.2.1/crates/uv-requirements/src/confirm.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-requirements/src/lookahead.rs` & `uv-0.2.1/crates/uv-requirements/src/lookahead.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-requirements/src/pyproject.rs` & `uv-0.2.1/crates/uv-requirements/src/pyproject.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-requirements/src/source_tree.rs` & `uv-0.2.1/crates/uv-requirements/src/source_tree.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-requirements/src/sources.rs` & `uv-0.2.1/crates/uv-requirements/src/sources.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-requirements/src/specification.rs` & `uv-0.2.1/crates/uv-requirements/src/specification.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-requirements/src/unnamed.rs` & `uv-0.2.1/crates/uv-requirements/src/unnamed.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-requirements/src/upgrade.rs` & `uv-0.2.1/crates/uv-requirements/src/upgrade.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-requirements/src/workspace.rs` & `uv-0.2.1/crates/uv-requirements/src/workspace.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-filename/Cargo.toml` & `uv-0.2.1/crates/distribution-filename/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-filename/src/lib.rs` & `uv-0.2.1/crates/distribution-filename/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap` & `uv-0.2.1/crates/distribution-filename/src/snapshots/distribution_filename__wheel__tests__ok_multiple_tags.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-filename/src/source_dist.rs` & `uv-0.2.1/crates/distribution-filename/src/source_dist.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-filename/src/wheel.rs` & `uv-0.2.1/crates/distribution-filename/src/wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep440-rs/Cargo.toml` & `uv-0.2.1/crates/pep440-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep440-rs/License-Apache` & `uv-0.2.1/crates/pep508-rs/License-Apache`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep440-rs/License-BSD` & `uv-0.2.1/crates/pep508-rs/License-BSD`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep440-rs/Readme.md` & `uv-0.2.1/crates/pep440-rs/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep440-rs/python/Readme.md` & `uv-0.2.1/crates/pep440-rs/python/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep440-rs/src/lib.rs` & `uv-0.2.1/crates/pep440-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep440-rs/src/version.rs` & `uv-0.2.1/crates/pep440-rs/src/version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pep440-rs/src/version_specifier.rs` & `uv-0.2.1/crates/pep440-rs/src/version_specifier.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/install-wheel-rs/Cargo.toml` & `uv-0.2.1/crates/install-wheel-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/install-wheel-rs/Readme.md` & `uv-0.2.1/crates/install-wheel-rs/Readme.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/install-wheel-rs/src/lib.rs` & `uv-0.2.1/crates/install-wheel-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/install-wheel-rs/src/linker.rs` & `uv-0.2.1/crates/install-wheel-rs/src/linker.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/install-wheel-rs/src/metadata.rs` & `uv-0.2.1/crates/install-wheel-rs/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/install-wheel-rs/src/script.rs` & `uv-0.2.1/crates/install-wheel-rs/src/script.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/install-wheel-rs/src/uninstall.rs` & `uv-0.2.1/crates/install-wheel-rs/src/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/install-wheel-rs/src/wheel.rs` & `uv-0.2.1/crates/install-wheel-rs/src/wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-fs/Cargo.toml` & `uv-0.2.1/crates/uv-fs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-fs/src/cachedir.rs` & `uv-0.2.1/crates/uv-fs/src/cachedir.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-fs/src/lib.rs` & `uv-0.2.1/crates/uv-fs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-fs/src/path.rs` & `uv-0.2.1/crates/uv-fs/src/path.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/Cargo.toml` & `uv-0.2.1/crates/uv-client/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/src/base_client.rs` & `uv-0.2.1/crates/uv-client/src/base_client.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/src/cached_client.rs` & `uv-0.2.1/crates/uv-client/src/cached_client.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/src/error.rs` & `uv-0.2.1/crates/uv-client/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/src/flat_index.rs` & `uv-0.2.1/crates/uv-client/src/flat_index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/src/html.rs` & `uv-0.2.1/crates/uv-client/src/html.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/src/httpcache/control.rs` & `uv-0.2.1/crates/uv-client/src/httpcache/control.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/src/httpcache/mod.rs` & `uv-0.2.1/crates/uv-client/src/httpcache/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/src/lib.rs` & `uv-0.2.1/crates/uv-client/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/src/linehaul.rs` & `uv-0.2.1/crates/uv-client/src/linehaul.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/src/middleware.rs` & `uv-0.2.1/crates/uv-client/src/middleware.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/src/registry_client.rs` & `uv-0.2.1/crates/uv-client/src/registry_client.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/src/remote_metadata.rs` & `uv-0.2.1/crates/uv-client/src/remote_metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/src/rkyvutil.rs` & `uv-0.2.1/crates/uv-client/src/rkyvutil.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/tests/remote_metadata.rs` & `uv-0.2.1/crates/uv-client/tests/remote_metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-client/tests/user_agent_version.rs` & `uv-0.2.1/crates/uv-client/tests/user_agent_version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/Cargo.toml` & `uv-0.2.1/crates/distribution-types/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 anyhow = { workspace = true }
 fs-err = { workspace = true }
 git2 = { workspace = true }
 indexmap = { workspace = true }
 itertools = { workspace = true }
 once_cell = { workspace = true }
 rkyv = { workspace = true }
-rustc-hash = { workspace = true }
 schemars = { workspace = true, optional = true }
 serde = { workspace = true, features = ["derive"] }
 serde_json = { workspace = true }
 thiserror = { workspace = true }
 tracing = { workspace = true }
 url = { workspace = true }
 urlencoding = { workspace = true }
```

### Comparing `uv-0.2.0/crates/distribution-types/src/annotation.rs` & `uv-0.2.1/crates/distribution-types/src/annotation.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/any.rs` & `uv-0.2.1/crates/distribution-types/src/any.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/buildable.rs` & `uv-0.2.1/crates/distribution-types/src/buildable.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/cached.rs` & `uv-0.2.1/crates/distribution-types/src/cached.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/editable.rs` & `uv-0.2.1/crates/distribution-types/src/editable.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/error.rs` & `uv-0.2.1/crates/distribution-types/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/file.rs` & `uv-0.2.1/crates/distribution-types/src/file.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/hash.rs` & `uv-0.2.1/crates/distribution-types/src/hash.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/id.rs` & `uv-0.2.1/crates/distribution-types/src/id.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/index_url.rs` & `uv-0.2.1/crates/distribution-types/src/index_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/installed.rs` & `uv-0.2.1/crates/distribution-types/src/installed.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/lib.rs` & `uv-0.2.1/crates/distribution-types/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/parsed_url.rs` & `uv-0.2.1/crates/distribution-types/src/parsed_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/prioritized_distribution.rs` & `uv-0.2.1/crates/distribution-types/src/prioritized_distribution.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/requirement.rs` & `uv-0.2.1/crates/distribution-types/src/requirement.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/requirements.rs` & `uv-0.2.1/crates/distribution-types/src/requirements.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/resolution.rs` & `uv-0.2.1/crates/distribution-types/src/resolution.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-use rustc_hash::FxHashMap;
+use std::collections::BTreeMap;
 
 use pep508_rs::VerbatimUrl;
 use uv_normalize::PackageName;
 
 use crate::{
     BuiltDist, DirectorySourceDist, Dist, InstalledDirectUrlDist, InstalledDist, LocalEditable,
     Name, Requirement, RequirementSource, ResolvedDist, SourceDist,
 };
 
 /// A set of packages pinned at specific versions.
 #[derive(Debug, Default, Clone)]
-pub struct Resolution(FxHashMap<PackageName, ResolvedDist>);
+pub struct Resolution(BTreeMap<PackageName, ResolvedDist>);
 
 impl Resolution {
     /// Create a new resolution from the given pinned packages.
-    pub fn new(packages: FxHashMap<PackageName, ResolvedDist>) -> Self {
+    pub fn new(packages: BTreeMap<PackageName, ResolvedDist>) -> Self {
         Self(packages)
     }
 
-    /// Return the distribution for the given package name, if it exists.
-    pub fn get(&self, package_name: &PackageName) -> Option<&ResolvedDist> {
-        self.0.get(package_name)
-    }
-
     /// Return the remote distribution for the given package name, if it exists.
     pub fn get_remote(&self, package_name: &PackageName) -> Option<&Dist> {
         match self.0.get(package_name) {
             Some(dist) => match dist {
                 ResolvedDist::Installable(dist) => Some(dist),
                 ResolvedDist::Installed(_) => None,
             },
@@ -40,34 +35,27 @@
     }
 
     /// Iterate over the [`ResolvedDist`] entities in this resolution.
     pub fn distributions(&self) -> impl Iterator<Item = &ResolvedDist> {
         self.0.values()
     }
 
-    /// Iterate over the [`ResolvedDist`] entities in this resolution.
-    pub fn into_distributions(self) -> impl Iterator<Item = ResolvedDist> {
-        self.0.into_values()
-    }
-
     /// Return the number of distributions in this resolution.
     pub fn len(&self) -> usize {
         self.0.len()
     }
 
     /// Return `true` if there are no pinned packages in this resolution.
     pub fn is_empty(&self) -> bool {
         self.0.is_empty()
     }
 
     /// Return the set of [`Requirement`]s that this resolution represents.
-    pub fn requirements(&self) -> Vec<Requirement> {
-        let mut requirements: Vec<_> = self.0.values().map(Requirement::from).collect();
-        requirements.sort_unstable_by(|a, b| a.name.cmp(&b.name));
-        requirements
+    pub fn requirements(&self) -> impl Iterator<Item = Requirement> + '_ {
+        self.0.values().map(Requirement::from)
     }
 
     /// Return an iterator over the [`LocalEditable`] entities in this resolution.
     pub fn editables(&self) -> impl Iterator<Item = LocalEditable> + '_ {
         self.0.values().filter_map(|dist| match dist {
             ResolvedDist::Installable(Dist::Source(SourceDist::Directory(
                 DirectorySourceDist {
```

### Comparing `uv-0.2.0/crates/distribution-types/src/resolved.rs` & `uv-0.2.1/crates/distribution-types/src/resolved.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/specified_requirement.rs` & `uv-0.2.1/crates/distribution-types/src/specified_requirement.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/distribution-types/src/traits.rs` & `uv-0.2.1/crates/distribution-types/src/traits.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-extract/Cargo.toml` & `uv-0.2.1/crates/uv-extract/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-extract/src/error.rs` & `uv-0.2.1/crates/uv-extract/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-extract/src/hash.rs` & `uv-0.2.1/crates/uv-extract/src/hash.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-extract/src/stream.rs` & `uv-0.2.1/crates/uv-extract/src/stream.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-extract/src/sync.rs` & `uv-0.2.1/crates/uv-extract/src/sync.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-extract/src/tar.rs` & `uv-0.2.1/crates/uv-extract/src/tar.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs` & `uv-0.2.1/crates/uv-extract/src/vendor/cloneable_seekable_reader.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-configuration/Cargo.toml` & `uv-0.2.1/crates/uv-configuration/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-configuration/src/authentication.rs` & `uv-0.2.1/crates/uv-configuration/src/authentication.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-configuration/src/build_options.rs` & `uv-0.2.1/crates/uv-configuration/src/build_options.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-configuration/src/concurrency.rs` & `uv-0.2.1/crates/uv-configuration/src/concurrency.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-configuration/src/config_settings.rs` & `uv-0.2.1/crates/uv-configuration/src/config_settings.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-configuration/src/constraints.rs` & `uv-0.2.1/crates/uv-configuration/src/constraints.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-configuration/src/name_specifiers.rs` & `uv-0.2.1/crates/uv-configuration/src/name_specifiers.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-configuration/src/overrides.rs` & `uv-0.2.1/crates/uv-configuration/src/overrides.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-configuration/src/package_options.rs` & `uv-0.2.1/crates/uv-configuration/src/package_options.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-configuration/src/preview.rs` & `uv-0.2.1/crates/uv-configuration/src/preview.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-configuration/src/target_triple.rs` & `uv-0.2.1/crates/uv-configuration/src/target_triple.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-dispatch/Cargo.toml` & `uv-0.2.1/crates/uv-dispatch/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-dispatch/src/lib.rs` & `uv-0.2.1/crates/uv-dispatch/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 use anyhow::{bail, Context, Result};
 use futures::FutureExt;
 use itertools::Itertools;
 use rustc_hash::FxHashMap;
 use tracing::{debug, instrument};
 
-use distribution_types::{IndexLocations, Name, Requirement, Resolution, SourceDist};
+use distribution_types::{CachedDist, IndexLocations, Name, Requirement, Resolution, SourceDist};
 use uv_build::{SourceBuild, SourceBuildContext};
 use uv_cache::Cache;
 use uv_client::RegistryClient;
 use uv_configuration::Concurrency;
 use uv_configuration::{BuildKind, ConfigSettings, NoBinary, NoBuild, Reinstall, SetupPyStrategy};
 use uv_distribution::DistributionDatabase;
 use uv_installer::{Downloader, Installer, Plan, Planner, SitePackages};
@@ -172,15 +172,15 @@
             venv = ?venv.root()
         )
     )]
     async fn install<'data>(
         &'data self,
         resolution: &'data Resolution,
         venv: &'data PythonEnvironment,
-    ) -> Result<()> {
+    ) -> Result<Vec<CachedDist>> {
         debug!(
             "Installing in {} in {}",
             resolution
                 .distributions()
                 .map(ToString::to_string)
                 .join(", "),
             venv.root().display(),
@@ -188,34 +188,36 @@
 
         // Determine the current environment markers.
         let tags = self.interpreter.tags()?;
 
         // Determine the set of installed packages.
         let site_packages = SitePackages::from_executable(venv)?;
 
+        let requirements = resolution.requirements().collect::<Vec<_>>();
+
         let Plan {
             cached,
             remote,
             reinstalls,
             extraneous: _,
-        } = Planner::with_requirements(&resolution.requirements()).build(
+        } = Planner::with_requirements(&requirements).build(
             site_packages,
             &Reinstall::None,
             &NoBinary::None,
             &HashStrategy::None,
             self.index_locations,
             self.cache(),
             venv,
             tags,
         )?;
 
         // Nothing to do.
         if remote.is_empty() && cached.is_empty() && reinstalls.is_empty() {
             debug!("No build requirements to install for build");
-            return Ok(());
+            return Ok(vec![]);
         }
 
         // Resolve any registry-based requirements.
         let remote = remote
             .iter()
             .map(|dist| {
                 resolution
@@ -276,15 +278,15 @@
             );
             Installer::new(venv)
                 .with_link_mode(self.link_mode)
                 .install(&wheels)
                 .context("Failed to install build dependencies")?;
         }
 
-        Ok(())
+        Ok(wheels)
     }
 
     #[instrument(skip_all, fields(version_id = version_id, subdirectory = ?subdirectory))]
     async fn setup_build<'data>(
         &'data self,
         source: &'data Path,
         subdirectory: Option<&'data Path>,
```

### Comparing `uv-0.2.0/crates/uv-virtualenv/Cargo.toml` & `uv-0.2.1/crates/uv-virtualenv/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-virtualenv/src/_virtualenv.py` & `uv-0.2.1/crates/uv-virtualenv/src/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-virtualenv/src/activator/activate` & `uv-0.2.1/crates/uv-virtualenv/src/activator/activate`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-virtualenv/src/activator/activate.bat` & `uv-0.2.1/crates/uv-virtualenv/src/activator/activate.bat`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-virtualenv/src/activator/activate.csh` & `uv-0.2.1/crates/uv-virtualenv/src/activator/activate.csh`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-virtualenv/src/activator/activate.fish` & `uv-0.2.1/crates/uv-virtualenv/src/activator/activate.fish`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-virtualenv/src/activator/activate.nu` & `uv-0.2.1/crates/uv-virtualenv/src/activator/activate.nu`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-virtualenv/src/activator/activate.ps1` & `uv-0.2.1/crates/uv-virtualenv/src/activator/activate.ps1`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-virtualenv/src/activator/activate_this.py` & `uv-0.2.1/crates/uv-virtualenv/src/activator/activate_this.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-virtualenv/src/activator/deactivate.bat` & `uv-0.2.1/crates/uv-virtualenv/src/activator/deactivate.bat`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-virtualenv/src/activator/pydoc.bat` & `uv-0.2.1/crates/uv-virtualenv/src/activator/pydoc.bat`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-virtualenv/src/bare.rs` & `uv-0.2.1/crates/uv-virtualenv/src/bare.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-virtualenv/src/lib.rs` & `uv-0.2.1/crates/uv-virtualenv/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-installer/Cargo.toml` & `uv-0.2.1/crates/uv-installer/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-installer/src/compile.rs` & `uv-0.2.1/crates/uv-installer/src/compile.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-installer/src/downloader.rs` & `uv-0.2.1/crates/uv-installer/src/downloader.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-installer/src/editable.rs` & `uv-0.2.1/crates/uv-installer/src/editable.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-installer/src/installer.rs` & `uv-0.2.1/crates/uv-installer/src/installer.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-installer/src/lib.rs` & `uv-0.2.1/crates/uv-installer/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-installer/src/pip_compileall.py` & `uv-0.2.1/crates/uv-installer/src/pip_compileall.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-installer/src/plan.rs` & `uv-0.2.1/crates/uv-installer/src/plan.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-installer/src/satisfies.rs` & `uv-0.2.1/crates/uv-installer/src/satisfies.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-installer/src/site_packages.rs` & `uv-0.2.1/crates/uv-installer/src/site_packages.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-installer/src/uninstall.rs` & `uv-0.2.1/crates/uv-installer/src/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-build/Cargo.toml` & `uv-0.2.1/crates/uv-build/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-build/src/lib.rs` & `uv-0.2.1/crates/uv-build/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/platform-tags/src/platform.rs` & `uv-0.2.1/crates/platform-tags/src/platform.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/platform-tags/src/tags.rs` & `uv-0.2.1/crates/platform-tags/src/tags.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pypi-types/Cargo.toml` & `uv-0.2.1/crates/pypi-types/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pypi-types/src/base_url.rs` & `uv-0.2.1/crates/pypi-types/src/base_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pypi-types/src/direct_url.rs` & `uv-0.2.1/crates/pypi-types/src/direct_url.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pypi-types/src/lenient_requirement.rs` & `uv-0.2.1/crates/pypi-types/src/lenient_requirement.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pypi-types/src/metadata.rs` & `uv-0.2.1/crates/pypi-types/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pypi-types/src/scheme.rs` & `uv-0.2.1/crates/pypi-types/src/scheme.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/pypi-types/src/simple_json.rs` & `uv-0.2.1/crates/pypi-types/src/simple_json.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/Cargo.toml` & `uv-0.2.1/crates/uv-interpreter/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/fetch-version-metadata.py` & `uv-0.2.1/crates/uv-interpreter/fetch-version-metadata.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/python/get_interpreter_info.py` & `uv-0.2.1/crates/uv-interpreter/python/get_interpreter_info.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/python/packaging/LICENSE.APACHE` & `uv-0.2.1/crates/uv-interpreter/python/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/python/packaging/LICENSE.BSD` & `uv-0.2.1/crates/uv-interpreter/python/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/python/packaging/_elffile.py` & `uv-0.2.1/crates/uv-interpreter/python/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/python/packaging/_manylinux.py` & `uv-0.2.1/crates/uv-interpreter/python/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/python/packaging/_musllinux.py` & `uv-0.2.1/crates/uv-interpreter/python/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/python-version-metadata.json` & `uv-0.2.1/crates/uv-interpreter/python-version-metadata.json`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/discovery.rs` & `uv-0.2.1/crates/uv-interpreter/src/discovery.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/environment.rs` & `uv-0.2.1/crates/uv-interpreter/src/environment.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/implementation.rs` & `uv-0.2.1/crates/uv-interpreter/src/implementation.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/interpreter.rs` & `uv-0.2.1/crates/uv-interpreter/src/interpreter.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/lib.rs` & `uv-0.2.1/crates/uv-interpreter/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/managed/downloads.rs` & `uv-0.2.1/crates/uv-interpreter/src/managed/downloads.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/managed/find.rs` & `uv-0.2.1/crates/uv-interpreter/src/managed/find.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/managed/python_versions.inc` & `uv-0.2.1/crates/uv-interpreter/src/managed/python_versions.inc`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/managed/python_versions.inc.mustache` & `uv-0.2.1/crates/uv-interpreter/src/managed/python_versions.inc.mustache`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/platform.rs` & `uv-0.2.1/crates/uv-interpreter/src/platform.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/py_launcher.rs` & `uv-0.2.1/crates/uv-interpreter/src/py_launcher.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/python_version.rs` & `uv-0.2.1/crates/uv-interpreter/src/python_version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/target.rs` & `uv-0.2.1/crates/uv-interpreter/src/target.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/src/virtualenv.rs` & `uv-0.2.1/crates/uv-interpreter/src/virtualenv.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-interpreter/template-version-metadata.py` & `uv-0.2.1/crates/uv-interpreter/template-version-metadata.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-workspace/Cargo.toml` & `uv-0.2.1/crates/uv-workspace/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-workspace/src/combine.rs` & `uv-0.2.1/crates/uv-workspace/src/combine.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-workspace/src/settings.rs` & `uv-0.2.1/crates/uv-workspace/src/settings.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-workspace/src/workspace.rs` & `uv-0.2.1/crates/uv-workspace/src/workspace.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/Cargo.toml` & `uv-0.2.1/crates/uv-distribution/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/archive.rs` & `uv-0.2.1/crates/uv-distribution/src/archive.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/distribution_database.rs` & `uv-0.2.1/crates/uv-distribution/src/distribution_database.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/download.rs` & `uv-0.2.1/crates/uv-distribution/src/download.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/error.rs` & `uv-0.2.1/crates/uv-distribution/src/error.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/git.rs` & `uv-0.2.1/crates/uv-distribution/src/git.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/index/built_wheel_index.rs` & `uv-0.2.1/crates/uv-distribution/src/index/built_wheel_index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/index/cached_wheel.rs` & `uv-0.2.1/crates/uv-distribution/src/index/cached_wheel.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/index/registry_wheel_index.rs` & `uv-0.2.1/crates/uv-distribution/src/index/registry_wheel_index.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/lib.rs` & `uv-0.2.1/crates/uv-distribution/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/locks.rs` & `uv-0.2.1/crates/uv-distribution/src/locks.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/reporter.rs` & `uv-0.2.1/crates/uv-distribution/src/reporter.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/source/built_wheel_metadata.rs` & `uv-0.2.1/crates/uv-distribution/src/source/built_wheel_metadata.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/source/mod.rs` & `uv-0.2.1/crates/uv-distribution/src/source/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-distribution/src/source/revision.rs` & `uv-0.2.1/crates/uv-distribution/src/source/revision.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/Cargo.toml` & `uv-0.2.1/crates/requirements-txt/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/lib.rs` & `uv-0.2.1/crates/requirements-txt/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/requirement.rs` & `uv-0.2.1/crates/requirements-txt/src/requirement.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-basic.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-constraints-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-for-poetry.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-include-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-poetry-with-hashes.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-small.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__line-endings-whitespace.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-basic.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-constraints-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-for-poetry.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-a.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-include-b.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-poetry-with-hashes.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-small.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-bare-url.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-bare-url.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-editable.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-unix-editable.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-whitespace.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-bare-url.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-bare-url.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-editable.txt.snap` & `uv-0.2.1/crates/requirements-txt/src/snapshots/requirements_txt__test__parse-windows-editable.txt.snap`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt` & `uv-0.2.1/crates/requirements-txt/test-data/requirements-txt/poetry-with-hashes.txt`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-git/Cargo.toml` & `uv-0.2.1/crates/uv-git/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-git/src/git.rs` & `uv-0.2.1/crates/uv-git/src/git.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-git/src/known_hosts.rs` & `uv-0.2.1/crates/uv-git/src/known_hosts.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-git/src/lib.rs` & `uv-0.2.1/crates/uv-git/src/lib.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-git/src/sha.rs` & `uv-0.2.1/crates/uv-git/src/sha.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-git/src/source.rs` & `uv-0.2.1/crates/uv-git/src/source.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-git/src/util/errors.rs` & `uv-0.2.1/crates/uv-git/src/util/errors.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-git/src/util/mod.rs` & `uv-0.2.1/crates/uv-git/src/util/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-git/src/util/retry.rs` & `uv-0.2.1/crates/uv-git/src/util/retry.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-types/Cargo.toml` & `uv-0.2.1/crates/uv-types/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-types/src/hash.rs` & `uv-0.2.1/crates/uv-types/src/hash.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-types/src/requirements.rs` & `uv-0.2.1/crates/uv-types/src/requirements.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv-types/src/traits.rs` & `uv-0.2.1/crates/uv-types/src/traits.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 use std::future::Future;
 use std::path::{Path, PathBuf};
 
 use anyhow::Result;
 use url::Url;
 
-use distribution_types::{IndexLocations, InstalledDist, Requirement, Resolution, SourceDist};
+use distribution_types::{
+    CachedDist, IndexLocations, InstalledDist, Requirement, Resolution, SourceDist,
+};
 use pep508_rs::PackageName;
 use uv_cache::Cache;
 use uv_configuration::{BuildKind, NoBinary, NoBuild, SetupPyStrategy};
 use uv_interpreter::{Interpreter, PythonEnvironment};
 
 use crate::BuildIsolation;
 
@@ -84,15 +86,15 @@
 
     /// Install the given set of package versions into the virtual environment. The environment must
     /// use the same base Python as [`BuildContext::interpreter`]
     fn install<'a>(
         &'a self,
         resolution: &'a Resolution,
         venv: &'a PythonEnvironment,
-    ) -> impl Future<Output = Result<()>> + 'a;
+    ) -> impl Future<Output = Result<Vec<CachedDist>>> + 'a;
 
     /// Setup a source distribution build by installing the required dependencies. A wrapper for
     /// `uv_build::SourceBuild::setup`.
     ///
     /// For PEP 517 builds, this calls `get_requires_for_build_wheel`.
     ///
     /// `version_id` is for error reporting only.
```

### Comparing `uv-0.2.0/crates/uv/Cargo.toml` & `uv-0.2.1/crates/uv/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "uv"
-version = "0.2.0"
+version = "0.2.1"
 edition = { workspace = true }
 rust-version = { workspace = true }
 homepage = { workspace = true }
 documentation = { workspace = true }
 repository = { workspace = true }
 authors = { workspace = true }
 license = { workspace = true }
```

### Comparing `uv-0.2.0/crates/uv/build.rs` & `uv-0.2.1/crates/uv/build.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/cli.rs` & `uv-0.2.1/crates/uv/src/cli.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1936,14 +1936,20 @@
     /// The command to run.
     pub(crate) target: String,
 
     /// The arguments to the command.
     #[arg(allow_hyphen_values = true)]
     pub(crate) args: Vec<OsString>,
 
+    /// Use the given package to provide the command.
+    ///
+    /// By default, the package name is assumed to match the command name.
+    #[arg(long)]
+    pub(crate) from: Option<String>,
+
     /// The Python interpreter to use to build the run environment.
     #[arg(
         long,
         short,
         env = "UV_PYTHON",
         verbatim_doc_comment,
         group = "discovery"
```

### Comparing `uv-0.2.0/crates/uv/src/commands/cache_clean.rs` & `uv-0.2.1/crates/uv/src/commands/cache_clean.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/commands/cache_prune.rs` & `uv-0.2.1/crates/uv/src/commands/cache_prune.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/commands/mod.rs` & `uv-0.2.1/crates/uv/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/commands/pip/check.rs` & `uv-0.2.1/crates/uv/src/commands/pip/check.rs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use std::fmt::Write;
+use std::time::Instant;
 
 use anyhow::Result;
-use distribution_types::InstalledDist;
 use owo_colors::OwoColorize;
-use std::time::Instant;
 use tracing::debug;
 
+use distribution_types::InstalledDist;
 use uv_cache::Cache;
 use uv_fs::Simplified;
 use uv_installer::{Diagnostic, SitePackages};
 use uv_interpreter::{PythonEnvironment, SystemPython};
 
 use crate::commands::{elapsed, ExitStatus};
 use crate::printer::Printer;
```

### Comparing `uv-0.2.0/crates/uv/src/commands/pip/compile.rs` & `uv-0.2.1/crates/uv/src/commands/pip/compile.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/commands/pip/freeze.rs` & `uv-0.2.1/crates/uv/src/commands/pip/freeze.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/commands/pip/install.rs` & `uv-0.2.1/crates/uv/src/commands/pip/install.rs`

 * *Files 15% similar despite different names*

```diff
@@ -15,32 +15,27 @@
 use uv_client::{BaseClientBuilder, Connectivity, FlatIndexClient, RegistryClientBuilder};
 use uv_configuration::{
     Concurrency, ConfigSettings, IndexStrategy, NoBinary, NoBuild, PreviewMode, Reinstall,
     SetupPyStrategy, Upgrade,
 };
 use uv_configuration::{KeyringProviderType, TargetTriple};
 use uv_dispatch::BuildDispatch;
-use uv_distribution::DistributionDatabase;
 use uv_fs::Simplified;
 use uv_installer::{SatisfiesResult, SitePackages};
 use uv_interpreter::{PythonEnvironment, PythonVersion, SystemPython, Target};
 use uv_normalize::PackageName;
-use uv_requirements::{
-    ExtrasSpecification, NamedRequirementsResolver, RequirementsSource, RequirementsSpecification,
-    SourceTreeResolver,
-};
+use uv_requirements::{ExtrasSpecification, RequirementsSource, RequirementsSpecification};
 use uv_resolver::{
     DependencyMode, ExcludeNewer, FlatIndex, InMemoryIndex, Lock, OptionsBuilder, PreReleaseMode,
     ResolutionMode,
 };
 use uv_types::{BuildIsolation, HashStrategy, InFlight};
 
 use crate::commands::pip::operations;
 use crate::commands::pip::operations::Modifications;
-use crate::commands::reporters::ResolverReporter;
 use crate::commands::{elapsed, ExitStatus};
 use crate::editables::ResolvedEditables;
 use crate::printer::Printer;
 
 /// Install packages into the current environment.
 #[allow(clippy::too_many_arguments, clippy::fn_params_excessive_bools)]
 pub(crate) async fn pip_install(
@@ -350,77 +345,32 @@
     // Resolve the requirements.
     let resolution = if let Some(ref root) = uv_lock {
         let root = PackageName::new(root.to_string())?;
         let encoded = fs::tokio::read_to_string("uv.lock").await?;
         let lock: Lock = toml::from_str(&encoded)?;
         lock.to_resolution(&markers, &tags, &root)
     } else {
-        // Resolve the requirements from the provided sources.
-        let requirements = {
-            // Convert from unnamed to named requirements.
-            let mut requirements = NamedRequirementsResolver::new(
-                requirements,
-                &hasher,
-                &index,
-                DistributionDatabase::new(&client, &resolve_dispatch, concurrency.downloads),
-            )
-            .with_reporter(ResolverReporter::from(printer))
-            .resolve()
-            .await?;
-
-            // Resolve any source trees into requirements.
-            if !source_trees.is_empty() {
-                requirements.extend(
-                    SourceTreeResolver::new(
-                        source_trees,
-                        extras,
-                        &hasher,
-                        &index,
-                        DistributionDatabase::new(
-                            &client,
-                            &resolve_dispatch,
-                            concurrency.downloads,
-                        ),
-                    )
-                    .with_reporter(ResolverReporter::from(printer))
-                    .resolve()
-                    .await?,
-                );
-            }
-
-            requirements
-        };
-
-        // Resolve the overrides from the provided sources.
-        let overrides = NamedRequirementsResolver::new(
-            overrides,
-            &hasher,
-            &index,
-            DistributionDatabase::new(&client, &resolve_dispatch, concurrency.downloads),
-        )
-        .with_reporter(ResolverReporter::from(printer))
-        .resolve()
-        .await?;
-
         let options = OptionsBuilder::new()
             .resolution_mode(resolution_mode)
             .prerelease_mode(prerelease_mode)
             .dependency_mode(dependency_mode)
             .exclude_newer(exclude_newer)
             .index_strategy(index_strategy)
             .build();
 
         match operations::resolve(
             requirements,
             constraints,
             overrides,
+            source_trees,
             project,
+            extras,
             &editables,
-            &hasher,
             site_packages.clone(),
+            &hasher,
             &reinstall,
             &upgrade,
             &interpreter,
             &tags,
             &markers,
             &client,
             &flat_index,
```

### Comparing `uv-0.2.0/crates/uv/src/commands/pip/list.rs` & `uv-0.2.1/crates/uv/src/commands/pip/list.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/commands/pip/operations.rs` & `uv-0.2.1/crates/uv/src/commands/pip/operations.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 //! Common operations shared across the `pip` API and subcommands.
 
 use std::fmt::Write;
+use std::path::PathBuf;
 
 use anyhow::{anyhow, Context};
 use itertools::Itertools;
 use owo_colors::OwoColorize;
 use tracing::debug;
 
-use distribution_types::{CachedDist, Dist, InstalledDist, Requirement};
+use distribution_types::{
+    CachedDist, Dist, InstalledDist, Requirement, UnresolvedRequirementSpecification,
+};
 use distribution_types::{
     DistributionMetadata, IndexLocations, InstalledMetadata, InstalledVersion, LocalDist, Name,
     ParsedUrl, RequirementSource, Resolution,
 };
 use install_wheel_rs::linker::LinkMode;
 use pep440_rs::{VersionSpecifier, VersionSpecifiers};
 use pep508_rs::{MarkerEnvironment, VerbatimUrl};
@@ -25,21 +28,22 @@
 use uv_dispatch::BuildDispatch;
 use uv_distribution::DistributionDatabase;
 use uv_fs::Simplified;
 use uv_installer::{Downloader, Plan, Planner, ResolvedEditable, SitePackages};
 use uv_interpreter::{Interpreter, PythonEnvironment};
 use uv_normalize::PackageName;
 use uv_requirements::{
-    ExtrasSpecification, LookaheadResolver, RequirementsSource, RequirementsSpecification,
+    ExtrasSpecification, LookaheadResolver, NamedRequirementsResolver, RequirementsSource,
+    RequirementsSpecification, SourceTreeResolver,
 };
 use uv_resolver::{
     DependencyMode, Exclusions, FlatIndex, InMemoryIndex, Manifest, Options, Preference,
     PythonRequirement, ResolutionGraph, Resolver,
 };
-use uv_types::{HashStrategy, InFlight};
+use uv_types::{HashStrategy, InFlight, InstalledPackagesProvider};
 use uv_warnings::warn_user;
 
 use crate::commands::reporters::{DownloadReporter, InstallReporter, ResolverReporter};
 use crate::commands::DryRunEvent;
 use crate::commands::{compile_bytecode, elapsed, ChangeEvent, ChangeEventKind};
 use crate::editables::ResolvedEditables;
 use crate::printer::Printer;
@@ -95,22 +99,24 @@
     }
 
     Ok(spec)
 }
 
 /// Resolve a set of requirements, similar to running `pip compile`.
 #[allow(clippy::too_many_arguments)]
-pub(crate) async fn resolve(
-    requirements: Vec<Requirement>,
+pub(crate) async fn resolve<InstalledPackages: InstalledPackagesProvider>(
+    requirements: Vec<UnresolvedRequirementSpecification>,
     constraints: Vec<Requirement>,
-    overrides: Vec<Requirement>,
+    overrides: Vec<UnresolvedRequirementSpecification>,
+    source_trees: Vec<PathBuf>,
     project: Option<PackageName>,
+    extras: &ExtrasSpecification,
     editables: &ResolvedEditables,
+    installed_packages: InstalledPackages,
     hasher: &HashStrategy,
-    site_packages: SitePackages,
     reinstall: &Reinstall,
     upgrade: &Upgrade,
     interpreter: &Interpreter,
     tags: &Tags,
     markers: &MarkerEnvironment,
     client: &RegistryClient,
     flat_index: &FlatIndex,
@@ -118,19 +124,89 @@
     build_dispatch: &BuildDispatch<'_>,
     concurrency: Concurrency,
     options: Options,
     printer: Printer,
 ) -> Result<ResolutionGraph, Error> {
     let start = std::time::Instant::now();
 
+    // Resolve the requirements from the provided sources.
+    let requirements = {
+        // Convert from unnamed to named requirements.
+        let mut requirements = NamedRequirementsResolver::new(
+            requirements,
+            hasher,
+            index,
+            DistributionDatabase::new(client, build_dispatch, concurrency.downloads),
+        )
+        .with_reporter(ResolverReporter::from(printer))
+        .resolve()
+        .await?;
+
+        // Resolve any source trees into requirements.
+        if !source_trees.is_empty() {
+            requirements.extend(
+                SourceTreeResolver::new(
+                    source_trees,
+                    extras,
+                    hasher,
+                    index,
+                    DistributionDatabase::new(client, build_dispatch, concurrency.downloads),
+                )
+                .with_reporter(ResolverReporter::from(printer))
+                .resolve()
+                .await?,
+            );
+        }
+
+        requirements
+    };
+
+    // Resolve the overrides from the provided sources.
+    let overrides = NamedRequirementsResolver::new(
+        overrides,
+        hasher,
+        index,
+        DistributionDatabase::new(client, build_dispatch, concurrency.downloads),
+    )
+    .with_reporter(ResolverReporter::from(printer))
+    .resolve()
+    .await?;
+
+    // Collect constraints and overrides.
+    let constraints = Constraints::from_requirements(constraints);
+    let overrides = Overrides::from_requirements(overrides);
+    let python_requirement = PythonRequirement::from_marker_environment(interpreter, markers);
+
+    // Map the editables to their metadata.
+    let editables = editables.as_metadata().map_err(Error::ParsedUrl)?;
+
+    // Determine any lookahead requirements.
+    let lookaheads = match options.dependency_mode {
+        DependencyMode::Transitive => {
+            LookaheadResolver::new(
+                &requirements,
+                &constraints,
+                &overrides,
+                &editables,
+                hasher,
+                index,
+                DistributionDatabase::new(client, build_dispatch, concurrency.downloads),
+            )
+            .with_reporter(ResolverReporter::from(printer))
+            .resolve(Some(markers))
+            .await?
+        }
+        DependencyMode::Direct => Vec::new(),
+    };
+
     // TODO(zanieb): Consider consuming these instead of cloning
     let exclusions = Exclusions::new(reinstall.clone(), upgrade.clone());
 
     // Prefer current site packages; filter out packages that are marked for reinstall or upgrade
-    let preferences = site_packages
+    let preferences = installed_packages
         .iter()
         .filter(|dist| !exclusions.contains(dist.name()))
         .map(|dist| {
             let source = match dist.installed_version() {
                 InstalledVersion::Version(version) => RequirementSource::Registry {
                     specifier: VersionSpecifiers::from(VersionSpecifier::equals_version(
                         version.clone(),
@@ -154,41 +230,14 @@
                 origin: None,
             };
             Ok(Preference::from_requirement(requirement))
         })
         .collect::<Result<_, _>>()
         .map_err(Error::UnsupportedInstalledDist)?;
 
-    // Collect constraints and overrides.
-    let constraints = Constraints::from_requirements(constraints);
-    let overrides = Overrides::from_requirements(overrides);
-    let python_requirement = PythonRequirement::from_marker_environment(interpreter, markers);
-
-    // Map the editables to their metadata.
-    let editables = editables.as_metadata().map_err(Error::ParsedUrl)?;
-
-    // Determine any lookahead requirements.
-    let lookaheads = match options.dependency_mode {
-        DependencyMode::Transitive => {
-            LookaheadResolver::new(
-                &requirements,
-                &constraints,
-                &overrides,
-                &editables,
-                hasher,
-                index,
-                DistributionDatabase::new(client, build_dispatch, concurrency.downloads),
-            )
-            .with_reporter(ResolverReporter::from(printer))
-            .resolve(Some(markers))
-            .await?
-        }
-        DependencyMode::Direct => Vec::new(),
-    };
-
     // Create a manifest of the requirements.
     let manifest = Manifest::new(
         requirements,
         constraints,
         overrides,
         preferences,
         project,
@@ -213,15 +262,15 @@
             &python_requirement,
             Some(markers),
             tags,
             flat_index,
             index,
             hasher,
             build_dispatch,
-            site_packages,
+            installed_packages,
             DistributionDatabase::new(client, build_dispatch, concurrency.downloads),
         )?
         .with_reporter(reporter);
 
         resolver.resolve().await?
     };
 
@@ -292,15 +341,14 @@
     let start = std::time::Instant::now();
 
     // Extract the requirements from the resolution, filtering out any editables that were already
     // required. If a package is already installed as editable, it may appear in the resolution
     // despite not being explicitly requested.
     let requirements = resolution
         .requirements()
-        .into_iter()
         .filter(|requirement| {
             if requirement.source.is_editable() {
                 !editables
                     .iter()
                     .any(|editable| requirement.name == *editable.name())
             } else {
                 true
```

### Comparing `uv-0.2.0/crates/uv/src/commands/pip/show.rs` & `uv-0.2.1/crates/uv/src/commands/pip/show.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/commands/pip/sync.rs` & `uv-0.2.1/crates/uv/src/commands/pip/sync.rs`

 * *Files 11% similar despite different names*

```diff
@@ -14,31 +14,26 @@
 use uv_client::{BaseClientBuilder, Connectivity, FlatIndexClient, RegistryClientBuilder};
 use uv_configuration::{
     Concurrency, ConfigSettings, IndexStrategy, NoBinary, NoBuild, PreviewMode, Reinstall,
     SetupPyStrategy, Upgrade,
 };
 use uv_configuration::{KeyringProviderType, TargetTriple};
 use uv_dispatch::BuildDispatch;
-use uv_distribution::DistributionDatabase;
 use uv_fs::Simplified;
 use uv_installer::SitePackages;
 use uv_interpreter::{PythonEnvironment, PythonVersion, SystemPython, Target};
-use uv_requirements::{
-    ExtrasSpecification, NamedRequirementsResolver, RequirementsSource, RequirementsSpecification,
-    SourceTreeResolver,
-};
+use uv_requirements::{ExtrasSpecification, RequirementsSource, RequirementsSpecification};
 use uv_resolver::{
     DependencyMode, ExcludeNewer, FlatIndex, InMemoryIndex, OptionsBuilder, PreReleaseMode,
     ResolutionMode,
 };
 use uv_types::{BuildIsolation, HashStrategy, InFlight};
 
 use crate::commands::pip::operations;
 use crate::commands::pip::operations::Modifications;
-use crate::commands::reporters::ResolverReporter;
 use crate::commands::ExitStatus;
 use crate::editables::ResolvedEditables;
 use crate::printer::Printer;
 
 /// Install a set of locked requirements into the current Python environment.
 #[allow(clippy::too_many_arguments, clippy::fn_params_excessive_bools)]
 pub(crate) async fn pip_sync(
@@ -296,73 +291,32 @@
         &client,
         &resolve_dispatch,
         concurrency,
         printer,
     )
     .await?;
 
-    // Resolve the requirements from the provided sources.
-    let requirements = {
-        // Convert from unnamed to named requirements.
-        let mut requirements = NamedRequirementsResolver::new(
-            requirements,
-            &hasher,
-            &index,
-            DistributionDatabase::new(&client, &resolve_dispatch, concurrency.downloads),
-        )
-        .with_reporter(ResolverReporter::from(printer))
-        .resolve()
-        .await?;
-
-        // Resolve any source trees into requirements.
-        if !source_trees.is_empty() {
-            requirements.extend(
-                SourceTreeResolver::new(
-                    source_trees,
-                    &extras,
-                    &hasher,
-                    &index,
-                    DistributionDatabase::new(&client, &resolve_dispatch, concurrency.downloads),
-                )
-                .with_reporter(ResolverReporter::from(printer))
-                .resolve()
-                .await?,
-            );
-        }
-
-        requirements
-    };
-
-    // Resolve the overrides from the provided sources.
-    let overrides = NamedRequirementsResolver::new(
-        overrides,
-        &hasher,
-        &index,
-        DistributionDatabase::new(&client, &resolve_dispatch, concurrency.downloads),
-    )
-    .with_reporter(ResolverReporter::from(printer))
-    .resolve()
-    .await?;
-
     let options = OptionsBuilder::new()
         .resolution_mode(resolution_mode)
         .prerelease_mode(prerelease_mode)
         .dependency_mode(dependency_mode)
         .exclude_newer(exclude_newer)
         .index_strategy(index_strategy)
         .build();
 
     let resolution = match operations::resolve(
         requirements,
         constraints,
         overrides,
+        source_trees,
         project,
+        &extras,
         &editables,
-        &hasher,
         site_packages.clone(),
+        &hasher,
         reinstall,
         &upgrade,
         interpreter,
         &tags,
         &markers,
         &client,
         &flat_index,
```

### Comparing `uv-0.2.0/crates/uv/src/commands/pip/uninstall.rs` & `uv-0.2.1/crates/uv/src/commands/pip/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/commands/project/lock.rs` & `uv-0.2.1/crates/uv/src/commands/project/lock.rs`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 use distribution_types::IndexLocations;
 use install_wheel_rs::linker::LinkMode;
 use uv_cache::Cache;
 use uv_client::{BaseClientBuilder, RegistryClientBuilder};
 use uv_configuration::{
     Concurrency, ConfigSettings, NoBinary, NoBuild, PreviewMode, Reinstall, SetupPyStrategy,
+    Upgrade,
 };
 use uv_dispatch::BuildDispatch;
 use uv_requirements::{ExtrasSpecification, ProjectWorkspace, RequirementsSpecification};
-use uv_resolver::{FlatIndex, InMemoryIndex, OptionsBuilder};
+use uv_resolver::{FlatIndex, InMemoryIndex, Options};
 use uv_types::{BuildIsolation, EmptyInstalledPackages, HashStrategy, InFlight};
 use uv_warnings::warn_user;
 
-use crate::commands::project::Error;
-use crate::commands::{project, ExitStatus};
+use crate::commands::{pip, project, ExitStatus};
 use crate::editables::ResolvedEditables;
 use crate::printer::Printer;
 
 /// Resolve the project requirements into a lockfile.
 #[allow(clippy::too_many_arguments)]
 pub(crate) async fn lock(
     preview: PreviewMode,
@@ -30,15 +30,15 @@
         warn_user!("`uv lock` is experimental and may change without warning.");
     }
 
     // Find the project requirements.
     let project = ProjectWorkspace::discover(std::env::current_dir()?)?;
 
     // Discover or create the virtual environment.
-    let venv = project::init(&project, cache, printer)?;
+    let venv = project::init_environment(&project, cache, printer)?;
 
     // TODO(zanieb): Support client configuration
     let client_builder = BaseClientBuilder::default();
 
     // Read all requirements from the provided sources.
     // TODO(zanieb): Consider allowing constraints and extras
     // TODO(zanieb): Allow specifying extras somehow
@@ -62,26 +62,29 @@
     let client = RegistryClientBuilder::new(cache.clone())
         .markers(markers)
         .platform(venv.interpreter().platform())
         .build();
 
     // TODO(charlie): Respect project configuration.
     let build_isolation = BuildIsolation::default();
+    let concurrency = Concurrency::default();
     let config_settings = ConfigSettings::default();
+    let extras = ExtrasSpecification::default();
     let flat_index = FlatIndex::default();
     let hasher = HashStrategy::default();
     let in_flight = InFlight::default();
     let index = InMemoryIndex::default();
     let index_locations = IndexLocations::default();
     let link_mode = LinkMode::default();
     let no_binary = NoBinary::default();
     let no_build = NoBuild::default();
+    let options = Options::default();
+    let reinstall = Reinstall::default();
     let setup_py = SetupPyStrategy::default();
-    let concurrency = Concurrency::default();
-    let reinstall = Reinstall::None;
+    let upgrade = Upgrade::default();
 
     // Create a build dispatch.
     let build_dispatch = BuildDispatch::new(
         &client,
         cache,
         &interpreter,
         &index_locations,
@@ -93,22 +96,14 @@
         build_isolation,
         link_mode,
         &no_build,
         &no_binary,
         concurrency,
     );
 
-    let options = OptionsBuilder::new()
-        // TODO(zanieb): Support resolver options
-        // .resolution_mode(resolution_mode)
-        // .prerelease_mode(prerelease_mode)
-        // .dependency_mode(dependency_mode)
-        // .exclude_newer(exclude_newer)
-        .build();
-
     // Build all editable distributions. The editables are shared between resolution and
     // installation, and should live for the duration of the command.
     let editables = ResolvedEditables::resolve(
         spec.editables
             .iter()
             .cloned()
             .map(ResolvedEditables::from_requirement),
@@ -122,34 +117,41 @@
         &build_dispatch,
         concurrency,
         printer,
     )
     .await?;
 
     // Resolve the requirements.
-    let resolution = project::resolve(
-        spec,
-        EmptyInstalledPackages,
+    let resolution = pip::operations::resolve(
+        spec.requirements,
+        spec.constraints,
+        spec.overrides,
+        spec.source_trees,
+        spec.project,
+        &extras,
         &editables,
+        EmptyInstalledPackages,
         &hasher,
+        &reinstall,
+        &upgrade,
         &interpreter,
         tags,
         markers,
         &client,
         &flat_index,
         &index,
         &build_dispatch,
+        concurrency,
         options,
         printer,
-        concurrency,
     )
     .await;
 
     let resolution = match resolution {
-        Err(Error::Resolve(uv_resolver::ResolveError::NoSolution(err))) => {
+        Err(pip::operations::Error::Resolve(uv_resolver::ResolveError::NoSolution(err))) => {
             let report = miette::Report::msg(format!("{err}"))
                 .context("No solution found when resolving dependencies:");
             eprint!("{report:?}");
             return Ok(ExitStatus::Failure);
         }
         result => result,
     }?;
```

### Comparing `uv-0.2.0/crates/uv/src/commands/project/run.rs` & `uv-0.2.1/crates/uv/src/commands/project/run.rs`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     let project_env = if isolated {
         None
     } else {
         debug!("Syncing project environment.");
 
         let project = ProjectWorkspace::discover(std::env::current_dir()?)?;
 
-        let venv = project::init(&project, cache, printer)?;
+        let venv = project::init_environment(&project, cache, printer)?;
 
         // Install the project requirements.
         Some(
             project::update_environment(
                 venv,
                 &project.requirements(),
                 preview,
```

### Comparing `uv-0.2.0/crates/uv/src/commands/project/sync.rs` & `uv-0.2.1/crates/uv/src/commands/project/sync.rs`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 use uv_dispatch::BuildDispatch;
 use uv_installer::SitePackages;
 use uv_requirements::ProjectWorkspace;
 use uv_resolver::{FlatIndex, InMemoryIndex, Lock};
 use uv_types::{BuildIsolation, HashStrategy, InFlight};
 use uv_warnings::warn_user;
 
-use crate::commands::{project, ExitStatus};
+use crate::commands::pip::operations::Modifications;
+use crate::commands::{pip, project, ExitStatus};
 use crate::editables::ResolvedEditables;
 use crate::printer::Printer;
 
 /// Sync the project environment.
 #[allow(clippy::too_many_arguments)]
 pub(crate) async fn sync(
     preview: PreviewMode,
@@ -29,15 +30,15 @@
         warn_user!("`uv sync` is experimental and may change without warning.");
     }
 
     // Find the project requirements.
     let project = ProjectWorkspace::discover(std::env::current_dir()?)?;
 
     // Discover or create the virtual environment.
-    let venv = project::init(&project, cache, printer)?;
+    let venv = project::init_environment(&project, cache, printer)?;
     let markers = venv.interpreter().markers();
     let tags = venv.interpreter().tags()?;
 
     // Read the lockfile.
     let resolution = {
         let encoded =
             fs_err::tokio::read_to_string(project.workspace().root().join("uv.lock")).await?;
@@ -50,26 +51,28 @@
     let client = RegistryClientBuilder::new(cache.clone())
         .markers(markers)
         .platform(venv.interpreter().platform())
         .build();
 
     // TODO(charlie): Respect project configuration.
     let build_isolation = BuildIsolation::default();
+    let compile = false;
+    let concurrency = Concurrency::default();
     let config_settings = ConfigSettings::default();
+    let dry_run = false;
     let flat_index = FlatIndex::default();
     let hasher = HashStrategy::default();
     let in_flight = InFlight::default();
     let index = InMemoryIndex::default();
     let index_locations = IndexLocations::default();
     let link_mode = LinkMode::default();
     let no_binary = NoBinary::default();
     let no_build = NoBuild::default();
-    let setup_py = SetupPyStrategy::default();
-    let concurrency = Concurrency::default();
     let reinstall = Reinstall::default();
+    let setup_py = SetupPyStrategy::default();
 
     // Create a build dispatch.
     let build_dispatch = BuildDispatch::new(
         &client,
         cache,
         venv.interpreter(),
         &index_locations,
@@ -102,28 +105,32 @@
         printer,
     )
     .await?;
 
     let site_packages = SitePackages::from_executable(&venv)?;
 
     // Sync the environment.
-    project::install(
+    pip::operations::install(
         &resolution,
-        editables,
+        &editables,
         site_packages,
+        Modifications::Sufficient,
+        &reinstall,
         &no_binary,
         link_mode,
+        compile,
         &index_locations,
         &hasher,
         tags,
         &client,
         &in_flight,
+        concurrency,
         &build_dispatch,
         cache,
         &venv,
+        dry_run,
         printer,
-        concurrency,
     )
     .await?;
 
     Ok(ExitStatus::Success)
 }
```

### Comparing `uv-0.2.0/crates/uv/src/commands/reporters.rs` & `uv-0.2.1/crates/uv/src/commands/reporters.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/commands/self_update.rs` & `uv-0.2.1/crates/uv/src/commands/self_update.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/commands/tool/run.rs` & `uv-0.2.1/crates/uv/src/commands/tool/run.rs`

 * *Files 4% similar despite different names*

```diff
@@ -20,27 +20,29 @@
 
 /// Run a command.
 #[allow(clippy::too_many_arguments)]
 pub(crate) async fn run(
     target: String,
     args: Vec<OsString>,
     python: Option<String>,
+    from: Option<String>,
     _isolated: bool,
     preview: PreviewMode,
     connectivity: Connectivity,
     cache: &Cache,
     printer: Printer,
 ) -> Result<ExitStatus> {
     if preview.is_disabled() {
         warn_user!("`uv tool run` is experimental and may change without warning.");
     }
 
-    // TODO(zanieb): Allow users to pass an explicit package name different than the target
-    // as well as additional requirements
-    let requirements = [RequirementsSource::from_package(target.clone())];
+    // TODO(zanieb): Allow users to pass additional requirements
+    let requirements = [RequirementsSource::from_package(
+        from.unwrap_or_else(|| target.clone()),
+    )];
 
     // TODO(zanieb): When implementing project-level tools, discover the project and check if it has the tool
     // TOOD(zanieb): Determine if we sould layer on top of the project environment if it is present
 
     // If necessary, create an environment for the ephemeral requirements.
     debug!("Syncing ephemeral environment.");
```

### Comparing `uv-0.2.0/crates/uv/src/commands/venv.rs` & `uv-0.2.1/crates/uv/src/commands/venv.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 use std::fmt::Write;
 use std::path::Path;
 use std::str::FromStr;
 use std::vec;
 
 use anstream::eprint;
 use anyhow::Result;
-use itertools::Itertools;
 use miette::{Diagnostic, IntoDiagnostic};
 use owo_colors::OwoColorize;
 use thiserror::Error;
 
-use distribution_types::{DistributionMetadata, IndexLocations, Name, Requirement, ResolvedDist};
+use distribution_types::{IndexLocations, Requirement};
 use install_wheel_rs::linker::LinkMode;
 use uv_auth::store_credentials_from_url;
 use uv_cache::Cache;
 use uv_client::{Connectivity, FlatIndexClient, RegistryClientBuilder};
 use uv_configuration::{Concurrency, KeyringProviderType};
 use uv_configuration::{ConfigSettings, IndexStrategy, NoBinary, NoBuild, SetupPyStrategy};
 use uv_dispatch::BuildDispatch;
 use uv_fs::Simplified;
 use uv_interpreter::{
     find_default_interpreter, find_interpreter, InterpreterRequest, SourceSelector,
 };
 use uv_resolver::{ExcludeNewer, FlatIndex, InMemoryIndex, OptionsBuilder};
 use uv_types::{BuildContext, BuildIsolation, HashStrategy, InFlight};
 
-use crate::commands::ExitStatus;
+use crate::commands::{pip, ExitStatus};
 use crate::printer::Printer;
 use crate::shell::Shell;
 
 /// Create a virtual environment.
 #[allow(
     clippy::unnecessary_wraps,
     clippy::too_many_arguments,
@@ -219,58 +218,44 @@
             &NoBuild::All,
             &NoBinary::None,
             concurrency,
         )
         .with_options(OptionsBuilder::new().exclude_newer(exclude_newer).build());
 
         // Resolve the seed packages.
-        let mut requirements =
+        let requirements = if interpreter.python_tuple() < (3, 12) {
+            // Only include `setuptools` and `wheel` on Python <3.12
             vec![
                 Requirement::from_pep508(pep508_rs::Requirement::from_str("pip").unwrap()).unwrap(),
-            ];
-
-        // Only include `setuptools` and `wheel` on Python <3.12
-        if interpreter.python_tuple() < (3, 12) {
-            requirements.push(
                 Requirement::from_pep508(pep508_rs::Requirement::from_str("setuptools").unwrap())
                     .unwrap(),
-            );
-            requirements.push(
                 Requirement::from_pep508(pep508_rs::Requirement::from_str("wheel").unwrap())
                     .unwrap(),
-            );
-        }
+            ]
+        } else {
+            vec![
+                Requirement::from_pep508(pep508_rs::Requirement::from_str("pip").unwrap()).unwrap(),
+            ]
+        };
+
+        // Resolve and install the requirements.
+        //
+        // Since the virtual environment is empty, and the set of requirements is trivial (no
+        // constraints, no editables, etc.), we can use the build dispatch APIs directly.
         let resolution = build_dispatch
             .resolve(&requirements)
             .await
             .map_err(VenvError::Seed)?;
-
-        // Install into the environment.
-        build_dispatch
+        let installed = build_dispatch
             .install(&resolution, &venv)
             .await
             .map_err(VenvError::Seed)?;
 
-        for distribution in resolution
-            .distributions()
-            .filter_map(|dist| match dist {
-                ResolvedDist::Installable(dist) => Some(dist),
-                ResolvedDist::Installed(_) => None,
-            })
-            .sorted_unstable_by(|a, b| a.name().cmp(b.name()).then(a.version().cmp(&b.version())))
-        {
-            writeln!(
-                printer.stderr(),
-                " {} {}{}",
-                "+".green(),
-                distribution.name().as_ref().bold(),
-                distribution.version_or_url().dimmed()
-            )
+        pip::operations::report_modifications(installed, Vec::new(), Vec::new(), printer)
             .into_diagnostic()?;
-        }
     }
 
     // Determine the appropriate activation command.
     let activation = match Shell::from_env() {
         None => None,
         Some(Shell::Bash | Shell::Zsh) => Some(format!(
             "source {}",
```

### Comparing `uv-0.2.0/crates/uv/src/commands/version.rs` & `uv-0.2.1/crates/uv/src/commands/version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/compat/mod.rs` & `uv-0.2.1/crates/uv/src/compat/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/editables.rs` & `uv-0.2.1/crates/uv/src/editables.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/logging.rs` & `uv-0.2.1/crates/uv/src/logging.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/main.rs` & `uv-0.2.1/crates/uv/src/main.rs`

 * *Files 0% similar despite different names*

```diff
@@ -614,14 +614,15 @@
         Commands::Tool(ToolNamespace {
             command: ToolCommand::Run(args),
         }) => {
             commands::run_tool(
                 args.target,
                 args.args,
                 args.python,
+                args.from,
                 globals.isolated,
                 globals.preview,
                 globals.connectivity,
                 &cache,
                 printer,
             )
             .await
```

### Comparing `uv-0.2.0/crates/uv/src/printer.rs` & `uv-0.2.1/crates/uv/src/printer.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/settings.rs` & `uv-0.2.1/crates/uv/src/settings.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/shell.rs` & `uv-0.2.1/crates/uv/src/shell.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/src/version.rs` & `uv-0.2.1/crates/uv/src/version.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/cache_prune.rs` & `uv-0.2.1/crates/uv/tests/cache_prune.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/common/mod.rs` & `uv-0.2.1/crates/uv/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/lock.rs` & `uv-0.2.1/crates/uv/tests/lock.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/pip_check.rs` & `uv-0.2.1/crates/uv/tests/pip_check.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/pip_compile.rs` & `uv-0.2.1/crates/uv/tests/pip_compile.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/pip_compile_scenarios.rs` & `uv-0.2.1/crates/uv/tests/pip_compile_scenarios.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/pip_freeze.rs` & `uv-0.2.1/crates/uv/tests/pip_freeze.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/pip_install.rs` & `uv-0.2.1/crates/uv/tests/pip_install.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/pip_install_scenarios.rs` & `uv-0.2.1/crates/uv/tests/pip_install_scenarios.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/pip_list.rs` & `uv-0.2.1/crates/uv/tests/pip_list.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/pip_show.rs` & `uv-0.2.1/crates/uv/tests/pip_show.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/pip_sync.rs` & `uv-0.2.1/crates/uv/tests/pip_sync.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/pip_uninstall.rs` & `uv-0.2.1/crates/uv/tests/pip_uninstall.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/self_update.rs` & `uv-0.2.1/crates/uv/tests/self_update.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/crates/uv/tests/venv.rs` & `uv-0.2.1/crates/uv/tests/venv.rs`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/Cargo.lock` & `uv-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1107,15 +1107,14 @@
  "itertools 0.13.0",
  "once_cell",
  "pep440_rs",
  "pep508_rs",
  "platform-tags",
  "pypi-types",
  "rkyv",
- "rustc-hash",
  "schemars",
  "serde",
  "serde_json",
  "thiserror",
  "tracing",
  "url",
  "urlencoding",
@@ -4471,15 +4470,15 @@
 name = "uuid"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 
 [[package]]
 name = "uv"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "anstream",
  "anyhow",
  "assert_cmd",
  "assert_fs",
  "axoupdater",
  "base64 0.22.1",
@@ -5054,15 +5053,15 @@
  "uv-configuration",
  "uv-interpreter",
  "uv-normalize",
 ]
 
 [[package]]
 name = "uv-version"
-version = "0.2.0"
+version = "0.2.1"
 
 [[package]]
 name = "uv-virtualenv"
 version = "0.0.4"
 dependencies = [
  "fs-err",
  "itertools 0.13.0",
```

### Comparing `uv-0.2.0/Cargo.toml` & `uv-0.2.1/Cargo.toml`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/pyproject.toml` & `uv-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "uv"
-version = "0.2.0"
+version = "0.2.1"
 description = "An extremely fast Python package installer and resolver, written in Rust."
 authors = [{ name = "Astral Software Inc.", email = "hey@astral.sh" }]
 requires-python = ">=3.8"
 keywords = [
   "uv", "requirements", "packaging"
 ]
 classifiers = [
```

### Comparing `uv-0.2.0/python/uv/__main__.py` & `uv-0.2.1/python/uv/__main__.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/python/uv/__init__.py` & `uv-0.2.1/python/uv/__init__.py`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/README.md` & `uv-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/LICENSE-APACHE` & `uv-0.2.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/LICENSE-MIT` & `uv-0.2.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `uv-0.2.0/PKG-INFO` & `uv-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uv
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

