# Comparing `tmp/antimatter-1.0.0-py3-none-any.whl.zip` & `tmp/antimatter-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,286 +1,143 @@
-Zip file size: 385927 bytes, number of entries: 284
--rw-r--r--  2.0 unx      327 b- defN 20-Apr-16 12:00 antimatter/__init__.py
--rw-r--r--  2.0 unx    10768 b- defN 20-Apr-16 12:00 antimatter/capsule.py
--rw-r--r--  2.0 unx      928 b- defN 20-Apr-16 12:00 antimatter/cell_path.py
--rw-r--r--  2.0 unx     3410 b- defN 20-Apr-16 12:00 antimatter/extra_helper.py
--rw-r--r--  2.0 unx    25527 b- defN 20-Apr-16 12:00 antimatter/session.py
+Zip file size: 114216 bytes, number of entries: 141
+-rw-r--r--  2.0 unx      390 b- defN 20-Apr-16 12:00 antimatter/__init__.py
+-rw-r--r--  2.0 unx    15233 b- defN 20-Apr-16 12:00 antimatter/capsule.py
+-rw-r--r--  2.0 unx      928 b- defN 20-Apr-16 12:00 antimatter/cell_utils.py
+-rw-r--r--  2.0 unx     5057 b- defN 20-Apr-16 12:00 antimatter/extra_helper.py
+-rw-r--r--  2.0 unx    28151 b- defN 20-Apr-16 12:00 antimatter/session.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/auth/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/auth/config/__init__.py
--rw-r--r--  2.0 unx    11557 b- defN 20-Apr-16 12:00 antimatter/auth/config/auth_config.py
--rw-r--r--  2.0 unx     1930 b- defN 20-Apr-16 12:00 antimatter/auth/config/global_identity.py
--rw-r--r--  2.0 unx      535 b- defN 20-Apr-16 12:00 antimatter/auth/config/profiles.py
--rw-r--r--  2.0 unx      429 b- defN 20-Apr-16 12:00 antimatter/auth/config/tokens.py
--rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/auth/google/__init__.py
--rw-r--r--  2.0 unx      495 b- defN 20-Apr-16 12:00 antimatter/auth/google/models.py
+-rw-r--r--  2.0 unx    14913 b- defN 20-Apr-16 12:00 antimatter/auth/config/auth_config.py
+-rw-r--r--  2.0 unx     1212 b- defN 20-Apr-16 12:00 antimatter/auth/config/global_identity.py
+-rw-r--r--  2.0 unx     1170 b- defN 20-Apr-16 12:00 antimatter/auth/config/profiles.py
+-rw-r--r--  2.0 unx     3180 b- defN 20-Apr-16 12:00 antimatter/auth/config/tokens.py
+-rw-r--r--  2.0 unx      383 b- defN 20-Apr-16 12:00 antimatter/authn/__init__.py
+-rw-r--r--  2.0 unx     1630 b- defN 20-Apr-16 12:00 antimatter/authn/apikey.py
+-rw-r--r--  2.0 unx     1596 b- defN 20-Apr-16 12:00 antimatter/authn/base.py
+-rw-r--r--  2.0 unx     6322 b- defN 20-Apr-16 12:00 antimatter/authn/google_oauth.py
+-rw-r--r--  2.0 unx     2313 b- defN 20-Apr-16 12:00 antimatter/authn/oauth_domain.py
+-rw-r--r--  2.0 unx     1129 b- defN 20-Apr-16 12:00 antimatter/authn/static_oauth.py
+-rw-r--r--  2.0 unx      627 b- defN 20-Apr-16 12:00 antimatter/authn/unauth.py
+-rw-r--r--  2.0 unx      102 b- defN 20-Apr-16 12:00 antimatter/authz/__init__.py
+-rw-r--r--  2.0 unx      692 b- defN 20-Apr-16 12:00 antimatter/authz/base.py
+-rw-r--r--  2.0 unx      794 b- defN 20-Apr-16 12:00 antimatter/authz/token.py
 -rw-r--r--  2.0 unx      759 b- defN 20-Apr-16 12:00 antimatter/builders/__init__.py
--rw-r--r--  2.0 unx     1630 b- defN 20-Apr-16 12:00 antimatter/builders/capability.py
--rw-r--r--  2.0 unx     2386 b- defN 20-Apr-16 12:00 antimatter/builders/fact_policy.py
--rw-r--r--  2.0 unx     3338 b- defN 20-Apr-16 12:00 antimatter/builders/read_context.py
--rw-r--r--  2.0 unx     4831 b- defN 20-Apr-16 12:00 antimatter/builders/read_context_rule.py
--rw-r--r--  2.0 unx     4174 b- defN 20-Apr-16 12:00 antimatter/builders/root_encryption_key.py
--rw-r--r--  2.0 unx     2118 b- defN 20-Apr-16 12:00 antimatter/builders/settings_patch.py
--rw-r--r--  2.0 unx     4390 b- defN 20-Apr-16 12:00 antimatter/builders/write_context.py
--rw-r--r--  2.0 unx     2460 b- defN 20-Apr-16 12:00 antimatter/builders/write_context_rule.py
+-rw-r--r--  2.0 unx     1627 b- defN 20-Apr-16 12:00 antimatter/builders/capability.py
+-rw-r--r--  2.0 unx     2383 b- defN 20-Apr-16 12:00 antimatter/builders/fact_policy.py
+-rw-r--r--  2.0 unx     3335 b- defN 20-Apr-16 12:00 antimatter/builders/read_context.py
+-rw-r--r--  2.0 unx     4828 b- defN 20-Apr-16 12:00 antimatter/builders/read_context_rule.py
+-rw-r--r--  2.0 unx     4259 b- defN 20-Apr-16 12:00 antimatter/builders/root_encryption_key.py
+-rw-r--r--  2.0 unx     2115 b- defN 20-Apr-16 12:00 antimatter/builders/settings_patch.py
+-rw-r--r--  2.0 unx     4387 b- defN 20-Apr-16 12:00 antimatter/builders/write_context.py
+-rw-r--r--  2.0 unx     2457 b- defN 20-Apr-16 12:00 antimatter/builders/write_context_rule.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/cap_prep/__init__.py
 -rw-r--r--  2.0 unx     3158 b- defN 20-Apr-16 12:00 antimatter/cap_prep/applicator.py
--rw-r--r--  2.0 unx     3811 b- defN 20-Apr-16 12:00 antimatter/cap_prep/prep.py
+-rw-r--r--  2.0 unx     3812 b- defN 20-Apr-16 12:00 antimatter/cap_prep/prep.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/cap_prep/tests/__init__.py
 -rw-r--r--  2.0 unx     3875 b- defN 20-Apr-16 12:00 antimatter/cap_prep/tests/test_applicator.py
--rw-r--r--  2.0 unx     2558 b- defN 20-Apr-16 12:00 antimatter/cap_prep/tests/test_prep.py
--rw-r--r--  2.0 unx       66 b- defN 20-Apr-16 12:00 antimatter/capabilities/__init__.py
--rw-r--r--  2.0 unx     1714 b- defN 20-Apr-16 12:00 antimatter/capabilities/converter.py
--rw-r--r--  2.0 unx    13909 b- defN 20-Apr-16 12:00 antimatter/client/__init__.py
--rw-r--r--  2.0 unx    24612 b- defN 20-Apr-16 12:00 antimatter/client/api_client.py
--rw-r--r--  2.0 unx      674 b- defN 20-Apr-16 12:00 antimatter/client/api_response.py
--rw-r--r--  2.0 unx    14983 b- defN 20-Apr-16 12:00 antimatter/client/configuration.py
--rw-r--r--  2.0 unx     5954 b- defN 20-Apr-16 12:00 antimatter/client/exceptions.py
--rw-r--r--  2.0 unx     9799 b- defN 20-Apr-16 12:00 antimatter/client/rest.py
--rw-r--r--  2.0 unx      549 b- defN 20-Apr-16 12:00 antimatter/client/api/__init__.py
--rw-r--r--  2.0 unx    31800 b- defN 20-Apr-16 12:00 antimatter/client/api/account_management_api.py
--rw-r--r--  2.0 unx   199539 b- defN 20-Apr-16 12:00 antimatter/client/api/authentication_api.py
--rw-r--r--  2.0 unx   146264 b- defN 20-Apr-16 12:00 antimatter/client/api/capsules_api.py
--rw-r--r--  2.0 unx   201452 b- defN 20-Apr-16 12:00 antimatter/client/api/contexts_api.py
--rw-r--r--  2.0 unx   107683 b- defN 20-Apr-16 12:00 antimatter/client/api/encryption_api.py
--rw-r--r--  2.0 unx   162476 b- defN 20-Apr-16 12:00 antimatter/client/api/general_api.py
--rw-r--r--  2.0 unx    79499 b- defN 20-Apr-16 12:00 antimatter/client/api/internal_api.py
--rw-r--r--  2.0 unx   175071 b- defN 20-Apr-16 12:00 antimatter/client/api/policy_api.py
--rw-r--r--  2.0 unx    12837 b- defN 20-Apr-16 12:00 antimatter/client/models/__init__.py
--rw-r--r--  2.0 unx     6771 b- defN 20-Apr-16 12:00 antimatter/client/models/access_log_entry.py
--rw-r--r--  2.0 unx     3245 b- defN 20-Apr-16 12:00 antimatter/client/models/access_log_entry_create_info.py
--rw-r--r--  2.0 unx     3085 b- defN 20-Apr-16 12:00 antimatter/client/models/access_log_entry_open_info.py
--rw-r--r--  2.0 unx     5291 b- defN 20-Apr-16 12:00 antimatter/client/models/access_log_entry_read_info.py
--rw-r--r--  2.0 unx     3151 b- defN 20-Apr-16 12:00 antimatter/client/models/access_log_results.py
--rw-r--r--  2.0 unx     3077 b- defN 20-Apr-16 12:00 antimatter/client/models/active_root_encryption_key_id.py
--rw-r--r--  2.0 unx     3041 b- defN 20-Apr-16 12:00 antimatter/client/models/add_capsule_log_entry_request.py
--rw-r--r--  2.0 unx     4841 b- defN 20-Apr-16 12:00 antimatter/client/models/add_read_context.py
--rw-r--r--  2.0 unx     3214 b- defN 20-Apr-16 12:00 antimatter/client/models/add_write_context.py
--rw-r--r--  2.0 unx     3170 b- defN 20-Apr-16 12:00 antimatter/client/models/antimatter_delegated_aws_key_info.py
--rw-r--r--  2.0 unx     2801 b- defN 20-Apr-16 12:00 antimatter/client/models/api_key_domain_identity_provider_details.py
--rw-r--r--  2.0 unx     3305 b- defN 20-Apr-16 12:00 antimatter/client/models/available_delegated_root_encryption_key_provider.py
--rw-r--r--  2.0 unx     3121 b- defN 20-Apr-16 12:00 antimatter/client/models/available_root_encryption_key_providers.py
--rw-r--r--  2.0 unx     6728 b- defN 20-Apr-16 12:00 antimatter/client/models/available_root_encryption_key_providers_providers_inner.py
--rw-r--r--  2.0 unx     3197 b- defN 20-Apr-16 12:00 antimatter/client/models/available_service_account_root_encryption_key_provider.py
--rw-r--r--  2.0 unx     3459 b- defN 20-Apr-16 12:00 antimatter/client/models/aws_service_account_key_info.py
--rw-r--r--  2.0 unx     3154 b- defN 20-Apr-16 12:00 antimatter/client/models/capability.py
--rw-r--r--  2.0 unx     4985 b- defN 20-Apr-16 12:00 antimatter/client/models/capability_definition.py
--rw-r--r--  2.0 unx     2964 b- defN 20-Apr-16 12:00 antimatter/client/models/capability_definition_list.py
--rw-r--r--  2.0 unx     2883 b- defN 20-Apr-16 12:00 antimatter/client/models/capability_list.py
--rw-r--r--  2.0 unx     3267 b- defN 20-Apr-16 12:00 antimatter/client/models/capability_rule.py
--rw-r--r--  2.0 unx     3640 b- defN 20-Apr-16 12:00 antimatter/client/models/capability_rule_match_expressions_inner.py
--rw-r--r--  2.0 unx     4572 b- defN 20-Apr-16 12:00 antimatter/client/models/capsule_create_response.py
--rw-r--r--  2.0 unx     4883 b- defN 20-Apr-16 12:00 antimatter/client/models/capsule_info.py
--rw-r--r--  2.0 unx     3039 b- defN 20-Apr-16 12:00 antimatter/client/models/capsule_list.py
--rw-r--r--  2.0 unx     2745 b- defN 20-Apr-16 12:00 antimatter/client/models/capsule_open_request.py
--rw-r--r--  2.0 unx     4211 b- defN 20-Apr-16 12:00 antimatter/client/models/capsule_open_response.py
--rw-r--r--  2.0 unx     3444 b- defN 20-Apr-16 12:00 antimatter/client/models/capsule_open_response_read_context_configuration.py
--rw-r--r--  2.0 unx     3787 b- defN 20-Apr-16 12:00 antimatter/client/models/capsule_seal_request.py
--rw-r--r--  2.0 unx     2962 b- defN 20-Apr-16 12:00 antimatter/client/models/conflict_error.py
--rw-r--r--  2.0 unx     7314 b- defN 20-Apr-16 12:00 antimatter/client/models/create_peer_domain.py
--rw-r--r--  2.0 unx     3122 b- defN 20-Apr-16 12:00 antimatter/client/models/data_tagging_hook_input.py
--rw-r--r--  2.0 unx     3199 b- defN 20-Apr-16 12:00 antimatter/client/models/data_tagging_hook_input_records_inner.py
--rw-r--r--  2.0 unx     2860 b- defN 20-Apr-16 12:00 antimatter/client/models/data_tagging_hook_input_records_inner_elements_inner.py
--rw-r--r--  2.0 unx     3559 b- defN 20-Apr-16 12:00 antimatter/client/models/data_tagging_hook_response.py
--rw-r--r--  2.0 unx     3032 b- defN 20-Apr-16 12:00 antimatter/client/models/data_tagging_hook_response_records_inner.py
--rw-r--r--  2.0 unx     2481 b- defN 20-Apr-16 12:00 antimatter/client/models/delete_tags.py
--rw-r--r--  2.0 unx     2830 b- defN 20-Apr-16 12:00 antimatter/client/models/domain.py
--rw-r--r--  2.0 unx     2971 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_add_read_context_rule200_response.py
--rw-r--r--  2.0 unx     2467 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_authenticate.py
--rw-r--r--  2.0 unx     2420 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_authenticate_response.py
--rw-r--r--  2.0 unx     2600 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_contact_issue_verify_request.py
--rw-r--r--  2.0 unx     4350 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_control_log_entry.py
--rw-r--r--  2.0 unx     3201 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_control_log_results.py
--rw-r--r--  2.0 unx     2969 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_fact_list.py
--rw-r--r--  2.0 unx     2933 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_hooks_list.py
--rw-r--r--  2.0 unx     3653 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_hooks_list_hooks_inner.py
--rw-r--r--  2.0 unx     3039 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_identity_api_key_principal_params.py
--rw-r--r--  2.0 unx     2966 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_identity_email_principal_params.py
--rw-r--r--  2.0 unx     3086 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_identity_hosted_domain_principal_params.py
--rw-r--r--  2.0 unx     7406 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_identity_principal_details.py
--rw-r--r--  2.0 unx     6312 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_identity_provider_details.py
--rw-r--r--  2.0 unx     5177 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_identity_provider_info.py
--rw-r--r--  2.0 unx     3204 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_identity_provider_list.py
--rw-r--r--  2.0 unx     2975 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_identity_provider_principal_list.py
--rw-r--r--  2.0 unx     3426 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_identity_provider_principal_params.py
--rw-r--r--  2.0 unx      942 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_identity_provider_principal_type.py
--rw-r--r--  2.0 unx      928 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_identity_provider_type.py
--rw-r--r--  2.0 unx     3297 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_insert_identity_provider_principal200_response.py
--rw-r--r--  2.0 unx     2964 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_insert_write_context_regex_rule200_response.py
--rw-r--r--  2.0 unx    14602 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_peer_config.py
--rw-r--r--  2.0 unx     2920 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_peer_list.py
--rw-r--r--  2.0 unx     3461 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_peer_list_peers_inner.py
--rw-r--r--  2.0 unx     3450 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_policy.py
--rw-r--r--  2.0 unx     7142 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_policy_rule.py
--rw-r--r--  2.0 unx     3911 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_private_info.py
--rw-r--r--  2.0 unx     3907 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_public_info.py
--rw-r--r--  2.0 unx     3037 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_resource_summary.py
--rw-r--r--  2.0 unx     3367 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_resource_summary_schema_inner.py
--rw-r--r--  2.0 unx     4011 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_settings.py
--rw-r--r--  2.0 unx     2865 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_settings_disaster_recovery.py
--rw-r--r--  2.0 unx     2887 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_settings_patch.py
--rw-r--r--  2.0 unx     3016 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_status.py
--rw-r--r--  2.0 unx     2866 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_status_notifications_inner.py
--rw-r--r--  2.0 unx     3039 b- defN 20-Apr-16 12:00 antimatter/client/models/domain_tag_info_results.py
--rw-r--r--  2.0 unx     2489 b- defN 20-Apr-16 12:00 antimatter/client/models/error.py
--rw-r--r--  2.0 unx     3824 b- defN 20-Apr-16 12:00 antimatter/client/models/fact.py
--rw-r--r--  2.0 unx     2772 b- defN 20-Apr-16 12:00 antimatter/client/models/fact_list.py
--rw-r--r--  2.0 unx     4250 b- defN 20-Apr-16 12:00 antimatter/client/models/fact_policy_rules_inner.py
--rw-r--r--  2.0 unx     4318 b- defN 20-Apr-16 12:00 antimatter/client/models/fact_policy_rules_inner_arguments_inner.py
--rw-r--r--  2.0 unx     4953 b- defN 20-Apr-16 12:00 antimatter/client/models/fact_type_definition.py
--rw-r--r--  2.0 unx     3892 b- defN 20-Apr-16 12:00 antimatter/client/models/gcp_service_account_key_info.py
--rw-r--r--  2.0 unx     3057 b- defN 20-Apr-16 12:00 antimatter/client/models/google_o_auth_domain_identity_provider_details.py
--rw-r--r--  2.0 unx     2501 b- defN 20-Apr-16 12:00 antimatter/client/models/hook_invocation.py
--rw-r--r--  2.0 unx     2689 b- defN 20-Apr-16 12:00 antimatter/client/models/invalid_request_error.py
--rw-r--r--  2.0 unx     3215 b- defN 20-Apr-16 12:00 antimatter/client/models/json_patch_request_add.py
--rw-r--r--  2.0 unx     6165 b- defN 20-Apr-16 12:00 antimatter/client/models/json_patch_request_add_value.py
--rw-r--r--  2.0 unx     2811 b- defN 20-Apr-16 12:00 antimatter/client/models/json_patch_request_copy.py
--rw-r--r--  2.0 unx     2811 b- defN 20-Apr-16 12:00 antimatter/client/models/json_patch_request_move.py
--rw-r--r--  2.0 unx     2823 b- defN 20-Apr-16 12:00 antimatter/client/models/json_patch_request_remove.py
--rw-r--r--  2.0 unx     3255 b- defN 20-Apr-16 12:00 antimatter/client/models/json_patch_request_replace.py
--rw-r--r--  2.0 unx     6197 b- defN 20-Apr-16 12:00 antimatter/client/models/json_patch_request_replace_value.py
--rw-r--r--  2.0 unx     3217 b- defN 20-Apr-16 12:00 antimatter/client/models/json_patch_request_tst.py
--rw-r--r--  2.0 unx     6166 b- defN 20-Apr-16 12:00 antimatter/client/models/json_patch_request_tst_value.py
--rw-r--r--  2.0 unx     3009 b- defN 20-Apr-16 12:00 antimatter/client/models/key_infos.py
--rw-r--r--  2.0 unx     6812 b- defN 20-Apr-16 12:00 antimatter/client/models/key_infos_key_information.py
--rw-r--r--  2.0 unx     3448 b- defN 20-Apr-16 12:00 antimatter/client/models/new_access_log_entry.py
--rw-r--r--  2.0 unx     4607 b- defN 20-Apr-16 12:00 antimatter/client/models/new_access_log_entry_read_info.py
--rw-r--r--  2.0 unx     3178 b- defN 20-Apr-16 12:00 antimatter/client/models/new_capability_definition.py
--rw-r--r--  2.0 unx     2720 b- defN 20-Apr-16 12:00 antimatter/client/models/new_domain.py
--rw-r--r--  2.0 unx     4777 b- defN 20-Apr-16 12:00 antimatter/client/models/new_domain_policy_rule.py
--rw-r--r--  2.0 unx     3006 b- defN 20-Apr-16 12:00 antimatter/client/models/new_domain_response.py
--rw-r--r--  2.0 unx     2683 b- defN 20-Apr-16 12:00 antimatter/client/models/new_fact.py
--rw-r--r--  2.0 unx     3261 b- defN 20-Apr-16 12:00 antimatter/client/models/new_fact_type_definition.py
--rw-r--r--  2.0 unx     3131 b- defN 20-Apr-16 12:00 antimatter/client/models/new_fact_type_definition_arguments_inner.py
--rw-r--r--  2.0 unx     6187 b- defN 20-Apr-16 12:00 antimatter/client/models/new_read_context_config_rule.py
--rw-r--r--  2.0 unx     9083 b- defN 20-Apr-16 12:00 antimatter/client/models/patch_request_inner.py
--rw-r--r--  2.0 unx      857 b- defN 20-Apr-16 12:00 antimatter/client/models/policy_rule_operation.py
--rw-r--r--  2.0 unx      834 b- defN 20-Apr-16 12:00 antimatter/client/models/policy_rule_result.py
--rw-r--r--  2.0 unx     4070 b- defN 20-Apr-16 12:00 antimatter/client/models/principal_info.py
--rw-r--r--  2.0 unx     3447 b- defN 20-Apr-16 12:00 antimatter/client/models/principal_summary.py
--rw-r--r--  2.0 unx     7791 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_config_rule.py
--rw-r--r--  2.0 unx     6947 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_details.py
--rw-r--r--  2.0 unx     3003 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_list.py
--rw-r--r--  2.0 unx     2865 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_parameter.py
--rw-r--r--  2.0 unx     4935 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_required_hook.py
--rw-r--r--  2.0 unx     3743 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_rule_facts_inner.py
--rw-r--r--  2.0 unx     3259 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_rule_facts_inner_arguments_inner.py
--rw-r--r--  2.0 unx     4218 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_rule_match_expressions_inner.py
--rw-r--r--  2.0 unx     5704 b- defN 20-Apr-16 12:00 antimatter/client/models/read_context_short_details.py
--rw-r--r--  2.0 unx     2920 b- defN 20-Apr-16 12:00 antimatter/client/models/resource_exhausted_error.py
--rw-r--r--  2.0 unx     2912 b- defN 20-Apr-16 12:00 antimatter/client/models/resource_not_found_error.py
--rw-r--r--  2.0 unx     2538 b- defN 20-Apr-16 12:00 antimatter/client/models/root_encryption_key_id_response.py
--rw-r--r--  2.0 unx     3016 b- defN 20-Apr-16 12:00 antimatter/client/models/root_encryption_key_item.py
--rw-r--r--  2.0 unx     4204 b- defN 20-Apr-16 12:00 antimatter/client/models/root_encryption_key_test_response.py
--rw-r--r--  2.0 unx     2642 b- defN 20-Apr-16 12:00 antimatter/client/models/rotate_key_encryption_key_response.py
--rw-r--r--  2.0 unx     2499 b- defN 20-Apr-16 12:00 antimatter/client/models/starred_domain_list.py
--rw-r--r--  2.0 unx     4076 b- defN 20-Apr-16 12:00 antimatter/client/models/tag.py
--rw-r--r--  2.0 unx     2488 b- defN 20-Apr-16 12:00 antimatter/client/models/tag_meta.py
--rw-r--r--  2.0 unx     3480 b- defN 20-Apr-16 12:00 antimatter/client/models/tag_set.py
--rw-r--r--  2.0 unx     3107 b- defN 20-Apr-16 12:00 antimatter/client/models/tag_set_span_tags_inner.py
--rw-r--r--  2.0 unx     3764 b- defN 20-Apr-16 12:00 antimatter/client/models/tag_summary.py
--rw-r--r--  2.0 unx     2988 b- defN 20-Apr-16 12:00 antimatter/client/models/tag_summary_elided_tags_inner.py
--rw-r--r--  2.0 unx     2843 b- defN 20-Apr-16 12:00 antimatter/client/models/tag_summary_unique_tags_inner.py
--rw-r--r--  2.0 unx      898 b- defN 20-Apr-16 12:00 antimatter/client/models/tag_type_field.py
--rw-r--r--  2.0 unx     2523 b- defN 20-Apr-16 12:00 antimatter/client/models/unauthorized_error.py
--rw-r--r--  2.0 unx     3011 b- defN 20-Apr-16 12:00 antimatter/client/models/upsert_span_tags_request.py
--rw-r--r--  2.0 unx     3079 b- defN 20-Apr-16 12:00 antimatter/client/models/verify_contact_response.py
--rw-r--r--  2.0 unx     3515 b- defN 20-Apr-16 12:00 antimatter/client/models/write_context_config_info.py
--rw-r--r--  2.0 unx     4649 b- defN 20-Apr-16 12:00 antimatter/client/models/write_context_config_info_required_hooks_inner.py
--rw-r--r--  2.0 unx     4932 b- defN 20-Apr-16 12:00 antimatter/client/models/write_context_details.py
--rw-r--r--  2.0 unx     3000 b- defN 20-Apr-16 12:00 antimatter/client/models/write_context_list.py
--rw-r--r--  2.0 unx     4337 b- defN 20-Apr-16 12:00 antimatter/client/models/write_context_regex_rule.py
--rw-r--r--  2.0 unx     3202 b- defN 20-Apr-16 12:00 antimatter/client/models/write_context_regex_tag.py
+-rw-r--r--  2.0 unx     2559 b- defN 20-Apr-16 12:00 antimatter/cap_prep/tests/test_prep.py
 -rw-r--r--  2.0 unx      561 b- defN 20-Apr-16 12:00 antimatter/constants/__init__.py
 -rw-r--r--  2.0 unx      227 b- defN 20-Apr-16 12:00 antimatter/constants/capability.py
 -rw-r--r--  2.0 unx      284 b- defN 20-Apr-16 12:00 antimatter/constants/domain_policy.py
 -rw-r--r--  2.0 unx      378 b- defN 20-Apr-16 12:00 antimatter/constants/fact_policy.py
 -rw-r--r--  2.0 unx      237 b- defN 20-Apr-16 12:00 antimatter/constants/hooks.py
 -rw-r--r--  2.0 unx      358 b- defN 20-Apr-16 12:00 antimatter/constants/identity_provider.py
 -rw-r--r--  2.0 unx     1083 b- defN 20-Apr-16 12:00 antimatter/constants/read_context_rule.py
 -rw-r--r--  2.0 unx      251 b- defN 20-Apr-16 12:00 antimatter/constants/settings_patch.py
 -rw-r--r--  2.0 unx      174 b- defN 20-Apr-16 12:00 antimatter/constants/write_context.py
+-rw-r--r--  2.0 unx      117 b- defN 20-Apr-16 12:00 antimatter/converters/__init__.py
+-rw-r--r--  2.0 unx      530 b- defN 20-Apr-16 12:00 antimatter/converters/capability.py
+-rw-r--r--  2.0 unx     3616 b- defN 20-Apr-16 12:00 antimatter/converters/tags.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/datatype/__init__.py
 -rw-r--r--  2.0 unx      556 b- defN 20-Apr-16 12:00 antimatter/datatype/datatypes.py
