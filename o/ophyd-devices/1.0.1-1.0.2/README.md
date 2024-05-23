# Comparing `tmp/ophyd_devices-1.0.1.tar.gz` & `tmp/ophyd_devices-1.0.2.tar.gz`

## Comparing `ophyd_devices-1.0.1.tar` & `ophyd_devices-1.0.2.tar`

### file list

```diff
@@ -1,385 +1,387 @@
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/README.md
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.git_hooks/pre-commit
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.gitlab/issue_templates/bug_report_template.md
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.gitlab/issue_templates/documentation_update_template.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.gitlab/issue_templates/feature_request_template.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.gitlab/merge_request_templates/default.md
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.gitignore
--rw-r--r--   0        0        0    19162 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.gitlab-ci.yml
--rw-r--r--   0        0        0    18519 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.pylintrc
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.readthedocs.yaml
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/CHANGELOG.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/LICENSE
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/README.md
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_config_template.yaml
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.git_hooks/post-commit
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.git_hooks/pre-commit
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.gitlab/issue_templates/bug_report_template.md
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.gitlab/issue_templates/documentation_update_template.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.gitlab/issue_templates/feature_request_template.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.gitlab/merge_request_templates/default.md
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/demo.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/pyproject.toml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/__init__.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/bec_magics.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/bec_startup.py
--rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/main.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/prettytable.py
--rw-r--r--   0        0        0    11083 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/progressbar.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/signals.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/__init__.py
--rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py
--rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py
--rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/scan_progress.py
--rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/__init__.py
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/conftest.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_bec_client.py
--rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py
--rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_live_table.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_move_callback.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_pretty_table.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_scan_progress.py
--rw-r--r--   0        0        0    25147 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py
--rw-r--r--   0        0        0    11024 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/README.md
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/pyproject.toml
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/__init__.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/alarm_handler.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/async_data.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bec_errors.py
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bec_service.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bec_yaml_loader.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bl_checks.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bl_conditions.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/callback_handler.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/channel_monitor.py
--rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/client.py
--rw-r--r--   0        0        0     9096 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/config_helper.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/connector.py
--rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/dap_plugin_objects.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/dap_plugins.py
--rw-r--r--   0        0        0    30862 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/device.py
--rw-r--r--   0        0        0    23274 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/devicemanager.py
--rw-r--r--   0        0        0    38065 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/endpoints.py
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/file_utils.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/lmfit_serializer.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/logbook_connector.py
--rw-r--r--   0        0        0     8690 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/logger.py
--rw-r--r--   0        0        0    24024 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/messages.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/numpy_encoder.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/observer.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/pdf_writer.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/plugin_helper.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/queue_items.py
--rw-r--r--   0        0        0    41414 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/redis_connector.py
--rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/request_items.py
--rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_data.py
--rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_items.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_manager.py
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_report.py
--rw-r--r--   0        0        0    17050 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scans.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scibec_validator.py
--rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/serialization.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/service_config.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/signature_serializer.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/user_scripts_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/configs/__init__.py
--rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/configs/demo_config.yaml
--rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/configs/openapi_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/__init__.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/fixtures.py
--rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/test_config.yaml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/test_service_config.yaml
--rw-r--r--   0        0        0    22469 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/__init__.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/import_utils.py
--rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/proxy.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/rpc_utils.py
--rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/scan_utils.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/threading_utils.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/conftest.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_async_data.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_beamline_checks.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_bec_logger.py
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_bec_messages.py
--rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_bec_service.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_bl_conditions.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_callback_handler.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_channel_monitor.py
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_config_helper.py
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_core_utils.py
--rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_dap_plugins.py
--rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_device_manager.py
--rw-r--r--   0        0        0    25863 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_devices.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_file_utils.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_import_utils.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_lmfit_serializer.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_observer.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_pdf_writer.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_plugin_helper.py
--rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_redis_connector.py
--rw-r--r--   0        0        0    22103 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_redis_connector_fakeredis.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_context.py
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_data.py
--rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_items.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_manager.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_object.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_report.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scibec_validator.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_serializer.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_signature_serializer.py
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_user_scripts_mixin.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_yaml_loader.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/create_plugin_structure.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/init_config.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/gitignore
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/setup_device_server.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/post-commit
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/pre-commit
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/README.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/pyproject.toml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/launch.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/service_handler.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/dap_server.py
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/dap_service.py
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/dap_service_manager.py
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/lmfit1d_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/cli/__init__.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/cli/launch.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/__init__.py
--rw-r--r--   0        0        0    18918 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/device_server.py
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/rpc_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/cli/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/cli/launch.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/__init__.py
--rw-r--r--   0        0        0     5525 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/config_update_handler.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/device_serializer.py
--rw-r--r--   0        0        0    22491 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/devicemanager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/tests/__init__.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/tests/utils.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/__init__.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/default_writer.py
--rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/file_writer.py
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/file_writer_manager.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/merged_dicts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/cli/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/cli/launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer_plugins/__init__.py
--rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/__init__.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/bec_emitter.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/emitter.py
--rw-r--r--   0        0        0    15950 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/scan_bundler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/cli/__init__.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/cli/launch.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/__init__.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/device_validation.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/errors.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/path_optimization.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_assembler.py
--rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_guard.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_manager.py
--rw-r--r--   0        0        0    34904 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_queue.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_server.py
--rw-r--r--   0        0        0    18406 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_stubs.py
--rw-r--r--   0        0        0    35666 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_worker.py
--rw-r--r--   0        0        0    52628 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/cli/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/cli/launch.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_plugins/__init__.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/tests/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/tests/fixtures.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/tests/utils.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/repeated_timer.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scihub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/cli/__init__.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/cli/launch.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/__init__.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/config_handler.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py
--rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scilog/__init__.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scilog/scilog.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_bec_server_utils/test_main.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/conftest.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_dap_server.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/conftest.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_config_handler.py
--rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_serializer.py
--rw-r--r--   0        0        0    28297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_server.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py
--rw-r--r--   0        0        0     9555 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/conftest.py
--rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/test_file_writer.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py
--rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/conftest.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_emitter.py
--rw-r--r--   0        0        0    25388 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/conftest.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_path_optimization.py
--rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_guard.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py
--rw-r--r--   0        0        0    27483 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py
--rw-r--r--   0        0        0    54003 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_worker.py
--rw-r--r--   0        0        0    87794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scans.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/conftest.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_repeated_timer.py
--rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scibec_connector.py
--rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scilog_connector.py
--rwxr-xr-x   0        0        0     3629 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bin/install_bec_dev.sh
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/Dockerfile.run_pytest
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/Dockerfile.run_server
--rwxr-xr-x   0        0        0      347 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/build_python_services.sh
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/docker-compose.yaml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/functionalAccounts.json
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/semantic_release.toml
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/test_config.yaml
--rw-r--r--   0        0        0   307212 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/architecture/BEC.drawio
--rw-r--r--   0        0        0   124683 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/architecture/BEC_config_db.drawio
--rw-r--r--   0        0        0    11580 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/architecture/BEC_config_db.svg
--rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/architecture/bec_architecture.png
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/Makefile
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/conf.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/make.bat
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/requirements.txt
--rw-r--r--   0        0        0    41260 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/_static/bec.png
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/_static/switcher.json
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/_static/css/custom.css
--rw-r--r--   0        0        0  4672990 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/_static/gif/bec_plotter.gif
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0        0        0   310535 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/BEC_context_user_centric.png
--rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/bec_architecture.png
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/bec_device_structure.drawio
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/bec_device_structure.png
--rw-r--r--   0        0        0    17460 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/gauss_scatter_plot.png
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/simulation_context_diagram.drawio
--rw-r--r--   0        0        0    69323 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/simulation_context_diagram.png
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/tab-complete-devices.png
--rw-r--r--   0        0        0    37244 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/vscode_debug_button.png
--rw-r--r--   0        0        0   374770 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/vscode_with_annotations.drawio
--rw-r--r--   0        0        0   711275 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/vscode_with_annotations.png
--rw-r--r--   0        0        0    96330 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/wm-devices.png
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/architecture.md
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/bec_cli.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/bec_config.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/bec_gui.md
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/bec_plugins.md
--rw-r--r--   0        0        0     9531 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/bec_sim.md
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/contributing.md
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/data_access.md
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/developer.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/event_data.md
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/external_sources.md
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/glossary.md
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/install_developer_env.md
--rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/logs.md
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/modules.rst
--rw-r--r--   0        0        0    17431 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/ophyd.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/reference.md
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/tests.md
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/vscode.md
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/introduction/introduction.md
--rw-r--r--   0        0        0    15339 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/user/command_line_interface.md
--rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/user/data_access_and_plotting.md
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/user/devices.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/user/graphical_user_interface.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/user/installation.md
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/user/user.md
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/pytest_bec_e2e/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/pytest_bec_e2e/pytest_bec_e2e/__init__.py
--rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/ophyd_patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/configs/__init__.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/configs/ophyd_devices_simulation.yaml
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/configs/ophyd_simulation.yaml
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/configs/sls_devices.yaml
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/SpmBase.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/XbpmBase.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/__init__.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/epics_motor_ex.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/mono_dccm.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/slits.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/slsDetector.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/sls_devices.py
--rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/specMotors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/__init__.py
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py
--rw-r--r--   0        0        0    18126 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py
--rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/psi_detector_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/protocols/__init__.py
--rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/protocols/bec_protocols.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/__init__.py
--rw-r--r--   0        0        0    27788 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/sim.py
--rw-r--r--   0        0        0    28125 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/sim_data.py
--rw-r--r--   0        0        0    12071 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/sim_frameworks.py
--rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/sim_signals.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/sim_test_devices.py
--rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/sim_xtreme.py
--rw-r--r--   0        0        0   671622 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt
--rw-r--r--   0        0        0   669534 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt
--rw-r--r--   0        0        0   670586 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt
--rw-r--r--   0        0        0   668300 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/__init__.py
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/bec_device_base.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/bec_scaninfo_mixin.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/bec_utils.py
--rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/controller.py
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/dynamic_pseudo.py
--rw-r--r--   0        0        0     7309 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/socket.py
--rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/static_device_test.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/tests/test_controller.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/tests/test_dynamic_pseudo.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/tests/test_ophyd_status_obj.py
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/tests/test_simulation.py
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/tests/test_socket.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/tests/test_static_device_test.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.gitignore
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/LICENSE
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7769 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/README.md
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.git_hooks/pre-commit
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.gitlab/issue_templates/bug_report_template.md
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.gitlab/issue_templates/documentation_update_template.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.gitlab/issue_templates/feature_request_template.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.gitlab/merge_request_templates/default.md
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.gitignore
+-rw-r--r--   0        0        0    19819 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.gitlab-ci.yml
+-rw-r--r--   0        0        0    18519 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.pylintrc
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.readthedocs.yaml
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/CHANGELOG.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/LICENSE
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/README.md
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_config_template.yaml
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.git_hooks/post-commit
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.git_hooks/pre-commit
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.gitlab/issue_templates/bug_report_template.md
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.gitlab/issue_templates/documentation_update_template.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.gitlab/issue_templates/feature_request_template.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/.gitlab/merge_request_templates/default.md
+-rw-r--r--   0        0        0     6867 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/demo.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/pyproject.toml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/__init__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/bec_magics.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/bec_startup.py
+-rw-r--r--   0        0        0     8631 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/main.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/prettytable.py
+-rw-r--r--   0        0        0    11090 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/progressbar.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/signals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/__init__.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py
+-rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py
+-rw-r--r--   0        0        0    12166 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/__init__.py
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/conftest.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_bec_client.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_device_progress.py
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_live_table.py
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_move_callback.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_pretty_table.py
+-rw-r--r--   0        0        0    25202 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py
+-rw-r--r--   0        0        0    11064 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/README.md
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/pyproject.toml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/__init__.py
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/alarm_handler.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/async_data.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bec_errors.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bec_service.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bec_yaml_loader.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bl_checks.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bl_conditions.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/callback_handler.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/channel_monitor.py
+-rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/client.py
+-rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/config_helper.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/connector.py
+-rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/dap_plugin_objects.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/dap_plugins.py
+-rw-r--r--   0        0        0    31017 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/device.py
+-rw-r--r--   0        0        0    23466 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/devicemanager.py
+-rw-r--r--   0        0        0    38756 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/endpoints.py
+-rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/file_utils.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/lmfit_serializer.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/logbook_connector.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/logger.py
+-rw-r--r--   0        0        0    24060 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/messages.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/numpy_encoder.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/observer.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/pdf_writer.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/plugin_helper.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/queue_items.py
+-rw-r--r--   0        0        0    41753 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/redis_connector.py
+-rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/request_items.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_data.py
+-rw-r--r--   0        0        0    11042 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_items.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_manager.py
+-rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_report.py
+-rw-r--r--   0        0        0    16698 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scans.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scibec_validator.py
+-rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/serialization.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/service_config.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/signature_serializer.py
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/user_scripts_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/configs/__init__.py
+-rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/configs/demo_config.yaml
+-rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/configs/openapi_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/__init__.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/fixtures.py
+-rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/test_config.yaml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/test_service_config.yaml
+-rw-r--r--   0        0        0    22495 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/__init__.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/import_utils.py
+-rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/proxy.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/rpc_utils.py
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/scan_utils.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/threading_utils.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/conftest.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_async_data.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_beamline_checks.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_bec_logger.py
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_bec_messages.py
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_bec_service.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_bl_conditions.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_callback_handler.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_channel_monitor.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_config_helper.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_core_utils.py
+-rw-r--r--   0        0        0    26550 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_dap_plugins.py
+-rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_device_manager.py
+-rw-r--r--   0        0        0    25863 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_devices.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_file_utils.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_import_utils.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_lmfit_serializer.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_observer.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_pdf_writer.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_plugin_helper.py
+-rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_redis_connector.py
+-rw-r--r--   0        0        0    22325 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_redis_connector_fakeredis.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_context.py
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_data.py
+-rw-r--r--   0        0        0    16743 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_items.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_manager.py
+-rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_object.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_report.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_scibec_validator.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_serializer.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_signature_serializer.py
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_user_scripts_mixin.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/tests/test_yaml_loader.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/create_plugin_structure.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/init_config.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/gitignore
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/setup_device_server.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/post-commit
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/pre-commit
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/README.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/pyproject.toml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/launch.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/service_handler.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/dap_server.py
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/dap_service.py
+-rw-r--r--   0        0        0     9729 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/dap_service_manager.py
+-rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/lmfit1d_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/cli/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/cli/launch.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/__init__.py
+-rw-r--r--   0        0        0    19037 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/device_server.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/rpc_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/cli/__init__.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/cli/launch.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/__init__.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/config_update_handler.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/device_serializer.py
+-rw-r--r--   0        0        0    22629 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/devicemanager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/tests/__init__.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/tests/utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/__init__.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/default_writer.py
+-rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/file_writer.py
+-rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/file_writer_manager.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/merged_dicts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/cli/__init__.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/cli/launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer_plugins/__init__.py
+-rw-r--r--   0        0        0    22204 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/__init__.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/bec_emitter.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/emitter.py
+-rw-r--r--   0        0        0    16121 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/scan_bundler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/cli/__init__.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/cli/launch.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/__init__.py
+-rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/device_validation.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/errors.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/path_optimization.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_assembler.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_guard.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_manager.py
+-rw-r--r--   0        0        0    35246 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_queue.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_server.py
+-rw-r--r--   0        0        0    18915 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_stubs.py
+-rw-r--r--   0        0        0    35721 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_worker.py
+-rw-r--r--   0        0        0    51830 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/cli/__init__.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/cli/launch.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_plugins/__init__.py
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/tests/__init__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/tests/fixtures.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/tests/utils.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/repeated_timer.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scihub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/cli/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/cli/launch.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/__init__.py
+-rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/config_handler.py
+-rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py
+-rw-r--r--   0        0        0    10735 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scilog/__init__.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scilog/scilog.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_bec_server_utils/test_main.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/conftest.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_dap_server.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/conftest.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_config_handler.py
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_serializer.py
+-rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_server.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/conftest.py
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/test_file_writer.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py
+-rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/conftest.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_emitter.py
+-rw-r--r--   0        0        0    25417 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/conftest.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_path_optimization.py
+-rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_guard.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py
+-rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py
+-rw-r--r--   0        0        0    53947 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_worker.py
+-rw-r--r--   0        0        0    87794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scans.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/conftest.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_repeated_timer.py
+-rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py
+-rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scibec_connector.py
+-rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scilog_connector.py
+-rwxr-xr-x   0        0        0     3629 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/bin/install_bec_dev.sh
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/Dockerfile.run_pytest
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/Dockerfile.run_server
+-rwxr-xr-x   0        0        0      347 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/build_python_services.sh
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/docker-compose.yaml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/functionalAccounts.json
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/semantic_release.toml
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/ci/test_config.yaml
+-rw-r--r--   0        0        0   307212 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/architecture/BEC.drawio
+-rw-r--r--   0        0        0   124683 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/architecture/BEC_config_db.drawio
+-rw-r--r--   0        0        0    11580 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/architecture/BEC_config_db.svg
+-rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/architecture/bec_architecture.png
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/Makefile
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/conf.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/make.bat
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/requirements.txt
+-rw-r--r--   0        0        0    41260 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/_static/bec.png
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/_static/switcher.json
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/_static/css/custom.css
+-rw-r--r--   0        0        0  4672990 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/_static/gif/bec_plotter.gif
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0        0        0   310535 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/BEC_context_user_centric.png
+-rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/bec_architecture.png
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/bec_device_structure.drawio
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/bec_device_structure.png
+-rw-r--r--   0        0        0    17460 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/gauss_scatter_plot.png
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/simulation_context_diagram.drawio
+-rw-r--r--   0        0        0    69323 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/simulation_context_diagram.png
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/tab-complete-devices.png
+-rw-r--r--   0        0        0    37244 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/vscode_debug_button.png
+-rw-r--r--   0        0        0   374770 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/vscode_with_annotations.drawio
+-rw-r--r--   0        0        0   711275 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/vscode_with_annotations.png
+-rw-r--r--   0        0        0    96330 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/assets/wm-devices.png
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/architecture.md
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/bec_cli.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/bec_config.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/bec_gui.md
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/bec_plugins.md
+-rw-r--r--   0        0        0     9531 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/bec_sim.md
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/contributing.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/data_access.md
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/developer.md
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/event_data.md
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/external_sources.md
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/glossary.md
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/install_developer_env.md
+-rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/logs.md
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/modules.rst
+-rw-r--r--   0        0        0    17464 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/ophyd.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/reference.md
+-rw-r--r--   0        0        0    16016 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/scans.md
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/tests.md
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/developer/vscode.md
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/introduction/introduction.md
+-rw-r--r--   0        0        0    15455 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/user/command_line_interface.md
+-rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/user/data_access_and_plotting.md
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/user/devices.md
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/user/graphical_user_interface.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/user/installation.md
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/docs/source/user/user.md
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/pytest_bec_e2e/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/pytest_bec_e2e/pytest_bec_e2e/__init__.py
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/__init__.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/ophyd_patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/configs/__init__.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/configs/ophyd_devices_simulation.yaml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/configs/ophyd_simulation.yaml
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/configs/sls_devices.yaml
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/SpmBase.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/XbpmBase.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/__init__.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/device_list.md
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/epics_motor_ex.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/mono_dccm.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/slits.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/sls_detector.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/sls_devices.py
+-rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/devices/specMotors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/__init__.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py
+-rw-r--r--   0        0        0    18126 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py
+-rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/psi_detector_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/interfaces/protocols/bec_protocols.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/__init__.py
+-rw-r--r--   0        0        0    27788 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/sim.py
+-rw-r--r--   0        0        0    28125 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/sim_data.py
+-rw-r--r--   0        0        0    12071 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/sim_frameworks.py
+-rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/sim_signals.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/sim_test_devices.py
+-rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/sim_xtreme.py
+-rw-r--r--   0        0        0   671622 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt
+-rw-r--r--   0        0        0   669534 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt
+-rw-r--r--   0        0        0   670586 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt
+-rw-r--r--   0        0        0   668300 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/__init__.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/bec_device_base.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/bec_scaninfo_mixin.py
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/bec_utils.py
+-rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/controller.py
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/dynamic_pseudo.py
+-rw-r--r--   0        0        0     7309 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/socket.py
+-rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/ophyd_devices/utils/static_device_test.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/tests/test_controller.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/tests/test_dynamic_pseudo.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/tests/test_ophyd_status_obj.py
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/tests/test_simulation.py
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/tests/test_socket.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/tests/test_static_device_test.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ophyd_devices-1.0.2/PKG-INFO
```

### Comparing `ophyd_devices-1.0.1/.gitlab-ci.yml` & `ophyd_devices-1.0.2/.gitlab-ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,19 @@
   - project: "bec/awi_utils"
     file: "/templates/check-packages-job.yml"
     inputs:
       stage: test
       path: "."
       pytest_args: "-v --random-order tests/"
       exclude_packages: ""
+  - project: "bec/awi_utils"
+    file: "templates/device-list-job.yml"
+    inputs:
+      target: $CI_PROJECT_NAME
+      token: $CI_UPDATES
 
 #commands to run in the Docker container before starting each job.
 before_script:
   - if [[ "$CI_PROJECT_PATH" != "bec/ophyd_devices" ]]; then
     echo -e "\033[35;1m Using branch $CHILD_PIPELINE_BRANCH of Ophyd Devices \033[0;m"; 
     test -d ophyd_devices || git clone --branch $CHILD_PIPELINE_BRANCH https://gitlab.psi.ch/bec/ophyd_devices.git; cd ophyd_devices;
     fi
```

### Comparing `ophyd_devices-1.0.1/CHANGELOG.md` & `ophyd_devices-1.0.2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,34 @@
 # CHANGELOG
 
 
 
+## v1.0.2 (2024-05-23)
+
+### Ci
+
+* ci: fixed dependency for bec ([`6630740`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/663074055977ca0a046a81bd9ba5187acf95afed))
+
+* ci: added ci token to update job ([`180891b`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/180891becdc1aa16da0c3b83c407e82a288d36d1))
+
+* ci: added device-list-update job ([`3405e2a`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/3405e2acf59cea33b025d376291ccda96db9ea07))
+
+### Documentation
+
+* docs: Update device list ([`d4f2ead`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/d4f2ead61b9eb4defb43d7e966a1ed5206461abd))
+
+* docs: Update device list ([`2f575d3`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/2f575d3aa221e646166bfeb0470de1847358acca))
+
+* docs: Update device list ([`b5adc09`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/b5adc097674068a90783a2ce4a093150d21cb736))
+
+### Fix
+
+* fix: pep8 compliant naming #64 ([`d705958`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/d7059589c84bacb560f738f4e4ae4aaf811b25d9))
+
+
 ## v1.0.1 (2024-05-15)
 
 ### Ci
 
 * ci: fixed bec_widgets env var ([`e900a4c`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/e900a4cb47c5ecaae8eca30d106771034dc9296d))
 
 * ci: fixed bec core dependency ([`8158e14`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/8158e145fe2358a736a2fb9d2d3de7e6c8db021c))
@@ -131,30 +154,7 @@
 
 ### Feature
 
 * feat: added support for nestes device configs ([`288f394`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/288f39483e83575d0bf3ec7a8e0d872b41b5b183))
 
 
 ## v0.31.0 (2024-04-19)
