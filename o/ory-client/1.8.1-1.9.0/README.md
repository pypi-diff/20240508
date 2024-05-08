# Comparing `tmp/ory-client-1.8.1.tar.gz` & `tmp/ory-client-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ory-client-1.8.1.tar", last modified: Fri Mar  8 12:35:26 2024, max compression
+gzip compressed data, was "ory-client-1.9.0.tar", last modified: Mon Mar 18 16:51:51 2024, max compression
```

## Comparing `ory-client-1.8.1.tar` & `ory-client-1.9.0.tar`

### file list

```diff
@@ -1,617 +1,617 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 12:35:26.313374 ory-client-1.8.1/
--rw-r--r--   0 root         (0) root         (0)      486 2024-03-08 12:35:26.313374 ory-client-1.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    41345 2024-03-08 12:30:15.000000 ory-client-1.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 12:35:26.213373 ory-client-1.8.1/ory_client/
--rw-r--r--   0 root         (0) root         (0)      835 2024-03-08 12:30:15.000000 ory-client-1.8.1/ory_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 12:35:26.217373 ory-client-1.8.1/ory_client/api/
--rw-r--r--   0 root         (0) root         (0)      214 2024-03-08 12:30:15.000000 ory-client-1.8.1/ory_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12519 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/api/courier_api.py
--rw-r--r--   0 root         (0) root         (0)    23194 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/api/events_api.py
--rw-r--r--   0 root         (0) root         (0)   207385 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/api/frontend_api.py
--rw-r--r--   0 root         (0) root         (0)   110149 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/api/identity_api.py
--rw-r--r--   0 root         (0) root         (0)    40790 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/api/jwk_api.py
--rw-r--r--   0 root         (0) root         (0)    16248 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/api/metadata_api.py
--rw-r--r--   0 root         (0) root         (0)   163217 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/api/o_auth2_api.py
--rw-r--r--   0 root         (0) root         (0)    45439 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/api/oidc_api.py
--rw-r--r--   0 root         (0) root         (0)    32053 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/api/permission_api.py
--rw-r--r--   0 root         (0) root         (0)   104681 2024-03-08 12:30:15.000000 ory-client-1.8.1/ory_client/api/project_api.py
--rw-r--r--   0 root         (0) root         (0)    34599 2024-03-08 12:30:15.000000 ory-client-1.8.1/ory_client/api/relationship_api.py
--rw-r--r--   0 root         (0) root         (0)     5921 2024-03-08 12:30:15.000000 ory-client-1.8.1/ory_client/api/wellknown_api.py
--rw-r--r--   0 root         (0) root         (0)    39202 2024-03-08 12:30:15.000000 ory-client-1.8.1/ory_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 12:35:26.217373 ory-client-1.8.1/ory_client/apis/
--rw-r--r--   0 root         (0) root         (0)     1032 2024-03-08 12:30:15.000000 ory-client-1.8.1/ory_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18031 2024-03-08 12:30:15.000000 ory-client-1.8.1/ory_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5198 2024-03-08 12:30:15.000000 ory-client-1.8.1/ory_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 12:35:26.249373 ory-client-1.8.1/ory_client/model/
--rw-r--r--   0 root         (0) root         (0)      344 2024-03-08 12:30:15.000000 ory-client-1.8.1/ory_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14362 2024-03-08 12:30:12.000000 ory-client-1.8.1/ory_client/model/accept_o_auth2_consent_request.py
--rw-r--r--   0 root         (0) root         (0)    13401 2024-03-08 12:30:12.000000 ory-client-1.8.1/ory_client/model/accept_o_auth2_consent_request_session.py
--rw-r--r--   0 root         (0) root         (0)    18750 2024-03-08 12:30:12.000000 ory-client-1.8.1/ory_client/model/accept_o_auth2_login_request.py
--rw-r--r--   0 root         (0) root         (0)    11650 2024-03-08 12:30:12.000000 ory-client-1.8.1/ory_client/model/active_project_in_console.py
--rw-r--r--   0 root         (0) root         (0)    11685 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/attribute.py
--rw-r--r--   0 root         (0) root         (0)    12253 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/attribute_filter.py
--rw-r--r--   0 root         (0) root         (0)    11965 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/attributes_count_datapoint.py
--rw-r--r--   0 root         (0) root         (0)    13840 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/authenticator_assurance_level.py
--rw-r--r--   0 root         (0) root         (0)    11964 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/batch_patch_identities_response.py
--rw-r--r--   0 root         (0) root         (0)    11792 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/check_opl_syntax_result.py
--rw-r--r--   0 root         (0) root         (0)    11697 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/check_permission_result.py
--rw-r--r--   0 root         (0) root         (0)    11927 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/cloud_account.py
--rw-r--r--   0 root         (0) root         (0)    13875 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/consistency_request_parameters.py
--rw-r--r--   0 root         (0) root         (0)    16213 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/continue_with.py
--rw-r--r--   0 root         (0) root         (0)    12647 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/continue_with_recovery_ui.py
--rw-r--r--   0 root         (0) root         (0)    11867 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/continue_with_recovery_ui_flow.py
--rw-r--r--   0 root         (0) root         (0)    12653 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/continue_with_set_ory_session_token.py
--rw-r--r--   0 root         (0) root         (0)    12647 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/continue_with_settings_ui.py
--rw-r--r--   0 root         (0) root         (0)    11634 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/continue_with_settings_ui_flow.py
--rw-r--r--   0 root         (0) root         (0)    12743 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/continue_with_verification_ui.py
--rw-r--r--   0 root         (0) root         (0)    12337 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/continue_with_verification_ui_flow.py
--rw-r--r--   0 root         (0) root         (0)    12313 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/courier_message_status.py
--rw-r--r--   0 root         (0) root         (0)    12189 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/courier_message_type.py
--rw-r--r--   0 root         (0) root         (0)    13118 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_custom_domain_body.py
--rw-r--r--   0 root         (0) root         (0)    12602 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_event_stream_body.py
--rw-r--r--   0 root         (0) root         (0)    17129 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_identity_body.py
--rw-r--r--   0 root         (0) root         (0)    12268 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_invite_response.py
--rw-r--r--   0 root         (0) root         (0)    12838 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)    11909 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_member_invite_response.py
--rw-r--r--   0 root         (0) root         (0)    11720 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_project_api_key_request.py
--rw-r--r--   0 root         (0) root         (0)    12388 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_project_body.py
--rw-r--r--   0 root         (0) root         (0)    12818 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_project_branding.py
--rw-r--r--   0 root         (0) root         (0)    11650 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_project_member_invite_body.py
--rw-r--r--   0 root         (0) root         (0)   145870 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_project_normalized_payload.py
--rw-r--r--   0 root         (0) root         (0)    12513 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_recovery_code_for_identity_body.py
--rw-r--r--   0 root         (0) root         (0)    12510 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_recovery_link_for_identity_body.py
--rw-r--r--   0 root         (0) root         (0)    12810 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_relationship_body.py
--rw-r--r--   0 root         (0) root         (0)    12912 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_subscription_body.py
--rw-r--r--   0 root         (0) root         (0)    12519 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_subscription_common.py
--rw-r--r--   0 root         (0) root         (0)    12261 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_verifiable_credential_request_body.py
--rw-r--r--   0 root         (0) root         (0)    11656 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_workspace_member_invite_body.py
--rw-r--r--   0 root         (0) root         (0)    11640 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_workspace_payload.py
--rw-r--r--   0 root         (0) root         (0)    12540 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/create_workspace_subscription_body.py
--rw-r--r--   0 root         (0) root         (0)    13492 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/credential_supported_draft00.py
--rw-r--r--   0 root         (0) root         (0)    15192 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/custom_domain.py
--rw-r--r--   0 root         (0) root         (0)    11634 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/delete_my_sessions_count.py
--rw-r--r--   0 root         (0) root         (0)    12057 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/email_template_data.py
--rw-r--r--   0 root         (0) root         (0)    11830 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/email_template_data_body.py
--rw-r--r--   0 root         (0) root         (0)    12160 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/error_authenticator_assurance_level_not_satisfied.py
--rw-r--r--   0 root         (0) root         (0)    12130 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/error_browser_location_change_required.py
--rw-r--r--   0 root         (0) root         (0)    12119 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/error_flow_replaced.py
--rw-r--r--   0 root         (0) root         (0)    11815 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/error_generic.py
--rw-r--r--   0 root         (0) root         (0)    12699 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/error_o_auth2.py
--rw-r--r--   0 root         (0) root         (0)    12528 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/event_stream.py
--rw-r--r--   0 root         (0) root         (0)    13201 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/expanded_permission_tree.py
--rw-r--r--   0 root         (0) root         (0)    12628 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/flow_error.py
--rw-r--r--   0 root         (0) root         (0)    14404 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/generic_error.py
--rw-r--r--   0 root         (0) root         (0)    12936 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/generic_error_content.py
--rw-r--r--   0 root         (0) root         (0)    12338 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/generic_usage.py
--rw-r--r--   0 root         (0) root         (0)    11849 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/get_attributes_count_response.py
--rw-r--r--   0 root         (0) root         (0)    11596 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/get_managed_identity_schema_location.py
--rw-r--r--   0 root         (0) root         (0)    11626 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/get_metrics_event_attributes_response.py
--rw-r--r--   0 root         (0) root         (0)    11611 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/get_metrics_event_types_response.py
--rw-r--r--   0 root         (0) root         (0)    11874 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/get_organization_response.py
--rw-r--r--   0 root         (0) root         (0)    13505 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/get_project_events_body.py
--rw-r--r--   0 root         (0) root         (0)    12199 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/get_project_events_response.py
--rw-r--r--   0 root         (0) root         (0)    11797 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/get_project_metrics_response.py
--rw-r--r--   0 root         (0) root         (0)    11849 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/get_session_activity_response.py
--rw-r--r--   0 root         (0) root         (0)    11672 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/get_version200_response.py
--rw-r--r--   0 root         (0) root         (0)    11716 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/health_not_ready_status.py
--rw-r--r--   0 root         (0) root         (0)    11590 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/health_status.py
--rw-r--r--   0 root         (0) root         (0)    18610 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity.py
--rw-r--r--   0 root         (0) root         (0)    14637 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_credentials.py
--rw-r--r--   0 root         (0) root         (0)    11908 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_credentials_code.py
--rw-r--r--   0 root         (0) root         (0)    11911 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_credentials_oidc.py
--rw-r--r--   0 root         (0) root         (0)    12763 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_credentials_oidc_provider.py
--rw-r--r--   0 root         (0) root         (0)    11732 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_credentials_password.py
--rw-r--r--   0 root         (0) root         (0)    12312 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_patch.py
--rw-r--r--   0 root         (0) root         (0)    12511 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_patch_response.py
--rw-r--r--   0 root         (0) root         (0)    12063 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_schema_container.py
--rw-r--r--   0 root         (0) root         (0)    12109 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_schema_preset.py
--rw-r--r--   0 root         (0) root         (0)    12084 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_schema_presets.py
--rw-r--r--   0 root         (0) root         (0)    12217 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)    12317 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_with_credentials.py
--rw-r--r--   0 root         (0) root         (0)    11917 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_with_credentials_oidc.py
--rw-r--r--   0 root         (0) root         (0)    12583 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_with_credentials_oidc_config.py
--rw-r--r--   0 root         (0) root         (0)    12296 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_with_credentials_oidc_config_provider.py
--rw-r--r--   0 root         (0) root         (0)    11957 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_with_credentials_password.py
--rw-r--r--   0 root         (0) root         (0)    12222 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/identity_with_credentials_password_config.py
--rw-r--r--   0 root         (0) root         (0)    11590 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/internal_get_project_branding_body.py
--rw-r--r--   0 root         (0) root         (0)    12074 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/internal_is_ax_welcome_screen_enabled_for_project_body.py
--rw-r--r--   0 root         (0) root         (0)    12881 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/internal_is_owner_for_project_by_slug_body.py
--rw-r--r--   0 root         (0) root         (0)    11767 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/internal_is_owner_for_project_by_slug_response.py
--rw-r--r--   0 root         (0) root         (0)    18024 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/introspected_o_auth2_token.py
--rw-r--r--   0 root         (0) root         (0)    12057 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/is_owner_for_project_by_slug.py
--rw-r--r--   0 root         (0) root         (0)    11628 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/is_ready200_response.py
--rw-r--r--   0 root         (0) root         (0)    11762 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/is_ready503_response.py
--rw-r--r--   0 root         (0) root         (0)    13595 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/json_patch.py
--rw-r--r--   0 root         (0) root         (0)    12088 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/json_patch_document.py
--rw-r--r--   0 root         (0) root         (0)    18000 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/json_web_key.py
--rw-r--r--   0 root         (0) root         (0)    12346 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)    11687 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/keto_namespace.py
--rw-r--r--   0 root         (0) root         (0)    11999 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/keto_namespaces.py
--rw-r--r--   0 root         (0) root         (0)    12087 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/list_custom_domains.py
--rw-r--r--   0 root         (0) root         (0)    11768 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/list_event_streams.py
--rw-r--r--   0 root         (0) root         (0)    12472 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/list_my_workspaces_response.py
--rw-r--r--   0 root         (0) root         (0)    11897 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/list_organizations_response.py
--rw-r--r--   0 root         (0) root         (0)    12413 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/list_workspace_projects_response.py
--rw-r--r--   0 root         (0) root         (0)    21060 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/login_flow.py
--rw-r--r--   0 root         (0) root         (0)    13275 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/login_flow_state.py
--rw-r--r--   0 root         (0) root         (0)    12148 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/logout_flow.py
--rw-r--r--   0 root         (0) root         (0)    13567 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/managed_identity_schema.py
--rw-r--r--   0 root         (0) root         (0)    11792 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/managed_identity_schema_validation_result.py
--rw-r--r--   0 root         (0) root         (0)    12096 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/managed_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)    14688 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/member_invite.py
--rw-r--r--   0 root         (0) root         (0)    11987 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/member_invites.py
--rw-r--r--   0 root         (0) root         (0)    16717 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/message.py
--rw-r--r--   0 root         (0) root         (0)    13688 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/message_dispatch.py
--rw-r--r--   0 root         (0) root         (0)    11924 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/metrics_datapoint.py
--rw-r--r--   0 root         (0) root         (0)    13562 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/migration_options.py
--rw-r--r--   0 root         (0) root         (0)    11555 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/namespace.py
--rw-r--r--   0 root         (0) root         (0)    12239 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/needs_privileged_session_error.py
--rw-r--r--   0 root         (0) root         (0)    14951 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/normalized_project.py
--rw-r--r--   0 root         (0) root         (0)   145178 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/normalized_project_revision.py
--rw-r--r--   0 root         (0) root         (0)    17424 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/normalized_project_revision_courier_channel.py
--rw-r--r--   0 root         (0) root         (0)    18363 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/normalized_project_revision_hook.py
--rw-r--r--   0 root         (0) root         (0)    15526 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/normalized_project_revision_identity_schema.py
--rw-r--r--   0 root         (0) root         (0)    12314 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/normalized_project_revision_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)    21407 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/normalized_project_revision_third_party_provider.py
--rw-r--r--   0 root         (0) root         (0)    13893 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/normalized_project_revision_tokenizer_template.py
--rw-r--r--   0 root         (0) root         (0)    12350 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/normalized_project_revision_tokenizer_templates.py
--rw-r--r--   0 root         (0) root         (0)    12047 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/normalized_projects.py
--rw-r--r--   0 root         (0) root         (0)    11898 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/null_duration.py
--rw-r--r--   0 root         (0) root         (0)    39393 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/o_auth2_client.py
--rw-r--r--   0 root         (0) root         (0)    15434 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/o_auth2_client_token_lifespans.py
--rw-r--r--   0 root         (0) root         (0)    18510 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/o_auth2_consent_request.py
--rw-r--r--   0 root         (0) root         (0)    18529 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/o_auth2_consent_request_open_id_connect_context.py
--rw-r--r--   0 root         (0) root         (0)    15310 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/o_auth2_consent_session.py
--rw-r--r--   0 root         (0) root         (0)    12544 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/o_auth2_consent_session_expires_at.py
--rw-r--r--   0 root         (0) root         (0)    12229 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/o_auth2_consent_sessions.py
--rw-r--r--   0 root         (0) root         (0)    17102 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/o_auth2_login_request.py
--rw-r--r--   0 root         (0) root         (0)    13573 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/o_auth2_logout_request.py
--rw-r--r--   0 root         (0) root         (0)    11881 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/o_auth2_redirect_to.py
--rw-r--r--   0 root         (0) root         (0)    13565 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/o_auth2_token_exchange.py
--rw-r--r--   0 root         (0) root         (0)    33786 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/oidc_configuration.py
--rw-r--r--   0 root         (0) root         (0)    24625 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/oidc_user_info.py
--rw-r--r--   0 root         (0) root         (0)    13150 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/organization.py
--rw-r--r--   0 root         (0) root         (0)    11924 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/organization_body.py
--rw-r--r--   0 root         (0) root         (0)    12865 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/pagination.py
--rw-r--r--   0 root         (0) root         (0)    12222 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/pagination_headers.py
--rw-r--r--   0 root         (0) root         (0)    12124 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/parse_error.py
--rw-r--r--   0 root         (0) root         (0)    11890 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/patch_identities_body.py
--rw-r--r--   0 root         (0) root         (0)    11790 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/perform_native_logout_body.py
--rw-r--r--   0 root         (0) root         (0)    11306 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/permissions_on_project.py
--rw-r--r--   0 root         (0) root         (0)    11635 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/permissions_on_workpace_response.py
--rw-r--r--   0 root         (0) root         (0)    11989 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/plan.py
--rw-r--r--   0 root         (0) root         (0)    14031 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/plan_details.py
--rw-r--r--   0 root         (0) root         (0)    11459 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/plan_features.py
--rw-r--r--   0 root         (0) root         (0)    11781 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/plans.py
--rw-r--r--   0 root         (0) root         (0)    12813 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/post_check_permission_body.py
--rw-r--r--   0 root         (0) root         (0)    12834 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/post_check_permission_or_error_body.py
--rw-r--r--   0 root         (0) root         (0)    11960 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/pricing.py
--rw-r--r--   0 root         (0) root         (0)    13831 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/project.py
--rw-r--r--   0 root         (0) root         (0)    13276 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/project_api_key.py
--rw-r--r--   0 root         (0) root         (0)    12000 2024-03-08 12:30:13.000000 ory-client-1.8.1/ory_client/model/project_api_keys.py
--rw-r--r--   0 root         (0) root         (0)    13358 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_branding.py
--rw-r--r--   0 root         (0) root         (0)    23906 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_branding_colors.py
--rw-r--r--   0 root         (0) root         (0)    26889 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_branding_theme.py
--rw-r--r--   0 root         (0) root         (0)    12084 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_branding_themes.py
--rw-r--r--   0 root         (0) root         (0)    12190 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_cors.py
--rw-r--r--   0 root         (0) root         (0)    12416 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_events_datapoint.py
--rw-r--r--   0 root         (0) root         (0)    12070 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_host.py
--rw-r--r--   0 root         (0) root         (0)    12120 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_member.py
--rw-r--r--   0 root         (0) root         (0)    11999 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_members.py
--rw-r--r--   0 root         (0) root         (0)    14913 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_metadata.py
--rw-r--r--   0 root         (0) root         (0)    12032 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_metadata_list.py
--rw-r--r--   0 root         (0) root         (0)    12163 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_revision_hooks.py
--rw-r--r--   0 root         (0) root         (0)    12284 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_revision_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)    12348 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_revision_third_party_login_providers.py
--rw-r--r--   0 root         (0) root         (0)    12114 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_revisions.py
--rw-r--r--   0 root         (0) root         (0)    11808 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_service_identity.py
--rw-r--r--   0 root         (0) root         (0)    11802 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_service_o_auth2.py
--rw-r--r--   0 root         (0) root         (0)    11814 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_service_permission.py
--rw-r--r--   0 root         (0) root         (0)    12615 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/project_services.py
--rw-r--r--   0 root         (0) root         (0)    11926 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/projects.py
--rw-r--r--   0 root         (0) root         (0)    16097 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/quota_usage.py
--rw-r--r--   0 root         (0) root         (0)    12720 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/recovery_code_for_identity.py
--rw-r--r--   0 root         (0) root         (0)    16698 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/recovery_flow.py
--rw-r--r--   0 root         (0) root         (0)    13316 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/recovery_flow_state.py
--rw-r--r--   0 root         (0) root         (0)    12615 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/recovery_identity_address.py
--rw-r--r--   0 root         (0) root         (0)    12181 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/recovery_link_for_identity.py
--rw-r--r--   0 root         (0) root         (0)    19640 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/registration_flow.py
--rw-r--r--   0 root         (0) root         (0)    13120 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/registration_flow_state.py
--rw-r--r--   0 root         (0) root         (0)    13273 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/reject_o_auth2_request.py
--rw-r--r--   0 root         (0) root         (0)    12783 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/relation_query.py
--rw-r--r--   0 root         (0) root         (0)    13010 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/relationship.py
--rw-r--r--   0 root         (0) root         (0)    11756 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/relationship_namespaces.py
--rw-r--r--   0 root         (0) root         (0)    12062 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/relationship_patch.py
--rw-r--r--   0 root         (0) root         (0)    12258 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/relationships.py
--rw-r--r--   0 root         (0) root         (0)    12263 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/revision_courier_channels.py
--rw-r--r--   0 root         (0) root         (0)    12410 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/rfc6749_error_json.py
--rw-r--r--   0 root         (0) root         (0)    12033 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/schema_patch.py
--rw-r--r--   0 root         (0) root         (0)    12969 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/self_service_flow_expired_error.py
--rw-r--r--   0 root         (0) root         (0)    15774 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/session.py
--rw-r--r--   0 root         (0) root         (0)    12342 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/session_activity_datapoint.py
--rw-r--r--   0 root         (0) root         (0)    13371 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/session_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)    12452 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/session_authentication_methods.py
--rw-r--r--   0 root         (0) root         (0)    12379 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/session_device.py
--rw-r--r--   0 root         (0) root         (0)    11805 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/set_active_project_in_console_body.py
--rw-r--r--   0 root         (0) root         (0)    13091 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/set_custom_domain_body.py
--rw-r--r--   0 root         (0) root         (0)    12593 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/set_event_stream_body.py
--rw-r--r--   0 root         (0) root         (0)    12725 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/set_project.py
--rw-r--r--   0 root         (0) root         (0)    12962 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/set_project_branding_theme_body.py
--rw-r--r--   0 root         (0) root         (0)    17601 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/settings_flow.py
--rw-r--r--   0 root         (0) root         (0)    13574 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/settings_flow_state.py
--rw-r--r--   0 root         (0) root         (0)    11710 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/source_position.py
--rw-r--r--   0 root         (0) root         (0)    11819 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/string_slice_json_format.py
--rw-r--r--   0 root         (0) root         (0)    12219 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/subject_set.py
--rw-r--r--   0 root         (0) root         (0)    18737 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/subscription.py
--rw-r--r--   0 root         (0) root         (0)    12500 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/successful_code_exchange_response.py
--rw-r--r--   0 root         (0) root         (0)    12473 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/successful_native_login.py
--rw-r--r--   0 root         (0) root         (0)    13754 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/successful_native_registration.py
--rw-r--r--   0 root         (0) root         (0)    12962 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/successful_project_update.py
--rw-r--r--   0 root         (0) root         (0)    12880 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/token_pagination.py
--rw-r--r--   0 root         (0) root         (0)    12237 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/token_pagination_headers.py
--rw-r--r--   0 root         (0) root         (0)    12930 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/token_pagination_request_parameters.py
--rw-r--r--   0 root         (0) root         (0)    13145 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/token_pagination_response_headers.py
--rw-r--r--   0 root         (0) root         (0)    13912 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/trust_o_auth2_jwt_grant_issuer.py
--rw-r--r--   0 root         (0) root         (0)    14486 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/trusted_o_auth2_jwt_grant_issuer.py
--rw-r--r--   0 root         (0) root         (0)    12399 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/trusted_o_auth2_jwt_grant_issuers.py
--rw-r--r--   0 root         (0) root         (0)    12089 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/trusted_o_auth2_jwt_grant_json_web_key.py
--rw-r--r--   0 root         (0) root         (0)    12714 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/ui_container.py
--rw-r--r--   0 root         (0) root         (0)    14031 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/ui_node.py
--rw-r--r--   0 root         (0) root         (0)    12852 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/ui_node_anchor_attributes.py
--rw-r--r--   0 root         (0) root         (0)    22091 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/ui_node_attributes.py
--rw-r--r--   0 root         (0) root         (0)    12956 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/ui_node_image_attributes.py
--rw-r--r--   0 root         (0) root         (0)    16763 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/ui_node_input_attributes.py
--rw-r--r--   0 root         (0) root         (0)    11669 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/ui_node_meta.py
--rw-r--r--   0 root         (0) root         (0)    14565 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/ui_node_script_attributes.py
--rw-r--r--   0 root         (0) root         (0)    12555 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/ui_node_text_attributes.py
--rw-r--r--   0 root         (0) root         (0)    11915 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/ui_nodes.py
--rw-r--r--   0 root         (0) root         (0)    12735 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/ui_text.py
--rw-r--r--   0 root         (0) root         (0)    11915 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/ui_texts.py
--rw-r--r--   0 root         (0) root         (0)    15089 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_identity_body.py
--rw-r--r--   0 root         (0) root         (0)    23673 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_login_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    13684 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_login_flow_with_code_method.py
--rw-r--r--   0 root         (0) root         (0)    12516 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_login_flow_with_lookup_secret_method.py
--rw-r--r--   0 root         (0) root         (0)    16813 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_login_flow_with_oidc_method.py
--rw-r--r--   0 root         (0) root         (0)    13823 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_login_flow_with_password_method.py
--rw-r--r--   0 root         (0) root         (0)    12937 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_login_flow_with_totp_method.py
--rw-r--r--   0 root         (0) root         (0)    13476 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_login_flow_with_web_authn_method.py
--rw-r--r--   0 root         (0) root         (0)    17254 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_recovery_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    14514 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_recovery_flow_with_code_method.py
--rw-r--r--   0 root         (0) root         (0)    13596 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_recovery_flow_with_link_method.py
--rw-r--r--   0 root         (0) root         (0)    22203 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_registration_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    13543 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_registration_flow_with_code_method.py
--rw-r--r--   0 root         (0) root         (0)    16740 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_registration_flow_with_oidc_method.py
--rw-r--r--   0 root         (0) root         (0)    13361 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_registration_flow_with_password_method.py
--rw-r--r--   0 root         (0) root         (0)    14145 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_registration_flow_with_web_authn_method.py
--rw-r--r--   0 root         (0) root         (0)    24071 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_settings_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    14085 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_settings_flow_with_lookup_method.py
--rw-r--r--   0 root         (0) root         (0)    15448 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_settings_flow_with_oidc_method.py
--rw-r--r--   0 root         (0) root         (0)    12897 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_settings_flow_with_password_method.py
--rw-r--r--   0 root         (0) root         (0)    13156 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_settings_flow_with_profile_method.py
--rw-r--r--   0 root         (0) root         (0)    13420 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_settings_flow_with_totp_method.py
--rw-r--r--   0 root         (0) root         (0)    14084 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_settings_flow_with_web_authn_method.py
--rw-r--r--   0 root         (0) root         (0)    12189 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_subscription_body.py
--rw-r--r--   0 root         (0) root         (0)    17336 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_verification_flow_body.py
--rw-r--r--   0 root         (0) root         (0)    14532 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_verification_flow_with_code_method.py
--rw-r--r--   0 root         (0) root         (0)    13646 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_verification_flow_with_link_method.py
--rw-r--r--   0 root         (0) root         (0)    11642 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/update_workspace_payload.py
--rw-r--r--   0 root         (0) root         (0)    11735 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/usage.py
--rw-r--r--   0 root         (0) root         (0)    13096 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/verifiable_credential_priming_response.py
--rw-r--r--   0 root         (0) root         (0)    11758 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/verifiable_credential_proof.py
--rw-r--r--   0 root         (0) root         (0)    11827 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/verifiable_credential_response.py
--rw-r--r--   0 root         (0) root         (0)    13725 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/verifiable_identity_address.py
--rw-r--r--   0 root         (0) root         (0)    16175 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/verification_flow.py
--rw-r--r--   0 root         (0) root         (0)    13344 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/verification_flow_state.py
--rw-r--r--   0 root         (0) root         (0)    11586 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/version.py
--rw-r--r--   0 root         (0) root         (0)    11694 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/warning.py
--rw-r--r--   0 root         (0) root         (0)    12525 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/workspace.py
--rw-r--r--   0 root         (0) root         (0)    12813 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/workspace_meta.py
--rw-r--r--   0 root         (0) root         (0)    11950 2024-03-08 12:30:14.000000 ory-client-1.8.1/ory_client/model/workspaces.py
--rw-r--r--   0 root         (0) root         (0)    82704 2024-03-08 12:30:15.000000 ory-client-1.8.1/ory_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 12:35:26.249373 ory-client-1.8.1/ory_client/models/
--rw-r--r--   0 root         (0) root         (0)    22098 2024-03-08 12:30:15.000000 ory-client-1.8.1/ory_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14398 2024-03-08 12:30:15.000000 ory-client-1.8.1/ory_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 12:35:26.213373 ory-client-1.8.1/ory_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      486 2024-03-08 12:35:26.000000 ory-client-1.8.1/ory_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24698 2024-03-08 12:35:26.000000 ory-client-1.8.1/ory_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 12:35:26.000000 ory-client-1.8.1/ory_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-03-08 12:35:26.000000 ory-client-1.8.1/ory_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-08 12:35:26.000000 ory-client-1.8.1/ory_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-03-08 12:35:26.313374 ory-client-1.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1278 2024-03-08 12:30:15.000000 ory-client-1.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 12:35:26.313374 ory-client-1.8.1/test/
--rw-r--r--   0 root         (0) root         (0)     1279 2024-03-08 12:30:12.000000 ory-client-1.8.1/test/test_accept_o_auth2_consent_request.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-03-08 12:30:12.000000 ory-client-1.8.1/test/test_accept_o_auth2_consent_request_session.py
--rw-r--r--   0 root         (0) root         (0)     1080 2024-03-08 12:30:12.000000 ory-client-1.8.1/test/test_accept_o_auth2_login_request.py
--rw-r--r--   0 root         (0) root         (0)      930 2024-03-08 12:30:12.000000 ory-client-1.8.1/test/test_active_project_in_console.py
--rw-r--r--   0 root         (0) root         (0)      836 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_attribute.py
--rw-r--r--   0 root         (0) root         (0)      879 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_attribute_filter.py
--rw-r--r--   0 root         (0) root         (0)      943 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_attributes_count_datapoint.py
--rw-r--r--   0 root         (0) root         (0)      964 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_authenticator_assurance_level.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_batch_patch_identities_response.py
--rw-r--r--   0 root         (0) root         (0)     1005 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_check_opl_syntax_result.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_check_permission_result.py
--rw-r--r--   0 root         (0) root         (0)      858 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_cloud_account.py
--rw-r--r--   0 root         (0) root         (0)      971 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_consistency_request_parameters.py
--rw-r--r--   0 root         (0) root         (0)     1620 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_continue_with.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_continue_with_recovery_ui.py
--rw-r--r--   0 root         (0) root         (0)      959 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_continue_with_recovery_ui_flow.py
--rw-r--r--   0 root         (0) root         (0)      988 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_continue_with_set_ory_session_token.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_continue_with_settings_ui.py
--rw-r--r--   0 root         (0) root         (0)      959 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_continue_with_settings_ui_flow.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_continue_with_verification_ui.py
--rw-r--r--   0 root         (0) root         (0)      987 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_continue_with_verification_ui_flow.py
--rw-r--r--   0 root         (0) root         (0)      979 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_courier_api.py
--rw-r--r--   0 root         (0) root         (0)      915 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_courier_message_status.py
--rw-r--r--   0 root         (0) root         (0)      901 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_courier_message_type.py
--rw-r--r--   0 root         (0) root         (0)      930 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_custom_domain_body.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_event_stream_body.py
--rw-r--r--   0 root         (0) root         (0)     1335 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_identity_body.py
--rw-r--r--   0 root         (0) root         (0)     1012 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_invite_response.py
--rw-r--r--   0 root         (0) root         (0)      910 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)      958 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_member_invite_response.py
--rw-r--r--   0 root         (0) root         (0)      959 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_project_api_key_request.py
--rw-r--r--   0 root         (0) root         (0)      894 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_project_body.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_project_branding.py
--rw-r--r--   0 root         (0) root         (0)      980 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_project_member_invite_body.py
--rw-r--r--   0 root         (0) root         (0)     2102 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_project_normalized_payload.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_recovery_code_for_identity_body.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_recovery_link_for_identity_body.py
--rw-r--r--   0 root         (0) root         (0)     1018 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_relationship_body.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_subscription_body.py
--rw-r--r--   0 root         (0) root         (0)      943 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_subscription_common.py
--rw-r--r--   0 root         (0) root         (0)     1186 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_verifiable_credential_request_body.py
--rw-r--r--   0 root         (0) root         (0)      994 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_workspace_member_invite_body.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_workspace_payload.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_create_workspace_subscription_body.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_credential_supported_draft00.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_custom_domain.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_delete_my_sessions_count.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_email_template_data.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_email_template_data_body.py
--rw-r--r--   0 root         (0) root         (0)     1183 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_error_authenticator_assurance_level_not_satisfied.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_error_browser_location_change_required.py
--rw-r--r--   0 root         (0) root         (0)      991 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_error_flow_replaced.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_error_generic.py
--rw-r--r--   0 root         (0) root         (0)      852 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_error_o_auth2.py
--rw-r--r--   0 root         (0) root         (0)      851 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_event_stream.py
--rw-r--r--   0 root         (0) root         (0)     1391 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_events_api.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_expanded_permission_tree.py
--rw-r--r--   0 root         (0) root         (0)      837 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_flow_error.py
--rw-r--r--   0 root         (0) root         (0)     5770 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_frontend_api.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_generic_error.py
--rw-r--r--   0 root         (0) root         (0)      908 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_generic_error_content.py
--rw-r--r--   0 root         (0) root         (0)      858 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_generic_usage.py
--rw-r--r--   0 root         (0) root         (0)     1104 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_get_attributes_count_response.py
--rw-r--r--   0 root         (0) root         (0)     1001 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_get_managed_identity_schema_location.py
--rw-r--r--   0 root         (0) root         (0)     1008 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_get_metrics_event_attributes_response.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_get_metrics_event_types_response.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_get_organization_response.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_get_project_events_body.py
--rw-r--r--   0 root         (0) root         (0)     1082 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_get_project_events_response.py
--rw-r--r--   0 root         (0) root         (0)     1064 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_get_project_metrics_response.py
--rw-r--r--   0 root         (0) root         (0)     1104 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_get_session_activity_response.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_get_version200_response.py
--rw-r--r--   0 root         (0) root         (0)      916 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_health_not_ready_status.py
--rw-r--r--   0 root         (0) root         (0)      858 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_health_status.py
--rw-r--r--   0 root         (0) root         (0)     1246 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity.py
--rw-r--r--   0 root         (0) root         (0)     3517 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_identity_api.py
--rw-r--r--   0 root         (0) root         (0)      907 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_credentials.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_credentials_code.py
--rw-r--r--   0 root         (0) root         (0)     1111 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_credentials_oidc.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_credentials_oidc_provider.py
--rw-r--r--   0 root         (0) root         (0)      964 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_credentials_password.py
--rw-r--r--   0 root         (0) root         (0)      987 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_patch.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_patch_response.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_schema_container.py
--rw-r--r--   0 root         (0) root         (0)      915 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_schema_preset.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_schema_presets.py
--rw-r--r--   0 root         (0) root         (0)     1021 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)     1270 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_with_credentials.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_with_credentials_oidc.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_with_credentials_oidc_config.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_with_credentials_oidc_config_provider.py
--rw-r--r--   0 root         (0) root         (0)     1193 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_with_credentials_password.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_identity_with_credentials_password_config.py
--rw-r--r--   0 root         (0) root         (0)      987 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_internal_get_project_branding_body.py
--rw-r--r--   0 root         (0) root         (0)     1103 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_internal_is_ax_welcome_screen_enabled_for_project_body.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_internal_is_owner_for_project_by_slug_body.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_internal_is_owner_for_project_by_slug_response.py
--rw-r--r--   0 root         (0) root         (0)      937 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_introspected_o_auth2_token.py
--rw-r--r--   0 root         (0) root         (0)      939 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_is_owner_for_project_by_slug.py
--rw-r--r--   0 root         (0) root         (0)      901 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_is_ready200_response.py
--rw-r--r--   0 root         (0) root         (0)      901 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_is_ready503_response.py
--rw-r--r--   0 root         (0) root         (0)      837 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_json_patch.py
--rw-r--r--   0 root         (0) root         (0)      979 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_json_patch_document.py
--rw-r--r--   0 root         (0) root         (0)      845 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_json_web_key.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_json_web_key_set.py
--rw-r--r--   0 root         (0) root         (0)     1757 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_jwk_api.py
--rw-r--r--   0 root         (0) root         (0)      865 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_keto_namespace.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_keto_namespaces.py
--rw-r--r--   0 root         (0) root         (0)      991 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_list_custom_domains.py
--rw-r--r--   0 root         (0) root         (0)      980 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_list_event_streams.py
--rw-r--r--   0 root         (0) root         (0)     1045 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_list_my_workspaces_response.py
--rw-r--r--   0 root         (0) root         (0)     1046 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_list_organizations_response.py
--rw-r--r--   0 root         (0) root         (0)     1088 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_list_workspace_projects_response.py
--rw-r--r--   0 root         (0) root         (0)     1211 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_login_flow.py
--rw-r--r--   0 root         (0) root         (0)      873 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_login_flow_state.py
--rw-r--r--   0 root         (0) root         (0)      844 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_logout_flow.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_managed_identity_schema.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_managed_identity_schema_validation_result.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_managed_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)      858 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_member_invite.py
--rw-r--r--   0 root         (0) root         (0)      962 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_member_invites.py
--rw-r--r--   0 root         (0) root         (0)     1183 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_message.py
--rw-r--r--   0 root         (0) root         (0)      879 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_message_dispatch.py
--rw-r--r--   0 root         (0) root         (0)     1122 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_metrics_datapoint.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_migration_options.py
--rw-r--r--   0 root         (0) root         (0)      836 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_namespace.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_needs_privileged_session_error.py
--rw-r--r--   0 root         (0) root         (0)     1178 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_normalized_project.py
--rw-r--r--   0 root         (0) root         (0)     2066 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_normalized_project_revision.py
--rw-r--r--   0 root         (0) root         (0)     1050 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_normalized_project_revision_courier_channel.py
--rw-r--r--   0 root         (0) root         (0)      979 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_normalized_project_revision_hook.py
--rw-r--r--   0 root         (0) root         (0)     1184 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_normalized_project_revision_identity_schema.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_normalized_project_revision_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)     1214 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_normalized_project_revision_third_party_provider.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_normalized_project_revision_tokenizer_template.py
--rw-r--r--   0 root         (0) root         (0)     1298 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_normalized_project_revision_tokenizer_templates.py
--rw-r--r--   0 root         (0) root         (0)     1017 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_normalized_projects.py
--rw-r--r--   0 root         (0) root         (0)      858 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_null_duration.py
--rw-r--r--   0 root         (0) root         (0)     5859 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_o_auth2_api.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_o_auth2_client.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_o_auth2_client_token_lifespans.py
--rw-r--r--   0 root         (0) root         (0)     1364 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_o_auth2_consent_request.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_o_auth2_consent_request_open_id_connect_context.py
--rw-r--r--   0 root         (0) root         (0)     1536 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_o_auth2_consent_session.py
--rw-r--r--   0 root         (0) root         (0)      981 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_o_auth2_consent_session_expires_at.py
--rw-r--r--   0 root         (0) root         (0)     1054 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_o_auth2_consent_sessions.py
--rw-r--r--   0 root         (0) root         (0)     1350 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_o_auth2_login_request.py
--rw-r--r--   0 root         (0) root         (0)     1007 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_o_auth2_logout_request.py
--rw-r--r--   0 root         (0) root         (0)      888 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_o_auth2_redirect_to.py
--rw-r--r--   0 root         (0) root         (0)      909 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_o_auth2_token_exchange.py
--rw-r--r--   0 root         (0) root         (0)     2217 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_oidc_api.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_oidc_configuration.py
--rw-r--r--   0 root         (0) root         (0)      859 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_oidc_user_info.py
--rw-r--r--   0 root         (0) root         (0)      992 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_organization.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_organization_body.py
--rw-r--r--   0 root         (0) root         (0)      843 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_pagination.py
--rw-r--r--   0 root         (0) root         (0)      893 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_pagination_headers.py
--rw-r--r--   0 root         (0) root         (0)      949 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_parse_error.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_patch_identities_body.py
--rw-r--r--   0 root         (0) root         (0)      937 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_perform_native_logout_body.py
--rw-r--r--   0 root         (0) root         (0)     1510 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_permission_api.py
--rw-r--r--   0 root         (0) root         (0)      915 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_permissions_on_project.py
--rw-r--r--   0 root         (0) root         (0)      979 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_permissions_on_workpace_response.py
--rw-r--r--   0 root         (0) root         (0)      801 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_plan.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_plan_details.py
--rw-r--r--   0 root         (0) root         (0)      955 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_plan_features.py
--rw-r--r--   0 root         (0) root         (0)      808 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_plans.py
--rw-r--r--   0 root         (0) root         (0)     1026 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_post_check_permission_body.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_post_check_permission_or_error_body.py
--rw-r--r--   0 root         (0) root         (0)      915 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_pricing.py
--rw-r--r--   0 root         (0) root         (0)     1024 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_project.py
--rw-r--r--   0 root         (0) root         (0)     3745 2024-03-08 12:30:15.000000 ory-client-1.8.1/test/test_project_api.py
--rw-r--r--   0 root         (0) root         (0)      866 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_project_api_key.py
--rw-r--r--   0 root         (0) root         (0)      975 2024-03-08 12:30:13.000000 ory-client-1.8.1/test/test_project_api_keys.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_branding.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_branding_colors.py
--rw-r--r--   0 root         (0) root         (0)      915 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_branding_theme.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_branding_themes.py
--rw-r--r--   0 root         (0) root         (0)      851 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_cors.py
--rw-r--r--   0 root         (0) root         (0)     1013 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_events_datapoint.py
--rw-r--r--   0 root         (0) root         (0)      851 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_host.py
--rw-r--r--   0 root         (0) root         (0)      865 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_member.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_members.py
--rw-r--r--   0 root         (0) root         (0)     1014 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_metadata.py
--rw-r--r--   0 root         (0) root         (0)     1017 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_metadata_list.py
--rw-r--r--   0 root         (0) root         (0)     1082 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_revision_hooks.py
--rw-r--r--   0 root         (0) root         (0)     1194 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_revision_identity_schemas.py
--rw-r--r--   0 root         (0) root         (0)     1276 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_revision_third_party_login_providers.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_revisions.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_service_identity.py
--rw-r--r--   0 root         (0) root         (0)      916 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_service_o_auth2.py
--rw-r--r--   0 root         (0) root         (0)      943 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_service_permission.py
--rw-r--r--   0 root         (0) root         (0)     1294 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_project_services.py
--rw-r--r--   0 root         (0) root         (0)      905 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_projects.py
--rw-r--r--   0 root         (0) root         (0)      844 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_quota_usage.py
--rw-r--r--   0 root         (0) root         (0)      937 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_recovery_code_for_identity.py
--rw-r--r--   0 root         (0) root         (0)     1048 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_recovery_flow.py
--rw-r--r--   0 root         (0) root         (0)      894 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_recovery_flow_state.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_recovery_identity_address.py
--rw-r--r--   0 root         (0) root         (0)      937 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_recovery_link_for_identity.py
--rw-r--r--   0 root         (0) root         (0)     1102 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_registration_flow.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_registration_flow_state.py
--rw-r--r--   0 root         (0) root         (0)      909 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_reject_o_auth2_request.py
--rw-r--r--   0 root         (0) root         (0)      954 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_relation_query.py
--rw-r--r--   0 root         (0) root         (0)      946 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_relationship.py
--rw-r--r--   0 root         (0) root         (0)     1659 2024-03-08 12:30:15.000000 ory-client-1.8.1/test/test_relationship_api.py
--rw-r--r--   0 root         (0) root         (0)     1012 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_relationship_namespaces.py
--rw-r--r--   0 root         (0) root         (0)      989 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_relationship_patch.py
--rw-r--r--   0 root         (0) root         (0)      960 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_relationships.py
--rw-r--r--   0 root         (0) root         (0)     1144 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_revision_courier_channels.py
--rw-r--r--   0 root         (0) root         (0)      887 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_rfc6749_error_json.py
--rw-r--r--   0 root         (0) root         (0)      851 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_schema_patch.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_self_service_flow_expired_error.py
--rw-r--r--   0 root         (0) root         (0)     1323 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_session.py
--rw-r--r--   0 root         (0) root         (0)      943 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_session_activity_datapoint.py
--rw-r--r--   0 root         (0) root         (0)     1122 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_session_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     1129 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_session_authentication_methods.py
--rw-r--r--   0 root         (0) root         (0)      865 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_session_device.py
--rw-r--r--   0 root         (0) root         (0)      981 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_set_active_project_in_console_body.py
--rw-r--r--   0 root         (0) root         (0)      909 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_set_custom_domain_body.py
--rw-r--r--   0 root         (0) root         (0)      902 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_set_event_stream_body.py
--rw-r--r--   0 root         (0) root         (0)     1046 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_set_project.py
--rw-r--r--   0 root         (0) root         (0)     1100 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_set_project_branding_theme_body.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_settings_flow.py
--rw-r--r--   0 root         (0) root         (0)      894 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_settings_flow_state.py
--rw-r--r--   0 root         (0) root         (0)      872 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_source_position.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_string_slice_json_format.py
--rw-r--r--   0 root         (0) root         (0)      844 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_subject_set.py
--rw-r--r--   0 root         (0) root         (0)      950 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_successful_code_exchange_response.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_successful_native_login.py
--rw-r--r--   0 root         (0) root         (0)     1224 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_successful_native_registration.py
--rw-r--r--   0 root         (0) root         (0)     1088 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_successful_project_update.py
--rw-r--r--   0 root         (0) root         (0)      879 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_token_pagination.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_token_pagination_headers.py
--rw-r--r--   0 root         (0) root         (0)     1000 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_token_pagination_request_parameters.py
--rw-r--r--   0 root         (0) root         (0)      986 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_token_pagination_response_headers.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_trust_o_auth2_jwt_grant_issuer.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_trusted_o_auth2_jwt_grant_issuer.py
--rw-r--r--   0 root         (0) root         (0)     1135 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_trusted_o_auth2_jwt_grant_issuers.py
--rw-r--r--   0 root         (0) root         (0)      997 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_trusted_o_auth2_jwt_grant_json_web_key.py
--rw-r--r--   0 root         (0) root         (0)     1005 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_ui_container.py
--rw-r--r--   0 root         (0) root         (0)     1097 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_ui_node.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_ui_node_anchor_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1639 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_ui_node_attributes.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_ui_node_image_attributes.py
--rw-r--r--   0 root         (0) root         (0)      996 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_ui_node_input_attributes.py
--rw-r--r--   0 root         (0) root         (0)      918 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_ui_node_meta.py
--rw-r--r--   0 root         (0) root         (0)      930 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_ui_node_script_attributes.py
--rw-r--r--   0 root         (0) root         (0)      989 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_ui_node_text_attributes.py
--rw-r--r--   0 root         (0) root         (0)      896 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_ui_nodes.py
--rw-r--r--   0 root         (0) root         (0)      816 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_ui_text.py
--rw-r--r--   0 root         (0) root         (0)      896 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_ui_texts.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_identity_body.py
--rw-r--r--   0 root         (0) root         (0)     1989 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_login_flow_body.py
--rw-r--r--   0 root         (0) root         (0)      981 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_login_flow_with_code_method.py
--rw-r--r--   0 root         (0) root         (0)     1038 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_login_flow_with_lookup_secret_method.py
--rw-r--r--   0 root         (0) root         (0)      981 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_login_flow_with_oidc_method.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_login_flow_with_password_method.py
--rw-r--r--   0 root         (0) root         (0)      981 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_login_flow_with_totp_method.py
--rw-r--r--   0 root         (0) root         (0)     1010 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_login_flow_with_web_authn_method.py
--rw-r--r--   0 root         (0) root         (0)     1292 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_recovery_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1002 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_recovery_flow_with_code_method.py
--rw-r--r--   0 root         (0) root         (0)     1002 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_recovery_flow_with_link_method.py
--rw-r--r--   0 root         (0) root         (0)     1779 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_registration_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1030 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_registration_flow_with_code_method.py
--rw-r--r--   0 root         (0) root         (0)     1030 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_registration_flow_with_oidc_method.py
--rw-r--r--   0 root         (0) root         (0)     1058 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_registration_flow_with_password_method.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_registration_flow_with_web_authn_method.py
--rw-r--r--   0 root         (0) root         (0)     2069 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_settings_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1016 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_settings_flow_with_lookup_method.py
--rw-r--r--   0 root         (0) root         (0)     1002 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_settings_flow_with_oidc_method.py
--rw-r--r--   0 root         (0) root         (0)     1030 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_settings_flow_with_password_method.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_settings_flow_with_profile_method.py
--rw-r--r--   0 root         (0) root         (0)     1002 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_settings_flow_with_totp_method.py
--rw-r--r--   0 root         (0) root         (0)     1031 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_settings_flow_with_web_authn_method.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_subscription_body.py
--rw-r--r--   0 root         (0) root         (0)     1352 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_verification_flow_body.py
--rw-r--r--   0 root         (0) root         (0)     1030 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_verification_flow_with_code_method.py
--rw-r--r--   0 root         (0) root         (0)     1030 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_verification_flow_with_link_method.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_update_workspace_payload.py
--rw-r--r--   0 root         (0) root         (0)      905 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_usage.py
--rw-r--r--   0 root         (0) root         (0)     1021 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_verifiable_credential_priming_response.py
--rw-r--r--   0 root         (0) root         (0)      950 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_verifiable_credential_proof.py
--rw-r--r--   0 root         (0) root         (0)      971 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_verifiable_credential_response.py
--rw-r--r--   0 root         (0) root         (0)      950 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_verifiable_identity_address.py
--rw-r--r--   0 root         (0) root         (0)      979 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_verification_flow.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_verification_flow_state.py
--rw-r--r--   0 root         (0) root         (0)      822 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_version.py
--rw-r--r--   0 root         (0) root         (0)      822 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_warning.py
--rw-r--r--   0 root         (0) root         (0)      863 2024-03-08 12:30:15.000000 ory-client-1.8.1/test/test_wellknown_api.py
--rw-r--r--   0 root         (0) root         (0)      836 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_workspace.py
--rw-r--r--   0 root         (0) root         (0)      865 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_workspace_meta.py
--rw-r--r--   0 root         (0) root         (0)      927 2024-03-08 12:30:14.000000 ory-client-1.8.1/test/test_workspaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 16:51:51.084114 ory-client-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)      486 2024-03-18 16:51:51.084114 ory-client-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    41345 2024-03-18 16:47:00.000000 ory-client-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 16:51:50.992114 ory-client-1.9.0/ory_client/
+-rw-r--r--   0 root         (0) root         (0)      835 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 16:51:50.996114 ory-client-1.9.0/ory_client/api/
+-rw-r--r--   0 root         (0) root         (0)      214 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12519 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api/courier_api.py
+-rw-r--r--   0 root         (0) root         (0)    23194 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api/events_api.py
+-rw-r--r--   0 root         (0) root         (0)   207385 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api/frontend_api.py
+-rw-r--r--   0 root         (0) root         (0)   110149 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api/identity_api.py
+-rw-r--r--   0 root         (0) root         (0)    40790 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api/jwk_api.py
+-rw-r--r--   0 root         (0) root         (0)    16248 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api/metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)   163217 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api/o_auth2_api.py
+-rw-r--r--   0 root         (0) root         (0)    45439 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api/oidc_api.py
+-rw-r--r--   0 root         (0) root         (0)    32053 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api/permission_api.py
+-rw-r--r--   0 root         (0) root         (0)   104681 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api/project_api.py
+-rw-r--r--   0 root         (0) root         (0)    34599 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api/relationship_api.py
+-rw-r--r--   0 root         (0) root         (0)     5921 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api/wellknown_api.py
+-rw-r--r--   0 root         (0) root         (0)    39202 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 16:51:50.996114 ory-client-1.9.0/ory_client/apis/
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18031 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5198 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 16:51:51.028114 ory-client-1.9.0/ory_client/model/
+-rw-r--r--   0 root         (0) root         (0)      344 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14362 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/accept_o_auth2_consent_request.py
+-rw-r--r--   0 root         (0) root         (0)    13401 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/accept_o_auth2_consent_request_session.py
+-rw-r--r--   0 root         (0) root         (0)    18750 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/accept_o_auth2_login_request.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/active_project_in_console.py
+-rw-r--r--   0 root         (0) root         (0)    11685 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/attribute.py
+-rw-r--r--   0 root         (0) root         (0)    12253 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/attribute_filter.py
+-rw-r--r--   0 root         (0) root         (0)    11965 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/attributes_count_datapoint.py
+-rw-r--r--   0 root         (0) root         (0)    13840 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/authenticator_assurance_level.py
+-rw-r--r--   0 root         (0) root         (0)    11964 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/batch_patch_identities_response.py
+-rw-r--r--   0 root         (0) root         (0)    11792 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/check_opl_syntax_result.py
+-rw-r--r--   0 root         (0) root         (0)    11697 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/check_permission_result.py
+-rw-r--r--   0 root         (0) root         (0)    11927 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/cloud_account.py
+-rw-r--r--   0 root         (0) root         (0)    13875 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/consistency_request_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    16213 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/continue_with.py
+-rw-r--r--   0 root         (0) root         (0)    12647 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/continue_with_recovery_ui.py
+-rw-r--r--   0 root         (0) root         (0)    11867 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/continue_with_recovery_ui_flow.py
+-rw-r--r--   0 root         (0) root         (0)    12653 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/continue_with_set_ory_session_token.py
+-rw-r--r--   0 root         (0) root         (0)    12647 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/continue_with_settings_ui.py
+-rw-r--r--   0 root         (0) root         (0)    11634 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/continue_with_settings_ui_flow.py
+-rw-r--r--   0 root         (0) root         (0)    12743 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/continue_with_verification_ui.py
+-rw-r--r--   0 root         (0) root         (0)    12337 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/continue_with_verification_ui_flow.py
+-rw-r--r--   0 root         (0) root         (0)    12313 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/courier_message_status.py
+-rw-r--r--   0 root         (0) root         (0)    12189 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/courier_message_type.py
+-rw-r--r--   0 root         (0) root         (0)    13118 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_custom_domain_body.py
+-rw-r--r--   0 root         (0) root         (0)    12602 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_event_stream_body.py
+-rw-r--r--   0 root         (0) root         (0)    17129 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)    12268 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_invite_response.py
+-rw-r--r--   0 root         (0) root         (0)    12838 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)    11909 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_member_invite_response.py
+-rw-r--r--   0 root         (0) root         (0)    11720 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_project_api_key_request.py
+-rw-r--r--   0 root         (0) root         (0)    12388 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_project_body.py
+-rw-r--r--   0 root         (0) root         (0)    12818 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_project_branding.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_project_member_invite_body.py
+-rw-r--r--   0 root         (0) root         (0)   146535 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_project_normalized_payload.py
+-rw-r--r--   0 root         (0) root         (0)    12513 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_recovery_code_for_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)    12510 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_recovery_link_for_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)    12810 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_relationship_body.py
+-rw-r--r--   0 root         (0) root         (0)    12912 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_subscription_body.py
+-rw-r--r--   0 root         (0) root         (0)    12519 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_subscription_common.py
+-rw-r--r--   0 root         (0) root         (0)    12261 2024-03-18 16:46:58.000000 ory-client-1.9.0/ory_client/model/create_verifiable_credential_request_body.py
+-rw-r--r--   0 root         (0) root         (0)    11656 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/create_workspace_member_invite_body.py
+-rw-r--r--   0 root         (0) root         (0)    11640 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/create_workspace_payload.py
+-rw-r--r--   0 root         (0) root         (0)    12540 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/create_workspace_subscription_body.py
+-rw-r--r--   0 root         (0) root         (0)    13492 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/credential_supported_draft00.py
+-rw-r--r--   0 root         (0) root         (0)    15192 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/custom_domain.py
+-rw-r--r--   0 root         (0) root         (0)    11634 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/delete_my_sessions_count.py
+-rw-r--r--   0 root         (0) root         (0)    12057 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/email_template_data.py
+-rw-r--r--   0 root         (0) root         (0)    11830 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/email_template_data_body.py
+-rw-r--r--   0 root         (0) root         (0)    12160 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/error_authenticator_assurance_level_not_satisfied.py
+-rw-r--r--   0 root         (0) root         (0)    12130 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/error_browser_location_change_required.py
+-rw-r--r--   0 root         (0) root         (0)    12119 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/error_flow_replaced.py
+-rw-r--r--   0 root         (0) root         (0)    11815 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/error_generic.py
+-rw-r--r--   0 root         (0) root         (0)    12699 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/error_o_auth2.py
+-rw-r--r--   0 root         (0) root         (0)    12528 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/event_stream.py
+-rw-r--r--   0 root         (0) root         (0)    13201 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/expanded_permission_tree.py
+-rw-r--r--   0 root         (0) root         (0)    12628 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/flow_error.py
+-rw-r--r--   0 root         (0) root         (0)    14404 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/generic_error.py
+-rw-r--r--   0 root         (0) root         (0)    12936 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/generic_error_content.py
+-rw-r--r--   0 root         (0) root         (0)    12338 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/generic_usage.py
+-rw-r--r--   0 root         (0) root         (0)    11849 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/get_attributes_count_response.py
+-rw-r--r--   0 root         (0) root         (0)    11596 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/get_managed_identity_schema_location.py
+-rw-r--r--   0 root         (0) root         (0)    11626 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/get_metrics_event_attributes_response.py
+-rw-r--r--   0 root         (0) root         (0)    11611 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/get_metrics_event_types_response.py
+-rw-r--r--   0 root         (0) root         (0)    11874 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/get_organization_response.py
+-rw-r--r--   0 root         (0) root         (0)    13505 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/get_project_events_body.py
+-rw-r--r--   0 root         (0) root         (0)    12199 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/get_project_events_response.py
+-rw-r--r--   0 root         (0) root         (0)    11797 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/get_project_metrics_response.py
+-rw-r--r--   0 root         (0) root         (0)    11849 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/get_session_activity_response.py
+-rw-r--r--   0 root         (0) root         (0)    11672 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/get_version200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11716 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/health_not_ready_status.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/health_status.py
+-rw-r--r--   0 root         (0) root         (0)    18610 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity.py
+-rw-r--r--   0 root         (0) root         (0)    14637 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    11908 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_credentials_code.py
+-rw-r--r--   0 root         (0) root         (0)    11911 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_credentials_oidc.py
+-rw-r--r--   0 root         (0) root         (0)    12763 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_credentials_oidc_provider.py
+-rw-r--r--   0 root         (0) root         (0)    11732 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_credentials_password.py
+-rw-r--r--   0 root         (0) root         (0)    12312 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_patch.py
+-rw-r--r--   0 root         (0) root         (0)    12511 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_patch_response.py
+-rw-r--r--   0 root         (0) root         (0)    12063 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_schema_container.py
+-rw-r--r--   0 root         (0) root         (0)    12109 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_schema_preset.py
+-rw-r--r--   0 root         (0) root         (0)    12084 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_schema_presets.py
+-rw-r--r--   0 root         (0) root         (0)    12217 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)    12317 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_with_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    11917 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_with_credentials_oidc.py
+-rw-r--r--   0 root         (0) root         (0)    12583 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_with_credentials_oidc_config.py
+-rw-r--r--   0 root         (0) root         (0)    12296 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_with_credentials_oidc_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)    11957 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_with_credentials_password.py
+-rw-r--r--   0 root         (0) root         (0)    12222 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/identity_with_credentials_password_config.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/internal_get_project_branding_body.py
+-rw-r--r--   0 root         (0) root         (0)    12074 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/internal_is_ax_welcome_screen_enabled_for_project_body.py
+-rw-r--r--   0 root         (0) root         (0)    12881 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/internal_is_owner_for_project_by_slug_body.py
+-rw-r--r--   0 root         (0) root         (0)    11767 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/internal_is_owner_for_project_by_slug_response.py
+-rw-r--r--   0 root         (0) root         (0)    18024 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/introspected_o_auth2_token.py
+-rw-r--r--   0 root         (0) root         (0)    12057 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/is_owner_for_project_by_slug.py
+-rw-r--r--   0 root         (0) root         (0)    11628 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/is_ready200_response.py
+-rw-r--r--   0 root         (0) root         (0)    11762 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/is_ready503_response.py
+-rw-r--r--   0 root         (0) root         (0)    13595 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/json_patch.py
+-rw-r--r--   0 root         (0) root         (0)    12088 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/json_patch_document.py
+-rw-r--r--   0 root         (0) root         (0)    18000 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)    12346 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)    11687 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/keto_namespace.py
+-rw-r--r--   0 root         (0) root         (0)    11999 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/keto_namespaces.py
+-rw-r--r--   0 root         (0) root         (0)    12087 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/list_custom_domains.py
+-rw-r--r--   0 root         (0) root         (0)    11768 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/list_event_streams.py
+-rw-r--r--   0 root         (0) root         (0)    12472 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/list_my_workspaces_response.py
+-rw-r--r--   0 root         (0) root         (0)    11897 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/list_organizations_response.py
+-rw-r--r--   0 root         (0) root         (0)    12413 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/list_workspace_projects_response.py
+-rw-r--r--   0 root         (0) root         (0)    21060 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/login_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13275 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/login_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)    12148 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/logout_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13567 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/managed_identity_schema.py
+-rw-r--r--   0 root         (0) root         (0)    11792 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/managed_identity_schema_validation_result.py
+-rw-r--r--   0 root         (0) root         (0)    12096 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/managed_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)    14688 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/member_invite.py
+-rw-r--r--   0 root         (0) root         (0)    11987 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/member_invites.py
+-rw-r--r--   0 root         (0) root         (0)    16717 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/message.py
+-rw-r--r--   0 root         (0) root         (0)    13688 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/message_dispatch.py
+-rw-r--r--   0 root         (0) root         (0)    11924 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/metrics_datapoint.py
+-rw-r--r--   0 root         (0) root         (0)    13562 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/migration_options.py
+-rw-r--r--   0 root         (0) root         (0)    11555 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/namespace.py
+-rw-r--r--   0 root         (0) root         (0)    12239 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/needs_privileged_session_error.py
+-rw-r--r--   0 root         (0) root         (0)    14951 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/normalized_project.py
+-rw-r--r--   0 root         (0) root         (0)   145843 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/normalized_project_revision.py
+-rw-r--r--   0 root         (0) root         (0)    17424 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/normalized_project_revision_courier_channel.py
+-rw-r--r--   0 root         (0) root         (0)    18363 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/normalized_project_revision_hook.py
+-rw-r--r--   0 root         (0) root         (0)    15526 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/normalized_project_revision_identity_schema.py
+-rw-r--r--   0 root         (0) root         (0)    12314 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/normalized_project_revision_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)    21407 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/normalized_project_revision_third_party_provider.py
+-rw-r--r--   0 root         (0) root         (0)    13893 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/normalized_project_revision_tokenizer_template.py
+-rw-r--r--   0 root         (0) root         (0)    12350 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/normalized_project_revision_tokenizer_templates.py
+-rw-r--r--   0 root         (0) root         (0)    12047 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/normalized_projects.py
+-rw-r--r--   0 root         (0) root         (0)    11898 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/null_duration.py
+-rw-r--r--   0 root         (0) root         (0)    39393 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/o_auth2_client.py
+-rw-r--r--   0 root         (0) root         (0)    15434 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/o_auth2_client_token_lifespans.py
+-rw-r--r--   0 root         (0) root         (0)    18510 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/o_auth2_consent_request.py
+-rw-r--r--   0 root         (0) root         (0)    18529 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/o_auth2_consent_request_open_id_connect_context.py
+-rw-r--r--   0 root         (0) root         (0)    15310 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/o_auth2_consent_session.py
+-rw-r--r--   0 root         (0) root         (0)    12544 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/o_auth2_consent_session_expires_at.py
+-rw-r--r--   0 root         (0) root         (0)    12229 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/o_auth2_consent_sessions.py
+-rw-r--r--   0 root         (0) root         (0)    17102 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/o_auth2_login_request.py
+-rw-r--r--   0 root         (0) root         (0)    13573 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/o_auth2_logout_request.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/o_auth2_redirect_to.py
+-rw-r--r--   0 root         (0) root         (0)    13565 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/o_auth2_token_exchange.py
+-rw-r--r--   0 root         (0) root         (0)    33786 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/oidc_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    24625 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/oidc_user_info.py
+-rw-r--r--   0 root         (0) root         (0)    13150 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/organization.py
+-rw-r--r--   0 root         (0) root         (0)    11924 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/organization_body.py
+-rw-r--r--   0 root         (0) root         (0)    12865 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/pagination.py
+-rw-r--r--   0 root         (0) root         (0)    12222 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/pagination_headers.py
+-rw-r--r--   0 root         (0) root         (0)    12124 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/parse_error.py
+-rw-r--r--   0 root         (0) root         (0)    11890 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/patch_identities_body.py
+-rw-r--r--   0 root         (0) root         (0)    11790 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/perform_native_logout_body.py
+-rw-r--r--   0 root         (0) root         (0)    11306 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/permissions_on_project.py
+-rw-r--r--   0 root         (0) root         (0)    11635 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/permissions_on_workpace_response.py
+-rw-r--r--   0 root         (0) root         (0)    11989 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/plan.py
+-rw-r--r--   0 root         (0) root         (0)    14438 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/plan_details.py
+-rw-r--r--   0 root         (0) root         (0)    11459 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/plan_features.py
+-rw-r--r--   0 root         (0) root         (0)    11781 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/plans.py
+-rw-r--r--   0 root         (0) root         (0)    12813 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/post_check_permission_body.py
+-rw-r--r--   0 root         (0) root         (0)    12834 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/post_check_permission_or_error_body.py
+-rw-r--r--   0 root         (0) root         (0)    11960 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/pricing.py
+-rw-r--r--   0 root         (0) root         (0)    13831 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project.py
+-rw-r--r--   0 root         (0) root         (0)    13276 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_api_key.py
+-rw-r--r--   0 root         (0) root         (0)    12000 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_api_keys.py
+-rw-r--r--   0 root         (0) root         (0)    13358 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_branding.py
+-rw-r--r--   0 root         (0) root         (0)    23906 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_branding_colors.py
+-rw-r--r--   0 root         (0) root         (0)    26889 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_branding_theme.py
+-rw-r--r--   0 root         (0) root         (0)    12084 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_branding_themes.py
+-rw-r--r--   0 root         (0) root         (0)    12190 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_cors.py
+-rw-r--r--   0 root         (0) root         (0)    12416 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_events_datapoint.py
+-rw-r--r--   0 root         (0) root         (0)    12070 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_host.py
+-rw-r--r--   0 root         (0) root         (0)    12120 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_member.py
+-rw-r--r--   0 root         (0) root         (0)    11999 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_members.py
+-rw-r--r--   0 root         (0) root         (0)    14913 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_metadata.py
+-rw-r--r--   0 root         (0) root         (0)    12032 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_metadata_list.py
+-rw-r--r--   0 root         (0) root         (0)    12163 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_revision_hooks.py
+-rw-r--r--   0 root         (0) root         (0)    12284 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_revision_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)    12348 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_revision_third_party_login_providers.py
+-rw-r--r--   0 root         (0) root         (0)    12114 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_revisions.py
+-rw-r--r--   0 root         (0) root         (0)    11808 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_service_identity.py
+-rw-r--r--   0 root         (0) root         (0)    11802 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_service_o_auth2.py
+-rw-r--r--   0 root         (0) root         (0)    11814 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_service_permission.py
+-rw-r--r--   0 root         (0) root         (0)    12615 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/project_services.py
+-rw-r--r--   0 root         (0) root         (0)    11926 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/projects.py
+-rw-r--r--   0 root         (0) root         (0)    16299 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/quota_usage.py
+-rw-r--r--   0 root         (0) root         (0)    12720 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/recovery_code_for_identity.py
+-rw-r--r--   0 root         (0) root         (0)    16698 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/recovery_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13316 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/recovery_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)    12615 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/recovery_identity_address.py
+-rw-r--r--   0 root         (0) root         (0)    12181 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/recovery_link_for_identity.py
+-rw-r--r--   0 root         (0) root         (0)    19640 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/registration_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13120 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/registration_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)    13273 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/reject_o_auth2_request.py
+-rw-r--r--   0 root         (0) root         (0)    12783 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/relation_query.py
+-rw-r--r--   0 root         (0) root         (0)    13010 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/relationship.py
+-rw-r--r--   0 root         (0) root         (0)    11756 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/relationship_namespaces.py
+-rw-r--r--   0 root         (0) root         (0)    12062 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/relationship_patch.py
+-rw-r--r--   0 root         (0) root         (0)    12258 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/relationships.py
+-rw-r--r--   0 root         (0) root         (0)    12263 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/revision_courier_channels.py
+-rw-r--r--   0 root         (0) root         (0)    12410 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/rfc6749_error_json.py
+-rw-r--r--   0 root         (0) root         (0)    12033 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/schema_patch.py
+-rw-r--r--   0 root         (0) root         (0)    12969 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/self_service_flow_expired_error.py
+-rw-r--r--   0 root         (0) root         (0)    15774 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/session.py
+-rw-r--r--   0 root         (0) root         (0)    12342 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/session_activity_datapoint.py
+-rw-r--r--   0 root         (0) root         (0)    13371 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/session_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)    12452 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/session_authentication_methods.py
+-rw-r--r--   0 root         (0) root         (0)    12379 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/session_device.py
+-rw-r--r--   0 root         (0) root         (0)    11805 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/set_active_project_in_console_body.py
+-rw-r--r--   0 root         (0) root         (0)    13091 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/set_custom_domain_body.py
+-rw-r--r--   0 root         (0) root         (0)    12593 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/set_event_stream_body.py
+-rw-r--r--   0 root         (0) root         (0)    12725 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/set_project.py
+-rw-r--r--   0 root         (0) root         (0)    12962 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/set_project_branding_theme_body.py
+-rw-r--r--   0 root         (0) root         (0)    17601 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/settings_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13574 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/settings_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)    11710 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/source_position.py
+-rw-r--r--   0 root         (0) root         (0)    11819 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/string_slice_json_format.py
+-rw-r--r--   0 root         (0) root         (0)    12219 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/subject_set.py
+-rw-r--r--   0 root         (0) root         (0)    18737 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    12500 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/successful_code_exchange_response.py
+-rw-r--r--   0 root         (0) root         (0)    12473 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/successful_native_login.py
+-rw-r--r--   0 root         (0) root         (0)    13754 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/successful_native_registration.py
+-rw-r--r--   0 root         (0) root         (0)    12962 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/successful_project_update.py
+-rw-r--r--   0 root         (0) root         (0)    12880 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/token_pagination.py
+-rw-r--r--   0 root         (0) root         (0)    12237 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/token_pagination_headers.py
+-rw-r--r--   0 root         (0) root         (0)    12930 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/token_pagination_request_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    13145 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/token_pagination_response_headers.py
+-rw-r--r--   0 root         (0) root         (0)    13912 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/trust_o_auth2_jwt_grant_issuer.py
+-rw-r--r--   0 root         (0) root         (0)    14486 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/trusted_o_auth2_jwt_grant_issuer.py
+-rw-r--r--   0 root         (0) root         (0)    12399 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/trusted_o_auth2_jwt_grant_issuers.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/trusted_o_auth2_jwt_grant_json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)    12714 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/ui_container.py
+-rw-r--r--   0 root         (0) root         (0)    14031 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/ui_node.py
+-rw-r--r--   0 root         (0) root         (0)    12852 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/ui_node_anchor_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    22091 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/ui_node_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    12956 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/ui_node_image_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    16763 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/ui_node_input_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    11669 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/ui_node_meta.py
+-rw-r--r--   0 root         (0) root         (0)    14565 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/ui_node_script_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    12555 2024-03-18 16:46:59.000000 ory-client-1.9.0/ory_client/model/ui_node_text_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    11915 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/ui_nodes.py
+-rw-r--r--   0 root         (0) root         (0)    12735 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/ui_text.py
+-rw-r--r--   0 root         (0) root         (0)    11915 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/ui_texts.py
+-rw-r--r--   0 root         (0) root         (0)    15089 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)    23673 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_login_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    13684 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_login_flow_with_code_method.py
+-rw-r--r--   0 root         (0) root         (0)    12516 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_login_flow_with_lookup_secret_method.py
+-rw-r--r--   0 root         (0) root         (0)    16813 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_login_flow_with_oidc_method.py
+-rw-r--r--   0 root         (0) root         (0)    13823 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_login_flow_with_password_method.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_login_flow_with_totp_method.py
+-rw-r--r--   0 root         (0) root         (0)    13476 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_login_flow_with_web_authn_method.py
+-rw-r--r--   0 root         (0) root         (0)    17254 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_recovery_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    14514 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_recovery_flow_with_code_method.py
+-rw-r--r--   0 root         (0) root         (0)    13596 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_recovery_flow_with_link_method.py
+-rw-r--r--   0 root         (0) root         (0)    22203 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_registration_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    13543 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_registration_flow_with_code_method.py
+-rw-r--r--   0 root         (0) root         (0)    16740 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_registration_flow_with_oidc_method.py
+-rw-r--r--   0 root         (0) root         (0)    13361 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_registration_flow_with_password_method.py
+-rw-r--r--   0 root         (0) root         (0)    14145 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_registration_flow_with_web_authn_method.py
+-rw-r--r--   0 root         (0) root         (0)    24071 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_settings_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    14085 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_settings_flow_with_lookup_method.py
+-rw-r--r--   0 root         (0) root         (0)    15448 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_settings_flow_with_oidc_method.py
+-rw-r--r--   0 root         (0) root         (0)    12897 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_settings_flow_with_password_method.py
+-rw-r--r--   0 root         (0) root         (0)    13156 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_settings_flow_with_profile_method.py
+-rw-r--r--   0 root         (0) root         (0)    13420 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_settings_flow_with_totp_method.py
+-rw-r--r--   0 root         (0) root         (0)    14084 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_settings_flow_with_web_authn_method.py
+-rw-r--r--   0 root         (0) root         (0)    12189 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_subscription_body.py
+-rw-r--r--   0 root         (0) root         (0)    17336 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_verification_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)    14532 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_verification_flow_with_code_method.py
+-rw-r--r--   0 root         (0) root         (0)    13646 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_verification_flow_with_link_method.py
+-rw-r--r--   0 root         (0) root         (0)    11642 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/update_workspace_payload.py
+-rw-r--r--   0 root         (0) root         (0)    11735 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/usage.py
+-rw-r--r--   0 root         (0) root         (0)    13096 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/verifiable_credential_priming_response.py
+-rw-r--r--   0 root         (0) root         (0)    11758 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/verifiable_credential_proof.py
+-rw-r--r--   0 root         (0) root         (0)    11827 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/verifiable_credential_response.py
+-rw-r--r--   0 root         (0) root         (0)    13725 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/verifiable_identity_address.py
+-rw-r--r--   0 root         (0) root         (0)    16175 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/verification_flow.py
+-rw-r--r--   0 root         (0) root         (0)    13344 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/verification_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)    11586 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/version.py
+-rw-r--r--   0 root         (0) root         (0)    11694 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/warning.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/workspace.py
+-rw-r--r--   0 root         (0) root         (0)    12813 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/workspace_meta.py
+-rw-r--r--   0 root         (0) root         (0)    11950 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model/workspaces.py
+-rw-r--r--   0 root         (0) root         (0)    82704 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 16:51:51.028114 ory-client-1.9.0/ory_client/models/
+-rw-r--r--   0 root         (0) root         (0)    22098 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14398 2024-03-18 16:47:00.000000 ory-client-1.9.0/ory_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 16:51:50.992114 ory-client-1.9.0/ory_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      486 2024-03-18 16:51:50.000000 ory-client-1.9.0/ory_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24698 2024-03-18 16:51:50.000000 ory-client-1.9.0/ory_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 16:51:50.000000 ory-client-1.9.0/ory_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-03-18 16:51:50.000000 ory-client-1.9.0/ory_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-03-18 16:51:50.000000 ory-client-1.9.0/ory_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-03-18 16:51:51.088114 ory-client-1.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-03-18 16:47:00.000000 ory-client-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 16:51:51.084114 ory-client-1.9.0/test/
+-rw-r--r--   0 root         (0) root         (0)     1279 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_accept_o_auth2_consent_request.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_accept_o_auth2_consent_request_session.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_accept_o_auth2_login_request.py
+-rw-r--r--   0 root         (0) root         (0)      930 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_active_project_in_console.py
+-rw-r--r--   0 root         (0) root         (0)      836 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_attribute.py
+-rw-r--r--   0 root         (0) root         (0)      879 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_attribute_filter.py
+-rw-r--r--   0 root         (0) root         (0)      943 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_attributes_count_datapoint.py
+-rw-r--r--   0 root         (0) root         (0)      964 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_authenticator_assurance_level.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_batch_patch_identities_response.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_check_opl_syntax_result.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_check_permission_result.py
+-rw-r--r--   0 root         (0) root         (0)      858 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_cloud_account.py
+-rw-r--r--   0 root         (0) root         (0)      971 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_consistency_request_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_continue_with.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_continue_with_recovery_ui.py
+-rw-r--r--   0 root         (0) root         (0)      959 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_continue_with_recovery_ui_flow.py
+-rw-r--r--   0 root         (0) root         (0)      988 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_continue_with_set_ory_session_token.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_continue_with_settings_ui.py
+-rw-r--r--   0 root         (0) root         (0)      959 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_continue_with_settings_ui_flow.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_continue_with_verification_ui.py
+-rw-r--r--   0 root         (0) root         (0)      987 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_continue_with_verification_ui_flow.py
+-rw-r--r--   0 root         (0) root         (0)      979 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_courier_api.py
+-rw-r--r--   0 root         (0) root         (0)      915 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_courier_message_status.py
+-rw-r--r--   0 root         (0) root         (0)      901 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_courier_message_type.py
+-rw-r--r--   0 root         (0) root         (0)      930 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_custom_domain_body.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_event_stream_body.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_invite_response.py
+-rw-r--r--   0 root         (0) root         (0)      910 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)      958 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_member_invite_response.py
+-rw-r--r--   0 root         (0) root         (0)      959 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_project_api_key_request.py
+-rw-r--r--   0 root         (0) root         (0)      894 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_project_body.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_project_branding.py
+-rw-r--r--   0 root         (0) root         (0)      980 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_project_member_invite_body.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_project_normalized_payload.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_recovery_code_for_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_recovery_link_for_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_relationship_body.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_subscription_body.py
+-rw-r--r--   0 root         (0) root         (0)      943 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_subscription_common.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-03-18 16:46:58.000000 ory-client-1.9.0/test/test_create_verifiable_credential_request_body.py
+-rw-r--r--   0 root         (0) root         (0)      994 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_create_workspace_member_invite_body.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_create_workspace_payload.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_create_workspace_subscription_body.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_credential_supported_draft00.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_custom_domain.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_delete_my_sessions_count.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_email_template_data.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_email_template_data_body.py
+-rw-r--r--   0 root         (0) root         (0)     1183 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_error_authenticator_assurance_level_not_satisfied.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_error_browser_location_change_required.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_error_flow_replaced.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_error_generic.py
+-rw-r--r--   0 root         (0) root         (0)      852 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_error_o_auth2.py
+-rw-r--r--   0 root         (0) root         (0)      851 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_event_stream.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_events_api.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_expanded_permission_tree.py
+-rw-r--r--   0 root         (0) root         (0)      837 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_flow_error.py
+-rw-r--r--   0 root         (0) root         (0)     5770 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_frontend_api.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_generic_error.py
+-rw-r--r--   0 root         (0) root         (0)      908 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_generic_error_content.py
+-rw-r--r--   0 root         (0) root         (0)      858 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_generic_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_get_attributes_count_response.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_get_managed_identity_schema_location.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_get_metrics_event_attributes_response.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_get_metrics_event_types_response.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_get_organization_response.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_get_project_events_body.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_get_project_events_response.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_get_project_metrics_response.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_get_session_activity_response.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_get_version200_response.py
+-rw-r--r--   0 root         (0) root         (0)      916 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_health_not_ready_status.py
+-rw-r--r--   0 root         (0) root         (0)      858 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_health_status.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)     3517 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_identity_api.py
+-rw-r--r--   0 root         (0) root         (0)      907 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_credentials.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_credentials_code.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_credentials_oidc.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_credentials_oidc_provider.py
+-rw-r--r--   0 root         (0) root         (0)      964 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_credentials_password.py
+-rw-r--r--   0 root         (0) root         (0)      987 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_patch.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_patch_response.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_schema_container.py
+-rw-r--r--   0 root         (0) root         (0)      915 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_schema_preset.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_schema_presets.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_with_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_with_credentials_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_with_credentials_oidc_config.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_with_credentials_oidc_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1193 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_with_credentials_password.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_identity_with_credentials_password_config.py
+-rw-r--r--   0 root         (0) root         (0)      987 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_internal_get_project_branding_body.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_internal_is_ax_welcome_screen_enabled_for_project_body.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_internal_is_owner_for_project_by_slug_body.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_internal_is_owner_for_project_by_slug_response.py
+-rw-r--r--   0 root         (0) root         (0)      937 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_introspected_o_auth2_token.py
+-rw-r--r--   0 root         (0) root         (0)      939 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_is_owner_for_project_by_slug.py
+-rw-r--r--   0 root         (0) root         (0)      901 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_is_ready200_response.py
+-rw-r--r--   0 root         (0) root         (0)      901 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_is_ready503_response.py
+-rw-r--r--   0 root         (0) root         (0)      837 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_json_patch.py
+-rw-r--r--   0 root         (0) root         (0)      979 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_json_patch_document.py
+-rw-r--r--   0 root         (0) root         (0)      845 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_json_web_key_set.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_jwk_api.py
+-rw-r--r--   0 root         (0) root         (0)      865 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_keto_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_keto_namespaces.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_list_custom_domains.py
+-rw-r--r--   0 root         (0) root         (0)      980 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_list_event_streams.py
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_list_my_workspaces_response.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_list_organizations_response.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_list_workspace_projects_response.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_login_flow.py
+-rw-r--r--   0 root         (0) root         (0)      873 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_login_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)      844 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_logout_flow.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_managed_identity_schema.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_managed_identity_schema_validation_result.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_managed_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)      858 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_member_invite.py
+-rw-r--r--   0 root         (0) root         (0)      962 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_member_invites.py
+-rw-r--r--   0 root         (0) root         (0)     1183 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_message.py
+-rw-r--r--   0 root         (0) root         (0)      879 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_message_dispatch.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_metrics_datapoint.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_migration_options.py
+-rw-r--r--   0 root         (0) root         (0)      836 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_needs_privileged_session_error.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_normalized_project.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_normalized_project_revision.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_normalized_project_revision_courier_channel.py
+-rw-r--r--   0 root         (0) root         (0)      979 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_normalized_project_revision_hook.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_normalized_project_revision_identity_schema.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_normalized_project_revision_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     1214 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_normalized_project_revision_third_party_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_normalized_project_revision_tokenizer_template.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_normalized_project_revision_tokenizer_templates.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_normalized_projects.py
+-rw-r--r--   0 root         (0) root         (0)      858 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_null_duration.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_o_auth2_api.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_o_auth2_client.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_o_auth2_client_token_lifespans.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_o_auth2_consent_request.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_o_auth2_consent_request_open_id_connect_context.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_o_auth2_consent_session.py
+-rw-r--r--   0 root         (0) root         (0)      981 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_o_auth2_consent_session_expires_at.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_o_auth2_consent_sessions.py
+-rw-r--r--   0 root         (0) root         (0)     1350 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_o_auth2_login_request.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_o_auth2_logout_request.py
+-rw-r--r--   0 root         (0) root         (0)      888 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_o_auth2_redirect_to.py
+-rw-r--r--   0 root         (0) root         (0)      909 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_o_auth2_token_exchange.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_oidc_api.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_oidc_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      859 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_oidc_user_info.py
+-rw-r--r--   0 root         (0) root         (0)      992 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_organization.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_organization_body.py
+-rw-r--r--   0 root         (0) root         (0)      843 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_pagination.py
+-rw-r--r--   0 root         (0) root         (0)      893 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_pagination_headers.py
+-rw-r--r--   0 root         (0) root         (0)      949 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_parse_error.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_patch_identities_body.py
+-rw-r--r--   0 root         (0) root         (0)      937 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_perform_native_logout_body.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_permission_api.py
+-rw-r--r--   0 root         (0) root         (0)      915 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_permissions_on_project.py
+-rw-r--r--   0 root         (0) root         (0)      979 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_permissions_on_workpace_response.py
+-rw-r--r--   0 root         (0) root         (0)      801 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_plan.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_plan_details.py
+-rw-r--r--   0 root         (0) root         (0)      955 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_plan_features.py
+-rw-r--r--   0 root         (0) root         (0)      808 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_plans.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_post_check_permission_body.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_post_check_permission_or_error_body.py
+-rw-r--r--   0 root         (0) root         (0)      915 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_pricing.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project.py
+-rw-r--r--   0 root         (0) root         (0)     3745 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_project_api.py
+-rw-r--r--   0 root         (0) root         (0)      866 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_api_key.py
+-rw-r--r--   0 root         (0) root         (0)      975 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_api_keys.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_branding.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_branding_colors.py
+-rw-r--r--   0 root         (0) root         (0)      915 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_branding_theme.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_branding_themes.py
+-rw-r--r--   0 root         (0) root         (0)      851 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_cors.py
+-rw-r--r--   0 root         (0) root         (0)     1013 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_events_datapoint.py
+-rw-r--r--   0 root         (0) root         (0)      851 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_host.py
+-rw-r--r--   0 root         (0) root         (0)      865 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_member.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_members.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_metadata_list.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_revision_hooks.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_revision_identity_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     1276 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_revision_third_party_login_providers.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_revisions.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_service_identity.py
+-rw-r--r--   0 root         (0) root         (0)      916 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_service_o_auth2.py
+-rw-r--r--   0 root         (0) root         (0)      943 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_service_permission.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_project_services.py
+-rw-r--r--   0 root         (0) root         (0)      905 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_projects.py
+-rw-r--r--   0 root         (0) root         (0)      844 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_quota_usage.py
+-rw-r--r--   0 root         (0) root         (0)      937 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_recovery_code_for_identity.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_recovery_flow.py
+-rw-r--r--   0 root         (0) root         (0)      894 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_recovery_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_recovery_identity_address.py
+-rw-r--r--   0 root         (0) root         (0)      937 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_recovery_link_for_identity.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_registration_flow.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_registration_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)      909 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_reject_o_auth2_request.py
+-rw-r--r--   0 root         (0) root         (0)      954 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_relation_query.py
+-rw-r--r--   0 root         (0) root         (0)      946 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_relationship.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_relationship_api.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_relationship_namespaces.py
+-rw-r--r--   0 root         (0) root         (0)      989 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_relationship_patch.py
+-rw-r--r--   0 root         (0) root         (0)      960 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_relationships.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_revision_courier_channels.py
+-rw-r--r--   0 root         (0) root         (0)      887 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_rfc6749_error_json.py
+-rw-r--r--   0 root         (0) root         (0)      851 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_schema_patch.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_self_service_flow_expired_error.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_session.py
+-rw-r--r--   0 root         (0) root         (0)      943 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_session_activity_datapoint.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_session_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_session_authentication_methods.py
+-rw-r--r--   0 root         (0) root         (0)      865 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_session_device.py
+-rw-r--r--   0 root         (0) root         (0)      981 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_set_active_project_in_console_body.py
+-rw-r--r--   0 root         (0) root         (0)      909 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_set_custom_domain_body.py
+-rw-r--r--   0 root         (0) root         (0)      902 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_set_event_stream_body.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_set_project.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_set_project_branding_theme_body.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_settings_flow.py
+-rw-r--r--   0 root         (0) root         (0)      894 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_settings_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)      872 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_source_position.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_string_slice_json_format.py
+-rw-r--r--   0 root         (0) root         (0)      844 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_subject_set.py
+-rw-r--r--   0 root         (0) root         (0)      950 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_successful_code_exchange_response.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_successful_native_login.py
+-rw-r--r--   0 root         (0) root         (0)     1224 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_successful_native_registration.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_successful_project_update.py
+-rw-r--r--   0 root         (0) root         (0)      879 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_token_pagination.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_token_pagination_headers.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_token_pagination_request_parameters.py
+-rw-r--r--   0 root         (0) root         (0)      986 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_token_pagination_response_headers.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_trust_o_auth2_jwt_grant_issuer.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_trusted_o_auth2_jwt_grant_issuer.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_trusted_o_auth2_jwt_grant_issuers.py
+-rw-r--r--   0 root         (0) root         (0)      997 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_trusted_o_auth2_jwt_grant_json_web_key.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_ui_container.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_ui_node.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_ui_node_anchor_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_ui_node_attributes.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_ui_node_image_attributes.py
+-rw-r--r--   0 root         (0) root         (0)      996 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_ui_node_input_attributes.py
+-rw-r--r--   0 root         (0) root         (0)      918 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_ui_node_meta.py
+-rw-r--r--   0 root         (0) root         (0)      930 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_ui_node_script_attributes.py
+-rw-r--r--   0 root         (0) root         (0)      989 2024-03-18 16:46:59.000000 ory-client-1.9.0/test/test_ui_node_text_attributes.py
+-rw-r--r--   0 root         (0) root         (0)      896 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_ui_nodes.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_ui_text.py
+-rw-r--r--   0 root         (0) root         (0)      896 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_ui_texts.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_identity_body.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_login_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)      981 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_login_flow_with_code_method.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_login_flow_with_lookup_secret_method.py
+-rw-r--r--   0 root         (0) root         (0)      981 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_login_flow_with_oidc_method.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_login_flow_with_password_method.py
+-rw-r--r--   0 root         (0) root         (0)      981 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_login_flow_with_totp_method.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_login_flow_with_web_authn_method.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_recovery_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_recovery_flow_with_code_method.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_recovery_flow_with_link_method.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_registration_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_registration_flow_with_code_method.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_registration_flow_with_oidc_method.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_registration_flow_with_password_method.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_registration_flow_with_web_authn_method.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_settings_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_settings_flow_with_lookup_method.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_settings_flow_with_oidc_method.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_settings_flow_with_password_method.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_settings_flow_with_profile_method.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_settings_flow_with_totp_method.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_settings_flow_with_web_authn_method.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_subscription_body.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_verification_flow_body.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_verification_flow_with_code_method.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_verification_flow_with_link_method.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_update_workspace_payload.py
+-rw-r--r--   0 root         (0) root         (0)      905 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_verifiable_credential_priming_response.py
+-rw-r--r--   0 root         (0) root         (0)      950 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_verifiable_credential_proof.py
+-rw-r--r--   0 root         (0) root         (0)      971 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_verifiable_credential_response.py
+-rw-r--r--   0 root         (0) root         (0)      950 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_verifiable_identity_address.py
+-rw-r--r--   0 root         (0) root         (0)      979 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_verification_flow.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_verification_flow_state.py
+-rw-r--r--   0 root         (0) root         (0)      822 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_version.py
+-rw-r--r--   0 root         (0) root         (0)      822 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_warning.py
+-rw-r--r--   0 root         (0) root         (0)      863 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_wellknown_api.py
+-rw-r--r--   0 root         (0) root         (0)      836 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_workspace.py
+-rw-r--r--   0 root         (0) root         (0)      865 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_workspace_meta.py
+-rw-r--r--   0 root         (0) root         (0)      927 2024-03-18 16:47:00.000000 ory-client-1.9.0/test/test_workspaces.py
```

### Comparing `ory-client-1.8.1/README.md` & `ory-client-1.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # ory-client
 Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed
 with a valid Personal Access Token. Public APIs are mostly used in browsers.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: v1.8.1