--rw-r--r--  2.0 unx     1791 b- defN 20-Apr-16 12:00 antimatter/datatype/infer.py
+-rw-r--r--  2.0 unx     1784 b- defN 20-Apr-16 12:00 antimatter/datatype/infer.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/datatype/tests/__init__.py
--rw-r--r--  2.0 unx      744 b- defN 20-Apr-16 12:00 antimatter/datatype/tests/test_factory.py
+-rw-r--r--  2.0 unx      737 b- defN 20-Apr-16 12:00 antimatter/datatype/tests/test_factory.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/dependencies/__init__.py
 -rw-r--r--  2.0 unx     3340 b- defN 20-Apr-16 12:00 antimatter/dependencies/package_hint.py
 -rw-r--r--  2.0 unx     2489 b- defN 20-Apr-16 12:00 antimatter/dependencies/versions.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/dependencies/tests/__init__.py
 -rw-r--r--  2.0 unx      252 b- defN 20-Apr-16 12:00 antimatter/dependencies/tests/test_package_hint.py
--rw-r--r--  2.0 unx      339 b- defN 20-Apr-16 12:00 antimatter/dependencies/tests/test_versions.py
--rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/errors/__init__.py
--rw-r--r--  2.0 unx     2156 b- defN 20-Apr-16 12:00 antimatter/errors/errors.py
+-rw-r--r--  2.0 unx      263 b- defN 20-Apr-16 12:00 antimatter/dependencies/tests/test_versions.py
+-rw-r--r--  2.0 unx       39 b- defN 20-Apr-16 12:00 antimatter/errors/__init__.py
+-rw-r--r--  2.0 unx     2272 b- defN 20-Apr-16 12:00 antimatter/errors/errors.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/fieldtype/__init__.py
--rw-r--r--  2.0 unx     3677 b- defN 20-Apr-16 12:00 antimatter/fieldtype/converters.py
+-rw-r--r--  2.0 unx     3640 b- defN 20-Apr-16 12:00 antimatter/fieldtype/converters.py
 -rw-r--r--  2.0 unx      567 b- defN 20-Apr-16 12:00 antimatter/fieldtype/fieldtypes.py
--rw-r--r--  2.0 unx     1324 b- defN 20-Apr-16 12:00 antimatter/fieldtype/infer.py
+-rw-r--r--  2.0 unx     1317 b- defN 20-Apr-16 12:00 antimatter/fieldtype/infer.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/fieldtype/tests/__init__.py
 -rw-r--r--  2.0 unx     1268 b- defN 20-Apr-16 12:00 antimatter/fieldtype/tests/test_fieldtypes.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/filetype/__init__.py
--rw-r--r--  2.0 unx     3142 b- defN 20-Apr-16 12:00 antimatter/filetype/extract.py
+-rw-r--r--  2.0 unx     3135 b- defN 20-Apr-16 12:00 antimatter/filetype/extract.py
 -rw-r--r--  2.0 unx     2607 b- defN 20-Apr-16 12:00 antimatter/filetype/infer.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/__init__.py
--rw-r--r--  2.0 unx     1491 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/test_filetypes.py
+-rw-r--r--  2.0 unx     1484 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/test_filetypes.py
 -rw-r--r--  2.0 unx     1446 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/test_infer.py
 -rw-r--r--  2.0 unx      176 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/fixtures/data-ndjson.json
 -rw-r--r--  2.0 unx      103 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/fixtures/data.csv
 -rw-r--r--  2.0 unx      194 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/fixtures/data.json
 -rw-r--r--  2.0 unx     2913 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/fixtures/data.parquet
 -rw-r--r--  2.0 unx      179 b- defN 20-Apr-16 12:00 antimatter/filetype/tests/fixtures/data.txt
--rw-r--r--  2.0 unx     1473 b- defN 20-Apr-16 12:00 antimatter/handlers/__init__.py
--rw-r--r--  2.0 unx     3602 b- defN 20-Apr-16 12:00 antimatter/handlers/base.py
--rw-r--r--  2.0 unx     2662 b- defN 20-Apr-16 12:00 antimatter/handlers/dict_list.py
+-rw-r--r--  2.0 unx     1474 b- defN 20-Apr-16 12:00 antimatter/handlers/__init__.py
+-rw-r--r--  2.0 unx     3595 b- defN 20-Apr-16 12:00 antimatter/handlers/base.py
+-rw-r--r--  2.0 unx     2666 b- defN 20-Apr-16 12:00 antimatter/handlers/dict_list.py
 -rw-r--r--  2.0 unx     2100 b- defN 20-Apr-16 12:00 antimatter/handlers/dictionary.py
--rw-r--r--  2.0 unx     8735 b- defN 20-Apr-16 12:00 antimatter/handlers/langchain.py
--rw-r--r--  2.0 unx     5001 b- defN 20-Apr-16 12:00 antimatter/handlers/pandas_dataframe.py
--rw-r--r--  2.0 unx     5617 b- defN 20-Apr-16 12:00 antimatter/handlers/pytorch_dataloader.py
--rw-r--r--  2.0 unx     1639 b- defN 20-Apr-16 12:00 antimatter/handlers/scalar.py
+-rw-r--r--  2.0 unx     8958 b- defN 20-Apr-16 12:00 antimatter/handlers/langchain.py
+-rw-r--r--  2.0 unx     4972 b- defN 20-Apr-16 12:00 antimatter/handlers/pandas_dataframe.py
+-rw-r--r--  2.0 unx     5608 b- defN 20-Apr-16 12:00 antimatter/handlers/pytorch_dataloader.py
+-rw-r--r--  2.0 unx     1642 b- defN 20-Apr-16 12:00 antimatter/handlers/scalar.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/__init__.py
--rw-r--r--  2.0 unx     5382 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/test_dict_list.py
--rw-r--r--  2.0 unx     2623 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/test_dictionary.py
--rw-r--r--  2.0 unx     1363 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/test_langchain.py
--rw-r--r--  2.0 unx    14370 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/test_pandas_dataframe.py
--rw-r--r--  2.0 unx     7210 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/test_pytorch_dataloader.py
--rw-r--r--  2.0 unx     1522 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/test_scalar.py
+-rw-r--r--  2.0 unx     5375 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/test_dict_list.py
+-rw-r--r--  2.0 unx     2616 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/test_dictionary.py
+-rw-r--r--  2.0 unx     1227 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/test_langchain.py
+-rw-r--r--  2.0 unx    14363 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/test_pandas_dataframe.py
+-rw-r--r--  2.0 unx     7203 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/test_pytorch_dataloader.py
+-rw-r--r--  2.0 unx     1515 b- defN 20-Apr-16 12:00 antimatter/handlers/tests/test_scalar.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/location/__init__.py
 -rw-r--r--  2.0 unx      791 b- defN 20-Apr-16 12:00 antimatter/location/infer.py
 -rw-r--r--  2.0 unx      290 b- defN 20-Apr-16 12:00 antimatter/location/locations.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/location/tests/__init__.py
 -rw-r--r--  2.0 unx      681 b- defN 20-Apr-16 12:00 antimatter/location/tests/test_infer.py
--rw-r--r--  2.0 unx      118 b- defN 20-Apr-16 12:00 antimatter/requirements/all.txt
--rw-r--r--  2.0 unx      227 b- defN 24-May-14 23:57 antimatter/requirements/core.txt
+-rw-r--r--  2.0 unx      145 b- defN 20-Apr-16 12:00 antimatter/requirements/all.txt
+-rw-r--r--  2.0 unx      262 b- defN 24-May-23 21:30 antimatter/requirements/core.txt
 -rw-r--r--  2.0 unx       12 b- defN 20-Apr-16 12:00 antimatter/requirements/dev.txt
--rw-r--r--  2.0 unx       66 b- defN 20-Apr-16 12:00 antimatter/requirements/langchain-huggingface.txt
--rw-r--r--  2.0 unx       36 b- defN 20-Apr-16 12:00 antimatter/requirements/langchain.txt
+-rw-r--r--  2.0 unx       77 b- defN 20-Apr-16 12:00 antimatter/requirements/langchain-huggingface.txt
+-rw-r--r--  2.0 unx       75 b- defN 20-Apr-16 12:00 antimatter/requirements/langchain.txt
 -rw-r--r--  2.0 unx       14 b- defN 20-Apr-16 12:00 antimatter/requirements/numpy.txt
 -rw-r--r--  2.0 unx       24 b- defN 20-Apr-16 12:00 antimatter/requirements/pandas.txt
 -rw-r--r--  2.0 unx       38 b- defN 20-Apr-16 12:00 antimatter/requirements/pyarrow.txt
 -rw-r--r--  2.0 unx       11 b- defN 20-Apr-16 12:00 antimatter/requirements/pytorch.txt
--rw-r--r--  2.0 unx      949 b- defN 20-Apr-16 12:00 antimatter/session_mixins/__init__.py
--rw-r--r--  2.0 unx     3391 b- defN 20-Apr-16 12:00 antimatter/session_mixins/capability_mixin.py
--rw-r--r--  2.0 unx     5037 b- defN 20-Apr-16 12:00 antimatter/session_mixins/capsule_mixin.py
--rw-r--r--  2.0 unx    14894 b- defN 20-Apr-16 12:00 antimatter/session_mixins/domain_mixin.py
--rw-r--r--  2.0 unx     1141 b- defN 20-Apr-16 12:00 antimatter/session_mixins/encryption_mixin.py
--rw-r--r--  2.0 unx     6208 b- defN 20-Apr-16 12:00 antimatter/session_mixins/fact_mixin.py
--rw-r--r--  2.0 unx    11843 b- defN 20-Apr-16 12:00 antimatter/session_mixins/general_mixin.py
--rw-r--r--  2.0 unx    12478 b- defN 20-Apr-16 12:00 antimatter/session_mixins/identity_provider_mixin.py
--rw-r--r--  2.0 unx     6063 b- defN 20-Apr-16 12:00 antimatter/session_mixins/policy_rule_mixin.py
--rw-r--r--  2.0 unx     6281 b- defN 20-Apr-16 12:00 antimatter/session_mixins/read_context_mixin.py
--rw-r--r--  2.0 unx     5713 b- defN 20-Apr-16 12:00 antimatter/session_mixins/root_encryption_key_mixin.py
--rw-r--r--  2.0 unx     2265 b- defN 20-Apr-16 12:00 antimatter/session_mixins/token.py
--rw-r--r--  2.0 unx     1727 b- defN 20-Apr-16 12:00 antimatter/session_mixins/verification_mixin.py
--rw-r--r--  2.0 unx     5977 b- defN 20-Apr-16 12:00 antimatter/session_mixins/write_context_mixin.py
+-rw-r--r--  2.0 unx      941 b- defN 20-Apr-16 12:00 antimatter/session_mixins/__init__.py
+-rw-r--r--  2.0 unx      319 b- defN 20-Apr-16 12:00 antimatter/session_mixins/base.py
+-rw-r--r--  2.0 unx     2810 b- defN 20-Apr-16 12:00 antimatter/session_mixins/capability_mixin.py
+-rw-r--r--  2.0 unx     4464 b- defN 20-Apr-16 12:00 antimatter/session_mixins/capsule_mixin.py
+-rw-r--r--  2.0 unx    13732 b- defN 20-Apr-16 12:00 antimatter/session_mixins/domain_mixin.py
+-rw-r--r--  2.0 unx      596 b- defN 20-Apr-16 12:00 antimatter/session_mixins/encryption_mixin.py
+-rw-r--r--  2.0 unx     5248 b- defN 20-Apr-16 12:00 antimatter/session_mixins/fact_mixin.py
+-rw-r--r--  2.0 unx    10949 b- defN 20-Apr-16 12:00 antimatter/session_mixins/general_mixin.py
+-rw-r--r--  2.0 unx    11657 b- defN 20-Apr-16 12:00 antimatter/session_mixins/identity_provider_mixin.py
+-rw-r--r--  2.0 unx     5439 b- defN 20-Apr-16 12:00 antimatter/session_mixins/policy_rule_mixin.py
+-rw-r--r--  2.0 unx     5530 b- defN 20-Apr-16 12:00 antimatter/session_mixins/read_context_mixin.py
+-rw-r--r--  2.0 unx     4805 b- defN 20-Apr-16 12:00 antimatter/session_mixins/root_encryption_key_mixin.py
+-rw-r--r--  2.0 unx     1296 b- defN 20-Apr-16 12:00 antimatter/session_mixins/starred_domain_mixin.py
+-rw-r--r--  2.0 unx     1106 b- defN 20-Apr-16 12:00 antimatter/session_mixins/verification_mixin.py
+-rw-r--r--  2.0 unx     5247 b- defN 20-Apr-16 12:00 antimatter/session_mixins/write_context_mixin.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/session_mixins/serializers/__init__.py
--rw-r--r--  2.0 unx     1202 b- defN 20-Apr-16 12:00 antimatter/session_mixins/serializers/identity_details.py
+-rw-r--r--  2.0 unx     1199 b- defN 20-Apr-16 12:00 antimatter/session_mixins/serializers/identity_details.py
 -rw-r--r--  2.0 unx       56 b- defN 20-Apr-16 12:00 antimatter/tags/__init__.py
--rw-r--r--  2.0 unx     1458 b- defN 20-Apr-16 12:00 antimatter/tags/tag.py
+-rw-r--r--  2.0 unx     1459 b- defN 20-Apr-16 12:00 antimatter/tags/tag.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/tests/__init__.py
--rw-r--r--  2.0 unx     3444 b- defN 20-Apr-16 12:00 antimatter/tests/test_capabilities.py
--rw-r--r--  2.0 unx     8051 b- defN 20-Apr-16 12:00 antimatter/tests/test_capsule.py
--rw-r--r--  2.0 unx      281 b- defN 20-Apr-16 12:00 antimatter/tests/test_cell_path.py
--rw-r--r--  2.0 unx     1815 b- defN 24-May-14 23:57 antimatter-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 23:57 antimatter-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-14 23:57 antimatter-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    28821 b- defN 24-May-14 23:57 antimatter-1.0.0.dist-info/RECORD
-284 files, 2047187 bytes uncompressed, 338767 bytes compressed:  83.5%
+-rw-r--r--  2.0 unx     4462 b- defN 20-Apr-16 12:00 antimatter/tests/test_api_key_auth.py
+-rw-r--r--  2.0 unx     9021 b- defN 20-Apr-16 12:00 antimatter/tests/test_capsule.py
+-rw-r--r--  2.0 unx      282 b- defN 20-Apr-16 12:00 antimatter/tests/test_cell_path.py
+-rw-r--r--  2.0 unx     7157 b- defN 20-Apr-16 12:00 antimatter/tests/test_converters.py
+-rw-r--r--  2.0 unx    13567 b- defN 20-Apr-16 12:00 antimatter/tests/test_google_oauth.py
+-rw-r--r--  2.0 unx      263 b- defN 20-Apr-16 12:00 antimatter/utils/__init__.py
+-rw-r--r--  2.0 unx     2324 b- defN 20-Apr-16 12:00 antimatter/utils/auth.py
+-rw-r--r--  2.0 unx     1893 b- defN 20-Apr-16 12:00 antimatter/utils/client.py
+-rw-r--r--  2.0 unx      220 b- defN 20-Apr-16 12:00 antimatter/utils/constants.py
+-rw-r--r--  2.0 unx     1031 b- defN 20-Apr-16 12:00 antimatter/utils/token.py
+-rw-r--r--  2.0 unx     2162 b- defN 24-May-23 21:30 antimatter-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-23 21:30 antimatter-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-23 21:30 antimatter-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    12909 b- defN 24-May-23 21:30 antimatter-1.1.0.dist-info/RECORD
+141 files, 361934 bytes uncompressed, 93420 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
 Filename: antimatter/__init__.py
 Comment: 
 
 Filename: antimatter/capsule.py
 Comment: 
 
-Filename: antimatter/cell_path.py
+Filename: antimatter/cell_utils.py
 Comment: 
 
 Filename: antimatter/extra_helper.py
 Comment: 
 
 Filename: antimatter/session.py
 Comment: 
@@ -27,549 +27,87 @@
 
 Filename: antimatter/auth/config/profiles.py
 Comment: 
 
 Filename: antimatter/auth/config/tokens.py
 Comment: 
 
-Filename: antimatter/auth/google/__init__.py
+Filename: antimatter/authn/__init__.py
 Comment: 
 
-Filename: antimatter/auth/google/models.py
+Filename: antimatter/authn/apikey.py
 Comment: 
 
-Filename: antimatter/builders/__init__.py
-Comment: 
-
-Filename: antimatter/builders/capability.py
-Comment: 
-
-Filename: antimatter/builders/fact_policy.py
-Comment: 
-
-Filename: antimatter/builders/read_context.py
-Comment: 
-
-Filename: antimatter/builders/read_context_rule.py
-Comment: 
-
-Filename: antimatter/builders/root_encryption_key.py
-Comment: 
-
-Filename: antimatter/builders/settings_patch.py
-Comment: 
-
-Filename: antimatter/builders/write_context.py
-Comment: 
-
-Filename: antimatter/builders/write_context_rule.py
-Comment: 
-
-Filename: antimatter/cap_prep/__init__.py
-Comment: 
-
-Filename: antimatter/cap_prep/applicator.py
-Comment: 
-
-Filename: antimatter/cap_prep/prep.py
-Comment: 
-
-Filename: antimatter/cap_prep/tests/__init__.py
-Comment: 
-
-Filename: antimatter/cap_prep/tests/test_applicator.py
-Comment: 
-
-Filename: antimatter/cap_prep/tests/test_prep.py
-Comment: 
-
-Filename: antimatter/capabilities/__init__.py
-Comment: 
-
-Filename: antimatter/capabilities/converter.py
-Comment: 
-
-Filename: antimatter/client/__init__.py
-Comment: 
-
-Filename: antimatter/client/api_client.py
-Comment: 
-
-Filename: antimatter/client/api_response.py
-Comment: 
-
-Filename: antimatter/client/configuration.py
-Comment: 
-
-Filename: antimatter/client/exceptions.py
-Comment: 
-
-Filename: antimatter/client/rest.py
-Comment: 
-
-Filename: antimatter/client/api/__init__.py
-Comment: 
-
-Filename: antimatter/client/api/account_management_api.py
-Comment: 
-
-Filename: antimatter/client/api/authentication_api.py
-Comment: 
-
-Filename: antimatter/client/api/capsules_api.py
-Comment: 
-
-Filename: antimatter/client/api/contexts_api.py
-Comment: 
-
-Filename: antimatter/client/api/encryption_api.py
-Comment: 
-
-Filename: antimatter/client/api/general_api.py
-Comment: 
-
-Filename: antimatter/client/api/internal_api.py
-Comment: 
-
-Filename: antimatter/client/api/policy_api.py
-Comment: 
-
-Filename: antimatter/client/models/__init__.py
-Comment: 
-
-Filename: antimatter/client/models/access_log_entry.py
-Comment: 
-
-Filename: antimatter/client/models/access_log_entry_create_info.py
-Comment: 
-
-Filename: antimatter/client/models/access_log_entry_open_info.py
-Comment: 
-
-Filename: antimatter/client/models/access_log_entry_read_info.py
-Comment: 
-
-Filename: antimatter/client/models/access_log_results.py
-Comment: 
-
-Filename: antimatter/client/models/active_root_encryption_key_id.py
-Comment: 
-
-Filename: antimatter/client/models/add_capsule_log_entry_request.py
-Comment: 
-
-Filename: antimatter/client/models/add_read_context.py
-Comment: 
-
-Filename: antimatter/client/models/add_write_context.py
-Comment: 
-
-Filename: antimatter/client/models/antimatter_delegated_aws_key_info.py
-Comment: 
-
-Filename: antimatter/client/models/api_key_domain_identity_provider_details.py
-Comment: 
-
-Filename: antimatter/client/models/available_delegated_root_encryption_key_provider.py
-Comment: 
-
-Filename: antimatter/client/models/available_root_encryption_key_providers.py
-Comment: 
-
-Filename: antimatter/client/models/available_root_encryption_key_providers_providers_inner.py
-Comment: 
-
-Filename: antimatter/client/models/available_service_account_root_encryption_key_provider.py
-Comment: 
-
-Filename: antimatter/client/models/aws_service_account_key_info.py
-Comment: 
-
-Filename: antimatter/client/models/capability.py
-Comment: 
-
-Filename: antimatter/client/models/capability_definition.py
-Comment: 
-
-Filename: antimatter/client/models/capability_definition_list.py
-Comment: 
-
-Filename: antimatter/client/models/capability_list.py
-Comment: 
-
-Filename: antimatter/client/models/capability_rule.py
-Comment: 
-
-Filename: antimatter/client/models/capability_rule_match_expressions_inner.py
-Comment: 
-
-Filename: antimatter/client/models/capsule_create_response.py
-Comment: 
-
-Filename: antimatter/client/models/capsule_info.py
-Comment: 
-
-Filename: antimatter/client/models/capsule_list.py
-Comment: 
-
-Filename: antimatter/client/models/capsule_open_request.py
-Comment: 
-
-Filename: antimatter/client/models/capsule_open_response.py
-Comment: 
-
-Filename: antimatter/client/models/capsule_open_response_read_context_configuration.py
-Comment: 
-
-Filename: antimatter/client/models/capsule_seal_request.py
-Comment: 
-
-Filename: antimatter/client/models/conflict_error.py
-Comment: 
-
-Filename: antimatter/client/models/create_peer_domain.py
-Comment: 
-
-Filename: antimatter/client/models/data_tagging_hook_input.py
-Comment: 
-
-Filename: antimatter/client/models/data_tagging_hook_input_records_inner.py
-Comment: 
-
-Filename: antimatter/client/models/data_tagging_hook_input_records_inner_elements_inner.py
-Comment: 
-
-Filename: antimatter/client/models/data_tagging_hook_response.py
-Comment: 
-
-Filename: antimatter/client/models/data_tagging_hook_response_records_inner.py
-Comment: 
-
-Filename: antimatter/client/models/delete_tags.py
-Comment: 
-
-Filename: antimatter/client/models/domain.py
-Comment: 
-
-Filename: antimatter/client/models/domain_add_read_context_rule200_response.py
-Comment: 
-
-Filename: antimatter/client/models/domain_authenticate.py
-Comment: 
-
-Filename: antimatter/client/models/domain_authenticate_response.py
-Comment: 
-
-Filename: antimatter/client/models/domain_contact_issue_verify_request.py
-Comment: 
-
-Filename: antimatter/client/models/domain_control_log_entry.py
-Comment: 
-
-Filename: antimatter/client/models/domain_control_log_results.py
-Comment: 
-
-Filename: antimatter/client/models/domain_fact_list.py
-Comment: 
-
-Filename: antimatter/client/models/domain_hooks_list.py
-Comment: 
-
-Filename: antimatter/client/models/domain_hooks_list_hooks_inner.py
-Comment: 
-
-Filename: antimatter/client/models/domain_identity_api_key_principal_params.py
-Comment: 
-
-Filename: antimatter/client/models/domain_identity_email_principal_params.py
-Comment: 
-
-Filename: antimatter/client/models/domain_identity_hosted_domain_principal_params.py
-Comment: 
-
-Filename: antimatter/client/models/domain_identity_principal_details.py
-Comment: 
-
-Filename: antimatter/client/models/domain_identity_provider_details.py
-Comment: 
-
-Filename: antimatter/client/models/domain_identity_provider_info.py
-Comment: 
-
-Filename: antimatter/client/models/domain_identity_provider_list.py
-Comment: 
-
-Filename: antimatter/client/models/domain_identity_provider_principal_list.py
-Comment: 
-
-Filename: antimatter/client/models/domain_identity_provider_principal_params.py
-Comment: 
-
-Filename: antimatter/client/models/domain_identity_provider_principal_type.py
-Comment: 
-
-Filename: antimatter/client/models/domain_identity_provider_type.py
-Comment: 
-
-Filename: antimatter/client/models/domain_insert_identity_provider_principal200_response.py
-Comment: 
-
-Filename: antimatter/client/models/domain_insert_write_context_regex_rule200_response.py
-Comment: 
-
-Filename: antimatter/client/models/domain_peer_config.py
-Comment: 
-
-Filename: antimatter/client/models/domain_peer_list.py
-Comment: 
-
-Filename: antimatter/client/models/domain_peer_list_peers_inner.py
-Comment: 
-
-Filename: antimatter/client/models/domain_policy.py
-Comment: 
-
-Filename: antimatter/client/models/domain_policy_rule.py
-Comment: 
-
-Filename: antimatter/client/models/domain_private_info.py
-Comment: 
-
-Filename: antimatter/client/models/domain_public_info.py
-Comment: 
-
-Filename: antimatter/client/models/domain_resource_summary.py
-Comment: 
-
-Filename: antimatter/client/models/domain_resource_summary_schema_inner.py
-Comment: 
-
-Filename: antimatter/client/models/domain_settings.py
-Comment: 
-
-Filename: antimatter/client/models/domain_settings_disaster_recovery.py
-Comment: 
-
-Filename: antimatter/client/models/domain_settings_patch.py
-Comment: 
-
-Filename: antimatter/client/models/domain_status.py
-Comment: 
-
-Filename: antimatter/client/models/domain_status_notifications_inner.py
-Comment: 
-
-Filename: antimatter/client/models/domain_tag_info_results.py
-Comment: 
-
-Filename: antimatter/client/models/error.py
-Comment: 
-
-Filename: antimatter/client/models/fact.py
-Comment: 
-
-Filename: antimatter/client/models/fact_list.py
-Comment: 
-
-Filename: antimatter/client/models/fact_policy_rules_inner.py
-Comment: 
-
-Filename: antimatter/client/models/fact_policy_rules_inner_arguments_inner.py
-Comment: 
-
-Filename: antimatter/client/models/fact_type_definition.py
-Comment: 
-
-Filename: antimatter/client/models/gcp_service_account_key_info.py
-Comment: 
-
-Filename: antimatter/client/models/google_o_auth_domain_identity_provider_details.py
-Comment: 
-
-Filename: antimatter/client/models/hook_invocation.py
-Comment: 
-
-Filename: antimatter/client/models/invalid_request_error.py
-Comment: 
-
-Filename: antimatter/client/models/json_patch_request_add.py
-Comment: 
-
-Filename: antimatter/client/models/json_patch_request_add_value.py
-Comment: 
-
-Filename: antimatter/client/models/json_patch_request_copy.py
-Comment: 
-
-Filename: antimatter/client/models/json_patch_request_move.py
-Comment: 
-
-Filename: antimatter/client/models/json_patch_request_remove.py
-Comment: 
-
-Filename: antimatter/client/models/json_patch_request_replace.py
-Comment: 
-
-Filename: antimatter/client/models/json_patch_request_replace_value.py
-Comment: 
-
-Filename: antimatter/client/models/json_patch_request_tst.py
-Comment: 
-
-Filename: antimatter/client/models/json_patch_request_tst_value.py
-Comment: 
-
-Filename: antimatter/client/models/key_infos.py
-Comment: 
-
-Filename: antimatter/client/models/key_infos_key_information.py
-Comment: 
-
-Filename: antimatter/client/models/new_access_log_entry.py
-Comment: 
-
-Filename: antimatter/client/models/new_access_log_entry_read_info.py
-Comment: 
-
-Filename: antimatter/client/models/new_capability_definition.py
-Comment: 
-
-Filename: antimatter/client/models/new_domain.py
-Comment: 
-
-Filename: antimatter/client/models/new_domain_policy_rule.py
-Comment: 
-
-Filename: antimatter/client/models/new_domain_response.py
-Comment: 
-
-Filename: antimatter/client/models/new_fact.py
-Comment: 
-
-Filename: antimatter/client/models/new_fact_type_definition.py
-Comment: 
-
-Filename: antimatter/client/models/new_fact_type_definition_arguments_inner.py
-Comment: 
-
-Filename: antimatter/client/models/new_read_context_config_rule.py
-Comment: 
-
-Filename: antimatter/client/models/patch_request_inner.py
-Comment: 
-
-Filename: antimatter/client/models/policy_rule_operation.py
-Comment: 
-
-Filename: antimatter/client/models/policy_rule_result.py
-Comment: 
-
-Filename: antimatter/client/models/principal_info.py
-Comment: 
-
-Filename: antimatter/client/models/principal_summary.py
-Comment: 
-
-Filename: antimatter/client/models/read_context_config_rule.py
-Comment: 
-
-Filename: antimatter/client/models/read_context_details.py
-Comment: 
-
-Filename: antimatter/client/models/read_context_list.py
-Comment: 
-
-Filename: antimatter/client/models/read_context_parameter.py
-Comment: 
-
-Filename: antimatter/client/models/read_context_required_hook.py
-Comment: 
-
-Filename: antimatter/client/models/read_context_rule_facts_inner.py
-Comment: 
-
-Filename: antimatter/client/models/read_context_rule_facts_inner_arguments_inner.py
+Filename: antimatter/authn/base.py
 Comment: 
 
