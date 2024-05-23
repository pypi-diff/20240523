# Comparing `tmp/trycourier-6.0.5.tar.gz` & `tmp/trycourier-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycourier-6.0.5.tar", max compression
+gzip compressed data, was "trycourier-6.1.0.tar", max compression
```

## Comparing `trycourier-6.0.5.tar` & `trycourier-6.1.0.tar`

### file list

```diff
@@ -1,368 +1,371 @@
--rw-r--r--   0        0        0     1063 2024-05-03 20:57:54.394602 trycourier-6.0.5/LICENSE
--rw-r--r--   0        0        0     5507 2024-05-03 20:57:54.394602 trycourier-6.0.5/README.md
--rw-r--r--   0        0        0      595 2024-05-03 20:57:54.394602 trycourier-6.0.5/pyproject.toml
--rw-r--r--   0        0        0    14204 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/__init__.py
--rw-r--r--   0        0        0      751 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/__init__.py
--rw-r--r--   0        0        0    28202 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/client.py
--rw-r--r--   0        0        0     1100 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/__init__.py
--rw-r--r--   0        0        0     1199 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/audience.py
--rw-r--r--   0        0        0      971 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/audience_list_response.py
--rw-r--r--   0        0        0      939 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/audience_member.py
--rw-r--r--   0        0        0     1052 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/audience_member_get_response.py
--rw-r--r--   0        0        0      996 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/audience_member_list_response.py
--rw-r--r--   0        0        0      901 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/audience_update_response.py
--rw-r--r--   0        0        0      971 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/base_filter_config.py
--rw-r--r--   0        0        0      386 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/comparison_operator.py
--rw-r--r--   0        0        0      249 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/filter.py
--rw-r--r--   0        0        0      255 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/filter_config.py
--rw-r--r--   0        0        0      152 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/logical_operator.py
--rw-r--r--   0        0        0     1191 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/nested_filter_config.py
--rw-r--r--   0        0        0      240 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/operator.py
--rw-r--r--   0        0        0     1252 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audiences/types/single_filter_config.py
--rw-r--r--   0        0        0      299 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audit_events/__init__.py
--rw-r--r--   0        0        0    10417 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audit_events/client.py
--rw-r--r--   0        0        0      453 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audit_events/types/__init__.py
--rw-r--r--   0        0        0      905 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audit_events/types/actor.py
--rw-r--r--   0        0        0     1164 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audit_events/types/audit_event.py
--rw-r--r--   0        0        0      988 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audit_events/types/get_audit_event_params.py
--rw-r--r--   0        0        0      886 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audit_events/types/list_audit_events_params.py
--rw-r--r--   0        0        0      983 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audit_events/types/list_audit_events_response.py
--rw-r--r--   0        0        0      906 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/audit_events/types/target.py
--rw-r--r--   0        0        0      137 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/auth_tokens/__init__.py
--rw-r--r--   0        0        0     7229 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/auth_tokens/client.py
--rw-r--r--   0        0        0      152 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/auth_tokens/types/__init__.py
--rw-r--r--   0        0        0      882 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/auth_tokens/types/issue_token_response.py
--rw-r--r--   0        0        0     1847 2024-05-03 20:57:54.394602 trycourier-6.0.5/src/courier/automations/__init__.py
--rw-r--r--   0        0        0    16885 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/client.py
--rw-r--r--   0        0        0     2836 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/__init__.py
--rw-r--r--   0        0        0      962 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/accessor_type.py
--rw-r--r--   0        0        0      988 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation.py
--rw-r--r--   0        0        0     1054 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_ad_hoc_invoke_params.py
--rw-r--r--   0        0        0      138 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_add_to_batch_max_items_type.py
--rw-r--r--   0        0        0     1954 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_add_to_batch_retain.py
--rw-r--r--   0        0        0      192 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_add_to_batch_retain_type.py
--rw-r--r--   0        0        0      178 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_add_to_batch_scope.py
--rw-r--r--   0        0        0     3128 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_add_to_batch_step.py
--rw-r--r--   0        0        0     1355 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_add_to_digest_step.py
--rw-r--r--   0        0        0     1048 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_cancel_step.py
--rw-r--r--   0        0        0     1331 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_delay_step.py
--rw-r--r--   0        0        0     1784 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_fetch_data_step.py
--rw-r--r--   0        0        0     1186 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_fetch_data_webhook.py
--rw-r--r--   0        0        0      171 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_fetch_data_webhook_method.py
--rw-r--r--   0        0        0     1108 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_invoke_params.py
--rw-r--r--   0        0        0      978 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_invoke_response.py
--rw-r--r--   0        0        0     1015 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_invoke_step.py
--rw-r--r--   0        0        0     1056 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_invoke_template_params.py
--rw-r--r--   0        0        0     1088 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_run_context.py
--rw-r--r--   0        0        0     1262 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_send_list_step.py
--rw-r--r--   0        0        0     1295 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_send_step.py
--rw-r--r--   0        0        0     1030 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_step.py
--rw-r--r--   0        0        0     1102 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_step_option.py
--rw-r--r--   0        0        0     1052 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_throttle_on_throttle.py
--rw-r--r--   0        0        0      176 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_throttle_scope.py
--rw-r--r--   0        0        0     2301 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_throttle_step.py
--rw-r--r--   0        0        0     1039 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_update_profile_step.py
--rw-r--r--   0        0        0     1058 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/automation_v_2_send_step.py
--rw-r--r--   0        0        0      184 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/merge_algorithm.py
--rw-r--r--   0        0        0      101 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/automations/types/profile.py
--rw-r--r--   0        0        0      419 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/brands/__init__.py
--rw-r--r--   0        0        0    29995 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/brands/client.py
--rw-r--r--   0        0        0      579 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/brands/types/__init__.py
--rw-r--r--   0        0        0     1716 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/brands/types/brand.py
--rw-r--r--   0        0        0      962 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/brands/types/brand_colors.py
--rw-r--r--   0        0        0      963 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/brands/types/brand_get_all_response.py
--rw-r--r--   0        0        0     1120 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/brands/types/brand_parameters.py
--rw-r--r--   0        0        0     1052 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/brands/types/brand_settings.py
--rw-r--r--   0        0        0      907 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/brands/types/brand_snippet.py
--rw-r--r--   0        0        0      915 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/brands/types/brand_snippets.py
--rw-r--r--   0        0        0      958 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/brands/types/brands_response.py
--rw-r--r--   0        0        0     1059 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/__init__.py
--rw-r--r--   0        0        0    30912 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/client.py
--rw-r--r--   0        0        0     1603 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/__init__.py
--rw-r--r--   0        0        0      975 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/bulk_create_job_response.py
--rw-r--r--   0        0        0      970 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/bulk_get_job_params.py
--rw-r--r--   0        0        0      899 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/bulk_get_job_response.py
--rw-r--r--   0        0        0     1015 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/bulk_get_job_users_params.py
--rw-r--r--   0        0        0     1022 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/bulk_get_job_users_response.py
--rw-r--r--   0        0        0      883 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/bulk_ingest_error.py
--rw-r--r--   0        0        0      955 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/bulk_ingest_users_params.py
--rw-r--r--   0        0        0      975 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/bulk_ingest_users_response.py
--rw-r--r--   0        0        0      184 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/bulk_job_status.py
--rw-r--r--   0        0        0      173 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/bulk_job_user_status.py
--rw-r--r--   0        0        0     1161 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/bulk_message_user_response.py
--rw-r--r--   0        0        0     1512 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/inbound_bulk_content_message.py
--rw-r--r--   0        0        0     1096 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/inbound_bulk_message.py
--rw-r--r--   0        0        0     1218 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/inbound_bulk_message_user.py
--rw-r--r--   0        0        0     1672 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/inbound_bulk_message_v_1.py
--rw-r--r--   0        0        0      310 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/inbound_bulk_message_v_2.py
--rw-r--r--   0        0        0     1165 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/inbound_bulk_template_message.py
--rw-r--r--   0        0        0     1046 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/bulk/types/job_details.py
--rw-r--r--   0        0        0    17491 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/client.py
--rw-r--r--   0        0        0     1127 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/__init__.py
--rw-r--r--   0        0        0      527 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/errors/__init__.py
--rw-r--r--   0        0        0      289 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/errors/already_exists_error.py
--rw-r--r--   0        0        0      277 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/errors/bad_request_error.py
--rw-r--r--   0        0        0      268 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/errors/conflict_error.py
--rw-r--r--   0        0        0      298 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/errors/message_not_found_error.py
--rw-r--r--   0        0        0      269 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/errors/not_found_error.py
--rw-r--r--   0        0        0      297 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/errors/payment_required_error.py
--rw-r--r--   0        0        0     1207 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/__init__.py
--rw-r--r--   0        0        0      988 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/already_exists.py
--rw-r--r--   0        0        0      985 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/bad_request.py
--rw-r--r--   0        0        0      939 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/base_error.py
--rw-r--r--   0        0        0      213 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/channel_classification.py
--rw-r--r--   0        0        0      935 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/channel_preference.py
--rw-r--r--   0        0        0      983 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/conflict.py
--rw-r--r--   0        0        0      876 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/email.py
--rw-r--r--   0        0        0      990 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/message_not_found.py
--rw-r--r--   0        0        0      983 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/not_found.py
--rw-r--r--   0        0        0     1137 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/notification_preference_details.py
--rw-r--r--   0        0        0      230 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/notification_preferences.py
--rw-r--r--   0        0        0      886 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/paging.py
--rw-r--r--   0        0        0      988 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/payment_required.py
--rw-r--r--   0        0        0      177 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/preference_status.py
--rw-r--r--   0        0        0     1038 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/recipient_preferences.py
--rw-r--r--   0        0        0      883 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/rule.py
--rw-r--r--   0        0        0     1353 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/commons/types/user_tenant_association.py
--rw-r--r--   0        0        0      853 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/core/api_error.py
--rw-r--r--   0        0        0     2088 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/core/request_options.py
--rw-r--r--   0        0        0      159 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/environment.py
--rw-r--r--   0        0        0      413 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/lists/__init__.py
--rw-r--r--   0        0        0    69860 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/lists/client.py
--rw-r--r--   0        0        0      569 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/lists/types/__init__.py
--rw-r--r--   0        0        0      937 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/lists/types/list.py
--rw-r--r--   0        0        0      957 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/lists/types/list_get_all_response.py
--rw-r--r--   0        0        0     1032 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/lists/types/list_get_subscriptions_response.py
--rw-r--r--   0        0        0      986 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/lists/types/list_put_params.py
--rw-r--r--   0        0        0     1166 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/lists/types/list_subscription_recipient.py
--rw-r--r--   0        0        0     1125 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/lists/types/put_subscriptions_recipient.py
--rw-r--r--   0        0        0      527 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/messages/__init__.py
--rw-r--r--   0        0        0    41212 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/messages/client.py
--rw-r--r--   0        0        0      747 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/messages/types/__init__.py
--rw-r--r--   0        0        0     1157 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/messages/types/list_messages_response.py
--rw-r--r--   0        0        0     2811 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/messages/types/message_details.py
--rw-r--r--   0        0        0      932 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/messages/types/message_history_response.py
--rw-r--r--   0        0        0      357 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/messages/types/message_status.py
--rw-r--r--   0        0        0      233 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/messages/types/reason.py
--rw-r--r--   0        0        0     1234 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/messages/types/render_output.py
--rw-r--r--   0        0        0     1022 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/messages/types/render_output_response.py
--rw-r--r--   0        0        0     1050 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/messages/types/rendered_message_block.py
--rw-r--r--   0        0        0     1499 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/messages/types/rendered_message_content.py
--rw-r--r--   0        0        0     1081 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/__init__.py
--rw-r--r--   0        0        0    45003 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/client.py
--rw-r--r--   0        0        0     1614 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/__init__.py
--rw-r--r--   0        0        0      943 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/base_check.py
--rw-r--r--   0        0        0      229 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/block_type.py
--rw-r--r--   0        0        0      947 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/check.py
--rw-r--r--   0        0        0      168 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/check_status.py
--rw-r--r--   0        0        0     1127 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/message_routing.py
--rw-r--r--   0        0        0      183 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/message_routing_channel.py
--rw-r--r--   0        0        0      161 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/message_routing_method.py
--rw-r--r--   0        0        0     1114 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/notification.py
--rw-r--r--   0        0        0     1216 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/notification_block.py
--rw-r--r--   0        0        0     1151 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/notification_channel.py
--rw-r--r--   0        0        0      931 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/notification_channel_content.py
--rw-r--r--   0        0        0      224 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/notification_content.py
--rw-r--r--   0        0        0      935 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/notification_content_hierarchy.py
--rw-r--r--   0        0        0     1139 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/notification_get_content_response.py
--rw-r--r--   0        0        0      989 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/notification_list_response.py
--rw-r--r--   0        0        0      938 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/notification_tag.py
--rw-r--r--   0        0        0      870 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/notification_tag_data.py
--rw-r--r--   0        0        0      908 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/submission_checks_get_response.py
--rw-r--r--   0        0        0      912 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/notifications/types/submission_checks_replace_response.py
--rw-r--r--   0        0        0     1877 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/__init__.py
--rw-r--r--   0        0        0    43043 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/client.py
--rw-r--r--   0        0        0     2897 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/__init__.py
--rw-r--r--   0        0        0      947 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/address.py
--rw-r--r--   0        0        0     1015 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/airship_profile.py
--rw-r--r--   0        0        0      867 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/airship_profile_audience.py
--rw-r--r--   0        0        0      893 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/delete_list_subscription_response.py
--rw-r--r--   0        0        0      104 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/device_type.py
--rw-r--r--   0        0        0      232 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/discord.py
--rw-r--r--   0        0        0      193 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/expo.py
--rw-r--r--   0        0        0     1348 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/get_list_subscriptions_list.py
--rw-r--r--   0        0        0     1092 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/get_list_subscriptions_response.py
--rw-r--r--   0        0        0     1036 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/intercom.py
--rw-r--r--   0        0        0      854 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/intercom_recipient.py
--rw-r--r--   0        0        0      883 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/merge_profile_response.py
--rw-r--r--   0        0        0      566 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/ms_teams.py
--rw-r--r--   0        0        0      886 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/ms_teams_base_properties.py
--rw-r--r--   0        0        0      895 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/multiple_tokens.py
--rw-r--r--   0        0        0      986 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/profile_get_parameters.py
--rw-r--r--   0        0        0     1019 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/profile_get_response.py
--rw-r--r--   0        0        0      885 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/replace_profile_response.py
--rw-r--r--   0        0        0      859 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/send_direct_message.py
--rw-r--r--   0        0        0      858 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/send_to_channel.py
--rw-r--r--   0        0        0     1005 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/send_to_ms_teams_channel_id.py
--rw-r--r--   0        0        0     1026 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/send_to_ms_teams_channel_name.py
--rw-r--r--   0        0        0     1015 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/send_to_ms_teams_conversation_id.py
--rw-r--r--   0        0        0      996 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/send_to_ms_teams_email.py
--rw-r--r--   0        0        0      999 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/send_to_ms_teams_user_id.py
--rw-r--r--   0        0        0      991 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/send_to_slack_channel.py
--rw-r--r--   0        0        0      987 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/send_to_slack_email.py
--rw-r--r--   0        0        0      990 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/send_to_slack_user_id.py
--rw-r--r--   0        0        0      316 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/slack.py
--rw-r--r--   0        0        0      866 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/slack_base_properties.py
--rw-r--r--   0        0        0      935 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/snooze_rule.py
--rw-r--r--   0        0        0      148 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/snooze_rule_type.py
--rw-r--r--   0        0        0      992 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/subscribe_to_lists_request.py
--rw-r--r--   0        0        0     1123 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/subscribe_to_lists_request_list_object.py
--rw-r--r--   0        0        0      887 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/subscribe_to_lists_response.py
--rw-r--r--   0        0        0      845 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/token.py
--rw-r--r--   0        0        0     2026 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/profiles/types/user_profile.py
--rw-r--r--   0        0        0        0 2024-05-03 20:57:54.398602 trycourier-6.0.5/src/courier/py.typed
--rw-r--r--   0        0        0     4101 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/__init__.py
--rw-r--r--   0        0        0     6149 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/__init__.py
--rw-r--r--   0        0        0      122 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/attachment.py
--rw-r--r--   0        0        0     1031 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/audience_filter.py
--rw-r--r--   0        0        0     1201 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/audience_recipient.py
--rw-r--r--   0        0        0     2961 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/base_message.py
--rw-r--r--   0        0        0     1039 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/base_message_send_to.py
--rw-r--r--   0        0        0      856 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/base_social_presence.py
--rw-r--r--   0        0        0     1366 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/brand_settings_email.py
--rw-r--r--   0        0        0     1637 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/brand_settings_in_app.py
--rw-r--r--   0        0        0     1367 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/brand_settings_social_presence.py
--rw-r--r--   0        0        0     1308 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/brand_template.py
--rw-r--r--   0        0        0     1201 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/brand_template_override.py
--rw-r--r--   0        0        0     2359 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/channel.py
--rw-r--r--   0        0        0      898 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/channel_metadata.py
--rw-r--r--   0        0        0      174 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/channel_source.py
--rw-r--r--   0        0        0      252 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/content.py
--rw-r--r--   0        0        0     1546 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/content_message.py
--rw-r--r--   0        0        0      183 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/criteria.py
--rw-r--r--   0        0        0      933 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/delay.py
--rw-r--r--   0        0        0     2131 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/elemental_action_node.py
--rw-r--r--   0        0        0     1126 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/elemental_base_node.py
--rw-r--r--   0        0        0     2524 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/elemental_channel_node.py
--rw-r--r--   0        0        0     1056 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/elemental_content.py
--rw-r--r--   0        0        0     1180 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/elemental_content_sugar.py
--rw-r--r--   0        0        0     1178 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/elemental_divider_node.py
--rw-r--r--   0        0        0     1449 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/elemental_group_node.py
--rw-r--r--   0        0        0     1689 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/elemental_image_node.py
--rw-r--r--   0        0        0     1384 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/elemental_meta_node.py
--rw-r--r--   0        0        0     8164 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/elemental_node.py
--rw-r--r--   0        0        0     1697 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/elemental_quote_node.py
--rw-r--r--   0        0        0     2459 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/elemental_text_node.py
--rw-r--r--   0        0        0     1063 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/email_footer.py
--rw-r--r--   0        0        0     1023 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/email_head.py
--rw-r--r--   0        0        0     1141 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/email_header.py
--rw-r--r--   0        0        0      119 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/expires_in_type.py
--rw-r--r--   0        0        0     1257 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/expiry.py
--rw-r--r--   0        0        0      160 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/i_action_button_style.py
--rw-r--r--   0        0        0      169 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/i_alignment.py
--rw-r--r--   0        0        0      160 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/i_preferences.py
--rw-r--r--   0        0        0     1139 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/i_profile_preferences.py
--rw-r--r--   0        0        0      909 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/icons.py
--rw-r--r--   0        0        0      172 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/in_app_placement.py
--rw-r--r--   0        0        0      886 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/invalid_list_pattern_recipient.py
--rw-r--r--   0        0        0      884 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/invalid_list_recipient.py
--rw-r--r--   0        0        0      884 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/invalid_user_recipient.py
--rw-r--r--   0        0        0     1027 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/list_filter.py
--rw-r--r--   0        0        0     1122 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/list_pattern_recipient.py
--rw-r--r--   0        0        0      848 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/list_pattern_recipient_type.py
--rw-r--r--   0        0        0     1185 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/list_recipient.py
--rw-r--r--   0        0        0      841 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/list_recipient_type.py
--rw-r--r--   0        0        0      848 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/locale.py
--rw-r--r--   0        0        0      160 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/locales.py
--rw-r--r--   0        0        0      906 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/logo.py
--rw-r--r--   0        0        0      227 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/message.py
--rw-r--r--   0        0        0     1502 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/message_channel_email_override.py
--rw-r--r--   0        0        0      154 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/message_channels.py
--rw-r--r--   0        0        0     1123 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/message_context.py
--rw-r--r--   0        0        0      123 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/message_data.py
--rw-r--r--   0        0        0     1723 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/message_metadata.py
--rw-r--r--   0        0        0      196 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/message_providers.py
--rw-r--r--   0        0        0     1477 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/message_providers_type.py
--rw-r--r--   0        0        0      181 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/message_recipient.py
--rw-r--r--   0        0        0      891 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/metadata.py
--rw-r--r--   0        0        0      910 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/ms_teams_recipient.py
--rw-r--r--   0        0        0      193 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/override.py
--rw-r--r--   0        0        0     1258 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/preference.py
--rw-r--r--   0        0        0      990 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/preferences.py
--rw-r--r--   0        0        0      583 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/recipient.py
--rw-r--r--   0        0        0      125 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/recipient_data.py
--rw-r--r--   0        0        0     1462 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/routing.py
--rw-r--r--   0        0        0      289 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/routing_channel.py
--rw-r--r--   0        0        0      154 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/routing_method.py
--rw-r--r--   0        0        0     1279 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/routing_strategy_channel.py
--rw-r--r--   0        0        0     1135 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/routing_strategy_provider.py
--rw-r--r--   0        0        0      175 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/rule_type.py
--rw-r--r--   0        0        0      898 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/slack_recipient.py
--rw-r--r--   0        0        0     1212 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/template_message.py
--rw-r--r--   0        0        0      160 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/text_align.py
--rw-r--r--   0        0        0      164 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/text_style.py
--rw-r--r--   0        0        0     1114 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/timeout.py
--rw-r--r--   0        0        0      916 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/timeouts.py
--rw-r--r--   0        0        0      856 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/tracking_override.py
--rw-r--r--   0        0        0     2035 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/user_recipient.py
--rw-r--r--   0        0        0      841 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/user_recipient_type.py
--rw-r--r--   0        0        0     1029 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/utm.py
--rw-r--r--   0        0        0     1101 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/send/types/widget_background.py
--rw-r--r--   0        0        0      411 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/templates/__init__.py
--rw-r--r--   0        0        0     5852 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/templates/client.py
--rw-r--r--   0        0        0      564 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/templates/types/__init__.py
--rw-r--r--   0        0        0       89 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/templates/types/channel_identifier.py
--rw-r--r--   0        0        0     1091 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/templates/types/list_templates_response.py
--rw-r--r--   0        0        0     1781 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/templates/types/notification_templates.py
--rw-r--r--   0        0        0     1351 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/templates/types/routing_strategy.py
--rw-r--r--   0        0        0      162 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/templates/types/routing_strategy_method.py
--rw-r--r--   0        0        0      889 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/templates/types/tag.py
--rw-r--r--   0        0        0      992 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/templates/types/tag_data.py
--rw-r--r--   0        0        0      449 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/tenants/__init__.py
--rw-r--r--   0        0        0    30811 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/tenants/client.py
--rw-r--r--   0        0        0      624 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/tenants/types/__init__.py
--rw-r--r--   0        0        0      959 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/tenants/types/default_preferences.py
--rw-r--r--   0        0        0     1737 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/tenants/types/list_users_for_tenant_response.py
--rw-r--r--   0        0        0     1005 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/tenants/types/subscription_topic.py
--rw-r--r--   0        0        0      184 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/tenants/types/subscription_topic_status.py
--rw-r--r--   0        0        0      110 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/tenants/types/template_property.py
--rw-r--r--   0        0        0     1868 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/tenants/types/tenant.py
--rw-r--r--   0        0        0     1698 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/tenants/types/tenant_list_response.py
--rw-r--r--   0        0        0       65 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/translations/__init__.py
--rw-r--r--   0        0        0    11268 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/translations/client.py
--rw-r--r--   0        0        0      155 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/types/__init__.py
--rw-r--r--   0        0        0     1592 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/types/send_message_response.py
--rw-r--r--   0        0        0     1354 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/__init__.py
--rw-r--r--   0        0        0     1067 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/client.py
--rw-r--r--   0        0        0      409 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/preferences/__init__.py
--rw-r--r--   0        0        0    18445 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/preferences/client.py
--rw-r--r--   0        0        0      561 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/preferences/types/__init__.py
--rw-r--r--   0        0        0     1345 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/preferences/types/topic_preference.py
--rw-r--r--   0        0        0     1276 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/preferences/types/topic_preference_update.py
--rw-r--r--   0        0        0      926 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/preferences/types/user_preferences_get_response.py
--rw-r--r--   0        0        0     1090 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/preferences/types/user_preferences_list_response.py
--rw-r--r--   0        0        0      873 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/preferences/types/user_preferences_update_response.py
--rw-r--r--   0        0        0      229 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tenants/__init__.py
--rw-r--r--   0        0        0    28780 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tenants/client.py
--rw-r--r--   0        0        0      308 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tenants/types/__init__.py
--rw-r--r--   0        0        0     1397 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py
--rw-r--r--   0        0        0     1740 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tenants/types/list_tenants_for_user_response.py
--rw-r--r--   0        0        0      765 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/__init__.py
--rw-r--r--   0        0        0    29460 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/client.py
--rw-r--r--   0        0        0     1135 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/__init__.py
--rw-r--r--   0        0        0      878 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/delete_user_token_opts.py
--rw-r--r--   0        0        0     1576 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/device.py
--rw-r--r--   0        0        0      117 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/expiry_date.py
--rw-r--r--   0        0        0      161 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/get_all_tokens_response.py
--rw-r--r--   0        0        0      875 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/get_user_token_opts.py
--rw-r--r--   0        0        0     1160 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/get_user_token_response.py
--rw-r--r--   0        0        0      861 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/get_user_tokens_opts.py
--rw-r--r--   0        0        0      183 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/patch_op.py
--rw-r--r--   0        0        0     1158 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/patch_operation.py
--rw-r--r--   0        0        0      928 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/patch_user_token_opts.py
--rw-r--r--   0        0        0      179 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/provider_key.py
--rw-r--r--   0        0        0      915 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/put_user_token_opts.py
--rw-r--r--   0        0        0      930 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/put_user_tokens_opts.py
--rw-r--r--   0        0        0      177 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/token_status.py
--rw-r--r--   0        0        0     1387 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/tracking.py
--rw-r--r--   0        0        0     1790 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/users/tokens/types/user_token.py
--rw-r--r--   0        0        0       78 2024-05-03 20:57:54.402602 trycourier-6.0.5/src/courier/version.py
--rw-r--r--   0        0        0     6000 1970-01-01 00:00:00.000000 trycourier-6.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-23 13:24:57.205938 trycourier-6.1.0/LICENSE
+-rw-r--r--   0        0        0     5386 2024-05-23 13:24:57.205938 trycourier-6.1.0/README.md
+-rw-r--r--   0        0        0     1340 2024-05-23 13:24:57.205938 trycourier-6.1.0/pyproject.toml
+-rw-r--r--   0        0        0    14258 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/__init__.py
+-rw-r--r--   0        0        0      751 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/__init__.py
+-rw-r--r--   0        0        0    29813 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/client.py
+-rw-r--r--   0        0        0     1100 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/__init__.py
+-rw-r--r--   0        0        0     1519 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/audience.py
+-rw-r--r--   0        0        0     1291 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/audience_list_response.py
+-rw-r--r--   0        0        0     1259 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/audience_member.py
+-rw-r--r--   0        0        0     1372 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/audience_member_get_response.py
+-rw-r--r--   0        0        0     1316 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/audience_member_list_response.py
+-rw-r--r--   0        0        0     1221 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/audience_update_response.py
+-rw-r--r--   0        0        0     1291 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/base_filter_config.py
+-rw-r--r--   0        0        0      386 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/comparison_operator.py
+-rw-r--r--   0        0        0      249 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/filter.py
+-rw-r--r--   0        0        0      255 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/filter_config.py
+-rw-r--r--   0        0        0      152 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/logical_operator.py
+-rw-r--r--   0        0        0     1454 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/nested_filter_config.py
+-rw-r--r--   0        0        0      240 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/operator.py
+-rw-r--r--   0        0        0     1515 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audiences/types/single_filter_config.py
+-rw-r--r--   0        0        0      299 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audit_events/__init__.py
+-rw-r--r--   0        0        0    10894 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audit_events/client.py
+-rw-r--r--   0        0        0      453 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audit_events/types/__init__.py
+-rw-r--r--   0        0        0     1225 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audit_events/types/actor.py
+-rw-r--r--   0        0        0     1484 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audit_events/types/audit_event.py
+-rw-r--r--   0        0        0     1308 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audit_events/types/get_audit_event_params.py
+-rw-r--r--   0        0        0     1206 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audit_events/types/list_audit_events_params.py
+-rw-r--r--   0        0        0     1303 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audit_events/types/list_audit_events_response.py
+-rw-r--r--   0        0        0     1226 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/audit_events/types/target.py
+-rw-r--r--   0        0        0      137 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/auth_tokens/__init__.py
+-rw-r--r--   0        0        0     7458 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/auth_tokens/client.py
+-rw-r--r--   0        0        0      152 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/auth_tokens/types/__init__.py
+-rw-r--r--   0        0        0     1202 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/auth_tokens/types/issue_token_response.py
+-rw-r--r--   0        0        0     1847 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/__init__.py
+-rw-r--r--   0        0        0    17316 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/client.py
+-rw-r--r--   0        0        0     2836 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/__init__.py
+-rw-r--r--   0        0        0     1282 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/accessor_type.py
+-rw-r--r--   0        0        0     1308 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation.py
+-rw-r--r--   0        0        0     1317 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_ad_hoc_invoke_params.py
+-rw-r--r--   0        0        0      138 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_add_to_batch_max_items_type.py
+-rw-r--r--   0        0        0     2274 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_add_to_batch_retain.py
+-rw-r--r--   0        0        0      192 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_add_to_batch_retain_type.py
+-rw-r--r--   0        0        0      178 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_add_to_batch_scope.py
+-rw-r--r--   0        0        0     3391 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_add_to_batch_step.py
+-rw-r--r--   0        0        0     1618 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_add_to_digest_step.py
+-rw-r--r--   0        0        0     1311 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_cancel_step.py
+-rw-r--r--   0        0        0     1594 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_delay_step.py
+-rw-r--r--   0        0        0     2047 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_fetch_data_step.py
+-rw-r--r--   0        0        0     1506 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_fetch_data_webhook.py
+-rw-r--r--   0        0        0      171 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_fetch_data_webhook_method.py
+-rw-r--r--   0        0        0     1428 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_invoke_params.py
+-rw-r--r--   0        0        0     1298 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_invoke_response.py
+-rw-r--r--   0        0        0     1278 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_invoke_step.py
+-rw-r--r--   0        0        0     1319 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_invoke_template_params.py
+-rw-r--r--   0        0        0     1408 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_run_context.py
+-rw-r--r--   0        0        0     1525 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_send_list_step.py
+-rw-r--r--   0        0        0     1558 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_send_step.py
+-rw-r--r--   0        0        0     1350 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_step.py
+-rw-r--r--   0        0        0     1102 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_step_option.py
+-rw-r--r--   0        0        0     1372 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_throttle_on_throttle.py
+-rw-r--r--   0        0        0      176 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_throttle_scope.py
+-rw-r--r--   0        0        0     2564 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_throttle_step.py
+-rw-r--r--   0        0        0     1359 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_update_profile_step.py
+-rw-r--r--   0        0        0     1321 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/automation_v_2_send_step.py
+-rw-r--r--   0        0        0      184 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/merge_algorithm.py
+-rw-r--r--   0        0        0      101 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/automations/types/profile.py
+-rw-r--r--   0        0        0      419 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/brands/__init__.py
+-rw-r--r--   0        0        0    31692 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/brands/client.py
+-rw-r--r--   0        0        0      579 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/brands/types/__init__.py
+-rw-r--r--   0        0        0     2036 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/brands/types/brand.py
+-rw-r--r--   0        0        0     1282 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/brands/types/brand_colors.py
+-rw-r--r--   0        0        0     1283 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/brands/types/brand_get_all_response.py
+-rw-r--r--   0        0        0     1440 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/brands/types/brand_parameters.py
+-rw-r--r--   0        0        0     1372 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/brands/types/brand_settings.py
+-rw-r--r--   0        0        0     1227 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/brands/types/brand_snippet.py
+-rw-r--r--   0        0        0     1235 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/brands/types/brand_snippets.py
+-rw-r--r--   0        0        0     1278 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/brands/types/brands_response.py
+-rw-r--r--   0        0        0     1059 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/bulk/__init__.py
+-rw-r--r--   0        0        0    32193 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/bulk/client.py
+-rw-r--r--   0        0        0     1603 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/bulk/types/__init__.py
+-rw-r--r--   0        0        0     1295 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/bulk/types/bulk_create_job_response.py
+-rw-r--r--   0        0        0     1290 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/bulk/types/bulk_get_job_params.py
+-rw-r--r--   0        0        0     1219 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/bulk/types/bulk_get_job_response.py
+-rw-r--r--   0        0        0     1335 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/bulk/types/bulk_get_job_users_params.py
+-rw-r--r--   0        0        0     1342 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/bulk/types/bulk_get_job_users_response.py
+-rw-r--r--   0        0        0     1203 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/bulk/types/bulk_ingest_error.py
+-rw-r--r--   0        0        0     1275 2024-05-23 13:24:57.205938 trycourier-6.1.0/src/courier/bulk/types/bulk_ingest_users_params.py
+-rw-r--r--   0        0        0     1295 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/bulk/types/bulk_ingest_users_response.py
+-rw-r--r--   0        0        0      184 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/bulk/types/bulk_job_status.py
+-rw-r--r--   0        0        0      173 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/bulk/types/bulk_job_user_status.py
+-rw-r--r--   0        0        0     1424 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/bulk/types/bulk_message_user_response.py
+-rw-r--r--   0        0        0     1775 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/bulk/types/inbound_bulk_content_message.py
+-rw-r--r--   0        0        0     1359 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/bulk/types/inbound_bulk_message.py
+-rw-r--r--   0        0        0     1538 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/bulk/types/inbound_bulk_message_user.py
+-rw-r--r--   0        0        0     1992 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/bulk/types/inbound_bulk_message_v_1.py
+-rw-r--r--   0        0        0      310 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/bulk/types/inbound_bulk_message_v_2.py
+-rw-r--r--   0        0        0     1428 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/bulk/types/inbound_bulk_template_message.py
+-rw-r--r--   0        0        0     1366 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/bulk/types/job_details.py
+-rw-r--r--   0        0        0    17721 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/client.py
+-rw-r--r--   0        0        0     1127 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/__init__.py
+-rw-r--r--   0        0        0      527 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/errors/__init__.py
+-rw-r--r--   0        0        0      289 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/errors/already_exists_error.py
+-rw-r--r--   0        0        0      277 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/errors/bad_request_error.py
+-rw-r--r--   0        0        0      268 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/errors/conflict_error.py
+-rw-r--r--   0        0        0      298 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/errors/message_not_found_error.py
+-rw-r--r--   0        0        0      269 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/errors/not_found_error.py
+-rw-r--r--   0        0        0      297 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/errors/payment_required_error.py
+-rw-r--r--   0        0        0     1207 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/already_exists.py
+-rw-r--r--   0        0        0     1248 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/bad_request.py
+-rw-r--r--   0        0        0     1259 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/base_error.py
+-rw-r--r--   0        0        0      213 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/channel_classification.py
+-rw-r--r--   0        0        0     1255 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/channel_preference.py
+-rw-r--r--   0        0        0     1246 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/conflict.py
+-rw-r--r--   0        0        0     1196 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/email.py
+-rw-r--r--   0        0        0     1253 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/message_not_found.py
+-rw-r--r--   0        0        0     1246 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/not_found.py
+-rw-r--r--   0        0        0     1457 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/notification_preference_details.py
+-rw-r--r--   0        0        0      230 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/notification_preferences.py
+-rw-r--r--   0        0        0     1206 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/paging.py
+-rw-r--r--   0        0        0     1251 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/payment_required.py
+-rw-r--r--   0        0        0      177 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/preference_status.py
+-rw-r--r--   0        0        0     1358 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/recipient_preferences.py
+-rw-r--r--   0        0        0     1203 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/rule.py
+-rw-r--r--   0        0        0     1673 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/commons/types/user_tenant_association.py
+-rw-r--r--   0        0        0     1126 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/core/api_error.py
+-rw-r--r--   0        0        0     2088 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      748 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/core/pydantic_utilities.py
+-rw-r--r--   0        0        0     1266 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/core/query_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/core/request_options.py
+-rw-r--r--   0        0        0     8148 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      159 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/environment.py
+-rw-r--r--   0        0        0      413 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/lists/__init__.py
+-rw-r--r--   0        0        0    72964 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/lists/client.py
+-rw-r--r--   0        0        0      570 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/lists/types/__init__.py
+-rw-r--r--   0        0        0     1257 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/lists/types/list_.py
+-rw-r--r--   0        0        0     1278 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/lists/types/list_get_all_response.py
+-rw-r--r--   0        0        0     1352 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/lists/types/list_get_subscriptions_response.py
+-rw-r--r--   0        0        0     1306 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/lists/types/list_put_params.py
+-rw-r--r--   0        0        0     1486 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/lists/types/list_subscription_recipient.py
+-rw-r--r--   0        0        0     1445 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/lists/types/put_subscriptions_recipient.py
+-rw-r--r--   0        0        0      527 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/messages/__init__.py
+-rw-r--r--   0        0        0    43247 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/messages/client.py
+-rw-r--r--   0        0        0      747 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/messages/types/__init__.py
+-rw-r--r--   0        0        0     1477 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/messages/types/list_messages_response.py
+-rw-r--r--   0        0        0     3131 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/messages/types/message_details.py
+-rw-r--r--   0        0        0     1222 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/messages/types/message_history_response.py
+-rw-r--r--   0        0        0      357 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/messages/types/message_status.py
+-rw-r--r--   0        0        0      233 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/messages/types/reason.py
+-rw-r--r--   0        0        0     1554 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/messages/types/render_output.py
+-rw-r--r--   0        0        0     1342 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/messages/types/render_output_response.py
+-rw-r--r--   0        0        0     1370 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/messages/types/rendered_message_block.py
+-rw-r--r--   0        0        0     1819 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/messages/types/rendered_message_content.py
+-rw-r--r--   0        0        0     1081 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/__init__.py
+-rw-r--r--   0        0        0    46792 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/client.py
+-rw-r--r--   0        0        0     1614 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/__init__.py
+-rw-r--r--   0        0        0     1263 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/base_check.py
+-rw-r--r--   0        0        0      229 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/block_type.py
+-rw-r--r--   0        0        0     1210 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/check.py
+-rw-r--r--   0        0        0      168 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/check_status.py
+-rw-r--r--   0        0        0     1447 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/message_routing.py
+-rw-r--r--   0        0        0      183 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/message_routing_channel.py
+-rw-r--r--   0        0        0      161 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/message_routing_method.py
+-rw-r--r--   0        0        0     1434 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/notification.py
+-rw-r--r--   0        0        0     1536 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/notification_block.py
+-rw-r--r--   0        0        0     1471 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/notification_channel.py
+-rw-r--r--   0        0        0     1251 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/notification_channel_content.py
+-rw-r--r--   0        0        0      224 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/notification_content.py
+-rw-r--r--   0        0        0     1255 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/notification_content_hierarchy.py
+-rw-r--r--   0        0        0     1459 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/notification_get_content_response.py
+-rw-r--r--   0        0        0     1309 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/notification_list_response.py
+-rw-r--r--   0        0        0     1258 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/notification_tag.py
+-rw-r--r--   0        0        0     1190 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/notification_tag_data.py
+-rw-r--r--   0        0        0     1228 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/submission_checks_get_response.py
+-rw-r--r--   0        0        0     1232 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/notifications/types/submission_checks_replace_response.py
+-rw-r--r--   0        0        0     1877 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/__init__.py
+-rw-r--r--   0        0        0    45944 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/client.py
+-rw-r--r--   0        0        0     2897 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/__init__.py
+-rw-r--r--   0        0        0     1267 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/address.py
+-rw-r--r--   0        0        0     1335 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/airship_profile.py
+-rw-r--r--   0        0        0     1187 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/airship_profile_audience.py
+-rw-r--r--   0        0        0     1213 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/delete_list_subscription_response.py
+-rw-r--r--   0        0        0      104 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/device_type.py
+-rw-r--r--   0        0        0      232 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/discord.py
+-rw-r--r--   0        0        0      193 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/expo.py
+-rw-r--r--   0        0        0     1668 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/get_list_subscriptions_list.py
+-rw-r--r--   0        0        0     1412 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/get_list_subscriptions_response.py
+-rw-r--r--   0        0        0     1356 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/intercom.py
+-rw-r--r--   0        0        0     1174 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/intercom_recipient.py
+-rw-r--r--   0        0        0     1203 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/merge_profile_response.py
+-rw-r--r--   0        0        0      566 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/ms_teams.py
+-rw-r--r--   0        0        0     1206 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/ms_teams_base_properties.py
+-rw-r--r--   0        0        0     1215 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/multiple_tokens.py
+-rw-r--r--   0        0        0     1306 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/profile_get_parameters.py
+-rw-r--r--   0        0        0     1339 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/profile_get_response.py
+-rw-r--r--   0        0        0     1205 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/replace_profile_response.py
+-rw-r--r--   0        0        0     1179 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/send_direct_message.py
+-rw-r--r--   0        0        0     1178 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/send_to_channel.py
+-rw-r--r--   0        0        0     1268 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/send_to_ms_teams_channel_id.py
+-rw-r--r--   0        0        0     1289 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/send_to_ms_teams_channel_name.py
+-rw-r--r--   0        0        0     1278 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/send_to_ms_teams_conversation_id.py
+-rw-r--r--   0        0        0     1259 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/send_to_ms_teams_email.py
+-rw-r--r--   0        0        0     1262 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/send_to_ms_teams_user_id.py
+-rw-r--r--   0        0        0     1254 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/send_to_slack_channel.py
+-rw-r--r--   0        0        0     1250 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/send_to_slack_email.py
+-rw-r--r--   0        0        0     1253 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/send_to_slack_user_id.py
+-rw-r--r--   0        0        0      316 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/slack.py
+-rw-r--r--   0        0        0     1186 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/slack_base_properties.py
+-rw-r--r--   0        0        0     1255 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/snooze_rule.py
+-rw-r--r--   0        0        0      148 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/snooze_rule_type.py
+-rw-r--r--   0        0        0     1312 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/subscribe_to_lists_request.py
+-rw-r--r--   0        0        0     1443 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/subscribe_to_lists_request_list_object.py
+-rw-r--r--   0        0        0     1207 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/subscribe_to_lists_response.py
+-rw-r--r--   0        0        0     1165 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/token.py
+-rw-r--r--   0        0        0     2346 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/profiles/types/user_profile.py
+-rw-r--r--   0        0        0        0 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/py.typed
+-rw-r--r--   0        0        0     4101 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/__init__.py
+-rw-r--r--   0        0        0     6149 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/__init__.py
+-rw-r--r--   0        0        0      122 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/attachment.py
+-rw-r--r--   0        0        0     1351 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/audience_filter.py
+-rw-r--r--   0        0        0     1521 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/audience_recipient.py
+-rw-r--r--   0        0        0     3281 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/base_message.py
+-rw-r--r--   0        0        0     1359 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/base_message_send_to.py
+-rw-r--r--   0        0        0     1176 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/base_social_presence.py
+-rw-r--r--   0        0        0     1686 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/brand_settings_email.py
+-rw-r--r--   0        0        0     1957 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/brand_settings_in_app.py
+-rw-r--r--   0        0        0     1687 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/brand_settings_social_presence.py
+-rw-r--r--   0        0        0     1628 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/brand_template.py
+-rw-r--r--   0        0        0     1464 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/brand_template_override.py
+-rw-r--r--   0        0        0     2679 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/channel.py
+-rw-r--r--   0        0        0     1218 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/channel_metadata.py
+-rw-r--r--   0        0        0      174 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/channel_source.py
+-rw-r--r--   0        0        0      252 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/content.py
+-rw-r--r--   0        0        0     1809 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/content_message.py
+-rw-r--r--   0        0        0      183 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/criteria.py
+-rw-r--r--   0        0        0     1253 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/delay.py
+-rw-r--r--   0        0        0     2394 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/elemental_action_node.py
+-rw-r--r--   0        0        0     1446 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/elemental_base_node.py
+-rw-r--r--   0        0        0     2787 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/elemental_channel_node.py
+-rw-r--r--   0        0        0     1376 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/elemental_content.py
+-rw-r--r--   0        0        0     1500 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/elemental_content_sugar.py
+-rw-r--r--   0        0        0     1441 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/elemental_divider_node.py
+-rw-r--r--   0        0        0     1712 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/elemental_group_node.py
+-rw-r--r--   0        0        0     1952 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/elemental_image_node.py
+-rw-r--r--   0        0        0     1647 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/elemental_meta_node.py
+-rw-r--r--   0        0        0     8164 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/elemental_node.py
+-rw-r--r--   0        0        0     1960 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/elemental_quote_node.py
+-rw-r--r--   0        0        0     2722 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/elemental_text_node.py
+-rw-r--r--   0        0        0     1383 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/email_footer.py
+-rw-r--r--   0        0        0     1343 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/email_head.py
+-rw-r--r--   0        0        0     1461 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/email_header.py
+-rw-r--r--   0        0        0      119 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/expires_in_type.py
+-rw-r--r--   0        0        0     1577 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/expiry.py
+-rw-r--r--   0        0        0      160 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/i_action_button_style.py
+-rw-r--r--   0        0        0      169 2024-05-23 13:24:57.209938 trycourier-6.1.0/src/courier/send/types/i_alignment.py
+-rw-r--r--   0        0        0      160 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/i_preferences.py
+-rw-r--r--   0        0        0     1459 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/i_profile_preferences.py
+-rw-r--r--   0        0        0     1229 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/icons.py
+-rw-r--r--   0        0        0      172 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/in_app_placement.py
+-rw-r--r--   0        0        0     1206 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/invalid_list_pattern_recipient.py
+-rw-r--r--   0        0        0     1204 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/invalid_list_recipient.py
+-rw-r--r--   0        0        0     1204 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/invalid_user_recipient.py
+-rw-r--r--   0        0        0     1347 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/list_filter.py
+-rw-r--r--   0        0        0     1385 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/list_pattern_recipient.py
+-rw-r--r--   0        0        0     1168 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/list_pattern_recipient_type.py
+-rw-r--r--   0        0        0     1448 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/list_recipient.py
+-rw-r--r--   0        0        0     1161 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/list_recipient_type.py
+-rw-r--r--   0        0        0     1168 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/locale.py
+-rw-r--r--   0        0        0      160 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/locales.py
+-rw-r--r--   0        0        0     1226 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/logo.py
+-rw-r--r--   0        0        0      227 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/message.py
+-rw-r--r--   0        0        0     1822 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/message_channel_email_override.py
+-rw-r--r--   0        0        0      154 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/message_channels.py
+-rw-r--r--   0        0        0     1443 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/message_context.py
+-rw-r--r--   0        0        0      123 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/message_data.py
+-rw-r--r--   0        0        0     2043 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/message_metadata.py
+-rw-r--r--   0        0        0      196 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/message_providers.py
+-rw-r--r--   0        0        0     1797 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/message_providers_type.py
+-rw-r--r--   0        0        0      181 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/message_recipient.py
+-rw-r--r--   0        0        0     1211 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/metadata.py
+-rw-r--r--   0        0        0     1230 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/ms_teams_recipient.py
+-rw-r--r--   0        0        0      193 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/override.py
+-rw-r--r--   0        0        0     1578 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/preference.py
+-rw-r--r--   0        0        0     1310 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/preferences.py
+-rw-r--r--   0        0        0      583 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/recipient.py
+-rw-r--r--   0        0        0      125 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/recipient_data.py
+-rw-r--r--   0        0        0     1782 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/routing.py
+-rw-r--r--   0        0        0      289 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/routing_channel.py
+-rw-r--r--   0        0        0      154 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/routing_method.py
+-rw-r--r--   0        0        0     1599 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/routing_strategy_channel.py
+-rw-r--r--   0        0        0     1455 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/routing_strategy_provider.py
+-rw-r--r--   0        0        0      175 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/rule_type.py
+-rw-r--r--   0        0        0     1218 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/slack_recipient.py
+-rw-r--r--   0        0        0     1475 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/template_message.py
+-rw-r--r--   0        0        0      160 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/text_align.py
+-rw-r--r--   0        0        0      164 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/text_style.py
+-rw-r--r--   0        0        0     1434 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/timeout.py
+-rw-r--r--   0        0        0     1236 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/timeouts.py
+-rw-r--r--   0        0        0     1176 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/tracking_override.py
+-rw-r--r--   0        0        0     2298 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/user_recipient.py
+-rw-r--r--   0        0        0     1161 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/user_recipient_type.py
+-rw-r--r--   0        0        0     1349 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/utm.py
+-rw-r--r--   0        0        0     1421 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/send/types/widget_background.py
+-rw-r--r--   0        0        0      411 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/templates/__init__.py
+-rw-r--r--   0        0        0     6163 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/templates/client.py
+-rw-r--r--   0        0        0      564 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/templates/types/__init__.py
+-rw-r--r--   0        0        0       89 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/templates/types/channel_identifier.py
+-rw-r--r--   0        0        0     1411 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/templates/types/list_templates_response.py
+-rw-r--r--   0        0        0     2101 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/templates/types/notification_templates.py
+-rw-r--r--   0        0        0     1671 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/templates/types/routing_strategy.py
+-rw-r--r--   0        0        0      162 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/templates/types/routing_strategy_method.py
+-rw-r--r--   0        0        0     1209 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/templates/types/tag.py
+-rw-r--r--   0        0        0     1312 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/templates/types/tag_data.py
+-rw-r--r--   0        0        0      503 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/tenants/__init__.py
+-rw-r--r--   0        0        0    44657 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/tenants/client.py
+-rw-r--r--   0        0        0      709 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/tenants/types/__init__.py
+-rw-r--r--   0        0        0     1279 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/tenants/types/default_preferences.py
+-rw-r--r--   0        0        0     2057 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/tenants/types/list_users_for_tenant_response.py
+-rw-r--r--   0        0        0     1302 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/tenants/types/subscription_topic.py
+-rw-r--r--   0        0        0     1800 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/tenants/types/subscription_topic_new.py
+-rw-r--r--   0        0        0      184 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/tenants/types/subscription_topic_status.py
+-rw-r--r--   0        0        0      110 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/tenants/types/template_property.py
+-rw-r--r--   0        0        0     2188 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/tenants/types/tenant.py
+-rw-r--r--   0        0        0     2018 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/tenants/types/tenant_list_response.py
+-rw-r--r--   0        0        0       65 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/translations/__init__.py
+-rw-r--r--   0        0        0    11799 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/translations/client.py
+-rw-r--r--   0        0        0      155 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/types/__init__.py
+-rw-r--r--   0        0        0     1911 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/types/send_message_response.py
+-rw-r--r--   0        0        0     1354 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/__init__.py
+-rw-r--r--   0        0        0     1067 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/client.py
+-rw-r--r--   0        0        0      409 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/preferences/__init__.py
+-rw-r--r--   0        0        0    19441 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/preferences/client.py
+-rw-r--r--   0        0        0      561 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/preferences/types/__init__.py
+-rw-r--r--   0        0        0     1666 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/preferences/types/topic_preference.py
+-rw-r--r--   0        0        0     1597 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/preferences/types/topic_preference_update.py
+-rw-r--r--   0        0        0     1247 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/preferences/types/user_preferences_get_response.py
+-rw-r--r--   0        0        0     1411 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/preferences/types/user_preferences_list_response.py
+-rw-r--r--   0        0        0     1194 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/preferences/types/user_preferences_update_response.py
+-rw-r--r--   0        0        0      229 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tenants/__init__.py
+-rw-r--r--   0        0        0    30238 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tenants/client.py
+-rw-r--r--   0        0        0      308 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tenants/types/__init__.py
+-rw-r--r--   0        0        0     1718 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py
+-rw-r--r--   0        0        0     2061 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tenants/types/list_tenants_for_user_response.py
+-rw-r--r--   0        0        0      765 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/__init__.py
+-rw-r--r--   0        0        0    30782 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/client.py
+-rw-r--r--   0        0        0     1135 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/__init__.py
+-rw-r--r--   0        0        0     1199 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/delete_user_token_opts.py
+-rw-r--r--   0        0        0     1897 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/device.py
+-rw-r--r--   0        0        0      117 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/expiry_date.py
+-rw-r--r--   0        0        0      161 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/get_all_tokens_response.py
+-rw-r--r--   0        0        0     1196 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/get_user_token_opts.py
+-rw-r--r--   0        0        0     1423 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/get_user_token_response.py
+-rw-r--r--   0        0        0     1182 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/get_user_tokens_opts.py
+-rw-r--r--   0        0        0      183 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/patch_op.py
+-rw-r--r--   0        0        0     1479 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/patch_operation.py
+-rw-r--r--   0        0        0     1249 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/patch_user_token_opts.py
+-rw-r--r--   0        0        0      179 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/provider_key.py
+-rw-r--r--   0        0        0     1236 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/put_user_token_opts.py
+-rw-r--r--   0        0        0     1251 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/put_user_tokens_opts.py
+-rw-r--r--   0        0        0      177 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/token_status.py
+-rw-r--r--   0        0        0     1708 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/tracking.py
+-rw-r--r--   0        0        0     2111 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/users/tokens/types/user_token.py
+-rw-r--r--   0        0        0       78 2024-05-23 13:24:57.213938 trycourier-6.1.0/src/courier/version.py
+-rw-r--r--   0        0        0     6341 1970-01-01 00:00:00.000000 trycourier-6.1.0/PKG-INFO
```

### Comparing `trycourier-6.0.5/LICENSE` & `trycourier-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/README.md` & `trycourier-6.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,164 +7,159 @@
 
 ## Installation
 
 Install from PyPI
 
 ```shell
 pip install trycourier
-# or 
+# or
 poetry add trycourier
 ```
 
 Python 3.7 or later is required.
 
 ## Usage