-- Package version: v1.8.1
+- API version: v1.9.0
+- Package version: v1.9.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >=3.6
 
 ## Installation & Usage
```

### Comparing `ory-client-1.8.1/ory_client/__init__.py` & `ory-client-1.9.0/ory_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # flake8: noqa
 
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "v1.8.1"
+__version__ = "v1.9.0"
 
 # import ApiClient
 from ory_client.api_client import ApiClient
 
 # import Configuration
 from ory_client.configuration import Configuration
```

### Comparing `ory-client-1.8.1/ory_client/api/courier_api.py` & `ory-client-1.9.0/ory_client/api/courier_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/api/events_api.py` & `ory-client-1.9.0/ory_client/api/events_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/api/frontend_api.py` & `ory-client-1.9.0/ory_client/api/frontend_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/api/identity_api.py` & `ory-client-1.9.0/ory_client/api/identity_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/api/jwk_api.py` & `ory-client-1.9.0/ory_client/api/jwk_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/api/metadata_api.py` & `ory-client-1.9.0/ory_client/api/metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/api/o_auth2_api.py` & `ory-client-1.9.0/ory_client/api/o_auth2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/api/oidc_api.py` & `ory-client-1.9.0/ory_client/api/oidc_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/api/permission_api.py` & `ory-client-1.9.0/ory_client/api/permission_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/api/project_api.py` & `ory-client-1.9.0/ory_client/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/api/relationship_api.py` & `ory-client-1.9.0/ory_client/api/relationship_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/api/wellknown_api.py` & `ory-client-1.9.0/ory_client/api/wellknown_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/api_client.py` & `ory-client-1.9.0/ory_client/api_client.py`

 * *Files identical despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/v1.8.1/python'
+        self.user_agent = 'OpenAPI-Generator/v1.9.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ory-client-1.8.1/ory_client/apis/__init__.py` & `ory-client-1.9.0/ory_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ory-client-1.8.1/ory_client/configuration.py` & `ory-client-1.9.0/ory_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -421,16 +421,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: v1.8.1\n"\
-               "SDK Package Version: v1.8.1".\
+               "Version of the API: v1.9.0\n"\
+               "SDK Package Version: v1.9.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ory-client-1.8.1/ory_client/exceptions.py` & `ory-client-1.9.0/ory_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `ory-client-1.8.1/ory_client/model/accept_o_auth2_consent_request.py` & `ory-client-1.9.0/ory_client/model/accept_o_auth2_consent_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/accept_o_auth2_consent_request_session.py` & `ory-client-1.9.0/ory_client/model/accept_o_auth2_consent_request_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/accept_o_auth2_login_request.py` & `ory-client-1.9.0/ory_client/model/accept_o_auth2_login_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/active_project_in_console.py` & `ory-client-1.9.0/ory_client/model/active_project_in_console.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/attribute.py` & `ory-client-1.9.0/ory_client/model/attribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/attribute_filter.py` & `ory-client-1.9.0/ory_client/model/attribute_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/attributes_count_datapoint.py` & `ory-client-1.9.0/ory_client/model/attributes_count_datapoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/authenticator_assurance_level.py` & `ory-client-1.9.0/ory_client/model/authenticator_assurance_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/batch_patch_identities_response.py` & `ory-client-1.9.0/ory_client/model/batch_patch_identities_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/check_opl_syntax_result.py` & `ory-client-1.9.0/ory_client/model/check_opl_syntax_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/check_permission_result.py` & `ory-client-1.9.0/ory_client/model/check_permission_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/cloud_account.py` & `ory-client-1.9.0/ory_client/model/cloud_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/consistency_request_parameters.py` & `ory-client-1.9.0/ory_client/model/consistency_request_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/continue_with.py` & `ory-client-1.9.0/ory_client/model/continue_with.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/continue_with_recovery_ui.py` & `ory-client-1.9.0/ory_client/model/continue_with_recovery_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/continue_with_recovery_ui_flow.py` & `ory-client-1.9.0/ory_client/model/continue_with_recovery_ui_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/continue_with_set_ory_session_token.py` & `ory-client-1.9.0/ory_client/model/continue_with_set_ory_session_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/continue_with_settings_ui.py` & `ory-client-1.9.0/ory_client/model/continue_with_settings_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/continue_with_settings_ui_flow.py` & `ory-client-1.9.0/ory_client/model/continue_with_settings_ui_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/continue_with_verification_ui.py` & `ory-client-1.9.0/ory_client/model/continue_with_verification_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/continue_with_verification_ui_flow.py` & `ory-client-1.9.0/ory_client/model/continue_with_verification_ui_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/courier_message_status.py` & `ory-client-1.9.0/ory_client/model/courier_message_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/courier_message_type.py` & `ory-client-1.9.0/ory_client/model/courier_message_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_custom_domain_body.py` & `ory-client-1.9.0/ory_client/model/create_custom_domain_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_event_stream_body.py` & `ory-client-1.9.0/ory_client/model/create_event_stream_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_identity_body.py` & `ory-client-1.9.0/ory_client/model/create_identity_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_invite_response.py` & `ory-client-1.9.0/ory_client/model/create_invite_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_json_web_key_set.py` & `ory-client-1.9.0/ory_client/model/create_json_web_key_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_member_invite_response.py` & `ory-client-1.9.0/ory_client/model/create_member_invite_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_project_api_key_request.py` & `ory-client-1.9.0/ory_client/model/create_project_api_key_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_project_body.py` & `ory-client-1.9.0/ory_client/model/create_project_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_project_branding.py` & `ory-client-1.9.0/ory_client/model/create_project_branding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_project_member_invite_body.py` & `ory-client-1.9.0/ory_client/model/create_project_member_invite_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_project_normalized_payload.py` & `ory-client-1.9.0/ory_client/model/create_project_normalized_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -246,14 +246,15 @@
             'kratos_courier_templates_verification_invalid_email_body_html': (str,),  # noqa: E501
             'kratos_courier_templates_verification_invalid_email_body_plaintext': (str,),  # noqa: E501
             'kratos_courier_templates_verification_invalid_email_subject': (str,),  # noqa: E501
             'kratos_courier_templates_verification_valid_email_body_html': (str,),  # noqa: E501
             'kratos_courier_templates_verification_valid_email_body_plaintext': (str,),  # noqa: E501
             'kratos_courier_templates_verification_valid_email_subject': (str,),  # noqa: E501
             'kratos_feature_flags_cacheable_sessions': (bool,),  # noqa: E501
