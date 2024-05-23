# Comparing `tmp/glean_sdk-60.1.0.tar.gz` & `tmp/glean_sdk-60.2.0.tar.gz`

## Comparing `glean_sdk-60.1.0.tar` & `glean_sdk-60.2.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0     1001     1002     1893 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/Cargo.toml
--rw-r--r--   0     1001     1002    16725 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/LICENSE
--rw-r--r--   0     1001     1002     1699 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/README.md
--rw-r--r--   0     1001     1002       76 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/build.rs
--rw-r--r--   0     1001     1002     4699 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/common_metric_data.rs
--rw-r--r--   0     1001     1002    36926 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/core/mod.rs
--rw-r--r--   0     1001     1002     7409 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/core_metrics.rs
--rw-r--r--   0     1001     1002     1776 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/coverage.rs
--rw-r--r--   0     1001     1002    66424 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/database/mod.rs
--rw-r--r--   0     1001     1002    10907 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/debug.rs
--rw-r--r--   0     1001     1002     7202 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/dispatcher/global.rs
--rw-r--r--   0     1001     1002    19263 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/dispatcher/mod.rs
--rw-r--r--   0     1001     1002     4755 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/error.rs
--rw-r--r--   0     1001     1002     8335 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/error_recording.rs
--rw-r--r--   0     1001     1002    48891 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/event_database/mod.rs
--rw-r--r--   0     1001     1002     2603 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/fd_logger.rs
--rw-r--r--   0     1001     1002    18704 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/glean.udl
--rw-r--r--   0     1001     1002      899 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/glean_metrics.rs
--rw-r--r--   0     1001     1002     6938 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/histogram/exponential.rs
--rw-r--r--   0     1001     1002     5764 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/histogram/functional.rs
--rw-r--r--   0     1001     1002     5770 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/histogram/linear.rs
--rw-r--r--   0     1001     1002     3930 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/histogram/mod.rs
--rw-r--r--   0     1001     1002    10750 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/internal_metrics.rs
--rw-r--r--   0     1001     1002     2534 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/internal_pings.rs
--rw-r--r--   0     1001     1002    47569 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/lib.rs
--rw-r--r--   0     1001     1002    41835 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/lib_unit_tests.rs
--rw-r--r--   0     1001     1002     4061 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/boolean.rs
--rw-r--r--   0     1001     1002     5241 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/counter.rs
--rw-r--r--   0     1001     1002     8437 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/custom_distribution.rs
--rw-r--r--   0     1001     1002    10449 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/datetime.rs
--rw-r--r--   0     1001     1002     4572 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/denominator.rs
--rw-r--r--   0     1001     1002     7478 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/event.rs
--rw-r--r--   0     1001     1002     9850 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/experiment.rs
--rw-r--r--   0     1001     1002     9862 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/labeled.rs
--rw-r--r--   0     1001     1002     9793 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/memory_distribution.rs
--rw-r--r--   0     1001     1002     1809 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/memory_unit.rs
--rw-r--r--   0     1001     1002    12047 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/mod.rs
--rw-r--r--   0     1001     1002     2959 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/numerator.rs
--rw-r--r--   0     1001     1002     5239 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/object.rs
--rw-r--r--   0     1001     1002    10983 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/ping.rs
--rw-r--r--   0     1001     1002     3818 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/quantity.rs
--rw-r--r--   0     1001     1002     5963 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/rate.rs
--rw-r--r--   0     1001     1002     1573 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/recorded_experiment.rs
--rw-r--r--   0     1001     1002     1797 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/remote_settings_config.rs
--rw-r--r--   0     1001     1002     5363 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/string.rs
--rw-r--r--   0     1001     1002     6514 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/string_list.rs
--rw-r--r--   0     1001     1002     5544 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/text.rs
--rw-r--r--   0     1001     1002     3768 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/time_unit.rs
--rw-r--r--   0     1001     1002    10380 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/timespan.rs
--rw-r--r--   0     1001     1002    21230 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/timing_distribution.rs
--rw-r--r--   0     1001     1002    10222 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/url.rs
--rw-r--r--   0     1001     1002     5063 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/metrics/uuid.rs
--rw-r--r--   0     1001     1002    15471 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/ping/mod.rs
--rw-r--r--   0     1001     1002    23631 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/scheduler.rs
--rw-r--r--   0     1001     1002     9495 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/storage/mod.rs
--rw-r--r--   0     1001     1002     2856 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/system.rs
--rw-r--r--   0     1001     1002     1380 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/boolean.rs
--rw-r--r--   0     1001     1002     1497 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/counter.rs
--rw-r--r--   0     1001     1002     2615 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/custom_distribution.rs
--rw-r--r--   0     1001     1002     1759 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/datetime.rs
--rw-r--r--   0     1001     1002     3788 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/event.rs
--rw-r--r--   0     1001     1002     1519 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/labeled.rs
--rw-r--r--   0     1001     1002     1804 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/memory_distribution.rs
--rw-r--r--   0     1001     1002     1642 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/mod.rs
--rw-r--r--   0     1001     1002     1584 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/numerator.rs
--rw-r--r--   0     1001     1002     1730 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/object.rs
--rw-r--r--   0     1001     1002      665 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/ping.rs
--rw-r--r--   0     1001     1002     1481 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/quantity.rs
--rw-r--r--   0     1001     1002     1823 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/rate.rs
--rw-r--r--   0     1001     1002     1574 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/string.rs
--rw-r--r--   0     1001     1002     1971 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/string_list.rs
--rw-r--r--   0     1001     1002     1568 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/text.rs
--rw-r--r--   0     1001     1002     2403 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/timespan.rs
--rw-r--r--   0     1001     1002     6069 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/timing_distribution.rs
--rw-r--r--   0     1001     1002     1645 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/url.rs
--rw-r--r--   0     1001     1002     1528 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/traits/uuid.rs
--rw-r--r--   0     1001     1002    16472 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/upload/directory.rs
--rw-r--r--   0     1001     1002    68645 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/upload/mod.rs
--rw-r--r--   0     1001     1002     3830 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/upload/policy.rs
--rw-r--r--   0     1001     1002    10852 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/upload/request.rs
--rw-r--r--   0     1001     1002     3150 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/upload/result.rs
--rw-r--r--   0     1001     1002    10750 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/src/util.rs
--rw-r--r--   0     1001     1002     2829 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/boolean.rs
--rw-r--r--   0     1001     1002     5330 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/common/mod.rs
--rw-r--r--   0     1001     1002     5294 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/counter.rs
--rw-r--r--   0     1001     1002    13398 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/custom_distribution.rs
--rw-r--r--   0     1001     1002     5974 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/datetime.rs
--rw-r--r--   0     1001     1002    16332 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/event.rs
--rw-r--r--   0     1001     1002    14418 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/labeled.rs
--rw-r--r--   0     1001     1002     5865 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/memory_distribution.rs
--rw-r--r--   0     1001     1002     3195 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/object.rs
--rw-r--r--   0     1001     1002     8742 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/ping.rs
--rw-r--r--   0     1001     1002    10544 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/ping_maker.rs
--rw-r--r--   0     1001     1002     3611 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/quantity.rs
--rw-r--r--   0     1001     1002     4058 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/rate.rs
--rw-r--r--   0     1001     1002     3314 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/storage.rs
--rw-r--r--   0     1001     1002     3730 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/string.rs
--rw-r--r--   0     1001     1002     7423 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/string_list.rs
--rw-r--r--   0     1001     1002     3470 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/text.rs
--rw-r--r--   0     1001     1002    10155 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/timespan.rs
--rw-r--r--   0     1001     1002    12973 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/timing_distribution.rs
--rw-r--r--   0     1001     1002     3375 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/tests/uuid.rs
--rw-r--r--   0     1001     1002      205 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/uniffi.toml
--rw-r--r--   0     1001     1002      299 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/tools/embedded-uniffi-bindgen/Cargo.toml
--rw-r--r--   0     1001     1002     1902 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/tools/embedded-uniffi-bindgen/README.md
--rw-r--r--   0     1001     1002       67 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/tools/embedded-uniffi-bindgen/src/lib.rs
--rw-r--r--   0     1001     1002     2571 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/tools/embedded-uniffi-bindgen/src/main.rs
--rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 glean_sdk-60.1.0/glean-core/bundle/Cargo.toml
--rw-r--r--   0     1001     1002    18704 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/bundle/src/glean.udl
--rw-r--r--   0     1001     1002      973 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/bundle/src/lib.rs
--rw-r--r--   0     1001     1002      205 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/bundle/uniffi.toml
--rw-r--r--   0     1001     1002    32669 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/Cargo.lock
--rw-r--r--   0        0        0      208 1970-01-01 00:00:00.000000 glean_sdk-60.1.0/Cargo.toml
--rw-r--r--   0     1001     1002     1209 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/pyproject.toml
--rw-r--r--   0     1001     1002     1479 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/__init__.py
--rw-r--r--   0     1001     1002      585 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_builtins.py
--rw-r--r--   0     1001     1002     1698 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_ffi.py
--rw-r--r--   0     1001     1002    12757 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_loader.py
--rw-r--r--   0     1001     1002     5161 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_process_dispatcher.py
--rw-r--r--   0     1001     1002      199 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_subprocess/__init__.py
--rw-r--r--   0     1001     1002     1336 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py
--rw-r--r--   0     1001     1002     1502 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/_util.py
--rw-r--r--   0     1001     1002     4278 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/config.py
--rw-r--r--   0     1001     1002    15982 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/glean.py
--rw-r--r--   0     1001     1002    23717 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics.yaml
--rw-r--r--   0     1001     1002     2034 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/__init__.py
--rw-r--r--   0     1001     1002     3803 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/datetime.py
--rw-r--r--   0     1001     1002     3289 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/event.py
--rw-r--r--   0     1001     1002     3225 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/labeled.py
--rw-r--r--   0     1001     1002     3402 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/object.py
--rw-r--r--   0     1001     1002     2408 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/ping.py
--rw-r--r--   0     1001     1002     1576 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/string.py
--rw-r--r--   0     1001     1002     4395 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/timespan.py
--rw-r--r--   0     1001     1002     5030 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/timing_distribution.py
--rw-r--r--   0     1001     1002     1628 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/url.py
--rw-r--r--   0     1001     1002     1757 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/metrics/uuid.py
--rw-r--r--   0     1001     1002      522 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/net/__init__.py
--rw-r--r--   0     1001     1002     1569 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/net/base_uploader.py
--rw-r--r--   0     1001     1002     3211 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/net/http_client.py
--rw-r--r--   0     1001     1002     5200 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/net/ping_upload_worker.py
--rw-r--r--   0     1001     1002     1068 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/net/ping_uploader.py
--rw-r--r--   0     1001     1002     5383 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/pings.yaml
--rw-r--r--   0     1001     1002     2883 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/glean-core/python/glean/testing/__init__.py
--rw-r--r--   0     1001     1002     3773 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/README.md
--rw-r--r--   0     1001     1002    16725 2024-05-06 10:11:07.000000 glean_sdk-60.1.0/LICENSE
--rw-r--r--   0        0        0     4703 1970-01-01 00:00:00.000000 glean_sdk-60.1.0/PKG-INFO
+-rw-r--r--   0     1001     1002     1893 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/Cargo.toml
+-rw-r--r--   0     1001     1002    16725 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/LICENSE
+-rw-r--r--   0     1001     1002     1699 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/README.md
+-rw-r--r--   0     1001     1002       76 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/build.rs
+-rw-r--r--   0     1001     1002     4699 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/common_metric_data.rs
+-rw-r--r--   0     1001     1002    37130 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/core/mod.rs
+-rw-r--r--   0     1001     1002     7409 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/core_metrics.rs
+-rw-r--r--   0     1001     1002     1776 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/coverage.rs
+-rw-r--r--   0     1001     1002    66424 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/database/mod.rs
+-rw-r--r--   0     1001     1002    10907 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/debug.rs
+-rw-r--r--   0     1001     1002     7202 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/dispatcher/global.rs
+-rw-r--r--   0     1001     1002    19263 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/dispatcher/mod.rs
+-rw-r--r--   0     1001     1002     4755 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/error.rs
+-rw-r--r--   0     1001     1002     8335 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/error_recording.rs
+-rw-r--r--   0     1001     1002    48891 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/event_database/mod.rs
+-rw-r--r--   0     1001     1002     2603 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/fd_logger.rs
+-rw-r--r--   0     1001     1002    18756 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/glean.udl
+-rw-r--r--   0     1001     1002      899 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/glean_metrics.rs
+-rw-r--r--   0     1001     1002     6938 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/histogram/exponential.rs
+-rw-r--r--   0     1001     1002     5764 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/histogram/functional.rs
+-rw-r--r--   0     1001     1002     5770 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/histogram/linear.rs
+-rw-r--r--   0     1001     1002     3930 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/histogram/mod.rs
+-rw-r--r--   0     1001     1002    10750 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/internal_metrics.rs
+-rw-r--r--   0     1001     1002     2534 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/internal_pings.rs
+-rw-r--r--   0     1001     1002    47787 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/lib.rs
+-rw-r--r--   0     1001     1002    41878 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/lib_unit_tests.rs
+-rw-r--r--   0     1001     1002     4061 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/boolean.rs
+-rw-r--r--   0     1001     1002     5241 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/counter.rs
+-rw-r--r--   0     1001     1002     8437 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/custom_distribution.rs
+-rw-r--r--   0     1001     1002    10449 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/datetime.rs
+-rw-r--r--   0     1001     1002     4572 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/denominator.rs
+-rw-r--r--   0     1001     1002     7478 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/event.rs
+-rw-r--r--   0     1001     1002     9850 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/experiment.rs
+-rw-r--r--   0     1001     1002     9862 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/labeled.rs
+-rw-r--r--   0     1001     1002     9793 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/memory_distribution.rs
+-rw-r--r--   0     1001     1002     1809 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/memory_unit.rs
+-rw-r--r--   0     1001     1002    12047 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/mod.rs
+-rw-r--r--   0     1001     1002     2959 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/numerator.rs
+-rw-r--r--   0     1001     1002     5239 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/object.rs
+-rw-r--r--   0     1001     1002    11699 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/ping.rs
+-rw-r--r--   0     1001     1002     3818 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/quantity.rs
+-rw-r--r--   0     1001     1002     5963 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/rate.rs
+-rw-r--r--   0     1001     1002     1573 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/recorded_experiment.rs
+-rw-r--r--   0     1001     1002     1797 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/remote_settings_config.rs
+-rw-r--r--   0     1001     1002     5363 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/string.rs
+-rw-r--r--   0     1001     1002     6514 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/string_list.rs
+-rw-r--r--   0     1001     1002     5544 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/text.rs
+-rw-r--r--   0     1001     1002     3768 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/time_unit.rs
+-rw-r--r--   0     1001     1002    10380 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/timespan.rs
+-rw-r--r--   0     1001     1002    21230 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/timing_distribution.rs
+-rw-r--r--   0     1001     1002    10222 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/url.rs
+-rw-r--r--   0     1001     1002     5063 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/uuid.rs
+-rw-r--r--   0     1001     1002    15471 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/ping/mod.rs
+-rw-r--r--   0     1001     1002    23631 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/scheduler.rs
+-rw-r--r--   0     1001     1002     9495 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/storage/mod.rs
+-rw-r--r--   0     1001     1002     2856 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/system.rs
+-rw-r--r--   0     1001     1002     1380 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/boolean.rs
+-rw-r--r--   0     1001     1002     1497 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/counter.rs
+-rw-r--r--   0     1001     1002     2615 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/custom_distribution.rs
+-rw-r--r--   0     1001     1002     1759 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/datetime.rs
+-rw-r--r--   0     1001     1002     3788 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/event.rs
+-rw-r--r--   0     1001     1002     1519 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/labeled.rs
+-rw-r--r--   0     1001     1002     1804 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/memory_distribution.rs
+-rw-r--r--   0     1001     1002     1642 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/mod.rs
+-rw-r--r--   0     1001     1002     1584 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/numerator.rs
+-rw-r--r--   0     1001     1002     1730 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/object.rs
+-rw-r--r--   0     1001     1002      665 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/ping.rs
+-rw-r--r--   0     1001     1002     1481 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/quantity.rs
+-rw-r--r--   0     1001     1002     1823 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/rate.rs
+-rw-r--r--   0     1001     1002     1574 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/string.rs
+-rw-r--r--   0     1001     1002     1971 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/string_list.rs
+-rw-r--r--   0     1001     1002     1568 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/text.rs
+-rw-r--r--   0     1001     1002     2403 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/timespan.rs
+-rw-r--r--   0     1001     1002     6069 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/timing_distribution.rs
+-rw-r--r--   0     1001     1002     1645 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/url.rs
+-rw-r--r--   0     1001     1002     1528 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/uuid.rs
+-rw-r--r--   0     1001     1002    16472 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/upload/directory.rs
+-rw-r--r--   0     1001     1002    68645 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/upload/mod.rs
+-rw-r--r--   0     1001     1002     3830 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/upload/policy.rs
+-rw-r--r--   0     1001     1002    10852 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/upload/request.rs
+-rw-r--r--   0     1001     1002     3150 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/upload/result.rs
+-rw-r--r--   0     1001     1002    10750 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/util.rs
+-rw-r--r--   0     1001     1002     2829 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/boolean.rs
+-rw-r--r--   0     1001     1002     5373 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/common/mod.rs
+-rw-r--r--   0     1001     1002     5294 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/counter.rs
+-rw-r--r--   0     1001     1002    13398 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/custom_distribution.rs
+-rw-r--r--   0     1001     1002     5974 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/datetime.rs
+-rw-r--r--   0     1001     1002    16375 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/event.rs
+-rw-r--r--   0     1001     1002    14418 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/labeled.rs
+-rw-r--r--   0     1001     1002     5865 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/memory_distribution.rs
+-rw-r--r--   0     1001     1002     3195 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/object.rs
+-rw-r--r--   0     1001     1002     8742 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/ping.rs
+-rw-r--r--   0     1001     1002    10630 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/ping_maker.rs
+-rw-r--r--   0     1001     1002     3611 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/quantity.rs
+-rw-r--r--   0     1001     1002     4058 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/rate.rs
+-rw-r--r--   0     1001     1002     3314 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/storage.rs
+-rw-r--r--   0     1001     1002     3730 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/string.rs
+-rw-r--r--   0     1001     1002     7423 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/string_list.rs
+-rw-r--r--   0     1001     1002     3470 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/text.rs
+-rw-r--r--   0     1001     1002    10155 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/timespan.rs
+-rw-r--r--   0     1001     1002    12973 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/timing_distribution.rs
+-rw-r--r--   0     1001     1002     3375 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/uuid.rs
+-rw-r--r--   0     1001     1002      205 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/uniffi.toml
+-rw-r--r--   0     1001     1002      299 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/tools/embedded-uniffi-bindgen/Cargo.toml
+-rw-r--r--   0     1001     1002     1902 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/tools/embedded-uniffi-bindgen/README.md
+-rw-r--r--   0     1001     1002       67 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/tools/embedded-uniffi-bindgen/src/lib.rs
+-rw-r--r--   0     1001     1002     2571 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/tools/embedded-uniffi-bindgen/src/main.rs
+-rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 glean_sdk-60.2.0/glean-core/bundle/Cargo.toml
+-rw-r--r--   0     1001     1002    18756 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/bundle/src/glean.udl
+-rw-r--r--   0     1001     1002      973 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/bundle/src/lib.rs
+-rw-r--r--   0     1001     1002      205 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/bundle/uniffi.toml
+-rw-r--r--   0     1001     1002    32669 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/Cargo.lock
+-rw-r--r--   0        0        0      208 1970-01-01 00:00:00.000000 glean_sdk-60.2.0/Cargo.toml
+-rw-r--r--   0     1001     1002     1209 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/pyproject.toml
+-rw-r--r--   0     1001     1002     1479 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/__init__.py
+-rw-r--r--   0     1001     1002      585 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_builtins.py
+-rw-r--r--   0     1001     1002     1698 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_ffi.py
+-rw-r--r--   0     1001     1002    12757 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_loader.py
+-rw-r--r--   0     1001     1002     5161 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_process_dispatcher.py
+-rw-r--r--   0     1001     1002      199 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_subprocess/__init__.py
+-rw-r--r--   0     1001     1002     1336 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py
+-rw-r--r--   0     1001     1002     1502 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_util.py
+-rw-r--r--   0     1001     1002     4278 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/config.py
+-rw-r--r--   0     1001     1002    16012 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/glean.py
+-rw-r--r--   0     1001     1002    23717 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics.yaml
+-rw-r--r--   0     1001     1002     2034 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/__init__.py
+-rw-r--r--   0     1001     1002     3803 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/datetime.py
+-rw-r--r--   0     1001     1002     3289 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/event.py
+-rw-r--r--   0     1001     1002     3225 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/labeled.py
+-rw-r--r--   0     1001     1002     3402 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/object.py
+-rw-r--r--   0     1001     1002     2408 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/ping.py
+-rw-r--r--   0     1001     1002     1576 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/string.py
+-rw-r--r--   0     1001     1002     4395 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/timespan.py
+-rw-r--r--   0     1001     1002     5030 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/timing_distribution.py
+-rw-r--r--   0     1001     1002     1628 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/url.py
+-rw-r--r--   0     1001     1002     1757 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/uuid.py
+-rw-r--r--   0     1001     1002      522 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/net/__init__.py
+-rw-r--r--   0     1001     1002     1569 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/net/base_uploader.py
+-rw-r--r--   0     1001     1002     3211 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/net/http_client.py
+-rw-r--r--   0     1001     1002     5230 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/net/ping_upload_worker.py
+-rw-r--r--   0     1001     1002     1068 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/net/ping_uploader.py
+-rw-r--r--   0     1001     1002     5383 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/pings.yaml
+-rw-r--r--   0     1001     1002     2883 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/testing/__init__.py
+-rw-r--r--   0     1001     1002     3773 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/README.md
+-rw-r--r--   0     1001     1002    16725 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/LICENSE
+-rw-r--r--   0        0        0     4703 1970-01-01 00:00:00.000000 glean_sdk-60.2.0/PKG-INFO
```

### Comparing `glean_sdk-60.1.0/glean-core/Cargo.toml` & `glean_sdk-60.2.0/glean-core/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "glean-core"
-version = "60.1.0"
+version = "60.2.0"
 authors = ["Jan-Erik Rediger <jrediger@mozilla.com>", "The Glean Team <glean-team@mozilla.com>"]
 description = "A modern Telemetry library"
 repository = "https://github.com/mozilla/glean"
 readme = "README.md"
 license = "MPL-2.0"
 edition = "2021"
 keywords = ["telemetry"]