+
 Use the `Courier` class to access all of our endpoints.
 
 ```python
-import os
 import courier
 
 from courier.client import Courier
 
 client = Courier(
   authorization_token="YOUR_TOKENY" # Defaults to COURIER_AUTH_TOKEN
 )
 
 response = client.send(
   message=courier.ContentMessage(
     to=courier.UserRecipient(
       email="marty_mcfly@email.com",
       data={
-        name: "Marty",
+        "name": "Marty",
       }
     ),
     content=courier.ElementalContentSugar(
       title="Back to the Future",
-      body="Oh my {{name}}, we need 1.21 Gigawatts!",
+      body="Oh my {name}, we need 1.21 Gigawatts!",
     ),
-    routing=courier.Routing(
-      method=courier.RoutingMethod.ALL,
-      channels=["email"]
-    )
+    routing=courier.Routing(method="all", channels=["inbox", "email"]),
   )
 )
 
 print(response)
 ```
 
 ## Async Client
-The SDK also exports an asynchronous client, `AsyncCourier`. 
+
+The SDK also exports an asynchronous client, `AsyncCourier`.
 
 ```python
 import os
 import courier
 import asyncio
 
 from courier.client import AsyncCourier
 
 client = AsyncCourier(
   authorization_token="YOUR_TOKEN" # Defaults to COURIER_AUTH_TOKEN
 )
 
-async def main() -> None: 
+async def main() -> None:
   response = await client.send(
     message=courier.ContentMessage(
       to=courier.UserRecipient(
         email="marty_mcfly@email.com",
         data={
-          name: "Marty",
+          "name": "Marty",
         }
       ),
       content=courier.ElementalContentSugar(
         title="Back to the Future",
-        body="Oh my {{name}}, we need 1.21 Gigawatts!",
+        body="Oh my {name}, we need 1.21 Gigawatts!",
       ),
-      routing=courier.Routing(
-        method=courier.RoutingMethod.ALL,
-        channels=["email"]
-      )
+      routing=courier.Routing(method="all", channels=["email", "inbox"]),
     )
   )
 
 asyncio.run(main())
 ```
 
 ## Timeouts
-By default, the client is configured to have a timeout of 60 seconds. 
-You can customize this value at client instantiation. 
+
+By default, the client is configured to have a timeout of 60 seconds.
+You can customize this value at client instantiation.
 
 ```python
 from courier.client import Courier
 
 client = Courier(
   authorization_token="YOUR_TOKEN",
   timeout=30
 )
 ```
 
 ## Handling Exceptions
-All exceptions thrown by the SDK will sublcass [courier.ApiError](./src/courier/core/api_error.py). 
+
+All exceptions thrown by the SDK will subclass [courier.ApiError](./src/courier/core/api_error.py).
 
 ```python
 import courier
 
 from courier.core import ApiError
 
 try:
   courier.send(...)
-except APIError as e:  
+except APIError as e:
   # handle any api related error
 ```
 
 ## Idempotency Keys
 