-
-### Build
-
-* build: fixed dependencies to compatible releases ([`26c04b5`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/26c04b5d03683b0159d5af127f19cda664bfb292))
-
-### Ci
-
-* ci: cleanup; added static device test job ([`ed66eac`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/ed66eacc5310e878deb35be69f335f1b8eb10950))
-
-* ci: added pipeline as trigger source ([`e59def1`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/e59def138fb465abf7a33d13e47e78ac382feebf))
-
-* ci: changed master to main ([`701be52`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/701be5262ad402ff6e6a665db4bd1d5b30b3abac))
-
-* ci: pull images via gitlab dependency proxy ([`8d68e7d`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/8d68e7df70e54984e460f50cee5356a7ada4e761))
-
-* ci: remove AdditionalTests dependency on pytest job ([`4ee86ab`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/4ee86aba371698820ea16ff94ae6946cd0041fe4))
-
-### Feature
-
-* feat: added support for directories as input for the static device test ([`9748ca6`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/9748ca666c3c8668e8ced80e7d24eeaf7f19c28e))
-
-
-## v0.30.5 (2024-04-12)
```

### Comparing `ophyd_devices-1.0.1/README.md` & `ophyd_devices-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/.gitlab/issue_templates/documentation_update_template.md` & `ophyd_devices-1.0.2/.gitlab/issue_templates/documentation_update_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/.gitlab/issue_templates/feature_request_template.md` & `ophyd_devices-1.0.2/.gitlab/issue_templates/feature_request_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/.gitlab/merge_request_templates/default.md` & `ophyd_devices-1.0.2/.gitlab/merge_request_templates/default.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/.gitignore` & `ophyd_devices-1.0.2/bec/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/.gitlab-ci.yml` & `ophyd_devices-1.0.2/bec/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -143,14 +143,15 @@
       junit: report.xml
       coverage_report:
         coverage_format: cobertura
         path: coverage.xml
 
 tests-3.11:
   stage: AdditionalTests
+  needs: []
   image: $CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX/python:3.11
   allow_failure: true
   script:
     - git clone --branch $OPHYD_DEVICES_BRANCH https://oauth2:$CI_OPHYD_DEVICES_KEY@gitlab.psi.ch/bec/ophyd_devices.git
     - export OPHYD_DEVICES_PATH=$PWD/ophyd_devices
     - pip install pytest pytest-random-order pytest-cov pytest-timeout
     - apt-get update
@@ -185,15 +186,15 @@
     - if: '$CI_PIPELINE_SOURCE == "pipeline"'
     - if: '$CI_MERGE_REQUEST_TARGET_BRANCH_NAME == "main"'
     - if: '$CI_MERGE_REQUEST_TARGET_BRANCH_NAME == "production"'
   script:
     # build and run the tests
     - echo $OPHYD_DEVICES_BRANCH 
     - echo "$CI_DEPENDENCY_PROXY_PASSWORD" | docker login $CI_DEPENDENCY_PROXY_SERVER --username $CI_DEPENDENCY_PROXY_USER --password-stdin
-    - docker build -t end2end_client:test -f ./ci/Dockerfile.run_pytest --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=bec_ipython_client --build-arg OPHYD_BRANCH=$OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX .
+    - docker build -t end2end_client:test -f ./ci/Dockerfile.run_pytest --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=bec_ipython_client --build-arg OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX .
     - docker run --network=host --name end2end_client end2end_client:test
 
   after_script:
     # copy the log files to the project directory in order to be reachable by git artifacts
     - docker cp end2end_client:/code/bec/test_files/. $CI_PROJECT_DIR
 
 # end-2-end-scibec:
@@ -246,20 +247,20 @@
 #   script:
 #     # download buildah & podman
 #     - apk add buildah
 #     - apk add podman
 #     # build containers
 #     # /!\ build-arg is interpreted differently by podman,
 #     # have to use buildah here
-#     - buildah bud --network=host -t device_server_vm -f ./ci/Dockerfile.run_server --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=device_server --build-arg OPHYD_BRANCH=$OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
-#     - buildah bud --network=host -t scan_server_vm -f ./ci/Dockerfile.run_server --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=scan_server --build-arg OPHYD_BRANCH=$OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
-#     - buildah bud --network=host -t scan_bundler_vm -f ./ci/Dockerfile.run_server --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=scan_bundler --build-arg OPHYD_BRANCH=$OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
-#     - buildah bud --network=host -t file_writer_vm -f ./ci/Dockerfile.run_server --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=file_writer --build-arg OPHYD_BRANCH=$OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
-#     - buildah bud --network=host -t dap_server_vm -f ./ci/Dockerfile.run_server --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=data_processing --build-arg OPHYD_BRANCH=$OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
-#     - buildah bud --network=host -t scihub_vm -f ./ci/Dockerfile.run_server --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=scihub --build-arg OPHYD_BRANCH=$OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
+#     - buildah bud --network=host -t device_server_vm -f ./ci/Dockerfile.run_server --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=device_server --build-arg OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
+#     - buildah bud --network=host -t scan_server_vm -f ./ci/Dockerfile.run_server --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=scan_server --build-arg OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
+#     - buildah bud --network=host -t scan_bundler_vm -f ./ci/Dockerfile.run_server --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=scan_bundler --build-arg OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
+#     - buildah bud --network=host -t file_writer_vm -f ./ci/Dockerfile.run_server --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=file_writer --build-arg OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
+#     - buildah bud --network=host -t dap_server_vm -f ./ci/Dockerfile.run_server --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=data_processing --build-arg OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
+#     - buildah bud --network=host -t scihub_vm -f ./ci/Dockerfile.run_server --build-arg PY_VERSION=3.10 --build-arg BEC_SERVICE=scihub --build-arg OPHYD_DEVICES_BRANCH --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
 #     # default service is bec_ipython_client
 #     - buildah bud --network=host -t end2end_client_test -f ./ci/Dockerfile.run_server --build-arg PY_VERSION=3.10 --build-arg CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
 
 #     # now for the run phase...
 #     - REDIS_IP=$(cat /etc/hosts | awk '{if ($2 == "redis") print $1;}')
 #     # Just checking that the IP is reachable from outside the container
 #     - ping -w 2 $REDIS_IP
@@ -453,20 +454,34 @@
   rules:
     - if: '$CI_COMMIT_REF_NAME == "main"'
 
 dev-pages:
   stage: Deploy
   needs: ["formatter"]
   rules:
-    - if: $CI_COMMIT_REF_NAME == "development"
+    - if: '$CI_PIPELINE_SOURCE == "schedule"'
+    - if: '$CI_PIPELINE_SOURCE == "web"'
+    - if: '$CI_PIPELINE_SOURCE == "pipeline"'
+    - if: '$CI_MERGE_REQUEST_TARGET_BRANCH_NAME == "main"'
+    - if: '$CI_MERGE_REQUEST_TARGET_BRANCH_NAME == "production"'
   script:
     - git config --global user.name "ci_update_bot"
     - git config --global user.email "ci_update_bot@bec.ch"
-    - git tag -f development "$CI_COMMIT_SHA"
-    - git push --force origin development
+    # - git tag -l | xargs git tag -d
+    # - git fetch --tags
+    # - git tag -d development || true
+    # - git push https://oauth2:$CI_DEV_DEPLOY@gitlab.psi.ch/bec/bec.git :refs/tags/development || true
+    # - git tag development $CI_COMMIT_SHA
+    # - git push https://oauth2:$CI_DEV_DEPLOY@gitlab.psi.ch/bec/bec.git development
+    
+    - git fetch --all
+    - git branch -a | grep MR_DEV_BRANCH
+    - git checkout remotes/origin/MR_DEV_BRANCH
+    - git reset --hard origin/$CI_COMMIT_REF_NAME
+    - git push --force -o ci.skip https://oauth2:$CI_DEV_DEPLOY@gitlab.psi.ch/bec/bec.git HEAD:refs/heads/MR_DEV_BRANCH;
 
     - curl -X POST -d "branches=development" -d "token=$RTD_TOKEN" https://readthedocs.org/api/v2/webhook/beamline-experiment-control/221870/
     - curl -X POST -d "branches=development" -d "token=$RTD_TOKEN_BEC" https://readthedocs.org/api/v2/webhook/bec/246899/
 
 pages:
   stage: Deploy
   needs: ["semver"]
```

### Comparing `ophyd_devices-1.0.1/bec/.pylintrc` & `ophyd_devices-1.0.2/bec/.pylintrc`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/.readthedocs.yaml` & `ophyd_devices-1.0.2/bec/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/CHANGELOG.md` & `ophyd_devices-1.0.2/bec/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,76 @@
 # CHANGELOG
 
 
 
+## v2.12.3 (2024-05-21)
+
+### Fix
+
+* fix: renamed table_wait to scan_progress ([`855f9a8`](https://gitlab.psi.ch/bec/bec/-/commit/855f9a8412e9c0d8b02d131ece533b4d85882b36))
+
+* fix: renamed scan_progress to device_progress ([`d344e85`](https://gitlab.psi.ch/bec/bec/-/commit/d344e8513781f29a1390adc92826f23d1702964b))
+
+
+## v2.12.2 (2024-05-17)
+
+### Fix
+
+* fix(scihub): added experimentId to scan entries in BEC db ([`8ba7213`](https://gitlab.psi.ch/bec/bec/-/commit/8ba7213e29ac0335bca126b9d8a08a9ec46e469f))
+
+
+## v2.12.1 (2024-05-17)
+
+### Fix
+
+* fix: race condition when reading new value from stream ([`87cc71a`](https://gitlab.psi.ch/bec/bec/-/commit/87cc71aa91c9d35b6483f4ef6c5de3c59575e9dc))
+
+* fix: import &#39;dap_plugin_objects&#39; at last minute to speed up initial import ([`d7db6be`](https://gitlab.psi.ch/bec/bec/-/commit/d7db6befe9b8e4689ed37ccad44f8a5d06694180))
+
+* fix: messages import made lazy to speed up initial import time
+
+TODO: put back imports as normal when Pydantic gets faster ([`791be9b`](https://gitlab.psi.ch/bec/bec/-/commit/791be9b25aa618d508feed99a201e0c58b56f3ce))
+
+* fix: do not import modules if only for type checking (faster import) ([`1c628fd`](https://gitlab.psi.ch/bec/bec/-/commit/1c628fd6105ef5df99e97c8945d3382c45ef5350))
+
+* fix: clean all imports from bec_lib, remove use of @threadlocked ([`8a017ef`](https://gitlab.psi.ch/bec/bec/-/commit/8a017ef3d7666f173a70f2e6a8606d73b1af0095))
+
+* fix: use lazy import to reduce bec_lib import time ([`649502e`](https://gitlab.psi.ch/bec/bec/-/commit/649502e364e4e4c0ea53f932418c479f2d6978d4))
+
+* fix: solve scope problem with &#39;name&#39; variable in lambda ([`417e73e`](https://gitlab.psi.ch/bec/bec/-/commit/417e73e5d65f0c774c92889a44d1262c7f4f343b))
+
+
+## v2.12.0 (2024-05-16)
+
+### Feature
+
+* feat(scan_bundler): added scan progress ([`27befe9`](https://gitlab.psi.ch/bec/bec/-/commit/27befe966607a3ae319dbee3af9e59ef0d044bc8))
+
+
+## v2.11.1 (2024-05-16)
+
+### Ci
+
+* ci: cleanup ARGs in dockerfiles ([`b670d1a`](https://gitlab.psi.ch/bec/bec/-/commit/b670d1aa6b6e2af0cb09e7dbc77ea5d1bc66593b))
+
+* ci: run AdditionalTests jobs on pipeline start
+
+This is a followup to !573 ([`c9ece7e`](https://gitlab.psi.ch/bec/bec/-/commit/c9ece7ef2f1f9b052ed9b92bcb29463cf8371c64))
+
+### Documentation
+
+* docs(bec_lib): improved scripts documentation ([`79f487e`](https://gitlab.psi.ch/bec/bec/-/commit/79f487ea8b9dc135102204872390631e59a60e54))
+
+### Fix
+
+* fix(bec_lib): fixed loading scripts from plugins
+
+User scripts from plugins were still relying on the old plugin structure ([`3264434`](https://gitlab.psi.ch/bec/bec/-/commit/3264434d40647d260400045f7bbd4c2ee9bb2c4e))
+
+
 ## v2.11.0 (2024-05-15)
 
 ### Feature
 
 * feat: add utility function to determine instance of an object by class name ([`0ccd13c`](https://gitlab.psi.ch/bec/bec/-/commit/0ccd13cd738dc12d4a587b4c5e0d6b447d7cfc50))
 
 * feat: add utilities to lazy import a module ([`a37ae57`](https://gitlab.psi.ch/bec/bec/-/commit/a37ae577f68c154dc3da544816b7c7f0cb532c50))
@@ -96,92 +161,12 @@
 ### Test
 
 * test: added more tests for scan queue ([`b664b92`](https://gitlab.psi.ch/bec/bec/-/commit/b664b92aae917d2067bfca48a60eeaf44ced0c98))
 
 
 ## v2.9.4 (2024-05-01)
 
-### Fix
-
-* fix: unified device message signature ([`c54dfc1`](https://gitlab.psi.ch/bec/bec/-/commit/c54dfc166fe9dd925b15e8cc8750cebaec8896cb))
-
 ### Refactor
 
 * refactor: added isort params to pyproject ([`0a1beae`](https://gitlab.psi.ch/bec/bec/-/commit/0a1beae06ae128d9817272644d2f38ca761756ab))
 
 * refactor(bec_lib): cleanup ([`6bf0998`](https://gitlab.psi.ch/bec/bec/-/commit/6bf0998c71387307ad8d842931488ec2aea566a8))
-
-
-## v2.9.3 (2024-05-01)
-
-### Fix
-
-* fix: fixed log message log type ([`af85937`](https://gitlab.psi.ch/bec/bec/-/commit/af8593794c2ea9d0b4851b367aca4e6546fc760f))
-
-* fix: fixed log message signature and added literal checks; closes #277 ([`ca7c238`](https://gitlab.psi.ch/bec/bec/-/commit/ca7c23851976111d81c811bf16b6d6f371d24dc6))
-
-* fix: logs should be send, not set_and_publish; closes #278 ([`3964870`](https://gitlab.psi.ch/bec/bec/-/commit/396487074905930c410978144e986d1b9b373a2c))
-
-* fix: device_req_status only needs set ([`587cfcc`](https://gitlab.psi.ch/bec/bec/-/commit/587cfccbe576dcd2eb10fc16e225ee3175f8d2a0))
-
-
-## v2.9.2 (2024-04-29)
-
-### Fix
-
-* fix(bec_startup): BECFigure starts up after client ([`6b48858`](https://gitlab.psi.ch/bec/bec/-/commit/6b488588fed818ee1fefae8d5620821381b2eee0))
-
-
-## v2.9.1 (2024-04-29)
-
-### Documentation
-
-* docs: updated docs for bec plugins ([`29b89dd`](https://gitlab.psi.ch/bec/bec/-/commit/29b89dd0173dfd9a692040d0acbf14bf47a6a46c))
-
-### Fix
-
-* fix: renamed dap_services to services ([`62549f5`](https://gitlab.psi.ch/bec/bec/-/commit/62549f57c9a497f0feceb63a8facd66669f56437))
-
-* fix: updated plugin helper script to new plugin structure ([`8e16efb`](https://gitlab.psi.ch/bec/bec/-/commit/8e16efb21a5f6f68eee61ff22a930bf9e7400110))
-
-
-## v2.9.0 (2024-04-29)
-
-### Documentation
-
-* docs: added section on logging ([`ebcd2a4`](https://gitlab.psi.ch/bec/bec/-/commit/ebcd2a4dbc2a52dc1e8679e54784daa0f6a3901b))
-
-### Feature
-
-* feat(bec_lib): added log monitor as CLI tool ([`0b624a4`](https://gitlab.psi.ch/bec/bec/-/commit/0b624a4ab5039c157edc1a3b589ba462f82879dd))
-
-* feat(bec_lib): added trace log with stack trace ([`650de81`](https://gitlab.psi.ch/bec/bec/-/commit/650de811090dc72407cfb746eb22aa883682d268))
-
-### Test
-
-* test(bec_lib): added test for log monitor ([`64d5c30`](https://gitlab.psi.ch/bec/bec/-/commit/64d5c304d98c04f5943dd6365de364974a6fc931))
-
-
-## v2.8.0 (2024-04-27)
-
-### Build
-
-* build: fixed fpdf version ([`94b6995`](https://gitlab.psi.ch/bec/bec/-/commit/94b6995fd32224557b2fc8b3aeafcf73acdb8a2c))
-
-### Feature
-
-* feat(bec_lib): added option to combine yaml files ([`39bb628`](https://gitlab.psi.ch/bec/bec/-/commit/39bb6281bda2960de7e70c45463f62dde2b454f5))
-
-
-## v2.7.3 (2024-04-26)
-
-### Documentation
-
-* docs: fixed bec config template ([`87d0986`](https://gitlab.psi.ch/bec/bec/-/commit/87d0986f21ba367dbb23db50c7c13f10b4007030))
-
-### Fix
-
-* fix: fixed loading of plugin-based configs ([`f927735`](https://gitlab.psi.ch/bec/bec/-/commit/f927735cd4012d4e4182596dc2ac2735d5ec4697))
-
-### Test
-
-* test(bec_lib): added test for unregistering callbacks ([`6e14de3`](https://gitlab.psi.ch/bec/bec/-/commit/6e14de35dc43b7eed3244f5fe327d79ddc1302ae))
```

### Comparing `ophyd_devices-1.0.1/bec/LICENSE` & `ophyd_devices-1.0.2/bec/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/README.md` & `ophyd_devices-1.0.2/bec/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/.gitlab/issue_templates/documentation_update_template.md` & `ophyd_devices-1.0.2/bec/.gitlab/issue_templates/documentation_update_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/.gitlab/issue_templates/feature_request_template.md` & `ophyd_devices-1.0.2/bec/.gitlab/issue_templates/feature_request_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/.gitlab/merge_request_templates/default.md` & `ophyd_devices-1.0.2/bec/.gitlab/merge_request_templates/default.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/demo.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from bec_ipython_client import BECIPythonClient
-from bec_lib import bec_logger
+from bec_lib.logger import bec_logger
 
 logger = bec_logger.logger
 bec_logger.level = bec_logger.LOGLEVEL.SUCCESS
 
 # CONFIG_PATH = "../bec_config.yaml"
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/pyproject.toml` & `ophyd_devices-1.0.2/bec/bec_ipython_client/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec_ipython_client"
-version = "2.11.0"
+version = "2.12.3"
 description = "BEC IPython client"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/bec_magics.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/bec_startup.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/bec_startup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import sys
 
 import numpy as np  # not needed but always nice to have
 
 from bec_ipython_client.main import BECIPythonClient as _BECIPythonClient
 from bec_ipython_client.main import main_dict as _main_dict
-from bec_lib import RedisConnector as _RedisConnector
-from bec_lib import bec_logger as _bec_logger
 from bec_lib import plugin_helper
+from bec_lib.logger import bec_logger as _bec_logger
+from bec_lib.redis_connector import RedisConnector as _RedisConnector
 
 try:
     from bec_widgets.cli.client import BECDockArea as _BECDockArea
 except ImportError:
     _BECDockArea = None
 
 logger = _bec_logger.logger
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/main.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 from IPython.terminal.ipapp import TerminalIPythonApp
 from IPython.terminal.prompts import Prompts, Token
 
 from bec_ipython_client.beamline_mixin import BeamlineMixin
 from bec_ipython_client.bec_magics import BECMagics
 from bec_ipython_client.callbacks.ipython_live_updates import IPythonLiveUpdates
 from bec_ipython_client.signals import ScanInterruption, SigintHandler
-from bec_lib import ServiceConfig, bec_logger, plugin_helper
+from bec_lib import plugin_helper
 from bec_lib.alarm_handler import AlarmBase
 from bec_lib.callback_handler import EventType
 from bec_lib.client import BECClient
 from bec_lib.connector import ConnectorBase