-Filename: antimatter/client/models/read_context_rule_match_expressions_inner.py
+Filename: antimatter/authn/google_oauth.py
 Comment: 
 
-Filename: antimatter/client/models/read_context_short_details.py
+Filename: antimatter/authn/oauth_domain.py
 Comment: 
 
-Filename: antimatter/client/models/resource_exhausted_error.py
+Filename: antimatter/authn/static_oauth.py
 Comment: 
 
-Filename: antimatter/client/models/resource_not_found_error.py
+Filename: antimatter/authn/unauth.py
 Comment: 
 
-Filename: antimatter/client/models/root_encryption_key_id_response.py
+Filename: antimatter/authz/__init__.py
 Comment: 
 
-Filename: antimatter/client/models/root_encryption_key_item.py
+Filename: antimatter/authz/base.py
 Comment: 
 
-Filename: antimatter/client/models/root_encryption_key_test_response.py
+Filename: antimatter/authz/token.py
 Comment: 
 
-Filename: antimatter/client/models/rotate_key_encryption_key_response.py
-Comment: 
-
-Filename: antimatter/client/models/starred_domain_list.py
-Comment: 
-
-Filename: antimatter/client/models/tag.py
-Comment: 
-
-Filename: antimatter/client/models/tag_meta.py
-Comment: 
-
-Filename: antimatter/client/models/tag_set.py
+Filename: antimatter/builders/__init__.py
 Comment: 
 
-Filename: antimatter/client/models/tag_set_span_tags_inner.py
+Filename: antimatter/builders/capability.py
 Comment: 
 
-Filename: antimatter/client/models/tag_summary.py
+Filename: antimatter/builders/fact_policy.py
 Comment: 
 
-Filename: antimatter/client/models/tag_summary_elided_tags_inner.py
+Filename: antimatter/builders/read_context.py
 Comment: 
 
-Filename: antimatter/client/models/tag_summary_unique_tags_inner.py
+Filename: antimatter/builders/read_context_rule.py
 Comment: 
 
-Filename: antimatter/client/models/tag_type_field.py
+Filename: antimatter/builders/root_encryption_key.py
 Comment: 
 
-Filename: antimatter/client/models/unauthorized_error.py
+Filename: antimatter/builders/settings_patch.py
 Comment: 
 
-Filename: antimatter/client/models/upsert_span_tags_request.py
+Filename: antimatter/builders/write_context.py
 Comment: 
 
-Filename: antimatter/client/models/verify_contact_response.py
+Filename: antimatter/builders/write_context_rule.py
 Comment: 
 
-Filename: antimatter/client/models/write_context_config_info.py
+Filename: antimatter/cap_prep/__init__.py
 Comment: 
 
-Filename: antimatter/client/models/write_context_config_info_required_hooks_inner.py
+Filename: antimatter/cap_prep/applicator.py
 Comment: 
 
-Filename: antimatter/client/models/write_context_details.py
+Filename: antimatter/cap_prep/prep.py
 Comment: 
 
-Filename: antimatter/client/models/write_context_list.py
+Filename: antimatter/cap_prep/tests/__init__.py
 Comment: 
 
-Filename: antimatter/client/models/write_context_regex_rule.py
+Filename: antimatter/cap_prep/tests/test_applicator.py
 Comment: 
 
-Filename: antimatter/client/models/write_context_regex_tag.py
+Filename: antimatter/cap_prep/tests/test_prep.py
 Comment: 
 
 Filename: antimatter/constants/__init__.py
 Comment: 
 
 Filename: antimatter/constants/capability.py
 Comment: 
@@ -591,14 +129,23 @@
 
 Filename: antimatter/constants/settings_patch.py
 Comment: 
 
 Filename: antimatter/constants/write_context.py
 Comment: 
 
+Filename: antimatter/converters/__init__.py
+Comment: 
+
+Filename: antimatter/converters/capability.py
+Comment: 
+
+Filename: antimatter/converters/tags.py
+Comment: 
+
 Filename: antimatter/datatype/__init__.py
 Comment: 
 
 Filename: antimatter/datatype/datatypes.py
 Comment: 
 
 Filename: antimatter/datatype/infer.py
@@ -771,14 +318,17 @@
 
 Filename: antimatter/requirements/pytorch.txt
 Comment: 
 
 Filename: antimatter/session_mixins/__init__.py
 Comment: 
 
+Filename: antimatter/session_mixins/base.py
+Comment: 
+
 Filename: antimatter/session_mixins/capability_mixin.py
 Comment: 
 
 Filename: antimatter/session_mixins/capsule_mixin.py
 Comment: 
 
 Filename: antimatter/session_mixins/domain_mixin.py
@@ -801,15 +351,15 @@
 
 Filename: antimatter/session_mixins/read_context_mixin.py
 Comment: 
 
 Filename: antimatter/session_mixins/root_encryption_key_mixin.py
 Comment: 
 
-Filename: antimatter/session_mixins/token.py
+Filename: antimatter/session_mixins/starred_domain_mixin.py
 Comment: 
 
 Filename: antimatter/session_mixins/verification_mixin.py
 Comment: 
 
 Filename: antimatter/session_mixins/write_context_mixin.py
 Comment: 
@@ -825,29 +375,50 @@
 
 Filename: antimatter/tags/tag.py
 Comment: 
 
 Filename: antimatter/tests/__init__.py
 Comment: 
 
-Filename: antimatter/tests/test_capabilities.py
+Filename: antimatter/tests/test_api_key_auth.py
 Comment: 
 
 Filename: antimatter/tests/test_capsule.py
 Comment: 
 
 Filename: antimatter/tests/test_cell_path.py
 Comment: 
 
-Filename: antimatter-1.0.0.dist-info/METADATA
+Filename: antimatter/tests/test_converters.py
+Comment: 
+
+Filename: antimatter/tests/test_google_oauth.py
+Comment: 
+
+Filename: antimatter/utils/__init__.py
+Comment: 
+
+Filename: antimatter/utils/auth.py
+Comment: 
+
+Filename: antimatter/utils/client.py
+Comment: 
+
+Filename: antimatter/utils/constants.py
+Comment: 
+
+Filename: antimatter/utils/token.py
+Comment: 
+
+Filename: antimatter-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: antimatter-1.0.0.dist-info/WHEEL
+Filename: antimatter-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: antimatter-1.0.0.dist-info/top_level.txt
+Filename: antimatter-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: antimatter-1.0.0.dist-info/RECORD
+Filename: antimatter-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## antimatter/__init__.py

```diff
@@ -1,6 +1,8 @@
 from antimatter.builders import *
 from antimatter.tags import CapsuleTag, ColumnTag, SpanTag, TagType
-from antimatter.cell_path import cell_path
+from antimatter.cell_utils import cell_path
 from antimatter.datatype.datatypes import Datatype
 from antimatter.fieldtype.fieldtypes import FieldType
 from antimatter.session import Session, new_domain, with_domain, load_domain
+from antimatter.authn import *
+from antimatter.authz import *
```

## antimatter/capsule.py

```diff
@@ -1,85 +1,113 @@
-import json
 from dataclasses import dataclass
 from collections import defaultdict
 from typing import Any, Dict, List, Tuple, Union
 
 import antimatter_engine as ae
 
 import antimatter.extra_helper as extra_helper
 import antimatter.handlers as handlers
-from antimatter.cell_path import cell_path
+from antimatter.cell_utils import cell_path
 from antimatter.datatype.datatypes import Datatype
 from antimatter.extra_helper import META_TYPE_KEY
 from antimatter.fieldtype import converters
 from antimatter.tags import SpanTag, ColumnTag, CapsuleTag
-
+from antimatter.converters import TagConverter
 
 class CapsuleBindings:
-    def __init__(self, capsule_session: ae.PySessionCapsule):
+    def __init__(self, capsule_session: ae.PySessionCapsule, redact_tags: List[SpanTag] = []):
         """
         CapsuleBindings holds the capsule session for the underlying Antimatter Capsule.
-
+        
         :param capsule_session: The bundle session for the underlying Antimatter Capsule Bundle
-        :param failed: A list of capsules in the Antimatter Capsule Bundle that could not be opened.
+        :param redact_tags: The tags to redact from the data. These can be in one of the following forms:
+                - A list of unary tags, like ['tag.antimatter.io/pii/email', 'tag.antimatter.io/pii/name']
+                - A list of key-value pairs, like ["tag.antimatter.io/pii/date=24/12/2021", "tag.antimatter.io/pii/credit_card=1234"]
+                - A list of dictionaries, like [{"tag.antimatter.io/pii/email": ""}, {"tag.antimatter.io/pii/date": "24/12/2021"}]
+                - A list of dictionaries as a name/value pair, like [{"name": "tag.antimatter.io/pii/email", "value": ""}, {"name": "tag.antimatter.io/pii/date", "value": "24/12/2021"}]
+                - Any combination of the above
         """
         self._capsule_session = capsule_session
-        if capsule_session is not None:
-            self.capsule_tags, self.column_names, self.column_tags, self.redacted_data, self.data_span_tags, self.extra_info = capsule_session.read_all_with_tags([])
+        self._refresh_data(redact_tags)
+    
+    def _refresh_data(self, redact_tags: List[SpanTag] = []):
+        self.redact_tags = [
+            ae.PyTag(tag.name, tag.tag_type.value, tag.tag_value, "manual", (0, 0, 0)) for tag in redact_tags
+        ]
+        if self._capsule_session is not None:
+            self.capsule_tags, self.column_names, self.column_tags, \
+                self.redacted_data, self.data_span_tags, \
+                    self.extra_info = self._capsule_session.read_all_with_tags(self.redact_tags)
 
     def read_extras(self) -> List[str]:
         """
         Get the extras field stored in the capsule.
 
         :return: The extras string.
         """
         return self.extra_info
 
-    def read_all(self) -> Tuple[List[str], List[List[bytes]], str]:
+    # TODO: turn this into capabilities style string.
+    def read_all(self, redact_tags: List[SpanTag] = []) -> Tuple[List[str], List[List[bytes]], str]:
         """
         Get the column definitions, redacted data and extras from the underlying capsule.
 
+        :param redact_tags: The tags to redact from the data. These can be in one of the following forms:
+                - A list of unary tags, like ['tag.antimatter.io/pii/email', 'tag.antimatter.io/pii/name']
+                - A list of key-value pairs, like ["tag.antimatter.io/pii/date=24/12/2021", "tag.antimatter.io/pii/credit_card=1234"]
+                - A list of dictionaries, like [{"tag.antimatter.io/pii/email": ""}, {"tag.antimatter.io/pii/date": "24/12/2021"}]
+                - A list of dictionaries as a name/value pair, like [{"name": "tag.antimatter.io/pii/email", "value": ""}, {"name": "tag.antimatter.io/pii/date", "value": "24/12/2021"}]
+                - Any combination of the above
         :return: The column definition list, a 2D list of list of string containing the redacted data, and the extras
                  string.
         """
+        if self.redact_tags != redact_tags:
+            self._refresh_data(redact_tags)
         return self.column_names, self.redacted_data, self.extra_info
 
-    def read_all_with_tags(self) -> Tuple[
+    def read_all_with_tags(self, redact_tags: List[SpanTag] = []) -> Tuple[
             List[ae.PyTag], 
             List[str], 
             List[List[ae.PyTag]], 
             List[List[List[bytes]]], 
             List[List[List[ae.PySpanTag]]], 
             str,
         ]:
         """
         Get the tag information (capsule, column, etc.), column definitions, redacted 
         data and extras from the underlying capsule. This method is meant to provide
         insight into what is being tagged along with the corresponding tag that was
         applied.
 
+        :param redact_tags: The tags to redact from the data. These can be in one of the following forms:
+                - A list of unary tags, like ['tag.antimatter.io/pii/email', 'tag.antimatter.io/pii/name']
+                - A list of key-value pairs, like ["tag.antimatter.io/pii/date=24/12/2021", "tag.antimatter.io/pii/credit_card=1234"]
+                - A list of dictionaries, like [{"tag.antimatter.io/pii/email": ""}, {"tag.antimatter.io/pii/date": "24/12/2021"}]
+                - A list of dictionaries as a name/value pair, like [{"name": "tag.antimatter.io/pii/email", "value": ""}, {"name": "tag.antimatter.io/pii/date", "value": "24/12/2021"}]
+                - Any combination of the above
         :return: The list of capsule tags, column definition list, list of column tags,
                  a 2D list of list of string containing the redacted data, a list of data span 
                  tags, and the extras string.
         """
+        if self.redact_tags != redact_tags:
+            self._refresh_data(redact_tags)
         return self.capsule_tags, self.column_names, self.column_tags, self.redacted_data, self.data_span_tags, self.extra_info
 
     def capsule_ids(self) -> List[str]:
         """
         Get a list capsule IDs associated with this CapsuleBinding.
         """
         return self._capsule_session.capsule_ids()
 
     def domain_id(self) -> str:
         """
         Get the domain ID associated with the capsule.
         """
         return self._capsule_session.domain_id()
 
-
 @dataclass
 class CapsuleMeta:
     datatype_in: Datatype
     extra: Dict[str, Any]
 
 
 class Capsule:
@@ -90,38 +118,45 @@
         capsule_binding: CapsuleBindings,
     ):
         """
         Capsule holds the capsule bindings for the underlying Antimatter Capsule
         and converts it into various different supported formats.
 
         :param capsule_binding:
-        The capsule bindings for the underlying Antimatter Capsule
+            The capsule bindings for the underlying Antimatter Capsule
         """
         self._capsule = capsule_binding
 
     @property
     def capsule(self) -> CapsuleBindings:
         """
         Get the capsule binding for the underlying Antimatter Capsule.
 
         :return: The Antimatter Capsule binding.
         """
         return self._capsule
 
-    def data(self, **kwargs) -> Any:
+    def data(self, redact_tags: List[str] = [], **kwargs) -> Any:
         """
         Get the data from the underlying Antimatter Capsule using the supplied
         read parameters. This will raise an error if the capsule is sealed.
 
+        :param redact_tags: The tags to redact from the data. These can be in one of the following forms:
+                - A list of unary tags, like ['tag.antimatter.io/pii/email', 'tag.antimatter.io/pii/name']
+                - A list of key-value pairs, like ["tag.antimatter.io/pii/date=24/12/2021", "tag.antimatter.io/pii/credit_card=1234"]
+                - A list of dictionaries, like [{"tag.antimatter.io/pii/email": ""}, {"tag.antimatter.io/pii/date": "24/12/2021"}]
+                - A list of dictionaries as a name/value pair, like [{"name": "tag.antimatter.io/pii/email", "value": ""}, {"name": "tag.antimatter.io/pii/date", "value": "24/12/2021"}]
+                - Any combination of the above
         :param kwargs: The extra arguments to pass to the data handler.
         :return: The data in its default format.
         """
-        column_names, rows, extra = self._capsule.read_all()
+        redact_tags = TagConverter.convert_tags(redact_tags)
+        column_names, rows, extra = self._capsule.read_all(redact_tags)
 
-        extra = json.loads(extra)
+        extra = extra_helper.extra_dict_from_string(extra, len(rows), column_names)
         default_dt_val = extra.get(META_TYPE_KEY, Datatype.Unknown.value)
         default_dt = Datatype(default_dt_val)
 
         h = handlers.factory(default_dt)  # TODO: try/except
         e = extra_helper.extra_for_capsule(default_dt, extra, **kwargs)
         d = h.from_generic(column_names, rows, e)
         return d
@@ -133,15 +168,15 @@
 
         :param dt: The datatype to use for reading data.
         :param kwargs: The extra arguments to pass to the data handler.
         :return: The data in the specified format.
         """
         dt = Datatype(dt)
         column_names, rows, extra = self._capsule.read_all()
-        extra = json.loads(extra)
+        extra = extra_helper.extra_dict_from_string(extra, len(rows), column_names)
 
         h = handlers.factory(dt)  # TODO: try/except
         e = extra_helper.extra_for_capsule(dt, extra, **kwargs)
         d = h.from_generic(column_names, rows, e)
         return d
 
     def _iterate_columns_first(self, action, column_names, redacted_data, capsule_tags, column_tags, data_span_tags):
@@ -186,45 +221,52 @@
                         start=t.start, end=t.end, tag_type=t.tag.tag_type, tag_value="")
                 for t in data_span_tags[rowidx][colidx]
             ],
             "row": rowidx,
         }
         return item
 
-    def data_with_tags(self, column_major: bool=False, inline=False, **kwargs) -> List[List[Dict]]:
+    def data_with_tags(self, column_major: bool=False, inline=False, redact_tags: List[str] = [], **kwargs) -> List[List[Dict]]:
         """
         Get the data and related tag information from the underlying Antimatter 
         Capsule using the supplied read parameters. This will raise an error if 
         the capsule is sealed.
 
         :param column_major: The orientation to use for the return list. A value of True
                      results in data being grouped together by column versus a value
                      of False which results in data being grouped together by row.
         :param inline: The option to markup the data with SpanTag information similar
                        to applying HTML blocks.
+        :param redact_tags: The tags to redact from the data. These can be in one of the following forms:
+                - A list of unary tags, like ['tag.antimatter.io/pii/email', 'tag.antimatter.io/pii/name']
+                - A list of key-value pairs, like ["tag.antimatter.io/pii/date=24/12/2021", "tag.antimatter.io/pii/credit_card=1234"]
+                - A list of dictionaries, like [{"tag.antimatter.io/pii/email": ""}, {"tag.antimatter.io/pii/date": "24/12/2021"}]
+                - A list of dictionaries as a name/value pair, like [{"name": "tag.antimatter.io/pii/email", "value": ""}, {"name": "tag.antimatter.io/pii/date", "value": "24/12/2021"}]
+                - Any combination of the above
         :param kwargs: The extra arguments to pass to the data handler.
         :return: The list of dictionaries providing insight to the Tags that were
                  found within a data item.
         """
-        capsule_tags, column_names, column_tags, redacted_data, data_span_tags, extra_info = \
-            self._capsule.read_all_with_tags()
+        redact_tags = TagConverter.convert_tags(redact_tags)
+        capsule_tags, column_names, column_tags, rows, data_span_tags, extra = \
+            self._capsule.read_all_with_tags(redact_tags)
         
-        extra_info = json.loads(extra_info)
+        extra = extra_helper.extra_dict_from_string(extra, len(rows), column_names)
 
         if not column_major:  
             iterate_func = self._iterate_rows_first
         else:
             iterate_func = self._iterate_columns_first
 
         action = lambda cname, colidx, row, rowidx, capsule_tags, column_tags, data_span_tags: \
-            self._process_data_item(cname, colidx, row, rowidx, capsule_tags, column_tags, data_span_tags, extra_info)
+            self._process_data_item(cname, colidx, row, rowidx, capsule_tags, column_tags, data_span_tags, extra)
 
         rv = list(
             iterate_func(
-                action, column_names, redacted_data, capsule_tags, column_tags, data_span_tags
+                action, column_names, rows, capsule_tags, column_tags, data_span_tags
             )
         )
 
         if inline:
             for group in rv:
                 for item in group:
                     if item["span_tags"]:
```

## antimatter/extra_helper.py

```diff
@@ -1,18 +1,59 @@
-from typing import Any, Dict, Optional
+import json
+from typing import Any, Dict, List, Optional
 
 from antimatter.datatype.datatypes import Datatype
 from antimatter.fieldtype.fieldtypes import FieldType
 
 META_TYPE_KEY = "_metadtype"
 COL_TYPE_KEY = "_coltype"
 DTYPE_KEY = "_dtype"
 
 ALL_META_KEYS = [META_TYPE_KEY, COL_TYPE_KEY, DTYPE_KEY]
 
+DEFAULT_COL_NAME = "content"
+
+
+def extra_dict_from_string(
+    serialized_extra: Optional[str],
+    row_cnt: int = -1,
+    col_names: List[str] = None,
+) -> Dict[str, Any]:
+    """
+    Parses an 'extra' dictionary from a string. The string, if present, is
+    expected to be a serialized JSON format dictionary.
+
+    If 'extra' is empty or None, a default extra dict will be returned based on
+    the row count and column names, following these rules for determining the
+    default type when the 'extra' dictionary is not supplied:
+    1. If it can be determined that the data is a scalar value by virtue of only
+    one row and column of data existing with the default 'content' column name,
+    the default type will be set as a Scalar value.
+    2. Otherwise, if only one row exists, the default type will be set as a Dict.
+    3. In all other cases, the default type will be set as a DictList.
+
+    :param serialized_extra: The serialized 'extra' dictionary
+    :param row_cnt: The number of rows in the data set
+    :param col_names: The names of the columns in the data set
+    :return: A parsed 'extra' dictionary
+    """
+    if col_names is None:
+        col_names = []
+    if not serialized_extra:
+        if row_cnt == 1:
+            if len(col_names) == 1 and col_names[0] == DEFAULT_COL_NAME:
+                top_lvl_type = Datatype.Scalar.value
+            else:
+                top_lvl_type = Datatype.Dict.value
+        else:
+            top_lvl_type = Datatype.DictList.value
+        return {top_lvl_type: {}, COL_TYPE_KEY: {}, META_TYPE_KEY: top_lvl_type}
+    else:
+        return json.loads(serialized_extra)
+
 
 def extra_for_session(
     dt: Datatype,
     from_capsule: Dict[str, Any],
     session_extra: Optional[Dict[str, Any]] = None,
 ) -> Dict[str, Any]:
     """
@@ -82,10 +123,10 @@
 
 def without_meta(extra: Optional[Dict[str, Any]]) -> Optional[Dict[str, Any]]:
     """
     Helper function to strip special metadata keys from the provided 'extra'
     dictionary. A new copy of the dictionary is made and returned.
 
     :param extra: the 'extra' dict to strip special metadata from
-    :return: the 'extra' dict wtih special metadata stripped
+    :return: the 'extra' dict with special metadata stripped
     """
     return {k: v for k, v in extra.items() if k not in ALL_META_KEYS}
```

## antimatter/session.py