-For `POST` methods, you can supply an `idempotencyKey` in the config parameter to 
-ensure the idempotency of the API Call. We recommend that you use a `V4 UUID` for the key. 
-Keys are eligible to be removed from the system after they're at least 24 hours old, 
-and a new request is generated if a key is reused after the original has been removed. 
-For more info, see [Idempotent Requests](https://docs.courier.com/reference/idempotent-requests) 
+For `POST` methods, you can supply an `idempotencyKey` in the config parameter to
+ensure the idempotency of the API Call. We recommend that you use a `V4 UUID` for the key.
+Keys are eligible to be removed from the system after they're at least 24 hours old,
+and a new request is generated if a key is reused after the original has been removed.
+For more info, see [Idempotent Requests](https://docs.courier.com/reference/idempotent-requests)
 in the Courier documentation.
 
 ```python
 import courier
 
 courier.send(
-  message={...}, 
-  idempotency_key"YOUR_KEY", 
+  message={...},
+  idempotency_key"YOUR_KEY",
   idempotency_expiration="YOUR_EXPIRATION")
 ```
 
 ## Additional Usage Examples
 
 ### Send Template Message
 
 ```python
 import courier
-
-from courier import Courier
+from courier.client import Courier
 
 client = Courier(
   authorization_token="YOUR_TOKEN")
 
 response = client.send(
     message=courier.TemplateMessage(
       template="my-template",
-      to=courier.UserRecipient(email="foo@bar.com")
+      to=courier.UserRecipient(user_id="abc-123")
     )
 )
-print(response.message_id)
+print(response.request_id)
 ```
 
 ### UTM Metadata with Message
 
 ```python
 import courier
-
-from courier import Courier
+from courier.client import Courier
 
 client = Courier(
   authorization_token="YOUR_TOKEN")
 
 response = client.send(
     message=courier.ContentMessage(
       content=courier.ElementalContent(
@@ -175,33 +170,31 @@
             href="courier.com",
             style="button",
             align="center"
           )
         ]
       ),
       to=courier.UserRecipient(email="foo@bar.com"),
-      routing=courier.Routing(
-        method=courier.RoutingMethod.SINGLE,
-        channels=["email"]
-      ),
+      routing=courier.Routing(method="all", channels=["email"]),
       metadata=courier.MessageMetadata(
         utm=courier.Utm(source="python")
       )
     )
 )
 print(response.request_id)
 ```
 
 ## Advanced
 
 ### Overriding HTTP Client
-You can override the httpx client to customize it for your use case. Some common usecases 
+
+You can override the httpx client to customize it for your use case. Some common usecases
 include support for proxies and transports.
 
-```python 
+```python
 import httpx
 from courier.client import Courier
 
 client = Courier(
     http_client=httpx.Client(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
```

### Comparing `trycourier-6.0.5/src/courier/__init__.py` & `trycourier-6.1.0/src/courier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,14 +308,15 @@
     Tag,
     TagData,
 )
 from .tenants import (
     DefaultPreferences,
     ListUsersForTenantResponse,
     SubscriptionTopic,
+    SubscriptionTopicNew,
     SubscriptionTopicStatus,
     TemplateProperty,
     Tenant,
     TenantListResponse,
 )
 from .version import __version__
 
@@ -576,14 +577,15 @@
     "SnoozeRuleType",
     "SubmissionChecksGetResponse",
     "SubmissionChecksReplaceResponse",
     "SubscribeToListsRequest",
     "SubscribeToListsRequestListObject",
     "SubscribeToListsResponse",
     "SubscriptionTopic",
+    "SubscriptionTopicNew",
     "SubscriptionTopicStatus",
     "Tag",
     "TagData",
     "Target",
     "TemplateMessage",
     "TemplateProperty",
     "Tenant",
```

### Comparing `trycourier-6.0.5/src/courier/audiences/__init__.py` & `trycourier-6.1.0/src/courier/audiences/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/audiences/client.py` & `trycourier-6.1.0/src/courier/audiences/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from json.decoder import JSONDecodeError
 
 from ..commons.errors.bad_request_error import BadRequestError
 from ..commons.types.bad_request import BadRequest
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from .types.audience import Audience
 from .types.audience_list_response import AudienceListResponse
 from .types.audience_member_list_response import AudienceMemberListResponse
 from .types.audience_update_response import AudienceUpdateResponse
 from .types.filter import Filter
 
 # this is used as the default value for optional parameters
@@ -54,16 +55,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -72,15 +75,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Audience, _response.json())  # type: ignore
+            return typing.cast(Audience, construct_type(type_=Audience, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
@@ -142,16 +145,18 @@
         if filter is not OMIT:
             _request["filter"] = filter
         _response = self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -166,15 +171,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(AudienceUpdateResponse, _response.json())  # type: ignore
+            return typing.cast(AudienceUpdateResponse, construct_type(type_=AudienceUpdateResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, audience_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
@@ -205,17 +210,22 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -272,24 +282,26 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}/members"
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -299,17 +311,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(AudienceMemberListResponse, _response.json())  # type: ignore
+            return typing.cast(AudienceMemberListResponse, construct_type(type_=AudienceMemberListResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list_audiences(
@@ -340,24 +354,26 @@
         client.audiences.list_audiences(
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audiences"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -367,17 +383,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(AudienceListResponse, _response.json())  # type: ignore
+            return typing.cast(AudienceListResponse, construct_type(type_=AudienceListResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -413,16 +431,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -431,15 +451,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Audience, _response.json())  # type: ignore
+            return typing.cast(Audience, construct_type(type_=Audience, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
@@ -501,16 +521,18 @@
         if filter is not OMIT:
             _request["filter"] = filter
         _response = await self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -525,15 +547,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(AudienceUpdateResponse, _response.json())  # type: ignore
+            return typing.cast(AudienceUpdateResponse, construct_type(type_=AudienceUpdateResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, audience_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
@@ -564,17 +586,22 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -631,24 +658,26 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}/members"
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -658,17 +687,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(AudienceMemberListResponse, _response.json())  # type: ignore
+            return typing.cast(AudienceMemberListResponse, construct_type(type_=AudienceMemberListResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list_audiences(
@@ -699,24 +730,26 @@
         await client.audiences.list_audiences(
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audiences"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -726,15 +759,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(AudienceListResponse, _response.json())  # type: ignore
+            return typing.cast(AudienceListResponse, construct_type(type_=AudienceListResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/audiences/types/__init__.py` & `trycourier-6.1.0/src/courier/audiences/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/audiences/types/audience.py` & `trycourier-6.1.0/src/courier/audiences/types/single_filter_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .filter import Filter
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .base_filter_config import BaseFilterConfig
 
 
-class Audience(pydantic_v1.BaseModel):
-    id: str = pydantic_v1.Field()
+class SingleFilterConfig(BaseFilterConfig):
     """
-    A unique identifier representing the audience_id
+    A single filter to use for filtering
     """
 
-    name: str = pydantic_v1.Field()
+    value: str = pydantic_v1.Field()
     """
-    The name of the audience
+    The value to use for filtering
     """
 
-    description: str = pydantic_v1.Field()
+    path: str = pydantic_v1.Field()
     """
-    A description of the audience
+    The attribe name from profile whose value will be operated against the filter value
     """
 
-    filter: Filter
-    created_at: str
-    updated_at: str
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/audiences/types/audience_list_response.py` & `trycourier-6.1.0/src/courier/brands/types/brand_get_all_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .audience import Audience
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .brand import Brand
 
 
-class AudienceListResponse(pydantic_v1.BaseModel):
-    items: typing.List[Audience]
+class BrandGetAllResponse(UncheckedBaseModel):
     paging: Paging
+    results: typing.List[Brand]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/audiences/types/audience_member.py` & `trycourier-6.1.0/src/courier/profiles/types/send_to_ms_teams_conversation_id.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .ms_teams_base_properties import MsTeamsBaseProperties
 
 
-class AudienceMember(pydantic_v1.BaseModel):
-    added_at: str
-    audience_id: str
-    audience_version: int
-    member_id: str
-    reason: str
+class SendToMsTeamsConversationId(MsTeamsBaseProperties):
+    conversation_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/audiences/types/audience_member_get_response.py` & `trycourier-6.1.0/src/courier/commons/types/bad_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .audience_member import AudienceMember
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .base_error import BaseError
 
 
-class AudienceMemberGetResponse(pydantic_v1.BaseModel):
-    audience_member: AudienceMember = pydantic_v1.Field(alias="audienceMember")
+class BadRequest(BaseError):
+    type: typing.Literal["invalid_request_error"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/audiences/types/audience_member_list_response.py` & `trycourier-6.1.0/src/courier/bulk/types/bulk_get_job_users_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .audience_member import AudienceMember
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .bulk_message_user_response import BulkMessageUserResponse
 
 
-class AudienceMemberListResponse(pydantic_v1.BaseModel):
-    items: typing.List[AudienceMember]
+class BulkGetJobUsersResponse(UncheckedBaseModel):
+    items: typing.List[BulkMessageUserResponse]
     paging: Paging
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/audiences/types/audience_update_response.py` & `trycourier-6.1.0/src/courier/audiences/types/audience_update_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .audience import Audience
 
 
-class AudienceUpdateResponse(pydantic_v1.BaseModel):
+class AudienceUpdateResponse(UncheckedBaseModel):
     audience: Audience
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/audiences/types/base_filter_config.py` & `trycourier-6.1.0/src/courier/messages/types/render_output_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .operator import Operator
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .render_output import RenderOutput
 
 
-class BaseFilterConfig(pydantic_v1.BaseModel):
-    operator: Operator = pydantic_v1.Field()
+class RenderOutputResponse(UncheckedBaseModel):
+    results: typing.List[RenderOutput] = pydantic_v1.Field()
     """
-    The operator to use for filtering
+    An array of render output of a previously sent message.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/audiences/types/nested_filter_config.py` & `trycourier-6.1.0/src/courier/audiences/types/audience.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from __future__ import annotations
-
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .base_filter_config import BaseFilterConfig
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .filter import Filter
+
+
+class Audience(UncheckedBaseModel):
+    id: str = pydantic_v1.Field()
+    """
+    A unique identifier representing the audience_id
+    """
 
+    name: str = pydantic_v1.Field()
+    """
+    The name of the audience
+    """
 
-class NestedFilterConfig(BaseFilterConfig):
+    description: str = pydantic_v1.Field()
     """
-    The operator to use for filtering
+    A description of the audience
     """
 
-    rules: typing.List[FilterConfig]
+    filter: Filter
+    created_at: str
+    updated_at: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
-
-
-from .filter_config import FilterConfig  # noqa: E402
-
-NestedFilterConfig.update_forward_refs()
```

### Comparing `trycourier-6.0.5/src/courier/audiences/types/single_filter_config.py` & `trycourier-6.1.0/src/courier/automations/types/automation_invoke_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .base_filter_config import BaseFilterConfig
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class SingleFilterConfig(BaseFilterConfig):
-    """
-    A single filter to use for filtering
-    """
-
-    value: str = pydantic_v1.Field()
-    """
-    The value to use for filtering
-    """
-
-    path: str = pydantic_v1.Field()
-    """
-    The attribe name from profile whose value will be operated against the filter value
-    """
+class AutomationInvokeResponse(UncheckedBaseModel):
+    run_id: str = pydantic_v1.Field(alias="runId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/audit_events/client.py` & `trycourier-6.1.0/src/courier/audit_events/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from .types.audit_event import AuditEvent
 from .types.list_audit_events_response import ListAuditEventsResponse
 
 
 class AuditEventsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(
+    def list_(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> ListAuditEventsResponse:
         """
         Fetch the list of audit events
 
         Parameters
         ----------
@@ -39,31 +40,33 @@
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.audit_events.list(
+        client.audit_events.list_(
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audit-events"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -73,15 +76,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListAuditEventsResponse, _response.json())  # type: ignore
+            return typing.cast(ListAuditEventsResponse, construct_type(type_=ListAuditEventsResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, audit_event_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> AuditEvent:
@@ -112,16 +115,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audit-events/{jsonable_encoder(audit_event_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -130,27 +135,27 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(AuditEvent, _response.json())  # type: ignore
+            return typing.cast(AuditEvent, construct_type(type_=AuditEvent, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAuditEventsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(
+    async def list_(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> ListAuditEventsResponse:
         """
         Fetch the list of audit events
 
         Parameters
         ----------
@@ -167,31 +172,33 @@
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.audit_events.list(
+        await client.audit_events.list_(
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audit-events"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -201,15 +208,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListAuditEventsResponse, _response.json())  # type: ignore
+            return typing.cast(ListAuditEventsResponse, construct_type(type_=ListAuditEventsResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, audit_event_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> AuditEvent:
@@ -240,16 +247,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"audit-events/{jsonable_encoder(audit_event_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -258,13 +267,13 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(AuditEvent, _response.json())  # type: ignore
+            return typing.cast(AuditEvent, construct_type(type_=AuditEvent, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/audit_events/types/actor.py` & `trycourier-6.1.0/src/courier/profiles/types/subscribe_to_lists_request_list_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.recipient_preferences import RecipientPreferences
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class Actor(pydantic_v1.BaseModel):
-    id: typing.Optional[str] = None
-    email: typing.Optional[str] = None
+class SubscribeToListsRequestListObject(UncheckedBaseModel):
+    list_id: str = pydantic_v1.Field(alias="listId")
+    preferences: typing.Optional[RecipientPreferences] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/audit_events/types/audit_event.py` & `trycourier-6.1.0/src/courier/send/types/routing_strategy_channel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .actor import Actor
-from .target import Target
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .message_providers import MessageProviders
+from .routing_method import RoutingMethod
 
 
-class AuditEvent(pydantic_v1.BaseModel):
-    actor: typing.Optional[Actor] = None
-    target: typing.Optional[Target] = None
-    audit_event_id: str = pydantic_v1.Field(alias="auditEventId")
-    source: str
-    timestamp: str
-    type: str
+class RoutingStrategyChannel(UncheckedBaseModel):
+    channel: str
+    config: typing.Optional[typing.Dict[str, typing.Any]] = None
+    method: typing.Optional[RoutingMethod] = None
+    providers: typing.Optional[MessageProviders] = None
+    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/audit_events/types/get_audit_event_params.py` & `trycourier-6.1.0/src/courier/bulk/types/bulk_get_job_users_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class GetAuditEventParams(pydantic_v1.BaseModel):
-    audit_event_id: str = pydantic_v1.Field(alias="auditEventId")
+class BulkGetJobUsersParams(UncheckedBaseModel):
+    job_id: str = pydantic_v1.Field(alias="jobId")
+    cursor: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/audit_events/types/list_audit_events_params.py` & `trycourier-6.1.0/src/courier/audit_events/types/list_audit_events_params.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class ListAuditEventsParams(pydantic_v1.BaseModel):
+class ListAuditEventsParams(UncheckedBaseModel):
     cursor: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/audit_events/types/list_audit_events_response.py` & `trycourier-6.1.0/src/courier/send/types/locale.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .audit_event import AuditEvent
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class ListAuditEventsResponse(pydantic_v1.BaseModel):
-    paging: Paging
-    results: typing.List[AuditEvent]
+class Locale(UncheckedBaseModel):
+    content: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/audit_events/types/target.py` & `trycourier-6.1.0/src/courier/users/tokens/types/get_user_tokens_opts.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 
 
-class Target(pydantic_v1.BaseModel):
-    id: typing.Optional[str] = None
-    email: typing.Optional[str] = None
+class GetUserTokensOpts(UncheckedBaseModel):
+    user_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/auth_tokens/client.py` & `trycourier-6.1.0/src/courier/auth_tokens/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from .types.issue_token_response import IssueTokenResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class AuthTokensClient:
@@ -61,16 +62,18 @@
             scope="string",
             expires_in="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "auth/issue-token"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"scope": scope, "expires_in": expires_in})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"scope": scope, "expires_in": expires_in}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -87,15 +90,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(IssueTokenResponse, _response.json())  # type: ignore
+            return typing.cast(IssueTokenResponse, construct_type(type_=IssueTokenResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -144,16 +147,18 @@
             scope="string",
             expires_in="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "auth/issue-token"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"scope": scope, "expires_in": expires_in})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"scope": scope, "expires_in": expires_in}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -170,13 +175,13 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(IssueTokenResponse, _response.json())  # type: ignore
+            return typing.cast(IssueTokenResponse, construct_type(type_=IssueTokenResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/auth_tokens/types/issue_token_response.py` & `trycourier-6.1.0/src/courier/users/tokens/types/get_user_token_opts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 
 
-class IssueTokenResponse(pydantic_v1.BaseModel):
-    token: typing.Optional[str] = None
+class GetUserTokenOpts(UncheckedBaseModel):
+    user_id: str
+    token: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/automations/__init__.py` & `trycourier-6.1.0/src/courier/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/automations/client.py` & `trycourier-6.1.0/src/courier/automations/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from .types.automation_ad_hoc_invoke_params import AutomationAdHocInvokeParams
 from .types.automation_invoke_params import AutomationInvokeParams
 from .types.automation_invoke_response import AutomationInvokeResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
@@ -73,16 +74,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"automations/{jsonable_encoder(template_id)}/invoke"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -99,15 +102,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(AutomationInvokeResponse, _response.json())  # type: ignore
+            return typing.cast(AutomationInvokeResponse, construct_type(type_=AutomationInvokeResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def invoke_ad_hoc_automation(
@@ -170,16 +173,18 @@
                 ),
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "automations/invoke"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -196,15 +201,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(AutomationInvokeResponse, _response.json())  # type: ignore
+            return typing.cast(AutomationInvokeResponse, construct_type(type_=AutomationInvokeResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -263,16 +268,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"automations/{jsonable_encoder(template_id)}/invoke"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -289,15 +296,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(AutomationInvokeResponse, _response.json())  # type: ignore
+            return typing.cast(AutomationInvokeResponse, construct_type(type_=AutomationInvokeResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def invoke_ad_hoc_automation(
@@ -360,16 +367,18 @@
                 ),
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "automations/invoke"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -386,13 +395,13 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(AutomationInvokeResponse, _response.json())  # type: ignore
+            return typing.cast(AutomationInvokeResponse, construct_type(type_=AutomationInvokeResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/__init__.py` & `trycourier-6.1.0/src/courier/automations/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/automations/types/accessor_type.py` & `trycourier-6.1.0/src/courier/automations/types/automation_invoke_template_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .automation_invoke_params import AutomationInvokeParams
 
 
-class AccessorType(pydantic_v1.BaseModel):
-    ref: str = pydantic_v1.Field(alias="$ref")
+class AutomationInvokeTemplateParams(AutomationInvokeParams):
+    template_id: str = pydantic_v1.Field(alias="templateId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation.py` & `trycourier-6.1.0/src/courier/automations/types/automation_step.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .automation_step_option import AutomationStepOption
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class Automation(pydantic_v1.BaseModel):
-    cancelation_token: typing.Optional[str] = None
-    steps: typing.List[AutomationStepOption]
+class AutomationStep(UncheckedBaseModel):
+    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
+    ref: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_ad_hoc_invoke_params.py` & `trycourier-6.1.0/src/courier/automations/types/automation_cancel_step.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .automation import Automation
-from .automation_invoke_params import AutomationInvokeParams
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .automation_step import AutomationStep
 
 
-class AutomationAdHocInvokeParams(AutomationInvokeParams):
-    automation: Automation
+class AutomationCancelStep(AutomationStep):
+    action: typing.Literal["cancel"]
+    cancelation_token: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_add_to_batch_retain.py` & `trycourier-6.1.0/src/courier/automations/types/automation_add_to_batch_retain.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .automation_add_to_batch_retain_type import AutomationAddToBatchRetainType
 
 
-class AutomationAddToBatchRetain(pydantic_v1.BaseModel):
+class AutomationAddToBatchRetain(UncheckedBaseModel):
     """
     Defines what items should be retained and passed along to the next steps when the batch is released
 
     Examples
     --------
     from courier import AutomationAddToBatchRetain
 
@@ -41,15 +42,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_add_to_batch_step.py` & `trycourier-6.1.0/src/courier/automations/types/automation_add_to_batch_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .automation_add_to_batch_max_items_type import AutomationAddToBatchMaxItemsType
 from .automation_add_to_batch_retain import AutomationAddToBatchRetain
 from .automation_add_to_batch_scope import AutomationAddToBatchScope
 from .automation_step import AutomationStep
 
 
 class AutomationAddToBatchStep(AutomationStep):
@@ -66,16 +66,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_add_to_digest_step.py` & `trycourier-6.1.0/src/courier/automations/types/automation_add_to_digest_step.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .automation_step import AutomationStep
 
 
 class AutomationAddToDigestStep(AutomationStep):
     """
     Examples
     --------
@@ -27,16 +27,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_cancel_step.py` & `trycourier-6.1.0/src/courier/automations/types/automation_invoke_step.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .automation_step import AutomationStep
 
 
-class AutomationCancelStep(AutomationStep):
-    action: typing.Literal["cancel"]
-    cancelation_token: typing.Optional[str] = None
+class AutomationInvokeStep(AutomationStep):
+    action: typing.Literal["invoke"]
+    template: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_delay_step.py` & `trycourier-6.1.0/src/courier/automations/types/automation_delay_step.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .automation_step import AutomationStep
 
 
 class AutomationDelayStep(AutomationStep):
     action: typing.Literal["delay"]
     duration: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
@@ -21,16 +21,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_fetch_data_step.py` & `trycourier-6.1.0/src/courier/automations/types/automation_fetch_data_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .automation_fetch_data_webhook import AutomationFetchDataWebhook
 from .automation_step import AutomationStep
 from .merge_algorithm import MergeAlgorithm
 
 
 class AutomationFetchDataStep(AutomationStep):
     """
@@ -36,16 +36,20 @@
     idempotency_key: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_fetch_data_webhook.py` & `trycourier-6.1.0/src/courier/auth_tokens/types/issue_token_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .automation_fetch_data_webhook_method import AutomationFetchDataWebhookMethod
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class AutomationFetchDataWebhook(pydantic_v1.BaseModel):
-    body: typing.Optional[typing.Dict[str, typing.Any]] = None
-    headers: typing.Optional[typing.Dict[str, typing.Any]] = None
-    params: typing.Optional[typing.Dict[str, typing.Any]] = None
-    method: AutomationFetchDataWebhookMethod
-    url: str
+class IssueTokenResponse(UncheckedBaseModel):
+    token: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_invoke_params.py` & `trycourier-6.1.0/src/courier/audit_events/types/target.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .profile import Profile
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class AutomationInvokeParams(pydantic_v1.BaseModel):
-    brand: typing.Optional[str] = None
-    data: typing.Optional[typing.Dict[str, typing.Any]] = None
-    profile: typing.Optional[Profile] = None
-    recipient: typing.Optional[str] = None
-    template: typing.Optional[str] = None
+class Target(UncheckedBaseModel):
+    id: typing.Optional[str] = None
+    email: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_invoke_response.py` & `trycourier-6.1.0/src/courier/bulk/types/bulk_ingest_users_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .inbound_bulk_message_user import InboundBulkMessageUser
 
 
-class AutomationInvokeResponse(pydantic_v1.BaseModel):
-    run_id: str = pydantic_v1.Field(alias="runId")
+class BulkIngestUsersParams(UncheckedBaseModel):
+    users: typing.List[InboundBulkMessageUser]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_invoke_step.py` & `trycourier-6.1.0/src/courier/audiences/types/audience_member.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .automation_step import AutomationStep
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class AutomationInvokeStep(AutomationStep):
-    action: typing.Literal["invoke"]
-    template: str
+class AudienceMember(UncheckedBaseModel):
+    added_at: str
+    audience_id: str
+    audience_version: int
+    member_id: str
+    reason: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_invoke_template_params.py` & `trycourier-6.1.0/src/courier/send/types/list_pattern_recipient.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .automation_invoke_params import AutomationInvokeParams
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .list_pattern_recipient_type import ListPatternRecipientType
+from .message_data import MessageData
 
 
-class AutomationInvokeTemplateParams(AutomationInvokeParams):
-    template_id: str = pydantic_v1.Field(alias="templateId")
+class ListPatternRecipient(ListPatternRecipientType):
+    list_pattern: typing.Optional[str] = None
+    data: typing.Optional[MessageData] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_run_context.py` & `trycourier-6.1.0/src/courier/audit_events/types/actor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .profile import Profile
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class AutomationRunContext(pydantic_v1.BaseModel):
-    brand: typing.Optional[str] = None
-    data: typing.Optional[typing.Any] = None
-    profile: typing.Optional[Profile] = None
-    template: typing.Optional[str] = None
-    recipient: typing.Optional[str] = None
+class Actor(UncheckedBaseModel):
+    id: typing.Optional[str] = None
+    email: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_send_list_step.py` & `trycourier-6.1.0/src/courier/automations/types/automation_send_step.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .automation_step import AutomationStep
 
 
-class AutomationSendListStep(AutomationStep):
-    action: typing.Literal["send-list"]
+class AutomationSendStep(AutomationStep):
+    action: typing.Literal["send"]
     brand: typing.Optional[str] = None
     data: typing.Optional[typing.Dict[str, typing.Any]] = None
-    list_: str = pydantic_v1.Field(alias="list")
     override: typing.Optional[typing.Dict[str, typing.Any]] = None
+    profile: typing.Optional[typing.Any] = None
+    recipient: typing.Optional[str] = None
     template: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_send_step.py` & `trycourier-6.1.0/src/courier/send/types/utm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .automation_step import AutomationStep
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class AutomationSendStep(AutomationStep):
-    action: typing.Literal["send"]
-    brand: typing.Optional[str] = None
-    data: typing.Optional[typing.Dict[str, typing.Any]] = None
-    override: typing.Optional[typing.Dict[str, typing.Any]] = None
-    profile: typing.Optional[typing.Any] = None
-    recipient: typing.Optional[str] = None
-    template: typing.Optional[str] = None
+class Utm(UncheckedBaseModel):
+    source: typing.Optional[str] = None
+    medium: typing.Optional[str] = None
+    campaign: typing.Optional[str] = None
+    term: typing.Optional[str] = None
+    content: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_step.py` & `trycourier-6.1.0/src/courier/send/types/email_footer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class AutomationStep(pydantic_v1.BaseModel):
-    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
-    ref: typing.Optional[str] = None
+class EmailFooter(UncheckedBaseModel):
+    content: typing.Optional[typing.Any] = None
+    inherit_default: typing.Optional[bool] = pydantic_v1.Field(alias="inheritDefault", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_step_option.py` & `trycourier-6.1.0/src/courier/automations/types/automation_step_option.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_throttle_on_throttle.py` & `trycourier-6.1.0/src/courier/commons/types/conflict.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .base_error import BaseError
 
 
-class AutomationThrottleOnThrottle(pydantic_v1.BaseModel):
-    node_id: str = pydantic_v1.Field(alias="$node_id")
-    """
-    The node to go to if the request is throttled
-    """
+class Conflict(BaseError):
+    type: typing.Literal["invalid_request_error"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_throttle_step.py` & `trycourier-6.1.0/src/courier/automations/types/automation_throttle_step.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .automation_step import AutomationStep
 from .automation_throttle_on_throttle import AutomationThrottleOnThrottle
 from .automation_throttle_scope import AutomationThrottleScope
 
 
 class AutomationThrottleStep(AutomationStep):
     """
@@ -54,16 +54,20 @@
     on_throttle: AutomationThrottleOnThrottle
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_update_profile_step.py` & `trycourier-6.1.0/src/courier/automations/types/automation_update_profile_step.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .merge_algorithm import MergeAlgorithm
 from .profile import Profile
 
 
-class AutomationUpdateProfileStep(pydantic_v1.BaseModel):
+class AutomationUpdateProfileStep(UncheckedBaseModel):
     action: typing.Literal["update-profile"]
     recipient_id: str
     profile: Profile
     merge: MergeAlgorithm
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/automations/types/automation_v_2_send_step.py` & `trycourier-6.1.0/src/courier/commons/types/not_found.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from ...send.types.message import Message
-from .automation_step import AutomationStep
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .base_error import BaseError
 
 
-class AutomationV2SendStep(AutomationStep):
-    action: typing.Literal["send"]
-    message: Message
+class NotFound(BaseError):
+    type: typing.Literal["invalid_request_error"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/brands/client.py` & `trycourier-6.1.0/src/courier/users/tenants/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,158 +1,182 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ..commons.errors.already_exists_error import AlreadyExistsError
-from ..commons.errors.bad_request_error import BadRequestError
-from ..commons.errors.conflict_error import ConflictError
-from ..commons.errors.payment_required_error import PaymentRequiredError
-from ..commons.types.already_exists import AlreadyExists
-from ..commons.types.bad_request import BadRequest
-from ..commons.types.conflict import Conflict
-from ..commons.types.payment_required import PaymentRequired
-from ..core.api_error import ApiError
-from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
-from ..core.remove_none_from_dict import remove_none_from_dict
-from ..core.request_options import RequestOptions
-from .types.brand import Brand
-from .types.brand_parameters import BrandParameters
-from .types.brand_settings import BrandSettings
-from .types.brand_snippets import BrandSnippets
-from .types.brands_response import BrandsResponse
+from ...commons.types.user_tenant_association import UserTenantAssociation
+from ...core.api_error import ApiError
+from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from ...core.jsonable_encoder import jsonable_encoder
+from ...core.query_encoder import encode_query
+from ...core.remove_none_from_dict import remove_none_from_dict
+from ...core.request_options import RequestOptions
+from ...core.unchecked_base_model import construct_type
+from .types.list_tenants_for_user_response import ListTenantsForUserResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class BrandsClient:
+class TenantsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def create(
+    def add_multple(
         self,
+        user_id: str,
         *,
-        request: BrandParameters,
-        idempotency_key: typing.Optional[str] = None,
-        idempotency_expiry: typing.Optional[str] = None,
+        tenants: typing.Sequence[UserTenantAssociation],
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> Brand:
+    ) -> None:
         """
+        This endpoint is used to add a user to
+        multiple tenants in one call.
+        A custom profile can also be supplied for each tenant.
+        This profile will be merged with the user's main
+        profile when sending to the user with that tenant.
+
         Parameters
         ----------
-        request : BrandParameters
-
-        idempotency_key : typing.Optional[str]
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
 
-        idempotency_expiry : typing.Optional[str]
-            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        tenants : typing.Sequence[UserTenantAssociation]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Brand
+        None
 
         Examples
         --------
-        from courier import BrandParameters, BrandSettings, BrandSnippets
+        from courier import UserTenantAssociation
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.brands.create(
-            request=BrandParameters(
-                id="string",
-                name="string",
-                settings=BrandSettings(),
-                snippets=BrandSnippets(),
-            ),
+        client.users.tenants.add_multple(
+            user_id="string",
+            tenants=[
+                UserTenantAssociation(
+                    user_id="string",
+                    type="user",
+                    tenant_id="string",
+                    profile={"string": {"key": "value"}},
+                )
+            ],
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder({"tenants": tenants})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder({"tenants": tenants}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
-                        "Idempotency-Key": str(idempotency_key) if idempotency_key is not None else None,
-                        "X-Idempotency-Expiration": str(idempotency_expiry) if idempotency_expiry is not None else None,
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Brand, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
-        if _response.status_code == 402:
-            raise PaymentRequiredError(pydantic_v1.parse_obj_as(PaymentRequired, _response.json()))  # type: ignore
-        if _response.status_code == 409:
-            raise AlreadyExistsError(pydantic_v1.parse_obj_as(AlreadyExists, _response.json()))  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, brand_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Brand:
+    def add(
+        self,
+        user_id: str,
+        tenant_id: str,
+        *,
+        profile: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> None:
         """
-        Fetch a specific brand by brand ID.
+        This endpoint is used to add a single tenant.
+
+        A custom profile can also be supplied with the tenant.
+        This profile will be merged with the user's main profile
+        when sending to the user with that tenant.
 
         Parameters
         ----------
-        brand_id : str
-            A unique identifier associated with the brand you wish to retrieve.
+        user_id : str
+            Id of the user to be added to the supplied tenant.
+
+        tenant_id : str
+            Id of the tenant the user should be added to.
+
+        profile : typing.Optional[typing.Dict[str, typing.Any]]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Brand
+        None
 
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.brands.get(
-            brand_id="string",
+        client.users.tenants.add(
+            user_id="string",
+            tenant_id="string",
+            profile={"string": {"key": "value"}},
         )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if profile is not OMIT:
+            _request["profile"] = profile
         _response = self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"users/{jsonable_encoder(user_id)}/tenants/{jsonable_encoder(tenant_id)}",
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -160,65 +184,61 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Brand, _response.json())  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def list(
-        self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
-    ) -> BrandsResponse:
+    def remove_all(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Get the list of brands.
+        Removes a user from any tenants they may have been associated with.
 
         Parameters
         ----------
-        cursor : typing.Optional[str]
-            A unique identifier that allows for fetching the next set of brands.
+        user_id : str
+            Id of the user to be removed from the supplied tenant.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        BrandsResponse
+        None
 
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.brands.list(
-            cursor="string",
+        client.users.tenants.remove_all(
+            user_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
                 )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -226,29 +246,32 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BrandsResponse, _response.json())  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, brand_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+    def remove(self, user_id: str, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Delete a brand by brand ID.
+        Removes a user from the supplied tenant.
 
         Parameters
         ----------
-        brand_id : str
-            A unique identifier associated with the brand you wish to retrieve.
+        user_id : str
+            Id of the user to be removed from the supplied tenant.
+
+        tenant_id : str
+            Id of the tenant the user should be removed from.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
         None
@@ -256,24 +279,33 @@
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.brands.delete(
-            brand_id="string",
+        client.users.tenants.remove(
+            user_id="string",
+            tenant_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="DELETE",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"users/{jsonable_encoder(user_id)}/tenants/{jsonable_encoder(tenant_id)}",
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -282,103 +314,83 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
-        if _response.status_code == 409:
-            raise ConflictError(pydantic_v1.parse_obj_as(Conflict, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def replace(
+    def list_(
         self,
-        brand_id: str,
+        user_id: str,
         *,
-        name: str,
-        settings: typing.Optional[BrandSettings] = OMIT,
-        snippets: typing.Optional[BrandSnippets] = OMIT,
+        limit: typing.Optional[int] = None,
+        cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> Brand:
+    ) -> ListTenantsForUserResponse:
         """
-        Replace an existing brand with the supplied values.
+        Returns a paginated list of user tenant associations.
 
         Parameters
         ----------
-        brand_id : str
-            A unique identifier associated with the brand you wish to update.
-
-        name : str
-            The name of the brand.
+        user_id : str
+            Id of the user to retrieve all associated tenants for.
 
-        settings : typing.Optional[BrandSettings]
+        limit : typing.Optional[int]
+            The number of accounts to return
+            (defaults to 20, maximum value of 100)
 
-        snippets : typing.Optional[BrandSnippets]
+        cursor : typing.Optional[str]
+            Continue the pagination with the next cursor
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Brand
+        ListTenantsForUserResponse
 
         Examples
         --------
-        from courier import (
-            BrandColors,
-            BrandSettings,
-            BrandSnippet,
-            BrandSnippets,
-            Email,
-        )
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.brands.replace(
-            brand_id="string",
-            name="string",
-            settings=BrandSettings(
-                colors=BrandColors(),
-                inapp={"key": "value"},
-                email=Email(),
-            ),
-            snippets=BrandSnippets(
-                items=[
-                    BrandSnippet(
-                        format="handlebars",
-                        name="string",
-                        value="string",
-                    )
-                ],
-            ),
+        client.users.tenants.list_(
+            user_id="string",
+            limit=1,
+            cursor="string",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if settings is not OMIT:
-            _request["settings"] = settings
-        if snippets is not OMIT:
-            _request["snippets"] = snippets
         _response = self._client_wrapper.httpx_client.request(
-            method="PUT",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "limit": limit,
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
+                )
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -386,143 +398,177 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Brand, _response.json())  # type: ignore
+            return typing.cast(ListTenantsForUserResponse, construct_type(type_=ListTenantsForUserResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncBrandsClient:
+class AsyncTenantsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def create(
+    async def add_multple(
         self,
+        user_id: str,
         *,
-        request: BrandParameters,
-        idempotency_key: typing.Optional[str] = None,
-        idempotency_expiry: typing.Optional[str] = None,
+        tenants: typing.Sequence[UserTenantAssociation],
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> Brand:
+    ) -> None:
         """
+        This endpoint is used to add a user to
+        multiple tenants in one call.
+        A custom profile can also be supplied for each tenant.
+        This profile will be merged with the user's main
+        profile when sending to the user with that tenant.
+
         Parameters
         ----------
-        request : BrandParameters
-
-        idempotency_key : typing.Optional[str]
+        user_id : str
+            The user's ID. This can be any uniquely identifiable string.
 
-        idempotency_expiry : typing.Optional[str]
-            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
+        tenants : typing.Sequence[UserTenantAssociation]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Brand
+        None
 
         Examples
         --------
-        from courier import BrandParameters, BrandSettings, BrandSnippets
+        from courier import UserTenantAssociation
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.brands.create(
-            request=BrandParameters(
-                id="string",
-                name="string",
-                settings=BrandSettings(),
-                snippets=BrandSnippets(),
-            ),
+        await client.users.tenants.add_multple(
+            user_id="string",
+            tenants=[
+                UserTenantAssociation(
+                    user_id="string",
+                    type="user",
+                    tenant_id="string",
+                    profile={"string": {"key": "value"}},
+                )
+            ],
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder({"tenants": tenants})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder({"tenants": tenants}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
-                        "Idempotency-Key": str(idempotency_key) if idempotency_key is not None else None,
-                        "X-Idempotency-Expiration": str(idempotency_expiry) if idempotency_expiry is not None else None,
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Brand, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
-        if _response.status_code == 402:
-            raise PaymentRequiredError(pydantic_v1.parse_obj_as(PaymentRequired, _response.json()))  # type: ignore
-        if _response.status_code == 409:
-            raise AlreadyExistsError(pydantic_v1.parse_obj_as(AlreadyExists, _response.json()))  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, brand_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Brand:
+    async def add(
+        self,
+        user_id: str,
+        tenant_id: str,
+        *,
+        profile: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> None:
         """
-        Fetch a specific brand by brand ID.
+        This endpoint is used to add a single tenant.
+
+        A custom profile can also be supplied with the tenant.
+        This profile will be merged with the user's main profile
+        when sending to the user with that tenant.
 
         Parameters
         ----------
-        brand_id : str
-            A unique identifier associated with the brand you wish to retrieve.
+        user_id : str
+            Id of the user to be added to the supplied tenant.
+
+        tenant_id : str
+            Id of the tenant the user should be added to.
+
+        profile : typing.Optional[typing.Dict[str, typing.Any]]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Brand
+        None
 
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.brands.get(
-            brand_id="string",
+        await client.users.tenants.add(
+            user_id="string",
+            tenant_id="string",
+            profile={"string": {"key": "value"}},
         )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if profile is not OMIT:
+            _request["profile"] = profile
         _response = await self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"users/{jsonable_encoder(user_id)}/tenants/{jsonable_encoder(tenant_id)}",
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -530,65 +576,61 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Brand, _response.json())  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def list(
-        self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
-    ) -> BrandsResponse:
+    async def remove_all(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Get the list of brands.
+        Removes a user from any tenants they may have been associated with.
 
         Parameters
         ----------
-        cursor : typing.Optional[str]
-            A unique identifier that allows for fetching the next set of brands.
+        user_id : str
+            Id of the user to be removed from the supplied tenant.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        BrandsResponse
+        None
 
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.brands.list(
-            cursor="string",
+        await client.users.tenants.remove_all(
+            user_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
                 )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -596,29 +638,34 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BrandsResponse, _response.json())  # type: ignore
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, brand_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+    async def remove(
+        self, user_id: str, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> None:
         """
-        Delete a brand by brand ID.
+        Removes a user from the supplied tenant.
 
         Parameters
         ----------
-        brand_id : str
-            A unique identifier associated with the brand you wish to retrieve.
+        user_id : str
+            Id of the user to be removed from the supplied tenant.
+
+        tenant_id : str
+            Id of the tenant the user should be removed from.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
         None
@@ -626,24 +673,33 @@
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.brands.delete(
-            brand_id="string",
+        await client.users.tenants.remove(
+            user_id="string",
+            tenant_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="DELETE",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"users/{jsonable_encoder(user_id)}/tenants/{jsonable_encoder(tenant_id)}",
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -652,103 +708,83 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
-        if _response.status_code == 409:
-            raise ConflictError(pydantic_v1.parse_obj_as(Conflict, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def replace(
+    async def list_(
         self,
-        brand_id: str,
+        user_id: str,
         *,
-        name: str,
-        settings: typing.Optional[BrandSettings] = OMIT,
-        snippets: typing.Optional[BrandSnippets] = OMIT,
+        limit: typing.Optional[int] = None,
+        cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> Brand:
+    ) -> ListTenantsForUserResponse:
         """
-        Replace an existing brand with the supplied values.
+        Returns a paginated list of user tenant associations.
 
         Parameters
         ----------
-        brand_id : str
-            A unique identifier associated with the brand you wish to update.
-
-        name : str
-            The name of the brand.
+        user_id : str
+            Id of the user to retrieve all associated tenants for.
 
-        settings : typing.Optional[BrandSettings]
+        limit : typing.Optional[int]
+            The number of accounts to return
+            (defaults to 20, maximum value of 100)
 
-        snippets : typing.Optional[BrandSnippets]
+        cursor : typing.Optional[str]
+            Continue the pagination with the next cursor
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Brand
+        ListTenantsForUserResponse
 
         Examples
         --------
-        from courier import (
-            BrandColors,
-            BrandSettings,
-            BrandSnippet,
-            BrandSnippets,
-            Email,
-        )
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.brands.replace(
-            brand_id="string",
-            name="string",
-            settings=BrandSettings(
-                colors=BrandColors(),
-                inapp={"key": "value"},
-                email=Email(),
-            ),
-            snippets=BrandSnippets(
-                items=[
-                    BrandSnippet(
-                        format="handlebars",
-                        name="string",
-                        value="string",
-                    )
-                ],
-            ),
+        await client.users.tenants.list_(
+            user_id="string",
+            limit=1,
+            cursor="string",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if settings is not OMIT:
-            _request["settings"] = settings
-        if snippets is not OMIT:
-            _request["snippets"] = snippets
         _response = await self._client_wrapper.httpx_client.request(
-            method="PUT",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "limit": limit,
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
+                )
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -756,13 +792,13 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Brand, _response.json())  # type: ignore
+            return typing.cast(ListTenantsForUserResponse, construct_type(type_=ListTenantsForUserResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/brands/types/__init__.py` & `trycourier-6.1.0/src/courier/brands/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/brands/types/brand.py` & `trycourier-6.1.0/src/courier/brands/types/brand.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .brand_settings import BrandSettings
 from .brand_snippets import BrandSnippets
 
 
-class Brand(pydantic_v1.BaseModel):
+class Brand(UncheckedBaseModel):
     created: int = pydantic_v1.Field()
     """
     The date/time of when the brand was created. Represented in milliseconds since Unix epoch.
     """
 
     id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
@@ -43,15 +44,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/brands/types/brand_colors.py` & `trycourier-6.1.0/src/courier/profiles/types/ms_teams_base_properties.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class BrandColors(pydantic_v1.BaseModel):
-    primary: typing.Optional[str] = None
-    secondary: typing.Optional[str] = None
-    tertiary: typing.Optional[str] = None
+class MsTeamsBaseProperties(UncheckedBaseModel):
+    tenant_id: str
+    service_url: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/brands/types/brand_get_all_response.py` & `trycourier-6.1.0/src/courier/audiences/types/audience_list_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .brand import Brand
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .audience import Audience
 
 
-class BrandGetAllResponse(pydantic_v1.BaseModel):
+class AudienceListResponse(UncheckedBaseModel):
+    items: typing.List[Audience]
     paging: Paging
-    results: typing.List[Brand]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/brands/types/brand_parameters.py` & `trycourier-6.1.0/src/courier/brands/types/brand_parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .brand_settings import BrandSettings
 from .brand_snippets import BrandSnippets
 
 
-class BrandParameters(pydantic_v1.BaseModel):
+class BrandParameters(UncheckedBaseModel):
     id: typing.Optional[str] = None
     name: str = pydantic_v1.Field()
     """
     The name of the brand.
     """
 
     settings: BrandSettings
     snippets: typing.Optional[BrandSnippets] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/brands/types/brand_settings.py` & `trycourier-6.1.0/src/courier/brands/types/brand_snippets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.email import Email
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .brand_colors import BrandColors
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .brand_snippet import BrandSnippet
 
 
-class BrandSettings(pydantic_v1.BaseModel):
-    colors: typing.Optional[BrandColors] = None
-    inapp: typing.Optional[typing.Any] = None
-    email: typing.Optional[Email] = None
+class BrandSnippets(UncheckedBaseModel):
+    items: typing.List[BrandSnippet]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/brands/types/brand_snippet.py` & `trycourier-6.1.0/src/courier/brands/types/brand_snippet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class BrandSnippet(pydantic_v1.BaseModel):
+class BrandSnippet(UncheckedBaseModel):
     format: typing.Literal["handlebars"]
     name: str
     value: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/brands/types/brand_snippets.py` & `trycourier-6.1.0/src/courier/profiles/types/send_to_ms_teams_email.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .brand_snippet import BrandSnippet
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .ms_teams_base_properties import MsTeamsBaseProperties
 
 
-class BrandSnippets(pydantic_v1.BaseModel):
-    items: typing.List[BrandSnippet]
+class SendToMsTeamsEmail(MsTeamsBaseProperties):
+    email: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/brands/types/brands_response.py` & `trycourier-6.1.0/src/courier/users/tokens/types/put_user_tokens_opts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.paging import Paging
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .brand import Brand
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
+from .user_token import UserToken
 
 
-class BrandsResponse(pydantic_v1.BaseModel):
-    paging: Paging
-    results: typing.List[Brand]
+class PutUserTokensOpts(UncheckedBaseModel):
+    user_id: str
+    tokens: typing.List[UserToken]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/bulk/__init__.py` & `trycourier-6.1.0/src/courier/bulk/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/bulk/client.py` & `trycourier-6.1.0/src/courier/bulk/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from json.decoder import JSONDecodeError
 
 from ..commons.errors.bad_request_error import BadRequestError
 from ..commons.types.bad_request import BadRequest
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from .types.bulk_create_job_response import BulkCreateJobResponse
 from .types.bulk_get_job_response import BulkGetJobResponse
 from .types.bulk_get_job_users_response import BulkGetJobUsersResponse
 from .types.bulk_ingest_users_params import BulkIngestUsersParams
 from .types.inbound_bulk_message import InboundBulkMessage
 
 # this is used as the default value for optional parameters
@@ -69,16 +70,18 @@
                 override={"key": "value"},
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "bulk"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"message": message})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"message": message}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -95,17 +98,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BulkCreateJobResponse, _response.json())  # type: ignore
+            return typing.cast(BulkCreateJobResponse, construct_type(type_=BulkCreateJobResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def ingest_users(
@@ -166,16 +171,18 @@
                 ],
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -241,16 +248,18 @@
         client.bulk.run_job(
             job_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}/run"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -266,15 +275,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_job(self, job_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> BulkGetJobResponse:
@@ -303,16 +314,18 @@
         client.bulk.get_job(
             job_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -321,17 +334,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BulkGetJobResponse, _response.json())  # type: ignore
+            return typing.cast(BulkGetJobResponse, construct_type(type_=BulkGetJobResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_users(
@@ -364,16 +379,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}/users"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -382,17 +399,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BulkGetJobUsersResponse, _response.json())  # type: ignore
+            return typing.cast(BulkGetJobUsersResponse, construct_type(type_=BulkGetJobUsersResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -443,16 +462,18 @@
                 override={"key": "value"},
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "bulk"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"message": message})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"message": message}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -469,17 +490,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BulkCreateJobResponse, _response.json())  # type: ignore
+            return typing.cast(BulkCreateJobResponse, construct_type(type_=BulkCreateJobResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def ingest_users(
@@ -540,16 +563,18 @@
                 ],
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -615,16 +640,18 @@
         await client.bulk.run_job(
             job_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}/run"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -640,15 +667,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_job(
@@ -679,16 +708,18 @@
         await client.bulk.get_job(
             job_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -697,17 +728,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BulkGetJobResponse, _response.json())  # type: ignore
+            return typing.cast(BulkGetJobResponse, construct_type(type_=BulkGetJobResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_users(
@@ -740,16 +773,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"bulk/{jsonable_encoder(job_id)}/users"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -758,15 +793,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(BulkGetJobUsersResponse, _response.json())  # type: ignore
+            return typing.cast(BulkGetJobUsersResponse, construct_type(type_=BulkGetJobUsersResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/__init__.py` & `trycourier-6.1.0/src/courier/bulk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/bulk/types/bulk_create_job_response.py` & `trycourier-6.1.0/src/courier/send/types/email_head.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class BulkCreateJobResponse(pydantic_v1.BaseModel):
-    job_id: str = pydantic_v1.Field(alias="jobId")
+class EmailHead(UncheckedBaseModel):
+    inherit_default: bool = pydantic_v1.Field(alias="inheritDefault")
+    content: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/bulk_get_job_params.py` & `trycourier-6.1.0/src/courier/profiles/types/send_to_ms_teams_channel_name.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .ms_teams_base_properties import MsTeamsBaseProperties
 
 
-class BulkGetJobParams(pydantic_v1.BaseModel):
-    job_id: str = pydantic_v1.Field(alias="jobId")
+class SendToMsTeamsChannelName(MsTeamsBaseProperties):
+    channel_name: str
+    team_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/bulk_get_job_response.py` & `trycourier-6.1.0/src/courier/notifications/types/submission_checks_replace_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .job_details import JobDetails
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .check import Check
 
 
-class BulkGetJobResponse(pydantic_v1.BaseModel):
-    job: JobDetails
+class SubmissionChecksReplaceResponse(UncheckedBaseModel):
+    checks: typing.List[Check]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/bulk_get_job_users_params.py` & `trycourier-6.1.0/src/courier/send/types/user_recipient_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class BulkGetJobUsersParams(pydantic_v1.BaseModel):
-    job_id: str = pydantic_v1.Field(alias="jobId")
-    cursor: typing.Optional[str] = None
-
+class UserRecipientType(UncheckedBaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/bulk_get_job_users_response.py` & `trycourier-6.1.0/src/courier/audiences/types/audience_member_list_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .bulk_message_user_response import BulkMessageUserResponse
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .audience_member import AudienceMember
 
 
-class BulkGetJobUsersResponse(pydantic_v1.BaseModel):
-    items: typing.List[BulkMessageUserResponse]
+class AudienceMemberListResponse(UncheckedBaseModel):
+    items: typing.List[AudienceMember]
     paging: Paging
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/bulk_ingest_error.py` & `trycourier-6.1.0/src/courier/profiles/types/send_to_ms_teams_channel_id.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .ms_teams_base_properties import MsTeamsBaseProperties
 
 
-class BulkIngestError(pydantic_v1.BaseModel):
-    user: typing.Any
-    error: typing.Any
+class SendToMsTeamsChannelId(MsTeamsBaseProperties):
+    channel_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/bulk_ingest_users_params.py` & `trycourier-6.1.0/src/courier/bulk/types/inbound_bulk_message.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .inbound_bulk_message_user import InboundBulkMessageUser
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .inbound_bulk_message_v_1 import InboundBulkMessageV1
+from .inbound_bulk_message_v_2 import InboundBulkMessageV2
 
 
-class BulkIngestUsersParams(pydantic_v1.BaseModel):
-    users: typing.List[InboundBulkMessageUser]
+class InboundBulkMessage(InboundBulkMessageV1):
+    message: typing.Optional[InboundBulkMessageV2] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/bulk_ingest_users_response.py` & `trycourier-6.1.0/src/courier/bulk/types/bulk_ingest_users_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .bulk_ingest_error import BulkIngestError
 
 
-class BulkIngestUsersResponse(pydantic_v1.BaseModel):
+class BulkIngestUsersResponse(UncheckedBaseModel):
     total: int
     errors: typing.Optional[typing.List[BulkIngestError]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/bulk_message_user_response.py` & `trycourier-6.1.0/src/courier/bulk/types/bulk_message_user_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .bulk_job_user_status import BulkJobUserStatus
 from .inbound_bulk_message_user import InboundBulkMessageUser
 
 
 class BulkMessageUserResponse(InboundBulkMessageUser):
     status: BulkJobUserStatus
     message_id: typing.Optional[str] = pydantic_v1.Field(alias="messageId", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/inbound_bulk_content_message.py` & `trycourier-6.1.0/src/courier/send/types/content_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from ...send.types.base_message import BaseMessage
-from ...send.types.content import Content
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .base_message import BaseMessage
+from .base_message_send_to import BaseMessageSendTo
+from .content import Content
 
 
-class InboundBulkContentMessage(BaseMessage):
+class ContentMessage(BaseMessage, BaseMessageSendTo):
     """
     The message property has the following primary top-level properties. They define the destination and content of the message.
     Additional advanced configuration fields [are defined below](https://www.courier.com/docs/reference/send/message/#other-message-properties).
     """
 
     content: Content = pydantic_v1.Field()
     """
@@ -22,16 +23,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/inbound_bulk_message.py` & `trycourier-6.1.0/src/courier/profiles/types/send_to_slack_email.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .inbound_bulk_message_v_1 import InboundBulkMessageV1
-from .inbound_bulk_message_v_2 import InboundBulkMessageV2
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .slack_base_properties import SlackBaseProperties
 
 
-class InboundBulkMessage(InboundBulkMessageV1):
-    message: typing.Optional[InboundBulkMessageV2] = None
+class SendToSlackEmail(SlackBaseProperties):
+    email: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/inbound_bulk_message_user.py` & `trycourier-6.1.0/src/courier/bulk/types/inbound_bulk_message_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...commons.types.recipient_preferences import RecipientPreferences
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from ...send.types.user_recipient import UserRecipient
 
 
-class InboundBulkMessageUser(pydantic_v1.BaseModel):
+class InboundBulkMessageUser(UncheckedBaseModel):
     preferences: typing.Optional[RecipientPreferences] = None
     profile: typing.Optional[typing.Any] = None
     recipient: typing.Optional[str] = None
     data: typing.Optional[typing.Any] = None
     to: typing.Optional[UserRecipient] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/inbound_bulk_message_v_1.py` & `trycourier-6.1.0/src/courier/send/types/elemental_image_node.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,60 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .elemental_base_node import ElementalBaseNode
+from .i_alignment import IAlignment
 
 
-class InboundBulkMessageV1(pydantic_v1.BaseModel):
-    brand: typing.Optional[str] = pydantic_v1.Field(default=None)
+class ElementalImageNode(ElementalBaseNode):
     """
-    A unique identifier that represents the brand that should be used
-    for rendering the notification.
+    Used to embed an image into the notification.
     """
 
-    data: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    src: str = pydantic_v1.Field()
     """
-    JSON that includes any data you want to pass to a message template.
-    The data will populate the corresponding template variables.
+    The source of the image.
     """
 
-    event: typing.Optional[str] = None
-    locale: typing.Optional[typing.Dict[str, typing.Any]] = None
-    override: typing.Optional[typing.Any] = pydantic_v1.Field(default=None)
+    href: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    JSON that is merged into the request sent by Courier to the provider
-    to override properties or to gain access to features in the provider
-    API that are not natively supported by Courier.
+    A URL to link to when the image is clicked.
+    """
+
+    align: typing.Optional[IAlignment] = pydantic_v1.Field(default=None)
+    """
+    The alignment of the image.
+    """
+
+    alt_text: typing.Optional[str] = pydantic_v1.Field(alias="altText", default=None)
+    """
+    Alternate text for the image.
+    """
+
+    width: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    CSS width properties to apply to the image. For example, 50px
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/inbound_bulk_template_message.py` & `trycourier-6.1.0/src/courier/bulk/types/inbound_bulk_template_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ...send.types.base_message import BaseMessage
 
 
 class InboundBulkTemplateMessage(BaseMessage):
     template: str = pydantic_v1.Field()
     """
     The id of the notification template to be rendered and sent to the recipient(s).
@@ -16,16 +16,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/bulk/types/job_details.py` & `trycourier-6.1.0/src/courier/bulk/types/job_details.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .bulk_job_status import BulkJobStatus
 from .inbound_bulk_message import InboundBulkMessage
 
 
-class JobDetails(pydantic_v1.BaseModel):
+class JobDetails(UncheckedBaseModel):
     definition: InboundBulkMessage
     enqueued: int
     failures: int
     received: int
     status: BulkJobStatus
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/client.py` & `trycourier-6.1.0/src/courier/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 from .auth_tokens.client import AsyncAuthTokensClient, AuthTokensClient
 from .automations.client import AsyncAutomationsClient, AutomationsClient
 from .brands.client import AsyncBrandsClient, BrandsClient
 from .bulk.client import AsyncBulkClient, BulkClient
 from .core.api_error import ApiError
 from .core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .core.jsonable_encoder import jsonable_encoder
-from .core.pydantic_utilities import pydantic_v1
+from .core.query_encoder import encode_query
 from .core.remove_none_from_dict import remove_none_from_dict
 from .core.request_options import RequestOptions
+from .core.unchecked_base_model import construct_type
 from .environment import CourierEnvironment
 from .lists.client import AsyncListsClient, ListsClient
 from .messages.client import AsyncMessagesClient, MessagesClient
 from .notifications.client import AsyncNotificationsClient, NotificationsClient
 from .profiles.client import AsyncProfilesClient, ProfilesClient
 from .send.types.message import Message
 from .templates.client import AsyncTemplatesClient, TemplatesClient
@@ -33,15 +34,15 @@
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class Courier:
     """
-    Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
+    Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propagate to these functions.
 
     Parameters
     ----------
     base_url : typing.Optional[str]
         The base url to use for requests from the client.
 
     environment : CourierEnvironment
@@ -178,16 +179,18 @@
                 to=AudienceRecipient(),
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "send"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"message": message})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"message": message}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -204,25 +207,25 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SendMessageResponse, _response.json())  # type: ignore
+            return typing.cast(SendMessageResponse, construct_type(type_=SendMessageResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncCourier:
     """
-    Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
+    Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propagate to these functions.
 
     Parameters
     ----------
     base_url : typing.Optional[str]
         The base url to use for requests from the client.
 
     environment : CourierEnvironment
@@ -359,16 +362,18 @@
                 to=AudienceRecipient(),
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "send"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"message": message})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"message": message}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -385,15 +390,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SendMessageResponse, _response.json())  # type: ignore
+            return typing.cast(SendMessageResponse, construct_type(type_=SendMessageResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/commons/__init__.py` & `trycourier-6.1.0/src/courier/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/commons/errors/__init__.py` & `trycourier-6.1.0/src/courier/commons/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/commons/types/__init__.py` & `trycourier-6.1.0/src/courier/commons/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/commons/types/already_exists.py` & `trycourier-6.1.0/src/courier/commons/types/message_not_found.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .base_error import BaseError
 
 
-class AlreadyExists(BaseError):
+class MessageNotFound(BaseError):
     type: typing.Literal["invalid_request_error"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/commons/types/bad_request.py` & `trycourier-6.1.0/src/courier/users/preferences/types/user_preferences_list_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .base_error import BaseError
+from ....commons.types.paging import Paging
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
+from .topic_preference import TopicPreference
 
 
-class BadRequest(BaseError):
-    type: typing.Literal["invalid_request_error"]
+class UserPreferencesListResponse(UncheckedBaseModel):
+    paging: Paging
+    items: typing.List[TopicPreference] = pydantic_v1.Field()
+    """
+    The Preferences associated with the user_id.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/commons/types/base_error.py` & `trycourier-6.1.0/src/courier/send/types/channel_metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .utm import Utm
 
 
-class BaseError(pydantic_v1.BaseModel):
-    message: str = pydantic_v1.Field()
-    """
-    A message describing the error that occurred.
-    """
+class ChannelMetadata(UncheckedBaseModel):
+    utm: typing.Optional[Utm] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/commons/types/channel_preference.py` & `trycourier-6.1.0/src/courier/bulk/types/bulk_get_job_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .channel_classification import ChannelClassification
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class ChannelPreference(pydantic_v1.BaseModel):
-    channel: ChannelClassification
+class BulkGetJobParams(UncheckedBaseModel):
+    job_id: str = pydantic_v1.Field(alias="jobId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/commons/types/conflict.py` & `trycourier-6.1.0/src/courier/audit_events/types/get_audit_event_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .base_error import BaseError
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class Conflict(BaseError):
-    type: typing.Literal["invalid_request_error"]
+class GetAuditEventParams(UncheckedBaseModel):
+    audit_event_id: str = pydantic_v1.Field(alias="auditEventId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/commons/types/email.py` & `trycourier-6.1.0/src/courier/profiles/types/send_to_ms_teams_user_id.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .ms_teams_base_properties import MsTeamsBaseProperties
 
 
-class Email(pydantic_v1.BaseModel):
-    footer: typing.Any
-    header: typing.Any
+class SendToMsTeamsUserId(MsTeamsBaseProperties):
+    user_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/commons/types/message_not_found.py` & `trycourier-6.1.0/src/courier/automations/types/accessor_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .base_error import BaseError
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class MessageNotFound(BaseError):
-    type: typing.Literal["invalid_request_error"]
+class AccessorType(UncheckedBaseModel):
+    ref: str = pydantic_v1.Field(alias="$ref")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/commons/types/not_found.py` & `trycourier-6.1.0/src/courier/profiles/types/send_to_slack_channel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .base_error import BaseError
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .slack_base_properties import SlackBaseProperties
 
 
-class NotFound(BaseError):
-    type: typing.Literal["invalid_request_error"]
+class SendToSlackChannel(SlackBaseProperties):
+    channel: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/commons/types/notification_preference_details.py` & `trycourier-6.1.0/src/courier/commons/types/notification_preference_details.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .channel_preference import ChannelPreference
 from .preference_status import PreferenceStatus
 from .rule import Rule
 
 
-class NotificationPreferenceDetails(pydantic_v1.BaseModel):
+class NotificationPreferenceDetails(UncheckedBaseModel):
     status: PreferenceStatus
     rules: typing.Optional[typing.List[Rule]] = None
     channel_preferences: typing.Optional[typing.List[ChannelPreference]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/commons/types/paging.py` & `trycourier-6.1.0/src/courier/profiles/types/snooze_rule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .snooze_rule_type import SnoozeRuleType
 
 
-class Paging(pydantic_v1.BaseModel):
-    cursor: typing.Optional[str] = None
-    more: bool
+class SnoozeRule(UncheckedBaseModel):
+    type: SnoozeRuleType
+    start: str
+    until: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/commons/types/payment_required.py` & `trycourier-6.1.0/src/courier/automations/types/automation_v_2_send_step.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .base_error import BaseError
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...send.types.message import Message
+from .automation_step import AutomationStep
 
 
-class PaymentRequired(BaseError):
-    type: typing.Literal["authorization_error"]
+class AutomationV2SendStep(AutomationStep):
+    action: typing.Literal["send"]
+    message: Message
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/commons/types/recipient_preferences.py` & `trycourier-6.1.0/src/courier/commons/types/recipient_preferences.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .notification_preferences import NotificationPreferences
 
 
-class RecipientPreferences(pydantic_v1.BaseModel):
+class RecipientPreferences(UncheckedBaseModel):
     categories: typing.Optional[NotificationPreferences] = None
     notifications: typing.Optional[NotificationPreferences] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/commons/types/rule.py` & `trycourier-6.1.0/src/courier/profiles/types/subscribe_to_lists_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .subscribe_to_lists_request_list_object import SubscribeToListsRequestListObject
 
 
-class Rule(pydantic_v1.BaseModel):
-    start: typing.Optional[str] = None
-    until: str
+class SubscribeToListsRequest(UncheckedBaseModel):
+    lists: typing.List[SubscribeToListsRequestListObject]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/commons/types/user_tenant_association.py` & `trycourier-6.1.0/src/courier/send/types/widget_background.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class UserTenantAssociation(pydantic_v1.BaseModel):
-    user_id: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    User ID for the assocation between tenant and user
-    """
-
-    type: typing.Optional[typing.Literal["user"]] = None
-    tenant_id: str = pydantic_v1.Field()
-    """
-    Tenant ID for the assocation between tenant and user
-    """
-
-    profile: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
-    """
-    Additional metadata to be applied to a user profile when used in a tenant context
-    """
+class WidgetBackground(UncheckedBaseModel):
+    top_color: typing.Optional[str] = pydantic_v1.Field(alias="topColor", default=None)
+    bottom_color: typing.Optional[str] = pydantic_v1.Field(alias="bottomColor", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/core/client_wrapper.py` & `trycourier-6.1.0/src/courier/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "trycourier",
-            "X-Fern-SDK-Version": "v6.0.5",
+            "X-Fern-SDK-Version": "v6.1.0",
         }
         headers["Authorization"] = f"Bearer {self._get_authorization_token()}"
         return headers
 
     def _get_authorization_token(self) -> str:
         if isinstance(self._authorization_token, str):
             return self._authorization_token
```

### Comparing `trycourier-6.0.5/src/courier/core/datetime_utils.py` & `trycourier-6.1.0/src/courier/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/core/file.py` & `trycourier-6.1.0/src/courier/core/file.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/core/http_client.py` & `trycourier-6.1.0/src/courier/core/http_client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/core/jsonable_encoder.py` & `trycourier-6.1.0/src/courier/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/core/request_options.py` & `trycourier-6.1.0/src/courier/core/request_options.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/lists/client.py` & `trycourier-6.1.0/src/courier/lists/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 from ..commons.errors.not_found_error import NotFoundError
 from ..commons.types.bad_request import BadRequest
 from ..commons.types.not_found import NotFound
 from ..commons.types.recipient_preferences import RecipientPreferences
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
-from .types.list import List
+from ..core.unchecked_base_model import construct_type
+from .types.list_ import List
 from .types.list_get_all_response import ListGetAllResponse
 from .types.list_get_subscriptions_response import ListGetSubscriptionsResponse
 from .types.list_put_params import ListPutParams
 from .types.put_subscriptions_recipient import PutSubscriptionsRecipient
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ListsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(
+    def list_(
         self,
         *,
         cursor: typing.Optional[str] = None,
         pattern: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListGetAllResponse:
         """
@@ -57,33 +58,35 @@
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.lists.list(
+        client.lists.list_(
             cursor="string",
             pattern="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "lists"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        "pattern": pattern,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            "pattern": pattern,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -93,17 +96,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListGetAllResponse, _response.json())  # type: ignore
+            return typing.cast(ListGetAllResponse, construct_type(type_=ListGetAllResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, list_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> List:
@@ -132,16 +137,18 @@
         client.lists.get(
             list_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -150,17 +157,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(List, _response.json())  # type: ignore
+            return typing.cast(List, construct_type(type_=List, object_=_response.json()))  # type: ignore
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFound, construct_type(type_=NotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
@@ -237,16 +246,18 @@
                 ),
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -261,15 +272,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(List, _response.json())  # type: ignore
+            return typing.cast(List, construct_type(type_=List, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, list_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
@@ -298,17 +309,22 @@
         client.lists.delete(
             list_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -355,16 +371,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/restore"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -425,24 +443,26 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/subscriptions"
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -452,39 +472,41 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListGetSubscriptionsResponse, _response.json())  # type: ignore
+            return typing.cast(ListGetSubscriptionsResponse, construct_type(type_=ListGetSubscriptionsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFound, construct_type(type_=NotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_subscribers(
         self,
         list_id: str,
         *,
-        request: typing.Sequence[PutSubscriptionsRecipient],
+        recipients: typing.Sequence[PutSubscriptionsRecipient],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Subscribes the users to the list, overwriting existing subscriptions. If the list does not exist, it will be automatically created.
 
         Parameters
         ----------
         list_id : str
             A unique identifier representing the list you wish to retrieve.
 
-        request : typing.Sequence[PutSubscriptionsRecipient]
+        recipients : typing.Sequence[PutSubscriptionsRecipient]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
         None
@@ -501,15 +523,15 @@
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.lists.update_subscribers(
             list_id="string",
-            request=[
+            recipients=[
                 PutSubscriptionsRecipient(
                     recipient_id="string",
                     preferences=RecipientPreferences(
                         categories={
                             "string": NotificationPreferenceDetails(
                                 status="OPTED_IN",
                                 rules=[
@@ -547,21 +569,23 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/subscriptions"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder({"recipients": recipients})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder({"recipients": recipients}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -573,39 +597,41 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def add_subscribers(
         self,
         list_id: str,
         *,
-        request: typing.Sequence[PutSubscriptionsRecipient],
+        recipients: typing.Sequence[PutSubscriptionsRecipient],
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Subscribes additional users to the list, without modifying existing subscriptions. If the list does not exist, it will be automatically created.
 
         Parameters
         ----------
         list_id : str
             A unique identifier representing the list you wish to retrieve.
 
-        request : typing.Sequence[PutSubscriptionsRecipient]
+        recipients : typing.Sequence[PutSubscriptionsRecipient]
 
         idempotency_key : typing.Optional[str]
 
         idempotency_expiry : typing.Optional[str]
             The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
         request_options : typing.Optional[RequestOptions]
@@ -627,15 +653,15 @@
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         client.lists.add_subscribers(
             list_id="string",
-            request=[
+            recipients=[
                 PutSubscriptionsRecipient(
                     recipient_id="string",
                     preferences=RecipientPreferences(
                         categories={
                             "string": NotificationPreferenceDetails(
                                 status="OPTED_IN",
                                 rules=[
@@ -673,21 +699,23 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/subscriptions"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder({"recipients": recipients})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder({"recipients": recipients}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         "Idempotency-Key": str(idempotency_key) if idempotency_key is not None else None,
@@ -701,15 +729,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def subscribe(
@@ -797,16 +827,18 @@
             _request["preferences"] = preferences
         _response = self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"lists/{jsonable_encoder(list_id)}/subscriptions/{jsonable_encoder(user_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -867,17 +899,22 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"lists/{jsonable_encoder(list_id)}/subscriptions/{jsonable_encoder(user_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -887,27 +924,29 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFound, construct_type(type_=NotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncListsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(
+    async def list_(
         self,
         *,
         cursor: typing.Optional[str] = None,
         pattern: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListGetAllResponse:
         """
@@ -931,33 +970,35 @@
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.lists.list(
+        await client.lists.list_(
             cursor="string",
             pattern="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "lists"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        "pattern": pattern,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            "pattern": pattern,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -967,17 +1008,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListGetAllResponse, _response.json())  # type: ignore
+            return typing.cast(ListGetAllResponse, construct_type(type_=ListGetAllResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, list_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> List:
@@ -1006,16 +1049,18 @@
         await client.lists.get(
             list_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -1024,17 +1069,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(List, _response.json())  # type: ignore
+            return typing.cast(List, construct_type(type_=List, object_=_response.json()))  # type: ignore
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFound, construct_type(type_=NotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
@@ -1111,16 +1158,18 @@
                 ),
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1135,15 +1184,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(List, _response.json())  # type: ignore
+            return typing.cast(List, construct_type(type_=List, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, list_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
@@ -1172,17 +1221,22 @@
         await client.lists.delete(
             list_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -1229,16 +1283,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/restore"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -1299,24 +1355,26 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/subscriptions"
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -1326,39 +1384,41 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListGetSubscriptionsResponse, _response.json())  # type: ignore
+            return typing.cast(ListGetSubscriptionsResponse, construct_type(type_=ListGetSubscriptionsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFound, construct_type(type_=NotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_subscribers(
         self,
         list_id: str,
         *,
-        request: typing.Sequence[PutSubscriptionsRecipient],
+        recipients: typing.Sequence[PutSubscriptionsRecipient],
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Subscribes the users to the list, overwriting existing subscriptions. If the list does not exist, it will be automatically created.
 
         Parameters
         ----------
         list_id : str
             A unique identifier representing the list you wish to retrieve.
 
-        request : typing.Sequence[PutSubscriptionsRecipient]
+        recipients : typing.Sequence[PutSubscriptionsRecipient]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
         None
@@ -1375,15 +1435,15 @@
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.lists.update_subscribers(
             list_id="string",
-            request=[
+            recipients=[
                 PutSubscriptionsRecipient(
                     recipient_id="string",
                     preferences=RecipientPreferences(
                         categories={
                             "string": NotificationPreferenceDetails(
                                 status="OPTED_IN",
                                 rules=[
@@ -1421,21 +1481,23 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/subscriptions"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder({"recipients": recipients})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder({"recipients": recipients}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -1447,39 +1509,41 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add_subscribers(
         self,
         list_id: str,
         *,
-        request: typing.Sequence[PutSubscriptionsRecipient],
+        recipients: typing.Sequence[PutSubscriptionsRecipient],
         idempotency_key: typing.Optional[str] = None,
         idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> None:
         """
         Subscribes additional users to the list, without modifying existing subscriptions. If the list does not exist, it will be automatically created.
 
         Parameters
         ----------
         list_id : str
             A unique identifier representing the list you wish to retrieve.
 
-        request : typing.Sequence[PutSubscriptionsRecipient]
+        recipients : typing.Sequence[PutSubscriptionsRecipient]
 
         idempotency_key : typing.Optional[str]
 
         idempotency_expiry : typing.Optional[str]
             The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
         request_options : typing.Optional[RequestOptions]
@@ -1501,15 +1565,15 @@
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
         await client.lists.add_subscribers(
             list_id="string",
-            request=[
+            recipients=[
                 PutSubscriptionsRecipient(
                     recipient_id="string",
                     preferences=RecipientPreferences(
                         categories={
                             "string": NotificationPreferenceDetails(
                                 status="OPTED_IN",
                                 rules=[
@@ -1547,21 +1611,23 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"lists/{jsonable_encoder(list_id)}/subscriptions"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder({"recipients": recipients})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder({"recipients": recipients}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         "Idempotency-Key": str(idempotency_key) if idempotency_key is not None else None,
@@ -1575,15 +1641,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def subscribe(
@@ -1671,16 +1739,18 @@
             _request["preferences"] = preferences
         _response = await self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"lists/{jsonable_encoder(list_id)}/subscriptions/{jsonable_encoder(user_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1741,17 +1811,22 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"lists/{jsonable_encoder(list_id)}/subscriptions/{jsonable_encoder(user_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -1761,13 +1836,15 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFound, construct_type(type_=NotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/lists/types/__init__.py` & `trycourier-6.1.0/src/courier/lists/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .list import List
+from .list_ import List
 from .list_get_all_response import ListGetAllResponse
 from .list_get_subscriptions_response import ListGetSubscriptionsResponse
 from .list_put_params import ListPutParams
 from .list_subscription_recipient import ListSubscriptionRecipient
 from .put_subscriptions_recipient import PutSubscriptionsRecipient
 
 __all__ = [
```

### Comparing `trycourier-6.0.5/src/courier/lists/types/list.py` & `trycourier-6.1.0/src/courier/bulk/types/bulk_ingest_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class List(pydantic_v1.BaseModel):
-    id: str
-    name: str
-    created: typing.Optional[int] = None
-    updated: typing.Optional[int] = None
+class BulkIngestError(UncheckedBaseModel):
+    user: typing.Any
+    error: typing.Any
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/lists/types/list_get_all_response.py` & `trycourier-6.1.0/src/courier/audit_events/types/list_audit_events_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .list import List
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .audit_event import AuditEvent
 
 
-class ListGetAllResponse(pydantic_v1.BaseModel):
+class ListAuditEventsResponse(UncheckedBaseModel):
     paging: Paging
-    items: typing.List[List]
+    results: typing.List[AuditEvent]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/lists/types/list_get_subscriptions_response.py` & `trycourier-6.1.0/src/courier/templates/types/tag.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .list_subscription_recipient import ListSubscriptionRecipient
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .tag_data import TagData
 
 
-class ListGetSubscriptionsResponse(pydantic_v1.BaseModel):
-    paging: Paging
-    items: typing.List[ListSubscriptionRecipient]
+class Tag(UncheckedBaseModel):
+    data: typing.List[TagData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/lists/types/list_put_params.py` & `trycourier-6.1.0/src/courier/notifications/types/notification_content_hierarchy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.recipient_preferences import RecipientPreferences
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class ListPutParams(pydantic_v1.BaseModel):
-    name: str
-    preferences: typing.Optional[RecipientPreferences] = None
+class NotificationContentHierarchy(UncheckedBaseModel):
+    parent: typing.Optional[str] = None
+    children: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/lists/types/list_subscription_recipient.py` & `trycourier-6.1.0/src/courier/lists/types/put_subscriptions_recipient.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...commons.types.recipient_preferences import RecipientPreferences
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class ListSubscriptionRecipient(pydantic_v1.BaseModel):
+class PutSubscriptionsRecipient(UncheckedBaseModel):
     recipient_id: str = pydantic_v1.Field(alias="recipientId")
-    created: typing.Optional[str] = None
     preferences: typing.Optional[RecipientPreferences] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/lists/types/put_subscriptions_recipient.py` & `trycourier-6.1.0/src/courier/profiles/types/profile_get_parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.recipient_preferences import RecipientPreferences
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class PutSubscriptionsRecipient(pydantic_v1.BaseModel):
+class ProfileGetParameters(UncheckedBaseModel):
     recipient_id: str = pydantic_v1.Field(alias="recipientId")
-    preferences: typing.Optional[RecipientPreferences] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/messages/__init__.py` & `trycourier-6.1.0/src/courier/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/messages/client.py` & `trycourier-6.1.0/src/courier/messages/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 from ..commons.errors.bad_request_error import BadRequestError
 from ..commons.errors.message_not_found_error import MessageNotFoundError
 from ..commons.types.bad_request import BadRequest
 from ..commons.types.message_not_found import MessageNotFound
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from .types.list_messages_response import ListMessagesResponse
 from .types.message_details import MessageDetails
 from .types.message_history_response import MessageHistoryResponse
 from .types.render_output_response import RenderOutputResponse
 
 
 class MessagesClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(
+    def list_(
         self,
         *,
         archived: typing.Optional[bool] = None,
         cursor: typing.Optional[str] = None,
         event: typing.Optional[str] = None,
         list_: typing.Optional[str] = None,
         message_id: typing.Optional[str] = None,
@@ -100,15 +101,15 @@
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.messages.list(
+        client.messages.list_(
             archived=True,
             cursor="string",
             event="string",
             list_="string",
             message_id="string",
             notification="string",
             provider="string",
@@ -120,37 +121,39 @@
             enqueued_after="string",
             trace_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "messages"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "archived": archived,
-                        "cursor": cursor,
-                        "event": event,
-                        "list": list_,
-                        "messageId": message_id,
-                        "notification": notification,
-                        "provider": provider,
-                        "recipient": recipient,
-                        "status": status,
-                        "tag": tag,
-                        "tags": tags,
-                        "tenant_id": tenant_id,
-                        "enqueued_after": enqueued_after,
-                        "traceId": trace_id,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "archived": archived,
+                            "cursor": cursor,
+                            "event": event,
+                            "list": list_,
+                            "messageId": message_id,
+                            "notification": notification,
+                            "provider": provider,
+                            "recipient": recipient,
+                            "status": status,
+                            "tag": tag,
+                            "tags": tags,
+                            "tenant_id": tenant_id,
+                            "enqueued_after": enqueued_after,
+                            "traceId": trace_id,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -160,15 +163,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListMessagesResponse, _response.json())  # type: ignore
+            return typing.cast(ListMessagesResponse, construct_type(type_=ListMessagesResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, message_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> MessageDetails:
@@ -199,16 +202,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -217,19 +222,23 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(MessageDetails, _response.json())  # type: ignore
+            return typing.cast(MessageDetails, construct_type(type_=MessageDetails, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise MessageNotFoundError(pydantic_v1.parse_obj_as(MessageNotFound, _response.json()))  # type: ignore
+            raise MessageNotFoundError(
+                typing.cast(MessageNotFound, construct_type(type_=MessageNotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def cancel(
@@ -272,16 +281,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}/cancel"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -295,15 +306,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(MessageDetails, _response.json())  # type: ignore
+            return typing.cast(MessageDetails, construct_type(type_=MessageDetails, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_history(
@@ -344,24 +355,26 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}/history"
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "type": type,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "type": type,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -371,19 +384,23 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(MessageHistoryResponse, _response.json())  # type: ignore
+            return typing.cast(MessageHistoryResponse, construct_type(type_=MessageHistoryResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise MessageNotFoundError(pydantic_v1.parse_obj_as(MessageNotFound, _response.json()))  # type: ignore
+            raise MessageNotFoundError(
+                typing.cast(MessageNotFound, construct_type(type_=MessageNotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_content(
@@ -414,16 +431,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}/output"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -432,19 +451,23 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(RenderOutputResponse, _response.json())  # type: ignore
+            return typing.cast(RenderOutputResponse, construct_type(type_=RenderOutputResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise MessageNotFoundError(pydantic_v1.parse_obj_as(MessageNotFound, _response.json()))  # type: ignore
+            raise MessageNotFoundError(
+                typing.cast(MessageNotFound, construct_type(type_=MessageNotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def archive(self, request_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
@@ -473,16 +496,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"requests/{jsonable_encoder(request_id)}/archive"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -506,15 +531,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncMessagesClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(
+    async def list_(
         self,
         *,
         archived: typing.Optional[bool] = None,
         cursor: typing.Optional[str] = None,
         event: typing.Optional[str] = None,
         list_: typing.Optional[str] = None,
         message_id: typing.Optional[str] = None,
@@ -586,15 +611,15 @@
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.messages.list(
+        await client.messages.list_(
             archived=True,
             cursor="string",
             event="string",
             list_="string",
             message_id="string",
             notification="string",
             provider="string",
@@ -606,37 +631,39 @@
             enqueued_after="string",
             trace_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "messages"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "archived": archived,
-                        "cursor": cursor,
-                        "event": event,
-                        "list": list_,
-                        "messageId": message_id,
-                        "notification": notification,
-                        "provider": provider,
-                        "recipient": recipient,
-                        "status": status,
-                        "tag": tag,
-                        "tags": tags,
-                        "tenant_id": tenant_id,
-                        "enqueued_after": enqueued_after,
-                        "traceId": trace_id,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "archived": archived,
+                            "cursor": cursor,
+                            "event": event,
+                            "list": list_,
+                            "messageId": message_id,
+                            "notification": notification,
+                            "provider": provider,
+                            "recipient": recipient,
+                            "status": status,
+                            "tag": tag,
+                            "tags": tags,
+                            "tenant_id": tenant_id,
+                            "enqueued_after": enqueued_after,
+                            "traceId": trace_id,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -646,15 +673,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListMessagesResponse, _response.json())  # type: ignore
+            return typing.cast(ListMessagesResponse, construct_type(type_=ListMessagesResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, message_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> MessageDetails:
@@ -685,16 +712,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -703,19 +732,23 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(MessageDetails, _response.json())  # type: ignore
+            return typing.cast(MessageDetails, construct_type(type_=MessageDetails, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise MessageNotFoundError(pydantic_v1.parse_obj_as(MessageNotFound, _response.json()))  # type: ignore
+            raise MessageNotFoundError(
+                typing.cast(MessageNotFound, construct_type(type_=MessageNotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def cancel(
@@ -758,16 +791,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}/cancel"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -781,15 +816,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(MessageDetails, _response.json())  # type: ignore
+            return typing.cast(MessageDetails, construct_type(type_=MessageDetails, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_history(
@@ -830,24 +865,26 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}/history"
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "type": type,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "type": type,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -857,19 +894,23 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(MessageHistoryResponse, _response.json())  # type: ignore
+            return typing.cast(MessageHistoryResponse, construct_type(type_=MessageHistoryResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise MessageNotFoundError(pydantic_v1.parse_obj_as(MessageNotFound, _response.json()))  # type: ignore
+            raise MessageNotFoundError(
+                typing.cast(MessageNotFound, construct_type(type_=MessageNotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_content(
@@ -900,16 +941,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"messages/{jsonable_encoder(message_id)}/output"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -918,19 +961,23 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(RenderOutputResponse, _response.json())  # type: ignore
+            return typing.cast(RenderOutputResponse, construct_type(type_=RenderOutputResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise MessageNotFoundError(pydantic_v1.parse_obj_as(MessageNotFound, _response.json()))  # type: ignore
+            raise MessageNotFoundError(
+                typing.cast(MessageNotFound, construct_type(type_=MessageNotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def archive(self, request_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
@@ -959,16 +1006,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"requests/{jsonable_encoder(request_id)}/archive"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
```

### Comparing `trycourier-6.0.5/src/courier/messages/types/__init__.py` & `trycourier-6.1.0/src/courier/messages/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/messages/types/list_messages_response.py` & `trycourier-6.1.0/src/courier/messages/types/list_messages_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .message_details import MessageDetails
 
 
-class ListMessagesResponse(pydantic_v1.BaseModel):
+class ListMessagesResponse(UncheckedBaseModel):
     paging: Paging = pydantic_v1.Field()
     """
     Paging information for the result set.
     """
 
     results: typing.List[MessageDetails] = pydantic_v1.Field()
     """
@@ -21,15 +22,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/messages/types/message_details.py` & `trycourier-6.1.0/src/courier/messages/types/message_details.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .message_status import MessageStatus
 from .reason import Reason
 
 
-class MessageDetails(pydantic_v1.BaseModel):
+class MessageDetails(UncheckedBaseModel):
     id: str = pydantic_v1.Field()
     """
     A unique identifier associated with the message you wish to retrieve (results from a send).
     """
 
     status: MessageStatus = pydantic_v1.Field()
     """
@@ -71,15 +72,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/messages/types/message_history_response.py` & `trycourier-6.1.0/src/courier/profiles/types/delete_list_subscription_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .message_details import MessageDetails
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class MessageHistoryResponse(pydantic_v1.BaseModel):
-    results: typing.List[MessageDetails]
+class DeleteListSubscriptionResponse(UncheckedBaseModel):
+    status: typing.Literal["SUCCESS"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/messages/types/render_output.py` & `trycourier-6.1.0/src/courier/users/preferences/types/user_preferences_update_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .rendered_message_content import RenderedMessageContent
-
-
-class RenderOutput(pydantic_v1.BaseModel):
-    channel: str = pydantic_v1.Field()
-    """
-    The channel used for rendering the message.
-    """
-
-    channel_id: str = pydantic_v1.Field()
-    """
-    The ID of channel used for rendering the message.
-    """
-
-    content: RenderedMessageContent = pydantic_v1.Field()
-    """
-    Content details of the rendered message.
-    """
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
+
+
+class UserPreferencesUpdateResponse(UncheckedBaseModel):
+    message: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/messages/types/render_output_response.py` & `trycourier-6.1.0/src/courier/send/types/invalid_list_recipient.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .render_output import RenderOutput
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class RenderOutputResponse(pydantic_v1.BaseModel):
-    results: typing.List[RenderOutput] = pydantic_v1.Field()
-    """
-    An array of render output of a previously sent message.
-    """
+class InvalidListRecipient(UncheckedBaseModel):
+    user_id: str
+    list_pattern: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/messages/types/rendered_message_block.py` & `trycourier-6.1.0/src/courier/profiles/types/get_list_subscriptions_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .get_list_subscriptions_list import GetListSubscriptionsList
 
 
-class RenderedMessageBlock(pydantic_v1.BaseModel):
-    type: str = pydantic_v1.Field()
+class GetListSubscriptionsResponse(UncheckedBaseModel):
+    paging: Paging
+    results: typing.List[GetListSubscriptionsList] = pydantic_v1.Field()
     """
-    The block type of the rendered message block.
-    """
-
-    text: str = pydantic_v1.Field()
-    """
-    The block text of the rendered message block.
+    An array of lists
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/messages/types/rendered_message_content.py` & `trycourier-6.1.0/src/courier/messages/types/rendered_message_content.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .rendered_message_block import RenderedMessageBlock
 
 
-class RenderedMessageContent(pydantic_v1.BaseModel):
+class RenderedMessageContent(UncheckedBaseModel):
     html: str = pydantic_v1.Field()
     """
     The html content of the rendered message.
     """
 
     title: str = pydantic_v1.Field()
     """
@@ -40,15 +41,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/notifications/__init__.py` & `trycourier-6.1.0/src/courier/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/notifications/client.py` & `trycourier-6.1.0/src/courier/notifications/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from .types.base_check import BaseCheck
 from .types.notification_block import NotificationBlock
 from .types.notification_channel import NotificationChannel
 from .types.notification_get_content_response import NotificationGetContentResponse
 from .types.notification_list_response import NotificationListResponse
 from .types.submission_checks_get_response import SubmissionChecksGetResponse
 from .types.submission_checks_replace_response import SubmissionChecksReplaceResponse
@@ -22,15 +23,15 @@
 OMIT = typing.cast(typing.Any, ...)
 
 
 class NotificationsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(
+    def list_(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> NotificationListResponse:
         """
         Parameters
         ----------
         cursor : typing.Optional[str]
 
@@ -44,31 +45,33 @@
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.notifications.list(
+        client.notifications.list_(
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "notifications"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -78,15 +81,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(NotificationListResponse, _response.json())  # type: ignore
+            return typing.cast(NotificationListResponse, construct_type(type_=NotificationListResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_content(
@@ -116,16 +119,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/content"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -134,15 +139,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(NotificationGetContentResponse, _response.json())  # type: ignore
+            return typing.cast(NotificationGetContentResponse, construct_type(type_=NotificationGetContentResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_draft_content(
@@ -172,16 +177,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/draft/content"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -190,15 +197,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(NotificationGetContentResponse, _response.json())  # type: ignore
+            return typing.cast(NotificationGetContentResponse, construct_type(type_=NotificationGetContentResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_variations(
@@ -267,16 +274,18 @@
         if channels is not OMIT:
             _request["channels"] = channels
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/variations"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -368,16 +377,18 @@
         if channels is not OMIT:
             _request["channels"] = channels
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/draft/variations"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -434,16 +445,18 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"notifications/{jsonable_encoder(id)}/{jsonable_encoder(submission_id)}/checks",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -452,15 +465,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SubmissionChecksGetResponse, _response.json())  # type: ignore
+            return typing.cast(SubmissionChecksGetResponse, construct_type(type_=SubmissionChecksGetResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def replace_submission_checks(
@@ -509,16 +522,18 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"notifications/{jsonable_encoder(id)}/{jsonable_encoder(submission_id)}/checks",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"checks": checks})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"checks": checks}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -533,15 +548,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SubmissionChecksReplaceResponse, _response.json())  # type: ignore
+            return typing.cast(SubmissionChecksReplaceResponse, construct_type(type_=SubmissionChecksReplaceResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def cancel_submission(
@@ -575,17 +590,22 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"notifications/{jsonable_encoder(id)}/{jsonable_encoder(submission_id)}/checks",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -605,15 +625,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncNotificationsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(
+    async def list_(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> NotificationListResponse:
         """
         Parameters
         ----------
         cursor : typing.Optional[str]
 
@@ -627,31 +647,33 @@
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.notifications.list(
+        await client.notifications.list_(
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "notifications"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -661,15 +683,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(NotificationListResponse, _response.json())  # type: ignore
+            return typing.cast(NotificationListResponse, construct_type(type_=NotificationListResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_content(
@@ -699,16 +721,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/content"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -717,15 +741,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(NotificationGetContentResponse, _response.json())  # type: ignore
+            return typing.cast(NotificationGetContentResponse, construct_type(type_=NotificationGetContentResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_draft_content(
@@ -755,16 +779,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/draft/content"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -773,15 +799,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(NotificationGetContentResponse, _response.json())  # type: ignore
+            return typing.cast(NotificationGetContentResponse, construct_type(type_=NotificationGetContentResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_variations(
@@ -850,16 +876,18 @@
         if channels is not OMIT:
             _request["channels"] = channels
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/variations"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -951,16 +979,18 @@
         if channels is not OMIT:
             _request["channels"] = channels
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"notifications/{jsonable_encoder(id)}/draft/variations"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1017,16 +1047,18 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"notifications/{jsonable_encoder(id)}/{jsonable_encoder(submission_id)}/checks",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -1035,15 +1067,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SubmissionChecksGetResponse, _response.json())  # type: ignore
+            return typing.cast(SubmissionChecksGetResponse, construct_type(type_=SubmissionChecksGetResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def replace_submission_checks(
@@ -1092,16 +1124,18 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"notifications/{jsonable_encoder(id)}/{jsonable_encoder(submission_id)}/checks",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"checks": checks})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"checks": checks}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1116,15 +1150,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SubmissionChecksReplaceResponse, _response.json())  # type: ignore
+            return typing.cast(SubmissionChecksReplaceResponse, construct_type(type_=SubmissionChecksReplaceResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def cancel_submission(
@@ -1158,17 +1192,22 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"notifications/{jsonable_encoder(id)}/{jsonable_encoder(submission_id)}/checks",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/__init__.py` & `trycourier-6.1.0/src/courier/notifications/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/notifications/types/base_check.py` & `trycourier-6.1.0/src/courier/notifications/types/submission_checks_get_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .check_status import CheckStatus
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .check import Check
 
 
-class BaseCheck(pydantic_v1.BaseModel):
-    id: str
-    status: CheckStatus
-    type: typing.Literal["custom"]
+class SubmissionChecksGetResponse(UncheckedBaseModel):
+    checks: typing.List[Check]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/check.py` & `trycourier-6.1.0/src/courier/bulk/types/bulk_create_job_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .base_check import BaseCheck
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class Check(BaseCheck):
-    updated: int
+class BulkCreateJobResponse(UncheckedBaseModel):
+    job_id: str = pydantic_v1.Field(alias="jobId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/message_routing.py` & `trycourier-6.1.0/src/courier/send/types/elemental_content.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from __future__ import annotations
-
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .message_routing_method import MessageRoutingMethod
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .elemental_node import ElementalNode
+
 
+class ElementalContent(UncheckedBaseModel):
+    version: str = pydantic_v1.Field()
+    """
+    For example, "2022-01-01"
+    """
 
-class MessageRouting(pydantic_v1.BaseModel):
-    method: MessageRoutingMethod
-    channels: typing.List[MessageRoutingChannel]
+    brand: typing.Optional[typing.Any] = None
+    elements: typing.List[ElementalNode]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
-
-
-from .message_routing_channel import MessageRoutingChannel  # noqa: E402
-
-MessageRouting.update_forward_refs()
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/notification.py` & `trycourier-6.1.0/src/courier/audit_events/types/audit_event.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .message_routing import MessageRouting
-from .notification_tag import NotificationTag
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .actor import Actor
+from .target import Target
 
 
-class Notification(pydantic_v1.BaseModel):
-    created_at: int
-    updated_at: int
-    id: str
-    routing: MessageRouting
-    tags: typing.Optional[NotificationTag] = None
-    title: typing.Optional[str] = None
-    topic_id: str
+class AuditEvent(UncheckedBaseModel):
+    actor: typing.Optional[Actor] = None
+    target: typing.Optional[Target] = None
+    audit_event_id: str = pydantic_v1.Field(alias="auditEventId")
+    source: str
+    timestamp: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/notification_block.py` & `trycourier-6.1.0/src/courier/users/tokens/types/delete_user_token_opts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .block_type import BlockType
-from .notification_content import NotificationContent
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 
 
-class NotificationBlock(pydantic_v1.BaseModel):
-    alias: typing.Optional[str] = None
-    context: typing.Optional[str] = None
-    id: str
-    type: BlockType
-    content: typing.Optional[NotificationContent] = None
-    locales: typing.Optional[typing.Dict[str, NotificationContent]] = None
-    checksum: typing.Optional[str] = None
+class DeleteUserTokenOpts(UncheckedBaseModel):
+    user_id: str
+    token: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/notification_channel.py` & `trycourier-6.1.0/src/courier/notifications/types/notification_tag.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .notification_channel_content import NotificationChannelContent
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .notification_tag_data import NotificationTagData
 
 
-class NotificationChannel(pydantic_v1.BaseModel):
-    id: str
-    type: typing.Optional[str] = None
-    content: typing.Optional[NotificationChannelContent] = None
-    locales: typing.Optional[typing.Dict[str, NotificationChannelContent]] = None
-    checksum: typing.Optional[str] = None
+class NotificationTag(UncheckedBaseModel):
+    data: typing.List[NotificationTagData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/notification_channel_content.py` & `trycourier-6.1.0/src/courier/tenants/types/default_preferences.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .subscription_topic import SubscriptionTopic
 
 
-class NotificationChannelContent(pydantic_v1.BaseModel):
-    subject: typing.Optional[str] = None
-    title: typing.Optional[str] = None
+class DefaultPreferences(UncheckedBaseModel):
+    items: typing.Optional[typing.List[SubscriptionTopic]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/notification_content_hierarchy.py` & `trycourier-6.1.0/src/courier/profiles/types/send_to_slack_user_id.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .slack_base_properties import SlackBaseProperties
 
 
-class NotificationContentHierarchy(pydantic_v1.BaseModel):
-    parent: typing.Optional[str] = None
-    children: typing.Optional[str] = None
+class SendToSlackUserId(SlackBaseProperties):
+    user_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/notification_get_content_response.py` & `trycourier-6.1.0/src/courier/brands/types/brands_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .notification_block import NotificationBlock
-from .notification_channel import NotificationChannel
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .brand import Brand
 
 
-class NotificationGetContentResponse(pydantic_v1.BaseModel):
-    blocks: typing.Optional[typing.List[NotificationBlock]] = None
-    channels: typing.Optional[typing.List[NotificationChannel]] = None
-    checksum: typing.Optional[str] = None
+class BrandsResponse(UncheckedBaseModel):
+    paging: Paging
+    results: typing.List[Brand]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/notification_list_response.py` & `trycourier-6.1.0/src/courier/messages/types/rendered_message_block.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .notification import Notification
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class NotificationListResponse(pydantic_v1.BaseModel):
-    paging: Paging
-    results: typing.List[Notification]
+class RenderedMessageBlock(UncheckedBaseModel):
+    type: str = pydantic_v1.Field()
+    """
+    The block type of the rendered message block.
+    """
+
+    text: str = pydantic_v1.Field()
+    """
+    The block text of the rendered message block.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/notification_tag.py` & `trycourier-6.1.0/src/courier/commons/types/email.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .notification_tag_data import NotificationTagData
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class NotificationTag(pydantic_v1.BaseModel):
-    data: typing.List[NotificationTagData]
+class Email(UncheckedBaseModel):
+    footer: typing.Any
+    header: typing.Any
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/notification_tag_data.py` & `trycourier-6.1.0/src/courier/profiles/types/token.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class NotificationTagData(pydantic_v1.BaseModel):
-    id: str
-    name: str
+class Token(UncheckedBaseModel):
+    token: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/submission_checks_get_response.py` & `trycourier-6.1.0/src/courier/lists/types/list_get_all_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .check import Check
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .list_ import List
 
 
-class SubmissionChecksGetResponse(pydantic_v1.BaseModel):
-    checks: typing.List[Check]
+class ListGetAllResponse(UncheckedBaseModel):
+    paging: Paging
+    items: typing.List[List]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/notifications/types/submission_checks_replace_response.py` & `trycourier-6.1.0/src/courier/notifications/types/notification_list_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .check import Check
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .notification import Notification
 
 
-class SubmissionChecksReplaceResponse(pydantic_v1.BaseModel):
-    checks: typing.List[Check]
+class NotificationListResponse(UncheckedBaseModel):
+    paging: Paging
+    results: typing.List[Notification]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/__init__.py` & `trycourier-6.1.0/src/courier/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/profiles/client.py` & `trycourier-6.1.0/src/courier/profiles/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from json.decoder import JSONDecodeError
 
 from ..commons.errors.bad_request_error import BadRequestError
 from ..commons.types.bad_request import BadRequest
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from .types.delete_list_subscription_response import DeleteListSubscriptionResponse
 from .types.get_list_subscriptions_response import GetListSubscriptionsResponse
 from .types.merge_profile_response import MergeProfileResponse
 from .types.profile_get_response import ProfileGetResponse
 from .types.replace_profile_response import ReplaceProfileResponse
 from .types.subscribe_to_lists_request import SubscribeToListsRequest
 from .types.subscribe_to_lists_response import SubscribeToListsResponse
@@ -56,16 +57,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -74,17 +77,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ProfileGetResponse, _response.json())  # type: ignore
+            return typing.cast(ProfileGetResponse, construct_type(type_=ProfileGetResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
@@ -131,16 +136,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"profile": profile})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"profile": profile}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -157,17 +164,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(MergeProfileResponse, _response.json())  # type: ignore
+            return typing.cast(MergeProfileResponse, construct_type(type_=MergeProfileResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def replace(
@@ -210,16 +219,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"profile": profile})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"profile": profile}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -234,17 +245,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ReplaceProfileResponse, _response.json())  # type: ignore
+            return typing.cast(ReplaceProfileResponse, construct_type(type_=ReplaceProfileResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
@@ -275,17 +288,22 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -295,15 +313,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_list_subscriptions(
@@ -344,24 +364,26 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}/lists"
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -371,17 +393,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(GetListSubscriptionsResponse, _response.json())  # type: ignore
+            return typing.cast(GetListSubscriptionsResponse, construct_type(type_=GetListSubscriptionsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def subscribe_to_lists(
@@ -431,16 +455,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}/lists"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -457,17 +483,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SubscribeToListsResponse, _response.json())  # type: ignore
+            return typing.cast(SubscribeToListsResponse, construct_type(type_=SubscribeToListsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_list_subscription(
@@ -500,17 +528,22 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}/lists"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -518,17 +551,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DeleteListSubscriptionResponse, _response.json())  # type: ignore
+            return typing.cast(DeleteListSubscriptionResponse, construct_type(type_=DeleteListSubscriptionResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -564,16 +599,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -582,17 +619,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ProfileGetResponse, _response.json())  # type: ignore
+            return typing.cast(ProfileGetResponse, construct_type(type_=ProfileGetResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
@@ -639,16 +678,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"profile": profile})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"profile": profile}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -665,17 +706,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(MergeProfileResponse, _response.json())  # type: ignore
+            return typing.cast(MergeProfileResponse, construct_type(type_=MergeProfileResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def replace(
@@ -718,16 +761,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"profile": profile})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"profile": profile}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -742,17 +787,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ReplaceProfileResponse, _response.json())  # type: ignore
+            return typing.cast(ReplaceProfileResponse, construct_type(type_=ReplaceProfileResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
@@ -783,17 +830,22 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -803,15 +855,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_list_subscriptions(
@@ -852,24 +906,26 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}/lists"
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -879,17 +935,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(GetListSubscriptionsResponse, _response.json())  # type: ignore
+            return typing.cast(GetListSubscriptionsResponse, construct_type(type_=GetListSubscriptionsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def subscribe_to_lists(
@@ -939,16 +997,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}/lists"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -965,17 +1025,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(SubscribeToListsResponse, _response.json())  # type: ignore
+            return typing.cast(SubscribeToListsResponse, construct_type(type_=SubscribeToListsResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_list_subscription(
@@ -1008,17 +1070,22 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"profiles/{jsonable_encoder(user_id)}/lists"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -1026,15 +1093,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(DeleteListSubscriptionResponse, _response.json())  # type: ignore
+            return typing.cast(DeleteListSubscriptionResponse, construct_type(type_=DeleteListSubscriptionResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/__init__.py` & `trycourier-6.1.0/src/courier/profiles/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/profiles/types/address.py` & `trycourier-6.1.0/src/courier/users/tokens/types/put_user_token_opts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
+from .user_token import UserToken
 
 
-class Address(pydantic_v1.BaseModel):
-    formatted: str
-    street_address: str
-    locality: str
-    region: str
-    postal_code: str
-    country: str
+class PutUserTokenOpts(UncheckedBaseModel):
+    user_id: str
+    token: UserToken
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/airship_profile.py` & `trycourier-6.1.0/src/courier/commons/types/rule.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .airship_profile_audience import AirshipProfileAudience
-from .device_type import DeviceType
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class AirshipProfile(pydantic_v1.BaseModel):
-    audience: AirshipProfileAudience
-    device_types: typing.List[DeviceType]
+class Rule(UncheckedBaseModel):
+    start: typing.Optional[str] = None
+    until: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/airship_profile_audience.py` & `trycourier-6.1.0/src/courier/send/types/list_recipient_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class AirshipProfileAudience(pydantic_v1.BaseModel):
-    named_user: str
-
+class ListRecipientType(UncheckedBaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/delete_list_subscription_response.py` & `trycourier-6.1.0/src/courier/send/types/metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .utm import Utm
 
 
-class DeleteListSubscriptionResponse(pydantic_v1.BaseModel):
-    status: typing.Literal["SUCCESS"]
+class Metadata(UncheckedBaseModel):
+    utm: typing.Optional[Utm] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/get_list_subscriptions_list.py` & `trycourier-6.1.0/src/courier/templates/types/tag_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.recipient_preferences import RecipientPreferences
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class GetListSubscriptionsList(pydantic_v1.BaseModel):
-    id: str
-    name: str = pydantic_v1.Field()
-    """
-    List name
-    """
-
-    created: str = pydantic_v1.Field()
+class TagData(UncheckedBaseModel):
+    id: str = pydantic_v1.Field()
     """
-    The date/time of when the list was created. Represented as a string in ISO format.
+    A unique identifier of the tag.
     """
 
-    updated: str = pydantic_v1.Field()
+    name: str = pydantic_v1.Field()
     """
-    The date/time of when the list was updated. Represented as a string in ISO format.
+    Name of the tag.
     """
 
-    preferences: typing.Optional[RecipientPreferences] = None
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/get_list_subscriptions_response.py` & `trycourier-6.1.0/src/courier/profiles/types/send_direct_message.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .get_list_subscriptions_list import GetListSubscriptionsList
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class GetListSubscriptionsResponse(pydantic_v1.BaseModel):
-    paging: Paging
-    results: typing.List[GetListSubscriptionsList] = pydantic_v1.Field()
-    """
-    An array of lists
-    """
+class SendDirectMessage(UncheckedBaseModel):
+    user_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/intercom.py` & `trycourier-6.1.0/src/courier/send/types/list_pattern_recipient_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .intercom_recipient import IntercomRecipient
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class Intercom(pydantic_v1.BaseModel):
-    from_: str = pydantic_v1.Field(alias="from")
-    to: IntercomRecipient
-
+class ListPatternRecipientType(UncheckedBaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/intercom_recipient.py` & `trycourier-6.1.0/src/courier/profiles/types/intercom_recipient.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class IntercomRecipient(pydantic_v1.BaseModel):
+class IntercomRecipient(UncheckedBaseModel):
     id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/ms_teams.py` & `trycourier-6.1.0/src/courier/profiles/types/ms_teams.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/profiles/types/ms_teams_base_properties.py` & `trycourier-6.1.0/src/courier/send/types/slack_recipient.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from ...profiles.types.slack import Slack
 
 
-class MsTeamsBaseProperties(pydantic_v1.BaseModel):
-    tenant_id: str
-    service_url: str
+class SlackRecipient(UncheckedBaseModel):
+    slack: Slack
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/multiple_tokens.py` & `trycourier-6.1.0/src/courier/send/types/tracking_override.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .token import Token
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class MultipleTokens(pydantic_v1.BaseModel):
-    tokens: typing.List[Token]
+class TrackingOverride(UncheckedBaseModel):
+    open: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/profile_get_parameters.py` & `trycourier-6.1.0/src/courier/profiles/types/merge_profile_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class ProfileGetParameters(pydantic_v1.BaseModel):
-    recipient_id: str = pydantic_v1.Field(alias="recipientId")
+class MergeProfileResponse(UncheckedBaseModel):
+    status: typing.Literal["SUCCESS"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/profile_get_response.py` & `trycourier-6.1.0/src/courier/automations/types/automation_throttle_on_throttle.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.recipient_preferences import RecipientPreferences
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class ProfileGetResponse(pydantic_v1.BaseModel):
-    profile: typing.Dict[str, typing.Any]
-    preferences: typing.Optional[RecipientPreferences] = None
+class AutomationThrottleOnThrottle(UncheckedBaseModel):
+    node_id: str = pydantic_v1.Field(alias="$node_id")
+    """
+    The node to go to if the request is throttled
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/send_direct_message.py` & `trycourier-6.1.0/src/courier/commons/types/paging.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class SendDirectMessage(pydantic_v1.BaseModel):
-    user_id: str
+class Paging(UncheckedBaseModel):
+    cursor: typing.Optional[str] = None
+    more: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/send_to_ms_teams_channel_id.py` & `trycourier-6.1.0/src/courier/tenants/types/subscription_topic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .ms_teams_base_properties import MsTeamsBaseProperties
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .subscription_topic_new import SubscriptionTopicNew
 
 
-class SendToMsTeamsChannelId(MsTeamsBaseProperties):
-    channel_id: str
+class SubscriptionTopic(SubscriptionTopicNew):
+    id: str = pydantic_v1.Field()
+    """
+    Topic ID
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/send_to_ms_teams_channel_name.py` & `trycourier-6.1.0/src/courier/automations/types/automation_ad_hoc_invoke_params.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .ms_teams_base_properties import MsTeamsBaseProperties
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .automation import Automation
+from .automation_invoke_params import AutomationInvokeParams
 
 
-class SendToMsTeamsChannelName(MsTeamsBaseProperties):
-    channel_name: str
-    team_id: str
+class AutomationAdHocInvokeParams(AutomationInvokeParams):
+    automation: Automation
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/send_to_ms_teams_email.py` & `trycourier-6.1.0/src/courier/send/types/invalid_list_pattern_recipient.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .ms_teams_base_properties import MsTeamsBaseProperties
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class SendToMsTeamsEmail(MsTeamsBaseProperties):
-    email: str
+class InvalidListPatternRecipient(UncheckedBaseModel):
+    user_id: str
+    list_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/send_to_ms_teams_user_id.py` & `trycourier-6.1.0/src/courier/profiles/types/multiple_tokens.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .ms_teams_base_properties import MsTeamsBaseProperties
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .token import Token
 
 
-class SendToMsTeamsUserId(MsTeamsBaseProperties):
-    user_id: str
+class MultipleTokens(UncheckedBaseModel):
+    tokens: typing.List[Token]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/send_to_slack_channel.py` & `trycourier-6.1.0/src/courier/audiences/types/base_filter_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .slack_base_properties import SlackBaseProperties
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .operator import Operator
 
 
-class SendToSlackChannel(SlackBaseProperties):
-    channel: str
+class BaseFilterConfig(UncheckedBaseModel):
+    operator: Operator = pydantic_v1.Field()
+    """
+    The operator to use for filtering
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/send_to_slack_email.py` & `trycourier-6.1.0/src/courier/profiles/types/airship_profile.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .slack_base_properties import SlackBaseProperties
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .airship_profile_audience import AirshipProfileAudience
+from .device_type import DeviceType
 
 
-class SendToSlackEmail(SlackBaseProperties):
-    email: str
+class AirshipProfile(UncheckedBaseModel):
+    audience: AirshipProfileAudience
+    device_types: typing.List[DeviceType]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/send_to_slack_user_id.py` & `trycourier-6.1.0/src/courier/send/types/base_social_presence.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .slack_base_properties import SlackBaseProperties
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class SendToSlackUserId(SlackBaseProperties):
-    user_id: str
+class BaseSocialPresence(UncheckedBaseModel):
+    url: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/slack_base_properties.py` & `trycourier-6.1.0/src/courier/profiles/types/replace_profile_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class SlackBaseProperties(pydantic_v1.BaseModel):
-    access_token: str
+class ReplaceProfileResponse(UncheckedBaseModel):
+    status: typing.Literal["SUCCESS"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/snooze_rule.py` & `trycourier-6.1.0/src/courier/messages/types/message_history_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .snooze_rule_type import SnoozeRuleType
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class SnoozeRule(pydantic_v1.BaseModel):
-    type: SnoozeRuleType
-    start: str
-    until: str
+class MessageHistoryResponse(UncheckedBaseModel):
+    results: typing.List[typing.Dict[str, typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/subscribe_to_lists_request.py` & `trycourier-6.1.0/src/courier/profiles/types/airship_profile_audience.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .subscribe_to_lists_request_list_object import SubscribeToListsRequestListObject
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class SubscribeToListsRequest(pydantic_v1.BaseModel):
-    lists: typing.List[SubscribeToListsRequestListObject]
+class AirshipProfileAudience(UncheckedBaseModel):
+    named_user: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/subscribe_to_lists_request_list_object.py` & `trycourier-6.1.0/src/courier/profiles/types/intercom.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.recipient_preferences import RecipientPreferences
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .intercom_recipient import IntercomRecipient
 
 
-class SubscribeToListsRequestListObject(pydantic_v1.BaseModel):
-    list_id: str = pydantic_v1.Field(alias="listId")
-    preferences: typing.Optional[RecipientPreferences] = None
+class Intercom(UncheckedBaseModel):
+    from_: str = pydantic_v1.Field(alias="from")
+    to: IntercomRecipient
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/subscribe_to_lists_response.py` & `trycourier-6.1.0/src/courier/bulk/types/bulk_get_job_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .job_details import JobDetails
 
 
-class SubscribeToListsResponse(pydantic_v1.BaseModel):
-    status: typing.Literal["SUCCESS"]
+class BulkGetJobResponse(UncheckedBaseModel):
+    job: JobDetails
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/profiles/types/user_profile.py` & `trycourier-6.1.0/src/courier/profiles/types/user_profile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .address import Address
 from .airship_profile import AirshipProfile
 from .discord import Discord
 from .expo import Expo
 from .intercom import Intercom
 from .ms_teams import MsTeams
 from .slack import Slack
 
 
-class UserProfile(pydantic_v1.BaseModel):
+class UserProfile(UncheckedBaseModel):
     address: Address
     birthdate: str
     email: str
     email_verified: bool
     family_name: str
     gender: str
     given_name: str
@@ -52,16 +53,20 @@
     ms_teams: MsTeams
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/__init__.py` & `trycourier-6.1.0/src/courier/send/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/send/types/__init__.py` & `trycourier-6.1.0/src/courier/send/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/send/types/audience_filter.py` & `trycourier-6.1.0/src/courier/send/types/audience_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class AudienceFilter(pydantic_v1.BaseModel):
+class AudienceFilter(UncheckedBaseModel):
     operator: typing.Literal["MEMBER_OF"] = pydantic_v1.Field()
     """
     Send to users only if they are member of the account
     """
 
     path: typing.Literal["account_id"]
     value: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/audience_recipient.py` & `trycourier-6.1.0/src/courier/send/types/audience_recipient.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .audience_filter import AudienceFilter
 from .message_data import MessageData
 
 
-class AudienceRecipient(pydantic_v1.BaseModel):
+class AudienceRecipient(UncheckedBaseModel):
     audience_id: str = pydantic_v1.Field()
     """
     A unique identifier associated with an Audience. A message will be sent to each user in the audience.
     """
 
     data: typing.Optional[MessageData] = None
     filters: typing.Optional[typing.List[AudienceFilter]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/base_message.py` & `trycourier-6.1.0/src/courier/send/types/base_message.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .delay import Delay
 from .expiry import Expiry
 from .message_channels import MessageChannels
 from .message_context import MessageContext
 from .message_data import MessageData
 from .message_metadata import MessageMetadata
 from .message_providers import MessageProviders
 from .routing import Routing
 from .timeout import Timeout
 
 
-class BaseMessage(pydantic_v1.BaseModel):
+class BaseMessage(UncheckedBaseModel):
     data: typing.Optional[MessageData] = pydantic_v1.Field(default=None)
     """
     An arbitrary object that includes any data you want to pass to the message.
     The data will populate the corresponding template or elements variables.
     """
 
     brand_id: typing.Optional[str] = None
@@ -62,15 +63,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/base_message_send_to.py` & `trycourier-6.1.0/src/courier/send/types/timeout.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .message_recipient import MessageRecipient
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .criteria import Criteria
 
 
-class BaseMessageSendTo(pydantic_v1.BaseModel):
-    to: typing.Optional[MessageRecipient] = pydantic_v1.Field(default=None)
-    """
-    The recipient or a list of recipients of the message
-    """
+class Timeout(UncheckedBaseModel):
+    provider: typing.Optional[typing.Dict[str, int]] = None
+    channel: typing.Optional[typing.Dict[str, int]] = None
+    message: typing.Optional[int] = None
+    escalation: typing.Optional[int] = None
+    criteria: typing.Optional[Criteria] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/base_social_presence.py` & `trycourier-6.1.0/src/courier/send/types/delay.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class BaseSocialPresence(pydantic_v1.BaseModel):
-    url: str
+class Delay(UncheckedBaseModel):
+    duration: int = pydantic_v1.Field()
+    """
+    The duration of the delay in milliseconds.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/brand_settings_email.py` & `trycourier-6.1.0/src/courier/send/types/brand_settings_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .brand_template_override import BrandTemplateOverride
 from .email_footer import EmailFooter
 from .email_head import EmailHead
 from .email_header import EmailHeader
 
 
-class BrandSettingsEmail(pydantic_v1.BaseModel):
+class BrandSettingsEmail(UncheckedBaseModel):
     template_override: typing.Optional[BrandTemplateOverride] = pydantic_v1.Field(
         alias="templateOverride", default=None
     )
     head: typing.Optional[EmailHead] = None
     footer: typing.Optional[EmailFooter] = None
     header: typing.Optional[EmailHeader] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/brand_settings_in_app.py` & `trycourier-6.1.0/src/courier/send/types/brand_settings_in_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...brands.types.brand_colors import BrandColors
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .icons import Icons
 from .in_app_placement import InAppPlacement
 from .preferences import Preferences
 from .widget_background import WidgetBackground
 
 
-class BrandSettingsInApp(pydantic_v1.BaseModel):
+class BrandSettingsInApp(UncheckedBaseModel):
     border_radius: typing.Optional[str] = pydantic_v1.Field(alias="borderRadius", default=None)
     disable_message_icon: typing.Optional[bool] = pydantic_v1.Field(alias="disableMessageIcon", default=None)
     font_family: typing.Optional[str] = pydantic_v1.Field(alias="fontFamily", default=None)
     placement: typing.Optional[InAppPlacement] = None
     widget_background: WidgetBackground = pydantic_v1.Field(alias="widgetBackground")
     colors: BrandColors
     icons: Icons
     preferences: Preferences
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/brand_settings_social_presence.py` & `trycourier-6.1.0/src/courier/notifications/types/message_routing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from __future__ import annotations
+
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .base_social_presence import BaseSocialPresence
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .message_routing_method import MessageRoutingMethod
 
 
-class BrandSettingsSocialPresence(pydantic_v1.BaseModel):
-    inherit_default: typing.Optional[bool] = pydantic_v1.Field(alias="inheritDefault", default=None)
-    facebook: typing.Optional[BaseSocialPresence] = None
-    instagram: typing.Optional[BaseSocialPresence] = None
-    linkedin: typing.Optional[BaseSocialPresence] = None
-    medium: typing.Optional[BaseSocialPresence] = None
-    twitter: typing.Optional[BaseSocialPresence] = None
+class MessageRouting(UncheckedBaseModel):
+    method: MessageRoutingMethod
+    channels: typing.List[MessageRoutingChannel]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
+
+
+from .message_routing_channel import MessageRoutingChannel  # noqa: E402
+
+MessageRouting.update_forward_refs()
```

### Comparing `trycourier-6.0.5/src/courier/send/types/brand_template.py` & `trycourier-6.1.0/src/courier/send/types/brand_template.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class BrandTemplate(pydantic_v1.BaseModel):
+class BrandTemplate(UncheckedBaseModel):
     background_color: typing.Optional[str] = pydantic_v1.Field(alias="backgroundColor", default=None)
     blocks_background_color: typing.Optional[str] = pydantic_v1.Field(alias="blocksBackgroundColor", default=None)
     enabled: bool
     footer: typing.Optional[str] = None
     head: typing.Optional[str] = None
     header: typing.Optional[str] = None
     width: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/brand_template_override.py` & `trycourier-6.1.0/src/courier/send/types/brand_template_override.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .brand_template import BrandTemplate
 
 
 class BrandTemplateOverride(BrandTemplate):
     mjml: BrandTemplate
     footer_background_color: typing.Optional[str] = pydantic_v1.Field(alias="footerBackgroundColor", default=None)
     footer_full_width: typing.Optional[bool] = pydantic_v1.Field(alias="footerFullWidth", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/channel.py` & `trycourier-6.1.0/src/courier/send/types/channel.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .channel_metadata import ChannelMetadata
 from .override import Override
 from .routing_method import RoutingMethod
 from .timeouts import Timeouts
 
 
-class Channel(pydantic_v1.BaseModel):
+class Channel(UncheckedBaseModel):
     brand_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     Id of the brand that should be used for rendering the message.
     If not specified, the brand configured as default brand will be used.
     """
 
     providers: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
@@ -47,16 +48,20 @@
     metadata: typing.Optional[ChannelMetadata] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/channel_metadata.py` & `trycourier-6.1.0/src/courier/lists/types/list_.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .utm import Utm
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class ChannelMetadata(pydantic_v1.BaseModel):
-    utm: typing.Optional[Utm] = None
+class List(UncheckedBaseModel):
+    id: str
+    name: str
+    created: typing.Optional[int] = None
+    updated: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/content_message.py` & `trycourier-6.1.0/src/courier/bulk/types/inbound_bulk_content_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .base_message import BaseMessage
-from .base_message_send_to import BaseMessageSendTo
-from .content import Content
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...send.types.base_message import BaseMessage
+from ...send.types.content import Content
 
 
-class ContentMessage(BaseMessage, BaseMessageSendTo):
+class InboundBulkContentMessage(BaseMessage):
     """
     The message property has the following primary top-level properties. They define the destination and content of the message.
     Additional advanced configuration fields [are defined below](https://www.courier.com/docs/reference/send/message/#other-message-properties).
     """
 
     content: Content = pydantic_v1.Field()
     """
@@ -23,16 +22,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/delay.py` & `trycourier-6.1.0/src/courier/profiles/types/send_to_channel.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class Delay(pydantic_v1.BaseModel):
-    duration: int = pydantic_v1.Field()
-    """
-    The duration of the delay in milliseconds.
-    """
+class SendToChannel(UncheckedBaseModel):
+    channel_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/elemental_action_node.py` & `trycourier-6.1.0/src/courier/send/types/elemental_action_node.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .elemental_base_node import ElementalBaseNode
 from .i_action_button_style import IActionButtonStyle
 from .i_alignment import IAlignment
 from .locales import Locales
 
 
 class ElementalActionNode(ElementalBaseNode):
@@ -52,16 +52,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/elemental_base_node.py` & `trycourier-6.1.0/src/courier/send/types/routing_strategy_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .metadata import Metadata
 
 
-class ElementalBaseNode(pydantic_v1.BaseModel):
-    channels: typing.Optional[typing.List[str]] = None
-    ref: typing.Optional[str] = None
+class RoutingStrategyProvider(UncheckedBaseModel):
+    name: str
+    config: typing.Optional[typing.Dict[str, typing.Any]] = None
     if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
-    loop: typing.Optional[str] = None
+    metadata: Metadata
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/elemental_channel_node.py` & `trycourier-6.1.0/src/courier/send/types/elemental_channel_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .elemental_base_node import ElementalBaseNode
 
 
 class ElementalChannelNode(ElementalBaseNode):
     """
     The channel element allows a notification to be customized based on which channel it is sent through.
     For example, you may want to display a detailed message when the notification is sent through email,
@@ -41,16 +41,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/elemental_content.py` & `trycourier-6.1.0/src/courier/users/preferences/types/user_preferences_get_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .elemental_node import ElementalNode
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
+from .topic_preference import TopicPreference
 
 
-class ElementalContent(pydantic_v1.BaseModel):
-    version: str = pydantic_v1.Field()
-    """
-    For example, "2022-01-01"
-    """
-
-    brand: typing.Optional[typing.Any] = None
-    elements: typing.List[ElementalNode]
+class UserPreferencesGetResponse(UncheckedBaseModel):
+    topic: TopicPreference
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/elemental_content_sugar.py` & `trycourier-6.1.0/src/courier/send/types/message_providers_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .metadata import Metadata
 
 
-class ElementalContentSugar(pydantic_v1.BaseModel):
+class MessageProvidersType(UncheckedBaseModel):
+    override: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
     """
-    Syntatic Sugar to provide a fast shorthand for Courier Elemental Blocks.
+    Provider specific overrides.
     """
 
-    title: str = pydantic_v1.Field()
+    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
     """
-    The title to be displayed by supported channels i.e. push, email (as subject)
+    A JavaScript conditional expression to determine if the message should be sent
+    through the channel. Has access to the data and profile object. For example,
+    `data.name === profile.name`
     """
 
-    body: str = pydantic_v1.Field()
-    """
-    The text content displayed in the notification.
-    """
+    timeouts: typing.Optional[int] = None
+    metadata: typing.Optional[Metadata] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/elemental_divider_node.py` & `trycourier-6.1.0/src/courier/send/types/elemental_meta_node.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .elemental_base_node import ElementalBaseNode
 
 
-class ElementalDividerNode(ElementalBaseNode):
+class ElementalMetaNode(ElementalBaseNode):
     """
-    Renders a dividing line between elements.
+    The meta element contains information describing the notification that may
+    be used by a particular channel or provider. One important field is the title
+    field which will be used as the title for channels that support it.
     """
 
-    color: typing.Optional[str] = pydantic_v1.Field(default=None)
+    title: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The CSS color to render the line with. For example, `#fff`
+    The title to be displayed by supported channels. For example, the email subject.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/elemental_group_node.py` & `trycourier-6.1.0/src/courier/send/types/elemental_group_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .elemental_base_node import ElementalBaseNode
 
 
 class ElementalGroupNode(ElementalBaseNode):
     """
     Allows you to group elements together. This can be useful when used in combination with "if" or "loop". See [control flow docs](https://www.courier.com/docs/platform/content/elemental/control-flow/) for more details.
     """
@@ -21,16 +21,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/elemental_image_node.py` & `trycourier-6.1.0/src/courier/send/types/elemental_quote_node.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .elemental_base_node import ElementalBaseNode
 from .i_alignment import IAlignment
+from .locales import Locales
+from .text_style import TextStyle
 
 
-class ElementalImageNode(ElementalBaseNode):
+class ElementalQuoteNode(ElementalBaseNode):
     """
-    Used to embed an image into the notification.
+    Renders a quote block.
     """
 
-    src: str = pydantic_v1.Field()
+    content: str = pydantic_v1.Field()
     """
-    The source of the image.
-    """
-
-    href: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    A URL to link to when the image is clicked.
+    The text value of the quote.
     """
 
     align: typing.Optional[IAlignment] = pydantic_v1.Field(default=None)
     """
-    The alignment of the image.
+    Alignment of the quote.
     """
 
-    alt_text: typing.Optional[str] = pydantic_v1.Field(alias="altText", default=None)
+    border_color: typing.Optional[str] = pydantic_v1.Field(alias="borderColor", default=None)
     """
-    Alternate text for the image.
+    CSS border color property. For example, `#fff`
     """
 
-    width: typing.Optional[str] = pydantic_v1.Field(default=None)
+    text_style: TextStyle
+    locales: Locales = pydantic_v1.Field()
     """
-    CSS width properties to apply to the image. For example, 50px
+    Region specific content. See [locales docs](https://www.courier.com/docs/platform/content/elemental/locales/) for more details.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/elemental_meta_node.py` & `trycourier-6.1.0/src/courier/audiences/types/nested_filter_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from __future__ import annotations
+
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .elemental_base_node import ElementalBaseNode
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .base_filter_config import BaseFilterConfig
 
 
-class ElementalMetaNode(ElementalBaseNode):
+class NestedFilterConfig(BaseFilterConfig):
     """
-    The meta element contains information describing the notification that may
-    be used by a particular channel or provider. One important field is the title
-    field which will be used as the title for channels that support it.
+    The operator to use for filtering
     """
 
-    title: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    The title to be displayed by supported channels. For example, the email subject.
-    """
+    rules: typing.List[FilterConfig]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
+
+
+from .filter_config import FilterConfig  # noqa: E402
+
+NestedFilterConfig.update_forward_refs()
```

### Comparing `trycourier-6.0.5/src/courier/send/types/elemental_node.py` & `trycourier-6.1.0/src/courier/send/types/elemental_node.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/send/types/elemental_quote_node.py` & `trycourier-6.1.0/src/courier/templates/types/notification_templates.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,60 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .elemental_base_node import ElementalBaseNode
-from .i_alignment import IAlignment
-from .locales import Locales
-from .text_style import TextStyle
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .routing_strategy import RoutingStrategy
+from .tag import Tag
 
 
-class ElementalQuoteNode(ElementalBaseNode):
+class NotificationTemplates(UncheckedBaseModel):
+    created_at: int = pydantic_v1.Field()
     """
-    Renders a quote block.
+    A UTC timestamp at which notification was created. This is stored as a millisecond representation of the Unix epoch (the time passed since January 1, 1970).
     """
 
-    content: str = pydantic_v1.Field()
+    id: str = pydantic_v1.Field()
     """
-    The text value of the quote.
+    A unique identifier associated with the notification.
     """
 
-    align: typing.Optional[IAlignment] = pydantic_v1.Field(default=None)
+    routing: RoutingStrategy = pydantic_v1.Field()
     """
-    Alignment of the quote.
+    Routing strategy used by this notification.
     """
 
-    border_color: typing.Optional[str] = pydantic_v1.Field(alias="borderColor", default=None)
+    tags: typing.List[Tag] = pydantic_v1.Field()
     """
-    CSS border color property. For example, `#fff`
+    A list of tags attached to the notification.
     """
 
-    text_style: TextStyle
-    locales: Locales = pydantic_v1.Field()
+    title: str = pydantic_v1.Field()
     """
-    Region specific content. See [locales docs](https://www.courier.com/docs/platform/content/elemental/locales/) for more details.
+    The title of the notification.
+    """
+
+    updated_at: int = pydantic_v1.Field()
+    """
+    A UTC timestamp at which notification was updated. This is stored as a millisecond representation of the Unix epoch (the time passed since January 1, 1970).
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/elemental_text_node.py` & `trycourier-6.1.0/src/courier/send/types/elemental_text_node.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .elemental_base_node import ElementalBaseNode
 from .locales import Locales
 from .text_align import TextAlign
 from .text_style import TextStyle
 
 
 class ElementalTextNode(ElementalBaseNode):
@@ -65,16 +65,20 @@
     format: typing.Optional[typing.Literal["markdown"]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/email_footer.py` & `trycourier-6.1.0/src/courier/commons/types/payment_required.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .base_error import BaseError
 
 
-class EmailFooter(pydantic_v1.BaseModel):
-    content: typing.Optional[typing.Any] = None
-    inherit_default: typing.Optional[bool] = pydantic_v1.Field(alias="inheritDefault", default=None)
+class PaymentRequired(BaseError):
+    type: typing.Literal["authorization_error"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/email_head.py` & `trycourier-6.1.0/src/courier/send/types/logo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class EmailHead(pydantic_v1.BaseModel):
-    inherit_default: bool = pydantic_v1.Field(alias="inheritDefault")
-    content: typing.Optional[str] = None
+class Logo(UncheckedBaseModel):
+    href: typing.Optional[str] = None
+    image: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/email_header.py` & `trycourier-6.1.0/src/courier/send/types/elemental_base_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .logo import Logo
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class EmailHeader(pydantic_v1.BaseModel):
-    inherit_default: typing.Optional[bool] = pydantic_v1.Field(alias="inheritDefault", default=None)
-    bar_color: typing.Optional[str] = pydantic_v1.Field(alias="barColor", default=None)
-    logo: Logo
+class ElementalBaseNode(UncheckedBaseModel):
+    channels: typing.Optional[typing.List[str]] = None
+    ref: typing.Optional[str] = None
+    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
+    loop: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/expiry.py` & `trycourier-6.1.0/src/courier/commons/types/channel_preference.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .expires_in_type import ExpiresInType
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .channel_classification import ChannelClassification
 
 
-class Expiry(pydantic_v1.BaseModel):
-    expires_at: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    An epoch timestamp or ISO8601 timestamp with timezone `(YYYY-MM-DDThh:mm:ss.sTZD)` that describes the time in which a message expires.
-    """
-
-    expires_in: ExpiresInType = pydantic_v1.Field()
-    """
-    A duration in the form of milliseconds or an ISO8601 Duration format (i.e. P1DT4H).
-    """
+class ChannelPreference(UncheckedBaseModel):
+    channel: ChannelClassification
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/i_profile_preferences.py` & `trycourier-6.1.0/src/courier/send/types/email_header.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .i_preferences import IPreferences
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .logo import Logo
 
 
-class IProfilePreferences(pydantic_v1.BaseModel):
-    categories: typing.Optional[IPreferences] = None
-    notifications: IPreferences
-    template_id: typing.Optional[str] = pydantic_v1.Field(alias="templateId", default=None)
+class EmailHeader(UncheckedBaseModel):
+    inherit_default: typing.Optional[bool] = pydantic_v1.Field(alias="inheritDefault", default=None)
+    bar_color: typing.Optional[str] = pydantic_v1.Field(alias="barColor", default=None)
+    logo: Logo
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/list_pattern_recipient.py` & `trycourier-6.1.0/src/courier/send/types/icons.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .list_pattern_recipient_type import ListPatternRecipientType
-from .message_data import MessageData
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class ListPatternRecipient(ListPatternRecipientType):
-    list_pattern: typing.Optional[str] = None
-    data: typing.Optional[MessageData] = None
+class Icons(UncheckedBaseModel):
+    bell: typing.Optional[str] = None
+    message: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/list_recipient.py` & `trycourier-6.1.0/src/courier/automations/types/automation_send_list_step.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .list_filter import ListFilter
-from .list_recipient_type import ListRecipientType
-from .message_data import MessageData
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .automation_step import AutomationStep
 
 
-class ListRecipient(ListRecipientType):
-    list_id: typing.Optional[str] = None
-    data: typing.Optional[MessageData] = None
-    filters: typing.Optional[typing.List[ListFilter]] = None
+class AutomationSendListStep(AutomationStep):
+    action: typing.Literal["send-list"]
+    brand: typing.Optional[str] = None
+    data: typing.Optional[typing.Dict[str, typing.Any]] = None
+    list_: str = pydantic_v1.Field(alias="list")
+    override: typing.Optional[typing.Dict[str, typing.Any]] = None
+    template: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/locale.py` & `trycourier-6.1.0/src/courier/send/types/ms_teams_recipient.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from ...profiles.types.ms_teams import MsTeams
 
 
-class Locale(pydantic_v1.BaseModel):
-    content: str
+class MsTeamsRecipient(UncheckedBaseModel):
+    ms_teams: MsTeams
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/logo.py` & `trycourier-6.1.0/src/courier/notifications/types/notification_tag_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class Logo(pydantic_v1.BaseModel):
-    href: typing.Optional[str] = None
-    image: typing.Optional[str] = None
+class NotificationTagData(UncheckedBaseModel):
+    id: str
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/message_channel_email_override.py` & `trycourier-6.1.0/src/courier/brands/types/brand_colors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...brands.types.brand import Brand
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .attachment import Attachment
-from .tracking_override import TrackingOverride
-
-
-class MessageChannelEmailOverride(pydantic_v1.BaseModel):
-    attachments: typing.Optional[typing.List[Attachment]] = None
-    bcc: typing.Optional[str] = None
-    brand: typing.Optional[Brand] = None
-    cc: typing.Optional[str] = None
-    from_: typing.Optional[str] = pydantic_v1.Field(alias="from", default=None)
-    html: typing.Optional[str] = None
-    reply_to: typing.Optional[str] = None
-    subject: typing.Optional[str] = None
-    text: typing.Optional[str] = None
-    tracking: TrackingOverride
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+
+
+class BrandColors(UncheckedBaseModel):
+    primary: typing.Optional[str] = None
+    secondary: typing.Optional[str] = None
+    tertiary: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/message_context.py` & `trycourier-6.1.0/src/courier/send/types/message_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class MessageContext(pydantic_v1.BaseModel):
+class MessageContext(UncheckedBaseModel):
     tenant_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     An id of a tenant, see [tenants api docs](https://www.courier.com/docs/reference/tenants/).
     Will load brand, default preferences and any other base context data associated with this tenant.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/message_metadata.py` & `trycourier-6.1.0/src/courier/send/types/message_metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .utm import Utm
 
 
-class MessageMetadata(pydantic_v1.BaseModel):
+class MessageMetadata(UncheckedBaseModel):
     event: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     An arbitrary string to tracks the event that generated this request (e.g. 'signup').
     """
 
     tags: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
     """
@@ -30,15 +31,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/message_providers_type.py` & `trycourier-6.1.0/src/courier/send/types/elemental_divider_node.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .metadata import Metadata
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .elemental_base_node import ElementalBaseNode
 
 
-class MessageProvidersType(pydantic_v1.BaseModel):
-    override: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+class ElementalDividerNode(ElementalBaseNode):
     """
-    Provider specific overrides.
+    Renders a dividing line between elements.
     """
 
-    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
+    color: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    A JavaScript conditional expression to determine if the message should be sent
-    through the channel. Has access to the data and profile object. For example,
-    `data.name === profile.name`
+    The CSS color to render the line with. For example, `#fff`
     """
 
-    timeouts: typing.Optional[int] = None
-    metadata: typing.Optional[Metadata] = None
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/metadata.py` & `trycourier-6.1.0/src/courier/brands/types/brand_settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.email import Email
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .utm import Utm
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .brand_colors import BrandColors
 
 
-class Metadata(pydantic_v1.BaseModel):
-    utm: typing.Optional[Utm] = None
+class BrandSettings(UncheckedBaseModel):
+    colors: typing.Optional[BrandColors] = None
+    inapp: typing.Optional[typing.Any] = None
+    email: typing.Optional[Email] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/ms_teams_recipient.py` & `trycourier-6.1.0/src/courier/lists/types/list_get_subscriptions_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from ...profiles.types.ms_teams import MsTeams
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .list_subscription_recipient import ListSubscriptionRecipient
 
 
-class MsTeamsRecipient(pydantic_v1.BaseModel):
-    ms_teams: MsTeams
+class ListGetSubscriptionsResponse(UncheckedBaseModel):
+    paging: Paging
+    items: typing.List[ListSubscriptionRecipient]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/preference.py` & `trycourier-6.1.0/src/courier/send/types/timeouts.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.channel_preference import ChannelPreference
-from ...commons.types.preference_status import PreferenceStatus
-from ...commons.types.rule import Rule
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .channel_source import ChannelSource
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class Preference(pydantic_v1.BaseModel):
-    status: PreferenceStatus
-    rules: typing.Optional[typing.List[Rule]] = None
-    channel_preferences: typing.Optional[typing.List[ChannelPreference]] = None
-    source: typing.Optional[ChannelSource] = None
+class Timeouts(UncheckedBaseModel):
+    provider: typing.Optional[int] = None
+    channel: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/recipient.py` & `trycourier-6.1.0/src/courier/send/types/recipient.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/send/types/routing.py` & `trycourier-6.1.0/src/courier/send/types/routing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .routing_channel import RoutingChannel
 from .routing_method import RoutingMethod
 
 
-class Routing(pydantic_v1.BaseModel):
+class Routing(UncheckedBaseModel):
     """
     Allows you to customize which channel(s) Courier will potentially deliver the message.
     If no routing key is specified, Courier will use the default routing configuration or
     routing defined by the template.
     """
 
     method: RoutingMethod
@@ -25,15 +26,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/routing_strategy_channel.py` & `trycourier-6.1.0/src/courier/commons/types/already_exists.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .message_providers import MessageProviders
-from .routing_method import RoutingMethod
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .base_error import BaseError
 
 
-class RoutingStrategyChannel(pydantic_v1.BaseModel):
-    channel: str
-    config: typing.Optional[typing.Dict[str, typing.Any]] = None
-    method: typing.Optional[RoutingMethod] = None
-    providers: typing.Optional[MessageProviders] = None
-    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
+class AlreadyExists(BaseError):
+    type: typing.Literal["invalid_request_error"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/routing_strategy_provider.py` & `trycourier-6.1.0/src/courier/users/tokens/types/tracking.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,49 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .metadata import Metadata
-
-
-class RoutingStrategyProvider(pydantic_v1.BaseModel):
-    name: str
-    config: typing.Optional[typing.Dict[str, typing.Any]] = None
-    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
-    metadata: Metadata
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
+
+
+class Tracking(UncheckedBaseModel):
+    os_version: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The operating system version
+    """
+
+    ip: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The IP address of the device
+    """
+
+    lat: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The latitude of the device
+    """
+
+    long_: typing.Optional[str] = pydantic_v1.Field(alias="long", default=None)
+    """
+    The longitude of the device
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/slack_recipient.py` & `trycourier-6.1.0/src/courier/profiles/types/address.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from ...profiles.types.slack import Slack
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class SlackRecipient(pydantic_v1.BaseModel):
-    slack: Slack
+class Address(UncheckedBaseModel):
+    formatted: str
+    street_address: str
+    locality: str
+    region: str
+    postal_code: str
+    country: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/template_message.py` & `trycourier-6.1.0/src/courier/send/types/template_message.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .base_message import BaseMessage
 from .base_message_send_to import BaseMessageSendTo
 
 
 class TemplateMessage(BaseMessage, BaseMessageSendTo):
     template: str = pydantic_v1.Field()
     """
@@ -17,16 +17,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/timeout.py` & `trycourier-6.1.0/src/courier/automations/types/automation_fetch_data_webhook.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .criteria import Criteria
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .automation_fetch_data_webhook_method import AutomationFetchDataWebhookMethod
 
 
-class Timeout(pydantic_v1.BaseModel):
-    provider: typing.Optional[typing.Dict[str, int]] = None
-    channel: typing.Optional[typing.Dict[str, int]] = None
-    message: typing.Optional[int] = None
-    escalation: typing.Optional[int] = None
-    criteria: typing.Optional[Criteria] = None
+class AutomationFetchDataWebhook(UncheckedBaseModel):
+    body: typing.Optional[typing.Dict[str, typing.Any]] = None
+    headers: typing.Optional[typing.Dict[str, typing.Any]] = None
+    params: typing.Optional[typing.Dict[str, typing.Any]] = None
+    method: AutomationFetchDataWebhookMethod
+    url: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/timeouts.py` & `trycourier-6.1.0/src/courier/profiles/types/slack_base_properties.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class Timeouts(pydantic_v1.BaseModel):
-    provider: typing.Optional[int] = None
-    channel: typing.Optional[int] = None
+class SlackBaseProperties(UncheckedBaseModel):
+    access_token: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/user_recipient.py` & `trycourier-6.1.0/src/courier/send/types/user_recipient.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .i_profile_preferences import IProfilePreferences
 from .message_context import MessageContext
 from .message_data import MessageData
 from .user_recipient_type import UserRecipientType
 
 
 class UserRecipient(UserRecipientType):
@@ -39,16 +39,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/send/types/utm.py` & `trycourier-6.1.0/src/courier/automations/types/automation_invoke_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .profile import Profile
 
 
-class Utm(pydantic_v1.BaseModel):
-    source: typing.Optional[str] = None
-    medium: typing.Optional[str] = None
-    campaign: typing.Optional[str] = None
-    term: typing.Optional[str] = None
-    content: typing.Optional[str] = None
+class AutomationInvokeParams(UncheckedBaseModel):
+    brand: typing.Optional[str] = None
+    data: typing.Optional[typing.Dict[str, typing.Any]] = None
+    profile: typing.Optional[Profile] = None
+    recipient: typing.Optional[str] = None
+    template: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/send/types/widget_background.py` & `trycourier-6.1.0/src/courier/send/types/invalid_user_recipient.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class WidgetBackground(pydantic_v1.BaseModel):
-    top_color: typing.Optional[str] = pydantic_v1.Field(alias="topColor", default=None)
-    bottom_color: typing.Optional[str] = pydantic_v1.Field(alias="bottomColor", default=None)
+class InvalidUserRecipient(UncheckedBaseModel):
+    list_id: str
+    list_pattern: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/templates/client.py` & `trycourier-6.1.0/src/courier/templates/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from .types.list_templates_response import ListTemplatesResponse
 
 
 class TemplatesClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(
+    def list_(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> ListTemplatesResponse:
         """
         Returns a list of notification templates
 
         Parameters
         ----------
@@ -38,31 +39,33 @@
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.templates.list(
+        client.templates.list_(
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "notifications"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -72,27 +75,27 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListTemplatesResponse, _response.json())  # type: ignore
+            return typing.cast(ListTemplatesResponse, construct_type(type_=ListTemplatesResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncTemplatesClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(
+    async def list_(
         self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
     ) -> ListTemplatesResponse:
         """
         Returns a list of notification templates
 
         Parameters
         ----------
@@ -109,31 +112,33 @@
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.templates.list(
+        await client.templates.list_(
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "notifications"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -143,13 +148,13 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListTemplatesResponse, _response.json())  # type: ignore
+            return typing.cast(ListTemplatesResponse, construct_type(type_=ListTemplatesResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/templates/types/__init__.py` & `trycourier-6.1.0/src/courier/templates/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/templates/types/list_templates_response.py` & `trycourier-6.1.0/src/courier/send/types/base_message_send_to.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.paging import Paging
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .notification_templates import NotificationTemplates
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .message_recipient import MessageRecipient
 
 
-class ListTemplatesResponse(pydantic_v1.BaseModel):
-    paging: Paging
-    results: typing.List[NotificationTemplates] = pydantic_v1.Field()
+class BaseMessageSendTo(UncheckedBaseModel):
+    to: typing.Optional[MessageRecipient] = pydantic_v1.Field(default=None)
     """
-    An array of Notification Templates
+    The recipient or a list of recipients of the message
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/templates/types/notification_templates.py` & `trycourier-6.1.0/src/courier/tenants/types/subscription_topic_new.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,41 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.channel_classification import ChannelClassification
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .routing_strategy import RoutingStrategy
-from .tag import Tag
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .subscription_topic_status import SubscriptionTopicStatus
 
 
-class NotificationTemplates(pydantic_v1.BaseModel):
-    created_at: int = pydantic_v1.Field()
+class SubscriptionTopicNew(UncheckedBaseModel):
+    status: SubscriptionTopicStatus
+    has_custom_routing: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
-    A UTC timestamp at which notification was created. This is stored as a millisecond representation of the Unix epoch (the time passed since January 1, 1970).
+    Override channel routing with custom preferences. This will override any template prefernces that are set, but a user can still customize their preferences
     """
 
-    id: str = pydantic_v1.Field()
+    custom_routing: typing.Optional[typing.List[ChannelClassification]] = pydantic_v1.Field(default=None)
     """
-    A unique identifier associated with the notification.
-    """
-
-    routing: RoutingStrategy = pydantic_v1.Field()
-    """
-    Routing strategy used by this notification.
-    """
-
-    tags: typing.List[Tag] = pydantic_v1.Field()
-    """
-    A list of tags attached to the notification.
-    """
-
-    title: str = pydantic_v1.Field()
-    """
-    The title of the notification.
-    """
-
-    updated_at: int = pydantic_v1.Field()
-    """
-    A UTC timestamp at which notification was updated. This is stored as a millisecond representation of the Unix epoch (the time passed since January 1, 1970).
+    The default channels to send to this tenant when has_custom_routing is enabled
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/templates/types/routing_strategy.py` & `trycourier-6.1.0/src/courier/templates/types/routing_strategy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .channel_identifier import ChannelIdentifier
 from .routing_strategy_method import RoutingStrategyMethod
 
 
-class RoutingStrategy(pydantic_v1.BaseModel):
+class RoutingStrategy(UncheckedBaseModel):
     method: RoutingStrategyMethod = pydantic_v1.Field()
     """
     The method for selecting channels to send the message with. Value can be either 'single' or 'all'. If not provided will default to 'single'
     """
 
     channels: typing.List[ChannelIdentifier] = pydantic_v1.Field()
     """
@@ -21,15 +22,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/tenants/client.py` & `trycourier-6.1.0/src/courier/tenants/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 from json.decoder import JSONDecodeError
 
 from ..commons.errors.bad_request_error import BadRequestError
 from ..commons.types.bad_request import BadRequest
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 from .types.default_preferences import DefaultPreferences
 from .types.list_users_for_tenant_response import ListUsersForTenantResponse
+from .types.subscription_topic_new import SubscriptionTopicNew
 from .types.tenant import Tenant
 from .types.tenant_list_response import TenantListResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
@@ -100,16 +102,18 @@
         if brand_id is not OMIT:
             _request["brand_id"] = brand_id
         _response = self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -124,17 +128,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Tenant, _response.json())  # type: ignore
+            return typing.cast(Tenant, construct_type(type_=Tenant, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Tenant:
@@ -163,16 +169,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -181,35 +189,41 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Tenant, _response.json())  # type: ignore
+            return typing.cast(Tenant, construct_type(type_=Tenant, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def list(
+    def list_(
         self,
         *,
+        parent_tenant_id: typing.Optional[str] = None,
         limit: typing.Optional[int] = None,
         cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> TenantListResponse:
         """
         Parameters
         ----------
+        parent_tenant_id : typing.Optional[str]
+            Filter the list of tenants by parent_id
+
         limit : typing.Optional[int]
-            The number of accousnts to return
+            The number of tenants to return
             (defaults to 20, maximum value of 100)
 
         cursor : typing.Optional[str]
             Continue the pagination with the next cursor
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
@@ -221,33 +235,37 @@
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.tenants.list(
+        client.tenants.list_(
+            parent_tenant_id="string",
             limit=1,
             cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "tenants"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "limit": limit,
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "parent_tenant_id": parent_tenant_id,
+                            "limit": limit,
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -257,15 +275,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(TenantListResponse, _response.json())  # type: ignore
+            return typing.cast(TenantListResponse, construct_type(type_=TenantListResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
@@ -294,17 +312,22 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -365,27 +388,116 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}/users"
             ),
-            params=jsonable_encoder(
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "limit": limit,
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
+                )
+            ),
+            headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
-                        "limit": limit,
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return typing.cast(ListUsersForTenantResponse, construct_type(type_=ListUsersForTenantResponse, object_=_response.json()))  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    def create_or_replace_default_preferences_for_topic(
+        self,
+        tenant_id: str,
+        topic_id: str,
+        *,
+        request: SubscriptionTopicNew,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> None:
+        """
+        Parameters
+        ----------
+        tenant_id : str
+            Id of the tenant to update the default preferences for.
+
+        topic_id : str
+            Id fo the susbcription topic you want to have a default preference for.
+
+        request : SubscriptionTopicNew
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
+        from courier import SubscriptionTopicNew
+        from courier.client import Courier
+
+        client = Courier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        client.tenants.create_or_replace_default_preferences_for_topic(
+            tenant_id="tenantABC",
+            topic_id="HB529N49MD4D5PMX9WR5P4JH78NA",
+            request=SubscriptionTopicNew(
+                status="OPTED_IN",
+                has_custom_routing=True,
+                custom_routing=["inbox"],
+            ),
+        )
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"tenants/{jsonable_encoder(tenant_id)}/default_preferences/items/{jsonable_encoder(topic_id)}",
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
+            ),
+            json=jsonable_encoder(request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -393,17 +505,82 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListUsersForTenantResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    def remove_default_preferences_for_topic(
+        self, tenant_id: str, topic_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> None:
+        """
+        Parameters
+        ----------
+        tenant_id : str
+            Id of the tenant to update the default preferences for.
+
+        topic_id : str
+            Id fo the susbcription topic you want to have a default preference for.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
+        from courier.client import Courier
+
+        client = Courier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        client.tenants.remove_default_preferences_for_topic(
+            tenant_id="string",
+            topic_id="string",
+        )
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"tenants/{jsonable_encoder(tenant_id)}/default_preferences/items/{jsonable_encoder(topic_id)}",
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
+            ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -486,16 +663,18 @@
         if brand_id is not OMIT:
             _request["brand_id"] = brand_id
         _response = await self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -510,17 +689,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Tenant, _response.json())  # type: ignore
+            return typing.cast(Tenant, construct_type(type_=Tenant, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Tenant:
@@ -549,16 +730,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -567,35 +750,41 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(Tenant, _response.json())  # type: ignore
+            return typing.cast(Tenant, construct_type(type_=Tenant, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def list(
+    async def list_(
         self,
         *,
+        parent_tenant_id: typing.Optional[str] = None,
         limit: typing.Optional[int] = None,
         cursor: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> TenantListResponse:
         """
         Parameters
         ----------
+        parent_tenant_id : typing.Optional[str]
+            Filter the list of tenants by parent_id
+
         limit : typing.Optional[int]
-            The number of accousnts to return
+            The number of tenants to return
             (defaults to 20, maximum value of 100)
 
         cursor : typing.Optional[str]
             Continue the pagination with the next cursor
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
@@ -607,33 +796,37 @@
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.tenants.list(
+        await client.tenants.list_(
+            parent_tenant_id="string",
             limit=1,
             cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "tenants"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "limit": limit,
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "parent_tenant_id": parent_tenant_id,
+                            "limit": limit,
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -643,15 +836,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(TenantListResponse, _response.json())  # type: ignore
+            return typing.cast(TenantListResponse, construct_type(type_=TenantListResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
@@ -680,17 +873,22 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -751,27 +949,116 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"tenants/{jsonable_encoder(tenant_id)}/users"
             ),
-            params=jsonable_encoder(
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "limit": limit,
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
+                )
+            ),
+            headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
-                        "limit": limit,
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return typing.cast(ListUsersForTenantResponse, construct_type(type_=ListUsersForTenantResponse, object_=_response.json()))  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def create_or_replace_default_preferences_for_topic(
+        self,
+        tenant_id: str,
+        topic_id: str,
+        *,
+        request: SubscriptionTopicNew,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> None:
+        """
+        Parameters
+        ----------
+        tenant_id : str
+            Id of the tenant to update the default preferences for.
+
+        topic_id : str
+            Id fo the susbcription topic you want to have a default preference for.
+
+        request : SubscriptionTopicNew
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
+        from courier import SubscriptionTopicNew
+        from courier.client import AsyncCourier
+
+        client = AsyncCourier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        await client.tenants.create_or_replace_default_preferences_for_topic(
+            tenant_id="tenantABC",
+            topic_id="HB529N49MD4D5PMX9WR5P4JH78NA",
+            request=SubscriptionTopicNew(
+                status="OPTED_IN",
+                has_custom_routing=True,
+                custom_routing=["inbox"],
+            ),
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            method="PUT",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"tenants/{jsonable_encoder(tenant_id)}/default_preferences/items/{jsonable_encoder(topic_id)}",
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
+            ),
+            json=jsonable_encoder(request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -779,15 +1066,80 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListUsersForTenantResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def remove_default_preferences_for_topic(
+        self, tenant_id: str, topic_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> None:
+        """
+        Parameters
+        ----------
+        tenant_id : str
+            Id of the tenant to update the default preferences for.
+
+        topic_id : str
+            Id fo the susbcription topic you want to have a default preference for.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
+        from courier.client import AsyncCourier
+
+        client = AsyncCourier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        await client.tenants.remove_default_preferences_for_topic(
+            tenant_id="string",
+            topic_id="string",
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"tenants/{jsonable_encoder(tenant_id)}/default_preferences/items/{jsonable_encoder(topic_id)}",
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
+            ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/tenants/types/__init__.py` & `trycourier-6.1.0/src/courier/tenants/types/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .default_preferences import DefaultPreferences
 from .list_users_for_tenant_response import ListUsersForTenantResponse
 from .subscription_topic import SubscriptionTopic
+from .subscription_topic_new import SubscriptionTopicNew
 from .subscription_topic_status import SubscriptionTopicStatus
 from .template_property import TemplateProperty
 from .tenant import Tenant
 from .tenant_list_response import TenantListResponse
 
 __all__ = [
     "DefaultPreferences",
     "ListUsersForTenantResponse",
     "SubscriptionTopic",
+    "SubscriptionTopicNew",
     "SubscriptionTopicStatus",
     "TemplateProperty",
     "Tenant",
     "TenantListResponse",
 ]
```

### Comparing `trycourier-6.0.5/src/courier/tenants/types/list_users_for_tenant_response.py` & `trycourier-6.1.0/src/courier/users/tenants/types/list_tenants_for_user_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.user_tenant_association import UserTenantAssociation
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ....commons.types.user_tenant_association import UserTenantAssociation
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 
 
-class ListUsersForTenantResponse(pydantic_v1.BaseModel):
+class ListTenantsForUserResponse(UncheckedBaseModel):
     items: typing.Optional[typing.List[UserTenantAssociation]] = None
     has_more: bool = pydantic_v1.Field()
     """
     Set to true when there are more pages that can be retrieved.
     """
 
     url: str = pydantic_v1.Field()
@@ -38,15 +39,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/tenants/types/subscription_topic.py` & `trycourier-6.1.0/src/courier/users/tokens/types/get_user_token_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .subscription_topic_status import SubscriptionTopicStatus
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .token_status import TokenStatus
+from .user_token import UserToken
 
 
-class SubscriptionTopic(pydantic_v1.BaseModel):
-    id: str = pydantic_v1.Field()
+class GetUserTokenResponse(UserToken):
+    status: typing.Optional[TokenStatus] = None
+    status_reason: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Topic ID
+    The reason for the token status.
     """
 
-    status: SubscriptionTopicStatus
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/tenants/types/tenant.py` & `trycourier-6.1.0/src/courier/users/tokens/types/device.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from .default_preferences import DefaultPreferences
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 
 
-class Tenant(pydantic_v1.BaseModel):
-    id: str = pydantic_v1.Field()
+class Device(UncheckedBaseModel):
+    app_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Id of the tenant.
+    Id of the application the token is used for
     """
 
-    name: str = pydantic_v1.Field()
+    ad_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Name of the tenant.
+    Id of the advertising identifier
     """
 
-    parent_tenant_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    device_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Tenant's parent id (if any).
+    Id of the device the token is associated with
     """
 
-    default_preferences: typing.Optional[DefaultPreferences] = pydantic_v1.Field(default=None)
+    platform: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Defines the preferences used for the account when the user hasn't specified their own.
+    The device platform i.e. android, ios, web
     """
 
-    properties: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    manufacturer: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Arbitrary properties accessible to a template.
+    The device manufacturer
     """
 
-    user_profile: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    model: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    A user profile object merged with user profile on send.
-    """
-
-    brand_id: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    Brand to be used for the account when one is not specified by the send call.
+    The device model
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/tenants/types/tenant_list_response.py` & `trycourier-6.1.0/src/courier/tenants/types/tenant_list_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 from .tenant import Tenant
 
 
-class TenantListResponse(pydantic_v1.BaseModel):
+class TenantListResponse(UncheckedBaseModel):
     cursor: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     A pointer to the next page of results. Defined only when has_more is set to true.
     """
 
     has_more: bool = pydantic_v1.Field()
     """
@@ -41,15 +42,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/translations/client.py` & `trycourier-6.1.0/src/courier/translations/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from json.decoder import JSONDecodeError
 
 from ..commons.errors.not_found_error import NotFoundError
 from ..commons.types.not_found import NotFound
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class TranslationsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
@@ -55,16 +56,18 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"translations/{jsonable_encoder(domain)}/{jsonable_encoder(locale)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -73,17 +76,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(str, _response.json())  # type: ignore
+            return typing.cast(str, construct_type(type_=str, object_=_response.json()))  # type: ignore
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFound, construct_type(type_=NotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
@@ -124,16 +129,18 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"translations/{jsonable_encoder(domain)}/{jsonable_encoder(locale)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -145,15 +152,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFound, construct_type(type_=NotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -195,16 +204,18 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"translations/{jsonable_encoder(domain)}/{jsonable_encoder(locale)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -213,17 +224,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(str, _response.json())  # type: ignore
+            return typing.cast(str, construct_type(type_=str, object_=_response.json()))  # type: ignore
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFound, construct_type(type_=NotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
@@ -264,16 +277,18 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"translations/{jsonable_encoder(domain)}/{jsonable_encoder(locale)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -285,13 +300,15 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFound, construct_type(type_=NotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/types/send_message_response.py` & `trycourier-6.1.0/src/courier/types/send_message_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class SendMessageResponse(pydantic_v1.BaseModel):
+class SendMessageResponse(UncheckedBaseModel):
     request_id: str = pydantic_v1.Field(alias="requestId")
     """
     A successful call to `POST /send` returns a `202` status code along with a `requestId` in the response body.
     
     For send requests that have a single recipient, the `requestId` is assigned to the derived message as its message_id. Therefore the `requestId` can be supplied to the Message's API for single recipient messages.
     
     For send requests that have multiple recipients (accounts, audiences, lists, etc.), Courier assigns a unique id to each derived message as its `message_id`. Therefore the `requestId` cannot be supplied to the Message's API for single-recipient messages.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/users/__init__.py` & `trycourier-6.1.0/src/courier/users/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/users/client.py` & `trycourier-6.1.0/src/courier/users/client.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/users/preferences/client.py` & `trycourier-6.1.0/src/courier/users/preferences/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,31 +7,32 @@
 from ...commons.errors.bad_request_error import BadRequestError
 from ...commons.errors.not_found_error import NotFoundError
 from ...commons.types.bad_request import BadRequest
 from ...commons.types.not_found import NotFound
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.query_encoder import encode_query
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
+from ...core.unchecked_base_model import construct_type
 from .types.topic_preference_update import TopicPreferenceUpdate
 from .types.user_preferences_get_response import UserPreferencesGetResponse
 from .types.user_preferences_list_response import UserPreferencesListResponse
 from .types.user_preferences_update_response import UserPreferencesUpdateResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class PreferencesClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(
+    def list_(
         self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> UserPreferencesListResponse:
         """
         Fetch all user preferences.
 
         Parameters
         ----------
@@ -48,25 +49,27 @@
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.users.preferences.list(
+        client.users.preferences.list_(
             user_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/preferences"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -75,17 +78,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(UserPreferencesListResponse, _response.json())  # type: ignore
+            return typing.cast(UserPreferencesListResponse, construct_type(type_=UserPreferencesListResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(
@@ -123,16 +128,18 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/preferences/{jsonable_encoder(topic_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -141,17 +148,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(UserPreferencesGetResponse, _response.json())  # type: ignore
+            return typing.cast(UserPreferencesGetResponse, construct_type(type_=UserPreferencesGetResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFound, construct_type(type_=NotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
@@ -202,16 +211,18 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/preferences/{jsonable_encoder(topic_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"topic": topic})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"topic": topic}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -226,29 +237,31 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(UserPreferencesUpdateResponse, _response.json())  # type: ignore
+            return typing.cast(UserPreferencesUpdateResponse, construct_type(type_=UserPreferencesUpdateResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncPreferencesClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(
+    async def list_(
         self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> UserPreferencesListResponse:
         """
         Fetch all user preferences.
 
         Parameters
         ----------
@@ -265,25 +278,27 @@
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.users.preferences.list(
+        await client.users.preferences.list_(
             user_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/preferences"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -292,17 +307,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(UserPreferencesListResponse, _response.json())  # type: ignore
+            return typing.cast(UserPreferencesListResponse, construct_type(type_=UserPreferencesListResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
@@ -340,16 +357,18 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/preferences/{jsonable_encoder(topic_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -358,17 +377,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(UserPreferencesGetResponse, _response.json())  # type: ignore
+            return typing.cast(UserPreferencesGetResponse, construct_type(type_=UserPreferencesGetResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 404:
-            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFound, construct_type(type_=NotFound, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
@@ -419,16 +440,18 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/preferences/{jsonable_encoder(topic_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"topic": topic})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"topic": topic}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -443,15 +466,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(UserPreferencesUpdateResponse, _response.json())  # type: ignore
+            return typing.cast(UserPreferencesUpdateResponse, construct_type(type_=UserPreferencesUpdateResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/users/preferences/types/__init__.py` & `trycourier-6.1.0/src/courier/users/preferences/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/users/preferences/types/topic_preference.py` & `trycourier-6.1.0/src/courier/users/preferences/types/topic_preference_update.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 
 import datetime as dt
 import typing
 
 from ....commons.types.channel_classification import ChannelClassification
 from ....commons.types.preference_status import PreferenceStatus
 from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 
 
-class TopicPreference(pydantic_v1.BaseModel):
+class TopicPreferenceUpdate(UncheckedBaseModel):
+    status: PreferenceStatus
     custom_routing: typing.Optional[typing.List[ChannelClassification]] = pydantic_v1.Field(default=None)
     """
     The Channels a user has chosen to receive notifications through for this topic
     """
 
-    default_status: PreferenceStatus
     has_custom_routing: typing.Optional[bool] = None
-    status: PreferenceStatus
-    topic_id: str
-    topic_name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/users/preferences/types/topic_preference_update.py` & `trycourier-6.1.0/src/courier/users/preferences/types/topic_preference.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,40 @@
 
 import datetime as dt
 import typing
 
 from ....commons.types.channel_classification import ChannelClassification
 from ....commons.types.preference_status import PreferenceStatus
 from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 
 
-class TopicPreferenceUpdate(pydantic_v1.BaseModel):
-    status: PreferenceStatus
+class TopicPreference(UncheckedBaseModel):
     custom_routing: typing.Optional[typing.List[ChannelClassification]] = pydantic_v1.Field(default=None)
     """
     The Channels a user has chosen to receive notifications through for this topic
     """
 
+    default_status: PreferenceStatus
     has_custom_routing: typing.Optional[bool] = None
+    status: PreferenceStatus
+    topic_id: str
+    topic_name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/users/preferences/types/user_preferences_get_response.py` & `trycourier-6.1.0/src/courier/notifications/types/check.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
-from .topic_preference import TopicPreference
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .base_check import BaseCheck
 
 
-class UserPreferencesGetResponse(pydantic_v1.BaseModel):
-    topic: TopicPreference
+class Check(BaseCheck):
+    updated: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/users/preferences/types/user_preferences_list_response.py` & `trycourier-6.1.0/src/courier/commons/types/base_error.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....commons.types.paging import Paging
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
-from .topic_preference import TopicPreference
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class UserPreferencesListResponse(pydantic_v1.BaseModel):
-    paging: Paging
-    items: typing.List[TopicPreference] = pydantic_v1.Field()
+class BaseError(UncheckedBaseModel):
+    message: str = pydantic_v1.Field()
     """
-    The Preferences associated with the user_id.
+    A message describing the error that occurred.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/users/tenants/client.py` & `trycourier-6.1.0/src/courier/brands/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,177 +1,169 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ...commons.types.user_tenant_association import UserTenantAssociation
-from ...core.api_error import ApiError
-from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from ...core.jsonable_encoder import jsonable_encoder
-from ...core.pydantic_utilities import pydantic_v1
-from ...core.remove_none_from_dict import remove_none_from_dict
-from ...core.request_options import RequestOptions
-from .types.list_tenants_for_user_response import ListTenantsForUserResponse
+from ..commons.errors.already_exists_error import AlreadyExistsError
+from ..commons.errors.bad_request_error import BadRequestError
+from ..commons.errors.conflict_error import ConflictError
+from ..commons.errors.payment_required_error import PaymentRequiredError
+from ..commons.types.already_exists import AlreadyExists
+from ..commons.types.bad_request import BadRequest
+from ..commons.types.conflict import Conflict
+from ..commons.types.payment_required import PaymentRequired
+from ..core.api_error import ApiError
+from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
+from ..core.remove_none_from_dict import remove_none_from_dict
+from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
+from .types.brand import Brand
+from .types.brand_parameters import BrandParameters
+from .types.brand_settings import BrandSettings
+from .types.brand_snippets import BrandSnippets
+from .types.brands_response import BrandsResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class TenantsClient:
+class BrandsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def add_multple(
+    def create(
         self,
-        user_id: str,
         *,
-        tenants: typing.Sequence[UserTenantAssociation],
+        request: BrandParameters,
+        idempotency_key: typing.Optional[str] = None,
+        idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> None:
+    ) -> Brand:
         """
-        This endpoint is used to add a user to
-        multiple tenants in one call.
-        A custom profile can also be supplied for each tenant.
-        This profile will be merged with the user's main
-        profile when sending to the user with that tenant.
-
         Parameters
         ----------
-        user_id : str
-            The user's ID. This can be any uniquely identifiable string.
+        request : BrandParameters
+
+        idempotency_key : typing.Optional[str]
 
-        tenants : typing.Sequence[UserTenantAssociation]
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        None
+        Brand
 
         Examples
         --------
-        from courier import UserTenantAssociation
+        from courier import BrandParameters, BrandSettings, BrandSnippets
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.users.tenants.add_multple(
-            user_id="string",
-            tenants=[
-                UserTenantAssociation(
-                    user_id="string",
-                    type="user",
-                    tenant_id="string",
-                    profile={"string": {"key": "value"}},
-                )
-            ],
+        client.brands.create(
+            request=BrandParameters(
+                id="string",
+                name="string",
+                settings=BrandSettings(),
+                snippets=BrandSnippets(),
+            ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="PUT",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder({"tenants": tenants})
+            json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"tenants": tenants}),
+                **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
+                        "Idempotency-Key": str(idempotency_key) if idempotency_key is not None else None,
+                        "X-Idempotency-Expiration": str(idempotency_expiry) if idempotency_expiry is not None else None,
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return typing.cast(Brand, construct_type(type_=Brand, object_=_response.json()))  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
+        if _response.status_code == 402:
+            raise PaymentRequiredError(
+                typing.cast(PaymentRequired, construct_type(type_=PaymentRequired, object_=_response.json()))  # type: ignore
+            )
+        if _response.status_code == 409:
+            raise AlreadyExistsError(
+                typing.cast(AlreadyExists, construct_type(type_=AlreadyExists, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def add(
-        self,
-        user_id: str,
-        tenant_id: str,
-        *,
-        profile: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> None:
+    def get(self, brand_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Brand:
         """
-        This endpoint is used to add a single tenant.
-
-        A custom profile can also be supplied with the tenant.
-        This profile will be merged with the user's main profile
-        when sending to the user with that tenant.
+        Fetch a specific brand by brand ID.
 
         Parameters
         ----------
-        user_id : str
-            Id of the user to be added to the supplied tenant.
-
-        tenant_id : str
-            Id of the tenant the user should be added to.
-
-        profile : typing.Optional[typing.Dict[str, typing.Any]]
+        brand_id : str
+            A unique identifier associated with the brand you wish to retrieve.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        None
+        Brand
 
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.users.tenants.add(
-            user_id="string",
-            tenant_id="string",
-            profile={"string": {"key": "value"}},
+        client.brands.get(
+            brand_id="string",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if profile is not OMIT:
-            _request["profile"] = profile
         _response = self._client_wrapper.httpx_client.request(
-            method="PUT",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"users/{jsonable_encoder(user_id)}/tenants/{jsonable_encoder(tenant_id)}",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -179,55 +171,66 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return typing.cast(Brand, construct_type(type_=Brand, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def remove_all(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+    def list_(
+        self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
+    ) -> BrandsResponse:
         """
-        Removes a user from any tenants they may have been associated with.
+        Get the list of brands.
 
         Parameters
         ----------
-        user_id : str
-            Id of the user to be removed from the supplied tenant.
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of brands.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        None
+        BrandsResponse
 
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.users.tenants.remove_all(
-            user_id="string",
+        client.brands.list_(
+            cursor="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="DELETE",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -236,32 +239,29 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return typing.cast(BrandsResponse, construct_type(type_=BrandsResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def remove(self, user_id: str, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+    def delete(self, brand_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Removes a user from the supplied tenant.
+        Delete a brand by brand ID.
 
         Parameters
         ----------
-        user_id : str
-            Id of the user to be removed from the supplied tenant.
-
-        tenant_id : str
-            Id of the tenant the user should be removed from.
+        brand_id : str
+            A unique identifier associated with the brand you wish to retrieve.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
         None
@@ -269,28 +269,29 @@
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.users.tenants.remove(
-            user_id="string",
-            tenant_id="string",
+        client.brands.delete(
+            brand_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="DELETE",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"users/{jsonable_encoder(user_id)}/tenants/{jsonable_encoder(tenant_id)}",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -299,81 +300,107 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
+        if _response.status_code == 409:
+            raise ConflictError(
+                typing.cast(Conflict, construct_type(type_=Conflict, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def list(
+    def replace(
         self,
-        user_id: str,
+        brand_id: str,
         *,
-        limit: typing.Optional[int] = None,
-        cursor: typing.Optional[str] = None,
+        name: str,
+        settings: typing.Optional[BrandSettings] = OMIT,
+        snippets: typing.Optional[BrandSnippets] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> ListTenantsForUserResponse:
+    ) -> Brand:
         """
-        Returns a paginated list of user tenant associations.
+        Replace an existing brand with the supplied values.
 
         Parameters
         ----------
-        user_id : str
-            Id of the user to retrieve all associated tenants for.
+        brand_id : str
+            A unique identifier associated with the brand you wish to update.
 
-        limit : typing.Optional[int]
-            The number of accounts to return
-            (defaults to 20, maximum value of 100)
+        name : str
+            The name of the brand.
 
-        cursor : typing.Optional[str]
-            Continue the pagination with the next cursor
+        settings : typing.Optional[BrandSettings]
+
+        snippets : typing.Optional[BrandSnippets]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        ListTenantsForUserResponse
+        Brand
 
         Examples
         --------
+        from courier import (
+            BrandColors,
+            BrandSettings,
+            BrandSnippet,
+            BrandSnippets,
+            Email,
+        )
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.users.tenants.list(
-            user_id="string",
-            limit=1,
-            cursor="string",
+        client.brands.replace(
+            brand_id="string",
+            name="string",
+            settings=BrandSettings(
+                colors=BrandColors(),
+                inapp={"key": "value"},
+                email=Email(),
+            ),
+            snippets=BrandSnippets(
+                items=[
+                    BrandSnippet(
+                        format="handlebars",
+                        name="string",
+                        value="string",
+                    )
+                ],
+            ),
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"name": name}
+        if settings is not OMIT:
+            _request["settings"] = settings
+        if snippets is not OMIT:
+            _request["snippets"] = snippets
         _response = self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
-            ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "limit": limit,
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="PUT",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
                 )
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -381,173 +408,153 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListTenantsForUserResponse, _response.json())  # type: ignore
+            return typing.cast(Brand, construct_type(type_=Brand, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncTenantsClient:
+class AsyncBrandsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def add_multple(
+    async def create(
         self,
-        user_id: str,
         *,
-        tenants: typing.Sequence[UserTenantAssociation],
+        request: BrandParameters,
+        idempotency_key: typing.Optional[str] = None,
+        idempotency_expiry: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> None:
+    ) -> Brand:
         """
-        This endpoint is used to add a user to
-        multiple tenants in one call.
-        A custom profile can also be supplied for each tenant.
-        This profile will be merged with the user's main
-        profile when sending to the user with that tenant.
-
         Parameters
         ----------
-        user_id : str
-            The user's ID. This can be any uniquely identifiable string.
+        request : BrandParameters
+
+        idempotency_key : typing.Optional[str]
 
-        tenants : typing.Sequence[UserTenantAssociation]
+        idempotency_expiry : typing.Optional[str]
+            The expiry can either be an ISO8601 datetime or a duration like "1 Day".
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        None
+        Brand
 
         Examples
         --------
-        from courier import UserTenantAssociation
+        from courier import BrandParameters, BrandSettings, BrandSnippets
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.users.tenants.add_multple(
-            user_id="string",
-            tenants=[
-                UserTenantAssociation(
-                    user_id="string",
-                    type="user",
-                    tenant_id="string",
-                    profile={"string": {"key": "value"}},
-                )
-            ],
+        await client.brands.create(
+            request=BrandParameters(
+                id="string",
+                name="string",
+                settings=BrandSettings(),
+                snippets=BrandSnippets(),
+            ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="PUT",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder({"tenants": tenants})
+            json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"tenants": tenants}),
+                **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
+                        "Idempotency-Key": str(idempotency_key) if idempotency_key is not None else None,
+                        "X-Idempotency-Expiration": str(idempotency_expiry) if idempotency_expiry is not None else None,
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return typing.cast(Brand, construct_type(type_=Brand, object_=_response.json()))  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
+        if _response.status_code == 402:
+            raise PaymentRequiredError(
+                typing.cast(PaymentRequired, construct_type(type_=PaymentRequired, object_=_response.json()))  # type: ignore
+            )
+        if _response.status_code == 409:
+            raise AlreadyExistsError(
+                typing.cast(AlreadyExists, construct_type(type_=AlreadyExists, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def add(
-        self,
-        user_id: str,
-        tenant_id: str,
-        *,
-        profile: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> None:
+    async def get(self, brand_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Brand:
         """
-        This endpoint is used to add a single tenant.
-
-        A custom profile can also be supplied with the tenant.
-        This profile will be merged with the user's main profile
-        when sending to the user with that tenant.
+        Fetch a specific brand by brand ID.
 
         Parameters
         ----------
-        user_id : str
-            Id of the user to be added to the supplied tenant.
-
-        tenant_id : str
-            Id of the tenant the user should be added to.
-
-        profile : typing.Optional[typing.Dict[str, typing.Any]]
+        brand_id : str
+            A unique identifier associated with the brand you wish to retrieve.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        None
+        Brand
 
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.users.tenants.add(
-            user_id="string",
-            tenant_id="string",
-            profile={"string": {"key": "value"}},
+        await client.brands.get(
+            brand_id="string",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if profile is not OMIT:
-            _request["profile"] = profile
         _response = await self._client_wrapper.httpx_client.request(
-            method="PUT",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"users/{jsonable_encoder(user_id)}/tenants/{jsonable_encoder(tenant_id)}",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -555,55 +562,66 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return typing.cast(Brand, construct_type(type_=Brand, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def remove_all(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
+    async def list_(
+        self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
+    ) -> BrandsResponse:
         """
-        Removes a user from any tenants they may have been associated with.
+        Get the list of brands.
 
         Parameters
         ----------
-        user_id : str
-            Id of the user to be removed from the supplied tenant.
+        cursor : typing.Optional[str]
+            A unique identifier that allows for fetching the next set of brands.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        None
+        BrandsResponse
 
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.users.tenants.remove_all(
-            user_id="string",
+        await client.brands.list_(
+            cursor="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="DELETE",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "brands"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "cursor": cursor,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -612,34 +630,29 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return typing.cast(BrandsResponse, construct_type(type_=BrandsResponse, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def remove(
-        self, user_id: str, tenant_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> None:
+    async def delete(self, brand_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Removes a user from the supplied tenant.
+        Delete a brand by brand ID.
 
         Parameters
         ----------
-        user_id : str
-            Id of the user to be removed from the supplied tenant.
-
-        tenant_id : str
-            Id of the tenant the user should be removed from.
+        brand_id : str
+            A unique identifier associated with the brand you wish to retrieve.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
         None
@@ -647,28 +660,29 @@
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.users.tenants.remove(
-            user_id="string",
-            tenant_id="string",
+        await client.brands.delete(
+            brand_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="DELETE",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/",
-                f"users/{jsonable_encoder(user_id)}/tenants/{jsonable_encoder(tenant_id)}",
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -677,81 +691,107 @@
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
+        if _response.status_code == 409:
+            raise ConflictError(
+                typing.cast(Conflict, construct_type(type_=Conflict, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def list(
+    async def replace(
         self,
-        user_id: str,
+        brand_id: str,
         *,
-        limit: typing.Optional[int] = None,
-        cursor: typing.Optional[str] = None,
+        name: str,
+        settings: typing.Optional[BrandSettings] = OMIT,
+        snippets: typing.Optional[BrandSnippets] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> ListTenantsForUserResponse:
+    ) -> Brand:
         """
-        Returns a paginated list of user tenant associations.
+        Replace an existing brand with the supplied values.
 
         Parameters
         ----------
-        user_id : str
-            Id of the user to retrieve all associated tenants for.
+        brand_id : str
+            A unique identifier associated with the brand you wish to update.
 
-        limit : typing.Optional[int]
-            The number of accounts to return
-            (defaults to 20, maximum value of 100)
+        name : str
+            The name of the brand.
 
-        cursor : typing.Optional[str]
-            Continue the pagination with the next cursor
+        settings : typing.Optional[BrandSettings]
+
+        snippets : typing.Optional[BrandSnippets]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        ListTenantsForUserResponse
+        Brand
 
         Examples
         --------
+        from courier import (
+            BrandColors,
+            BrandSettings,
+            BrandSnippet,
+            BrandSnippets,
+            Email,
+        )
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.users.tenants.list(
-            user_id="string",
-            limit=1,
-            cursor="string",
+        await client.brands.replace(
+            brand_id="string",
+            name="string",
+            settings=BrandSettings(
+                colors=BrandColors(),
+                inapp={"key": "value"},
+                email=Email(),
+            ),
+            snippets=BrandSnippets(
+                items=[
+                    BrandSnippet(
+                        format="handlebars",
+                        name="string",
+                        value="string",
+                    )
+                ],
+            ),
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"name": name}
+        if settings is not OMIT:
+            _request["settings"] = settings
+        if snippets is not OMIT:
+            _request["snippets"] = snippets
         _response = await self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tenants"
-            ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "limit": limit,
-                        "cursor": cursor,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="PUT",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"brands/{jsonable_encoder(brand_id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
                 )
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -759,13 +799,13 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(ListTenantsForUserResponse, _response.json())  # type: ignore
+            return typing.cast(Brand, construct_type(type_=Brand, object_=_response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py` & `trycourier-6.1.0/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 
 
-class AddUserToSingleTenantsParamsProfile(pydantic_v1.BaseModel):
+class AddUserToSingleTenantsParamsProfile(UncheckedBaseModel):
     """
     AddUserToSingleTenantsParamsProfile is no longer used for Add a User to a Single Tenant
     """
 
     title: str
     email: str = pydantic_v1.Field()
     """
@@ -34,15 +35,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/users/tenants/types/list_tenants_for_user_response.py` & `trycourier-6.1.0/src/courier/tenants/types/list_users_for_tenant_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....commons.types.user_tenant_association import UserTenantAssociation
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ...commons.types.user_tenant_association import UserTenantAssociation
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class ListTenantsForUserResponse(pydantic_v1.BaseModel):
+class ListUsersForTenantResponse(UncheckedBaseModel):
     items: typing.Optional[typing.List[UserTenantAssociation]] = None
     has_more: bool = pydantic_v1.Field()
     """
     Set to true when there are more pages that can be retrieved.
     """
 
     url: str = pydantic_v1.Field()
@@ -38,15 +39,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/users/tokens/__init__.py` & `trycourier-6.1.0/src/courier/users/tokens/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/users/tokens/client.py` & `trycourier-6.1.0/src/courier/users/tokens/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from json.decoder import JSONDecodeError
 
 from ...commons.errors.bad_request_error import BadRequestError
 from ...commons.types.bad_request import BadRequest
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.query_encoder import encode_query
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
+from ...core.unchecked_base_model import construct_type
 from .types.get_all_tokens_response import GetAllTokensResponse
 from .types.get_user_token_response import GetUserTokenResponse
 from .types.patch_user_token_opts import PatchUserTokenOpts
 from .types.user_token import UserToken
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
@@ -53,16 +54,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tokens"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -76,15 +79,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def add(
@@ -145,16 +150,18 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/tokens/{jsonable_encoder(token)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -171,15 +178,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
@@ -228,16 +237,18 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="PATCH",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/tokens/{jsonable_encoder(token)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -254,15 +265,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(
@@ -300,16 +313,18 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/tokens/{jsonable_encoder(token)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -318,24 +333,26 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(GetUserTokenResponse, _response.json())  # type: ignore
+            return typing.cast(GetUserTokenResponse, construct_type(type_=GetUserTokenResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def list(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> GetAllTokensResponse:
+    def list_(self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> GetAllTokensResponse:
         """
         Gets all tokens available for a :user_id
 
         Parameters
         ----------
         user_id : str
             The user's ID. This can be any uniquely identifiable string.
@@ -350,25 +367,27 @@
         Examples
         --------
         from courier.client import Courier
 
         client = Courier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        client.users.tokens.list(
+        client.users.tokens.list_(
             user_id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tokens"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -377,17 +396,19 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(GetAllTokensResponse, _response.json())  # type: ignore
+            return typing.cast(GetAllTokensResponse, construct_type(type_=GetAllTokensResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -423,16 +444,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tokens"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -446,15 +469,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add(
@@ -515,16 +540,18 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="PUT",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/tokens/{jsonable_encoder(token)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -541,15 +568,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
@@ -598,16 +627,18 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="PATCH",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/tokens/{jsonable_encoder(token)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -624,15 +655,17 @@
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(
@@ -670,16 +703,18 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"users/{jsonable_encoder(user_id)}/tokens/{jsonable_encoder(token)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -688,24 +723,26 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(GetUserTokenResponse, _response.json())  # type: ignore
+            return typing.cast(GetUserTokenResponse, construct_type(type_=GetUserTokenResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def list(
+    async def list_(
         self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> GetAllTokensResponse:
         """
         Gets all tokens available for a :user_id
 
         Parameters
         ----------
@@ -722,25 +759,27 @@
         Examples
         --------
         from courier.client import AsyncCourier
 
         client = AsyncCourier(
             authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        await client.users.tokens.list(
+        await client.users.tokens.list_(
             user_id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/tokens"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -749,15 +788,17 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(GetAllTokensResponse, _response.json())  # type: ignore
+            return typing.cast(GetAllTokensResponse, construct_type(type_=GetAllTokensResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(
+                typing.cast(BadRequest, construct_type(type_=BadRequest, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.5/src/courier/users/tokens/types/__init__.py` & `trycourier-6.1.0/src/courier/users/tokens/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.5/src/courier/users/tokens/types/delete_user_token_opts.py` & `trycourier-6.1.0/src/courier/notifications/types/notification_channel_content.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class DeleteUserTokenOpts(pydantic_v1.BaseModel):
-    user_id: str
-    token: str
+class NotificationChannelContent(UncheckedBaseModel):
+    subject: typing.Optional[str] = None
+    title: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/users/tokens/types/get_user_token_response.py` & `trycourier-6.1.0/src/courier/send/types/preferences.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
-from .token_status import TokenStatus
-from .user_token import UserToken
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class GetUserTokenResponse(UserToken):
-    status: typing.Optional[TokenStatus] = None
-    status_reason: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    The reason for the token status.
-    """
+class Preferences(UncheckedBaseModel):
+    template_ids: typing.List[str] = pydantic_v1.Field(alias="templateIds")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/users/tokens/types/patch_operation.py` & `trycourier-6.1.0/src/courier/send/types/list_filter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class PatchOperation(pydantic_v1.BaseModel):
-    op: str = pydantic_v1.Field()
+class ListFilter(UncheckedBaseModel):
+    operator: typing.Literal["MEMBER_OF"] = pydantic_v1.Field()
     """
-    The operation to perform.
+    Send to users only if they are member of the account
     """
 
-    path: str = pydantic_v1.Field()
-    """
-    The JSON path specifying the part of the profile to operate on.
-    """
-
-    value: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    The value for the operation.
-    """
+    path: typing.Literal["account_id"]
+    value: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/users/tokens/types/patch_user_token_opts.py` & `trycourier-6.1.0/src/courier/profiles/types/subscribe_to_lists_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
-from .patch_operation import PatchOperation
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class PatchUserTokenOpts(pydantic_v1.BaseModel):
-    patch: typing.List[PatchOperation]
+class SubscribeToListsResponse(UncheckedBaseModel):
+    status: typing.Literal["SUCCESS"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/users/tokens/types/put_user_token_opts.py` & `trycourier-6.1.0/src/courier/profiles/types/profile_get_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
-from .user_token import UserToken
+from ...commons.types.recipient_preferences import RecipientPreferences
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class PutUserTokenOpts(pydantic_v1.BaseModel):
-    user_id: str
-    token: UserToken
+class ProfileGetResponse(UncheckedBaseModel):
+    profile: typing.Dict[str, typing.Any]
+    preferences: typing.Optional[RecipientPreferences] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/src/courier/users/tokens/types/tracking.py` & `trycourier-6.1.0/src/courier/send/types/brand_settings_social_presence.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from .base_social_presence import BaseSocialPresence
 
 
-class Tracking(pydantic_v1.BaseModel):
-    os_version: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    The operating system version
-    """
-
-    ip: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    The IP address of the device
-    """
-
-    lat: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    The latitude of the device
-    """
-
-    long_: typing.Optional[str] = pydantic_v1.Field(alias="long", default=None)
-    """
-    The longitude of the device
-    """
+class BrandSettingsSocialPresence(UncheckedBaseModel):
+    inherit_default: typing.Optional[bool] = pydantic_v1.Field(alias="inheritDefault", default=None)
+    facebook: typing.Optional[BaseSocialPresence] = None
+    instagram: typing.Optional[BaseSocialPresence] = None
+    linkedin: typing.Optional[BaseSocialPresence] = None
+    medium: typing.Optional[BaseSocialPresence] = None
+    twitter: typing.Optional[BaseSocialPresence] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `trycourier-6.0.5/src/courier/users/tokens/types/user_token.py` & `trycourier-6.1.0/src/courier/users/tokens/types/user_token.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 from .device import Device
 from .expiry_date import ExpiryDate
 from .provider_key import ProviderKey
 from .tracking import Tracking
 
 
-class UserToken(pydantic_v1.BaseModel):
+class UserToken(UncheckedBaseModel):
     token: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     Full body of the token. Must match token in URL.
     """
 
     provider_key: ProviderKey
     expiry_date: typing.Optional[ExpiryDate] = pydantic_v1.Field(default=None)
@@ -39,15 +40,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.5/PKG-INFO` & `trycourier-6.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: trycourier
-Version: 6.0.5
+Version: 6.1.0
 Summary: 
 Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Dist: httpx (>=0.21.2)
 Requires-Dist: pydantic (>=1.9.2)
 Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown
 
 [![Courier: Your Complete Communication Stack](https://marketing-assets-public.s3.us-west-1.amazonaws.com/github_nodejs.png)](https://courier.com)
 
@@ -22,164 +32,159 @@
 
 ## Installation
 
 Install from PyPI
 
 ```shell
 pip install trycourier
-# or 
+# or
 poetry add trycourier
 ```
 
 Python 3.7 or later is required.
 
 ## Usage
+
 Use the `Courier` class to access all of our endpoints.
 
 ```python
-import os
 import courier
 
 from courier.client import Courier
 
 client = Courier(
   authorization_token="YOUR_TOKENY" # Defaults to COURIER_AUTH_TOKEN
 )
 
 response = client.send(
   message=courier.ContentMessage(
     to=courier.UserRecipient(
       email="marty_mcfly@email.com",
       data={
-        name: "Marty",
+        "name": "Marty",
       }
     ),
     content=courier.ElementalContentSugar(
       title="Back to the Future",
-      body="Oh my {{name}}, we need 1.21 Gigawatts!",
+      body="Oh my {name}, we need 1.21 Gigawatts!",
     ),
-    routing=courier.Routing(
-      method=courier.RoutingMethod.ALL,
-      channels=["email"]
-    )
+    routing=courier.Routing(method="all", channels=["inbox", "email"]),
   )
 )
 
 print(response)
 ```
 
 ## Async Client
-The SDK also exports an asynchronous client, `AsyncCourier`. 
+
+The SDK also exports an asynchronous client, `AsyncCourier`.
 
 ```python
 import os
 import courier
 import asyncio
 
 from courier.client import AsyncCourier
 
 client = AsyncCourier(
   authorization_token="YOUR_TOKEN" # Defaults to COURIER_AUTH_TOKEN
 )
 
-async def main() -> None: 
+async def main() -> None:
   response = await client.send(
     message=courier.ContentMessage(
       to=courier.UserRecipient(
         email="marty_mcfly@email.com",
         data={
-          name: "Marty",
+          "name": "Marty",
         }
       ),
       content=courier.ElementalContentSugar(
         title="Back to the Future",
-        body="Oh my {{name}}, we need 1.21 Gigawatts!",
+        body="Oh my {name}, we need 1.21 Gigawatts!",
       ),
-      routing=courier.Routing(
-        method=courier.RoutingMethod.ALL,
-        channels=["email"]
-      )
+      routing=courier.Routing(method="all", channels=["email", "inbox"]),
     )
   )
 
 asyncio.run(main())
 ```
 
 ## Timeouts
-By default, the client is configured to have a timeout of 60 seconds. 
-You can customize this value at client instantiation. 
+
+By default, the client is configured to have a timeout of 60 seconds.
+You can customize this value at client instantiation.
 
 ```python
 from courier.client import Courier
 
 client = Courier(
   authorization_token="YOUR_TOKEN",
   timeout=30
 )
 ```
 
 ## Handling Exceptions
-All exceptions thrown by the SDK will sublcass [courier.ApiError](./src/courier/core/api_error.py). 
+
+All exceptions thrown by the SDK will subclass [courier.ApiError](./src/courier/core/api_error.py).
 
 ```python
 import courier
 
 from courier.core import ApiError
 
 try:
   courier.send(...)
-except APIError as e:  
+except APIError as e:
   # handle any api related error
 ```
 
 ## Idempotency Keys
 
-For `POST` methods, you can supply an `idempotencyKey` in the config parameter to 
-ensure the idempotency of the API Call. We recommend that you use a `V4 UUID` for the key. 
-Keys are eligible to be removed from the system after they're at least 24 hours old, 
-and a new request is generated if a key is reused after the original has been removed. 
-For more info, see [Idempotent Requests](https://docs.courier.com/reference/idempotent-requests) 
+For `POST` methods, you can supply an `idempotencyKey` in the config parameter to
+ensure the idempotency of the API Call. We recommend that you use a `V4 UUID` for the key.
+Keys are eligible to be removed from the system after they're at least 24 hours old,
+and a new request is generated if a key is reused after the original has been removed.
+For more info, see [Idempotent Requests](https://docs.courier.com/reference/idempotent-requests)
 in the Courier documentation.
 
 ```python
 import courier
 
 courier.send(
-  message={...}, 
-  idempotency_key"YOUR_KEY", 
+  message={...},
+  idempotency_key"YOUR_KEY",
   idempotency_expiration="YOUR_EXPIRATION")
 ```
 
 ## Additional Usage Examples
 
 ### Send Template Message
 
 ```python
 import courier
-
-from courier import Courier
+from courier.client import Courier
 
 client = Courier(
   authorization_token="YOUR_TOKEN")
 
 response = client.send(
     message=courier.TemplateMessage(
       template="my-template",
-      to=courier.UserRecipient(email="foo@bar.com")
+      to=courier.UserRecipient(user_id="abc-123")
     )
 )
-print(response.message_id)
+print(response.request_id)
 ```
 
 ### UTM Metadata with Message
 
 ```python
 import courier
-
-from courier import Courier
+from courier.client import Courier
 
 client = Courier(
   authorization_token="YOUR_TOKEN")
 
 response = client.send(
     message=courier.ContentMessage(
       content=courier.ElementalContent(
@@ -190,33 +195,31 @@
             href="courier.com",
             style="button",
             align="center"
           )
         ]
       ),
       to=courier.UserRecipient(email="foo@bar.com"),
-      routing=courier.Routing(
-        method=courier.RoutingMethod.SINGLE,
-        channels=["email"]
-      ),
+      routing=courier.Routing(method="all", channels=["email"]),
       metadata=courier.MessageMetadata(
         utm=courier.Utm(source="python")
       )
     )
 )
 print(response.request_id)
 ```
 
 ## Advanced
 
 ### Overriding HTTP Client
-You can override the httpx client to customize it for your use case. Some common usecases 
+
+You can override the httpx client to customize it for your use case. Some common usecases
 include support for proxies and transports.
 
-```python 
+```python
 import httpx
 from courier.client import Courier
 
 client = Courier(
     http_client=httpx.Client(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
```