```

### Comparing `glean_sdk-60.1.0/glean-core/LICENSE` & `glean_sdk-60.2.0/glean-core/LICENSE`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/README.md` & `glean_sdk-60.2.0/glean-core/README.md`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/common_metric_data.rs` & `glean_sdk-60.2.0/glean-core/src/common_metric_data.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/core/mod.rs` & `glean_sdk-60.2.0/glean-core/src/core/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 ///     use_core_mps: false,
 ///     trim_data_to_registered_pings: false,
 ///     log_level: None,
 ///     rate_limit: None,
 ///     enable_event_timestamps: true,
 ///     experimentation_id: None,
 ///     enable_internal_pings: true,
+///     ping_schedule: Default::default(),
 /// };
 /// let mut glean = Glean::new(cfg).unwrap();
 /// let ping = PingType::new("sample", true, false, true, true, true, vec![], vec![]);
 /// glean.register_ping_type(&ping);
 ///
 /// let call_counter: CounterMetric = CounterMetric::new(CommonMetricData {
 ///     name: "calls".into(),
@@ -160,14 +161,15 @@
     pub(crate) upload_manager: PingUploadManager,
     debug: DebugOptions,
     pub(crate) app_build: String,
     pub(crate) schedule_metrics_pings: bool,
     pub(crate) remote_settings_epoch: AtomicU8,
     pub(crate) remote_settings_config: Arc<Mutex<RemoteSettingsConfig>>,
     pub(crate) with_timestamps: bool,