```diff
@@ -1,87 +1,100 @@
 import json
 import os
 import sys
 from dataclasses import dataclass
-from typing import Any, Callable, List, Optional, Union, Dict
+from typing import Any, Callable, Dict, List, Optional, Union
 from urllib.parse import quote_plus, urlparse
 
-import antimatter_engine as am
-
-from antimatter.auth.config.auth_config import AuthConfig
-from antimatter.filetype.extract import extract_from_file
-from antimatter.filetype.infer import infer_filetype
-
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 import antimatter.handlers as handlers
+from antimatter.auth.config.auth_config import AuthConfig
+from antimatter.authn import (ApiKeyAuthentication, Authentication, GoogleOAuthAuthentication,
+                              OAuthDomainAuthentication, StaticOAuthAuthentication, Unauthenticated)
+from antimatter.authz import TokenAuthorization
 from antimatter.cap_prep.prep import Preparer
-from antimatter.tags import ColumnTag, SpanTag
 from antimatter.capsule import Capsule, CapsuleBindings
-from antimatter.client import ApiClient, Configuration, GeneralApi
 from antimatter.datatype.datatypes import Datatype
 from antimatter.datatype.infer import infer_datatype
-from antimatter.errors import errors
+from antimatter import errors
 from antimatter.extra_helper import extra_for_session
-from antimatter.session_mixins import *
-
-# #version
-API_TARGET_VERSION = "v1"
+from antimatter.filetype.extract import extract_from_file
+from antimatter.filetype.infer import infer_filetype
+from antimatter.session_mixins import (
+    CapabilityMixin, CapsuleMixin, DomainMixin, EncryptionMixin, FactMixin,
+    GeneralMixin, IdentityProviderMixin, PolicyRuleMixin, ReadContextMixin,
+    RootEncryptionKeyMixin, StarredDomainMixin, VerificationMixin, WriteContextMixin
+)
+from antimatter.tags import ColumnTag, SpanTag
 
 
 def new_domain(
     email: str,
+    provider: str = None,
     display_name: Optional[str] = None,
     config_path: Optional[str] = None,
     add_to_config: bool = True,
     make_active: bool = False,
 ) -> "Session":
     """
     Create a new domain with the provided email as the admin contact. A
     verification email will be sent to that email. Verification must be completed
     before the Antimatter API can be interacted with.
+    If the provider is 'google', the session will be authenticated with a Google
+    OAuth token. That domain will be added to the starred domains as well.
 
     :param email: The admin contact email used for email verification
     :param display_name: The display name for the new domain
     :param config_path: The path to the domain profile config file; default is ~/.antimatter/config
     :param add_to_config: Whether to add the new domain to the config file; default is True
     :param make_active: Whether to make the new domain the active profile in the config file; default is False
+    :param provider: The provider to use for authentication; default is None
     :return: A Session holding the newly created domain_id and api_key
     """
-    host = os.getenv("ANTIMATTER_API_URL", "https://api.antimatter.io")
-    client = GeneralApi(
-        api_client=ApiClient(
-            configuration=Configuration(
-                host=f"{host}/{API_TARGET_VERSION}",
-            )
-        )
-    )
-    dm = client.domain_add_new(openapi_client.NewDomain(admin_email=email, display_name=display_name))
-
     # Try to create the Session before potentially adding to the config file - if creating
     # the Session produces an erroneous result, we don't want to add it to the config
-    sess = Session(domain=dm.id, api_key=dm.api_key, email=email)
-
-    if add_to_config or make_active:
-        auth_conf = AuthConfig.from_file(config_path)
-        try:
-            auth_conf.add_profile(
-                domain_id=dm.id,
-                api_key=dm.api_key,
-                name=display_name,
-                mark_active=make_active,
-                write_to_file=True,
-            )
-        except Exception as e:
-            # Catch any failures as we don't want the caller to lose the domain ID and API key
-            # if saving to a config file goes wrong
-            print(f"error saving profile to config file: {e}", file=sys.stderr)
+    authn = None
+    auth_conf = AuthConfig.from_file(config_path)
+    if provider == 'google':
+        authn = GoogleOAuthAuthentication()
+        session = Session(authn)
+        session.new_domain(email, reauthenticate=True, display_name=display_name)
+        if add_to_config or make_active:
+            try:
+                auth_conf.add_profile(
+                    domain_id=session.domain_id,
+                    token=authn.get_config_token(),
+                    name=display_name,
+                    mark_active=make_active,
+                    write_to_file=True,
+                )
+            except Exception as e:
+                # Catch any failures as we don't want the caller to lose the domain ID and API key
+                # if saving to a config file goes wrong
+                print(f"error saving profile to config file: {e}", file=sys.stderr)
+    else:
+        authn = Unauthenticated()
+        session = Session(authn)
+        dm = session.new_domain(email, display_name=display_name, reauthenticate=True)
+        if add_to_config or make_active:
+            try:
+                auth_conf.add_profile(
+                    domain_id=session.domain_id,
+                    api_key=session.api_key,
+                    name=display_name,
+                    mark_active=make_active,
+                    write_to_file=True,
+                )
+            except Exception as e:
+                # Catch any failures as we don't want the caller to lose the domain ID and API key
+                # if saving to a config file goes wrong
+                print(f"error saving profile to config file: {e}", file=sys.stderr)
 
     # Finally, return the Session
-    return sess
-
+    return session
 
 def with_domain(domain_id: str, api_key: str) -> "Session":
     """
     Create a session using an existing domain ID and API key.
 
     :param domain_id: The domain ID
     :param api_key: The API key for the domain
@@ -89,26 +102,29 @@
     """
     return load_domain(domain_id=domain_id, api_key=api_key)
 
 
 def load_domain(
     domain_id: Optional[str] = None,
     api_key: Optional[str] = None,
+    provider: Optional[str] = None,
     display_name: Optional[str] = None,
     config_path: Optional[str] = None,
     add_to_config: bool = False,
     make_active: bool = False,
 ) -> "Session":
     """
     Load an existing domain. There are several different ways to specify the domain
     credentials to use, from highest to lowest priority.
 
     1. Using display name. If this is present, it will attempt to load a profile
     from the config file with this name.
     2. Using domain_id and api_key as the credentials.
+    3. Using domain_id and a provider. If this is present, it will attempt to load a profile
+    using a oauth provider.
     3. Using only domain_id. If this is present, it will attempt to load a profile
     from the config file that matches this domain ID.
 
     If domain_id is not provided, this will check the ANTIMATTER_DOMAIN_ID env var
     for a domain ID.
 
     If api_key is not provided, this will check the ANTIMATTER_API_KEY env var for
@@ -133,72 +149,91 @@
     """
     if not domain_id:
         domain_id = os.getenv("ANTIMATTER_DOMAIN_ID", None)
     if not api_key:
         api_key = os.getenv("ANTIMATTER_API_KEY", None)
     if not config_path:
         config_path = os.getenv("ANTIMATTER_CONFIG_PATH", None)
+    if not provider:
+        provider = os.getenv("ANTIMATTER_OAUTH_PROVIDER", None)
 
-    # If a domain and API key are available, and no display name was specified, and no flags
+    # If a domain and API key or provider are available, and no display name was specified, and no flags
     # have been set to save to the config file, skip loading the auth config profiles
     # because we won't use them
-    if not display_name and domain_id and api_key and not add_to_config and not make_active:
+    if not display_name and domain_id and (api_key or provider) and not add_to_config and not make_active:
         auth_conf = AuthConfig()
     else:
         auth_conf = AuthConfig.from_file(config_path)
 
     name = None
     from_conf = False
+    token = None
 
     # If a display name is specified, load that profile
     if display_name:
         pconf = auth_conf.get_profile(name=display_name)
         if pconf is None:
             raise errors.SessionLoadError(f"could not find profile {display_name} in profile config")
         name = pconf.name
         domain_id = pconf.domain_id
         api_key = pconf.api_key
         from_conf = True
+        token = pconf.token
     # If a domain ID is specified, but not an API key, load the profile with that domain ID
-    elif domain_id and not api_key:
+    elif domain_id and not (api_key or provider):
         pconf = auth_conf.get_profile(domain_id=domain_id)
         if pconf is None:
             raise errors.SessionLoadError(f"could not find profile with domain ID {domain_id} in profile config")
         name = pconf.name
         api_key = pconf.api_key
         from_conf = True
+        token = pconf.token
     # If no display name or domain ID were specified, load the active profile from the auth config
     # We deliberately aren't confirming the API key is unset here, due in part to the issue where the
     # Session sets the env var
     elif not domain_id:
         pconf = auth_conf.get_profile()
         if pconf is None:
             raise errors.SessionLoadError("no active profile found")
         name = pconf.name
         domain_id = pconf.domain_id
         api_key = pconf.api_key
         from_conf = True
+        token = pconf.token
 
-    # If we get to this point without a domain ID and API key, we somehow failed to load the domain
-    if not domain_id or not api_key:
-        raise errors.SessionLoadError("failed to load domain - no domain ID or API key found")
+    # If we get to this point without a domain ID and API key or token, we somehow failed to load the domain
+    if not domain_id:
+        raise errors.SessionLoadError("failed to load domain - no domain ID")
+    if not (api_key or token):
+        raise errors.SessionLoadError("failed to load domain - no API key or oauth token found")
 
     # Try to initialize the Session before potentially adding to the config file - if initializing
     # the Session produces an erroneous result, we don't want to add it to the config
-    sess = Session(domain=domain_id, api_key=api_key)
+    if api_key:
+        authn = ApiKeyAuthentication(
+            domain_id=domain_id,
+            api_key=api_key,
+        )
+    elif token:
+        authn = OAuthDomainAuthentication(
+            domain_id=domain_id,
+            oauth_authentication=GoogleOAuthAuthentication(token),
+        )
+    sess = Session(authn)
 
     # If the flag is set to add to the auth config, and the profile didn't already come from the
     # auth config, then write it to the config, marking as active if that flag is also set
     if (add_to_config or make_active) and not from_conf:
         auth_conf.add_profile(
             domain_id=domain_id,
             api_key=api_key,
             name=name,
             mark_active=make_active,
             write_to_file=True,
+            token=token,
         )
 
     # Finally, return the session
     return sess
 
 
 @dataclass
@@ -229,121 +264,140 @@
     def save(self, filename: str):
         """
         Save the capsule to a file
         """
         with open(filename, "wb") as f:
             f.write(self.raw)
 
-
 class Session(
     CapabilityMixin, CapsuleMixin, DomainMixin, EncryptionMixin,
     FactMixin, GeneralMixin, IdentityProviderMixin, PolicyRuleMixin,
-    ReadContextMixin, WriteContextMixin, VerificationMixin, RootEncryptionKeyMixin
+    ReadContextMixin, WriteContextMixin, VerificationMixin, RootEncryptionKeyMixin,
+    StarredDomainMixin
 ):
     """
     The Session establishes auth and the domain you are working with, providing
     both a standard instantiation or a context manager in which a Capsule and
     its underlying data can be interacted with.
     """
+    def __init__(self, authn: Authentication):
+        authz = TokenAuthorization(authn)
+        self.authz = authz
+        self._act_for_domain = None
 
-    def __init__(self, domain: str, api_key: str, email: Optional[str] = None):
-        self._domain = domain
-        self._api_key = api_key
-        self._email = email
-        os.environ['ANTIMATTER_API_KEY'] = api_key
-        self._try_init_client(default_values_on_failure=True)
         super().__init__(
-            domain=domain,
-            api_key=api_key,
-            client_func=self._get_client,
-            session=self._session,
-            email=self._email,
+            authz=self.authz,
         )
 
     @property
     def domain_id(self):
-        """
-        Return the current domain ID
-        """
-        return self._domain
+        return self._act_for_domain if self._act_for_domain is not None else self.authz.auth_client.get_domain_id()
 
-    @property
-    def api_key(self):
+    @classmethod
+    def from_api_key(cls, domain_id: str, api_key: str) -> "Session":
         """
-        Return the api key in use by this session
-        """
-        return self._api_key
-
-    def __enter__(self):
-        # TODO: handle any resources/auth; call python rust wrapper to create a rust session
-        return self
+        Create a new session with the provided domain ID and API key.
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        # TODO: close any resources/auth; call python rust wrapper to close the rust session
-        return
+        :param domain_id: The domain ID
+        :param api_key: The API key for the domain
+
+        :return: A Session holding the domain_id and api_key
+        """
+        authn = ApiKeyAuthentication(domain_id, api_key)
+        return cls(authn)
+    
+    @classmethod
+    def from_google_oauth(cls, domain: str=None, identity_provider_name: str="google", reset_credentials: bool = False, token: str = None) -> "Session":
+        """
+        Create a new session authenticated with a Google OAuth token.
+        If a domain is provided, the session will be authenticated with that domain and identity provider (default: google).
+        If a token is provided, the session will be authenticated with that token. The token refresh is not handled by the session in that case.
+        Upstream services should handle the token refresh.
+        
+        :param domain: Optional domain ID to authenticate with
+        :param identity_provider_name: Optional identity provider name to authenticate with
+        :param reset_credentials: If True, any stored oauth credentials will be reset
+        :param token: An optional static OAuth token
+        :return: A Session authenticated with a Google OAuth token
+        """
+        if token:
+            authn = StaticOAuthAuthentication(token)
+        else:
+            authn = GoogleOAuthAuthentication(reset_credentials=reset_credentials)
+        if domain:
+            authn = OAuthDomainAuthentication(domain, identity_provider_name=identity_provider_name, oauth_authentication=authn)
+        return cls(authn)
 
-    def _get_client(self) -> ApiClient:
-        return self._client
+    @property
+    def api_key(self):
+        if not isinstance(self.authz.auth_client, ApiKeyAuthentication):
+            raise ValueError("API key is not available for this session")
+        return self.authz.auth_client._api_key
 
     def config(self):
         """
         Returns the configuration of this Session
         """
         return {
-            "domain": self._domain,
-            "api_key": self._api_key,
-            "email": self._email,
+            "domain_id": self.domain_id,
+            "api_key": self.api_key,
         }
 
-    def _try_init_client(self, default_values_on_failure: bool = False) -> bool:
-        """
-        Try to initialize the client and session with the domain and API key.
-        If default_values_on_failure is True, an empty underlying session and
-        default client with no authentication will be created if the domain has
-        not yet been verified.
 
-        :param default_values_on_failure: Whether to set default client and session values on failure
-        :return: True if the client and session were authenticated
+    @property
+    def _email(self):
+        return self.authz.auth_client.get_email()
+
+    def new_domain(self, admin_email: str, reauthenticate: bool = False, display_name: str = None) -> Dict[str, Any]:
         """
-        host = os.getenv("ANTIMATTER_API_URL", "https://api.antimatter.io")
-        try:
-            self._session = am.PySession(self._domain)
-            self._client = ApiClient(
-                configuration=Configuration(
-                    host=f"{host}/{API_TARGET_VERSION}", access_token=self._api_key,
-                )
-            )
-        except Exception as e:
-            str_e = str(e).lower()
-            # Catch the error where the domain is still awaiting verification
-            if "code: 401" not in str_e or "domain contains no verified contacts" not in str_e:
-                if "domain auth error" in str_e:
-                    if "code: 400" in str_e and "apikey" in str_e and "failed to identify the token" in str_e:
-                        raise errors.SessionError(
-                            f"domain auth error: failed to identify the API key '{self._api_key}', please check format",
-                        ) from None
-                    elif "code: 404" in str_e and "antimatter domain" in str_e and "does not exist" in str_e:
-                        raise errors.SessionError(f"domain auth error: domain '{self._domain}' does not exist") from None
-                    elif "code: 404" in str_e and "page not found" in str_e:
-                        raise errors.SessionError(
-                            f"domain auth error: failed to identify domain '{self._domain}', please check format",
-                        ) from None
-                    elif "code: 400" in str_e and "apikey" in str_e and "invalid" in str_e:
-                        raise errors.SessionError("domain auth error: invalid domain or API key provided") from None
-                    else:
-                        raise
-                else:
-                    raise
-            if default_values_on_failure:
-                # Set up a default empty session and client without auth
-                self._session = None
-                self._client = ApiClient(configuration=Configuration(host=f"{host}/{API_TARGET_VERSION}"))
-            return False
+        Create a new domain with the provided email as the admin contact. A
+        verification email will be sent to that email. Verification must be completed
+        before the Antimatter API can be interacted with.
+
+        :param admin_email: The email address of the domain administrator
+        :param reauthenticate: If True, the current session will be reauthenticated with the new domain
+        :param display_name: The display name for the domain
+        :return: The domain metadata
+        """
+        dm = openapi_client.GeneralApi(self.authz.get_client()).domain_add_new(
+            openapi_client.NewDomain(admin_email=admin_email, displayName=display_name)
+        )
+        if self.authz.auth_client.get_token_scope() == "google_oauth_token":
+            self.add_starred_domain(dm.id)
 
-        return True
+        if reauthenticate:
+            if isinstance(self.authz.auth_client, ApiKeyAuthentication) or isinstance(self.authz.auth_client, Unauthenticated):
+                self.authz = TokenAuthorization(ApiKeyAuthentication(dm.id, dm.api_key))
+            elif isinstance(self.authz.auth_client, GoogleOAuthAuthentication) or isinstance(self.authz.auth_client, StaticOAuthAuthentication):
+                self.authz = TokenAuthorization(OAuthDomainAuthentication(dm.id, oauth_authentication=self.authz.auth_client))
+
+        return dm.model_dump()
+
+    def with_domain(self, domain_id: str=None, nickname: str=None, alias: str = None) -> None:
+        """
+        Use a child domain for the current session.
+        Uses the parent's authz to authenticate and authorize all requests.
+        Obtains the child domain either by domain ID or nickname or alias.
+
+        :param domain_id: The domain ID of the child domain
+        :param nickname: The nickname of the child domain
+        :param alias: The alias of the child domain
+        """
+        if not domain_id and not nickname and not alias:
+            raise ValueError("specify a 'domain_id' or 'nickname' when using a child domain")
+
+        if domain_id == "" or domain_id is None:
+            domain_id = self.get_peer(nickname=nickname, alias=alias)
+            if not domain_id:
+                raise ValueError(f"child domain with nickname '{nickname}' or alias '{alias}' not found")
+        self._act_for_domain = domain_id
+
+    @property
+    def session(self):
+        return self.authz.get_session()
 
     def load_capsule(
         self,
         path: Optional[str] = None,
         data: Optional[Union[bytes, EncapsulateResponse]] = None,
         read_context: str = None,
         read_params: Dict[str, str] = {},
@@ -358,29 +412,25 @@
         data is data for saving to an Antimatter Capsule, `as_datatype` will
         specify the default format for the data when loaded from the blob.
 
         :param path: The location of the Capsule as a local or remote path.
         :param data: The data to load into an Antimatter Capsule.
         :param read_context: The name of the role policy to use for reading data
         """
-        if self._session is None:
-            if not self._try_init_client():
-                raise errors.SessionVerificationPendingError(ADMIN_VERIFICATION_PROMPT)
-
         if not read_context:
             raise ValueError("specify a 'read_context' when loading a capsule")
 
         if not path and not data:
             raise ValueError("specify a 'path' or the raw 'data' when loading a capsule")
 
         if data and isinstance(data, EncapsulateResponse):
             data = data.raw
 
         try:
-            capsule_session = self._session.open_capsule(read_context, read_params, path, data)
+            capsule_session = self.authz.get_session().open_capsule(read_context, read_params, path, data)
             cap = CapsuleBindings(capsule_session)
             capsule = Capsule(capsule_binding=cap)
             return capsule
         except Exception as e:
             str_e = str(e).lower()
             if "read_context" in str_e or "readcontext" in str_e:
                 raise errors.CapsuleLoadError(
@@ -423,21 +473,16 @@
                 this file will be used instead of the 'data' parameter.
         :param data_file_hint: Optional hint indicating the format of the data in the file specified by
                 'data_file_hint'. Supported formats include 'json', 'csv', 'txt', 'parquet'.
                 If not specified, data will be read as plain text.
         :return: The response containing capsule metadata and the raw blob of the
                 capsule if no path was provided.
         """
-        if self._session is None:
-            if not self._try_init_client():
-                raise errors.SessionVerificationPendingError(ADMIN_VERIFICATION_PROMPT)
-
         if data is None and path is None:
             raise ValueError("specify one of 'data' or 'path' when creating a capsule")
-
         as_datatype = Datatype(as_datatype)
         if column_tags is None:
             column_tags = []
         if span_tags is None:
             span_tags = []
         if skip_classify_on_column_names is None:
             skip_classify_on_column_names = []
@@ -465,15 +510,15 @@
 
         # if a cell path is not specified, assume it means the first cell
         for idx, st in enumerate(span_tags):
             if not st.cell_path:
                 span_tags[idx].cell_path = f"{col_names[0]}[0]"
 
         try:
-            raw, capsule_ids = self._session.encapsulate(
+            raw, capsule_ids = self.authz.get_session().encapsulate(
                 *Preparer.prepare(col_names, column_tags, skip_classify_on_column_names, raw, span_tags, extra),
                 write_context,
                 [],
                 jextra,
                 path,
                 subdomains_from,
                 create_subdomains)
@@ -490,19 +535,14 @@
                 ) from None
             raise errors.CapsuleSaveError("encapsulating data") from e
 
         if raw is not None:
             raw = bytes(raw)
         return EncapsulateResponse(capsule_ids=capsule_ids, raw=raw, load_capsule_func=self.load_capsule)
 
-    def refresh_token(self):
-        return openapi_client.AuthenticationApi(self._get_client()).domain_authenticate(
-            self._domain,
-            domain_authenticate=openapi_client.DomainAuthenticate(token=self._api_key)).token
-
     def with_new_peer_domain(
         self,
         import_alias_for_child: str,
         display_name_for_child: str,
         nicknames: Optional[List[str]] = None,
         import_alias_for_parent: Optional[str] = None,
         display_name_for_parent: Optional[str] = None,
@@ -551,40 +591,38 @@
             link_write_contexts=link_write_contexts,
             link_capabilities=link_capabilities,
             link_domain_policy=link_domain_policy,
             link_capsule_access_log=link_capsule_access_log,
             link_control_log=link_control_log,
             link_capsule_manifest=link_capsule_manifest,
         )
-        return Session(dm.get("id"), dm.get("api_key"))
+        return Session.from_api_key(dm.get("id"), dm.get("api_key"))
 
-    @exec_with_token
     def get_admin_url(
         self,
         company_name: str,
         peer_domain_id: Optional[str] = None,
         nickname: Optional[str] = None,
         alias: Optional[str] = None,
     ) -> Optional[str]:
         """
         Generate the admin URL for the domain. By default, this is the domain
         for this session. If one of the peer_domain_id, nickname, or alias are
         provided, the admin URL will be generated for the subdomain that
         matches.
-
         :param company_name: The name of the company to display
         :param peer_domain_id: The domain ID of the peer
         :param nickname: The nickname for the peer domain
         :param alias: One of the aliases of the peer domain
         :return: The admin URL
         """
         if not peer_domain_id and (nickname or alias):
             peer_domain_id = self.get_peer(nickname=nickname, alias=alias)
 
-        api_client = self._get_client()
+        api_client = self.authz.get_client()
         auth_api = openapi_client.AuthenticationApi(api_client=api_client)
 
         _id = self.domain_id
         tkn = api_client.configuration.access_token
         if peer_domain_id:
             _id = peer_domain_id
             tkn = auth_api.domain_authenticate(
```

## antimatter/auth/config/auth_config.py

```diff
@@ -1,25 +1,28 @@
+import os
 from copy import deepcopy
 from os.path import expanduser, isfile
 from pathlib import Path
 from typing import Any, Dict, List, Optional
+from pathlib import Path
 
 import yaml
 
-from antimatter.auth.config.global_identity import GlobalIdentity, OidcTokenFactory
+from antimatter.auth.config.global_identity import GlobalIdentity
+from antimatter.auth.config.tokens import OidcTokenFactory, OidcToken
 from antimatter.auth.config.profiles import Profile
 
 SUPPORTED_SCHEMA_VERSIONS = ["v1"]
 SUPPORTED_TOKEN_TYPES = ["google"]
 _SCHEMA_KEY = "schema"
 _PROFILES_KEY = "profiles"
 _ACTIVE_PROFILE_KEY = "active_profile"
 _GLOBAL_IDENT_KEY = "global_identities"
 _ACTIVE_GLOBAL_IDENT_KEY = "active_global_identity"
-_DEFAULT_CONFIG_PATH = "~/.antimatter/config"
+_DEFAULT_CONFIG_PATH = os.path.join(Path.home(), ".antimatter", "config")
 
 
 class AuthConfig:
     """
     The AuthConfig is responsible for interacting with the config file and locally
     storing profile and identity information.
     """
@@ -67,23 +70,38 @@
 
         conf = AuthConfig()
         conf.schema = schema_version
         conf.profiles = [Profile.from_dict(prof) for prof in conf_dict.get(_PROFILES_KEY, [])]
         conf.active_profile = conf_dict.get(_ACTIVE_PROFILE_KEY, None)
         conf.global_identities = [GlobalIdentity.from_dict(glob_id) for glob_id in conf_dict.get(_GLOBAL_IDENT_KEY, [])]
         conf.active_global_identity = conf_dict.get(_ACTIVE_GLOBAL_IDENT_KEY, None)
+        conf.add_observers()
         return conf
+    
+    def add_observers(self):
+        for profile in self.profiles:
+            if profile.token is not None:
+                profile.token.add_observer(self.to_file)
+        for global_identity in self.global_identities:
+            global_identity.token.add_observer(self.to_file)
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Convert an AuthConfig into a dictionary.
 
         :return: The dictionary containing AuthConfig values
         """
-        _dict = {_SCHEMA_KEY: self.schema}
+        _dict = {
+            _SCHEMA_KEY: self.schema,
+            _PROFILES_KEY: [],
+            _ACTIVE_PROFILE_KEY: None,
+            _GLOBAL_IDENT_KEY: [],
+            _ACTIVE_GLOBAL_IDENT_KEY: None,
+        }
+
         if self.profiles:
             _dict[_PROFILES_KEY] = [prof.to_dict() for prof in self.profiles]
         if self.active_profile:
             _dict[_ACTIVE_PROFILE_KEY] = self.active_profile
         if self.global_identities:
             _dict[_GLOBAL_IDENT_KEY] = [global_ident.to_dict() for global_ident in self.global_identities]
         if self.active_global_identity:
@@ -134,21 +152,22 @@
         serialized = self.to_dict()
         with open(path, "w") as f:
             yaml.safe_dump(serialized, f)
 
     def add_profile(
         self,
         domain_id: str,
-        api_key: str,
+        api_key: str = None,
         name: Optional[str] = None,
         default_read_context: Optional[str] = None,
         default_write_context: Optional[str] = None,
         mark_active: bool = False,
         write_to_file: bool = False,
         path: Optional[str] = None,
+        token: Optional[OidcToken] = None,
     ) -> None:
         """
         Add a profile to the AuthConfig with the provided domain ID and API key. If
         no display name is provided, the domain ID will be used. If write_to_file is
         set to True, the updated AuthConfig will be written to the file it was loaded
         from, or the override path.
 
@@ -170,20 +189,58 @@
 
         prof = Profile(
             name=name,
             domain_id=domain_id,
             api_key=api_key,
             default_read_context=default_read_context,
             default_write_context=default_write_context,
+            token=token,
         )
         self.profiles.append(prof)
         if mark_active:
             self.active_profile = name
         if write_to_file:
             self.to_file(path=path)
+        
+    def update_profile(
+        self,
+        name: str,
+        domain_id: str,
+        api_key: Optional[str] = None,
+        token: Optional[OidcToken] = None,
+        default_read_context: Optional[str] = None,
+        default_write_context: Optional[str] = None,
+        write_to_file: bool = False,
+        path: Optional[str] = None,
+    ):
+        """
+        Update a profile with the provided domain ID and API key. If write_to_file is
+        set to True, the updated AuthConfig will be written to the file it was loaded
+        from, or the override path.
+
+        :param name: The display name of the profile to update
+        :param domain_id: The domain ID for the profile
+        :param api_key: The API key for the profile
+        :param token: The token for the profile
+        :param default_read_context: The default read context
+        :param default_write_context: The default write context
+        :param write_to_file: If True, overwrite the config file with the updated contents of the AuthConfig
+        :param path: Override path to the config file
+        """
+        prof = self.get_profile(name=name)
+        if prof is None:
+            raise ValueError(f"No profile found with name '{name}'")
+        
+        prof.domain_id = domain_id
+        prof.api_key = api_key
+        prof.token = token
+        prof.default_read_context = default_read_context
+        prof.default_write_context = default_write_context
+        if write_to_file:
+            self.to_file(path=path)
 
     def add_global_identity(
         self,
         token_type: str,
         name: str,
         mark_active: bool = False,
         write_to_file: bool = False,
@@ -206,14 +263,42 @@
         token = OidcTokenFactory.from_cli_type(token_type)
         global_ident = GlobalIdentity(name=name, token=token(**kwargs))
         self.global_identities.append(global_ident)
         if mark_active:
             self.active_global_identity = name
         if write_to_file:
             self.to_file(path=path)
+        
+    def update_global_identity(
+        self,
+        name: str,
+        token_type: str,
+        write_to_file: bool = False,
+        path: Optional[str] = None,
+        **kwargs,
+    ) -> None:
+        """
+        Update a global identity with the provided token type and kwargs. If write_to_file
+        is set to True, the updated AuthConfig will be written to the file it was loaded
+        from, or the override path.
+
+        :param name: The display name of the global identity to update
+        :param token_type: The token type for the global identity
+        :param write_to_file: If True, overwrite the config file with the updated contents of the AuthConfig
+        :param path: Override path to the config file
+        :param kwargs: The kwargs with which to initialize the global identity token
+        """
+        global_ident = self.get_global_identity(name)
+        if global_ident is None:
+            raise ValueError(f"No global identity found with name '{name}'")
+
+        token = OidcTokenFactory.from_cli_type(token_type)
+        global_ident.token = token(**kwargs)
+        if write_to_file:
+            self.to_file(path=path)
 
     def get_profile(self, name: Optional[str] = None, domain_id: Optional[str] = None) -> Optional[Profile]:
         """
         Get the profile using either the name or domain_id. Name has higher
         precedence if both are provided. If neither are provided, the active
         profile will be used.
```

## antimatter/auth/config/global_identity.py

```diff
@@ -1,38 +1,17 @@
 from dataclasses import dataclass
 from typing import Any, Dict, Type
 
-from antimatter.auth.config.tokens import OidcToken, OidcTokenType
-from antimatter.auth.google.models import GoogleOidcToken
+from antimatter.auth.config.tokens import OidcToken, OidcTokenFactory
+
 
 _NAME_KEY = "name"
 _TOKEN_KEY = "token"
 _TYPE_KEY = "type"
 
-
-class OidcTokenFactory:
-    """
-    The token factory for converting config file keywords or CLI keywords into
-    specific token formats.
-    """
-
-    @staticmethod
-    def from_dict_type(token_type: str) -> Type["OidcToken"]:
-        t = OidcTokenType(token_type)  # We'll raise an error here if the token type is invalid
-        if t is OidcTokenType.Google:
-            return GoogleOidcToken
-        assert False  # Should be unreachable
-
-    @staticmethod
-    def from_cli_type(cli_type: str) -> Type["OidcToken"]:
-        if cli_type == "google":
-            return GoogleOidcToken
-        raise ValueError(f"'{cli_type}' is not a supported token type")
-
-
 @dataclass
 class GlobalIdentity:
     """
     Global identity structure, containing name and token.
     """
     name: str
     token: OidcToken
```

## antimatter/auth/config/profiles.py

```diff
@@ -1,22 +1,36 @@
 from dataclasses import asdict, dataclass
 from typing import Any, Dict, Optional
-
+from antimatter.auth.config.tokens import OidcToken
 
 @dataclass
 class Profile:
     """
-    Profile structure, containing the name, domain ID, API key, and default
-    read and write contexts.
+    Profile structure, containing the name, domain ID, API key, default
+    read and write contexts and token
     """
     name: str
     domain_id: str
     api_key: str
     default_read_context: Optional[str]
     default_write_context: Optional[str]
+    token: Optional[OidcToken]
 
     @staticmethod
     def from_dict(json: Dict[str, Any]) -> "Profile":
-        return Profile(**json)
+        if json is None:
+            return None
+        json["oidc_token"] = OidcToken.from_dict(json["oidc_token"]) if json.get("oidc_token") else None
+        return Profile(
+            name=json["name"],
+            domain_id=json["domain_id"],
+            api_key=json["api_key"],
+            default_read_context=json.get("default_read_context"),
+            default_write_context=json.get("default_write_context"),
+            token=json["oidc_token"],
+        )
 
     def to_dict(self) -> Dict[str, Any]:
-        return asdict(self)
+        d = asdict(self)
+        del d["token"]
+        d["oidc_token"] = self.token.to_dict() if self.token else None
+        return d
```

## antimatter/auth/config/tokens.py