+            'kratos_feature_flags_cacheable_sessions_max_age': (str,),  # noqa: E501
             'kratos_feature_flags_use_continue_with_transitions': (bool,),  # noqa: E501
             'kratos_identity_schemas': (ProjectRevisionIdentitySchemas,),  # noqa: E501
             'kratos_oauth2_provider_headers': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'kratos_oauth2_provider_override_return_to': (bool,),  # noqa: E501
             'kratos_oauth2_provider_url': (str,),  # noqa: E501
             'kratos_preview_default_read_consistency_level': (str,),  # noqa: E501
             'kratos_secrets_cipher': (StringSliceJSONFormat,),  # noqa: E501
@@ -448,14 +449,15 @@
         'kratos_courier_templates_verification_invalid_email_body_html': 'kratos_courier_templates_verification_invalid_email_body_html',  # noqa: E501
         'kratos_courier_templates_verification_invalid_email_body_plaintext': 'kratos_courier_templates_verification_invalid_email_body_plaintext',  # noqa: E501
         'kratos_courier_templates_verification_invalid_email_subject': 'kratos_courier_templates_verification_invalid_email_subject',  # noqa: E501
         'kratos_courier_templates_verification_valid_email_body_html': 'kratos_courier_templates_verification_valid_email_body_html',  # noqa: E501
         'kratos_courier_templates_verification_valid_email_body_plaintext': 'kratos_courier_templates_verification_valid_email_body_plaintext',  # noqa: E501
         'kratos_courier_templates_verification_valid_email_subject': 'kratos_courier_templates_verification_valid_email_subject',  # noqa: E501
         'kratos_feature_flags_cacheable_sessions': 'kratos_feature_flags_cacheable_sessions',  # noqa: E501