+from bec_lib.logger import bec_logger
+from bec_lib.service_config import ServiceConfig
 
 logger = bec_logger.logger
 
 
 class BECIPythonClient:
     def __init__(
         self,
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/prettytable.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/progressbar.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/progressbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 from typing import Any
 
 import numpy as np
 import rich.progress
 from rich.text import Text
 
-from bec_lib import bec_logger
+from bec_lib.logger import bec_logger
 
 logger = bec_logger.logger
 
 
 class MoveTaskProgressColumn(rich.progress.TaskProgressColumn):
     """Custom progress column for the move device progress bar"""
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/signals.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/signals.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import collections
 import time
 from typing import TYPE_CHECKING
 
-from bec_ipython_client.callbacks.scan_progress import LiveUpdatesScanProgress
-from bec_lib import bec_logger
+from bec_ipython_client.callbacks.device_progress import LiveUpdatesDeviceProgress
 from bec_lib.bec_errors import ScanInterruption
+from bec_lib.logger import bec_logger
 
 from .live_table import LiveUpdatesTable
 from .move_device import LiveUpdatesReadbackProgressbar
 from .utils import ScanRequestMixin, check_alarms
 
 if TYPE_CHECKING:
     from bec_lib import messages
@@ -42,15 +42,15 @@
         """Process instructions for the live updates.
 
         Args:
             report_instructions (list): The list of report instructions.
         """
         scan_type = self._active_request.content["scan_type"]
         if scan_type in ["open_scan_def", "close_scan_def"]:
-            self._process_instruction({"table_wait": 0})
+            self._process_instruction({"scan_progress": 0})
             return
         if scan_type == "close_scan_group":
             return
 
         if not report_instructions:
             return
 
@@ -74,24 +74,24 @@
             if scan_report_type == "readback":
                 LiveUpdatesReadbackProgressbar(
                     self.client,
                     report_instruction=instr,
                     request=self._active_request,
                     callbacks=self._user_callback,
                 ).run()
-            elif scan_report_type == "table_wait":
+            elif scan_report_type == "scan_progress":
                 LiveUpdatesTable(
                     self.client,
                     report_instruction=instr,
                     request=self._active_request,
                     callbacks=self._user_callback,
                     print_table_data=self.print_table_data,
                 ).run()
-            elif scan_report_type == "scan_progress":
-                LiveUpdatesScanProgress(
+            elif scan_report_type == "device_progress":
+                LiveUpdatesDeviceProgress(
                     self.client,
                     report_instruction=instr,
                     request=self._active_request,
                     callbacks=self._user_callback,
                 ).run()
             else:
                 raise ValueError(f"Unknown scan report type: {scan_report_type}")
@@ -132,17 +132,15 @@
         available_blocks = [
             req_block
             for req_block in queue.request_blocks
             if req_block["RID"] == request.metadata["RID"]
         ]
         return available_blocks
 
-    def process_request(
-        self, request: messages.ScanQueueMessage, scan_report_type: str, callbacks: any
-    ) -> None:
+    def process_request(self, request: messages.ScanQueueMessage, callbacks: any) -> None:
         """Process the request and report instructions."""
         # pylint: disable=protected-access
         try:
             with self.client._sighandler:
                 # pylint: disable=protected-access
                 self._active_request = request
                 self._user_callback = callbacks
@@ -164,15 +162,15 @@
                 req_block = available_blocks[self._request_block_index[req_id]]
                 report_instructions = req_block.get("report_instructions", [])
                 self._process_report_instructions(report_instructions)
 
             self._reset()
 
         except ScanInterruption as scan_interr:
-            self._interrupted_request = (request, scan_report_type)
+            self._interrupted_request = (request,)
             if self._current_queue and self.client._service_config.abort_on_ctrl_c:
                 self._wait_for_cleanup()
             self._reset(forced=True)
             raise scan_interr
 
     def _wait_for_cleanup(self):
         """Wait for the scan to be cleaned up."""
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 import time
 from collections.abc import Callable
 from typing import TYPE_CHECKING
 
 from bec_ipython_client.prettytable import PrettyTable
 from bec_ipython_client.progressbar import ScanProgressBar
-from bec_lib import bec_logger, messages
+from bec_lib.logger import bec_logger
 
 from .utils import LiveUpdatesBase, check_alarms
 
 if TYPE_CHECKING:
+    from bec_lib import messages
     from bec_lib.client import BECClient
 
 logger = bec_logger.logger
 
 
 def sort_devices(devices, scan_devices) -> list:
     """sort the devices to ensure that the table starts with scan motors"""
@@ -34,15 +35,15 @@
     Raises:
         TimeoutError: Raised if no queue item is added before reaching a predefined timeout.
         RuntimeError: Raised if more points than requested are returned.
         ScanRequestError: Raised if the scan was rejected by the server.
     """
 
     MAX_DEVICES = 10
-    REPORT_TYPE = "table_wait"
+    REPORT_TYPE = "scan_progress"
 
     def __init__(
         self,
         bec: BECClient,
         report_instruction: dict = None,
         request: messages.ScanQueueMessage = None,
         callbacks: list[Callable] = None,
@@ -55,15 +56,17 @@
         self.scan_item = None
         self.dev_values = None
         self.point_data = None
         self.point_id = 0
         self.table = None
         self.__print_table_data = None
         self._print_table_data = (
-            print_table_data if print_table_data is not None else self.REPORT_TYPE == "table_wait"
+            print_table_data
+            if print_table_data is not None
+            else self.REPORT_TYPE == "scan_progress"
         )
 
     def wait_for_scan_to_start(self):
         """wait until the scan starts"""
         while True:
             queue_pos = self.scan_item.queue.queue_position
             self.check_alarms()
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 from collections.abc import Callable
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from bec_ipython_client.progressbar import DeviceProgressBar
-from bec_lib import DeviceManagerBase, MessageEndpoints, messages
+from bec_lib.endpoints import MessageEndpoints
 
 from .utils import LiveUpdatesBase, check_alarms
 
 if TYPE_CHECKING:
+    from bec_lib import messages
     from bec_lib.client import BECClient
+    from bec_lib.devicemanager import DeviceManagerBase
 
 
 class ReadbackDataMixin:
     def __init__(self, device_manager: DeviceManagerBase, devices: list) -> None:
         """Mixin to get the current device values and request-done messages.
 
         Args:
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/scan_progress.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import time
 
 from bec_ipython_client.progressbar import ScanProgressBar
-from bec_lib import MessageEndpoints, bec_logger
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 
 from .live_table import LiveUpdatesTable
 
 logger = bec_logger.logger
 
 
-class LiveUpdatesScanProgress(LiveUpdatesTable):
+class LiveUpdatesDeviceProgress(LiveUpdatesTable):
     """Live updates for scans using a progress bar based on the progress of one or more devices"""
 
-    REPORT_TYPE = "scan_progress"
+    REPORT_TYPE = "device_progress"
 
     def _run_update(self, device_names: str):
         """Run the update loop for the progress bar.
 
         Args:
             device_names (str): The name of the device to monitor.
         """
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import abc
 import threading
 import time
 import traceback
 from collections.abc import Callable
 from typing import TYPE_CHECKING
 
-from bec_lib import bec_logger, messages
+from bec_lib.logger import bec_logger
 from bec_lib.request_items import RequestItem
 
 if TYPE_CHECKING:
+    from bec_lib import messages
     from bec_lib.client import BECClient
 
 logger = bec_logger.logger
 
 
 class ScanRequestError(Exception):
     """Error raised when a scan request is rejected"""
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml` & `ophyd_devices-1.0.2/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_bec_client.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_bec_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import sys
 from unittest import mock
 
 import IPython
 import pytest
 
 from bec_ipython_client import BECIPythonClient, main
-from bec_lib import RedisConnector, ServiceConfig
+from bec_lib.redis_connector import RedisConnector
+from bec_lib.service_config import ServiceConfig
 
 
 def test_bec_entry_point_globals_and_post_startup(tmpdir):  # , capfd):
     file_to_execute = tmpdir / "post_startup.py"
     with open(file_to_execute, "w") as f:
         f.write(
             """
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,11 +149,11 @@
 #     )
 #     live_updates._active_request = request_msg
 #     live_updates._user_callback = []
 #     client.queue.queue_storage.current_scan_queue = {"primary": {"status": "RUNNING"}}
 #     with mock.patch(
 #         "bec_client_mock.callbacks.ipython_live_updates.LiveUpdatesTable", new_callable=mock.Co
 #     ) as table:
-#         live_updates._process_instruction({"table_wait": 10})
+#         live_updates._process_instruction({"scan_progress": 10})
 #         table.assert_called_once_with(
-#             client, report_instructions={"table_wait": 10}, request=request_msg, callbacks=[]
+#             client, report_instructions={"scan_progress": 10}, request=request_msg, callbacks=[]
 #         )
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_live_table.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_live_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,28 +75,28 @@
 )
 def test_get_devices_from_scan_data(bec_client_mock, request_msg, scan_report_devices):
     client = bec_client_mock
     client.start()
     data = messages.ScanMessage(
         point_id=0, scan_id="", data={}, metadata={"scan_report_devices": scan_report_devices}
     )
-    live_update = LiveUpdatesTable(client, {"table_wait": 10}, request_msg)
+    live_update = LiveUpdatesTable(client, {"scan_progress": 10}, request_msg)
     devices = live_update.get_devices_from_scan_data(data)
     assert devices[0 : len(scan_report_devices)] == scan_report_devices
 
 
 @pytest.mark.timeout(20)
 def test_wait_for_request_acceptance(client_with_grid_scan):
     client, request_msg = client_with_grid_scan
     response_msg = messages.RequestResponseMessage(
         accepted=True, message={"msg": ""}, metadata={"RID": "something"}
     )
     client.queue.request_storage.update_with_request(request_msg)
     client.queue.request_storage.update_with_response(response_msg)
-    live_update = LiveUpdatesTable(client, {"table_wait": 10}, request_msg)
+    live_update = LiveUpdatesTable(client, {"scan_progress": 10}, request_msg)
     with mock.patch.object(client.queue.queue_storage, "find_queue_item_by_requestID"):
         live_update.wait_for_request_acceptance()
 
 
 class ScanItemMock:
     def __init__(self, data):
         self.data = data
@@ -106,15 +106,15 @@
 def test_print_table_data(client_with_grid_scan):
     client, request_msg = client_with_grid_scan
     response_msg = messages.RequestResponseMessage(
         accepted=True, message={"msg": ""}, metadata={"RID": "something"}
     )
     client.queue.request_storage.update_with_request(request_msg)
     client.queue.request_storage.update_with_response(response_msg)
-    live_update = LiveUpdatesTable(client, {"table_wait": 10}, request_msg)
+    live_update = LiveUpdatesTable(client, {"scan_progress": 10}, request_msg)
     live_update.point_data = messages.ScanMessage(
         point_id=0,
         scan_id="",
         data={"samx": {"samx": {"value": 0}}},
         metadata={"scan_report_devices": ["samx"], "scan_type": "step"},
     )
     live_update.scan_item = ScanItemMock(data=[live_update.point_data])
@@ -126,15 +126,15 @@
 def test_print_table_data_lamni_flyer(client_with_grid_scan):
     client, request_msg = client_with_grid_scan
     response_msg = messages.RequestResponseMessage(
         accepted=True, message={"msg": ""}, metadata={"RID": "something"}
     )
     client.queue.request_storage.update_with_request(request_msg)
     client.queue.request_storage.update_with_response(response_msg)
-    live_update = LiveUpdatesTable(client, {"table_wait": 10}, request_msg)
+    live_update = LiveUpdatesTable(client, {"scan_progress": 10}, request_msg)
     live_update.point_data = messages.ScanMessage(
         point_id=0,
         scan_id="",
         data={"lamni_flyer_1": {"value": 0}},
         metadata={"scan_report_devices": ["samx"], "scan_type": "fly"},
     )
     live_update.scan_item = ScanItemMock(data=[live_update.point_data])
@@ -146,15 +146,15 @@
 def test_print_table_data_hinted_value(client_with_grid_scan):
     client, request_msg = client_with_grid_scan
     response_msg = messages.RequestResponseMessage(
         accepted=True, message={"msg": ""}, metadata={"RID": "something"}
     )
     client.queue.request_storage.update_with_request(request_msg)
     client.queue.request_storage.update_with_response(response_msg)
-    live_update = LiveUpdatesTable(client, {"table_wait": 10}, request_msg)
+    live_update = LiveUpdatesTable(client, {"scan_progress": 10}, request_msg)
     client.device_manager.devices["samx"]._info["hints"] = {"fields": ["samx_hint"]}
     client.device_manager.devices["samx"].precision = 3
     live_update.point_data = messages.ScanMessage(
         point_id=0,
         scan_id="",
         data={"samx": {"samx_hint": {"value": 0}}},
         metadata={"scan_report_devices": ["samx"], "scan_type": "fly"},
@@ -174,15 +174,15 @@
 def test_print_table_data_hinted_value_with_precision(client_with_grid_scan):
     client, request_msg = client_with_grid_scan
     response_msg = messages.RequestResponseMessage(
         accepted=True, message={"msg": ""}, metadata={"RID": "something"}
     )
     client.queue.request_storage.update_with_request(request_msg)
     client.queue.request_storage.update_with_response(response_msg)
-    live_update = LiveUpdatesTable(client, {"table_wait": 10}, request_msg)
+    live_update = LiveUpdatesTable(client, {"scan_progress": 10}, request_msg)
     client.device_manager.devices["samx"]._info["hints"] = {"fields": ["samx_hint"]}
     client.device_manager.devices["samx"].precision = 2
     live_update.point_data = messages.ScanMessage(
         point_id=0,
         scan_id="",
         data={"samx": {"samx_hint": {"value": 0}}},
         metadata={"scan_report_devices": ["samx"], "scan_type": "fly"},
@@ -219,15 +219,15 @@
 def test_print_table_data_variants(client_with_grid_scan, value, expected):
     client, request_msg = client_with_grid_scan
     response_msg = messages.RequestResponseMessage(
         accepted=True, message={"msg": ""}, metadata={"RID": "something"}
     )
     client.queue.request_storage.update_with_request(request_msg)
     client.queue.request_storage.update_with_response(response_msg)
-    live_update = LiveUpdatesTable(client, {"table_wait": 10}, request_msg)
+    live_update = LiveUpdatesTable(client, {"scan_progress": 10}, request_msg)
     live_update.point_data = messages.ScanMessage(
         point_id=0,
         scan_id="",
         data={"lamni_flyer_1": {"value": value}},
         metadata={"scan_report_devices": ["samx"], "scan_type": "fly"},
     )
     live_update.scan_item = ScanItemMock(data=[live_update.point_data])
@@ -250,15 +250,15 @@
     client_msg = messages.ClientInfoMessage(
         message="message", RID="something", show_asap=True, source="scan_server"
     )
     client.queue.request_storage.update_with_client_message(client_msg)
     with mock.patch.object(
         client.queue.request_storage.scan_manager.queue_storage, "find_queue_item_by_requestID"
     ):
-        live_update = LiveUpdatesTable(client, {"table_wait": 10}, request_msg)
+        live_update = LiveUpdatesTable(client, {"scan_progress": 10}, request_msg)
         live_update.wait_for_request_acceptance()
         result = StringIO()
         with redirect_stdout(result):
             live_update._print_client_msgs_asap()
             rtr1 = "Client info (scan_server) : message" + "\n"
             assert result.getvalue() == rtr1
             # second time should not add anything
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_move_callback.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_move_callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import pytest
 
 from bec_ipython_client.callbacks.move_device import (
     LiveUpdatesReadbackProgressbar,
     ReadbackDataMixin,
 )
-from bec_lib import MessageEndpoints, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
 
 
 @pytest.fixture
 def readback_data_mixin(bec_client_mock):
     with mock.patch.object(bec_client_mock.device_manager, "connector"):
         yield ReadbackDataMixin(bec_client_mock.device_manager, ["samx", "samy"])
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_scan_progress.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/client_tests/test_device_progress.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from unittest import mock
 
-from bec_ipython_client.callbacks.scan_progress import LiveUpdatesScanProgress
+from bec_ipython_client.callbacks.device_progress import LiveUpdatesDeviceProgress
 from bec_lib import messages
 
 
 def test_update_progressbar_continues_without_device_data():
     bec = mock.MagicMock()
     request = mock.MagicMock()
-    live_update = LiveUpdatesScanProgress(bec=bec, report_instruction={}, request=request)
+    live_update = LiveUpdatesDeviceProgress(bec=bec, report_instruction={}, request=request)
     progressbar = mock.MagicMock()
 
     bec.connector.get.return_value = None
     res = live_update._update_progressbar(progressbar, "async_dev1")
     assert res is False
 
 
 def test_update_progressbar_continues_when_scan_id_doesnt_match():
     bec = mock.MagicMock()
     request = mock.MagicMock()
-    live_update = LiveUpdatesScanProgress(bec=bec, report_instruction={}, request=request)
+    live_update = LiveUpdatesDeviceProgress(bec=bec, report_instruction={}, request=request)
     progressbar = mock.MagicMock()
     live_update.scan_item = mock.MagicMock()
     live_update.scan_item.scan_id = "scan_id2"
 
     bec.connector.get.return_value = messages.ProgressMessage(
         value=1, max_value=10, done=False, metadata={"scan_id": "scan_id"}
     )
     res = live_update._update_progressbar(progressbar, "async_dev1")
     assert res is False
 
 
 def test_update_progressbar_updates_max_value():
     bec = mock.MagicMock()
     request = mock.MagicMock()
-    live_update = LiveUpdatesScanProgress(bec=bec, report_instruction={}, request=request)
+    live_update = LiveUpdatesDeviceProgress(bec=bec, report_instruction={}, request=request)
     progressbar = mock.MagicMock()
     live_update.scan_item = mock.MagicMock()
     live_update.scan_item.scan_id = "scan_id"
 
     bec.connector.get.return_value = messages.ProgressMessage(
         value=10, max_value=20, done=False, metadata={"scan_id": "scan_id"}
     )
@@ -46,15 +46,15 @@
     assert progressbar.max_points == 20
     progressbar.update.assert_called_once_with(10)
 
 
 def test_update_progressbar_returns_true_when_max_value_is_reached():
     bec = mock.MagicMock()
     request = mock.MagicMock()
-    live_update = LiveUpdatesScanProgress(bec=bec, report_instruction={}, request=request)
+    live_update = LiveUpdatesDeviceProgress(bec=bec, report_instruction={}, request=request)
     progressbar = mock.MagicMock()
     live_update.scan_item = mock.MagicMock()
     live_update.scan_item.scan_id = "scan_id"
 
     bec.connector.get.return_value = messages.ProgressMessage(
         value=10, max_value=10, done=True, metadata={"scan_id": "scan_id"}
     )
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 import time
 from unittest.mock import PropertyMock
 
 import numpy as np
 import pytest
 
 from bec_ipython_client.callbacks.utils import ScanRequestError
-from bec_lib import MessageEndpoints, bec_logger, configs
+from bec_lib import configs
 from bec_lib.alarm_handler import AlarmBase
 from bec_lib.bec_errors import ScanAbortion, ScanInterruption
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 
 logger = bec_logger.logger
 
 
 @pytest.mark.timeout(100)
 def test_grid_scan(capsys, bec_ipython_client_fixture):
     bec = bec_ipython_client_fixture
```

### Comparing `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py` & `ophyd_devices-1.0.2/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import time
 
 import numpy as np
 import pytest
 import yaml
 
-from bec_lib import DeviceConfigError, bec_logger
 from bec_lib.alarm_handler import AlarmBase
+from bec_lib.devicemanager import DeviceConfigError
+from bec_lib.logger import bec_logger
 
 logger = bec_logger.logger
 
 
 @pytest.mark.timeout(100)
 def test_grid_scan_lib(bec_client_lib):
     bec = bec_client_lib
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/README.md` & `ophyd_devices-1.0.2/bec/bec_lib/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ## Documentation
 
 The documentation is part of the BEC documentation and can be found [here](https://bec.readthedocs.io/en/latest/).
 
 ## Usage
 
 ```python
-from bec_lib import BECClient
+from bec_lib.client import BECClient
 
 # Create a new BECClient instance and start it
 bec = BECClient()
 bec.start()
 
 # Convenient access to scans and devices
 scans = bec.scans
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/pyproject.toml` & `ophyd_devices-1.0.2/bec/bec_lib/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec_lib"
-version = "2.11.0"
+version = "2.12.3"
 description = "BEC library"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
@@ -45,16 +45,16 @@
     "pytest~=8.0",
     "pytest-random-order~=1.1",
     "pytest-timeout~=2.2",
     "pytest-redis~=3.0",
 ]
 
 [project.scripts]
-bec-channel-monitor = "bec_lib:channel_monitor_launch"
-bec-log-monitor = "bec_lib:log_monitor_launch"
+bec-channel-monitor = "bec_lib.channel_monitor:channel_monitor_launch"
+bec-log-monitor = "bec_lib.channel_monitor:log_monitor_launch"
 
 [project.entry-points.pytest11]
 bec_lib_fixtures = "bec_lib.tests.fixtures"
 
 [project.urls]
 "Bug Tracker" = "https://gitlab.psi.ch/bec/bec/issues"
 Homepage = "https://gitlab.psi.ch/bec/bec"
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/alarm_handler.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/alarm_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from __future__ import annotations
 
 import enum
 import threading
 from collections import deque
 from typing import TYPE_CHECKING
 
-from bec_lib import messages
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
 from bec_lib.utils import threadlocked
 
 if TYPE_CHECKING:
+    from bec_lib import messages
     from bec_lib.redis_connector import RedisConnector
 
 
 logger = bec_logger.logger
 
 
 class Alarms(int, enum.Enum):
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/async_data.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/async_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bec_service.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bec_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,26 @@
 from dataclasses import asdict, dataclass
 from typing import TYPE_CHECKING, Any
 
 import psutil
 from rich.console import Console
 from rich.table import Table
 
-from bec_lib import messages
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
-from bec_lib.messages import BECStatus
 from bec_lib.service_config import ServiceConfig
+from bec_lib.utils.import_utils import lazy_import, lazy_import_from
 
 if TYPE_CHECKING:
     from bec_lib.connector import ConnectorBase
 
+# TODO: put back normal imports when Pydantic gets faster
+messages = lazy_import("bec_lib.messages")
+BECStatus = lazy_import_from("bec_lib.messages", ("BECStatus",))
+
 
 logger = bec_logger.logger
 
 SERVICE_CONFIG = None
 
 
 class BECService:
@@ -281,15 +284,17 @@
 
     @property
     def service_status(self):
         """get the status of active services"""
         self._update_existing_services()
         return self._services_info
 
-    def wait_for_service(self, name, status=BECStatus.RUNNING):
+    def wait_for_service(self, name, status=None):
+        if status is None:
+            status = BECStatus.RUNNING
         logger.info(f"Waiting for {name}.")
         while True:
             service_status_msg = self.service_status.get(name)
             if service_status_msg is not None:
                 service_status = BECStatus(service_status_msg.content["status"])
                 if service_status == status:
                     break
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bec_yaml_loader.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bec_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bl_checks.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bl_checks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bl_conditions.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/bl_conditions.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/callback_handler.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/channel_monitor.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/channel_monitor.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/client.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,33 +10,35 @@
 import importlib
 import inspect
 from typing import TYPE_CHECKING
 
 from rich.console import Console
 from rich.table import Table
 
-from bec_lib import messages
 from bec_lib.alarm_handler import AlarmHandler, Alarms
 from bec_lib.bec_service import BECService
 from bec_lib.bl_checks import BeamlineChecks
 from bec_lib.callback_handler import CallbackHandler, EventType
 from bec_lib.dap_plugins import DAPPlugins
 from bec_lib.devicemanager import DeviceManagerBase
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
-from bec_lib.redis_connector import RedisConnector
-from bec_lib.scan_manager import ScanManager
-from bec_lib.scans import Scans
 from bec_lib.service_config import ServiceConfig
 from bec_lib.user_scripts_mixin import UserScriptsMixin
+from bec_lib.utils.import_utils import lazy_import_from
 
 if TYPE_CHECKING:
     from bec_lib.connector import ConnectorBase
 
 logger = bec_logger.logger
+# TODO: put back normal import when Pydantic gets faster
+VariableMessage = lazy_import_from("bec_lib.messages", ("VariableMessage",))
+RedisConnector = lazy_import_from("bec_lib.redis_connector", ("RedisConnector",))
+ScanManager = lazy_import_from("bec_lib.scan_manager", ("ScanManager",))
+Scans = lazy_import_from("bec_lib.scans", ("Scans",))
 
 
 class BECClient(BECService, UserScriptsMixin):
     """
     The BECClient class is the main entry point for the BEC client and all derived classes.
     """
 
@@ -160,15 +162,15 @@
         """currently stored pre-scan macros"""
         return self.connector.lrange(MessageEndpoints.pre_scan_macros(), 0, -1)
 
     @pre_scan_macros.setter
     def pre_scan_macros(self, hooks: list[str]):
         self.connector.delete(MessageEndpoints.pre_scan_macros())
         for hook in hooks:
-            msg = messages.VariableMessage(value=hook)
+            msg = VariableMessage(value=hook)
             self.connector.lpush(MessageEndpoints.pre_scan_macros(), msg)
 
     def _load_scans(self):
         self.scans = Scans(self._parent)
         builtins.__dict__["scans"] = self.scans
 
     def load_high_level_interface(self, module_name: str) -> None:
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/config_helper.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/config_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,26 @@
 import time
 import uuid
 from typing import TYPE_CHECKING
 
 import yaml
 
 import bec_lib
-from bec_lib import messages
 from bec_lib.bec_errors import DeviceConfigError, ServiceConfigError
 from bec_lib.bec_yaml_loader import yaml_load
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.file_utils import DeviceConfigWriter
 from bec_lib.logger import bec_logger
-from bec_lib.messages import DeviceConfigMessage, RequestResponseMessage
+from bec_lib.utils.import_utils import lazy_import_from
+
+# TODO: put back normal import when Pydantic gets faster
+DeviceConfigMessage = lazy_import_from("bec_lib.messages", ("DeviceConfigMessage",))
 
 if TYPE_CHECKING:
+    from bec_lib.messages import RequestResponseMessage, ServiceResponseMessage
     from bec_lib.redis_connector import RedisConnector
 
 logger = bec_logger.logger
 
 
 class ConfigHelper:
     """Config Helper"""
@@ -162,15 +165,15 @@
                 raise DeviceConfigError(
                     f"Failed to update the config for some devices. The following devices were disabled: {devices}."
                 )
         finally:
             # wait for the device server and scan server to acknowledge the config change
             self.wait_for_service_response(RID)
 
-    def wait_for_service_response(self, RID: str, timeout=10) -> messages.ServiceResponseMessage:
+    def wait_for_service_response(self, RID: str, timeout=10) -> ServiceResponseMessage:
         """
         wait for service response
 
         Args:
             RID (str): request id
             timeout (int, optional): timeout in seconds. Defaults to 10.
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/connector.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 This module defines the interface for a connector
 """
 
 from __future__ import annotations
 
 import abc
+from typing import TYPE_CHECKING
 
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
-from bec_lib.messages import BECMessage, LogMessage
+
+if TYPE_CHECKING:
+    from bec_lib.messages import BECMessage
 
 logger = bec_logger.logger
 
 
 class ConsumerConnectorError(Exception):
     """
     ConsumerConnectorError is raised when there is an error with the connector
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/dap_plugin_objects.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/dap_plugin_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 from __future__ import annotations
 
 import builtins
 import time
 import uuid
 from typing import TYPE_CHECKING
 
-import lmfit
 import numpy as np
 from typeguard import typechecked
 
 from bec_lib import messages
 from bec_lib.device import DeviceBase
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.lmfit_serializer import serialize_param_object
 from bec_lib.scan_items import ScanItem
 from bec_lib.scan_report import ScanReport
+from bec_lib.utils.import_utils import lazy_import
+
+lmfit = lazy_import("lmfit")
 
 if TYPE_CHECKING:
     from bec_lib.client import BECClient
 
 try:
     import matplotlib.pyplot as plt
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/dap_plugins.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/dap_plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module provides the DAPPlugins class, which is used to access all available DAP plugins.
 """
 
 from __future__ import annotations
 
-import bec_lib.dap_plugin_objects as dap_plugin_objects
+import importlib
+
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
 from bec_lib.signature_serializer import dict_to_signature
 
 logger = bec_logger.logger
 
 
@@ -70,14 +71,15 @@
                         plugin_info.get("signature"),
                     )
                 # pylint: disable=broad-except
                 except Exception as e:
                     logger.error(f"Error importing plugin {plugin_name}: {e}")
 
     def _get_plugin_class(self, plugin_info):
+        dap_plugin_objects = importlib.import_module("bec_lib.dap_plugin_objects")
         if hasattr(dap_plugin_objects, plugin_info["class"]):
             return getattr(dap_plugin_objects, plugin_info["class"])
         if plugin_info.get("auto_run_supported"):
             return dap_plugin_objects.DAPPluginObjectAutoRun
         return dap_plugin_objects.DAPPluginObject
 
     def _set_plugin(
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/device.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,28 @@
 import time
 import uuid
 from collections import namedtuple
 from typing import TYPE_CHECKING, Any
 
 from typeguard import typechecked
 
-from bec_lib import messages
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
+from bec_lib.utils.import_utils import lazy_import
+
+# TODO: put back normal import when Pydantic gets faster
+# from bec_lib import messages
+messages = lazy_import("bec_lib.messages")
 
-logger = bec_logger.logger
 
 if TYPE_CHECKING:
     from bec_lib.redis_connector import RedisConnector
 
+logger = bec_logger.logger
+
 
 class RPCError(Exception):
     """Exception raised when an RPC call fails."""
 
 
 class ScanRequestError(Exception):
     """Exception raised when a scan request is rejected."""
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/devicemanager.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/devicemanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,29 @@
 import traceback
 from typing import TYPE_CHECKING
 
 from rich.console import Console
 from rich.table import Table
 from typeguard import typechecked
 
-from bec_lib import messages
 from bec_lib.bec_errors import DeviceConfigError
 from bec_lib.config_helper import ConfigHelper
 from bec_lib.device import ComputedSignal, Device, DeviceBase, Positioner, ReadoutPriority, Signal
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
-from bec_lib.messages import BECStatus, DeviceConfigMessage, DeviceInfoMessage
+from bec_lib.utils.import_utils import lazy_import_from
+
+# TODO: put back normal import when Pydantic gets faster
+BECStatus, ServiceResponseMessage = lazy_import_from(
+    "bec_lib.messages", ("BECStatus", "ServiceResponseMessage")
+)
 
 if TYPE_CHECKING:
-    from bec_lib import BECService
+    from bec_lib.bec_service import BECService
+    from bec_lib.messages import DeviceConfigMessage, DeviceInfoMessage
 
 logger = bec_logger.logger
 
 
 class DeviceContainer(dict):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -466,15 +471,15 @@
         Returns:
 
         """
         if not msg.metadata.get("RID"):
             return
         self.connector.lpush(
             MessageEndpoints.service_response(msg.metadata["RID"]),
-            messages.ServiceResponseMessage(
+            ServiceResponseMessage(
                 # pylint: disable=no-member
                 response={"accepted": True, "service": self._service._service_name}
             ),
             expire=100,
         )
 
     def _add_action(self, config) -> None:
@@ -541,15 +546,15 @@
 
     def _get_redis_device_config(self) -> list:
         devices = self.connector.get(MessageEndpoints.device_config())
         if not devices:
             return []
         return devices.content["resource"]
 
-    def _add_device(self, dev: dict, msg: messages.DeviceInfoMessage):
+    def _add_device(self, dev: dict, msg: DeviceInfoMessage):
         name = msg.content["device"]
         info = msg.content["info"]
 
         base_class = info["device_info"]["device_base_class"]
 
         if base_class == "device":
             logger.info(f"Adding new device {name}")
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/endpoints.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 """
 Endpoints for communication within the BEC.
 """
 
+from __future__ import annotations
+
 # pylint: disable=too-many-public-methods
 import enum
 from dataclasses import dataclass
 
-from bec_lib import messages
+from bec_lib.utils.import_utils import lazy_import
+
+# TODO: put back normal import when Pydantic gets faster
+# from bec_lib import messages
+messages = lazy_import("bec_lib.messages")
 
 
 class MessageOp(list[str], enum.Enum):
     """Message operation enum"""
 
     SET_PUBLISH = ["register", "set_and_publish", "delete", "get", "keys"]
     SEND = ["send", "register"]
@@ -516,14 +522,30 @@
         return EndpointInfo(
             endpoint=endpoint,
             message_type=messages.ScanStatusMessage,
             message_op=MessageOp.SET_PUBLISH,
         )
 
     @staticmethod
+    def scan_progress() -> EndpointInfo:
+        """
+        Endpoint for scan progress. This endpoint is used to publish the scan progress using
+        a messages.ProgressMessage message.
+
+        Returns:
+            EndpointInfo: Endpoint for scan progress.
+        """
+        endpoint = "scans/scan_progress"
+        return EndpointInfo(
+            endpoint=endpoint,
+            message_type=messages.ProgressMessage,
+            message_op=MessageOp.SET_PUBLISH,
+        )
+
+    @staticmethod
     def available_scans() -> EndpointInfo:
         """
         Endpoint for available scans. This endpoint is used to publish the available scans
         using an AvailableResourceMessage.
 
         Returns:
             EndpointInfo: Endpoint for available scans.
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/file_utils.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/file_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 import os
 import warnings
 from typing import TYPE_CHECKING
 
 from bec_lib.bec_errors import ServiceConfigError
 from bec_lib.endpoints import MessageEndpoints
-from bec_lib.messages import ScanStatusMessage
+from bec_lib.utils.import_utils import lazy_import_from
+
+# TODO: put back normal import when Pydantic gets faster
+ScanStatusMessage = lazy_import_from("bec_lib.messages", ("ScanStatusMessage",))
 
 if TYPE_CHECKING:
     from bec_lib.redis_connector import RedisConnector
 
 
 class ServiceConfigParser:
     """Service Config Parser"""
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/lmfit_serializer.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/lmfit_serializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 This module contains functions for serializing and deserializing lmfit objects.
 """
 
-from lmfit import Parameter, Parameters
+from bec_lib.utils.import_utils import lazy_import_from
+
+Parameter, Parameters = lazy_import_from("lmfit", ("Parameter", "Parameters"))
 
 
 def serialize_param_object(param: Parameter) -> dict:
     """
     Serialize lmfit.Parameter object to JSON-serializable dictionary.
 
     Args:
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/logbook_connector.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/logger.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 import json
 import os
 import sys
 import traceback
 from itertools import takewhile
 from typing import TYPE_CHECKING
 
-from loguru import logger as loguru_logger
-
 # TODO: Importing bec_lib, instead of `from bec_lib.messages import LogMessage`, avoids potential
 # logger <-> messages circular import. But there could be a better solution.
 import bec_lib
 from bec_lib.bec_errors import ServiceConfigError
 from bec_lib.endpoints import MessageEndpoints
-from bec_lib.file_utils import LogWriter
+from bec_lib.utils.import_utils import lazy_import_from
 
 if TYPE_CHECKING:
     from bec_lib.connector import ConnectorBase
 
+loguru_logger = lazy_import_from("loguru", ("logger",))
+LogWriter = lazy_import_from("bec_lib.file_utils", ("LogWriter",))
+
 
 class LogLevel(int, enum.Enum):
     """Mapping of Loguru log levels to BEC log levels."""
 
     TRACE = 5
     DEBUG = 10
     INFO = 20
@@ -75,18 +76,16 @@
         self.bootstrap_server = None
         self.connector = None
         self.service_name = None
         self.writer_mixin = None
         self._base_path = None
         self.logger = loguru_logger
         self._log_level = LogLevel.INFO
-        self.level = self._log_level
         self._configured = False
         # self.logger.level("CONSOLE_LOG", no=21, color="<yellow>", icon="📣")
-        self._update_logger_level()
 
     def __new__(cls):
         if not hasattr(cls, "_logger") or cls._logger is None:
             cls._logger = super(BECLogger, cls).__new__(cls)
         return cls._logger
 
     @classmethod
@@ -112,14 +111,16 @@
         Configure the logger.
 
         Args:
             bootstrap_server (list): List of bootstrap servers.
             connector_cls (ConnectorBase): Connector class.
             service_name (str): Name of the service to which the logger belongs.
         """
+        self.level = self._log_level
+        self._update_logger_level()
         if not self._base_path:
             self._update_base_path(service_config)
         if os.path.exists(self._base_path) is False:
             self.writer_mixin.create_directory(self._base_path)
         self.bootstrap_server = bootstrap_server
         self.connector = connector_cls(bootstrap_server)
         self.service_name = service_name
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/messages.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import enum
 import time
 import warnings
 from copy import deepcopy
 from typing import Any, ClassVar, Literal
 
 import numpy as np
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/numpy_encoder.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/observer.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/observer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/pdf_writer.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/plugin_helper.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/plugin_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/queue_items.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/redis_connector.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/redis_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,16 +536,23 @@
             # directly calling the callback. This is because we need to have a backpressure
             # mechanism in place, and we cannot rely on the dispatcher thread to handle it.
             for topic in topics:
                 self._add_direct_stream_listener(topic, cb_ref, **kwargs)
         else:
             with self._stream_topics_subscription_lock:
                 for topic in topics:
+                    try:
+                        stream_info = self._redis_conn.xinfo_stream(topic)
+                    except redis.exceptions.ResponseError:
+                        # no such key
+                        last_id = "0-0"
+                    else:
+                        last_id = stream_info["last-entry"][0].decode()
                     new_subscription = StreamSubscriptionInfo(
-                        id="0-0" if from_start else "$",
+                        id="0-0" if from_start else last_id,
                         topic=topic,
                         newest_only=newest_only,
                         from_start=from_start,
                         cb_ref=cb_ref,
                         kwargs=kwargs,
                     )
                     subscriptions = self._stream_topics_subscription[topic]
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/request_items.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/request_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 
 from __future__ import annotations
 
 import threading
 from collections import deque
 from typing import TYPE_CHECKING
 
-from bec_lib import messages
 from bec_lib.callback_handler import CallbackHandler
 from bec_lib.logger import bec_logger
-from bec_lib.utils import threadlocked
 
 logger = bec_logger.logger
 
 
 if TYPE_CHECKING:
+    from bec_lib import messages
     from bec_lib.queue_items import QueueItem
     from bec_lib.scan_items import ScanItem
     from bec_lib.scan_manager import ScanManager
 
 
 class RequestItem:
     # pylint: disable=too-many-arguments
@@ -130,58 +129,58 @@
     """stores request items"""
 
     def __init__(self, scan_manager: ScanManager, maxlen=50) -> None:
         self.storage: deque[RequestItem] = deque(maxlen=maxlen)
         self._lock = threading.RLock()
         self.scan_manager = scan_manager
 
-    @threadlocked
     def find_request_by_ID(self, requestID: str) -> RequestItem | None:
         """find a request item based on its requestID"""
-        for request in self.storage:
-            if request.requestID == requestID:
-                return request
-        return None
+        with self._lock:
+            for request in self.storage:
+                if request.requestID == requestID:
+                    return request
+            return None
 
-    @threadlocked
     def update_with_response(self, response_msg: messages.RequestResponseMessage) -> None:
         """create or update request item based on a new RequestResponseMessage"""
-        request_item = self.find_request_by_ID(response_msg.metadata.get("RID"))
-        if request_item:
-            request_item.update_with_response(response_msg)
-            logger.debug("Scan queue request exists. Updating with response.")
-            return
-
-        # it could be that the response arrived before the request
-        self.storage.append(RequestItem.from_response(self.scan_manager, response_msg))
-        logger.debug("Scan queue request does not exist. Creating from response.")
+        with self._lock:
+            request_item = self.find_request_by_ID(response_msg.metadata.get("RID"))
+            if request_item:
+                request_item.update_with_response(response_msg)
+                logger.debug("Scan queue request exists. Updating with response.")
+                return
+
+            # it could be that the response arrived before the request
+            self.storage.append(RequestItem.from_response(self.scan_manager, response_msg))
+            logger.debug("Scan queue request does not exist. Creating from response.")
 
-    @threadlocked
     def update_with_request(self, request_msg: messages.ScanQueueMessage) -> None:
         """create or update request item based on a new ScanQueueMessage (i.e. request message)"""
-        if not request_msg.metadata:
-            return
+        with self._lock:
+            if not request_msg.metadata:
+                return
+
+            if not request_msg.metadata.get("RID"):
+                return
+
+            request_item = self.find_request_by_ID(request_msg.metadata.get("RID"))
+            if request_item:
+                request_item.update_with_request(request_msg)
+                return
 
-        if not request_msg.metadata.get("RID"):
+            self.storage.append(RequestItem.from_request(self.scan_manager, request_msg))
             return
 
-        request_item = self.find_request_by_ID(request_msg.metadata.get("RID"))
-        if request_item:
-            request_item.update_with_request(request_msg)
-            return
-
-        self.storage.append(RequestItem.from_request(self.scan_manager, request_msg))
-        return
-
-    @threadlocked
     def update_with_client_message(self, client_message: messages.ClientInfoMessage) -> None:
         """Update the request item with a new ClientInfoMessage"""
-        if not client_message.RID:
-            return
+        with self._lock:
+            if not client_message.RID:
+                return
+
+            request_item = self.find_request_by_ID(client_message.RID)
+            if request_item:
+                request_item.update_with_client_message(client_message)
+                return
 
-        request_item = self.find_request_by_ID(client_message.RID)
-        if request_item:
-            request_item.update_with_client_message(client_message)
+            self.storage.append(RequestItem.from_client_message(self.scan_manager, client_message))
             return
-
-        self.storage.append(RequestItem.from_client_message(self.scan_manager, client_message))
-        return
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_data.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 This module contains the classes for storing scan data from scan_segments. 
 """
 
+from __future__ import annotations
+
 import collections
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 from _collections_abc import dict_items, dict_keys, dict_values
 
-from bec_lib import messages
+if TYPE_CHECKING:
+    from bec_lib import messages
 
 
 class SignalData:
     """
     SignalData is a container for storing signal data.
     """
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_items.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 information about a scan. The ScanStorage class is used to store scan items.
 """
 
 from __future__ import annotations
 
 import builtins
 import datetime
+import importlib
 import sys
 import threading
 import time
 from collections import defaultdict, deque
 from typing import TYPE_CHECKING
 
-from bec_lib import messages
 from bec_lib.async_data import AsyncDataHandler
 from bec_lib.logger import bec_logger
 from bec_lib.scan_data import ScanData
 from bec_lib.utils import threadlocked
 
 if TYPE_CHECKING:
+    from bec_lib import messages
     from bec_lib.scan_manager import ScanManager
 
-logger = bec_logger.logger
+    try:
+        import pandas as pd
+    except ImportError:
+        logger.info("Unable to import `pandas` optional dependency")
 
-try:
-    import pandas as pd
-except ImportError:
-    logger.info("Unable to import `pandas` optional dependency")
+logger = bec_logger.logger
 
 
 class ScanItem:
     status: dict
 
     # pylint: disable=too-many-arguments
     def __init__(
@@ -84,19 +85,23 @@
     def poll_callbacks(self):
         for rid in self.queue.requestIDs:
             req = self.scan_manager.request_storage.find_request_by_ID(rid)
             if req is None:
                 continue
             req.callbacks.poll()
 
-    def to_pandas(self) -> pd.DataFrame:
-        """convert to pandas dataframe"""
-        if "pandas" not in sys.modules:
+    def _get_pandas(self):
+        try:
+            return importlib.import_module("pandas")
+        except ImportError:
             raise ImportError("Install `pandas` to use to_pandas() method")
 
+    def to_pandas(self) -> pd.DataFrame:
+        """convert to pandas dataframe"""
+        pd = self._get_pandas()
         tmp = defaultdict(list)
         for scan_msg in self.data.messages.values():
             scan_msg_data = scan_msg.content["data"]
             for dev, dev_data in scan_msg_data.items():
                 for signal, signal_data in dev_data.items():
                     for key, value in signal_data.items():
                         tmp[(dev, signal, key)].append(value)
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_manager.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_report.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scan_report.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scans.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scans.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,28 +101,20 @@
         report.request.callbacks.register_many("scan_segment", callback, sync=True)
         report.request.callbacks.register_many("scan_segment", async_callback, sync=False)
 
         if scans._scan_export and scans._scan_export.scans is not None:
             scans._scan_export.scans.append(report)
 
         if not hide_report and self.client.live_updates:
-            scan_report_type = self._get_scan_report_type(hide_report)
-            # call process_requests even if report_type is None
-            self.client.live_updates.process_request(request, scan_report_type, callback)
+            self.client.live_updates.process_request(request, callback)
 
         self.client.callbacks.poll()
 
         return report
 
-    def _get_scan_report_type(self, hide_report) -> str:
-        """get the scan report type"""
-        if hide_report:
-            return None
-        return self.scan_info.get("scan_report_hint")
-
     def _start_register(self, request: messages.ScanQueueMessage) -> ConsumerConnector:
         """Start a register for the given request"""
         register = self.client.device_manager.connector.register(
             [
                 MessageEndpoints.device_readback(dev)
                 for dev in request.content["parameter"]["args"].keys()
             ],
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scibec_validator.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/serialization.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/serialization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/service_config.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/service_config.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/signature_serializer.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/signature_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/user_scripts_mixin.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/user_scripts_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,31 +8,27 @@
 import glob
 import importlib
 import inspect
 import os
 import pathlib
 from typing import TYPE_CHECKING
 
-from pylint import lint
-from pylint.reporters import CollectingReporter
 from rich.console import Console
 from rich.table import Table
 
 from bec_lib.callback_handler import EventType
 from bec_lib.logger import bec_logger
+from bec_lib.utils.import_utils import lazy_import, lazy_import_from
 
 if TYPE_CHECKING:
     from pylint.message import Message
 
 logger = bec_logger.logger
-
-try:
-    from bec_plugins import bec_ipython_client as client_plugins
-except ImportError:
-    client_plugins = None
+pylint = lazy_import("pylint")
+CollectingReporter = lazy_import_from("pylint.reporters", ("CollectingReporter",))
 
 
 class UserScriptsMixin:
     def __init__(self) -> None:
         super().__init__()
         self._scripts = {}
 
@@ -50,20 +46,23 @@
 
         # load all scripts from the user's script directory in the home directory
         user_script_dir = os.path.join(os.path.expanduser("~"), "bec", "scripts")
         if os.path.exists(user_script_dir):
             script_files.extend(glob.glob(os.path.abspath(os.path.join(user_script_dir, "*.py"))))
 
         # load scripts from the plugins
-        if client_plugins:
-            plugin_scripts_dir = os.path.join(client_plugins.__path__[0], "scripts")
-            if os.path.exists(plugin_scripts_dir):
-                script_files.extend(
-                    glob.glob(os.path.abspath(os.path.join(plugin_scripts_dir, "*.py")))
-                )
+        plugins = importlib.metadata.entry_points(group="bec")
+        for plugin in plugins:
+            if plugin.name == "plugin_bec":
+                plugin = plugin.load()
+                plugin_scripts_dir = os.path.join(plugin.__path__[0], "scripts")
+                if os.path.exists(plugin_scripts_dir):
+                    script_files.extend(
+                        glob.glob(os.path.abspath(os.path.join(plugin_scripts_dir, "*.py")))
+                    )
 
         for file in script_files:
             self.load_user_script(file)
         builtins.__dict__.update({name: v["cls"] for name, v in self._scripts.items()})
 
     def forget_all_user_scripts(self) -> None:
         """unload / remove loaded user scripts from builtins. Files will remain untouched.
@@ -131,15 +130,15 @@
         module_members = inspect.getmembers(plugin_module)
         return module_members
 
     def _run_linter_on_file(self, file) -> None:
         accepted_vars = ",".join([key for key in builtins.__dict__ if not key.startswith("_")])
         reporter = CollectingReporter()
         print(f"{accepted_vars}")
-        lint.Run(
+        pylint.lint.Run(
             [file, "--errors-only", f"--additional-builtins={accepted_vars}"],
             exit=False,
             reporter=reporter,
         )
         if not reporter.messages:
             return
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/configs/demo_config.yaml` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/configs/demo_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/configs/openapi_schema.json` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/fixtures.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/test_config.yaml` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/test_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/utils.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import time
 import uuid
 from typing import TYPE_CHECKING
 
 import yaml
 
 import bec_lib
-from bec_lib import BECClient, messages
+from bec_lib import messages
+from bec_lib.client import BECClient
 from bec_lib.connector import ConnectorBase
 from bec_lib.devicemanager import DeviceManagerBase
 from bec_lib.endpoints import EndpointInfo, MessageEndpoints
 from bec_lib.logger import bec_logger
 from bec_lib.scans import Scans
 
 if TYPE_CHECKING:
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/import_utils.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/import_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def lazy_import(module_name):
     return Proxy(lambda: import_module(module_name), init_once=True)
 
 
 def lazy_import_from(module_name, from_list):
-    ret = (Proxy(lambda: getattr(import_module(module_name), name)) for name in from_list)
+    ret = (Proxy(lambda name=name: getattr(import_module(module_name), name)) for name in from_list)
     if len(from_list) == 1:
         return next(ret)
     else:
         return ret
 
 
 def isinstance_based_on_class_name(obj: Any, full_class_name: str):
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/proxy.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/rpc_utils.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/rpc_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/scan_utils.py` & `ophyd_devices-1.0.2/bec/bec_lib/bec_lib/utils/scan_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_async_data.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_async_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_beamline_checks.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_beamline_checks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_bec_logger.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_bec_logger.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_bec_messages.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_bec_messages.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_bec_service.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_bec_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import os
 from pathlib import Path
 from unittest import mock
 
 import pytest
 
 import bec_lib
-from bec_lib import bec_logger, messages
+from bec_lib import messages
 from bec_lib.bec_service import BECService
 from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 from bec_lib.messages import BECStatus
 from bec_lib.service_config import ServiceConfig
 
 # pylint: disable=no-member
 # pylint: disable=missing-function-docstring
 # pylint: disable=redefined-outer-name
 # pylint: disable=protected-access
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_bl_conditions.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_bl_conditions.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_callback_handler.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_callback_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_channel_monitor.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_channel_monitor.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_config_helper.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_config_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_core_utils.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_core_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_dap_plugins.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_dap_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from math import inf
 from unittest import mock
 
 import pytest
 
-from bec_lib import MessageEndpoints, messages
+from bec_lib import messages
 from bec_lib.dap_plugin_objects import DAPPluginObject, LmfitService1D
 from bec_lib.dap_plugins import DAPPlugins
 from bec_lib.device import DeviceBase
+from bec_lib.endpoints import MessageEndpoints
 from bec_lib.scan_items import ScanItem
 from bec_lib.scan_report import ScanReport
 
 
 @pytest.fixture
 def dap_plugin_message():
     msg = messages.AvailableResourceMessage(
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_device_manager.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_devices.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_file_utils.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_lmfit_serializer.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_observer.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_plugin_helper.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_plugin_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import bec_lib
 from bec_lib import plugin_helper
 
 
 @pytest.mark.parametrize(
     "class_spec, out_name",
-    [("bec_lib.messages.BECMessage", "BECMessage"), ("bec_lib.BECStatus", "BECStatus")],
+    [("bec_lib.messages.BECMessage", "BECMessage"), ("bec_lib.messages.BECStatus", "BECStatus")],
 )
 def test_get_plugin_class(class_spec, out_name):
     cls = plugin_helper.get_plugin_class(class_spec, [bec_lib])
     assert cls.__name__ == out_name
 
 
 @pytest.mark.parametrize(
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_redis_connector.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_redis_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_redis_connector_fakeredis.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_redis_connector_fakeredis.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,15 +441,15 @@
         connector.xadd(ep, {"data": 2})
         connector.poll_messages()
     assert mock.call({"data": 2}, a=1) in cb_mock.mock_calls
     connector.unregister(endpoint)
     assert len(connector._stream_topics_subscription) == 0
 
 
-@pytest.mark.timeout(5)
+@pytest.mark.timeout(10)
 def test_redis_connector_register_stream_from_start(connected_connector):
     connector = connected_connector
     cb_mock1 = mock.Mock(spec=[])  # spec is here to remove all attributes
     cb_mock2 = mock.Mock(spec=[])  # spec is here to remove all attributes
     connector.xadd("test", {"data": 1})
     connector.xadd("test", {"data": 2})
     connector.register(TestStreamEndpoint, cb=cb_mock1, from_start=True, start_thread=False, a=1)
@@ -464,14 +464,19 @@
     cb_mock2.assert_called_once_with({"data": 3}, a=2)
     cb_mock1.reset_mock()
     connector.register(TestStreamEndpoint, cb=cb_mock1, from_start=True, start_thread=False, a=3)
     connector.poll_messages(timeout=1)
     cb_mock1.assert_has_calls(
         [mock.call({"data": 1}, a=3), mock.call({"data": 2}, a=3), mock.call({"data": 3}, a=3)]
     )
+    cb_mock1.reset_mock()
+    connector.register(TestStreamEndpoint, cb=cb_mock1, start_thread=False, a=4)
+    with pytest.raises(TimeoutError):
+        connector.poll_messages(timeout=1)
+    cb_mock1.assert_not_called()
 
 
 @pytest.mark.timeout(5)
 def test_redis_connector_register_stream_newest_only(connected_connector):
     connector = connected_connector
     endpoint = TestStreamEndpoint
     # simulate callback taking 1s to perform its task
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_context.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_context.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_data.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_items.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_items.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,16 +104,16 @@
 
 
 def test_scan_item_to_pandas_raises_without_pandas_installed():
     """Test that to_pandas raises an ImportError if pandas is not installed."""
     scan_manager = ScanManager(ConnectorMock(""))
     scan_item = ScanItem(scan_manager, "queue_id", [1], ["scan_id"], "status")
 
-    with mock.patch.dict("sys.modules"):
-        del sys.modules["pandas"]
+    with mock.patch.object(scan_item, "_get_pandas") as get_pandas:
+        get_pandas.side_effect = ImportError
         with pytest.raises(ImportError):
             scan_item.to_pandas()
 
 
 def test_scan_item_str():
     scan_manager = ScanManager(ConnectorMock(""))
     scan_item = ScanItem(scan_manager, "queue_id", [1], ["scan_id"], "status")
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_manager.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from unittest import mock
 
 import pytest
 
-from bec_lib import MessageEndpoints, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
 from bec_lib.scan_manager import ScanManager
 
 
 @pytest.fixture
 def scan_manager():
     connector = mock.MagicMock()
     manager = ScanManager(connector=connector)
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_object.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 @pytest.fixture
 def scan_obj(bec_client_mock):
     scan_info = {
         "class": "FermatSpiralScan",
         "arg_input": {"device": "device", "start": "float", "stop": "float"},
         "required_kwargs": ["step", "relative"],
         "arg_bundle_size": {"bundle": 3, "min": 2, "max": 2},
-        "scan_report_hint": "table",
         "doc": (
             "\n        A scan following Fermat's spiral.\n\n        Args:\n            *args: pairs"
             " of device / start position / end position / steps arguments\n            relative:"
             " Start from an absolute or relative position\n            burst: number of acquisition"
             " per point\n            optim_trajectory: routine used for the trajectory"
             " optimization, e.g. 'corridor'. Default: None\n\n        Returns:\n\n       "
             " Examples:\n            >>> scans.fermat_scan(dev.motor1, -5, 5, dev.motor2, -5, 5,"
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_report.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_scan_report.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_serializer.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_signature_serializer.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_signature_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_user_scripts_mixin.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/tests/test_yaml_loader.py` & `ophyd_devices-1.0.2/bec/bec_lib/tests/test_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/create_plugin_structure.py` & `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/create_plugin_structure.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/init_config.py` & `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/init_config.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md` & `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/gitignore` & `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py` & `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 The script is executed in the global namespace of the IPython shell. This
 means that all variables defined here are available in the shell.
 
 While command-line arguments have to be set in the pre-startup script, the
 post-startup script can be used to load beamline specific information and
 to setup the prompts.
 
-    from bec_lib import bec_logger
+    from bec_lib.logger import bec_logger
 
     logger = bec_logger.logger
 
     # pylint: disable=import-error
     _args = _main_dict["args"]
 
     _session_name = "cSAXS"
```

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py` & `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml` & `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py` & `ophyd_devices-1.0.2/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,12 +21,14 @@
 - self.cleanup                           # send a close scan message and perform additional cleanups if needed
 """
 
 # import time
 
 # import numpy as np
 
-# from bec_lib import MessageEndpoints, bec_logger, messages
+# from bec_lib.endpoints import MessageEndpoints
+# from bec_lib.logger import bec_logger
+# from bec_lib import messages
 # from bec_server.scan_server.errors import ScanAbortion
 # from bec_server.scan_server.scans import FlyScanBase, RequestBase, ScanArgType, ScanBase
 
 # logger = bec_logger.logger
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/pyproject.toml` & `ophyd_devices-1.0.2/bec/bec_server/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec-server"
-version = "2.11.0"
+version = "2.12.3"
 description = "BEC server"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/launch.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/service_handler.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/service_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/dap_server.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/dap_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from bec_lib import BECClient, ServiceConfig, bec_logger
+from bec_lib.client import BECClient
 from bec_lib.connector import ConnectorBase
+from bec_lib.logger import bec_logger
+from bec_lib.service_config import ServiceConfig
 
 from .dap_service_manager import DAPServiceManager
 
 logger = bec_logger.logger
 
 
 class DAPServer(BECClient):
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/dap_service.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/dap_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import abc
 from typing import TYPE_CHECKING
 
 # import numpy as np
-from bec_lib import bec_logger
+from bec_lib.logger import bec_logger
 from bec_lib.signature_serializer import signature_to_dict
 
 if TYPE_CHECKING:
-    from bec_lib import BECClient
+    from bec_lib.client import BECClient
 
 
 logger = bec_logger.logger
 
 
 class DAPError(Exception):
     pass
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/dap_service_manager.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/dap_service_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import annotations
 
-from bec_lib import BECClient, MessageEndpoints, bec_logger, messages
+from bec_lib import messages
+from bec_lib.client import BECClient
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 from bec_lib.redis_connector import MessageObject
 
 logger = bec_logger.logger
 
 
 class DAPServiceManager:
     """Base class for data processing services."""
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/lmfit1d_service.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/lmfit1d_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 import threading
 import time
 from typing import TYPE_CHECKING
 
 import lmfit
 import numpy as np
 
-from bec_lib import DeviceBase, MessageEndpoints, bec_logger, messages
+from bec_lib import messages
+from bec_lib.device import DeviceBase
+from bec_lib.endpoints import MessageEndpoints
 from bec_lib.lmfit_serializer import deserialize_param_object, serialize_lmfit_params
+from bec_lib.logger import bec_logger
 from bec_lib.serialization import MsgpackSerialization
 from bec_server.data_processing.dap_service import DAPError, DAPServiceBase
 
 if TYPE_CHECKING:
     from bec_lib.scan_items import ScanItem
 
 logger = bec_logger.logger
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/cli/launch.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/data_processing/cli/launch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Description: Launch the data processing server.
 # This script is the entry point for the Data Processing Server. It is called either
 # by the bec-dap entry point or directly from the command line.
 import argparse
 import threading
 
 import bec_server.data_processing as data_processing
-from bec_lib import RedisConnector, ServiceConfig, bec_logger
+from bec_lib.logger import bec_logger
+from bec_lib.redis_connector import RedisConnector
+from bec_lib.service_config import ServiceConfig
 from bec_server.data_processing.lmfit1d_service import LmfitService1D
 
 logger = bec_logger.logger
 bec_logger.level = bec_logger.LOGLEVEL.INFO
 
 
 def main():
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/device_server.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/device_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,21 @@
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 
 import ophyd
 from ophyd import Kind, OphydObject, Staged
 from ophyd.utils import errors as ophyd_errors
 
-from bec_lib import Alarms, BECService, MessageEndpoints, bec_logger, messages
+from bec_lib import messages
+from bec_lib.alarm_handler import Alarms
+from bec_lib.bec_service import BECService
 from bec_lib.connector import ConnectorBase
 from bec_lib.device import OnFailure
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 from bec_lib.messages import BECStatus
 from bec_server.device_server.devices.devicemanager import DeviceManagerDS
 from bec_server.device_server.rpc_mixin import RPCMixin
 
 logger = bec_logger.logger
 
 register_stop = threading.Event()
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/rpc_mixin.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/rpc_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import traceback
 from contextlib import redirect_stdout
 from io import StringIO
 from typing import Any
 
 import ophyd
 
-from bec_lib import Alarms, MessageEndpoints, bec_logger, messages
+from bec_lib import messages
+from bec_lib.alarm_handler import Alarms
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 from bec_server.device_server.devices import is_serializable, rgetattr
 
 logger = bec_logger.logger
 
 
 class RPCMixin:
     """Mixin for handling RPC calls"""
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/cli/launch.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/cli/launch.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 for entry_point in entry_points:
     if entry_point.name == "plugin_ds_startup":
         entry_point.load()()
 
 import argparse
 import threading
 
-from bec_lib import RedisConnector, ServiceConfig, bec_logger
+from bec_lib.logger import bec_logger
+from bec_lib.redis_connector import RedisConnector
+from bec_lib.service_config import ServiceConfig
 from bec_server import device_server
 
 logger = bec_logger.logger
 bec_logger.level = bec_logger.LOGLEVEL.INFO
 
 
 def main():
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/config_update_handler.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/config_update_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
 import copy
 import traceback
 from typing import TYPE_CHECKING
 
-from bec_lib import DeviceConfigError, MessageEndpoints, bec_logger, messages
+from bec_lib import messages
+from bec_lib.devicemanager import DeviceConfigError
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 
 if TYPE_CHECKING:
     from devicemanager import DeviceManagerDS
 
 logger = bec_logger.logger
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/device_serializer.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/devicemanager.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/devices/devicemanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,21 @@
 import numpy as np
 import ophyd
 import ophyd_devices as opd
 from ophyd.ophydobj import OphydObject
 from ophyd.signal import EpicsSignalBase
 from typeguard import typechecked
 
-from bec_lib import (
-    BECService,
-    DeviceBase,
-    DeviceConfigError,
-    DeviceManagerBase,
-    MessageEndpoints,
-    bec_logger,
-    messages,
-    plugin_helper,
-)
+from bec_lib import messages, plugin_helper
+from bec_lib.bec_errors import DeviceConfigError
+from bec_lib.bec_service import BECService
+from bec_lib.device import DeviceBase
+from bec_lib.devicemanager import DeviceManagerBase
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 from bec_server.device_server.devices.config_update_handler import ConfigUpdateHandler
 from bec_server.device_server.devices.device_serializer import get_device_info
 
 logger = bec_logger.logger
 
 
 def rgetattr(obj, attr, *args):
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/tests/utils.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/device_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/default_writer.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/default_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from bec_lib import DeviceManagerBase
+    from bec_lib.devicemanager import DeviceManagerBase
     from bec_server.file_writer.file_writer import HDF5Storage
 
 
 def NeXus_format(
     storage: HDF5Storage, data: dict, file_references: dict, device_manager: DeviceManagerBase
 ) -> HDF5Storage:
     """
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/file_writer.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/file_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import json
 import os
 import traceback
 import typing
 
 import h5py
 
-from bec_lib import MessageEndpoints, bec_logger, messages, plugin_helper
+from bec_lib import messages, plugin_helper
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 
 from .default_writer import NeXus_format as default_NeXus_format
 from .merged_dicts import merge_dicts
 
 logger = bec_logger.logger
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/file_writer_manager.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/file_writer_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from __future__ import annotations
 
 import threading
 import traceback
 
-from bec_lib import (
-    BECService,
-    DeviceManagerBase,
-    MessageEndpoints,
-    ServiceConfig,
-    bec_logger,
-    messages,
-    threadlocked,
-)
+from bec_lib import messages
 from bec_lib.alarm_handler import Alarms
 from bec_lib.async_data import AsyncDataHandler
+from bec_lib.bec_service import BECService
+from bec_lib.devicemanager import DeviceManagerBase
+from bec_lib.endpoints import MessageEndpoints
 from bec_lib.file_utils import FileWriter
+from bec_lib.logger import bec_logger
 from bec_lib.redis_connector import MessageObject, RedisConnector
+from bec_lib.service_config import ServiceConfig
 from bec_server.file_writer.file_writer import NexusFileWriter
 
 logger = bec_logger.logger
 
 
 class ScanStorage:
     def __init__(self, scan_number: int, scan_id: str) -> None:
@@ -250,29 +247,29 @@
             scan_id (str): Scan ID
             device_name (str): Device name
         """
         self.scan_storage[scan_id].async_data[device_name] = AsyncDataHandler.process_async_data(
             msgs
         )
 
-    @threadlocked
     def check_storage_status(self, scan_id: str) -> None:
         """
         Check if the scan storage is ready to be written to file and write it if it is.
 
         Args:
             scan_id (str): Scan ID
         """
-        if not self.scan_storage.get(scan_id):
-            return
-        self.update_baseline_reading(scan_id)
-        self.update_file_references(scan_id)
-        if self.scan_storage[scan_id].ready_to_write():
-            self.update_async_data(scan_id)
-            self.write_file(scan_id)
+        with self._lock:
+            if not self.scan_storage.get(scan_id):
+                return
+            self.update_baseline_reading(scan_id)
+            self.update_file_references(scan_id)
+            if self.scan_storage[scan_id].ready_to_write():
+                self.update_async_data(scan_id)
+                self.write_file(scan_id)
 
     def write_file(self, scan_id: str) -> None:
         """
         Write scan data to file.
 
         Args:
             scan_id (str): Scan ID
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/merged_dicts.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer/merged_dicts.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/cli/launch.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/cli/launch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-# This file is the entry point for the file writer service.
-# It is called either by the bec-file-writer entry point or directly from the command line.
+# Description: Launch the scan bundler.
+# This script is the entry point for the Scan Bundler. It is called either
+# by the bec-scan-bundler entry point or directly from the command line.
 import argparse
-import os
 import threading
 
-from bec_lib import RedisConnector, ServiceConfig, bec_logger
-from bec_server import file_writer
+from bec_lib.logger import bec_logger
+from bec_lib.redis_connector import RedisConnector
+from bec_lib.service_config import ServiceConfig
+from bec_server import scan_bundler
 
 logger = bec_logger.logger
 bec_logger.level = bec_logger.LOGLEVEL.INFO
 
 
 def main():
     """
-    Launch the file writer.
+    Launch the scan bundler.
     """
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("--config", default="", help="path to the config file")
     clargs = parser.parse_args()
     config_path = clargs.config
 
     config = ServiceConfig(config_path)
 
-    file_writer_manager = file_writer.FileWriterManager(config, RedisConnector)
+    sb = scan_bundler.ScanBundler(config, RedisConnector)
+
     try:
         event = threading.Event()
-        logger.success("Started FileWriter")
+        logger.success("Started ScanBundler")
         event.wait()
     except KeyboardInterrupt:
-        file_writer_manager.shutdown()
+        sb.shutdown()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 
 if TYPE_CHECKING:
-    from bec_lib import DeviceManagerBase
+    from bec_lib.devicemanager import DeviceManagerBase
     from bec_server.file_writer.file_writer import HDF5Storage
 
 
 def get_entry(data: dict, name: str, default=None) -> Any:
     """
     Get an entry from the scan data assuming a <device>.<device>.value structure.
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/bec_emitter.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/bec_emitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from bec_lib import MessageEndpoints, bec_logger, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 
 from .emitter import EmitterBase
 
 logger = bec_logger.logger
 
 if TYPE_CHECKING:
     from .scan_bundler import ScanBundler
@@ -38,14 +40,29 @@
             },
         )
         self.add_message(
             msg,
             MessageEndpoints.scan_segment(),
             MessageEndpoints.public_scan_segment(scan_id=scan_id, point_id=point_id),
         )
+        self._update_scan_progress(scan_id, point_id)
+
+    def _update_scan_progress(self, scan_id: str, point_id: int, done=False) -> None:
+        info = self.scan_bundler.sync_storage[scan_id]["info"]
+        msg = messages.ProgressMessage(
+            value=point_id + 1,
+            max_value=info.get("num_points", point_id + 1),
+            done=done,
+            metadata={
+                "scan_id": scan_id,
+                "RID": info.get("RID", ""),
+                "queue_id": info.get("queue_id", ""),
+            },
+        )
+        self.scan_bundler.connector.set_and_publish(MessageEndpoints.scan_progress(), msg)
 
     def _send_baseline(self, scan_id: str) -> None:
         sb = self.scan_bundler
 
         msg = messages.ScanBaselineMessage(
             scan_id=scan_id,
             data=sb.sync_storage[scan_id]["baseline"],
@@ -53,7 +70,13 @@
         )
         pipe = sb.connector.pipeline()
         sb.connector.set(
             MessageEndpoints.public_scan_baseline(scan_id=scan_id), msg, expire=1800, pipe=pipe
         )
         sb.connector.set_and_publish(MessageEndpoints.scan_baseline(), msg, pipe=pipe)
         pipe.execute()
+
+    def on_scan_status_update(self, status_msg: messages.ScanStatusMessage):
+        if status_msg.status == "open":
+            return
+        num_points = status_msg.info.get("num_points", 0) - 1
+        self._update_scan_progress(status_msg.scan_id, num_points, done=True)
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import time
 import uuid
 from typing import TYPE_CHECKING
 
 import msgpack
 
-from bec_lib import MessageEndpoints, bec_logger
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 
 from .emitter import EmitterBase
 
 logger = bec_logger.logger
 
 if TYPE_CHECKING:
     from .scan_bundler import ScanBundler
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/emitter.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/emitter.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,12 +58,15 @@
 
     def on_baseline_emit(self, scan_id: str):
         pass
 
     def on_cleanup(self, scan_id: str):
         pass
 
+    def on_scan_status_update(self, status_msg: messages.ScanStatusMessage):
+        pass
+
     def shutdown(self):
         if self._buffered_connector_thread:
             self._buffered_publisher_stop_event.set()
             self._buffered_connector_thread.join()
             self._buffered_connector_thread = None
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/scan_bundler.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_bundler/scan_bundler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import collections
 import threading
 import time
 import traceback
 from collections.abc import Callable
 from concurrent.futures import ThreadPoolExecutor
 
-from bec_lib import BECService, BECStatus, DeviceManagerBase, MessageEndpoints, bec_logger, messages
+from bec_lib import messages
+from bec_lib.bec_service import BECService
 from bec_lib.connector import ConnectorBase
+from bec_lib.devicemanager import DeviceManagerBase
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 
 from .bec_emitter import BECEmitter
 from .bluesky_emitter import BlueskyEmitter
 
 logger = bec_logger.logger
 
 
@@ -48,15 +52,15 @@
         self.current_queue = None
         self.executor = ThreadPoolExecutor(max_workers=4)
         self.executor_tasks = collections.deque(maxlen=100)
         self.scan_id_history = collections.deque(maxlen=10)
         self._lock = threading.Lock()
         self._emitter = []
         self._initialize_emitters()
-        self.status = BECStatus.RUNNING
+        self.status = messages.BECStatus.RUNNING
 
     def _initialize_emitters(self):
         self._emitter = [BECEmitter(self), BlueskyEmitter(self)]
 
     def run_emitter(self, emitter_method: Callable, *args, **kwargs):
         for emi in self._emitter:
             try:
@@ -94,23 +98,23 @@
         logger.info(f"Received new scan status: {msg}")
         scan_id = msg.content["scan_id"]
         self.cleanup_storage()
         if scan_id not in self.sync_storage:
             self._initialize_scan_container(msg)
             if scan_id not in self.scan_id_history:
                 self.scan_id_history.append(scan_id)
+        self.run_emitter("on_scan_status_update", msg)
         if msg.content.get("status") != "open":
             self._scan_status_modification(msg)
 
     def _scan_status_modification(self, msg: messages.ScanStatusMessage):
         status = msg.content.get("status")
         if status not in ["closed", "aborted", "paused", "halted"]:
             logger.error(f"Unknown scan status {status}")
             return
-
         scan_id = msg.content.get("scan_id")
         if not scan_id:
             logger.warning(f"Received scan status update without scan_id: {msg}")
             return
         if self.sync_storage.get(scan_id):
             self.sync_storage[scan_id]["status"] = status
         else:
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/cli/launch.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/cli/launch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-# Description: Launch the scan bundler.
-# This script is the entry point for the Scan Bundler. It is called either
-# by the bec-scan-bundler entry point or directly from the command line.
+# This file is the entry point for the Scan Server.
+# It is called either by the bec-scan-server entry point or directly from the command line.
+
 import argparse
 import threading
 
-from bec_lib import RedisConnector, ServiceConfig, bec_logger
-from bec_server import scan_bundler
+from bec_lib.logger import bec_logger
+from bec_lib.redis_connector import RedisConnector
+from bec_lib.service_config import ServiceConfig
+from bec_server import scan_server
 
 logger = bec_logger.logger
 bec_logger.level = bec_logger.LOGLEVEL.INFO
 
 
 def main():
     """
-    Launch the scan bundler.
+    Launch the scan server.
     """
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("--config", default="", help="path to the config file")
     clargs = parser.parse_args()
     config_path = clargs.config
 
     config = ServiceConfig(config_path)
 
-    sb = scan_bundler.ScanBundler(config, RedisConnector)
-
+    bec_server = scan_server.scan_server.ScanServer(config=config, connector_cls=RedisConnector)
     try:
         event = threading.Event()
-        logger.success("Started ScanBundler")
+        # pylint: disable=E1102
+        logger.success("Started ScanServer")
         event.wait()
-    except KeyboardInterrupt:
-        sb.shutdown()
+    except KeyboardInterrupt as e:
+        bec_server.shutdown()
+        event.set()
+        raise e
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/device_validation.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/device_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from collections.abc import Callable
 
-from bec_lib import DeviceStatus, MessageEndpoints, bec_logger, messages
+from bec_lib import messages
+from bec_lib.device import DeviceStatus
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 
 logger = bec_logger.logger
 
 
 class DeviceValidation:
     """
     Mixin class for validation methods
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/path_optimization.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_assembler.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_assembler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import traceback
 
-from bec_lib import bec_logger, messages
+from bec_lib import messages
+from bec_lib.logger import bec_logger
 
 from .errors import ScanAbortion
 from .scans import RequestBase, unpack_scan_args
 
 logger = bec_logger.logger
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_guard.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_guard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import traceback
 
-from bec_lib import MessageEndpoints, bec_logger, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 
 logger = bec_logger.logger
 
 
 class ScanRejection(Exception):
     pass
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_manager.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import inspect
 
-from bec_lib import MessageEndpoints, bec_logger, plugin_helper
+from bec_lib import plugin_helper
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 from bec_lib.messages import AvailableResourceMessage
 from bec_lib.signature_serializer import signature_to_dict
 
 from . import scans as ScanServerScans
 
 logger = bec_logger.logger
 
@@ -71,15 +73,14 @@
             self.scan_dict[scan_cls.__name__] = scan_cls
             self.available_scans[scan_cls.scan_name] = {
                 "class": scan_cls.__name__,
                 "base_class": base_cls,
                 "arg_input": scan_cls.arg_input,
                 "required_kwargs": scan_cls.required_kwargs,
                 "arg_bundle_size": scan_cls.arg_bundle_size,
-                "scan_report_hint": scan_cls.scan_report_hint,
                 "doc": scan_cls.__doc__ or scan_cls.__init__.__doc__,
                 "signature": signature_to_dict(scan_cls.__init__),
             }
 
     def publish_available_scans(self):
         """send all available scans to the broker"""
         self.parent.connector.set(
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_queue.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 import traceback
 import uuid
 from enum import Enum
 
 from rich.console import Console
 from rich.table import Table
 
-from bec_lib import Alarms, MessageEndpoints, bec_logger, messages, threadlocked
+from bec_lib import messages
+from bec_lib.alarm_handler import Alarms
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 
 from .errors import LimitError, ScanAbortion
 from .scan_assembler import ScanAssembler
 from .scans import ScanBase
 
 logger = bec_logger.logger
 
@@ -80,27 +83,27 @@
                 severity=Alarms.MAJOR,
                 source=msg.content,
                 msg=content,
                 alarm_type=exc.__class__.__name__,
                 metadata=msg.metadata,
             )
 
-    @threadlocked
     def add_queue(self, queue_name: str) -> None:
         """add a new queue to the queue manager"""
-        if queue_name in self.queues:
-            queue = self.queues[queue_name]
-            if not queue.scan_worker.is_alive():
-                logger.info(f"Restarting worker for queue {queue_name}")
-                queue.clear()
-                self.queues[queue_name] = ScanQueue(self, queue_name=queue_name)
-                self.queues[queue_name].start_worker()
-            return
-        self.queues[queue_name] = ScanQueue(self, queue_name=queue_name)
-        self.queues[queue_name].start_worker()
+        with self._lock:
+            if queue_name in self.queues:
+                queue = self.queues[queue_name]
+                if not queue.scan_worker.is_alive():
+                    logger.info(f"Restarting worker for queue {queue_name}")
+                    queue.clear()
+                    self.queues[queue_name] = ScanQueue(self, queue_name=queue_name)
+                    self.queues[queue_name].start_worker()
+                return
+            self.queues[queue_name] = ScanQueue(self, queue_name=queue_name)
+            self.queues[queue_name].start_worker()
 
     def _start_scan_queue_register(self) -> None:
         self.connector.register(
             MessageEndpoints.scan_queue_insert(), cb=self._scan_queue_callback, parent=self
         )
         self.connector.register(
             MessageEndpoints.scan_queue_modification(),
@@ -121,29 +124,29 @@
     def _scan_queue_modification_callback(msg, parent, **_kwargs):
         scan_mod_msg = msg.value
         logger.info(f"Receiving scan modification: {scan_mod_msg.content}")
         if scan_mod_msg:
             parent.scan_interception(scan_mod_msg)
             parent.send_queue_status()
 
-    @threadlocked
     def scan_interception(self, scan_mod_msg: messages.ScanQueueModificationMessage) -> None:
         """handle a scan interception by compiling the requested method name and forwarding the request.
 
         Args:
             scan_mod_msg (messages.ScanQueueModificationMessage): ScanQueueModificationMessage
 
         """
-        logger.info(f"Scan interception: {scan_mod_msg}")
-        action = scan_mod_msg.content["action"]
-        parameter = scan_mod_msg.content["parameter"]
-        queue = scan_mod_msg.content.get("queue", "primary")
-        getattr(self, f"set_{action}")(
-            scan_id=scan_mod_msg.content["scan_id"], queue=queue, parameter=parameter
-        )
+        with self._lock:
+            logger.info(f"Scan interception: {scan_mod_msg}")
+            action = scan_mod_msg.content["action"]
+            parameter = scan_mod_msg.content["parameter"]
+            queue = scan_mod_msg.content.get("queue", "primary")
+            getattr(self, f"set_{action}")(
+                scan_id=scan_mod_msg.content["scan_id"], queue=queue, parameter=parameter
+            )
 
     @requires_queue
     def set_pause(self, scan_id=None, queue="primary", parameter: dict = None) -> None:
         # pylint: disable=unused-argument
         """pause the queue and the currenlty running instruction queue"""
         que = self.queues[queue]
         with AutoResetCM(que):
@@ -242,27 +245,27 @@
                 continue
 
             if len(self.queues[queue].queue) > 0 and scan_id in self.queues[queue].queue[0].scan_id:
                 time.sleep(0.1)
                 continue
             return history[-1]
 
-    @threadlocked
     def send_queue_status(self) -> None:
         """send the current queue to redis"""
-        queue_export = self.export_queue()
-        if not queue_export:
-            return
-        logger.info("New scan queue:")
-        for queue in self.describe_queue():
-            logger.info(f"\n {queue}")
-        self.connector.set_and_publish(
-            MessageEndpoints.scan_queue_status(),
-            messages.ScanQueueStatusMessage(queue=queue_export),
-        )
+        with self._lock:
+            queue_export = self.export_queue()
+            if not queue_export:
+                return
+            logger.info("New scan queue:")
+            for queue in self.describe_queue():
+                logger.info(f"\n {queue}")
+            self.connector.set_and_publish(
+                MessageEndpoints.scan_queue_status(),
+                messages.ScanQueueStatusMessage(queue=queue_export),
+            )
 
     def describe_queue(self) -> list:
         """create a rich.table description of the current scan queue"""
         queue_tables = []
         console = Console()
         for queue_name, scan_queue in self.queues.items():
             table = Table(title=f"{queue_name} queue / {scan_queue.status}")
@@ -407,54 +410,54 @@
 
     def __next__(self):
         while not self.signal_event.is_set():
             updated = self._next_instruction_queue()
             if updated:
                 return self.active_instruction_queue
 
-    @threadlocked
     def _next_instruction_queue(self) -> bool:
         """get the next instruction queue from the queue. If no update is available, it will return False."""
-        try:
-            aiq = self.active_instruction_queue
-            if (
-                aiq is not None
-                and len(self.queue) > 0
-                and self.queue[0].status != InstructionQueueStatus.PENDING
-            ):
-                logger.info(f"Removing queue item {self.queue[0].describe()} from queue")
-                self.queue.popleft()
-                self.queue_manager.send_queue_status()
-
-            if self.status != ScanQueueStatus.PAUSED:
-                if len(self.queue) == 0:
-                    if aiq is None:
-                        time.sleep(0.1)
+        with self._lock:
+            try:
+                aiq = self.active_instruction_queue
+                if (
+                    aiq is not None
+                    and len(self.queue) > 0
+                    and self.queue[0].status != InstructionQueueStatus.PENDING
+                ):
+                    logger.info(f"Removing queue item {self.queue[0].describe()} from queue")
+                    self.queue.popleft()
+                    self.queue_manager.send_queue_status()
+
+                if self.status != ScanQueueStatus.PAUSED:
+                    if len(self.queue) == 0:
+                        if aiq is None:
+                            time.sleep(0.1)
+                            return False
+                        self.active_instruction_queue = None
+                        time.sleep(0.01)
                         return False
-                    self.active_instruction_queue = None
-                    time.sleep(0.01)
-                    return False
+
+                    self.active_instruction_queue = self.queue[0]
+                    self.history_queue.append(self.active_instruction_queue)
+                    return True
+
+                while self.status == ScanQueueStatus.PAUSED and not self.signal_event.is_set():
+                    if len(self.queue) == 0 and self.auto_reset_enabled:
+                        # we don't need to pause if there is no scan enqueued
+                        self.status = ScanQueueStatus.RUNNING
+                        logger.info("resetting queue status to running")
+                    time.sleep(0.1)
 
                 self.active_instruction_queue = self.queue[0]
                 self.history_queue.append(self.active_instruction_queue)
                 return True
-
-            while self.status == ScanQueueStatus.PAUSED and not self.signal_event.is_set():
-                if len(self.queue) == 0 and self.auto_reset_enabled:
-                    # we don't need to pause if there is no scan enqueued
-                    self.status = ScanQueueStatus.RUNNING
-                    logger.info("resetting queue status to running")
-                time.sleep(0.1)
-
-            self.active_instruction_queue = self.queue[0]
-            self.history_queue.append(self.active_instruction_queue)
-            return True
-        except IndexError:
-            time.sleep(0.01)
-        return False
+            except IndexError:
+                time.sleep(0.01)
+            return False
 
     def insert(self, msg: messages.ScanQueueMessage, position=-1, **_kwargs):
         """insert a new message to the queue"""
         while self.worker_status == InstructionQueueStatus.STOPPED:
             logger.info("Waiting for worker to become active.")
             time.sleep(0.1)
         target_group = msg.metadata.get("queue_group")
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_server.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from __future__ import annotations
 
-from bec_lib import Alarms, BECService, BECStatus
-from bec_lib import DeviceManagerBase as DeviceManager
-from bec_lib import MessageEndpoints, ServiceConfig, bec_logger, messages
+from bec_lib import messages
+from bec_lib.alarm_handler import Alarms
+from bec_lib.bec_service import BECService
 from bec_lib.connector import ConnectorBase
+from bec_lib.devicemanager import DeviceManagerBase as DeviceManager
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
+from bec_lib.service_config import ServiceConfig
 
 from .scan_assembler import ScanAssembler
 from .scan_guard import ScanGuard
 from .scan_manager import ScanManager
 from .scan_queue import QueueManager
 
 logger = bec_logger.logger
@@ -27,15 +31,15 @@
         self._start_queue_manager()
         self._start_device_manager()
         self._start_scan_guard()
         self._start_scan_assembler()
         # self._start_scan_server()
         self._start_alarm_handler()
         self._reset_scan_number()
-        self.status = BECStatus.RUNNING
+        self.status = messages.BECStatus.RUNNING
 
     def _start_device_manager(self):
         self.wait_for_service("DeviceServer")
         self.device_manager = DeviceManager(self)
         self.device_manager.initialize([self.bootstrap_server])
 
     def _start_scan_manager(self):
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_stubs.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_stubs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,39 @@
+"""
+Scan stubs are commands that can be used to control devices during a scan. They typically yield device messages that are
+consumed by the scan worker and potentially forwarded to the device server.
+"""
+
 from __future__ import annotations
 
 import threading
 import time
 import uuid
 from collections.abc import Callable
 from typing import Generator, Literal
 
 import numpy as np
 
-from bec_lib import MessageEndpoints, Status, bec_logger, messages
+from bec_lib import messages
 from bec_lib.connector import ConnectorBase
+from bec_lib.device import Status
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 
 from .errors import DeviceMessageError, ScanAbortion
 
 logger = bec_logger.logger
 
 
 class ScanStubs:
+    """
+    Scan stubs are commands that can be used to control devices during a scan. They typically yield device messages that are
+    consumed by the scan worker and potentially forwarded to the device server.
+    """
+
     def __init__(
         self,
         connector: ConnectorBase,
         device_msg_callback: Callable = None,
         shutdown_event: threading.Event = None,
     ) -> None:
         self.connector = connector
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_worker.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import datetime
 import threading
 import time
 import traceback
 
-from bec_lib import Alarms, DeviceBase, MessageEndpoints, bec_logger, messages
+from bec_lib import messages
+from bec_lib.alarm_handler import Alarms
+from bec_lib.device import DeviceBase
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 
 from .device_validation import DeviceValidation
 from .errors import DeviceMessageError, ScanAbortion
 from .scan_queue import InstructionQueueItem, InstructionQueueStatus, RequestBlock
 
 logger = bec_logger.logger
 
@@ -66,19 +70,19 @@
         if self.max_point_id:
             num_points += 1
 
         active_rb = self.current_instruction_queue_item.active_request_block
 
         self._initialize_scan_info(active_rb, instr, num_points)
 
-        # only append the table_wait if the scan is not using scan_progress
+        # only append the scan_progress if the scan is not using device_progress
         if not self.scan_report_instructions or not self.scan_report_instructions[-1].get(
-            "scan_progress"
+            "device_progress"
         ):
-            self.scan_report_instructions.append({"table_wait": num_points})
+            self.scan_report_instructions.append({"scan_progress": num_points})
         self.current_instruction_queue_item.parent.queue_manager.send_queue_status()
 
         self._send_scan_status("open")
 
     def close_scan(self, instr: messages.DeviceInstructionMessage, max_point_id: int) -> None:
         """
         Close a scan and emit a scan status message.
@@ -647,15 +651,14 @@
                 "scan_number": self.parent.scan_number,
                 "dataset_number": self.parent.dataset_number,
                 "exp_time": self._exposure_time,
                 "frames_per_trigger": active_rb.scan.frames_per_trigger,
                 "settling_time": active_rb.scan.settling_time,
                 "readout_time": active_rb.scan.readout_time,
                 "acquisition_config": active_rb.scan.acquisition_config,
-                "scan_report_hint": active_rb.scan.scan_report_hint,
                 "scan_report_devices": active_rb.scan.scan_report_devices,
                 "monitor_sync": active_rb.scan.monitor_sync,
                 "num_points": num_points,
             }
         )
         self.current_scan_info["scan_msgs"] = [
             str(scan_msg) for scan_msg in self.current_instruction_queue_item.scan_msgs
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scans.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scans.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import threading
 import time
 from abc import ABC, abstractmethod
 from typing import Any, Literal
 
 import numpy as np
 
-from bec_lib import DeviceManagerBase, MessageEndpoints, bec_logger
+from bec_lib.devicemanager import DeviceManagerBase
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 
 from .errors import LimitError, ScanAbortion
 from .path_optimization import PathOptimizerMixin
 from .scan_stubs import ScanStubs
 
 logger = bec_logger.logger
 
@@ -174,15 +176,14 @@
 
 class RequestBase(ABC):
     """
     Base class for all scan requests.
     """
 
     scan_name = ""
-    scan_report_hint = None
     arg_input = {"device": ScanArgType.DEVICE}
     arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": None}
     required_kwargs = []
     return_to_start_after_abort = False
 
     def __init__(
         self,
@@ -312,40 +313,34 @@
     11. cleanup
 
     A subclass of ScanBase must implement the following methods:
     - _calculate_positions
 
     Attributes:
         scan_name (str): name of the scan
-        scan_report_hint (str): hint for the scan report
         scan_type (str): scan type. Can be "step" or "fly"
         arg_input (list): list of scan argument types
         arg_bundle_size (dict):
             - bundle: number of arguments that are bundled together
             - min: minimum number of bundles
             - max: maximum number of bundles
         required_kwargs (list): list of required kwargs
         return_to_start_after_abort (bool): if True, the scan will return to the start position after an abort
     """
 
     scan_name = ""
-    scan_report_hint = None
     scan_type = "step"
     arg_input = {"device": ScanArgType.DEVICE}
     arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": None}
     required_kwargs = ["required"]
     return_to_start_after_abort = True
 
     # perform pre-move action before the pre_scan trigger is sent
     pre_move = True
 
-    # # synchronize primary readings with the scan motor readings. Set to False if the master device
-    # # does not provide single readouts or are too fast to be synchronized with primary readings
-    # enforce_sync = True
-
     def __init__(
         self,
         *args,
         device_manager: DeviceManagerBase = None,
         parameter: dict = None,
         exp_time: float = 0,
         readout_time: float = 0,
@@ -465,15 +460,15 @@
         for ind, pos in self._get_position():
             for self.burst_index in range(self.burst_at_each_point):
                 yield from self._at_each_point(ind, pos)
             self.burst_index = 0
 
     def return_to_start(self):
         """return to the start position"""
-        yield from self._move_and_wait(self.start_pos)
+        yield from self._move_scan_motors_and_wait(self.start_pos)
 
     def finalize(self):
         """finalize the scan"""
         yield from self.return_to_start()
         yield from self.stubs.wait(wait_type="read", group="primary", wait_group="readout_primary")
         yield from self.stubs.complete(device=None)
 
@@ -482,15 +477,15 @@
         yield from self.stubs.unstage()
 
     def cleanup(self):
         """call the cleanup procedure"""
         yield from self.close_scan()
 
     def _at_each_point(self, ind=None, pos=None):
-        yield from self._move_and_wait(pos)
+        yield from self._move_scan_motors_and_wait(pos)
         if ind > 0:
             yield from self.stubs.wait(
                 wait_type="read", group="primary", wait_group="readout_primary"
             )
         time.sleep(self.settling_time)
         yield from self.stubs.trigger(group="trigger", point_id=self.point_id)
         yield from self.stubs.wait(wait_type="trigger", group="trigger", wait_time=self.exp_time)
@@ -499,15 +494,15 @@
         )
         yield from self.stubs.wait(
             wait_type="read", group="scan_motor", wait_group="readout_primary"
         )
 
         self.point_id += 1
 
-    def _move_and_wait(self, pos):
+    def _move_scan_motors_and_wait(self, pos):
         if not isinstance(pos, list) and not isinstance(pos, np.ndarray):
             pos = [pos]
         if len(pos) == 0:
             return
         for ind, val in enumerate(self.scan_motors):
             yield from self.stubs.set(device=val, value=pos[ind], wait_group="scan_motor")
 
@@ -522,15 +517,15 @@
 
     def pre_scan(self):
         """
         pre scan procedure. This method is called before the scan_core method and can be used to
         perform additional tasks before the scan is started. This
         """
         if self.pre_move and len(self.positions) > 0:
-            yield from self._move_and_wait(self.positions[0])
+            yield from self._move_scan_motors_and_wait(self.positions[0])
         yield from self.stubs.pre_scan()
 
     def run(self):
         """run the scan. This method is called by the scan server and is the main entry point for the scan."""
         self.initialize()
         yield from self.read_scan_motors()
         yield from self.prepare_positions()
@@ -627,25 +622,23 @@
 
 class ScanStub(RequestBase):
     pass
 
 
 class OpenScanDef(ScanStub):
     scan_name = "open_scan_def"
-    scan_report_hint = None
     arg_input = {}
     arg_bundle_size = {"bundle": len(arg_input), "min": 0, "max": 0}
 
     def run(self):
         yield from self.stubs.open_scan_def()
 
 
 class CloseScanDef(ScanStub):
     scan_name = "close_scan_def"
-    scan_report_hint = "table"
     arg_input = {}
     arg_bundle_size = {"bundle": len(arg_input), "min": 0, "max": 0}
 
     def run(self):
         yield from self.stubs.close_scan_def()
 
 
@@ -658,29 +651,27 @@
         yield from self.stubs.close_scan_group()
 
 
 class DeviceRPC(ScanStub):
     scan_name = "device_rpc"
     arg_input = [ScanArgType.DEVICE, ScanArgType.STR, ScanArgType.LIST, ScanArgType.DICT]
     arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": 1}
-    scan_report_hint = None
 
     def _get_scan_motors(self):
         pass
 
     def run(self):
         # different to calling self.device_rpc, this procedure will not wait for a reply and therefore not check any errors.
         yield from self.stubs.rpc(device=self.parameter.get("device"), parameter=self.parameter)
 
 
 class Move(RequestBase):
     scan_name = "mv"
     arg_input = {"device": ScanArgType.DEVICE, "target": ScanArgType.FLOAT}
     arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": None}
-    scan_report_hint = None
     required_kwargs = ["relative"]
 
     def __init__(self, *args, relative=False, **kwargs):
         """
         Move device(s) to an absolute position
         Args:
             *args (Device, float): pairs of device / position arguments
@@ -722,27 +713,15 @@
 
     def prepare_positions(self):
         self._calculate_positions()
         yield from self._set_position_offset()
         self._check_limits()
 
     def scan_report_instructions(self):
-        if not self.scan_report_hint:
-            yield None
-            return
-        yield from self.stubs.scan_report_instruction(
-            {
-                "readback": {
-                    "RID": self.metadata["RID"],
-                    "devices": self.scan_motors,
-                    "start": self.start_pos,
-                    "end": self.positions[0],
-                }
-            }
-        )
+        yield None
 
     def run(self):
         self.initialize()
         yield from self.prepare_positions()
         yield from self.scan_report_instructions()
         yield from self._at_each_point()
 
@@ -758,29 +737,39 @@
         ScanReport
 
     Examples:
         >>> scans.umv(dev.samx, 1, dev.samy,2)
     """
 
     scan_name = "umv"
-    scan_report_hint = "readback"
 
     def _at_each_point(self, pos=None):
         for ii, motor in enumerate(self.scan_motors):
             yield from self.stubs.set(
                 device=motor, value=self.positions[0][ii], wait_group="scan_motor"
             )
 
         for motor in self.scan_motors:
             yield from self.stubs.wait(wait_type="move", device=motor, wait_group="scan_motor")
 
+    def scan_report_instructions(self):
+        yield from self.stubs.scan_report_instruction(
+            {
+                "readback": {
+                    "RID": self.metadata["RID"],
+                    "devices": self.scan_motors,
+                    "start": self.start_pos,
+                    "end": self.positions[0],
+                }
+            }
+        )
+
 
 class Scan(ScanBase):
     scan_name = "grid_scan"
-    scan_report_hint = "table"
     arg_input = {
         "device": ScanArgType.DEVICE,
         "start": ScanArgType.FLOAT,
         "stop": ScanArgType.FLOAT,
         "steps": ScanArgType.INT,
     }
     arg_bundle_size = {"bundle": len(arg_input), "min": 2, "max": None}
@@ -826,15 +815,14 @@
             self.positions = get_2D_raster_pos(self.axis)
         else:
             self.positions = np.vstack(tuple(self.axis)).T
 
 
 class FermatSpiralScan(ScanBase):
     scan_name = "fermat_scan"
-    scan_report_hint = "table"
     required_kwargs = ["step", "relative"]
     arg_input = {
         "device": ScanArgType.DEVICE,
         "start": ScanArgType.FLOAT,
         "stop": ScanArgType.FLOAT,
     }
     arg_bundle_size = {"bundle": len(arg_input), "min": 2, "max": 2}
@@ -892,15 +880,14 @@
             spiral_type=self.spiral_type,
             center=False,
         )
 
 
 class RoundScan(ScanBase):
     scan_name = "round_scan"
-    scan_report_hint = "table"
     required_kwargs = ["relative"]
     arg_input = {
         "motor_1": ScanArgType.DEVICE,
         "motor_2": ScanArgType.DEVICE,
         "inner_ring": ScanArgType.FLOAT,
         "outer_ring": ScanArgType.FLOAT,
         "number_of_rings": ScanArgType.INT,
@@ -950,15 +937,14 @@
         self.positions = get_round_scan_positions(
             r_in=params[1], r_out=params[2], nr=params[3], nth=params[4]
         )
 
 
 class ContLineScan(ScanBase):
     scan_name = "cont_line_scan"
-    scan_report_hint = "table"
     required_kwargs = ["steps", "relative"]
     arg_input = {
         "device": ScanArgType.DEVICE,
         "start": ScanArgType.FLOAT,
         "stop": ScanArgType.FLOAT,
     }
     arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": 1}
@@ -1008,15 +994,15 @@
 
     def _at_each_point(self):
         yield from self.stubs.trigger(group="trigger", point_id=self.point_id)
         yield from self.stubs.read(group="primary", wait_group="primary", point_id=self.point_id)
         self.point_id += 1
 
     def scan_core(self):
-        yield from self._move_and_wait(self.positions[0] - self.offset)
+        yield from self._move_scan_motors_and_wait(self.positions[0] - self.offset)
         # send the slow motor on its way
         yield from self.stubs.set(
             device=self.scan_motors[0], value=self.positions[-1][0], wait_group="scan_motor"
         )
 
         while self.point_id < len(self.positions[:]):
             cont_motor_positions = self.device_manager.devices[self.scan_motors[0]].readback()
@@ -1032,15 +1018,14 @@
                 continue
             if cont_motor_positions > self.positions[self.point_id][0]:
                 raise ScanAbortion(f"Skipped point {self.point_id + 1}")
 
 
 class RoundScanFlySim(SyncFlyScanBase):
     scan_name = "round_scan_fly"
-    scan_report_hint = "table"
     scan_type = "fly"
     pre_move = False
     required_kwargs = ["relative"]
     arg_input = {
         "flyer": ScanArgType.DEVICE,
         "inner_ring": ScanArgType.FLOAT,
         "outer_ring": ScanArgType.FLOAT,
@@ -1114,15 +1099,14 @@
 
             time.sleep(1)
             logger.debug("reading monitors")
 
 
 class RoundROIScan(ScanBase):
     scan_name = "round_roi_scan"
-    scan_report_hint = "table"
     required_kwargs = ["dr", "nth", "relative"]
     arg_input = {
         "motor_1": ScanArgType.DEVICE,
         "motor_2": ScanArgType.DEVICE,
         "width_1": ScanArgType.FLOAT,
         "width_2": ScanArgType.FLOAT,
     }
@@ -1169,15 +1153,14 @@
         self.positions = get_round_roi_scan_positions(
             lx=params[0][0], ly=params[1][0], dr=self.dr, nth=self.nth
         )
 
 
 class ListScan(ScanBase):
     scan_name = "list_scan"
-    scan_report_hint = "table"
     required_kwargs = ["relative"]
     arg_input = {"device": ScanArgType.DEVICE, "positions": ScanArgType.LIST}
     arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": None}
 
     def __init__(self, *args, parameter: dict = None, **kwargs):
         """
         A scan following the positions specified in a list.
@@ -1202,15 +1185,14 @@
 
     def _calculate_positions(self):
         self.positions = np.vstack(tuple(self.caller_args.values())).T.tolist()
 
 
 class TimeScan(ScanBase):
     scan_name = "time_scan"
-    scan_report_hint = "table"
     required_kwargs = ["points", "interval"]
     arg_input = {}
     arg_bundle_size = {"bundle": len(arg_input), "min": None, "max": None}
 
     def __init__(
         self,
         points: int,
@@ -1269,15 +1251,14 @@
     def scan_core(self):
         for ind in range(self.num_pos):
             yield from self._at_each_point(ind)
 
 
 class MonitorScan(ScanBase):
     scan_name = "monitor_scan"
-    scan_report_hint = "table"
     required_kwargs = ["relative"]
     arg_input = {
         "device": ScanArgType.DEVICE,
         "start": ScanArgType.FLOAT,
         "stop": ScanArgType.FLOAT,
     }
     arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": 1}
@@ -1361,15 +1342,14 @@
             )
             self.point_id += 1
             self.num_pos += 1
 
 
 class Acquire(ScanBase):
     scan_name = "acquire"
-    scan_report_hint = "table"
     required_kwargs = []
     arg_input = {}
     arg_bundle_size = {"bundle": len(arg_input), "min": None, "max": None}
 
     def __init__(self, *args, exp_time: float = 0, burst_at_each_point: int = 1, **kwargs):
         """
         A simple acquisition at the current position.
@@ -1423,15 +1403,14 @@
         yield from self.finalize()
         yield from self.unstage()
         yield from self.cleanup()
 
 
 class LineScan(ScanBase):
     scan_name = "line_scan"
-    scan_report_hint = "table"
     required_kwargs = ["steps", "relative"]
     arg_input = {
         "device": ScanArgType.DEVICE,
         "start": ScanArgType.FLOAT,
         "stop": ScanArgType.FLOAT,
     }
     arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": None}
@@ -1478,15 +1457,14 @@
 
 class ScanComponent(ScanBase):
     pass
 
 
 class OpenInteractiveScan(ScanComponent):
     scan_name = "open_interactive_scan"
-    scan_report_hint = ""
     required_kwargs = []
     arg_input = {"device": ScanArgType.DEVICE}
     arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": None}
 
     def __init__(self, *args, **kwargs):
         """
         An interactive scan for one or more motors.
@@ -1522,15 +1500,14 @@
         yield from self.open_scan()
         yield from self.stage()
         yield from self.run_baseline_reading()
 
 
 class AddInteractiveScanPoint(ScanComponent):
     scan_name = "interactive_scan_trigger"
-    scan_report_hint = ""
     arg_input = {"device": ScanArgType.DEVICE}
     arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": None}
 
     def __init__(self, *args, **kwargs):
         """
         An interactive scan for one or more motors.
 
@@ -1569,15 +1546,14 @@
         yield from self.open_scan()
         yield from self._at_each_point()
         yield from self.close_scan()
 
 
 class CloseInteractiveScan(ScanComponent):
     scan_name = "close_interactive_scan"
-    scan_report_hint = ""
     arg_input = {}
     arg_bundle_size = {"bundle": len(arg_input), "min": None, "max": None}
 
     def __init__(self, *args, **kwargs):
         """
         An interactive scan for one or more motors.
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/cli/launch.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/cli/launch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-# This file is the entry point for the Scan Server.
-# It is called either by the bec-scan-server entry point or directly from the command line.
-
+# Description: Launch the SciHub connector.
+# This script is the entry point for the SciHub connector. It is called either
+# by the bec-dap entry point or directly from the command line.
 import argparse
 import threading
 
-from bec_lib import RedisConnector, ServiceConfig, bec_logger
-from bec_server import scan_server
+from bec_lib.logger import bec_logger
+from bec_lib.redis_connector import RedisConnector
+from bec_lib.service_config import ServiceConfig
+from bec_server import scihub
 
 logger = bec_logger.logger
 bec_logger.level = bec_logger.LOGLEVEL.INFO
 
 
 def main():
     """
-    Launch the scan server.
+    Launch the SciHub connector.
     """
+
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("--config", default="", help="path to the config file")
     clargs = parser.parse_args()
     config_path = clargs.config
 
     config = ServiceConfig(config_path)
 
-    bec_server = scan_server.scan_server.ScanServer(config=config, connector_cls=RedisConnector)
+    sh = scihub.SciHub(config, RedisConnector)
+
     try:
         event = threading.Event()
-        # pylint: disable=E1102
-        logger.success("Started ScanServer")
+        logger.success("Started SciHub connector")
         event.wait()
-    except KeyboardInterrupt as e:
-        bec_server.shutdown()
-        event.set()
-        raise e
+    except KeyboardInterrupt:
+        sh.shutdown()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import time
 
-from bec_lib import bec_logger
+from bec_lib.logger import bec_logger
 from bec_server.scan_server.scans import ScanArgType, ScanBase, SyncFlyScanBase
 
 logger = bec_logger.logger
 
 
 class OTFScan(SyncFlyScanBase):
     scan_name = "otf_scan"
-    scan_report_hint = "table"
     required_kwargs = ["e1", "e2", "time"]
     arg_input = {}
     arg_bundle_size = {"bundle": len(arg_input), "min": None, "max": None}
 
     def __init__(self, *args, parameter: dict = None, **kwargs):
         """Scans the energy from e1 to e2 in <time> minutes.
 
@@ -62,15 +61,14 @@
             if status:
                 break
             time.sleep(1)
 
 
 class HystScan(ScanBase):
     scan_name = "hyst_scan"
-    scan_report_hint = "table"
     required_kwargs = []
     arg_input = {
         "field_motor": ScanArgType.DEVICE,
         "start_field": ScanArgType.FLOAT,
         "end_field": ScanArgType.FLOAT,
         "mono": ScanArgType.DEVICE,
         "energy1": ScanArgType.FLOAT,
@@ -120,15 +118,15 @@
             if len(self.positions) - 1 == self._current_scan_motor_index or (
                 self._current_scan_motor_index == 0 and self._scan_motor_direction < 0
             ):
                 self._scan_motor_direction *= -1
             self._current_scan_motor_index += self._scan_motor_direction
 
     def scan_core(self):
-        # yield from self._move_and_wait(self.positions[0])
+        # yield from self._move_scan_motors_and_wait(self.positions[0])
         status = yield from self.stubs.send_rpc_and_wait(
             "field_x", "ramprate.set", self.default_ramp_rate
         )
         status.wait()
         yield from self.stubs.set(
             device=self.flyer, value=self.flyer_positions[0], wait_group="flyer"
         )
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/tests/utils.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scan_server/tests/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from bec_lib import ServiceConfig
 from bec_lib.messages import BECStatus
+from bec_lib.service_config import ServiceConfig
 from bec_lib.tests.utils import ConnectorMock
 from bec_server.scan_server.scan_server import ScanServer
 from bec_server.scan_server.scan_worker import InstructionQueueStatus
 
 # pylint: disable=missing-function-docstring
 # pylint: disable=protected-access
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/repeated_timer.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/repeated_timer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scihub.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scihub.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from bec_lib import BECService, BECStatus, ServiceConfig
+from bec_lib import messages
+from bec_lib.bec_service import BECService
 from bec_lib.connector import ConnectorBase
+from bec_lib.service_config import ServiceConfig
 from bec_server.scihub.scibec import SciBecConnector
 from bec_server.scihub.scilog import SciLogConnector
 
 
 class SciHub(BECService):
     def __init__(self, config: ServiceConfig, connector_cls: ConnectorBase) -> None:
         super().__init__(config, connector_cls, unique_service=True)
         self.config = config
         self.scibec_connector = None
         self.scilog_connector = None
         self._start_scibec_connector()
         self._start_scilog_connector()
-        self.status = BECStatus.RUNNING
+        self.status = messages.BECStatus.RUNNING
 
     def _start_scibec_connector(self):
         self.wait_for_service("DeviceServer")
         self.scibec_connector = SciBecConnector(self, self.connector)
 
     def _start_scilog_connector(self):
         self.scilog_connector = SciLogConnector(self, self.connector)
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/config_handler.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/config_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 import os
 import time
 import traceback
 import uuid
 from typing import TYPE_CHECKING
 
 import bec_lib
-from bec_lib import DeviceConfigError
-from bec_lib import DeviceManagerBase as DeviceManager
-from bec_lib import MessageEndpoints, bec_logger, messages
+from bec_lib import messages
+from bec_lib.bec_errors import DeviceConfigError
 from bec_lib.connector import ConnectorBase
+from bec_lib.devicemanager import DeviceManagerBase as DeviceManager
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 from bec_lib.scibec_validator import SciBecValidator
 
 if TYPE_CHECKING:
     from bec_lib.device import DeviceBase
     from bec_server.scihub.scibec.scibec_connector import SciBecConnector
 
 logger = bec_logger.logger
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import os
 from typing import TYPE_CHECKING
 
 import py_scibec
 from dotenv import dotenv_values
 from py_scibec import SciBecCore
 
-from bec_lib import MessageEndpoints, bec_logger, messages
+from bec_lib import messages
 from bec_lib.connector import ConnectorBase
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 from bec_server.scihub.repeated_timer import RepeatedTimer
 
 from .config_handler import ConfigHandler
 from .scibec_metadata_handler import SciBecMetadataHandler
 
 if TYPE_CHECKING:
     from bec_server.scihub import SciHub
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import time
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 import py_scibec
 import py_scibec_openapi_client.models as py_scibec_models
 
-from bec_lib import MessageEndpoints, bec_logger
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 from bec_lib.serialization import json_ext
 
 logger = bec_logger.logger
 
 if TYPE_CHECKING:
     from bec_lib import messages
     from bec_server.scihub.scibec import SciBecConnector
@@ -106,14 +107,15 @@
                     "scanId": info.get("scan_id", ""),
                     "queueId": info.get("queue_id", ""),
                     "requestId": info.get("RID", ""),
                     "exitStatus": msg.content["status"],
                     # "queue": info.get("stream", ""),
                     "metadata": info,
                     # "sessionId": session_id,
+                    "experimentId": experiment_id,
                     "datasetId": dataset.id,
                     "scanNumber": info.get("scan_number", 0),
                 }
             )
             scan = scibec.scan.scan_controller_create(new_scan)
             # scan = scibec.add_scan(scan_data)
         else:
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scilog/scilog.py` & `ophyd_devices-1.0.2/bec/bec_server/bec_server/scihub/scilog/scilog.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 
 import os
 from typing import TYPE_CHECKING
 
 import requests
 from dotenv import dotenv_values
 
-from bec_lib import MessageEndpoints, RedisConnector, bec_logger, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
+from bec_lib.redis_connector import RedisConnector
 from bec_server.scihub.repeated_timer import RepeatedTimer
 
 logger = bec_logger.logger
 
 if TYPE_CHECKING:
     from bec_server.scihub import SciHub
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_bec_server_utils/test_main.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_bec_server_utils/test_main.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/conftest.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from bec_lib import bec_logger
+from bec_lib.logger import bec_logger
 
 ### THE NEXT FIXTURE HAS TO BE RE-ACTIVATED ONCE
 ### OPHYD "STATUS CALLBACKS" THREADS ARE CLEANED
 ### (NEXT OPHYD RELEASE)
 # overwrite threads_check fixture from bec_lib,
 # to have it in autouse
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_config_handler.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_config_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os
 from unittest import mock
 
 import numpy as np
 import pytest
 import yaml
 
-import bec_lib
-from bec_lib import MessageEndpoints, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
 from bec_server.device_server.devices.devicemanager import DeviceManagerDS
 
 # pylint: disable=missing-function-docstring
 # pylint: disable=protected-access
 
 
 class ControllerMock:
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_serializer.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_server.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from unittest import mock
 from unittest.mock import ANY
 
 import pytest
 from ophyd import Staged
 from ophyd.utils import errors as ophyd_errors
 
-from bec_lib import Alarms, MessageEndpoints, ServiceConfig, messages
+from bec_lib import messages
+from bec_lib.alarm_handler import Alarms
+from bec_lib.endpoints import MessageEndpoints
 from bec_lib.messages import BECStatus
 from bec_lib.redis_connector import MessageObject
+from bec_lib.service_config import ServiceConfig
 from bec_lib.tests.utils import ConnectorMock
 from bec_server.device_server import DeviceServer
 from bec_server.device_server.device_server import InvalidDeviceError
 from bec_server.device_server.devices.devicemanager import DeviceManagerDS
 
 # pylint: disable=missing-function-docstring
 # pylint: disable=protected-access
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # pylint: skip-file
 from collections import namedtuple
 from unittest import mock
 
 import pytest
 from ophyd import Device, Kind, Signal, Staged, StatusBase
 
-from bec_lib import Alarms, MessageEndpoints, messages
+from bec_lib import messages
+from bec_lib.alarm_handler import Alarms
+from bec_lib.endpoints import MessageEndpoints
 from bec_server.device_server.rpc_mixin import RPCMixin
 
 
 @pytest.fixture
 def rpc_cls():
     rpc_mixin = RPCMixin()
     rpc_mixin.connector = mock.MagicMock()
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/test_file_writer.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/test_file_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,15 +124,14 @@
                 "num_points": 2,
                 "positions": [[-100], [100]],
                 "scan_name": "monitor_scan",
                 "scan_type": "fly",
                 "scan_number": 88,
                 "dataset_number": 88,
                 "exp_time": 0.1,
-                "scan_report_hint": "table",
                 "scan_report_devices": ["samx"],
                 "scan_msgs": [
                     "ScanQueueMessage(({'scan_type': 'monitor_scan', 'parameter': {'args': {'samx':"
                     " [-100, 100]}, 'kwargs': {'relative': False}}, 'queue': 'primary'}, {'RID':"
                     " '5ee455b8-d0ef-452d-b54a-e7cea5cea19e'})))"
                 ],
             },
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import os
 from unittest import mock
 
 import numpy as np
 import pytest
 
 import bec_lib
-from bec_lib import MessageEndpoints, ServiceConfig, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
 from bec_lib.redis_connector import MessageObject
+from bec_lib.service_config import ServiceConfig
 from bec_lib.tests.utils import ConnectorMock
 from bec_server.file_writer import FileWriterManager
 from bec_server.file_writer.file_writer import FileWriter
 from bec_server.file_writer.file_writer_manager import ScanStorage
 
 # pylint: disable=missing-function-docstring
 # pylint: disable=protected-access
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/conftest.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 from unittest import mock
 
 import pytest
 import yaml
 
 import bec_lib
-from bec_lib import DeviceManagerBase, ServiceConfig, bec_logger, messages
+from bec_lib.devicemanager import DeviceManagerBase
+from bec_lib.logger import bec_logger
 from bec_lib.messages import BECStatus
+from bec_lib.service_config import ServiceConfig
 from bec_lib.tests.utils import ConnectorMock
 from bec_server.scan_bundler import ScanBundler
 
 # overwrite threads_check fixture from bec_lib,
 # to have it in autouse
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from unittest import mock
 
 import pytest
 
-from bec_lib import MessageEndpoints, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
 from bec_server.scan_bundler.bec_emitter import BECEmitter
 
 
 @pytest.fixture
 def bec_emitter_mock(scan_bundler_mock):
     emitter = BECEmitter(scan_bundler_mock)
     yield emitter
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import mock
 
 import msgpack
 import pytest
 
-from bec_lib import MessageEndpoints
+from bec_lib.endpoints import MessageEndpoints
 from bec_server.scan_bundler.bluesky_emitter import BlueskyEmitter
 
 
 @pytest.fixture
 def bls_emitter(scan_bundler_mock):
     emitter = BlueskyEmitter(scan_bundler_mock)
     yield emitter
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_emitter.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from unittest import mock
 
 import pytest
 
-from bec_lib import MessageEndpoints, messages
+from bec_lib import messages
 from bec_lib.connector import MessageObject
+from bec_lib.endpoints import MessageEndpoints
 
 # pylint: disable=missing-function-docstring
 # pylint: disable=protected-access
 
 
 @pytest.fixture()
 def dummy_signal_data():
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_path_optimization.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_path_optimization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_guard.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_guard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from unittest import mock
 
 import pytest
 
-from bec_lib import MessageEndpoints, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
 from bec_lib.redis_connector import MessageObject
 from bec_server.scan_server.scan_guard import ScanGuard, ScanRejection, ScanStatus
 from bec_server.scan_server.tests.fixtures import scan_server_mock
 
 
 @pytest.fixture
 def scan_guard_mock(scan_server_mock):
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import uuid
 from unittest import mock
 
 import pytest
 
-from bec_lib import Alarms, MessageEndpoints, messages
+from bec_lib import messages
+from bec_lib.alarm_handler import Alarms
+from bec_lib.endpoints import MessageEndpoints
 from bec_lib.redis_connector import MessageObject
 from bec_server.scan_server.scan_assembler import ScanAssembler
 from bec_server.scan_server.scan_queue import (
     InstructionQueueItem,
     InstructionQueueStatus,
     QueueManager,
     RequestBlock,
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import threading
 from unittest import mock
 
 import pytest
 
-from bec_lib import MessageEndpoints, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
 from bec_lib.tests.utils import ConnectorMock
 from bec_server.scan_server.errors import DeviceMessageError
 from bec_server.scan_server.scan_stubs import ScanAbortion, ScanStubs
 
 
 @pytest.fixture
 def stubs():
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_worker.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scan_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: skip-file
 import uuid
 from unittest import mock
 
 import pytest
 
-from bec_lib import MessageEndpoints, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
 from bec_lib.tests.utils import ConnectorMock
 from bec_server.scan_server.errors import DeviceMessageError, ScanAbortion
 from bec_server.scan_server.scan_assembler import ScanAssembler
 from bec_server.scan_server.scan_queue import (
     InstructionQueueItem,
     InstructionQueueStatus,
     QueueManager,
@@ -1067,15 +1068,15 @@
                                 worker.device_manager.devices["samy"],
                             ]
                         else:
                             assert worker.scan_id == 111
                             assert worker.scan_motors == ["bpm4i"]
                         init_mock.assert_called_once_with(active_rb, instr, corr_num_points)
                         assert active_rb.scan_report_instructions == [
-                            {"table_wait": corr_num_points}
+                            {"scan_progress": corr_num_points}
                         ]
                         queue_status_mock.assert_called_once()
                         send_mock.assert_called_once_with("open")
 
 
 @pytest.mark.parametrize(
     "msg",
@@ -1104,15 +1105,14 @@
             "on_request": [],
         }
         worker._initialize_scan_info(rb, msg, msg.content["parameter"].get("num_points"))
 
         assert worker.current_scan_info["RID"] == "something"
         assert worker.current_scan_info["scan_number"] == 2
         assert worker.current_scan_info["dataset_number"] == 3
-        assert worker.current_scan_info["scan_report_hint"] == rb.scan.scan_report_hint
         assert worker.current_scan_info["scan_report_devices"] == rb.scan.scan_report_devices
         assert worker.current_scan_info["num_points"] == 100
         assert worker.current_scan_info["scan_msgs"] == []
         assert worker.current_scan_info["monitor_sync"] == "bec"
         assert worker.current_scan_info["frames_per_trigger"] == 1
         assert worker.current_scan_info["args"] == {"samx": (-5, 5, 3)}
         assert worker.current_scan_info["kwargs"] == {}
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scans.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scan_server/test_scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/conftest.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from py_scibec_openapi_client.models.beamline_with_relations import BeamlineWithRelations
 from py_scibec_openapi_client.models.dataset_with_relations import DatasetWithRelations
 from py_scibec_openapi_client.models.experiment_with_relations import ExperimentWithRelations
 from py_scibec_openapi_client.models.scan_with_relations import ScanWithRelations
 
-from bec_lib import bec_logger
+from bec_lib.logger import bec_logger
 
 # overwrite threads_check fixture from bec_lib,
 # to have it in autouse
 
 
 @pytest.fixture(autouse=True)
 def threads_check(threads_check):
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_repeated_timer.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_repeated_timer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 import pytest
 import yaml
 from fastjsonschema import JsonSchemaException
 from test_scibec_connector import SciBecMock, SciHubMock
 
 import bec_lib
-from bec_lib import DeviceBase, messages
+from bec_lib import messages
 from bec_lib.bec_errors import DeviceConfigError
-from bec_lib.device import OnFailure, ReadoutPriority
+from bec_lib.device import DeviceBase, OnFailure, ReadoutPriority
 from bec_server.scihub import SciHub
 from bec_server.scihub.scibec import ConfigHandler, SciBecConnector
 
 dir_path = os.path.dirname(bec_lib.__file__)
 
 
 @pytest.fixture()
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scibec_connector.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scibec_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from unittest import mock
 
 import pytest
 
-from bec_lib import MessageEndpoints, ServiceConfig, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
 from bec_lib.messages import BECStatus
+from bec_lib.service_config import ServiceConfig
 from bec_lib.tests.utils import ConnectorMock
 from bec_server.scihub import SciHub
 from bec_server.scihub.scibec import SciBecConnector
 
 
 class SciHubMocked(SciHub):
     def _start_metrics_emitter(self):
```

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scilog_connector.py` & `ophyd_devices-1.0.2/bec/bec_server/tests/tests_scihub/test_scilog_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from unittest import mock
 
 from test_scibec_connector import SciHubMock
 
-from bec_lib import MessageEndpoints, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
 from bec_server.scihub.scilog import SciLogConnector
 
 
 def test_scilog_connector(SciHubMock):
     scilog = SciLogConnector(SciHubMock, SciHubMock.connector)
     scilog.shutdown()
```

### Comparing `ophyd_devices-1.0.1/bec/bin/install_bec_dev.sh` & `ophyd_devices-1.0.2/bec/bin/install_bec_dev.sh`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/ci/Dockerfile.run_server` & `ophyd_devices-1.0.2/bec/ci/Dockerfile.run_pytest`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # set base image (host OS)
-ARG PY_VERSION=3.10 OPHYD_BRANCH=master BEC_SERVICE=bec_ipython_client
-
-ARG BEC_SERVICE=bec_ipython_client OPHYD_BRANCH=master
-ARG CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
+ARG PY_VERSION=3.10 CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX
 
 FROM $CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX/python:${PY_VERSION}
 
-RUN echo "Building ${BEC_SERVICE} with Ophyd branch ${OPHYD_BRANCH}"
+ARG BEC_SERVICE=bec_ipython_client OPHYD_DEVICES_BRANCH=main
+
+RUN echo "Building ${BEC_SERVICE} with Ophyd branch ${OPHYD_DEVICES_BRANCH} "
 
 RUN apt update
+RUN apt install redis -y
 RUN apt install git -y
 
 # set the working directory in the container
 WORKDIR /code
 
 # copy the content of the local opaas directory to the working directory
 COPY . ./bec
 
+RUN mkdir /code/bec/test_files
 ENV OPHYD_DEVICES_PATH=/code/bec/ophyd_devices
 
 WORKDIR /code/bec
-RUN git clone --branch ${OPHYD_BRANCH} https://gitlab.psi.ch/bec/ophyd_devices
+RUN git clone --branch ${OPHYD_DEVICES_BRANCH} https://gitlab.psi.ch/bec/ophyd_devices
 WORKDIR /code/bec/ophyd_devices
 RUN pip install -e .
-WORKDIR /code/bec/pytest_bec_e2e
-RUN pip install -e .
+WORKDIR /code/bec/
+
+RUN pip install -e pytest_bec_e2e
+RUN pip install -e bec_server[dev]
+RUN pip install -e bec_ipython_client[dev]
+RUN pip install -e bec_lib[dev]
+
 WORKDIR /code/bec/${BEC_SERVICE}
-RUN pip install -e .[dev]
 
+# command to run on container start
+ENTRYPOINT ["pytest", "--files-path", "/code/bec/test_files", "--start-servers", "--flush-redis", "-v", "--random-order", "--maxfail=2",  "./tests/end-2-end"]
```

### Comparing `ophyd_devices-1.0.1/bec/ci/docker-compose.yaml` & `ophyd_devices-1.0.2/bec/ci/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/ci/semantic_release.toml` & `ophyd_devices-1.0.2/bec/ci/semantic_release.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/architecture/BEC.drawio` & `ophyd_devices-1.0.2/bec/docs/architecture/BEC.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/architecture/BEC_config_db.drawio` & `ophyd_devices-1.0.2/bec/docs/architecture/BEC_config_db.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/architecture/BEC_config_db.svg` & `ophyd_devices-1.0.2/bec/docs/architecture/BEC_config_db.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/architecture/bec_architecture.png` & `ophyd_devices-1.0.2/bec/docs/architecture/bec_architecture.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/Makefile` & `ophyd_devices-1.0.2/bec/docs/source/Makefile`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/conf.py` & `ophyd_devices-1.0.2/bec/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/make.bat` & `ophyd_devices-1.0.2/bec/docs/source/make.bat`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/_static/bec.png` & `ophyd_devices-1.0.2/bec/docs/source/_static/bec.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/_static/css/custom.css` & `ophyd_devices-1.0.2/bec/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/_static/gif/bec_plotter.gif` & `ophyd_devices-1.0.2/bec/docs/source/_static/gif/bec_plotter.gif`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/_templates/custom-class-template.rst` & `ophyd_devices-1.0.2/bec/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/_templates/custom-module-template.rst` & `ophyd_devices-1.0.2/bec/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/assets/BEC_context_user_centric.png` & `ophyd_devices-1.0.2/bec/docs/source/assets/BEC_context_user_centric.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/assets/bec_architecture.png` & `ophyd_devices-1.0.2/bec/docs/source/assets/bec_architecture.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/assets/bec_device_structure.drawio` & `ophyd_devices-1.0.2/bec/docs/source/assets/bec_device_structure.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/assets/bec_device_structure.png` & `ophyd_devices-1.0.2/bec/docs/source/assets/bec_device_structure.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/assets/gauss_scatter_plot.png` & `ophyd_devices-1.0.2/bec/docs/source/assets/gauss_scatter_plot.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/assets/simulation_context_diagram.drawio` & `ophyd_devices-1.0.2/bec/docs/source/assets/simulation_context_diagram.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/assets/simulation_context_diagram.png` & `ophyd_devices-1.0.2/bec/docs/source/assets/simulation_context_diagram.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/assets/tab-complete-devices.png` & `ophyd_devices-1.0.2/bec/docs/source/assets/tab-complete-devices.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/assets/vscode_debug_button.png` & `ophyd_devices-1.0.2/bec/docs/source/assets/vscode_debug_button.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/assets/vscode_with_annotations.drawio` & `ophyd_devices-1.0.2/bec/docs/source/assets/vscode_with_annotations.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/assets/vscode_with_annotations.png` & `ophyd_devices-1.0.2/bec/docs/source/assets/vscode_with_annotations.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/assets/wm-devices.png` & `ophyd_devices-1.0.2/bec/docs/source/assets/wm-devices.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/developer/architecture.md` & `ophyd_devices-1.0.2/bec/docs/source/developer/architecture.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/developer/bec_plugins.md` & `ophyd_devices-1.0.2/bec/docs/source/developer/bec_plugins.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/developer/bec_sim.md` & `ophyd_devices-1.0.2/bec/docs/source/developer/bec_sim.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/developer/contributing.md` & `ophyd_devices-1.0.2/bec/docs/source/developer/contributing.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/developer/developer.md` & `ophyd_devices-1.0.2/bec/docs/source/developer/developer.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 bec_gui/
 bec_config/
 data_access/
 event_data/
 ophyd/
 external_sources/
 bec_plugins/
+scans/
 glossary/
 reference/
 ```
 
 ***
 **Developer Documentation for BEC**
 
@@ -41,14 +42,15 @@
 * [BEC Graphical User Interface (GUI)](#developer.bec_gui): Learn how to use the graphical user interface to interact with BEC and explore how to create your own GUIs.
 * [BEC Configuration](#developer.bec_config): Learn about the different ways of customizing BEC to your needs.
 * [Data Access](#developer.data_access): Explore different ways of accessing data acquired with BEC.
 * [Event Data](#developer.data_access): Explore the handling of event data in BEC to streamline your data analysis and live feedback.
 * [Ophyd](#developer.ophyd): Familiarize yourself with Ophyd, the underlying library for device control in BEC, and learn how to integrate and work with Ophyd devices in the BEC context.
 * [External Sources](#developer.external_sources): Understand how to incorporate external data sources into your BEC workflow.
 * [BEC Plugins](#developer.bec_plugins): Learn how to create and use plugins to extend BEC's functionality and tailor it to your needs.
+* [Scans](#developer.scans): Dive into the world of scans in BEC, understand the basic structure of a scan, and learn how to create a scan plugin.
 * [Writing tests](#developer.tests): how to write tests for your code, and usage information about BEC fixtures
 * [Glossary](#developer.glossary): Refer to a glossary of terms used throughout the BEC documentation.
 * [Reference](#developer.reference): Access a comprehensive reference of all BEC classes, functions, and methods.
 
 
 We invite you to embark on your BEC development journey, empowering you to contribute to this dynamic project and tailor it to the unique requirements of your experiments. Happy coding!
```

### Comparing `ophyd_devices-1.0.1/bec/docs/source/developer/external_sources.md` & `ophyd_devices-1.0.2/bec/docs/source/developer/external_sources.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 (developer.external_sources)=
 # External data sources
 Large data sources typically have their own data pipeline, optimized for their specific use case and data throughput. Yet, it is often desirable to use the BEC to be informed and potentially link to these external data sources.
 As of now, only external data sources that are based on HDF5 files are supported. BEC can be informed about new HDF5 files by emitting a [FileMessage](#bec_lib.messages.FileMessage) to the [public_file endpoint](#bec_lib.endpoints.MessageEndpoints.public_file), e.g.
 
 ```python
-from bec_lib import MessageEndpoints, messages, RedisConnector
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib import messages
+from bec_lib.redis_connector import RedisConnector
 
 scan_id = "scan id of the current scan"
 
 # get a new producer for redis messages
 producer = RedisConnector(["localhost:6379"]).producer()
 
 # prepare the message
```

### Comparing `ophyd_devices-1.0.1/bec/docs/source/developer/glossary.md` & `ophyd_devices-1.0.2/bec/docs/source/developer/glossary.md`

 * *Files 23% similar despite different names*

```diff
@@ -3,13 +3,18 @@
 
 ```{glossary}
 :sorted:
 scan_id 
     The ``scan_id`` is the unique identifier for a scan. It is a string, typically uuid4, that is generated automatically by the scan server. It is used to uniquely identify a scan, even across multiple experiments and beamlines.
 scan_number
     The ``scan_number`` is an integer that is assigned to a scan by the scan server. It can be used to identify a scan within an experiment but is typically reset to 1 for each new experiment. The ``scan_number`` is also used by the file_writer to name the files that are generated by a scan.
-requestID
-    The ``requestID`` is an identifier for a request to the scan server. As of now, it is a uuid4 string that is generated by the bec_lib during the preparation of a new request. A scan can comprise instructions from multiple requests.
+dataset_number
+    The ``dataset_number`` is an integer that is assigned to a dataset by the scan server. It is used to group scans into larger, logical units. The ``dataset_number`` is typically reset to 1 for each new experiment.
+request_id
+    The ``request_id`` is an identifier for a request to the scan server. As of now, it is a uuid4 string that is generated by the bec_lib during the preparation of a new request. A scan can comprise instructions from multiple requests.
 queue_id
     The ``queue_id`` is an identifier for an element in a queue. Each queue element can contain multiple scans and thus enforce the sequential execution of those scans. The ``queue_id`` is a uuid4 string that is generated by the bec_lib during the preparation of a new queue element.
+DIID
+    The ``DIID`` is the device instruction ID. It is a continuously increasing integer that is assigned to each device instruction in a scan. The ``DIID`` is used to uniquely identify each device instruction and its response in the scan. 
+
 
 ```
```

### Comparing `ophyd_devices-1.0.1/bec/docs/source/developer/install_developer_env.md` & `ophyd_devices-1.0.2/bec/docs/source/developer/install_developer_env.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/developer/logs.md` & `ophyd_devices-1.0.2/bec/docs/source/developer/logs.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 The log level can be set for each service and even each sink individually. While this is normally not necessary, it can be useful for not flooding the terminal with log messages. To this end, the default log level of the stdout sink of the client is set to SUCCESS while the log level of the file sink is set to INFO.
 ```
 
 ## Usage
 Using the logger in BEC is straightforward. The logger is already included in the BEC environment and can be imported via
 
 ```python
-from bec_lib import bec_logger
+from bec_lib.logger import bec_logger
 logger = bec_logger.logger
 ```
 
 `logger` can be used to log messages of different types. The following example shows how to log messages of different types:
 
 ```python
 logger.trace("This is a trace message")
```

### Comparing `ophyd_devices-1.0.1/bec/docs/source/developer/ophyd.md` & `ophyd_devices-1.0.2/bec/docs/source/developer/ophyd.md`

 * *Files 0% similar despite different names*

```diff
@@ -173,14 +173,15 @@
 * **kickoff() -> ophyd.DeviceStatus**\
 Upon calling kickoff, the flyer should start and return a status object that resolves once the flyer flies, i.e. is ready to or already acquiring data.
 
 * **complete() -> ophyd.DeviceStatus**\
 The complete method of the flyer returns a status object. 
 This status should resolve once the flyer finishes, thus, the method can be used to identify when a flyer is finished.
 
+(developer.ophyd_device_config)=
 ## Ophyd device configuration
 As mentioned before, BEC creates representative devices and signals dynamically on the devices server, following the specifications given in the device configuration. 
 As explained in the [device configuration](#developer.bec_config) section, the device configuration can be loaded from and stored to a yaml file and contains all necessary information about the devices. 
 
 An example of an ophyd device based on EPICS is a single PV, e.g. the synchrotron's ring current: 
 
 ```yaml
```

### Comparing `ophyd_devices-1.0.1/bec/docs/source/developer/tests.md` & `ophyd_devices-1.0.2/bec/docs/source/developer/tests.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 threads may come from third-party libraries, like `loguru` which is used by BEC for logging. In case of `loguru`, call
 `bec_logger.logger.remove()` to clean it.
 
 It could be useful to automatically enable the threads check and `loguru` cleaning for all tests ; in this case, add the
 following fixture to a `conftest.py` file with your new test files:
 
 ```
-from bec_lib import bec_logger
+from bec_lib.logger import bec_logger
 def auto_check_threads(threads_check):
     yield
     bec_logger.logger.remove()
 ```
 
 ### dm and dm_with_devices
```

### Comparing `ophyd_devices-1.0.1/bec/docs/source/developer/vscode.md` & `ophyd_devices-1.0.2/bec/docs/source/developer/vscode.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/introduction/introduction.md` & `ophyd_devices-1.0.2/bec/docs/source/introduction/introduction.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/user/command_line_interface.md` & `ophyd_devices-1.0.2/bec/docs/source/user/command_line_interface.md`

 * *Files 2% similar despite different names*

```diff
@@ -300,15 +300,19 @@
 
 ### How to write a script
 -----------------------
 
 Scripts are user defined functions that can be executed from the BEC console (CLI). 
 They are stored in the ``scripts`` folder and can be edited with any text editor. 
 The scripts are loaded automatically on startup of the BEC console but can also be reloaded by typing ``bec.load_all_user_scripts()`` in the command-line.
-This command will load scripts from three locations: `~/bec/scripts/.`, `bec/bec_lib/scripts/.` and the beamline plugin directory, e.g. `/csaxs-bec/bec_plugins/scripts/.`
+This command will load scripts from three locations: 
+
+1. from `~/bec/scripts/` in your home directory, 
+1. from the beamline plugin directory, e.g. `/csaxs_bec/csaxs_bec/scripts/`
+1. from `bec/bec_lib/scripts/` (only useful if you have the entire source code of BEC installed locally).
 
 
 An example of a user script could be a function to move a specific motor to a predefined position:
 
 ```python 
     def samx_in():
         umv(dev.samx, 0)
```

### Comparing `ophyd_devices-1.0.1/bec/docs/source/user/data_access_and_plotting.md` & `ophyd_devices-1.0.2/bec/docs/source/user/data_access_and_plotting.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/user/devices.md` & `ophyd_devices-1.0.2/bec/docs/source/user/devices.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/user/graphical_user_interface.md` & `ophyd_devices-1.0.2/bec/docs/source/user/graphical_user_interface.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/user/installation.md` & `ophyd_devices-1.0.2/bec/docs/source/user/installation.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/docs/source/user/user.md` & `ophyd_devices-1.0.2/bec/docs/source/user/user.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/bec/pytest_bec_e2e/pyproject.toml` & `ophyd_devices-1.0.2/bec/pytest_bec_e2e/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytest-bec-e2e"
-version = "2.11.0"
+version = "2.12.3"
 description = "BEC pytest plugin for end-to-end tests"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.0.1/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py` & `ophyd_devices-1.0.2/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 import tempfile
 
 import pytest
 from pytest_redis import factories as pytest_redis_factories
 from redis import Redis
 
 from bec_ipython_client import BECIPythonClient
-from bec_lib import BECClient, ConfigHelper, RedisConnector, ServiceConfig
+from bec_lib.client import BECClient
+from bec_lib.config_helper import ConfigHelper
+from bec_lib.redis_connector import RedisConnector
+from bec_lib.service_config import ServiceConfig
 from bec_lib.tests.utils import wait_for_empty_queue
 
 
 @pytest.hookimpl
 def pytest_addoption(parser):
     parser.addoption("--start-servers", action="store_true", default=False)
     parser.addoption("--bec-redis-host", action="store", default="localhost")
```

### Comparing `ophyd_devices-1.0.1/ophyd_devices/__init__.py` & `ophyd_devices-1.0.2/ophyd_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/ophyd_patch.py` & `ophyd_devices-1.0.2/ophyd_devices/ophyd_patch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/configs/ophyd_devices_simulation.yaml` & `ophyd_devices-1.0.2/ophyd_devices/configs/ophyd_devices_simulation.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/configs/ophyd_simulation.yaml` & `ophyd_devices-1.0.2/ophyd_devices/configs/ophyd_simulation.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/devices/SpmBase.py` & `ophyd_devices-1.0.2/ophyd_devices/devices/SpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/devices/XbpmBase.py` & `ophyd_devices-1.0.2/ophyd_devices/devices/XbpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/devices/__init__.py` & `ophyd_devices-1.0.2/ophyd_devices/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/devices/epics_motor_ex.py` & `ophyd_devices-1.0.2/ophyd_devices/devices/epics_motor_ex.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/devices/mono_dccm.py` & `ophyd_devices-1.0.2/ophyd_devices/devices/mono_dccm.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/devices/slits.py` & `ophyd_devices-1.0.2/ophyd_devices/devices/slits.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/devices/slsDetector.py` & `ophyd_devices-1.0.2/ophyd_devices/devices/sls_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ophyd import ADComponent as ADCpt
 from ophyd import CamBase, DetectorBase, EpicsSignal, EpicsSignalRO, EpicsSignalWithRBV
 from ophyd.areadetector.plugins import FileBase
 
 
-class slsDetectorCam(CamBase, FileBase):
+class SLSDetectorCam(CamBase, FileBase):
     detector_type = ADCpt(EpicsSignalRO, "DetectorType_RBV")
     setting = ADCpt(EpicsSignalWithRBV, "Setting")
     delay_time = ADCpt(EpicsSignalWithRBV, "DelayTime")
     threshold_energy = ADCpt(EpicsSignalWithRBV, "ThresholdEnergy")
     enable_trimbits = ADCpt(EpicsSignalWithRBV, "Trimbits")
     bit_depth = ADCpt(EpicsSignalWithRBV, "BitDepth")
     num_gates = ADCpt(EpicsSignalWithRBV, "NumGates")
@@ -37,9 +37,9 @@
     gate3_delay = ADCpt(EpicsSignalWithRBV, "Gate3Delay")
     gate3_width = ADCpt(EpicsSignalWithRBV, "Gate3Width")
     # Moench
     json_frame_mode = ADCpt(EpicsSignalWithRBV, "JsonFrameMode")
     json_detector_mode = ADCpt(EpicsSignalWithRBV, "JsonDetectorMode")
 
 
-class slsDetector(DetectorBase):
-    cam = ADCpt(slsDetectorCam, "cam1:")
+class SLSDetector(DetectorBase):
+    cam = ADCpt(SLSDetectorCam, "cam1:")
```

### Comparing `ophyd_devices-1.0.1/ophyd_devices/devices/sls_devices.py` & `ophyd_devices-1.0.2/ophyd_devices/devices/sls_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/devices/specMotors.py` & `ophyd_devices-1.0.2/ophyd_devices/devices/specMotors.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py` & `ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py` & `ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/psi_detector_base.py` & `ophyd_devices-1.0.2/ophyd_devices/interfaces/base_classes/psi_detector_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/interfaces/protocols/bec_protocols.py` & `ophyd_devices-1.0.2/ophyd_devices/interfaces/protocols/bec_protocols.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/sim/sim.py` & `ophyd_devices-1.0.2/ophyd_devices/sim/sim.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/sim/sim_data.py` & `ophyd_devices-1.0.2/ophyd_devices/sim/sim_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/sim/sim_frameworks.py` & `ophyd_devices-1.0.2/ophyd_devices/sim/sim_frameworks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/sim/sim_signals.py` & `ophyd_devices-1.0.2/ophyd_devices/sim/sim_signals.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/sim/sim_test_devices.py` & `ophyd_devices-1.0.2/ophyd_devices/sim/sim_test_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/sim/sim_xtreme.py` & `ophyd_devices-1.0.2/ophyd_devices/sim/sim_xtreme.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt` & `ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt` & `ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt` & `ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt` & `ophyd_devices-1.0.2/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/tests/utils.py` & `ophyd_devices-1.0.2/ophyd_devices/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/utils/bec_device_base.py` & `ophyd_devices-1.0.2/ophyd_devices/utils/bec_device_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/utils/bec_scaninfo_mixin.py` & `ophyd_devices-1.0.2/ophyd_devices/utils/bec_scaninfo_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/utils/bec_utils.py` & `ophyd_devices-1.0.2/ophyd_devices/utils/bec_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/utils/controller.py` & `ophyd_devices-1.0.2/ophyd_devices/utils/controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/utils/dynamic_pseudo.py` & `ophyd_devices-1.0.2/ophyd_devices/utils/dynamic_pseudo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/utils/socket.py` & `ophyd_devices-1.0.2/ophyd_devices/utils/socket.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/ophyd_devices/utils/static_device_test.py` & `ophyd_devices-1.0.2/ophyd_devices/utils/static_device_test.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/tests/test_controller.py` & `ophyd_devices-1.0.2/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/tests/test_dynamic_pseudo.py` & `ophyd_devices-1.0.2/tests/test_dynamic_pseudo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/tests/test_ophyd_status_obj.py` & `ophyd_devices-1.0.2/tests/test_ophyd_status_obj.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/tests/test_simulation.py` & `ophyd_devices-1.0.2/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/tests/test_socket.py` & `ophyd_devices-1.0.2/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/.gitignore` & `ophyd_devices-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/LICENSE` & `ophyd_devices-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.1/pyproject.toml` & `ophyd_devices-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ophyd_devices"
-version = "1.0.1"
+version = "1.0.2"
 description = "Custom device implementations based on the ophyd hardware abstraction layer"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "ophyd ~= 1.9",
     "typeguard ~= 4.1, >=4.1.4",
     "prettytable ~= 3.9",
-    "bec_lib ~= 2.8",
+    "bec_lib ~= 2.12, >=2.12.2",
     "numpy ~= 1.24",
     "pyyaml ~= 6.0",
     "std_daq_client ~= 1.3",
     "pyepics ~= 3.5",
     "pytest ~= 8.0",
     "h5py ~= 3.10",
     "hdf5plugin ~= 4.3",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "bec-server~=2.7",
+    "bec-server~= 2.12, >=2.12.2",
     "black~=24.0",
     "isort~=5.13, >=5.13.2",
     "coverage~=7.0",
     "pylint~=3.0",
     "pytest-random-order~=1.1",
 ]
```

### Comparing `ophyd_devices-1.0.1/PKG-INFO` & `ophyd_devices-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.3
 Name: ophyd_devices
-Version: 1.0.1
+Version: 1.0.2
 Summary: Custom device implementations based on the ophyd hardware abstraction layer
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/ophyd_devices/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/ophyd_devices
 Project-URL: documentation, https://bec.readthedocs.org
 Project-URL: changelog, https://gitlab.psi.ch/bec/ophyd_devices/blob/main/CHANGELOG.md
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
-Requires-Dist: bec-lib~=2.8
+Requires-Dist: bec-lib>=2.12.2,~=2.12
 Requires-Dist: h5py~=3.10
 Requires-Dist: hdf5plugin~=4.3
 Requires-Dist: numpy~=1.24
 Requires-Dist: ophyd~=1.9
 Requires-Dist: prettytable~=3.9
 Requires-Dist: pyepics~=3.5
 Requires-Dist: pytest~=8.0
 Requires-Dist: pyyaml~=6.0
 Requires-Dist: std-daq-client~=1.3
 Requires-Dist: typeguard>=4.1.4,~=4.1
 Provides-Extra: dev
-Requires-Dist: bec-server~=2.7; extra == 'dev'
+Requires-Dist: bec-server>=2.12.2,~=2.12; extra == 'dev'
 Requires-Dist: black~=24.0; extra == 'dev'
 Requires-Dist: coverage~=7.0; extra == 'dev'
 Requires-Dist: isort>=5.13.2,~=5.13; extra == 'dev'
 Requires-Dist: pylint~=3.0; extra == 'dev'
 Requires-Dist: pytest-random-order~=1.1; extra == 'dev'
```