```diff
@@ -1,23 +1,119 @@
 from enum import Enum
-from typing import Any, Dict
+from typing import Any, Dict, List, Callable, Type
+from dataclasses import dataclass, asdict
+
+class OidcTokenFactory:
+    """
+    The token factory for converting config file keywords or CLI keywords into
+    specific token formats.
+    """
+
+    @staticmethod
+    def from_dict_type(token_type: str) -> Type["OidcToken"]:
+        t = OidcTokenType(token_type)  # We'll raise an error here if the token type is invalid
+        if t is OidcTokenType.Google:
+            return GoogleOidcToken
+        if t is OidcTokenType.Static:
+            return StaticToken
+        assert False  # Should be unreachable
+
+    @staticmethod
+    def from_cli_type(cli_type: str) -> Type["OidcToken"]:
+        if cli_type == "google":
+            return GoogleOidcToken
+        if cli_type == "static":
+            return StaticToken
+        raise ValueError(f"'{cli_type}' is not a supported token type")
 
 
 class OidcTokenType(str, Enum):
     """
     The enumerated supported OIDC token types.
     """
     Google = "GoogleToken"
+    Static = "StaticToken"
 
 
 class OidcToken:
     """
     The base OIDC token.
     """
 
     type: OidcTokenType
+    observers: List[Callable] = []
 
     def __init__(self, *args, **kwargs):
         pass
 
+    @staticmethod
+    def from_dict(json: Dict[str, Any]) -> "OidcToken":
+        token_type = json.get("type")
+
+        cls = OidcTokenFactory.from_dict_type(token_type)
+        if cls:
+            return cls.from_dict(json)
+        raise ValueError(f"Unsupported token type: {token_type}")
+
     def to_dict(self) -> Dict[str, Any]:
         raise NotImplementedError("must serialize specific token type")
+    
+    def add_observer(self, observer: Callable):
+        self.observers.append(observer)
+    
+    def notify_observers(self):
+        for observer in self.observers:
+            observer()
+
+
+@dataclass
+class StaticToken(OidcToken):
+    """
+    A static oauth token format.
+    """
+    token: str
+    type: OidcTokenType = OidcTokenType.Static
+
+    def to_dict(self) -> Dict[str, Any]:
+        json = asdict(self)
+        json["type"] = self.type.value
+        return json
+
+    @staticmethod
+    def from_dict(json: Dict[str, Any]) -> "StaticToken":
+        return StaticToken(**json)
+
+@dataclass
+class GoogleOidcToken(OidcToken):
+    """
+    The Google OIDC token format.
+    """
+    access_token: str
+    id_token: str
+    refresh_token: str
+    expires_at: int
+    type: OidcTokenType = OidcTokenType.Google
+
+    def to_dict(self) -> Dict[str, Any]:
+        json = asdict(self)
+        json["type"] = self.type.value
+        return json
+
+    @staticmethod
+    def from_dict(json: Dict[str, Any]) -> "GoogleOidcToken":
+        return GoogleOidcToken(
+            access_token=json["access_token"],
+            id_token=json["id_token"],
+            refresh_token=json["refresh_token"],
+            expires_at=json["expires_at"],
+            type=OidcTokenType.Google
+        )
+
+    @staticmethod
+    def init() -> "GoogleOidcToken":
+        return GoogleOidcToken(
+            access_token=None,
+            id_token=None,
+            refresh_token=None,
+            expires_at=None,
+            type=OidcTokenType.Google
+        )
```

## antimatter/builders/capability.py

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional, Tuple, Union
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 from antimatter.constants import CapabilityOperator
 
 
 class CapabilityRulesBuilder:
     """
     Builder class for creating a CapabilityRule.
```

## antimatter/builders/fact_policy.py

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 from typing import List, Optional, Tuple, Union
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 from antimatter.constants import FactArgumentSource, FactOperator
 
 
 class FactPolicyArgumentBuilder:
     """
     Builder class for creating a FactPolicyRulesInnerArgumentsInner.
```

## antimatter/builders/read_context.py

```diff
@@ -1,10 +1,10 @@
 from typing import Union
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 from antimatter.constants import Hook
 
 
 class ReadContextBuilder:
     """
     A builder class for constructing a ReadContext object.
     """
```

## antimatter/builders/read_context_rule.py

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 from typing import List, Optional, Union
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 from antimatter.builders.fact_policy import FactOperator
 from antimatter.constants import Action, Operator, Source, TokenFormat, TokenScope
 
 class ReadContextRuleBuilder:
     """
     Builder class for creating a ReadContextConfigRule.
     """
```

## antimatter/builders/root_encryption_key.py

```diff
@@ -1,31 +1,32 @@
 import base64
 
 from typing import List, Union
 
-from antimatter.client import (
+from antimatter_api import (
     AWSServiceAccountKeyInfo, GCPServiceAccountKeyInfo, AntimatterDelegatedAWSKeyInfo, KeyInfosKeyInformation,
     KeyInfos
 )
 
 
 class OverrideKeyInfosKeyInformation(KeyInfosKeyInformation):
     one_of_schemas: List[str] = ["AWSServiceAccountKeyInfo", "AntimatterDelegatedAWSKeyInfo", "GCPServiceAccountKeyInfo"]
 
 
 def aws_service_account_key_info(access_key_id: str, secret_access_key: str, key_arn: str = "") -> KeyInfos:
     """
     Create a KeyInfos object with AWS service account key information
 
     Example usage:
-    ```
-    key_info = aws_service_account_key_info(
-        access_key_id="access_key_id", secret_access_key="secret_access_key", key_arn="key_arn"
-    )
-    ```
+
+    .. code-block:: python
+
+        key_info = aws_service_account_key_info(
+            access_key_id="access_key_id", secret_access_key="secret_access_key", key_arn="key_arn"
+        )
 
     :param access_key_id: The access key ID
     :param secret_access_key: The secret access key
     :param key_arn: The key ARN
 
     :return: A KeyInfos object with the specified key information
     """
@@ -38,17 +39,18 @@
     )
 
 def antimatter_delegated_aws_key_info(key_arn: str) -> KeyInfos:
     """
     Create a KeyInfos object with Antimatter delegated AWS key information
 
     Example usage:
-    ```
-    key_info = antimatter_delegated_aws_key_info(key_arn="key_arn")
-    ```
+
+    .. code-block:: python
+
+        key_info = antimatter_delegated_aws_key_info(key_arn="key_arn")
 
     :param key_arn: The key ARN
 
     :return: A KeyInfos object with the specified key information
     """
     return KeyInfos(
         keyInformation=OverrideKeyInfosKeyInformation(
@@ -64,24 +66,26 @@
         service_account_credentials: str = "",
         service_account_credentials_path: str = "",
     ) -> KeyInfos:
     """
     Create a KeyInfos object with GCP service account key information
 
     Example usage:
-    ```
-    key_info = gcp_service_account_key_info(
-        project_id="project_id",
-        location="location",
-        key_ring_id="key_ring_id",
-        key_id="key_id",
-        service_account_credentials="<service_account_credentials_as_json_string>",
-        service_account_credentials_path="/path/to/service_account_credentials.json"
-    )
-    ```
+
+    .. code-block:: python
+
+        key_info = gcp_service_account_key_info(
+            project_id="project_id",
+            location="location",
+            key_ring_id="key_ring_id",
+            key_id="key_id",
+            service_account_credentials="<service_account_credentials_as_json_string>",
+            service_account_credentials_path="/path/to/service_account_credentials.json"
+        )
+
     Either `service_account_credentials` or `service_account_credentials_path` should be provided.
 
     :param project_id: The project ID
     :param location: The location
     :param key_ring_id: The key ring ID
     :param key_id: The key ID
     :param service_account_credentials: The service account credentials as JSON string
```

## antimatter/builders/settings_patch.py

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import Union
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 from antimatter.constants import PatchOperation
 
 @dataclass
 class SettingsPatchBuilder:
     """
     Builder class for creating a settings patch.
```

## antimatter/builders/write_context.py

```diff
@@ -1,10 +1,10 @@
 from typing import Union
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 from antimatter.constants import Hook, WriteContextHookMode
 
 class WriteContextBuilder:
     """
     Builder class for creating WriteContext objects.
     """
     def __init__(self) -> None:
```

## antimatter/builders/write_context_rule.py

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Union
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 from antimatter.tags import TagType
 
 
 class WriteContextRegexRuleBuilder:
     """
     Builder class for creating a WriteContextRegexRule
     """
```

## antimatter/cap_prep/prep.py

```diff
@@ -1,15 +1,15 @@
 from collections import defaultdict
 from typing import Any, Dict, List, Tuple
 
 import antimatter_engine as am
 
 from antimatter.cap_prep.applicator import SpanTagApplicator, TAG_SOURCE, TAG_VERSION
 from antimatter.tags import ColumnTag, SpanTag
-from antimatter.cell_path import cell_path
+from antimatter.cell_utils import cell_path
 from antimatter.extra_helper import get_field_type
 
 
 class Preparer:
     """
     Preparer is a helper class to prepare data for encapsulation, packing it in
     the intermediary data formats.
```

## antimatter/cap_prep/tests/test_prep.py

```diff
@@ -1,15 +1,15 @@
 from collections import defaultdict
 
 import pytest
 
 from antimatter.tags import ColumnTag, SpanTag 
 import antimatter.handlers as handlers
 from antimatter.cap_prep.prep import Preparer