+        'kratos_feature_flags_cacheable_sessions_max_age': 'kratos_feature_flags_cacheable_sessions_max_age',  # noqa: E501
         'kratos_feature_flags_use_continue_with_transitions': 'kratos_feature_flags_use_continue_with_transitions',  # noqa: E501
         'kratos_identity_schemas': 'kratos_identity_schemas',  # noqa: E501
         'kratos_oauth2_provider_headers': 'kratos_oauth2_provider_headers',  # noqa: E501
         'kratos_oauth2_provider_override_return_to': 'kratos_oauth2_provider_override_return_to',  # noqa: E501
         'kratos_oauth2_provider_url': 'kratos_oauth2_provider_url',  # noqa: E501
         'kratos_preview_default_read_consistency_level': 'kratos_preview_default_read_consistency_level',  # noqa: E501
         'kratos_secrets_cipher': 'kratos_secrets_cipher',  # noqa: E501
@@ -690,14 +692,15 @@
             kratos_courier_templates_verification_invalid_email_body_html (str): Configures the Ory Kratos Invalid Verification Email Body HTML Template  This governs the \"courier.smtp.templates.verification.invalid.email.body.html\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_invalid_email_body_plaintext (str): Configures the Ory Kratos Invalid Verification Email Body Plaintext Template  This governs the \"courier.smtp.templates.verification.invalid.email.body.plaintext\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_invalid_email_subject (str): Configures the Ory Kratos Invalid Verification Email Subject Template  This governs the \"courier.smtp.templates.verification.invalid.email.subject\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_valid_email_body_html (str): Configures the Ory Kratos Valid Verification Email Body HTML Template  This governs the \"courier.smtp.templates.verification.valid.email.body.html\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_valid_email_body_plaintext (str): Configures the Ory Kratos Valid Verification Email Body Plaintext Template  This governs the \"courier.smtp.templates.verification.valid.email.body.plaintext\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_valid_email_subject (str): Configures the Ory Kratos Valid Verification Email Subject Template  This governs the \"courier.smtp.templates.verification.valid.email.subject\" setting.. [optional]  # noqa: E501
             kratos_feature_flags_cacheable_sessions (bool): Configures the Ory Kratos Session caching feature flag  This governs the \"feature_flags.cacheable_sessions\" setting.. [optional]  # noqa: E501