+    pub(crate) ping_schedule: HashMap<String, Vec<String>>,
 }
 
 impl Glean {
     /// Creates and initializes a new Glean object for use in a subprocess.
     ///
     /// Importantly, this will not send any pings at startup, since that
     /// sort of management should only happen in the main process.
@@ -220,14 +222,15 @@
             debug: DebugOptions::new(),
             app_build: cfg.app_build.to_string(),
             // Subprocess doesn't use "metrics" pings so has no need for a scheduler.
             schedule_metrics_pings: false,
             remote_settings_epoch: AtomicU8::new(0),
             remote_settings_config: Arc::new(Mutex::new(RemoteSettingsConfig::new())),
             with_timestamps: cfg.enable_event_timestamps,
+            ping_schedule: cfg.ping_schedule.clone(),
         };
 
         // Ensuring these pings are registered.
         let pings = this.internal_pings.clone();
         this.register_ping_type(&pings.baseline);
         this.register_ping_type(&pings.metrics);
         this.register_ping_type(&pings.events);
@@ -321,14 +324,15 @@
             use_core_mps: false,
             trim_data_to_registered_pings: false,
             log_level: None,
             rate_limit: None,
             enable_event_timestamps: true,
             experimentation_id: None,
             enable_internal_pings,
+            ping_schedule: Default::default(),
         };
 
         let mut glean = Self::new(cfg).unwrap();
 
         // Disable all upload manager policies for testing
         glean.upload_manager = PingUploadManager::no_policy(data_path);