-from antimatter.cell_path import cell_path
+from antimatter.cell_utils import cell_path
 from antimatter.datatype.infer import infer_datatype
 from antimatter.extra_helper import extra_for_session
 
 some_col = "some"
 name_col = "name"
 std_data = [
     {some_col: "data", name_col: "The name is Adam Smith"},
```

## antimatter/datatype/infer.py

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-from antimatter.errors import errors
+from antimatter import errors
 from antimatter.datatype.datatypes import Datatype
 from antimatter.fieldtype.infer import infer_fieldtype
 
 DICT_LIST_FMT_ERROR = "data in a list format must contain dictionaries"
 
 
 def infer_datatype(data: Any) -> Datatype:
```

## antimatter/datatype/tests/test_factory.py

```diff
@@ -1,11 +1,11 @@
 import pytest
 
 from antimatter.datatype.datatypes import Datatype
-from antimatter.errors.errors import HandlerFactoryError
+from antimatter.errors import HandlerFactoryError
 from antimatter.handlers import factory
 
 datatypes = [dt for dt in Datatype if dt is not Datatype.Unknown]
 
 
 class TestHandlerFactory:
     """
```

## antimatter/dependencies/tests/test_versions.py

```diff
@@ -1,10 +1,9 @@
 import pytest
 
-from antimatter.dependencies.versions import as_install_hint, _parse_requirements
-from antimatter.errors.errors import MissingDependency
+from antimatter.dependencies.versions import as_install_hint
 
 
 def test_as_install_hint():
     # For this to pass, the requirements will need to be findable and parseable
     hint = as_install_hint("pandas")
     assert "pip install pandas" in hint
```

## antimatter/errors/__init__.py

```diff
@@ -0,0 +1,3 @@
+00000000: 6672 6f6d 2061 6e74 696d 6174 7465 722e  from antimatter.
+00000010: 6572 726f 7273 2e65 7272 6f72 7320 696d  errors.errors im
+00000020: 706f 7274 202a 0a                        port *.
```

## antimatter/errors/errors.py

```diff
@@ -91,7 +91,11 @@
 
     def __init__(self, err: ModuleNotFoundError, override: str = None):
         self.err = err.msg
         self.hint = as_install_hint(override or err.name)
 
     def __str__(self):
         return f"{self.err}. {self.hint}"
+
+class PermissionDenied(Exception):
+    """Error for when a user does not have the required permissions"""
+    pass
```

## antimatter/fieldtype/converters.py

```diff
@@ -1,13 +1,12 @@
 import datetime
 import decimal
 import re
 from typing import Any, Callable, Optional
 
-from antimatter.errors import errors
 from antimatter.fieldtype.fieldtypes import FieldType
 
 
 class Standard:
     @staticmethod
     def field_converter_from_generic(ft: FieldType) -> Optional[Callable[[bytes], Any]]:
         """
```

## antimatter/fieldtype/infer.py

```diff
@@ -1,12 +1,12 @@
 import datetime
 import decimal
 from typing import Any
 
-from antimatter.errors import errors
+from antimatter import errors
 from antimatter.fieldtype.fieldtypes import FieldType
 
 
 def infer_fieldtype(field: Any) -> FieldType:
     """
     Convenience handler for inferring the FieldType from an instance of a data
     field. Supported data types include scalar python values, decimal types,
```

## antimatter/filetype/extract.py

```diff
@@ -1,12 +1,12 @@
 import csv
 import json
 from typing import Any, Dict, List
 
-from antimatter.errors.errors import DataFormatError, MissingDependency
+from antimatter.errors import DataFormatError, MissingDependency
 
 
 def extract_from_file(path: str, hint: str) -> Any:
     """
     Extracts data from a file based on the provided hint about the file's format.
 
     :param path: The path to the file.
```

## antimatter/filetype/tests/test_filetypes.py

```diff
@@ -1,12 +1,12 @@
 import os
 import pandas as pd
 import pytest
 from antimatter.filetype.extract import extract_from_file, extract_from_csv, extract_from_json, extract_from_ndjson, extract_from_parquet, extract_from_txt
-from antimatter.errors import errors
+from antimatter import errors
 
 fixtures_dir = os.path.join(os.path.dirname(__file__), 'fixtures')
 
 class TestExtractFromFile:
     def test_invalid_hint(self):
         with pytest.raises(errors.DataFormatError):
             extract_from_file(os.path.join(fixtures_dir, "data.txt"), "invalid")
```

## antimatter/handlers/__init__.py

```diff
@@ -1,9 +1,9 @@
 from antimatter.datatype.datatypes import Datatype
-from antimatter.errors.errors import HandlerFactoryError
+from antimatter.errors import HandlerFactoryError
 from antimatter.handlers.base import DataHandler
 from antimatter.handlers.dict_list import DictList
 from antimatter.handlers.dictionary import Dictionary
 from antimatter.handlers.langchain import LangchainHandler
 from antimatter.handlers.pandas_dataframe import PandasDataFrame
 from antimatter.handlers.pytorch_dataloader import PytorchDataLoader
 from antimatter.handlers.scalar import ScalarHandler
@@ -11,16 +11,16 @@
 
 def factory(datatype: Datatype) -> DataHandler:
     """
     Factory returns an instance of a DataHandler matching the provided Datatype.
 
     :param datatype: The Datatype to get a handler for.
     :return:
-    An implementation of the abstract DataHandler for handling data of the
-    given type.
+        An implementation of the abstract DataHandler for handling data of the
+        given type.
     """
     if datatype is Datatype.Unknown:
         raise HandlerFactoryError("cannot create factory from 'Unknown' Datatype")
     elif datatype is Datatype.Scalar:
         return ScalarHandler()
     elif datatype is Datatype.Dict:
         return Dictionary()
```

## antimatter/handlers/base.py

```diff
@@ -1,11 +1,11 @@
 import abc
 from typing import Any, Callable, Dict, List, Tuple
 
-from antimatter.errors import errors
+from antimatter import errors
 from antimatter.fieldtype import converters
 from antimatter.fieldtype.fieldtypes import FieldType
 
 
 class DataHandler(abc.ABC):
     """
     Abstract base DataHandler defining the supporting methods a handler for a
```

## antimatter/handlers/dict_list.py

```diff
@@ -12,15 +12,15 @@
     def from_generic(self, cols: List[str], generic_data: List[List[bytes]], extra: dict) -> List[Dict[str, Any]]:
         """
         from_generic takes the generic data and passes it on as a list of
         dictionaries
 
         :param cols: the column names
         :param generic_data:
-        the capsule's generic data format holding the row values
+            the capsule's generic data format holding the row values
         :param extra: extra data for the DataHandler
         :return: the data in a dictionary list format
         """
         col_ft_cache = {}
 
         data = []
         for generic_row in generic_data:
```

## antimatter/handlers/langchain.py

```diff
@@ -1,34 +1,44 @@
 import base64
 import json
 from typing import Any, Dict, List, Tuple
-
+import numpy as np
+import uuid
+from dataclasses import dataclass
 
 # For type hinting
 try:
     from langchain.callbacks.manager import CallbackManagerForRetrieverRun
     from langchain.pydantic_v1 import BaseModel
     from langchain.schema.document import Document
     from langchain.schema.embeddings import Embeddings
     from langchain.schema.retriever import BaseRetriever
     from langchain.schema.vectorstore import VectorStoreRetriever
 except ModuleNotFoundError:
     pass
 
-from antimatter.errors.errors import HandlerError, MissingDependency
+from antimatter.errors import MissingDependency
 from antimatter.extra_helper import COL_TYPE_KEY
 from antimatter.fieldtype.fieldtypes import FieldType
 from antimatter.fieldtype.infer import infer_fieldtype
-from antimatter.handlers import DataHandler
+from antimatter.handlers.base import DataHandler
 
 
 class EmbeddingClient:
     OPEN_AI = "openai"
     HUGGING_FACE = "huggingface"
 
+@dataclass
+class BaseDocument:
+    """
+    BaseDocument is a wrapper around the langchain Document.
+    It is used to store the page content of the document.
+    """
+    content: Any
+    embedding: List[float]
 
 class LangchainHandler(DataHandler):
     """
     The LangchainHandler DataHandler supports an implementation of a langchain
     Retriever. This handler assumes that the underlying data is a list of
     two-dimensional data.
     """
@@ -62,23 +72,24 @@
         assert isinstance(data, LangchainHandler.Retriever)
 
         cols = set()
         rows = []
         extra = {}
 
         col_ft_cache = {}
-        if data.data:
+        if data.vectors:
             extra[COL_TYPE_KEY] = {}
 
         # First pass: get column names
-        [cols.add(key) for d in data.data for key in d]
+        [cols.add(key) for _, docs in data.vectors.items() for key in docs.content]
 
         # Second pass: flatten dicts into rows
         cols = list(cols)
-        for d in data.data:
+        for _, docs in data.vectors.items():
+            d = docs.content
             row = []
             for cname in cols:
                 # TODO: Handle 'missing' values using 'extras' dict
                 val = d.get(cname)
                 if val is None:
                     val = ""
                 else:
@@ -95,20 +106,17 @@
 
     try:
         class Retriever(BaseRetriever):
             """
             Retriever is a wrapper around the langchain Retriever.
             It is used to store and retrieve data from the langchain Retriever.
             """
-
+            vectors: Dict[str, BaseDocument] = {}
+            k: int = 10
             embeddings: Embeddings = None
-            delegate: VectorStoreRetriever = None
-            # We need 2 copies of the data because it can't be retrieved from the
-            # underlying delegate in a non-hacky way
-            data: List[Dict[str, bytes]] = None
             extra: Dict[str, Any] = None
 
             def encrypt(self, data):
                 return base64.b64encode(str(data).encode('utf-8')).decode("utf-8")
 
             def decrypt(self, data):
                 return base64.b64decode(data).decode("utf-8")
@@ -116,35 +124,38 @@
             def __init__(self, data: List[Dict[str, bytes]], extra: Dict[str, Any] = None):
                 try:
                     from langchain.callbacks.manager import CallbackManagerForRetrieverRun
                     from langchain.pydantic_v1 import BaseModel
                     from langchain.schema.document import Document
                     from langchain.schema.embeddings import Embeddings
                     from langchain.schema.retriever import BaseRetriever
-                    from langchain.schema.vectorstore import VectorStoreRetriever
-                    from langchain_community.vectorstores import FAISS
                 except ModuleNotFoundError as me:
                     raise MissingDependency(me)
 
                 super().__init__()
                 if extra is None:
                     extra = {}
                 self.embeddings = LangchainHandler.Embed(extra=extra)
-                self.data = data
                 self.extra = extra
-                knowledgebase = []
                 for row in data:
                     embedding = self.embeddings.embed_documents([json.dumps(row)])
-                    knowledgebase.append((self.encrypt(row), embedding[0]))
-                faiss = FAISS.from_embeddings(knowledgebase, self.embeddings)
-                self.delegate: VectorStoreRetriever = faiss.as_retriever(search_kwargs={"k": self.extra.get("k", 10)})
+                    self.vectors[uuid.uuid4().hex] = BaseDocument(
+                        content=row,
+                        embedding=embedding[0]
+                    )
 
             def _get_relevant_documents(self, query: str, *, run_manager: CallbackManagerForRetrieverRun) -> List[Document]:
-                docs = self.delegate.get_relevant_documents(query, run_manager=run_manager)
-                return [Document(page_content=self.decrypt(d.page_content)) for d in docs]
+                """Return the first k documents from the list of documents"""
+                distances = {id: np.linalg.norm(docs.embedding - self.embeddings.embed_query(query)) for id, docs in self.vectors.items()}
+                return [Document(
+                    page_content=json.dumps(self.vectors[id].content)
+                ) for id, _ in sorted(distances.items(), key=lambda x: x[1])[:self.k]]
+
+            async def _aget_relevant_documents(self, query: str) -> List[Document]:
+                return self._get_relevant_documents(query)
 
         class Embed(BaseModel, Embeddings):
             """
             Embed is a wrapper around the embedding client.
             Currently, it supports the following embedding clients:
             - OpenAI
             - Huggingface flan-t5-base (default)
```

## antimatter/handlers/pandas_dataframe.py

```diff
@@ -4,18 +4,17 @@
 # For type hinting
 try:
     import pandas as pd
 except ModuleNotFoundError:
     pass
 
 import antimatter.extra_helper as extra_helper
-from antimatter.errors import errors
-from antimatter.errors.errors import MissingDependency
+from antimatter.errors import DataFormatError, MissingDependency
 from antimatter.fieldtype.infer import infer_fieldtype
-from antimatter.handlers import DataHandler
+from antimatter.handlers.base import DataHandler
 
 
 class PandasDataFrame(DataHandler):
     """
     The PandasDataFrame DataHandler supports a pandas DataFrame. There are
     some restrictions on the underlying dataset which must be a two-dimensional
     data set, or a list of two-dimensional data sets.
@@ -88,15 +87,15 @@
 
         rows = []
         extra = {}
         cols = df.columns.tolist()
         col_ft_cache = {}
 
         if self._data_is_not_2d(df):
-            raise errors.DataFormatError("only 2-dimensional DataFrames are supported")
+            raise DataFormatError("only 2-dimensional DataFrames are supported")
 
         data = df.to_dict(orient="records")
 
         # Get dtypes for each column
         if data:
             extra[extra_helper.COL_TYPE_KEY] = {}
```

## antimatter/handlers/pytorch_dataloader.py

```diff
@@ -1,21 +1,21 @@
 from typing import Any, Dict, List, Tuple
 
-from antimatter.errors.errors import MissingDependency
+from antimatter.errors import MissingDependency
 
 # For type hinting
 try:
     from torch.utils.data import DataLoader, Dataset
 except ModuleNotFoundError:
     pass
 
 import antimatter.extra_helper as extra_helper
-from antimatter.errors import errors
+from antimatter import errors
 from antimatter.fieldtype.infer import infer_fieldtype
-from antimatter.handlers import DataHandler
+from antimatter.handlers.base import DataHandler
 
 
 class PytorchDataLoader(DataHandler):
     """
     The PytorchDataLoader DataHandler supports a pytorch DataLoader. There are
     some restrictions on the underlying dataset, which must be iterable, producing
     two-dimensional dictionaries.
```

## antimatter/handlers/scalar.py

```diff
@@ -1,16 +1,14 @@
 from typing import Any, Dict, List, Tuple
 
 import antimatter.extra_helper as extra_helper
-from antimatter.extra_helper import COL_TYPE_KEY
+from antimatter.extra_helper import COL_TYPE_KEY, DEFAULT_COL_NAME
 from antimatter.fieldtype.infer import infer_fieldtype
 from antimatter.handlers.base import DataHandler
 
-COLUMN_NAME = "content"
-
 
 class ScalarHandler(DataHandler):
     """
     The Scalar DataHandler supports a scalar value. 
     """
 
     def from_generic(self, cols: List[str], generic_data: List[List[bytes]], extra: Dict[str, Any]) -> Any:
@@ -34,8 +32,8 @@
         to_generic converts a scalar value into the generic data format.
 
         :param data: the scalar value to wrap into a generic format
         :return: the data in its generic form
         """
         ft = infer_fieldtype(data)
         field = self.field_converter_to_generic(ft)(data)
-        return [COLUMN_NAME], [[field]], {COL_TYPE_KEY: {COLUMN_NAME: ft.value}}
+        return [DEFAULT_COL_NAME], [[field]], {COL_TYPE_KEY: {DEFAULT_COL_NAME: ft.value}}
```

## antimatter/handlers/tests/test_dict_list.py

```diff
@@ -1,13 +1,13 @@
 import datetime
 import decimal
 
 import pytest
 
-from antimatter.errors import errors
+from antimatter import errors
 from antimatter.handlers import DictList
 
 
 class TestDictList:
     @pytest.mark.parametrize(
         "data",
         (
```

## antimatter/handlers/tests/test_dictionary.py

```diff
@@ -1,13 +1,13 @@
 import datetime
 import decimal
 
 import pytest
 
-from antimatter.errors import errors
+from antimatter import errors
 from antimatter.handlers import Dictionary
 
 
 class TestDictionary:
     @pytest.mark.parametrize(
         "data",
         (
```

## antimatter/handlers/tests/test_langchain.py

```diff
@@ -1,22 +1,17 @@
 import pytest
 
-from antimatter.handlers import LangchainHandler
+from antimatter.handlers.langchain import LangchainHandler
 
 
 class TestLangchain:
     @pytest.mark.parametrize(
         "data",
         (
             LangchainHandler.Retriever([{"a": "1", "b": "2", "c": "4"}]),
-            # Retriever([
-            #     {"a": "1", "b": "2", "c": "4"},
-            #     {"a": "5", "b": "3", "d": "8"},
-            #     {"a": "0", "b": "7", "c": "6", "d": "9"},
-            # ]),
             LangchainHandler.Retriever([{}]),
             LangchainHandler.Retriever(
                 [
                     {"a": "1", "b": "2", "c": "4", "d": "6"},
                     {"a": "5", "b": "3", "c": "1", "d": "8"},
                     {"a": "0", "b": "7", "c": "6", "d": "9"},
                 ]
@@ -29,8 +24,8 @@
             "retriever data embeddings of multiples dictionaries with string values",
         ),
     )
     def test_lossless_conversions(self, data):
         handler = LangchainHandler()
         cols, rows, extra = handler.to_generic(data)
         generic = handler.from_generic(cols, rows, extra)
-        assert generic.data == data.data
+        assert list(generic.vectors.values())[0].content == list(data.vectors.values())[0].content
```

## antimatter/handlers/tests/test_pandas_dataframe.py

```diff
@@ -2,15 +2,15 @@
 import decimal
 
 import numpy as np
 import pandas as pd
 import pyarrow
 import pytest
 
-from antimatter.errors import errors
+from antimatter import errors
 from antimatter.handlers import PandasDataFrame
 
 
 class TestPandasDataFrame:
     @pytest.mark.parametrize(
         "data",
         (
```

## antimatter/handlers/tests/test_pytorch_dataloader.py

```diff
@@ -1,14 +1,14 @@
 import datetime
 import decimal
 
 import pytest
 from torch.utils.data import DataLoader
 
-from antimatter.errors import errors
+from antimatter import errors
 from antimatter.handlers.pytorch_dataloader import PytorchDataLoader
 
 
 class TestPytorchDataLoader:
     @pytest.mark.parametrize(
         "data",
         (
```

## antimatter/handlers/tests/test_scalar.py

```diff
@@ -1,14 +1,14 @@
 import datetime
 import decimal
 import os
 
 import pytest
 
-from antimatter.errors import errors
+from antimatter import errors
 from antimatter.handlers import ScalarHandler
 
 
 class TestScalar:
     @pytest.mark.parametrize(
         "data",
         (
```

## antimatter/requirements/all.txt

```diff
@@ -1,7 +1,8 @@
 langchain>=0.0.341
 faiss-cpu>=1.7.3
 transformers>=4.23
 torch>=2.0
 numpy>=1.23.3
 pandas[performance]>=2.0
 pyarrow>=2.0
+langchain_community>=0.2.0
```

## antimatter/requirements/core.txt

```diff
@@ -1,9 +1,12 @@
+# This will be replaced by the build system with the appropriate version
+antimatter-engine==1.1.0
+antimatter_api==1.0.7
 annotated_types>=0.6
 packaging>=21.1
 pydantic>=2.0
 python-dateutil>=2.1
 pyyaml
 cbor2~=5.5
 urllib3>=2.0.2
-# This will be replaced by the build system with the appropriate version from client/VERSION.txt
-antimatter-engine==1.0.0
+google-auth>=2.29.0
+requests>=2.31.0
```

## antimatter/requirements/langchain-huggingface.txt

```diff
@@ -1,4 +1,5 @@
 langchain>=0.0.341
 faiss-cpu>=1.7.3
 transformers>=4.23
 torch>=2.0
+numpy>=1.26
```

## antimatter/requirements/langchain.txt

```diff
@@ -1,2 +1,4 @@
 langchain>=0.0.341
 faiss-cpu>=1.7.3
+numpy>=1.26
+langchain_community>=0.2.0
```

## antimatter/session_mixins/__init__.py

```diff
@@ -3,11 +3,12 @@
 from antimatter.session_mixins.domain_mixin import DomainMixin
 from antimatter.session_mixins.encryption_mixin import EncryptionMixin
 from antimatter.session_mixins.fact_mixin import FactMixin
 from antimatter.session_mixins.general_mixin import GeneralMixin
 from antimatter.session_mixins.identity_provider_mixin import IdentityProviderMixin
 from antimatter.session_mixins.policy_rule_mixin import PolicyRuleMixin
 from antimatter.session_mixins.read_context_mixin import ReadContextMixin
-from antimatter.session_mixins.token import exec_with_token
+
 from antimatter.session_mixins.write_context_mixin import WriteContextMixin
-from antimatter.session_mixins.verification_mixin import VerificationMixin, ADMIN_VERIFICATION_PROMPT
+from antimatter.session_mixins.verification_mixin import VerificationMixin
 from antimatter.session_mixins.root_encryption_key_mixin import RootEncryptionKeyMixin
+from antimatter.session_mixins.starred_domain_mixin import StarredDomainMixin
```

## antimatter/session_mixins/capability_mixin.py

```diff
@@ -1,51 +1,38 @@
 from typing import Any, Callable, Dict, List, Optional
 
-import antimatter.client as openapi_client
-from antimatter.session_mixins.token import exec_with_token
+import antimatter_api as openapi_client
 
+from antimatter.session_mixins.base import BaseMixin
 
-class CapabilityMixin:
+class CapabilityMixin(BaseMixin):
     """
     Session mixin defining CRUD functionality for capabilities.
     """
 
-    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
-        try:
-            super().__init__(domain=domain, client_func=client_func, **kwargs)
-        except TypeError:
-            super().__init__()  # If this is last mixin, super() will be object()
-        self._domain = domain
-        self._client_func = client_func
-
-    @exec_with_token
-    def get_capabilities(self) -> List[Dict[str, Any]]:
+    def list_capabilities(self) -> List[Dict[str, Any]]:
         """
         Get the capabilities for the session's domain.
 
         :return: A list of capabilities.
         """
         capabilities = []
-        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
-        for capability in auth_api.domain_get_capabilities(domain_id=self._domain).capabilities:
+        for capability in openapi_client.AuthenticationApi(self.authz.get_client()).domain_get_capabilities(domain_id=self.domain_id).capabilities:
             capabilities.append(capability.model_dump())
         return capabilities
 
-    @exec_with_token
     def get_capability(self, name: str) -> Dict[str, Any]:
         """
         Get a specific capability for the session's domain.
 
         :param name: The name for this capability, like "admin"
         :return: The details of the capability.
         """
-        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
-        return auth_api.domain_get_capability(domain_id=self._domain, capability=name).model_dump()
+        return openapi_client.AuthenticationApi(self.authz.get_client()).domain_get_capability(domain_id=self.domain_id, capability=name).model_dump()
 
-    @exec_with_token
     def put_capability(
             self,
             name: str,
             summary: str,
             description: Optional[str] = None,
             unary: bool = True,
             create_only: bool = False,
@@ -57,32 +44,29 @@
         the capability.
 
         :param name: The name for this capability, like "admin"
         :param summary: A short, single sentence description of this capability
         :param description: An optional longer form description of this capability
         :param unary: A unary capability does not have a value
         :param create_only:
-        If True, an error will be returned if a capability with the name already exists
+            If True, an error will be returned if a capability with the name already exists
         """
         if description is None:
             description = ""
-        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
-        auth_api.domain_put_capability(
-            domain_id=self._domain,
+        openapi_client.AuthenticationApi(self.authz.get_client()).domain_put_capability(
+            domain_id=self.domain_id,
             capability=name,
             new_capability_definition=openapi_client.NewCapabilityDefinition(
                 unary=unary,
                 summary=summary,
                 description=description,
             ),
             createonly=create_only,
         )
 
-    @exec_with_token
     def delete_capability(self, name: str) -> None:
         """
         Delete a capability.
 
         :param name: The name of the capability, like "admin"
         """
-        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
-        auth_api.domain_delete_capability(domain_id=self._domain, capability=name)
+        openapi_client.AuthenticationApi(self.authz.get_client()).domain_delete_capability(domain_id=self.domain_id, capability=name)
```

## antimatter/session_mixins/capsule_mixin.py

```diff
@@ -1,120 +1,105 @@
 from datetime import datetime
 from typing import Any, Callable, Dict, Iterator, List, Optional
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 from antimatter.tags import CapsuleTag
 from antimatter.cap_prep.applicator import TAG_SOURCE, TAG_VERSION
-from antimatter.session_mixins.token import exec_with_token
 
+from antimatter.session_mixins.base import BaseMixin
 
-class CapsuleMixin:
+
+class CapsuleMixin(BaseMixin):
     """
     Session mixin defining CRUD functionality for capsules and tags.
     """
 
     _page_res_size: int = 100
 
-    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
-        try:
-            super().__init__(domain=domain, client_func=client_func, **kwargs)
-        except TypeError:
-            super().__init__()  # If this is last mixin, super() will be object()
-        self._domain = domain
-        self._client_func = client_func
-
-    @exec_with_token
     def list_capsules(
         self,
         start_date: Optional[datetime] = None,
         end_date: Optional[datetime] = None,
         span_tag: Optional[str] = None,
         sort_on: Optional[str] = None,
         ascending: Optional[bool] = None,
     ) -> Iterator[Dict[str, Any]]:
         """
         Returns an iterator over the capsules available for the current domain and auth
 
         :param start_date:
-        The earlier date of the date range. As results are returned in reverse chronological order, this date
-        corresponds with the end of the result set.
+            The earlier date of the date range. As results are returned in reverse chronological order, this date
+            corresponds with the end of the result set.
         :param end_date:
-        The later date of the date range. As results are returned in reverse chronological order, this date
-        corresponds with the beginning of the result set. If not specified, defaults to the current time.
+            The later date of the date range. As results are returned in reverse chronological order, this date
+            corresponds with the beginning of the result set. If not specified, defaults to the current time.
         :param span_tag:
-        The span tag you would like to filter on. This accepts a tag key only and will return all span tag key
-        results matching the provided tag key. If not specified, this field is ignored.
+            The span tag you would like to filter on. This accepts a tag key only and will return all span tag key
+            results matching the provided tag key. If not specified, this field is ignored.
         :param sort_on:
-        The capsule field you would like to sort on. This accepts the field only and will return results ordered
-        on the provided field. If not specified, this field is ignored.
+            The capsule field you would like to sort on. This accepts the field only and will return results ordered
+            on the provided field. If not specified, this field is ignored.
         :param ascending:
-        This defines whether a sorted result should be order ascending. This accepts a boolean value and when true
-        will work in combination with the sort_on and start_after parameters to return values in ascending order.
-        If not specified, this field is ignored and treated as false.
+            This defines whether a sorted result should be order ascending. This accepts a boolean value and when true
+            will work in combination with the sort_on and start_after parameters to return values in ascending order.
+            If not specified, this field is ignored and treated as false.
         """
         pagination = None
-        capsules_api = openapi_client.CapsulesApi(api_client=self._client_func())
         while True:
-            res = capsules_api.domain_list_capsules(
-                domain_id=self._domain,
+            res = openapi_client.CapsulesApi(self.authz.get_client()).domain_list_capsules(
+                domain_id=self.domain_id,
                 start_date=start_date,
                 end_date=end_date,
                 num_results=self._page_res_size,
                 span_tags=span_tag,
                 sort_on=sort_on,
                 start_after=pagination,
                 ascending=ascending,
             )
             if not res.results:
                 break
             for capsule in res.results:
                 pagination = capsule.page_key
                 yield capsule.model_dump(exclude={"page_key"})
 
-    @exec_with_token
     def get_capsule_info(self, capsule_id: str) -> Dict[str, Any]:
         """
         Get the summary information about the capsule.
 
         :param capsule_id: The identifier for the capsule
         :return: The summary information about the capsule
         """
-        capsules_api = openapi_client.CapsulesApi(api_client=self._client_func())
-        return capsules_api.domain_get_capsule_info(
-            domain_id=self._domain, capsule_id=capsule_id,
+        return openapi_client.CapsulesApi(self.authz.get_client()).domain_get_capsule_info(
+            domain_id=self.domain_id, capsule_id=capsule_id,
         ).model_dump()
 
-    @exec_with_token
     def upsert_capsule_tags(self, capsule_id: str, tags: List[CapsuleTag]) -> None:
         """
         Upsert the capsule-level tags to apply to a capsule.
 
         :param capsule_id: The capsule to apply tags to
         :param tags: The tags to apply to the capsule
         """
-        capsules_api = openapi_client.CapsulesApi(api_client=self._client_func())
-        capsules_api.domain_upsert_capsule_tags(
-            domain_id=self._domain, capsule_id=capsule_id, tag=[
+        openapi_client.CapsulesApi(self.authz.get_client()).domain_upsert_capsule_tags(
+            domain_id=self.domain_id, capsule_id=capsule_id, tag=[
                 openapi_client.Tag(
                     name=tag.name,
                     value=tag.tag_value,
                     type=tag.tag_type.name.lower(),
                     hook_version=f"{TAG_VERSION[0]}.{TAG_VERSION[1]}.{TAG_VERSION[2]}",
                     source=TAG_SOURCE,
                 ) for tag in tags
             ]
         )
 
-    @exec_with_token
     def delete_capsule_tags(self, capsule_id: str, tag_names: List[str]) -> None:
         """
         Delete capsule-level tags
 
         :param capsule_id: The capsule to delete tags from
         :param tag_names: The names of the tags to delete
         """
-        capsules_api = openapi_client.CapsulesApi(api_client=self._client_func())
-        capsules_api.domain_delete_capsule_tags(
-            domain_id=self._domain,
+        openapi_client.CapsulesApi(self.authz.get_client()).domain_delete_capsule_tags(
+            domain_id=self.domain_id,
             capsule_id=capsule_id,
             delete_tags=openapi_client.DeleteTags(names=tag_names),
         )
```

## antimatter/session_mixins/domain_mixin.py

```diff
@@ -1,37 +1,18 @@
 from typing import Any, Callable, Dict, List, Optional
 
-import antimatter.client as openapi_client
-from antimatter.session_mixins.token import exec_with_token
+import antimatter_api as openapi_client
+from antimatter.session_mixins.base import BaseMixin
 
 
-class DomainMixin:
+class DomainMixin(BaseMixin):
     """
     Session mixin defining CRUD functionality for domains, including peering.
     """
 
-    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
-        try:
-            super().__init__(domain=domain, client_func=client_func, **kwargs)
-        except TypeError:
-            super().__init__()  # If this is last mixin, super() will be object()
-        self._domain = domain
-        self._client_func = client_func
-
-    @exec_with_token
-    def new_domain(self, admin_email: str) -> Dict[str, Any]:
-        """
-        Create a new domain with no default peer relationships.
-        """
-        general_api = openapi_client.GeneralApi(api_client=self._client_func())
-        return general_api.domain_add_new(
-            new_domain=openapi_client.NewDomain(admin_email=admin_email),
-        ).model_dump()
-
-    @exec_with_token
     def new_peer_domain(
         self,
         import_alias_for_child: str,
         display_name_for_child: str,
         nicknames: Optional[List[str]] = None,
         import_alias_for_parent: Optional[str] = None,
         display_name_for_parent: Optional[str] = None,
@@ -63,17 +44,16 @@
         :param link_domain_policy: Whether to link domain policy
         :param link_capsule_access_log: Whether to link capsule access log
         :param link_control_log: Whether to link control log
         :param link_capsule_manifest: Whether to link capsule manifest
 
         :return: The new peer domain
         """
-        general_api = openapi_client.GeneralApi(api_client=self._client_func())
-        return general_api.domain_create_peer_domain(
-            domain_id=self._domain,
+        return openapi_client.GeneralApi(self.authz.get_client()).domain_create_peer_domain(
+            domain_id=self.domain_id,
             create_peer_domain=openapi_client.CreatePeerDomain(
                 import_alias_for_child=import_alias_for_child,
                 display_name_for_child=display_name_for_child,
                 nicknames=nicknames,
                 import_alias_for_parent=import_alias_for_parent,
                 display_name_for_parent=display_name_for_parent,
                 link_all=link_all,
@@ -85,38 +65,33 @@
                 link_domain_policy=link_domain_policy,
                 link_capsule_access_log=link_capsule_access_log,
                 link_control_log=link_control_log,
                 link_capsule_manifest=link_capsule_manifest,
             )
         ).model_dump()
 
-    @exec_with_token
     def get_peer(self, nickname: Optional[str] = None, alias: Optional[str] = None) -> str:
         """
         Retrieve the domain ID of a domain that is configured as a peer of this
         session's domain by using either its alias or one of its nicknames.
 
         :param nickname: The nickname for the peer domain
         :param alias: One of the aliases of the peer domain
         :return: The domain ID
         """
-        general_api = openapi_client.GeneralApi(api_client=self._client_func())
-        return general_api.domain_get_peer(domain_id=self._domain, nickname=nickname, alias=alias).id
+        return openapi_client.GeneralApi(self.authz.get_client()).domain_get_peer(domain_id=self.domain_id, nickname=nickname, alias=alias).id
 
-    @exec_with_token
     def list_peers(self):
         """
         Return a list of the peers of this session's domain.
 
         :return: The peer list, containing IDs and other information about the domains
         """
-        general_api = openapi_client.GeneralApi(api_client=self._client_func())
-        return [p.model_dump() for p in general_api.domain_list_peers(domain_id=self._domain).peers]
+        return [p.model_dump() for p in openapi_client.GeneralApi(self.authz.get_client()).domain_list_peers(domain_id=self.domain_id).peers]
 
-    @exec_with_token
     def get_peer_config(
         self,
         peer_domain_id: Optional[str] = None,
         nickname: Optional[str] = None,
         alias: Optional[str] = None,
     ) -> Dict[str, Any]:
         """
@@ -126,20 +101,18 @@
         :param peer_domain_id: The domain ID of the peer
         :param nickname: The nickname for the peer domain
         :param alias: One of the aliases of the peer domain
         :return: The full peer configuration
         """
         if not peer_domain_id and (nickname or alias):
             peer_domain_id = self.get_peer(nickname=nickname, alias=alias)
-        general_api = openapi_client.GeneralApi(api_client=self._client_func())
-        return general_api.domain_get_peer_config(
-            domain_id=self._domain, peer_domain_id=peer_domain_id,
+        return openapi_client.GeneralApi(self.authz.get_client()).domain_get_peer_config(
+            domain_id=self.domain_id, peer_domain_id=peer_domain_id,
         ).model_dump()
 
-    @exec_with_token
     def update_peer(
         self,
         display_name: str,
         peer_domain_id: Optional[str] = None,
         nickname: Optional[str] = None,
         alias: Optional[str] = None,
         export_identity_providers: Optional[List[str]] = None,
@@ -222,17 +195,16 @@
         :param import_precedence: The precedence of the import
         :param import_capsule_access_log: Whether to import the capsule access log
         :param import_control_log: Whether to import the control log
         :param import_capsule_manifest: Whether to import the capsule manifest
         """
         if not peer_domain_id and (nickname or alias):
             peer_domain_id = self.get_peer(nickname=nickname, alias=alias)
-        general_api = openapi_client.GeneralApi(api_client=self._client_func())
-        general_api.domain_update_peer(
-            domain_id=self._domain,
+        openapi_client.GeneralApi(self.authz.get_client()).domain_update_peer(
+            domain_id=self.domain_id,
             peer_domain_id=peer_domain_id,
             domain_peer_config=openapi_client.DomainPeerConfig(
                 display_name=display_name,
                 export_identity_providers=export_identity_providers,
                 export_all_identity_providers=export_all_identity_providers,
                 export_facts=export_facts,
                 export_all_facts=export_all_facts,
@@ -266,15 +238,14 @@
                 import_precedence=import_precedence,
                 import_capsule_access_log=import_capsule_access_log,
                 import_control_log=import_control_log,
                 import_capsule_manifest=import_capsule_manifest,
             )
         )
 
-    @exec_with_token
     def delete_peer(
         self,
         peer_domain_id: Optional[str] = None,
         nickname: Optional[str] = None,
         alias: Optional[str] = None,
     ) -> None:
         """
@@ -283,18 +254,17 @@
 
         :param peer_domain_id: The domain ID of the peer
         :param nickname: The nickname for the peer domain
         :param alias: One of the aliases of the peer domain
         """
         if not peer_domain_id and (nickname or alias):
             peer_domain_id = self.get_peer(nickname=nickname, alias=alias)
-        general_api = openapi_client.GeneralApi(api_client=self._client_func())
-        general_api.domain_delete_peer(domain_id=self._domain, peer_domain_id=peer_domain_id)
+        openapi_client.GeneralApi(self.authz.get_client()).domain_delete_peer(domain_id=self.domain_id, peer_domain_id=peer_domain_id)
 
-    @exec_with_token
     def get_top_tags(self) -> List[str]:
         """
         Get domain tag info returns a list containing the top 100 tag names for the current session's domain.
         """
-        capsules_api = openapi_client.CapsulesApi(api_client=self._client_func())
-        res = capsules_api.domain_get_tag_info(domain_id=self._domain)
+        res = openapi_client.GeneralApi(self.authz.get_client()).domain_get_tag_info(
+            domain_id=self.domain_id,
+        )
         return [r.name for r in res.tags]
```

## antimatter/session_mixins/encryption_mixin.py

```diff
@@ -1,30 +1,17 @@
 from typing import Callable
 
-import antimatter.client as openapi_client
-from antimatter.session_mixins.token import exec_with_token
+import antimatter_api as openapi_client
 
+from antimatter.session_mixins.base import BaseMixin
 
-class EncryptionMixin:
+class EncryptionMixin(BaseMixin):
     """
     Session mixin defining CRUD functionality for encryption functionality.
-
-    :param domain: The domain to use for the session.
-    :param client: The client to use for the session.
     """
 
-    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
-        try:
-            super().__init__(domain=domain, client_func=client_func, **kwargs)
-        except TypeError:
-            super().__init__()  # If this is last mixin, super() will be object()
-        self._domain = domain
-        self._client_func = client_func
-
-    @exec_with_token
     def flush_encryption_keys(self):
         """
         Flush all keys in memory. The keys will be immediately reloaded from persistent
         storage, forcing a check that the domain's root key is still available
         """
-        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
-        encryption_api.domain_flush_encryption_keys(domain_id=self._domain)
+        openapi_client.EncryptionApi(self.authz.get_client()).domain_flush_encryption_keys(domain_id=self.domain_id)
```

## antimatter/session_mixins/fact_mixin.py

```diff
@@ -1,130 +1,104 @@
 from typing import Any, Callable, Dict, List, Optional
 
-import antimatter.client as openapi_client
-from antimatter.session_mixins.token import exec_with_token
+import antimatter_api as openapi_client
 
+from antimatter.session_mixins.base import BaseMixin
 
-class FactMixin:
+
+class FactMixin(BaseMixin):
     """
     Session mixin defining CRUD functionality for facts and fact types.
-
-    :param domain: The domain to use for the session.
-    :param client: The client to use for the session.
     """
-
-    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
-        try:
-            super().__init__(domain=domain, client_func=client_func, **kwargs)
-        except TypeError:
-            super().__init__()  # If this is last mixin, super() will be object()
-        self._domain = domain
-        self._client_func = client_func
-
-    @exec_with_token
     def list_fact_types(self):
         """
         Returns a list of fact types available for the current domain and auth
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
-        return [fact.model_dump() for fact in policy_api.domain_list_fact_types(self._domain).fact_types]
+        return [fact.model_dump() for fact in openapi_client.PolicyApi(self.authz.get_client()).domain_list_fact_types(self.domain_id).fact_types]
 
-    @exec_with_token
     def list_facts(self, fact_type: str):
         """
         Returns a list of facts for the given fact type
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
-        return [fact.model_dump() for fact in policy_api.domain_list_facts(self._domain, fact_type=fact_type).facts]
+        return [fact.model_dump() for fact in openapi_client.PolicyApi(self.authz.get_client()).domain_list_facts(self.domain_id, fact_type=fact_type).facts]
 
-    @exec_with_token
     def add_fact_type(
         self,
         name: str,
         description: str,
         arguments: Dict[str, str],
     ) -> None:
         """
         Upserts a fact type for the current domain and auth
 
         :param name: The "type name" for this fact, like "has_role"
         :param description: The human-readable description of the fact type
         :param arguments: Name:description argument pairs for the fact type
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
-        policy_api.domain_put_fact_type(
-            domain_id=self._domain,
+        openapi_client.PolicyApi(self.authz.get_client()).domain_put_fact_type(
+            domain_id=self.domain_id,
             fact_type=name,
             new_fact_type_definition=openapi_client.NewFactTypeDefinition(
                 description=description,
                 arguments=[
                     openapi_client.NewFactTypeDefinitionArgumentsInner(name=name, description=desc)
                     for name, desc in arguments.items()
                 ]
             ),
         )
 
-    @exec_with_token
     def add_fact(
         self,
         fact_type: str,
         *arguments: str,
     ) -> Dict[str, Any]:
         """
         Upserts a fact for the current domain and auth
 
         :param fact_type: The name of the type of fact being added
         :param arguments: The fact arguments to add
         :return: The upserted fact
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
-        return policy_api.domain_upsert_fact(
-            domain_id=self._domain,
+        return openapi_client.PolicyApi(self.authz.get_client()).domain_upsert_fact(
+            domain_id=self.domain_id,
             fact_type=fact_type,
             new_fact=openapi_client.NewFact(arguments=arguments)
         ).model_dump()
 
-    @exec_with_token
     def get_fact_type(self, fact_type: str) -> Dict[str, Any]:
         """
         Get the fact type details for the given fact type
 
         :param fact_type: The "type name" for this fact, like "has_role"
         :return: The fact type details
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
-        return policy_api.domain_get_fact_type(
-            domain_id=self._domain, fact_type=fact_type
+        return openapi_client.PolicyApi(self.authz.get_client()).domain_get_fact_type(
+            domain_id=self.domain_id, fact_type=fact_type
         ).model_dump()
 
-    @exec_with_token
     def get_fact(self, fact_type: str, fact_id: str) -> Dict[str, Any]:
         """
         Returns the fact details for the given fact type and name
 
         :param fact_type: The "type name" for this fact, like "has_role"
         :param fact_id: The ID for the fact to be retrieved
         :return: The fact details
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
-        return policy_api.domain_get_fact_by_id(
-            domain_id=self._domain, fact_type=fact_type, fact_id=fact_id
+        return openapi_client.PolicyApi(self.authz.get_client()).domain_get_fact_by_id(
+            domain_id=self.domain_id, fact_type=fact_type, fact_id=fact_id
         ).model_dump()
 
-    @exec_with_token
     def delete_fact_type(self, fact_type: str) -> None:
         """
         Delete a fact type AND ALL FACTS INSIDE IT.
 
         :param fact_type: The "type name" for this fact, like "has_role"
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
-        policy_api.domain_delete_fact_type(domain_id=self._domain, fact_type=fact_type, confirm=fact_type)
+        openapi_client.PolicyApi(self.authz.get_client()).domain_delete_fact_type(domain_id=self.domain_id, fact_type=fact_type, confirm=fact_type)
 
-    @exec_with_token
     def delete_fact(
         self,
         fact_type: str,
         *arguments: str,
         fact_id: Optional[str] = None,
     ) -> None:
         """
@@ -133,27 +107,24 @@
         are provided, each must fully match the name and/or arguments of the fact
         for it to be deleted.
 
         :param fact_type: The "type name" for this fact, like "has_role"
         :param fact_id: The ID for the fact to be deleted
         :param arguments: The arguments for the fact to be deleted
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
         if fact_id is None and arguments is not None:
             for fact in self.list_facts(fact_type=fact_type):
                 if list(arguments) == fact.get("arguments", []):
-                    policy_api.domain_delete_fact_by_id(
-                        domain_id=self._domain, fact_type=fact_type, fact_id=fact["id"])
+                    openapi_client.PolicyApi(self.authz.get_client()).domain_delete_fact_by_id(
+                        domain_id=self.domain_id, fact_type=fact_type, fact_id=fact["id"])
         else:
-            policy_api.domain_delete_fact_by_id(domain_id=self._domain, fact_type=fact_type, fact_id=fact_id)
+            openapi_client.PolicyApi(self.authz.get_client()).domain_delete_fact_by_id(domain_id=self.domain_id, fact_type=fact_type, fact_id=fact_id)
 
-    @exec_with_token
     def delete_all_facts(self, fact_type: str) -> None:
         """
         Delete all the facts for the given fact type.
 
         :param fact_type: The "type name" for this fact, like "has_role"
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
         for fact in self.list_facts(fact_type=fact_type):
-            policy_api.domain_delete_fact_by_id(
-                domain_id=self._domain, fact_type=fact_type, fact_id=fact["id"])
+            openapi_client.PolicyApi(self.authz.get_client()).domain_delete_fact_by_id(
+                domain_id=self.domain_id, fact_type=fact_type, fact_id=fact["id"])
```

## antimatter/session_mixins/general_mixin.py

```diff
@@ -1,118 +1,94 @@
 from datetime import datetime, timezone
 from typing import Any, Callable, Dict, Iterator, List, Optional
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 from antimatter.builders.settings_patch import SettingsPatchBuilder
 from antimatter.session_mixins.serializers.identity_details import serialize_identity_provider_info_dict
-from antimatter.session_mixins.token import exec_with_token
 
+from antimatter.session_mixins.base import BaseMixin
 
-class GeneralMixin:
+
+class GeneralMixin(BaseMixin):
     """
     Session mixin defining CRUD functionality for other general functionality.
-
-    :param domain: The domain to use for the session.
-    :param client: The client to use for the session.
     """
-
     _page_res_size: int = 100
 
-    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
-        try:
-            super().__init__(domain=domain, client_func=client_func, **kwargs)
-        except TypeError:
-            super().__init__()  # If this is last mixin, super() will be object()
-        self._domain = domain
-        self._client_func = client_func
-
-    @exec_with_token
     def get_private_info(self) -> Dict[str, Any]:
         """
         Returns a Domain's summary information.
 
         :return: The private summary info for a domain
         """
         # Disable warnings because of a bug in DomainIdentityProviderDetails autogenerated code
-        general_api = openapi_client.GeneralApi(api_client=self._client_func())
-        res = general_api.domain_get_private_info(domain_id=self._domain).model_dump(warnings=False)
+        res = openapi_client.GeneralApi(self.authz.get_client()).domain_get_private_info(domain_id=self.domain_id).model_dump(warnings=False)
         if "identity_providers" in res:
             res["identity_providers"] = [
                 serialize_identity_provider_info_dict(prov) for prov in res["identity_providers"]
             ]
         return res
 
     def get_public_info(self) -> Dict[str, Any]:
         """
         Returns a Domain's summary information. This endpoint does not require
         authorization
 
         :return: The public summary info for a domain
         """
         # Disable warnings because of a bug in DomainIdentityProviderDetails autogenerated code
-        general_api = openapi_client.GeneralApi(api_client=self._client_func())
-        res = general_api.domain_get_public_info(domain_id=self._domain).model_dump(warnings=False)
+        res = openapi_client.GeneralApi(self.authz.get_client()).domain_get_public_info(domain_id=self.domain_id).model_dump(warnings=False)
         if "identity_providers" in res:
             res["identity_providers"] = [
                 serialize_identity_provider_info_dict(prov) for prov in res["identity_providers"]
             ]
         return res
 
-    @exec_with_token
     def get_settings(self) -> Dict[str, Any]:
         """
         Return the domain settings.
         """
-        general_api = openapi_client.GeneralApi(api_client=self._client_func())
-        return general_api.domain_get_settings(domain_id=self._domain).model_dump()
+        return openapi_client.GeneralApi(self.authz.get_client()).domain_get_settings(domain_id=self.domain_id).model_dump()
 
-    @exec_with_token
     def patch_settings(self, *patch: SettingsPatchBuilder) -> Dict[str, Any]:
         """
         Applies the given patch to the domain settings. The user must have
         permissions on all resources the patch references.
 
         :param patch: The patch or patches to make to the settings. The path is the patch is
                         a JSON pointer path.
         :return: The domain settings after applying the patch
         """
-        general_api = openapi_client.GeneralApi(api_client=self._client_func())
-        return general_api.domain_patch_settings(
-            domain_id=self._domain,
-            domain_settings_patch=openapi_client.DomainSettingsPatch(patch=[p.build() for p in patch])
+        return openapi_client.GeneralApi(self.authz.get_client()).domain_patch_settings(
+            domain_id=self.domain_id,
+            domain_settings_patch=openapi_client.DomainSettingsPatch(patch=[p.build() for p in patch if p is not None])
         ).model_dump()
 
-    @exec_with_token
     def get_status(self) -> Dict[str, Any]:
         """
         Return the domain status, which contains important notifications for
         administrators of the domain.
         """
-        general_api = openapi_client.GeneralApi(api_client=self._client_func())
-        return general_api.domain_get_status(domain_id=self._domain).model_dump()
+        return openapi_client.GeneralApi(self.authz.get_client()).domain_get_status(domain_id=self.domain_id).model_dump()
 
-    @exec_with_token
     def list_hooks(self) -> List[Dict[str, Any]]:
         """
         Return a list of available hooks in this domain. A hook is a data processor,
         like a PII classifier
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        return [h.model_dump() for h in contexts_api.domain_list_hooks(domain_id=self._domain).hooks]
+        return [h.model_dump() for h in openapi_client.ContextsApi(self.authz.get_client()).domain_list_hooks(domain_id=self.domain_id).hooks]
 
-    @exec_with_token
-    def list_resources(self) -> Dict[str, Any]:
+    def list_resources(self) -> List[Dict[str, Any]]:
         """
         Return a list of resource strings that can be used in policy rules, and
         the set of permissions that you can assign to them.
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
-        return policy_api.domain_list_resources(domain_id=self._domain).model_dump()
+        res = openapi_client.PolicyApi(self.authz.get_client()).domain_list_resources(domain_id=self.domain_id)
+        return [r.model_dump() for r in res.var_schema]
 
-    @exec_with_token
     def query_access_log(
         self,
         start_date: Optional[datetime] = None,
         end_date: Optional[datetime] = None,
         session: Optional[str] = None,
         location: Optional[str] = None,
         location_prefixed: Optional[bool] = None,
@@ -151,15 +127,14 @@
                     not specified, this field is ignored
         :param redacted_or_tokenized_tag: The redacted or tokenized tag key you would like ot filter on. This accepts
                     a tag key only and will return all redacted and tokenized tag key results
                     matching the provided tag key. If not specified, this field is ignored
         :param capsule_id: The ID for a specific capsule. Use this to limit results to a single capsule
         :return: An iterator over the access logs matching the filters
         """
-        capsules_api = openapi_client.CapsulesApi(api_client=self._client_func())
         pagination = None
         has_more = True
         if start_date is not None:
             start_date = start_date.astimezone(timezone.utc)
         if end_date is not None:
             end_date = end_date.astimezone(timezone.utc)
         while has_more:
@@ -172,25 +147,24 @@
                 "location": location,
                 "location_prefixed": location_prefixed,
                 "operation_type": operation_type,
                 "allowed_tag": allowed_tag,
                 "redacted_or_tokenized_tag": redacted_or_tokenized_tag,
             }
             if capsule_id is None:
-                res = capsules_api.domain_query_access_log(domain_id=self._domain, **kwargs)
+                res = openapi_client.CapsulesApi(self.authz.get_client()).domain_query_access_log(domain_id=self.domain_id, **kwargs)
             else:
-                res = capsules_api.domain_query_access_log_single_capsule(
-                    domain_id=self._domain, capsule_id=capsule_id, **kwargs,
+                res = openapi_client.CapsulesApi(self.authz.get_client()).domain_query_access_log_single_capsule(
+                    domain_id=self.domain_id, capsule_id=capsule_id, **kwargs,
                 )
             has_more = res.has_more
             for log in res.results:
                 pagination = log.id
                 yield log.model_dump()
 
-    @exec_with_token
     def query_control_log(
         self,
         start_date: Optional[datetime] = None,
         end_date: Optional[datetime] = None,
         session: Optional[str] = None,
         url: Optional[str] = None,
         description: Optional[str] = None,
@@ -214,24 +188,23 @@
                     will return results starting with the provided string. If not specified,
                     this field is ignored
         :param description: The description you would like to filter on. This is an in matched filter
                     and will return results that  contain the provided string. If not specified,
                     this field is ignored
         :return: An iterator over the control logs matching the filters
         """
-        general_api = openapi_client.GeneralApi(api_client=self._client_func())
         pagination = None
         has_more = True
         if start_date is not None:
             start_date = start_date.astimezone(timezone.utc)
         if end_date is not None:
             end_date = end_date.astimezone(timezone.utc)
         while has_more:
-            res = general_api.domain_query_control_log(
-                domain_id=self._domain,
+            res = openapi_client.GeneralApi(self.authz.get_client()).domain_query_control_log(
+                domain_id=self.domain_id,
                 start_date=start_date,
                 end_date=end_date,
                 num_results=self._page_res_size,
                 start_from_id=pagination,
                 session=session,
                 url=url,
                 description=description,
```

## antimatter/session_mixins/identity_provider_mixin.py

```diff
@@ -1,93 +1,82 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 from antimatter.constants.identity_provider import PrincipalType, ProviderType
 from antimatter.session_mixins.serializers.identity_details import serialize_identity_principal_details_dict, \
     serialize_identity_provider_info_dict
-from antimatter.session_mixins.token import exec_with_token
-from antimatter.capabilities import CapabilityConverter
+
+from antimatter.converters import CapabilityConverter
+from antimatter.session_mixins.base import BaseMixin
 
 
 class OverrideDomainIdentityPrincipalDetails(openapi_client.DomainIdentityPrincipalDetails):
     """
     This override provides a local way to pass domain identity principal details
     to the openapi generated client that mitigates the pydantic serializing error
     it produces due to a bug in the generator.
 
     The code that the generator currently produces looks like:
-    ```
-    one_of_schemas: List[str] = Literal["APIKeyDomainIdentityProviderDetails", "GoogleOAuthDomainIdentityProviderDetails"]
-    ```
+    .. code-block:: python
+
+        one_of_schemas: List[str] = Literal["APIKeyDomainIdentityProviderDetails", "GoogleOAuthDomainIdentityProviderDetails"]
+
     that will produce the error:
-    ```
-    /Users/daniel/.pyenv/versions/pycapsule-3.11/lib/python3.11/site-packages/pydantic/main.py:308: UserWarning: Pydantic serializer warnings:
-    Expected `list[str]` but got `_LiteralGenericAlias` - serialized value may not be as expected
-    return self.__pydantic_serializer__.to_python(
-    ```
+
+    .. code-block:: text
+
+        /Users/daniel/.pyenv/versions/pycapsule-3.11/lib/python3.11/site-packages/pydantic/main.py:308: UserWarning: Pydantic serializer warnings:
+        Expected `list[str]` but got `_LiteralGenericAlias` - serialized value may not be as expected
+        return self.__pydantic_serializer__.to_python(
+
     """
     one_of_schemas: List[str] = [
         "DomainIdentityAPIKeyPrincipalParams",
         "DomainIdentityEmailPrincipalParams",
         "DomainIdentityHostedDomainPrincipalParams",
     ]
 
 
-class IdentityProviderMixin:
+class IdentityProviderMixin(BaseMixin):
     """
     Session mixin defining identity provider CRUD functionality.
-
-    :param domain: The domain to use for the session.
-    :param client: The client to use for the session.
     """
-
-    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
-        try:
-            super().__init__(domain=domain, client_func=client_func, **kwargs)
-        except TypeError:
-            super().__init__()  # If this is last mixin, super() will be object()
-        self._domain = domain
-        self._client_func = client_func
-
-    @exec_with_token
     def upsert_identity_provider(
         self,
         provider_name: str,
         provider_type: Union[str, ProviderType] = ProviderType.ApiKey,
         client_id: Optional[str] = None,
     ) -> Dict[str, Any]:
         """
         Create or update an identity provider.
 
         :param provider_name: The name of a new or existing identity provider
         :param provider_type: The provider type for identity management
         :param client_id: If the provider type is 'GoogleOAuth', a client ID must be provided
         :return: The identity provider summary
         """
-        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
         provider_type = ProviderType(provider_type)
         provider_params = None
         if ProviderType(provider_type) is ProviderType.GoogleOAuth:
             provider_params = openapi_client.GoogleOAuthDomainIdentityProviderDetails(
                 type=ProviderType.GoogleOAuth.value,
                 client_id=client_id,
             )
         elif ProviderType(provider_type) is ProviderType.ApiKey:
             provider_params = openapi_client.APIKeyDomainIdentityProviderDetails(
                 type=ProviderType.ApiKey.value,
             )
         # Disable warnings because of a bug in DomainIdentityProviderDetails autogenerated code
-        res = auth_api.domain_upsert_identity_provider(
-            domain_id=self._domain,
+        res = openapi_client.AuthenticationApi(self.authz.get_client()).domain_upsert_identity_provider(
+            domain_id=self.domain_id,
             identity_provider_name=provider_name,
             domain_identity_provider_details=openapi_client.DomainIdentityProviderDetails(provider_params)
         ).model_dump(warnings=False)
         return serialize_identity_provider_info_dict(res)
 
-    @exec_with_token
     def insert_identity_provider_principal(
         self,
         provider_name: str,
         capabilities: List[Union[str, Dict[str, Any]]],
         principal_type: Union[str, PrincipalType],
         principal_value: Optional[str] = None,
         comment: Optional[str] = None,
@@ -105,15 +94,14 @@
                 - A list of dictionaries as a name/value pair, like [{"name": "admin", "value": "True"}, {"name": "read_only", "value": "False"}]
                 - Any combination of the above
         :param principal_type: The type of principal to create. One of 'APIKey', 'Email', or 'HostedDomain'
         :param principal_value: The appropriate identifying value for the principal, depending on type
         :param comment: An optional comment for the identity provider principal
         :return: The ID of the inserted principal and any additional metadata
         """
-        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
         capabilities = CapabilityConverter.convert_capabilities(capabilities)
         principal_type = PrincipalType(principal_type)
         inner_params = None
         if PrincipalType(principal_type) is PrincipalType.ApiKey:
             inner_params = openapi_client.DomainIdentityAPIKeyPrincipalParams(
                 type=principal_type.value, api_key_id=principal_value,
                 comment=comment,
@@ -122,24 +110,23 @@
             inner_params = openapi_client.DomainIdentityEmailPrincipalParams(
                 type=principal_type.value, email=principal_value, comment=comment,
             )
         elif PrincipalType(principal_type) is PrincipalType.HostedDomain:
             inner_params = openapi_client.DomainIdentityHostedDomainPrincipalParams(
                 type=principal_type.value, hosted_domain=principal_value, comment=comment,
             )
-        return auth_api.domain_insert_identity_provider_principal(
-            domain_id=self._domain,
+        return openapi_client.AuthenticationApi(self.authz.get_client()).domain_insert_identity_provider_principal(
+            domain_id=self.domain_id,
             identity_provider_name=provider_name,
             domain_identity_provider_principal_params=openapi_client.DomainIdentityProviderPrincipalParams(
                 capabilities=[openapi_client.Capability(name=k, value=v) for k, v in capabilities.items()],
                 details=OverrideDomainIdentityPrincipalDetails(inner_params)
             ),
         ).model_dump(exclude_none=True)
 
-    @exec_with_token
     def update_identity_provider_principal(
         self,
         provider_name: str,
         principal_id: str,
         capabilities: List[Union[str, Dict[str, Any]]],
     ) -> None:
         """
@@ -150,113 +137,102 @@
         :param capabilities: The capabilities to attach to the principal. These can be in one of the following forms:
                 - A list of unary capabilities, like ['admin', 'read_only']
                 - A list of key-value pairs, like ["admin=True", "read_only=False"]
                 - A list of dictionaries, like [{"admin": "True"}, {"read_only": "False"}]
                 - A list of dictionaries as a name/value pair, like [{"name": "admin", "value": "True"}, {"name": "read_only", "value": "False"}]
                 - Any combination of the above
         """
-        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
         capabilities = CapabilityConverter.convert_capabilities(capabilities)
-        auth_api.domain_update_identity_provider_principal(
-            domain_id=self._domain,
+        openapi_client.AuthenticationApi(self.authz.get_client()).domain_update_identity_provider_principal(
+            domain_id=self.domain_id,
             identity_provider_name=provider_name,
             principal_id=principal_id,
             capability_list=openapi_client.CapabilityList(
                 capabilities=[openapi_client.Capability(name=k, value=v) for k, v in capabilities.items()]
             ),
         )
 
-    @exec_with_token
     def get_identity_provider(self, provider_name: str) -> Dict[str, Any]:
         """
         Retrieve detailed information and configuration of an identity provider
 
         :param provider_name: The name of an existing identity provider
         :return: The identity provider details
         """
-        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
-        res = auth_api.domain_get_identity_provider(
-            domain_id=self._domain, identity_provider_name=provider_name,
+        res = openapi_client.AuthenticationApi(self.authz.get_client()).domain_get_identity_provider(
+            domain_id=self.domain_id, identity_provider_name=provider_name,
         ).model_dump(warnings=False)
         return serialize_identity_provider_info_dict(res)
 
-    @exec_with_token
     def list_identity_providers(self) -> List[Dict[str, Any]]:
         """
         Retrieve the domain's identity providers and a brief overview of their
         configuration.
         """
-        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
-        res = auth_api.domain_list_identity_providers(domain_id=self._domain)
+        res = openapi_client.AuthenticationApi(self.authz.get_client()).domain_list_identity_providers(domain_id=self.domain_id)
         if not res.identity_providers:
             return []
 
         # Disable warnings because of a bug in DomainIdentityProviderDetails autogenerated code
         return [
             serialize_identity_provider_info_dict(prov.model_dump(warnings=False))
             for prov in res.identity_providers
         ]
 
-    @exec_with_token
     def get_identity_provider_principal(
         self,
         provider_name: str,
         principal_id: Optional[str] = None,
     ) -> Union[List[Dict[str, Any]], Dict[str, Any]]:
         """
         Get either a summary of all the principals for an identity provider, or
         detailed information about a single principal if a principal_id is
         provided
 
         :param provider_name: The name of an existing identity provider
         :param principal_id: The ID of the principal; None to get all principals
         :return: The principal information
         """
-        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
         if principal_id is None:
-            res = auth_api.domain_get_identity_provider_principals(
-                domain_id=self._domain, identity_provider_name=provider_name,
+            res = openapi_client.AuthenticationApi(self.authz.get_client()).domain_get_identity_provider_principals(
+                domain_id=self.domain_id, identity_provider_name=provider_name,
             )
             principals = []
             for principal in res.principals:
                 principal = principal.model_dump()
                 if t := principal.get("principal_type"):
                     principal["principal_type"] = t.value
                 principals.append(principal)
             return principals
         else:
-            res = auth_api.domain_get_identity_provider_principal(
-                domain_id=self._domain,
+            res = openapi_client.AuthenticationApi(self.authz.get_client()).domain_get_identity_provider_principal(
+                domain_id=self.domain_id,
                 identity_provider_name=provider_name,
                 principal_id=principal_id,
             )
             return serialize_identity_principal_details_dict(res.model_dump(warnings=False))
 
-    @exec_with_token
     def delete_identity_provider(self, provider_name: str) -> None:
         """
         Delete an identity provider. All domain tokens created using this
         identity provider will be invalidated. Take care not to remove the
         identity provider that is providing you admin access to your domain, as
         you may lock yourself out.
 
         :param provider_name: The name of the identity provider to fully delete
         """
-        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
-        auth_api.domain_delete_identity_provider(domain_id=self._domain, identity_provider_name=provider_name)
+        openapi_client.AuthenticationApi(self.authz.get_client()).domain_delete_identity_provider(domain_id=self.domain_id, identity_provider_name=provider_name)
 
-    @exec_with_token
     def delete_identity_provider_principal(
         self, provider_name: str, principal_id: str,
     ) -> None:
         """
         Delete an identity provider principal.
 
         :param provider_name: The name of the identity provider to delete a principal from
         :param principal_id: The ID of the principal to delete
         """
-        auth_api = openapi_client.AuthenticationApi(api_client=self._client_func())
-        auth_api.domain_delete_identity_provider_principal(
-            domain_id=self._domain,
+        openapi_client.AuthenticationApi(self.authz.get_client()).domain_delete_identity_provider_principal(
+            domain_id=self.domain_id,
             identity_provider_name=provider_name,
             principal_id=principal_id,
         )
```

## antimatter/session_mixins/policy_rule_mixin.py

```diff
@@ -1,33 +1,22 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 from antimatter.constants import domain_policy
 from antimatter.builders.capability import CapabilityRulesBuilder
 from antimatter.builders.fact_policy import FactPoliciesBuilder
-from antimatter.session_mixins.token import exec_with_token
 
+from antimatter.session_mixins.base import BaseMixin
 
-class PolicyRuleMixin:
+
+class PolicyRuleMixin(BaseMixin):
     """
     Session mixin defining policy rule CRUD functionality.
-
-    :param domain: The domain to use for the session.
-    :param client: The client to use for the session.
     """
 
-    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
-        try:
-            super().__init__(domain=domain, client_func=client_func, **kwargs)
-        except TypeError:
-            super().__init__()  # If this is last mixin, super() will be object()
-        self._domain = domain
-        self._client_func = client_func
-
-    @exec_with_token
     def create_policy_rule(
             self,
             capability_rules: CapabilityRulesBuilder,
             path: str,
             operation: Union[str, domain_policy.Operation],
             result: Union[str, domain_policy.Result],
             priority: int = 0,
@@ -43,55 +32,49 @@
         :param path: The path this rule governs. May contain glob expressions (e.g. '*' and '**')
         :param operation: The operation to apply the policy to
         :param result: Whether to 'allow' or 'deny' the operation performed that matches this rule
         :param priority: The priority of this rule. Lower priority rules are evaluated first
         :param disabled: If this rule is disabled or not
         :return: A dictionary containing the created rule from the server
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
-        res = policy_api.domain_create_policy_rule(
-            domain_id=self._domain,
+        res = openapi_client.PolicyApi(self.authz.get_client()).domain_create_policy_rule(
+            domain_id=self.domain_id,
             new_domain_policy_rule=openapi_client.NewDomainPolicyRule(
-                domain_identity=capability_rules.build(),
-                facts=facts.build(),
+                domain_identity=capability_rules.build() if capability_rules is not None else None,
+                facts=facts.build() if facts is not None else [],
                 path=path,
                 operation=domain_policy.Operation(operation).value,
                 result=domain_policy.Result(result).value,
                 priority=priority,
                 disabled=disabled,
             ),
         )
         policy_rule = res.model_dump()
         return policy_rule
 
-    @exec_with_token
     def delete_policy_rule(self, rule_id: str):
         """
         Delete a domain policy rule on the session's domain.
 
         :param rule_id: Identifier of the policy rule to delete
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
-        policy_api.domain_delete_policy_rule(domain_id=self._domain, rule_id=rule_id)
+        openapi_client.PolicyApi(self.authz.get_client()).domain_delete_policy_rule(domain_id=self.domain_id, rule_id=rule_id)
 
-    @exec_with_token
     def list_policy_rules(self):
         """
         Get the domain's policy rules.
 
         :return: A list of policy rules.
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
-        res = policy_api.domain_list_policy_rules(domain_id=self._domain)
+        res = openapi_client.PolicyApi(self.authz.get_client()).domain_list_policy_rules(domain_id=self.domain_id)
         policy_rules = []
         for rule in res.rules:
             policy_rules.append(rule.model_dump())
         return policy_rules
 
-    @exec_with_token
     def update_policy_rule(
         self,
         rule_id: str,
         capability_rules: CapabilityRulesBuilder,
         facts: FactPoliciesBuilder,
         path: str,
         operation: Union[str, domain_policy.Operation],
@@ -108,35 +91,32 @@
                     These assertions will be ANDed together, and ANDed with the capability rules.
         :param path: The path this rule governs. May contain glob expressions (e.g. '*' and '**')
         :param operation: The operation to apply the policy to
         :param result: Whether to 'allow' or 'deny' the operation performed that matches this rule
         :param priority: The priority of this rule. Lower priority rules are evaluated first
         :param disabled: If this rule is disabled or not
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
-        policy_api.domain_update_policy_rule(
-            domain_id=self._domain,
+        openapi_client.PolicyApi(self.authz.get_client()).domain_update_policy_rule(
+            domain_id=self.domain_id,
             rule_id=rule_id,
             new_domain_policy_rule=openapi_client.NewDomainPolicyRule(
-                domain_identity=capability_rules.build(),
-                facts=facts.build(),
+                domain_identity=capability_rules.build() if capability_rules is not None else None,
+                facts=facts.build() if facts is not None else None,
                 path=path,
                 operation=domain_policy.Operation(operation).value,
                 result=domain_policy.Result(result).value,
                 priority=priority,
                 disabled=disabled,
             ),
         )
 
-    @exec_with_token
     def renumber_policy_rules(self) -> List[Dict[str, Any]]:
         """
         Re-assign rule priority numbers for the session's domain to integer multiples of 10
 
         :return: The full list of renumbered policy rules in this domain
         """
-        policy_api = openapi_client.PolicyApi(api_client=self._client_func())
-        res = policy_api.domain_renumber_policy_rules(domain_id=self._domain)
+        res = openapi_client.PolicyApi(self.authz.get_client()).domain_renumber_policy_rules(domain_id=self.domain_id)
         policy_rules = []
         for rule in res.rules:
             policy_rules.append(rule.model_dump())
         return policy_rules
```

## antimatter/session_mixins/read_context_mixin.py

```diff
@@ -1,166 +1,143 @@
 from typing import Any, Callable, Dict, List
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 from antimatter.builders import ReadContextBuilder, ReadContextRuleBuilder
-from antimatter.session_mixins.token import exec_with_token
 
+from antimatter.session_mixins.base import BaseMixin
 
-class ReadContextMixin:
+
+class ReadContextMixin(BaseMixin):
     """
     Session mixin defining CRUD functionality for read contexts.
-
-    :param domain: The domain to use for the session.
-    :param client: The client to use for the session.
     """
-    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
-        try:
-            super().__init__(domain=domain, client_func=client_func, **kwargs)
-        except TypeError:
-            super().__init__()  # If this is last mixin, super() will be object()
-        self._domain = domain
-        self._client_func = client_func
-
-    @exec_with_token
     def add_read_context(
         self,
         name: str,
         builder: ReadContextBuilder
     ) -> None:
         """
         Upserts a read context for the current domain and auth
 
         :param name: The name of the read context to add or update
         :param builder: The builder containing read context configuration
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        contexts_api.domain_upsert_read_context(
-            domain_id=self._domain, context_name=name, add_read_context=builder.build(),
+        if builder is None:
+            raise ValueError("Read context builder is required")
+        openapi_client.ContextsApi(self.authz.get_client()).domain_upsert_read_context(
+            domain_id=self.domain_id, context_name=name, add_read_context=builder.build(),
         )
 
-    @exec_with_token
     def list_read_context(self) -> List[Dict[str, Any]]:
         """
         Returns a list of read contexts available for the current domain and auth
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        return [ctx.model_dump() for ctx in contexts_api.domain_list_read_contexts(self._domain).read_contexts]
+        return [ctx.model_dump() for ctx in openapi_client.ContextsApi(self.authz.get_client()).domain_list_read_contexts(self.domain_id).read_contexts]
 
-    @exec_with_token
     def describe_read_context(self, name: str) -> Dict[str, Any]:
         """
         Returns the read context with the given name for the current domain and auth
 
         :param name: The name of the read context to describe
         :return: The full details of the read context
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        return contexts_api.domain_get_read_context(self._domain, context_name=name).model_dump()
+        return openapi_client.ContextsApi(self.authz.get_client()).domain_get_read_context(self.domain_id, context_name=name).model_dump()
 
-    @exec_with_token
     def delete_read_context(self, name: str) -> None:
         """
         Delete a read context. All configuration associated with this read
         context will also be deleted. Domain policy rules referencing this read
         context will be left as-is.
 
         :param name: The name of the read context to delete
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        contexts_api.domain_delete_read_context(domain_id=self._domain, context_name=name)
+        openapi_client.ContextsApi(self.authz.get_client()).domain_delete_read_context(domain_id=self.domain_id, context_name=name)
 
-    @exec_with_token
     def list_read_context_rules(self, name: str) -> List[Dict[str, Any]]:
         """
         List all rules for the read context
 
         :param name: The name of the read context to list rules from
         :return: The list of read context rules
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        return [r.model_dump() for r in contexts_api.domain_get_read_context(self._domain, context_name=name).rules]
+        return [r.model_dump() for r in openapi_client.ContextsApi(self.authz.get_client()).domain_get_read_context(self.domain_id, context_name=name).rules]
 
-    @exec_with_token
     def add_read_context_rules(
         self,
         name: str,
         rule_builder: ReadContextRuleBuilder,
     ) -> str:
         """
         Adds rules to a read context
 
         :param name: The name of the read context to add rules to
         :param rule_builder: The builder containing rule configuration for the read context
         :return: The unique ID for the added read context rule
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        return contexts_api.domain_add_read_context_rule(
-            domain_id=self._domain,
+        if rule_builder is None:
+            raise ValueError("Read context rule builder is required")
+        return openapi_client.ContextsApi(self.authz.get_client()).domain_add_read_context_rule(
+            domain_id=self.domain_id,
             context_name=name,
-            new_read_context_config_rule=rule_builder.build()
+            new_read_context_config_rule=rule_builder.build(),
         ).id
 
-    @exec_with_token
     def update_read_context_rule(
         self,
         name: str,
         rule_id: str,
         rule_builder: ReadContextRuleBuilder,
     ) -> None:
         """
         Update a read context configuration rule. The rule must already exist.
 
         :param name: The name of the read context to update a rule for
         :param rule_id: The unique ID of the rule to update
         :param rule_builder: The builder containing rule configuration
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        contexts_api.domain_update_read_context_rule(
-            domain_id=self._domain,
+        if rule_builder is None:
+            raise ValueError("Read context rule builder is required")
+        openapi_client.ContextsApi(self.authz.get_client()).domain_update_read_context_rule(
+            domain_id=self.domain_id,
             context_name=name,
             rule_id=rule_id,
             new_read_context_config_rule=rule_builder.build()
         )
 
-    @exec_with_token
     def delete_read_context_rule(
         self,
         name: str,
         rule_id: str,
     ) -> None:
         """
         Deletes a rule from a read context
 
         :param name: The name of the read context to delete a rule from
         :param rule_id: The unique ID of the rule to delete
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        contexts_api.domain_delete_read_context_rule(
-            domain_id=self._domain,
+        openapi_client.ContextsApi(self.authz.get_client()).domain_delete_read_context_rule(
+            domain_id=self.domain_id,
             context_name=name,
             rule_id=rule_id,
         )
 
-    @exec_with_token
     def delete_read_context_rules(self, name: str) -> None:
         """
         Deletes all the read context rules
 
         :param name: The name of the read context to delete all the rules from
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
         for rule in self.list_read_context_rules(name):
-            contexts_api.domain_delete_read_context_rule(
-                domain_id=self._domain,
+            openapi_client.ContextsApi(self.authz.get_client()).domain_delete_read_context_rule(
+                domain_id=self.domain_id,
                 context_name=name,
                 rule_id=rule["id"],
             )
 
-    @exec_with_token
     def flush_read_context(self, name: str) -> None:
         """
         Flushes the read context and all associated rules
 
         :param name: The name of the read context to flush
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        contexts_api.domain_read_context_flush(domain_id=self._domain, context_name=name)
+        contexts_api = openapi_client.ContextsApi(api_client=self.authz.get_client())
+        contexts_api.domain_read_context_flush(domain_id=self.domain_id, context_name=name)
```

## antimatter/session_mixins/root_encryption_key_mixin.py

```diff
@@ -1,141 +1,118 @@
 from typing import Any, Callable, Dict, List
 
-import antimatter.client as openapi_client
-from antimatter.session_mixins.token import exec_with_token
+import antimatter_api as openapi_client
+from antimatter_api import KeyInfos, ActiveRootEncryptionKeyID
 
+from antimatter.session_mixins.base import BaseMixin
 
-class RootEncryptionKeyMixin:
+
+class RootEncryptionKeyMixin(BaseMixin):
     """
     Session mixin defining CRUD functionality for root encryption keys
-
-    :param domain: The domain to use for the session.
-    :param client: The client to use for the session.
     """
-    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
-        try:
-            super().__init__(domain=domain, client_func=client_func, **kwargs)
-        except TypeError:
-            super().__init__()  # If this is last mixin, super() will be object()
-        self._domain = domain
-        self._client_func = client_func
 
-    @exec_with_token
     def get_active_root_encryption_key(self) -> Dict[str, Any]:
         """
         Get the active root encryption key
 
         :return: The active root encryption key
         """
-        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
-        return encryption_api.domain_get_active_external_root_encryption_key(domain_id=self._domain).model_dump()
+        return openapi_client.EncryptionApi(self.authz.get_client()).domain_get_active_external_root_encryption_key(domain_id=self.domain_id).model_dump()
 
-    @exec_with_token
     def list_root_encryption_keys(self) -> List[Dict[str, Any]]:
         """
         List all root encryption keys
 
         :return: A list of root encryption keys
         """
-        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
-        return [key.model_dump() for key in encryption_api.domain_list_external_root_encryption_key(domain_id=self._domain)]
+        return [key.model_dump() for key in openapi_client.EncryptionApi(self.authz.get_client()).domain_list_external_root_encryption_key(domain_id=self.domain_id)]
 
-    @exec_with_token
     def test_root_encryption_key(self, root_encryption_key_id: str) -> Dict[str, Any]:
         """
         Attempt to test a root encryption key to encrypt and decrypt
 
         :param key: The key to test
         :return: The result of the test
         """
-        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
-        return encryption_api.domain_external_root_encryption_key_test(
-            domain_id=self._domain,root_encryption_key_id=root_encryption_key_id,
+        return openapi_client.EncryptionApi(self.authz.get_client()).domain_external_root_encryption_key_test(
+            domain_id=self.domain_id,root_encryption_key_id=root_encryption_key_id,
             body={}
         ).model_dump()
     
-    @exec_with_token
-    def add_root_encryption_key(self, key_infos: openapi_client.KeyInfos, description: str = "") -> str:
+    def add_root_encryption_key(self, key_infos: KeyInfos, description: str = "") -> str:
         """
         Add a new root encryption key.
         Use the builder functions in `antimatter.builders.root_encryption_key` to create the key information.
 
         For example:
-        ```
-        key_info = antimatter.builders.antimatter_delegated_aws_key_info(key_arn="key_arn")
-        key_id = session.add_root_encryption_key(key_info)
 
-        key_info = antimatter.builders.aws_service_account_key_info(
-            access_key_id="access_key_id", secret_access_key
-        )
-        key_id = session.add_root_encryption_key(key_info)
+        .. code-block:: python
 
-        key_info = antimatter.builders.gcp_service_account_key_info(
-            service_account_credentials="service_account_credentials", project_id="project_id", location="location"
-        )
-        key_id = session.add_root_encryption_key(key_info)
-        ```
+            key_info = antimatter.builders.antimatter_delegated_aws_key_info(key_arn="key_arn")
+            key_id = session.add_root_encryption_key(key_info)
+
+            key_info = antimatter.builders.aws_service_account_key_info(
+                access_key_id="access_key_id", secret_access_key
+            )
+            key_id = session.add_root_encryption_key(key_info)
+
+            key_info = antimatter.builders.gcp_service_account_key_info(
+                service_account_credentials="service_account_credentials", project_id="project_id", location="location"
+            )
+            key_id = session.add_root_encryption_key(key_info)
 
         :param key_infos: The key information to add
         :param description: The description of the key
         """
         assert key_infos is not None, "Key information is required"
 
-        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
         key_infos.description = description
-        return encryption_api.domain_add_external_root_encryption_key(
-            domain_id=self._domain,
+        return openapi_client.EncryptionApi(self.authz.get_client()).domain_add_external_root_encryption_key(
+            domain_id=self.domain_id,
             key_infos=key_infos
         ).rek_id
 
-    @exec_with_token
     def delete_root_encryption_key(self, root_encryption_key_id: str):
         """
         Delete a root encryption key. Only possible if key is not in use by any data key encryption keys
 
         :param key: The key to delete
         """
-        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
-        encryption_api.domain_delete_external_root_encryption_key(
-            domain_id=self._domain,
+        openapi_client.EncryptionApi(self.authz.get_client()).domain_delete_external_root_encryption_key(
+            domain_id=self.domain_id,
             root_encryption_key_id=root_encryption_key_id
         )
 
-    @exec_with_token
     def set_active_root_encryption_key(self, root_encryption_key_id: str) -> None:
         """
         Set the active root encryption key for the domain
 
         :param key: The key to set as active
         """
-        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
-        encryption_api.domain_set_active_external_root_encryption_key(
-            domain_id=self._domain,
+        openapi_client.EncryptionApi(self.authz.get_client()).domain_set_active_external_root_encryption_key(
+            domain_id=self.domain_id,
             active_root_encryption_key_id=openapi_client.ActiveRootEncryptionKeyID(key_id=root_encryption_key_id)
         )
 
-    @exec_with_token
-    def rotate_encryption_keys(self) -> bool:
+    def rotate_encryption_keys(self) -> None:
         """
         Rotates the root encryption keys. This is a batched operation and if 'True' is
         returned, this indicates whether there are more key encryption keys that can be rotated.
         """
-        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
-        return encryption_api.domain_rotate_root_encryption_keys(
-            domain_id=self._domain, body={},
+        return openapi_client.EncryptionApi(self.authz.get_client()).domain_rotate_root_encryption_keys(
+            domain_id=self.domain_id, body={},
         ).has_more
 
-    @exec_with_token
     def list_key_providers(self) -> List[Dict[str, Any]]:
         """
         Retrieve the domain's key providers and a brief overview of their
         configuration.
         """
-        encryption_api = openapi_client.EncryptionApi(api_client=self._client_func())
-        res = encryption_api.domain_get_external_root_encryption_key_providers(domain_id=self._domain)
+        res = openapi_client.EncryptionApi(self.authz.get_client()).domain_get_external_root_encryption_key_providers(domain_id=self.domain_id)
         if not res.providers:
             return []
         return [
             provider.actual_instance.model_dump()
             for provider in res.providers
             if provider.actual_instance is not None
         ]
```

## antimatter/session_mixins/verification_mixin.py

```diff
@@ -1,48 +1,27 @@
 from typing import Callable, Optional
 
-import antimatter.client as openapi_client
-from antimatter.errors import errors
+import antimatter_api as openapi_client
+from antimatter import errors
+from antimatter.session_mixins.base import BaseMixin
+from antimatter.authz import Authorization
 
-ADMIN_VERIFICATION_PROMPT = (
-    "domain not authenticated - check email to verify account; verification email "
-    "can be sent again with session.resend_verification_email()"
-)
-
-
-class VerificationMixin:
+class VerificationMixin(BaseMixin):
     """
     Session mixin defining CRUD functionality for verification actions.
     """
-
-    def __init__(
-        self,
-        domain: str,
-        client_func: Callable[[], openapi_client.ApiClient],
-        email: Optional[str],
-        **kwargs,
-    ):
-        try:
-            super().__init__(domain=domain, client_func=client_func, email=email, **kwargs)
-        except TypeError:
-            super().__init__()  # If this is last mixin, super() will be object()
-        self._domain = domain
-        self._client_func = client_func
-        self._email = email
-
     def resend_verification_email(self, email: Optional[str] = None):
         """
         Resend the verification email to the admin contact email. If the session
         was called with an email, that will be used if none is provided.
 
         :param email: The email to resend the verification email for.
         """
         if not email and not self._email:
             raise errors.SessionVerificationPendingError("unable to resend verification email: email unknown")
 
-        authentication_api = openapi_client.AuthenticationApi(api_client=self._client_func())
-        authentication_api.domain_contact_issue_verify(
-            domain_id=self._domain,
+        openapi_client.AuthenticationApi(self.authz.get_client()).domain_contact_issue_verify(
+            domain_id=self.domain_id,
             domain_contact_issue_verify_request=openapi_client.DomainContactIssueVerifyRequest(
                 admin_email=email or self._email,
             )
         )
```

## antimatter/session_mixins/write_context_mixin.py

```diff
@@ -1,152 +1,129 @@
 from typing import Any, Callable, Dict, List
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 from antimatter.builders import WriteContextBuilder, WriteContextConfigurationBuilder, WriteContextRegexRuleBuilder
-from antimatter.session_mixins.token import exec_with_token
+from antimatter.session_mixins.base import BaseMixin
 
 
-class WriteContextMixin:
+class WriteContextMixin(BaseMixin):
     """
     Session mixin defining CRUD functionality for write contexts.
-
-    :param domain: The domain to use for the session.
-    :param client: The client to use for the session.
     """
 
-    def __init__(self, domain: str, client_func: Callable[[], openapi_client.ApiClient], **kwargs):
-        try:
-            super().__init__(domain=domain, client_func=client_func, **kwargs)
-        except TypeError:
-            super().__init__()  # If this is last mixin, super() will be object()
-        self._domain = domain
-        self._client_func = client_func
-
-    @exec_with_token
     def add_write_context(
         self,
         name: str,
         builder: WriteContextBuilder,
     ) -> None:
         """
         Upserts a write context for the current domain and auth
 
         :param name: The name of the write context to add or update
         :param builder: The builder containing write context configuration
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        contexts_api.domain_upsert_write_context(
-            domain_id=self._domain, context_name=name, add_write_context=builder.build(),
+        if builder is None:
+            raise ValueError("Write context builder is required")
+        openapi_client.ContextsApi(self.authz.get_client()).domain_upsert_write_context(
+            domain_id=self.domain_id, context_name=name, add_write_context=builder.build(),
         )
 
-    @exec_with_token
     def list_write_context(self) -> List[Dict[str, Any]]:
         """
         Returns a list of write contexts available for the current domain and auth
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        return [ctx.model_dump() for ctx in contexts_api.domain_list_write_contexts(self._domain).write_contexts]
+        return [ctx.model_dump() for ctx in openapi_client.ContextsApi(self.authz.get_client()).domain_list_write_contexts(self.domain_id).write_contexts]
 
-    @exec_with_token
     def describe_write_context(self, name: str) -> Dict[str, Any]:
         """
         Returns the write context with the given name for the current domain and auth
 
         :param name: The name of the write context to describe
         :return: The full details of the write context
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        return contexts_api.domain_describe_write_context(self._domain, context_name=name).model_dump()
+        return openapi_client.ContextsApi(self.authz.get_client()).domain_describe_write_context(self.domain_id, context_name=name).model_dump()
 
-    @exec_with_token
     def upsert_write_context_configuration(
         self,
         name: str,
         builder: WriteContextConfigurationBuilder,
     ) -> None:
         """
         Update a write context configuration. The write context must already exist.
 
         :param name: The name of the write context to update the configuration for
         :param builder: The builder containing write context configuration
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        contexts_api.domain_upsert_write_context_configuration(
-            domain_id=self._domain,
+        if builder is None:
+            raise ValueError("Write context configuration builder is required")
+        openapi_client.ContextsApi(self.authz.get_client()).domain_upsert_write_context_configuration(
+            domain_id=self.domain_id,
             context_name=name,
             write_context_config_info=builder.build(),
         )
 
-    @exec_with_token
     def delete_write_context(self, name: str) -> None:
         """
         Delete a write context. All configuration associated with this write
         context will also be deleted. Domain policy rules referencing this write
         context will be left as-is.
 
         :param name: The name of the write context to delete
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        contexts_api.domain_delete_write_context(domain_id=self._domain, context_name=name)
+        openapi_client.ContextsApi(self.authz.get_client()).domain_delete_write_context(domain_id=self.domain_id, context_name=name)
 
-    @exec_with_token
     def list_write_context_regex_rules(self, context_name: str) -> List[Dict[str, Any]]:
         """
         List all regex rules for the write context.
 
         :param context_name: The name of the write context
         :return: The list of rules
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        return [rule.model_dump() for rule in contexts_api.domain_get_write_context_regex_rules(
-            domain_id=self._domain,
+        return [rule.model_dump() for rule in openapi_client.ContextsApi(self.authz.get_client()).domain_get_write_context_regex_rules(
+            domain_id=self.domain_id,
             context_name=context_name,
         )]
 
-    @exec_with_token
     def insert_write_context_regex_rule(
         self,
         context_name: str,
         builder: WriteContextRegexRuleBuilder,
     ) -> str:
         """
         Create a new regex rule for a write context.
 
         :param context_name: The name of the write context
         :param builder: The builder containing write context regex rule configuration
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        return contexts_api.domain_insert_write_context_regex_rule(
-            domain_id=self._domain,
+        if builder is None:
+            raise ValueError("Write context regex rule builder is required")
+        return openapi_client.ContextsApi(self.authz.get_client()).domain_insert_write_context_regex_rule(
+            domain_id=self.domain_id,
             context_name=context_name,
             write_context_regex_rule=builder.build(),
         ).rule_id
 
-    @exec_with_token
     def delete_write_context_regex_rule(self, context_name: str, rule_id: str) -> None:
         """
         Delete a regex classifier rule for the context.
 
         :param context_name: The name of the write context
         :param rule_id: The ID of the rule to delete
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
-        contexts_api.domain_delete_write_context_regex_rule(
-            domain_id=self._domain,
+        openapi_client.ContextsApi(self.authz.get_client()).domain_delete_write_context_regex_rule(
+            domain_id=self.domain_id,
             context_name=context_name,
             rule_id=rule_id,
         )
 
-    @exec_with_token
     def delete_write_context_regex_rules(self, context_name: str) -> None:
         """
         Delete the regex classifier rules for the context.
 
         :param context_name: The name of the write context
         """
-        contexts_api = openapi_client.ContextsApi(api_client=self._client_func())
         for rule in self.list_write_context_regex_rules(context_name=context_name):
-            contexts_api.domain_delete_write_context_regex_rule(
-                domain_id=self._domain,
+            openapi_client.ContextsApi(self.authz.get_client()).domain_delete_write_context_regex_rule(
+                domain_id=self.domain_id,
                 context_name=context_name,
                 rule_id=rule["id"],
             )
```

## antimatter/session_mixins/serializers/identity_details.py

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, Optional
 
-import antimatter.client as openapi_client
+import antimatter_api as openapi_client
 
 
 def serialize_identity_provider_info_dict(model: Optional[Dict[str, Any]]) -> Optional[Dict[str, Any]]:
     """
     Serialize an identity provider info dictionary
 
     :param model: The identity provider info dictionary
```

## antimatter/tags/tag.py

```diff
@@ -18,15 +18,15 @@
 class SpanTag:
     """
     Defines a span tag manually to the data contained in the cell path. The tag
     is applied to the subset of data contained between start (inclusive) and end
     (exclusive).
 
     The cell path describes which cell to apply this tag to. Cell paths can be
-    created using the antimatter.cell_path.cell_path(cname, rnum) helper function,
+    created using the antimatter.cell_utils.cell_path(cname, rnum) helper function,
     which takes the name of the column and the row number. As an example, if the
     cell to apply this span tag to was in a column named "name" and was in row 10
     of the data, the cell path would be "name[9]" (the first row would be number 0).
     """
     name: str
     start: Optional[int] = None
     end: Optional[int] = None
```

## antimatter/tests/test_capsule.py

```diff
@@ -2,27 +2,29 @@
 
 import pytest
 
 from antimatter.tags import ColumnTag, SpanTag
 from antimatter.capsule import Capsule, CapsuleBindings, _markup_bytes
 import antimatter_engine as ae
 
+
 @pytest.fixture
 def mock_capsule_bindings(monkeypatch, capsule_tags, column_names, column_tags, redacted_data, data_span_tags, extra_info):
     mock_capsule_bindings = CapsuleBindings(None)
     
     # mock the read_all_with_tags method
     monkeypatch.setattr(
         mock_capsule_bindings, 
         'read_all_with_tags', 
-        lambda: (capsule_tags, column_names, column_tags, redacted_data, data_span_tags, extra_info)
+        lambda tags: (capsule_tags, column_names, column_tags, redacted_data, data_span_tags, extra_info)
     )
 
     return mock_capsule_bindings
 
+
 @pytest.mark.parametrize(
     "capsule_tags, column_names, column_tags, redacted_data, data_span_tags, extra_info",
     [
         # Test case 1
         (
             [],  # capsule_tags
             ['email', 'bytes', 'fname', 'bio', 'duration', 'dt', 'float', 'age', 'status', 'id'],  # column_names
@@ -79,15 +81,15 @@
     assert result[1][1]['data'] == b'asdf'
     assert result[1][2]['data'] == 'Bob'
     assert result[1][3]['data'] == 'Born on November 1 1985 in Pittsburg, PA.'
     assert result[1][4]['data'] == datetime.timedelta(0)
     assert result[1][5]['data'] == datetime.datetime.strptime('2024-01-10 14:44:07.625505', "%Y-%m-%d %H:%M:%S.%f")
     assert result[1][6]['data'] == 6.28
     assert result[1][7]['data'] == 0
-    assert result[1][8]['data'] == False
+    assert result[1][8]['data'] is False
     assert result[1][9]['data'] == 33
 
 
 test_data = [
     # Basic non-overlapping
     (
         b"the {redacted} {redacted}",
@@ -164,7 +166,38 @@
     "Partially overlapping tags",
     "Nested overlaps with different starts and ends",
     "Test case with invalid UTF-8 byte",
 ]
 @pytest.mark.parametrize("input_bytes, span_tags, expected_output", test_data, ids=test_ids)
 def test_markup_bytes(input_bytes, span_tags, expected_output):
     assert _markup_bytes(input_bytes, span_tags) == expected_output
+
+
+@pytest.mark.parametrize(
+    ("col_names", "data", "expected_output"),
+    (
+        (["content"], [[b"hello antimatter"]], "hello antimatter"),
+        (["data"], [[b"hello antimatter"]], {"data": "hello antimatter"}),
+        (["data"], [[b"hello"], [b"antimatter"]], [{"data": "hello"}, {"data": "antimatter"}]),
+    ),
+    ids=(
+        "Scalar value",
+        "Dict value",
+        "DictList value",
+    )
+)
+def test_capsule_data_no_extra_info(col_names, data, expected_output):
+    # Be aware that this tests assumes only one column. To support extra columns,
+    # the 'column_tags' and 'data_span_tags' will need to have their shape adjusted
+    # to match
+    cb = CapsuleBindings(None)
+    cb.capsule_tags = []
+    cb.column_names = col_names
+    cb.column_tags = [[]]
+    cb.redacted_data = data
+    cb.data_span_tags = [[[]] for _ in data]
+    cb.extra_info = ""
+
+    cap = Capsule(cb)
+    output = cap.data()
+
+    assert output == expected_output
```

## antimatter/tests/test_cell_path.py

```diff
@@ -1,8 +1,8 @@
-from antimatter.cell_path import cell_path, col_name, row_num
+from antimatter.cell_utils import cell_path, col_name, row_num
 
 
 def test_cell_path():
     cname = "column"
     rnum = 42
     expected = "column[42]"
```

## Comparing `antimatter/cell_path.py` & `antimatter/cell_utils.py`

 * *Files identical despite different names*

## Comparing `antimatter-1.0.0.dist-info/METADATA` & `antimatter-1.1.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 Metadata-Version: 2.1
 Name: antimatter
-Version: 1.0.0
+Version: 1.1.0
 Summary: library for interacting with capsules in various formats
 Author: Antimatter Team
 Author-email: support@antimatter.io
 Requires-Python: >=3.8
+Requires-Dist: antimatter-engine ==1.1.0
+Requires-Dist: antimatter-api ==1.0.7
 Requires-Dist: annotated-types >=0.6
 Requires-Dist: packaging >=21.1
 Requires-Dist: pydantic >=2.0
 Requires-Dist: python-dateutil >=2.1
 Requires-Dist: pyyaml
 Requires-Dist: cbor2 ~=5.5
 Requires-Dist: urllib3 >=2.0.2
-Requires-Dist: antimatter-engine ==1.0.0
+Requires-Dist: google-auth >=2.29.0
+Requires-Dist: requests >=2.31.0
 Provides-Extra: all
 Requires-Dist: langchain >=0.0.341 ; extra == 'all'
 Requires-Dist: faiss-cpu >=1.7.3 ; extra == 'all'
 Requires-Dist: transformers >=4.23 ; extra == 'all'
 Requires-Dist: torch >=2.0 ; extra == 'all'
 Requires-Dist: numpy >=1.23.3 ; extra == 'all'
 Requires-Dist: pandas[performance] >=2.0 ; extra == 'all'
 Requires-Dist: pyarrow >=2.0 ; extra == 'all'
+Requires-Dist: langchain-community >=0.2.0 ; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: pytest >=7.0 ; extra == 'dev'
 Provides-Extra: langchain
 Requires-Dist: langchain >=0.0.341 ; extra == 'langchain'
 Requires-Dist: faiss-cpu >=1.7.3 ; extra == 'langchain'
+Requires-Dist: numpy >=1.26 ; extra == 'langchain'
+Requires-Dist: langchain-community >=0.2.0 ; extra == 'langchain'
 Provides-Extra: langchain-huggingface
 Requires-Dist: langchain >=0.0.341 ; extra == 'langchain-huggingface'
 Requires-Dist: faiss-cpu >=1.7.3 ; extra == 'langchain-huggingface'
 Requires-Dist: transformers >=4.23 ; extra == 'langchain-huggingface'
 Requires-Dist: torch >=2.0 ; extra == 'langchain-huggingface'
+Requires-Dist: numpy >=1.26 ; extra == 'langchain-huggingface'
 Provides-Extra: numpy
 Requires-Dist: numpy >=1.23.3 ; extra == 'numpy'
 Provides-Extra: pandas
 Requires-Dist: pandas[performance] >=1.5 ; extra == 'pandas'
 Provides-Extra: pyarrow
 Requires-Dist: pandas[performance] >=2.0 ; extra == 'pyarrow'
 Requires-Dist: pyarrow >=2.0 ; extra == 'pyarrow'
```

### html2text {}

```diff
@@ -1,23 +1,28 @@
-Metadata-Version: 2.1 Name: antimatter Version: 1.0.0 Summary: library for
+Metadata-Version: 2.1 Name: antimatter Version: 1.1.0 Summary: library for
 interacting with capsules in various formats Author: Antimatter Team Author-
-email: support@antimatter.io Requires-Python: >=3.8 Requires-Dist: annotated-
+email: support@antimatter.io Requires-Python: >=3.8 Requires-Dist: antimatter-
+engine ==1.1.0 Requires-Dist: antimatter-api ==1.0.7 Requires-Dist: annotated-
 types >=0.6 Requires-Dist: packaging >=21.1 Requires-Dist: pydantic >=2.0
 Requires-Dist: python-dateutil >=2.1 Requires-Dist: pyyaml Requires-Dist: cbor2
-~=5.5 Requires-Dist: urllib3 >=2.0.2 Requires-Dist: antimatter-engine ==1.0.0
-Provides-Extra: all Requires-Dist: langchain >=0.0.341 ; extra == 'all'
-Requires-Dist: faiss-cpu >=1.7.3 ; extra == 'all' Requires-Dist: transformers
->=4.23 ; extra == 'all' Requires-Dist: torch >=2.0 ; extra == 'all' Requires-
-Dist: numpy >=1.23.3 ; extra == 'all' Requires-Dist: pandas[performance] >=2.0
-; extra == 'all' Requires-Dist: pyarrow >=2.0 ; extra == 'all' Provides-Extra:
-dev Requires-Dist: pytest >=7.0 ; extra == 'dev' Provides-Extra: langchain
-Requires-Dist: langchain >=0.0.341 ; extra == 'langchain' Requires-Dist: faiss-
-cpu >=1.7.3 ; extra == 'langchain' Provides-Extra: langchain-huggingface
-Requires-Dist: langchain >=0.0.341 ; extra == 'langchain-huggingface' Requires-
-Dist: faiss-cpu >=1.7.3 ; extra == 'langchain-huggingface' Requires-Dist:
-transformers >=4.23 ; extra == 'langchain-huggingface' Requires-Dist: torch
->=2.0 ; extra == 'langchain-huggingface' Provides-Extra: numpy Requires-Dist:
-numpy >=1.23.3 ; extra == 'numpy' Provides-Extra: pandas Requires-Dist: pandas
-[performance] >=1.5 ; extra == 'pandas' Provides-Extra: pyarrow Requires-Dist:
-pandas[performance] >=2.0 ; extra == 'pyarrow' Requires-Dist: pyarrow >=2.0 ;
-extra == 'pyarrow' Provides-Extra: pytorch Requires-Dist: torch >=2.0 ; extra
-== 'pytorch' For more information, please visit the docs at _P_y_t_h_o_n_ _d_o_c_s.
+~=5.5 Requires-Dist: urllib3 >=2.0.2 Requires-Dist: google-auth >=2.29.0
+Requires-Dist: requests >=2.31.0 Provides-Extra: all Requires-Dist: langchain
+>=0.0.341 ; extra == 'all' Requires-Dist: faiss-cpu >=1.7.3 ; extra == 'all'
+Requires-Dist: transformers >=4.23 ; extra == 'all' Requires-Dist: torch >=2.0
+; extra == 'all' Requires-Dist: numpy >=1.23.3 ; extra == 'all' Requires-Dist:
+pandas[performance] >=2.0 ; extra == 'all' Requires-Dist: pyarrow >=2.0 ; extra
+== 'all' Requires-Dist: langchain-community >=0.2.0 ; extra == 'all' Provides-
+Extra: dev Requires-Dist: pytest >=7.0 ; extra == 'dev' Provides-Extra:
+langchain Requires-Dist: langchain >=0.0.341 ; extra == 'langchain' Requires-
+Dist: faiss-cpu >=1.7.3 ; extra == 'langchain' Requires-Dist: numpy >=1.26 ;
+extra == 'langchain' Requires-Dist: langchain-community >=0.2.0 ; extra ==
+'langchain' Provides-Extra: langchain-huggingface Requires-Dist: langchain
+>=0.0.341 ; extra == 'langchain-huggingface' Requires-Dist: faiss-cpu >=1.7.3 ;
+extra == 'langchain-huggingface' Requires-Dist: transformers >=4.23 ; extra ==
+'langchain-huggingface' Requires-Dist: torch >=2.0 ; extra == 'langchain-
+huggingface' Requires-Dist: numpy >=1.26 ; extra == 'langchain-huggingface'
+Provides-Extra: numpy Requires-Dist: numpy >=1.23.3 ; extra == 'numpy'
+Provides-Extra: pandas Requires-Dist: pandas[performance] >=1.5 ; extra ==
+'pandas' Provides-Extra: pyarrow Requires-Dist: pandas[performance] >=2.0 ;
+extra == 'pyarrow' Requires-Dist: pyarrow >=2.0 ; extra == 'pyarrow' Provides-
+Extra: pytorch Requires-Dist: torch >=2.0 ; extra == 'pytorch' For more
+information, please visit the docs at _P_y_t_h_o_n_ _d_o_c_s.
```