+            kratos_feature_flags_cacheable_sessions_max_age (str): Configures the Ory Kratos Session caching max-age feature flag  This governs the \"feature_flags.cacheable_sessions_max_age\" setting.. [optional]  # noqa: E501
             kratos_feature_flags_use_continue_with_transitions (bool): Configures the Ory Kratos Session use_continue_with_transitions flag  This governs the \"feature_flags.use_continue_with_transitions\" setting.. [optional]  # noqa: E501
             kratos_identity_schemas (ProjectRevisionIdentitySchemas): [optional]  # noqa: E501
             kratos_oauth2_provider_headers ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): NullJSONRawMessage represents a json.RawMessage that works well with JSON, SQL, and Swagger and is NULLable-. [optional]  # noqa: E501
             kratos_oauth2_provider_override_return_to (bool): Kratos OAuth2 Provider Override Return To  Enabling this allows Kratos to set the return_to parameter automatically to the OAuth2 request URL on the login flow, allowing complex flows such as recovery to continue to the initial OAuth2 flow.. [optional]  # noqa: E501
             kratos_oauth2_provider_url (str): The Revisions' OAuth2 Provider Integration URL  This governs the \"oauth2_provider.url\" setting.. [optional]  # noqa: E501
             kratos_preview_default_read_consistency_level (str): Configures the default read consistency level for identity APIs  This governs the `preview.default_read_consistency_level` setting.  The read consistency level determines the consistency guarantee for reads:  strong (slow): The read is guaranteed to return the most recent data committed at the start of the read. eventual (very fast): The result will return data that is about 4.8 seconds old.  Setting the default consistency level to `eventual` may cause regressions in the future as we add consistency controls to more APIs. Currently, the following APIs will be affected by this setting:  `GET /admin/identities`  Defaults to \"strong\" for new and existing projects. This feature is in preview. Use with caution.. [optional]  # noqa: E501
             kratos_secrets_cipher (StringSliceJSONFormat): [optional]  # noqa: E501
@@ -973,14 +976,15 @@
             kratos_courier_templates_verification_invalid_email_body_html (str): Configures the Ory Kratos Invalid Verification Email Body HTML Template  This governs the \"courier.smtp.templates.verification.invalid.email.body.html\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_invalid_email_body_plaintext (str): Configures the Ory Kratos Invalid Verification Email Body Plaintext Template  This governs the \"courier.smtp.templates.verification.invalid.email.body.plaintext\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_invalid_email_subject (str): Configures the Ory Kratos Invalid Verification Email Subject Template  This governs the \"courier.smtp.templates.verification.invalid.email.subject\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_valid_email_body_html (str): Configures the Ory Kratos Valid Verification Email Body HTML Template  This governs the \"courier.smtp.templates.verification.valid.email.body.html\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_valid_email_body_plaintext (str): Configures the Ory Kratos Valid Verification Email Body Plaintext Template  This governs the \"courier.smtp.templates.verification.valid.email.body.plaintext\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_valid_email_subject (str): Configures the Ory Kratos Valid Verification Email Subject Template  This governs the \"courier.smtp.templates.verification.valid.email.subject\" setting.. [optional]  # noqa: E501
             kratos_feature_flags_cacheable_sessions (bool): Configures the Ory Kratos Session caching feature flag  This governs the \"feature_flags.cacheable_sessions\" setting.. [optional]  # noqa: E501
+            kratos_feature_flags_cacheable_sessions_max_age (str): Configures the Ory Kratos Session caching max-age feature flag  This governs the \"feature_flags.cacheable_sessions_max_age\" setting.. [optional]  # noqa: E501
             kratos_feature_flags_use_continue_with_transitions (bool): Configures the Ory Kratos Session use_continue_with_transitions flag  This governs the \"feature_flags.use_continue_with_transitions\" setting.. [optional]  # noqa: E501
             kratos_identity_schemas (ProjectRevisionIdentitySchemas): [optional]  # noqa: E501
             kratos_oauth2_provider_headers ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): NullJSONRawMessage represents a json.RawMessage that works well with JSON, SQL, and Swagger and is NULLable-. [optional]  # noqa: E501
             kratos_oauth2_provider_override_return_to (bool): Kratos OAuth2 Provider Override Return To  Enabling this allows Kratos to set the return_to parameter automatically to the OAuth2 request URL on the login flow, allowing complex flows such as recovery to continue to the initial OAuth2 flow.. [optional]  # noqa: E501
             kratos_oauth2_provider_url (str): The Revisions' OAuth2 Provider Integration URL  This governs the \"oauth2_provider.url\" setting.. [optional]  # noqa: E501
             kratos_preview_default_read_consistency_level (str): Configures the default read consistency level for identity APIs  This governs the `preview.default_read_consistency_level` setting.  The read consistency level determines the consistency guarantee for reads:  strong (slow): The read is guaranteed to return the most recent data committed at the start of the read. eventual (very fast): The result will return data that is about 4.8 seconds old.  Setting the default consistency level to `eventual` may cause regressions in the future as we add consistency controls to more APIs. Currently, the following APIs will be affected by this setting:  `GET /admin/identities`  Defaults to \"strong\" for new and existing projects. This feature is in preview. Use with caution.. [optional]  # noqa: E501
             kratos_secrets_cipher (StringSliceJSONFormat): [optional]  # noqa: E501
```

### Comparing `ory-client-1.8.1/ory_client/model/create_recovery_code_for_identity_body.py` & `ory-client-1.9.0/ory_client/model/create_recovery_code_for_identity_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_recovery_link_for_identity_body.py` & `ory-client-1.9.0/ory_client/model/create_recovery_link_for_identity_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_relationship_body.py` & `ory-client-1.9.0/ory_client/model/create_relationship_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_subscription_body.py` & `ory-client-1.9.0/ory_client/model/create_subscription_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_subscription_common.py` & `ory-client-1.9.0/ory_client/model/create_subscription_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_verifiable_credential_request_body.py` & `ory-client-1.9.0/ory_client/model/create_verifiable_credential_request_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_workspace_member_invite_body.py` & `ory-client-1.9.0/ory_client/model/create_workspace_member_invite_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_workspace_payload.py` & `ory-client-1.9.0/ory_client/model/create_workspace_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/create_workspace_subscription_body.py` & `ory-client-1.9.0/ory_client/model/create_workspace_subscription_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/credential_supported_draft00.py` & `ory-client-1.9.0/ory_client/model/credential_supported_draft00.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/custom_domain.py` & `ory-client-1.9.0/ory_client/model/custom_domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/delete_my_sessions_count.py` & `ory-client-1.9.0/ory_client/model/delete_my_sessions_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/email_template_data.py` & `ory-client-1.9.0/ory_client/model/email_template_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/email_template_data_body.py` & `ory-client-1.9.0/ory_client/model/email_template_data_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/error_authenticator_assurance_level_not_satisfied.py` & `ory-client-1.9.0/ory_client/model/error_authenticator_assurance_level_not_satisfied.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/error_browser_location_change_required.py` & `ory-client-1.9.0/ory_client/model/error_browser_location_change_required.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/error_flow_replaced.py` & `ory-client-1.9.0/ory_client/model/error_flow_replaced.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/error_generic.py` & `ory-client-1.9.0/ory_client/model/error_generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/error_o_auth2.py` & `ory-client-1.9.0/ory_client/model/error_o_auth2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/event_stream.py` & `ory-client-1.9.0/ory_client/model/event_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/expanded_permission_tree.py` & `ory-client-1.9.0/ory_client/model/expanded_permission_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/flow_error.py` & `ory-client-1.9.0/ory_client/model/flow_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/generic_error.py` & `ory-client-1.9.0/ory_client/model/generic_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/generic_error_content.py` & `ory-client-1.9.0/ory_client/model/generic_error_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/generic_usage.py` & `ory-client-1.9.0/ory_client/model/generic_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/get_attributes_count_response.py` & `ory-client-1.9.0/ory_client/model/get_attributes_count_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/get_managed_identity_schema_location.py` & `ory-client-1.9.0/ory_client/model/get_managed_identity_schema_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/get_metrics_event_attributes_response.py` & `ory-client-1.9.0/ory_client/model/get_metrics_event_attributes_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/get_metrics_event_types_response.py` & `ory-client-1.9.0/ory_client/model/get_metrics_event_types_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/get_organization_response.py` & `ory-client-1.9.0/ory_client/model/get_organization_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/get_project_events_body.py` & `ory-client-1.9.0/ory_client/model/get_project_events_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/get_project_events_response.py` & `ory-client-1.9.0/ory_client/model/get_project_events_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/get_project_metrics_response.py` & `ory-client-1.9.0/ory_client/model/get_project_metrics_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/get_session_activity_response.py` & `ory-client-1.9.0/ory_client/model/get_session_activity_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/get_version200_response.py` & `ory-client-1.9.0/ory_client/model/get_version200_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/health_not_ready_status.py` & `ory-client-1.9.0/ory_client/model/health_not_ready_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/health_status.py` & `ory-client-1.9.0/ory_client/model/health_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity.py` & `ory-client-1.9.0/ory_client/model/identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_credentials.py` & `ory-client-1.9.0/ory_client/model/identity_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_credentials_code.py` & `ory-client-1.9.0/ory_client/model/identity_credentials_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_credentials_oidc.py` & `ory-client-1.9.0/ory_client/model/identity_credentials_oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_credentials_oidc_provider.py` & `ory-client-1.9.0/ory_client/model/identity_credentials_oidc_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_credentials_password.py` & `ory-client-1.9.0/ory_client/model/identity_credentials_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_patch.py` & `ory-client-1.9.0/ory_client/model/identity_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_patch_response.py` & `ory-client-1.9.0/ory_client/model/identity_patch_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_schema_container.py` & `ory-client-1.9.0/ory_client/model/identity_schema_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_schema_preset.py` & `ory-client-1.9.0/ory_client/model/identity_schema_preset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_schema_presets.py` & `ory-client-1.9.0/ory_client/model/identity_schema_presets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_schemas.py` & `ory-client-1.9.0/ory_client/model/identity_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_with_credentials.py` & `ory-client-1.9.0/ory_client/model/identity_with_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_with_credentials_oidc.py` & `ory-client-1.9.0/ory_client/model/identity_with_credentials_oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_with_credentials_oidc_config.py` & `ory-client-1.9.0/ory_client/model/identity_with_credentials_oidc_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_with_credentials_oidc_config_provider.py` & `ory-client-1.9.0/ory_client/model/identity_with_credentials_oidc_config_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_with_credentials_password.py` & `ory-client-1.9.0/ory_client/model/identity_with_credentials_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/identity_with_credentials_password_config.py` & `ory-client-1.9.0/ory_client/model/identity_with_credentials_password_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/internal_get_project_branding_body.py` & `ory-client-1.9.0/ory_client/model/internal_get_project_branding_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/internal_is_ax_welcome_screen_enabled_for_project_body.py` & `ory-client-1.9.0/ory_client/model/internal_is_ax_welcome_screen_enabled_for_project_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/internal_is_owner_for_project_by_slug_body.py` & `ory-client-1.9.0/ory_client/model/internal_is_owner_for_project_by_slug_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/internal_is_owner_for_project_by_slug_response.py` & `ory-client-1.9.0/ory_client/model/internal_is_owner_for_project_by_slug_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/introspected_o_auth2_token.py` & `ory-client-1.9.0/ory_client/model/introspected_o_auth2_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/is_owner_for_project_by_slug.py` & `ory-client-1.9.0/ory_client/model/is_owner_for_project_by_slug.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/is_ready200_response.py` & `ory-client-1.9.0/ory_client/model/is_ready200_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/is_ready503_response.py` & `ory-client-1.9.0/ory_client/model/is_ready503_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/json_patch.py` & `ory-client-1.9.0/ory_client/model/json_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/json_patch_document.py` & `ory-client-1.9.0/ory_client/model/json_patch_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/json_web_key.py` & `ory-client-1.9.0/ory_client/model/json_web_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/json_web_key_set.py` & `ory-client-1.9.0/ory_client/model/json_web_key_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/keto_namespace.py` & `ory-client-1.9.0/ory_client/model/keto_namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/keto_namespaces.py` & `ory-client-1.9.0/ory_client/model/keto_namespaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/list_custom_domains.py` & `ory-client-1.9.0/ory_client/model/list_custom_domains.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/list_event_streams.py` & `ory-client-1.9.0/ory_client/model/list_event_streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/list_my_workspaces_response.py` & `ory-client-1.9.0/ory_client/model/list_my_workspaces_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/list_organizations_response.py` & `ory-client-1.9.0/ory_client/model/list_organizations_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/list_workspace_projects_response.py` & `ory-client-1.9.0/ory_client/model/list_workspace_projects_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/login_flow.py` & `ory-client-1.9.0/ory_client/model/login_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/login_flow_state.py` & `ory-client-1.9.0/ory_client/model/login_flow_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/logout_flow.py` & `ory-client-1.9.0/ory_client/model/logout_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/managed_identity_schema.py` & `ory-client-1.9.0/ory_client/model/managed_identity_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/managed_identity_schema_validation_result.py` & `ory-client-1.9.0/ory_client/model/managed_identity_schema_validation_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/managed_identity_schemas.py` & `ory-client-1.9.0/ory_client/model/managed_identity_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/member_invite.py` & `ory-client-1.9.0/ory_client/model/member_invite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/member_invites.py` & `ory-client-1.9.0/ory_client/model/member_invites.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/message.py` & `ory-client-1.9.0/ory_client/model/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/message_dispatch.py` & `ory-client-1.9.0/ory_client/model/message_dispatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/metrics_datapoint.py` & `ory-client-1.9.0/ory_client/model/metrics_datapoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/migration_options.py` & `ory-client-1.9.0/ory_client/model/migration_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/namespace.py` & `ory-client-1.9.0/ory_client/model/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/needs_privileged_session_error.py` & `ory-client-1.9.0/ory_client/model/needs_privileged_session_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/normalized_project.py` & `ory-client-1.9.0/ory_client/model/normalized_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/normalized_project_revision.py` & `ory-client-1.9.0/ory_client/model/normalized_project_revision.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -241,14 +241,15 @@
             'kratos_courier_templates_verification_invalid_email_body_html': (str,),  # noqa: E501
             'kratos_courier_templates_verification_invalid_email_body_plaintext': (str,),  # noqa: E501
             'kratos_courier_templates_verification_invalid_email_subject': (str,),  # noqa: E501
             'kratos_courier_templates_verification_valid_email_body_html': (str,),  # noqa: E501
             'kratos_courier_templates_verification_valid_email_body_plaintext': (str,),  # noqa: E501
             'kratos_courier_templates_verification_valid_email_subject': (str,),  # noqa: E501
             'kratos_feature_flags_cacheable_sessions': (bool,),  # noqa: E501
+            'kratos_feature_flags_cacheable_sessions_max_age': (str,),  # noqa: E501
             'kratos_feature_flags_use_continue_with_transitions': (bool,),  # noqa: E501
             'kratos_identity_schemas': (ProjectRevisionIdentitySchemas,),  # noqa: E501
             'kratos_oauth2_provider_headers': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'kratos_oauth2_provider_override_return_to': (bool,),  # noqa: E501
             'kratos_oauth2_provider_url': (str,),  # noqa: E501
             'kratos_preview_default_read_consistency_level': (str,),  # noqa: E501
             'kratos_secrets_cipher': (StringSliceJSONFormat,),  # noqa: E501
@@ -441,14 +442,15 @@
         'kratos_courier_templates_verification_invalid_email_body_html': 'kratos_courier_templates_verification_invalid_email_body_html',  # noqa: E501
         'kratos_courier_templates_verification_invalid_email_body_plaintext': 'kratos_courier_templates_verification_invalid_email_body_plaintext',  # noqa: E501
         'kratos_courier_templates_verification_invalid_email_subject': 'kratos_courier_templates_verification_invalid_email_subject',  # noqa: E501
         'kratos_courier_templates_verification_valid_email_body_html': 'kratos_courier_templates_verification_valid_email_body_html',  # noqa: E501
         'kratos_courier_templates_verification_valid_email_body_plaintext': 'kratos_courier_templates_verification_valid_email_body_plaintext',  # noqa: E501
         'kratos_courier_templates_verification_valid_email_subject': 'kratos_courier_templates_verification_valid_email_subject',  # noqa: E501
         'kratos_feature_flags_cacheable_sessions': 'kratos_feature_flags_cacheable_sessions',  # noqa: E501
+        'kratos_feature_flags_cacheable_sessions_max_age': 'kratos_feature_flags_cacheable_sessions_max_age',  # noqa: E501
         'kratos_feature_flags_use_continue_with_transitions': 'kratos_feature_flags_use_continue_with_transitions',  # noqa: E501
         'kratos_identity_schemas': 'kratos_identity_schemas',  # noqa: E501
         'kratos_oauth2_provider_headers': 'kratos_oauth2_provider_headers',  # noqa: E501
         'kratos_oauth2_provider_override_return_to': 'kratos_oauth2_provider_override_return_to',  # noqa: E501
         'kratos_oauth2_provider_url': 'kratos_oauth2_provider_url',  # noqa: E501
         'kratos_preview_default_read_consistency_level': 'kratos_preview_default_read_consistency_level',  # noqa: E501
         'kratos_secrets_cipher': 'kratos_secrets_cipher',  # noqa: E501
@@ -681,14 +683,15 @@
             kratos_courier_templates_verification_invalid_email_body_html (str): Configures the Ory Kratos Invalid Verification Email Body HTML Template  This governs the \"courier.smtp.templates.verification.invalid.email.body.html\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_invalid_email_body_plaintext (str): Configures the Ory Kratos Invalid Verification Email Body Plaintext Template  This governs the \"courier.smtp.templates.verification.invalid.email.body.plaintext\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_invalid_email_subject (str): Configures the Ory Kratos Invalid Verification Email Subject Template  This governs the \"courier.smtp.templates.verification.invalid.email.subject\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_valid_email_body_html (str): Configures the Ory Kratos Valid Verification Email Body HTML Template  This governs the \"courier.smtp.templates.verification.valid.email.body.html\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_valid_email_body_plaintext (str): Configures the Ory Kratos Valid Verification Email Body Plaintext Template  This governs the \"courier.smtp.templates.verification.valid.email.body.plaintext\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_valid_email_subject (str): Configures the Ory Kratos Valid Verification Email Subject Template  This governs the \"courier.smtp.templates.verification.valid.email.subject\" setting.. [optional]  # noqa: E501
             kratos_feature_flags_cacheable_sessions (bool): Configures the Ory Kratos Session caching feature flag  This governs the \"feature_flags.cacheable_sessions\" setting.. [optional]  # noqa: E501
+            kratos_feature_flags_cacheable_sessions_max_age (str): Configures the Ory Kratos Session caching max-age feature flag  This governs the \"feature_flags.cacheable_sessions_max_age\" setting.. [optional]  # noqa: E501
             kratos_feature_flags_use_continue_with_transitions (bool): Configures the Ory Kratos Session use_continue_with_transitions flag  This governs the \"feature_flags.use_continue_with_transitions\" setting.. [optional]  # noqa: E501
             kratos_identity_schemas (ProjectRevisionIdentitySchemas): [optional]  # noqa: E501
             kratos_oauth2_provider_headers ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): NullJSONRawMessage represents a json.RawMessage that works well with JSON, SQL, and Swagger and is NULLable-. [optional]  # noqa: E501
             kratos_oauth2_provider_override_return_to (bool): Kratos OAuth2 Provider Override Return To  Enabling this allows Kratos to set the return_to parameter automatically to the OAuth2 request URL on the login flow, allowing complex flows such as recovery to continue to the initial OAuth2 flow.. [optional]  # noqa: E501
             kratos_oauth2_provider_url (str): The Revisions' OAuth2 Provider Integration URL  This governs the \"oauth2_provider.url\" setting.. [optional]  # noqa: E501
             kratos_preview_default_read_consistency_level (str): Configures the default read consistency level for identity APIs  This governs the `preview.default_read_consistency_level` setting.  The read consistency level determines the consistency guarantee for reads:  strong (slow): The read is guaranteed to return the most recent data committed at the start of the read. eventual (very fast): The result will return data that is about 4.8 seconds old.  Setting the default consistency level to `eventual` may cause regressions in the future as we add consistency controls to more APIs. Currently, the following APIs will be affected by this setting:  `GET /admin/identities`  Defaults to \"strong\" for new and existing projects. This feature is in preview. Use with caution.. [optional]  # noqa: E501
             kratos_secrets_cipher (StringSliceJSONFormat): [optional]  # noqa: E501
@@ -961,14 +964,15 @@
             kratos_courier_templates_verification_invalid_email_body_html (str): Configures the Ory Kratos Invalid Verification Email Body HTML Template  This governs the \"courier.smtp.templates.verification.invalid.email.body.html\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_invalid_email_body_plaintext (str): Configures the Ory Kratos Invalid Verification Email Body Plaintext Template  This governs the \"courier.smtp.templates.verification.invalid.email.body.plaintext\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_invalid_email_subject (str): Configures the Ory Kratos Invalid Verification Email Subject Template  This governs the \"courier.smtp.templates.verification.invalid.email.subject\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_valid_email_body_html (str): Configures the Ory Kratos Valid Verification Email Body HTML Template  This governs the \"courier.smtp.templates.verification.valid.email.body.html\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_valid_email_body_plaintext (str): Configures the Ory Kratos Valid Verification Email Body Plaintext Template  This governs the \"courier.smtp.templates.verification.valid.email.body.plaintext\" setting.. [optional]  # noqa: E501
             kratos_courier_templates_verification_valid_email_subject (str): Configures the Ory Kratos Valid Verification Email Subject Template  This governs the \"courier.smtp.templates.verification.valid.email.subject\" setting.. [optional]  # noqa: E501
             kratos_feature_flags_cacheable_sessions (bool): Configures the Ory Kratos Session caching feature flag  This governs the \"feature_flags.cacheable_sessions\" setting.. [optional]  # noqa: E501
+            kratos_feature_flags_cacheable_sessions_max_age (str): Configures the Ory Kratos Session caching max-age feature flag  This governs the \"feature_flags.cacheable_sessions_max_age\" setting.. [optional]  # noqa: E501
             kratos_feature_flags_use_continue_with_transitions (bool): Configures the Ory Kratos Session use_continue_with_transitions flag  This governs the \"feature_flags.use_continue_with_transitions\" setting.. [optional]  # noqa: E501
             kratos_identity_schemas (ProjectRevisionIdentitySchemas): [optional]  # noqa: E501
             kratos_oauth2_provider_headers ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): NullJSONRawMessage represents a json.RawMessage that works well with JSON, SQL, and Swagger and is NULLable-. [optional]  # noqa: E501
             kratos_oauth2_provider_override_return_to (bool): Kratos OAuth2 Provider Override Return To  Enabling this allows Kratos to set the return_to parameter automatically to the OAuth2 request URL on the login flow, allowing complex flows such as recovery to continue to the initial OAuth2 flow.. [optional]  # noqa: E501
             kratos_oauth2_provider_url (str): The Revisions' OAuth2 Provider Integration URL  This governs the \"oauth2_provider.url\" setting.. [optional]  # noqa: E501
             kratos_preview_default_read_consistency_level (str): Configures the default read consistency level for identity APIs  This governs the `preview.default_read_consistency_level` setting.  The read consistency level determines the consistency guarantee for reads:  strong (slow): The read is guaranteed to return the most recent data committed at the start of the read. eventual (very fast): The result will return data that is about 4.8 seconds old.  Setting the default consistency level to `eventual` may cause regressions in the future as we add consistency controls to more APIs. Currently, the following APIs will be affected by this setting:  `GET /admin/identities`  Defaults to \"strong\" for new and existing projects. This feature is in preview. Use with caution.. [optional]  # noqa: E501
             kratos_secrets_cipher (StringSliceJSONFormat): [optional]  # noqa: E501