```

### Comparing `glean_sdk-60.1.0/glean-core/src/core_metrics.rs` & `glean_sdk-60.2.0/glean-core/src/core_metrics.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/coverage.rs` & `glean_sdk-60.2.0/glean-core/src/coverage.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/database/mod.rs` & `glean_sdk-60.2.0/glean-core/src/database/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/debug.rs` & `glean_sdk-60.2.0/glean-core/src/debug.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/dispatcher/global.rs` & `glean_sdk-60.2.0/glean-core/src/dispatcher/global.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/dispatcher/mod.rs` & `glean_sdk-60.2.0/glean-core/src/dispatcher/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/error.rs` & `glean_sdk-60.2.0/glean-core/src/error.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/error_recording.rs` & `glean_sdk-60.2.0/glean-core/src/error_recording.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/event_database/mod.rs` & `glean_sdk-60.2.0/glean-core/src/event_database/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/fd_logger.rs` & `glean_sdk-60.2.0/glean-core/src/fd_logger.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/glean.udl` & `glean_sdk-60.2.0/glean-core/src/glean.udl`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     boolean use_core_mps;
     boolean trim_data_to_registered_pings;
     LevelFilter? log_level;
     PingRateLimit? rate_limit;
     boolean enable_event_timestamps;
     string? experimentation_id;
     boolean enable_internal_pings;
+    record<string, sequence<string>> ping_schedule;
 };
 
 // How to specify the rate pings may be uploaded before they are throttled.
 dictionary PingRateLimit {
     u64 seconds_per_interval;
     u32 pings_per_interval;
 };
```

### Comparing `glean_sdk-60.1.0/glean-core/src/glean_metrics.rs` & `glean_sdk-60.2.0/glean-core/src/glean_metrics.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/histogram/exponential.rs` & `glean_sdk-60.2.0/glean-core/src/histogram/exponential.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/histogram/functional.rs` & `glean_sdk-60.2.0/glean-core/src/histogram/functional.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/histogram/linear.rs` & `glean_sdk-60.2.0/glean-core/src/histogram/linear.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/histogram/mod.rs` & `glean_sdk-60.2.0/glean-core/src/histogram/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/internal_metrics.rs` & `glean_sdk-60.2.0/glean-core/src/internal_metrics.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/internal_pings.rs` & `glean_sdk-60.2.0/glean-core/src/internal_pings.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/lib.rs` & `glean_sdk-60.2.0/glean-core/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,18 @@
     pub enable_event_timestamps: bool,
     /// An experimentation identifier derived by the application to be sent with all pings, it should
     /// be noted that this has an underlying StringMetric and so should conform to the limitations that
     /// StringMetric places on length, etc.
     pub experimentation_id: Option<String>,
     /// Whether to enable internal pings. Default: true
     pub enable_internal_pings: bool,
+    /// A ping schedule map.
+    /// Maps a ping name to a list of pings to schedule along with it.
+    /// Only used if the ping's own ping schedule list is empty.
+    pub ping_schedule: HashMap<String, Vec<String>>,
 }
 
 /// How to specify the rate at which pings may be uploaded before they are throttled.
 #[derive(Debug, Clone)]
 pub struct PingRateLimit {
     /// Length of time in seconds of a ping uploading interval.
     pub seconds_per_interval: u64,
```

### Comparing `glean_sdk-60.1.0/glean-core/src/lib_unit_tests.rs` & `glean_sdk-60.2.0/glean-core/src/lib_unit_tests.rs`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,15 @@
         use_core_mps: false,
         trim_data_to_registered_pings: false,
         log_level: None,
         rate_limit: None,
         enable_event_timestamps: true,
         experimentation_id: Some(experimentation_id.to_string()),
         enable_internal_pings: true,
+        ping_schedule: Default::default(),
     })
     .unwrap();
 
     // Check that the correct value was stored
     if let Some(exp_id) = glean
         .additional_metrics
         .experimentation_id
```

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/boolean.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/boolean.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/counter.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/counter.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/custom_distribution.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/custom_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/datetime.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/datetime.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/denominator.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/denominator.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/event.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/event.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/experiment.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/experiment.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/labeled.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/labeled.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/memory_distribution.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/memory_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/memory_unit.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/memory_unit.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/mod.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/numerator.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/numerator.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/object.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/object.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/ping.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/ping.rs`

 * *Files 6% similar despite different names*

```diff
@@ -279,15 +279,33 @@
                 glean.upload_manager.enqueue_ping_from_file(glean, &doc_id);
 
                 log::info!(
                     "The ping '{}' was submitted and will be sent as soon as possible",
                     ping.name
                 );
 
-                if !ping.schedules_pings.is_empty() {
+                if ping.schedules_pings.is_empty() {
+                    let ping_schedule = glean
+                        .ping_schedule
+                        .get(ping.name)
+                        .map(|v| &v[..])
+                        .unwrap_or(&[]);
+
+                    if !ping_schedule.is_empty() {
+                        log::info!(
+                            "The ping '{}' is being used to schedule other pings: {:?}",
+                            ping.name,
+                            ping_schedule
+                        );
+
+                        for scheduled_ping_name in ping_schedule {
+                            glean.submit_ping_by_name(scheduled_ping_name, reason);
+                        }
+                    }
+                } else {
                     log::info!(
                         "The ping '{}' is being used to schedule other pings: {:?}",
                         ping.name,
                         ping.schedules_pings
                     );
                     for scheduled_ping_name in &ping.schedules_pings {
                         glean.submit_ping_by_name(scheduled_ping_name, reason);
```

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/quantity.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/quantity.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/rate.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/rate.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/recorded_experiment.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/recorded_experiment.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/remote_settings_config.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/remote_settings_config.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/string.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/string.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/string_list.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/string_list.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/text.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/text.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/time_unit.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/time_unit.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/timespan.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/timespan.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/timing_distribution.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/timing_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/url.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/url.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/metrics/uuid.rs` & `glean_sdk-60.2.0/glean-core/src/metrics/uuid.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/ping/mod.rs` & `glean_sdk-60.2.0/glean-core/src/ping/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/scheduler.rs` & `glean_sdk-60.2.0/glean-core/src/scheduler.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/storage/mod.rs` & `glean_sdk-60.2.0/glean-core/src/storage/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/system.rs` & `glean_sdk-60.2.0/glean-core/src/system.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/boolean.rs` & `glean_sdk-60.2.0/glean-core/src/traits/boolean.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/counter.rs` & `glean_sdk-60.2.0/glean-core/src/traits/counter.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/custom_distribution.rs` & `glean_sdk-60.2.0/glean-core/src/traits/custom_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/datetime.rs` & `glean_sdk-60.2.0/glean-core/src/traits/datetime.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/event.rs` & `glean_sdk-60.2.0/glean-core/src/traits/event.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/labeled.rs` & `glean_sdk-60.2.0/glean-core/src/traits/labeled.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/memory_distribution.rs` & `glean_sdk-60.2.0/glean-core/src/traits/memory_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/mod.rs` & `glean_sdk-60.2.0/glean-core/src/traits/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/numerator.rs` & `glean_sdk-60.2.0/glean-core/src/traits/numerator.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/object.rs` & `glean_sdk-60.2.0/glean-core/src/traits/object.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/ping.rs` & `glean_sdk-60.2.0/glean-core/src/traits/ping.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/quantity.rs` & `glean_sdk-60.2.0/glean-core/src/traits/quantity.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/rate.rs` & `glean_sdk-60.2.0/glean-core/src/traits/rate.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/string.rs` & `glean_sdk-60.2.0/glean-core/src/traits/string.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/string_list.rs` & `glean_sdk-60.2.0/glean-core/src/traits/string_list.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/text.rs` & `glean_sdk-60.2.0/glean-core/src/traits/text.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/timespan.rs` & `glean_sdk-60.2.0/glean-core/src/traits/timespan.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/timing_distribution.rs` & `glean_sdk-60.2.0/glean-core/src/traits/timing_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/url.rs` & `glean_sdk-60.2.0/glean-core/src/traits/url.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/traits/uuid.rs` & `glean_sdk-60.2.0/glean-core/src/traits/uuid.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/upload/directory.rs` & `glean_sdk-60.2.0/glean-core/src/upload/directory.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/upload/mod.rs` & `glean_sdk-60.2.0/glean-core/src/upload/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/upload/policy.rs` & `glean_sdk-60.2.0/glean-core/src/upload/policy.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/upload/request.rs` & `glean_sdk-60.2.0/glean-core/src/upload/request.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/upload/result.rs` & `glean_sdk-60.2.0/glean-core/src/upload/result.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/src/util.rs` & `glean_sdk-60.2.0/glean-core/src/util.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/boolean.rs` & `glean_sdk-60.2.0/glean-core/tests/boolean.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/common/mod.rs` & `glean_sdk-60.2.0/glean-core/tests/common/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         use_core_mps: false,
         trim_data_to_registered_pings: false,
         log_level: None,
         rate_limit: None,
         enable_event_timestamps: false,
         experimentation_id: None,
         enable_internal_pings: true,
+        ping_schedule: Default::default(),
     };
     let glean = Glean::new(cfg).unwrap();
 
     (glean, dir)
 }
 
 /// Converts an iso8601::DateTime to a chrono::DateTime<FixedOffset>
```

### Comparing `glean_sdk-60.1.0/glean-core/tests/counter.rs` & `glean_sdk-60.2.0/glean-core/tests/counter.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/custom_distribution.rs` & `glean_sdk-60.2.0/glean-core/tests/custom_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/datetime.rs` & `glean_sdk-60.2.0/glean-core/tests/datetime.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/event.rs` & `glean_sdk-60.2.0/glean-core/tests/event.rs`

 * *Files 1% similar despite different names*

```diff
@@ -482,14 +482,15 @@
         use_core_mps: false,
         trim_data_to_registered_pings: false,
         log_level: None,
         rate_limit: None,
         enable_event_timestamps: true,
         experimentation_id: None, // Enabling event timestamps
         enable_internal_pings: true,
+        ping_schedule: Default::default(),
     };
     let glean = Glean::new(cfg).unwrap();
 
     let store_name = "store-name";
     let event = EventMetric::new(
         CommonMetricData {
             name: "name".into(),
```

### Comparing `glean_sdk-60.1.0/glean-core/tests/labeled.rs` & `glean_sdk-60.2.0/glean-core/tests/labeled.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/memory_distribution.rs` & `glean_sdk-60.2.0/glean-core/tests/memory_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/object.rs` & `glean_sdk-60.2.0/glean-core/tests/object.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/ping.rs` & `glean_sdk-60.2.0/glean-core/tests/ping.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/ping_maker.rs` & `glean_sdk-60.2.0/glean-core/tests/ping_maker.rs`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         use_core_mps: false,
         trim_data_to_registered_pings: false,
         log_level: None,
         rate_limit: None,
         enable_event_timestamps: true,
         experimentation_id: Some("test-experimentation-id".to_string()),
         enable_internal_pings: true,
+        ping_schedule: Default::default(),
     })
     .unwrap();
     let ping_maker = PingMaker::new();
     let ping_type = PingType::new("store1", true, false, true, true, true, vec![], vec![]);
     glean.register_ping_type(&ping_type);
 
     // Record something, so the ping will have data
@@ -141,14 +142,15 @@
         use_core_mps: false,
         trim_data_to_registered_pings: false,
         log_level: None,
         rate_limit: None,
         enable_event_timestamps: true,
         experimentation_id: Some("test-experimentation-id".to_string()),
         enable_internal_pings: true,
+        ping_schedule: Default::default(),
     })
     .unwrap();
     let ping_maker = PingMaker::new();
 
     let unknown_ping_type = PingType::new("unknown", true, false, true, true, true, vec![], vec![]);
     glean.register_ping_type(&unknown_ping_type);