```

### Comparing `ory-client-1.8.1/ory_client/model/normalized_project_revision_courier_channel.py` & `ory-client-1.9.0/ory_client/model/normalized_project_revision_courier_channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/normalized_project_revision_hook.py` & `ory-client-1.9.0/ory_client/model/normalized_project_revision_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/normalized_project_revision_identity_schema.py` & `ory-client-1.9.0/ory_client/model/normalized_project_revision_identity_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/normalized_project_revision_identity_schemas.py` & `ory-client-1.9.0/ory_client/model/normalized_project_revision_identity_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/normalized_project_revision_third_party_provider.py` & `ory-client-1.9.0/ory_client/model/normalized_project_revision_third_party_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/normalized_project_revision_tokenizer_template.py` & `ory-client-1.9.0/ory_client/model/normalized_project_revision_tokenizer_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/normalized_project_revision_tokenizer_templates.py` & `ory-client-1.9.0/ory_client/model/normalized_project_revision_tokenizer_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/normalized_projects.py` & `ory-client-1.9.0/ory_client/model/normalized_projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/null_duration.py` & `ory-client-1.9.0/ory_client/model/null_duration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/o_auth2_client.py` & `ory-client-1.9.0/ory_client/model/o_auth2_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/o_auth2_client_token_lifespans.py` & `ory-client-1.9.0/ory_client/model/o_auth2_client_token_lifespans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/o_auth2_consent_request.py` & `ory-client-1.9.0/ory_client/model/o_auth2_consent_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/o_auth2_consent_request_open_id_connect_context.py` & `ory-client-1.9.0/ory_client/model/o_auth2_consent_request_open_id_connect_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/o_auth2_consent_session.py` & `ory-client-1.9.0/ory_client/model/o_auth2_consent_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/o_auth2_consent_session_expires_at.py` & `ory-client-1.9.0/ory_client/model/o_auth2_consent_session_expires_at.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/o_auth2_consent_sessions.py` & `ory-client-1.9.0/ory_client/model/o_auth2_consent_sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/o_auth2_login_request.py` & `ory-client-1.9.0/ory_client/model/o_auth2_login_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/o_auth2_logout_request.py` & `ory-client-1.9.0/ory_client/model/o_auth2_logout_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/o_auth2_redirect_to.py` & `ory-client-1.9.0/ory_client/model/o_auth2_redirect_to.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/o_auth2_token_exchange.py` & `ory-client-1.9.0/ory_client/model/o_auth2_token_exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/oidc_configuration.py` & `ory-client-1.9.0/ory_client/model/oidc_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/oidc_user_info.py` & `ory-client-1.9.0/ory_client/model/oidc_user_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/organization.py` & `ory-client-1.9.0/ory_client/model/organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/organization_body.py` & `ory-client-1.9.0/ory_client/model/organization_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/pagination.py` & `ory-client-1.9.0/ory_client/model/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/pagination_headers.py` & `ory-client-1.9.0/ory_client/model/pagination_headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/parse_error.py` & `ory-client-1.9.0/ory_client/model/parse_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/patch_identities_body.py` & `ory-client-1.9.0/ory_client/model/patch_identities_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/perform_native_logout_body.py` & `ory-client-1.9.0/ory_client/model/perform_native_logout_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/permissions_on_project.py` & `ory-client-1.9.0/ory_client/model/permissions_on_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/permissions_on_workpace_response.py` & `ory-client-1.9.0/ory_client/model/permissions_on_workpace_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/plan.py` & `ory-client-1.9.0/ory_client/model/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/plan_details.py` & `ory-client-1.9.0/ory_client/model/plan_details.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -91,14 +91,15 @@
             'base_fee_monthly': (int,),  # noqa: E501
             'base_fee_yearly': (int,),  # noqa: E501
             'custom': (bool,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'features': (PlanFeatures,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'version': (int,),  # noqa: E501
+            'latest': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -106,14 +107,15 @@
         'base_fee_monthly': 'base_fee_monthly',  # noqa: E501
         'base_fee_yearly': 'base_fee_yearly',  # noqa: E501
         'custom': 'custom',  # noqa: E501
         'description': 'description',  # noqa: E501
         'features': 'features',  # noqa: E501
         'name': 'name',  # noqa: E501
         'version': 'version',  # noqa: E501
+        'latest': 'latest',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -158,14 +160,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            latest (bool): Latest is true if the plan is the latest version of a plan and should be available for self-service usage.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -259,14 +262,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            latest (bool): Latest is true if the plan is the latest version of a plan and should be available for self-service usage.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ory-client-1.8.1/ory_client/model/plan_features.py` & `ory-client-1.9.0/ory_client/model/plan_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/plans.py` & `ory-client-1.9.0/ory_client/model/plans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/post_check_permission_body.py` & `ory-client-1.9.0/ory_client/model/post_check_permission_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/post_check_permission_or_error_body.py` & `ory-client-1.9.0/ory_client/model/post_check_permission_or_error_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/pricing.py` & `ory-client-1.9.0/ory_client/model/pricing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project.py` & `ory-client-1.9.0/ory_client/model/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_api_key.py` & `ory-client-1.9.0/ory_client/model/project_api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_api_keys.py` & `ory-client-1.9.0/ory_client/model/project_api_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_branding.py` & `ory-client-1.9.0/ory_client/model/project_branding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_branding_colors.py` & `ory-client-1.9.0/ory_client/model/project_branding_colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_branding_theme.py` & `ory-client-1.9.0/ory_client/model/project_branding_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_branding_themes.py` & `ory-client-1.9.0/ory_client/model/project_branding_themes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_cors.py` & `ory-client-1.9.0/ory_client/model/project_cors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_events_datapoint.py` & `ory-client-1.9.0/ory_client/model/project_events_datapoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_host.py` & `ory-client-1.9.0/ory_client/model/project_host.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_member.py` & `ory-client-1.9.0/ory_client/model/project_member.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_members.py` & `ory-client-1.9.0/ory_client/model/project_members.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_metadata.py` & `ory-client-1.9.0/ory_client/model/project_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_metadata_list.py` & `ory-client-1.9.0/ory_client/model/project_metadata_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_revision_hooks.py` & `ory-client-1.9.0/ory_client/model/project_revision_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_revision_identity_schemas.py` & `ory-client-1.9.0/ory_client/model/project_revision_identity_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_revision_third_party_login_providers.py` & `ory-client-1.9.0/ory_client/model/project_revision_third_party_login_providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_revisions.py` & `ory-client-1.9.0/ory_client/model/project_revisions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_service_identity.py` & `ory-client-1.9.0/ory_client/model/project_service_identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_service_o_auth2.py` & `ory-client-1.9.0/ory_client/model/project_service_o_auth2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_service_permission.py` & `ory-client-1.9.0/ory_client/model/project_service_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/project_services.py` & `ory-client-1.9.0/ory_client/model/project_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/projects.py` & `ory-client-1.9.0/ory_client/model/projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/quota_usage.py` & `ory-client-1.9.0/ory_client/model/quota_usage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -58,28 +58,30 @@
     allowed_values = {
         ('feature',): {
             'REGION_EU': "region_eu",
             'REGION_US': "region_us",
             'REGION_APAC': "region_apac",
             'REGION_GLOBAL': "region_global",
             'PRODUCTION_PROJECTS': "production_projects",
+            'DEVELOPMENT_PROJECTS': "development_projects",
             'DAILY_ACTIVE_USERS': "daily_active_users",
             'CUSTOM_DOMAINS': "custom_domains",
             'EVENT_STREAMS': "event_streams",
             'SLA': "sla",
             'COLLABORATOR_SEATS': "collaborator_seats",
             'EDGE_CACHE': "edge_cache",
             'BRANDING_THEMES': "branding_themes",
             'ZENDESK_SUPPORT': "zendesk_support",
             'PROJECT_METRICS': "project_metrics",
             'PROJECT_METRICS_TIME_WINDOW': "project_metrics_time_window",
             'PROJECT_METRICS_EVENTS_HISTORY': "project_metrics_events_history",
             'ORGANIZATIONS': "organizations",
             'ROP_GRANT': "rop_grant",
             'CONCIERGE_ONBOARDING': "concierge_onboarding",
+            'CREDIT': "credit",
             'RATE_LIMIT_TIER': "rate_limit_tier",
             'SESSION_RATE_LIMIT_TIER': "session_rate_limit_tier",
             'IDENTITIES_LIST_RATE_LIMIT_TIER': "identities_list_rate_limit_tier",
             'PERMISSION_CHECKS_RATE_LIMIT_TIER': "permission_checks_rate_limit_tier",
             'OAUTH2_INTROSPECT_RATE_LIMIT_TIER': "oauth2_introspect_rate_limit_tier",
         },
     }
@@ -139,15 +141,15 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, additional_price, can_use_more, feature, feature_available, included, used, *args, **kwargs):  # noqa: E501
         """QuotaUsage - a model defined in OpenAPI
 
         Args:
             additional_price (int): The additional price per unit in cents.
             can_use_more (bool):
-            feature (str):  region_eu RegionEU region_us RegionUS region_apac RegionAPAC region_global RegionGlobal production_projects ProductionProjects daily_active_users DailyActiveUsers custom_domains CustomDomains event_streams EventStreams sla SLA collaborator_seats CollaboratorSeats edge_cache EdgeCache branding_themes BrandingThemes zendesk_support ZendeskSupport project_metrics ProjectMetrics project_metrics_time_window ProjectMetricsTimeWindow project_metrics_events_history ProjectMetricsEventsHistory organizations Organizations rop_grant ResourceOwnerPasswordGrant concierge_onboarding ConciergeOnboarding rate_limit_tier RateLimitTier session_rate_limit_tier RateLimitTierSessions identities_list_rate_limit_tier RateLimitTierIdentitiesList permission_checks_rate_limit_tier RateLimitTierPermissionChecks oauth2_introspect_rate_limit_tier RateLimitTierOAuth2Introspect
+            feature (str):  region_eu RegionEU region_us RegionUS region_apac RegionAPAC region_global RegionGlobal production_projects ProductionProjects development_projects DevelopmentProjects daily_active_users DailyActiveUsers custom_domains CustomDomains event_streams EventStreams sla SLA collaborator_seats CollaboratorSeats edge_cache EdgeCache branding_themes BrandingThemes zendesk_support ZendeskSupport project_metrics ProjectMetrics project_metrics_time_window ProjectMetricsTimeWindow project_metrics_events_history ProjectMetricsEventsHistory organizations Organizations rop_grant ResourceOwnerPasswordGrant concierge_onboarding ConciergeOnboarding credit Credit rate_limit_tier RateLimitTier session_rate_limit_tier RateLimitTierSessions identities_list_rate_limit_tier RateLimitTierIdentitiesList permission_checks_rate_limit_tier RateLimitTierPermissionChecks oauth2_introspect_rate_limit_tier RateLimitTierOAuth2Introspect
             feature_available (bool):
             included (int):
             used (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -238,15 +240,15 @@
     @convert_js_args_to_python_args
     def __init__(self, additional_price, can_use_more, feature, feature_available, included, used, *args, **kwargs):  # noqa: E501
         """QuotaUsage - a model defined in OpenAPI
 
         Args:
             additional_price (int): The additional price per unit in cents.
             can_use_more (bool):
-            feature (str):  region_eu RegionEU region_us RegionUS region_apac RegionAPAC region_global RegionGlobal production_projects ProductionProjects daily_active_users DailyActiveUsers custom_domains CustomDomains event_streams EventStreams sla SLA collaborator_seats CollaboratorSeats edge_cache EdgeCache branding_themes BrandingThemes zendesk_support ZendeskSupport project_metrics ProjectMetrics project_metrics_time_window ProjectMetricsTimeWindow project_metrics_events_history ProjectMetricsEventsHistory organizations Organizations rop_grant ResourceOwnerPasswordGrant concierge_onboarding ConciergeOnboarding rate_limit_tier RateLimitTier session_rate_limit_tier RateLimitTierSessions identities_list_rate_limit_tier RateLimitTierIdentitiesList permission_checks_rate_limit_tier RateLimitTierPermissionChecks oauth2_introspect_rate_limit_tier RateLimitTierOAuth2Introspect
+            feature (str):  region_eu RegionEU region_us RegionUS region_apac RegionAPAC region_global RegionGlobal production_projects ProductionProjects development_projects DevelopmentProjects daily_active_users DailyActiveUsers custom_domains CustomDomains event_streams EventStreams sla SLA collaborator_seats CollaboratorSeats edge_cache EdgeCache branding_themes BrandingThemes zendesk_support ZendeskSupport project_metrics ProjectMetrics project_metrics_time_window ProjectMetricsTimeWindow project_metrics_events_history ProjectMetricsEventsHistory organizations Organizations rop_grant ResourceOwnerPasswordGrant concierge_onboarding ConciergeOnboarding credit Credit rate_limit_tier RateLimitTier session_rate_limit_tier RateLimitTierSessions identities_list_rate_limit_tier RateLimitTierIdentitiesList permission_checks_rate_limit_tier RateLimitTierPermissionChecks oauth2_introspect_rate_limit_tier RateLimitTierOAuth2Introspect
             feature_available (bool):
             included (int):
             used (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
```

### Comparing `ory-client-1.8.1/ory_client/model/recovery_code_for_identity.py` & `ory-client-1.9.0/ory_client/model/recovery_code_for_identity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/recovery_flow.py` & `ory-client-1.9.0/ory_client/model/recovery_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/recovery_flow_state.py` & `ory-client-1.9.0/ory_client/model/recovery_flow_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/recovery_identity_address.py` & `ory-client-1.9.0/ory_client/model/recovery_identity_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/recovery_link_for_identity.py` & `ory-client-1.9.0/ory_client/model/recovery_link_for_identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/registration_flow.py` & `ory-client-1.9.0/ory_client/model/registration_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/registration_flow_state.py` & `ory-client-1.9.0/ory_client/model/registration_flow_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/reject_o_auth2_request.py` & `ory-client-1.9.0/ory_client/model/reject_o_auth2_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/relation_query.py` & `ory-client-1.9.0/ory_client/model/relation_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/relationship.py` & `ory-client-1.9.0/ory_client/model/relationship.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/relationship_namespaces.py` & `ory-client-1.9.0/ory_client/model/relationship_namespaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/relationship_patch.py` & `ory-client-1.9.0/ory_client/model/relationship_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/relationships.py` & `ory-client-1.9.0/ory_client/model/relationships.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/revision_courier_channels.py` & `ory-client-1.9.0/ory_client/model/revision_courier_channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/rfc6749_error_json.py` & `ory-client-1.9.0/ory_client/model/rfc6749_error_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/schema_patch.py` & `ory-client-1.9.0/ory_client/model/schema_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/self_service_flow_expired_error.py` & `ory-client-1.9.0/ory_client/model/self_service_flow_expired_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/session.py` & `ory-client-1.9.0/ory_client/model/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/session_activity_datapoint.py` & `ory-client-1.9.0/ory_client/model/session_activity_datapoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/session_authentication_method.py` & `ory-client-1.9.0/ory_client/model/session_authentication_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/session_authentication_methods.py` & `ory-client-1.9.0/ory_client/model/session_authentication_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/session_device.py` & `ory-client-1.9.0/ory_client/model/session_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/set_active_project_in_console_body.py` & `ory-client-1.9.0/ory_client/model/set_active_project_in_console_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/set_custom_domain_body.py` & `ory-client-1.9.0/ory_client/model/set_custom_domain_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/set_event_stream_body.py` & `ory-client-1.9.0/ory_client/model/set_event_stream_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/set_project.py` & `ory-client-1.9.0/ory_client/model/set_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/set_project_branding_theme_body.py` & `ory-client-1.9.0/ory_client/model/set_project_branding_theme_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/settings_flow.py` & `ory-client-1.9.0/ory_client/model/settings_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/settings_flow_state.py` & `ory-client-1.9.0/ory_client/model/settings_flow_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/source_position.py` & `ory-client-1.9.0/ory_client/model/source_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/string_slice_json_format.py` & `ory-client-1.9.0/ory_client/model/string_slice_json_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/subject_set.py` & `ory-client-1.9.0/ory_client/model/subject_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/subscription.py` & `ory-client-1.9.0/ory_client/model/subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/successful_code_exchange_response.py` & `ory-client-1.9.0/ory_client/model/successful_code_exchange_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/successful_native_login.py` & `ory-client-1.9.0/ory_client/model/successful_native_login.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/successful_native_registration.py` & `ory-client-1.9.0/ory_client/model/successful_native_registration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/successful_project_update.py` & `ory-client-1.9.0/ory_client/model/successful_project_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/token_pagination.py` & `ory-client-1.9.0/ory_client/model/token_pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/token_pagination_headers.py` & `ory-client-1.9.0/ory_client/model/token_pagination_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/token_pagination_request_parameters.py` & `ory-client-1.9.0/ory_client/model/token_pagination_request_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/token_pagination_response_headers.py` & `ory-client-1.9.0/ory_client/model/token_pagination_response_headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/trust_o_auth2_jwt_grant_issuer.py` & `ory-client-1.9.0/ory_client/model/trust_o_auth2_jwt_grant_issuer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/trusted_o_auth2_jwt_grant_issuer.py` & `ory-client-1.9.0/ory_client/model/trusted_o_auth2_jwt_grant_issuer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/trusted_o_auth2_jwt_grant_issuers.py` & `ory-client-1.9.0/ory_client/model/trusted_o_auth2_jwt_grant_issuers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/trusted_o_auth2_jwt_grant_json_web_key.py` & `ory-client-1.9.0/ory_client/model/trusted_o_auth2_jwt_grant_json_web_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/ui_container.py` & `ory-client-1.9.0/ory_client/model/ui_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/ui_node.py` & `ory-client-1.9.0/ory_client/model/ui_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/ui_node_anchor_attributes.py` & `ory-client-1.9.0/ory_client/model/ui_node_anchor_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/ui_node_attributes.py` & `ory-client-1.9.0/ory_client/model/ui_node_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/ui_node_image_attributes.py` & `ory-client-1.9.0/ory_client/model/ui_node_image_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/ui_node_input_attributes.py` & `ory-client-1.9.0/ory_client/model/ui_node_input_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/ui_node_meta.py` & `ory-client-1.9.0/ory_client/model/ui_node_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/ui_node_script_attributes.py` & `ory-client-1.9.0/ory_client/model/ui_node_script_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/ui_node_text_attributes.py` & `ory-client-1.9.0/ory_client/model/ui_node_text_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/ui_nodes.py` & `ory-client-1.9.0/ory_client/model/ui_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/ui_text.py` & `ory-client-1.9.0/ory_client/model/ui_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/ui_texts.py` & `ory-client-1.9.0/ory_client/model/ui_texts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_identity_body.py` & `ory-client-1.9.0/ory_client/model/update_identity_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_login_flow_body.py` & `ory-client-1.9.0/ory_client/model/update_login_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_login_flow_with_code_method.py` & `ory-client-1.9.0/ory_client/model/update_login_flow_with_code_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_login_flow_with_lookup_secret_method.py` & `ory-client-1.9.0/ory_client/model/update_login_flow_with_lookup_secret_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_login_flow_with_oidc_method.py` & `ory-client-1.9.0/ory_client/model/update_login_flow_with_oidc_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_login_flow_with_password_method.py` & `ory-client-1.9.0/ory_client/model/update_login_flow_with_password_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_login_flow_with_totp_method.py` & `ory-client-1.9.0/ory_client/model/update_login_flow_with_totp_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_login_flow_with_web_authn_method.py` & `ory-client-1.9.0/ory_client/model/update_login_flow_with_web_authn_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_recovery_flow_body.py` & `ory-client-1.9.0/ory_client/model/update_recovery_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_recovery_flow_with_code_method.py` & `ory-client-1.9.0/ory_client/model/update_recovery_flow_with_code_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_recovery_flow_with_link_method.py` & `ory-client-1.9.0/ory_client/model/update_recovery_flow_with_link_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_registration_flow_body.py` & `ory-client-1.9.0/ory_client/model/update_registration_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_registration_flow_with_code_method.py` & `ory-client-1.9.0/ory_client/model/update_registration_flow_with_code_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_registration_flow_with_oidc_method.py` & `ory-client-1.9.0/ory_client/model/update_registration_flow_with_oidc_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_registration_flow_with_password_method.py` & `ory-client-1.9.0/ory_client/model/update_registration_flow_with_password_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_registration_flow_with_web_authn_method.py` & `ory-client-1.9.0/ory_client/model/update_registration_flow_with_web_authn_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_settings_flow_body.py` & `ory-client-1.9.0/ory_client/model/update_settings_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_settings_flow_with_lookup_method.py` & `ory-client-1.9.0/ory_client/model/update_settings_flow_with_lookup_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_settings_flow_with_oidc_method.py` & `ory-client-1.9.0/ory_client/model/update_settings_flow_with_oidc_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_settings_flow_with_password_method.py` & `ory-client-1.9.0/ory_client/model/update_settings_flow_with_password_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_settings_flow_with_profile_method.py` & `ory-client-1.9.0/ory_client/model/update_settings_flow_with_profile_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_settings_flow_with_totp_method.py` & `ory-client-1.9.0/ory_client/model/update_settings_flow_with_totp_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_settings_flow_with_web_authn_method.py` & `ory-client-1.9.0/ory_client/model/update_settings_flow_with_web_authn_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_subscription_body.py` & `ory-client-1.9.0/ory_client/model/update_subscription_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_verification_flow_body.py` & `ory-client-1.9.0/ory_client/model/update_verification_flow_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_verification_flow_with_code_method.py` & `ory-client-1.9.0/ory_client/model/update_verification_flow_with_code_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_verification_flow_with_link_method.py` & `ory-client-1.9.0/ory_client/model/update_verification_flow_with_link_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/update_workspace_payload.py` & `ory-client-1.9.0/ory_client/model/update_workspace_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/usage.py` & `ory-client-1.9.0/ory_client/model/usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/verifiable_credential_priming_response.py` & `ory-client-1.9.0/ory_client/model/verifiable_credential_priming_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/verifiable_credential_proof.py` & `ory-client-1.9.0/ory_client/model/verifiable_credential_proof.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/verifiable_credential_response.py` & `ory-client-1.9.0/ory_client/model/verifiable_credential_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/verifiable_identity_address.py` & `ory-client-1.9.0/ory_client/model/verifiable_identity_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/verification_flow.py` & `ory-client-1.9.0/ory_client/model/verification_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/verification_flow_state.py` & `ory-client-1.9.0/ory_client/model/verification_flow_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/version.py` & `ory-client-1.9.0/ory_client/model/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/warning.py` & `ory-client-1.9.0/ory_client/model/warning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/workspace.py` & `ory-client-1.9.0/ory_client/model/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/workspace_meta.py` & `ory-client-1.9.0/ory_client/model/workspace_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model/workspaces.py` & `ory-client-1.9.0/ory_client/model/workspaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `ory-client-1.8.1/ory_client/model_utils.py` & `ory-client-1.9.0/ory_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

### Comparing `ory-client-1.8.1/ory_client/models/__init__.py` & `ory-client-1.9.0/ory_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ory-client-1.8.1/ory_client/rest.py` & `ory-client-1.9.0/ory_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

### Comparing `ory-client-1.8.1/ory_client.egg-info/SOURCES.txt` & `ory-client-1.9.0/ory_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ory-client-1.8.1/setup.py` & `ory-client-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "ory-client"
-VERSION = "v1.8.1"
+VERSION = "v1.9.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `ory-client-1.8.1/test/test_accept_o_auth2_consent_request.py` & `ory-client-1.9.0/test/test_accept_o_auth2_consent_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_accept_o_auth2_consent_request_session.py` & `ory-client-1.9.0/test/test_accept_o_auth2_consent_request_session.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_accept_o_auth2_login_request.py` & `ory-client-1.9.0/test/test_accept_o_auth2_login_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_active_project_in_console.py` & `ory-client-1.9.0/test/test_set_active_project_in_console_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.active_project_in_console import ActiveProjectInConsole
+from ory_client.model.set_active_project_in_console_body import SetActiveProjectInConsoleBody
 
 
-class TestActiveProjectInConsole(unittest.TestCase):
-    """ActiveProjectInConsole unit test stubs"""
+class TestSetActiveProjectInConsoleBody(unittest.TestCase):
+    """SetActiveProjectInConsoleBody unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testActiveProjectInConsole(self):
-        """Test ActiveProjectInConsole"""
+    def testSetActiveProjectInConsoleBody(self):
+        """Test SetActiveProjectInConsoleBody"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ActiveProjectInConsole()  # noqa: E501
+        # model = SetActiveProjectInConsoleBody()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_attribute.py` & `ory-client-1.9.0/test/test_error_o_auth2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.attribute import Attribute
+from ory_client.model.error_o_auth2 import ErrorOAuth2
 
 
-class TestAttribute(unittest.TestCase):
-    """Attribute unit test stubs"""
+class TestErrorOAuth2(unittest.TestCase):
+    """ErrorOAuth2 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAttribute(self):
-        """Test Attribute"""
+    def testErrorOAuth2(self):
+        """Test ErrorOAuth2"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Attribute()  # noqa: E501
+        # model = ErrorOAuth2()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_attribute_filter.py` & `ory-client-1.9.0/test/test_attribute_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_attributes_count_datapoint.py` & `ory-client-1.9.0/test/test_attributes_count_datapoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_authenticator_assurance_level.py` & `ory-client-1.9.0/test/test_authenticator_assurance_level.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_batch_patch_identities_response.py` & `ory-client-1.9.0/test/test_batch_patch_identities_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_check_opl_syntax_result.py` & `ory-client-1.9.0/test/test_check_opl_syntax_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_check_permission_result.py` & `ory-client-1.9.0/test/test_check_permission_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_cloud_account.py` & `ory-client-1.9.0/test/test_cloud_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_consistency_request_parameters.py` & `ory-client-1.9.0/test/test_consistency_request_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_continue_with.py` & `ory-client-1.9.0/test/test_continue_with.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_continue_with_recovery_ui.py` & `ory-client-1.9.0/test/test_continue_with_recovery_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_continue_with_recovery_ui_flow.py` & `ory-client-1.9.0/test/test_continue_with_recovery_ui_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_continue_with_set_ory_session_token.py` & `ory-client-1.9.0/test/test_continue_with_set_ory_session_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_continue_with_settings_ui.py` & `ory-client-1.9.0/test/test_continue_with_settings_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_continue_with_settings_ui_flow.py` & `ory-client-1.9.0/test/test_continue_with_settings_ui_flow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_continue_with_verification_ui.py` & `ory-client-1.9.0/test/test_continue_with_verification_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_continue_with_verification_ui_flow.py` & `ory-client-1.9.0/test/test_continue_with_verification_ui_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_courier_api.py` & `ory-client-1.9.0/test/test_courier_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_courier_message_status.py` & `ory-client-1.9.0/test/test_courier_message_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_courier_message_type.py` & `ory-client-1.9.0/test/test_courier_message_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_custom_domain_body.py` & `ory-client-1.9.0/test/test_create_custom_domain_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_event_stream_body.py` & `ory-client-1.9.0/test/test_create_event_stream_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_identity_body.py` & `ory-client-1.9.0/test/test_create_identity_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_invite_response.py` & `ory-client-1.9.0/test/test_create_invite_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_json_web_key_set.py` & `ory-client-1.9.0/test/test_create_json_web_key_set.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_member_invite_response.py` & `ory-client-1.9.0/test/test_create_member_invite_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_project_api_key_request.py` & `ory-client-1.9.0/test/test_create_project_api_key_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_project_body.py` & `ory-client-1.9.0/test/test_create_project_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_project_branding.py` & `ory-client-1.9.0/test/test_create_project_branding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_project_member_invite_body.py` & `ory-client-1.9.0/test/test_create_project_member_invite_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_project_normalized_payload.py` & `ory-client-1.9.0/test/test_create_project_normalized_payload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_recovery_code_for_identity_body.py` & `ory-client-1.9.0/test/test_create_recovery_code_for_identity_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_recovery_link_for_identity_body.py` & `ory-client-1.9.0/test/test_create_recovery_link_for_identity_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_relationship_body.py` & `ory-client-1.9.0/test/test_create_relationship_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_subscription_body.py` & `ory-client-1.9.0/test/test_create_subscription_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_subscription_common.py` & `ory-client-1.9.0/test/test_create_subscription_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_verifiable_credential_request_body.py` & `ory-client-1.9.0/test/test_create_verifiable_credential_request_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_workspace_member_invite_body.py` & `ory-client-1.9.0/test/test_create_workspace_member_invite_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_workspace_payload.py` & `ory-client-1.9.0/test/test_create_workspace_payload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_create_workspace_subscription_body.py` & `ory-client-1.9.0/test/test_create_workspace_subscription_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_credential_supported_draft00.py` & `ory-client-1.9.0/test/test_credential_supported_draft00.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_custom_domain.py` & `ory-client-1.9.0/test/test_custom_domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_delete_my_sessions_count.py` & `ory-client-1.9.0/test/test_delete_my_sessions_count.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_email_template_data.py` & `ory-client-1.9.0/test/test_email_template_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_email_template_data_body.py` & `ory-client-1.9.0/test/test_email_template_data_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_error_authenticator_assurance_level_not_satisfied.py` & `ory-client-1.9.0/test/test_error_authenticator_assurance_level_not_satisfied.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_error_browser_location_change_required.py` & `ory-client-1.9.0/test/test_error_browser_location_change_required.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_error_flow_replaced.py` & `ory-client-1.9.0/test/test_error_flow_replaced.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_error_generic.py` & `ory-client-1.9.0/test/test_error_generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_error_o_auth2.py` & `ory-client-1.9.0/test/test_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.error_o_auth2 import ErrorOAuth2
+from ory_client.model.version import Version
 
 
-class TestErrorOAuth2(unittest.TestCase):
-    """ErrorOAuth2 unit test stubs"""
+class TestVersion(unittest.TestCase):
+    """Version unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testErrorOAuth2(self):
-        """Test ErrorOAuth2"""
+    def testVersion(self):
+        """Test Version"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ErrorOAuth2()  # noqa: E501
+        # model = Version()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_event_stream.py` & `ory-client-1.9.0/test/test_event_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_events_api.py` & `ory-client-1.9.0/test/test_events_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_expanded_permission_tree.py` & `ory-client-1.9.0/test/test_expanded_permission_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_flow_error.py` & `ory-client-1.9.0/test/test_flow_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_frontend_api.py` & `ory-client-1.9.0/test/test_frontend_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_generic_error.py` & `ory-client-1.9.0/test/test_generic_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_generic_error_content.py` & `ory-client-1.9.0/test/test_generic_error_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_generic_usage.py` & `ory-client-1.9.0/test/test_usage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
 from ory_client.model.generic_usage import GenericUsage
+globals()['GenericUsage'] = GenericUsage
+from ory_client.model.usage import Usage
 
 
-class TestGenericUsage(unittest.TestCase):
-    """GenericUsage unit test stubs"""
+class TestUsage(unittest.TestCase):
+    """Usage unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testGenericUsage(self):
-        """Test GenericUsage"""
+    def testUsage(self):
+        """Test Usage"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = GenericUsage()  # noqa: E501
+        # model = Usage()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_get_attributes_count_response.py` & `ory-client-1.9.0/test/test_get_attributes_count_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_get_managed_identity_schema_location.py` & `ory-client-1.9.0/test/test_get_managed_identity_schema_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_get_metrics_event_attributes_response.py` & `ory-client-1.9.0/test/test_get_metrics_event_attributes_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_get_metrics_event_types_response.py` & `ory-client-1.9.0/test/test_get_metrics_event_types_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_get_organization_response.py` & `ory-client-1.9.0/test/test_get_organization_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_get_project_events_body.py` & `ory-client-1.9.0/test/test_get_project_events_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_get_project_events_response.py` & `ory-client-1.9.0/test/test_get_project_events_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_get_project_metrics_response.py` & `ory-client-1.9.0/test/test_get_project_metrics_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_get_session_activity_response.py` & `ory-client-1.9.0/test/test_get_session_activity_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_get_version200_response.py` & `ory-client-1.9.0/test/test_get_version200_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_health_not_ready_status.py` & `ory-client-1.9.0/test/test_health_not_ready_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_health_status.py` & `ory-client-1.9.0/test/test_health_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity.py` & `ory-client-1.9.0/test/test_identity.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_api.py` & `ory-client-1.9.0/test/test_identity_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_credentials.py` & `ory-client-1.9.0/test/test_identity_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_credentials_code.py` & `ory-client-1.9.0/test/test_identity_credentials_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_credentials_oidc.py` & `ory-client-1.9.0/test/test_identity_credentials_oidc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_credentials_oidc_provider.py` & `ory-client-1.9.0/test/test_identity_credentials_oidc_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_credentials_password.py` & `ory-client-1.9.0/test/test_identity_credentials_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_patch.py` & `ory-client-1.9.0/test/test_identity_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_patch_response.py` & `ory-client-1.9.0/test/test_identity_patch_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_schema_container.py` & `ory-client-1.9.0/test/test_identity_schema_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_schema_preset.py` & `ory-client-1.9.0/test/test_identity_schema_presets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
 from ory_client.model.identity_schema_preset import IdentitySchemaPreset
+globals()['IdentitySchemaPreset'] = IdentitySchemaPreset
+from ory_client.model.identity_schema_presets import IdentitySchemaPresets
 
 
-class TestIdentitySchemaPreset(unittest.TestCase):
-    """IdentitySchemaPreset unit test stubs"""
+class TestIdentitySchemaPresets(unittest.TestCase):
+    """IdentitySchemaPresets unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIdentitySchemaPreset(self):
-        """Test IdentitySchemaPreset"""
+    def testIdentitySchemaPresets(self):
+        """Test IdentitySchemaPresets"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IdentitySchemaPreset()  # noqa: E501
+        # model = IdentitySchemaPresets()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_identity_schema_presets.py` & `ory-client-1.9.0/test/test_identity_schemas.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.identity_schema_preset import IdentitySchemaPreset
-globals()['IdentitySchemaPreset'] = IdentitySchemaPreset
-from ory_client.model.identity_schema_presets import IdentitySchemaPresets
+from ory_client.model.identity_schema_container import IdentitySchemaContainer
+globals()['IdentitySchemaContainer'] = IdentitySchemaContainer
+from ory_client.model.identity_schemas import IdentitySchemas
 
 
-class TestIdentitySchemaPresets(unittest.TestCase):
-    """IdentitySchemaPresets unit test stubs"""
+class TestIdentitySchemas(unittest.TestCase):
+    """IdentitySchemas unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIdentitySchemaPresets(self):
-        """Test IdentitySchemaPresets"""
+    def testIdentitySchemas(self):
+        """Test IdentitySchemas"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IdentitySchemaPresets()  # noqa: E501
+        # model = IdentitySchemas()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_identity_schemas.py` & `ory-client-1.9.0/test/test_warning.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.identity_schema_container import IdentitySchemaContainer
-globals()['IdentitySchemaContainer'] = IdentitySchemaContainer
-from ory_client.model.identity_schemas import IdentitySchemas
+from ory_client.model.warning import Warning
 
 
-class TestIdentitySchemas(unittest.TestCase):
-    """IdentitySchemas unit test stubs"""
+class TestWarning(unittest.TestCase):
+    """Warning unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIdentitySchemas(self):
-        """Test IdentitySchemas"""
+    def testWarning(self):
+        """Test Warning"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IdentitySchemas()  # noqa: E501
+        # model = Warning()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_identity_with_credentials.py` & `ory-client-1.9.0/test/test_identity_with_credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_with_credentials_oidc.py` & `ory-client-1.9.0/test/test_identity_with_credentials_oidc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_with_credentials_oidc_config.py` & `ory-client-1.9.0/test/test_identity_with_credentials_oidc_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_with_credentials_oidc_config_provider.py` & `ory-client-1.9.0/test/test_identity_with_credentials_oidc_config_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_with_credentials_password.py` & `ory-client-1.9.0/test/test_identity_with_credentials_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_identity_with_credentials_password_config.py` & `ory-client-1.9.0/test/test_identity_with_credentials_password_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_internal_get_project_branding_body.py` & `ory-client-1.9.0/test/test_internal_get_project_branding_body.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_internal_is_ax_welcome_screen_enabled_for_project_body.py` & `ory-client-1.9.0/test/test_internal_is_ax_welcome_screen_enabled_for_project_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_internal_is_owner_for_project_by_slug_body.py` & `ory-client-1.9.0/test/test_internal_is_owner_for_project_by_slug_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_internal_is_owner_for_project_by_slug_response.py` & `ory-client-1.9.0/test/test_internal_is_owner_for_project_by_slug_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_introspected_o_auth2_token.py` & `ory-client-1.9.0/test/test_introspected_o_auth2_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_is_owner_for_project_by_slug.py` & `ory-client-1.9.0/test/test_is_owner_for_project_by_slug.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_is_ready200_response.py` & `ory-client-1.9.0/test/test_is_ready200_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_is_ready503_response.py` & `ory-client-1.9.0/test/test_is_ready503_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_json_patch.py` & `ory-client-1.9.0/test/test_json_patch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_json_patch_document.py` & `ory-client-1.9.0/test/test_json_patch_document.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_json_web_key.py` & `ory-client-1.9.0/test/test_json_web_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_json_web_key_set.py` & `ory-client-1.9.0/test/test_json_web_key_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_jwk_api.py` & `ory-client-1.9.0/test/test_jwk_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_keto_namespace.py` & `ory-client-1.9.0/test/test_keto_namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_keto_namespaces.py` & `ory-client-1.9.0/test/test_keto_namespaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_list_custom_domains.py` & `ory-client-1.9.0/test/test_list_custom_domains.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_list_event_streams.py` & `ory-client-1.9.0/test/test_list_event_streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_list_my_workspaces_response.py` & `ory-client-1.9.0/test/test_list_my_workspaces_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_list_organizations_response.py` & `ory-client-1.9.0/test/test_list_organizations_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_list_workspace_projects_response.py` & `ory-client-1.9.0/test/test_list_workspace_projects_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_login_flow.py` & `ory-client-1.9.0/test/test_login_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_login_flow_state.py` & `ory-client-1.9.0/test/test_login_flow_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_logout_flow.py` & `ory-client-1.9.0/test/test_logout_flow.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_managed_identity_schema.py` & `ory-client-1.9.0/test/test_managed_identity_schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_managed_identity_schema_validation_result.py` & `ory-client-1.9.0/test/test_managed_identity_schema_validation_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_managed_identity_schemas.py` & `ory-client-1.9.0/test/test_managed_identity_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_member_invite.py` & `ory-client-1.9.0/test/test_member_invite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_member_invites.py` & `ory-client-1.9.0/test/test_member_invites.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_message.py` & `ory-client-1.9.0/test/test_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_message_dispatch.py` & `ory-client-1.9.0/test/test_message_dispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_metadata_api.py` & `ory-client-1.9.0/test/test_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_metrics_datapoint.py` & `ory-client-1.9.0/test/test_metrics_datapoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_migration_options.py` & `ory-client-1.9.0/test/test_migration_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_namespace.py` & `ory-client-1.9.0/test/test_namespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_needs_privileged_session_error.py` & `ory-client-1.9.0/test/test_needs_privileged_session_error.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_normalized_project.py` & `ory-client-1.9.0/test/test_normalized_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_normalized_project_revision.py` & `ory-client-1.9.0/test/test_normalized_project_revision.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_normalized_project_revision_courier_channel.py` & `ory-client-1.9.0/test/test_normalized_project_revision_courier_channel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_normalized_project_revision_hook.py` & `ory-client-1.9.0/test/test_project_revisions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.normalized_project_revision_hook import NormalizedProjectRevisionHook
+from ory_client.model.normalized_project_revision import NormalizedProjectRevision
+globals()['NormalizedProjectRevision'] = NormalizedProjectRevision
+from ory_client.model.project_revisions import ProjectRevisions
 
 
-class TestNormalizedProjectRevisionHook(unittest.TestCase):
-    """NormalizedProjectRevisionHook unit test stubs"""
+class TestProjectRevisions(unittest.TestCase):
+    """ProjectRevisions unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testNormalizedProjectRevisionHook(self):
-        """Test NormalizedProjectRevisionHook"""
+    def testProjectRevisions(self):
+        """Test ProjectRevisions"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = NormalizedProjectRevisionHook()  # noqa: E501
+        # model = ProjectRevisions()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_normalized_project_revision_identity_schema.py` & `ory-client-1.9.0/test/test_normalized_project_revision_identity_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_normalized_project_revision_identity_schemas.py` & `ory-client-1.9.0/test/test_normalized_project_revision_identity_schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_normalized_project_revision_third_party_provider.py` & `ory-client-1.9.0/test/test_normalized_project_revision_third_party_provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_normalized_project_revision_tokenizer_template.py` & `ory-client-1.9.0/test/test_normalized_project_revision_tokenizer_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_normalized_project_revision_tokenizer_templates.py` & `ory-client-1.9.0/test/test_normalized_project_revision_tokenizer_templates.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_normalized_projects.py` & `ory-client-1.9.0/test/test_normalized_projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_null_duration.py` & `ory-client-1.9.0/test/test_null_duration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_o_auth2_api.py` & `ory-client-1.9.0/test/test_o_auth2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_o_auth2_client.py` & `ory-client-1.9.0/test/test_o_auth2_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_o_auth2_client_token_lifespans.py` & `ory-client-1.9.0/test/test_o_auth2_client_token_lifespans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_o_auth2_consent_request.py` & `ory-client-1.9.0/test/test_o_auth2_consent_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_o_auth2_consent_request_open_id_connect_context.py` & `ory-client-1.9.0/test/test_o_auth2_consent_request_open_id_connect_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_o_auth2_consent_session.py` & `ory-client-1.9.0/test/test_o_auth2_consent_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_o_auth2_consent_session_expires_at.py` & `ory-client-1.9.0/test/test_o_auth2_consent_session_expires_at.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_o_auth2_consent_sessions.py` & `ory-client-1.9.0/test/test_o_auth2_consent_sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_o_auth2_login_request.py` & `ory-client-1.9.0/test/test_o_auth2_login_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_o_auth2_logout_request.py` & `ory-client-1.9.0/test/test_o_auth2_logout_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_o_auth2_redirect_to.py` & `ory-client-1.9.0/test/test_o_auth2_redirect_to.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_o_auth2_token_exchange.py` & `ory-client-1.9.0/test/test_o_auth2_token_exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_oidc_api.py` & `ory-client-1.9.0/test/test_oidc_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_oidc_configuration.py` & `ory-client-1.9.0/test/test_oidc_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_oidc_user_info.py` & `ory-client-1.9.0/test/test_oidc_user_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_organization.py` & `ory-client-1.9.0/test/test_organization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_organization_body.py` & `ory-client-1.9.0/test/test_organization_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_pagination.py` & `ory-client-1.9.0/test/test_pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_pagination_headers.py` & `ory-client-1.9.0/test/test_token_pagination_headers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.pagination_headers import PaginationHeaders
+from ory_client.model.token_pagination_headers import TokenPaginationHeaders
 
 
-class TestPaginationHeaders(unittest.TestCase):
-    """PaginationHeaders unit test stubs"""
+class TestTokenPaginationHeaders(unittest.TestCase):
+    """TokenPaginationHeaders unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPaginationHeaders(self):
-        """Test PaginationHeaders"""
+    def testTokenPaginationHeaders(self):
+        """Test TokenPaginationHeaders"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PaginationHeaders()  # noqa: E501
+        # model = TokenPaginationHeaders()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_parse_error.py` & `ory-client-1.9.0/test/test_parse_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_patch_identities_body.py` & `ory-client-1.9.0/test/test_patch_identities_body.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_perform_native_logout_body.py` & `ory-client-1.9.0/test/test_perform_native_logout_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_permission_api.py` & `ory-client-1.9.0/test/test_permission_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_permissions_on_project.py` & `ory-client-1.9.0/test/test_permissions_on_project.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_permissions_on_workpace_response.py` & `ory-client-1.9.0/test/test_permissions_on_workpace_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_plan.py` & `ory-client-1.9.0/test/test_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_plan_details.py` & `ory-client-1.9.0/test/test_plan_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_plan_features.py` & `ory-client-1.9.0/test/test_ui_node_text_attributes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.generic_usage import GenericUsage
-globals()['GenericUsage'] = GenericUsage
-from ory_client.model.plan_features import PlanFeatures
+from ory_client.model.ui_text import UiText
+globals()['UiText'] = UiText
+from ory_client.model.ui_node_text_attributes import UiNodeTextAttributes
 
 
-class TestPlanFeatures(unittest.TestCase):
-    """PlanFeatures unit test stubs"""
+class TestUiNodeTextAttributes(unittest.TestCase):
+    """UiNodeTextAttributes unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPlanFeatures(self):
-        """Test PlanFeatures"""
+    def testUiNodeTextAttributes(self):
+        """Test UiNodeTextAttributes"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PlanFeatures()  # noqa: E501
+        # model = UiNodeTextAttributes()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_plans.py` & `ory-client-1.9.0/test/test_plans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_post_check_permission_body.py` & `ory-client-1.9.0/test/test_post_check_permission_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_post_check_permission_or_error_body.py` & `ory-client-1.9.0/test/test_post_check_permission_or_error_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_pricing.py` & `ory-client-1.9.0/test/test_pricing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project.py` & `ory-client-1.9.0/test/test_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_api.py` & `ory-client-1.9.0/test/test_project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_api_key.py` & `ory-client-1.9.0/test/test_project_api_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_api_keys.py` & `ory-client-1.9.0/test/test_projects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.project_api_key import ProjectApiKey
-globals()['ProjectApiKey'] = ProjectApiKey
-from ory_client.model.project_api_keys import ProjectApiKeys
+from ory_client.model.project import Project
+globals()['Project'] = Project
+from ory_client.model.projects import Projects
 
 
-class TestProjectApiKeys(unittest.TestCase):
-    """ProjectApiKeys unit test stubs"""
+class TestProjects(unittest.TestCase):
+    """Projects unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProjectApiKeys(self):
-        """Test ProjectApiKeys"""
+    def testProjects(self):
+        """Test Projects"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ProjectApiKeys()  # noqa: E501
+        # model = Projects()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_project_branding.py` & `ory-client-1.9.0/test/test_project_branding.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_branding_colors.py` & `ory-client-1.9.0/test/test_project_branding_colors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_branding_theme.py` & `ory-client-1.9.0/test/test_project_branding_theme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_branding_themes.py` & `ory-client-1.9.0/test/test_project_branding_themes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_cors.py` & `ory-client-1.9.0/test/test_project_cors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_events_datapoint.py` & `ory-client-1.9.0/test/test_project_events_datapoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_host.py` & `ory-client-1.9.0/test/test_session_device.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.project_host import ProjectHost
+from ory_client.model.session_device import SessionDevice
 
 
-class TestProjectHost(unittest.TestCase):
-    """ProjectHost unit test stubs"""
+class TestSessionDevice(unittest.TestCase):
+    """SessionDevice unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProjectHost(self):
-        """Test ProjectHost"""
+    def testSessionDevice(self):
+        """Test SessionDevice"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ProjectHost()  # noqa: E501
+        # model = SessionDevice()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_project_member.py` & `ory-client-1.9.0/test/test_project_members.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
 from ory_client.model.project_member import ProjectMember
+globals()['ProjectMember'] = ProjectMember
+from ory_client.model.project_members import ProjectMembers
 
 
-class TestProjectMember(unittest.TestCase):
-    """ProjectMember unit test stubs"""
+class TestProjectMembers(unittest.TestCase):
+    """ProjectMembers unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProjectMember(self):
-        """Test ProjectMember"""
+    def testProjectMembers(self):
+        """Test ProjectMembers"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ProjectMember()  # noqa: E501
+        # model = ProjectMembers()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_project_members.py` & `ory-client-1.9.0/test/test_project_service_identity.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.project_member import ProjectMember
-globals()['ProjectMember'] = ProjectMember
-from ory_client.model.project_members import ProjectMembers
+from ory_client.model.project_service_identity import ProjectServiceIdentity
 
 
-class TestProjectMembers(unittest.TestCase):
-    """ProjectMembers unit test stubs"""
+class TestProjectServiceIdentity(unittest.TestCase):
+    """ProjectServiceIdentity unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProjectMembers(self):
-        """Test ProjectMembers"""
+    def testProjectServiceIdentity(self):
+        """Test ProjectServiceIdentity"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ProjectMembers()  # noqa: E501
+        # model = ProjectServiceIdentity()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_project_metadata.py` & `ory-client-1.9.0/test/test_project_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_metadata_list.py` & `ory-client-1.9.0/test/test_project_metadata_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_revision_hooks.py` & `ory-client-1.9.0/test/test_project_revision_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_revision_identity_schemas.py` & `ory-client-1.9.0/test/test_project_revision_identity_schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_revision_third_party_login_providers.py` & `ory-client-1.9.0/test/test_project_revision_third_party_login_providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_revisions.py` & `ory-client-1.9.0/test/test_schema_patch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.normalized_project_revision import NormalizedProjectRevision
-globals()['NormalizedProjectRevision'] = NormalizedProjectRevision
-from ory_client.model.project_revisions import ProjectRevisions
+from ory_client.model.schema_patch import SchemaPatch
 
 
-class TestProjectRevisions(unittest.TestCase):
-    """ProjectRevisions unit test stubs"""
+class TestSchemaPatch(unittest.TestCase):
+    """SchemaPatch unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProjectRevisions(self):
-        """Test ProjectRevisions"""
+    def testSchemaPatch(self):
+        """Test SchemaPatch"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ProjectRevisions()  # noqa: E501
+        # model = SchemaPatch()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_project_service_identity.py` & `ory-client-1.9.0/test/test_project_service_o_auth2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.project_service_identity import ProjectServiceIdentity
+from ory_client.model.project_service_o_auth2 import ProjectServiceOAuth2
 
 
-class TestProjectServiceIdentity(unittest.TestCase):
-    """ProjectServiceIdentity unit test stubs"""
+class TestProjectServiceOAuth2(unittest.TestCase):
+    """ProjectServiceOAuth2 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProjectServiceIdentity(self):
-        """Test ProjectServiceIdentity"""
+    def testProjectServiceOAuth2(self):
+        """Test ProjectServiceOAuth2"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ProjectServiceIdentity()  # noqa: E501
+        # model = ProjectServiceOAuth2()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_project_service_o_auth2.py` & `ory-client-1.9.0/test/test_project_api_keys.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.project_service_o_auth2 import ProjectServiceOAuth2
+from ory_client.model.project_api_key import ProjectApiKey
+globals()['ProjectApiKey'] = ProjectApiKey
+from ory_client.model.project_api_keys import ProjectApiKeys
 
 
-class TestProjectServiceOAuth2(unittest.TestCase):
-    """ProjectServiceOAuth2 unit test stubs"""
+class TestProjectApiKeys(unittest.TestCase):
+    """ProjectApiKeys unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProjectServiceOAuth2(self):
-        """Test ProjectServiceOAuth2"""
+    def testProjectApiKeys(self):
+        """Test ProjectApiKeys"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ProjectServiceOAuth2()  # noqa: E501
+        # model = ProjectApiKeys()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_project_service_permission.py` & `ory-client-1.9.0/test/test_project_service_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_project_services.py` & `ory-client-1.9.0/test/test_project_services.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_projects.py` & `ory-client-1.9.0/test/test_reject_o_auth2_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.project import Project
-globals()['Project'] = Project
-from ory_client.model.projects import Projects
+from ory_client.model.reject_o_auth2_request import RejectOAuth2Request
 
 
-class TestProjects(unittest.TestCase):
-    """Projects unit test stubs"""
+class TestRejectOAuth2Request(unittest.TestCase):
+    """RejectOAuth2Request unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProjects(self):
-        """Test Projects"""
+    def testRejectOAuth2Request(self):
+        """Test RejectOAuth2Request"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Projects()  # noqa: E501
+        # model = RejectOAuth2Request()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_quota_usage.py` & `ory-client-1.9.0/test/test_quota_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_recovery_code_for_identity.py` & `ory-client-1.9.0/test/test_recovery_code_for_identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_recovery_flow.py` & `ory-client-1.9.0/test/test_recovery_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_recovery_flow_state.py` & `ory-client-1.9.0/test/test_recovery_flow_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_recovery_identity_address.py` & `ory-client-1.9.0/test/test_recovery_identity_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_recovery_link_for_identity.py` & `ory-client-1.9.0/test/test_recovery_link_for_identity.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_registration_flow.py` & `ory-client-1.9.0/test/test_registration_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_registration_flow_state.py` & `ory-client-1.9.0/test/test_registration_flow_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_reject_o_auth2_request.py` & `ory-client-1.9.0/test/test_active_project_in_console.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.reject_o_auth2_request import RejectOAuth2Request
+from ory_client.model.active_project_in_console import ActiveProjectInConsole
 
 
-class TestRejectOAuth2Request(unittest.TestCase):
-    """RejectOAuth2Request unit test stubs"""
+class TestActiveProjectInConsole(unittest.TestCase):
+    """ActiveProjectInConsole unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRejectOAuth2Request(self):
-        """Test RejectOAuth2Request"""
+    def testActiveProjectInConsole(self):
+        """Test ActiveProjectInConsole"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = RejectOAuth2Request()  # noqa: E501
+        # model = ActiveProjectInConsole()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_relation_query.py` & `ory-client-1.9.0/test/test_relationships.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.subject_set import SubjectSet
-globals()['SubjectSet'] = SubjectSet
-from ory_client.model.relation_query import RelationQuery
+from ory_client.model.relationship import Relationship
+globals()['Relationship'] = Relationship
+from ory_client.model.relationships import Relationships
 
 
-class TestRelationQuery(unittest.TestCase):
-    """RelationQuery unit test stubs"""
+class TestRelationships(unittest.TestCase):
+    """Relationships unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRelationQuery(self):
-        """Test RelationQuery"""
+    def testRelationships(self):
+        """Test Relationships"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = RelationQuery()  # noqa: E501
+        # model = Relationships()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_relationship.py` & `ory-client-1.9.0/test/test_relationship.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_relationship_api.py` & `ory-client-1.9.0/test/test_relationship_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_relationship_namespaces.py` & `ory-client-1.9.0/test/test_relationship_namespaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_relationship_patch.py` & `ory-client-1.9.0/test/test_relationship_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_relationships.py` & `ory-client-1.9.0/test/test_ui_node_anchor_attributes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.relationship import Relationship
-globals()['Relationship'] = Relationship
-from ory_client.model.relationships import Relationships
+from ory_client.model.ui_text import UiText
+globals()['UiText'] = UiText
+from ory_client.model.ui_node_anchor_attributes import UiNodeAnchorAttributes
 
 
-class TestRelationships(unittest.TestCase):
-    """Relationships unit test stubs"""
+class TestUiNodeAnchorAttributes(unittest.TestCase):
+    """UiNodeAnchorAttributes unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRelationships(self):
-        """Test Relationships"""
+    def testUiNodeAnchorAttributes(self):
+        """Test UiNodeAnchorAttributes"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Relationships()  # noqa: E501
+        # model = UiNodeAnchorAttributes()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_revision_courier_channels.py` & `ory-client-1.9.0/test/test_revision_courier_channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_rfc6749_error_json.py` & `ory-client-1.9.0/test/test_rfc6749_error_json.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_schema_patch.py` & `ory-client-1.9.0/test/test_identity_schema_preset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.schema_patch import SchemaPatch
+from ory_client.model.identity_schema_preset import IdentitySchemaPreset
 
 
-class TestSchemaPatch(unittest.TestCase):
-    """SchemaPatch unit test stubs"""
+class TestIdentitySchemaPreset(unittest.TestCase):
+    """IdentitySchemaPreset unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSchemaPatch(self):
-        """Test SchemaPatch"""
+    def testIdentitySchemaPreset(self):
+        """Test IdentitySchemaPreset"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SchemaPatch()  # noqa: E501
+        # model = IdentitySchemaPreset()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_self_service_flow_expired_error.py` & `ory-client-1.9.0/test/test_self_service_flow_expired_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_session.py` & `ory-client-1.9.0/test/test_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_session_activity_datapoint.py` & `ory-client-1.9.0/test/test_session_activity_datapoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_session_authentication_method.py` & `ory-client-1.9.0/test/test_session_authentication_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_session_authentication_methods.py` & `ory-client-1.9.0/test/test_session_authentication_methods.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_session_device.py` & `ory-client-1.9.0/test/test_workspace.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.session_device import SessionDevice
+from ory_client.model.workspace import Workspace
 
 
-class TestSessionDevice(unittest.TestCase):
-    """SessionDevice unit test stubs"""
+class TestWorkspace(unittest.TestCase):
+    """Workspace unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSessionDevice(self):
-        """Test SessionDevice"""
+    def testWorkspace(self):
+        """Test Workspace"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SessionDevice()  # noqa: E501
+        # model = Workspace()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_set_active_project_in_console_body.py` & `ory-client-1.9.0/test/test_ui_container.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.set_active_project_in_console_body import SetActiveProjectInConsoleBody
+from ory_client.model.ui_nodes import UiNodes
+from ory_client.model.ui_texts import UiTexts
+globals()['UiNodes'] = UiNodes
+globals()['UiTexts'] = UiTexts
+from ory_client.model.ui_container import UiContainer
 
 
-class TestSetActiveProjectInConsoleBody(unittest.TestCase):
-    """SetActiveProjectInConsoleBody unit test stubs"""
+class TestUiContainer(unittest.TestCase):
+    """UiContainer unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSetActiveProjectInConsoleBody(self):
-        """Test SetActiveProjectInConsoleBody"""
+    def testUiContainer(self):
+        """Test UiContainer"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SetActiveProjectInConsoleBody()  # noqa: E501
+        # model = UiContainer()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_set_custom_domain_body.py` & `ory-client-1.9.0/test/test_set_custom_domain_body.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_set_event_stream_body.py` & `ory-client-1.9.0/test/test_set_event_stream_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_set_project.py` & `ory-client-1.9.0/test/test_set_project.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_set_project_branding_theme_body.py` & `ory-client-1.9.0/test/test_set_project_branding_theme_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_settings_flow.py` & `ory-client-1.9.0/test/test_settings_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_settings_flow_state.py` & `ory-client-1.9.0/test/test_settings_flow_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_source_position.py` & `ory-client-1.9.0/test/test_source_position.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_string_slice_json_format.py` & `ory-client-1.9.0/test/test_string_slice_json_format.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_subject_set.py` & `ory-client-1.9.0/test/test_subject_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_subscription.py` & `ory-client-1.9.0/test/test_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_successful_code_exchange_response.py` & `ory-client-1.9.0/test/test_successful_code_exchange_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_successful_native_login.py` & `ory-client-1.9.0/test/test_successful_native_login.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_successful_native_registration.py` & `ory-client-1.9.0/test/test_successful_native_registration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_successful_project_update.py` & `ory-client-1.9.0/test/test_successful_project_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_token_pagination.py` & `ory-client-1.9.0/test/test_token_pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_token_pagination_headers.py` & `ory-client-1.9.0/test/test_token_pagination_response_headers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.token_pagination_headers import TokenPaginationHeaders
+from ory_client.model.token_pagination_response_headers import TokenPaginationResponseHeaders
 
 
-class TestTokenPaginationHeaders(unittest.TestCase):
-    """TokenPaginationHeaders unit test stubs"""
+class TestTokenPaginationResponseHeaders(unittest.TestCase):
+    """TokenPaginationResponseHeaders unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTokenPaginationHeaders(self):
-        """Test TokenPaginationHeaders"""
+    def testTokenPaginationResponseHeaders(self):
+        """Test TokenPaginationResponseHeaders"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TokenPaginationHeaders()  # noqa: E501
+        # model = TokenPaginationResponseHeaders()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_token_pagination_request_parameters.py` & `ory-client-1.9.0/test/test_token_pagination_request_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_token_pagination_response_headers.py` & `ory-client-1.9.0/test/test_project_host.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.token_pagination_response_headers import TokenPaginationResponseHeaders
+from ory_client.model.project_host import ProjectHost
 
 
-class TestTokenPaginationResponseHeaders(unittest.TestCase):
-    """TokenPaginationResponseHeaders unit test stubs"""
+class TestProjectHost(unittest.TestCase):
+    """ProjectHost unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTokenPaginationResponseHeaders(self):
-        """Test TokenPaginationResponseHeaders"""
+    def testProjectHost(self):
+        """Test ProjectHost"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TokenPaginationResponseHeaders()  # noqa: E501
+        # model = ProjectHost()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_trust_o_auth2_jwt_grant_issuer.py` & `ory-client-1.9.0/test/test_trust_o_auth2_jwt_grant_issuer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_trusted_o_auth2_jwt_grant_issuer.py` & `ory-client-1.9.0/test/test_trusted_o_auth2_jwt_grant_issuer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_trusted_o_auth2_jwt_grant_issuers.py` & `ory-client-1.9.0/test/test_trusted_o_auth2_jwt_grant_issuers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_trusted_o_auth2_jwt_grant_json_web_key.py` & `ory-client-1.9.0/test/test_trusted_o_auth2_jwt_grant_json_web_key.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_ui_container.py` & `ory-client-1.9.0/test/test_ui_node.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.ui_nodes import UiNodes
+from ory_client.model.ui_node_attributes import UiNodeAttributes
+from ory_client.model.ui_node_meta import UiNodeMeta
 from ory_client.model.ui_texts import UiTexts
-globals()['UiNodes'] = UiNodes
+globals()['UiNodeAttributes'] = UiNodeAttributes
+globals()['UiNodeMeta'] = UiNodeMeta
 globals()['UiTexts'] = UiTexts
-from ory_client.model.ui_container import UiContainer
+from ory_client.model.ui_node import UiNode
 
 
-class TestUiContainer(unittest.TestCase):
-    """UiContainer unit test stubs"""
+class TestUiNode(unittest.TestCase):
+    """UiNode unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUiContainer(self):
-        """Test UiContainer"""
+    def testUiNode(self):
+        """Test UiNode"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UiContainer()  # noqa: E501
+        # model = UiNode()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_ui_node.py` & `ory-client-1.9.0/test/test_ui_node_meta.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.ui_node_attributes import UiNodeAttributes
+from ory_client.model.ui_text import UiText
+globals()['UiText'] = UiText
 from ory_client.model.ui_node_meta import UiNodeMeta
-from ory_client.model.ui_texts import UiTexts
-globals()['UiNodeAttributes'] = UiNodeAttributes
-globals()['UiNodeMeta'] = UiNodeMeta
-globals()['UiTexts'] = UiTexts
-from ory_client.model.ui_node import UiNode
 
 
-class TestUiNode(unittest.TestCase):
-    """UiNode unit test stubs"""
+class TestUiNodeMeta(unittest.TestCase):
+    """UiNodeMeta unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUiNode(self):
-        """Test UiNode"""
+    def testUiNodeMeta(self):
+        """Test UiNodeMeta"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UiNode()  # noqa: E501
+        # model = UiNodeMeta()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_ui_node_anchor_attributes.py` & `ory-client-1.9.0/test/test_ui_node_input_attributes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
 from ory_client.model.ui_text import UiText
 globals()['UiText'] = UiText
-from ory_client.model.ui_node_anchor_attributes import UiNodeAnchorAttributes
+from ory_client.model.ui_node_input_attributes import UiNodeInputAttributes
 
 
-class TestUiNodeAnchorAttributes(unittest.TestCase):
-    """UiNodeAnchorAttributes unit test stubs"""
+class TestUiNodeInputAttributes(unittest.TestCase):
+    """UiNodeInputAttributes unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUiNodeAnchorAttributes(self):
-        """Test UiNodeAnchorAttributes"""
+    def testUiNodeInputAttributes(self):
+        """Test UiNodeInputAttributes"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UiNodeAnchorAttributes()  # noqa: E501
+        # model = UiNodeInputAttributes()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_ui_node_attributes.py` & `ory-client-1.9.0/test/test_ui_node_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_ui_node_image_attributes.py` & `ory-client-1.9.0/test/test_ui_node_script_attributes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.ui_node_image_attributes import UiNodeImageAttributes
+from ory_client.model.ui_node_script_attributes import UiNodeScriptAttributes
 
 
-class TestUiNodeImageAttributes(unittest.TestCase):
-    """UiNodeImageAttributes unit test stubs"""
+class TestUiNodeScriptAttributes(unittest.TestCase):
+    """UiNodeScriptAttributes unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUiNodeImageAttributes(self):
-        """Test UiNodeImageAttributes"""
+    def testUiNodeScriptAttributes(self):
+        """Test UiNodeScriptAttributes"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UiNodeImageAttributes()  # noqa: E501
+        # model = UiNodeScriptAttributes()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_ui_node_input_attributes.py` & `ory-client-1.9.0/test/test_attribute.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.ui_text import UiText
-globals()['UiText'] = UiText
-from ory_client.model.ui_node_input_attributes import UiNodeInputAttributes
+from ory_client.model.attribute import Attribute
 
 
-class TestUiNodeInputAttributes(unittest.TestCase):
-    """UiNodeInputAttributes unit test stubs"""
+class TestAttribute(unittest.TestCase):
+    """Attribute unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUiNodeInputAttributes(self):
-        """Test UiNodeInputAttributes"""
+    def testAttribute(self):
+        """Test Attribute"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UiNodeInputAttributes()  # noqa: E501
+        # model = Attribute()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_ui_node_meta.py` & `ory-client-1.9.0/test/test_ui_nodes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.ui_text import UiText
-globals()['UiText'] = UiText
-from ory_client.model.ui_node_meta import UiNodeMeta
+from ory_client.model.ui_node import UiNode
+globals()['UiNode'] = UiNode
+from ory_client.model.ui_nodes import UiNodes
 
 
-class TestUiNodeMeta(unittest.TestCase):
-    """UiNodeMeta unit test stubs"""
+class TestUiNodes(unittest.TestCase):
+    """UiNodes unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUiNodeMeta(self):
-        """Test UiNodeMeta"""
+    def testUiNodes(self):
+        """Test UiNodes"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UiNodeMeta()  # noqa: E501
+        # model = UiNodes()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_ui_node_script_attributes.py` & `ory-client-1.9.0/test/test_workspaces.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.ui_node_script_attributes import UiNodeScriptAttributes
+from ory_client.model.workspace import Workspace
+globals()['Workspace'] = Workspace
+from ory_client.model.workspaces import Workspaces
 
 
-class TestUiNodeScriptAttributes(unittest.TestCase):
-    """UiNodeScriptAttributes unit test stubs"""
+class TestWorkspaces(unittest.TestCase):
+    """Workspaces unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUiNodeScriptAttributes(self):
-        """Test UiNodeScriptAttributes"""
+    def testWorkspaces(self):
+        """Test Workspaces"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UiNodeScriptAttributes()  # noqa: E501
+        # model = Workspaces()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_ui_node_text_attributes.py` & `ory-client-1.9.0/test/test_update_workspace_payload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.ui_text import UiText
-globals()['UiText'] = UiText
-from ory_client.model.ui_node_text_attributes import UiNodeTextAttributes
+from ory_client.model.update_workspace_payload import UpdateWorkspacePayload
 
 
-class TestUiNodeTextAttributes(unittest.TestCase):
-    """UiNodeTextAttributes unit test stubs"""
+class TestUpdateWorkspacePayload(unittest.TestCase):
+    """UpdateWorkspacePayload unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUiNodeTextAttributes(self):
-        """Test UiNodeTextAttributes"""
+    def testUpdateWorkspacePayload(self):
+        """Test UpdateWorkspacePayload"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UiNodeTextAttributes()  # noqa: E501
+        # model = UpdateWorkspacePayload()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_ui_nodes.py` & `ory-client-1.9.0/test/test_wellknown_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
-import sys
 import unittest
 
 import ory_client
-from ory_client.model.ui_node import UiNode
-globals()['UiNode'] = UiNode
-from ory_client.model.ui_nodes import UiNodes
+from ory_client.api.wellknown_api import WellknownApi  # noqa: E501
 
 
-class TestUiNodes(unittest.TestCase):
-    """UiNodes unit test stubs"""
+class TestWellknownApi(unittest.TestCase):
+    """WellknownApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = WellknownApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testUiNodes(self):
-        """Test UiNodes"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = UiNodes()  # noqa: E501
+    def test_discover_json_web_keys(self):
+        """Test case for discover_json_web_keys
+
+        Discover Well-Known JSON Web Keys  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_ui_text.py` & `ory-client-1.9.0/test/test_ui_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_ui_texts.py` & `ory-client-1.9.0/test/test_ui_texts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_identity_body.py` & `ory-client-1.9.0/test/test_update_identity_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_login_flow_body.py` & `ory-client-1.9.0/test/test_update_login_flow_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_login_flow_with_code_method.py` & `ory-client-1.9.0/test/test_update_login_flow_with_code_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_login_flow_with_lookup_secret_method.py` & `ory-client-1.9.0/test/test_update_login_flow_with_lookup_secret_method.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_login_flow_with_oidc_method.py` & `ory-client-1.9.0/test/test_update_login_flow_with_oidc_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_login_flow_with_password_method.py` & `ory-client-1.9.0/test/test_update_login_flow_with_password_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_login_flow_with_totp_method.py` & `ory-client-1.9.0/test/test_update_login_flow_with_totp_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_login_flow_with_web_authn_method.py` & `ory-client-1.9.0/test/test_update_settings_flow_with_web_authn_method.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.update_login_flow_with_web_authn_method import UpdateLoginFlowWithWebAuthnMethod
+from ory_client.model.update_settings_flow_with_web_authn_method import UpdateSettingsFlowWithWebAuthnMethod
 
 
-class TestUpdateLoginFlowWithWebAuthnMethod(unittest.TestCase):
-    """UpdateLoginFlowWithWebAuthnMethod unit test stubs"""
+class TestUpdateSettingsFlowWithWebAuthnMethod(unittest.TestCase):
+    """UpdateSettingsFlowWithWebAuthnMethod unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUpdateLoginFlowWithWebAuthnMethod(self):
-        """Test UpdateLoginFlowWithWebAuthnMethod"""
+    def testUpdateSettingsFlowWithWebAuthnMethod(self):
+        """Test UpdateSettingsFlowWithWebAuthnMethod"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UpdateLoginFlowWithWebAuthnMethod()  # noqa: E501
+        # model = UpdateSettingsFlowWithWebAuthnMethod()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_update_recovery_flow_body.py` & `ory-client-1.9.0/test/test_update_recovery_flow_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_recovery_flow_with_code_method.py` & `ory-client-1.9.0/test/test_update_recovery_flow_with_code_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_recovery_flow_with_link_method.py` & `ory-client-1.9.0/test/test_update_recovery_flow_with_link_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_registration_flow_body.py` & `ory-client-1.9.0/test/test_update_registration_flow_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_registration_flow_with_code_method.py` & `ory-client-1.9.0/test/test_update_registration_flow_with_code_method.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_registration_flow_with_oidc_method.py` & `ory-client-1.9.0/test/test_update_registration_flow_with_oidc_method.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_registration_flow_with_password_method.py` & `ory-client-1.9.0/test/test_update_registration_flow_with_password_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_registration_flow_with_web_authn_method.py` & `ory-client-1.9.0/test/test_update_registration_flow_with_web_authn_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_settings_flow_body.py` & `ory-client-1.9.0/test/test_update_settings_flow_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_settings_flow_with_lookup_method.py` & `ory-client-1.9.0/test/test_update_settings_flow_with_lookup_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_settings_flow_with_oidc_method.py` & `ory-client-1.9.0/test/test_update_settings_flow_with_oidc_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_settings_flow_with_password_method.py` & `ory-client-1.9.0/test/test_update_settings_flow_with_password_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_settings_flow_with_profile_method.py` & `ory-client-1.9.0/test/test_update_settings_flow_with_profile_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_settings_flow_with_totp_method.py` & `ory-client-1.9.0/test/test_update_settings_flow_with_totp_method.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_settings_flow_with_web_authn_method.py` & `ory-client-1.9.0/test/test_update_login_flow_with_web_authn_method.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.update_settings_flow_with_web_authn_method import UpdateSettingsFlowWithWebAuthnMethod
+from ory_client.model.update_login_flow_with_web_authn_method import UpdateLoginFlowWithWebAuthnMethod
 
 
-class TestUpdateSettingsFlowWithWebAuthnMethod(unittest.TestCase):
-    """UpdateSettingsFlowWithWebAuthnMethod unit test stubs"""
+class TestUpdateLoginFlowWithWebAuthnMethod(unittest.TestCase):
+    """UpdateLoginFlowWithWebAuthnMethod unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUpdateSettingsFlowWithWebAuthnMethod(self):
-        """Test UpdateSettingsFlowWithWebAuthnMethod"""
+    def testUpdateLoginFlowWithWebAuthnMethod(self):
+        """Test UpdateLoginFlowWithWebAuthnMethod"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UpdateSettingsFlowWithWebAuthnMethod()  # noqa: E501
+        # model = UpdateLoginFlowWithWebAuthnMethod()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_update_subscription_body.py` & `ory-client-1.9.0/test/test_update_subscription_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_verification_flow_body.py` & `ory-client-1.9.0/test/test_update_verification_flow_body.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_verification_flow_with_code_method.py` & `ory-client-1.9.0/test/test_update_verification_flow_with_code_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_verification_flow_with_link_method.py` & `ory-client-1.9.0/test/test_update_verification_flow_with_link_method.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_update_workspace_payload.py` & `ory-client-1.9.0/test/test_generic_usage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.update_workspace_payload import UpdateWorkspacePayload
+from ory_client.model.generic_usage import GenericUsage
 
 
-class TestUpdateWorkspacePayload(unittest.TestCase):
-    """UpdateWorkspacePayload unit test stubs"""
+class TestGenericUsage(unittest.TestCase):
+    """GenericUsage unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUpdateWorkspacePayload(self):
-        """Test UpdateWorkspacePayload"""
+    def testGenericUsage(self):
+        """Test GenericUsage"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UpdateWorkspacePayload()  # noqa: E501
+        # model = GenericUsage()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_usage.py` & `ory-client-1.9.0/test/test_pagination_headers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.generic_usage import GenericUsage
-globals()['GenericUsage'] = GenericUsage
-from ory_client.model.usage import Usage
+from ory_client.model.pagination_headers import PaginationHeaders
 
 
-class TestUsage(unittest.TestCase):
-    """Usage unit test stubs"""
+class TestPaginationHeaders(unittest.TestCase):
+    """PaginationHeaders unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUsage(self):
-        """Test Usage"""
+    def testPaginationHeaders(self):
+        """Test PaginationHeaders"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Usage()  # noqa: E501
+        # model = PaginationHeaders()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_verifiable_credential_priming_response.py` & `ory-client-1.9.0/test/test_verifiable_credential_priming_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_verifiable_credential_proof.py` & `ory-client-1.9.0/test/test_verifiable_credential_proof.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_verifiable_credential_response.py` & `ory-client-1.9.0/test/test_verifiable_credential_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_verifiable_identity_address.py` & `ory-client-1.9.0/test/test_verifiable_identity_address.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_verification_flow.py` & `ory-client-1.9.0/test/test_verification_flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_verification_flow_state.py` & `ory-client-1.9.0/test/test_verification_flow_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `ory-client-1.8.1/test/test_version.py` & `ory-client-1.9.0/test/test_workspace_meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.version import Version
+from ory_client.model.workspace_meta import WorkspaceMeta
 
 
-class TestVersion(unittest.TestCase):
-    """Version unit test stubs"""
+class TestWorkspaceMeta(unittest.TestCase):
+    """WorkspaceMeta unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVersion(self):
-        """Test Version"""
+    def testWorkspaceMeta(self):
+        """Test WorkspaceMeta"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Version()  # noqa: E501
+        # model = WorkspaceMeta()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_warning.py` & `ory-client-1.9.0/test/test_plan_features.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.warning import Warning
+from ory_client.model.generic_usage import GenericUsage
+globals()['GenericUsage'] = GenericUsage
+from ory_client.model.plan_features import PlanFeatures
 
 
-class TestWarning(unittest.TestCase):
-    """Warning unit test stubs"""
+class TestPlanFeatures(unittest.TestCase):
+    """PlanFeatures unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWarning(self):
-        """Test Warning"""
+    def testPlanFeatures(self):
+        """Test PlanFeatures"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Warning()  # noqa: E501
+        # model = PlanFeatures()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ory-client-1.8.1/test/test_workspace.py` & `ory-client-1.9.0/test/test_project_member.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Ory APIs
 
     Documentation for all public and administrative Ory APIs. Administrative APIs can only be accessed with a valid Personal Access Token. Public APIs are mostly used in browsers.   # noqa: E501
 
-    The version of the OpenAPI document: v1.8.1
+    The version of the OpenAPI document: v1.9.0
     Contact: support@ory.sh
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ory_client
-from ory_client.model.workspace import Workspace
+from ory_client.model.project_member import ProjectMember
 
 
-class TestWorkspace(unittest.TestCase):
-    """Workspace unit test stubs"""
+class TestProjectMember(unittest.TestCase):
+    """ProjectMember unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWorkspace(self):
-        """Test Workspace"""
+    def testProjectMember(self):
+        """Test ProjectMember"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Workspace()  # noqa: E501
+        # model = ProjectMember()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