```

### Comparing `glean_sdk-60.1.0/glean-core/tests/quantity.rs` & `glean_sdk-60.2.0/glean-core/tests/quantity.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/rate.rs` & `glean_sdk-60.2.0/glean-core/tests/rate.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/storage.rs` & `glean_sdk-60.2.0/glean-core/tests/storage.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/string.rs` & `glean_sdk-60.2.0/glean-core/tests/string.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/string_list.rs` & `glean_sdk-60.2.0/glean-core/tests/string_list.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/text.rs` & `glean_sdk-60.2.0/glean-core/tests/text.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/timespan.rs` & `glean_sdk-60.2.0/glean-core/tests/timespan.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/timing_distribution.rs` & `glean_sdk-60.2.0/glean-core/tests/timing_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/tests/uuid.rs` & `glean_sdk-60.2.0/glean-core/tests/uuid.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/tools/embedded-uniffi-bindgen/README.md` & `glean_sdk-60.2.0/tools/embedded-uniffi-bindgen/README.md`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/tools/embedded-uniffi-bindgen/src/main.rs` & `glean_sdk-60.2.0/tools/embedded-uniffi-bindgen/src/main.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/bundle/Cargo.toml` & `glean_sdk-60.2.0/glean-core/bundle/Cargo.toml`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/bundle/src/glean.udl` & `glean_sdk-60.2.0/glean-core/bundle/src/glean.udl`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     boolean use_core_mps;
     boolean trim_data_to_registered_pings;
     LevelFilter? log_level;
     PingRateLimit? rate_limit;
     boolean enable_event_timestamps;
     string? experimentation_id;
     boolean enable_internal_pings;
+    record<string, sequence<string>> ping_schedule;
 };
 
 // How to specify the rate pings may be uploaded before they are throttled.
 dictionary PingRateLimit {
     u64 seconds_per_interval;
     u32 pings_per_interval;
 };
```

### Comparing `glean_sdk-60.1.0/glean-core/bundle/src/lib.rs` & `glean_sdk-60.2.0/glean-core/bundle/src/lib.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/Cargo.lock` & `glean_sdk-60.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "glean"
-version = "60.1.0"
+version = "60.2.0"
 dependencies = [
  "crossbeam-channel",
  "env_logger",
  "flate2",
  "glean-core",
  "inherent",
  "jsonschema-valid",
@@ -355,15 +355,15 @@
 version = "1.0.0"
 dependencies = [
  "glean-core",
 ]
 
 [[package]]
 name = "glean-core"
-version = "60.1.0"
+version = "60.2.0"
 dependencies = [
  "android_logger",
  "bincode",
  "chrono",
  "crossbeam-channel",
  "ctor",
  "env_logger",
```

### Comparing `glean_sdk-60.1.0/pyproject.toml` & `glean_sdk-60.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "glean-sdk"
-version = "60.1.0"
+version = "60.2.0"
 requires-python = ">=3.8"
 classifiers = [
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: 3",
```

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/__init__.py` & `glean_sdk-60.2.0/glean-core/python/glean/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/_builtins.py` & `glean_sdk-60.2.0/glean-core/python/glean/_builtins.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/_ffi.py` & `glean_sdk-60.2.0/glean-core/python/glean/_ffi.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/_loader.py` & `glean_sdk-60.2.0/glean-core/python/glean/_loader.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/_process_dispatcher.py` & `glean_sdk-60.2.0/glean-core/python/glean/_process_dispatcher.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py` & `glean_sdk-60.2.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/_util.py` & `glean_sdk-60.2.0/glean-core/python/glean/_util.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/config.py` & `glean_sdk-60.2.0/glean-core/python/glean/config.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/glean.py` & `glean_sdk-60.2.0/glean-core/python/glean/glean.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,14 +230,15 @@
             app_build=cls._application_build_id,
             trim_data_to_registered_pings=False,
             log_level=None,
             rate_limit=None,
             enable_event_timestamps=configuration.enable_event_timestamps,
             experimentation_id=configuration.experimentation_id,
             enable_internal_pings=configuration.enable_internal_pings,
+            ping_schedule={},
         )
 
         _uniffi.glean_initialize(cfg, client_info, callbacks)
         cls._initialized = True
 
     @classmethod
     def _initialize_with_tempdir_for_testing(
```

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/metrics.yaml` & `glean_sdk-60.2.0/glean-core/python/glean/metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/metrics/__init__.py` & `glean_sdk-60.2.0/glean-core/python/glean/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/metrics/datetime.py` & `glean_sdk-60.2.0/glean-core/python/glean/metrics/datetime.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/metrics/event.py` & `glean_sdk-60.2.0/glean-core/python/glean/metrics/event.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/metrics/labeled.py` & `glean_sdk-60.2.0/glean-core/python/glean/metrics/labeled.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/metrics/object.py` & `glean_sdk-60.2.0/glean-core/python/glean/metrics/object.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/metrics/ping.py` & `glean_sdk-60.2.0/glean-core/python/glean/metrics/ping.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/metrics/string.py` & `glean_sdk-60.2.0/glean-core/python/glean/metrics/string.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/metrics/timespan.py` & `glean_sdk-60.2.0/glean-core/python/glean/metrics/timespan.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/metrics/timing_distribution.py` & `glean_sdk-60.2.0/glean-core/python/glean/metrics/timing_distribution.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/metrics/url.py` & `glean_sdk-60.2.0/glean-core/python/glean/metrics/url.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/metrics/uuid.py` & `glean_sdk-60.2.0/glean-core/python/glean/metrics/uuid.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/net/__init__.py` & `glean_sdk-60.2.0/glean-core/python/glean/net/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/net/base_uploader.py` & `glean_sdk-60.2.0/glean-core/python/glean/net/base_uploader.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/net/http_client.py` & `glean_sdk-60.2.0/glean-core/python/glean/net/http_client.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/net/ping_upload_worker.py` & `glean_sdk-60.2.0/glean-core/python/glean/net/ping_upload_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
             app_build="",
             trim_data_to_registered_pings=False,
             log_level=None,
             rate_limit=None,
             enable_event_timestamps=False,
             experimentation_id=None,
             enable_internal_pings=False,
+            ping_schedule={},
         )
         if not glean_initialize_for_subprocess(cfg):
             log.error("Couldn't initialize Glean in subprocess")
             sys.exit(1)
 
     # Limits are enforced by glean-core to avoid an inifinite loop here.
     # Whenever a limit is reached, this binding will receive `UploadTaskTag.DONE` and step out.
```

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/net/ping_uploader.py` & `glean_sdk-60.2.0/glean-core/python/glean/net/ping_uploader.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/pings.yaml` & `glean_sdk-60.2.0/glean-core/python/glean/pings.yaml`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/glean-core/python/glean/testing/__init__.py` & `glean_sdk-60.2.0/glean-core/python/glean/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/README.md` & `glean_sdk-60.2.0/README.md`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/LICENSE` & `glean_sdk-60.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.1.0/PKG-INFO` & `glean_sdk-60.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: glean-sdk
-Version: 60.1.0
+Version: 60.2.0
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: semver >=2.13.0
 Requires-Dist: glean-parser ~=14.0
```

