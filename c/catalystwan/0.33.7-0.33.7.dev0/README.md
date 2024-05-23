# Comparing `tmp/catalystwan-0.33.7.tar.gz` & `tmp/catalystwan-0.33.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystwan-0.33.7.tar", max compression
+gzip compressed data, was "catalystwan-0.33.7.dev0.tar", max compression
```

## Comparing `catalystwan-0.33.7.tar` & `catalystwan-0.33.7.dev0.tar`

### file list

```diff
@@ -1,345 +1,548 @@
--rw-r--r--   0        0        0    11375 2024-05-22 15:33:19.606312 catalystwan-0.33.7/LICENSE
--rw-r--r--   0        0        0    13654 2024-05-22 15:33:19.606312 catalystwan-0.33.7/README.md
--rw-r--r--   0        0        0     2524 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/__init__.py
--rw-r--r--   0        0        0     1533 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/abstractions.py
--rw-r--r--   0        0        0        0 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/__init__.py
--rw-r--r--   0        0        0     6689 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/admin_tech_api.py
--rw-r--r--   0        0        0    14935 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/administration.py
--rw-r--r--   0        0        0     6314 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/alarms_api.py
--rw-r--r--   0        0        0     3220 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/api_container.py
--rw-r--r--   0        0        0    11636 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/basic_api.py
--rw-r--r--   0        0        0     2053 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/config_device_inventory_api.py
--rw-r--r--   0        0        0     4301 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/config_group_api.py
--rw-r--r--   0        0        0     4645 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/configuration_groups/parcel.py
--rw-r--r--   0        0        0     1290 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/configuration_groups/parcels/cellular_controller.py
--rw-r--r--   0        0        0     7315 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/dashboard_api.py
--rw-r--r--   0        0        0     7360 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/device_action_api.py
--rw-r--r--   0        0        0    15767 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/feature_profile_api.py
--rw-r--r--   0        0        0     1919 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/logs_api.py
--rw-r--r--   0        0        0     2449 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/monitoring_status_api.py
--rw-r--r--   0        0        0     6036 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/mtt_aaa_api.py
--rw-r--r--   0        0        0     4394 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/omp_api.py
--rw-r--r--   0        0        0     5691 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/packet_capture_api.py
--rw-r--r--   0        0        0     1654 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/parcel_api.py
--rw-r--r--   0        0        0     5600 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/partition_manager_api.py
--rw-r--r--   0        0        0    28976 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/policy_api.py
--rw-r--r--   0        0        0     2284 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/resource_pool_api.py
--rw-r--r--   0        0        0    11320 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/software_action_api.py
--rw-r--r--   0        0        0     5473 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/speedtest_api.py
--rw-r--r--   0        0        0     7149 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/task_status_api.py
--rw-r--r--   0        0        0    29260 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/template_api.py
--rw-r--r--   0        0        0     3540 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/README.md
--rw-r--r--   0        0        0      251 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/bool_str.py
--rw-r--r--   0        0        0     7481 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/cli_template.py
--rw-r--r--   0        0        0     3107 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/device_template/device_template.py
--rw-r--r--   0        0        0      571 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/device_template/device_template_payload.json.j2
--rw-r--r--   0        0        0      137 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/device_variable.py
--rw-r--r--   0        0        0     5029 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/feature_template.py
--rw-r--r--   0        0        0     6576 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/feature_template_field.py
--rw-r--r--   0        0        0      661 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/feature_template_payload.py
--rw-r--r--   0        0        0     3244 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_aaa_model.py
--rw-r--r--   0        0        0      667 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_banner_model.py
--rw-r--r--   0        0        0     2180 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_bfd_model.py
--rw-r--r--   0        0        0    12522 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_bgp_model.py
--rw-r--r--   0        0        0     3436 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_logging_model.py
--rw-r--r--   0        0        0     1584 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_ntp_model.py
--rw-r--r--   0        0        0     3835 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_omp_model.py
--rw-r--r--   0        0        0     6749 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_ospf.py
--rw-r--r--   0        0        0    13901 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_ospfv3.py
--rw-r--r--   0        0        0     9589 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
--rw-r--r--   0        0        0     2581 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_snmp_model.py
--rw-r--r--   0        0        0     8986 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_system.py
--rw-r--r--   0        0        0    21665 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_vpn_interface_model.py
--rw-r--r--   0        0        0    15836 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_vpn_model.py
--rw-r--r--   0        0        0      472 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cli_template.py
--rw-r--r--   0        0        0     1835 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/omp_vsmart_model.py
--rw-r--r--   0        0        0      806 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/security_vsmart_model.py
--rw-r--r--   0        0        0     1882 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/supported.py
--rw-r--r--   0        0        0     2624 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/system_vsmart_model.py
--rw-r--r--   0        0        0     2261 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/aaa_model.py
--rw-r--r--   0        0        0    11178 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
--rw-r--r--   0        0        0     1041 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
--rw-r--r--   0        0        0     4264 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
--rw-r--r--   0        0        0     3735 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
--rw-r--r--   0        0        0     1999 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
--rw-r--r--   0        0        0     2558 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
--rw-r--r--   0        0        0     4547 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
--rw-r--r--   0        0        0     1843 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
--rw-r--r--   0        0        0     2247 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
--rw-r--r--   0        0        0     2098 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
--rw-r--r--   0        0        0      683 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
--rw-r--r--   0        0        0     7113 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/tenant/tenant.json.j2
--rw-r--r--   0        0        0     1460 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/tenant/tenant_model.py
--rw-r--r--   0        0        0     5013 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/tenant_backup_restore_api.py
--rw-r--r--   0        0        0     4406 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/tenant_management_api.py
--rw-r--r--   0        0        0     5090 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/tenant_migration_api.py
--rw-r--r--   0        0        0    15887 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/versions_utils.py
--rw-r--r--   0        0        0     7715 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/virtual_image_action_api.py
--rw-r--r--   0        0        0    21802 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/dataclasses.py
--rw-r--r--   0        0        0    25866 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/__init__.py
--rw-r--r--   0        0        0    11938 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/administration_user_and_group.py
--rw-r--r--   0        0        0     6731 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/certificate_management_device.py
--rw-r--r--   0        0        0     1476 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/certificate_management_vmanage.py
--rw-r--r--   0        0        0     4035 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/client.py
--rw-r--r--   0        0        0     2722 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/cluster_management.py
--rw-r--r--   0        0        0      983 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/configuration/device/software_update.py
--rw-r--r--   0        0        0     9447 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/configuration/disaster_recovery.py
--rw-r--r--   0        0        0     4037 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
--rw-r--r--   0        0        0     2064 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
--rw-r--r--   0        0        0     4836 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
--rw-r--r--   0        0        0     2028 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
--rw-r--r--   0        0        0     2091 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
--rw-r--r--   0        0        0     2092 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/control.py
--rw-r--r--   0        0        0     2247 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/device_access.py
--rw-r--r--   0        0        0     2324 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
--rw-r--r--   0        0        0     2174 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
--rw-r--r--   0        0        0     2032 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/mesh.py
--rw-r--r--   0        0        0     2073 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/qos_map.py
--rw-r--r--   0        0        0     2132 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/rewrite.py
--rw-r--r--   0        0        0     2039 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/rule_set.py
--rw-r--r--   0        0        0     2159 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/security_group.py
--rw-r--r--   0        0        0     2104 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
--rw-r--r--   0        0        0     2263 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
--rw-r--r--   0        0        0     2186 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
--rw-r--r--   0        0        0     1793 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/app.py
--rw-r--r--   0        0        0     1950 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/app_probe.py
--rw-r--r--   0        0        0     1848 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/as_path.py
--rw-r--r--   0        0        0     1870 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/class_map.py
--rw-r--r--   0        0        0     1827 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/color.py
--rw-r--r--   0        0        0     1911 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/community.py
--rw-r--r--   0        0        0     2016 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
--rw-r--r--   0        0        0     1932 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/data_prefix.py
--rw-r--r--   0        0        0     2079 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/expanded_community.py
--rw-r--r--   0        0        0     1806 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/fqdn.py
--rw-r--r--   0        0        0     1953 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/geo_location.py
--rw-r--r--   0        0        0     1974 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/ips_signature.py
--rw-r--r--   0        0        0     1932 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
--rw-r--r--   0        0        0     1890 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/local_app.py
--rw-r--r--   0        0        0     1953 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/local_domain.py
--rw-r--r--   0        0        0     1848 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/mirror.py
--rw-r--r--   0        0        0     1874 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/policer.py
--rw-r--r--   0        0        0     1806 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/port.py
--rw-r--r--   0        0        0     2115 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
--rw-r--r--   0        0        0     1848 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/prefix.py
--rw-r--r--   0        0        0     1974 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/protocol_name.py
--rw-r--r--   0        0        0     1781 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/region.py
--rw-r--r--   0        0        0     1946 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/site.py
--rw-r--r--   0        0        0     1845 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/sla.py
--rw-r--r--   0        0        0     1806 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/tloc.py
--rw-r--r--   0        0        0     1926 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
--rw-r--r--   0        0        0     1926 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/url_block_list.py
--rw-r--r--   0        0        0     1787 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/vpn.py
--rw-r--r--   0        0        0     1806 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/zone.py
--rw-r--r--   0        0        0     1782 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/security_template.py
--rw-r--r--   0        0        0     1738 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/vedge_template.py
--rw-r--r--   0        0        0     2974 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/vsmart_template.py
--rw-r--r--   0        0        0     8865 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/software_actions.py
--rw-r--r--   0        0        0     6820 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_dashboard_status.py
--rw-r--r--   0        0        0    13587 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_device_actions.py
--rw-r--r--   0        0        0    13973 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_device_inventory.py
--rw-r--r--   0        0        0      881 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_device_template.py
--rw-r--r--   0        0        0     5277 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_feature_profile.py
--rw-r--r--   0        0        0     5158 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_group.py
--rw-r--r--   0        0        0    24950 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_settings.py
--rw-r--r--   0        0        0    14444 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/endpoints_container.py
--rw-r--r--   0        0        0      760 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/misc.py
--rw-r--r--   0        0        0     8272 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/monitoring/device_details.py
--rw-r--r--   0        0        0      400 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/monitoring/security_policy.py
--rw-r--r--   0        0        0      347 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/monitoring/server_info.py
--rw-r--r--   0        0        0     1929 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/monitoring/status.py
--rw-r--r--   0        0        0     1446 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/real_time_monitoring/reboot_history.py
--rw-r--r--   0        0        0     1419 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/sdavc_cloud_connector.py
--rw-r--r--   0        0        0     1047 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/tenant_backup_restore.py
--rw-r--r--   0        0        0     7648 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/tenant_management.py
--rw-r--r--   0        0        0     3582 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/tenant_migration.py
--rw-r--r--   0        0        0     3661 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
--rw-r--r--   0        0        0      802 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/url_monitoring.py
--rw-r--r--   0        0        0     5735 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/exceptions.py
--rw-r--r--   0        0        0     1902 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/integration_tests/test_find_template_values.py
--rw-r--r--   0        0        0      676 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/logging.conf
--rw-r--r--   0        0        0     3079 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/common.py
--rw-r--r--   0        0        0      171 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/common.py
--rw-r--r--   0        0        0     1090 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/config_migration.py
--rw-r--r--   0        0        0    10043 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/README.md
--rw-r--r--   0        0        0      663 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/builder.py
--rw-r--r--   0        0        0     9117 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/common.py
--rw-r--r--   0        0        0     1086 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py
--rw-r--r--   0        0        0     5553 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
--rw-r--r--   0        0        0     1342 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
--rw-r--r--   0        0        0     1121 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
--rw-r--r--   0        0        0      577 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
--rw-r--r--   0        0        0     1033 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
--rw-r--r--   0        0        0      885 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
--rw-r--r--   0        0        0      731 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
--rw-r--r--   0        0        0     1034 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
--rw-r--r--   0        0        0     1034 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
--rw-r--r--   0        0        0     1268 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py
--rw-r--r--   0        0        0     2867 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
--rw-r--r--   0        0        0     1028 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
--rw-r--r--   0        0        0     5197 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
--rw-r--r--   0        0        0      925 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
--rw-r--r--   0        0        0     1581 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
--rw-r--r--   0        0        0     1177 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
--rw-r--r--   0        0        0      759 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
--rw-r--r--   0        0        0      738 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
--rw-r--r--   0        0        0     1182 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
--rw-r--r--   0        0        0     1496 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
--rw-r--r--   0        0        0      801 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
--rw-r--r--   0        0        0      691 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
--rw-r--r--   0        0        0     1131 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
--rw-r--r--   0        0        0      883 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
--rw-r--r--   0        0        0     1384 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
--rw-r--r--   0        0        0    14665 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
--rw-r--r--   0        0        0     8961 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
--rw-r--r--   0        0        0    14020 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
--rw-r--r--   0        0        0     3448 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
--rw-r--r--   0        0        0     3835 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
--rw-r--r--   0        0        0     2777 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
--rw-r--r--   0        0        0    14424 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
--rw-r--r--   0        0        0     9128 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
--rw-r--r--   0        0        0     6575 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
--rw-r--r--   0        0        0     7971 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
--rw-r--r--   0        0        0    24489 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
--rw-r--r--   0        0        0    10081 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
--rw-r--r--   0        0        0     3294 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
--rw-r--r--   0        0        0     6725 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
--rw-r--r--   0        0        0    11900 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
--rw-r--r--   0        0        0     6391 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
--rw-r--r--   0        0        0     6993 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
--rw-r--r--   0        0        0     5179 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
--rw-r--r--   0        0        0     3790 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
--rw-r--r--   0        0        0     5294 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
--rw-r--r--   0        0        0    13826 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
--rw-r--r--   0        0        0     2179 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
--rw-r--r--   0        0        0      167 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/profile_type.py
--rw-r--r--   0        0        0     1041 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/device_inventory.py
--rw-r--r--   0        0        0      341 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/feature_profile_parcel.py
--rw-r--r--   0        0        0      785 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/misc/application_protocols.py
--rw-r--r--   0        0        0      346 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/monitoring/security_policy.py
--rw-r--r--   0        0        0      405 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/monitoring/server_info.py
--rw-r--r--   0        0        0     4567 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/__init__.py
--rw-r--r--   0        0        0     9426 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/centralized.py
--rw-r--r--   0        0        0     5540 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/access_control_list.py
--rw-r--r--   0        0        0     5726 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/access_control_list_ipv6.py
--rw-r--r--   0        0        0    11851 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/control.py
--rw-r--r--   0        0        0     3861 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/device_access.py
--rw-r--r--   0        0        0     3961 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/device_access_ipv6.py
--rw-r--r--   0        0        0     3004 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/hub_and_spoke.py
--rw-r--r--   0        0        0     1184 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/mesh.py
--rw-r--r--   0        0        0     3454 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/qos_map.py
--rw-r--r--   0        0        0     1193 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/rewrite.py
--rw-r--r--   0        0        0    12252 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/rule_set.py
--rw-r--r--   0        0        0     2948 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/security_group.py
--rw-r--r--   0        0        0    13309 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/traffic_data.py
--rw-r--r--   0        0        0     1074 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/vpn_membership.py
--rw-r--r--   0        0        0     9345 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/zone_based_firewall.py
--rw-r--r--   0        0        0    10893 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/lists.py
--rw-r--r--   0        0        0    14613 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/lists_entries.py
--rw-r--r--   0        0        0     5558 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/localized.py
--rw-r--r--   0        0        0     3553 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/policy.py
--rw-r--r--   0        0        0    31904 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/policy_definition.py
--rw-r--r--   0        0        0     1274 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/policy_list.py
--rw-r--r--   0        0        0     7100 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/security.py
--rw-r--r--   0        0        0     5239 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/tenant.py
--rw-r--r--   0        0        0      924 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/url_monitoring.py
--rw-r--r--   0        0        0     9717 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/response.py
--rw-r--r--   0        0        0    19888 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/session.py
--rw-r--r--   0        0        0      401 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
--rw-r--r--   0        0        0      513 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/banner_1.json
--rw-r--r--   0        0        0      116 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/alias.json
--rw-r--r--   0        0        0      114 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/basic.json
--rw-r--r--   0        0        0      109 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/basic_no_value.json
--rw-r--r--   0        0        0      848 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/children.json
--rw-r--r--   0        0        0     2348 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/children_nested.json
--rw-r--r--   0        0        0     2348 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      274 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/data_path.json
--rw-r--r--   0        0        0     2973 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/cisco_bfd.json
--rw-r--r--   0        0        0    11100 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/complex_aaa.json
--rw-r--r--   0        0        0    41165 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
--rw-r--r--   0        0        0     5219 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/default_cisco_system.json
--rw-r--r--   0        0        0     5505 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/iuo.json
--rw-r--r--   0        0        0      249 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/omp_1.json
--rw-r--r--   0        0        0      875 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/omp_2.json
--rw-r--r--   0        0        0     1682 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/omp_3.json
--rw-r--r--   0        0        0      662 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/__init__.py
--rw-r--r--   0        0        0     2828 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_aaa.py
--rw-r--r--   0        0        0      303 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_banner.py
--rw-r--r--   0        0        0      587 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_bfd.py
--rw-r--r--   0        0        0      344 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_system.py
--rw-r--r--   0        0        0     8078 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_vpn.py
--rw-r--r--   0        0        0     1091 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/omp_vsmart.py
--rw-r--r--   0        0        0      605 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/alias.json
--rw-r--r--   0        0        0      574 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/basic.json
--rw-r--r--   0        0        0     1810 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/children.json
--rw-r--r--   0        0        0     4005 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/children_nested.json
--rw-r--r--   0        0        0     4005 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      731 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/data_path.json
--rw-r--r--   0        0        0    43436 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/cedge_aaa.json
--rw-r--r--   0        0        0     1200 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_banner.json
--rw-r--r--   0        0        0     9495 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_bfd.json
--rw-r--r--   0        0        0    99045 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_system.json
--rw-r--r--   0        0        0    87854 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_vpn.json
--rw-r--r--   0        0        0     5939 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/omp-vsmart.json
--rw-r--r--   0        0        0     1381 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/test_chose_model.py
--rw-r--r--   0        0        0     2598 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/test_deserialize_model.py
--rw-r--r--   0        0        0     6762 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/test_find_template_values.py
--rw-r--r--   0        0        0     4598 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/test_generate_payload.py
--rw-r--r--   0        0        0     1756 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/test_serialize_model.py
--rw-r--r--   0        0        0     8145 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_admin_tech_api.py
--rw-r--r--   0        0        0    17792 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_administration.py
--rw-r--r--   0        0        0    11116 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_alarms_api.py
--rw-r--r--   0        0        0     8322 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_cli_template.py
--rw-r--r--   0        0        0     5494 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_creation_tools.py
--rw-r--r--   0        0        0     3981 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_device_action_api.py
--rw-r--r--   0        0        0    28159 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_devices_api.py
--rw-r--r--   0        0        0    33583 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_endpoints.py
--rw-r--r--   0        0        0      894 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_feature_template_field.py
--rw-r--r--   0        0        0     1545 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_logs_api.py
--rw-r--r--   0        0        0     2896 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_monitoring_security_policy.py
--rw-r--r--   0        0        0     1809 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_monitoring_server_info.py
--rw-r--r--   0        0        0     5489 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_monitoring_status_api.py
--rw-r--r--   0        0        0    11026 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_mtt_aaa_api.py
--rw-r--r--   0        0        0    16472 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_omp_api.py
--rw-r--r--   0        0        0     5223 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_packet_capture.py
--rw-r--r--   0        0        0     5727 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_partition_manager_api.py
--rw-r--r--   0        0        0     7883 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_response.py
--rw-r--r--   0        0        0     6724 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_session.py
--rw-r--r--   0        0        0     7117 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_software_action_api.py
--rw-r--r--   0        0        0     6071 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_speed_test_api.py
--rw-r--r--   0        0        0    14926 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_task_status_api.py
--rw-r--r--   0        0        0    15050 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_templates.py
--rw-r--r--   0        0        0     3705 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_tenant_backup_restore_api.py
--rw-r--r--   0        0        0     6114 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_tenant_management_api.py
--rw-r--r--   0        0        0     4506 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_tenant_migration_api.py
--rw-r--r--   0        0        0    12377 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/tests/test_typed_list.py
--rw-r--r--   0        0        0     3746 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/tests/test_url_monitoring.py
--rw-r--r--   0        0        0     2968 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/tests/test_version.py
--rw-r--r--   0        0        0    10377 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/tests/test_version_utils.py
--rw-r--r--   0        0        0     3343 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/tests/test_vmanage_auth.py
--rw-r--r--   0        0        0     9379 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/typed_list.py
--rw-r--r--   0        0        0        0 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/__init__.py
--rw-r--r--   0        0        0      266 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/alarm_status.py
--rw-r--r--   0        0        0      253 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/certificate_status.py
--rw-r--r--   0        0        0      279 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/colors.py
--rw-r--r--   0        0        0      154 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/config_status.py
--rw-r--r--   0        0        0     4778 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/creation_tools.py
--rw-r--r--   0        0        0     7281 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/dashboard.py
--rw-r--r--   0        0        0     2863 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/device_model.py
--rw-r--r--   0        0        0     2110 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/dict.py
--rw-r--r--   0        0        0      953 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/feature_template/choose_model.py
--rw-r--r--   0        0        0     4882 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/feature_template/find_template_values.py
--rw-r--r--   0        0        0      584 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/operation_status.py
--rw-r--r--   0        0        0      196 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/personality.py
--rw-r--r--   0        0        0      360 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/pydantic_field.py
--rw-r--r--   0        0        0      172 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/reachability.py
--rw-r--r--   0        0        0      407 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/session_type.py
--rw-r--r--   0        0        0      149 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/template_type.py
--rw-r--r--   0        0        0    17168 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/timezone.py
--rw-r--r--   0        0        0     3930 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/upgrades_helper.py
--rw-r--r--   0        0        0      159 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/validate_status.py
--rw-r--r--   0        0        0     3032 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/version.py
--rw-r--r--   0        0        0     5415 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/vmanage_auth.py
--rw-r--r--   0        0        0     9946 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/workflows/tenant_migration.py
--rw-r--r--   0        0        0      862 2024-05-22 15:33:19.626312 catalystwan-0.33.7/pyproject.toml
--rw-r--r--   0        0        0    17267 1970-01-01 00:00:00.000000 catalystwan-0.33.7/setup.py
--rw-r--r--   0        0        0    14781 1970-01-01 00:00:00.000000 catalystwan-0.33.7/PKG-INFO
+-rw-r--r--   0        0        0    11375 2024-05-22 21:06:37.207814 catalystwan-0.33.7.dev0/LICENSE
+-rw-r--r--   0        0        0    13533 2024-05-22 21:06:37.207814 catalystwan-0.33.7.dev0/README.md
+-rw-r--r--   0        0        0     2558 2024-05-22 21:06:37.207814 catalystwan-0.33.7.dev0/catalystwan/__init__.py
+-rw-r--r--   0        0        0     1532 2024-05-22 21:06:37.207814 catalystwan-0.33.7.dev0/catalystwan/abstractions.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:06:37.207814 catalystwan-0.33.7.dev0/catalystwan/api/__init__.py
+-rw-r--r--   0        0        0     6689 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/admin_tech_api.py
+-rw-r--r--   0        0        0    14935 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/administration.py
+-rw-r--r--   0        0        0     6314 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/alarms_api.py
+-rw-r--r--   0        0        0     3293 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/api_container.py
+-rw-r--r--   0        0        0    11636 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/basic_api.py
+-rw-r--r--   0        0        0      386 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/builders/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/builders/feature_profiles/__init__.py
+-rw-r--r--   0        0        0     2017 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/builders/feature_profiles/builder_factory.py
+-rw-r--r--   0        0        0     2679 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/builders/feature_profiles/cli.py
+-rw-r--r--   0        0        0     2696 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/builders/feature_profiles/other.py
+-rw-r--r--   0        0        0     3146 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/builders/feature_profiles/report.py
+-rw-r--r--   0        0        0     5727 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/builders/feature_profiles/service.py
+-rw-r--r--   0        0        0     2768 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/builders/feature_profiles/system.py
+-rw-r--r--   0        0        0     4328 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/builders/feature_profiles/transport.py
+-rw-r--r--   0        0        0     2053 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/config_device_inventory_api.py
+-rw-r--r--   0        0        0     4760 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/config_group_api.py
+-rw-r--r--   0        0        0     6672 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/configuration_groups/parcel.py
+-rw-r--r--   0        0        0     7315 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/dashboard_api.py
+-rw-r--r--   0        0        0     7360 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/device_action_api.py
+-rw-r--r--   0        0        0    53328 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/feature_profile_api.py
+-rw-r--r--   0        0        0     1919 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/logs_api.py
+-rw-r--r--   0        0        0     2449 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/monitoring_status_api.py
+-rw-r--r--   0        0        0     6036 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/mtt_aaa_api.py
+-rw-r--r--   0        0        0     4394 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/omp_api.py
+-rw-r--r--   0        0        0     5691 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/packet_capture_api.py
+-rw-r--r--   0        0        0     1654 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/parcel_api.py
+-rw-r--r--   0        0        0     5600 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/partition_manager_api.py
+-rw-r--r--   0        0        0    36861 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/policy_api.py
+-rw-r--r--   0        0        0     2284 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/resource_pool_api.py
+-rw-r--r--   0        0        0    11320 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/software_action_api.py
+-rw-r--r--   0        0        0     5473 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/speedtest_api.py
+-rw-r--r--   0        0        0     7149 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/task_status_api.py
+-rw-r--r--   0        0        0    30133 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/template_api.py
+-rw-r--r--   0        0        0     3540 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/README.md
+-rw-r--r--   0        0        0      251 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/bool_str.py
+-rw-r--r--   0        0        0     7481 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/cli_template.py
+-rw-r--r--   0        0        0     3425 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/device_template/device_template.py
+-rw-r--r--   0        0        0      571 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/device_template/device_template_payload.json.j2
+-rw-r--r--   0        0        0      137 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/device_variable.py
+-rw-r--r--   0        0        0     5029 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/feature_template.py
+-rw-r--r--   0        0        0     6576 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/feature_template_field.py
+-rw-r--r--   0        0        0      661 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/feature_template_payload.py
+-rw-r--r--   0        0        0     3244 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_aaa_model.py
+-rw-r--r--   0        0        0      667 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_banner_model.py
+-rw-r--r--   0        0        0     2180 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_bfd_model.py
+-rw-r--r--   0        0        0    12522 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_bgp_model.py
+-rw-r--r--   0        0        0     3436 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_logging_model.py
+-rw-r--r--   0        0        0     1584 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_ntp_model.py
+-rw-r--r--   0        0        0     3835 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_omp_model.py
+-rw-r--r--   0        0        0     6749 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_ospf.py
+-rw-r--r--   0        0        0    13901 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_ospfv3.py
+-rw-r--r--   0        0        0     9589 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
+-rw-r--r--   0        0        0     2581 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_snmp_model.py
+-rw-r--r--   0        0        0     8986 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_system.py
+-rw-r--r--   0        0        0    21665 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_vpn_interface_model.py
+-rw-r--r--   0        0        0    15836 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_vpn_model.py
+-rw-r--r--   0        0        0      472 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cli_template.py
+-rw-r--r--   0        0        0     1835 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/omp_vsmart_model.py
+-rw-r--r--   0        0        0      806 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/security_vsmart_model.py
+-rw-r--r--   0        0        0     1882 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/supported.py
+-rw-r--r--   0        0        0     2624 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/models/system_vsmart_model.py
+-rw-r--r--   0        0        0     2261 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/aaa/aaa_model.py
+-rw-r--r--   0        0        0    11178 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
+-rw-r--r--   0        0        0     1041 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
+-rw-r--r--   0        0        0     4264 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
+-rw-r--r--   0        0        0     3735 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
+-rw-r--r--   0        0        0     1999 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
+-rw-r--r--   0        0        0     2558 2024-05-22 21:06:37.211814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
+-rw-r--r--   0        0        0     4547 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
+-rw-r--r--   0        0        0     1843 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
+-rw-r--r--   0        0        0     2247 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
+-rw-r--r--   0        0        0     2098 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
+-rw-r--r--   0        0        0      683 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
+-rw-r--r--   0        0        0     7113 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/tenant/tenant.json.j2
+-rw-r--r--   0        0        0     1460 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/tenant/tenant_model.py
+-rw-r--r--   0        0        0     5013 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/api/tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     4406 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/api/tenant_management_api.py
+-rw-r--r--   0        0        0     5090 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/api/tenant_migration_api.py
+-rw-r--r--   0        0        0    13729 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/api/versions_utils.py
+-rw-r--r--   0        0        0    21802 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/dataclasses.py
+-rw-r--r--   0        0        0    27207 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/__init__.py
+-rw-r--r--   0        0        0    11938 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/administration_user_and_group.py
+-rw-r--r--   0        0        0     6731 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/certificate_management_device.py
+-rw-r--r--   0        0        0     1476 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/certificate_management_vmanage.py
+-rw-r--r--   0        0        0     4035 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/client.py
+-rw-r--r--   0        0        0     2722 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/cluster_management.py
+-rw-r--r--   0        0        0      983 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/device/software_update.py
+-rw-r--r--   0        0        0     9447 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/disaster_recovery.py
+-rw-r--r--   0        0        0     3876 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/application_priority.py
+-rw-r--r--   0        0        0     2406 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/cli.py
+-rw-r--r--   0        0        0     3557 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/dns_security.py
+-rw-r--r--   0        0        0     3735 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/embedded_security.py
+-rw-r--r--   0        0        0     2600 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py
+-rw-r--r--   0        0        0     4037 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
+-rw-r--r--   0        0        0     2747 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py
+-rw-r--r--   0        0        0     3315 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/sig_security.py
+-rw-r--r--   0        0        0    10040 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
+-rw-r--r--   0        0        0     3679 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/topology.py
+-rw-r--r--   0        0        0     6471 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
+-rw-r--r--   0        0        0     1361 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/abstractions.py
+-rw-r--r--   0        0        0     1969 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     2024 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2046 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/aip.py
+-rw-r--r--   0        0        0     2046 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/amp.py
+-rw-r--r--   0        0        0     1756 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/cflowd.py
+-rw-r--r--   0        0        0     2025 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/control.py
+-rw-r--r--   0        0        0     2170 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/device_access.py
+-rw-r--r--   0        0        0     2239 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     1853 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/dns_security.py
+-rw-r--r--   0        0        0     2099 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     1995 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/intrusion_prevention.py
+-rw-r--r--   0        0        0     1954 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/mesh.py
+-rw-r--r--   0        0        0     1991 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     2065 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/rewrite.py
+-rw-r--r--   0        0        0     1798 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/route_policy.py
+-rw-r--r--   0        0        0     1967 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     2092 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/security_group.py
+-rw-r--r--   0        0        0     1879 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/ssl_decryption.py
+-rw-r--r--   0        0        0     1985 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/ssl_decryption_utd_profile.py
+-rw-r--r--   0        0        0     2029 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     1869 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/url_filtering.py
+-rw-r--r--   0        0        0     2184 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0     2111 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1740 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/app.py
+-rw-r--r--   0        0        0     1900 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/app_probe.py
+-rw-r--r--   0        0        0     1793 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/as_path.py
+-rw-r--r--   0        0        0     1813 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/class_map.py
+-rw-r--r--   0        0        0     1772 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/color.py
+-rw-r--r--   0        0        0     1854 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/community.py
+-rw-r--r--   0        0        0     1971 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0     1873 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/data_prefix.py
+-rw-r--r--   0        0        0     2023 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/expanded_community.py
+-rw-r--r--   0        0        0     1978 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/extended_community.py
+-rw-r--r--   0        0        0     1752 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1893 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/geo_location.py
+-rw-r--r--   0        0        0     1930 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1873 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0     1833 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/local_app.py
+-rw-r--r--   0        0        0     1893 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/local_domain.py
+-rw-r--r--   0        0        0     1792 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/mirror.py
+-rw-r--r--   0        0        0     1817 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/policer.py
+-rw-r--r--   0        0        0     1752 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/port.py
+-rw-r--r--   0        0        0     2065 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1852 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/prefix.py
+-rw-r--r--   0        0        0     1930 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1683 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/region.py
+-rw-r--r--   0        0        0     1892 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/site.py
+-rw-r--r--   0        0        0     1782 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/sla.py
+-rw-r--r--   0        0        0     1940 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py
+-rw-r--r--   0        0        0     1752 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/tloc.py
+-rw-r--r--   0        0        0     1872 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/trunkgroup.py
+-rw-r--r--   0        0        0     1930 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/umbrella_data.py
+-rw-r--r--   0        0        0     1863 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
+-rw-r--r--   0        0        0     1863 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/url_block_list.py
+-rw-r--r--   0        0        0     1734 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/vpn.py
+-rw-r--r--   0        0        0     1752 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/zone.py
+-rw-r--r--   0        0        0     1726 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/security_template.py
+-rw-r--r--   0        0        0     1738 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/vedge_template.py
+-rw-r--r--   0        0        0     2974 2024-05-22 21:06:37.215814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/vsmart_template.py
+-rw-r--r--   0        0        0     8865 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/software_actions.py
+-rw-r--r--   0        0        0     6820 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_dashboard_status.py
+-rw-r--r--   0        0        0    10675 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_device_actions.py
+-rw-r--r--   0        0        0    13973 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_device_inventory.py
+-rw-r--r--   0        0        0      881 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_device_template.py
+-rw-r--r--   0        0        0     5277 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_feature_profile.py
+-rw-r--r--   0        0        0     6387 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_group.py
+-rw-r--r--   0        0        0    27565 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_settings.py
+-rw-r--r--   0        0        0    14794 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/endpoints_container.py
+-rw-r--r--   0        0        0      760 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/misc.py
+-rw-r--r--   0        0        0     8272 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/monitoring/device_details.py
+-rw-r--r--   0        0        0      347 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/monitoring/server_info.py
+-rw-r--r--   0        0        0     1929 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/monitoring/status.py
+-rw-r--r--   0        0        0     1446 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/real_time_monitoring/reboot_history.py
+-rw-r--r--   0        0        0     1419 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/sdavc_cloud_connector.py
+-rw-r--r--   0        0        0     1047 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/tenant_backup_restore.py
+-rw-r--r--   0        0        0     7648 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/tenant_management.py
+-rw-r--r--   0        0        0     3649 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/tenant_migration.py
+-rw-r--r--   0        0        0     3661 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
+-rw-r--r--   0        0        0     6246 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/exceptions.py
+-rw-r--r--   0        0        0     1340 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/integration_tests/feature_profile/sdwan/base.py
+-rw-r--r--   0        0        0     5165 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_application_priority.py
+-rw-r--r--   0        0        0     2364 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_cli.py
+-rw-r--r--   0        0        0     4587 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_dns_security.py
+-rw-r--r--   0        0        0     1834 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_other.py
+-rw-r--r--   0        0        0    28479 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_service.py
+-rw-r--r--   0        0        0    14507 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_sig_security.py
+-rw-r--r--   0        0        0     9901 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_system.py
+-rw-r--r--   0        0        0    61890 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py
+-rw-r--r--   0        0        0     4124 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/integration_tests/feature_profile/sdwan/topology/test_topology.py
+-rw-r--r--   0        0        0     1078 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/integration_tests/test_config_migration.py
+-rw-r--r--   0        0        0     1902 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/integration_tests/test_find_template_values.py
+-rw-r--r--   0        0        0      676 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/logging.conf
+-rw-r--r--   0        0        0    16090 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/common.py
+-rw-r--r--   0        0        0      194 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/common.py
+-rw-r--r--   0        0        0    12883 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/config_migration.py
+-rw-r--r--   0        0        0       89 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/docs/README.md
+-rw-r--r--   0        0        0   142336 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/docs/diagram.png
+-rw-r--r--   0        0        0    10043 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/README.md
+-rw-r--r--   0        0        0      663 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/builder.py
+-rw-r--r--   0        0        0    25676 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/common.py
+-rw-r--r--   0        0        0     5106 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/parcel.py
+-rw-r--r--   0        0        0      661 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/application_priority/__init__.py
+-rw-r--r--   0        0        0     1385 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/application_priority/policy_settings.py
+-rw-r--r--   0        0        0     1554 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/application_priority/qos_policy.py
+-rw-r--r--   0        0        0      292 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/cli/__init__.py
+-rw-r--r--   0        0        0      480 2024-05-22 21:06:37.219814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/cli/config.py
+-rw-r--r--   0        0        0      275 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/dns_security/__init__.py
+-rw-r--r--   0        0        0     2787 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/dns_security/dns.py
+-rw-r--r--   0        0        0      507 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/__init__.py
+-rw-r--r--   0        0        0    16716 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/ngfirewall.py
+-rw-r--r--   0        0        0     4103 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/policy.py
+-rw-r--r--   0        0        0      420 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/other/__init__.py
+-rw-r--r--   0        0        0     4750 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py
+-rw-r--r--   0        0        0     3950 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py
+-rw-r--r--   0        0        0     5256 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
+-rw-r--r--   0        0        0     1426 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
+-rw-r--r--   0        0        0     1203 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
+-rw-r--r--   0        0        0      825 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py
+-rw-r--r--   0        0        0      653 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
+-rw-r--r--   0        0        0     1244 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
+-rw-r--r--   0        0        0     1034 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
+-rw-r--r--   0        0        0      807 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
+-rw-r--r--   0        0        0     1152 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
+-rw-r--r--   0        0        0     1706 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
+-rw-r--r--   0        0        0      737 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py
+-rw-r--r--   0        0        0     1332 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py
+-rw-r--r--   0        0        0     3106 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
+-rw-r--r--   0        0        0     1106 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
+-rw-r--r--   0        0        0     5272 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
+-rw-r--r--   0        0        0     1215 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
+-rw-r--r--   0        0        0     1641 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
+-rw-r--r--   0        0        0     1442 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py
+-rw-r--r--   0        0        0     1898 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py
+-rw-r--r--   0        0        0     1277 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
+-rw-r--r--   0        0        0      871 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
+-rw-r--r--   0        0        0      830 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
+-rw-r--r--   0        0        0     1288 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
+-rw-r--r--   0        0        0     1398 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py
+-rw-r--r--   0        0        0     1604 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
+-rw-r--r--   0        0        0      907 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
+-rw-r--r--   0        0        0      799 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
+-rw-r--r--   0        0        0     1408 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
+-rw-r--r--   0        0        0     3388 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py
+-rw-r--r--   0        0        0     3935 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py
+-rw-r--r--   0        0        0     1079 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
+-rw-r--r--   0        0        0     3679 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py
+-rw-r--r--   0        0        0     1461 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
+-rw-r--r--   0        0        0     2255 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py
+-rw-r--r--   0        0        0    14507 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
+-rw-r--r--   0        0        0    10235 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
+-rw-r--r--   0        0        0    14485 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
+-rw-r--r--   0        0        0     5289 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
+-rw-r--r--   0        0        0     4001 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
+-rw-r--r--   0        0        0     1349 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
+-rw-r--r--   0        0        0    12626 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
+-rw-r--r--   0        0        0     6938 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
+-rw-r--r--   0        0        0     6350 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
+-rw-r--r--   0        0        0     5349 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/multilink.py
+-rw-r--r--   0        0        0     8633 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
+-rw-r--r--   0        0        0    24965 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
+-rw-r--r--   0        0        0    10821 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
+-rw-r--r--   0        0        0     3291 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
+-rw-r--r--   0        0        0     7362 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
+-rw-r--r--   0        0        0    12770 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
+-rw-r--r--   0        0        0     9187 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
+-rw-r--r--   0        0        0     6966 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
+-rw-r--r--   0        0        0     5161 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
+-rw-r--r--   0        0        0     3705 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
+-rw-r--r--   0        0        0     5706 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
+-rw-r--r--   0        0        0      297 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/sig_security/__init__.py
+-rw-r--r--   0        0        0    16817 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/sig_security/sig_security.py
+-rw-r--r--   0        0        0     1058 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py
+-rw-r--r--   0        0        0    15436 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
+-rw-r--r--   0        0        0      977 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py
+-rw-r--r--   0        0        0    10457 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py
+-rw-r--r--   0        0        0     2623 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py
+-rw-r--r--   0        0        0     6396 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py
+-rw-r--r--   0        0        0     6355 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py
+-rw-r--r--   0        0        0     2935 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py
+-rw-r--r--   0        0        0     3932 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py
+-rw-r--r--   0        0        0     5166 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py
+-rw-r--r--   0        0        0     6653 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/security.py
+-rw-r--r--   0        0        0     6841 2024-05-22 21:06:37.223814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py
+-rw-r--r--   0        0        0      726 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/topology/__init__.py
+-rw-r--r--   0        0        0    12828 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/topology/custom_control.py
+-rw-r--r--   0        0        0     2162 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/topology/hubspoke.py
+-rw-r--r--   0        0        0      799 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/topology/mesh.py
+-rw-r--r--   0        0        0     2530 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py
+-rw-r--r--   0        0        0    26093 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/bgp.py
+-rw-r--r--   0        0        0     2276 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
+-rw-r--r--   0        0        0     2668 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_profile.py
+-rw-r--r--   0        0        0     1579 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/gps.py
+-rw-r--r--   0        0        0     5634 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/management/ethernet.py
+-rw-r--r--   0        0        0     4400 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/t1e1controller.py
+-rw-r--r--   0        0        0    12662 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn.py
+-rw-r--r--   0        0        0     9090 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/cellular.py
+-rw-r--r--   0        0        0    13993 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ethernet.py
+-rw-r--r--   0        0        0     2169 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/gre.py
+-rw-r--r--   0        0        0     5137 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ipsec.py
+-rw-r--r--   0        0        0    11421 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/multilink.py
+-rw-r--r--   0        0        0    16558 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/protocol_over.py
+-rw-r--r--   0        0        0     8889 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/t1e1serial.py
+-rw-r--r--   0        0        0      157 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/profile_type.py
+-rw-r--r--   0        0        0      378 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/configuration/topology_group.py
+-rw-r--r--   0        0        0     1041 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/device_inventory.py
+-rw-r--r--   0        0        0      341 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/feature_profile_parcel.py
+-rw-r--r--   0        0        0      785 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/misc/application_protocols.py
+-rw-r--r--   0        0        0      405 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/monitoring/server_info.py
+-rw-r--r--   0        0        0    10542 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/__init__.py
+-rw-r--r--   0        0        0     8738 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/centralized.py
+-rw-r--r--   0        0        0     5789 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     5991 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2204 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/aip.py
+-rw-r--r--   0        0        0     2598 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/amp.py
+-rw-r--r--   0        0        0     3159 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/cflowd.py
+-rw-r--r--   0        0        0    12117 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/control.py
+-rw-r--r--   0        0        0     4134 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/device_access.py
+-rw-r--r--   0        0        0     4250 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     4585 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/dns_security.py
+-rw-r--r--   0        0        0     3251 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     2139 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/intrusion_prevention.py
+-rw-r--r--   0        0        0     1403 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/mesh.py
+-rw-r--r--   0        0        0     3520 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     1410 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/rewrite.py
+-rw-r--r--   0        0        0     6150 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/route_policy.py
+-rw-r--r--   0        0        0    12381 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     3147 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/security_group.py
+-rw-r--r--   0        0        0     7992 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/ssl_decryption.py
+-rw-r--r--   0        0        0     3539 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/ssl_decryption_utd_profile.py
+-rw-r--r--   0        0        0    14018 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     2684 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/url_filtering.py
+-rw-r--r--   0        0        0     1329 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0    10584 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1094 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/app.py
+-rw-r--r--   0        0        0     1295 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/app_probe.py
+-rw-r--r--   0        0        0      651 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/as_path.py
+-rw-r--r--   0        0        0      789 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/class_map.py
+-rw-r--r--   0        0        0      661 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/color.py
+-rw-r--r--   0        0        0     2634 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/communities.py
+-rw-r--r--   0        0        0      918 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0      860 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/data_prefix.py
+-rw-r--r--   0        0        0      495 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1055 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/geo_location.py
+-rw-r--r--   0        0        0      817 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1111 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0      990 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/local_app.py
+-rw-r--r--   0        0        0      923 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/local_domain.py
+-rw-r--r--   0        0        0      714 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/mirror.py
+-rw-r--r--   0        0        0     1127 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/policer.py
+-rw-r--r--   0        0        0      771 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/port.py
+-rw-r--r--   0        0        0     3196 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1055 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/prefix.py
+-rw-r--r--   0        0        0      723 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1325 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/region.py
+-rw-r--r--   0        0        0      942 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/site.py
+-rw-r--r--   0        0        0     6864 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/sla.py
+-rw-r--r--   0        0        0      970 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/threat_grid_api_key.py
+-rw-r--r--   0        0        0      960 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/tloc.py
+-rw-r--r--   0        0        0     2111 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/trunkgroup.py
+-rw-r--r--   0        0        0      824 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/umbrella_data.py
+-rw-r--r--   0        0        0      856 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/url.py
+-rw-r--r--   0        0        0     1071 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/vpn.py
+-rw-r--r--   0        0        0     1405 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/list/zone.py
+-rw-r--r--   0        0        0     6204 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/localized.py
+-rw-r--r--   0        0        0     3752 2024-05-22 21:06:37.227814 catalystwan-0.33.7.dev0/catalystwan/models/policy/policy.py
+-rw-r--r--   0        0        0    37156 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/models/policy/policy_definition.py
+-rw-r--r--   0        0        0     1557 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/models/policy/policy_list.py
+-rw-r--r--   0        0        0     9385 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/models/policy/security.py
+-rw-r--r--   0        0        0     2437 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/models/templates.py
+-rw-r--r--   0        0        0     5239 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/models/tenant.py
+-rw-r--r--   0        0        0     9717 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/response.py
+-rw-r--r--   0        0        0    19497 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/session.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/config_migration/__init__.py
+-rw-r--r--   0        0        0     1236 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/config_migration/test_converter_chooser.py
+-rw-r--r--   0        0        0      467 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/config_migration/test_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/config_migration/test_data/feature_templates/__init__.py
+-rw-r--r--   0        0        0    10804 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/config_migration/test_data/feature_templates/interface.py
+-rw-r--r--   0        0        0      519 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/config_migration/test_data/feature_templates/malformed.py
+-rw-r--r--   0        0        0     3185 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/config_migration/test_data/feature_templates/vpn.py
+-rw-r--r--   0        0        0     3583 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/config_migration/test_device_template_with_info.py
+-rw-r--r--   0        0        0     6139 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/config_migration/test_merge_parcels.py
+-rw-r--r--   0        0        0     4525 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/config_migration/test_normalizer.py
+-rw-r--r--   0        0        0    10765 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/config_migration/test_transform.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/models/__init__.py
+-rw-r--r--   0        0        0      401 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
+-rw-r--r--   0        0        0      513 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/banner_1.json
+-rw-r--r--   0        0        0      116 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/basic/alias.json
+-rw-r--r--   0        0        0      114 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/basic/basic.json
+-rw-r--r--   0        0        0      109 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/basic/basic_no_value.json
+-rw-r--r--   0        0        0      848 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/basic/children.json
+-rw-r--r--   0        0        0     2348 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/basic/children_nested.json
+-rw-r--r--   0        0        0     2348 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      274 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/basic/data_path.json
+-rw-r--r--   0        0        0     2973 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/cisco_bfd.json
+-rw-r--r--   0        0        0    11100 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/complex_aaa.json
+-rw-r--r--   0        0        0    41165 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
+-rw-r--r--   0        0        0     5219 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/default_cisco_system.json
+-rw-r--r--   0        0        0     5505 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/iuo.json
+-rw-r--r--   0        0        0      249 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/omp_1.json
+-rw-r--r--   0        0        0      875 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/omp_2.json
+-rw-r--r--   0        0        0     1682 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/omp_3.json
+-rw-r--r--   0        0        0      662 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/models/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/models/cisco_aaa.py
+-rw-r--r--   0        0        0      303 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/models/cisco_banner.py
+-rw-r--r--   0        0        0      587 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/models/cisco_bfd.py
+-rw-r--r--   0        0        0      344 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/models/cisco_system.py
+-rw-r--r--   0        0        0     8078 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/models/cisco_vpn.py
+-rw-r--r--   0        0        0     1091 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/models/omp_vsmart.py
+-rw-r--r--   0        0        0      605 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/basic/alias.json
+-rw-r--r--   0        0        0      574 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/basic/basic.json
+-rw-r--r--   0        0        0     1810 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/basic/children.json
+-rw-r--r--   0        0        0     4005 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/basic/children_nested.json
+-rw-r--r--   0        0        0     4005 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      731 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/basic/data_path.json
+-rw-r--r--   0        0        0    43436 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/cedge_aaa.json
+-rw-r--r--   0        0        0     1200 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/cisco_banner.json
+-rw-r--r--   0        0        0     9495 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/cisco_bfd.json
+-rw-r--r--   0        0        0    99045 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/cisco_system.json
+-rw-r--r--   0        0        0    87854 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/cisco_vpn.json
+-rw-r--r--   0        0        0     5939 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/omp-vsmart.json
+-rw-r--r--   0        0        0     1381 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/test_chose_model.py
+-rw-r--r--   0        0        0     2598 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/test_deserialize_model.py
+-rw-r--r--   0        0        0     6762 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/test_find_template_values.py
+-rw-r--r--   0        0        0     4598 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/test_generate_payload.py
+-rw-r--r--   0        0        0     1755 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/templates/test_serialize_model.py
+-rw-r--r--   0        0        0     8145 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/test_admin_tech_api.py
+-rw-r--r--   0        0        0    17792 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/test_administration.py
+-rw-r--r--   0        0        0    11116 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/test_alarms_api.py
+-rw-r--r--   0        0        0     8322 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/test_cli_template.py
+-rw-r--r--   0        0        0     5494 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/test_creation_tools.py
+-rw-r--r--   0        0        0     3981 2024-05-22 21:06:37.231814 catalystwan-0.33.7.dev0/catalystwan/tests/test_device_action_api.py
+-rw-r--r--   0        0        0    28159 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_devices_api.py
+-rw-r--r--   0        0        0    34864 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_endpoints.py
+-rw-r--r--   0        0        0    10585 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_feature_profile_api.py
+-rw-r--r--   0        0        0      894 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_feature_template_field.py
+-rw-r--r--   0        0        0     1545 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_logs_api.py
+-rw-r--r--   0        0        0     1899 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_models_common.py
+-rw-r--r--   0        0        0     1809 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_monitoring_server_info.py
+-rw-r--r--   0        0        0     5489 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_monitoring_status_api.py
+-rw-r--r--   0        0        0    11026 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_mtt_aaa_api.py
+-rw-r--r--   0        0        0    10026 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_normalize_to_model_definition.py
+-rw-r--r--   0        0        0    16472 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_omp_api.py
+-rw-r--r--   0        0        0     5223 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_packet_capture.py
+-rw-r--r--   0        0        0     5727 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_partition_manager_api.py
+-rw-r--r--   0        0        0     7926 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_response.py
+-rw-r--r--   0        0        0     6724 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_session.py
+-rw-r--r--   0        0        0     7117 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_software_action_api.py
+-rw-r--r--   0        0        0     6071 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_speed_test_api.py
+-rw-r--r--   0        0        0    14926 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_task_status_api.py
+-rw-r--r--   0        0        0    15055 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_templates.py
+-rw-r--r--   0        0        0     3705 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     6114 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_tenant_management_api.py
+-rw-r--r--   0        0        0     4506 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_tenant_migration_api.py
+-rw-r--r--   0        0        0    12377 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_typed_list.py
+-rw-r--r--   0        0        0     2968 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_version.py
+-rw-r--r--   0        0        0    10377 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_version_utils.py
+-rw-r--r--   0        0        0     3343 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/tests/test_vmanage_auth.py
+-rw-r--r--   0        0        0     9379 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/typed_list.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/__init__.py
+-rw-r--r--   0        0        0      266 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/alarm_status.py
+-rw-r--r--   0        0        0      253 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/certificate_status.py
+-rw-r--r--   0        0        0      279 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/colors.py
+-rw-r--r--   0        0        0      239 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/exceptions.py
+-rw-r--r--   0        0        0      320 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/__init__.py
+-rw-r--r--   0        0        0     3433 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/aaa.py
+-rw-r--r--   0        0        0     5810 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/appqoe.py
+-rw-r--r--   0        0        0      784 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/banner.py
+-rw-r--r--   0        0        0      268 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/base.py
+-rw-r--r--   0        0        0     3283 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/basic.py
+-rw-r--r--   0        0        0      898 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/bfd.py
+-rw-r--r--   0        0        0     4591 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/bgp.py
+-rw-r--r--   0        0        0     1520 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/cellular_controller.py
+-rw-r--r--   0        0        0     3269 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/cellular_profile.py
+-rw-r--r--   0        0        0      756 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/cli.py
+-rw-r--r--   0        0        0     1932 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/cloud_credentials.py
+-rw-r--r--   0        0        0     4387 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/dhcp.py
+-rw-r--r--   0        0        0     5349 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/eigrp.py
+-rw-r--r--   0        0        0     6240 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/ethernet.py
+-rw-r--r--   0        0        0      578 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/global_.py
+-rw-r--r--   0        0        0     1573 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/gps.py
+-rw-r--r--   0        0        0      331 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/helpers.py
+-rw-r--r--   0        0        0    12974 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/lan/ethernet.py
+-rw-r--r--   0        0        0     5619 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/lan/gre.py
+-rw-r--r--   0        0        0     5331 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/lan/ipsec.py
+-rw-r--r--   0        0        0     9349 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/lan/multilink.py
+-rw-r--r--   0        0        0     7411 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/lan/svi.py
+-rw-r--r--   0        0        0     1963 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/logging_.py
+-rw-r--r--   0        0        0     4855 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/model_definition_normalizer.py
+-rw-r--r--   0        0        0    13085 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/multicast.py
+-rw-r--r--   0        0        0     5329 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/normalizer.py
+-rw-r--r--   0        0        0     2295 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/ntp.py
+-rw-r--r--   0        0        0     1475 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/omp.py
+-rw-r--r--   0        0        0     5520 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/ospf.py
+-rw-r--r--   0        0        0    11012 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py
+-rw-r--r--   0        0        0     6200 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py
+-rw-r--r--   0        0        0     1568 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/security.py
+-rw-r--r--   0        0        0    10159 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/sig.py
+-rw-r--r--   0        0        0     2240 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/snmp.py
+-rw-r--r--   0        0        0     9032 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/switchport.py
+-rw-r--r--   0        0        0     2776 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py
+-rw-r--r--   0        0        0     2250 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/ucse.py
+-rw-r--r--   0        0        0    33006 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/vpn.py
+-rw-r--r--   0        0        0     5742 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/cellular.py
+-rw-r--r--   0        0        0    13158 2024-05-22 21:06:37.235814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/ethernet.py
+-rw-r--r--   0        0        0     4844 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/gre.py
+-rw-r--r--   0        0        0     6866 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/ipsec.py
+-rw-r--r--   0        0        0    14360 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/multilink.py
+-rw-r--r--   0        0        0    18190 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/protocol_over.py
+-rw-r--r--   0        0        0     5344 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/t1e1serial.py
+-rw-r--r--   0        0        0     8057 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py
+-rw-r--r--   0        0        0     2540 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/policy/policy_definitions.py
+-rw-r--r--   0        0        0     9564 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/converters/policy/policy_lists.py
+-rw-r--r--   0        0        0     6038 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/creators/config_pusher.py
+-rw-r--r--   0        0        0     5570 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/creators/strategy/parcels.py
+-rw-r--r--   0        0        0     1686 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/factories/feature_profile_api.py
+-rw-r--r--   0        0        0     1257 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/factories/parcel_pusher.py
+-rw-r--r--   0        0        0     1671 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/reverters/config_reverter.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/steps/__init__.py
+-rw-r--r--   0        0        0     3174 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/steps/constants.py
+-rw-r--r--   0        0        0     5979 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_migration/steps/transform.py
+-rw-r--r--   0        0        0      154 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/config_status.py
+-rw-r--r--   0        0        0     4778 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/creation_tools.py
+-rw-r--r--   0        0        0     7281 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/dashboard.py
+-rw-r--r--   0        0        0     2863 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/device_model.py
+-rw-r--r--   0        0        0     2110 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/dict.py
+-rw-r--r--   0        0        0      953 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/feature_template/choose_model.py
+-rw-r--r--   0        0        0     4882 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/feature_template/find_template_values.py
+-rw-r--r--   0        0        0      584 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/operation_status.py
+-rw-r--r--   0        0        0      196 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/personality.py
+-rw-r--r--   0        0        0      360 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/pydantic_field.py
+-rw-r--r--   0        0        0      172 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/reachability.py
+-rw-r--r--   0        0        0      407 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/session_type.py
+-rw-r--r--   0        0        0      149 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/template_type.py
+-rw-r--r--   0        0        0     9825 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/timezone.py
+-rw-r--r--   0        0        0     3930 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/upgrades_helper.py
+-rw-r--r--   0        0        0      159 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/utils/validate_status.py
+-rw-r--r--   0        0        0     3032 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/version.py
+-rw-r--r--   0        0        0     5415 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/vmanage_auth.py
+-rw-r--r--   0        0        0    15970 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/workflows/config_migration.py
+-rw-r--r--   0        0        0     9946 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/catalystwan/workflows/tenant_migration.py
+-rw-r--r--   0        0        0      866 2024-05-22 21:06:37.239814 catalystwan-0.33.7.dev0/pyproject.toml
+-rw-r--r--   0        0        0    18717 1970-01-01 00:00:00.000000 catalystwan-0.33.7.dev0/setup.py
+-rw-r--r--   0        0        0    14665 1970-01-01 00:00:00.000000 catalystwan-0.33.7.dev0/PKG-INFO
```

### Comparing `catalystwan-0.33.7/LICENSE` & `catalystwan-0.33.7.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/README.md` & `catalystwan-0.33.7.dev0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -178,30 +178,28 @@
 n = 24
 alarms_from_n_hours = session.api.alarms.get(from_time=n)
 ```
 
 To get all critical alarms from past `n` hours:
 
 ```python
-from catalystwan.utils.alarm_status import Severity
 n = 48
 critical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)
 ```
 
 </details>
 
 <details>
     <summary> <b>Users</b> <i>(click to expand)</i></summary>
 
 ```python
 # Get all users
 session.api.users.get()
 
 # Create user
-from catalystwan.endpoints.administration_user_and_group import User
 new_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")
 session.api.users.create(new_user)
 
 # Update user data
 new_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")
 session.api.users.update(new_user_update)
```

#### html2text {}

```diff
@@ -72,20 +72,18 @@
 session.api.repository.upload_image(image) # Install software install_task =
 session.api.software.install(devices=vsmarts, image=image) # Check action
 status install_task.wait_for_completed() ``` GGeett aallaarrmmss (click to expand) To
 get all alarms: ```python alarms = session.api.alarms.get() ``` To get all not
 viewed alarms: ```python not_viewed_alarms = session.api.alarms.get().filter
 (viewed=False) ``` To get all alarms from past `n` hours: ```python n = 24
 alarms_from_n_hours = session.api.alarms.get(from_time=n) ``` To get all
-critical alarms from past `n` hours: ```python from
-catalystwan.utils.alarm_status import Severity n = 48 critical_alarms =
+critical alarms from past `n` hours: ```python n = 48 critical_alarms =
 session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL) ```
 UUsseerrss (click to expand) ```python # Get all users session.api.users.get() #
-Create user from catalystwan.endpoints.administration_user_and_group import
-User new_user = User(username="new_user", password="new_user", group=
+Create user new_user = User(username="new_user", password="new_user", group=
 ["netadmin"], description="new user") session.api.users.create(new_user) #
 Update user data new_user_update = UserUpdateRequest(username="new_user",
 group=["netadmin", "netops"], locale="en_US", description="updated-new_user-
 description") session.api.users.update(new_user_update) # Update user password
 session.api.users.update_password("new_user", "n3W-P4s$w0rd") # Reset user
 session.api.users.reset("new_user") # Delete user session.api.users.delete
 ("new_user") # Get current user authentication type and role
```

### Comparing `catalystwan-0.33.7/catalystwan/__init__.py` & `catalystwan-0.33.7.dev0/catalystwan/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from os import environ
 from pathlib import Path
 from traceback import FrameSummary, StackSummary, extract_stack
 from typing import Callable, Final, List, Optional
 
 import urllib3
 
-USER_AGENT = f"{__package__}/{metadata.version(__package__)}"
+PACKAGE_VERSION = metadata.version(__package__)
+USER_AGENT = f"{__package__}/{PACKAGE_VERSION}"
 
 
 def with_proc_info_header(method: Callable[..., str]) -> Callable[..., str]:
     """
     Adds process ID and external caller information before first line of returned string
     """
```

### Comparing `catalystwan-0.33.7/catalystwan/abstractions.py` & `catalystwan-0.33.7.dev0/catalystwan/abstractions.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,9 +50,9 @@
         ...
 
     @property
     def session_type(self) -> Optional[SessionType]:
         ...
 
     @property
-    def validate_responses(self) -> bool:
+    def validate_response(self) -> bool:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/api/admin_tech_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/administration.py` & `catalystwan-0.33.7.dev0/catalystwan/api/administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/alarms_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/api_container.py` & `catalystwan-0.33.7.dev0/catalystwan/api/api_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,32 +11,32 @@
     ResourceGroupsAPI,
     SessionsAPI,
     UserGroupsAPI,
     UsersAPI,
 )
 from catalystwan.api.alarms_api import AlarmsAPI
 from catalystwan.api.basic_api import DevicesAPI, DeviceStateAPI
+from catalystwan.api.builders import BuilderAPI
 from catalystwan.api.config_device_inventory_api import ConfigurationDeviceInventoryAPI
 from catalystwan.api.config_group_api import ConfigGroupAPI
 from catalystwan.api.dashboard_api import DashboardAPI
-from catalystwan.api.feature_profile_api import SDRoutingFeatureProfilesAPI
+from catalystwan.api.feature_profile_api import SDRoutingFeatureProfilesAPI, SDWANFeatureProfilesAPI
 from catalystwan.api.logs_api import LogsAPI
 from catalystwan.api.omp_api import OmpAPI
 from catalystwan.api.packet_capture_api import PacketCaptureAPI
 from catalystwan.api.partition_manager_api import PartitionManagerAPI
 from catalystwan.api.policy_api import PolicyAPI
 from catalystwan.api.resource_pool_api import ResourcePoolAPI
 from catalystwan.api.software_action_api import SoftwareActionAPI
 from catalystwan.api.speedtest_api import SpeedtestAPI
 from catalystwan.api.template_api import TemplatesAPI
 from catalystwan.api.tenant_backup_restore_api import TenantBackupRestoreAPI
 from catalystwan.api.tenant_management_api import TenantManagementAPI
 from catalystwan.api.tenant_migration_api import TenantMigrationAPI
 from catalystwan.api.versions_utils import RepositoryAPI
-from catalystwan.api.virtual_image_action_api import LxcActionAPI
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
 
 class APIContainer:
     def __init__(self, session: ManagerSession):
@@ -55,16 +55,17 @@
         self.speedtest = SpeedtestAPI(session)
         self.templates = TemplatesAPI(session)
         self.tenant_backup = TenantBackupRestoreAPI(session)
         self.tenant_migration = TenantMigrationAPI(session)
         self.repository = RepositoryAPI(session)
         self.resource_pool = ResourcePoolAPI(session)
         self.software = SoftwareActionAPI(session)
-        self.lxcsoftware = LxcActionAPI(session)
         self.partition = PartitionManagerAPI(session)
         self.users = UsersAPI(session)
         self.cluster_management = ClusterManagementAPI(session)
         self.user_groups = UserGroupsAPI(session)
         self.resource_groups = ResourceGroupsAPI(session)
         self.sessions = SessionsAPI(session)
         self.policy = PolicyAPI(session)
         self.sd_routing_feature_profiles = SDRoutingFeatureProfilesAPI(session)
+        self.sdwan_feature_profiles = SDWANFeatureProfilesAPI(session)
+        self.builders = BuilderAPI(session)
```

### Comparing `catalystwan-0.33.7/catalystwan/api/basic_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/basic_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/config_device_inventory_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/config_device_inventory_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/config_group_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/config_group_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,139 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Optional, overload
+from uuid import UUID
+
+from catalystwan.typed_list import DataSequence
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
 from catalystwan.endpoints.configuration_group import (
+    ConfigGroup,
     ConfigGroupAssociatePayload,
     ConfigGroupCreationPayload,
     ConfigGroupCreationResponse,
     ConfigGroupDeployPayload,
     ConfigGroupDeployResponse,
     ConfigGroupDisassociateResponse,
     ConfigGroupEditPayload,
     ConfigGroupEditResponse,
-    ConfigGroupResponsePayload,
     ConfigGroupVariablesCreatePayload,
     ConfigGroupVariablesCreateResponse,
     ConfigGroupVariablesEditPayload,
     ConfigurationGroup,
     DeviceId,
     ProfileId,
     Solution,
 )
 
 
 class ConfigGroupAPI:
     def __init__(self, session: ManagerSession):
-        self.session = session
-        self.endpoint = ConfigurationGroup(session)
+        self._session = session
+        self._endpoints = ConfigurationGroup(session)
 
     def associate(self, cg_id: str, device_ids: list) -> None:
         """
         Associates given config-group to specified list of devices
         """
         devices = []
 
         for device_id in device_ids:
             devices.append(DeviceId(id=device_id))
 
         payload = ConfigGroupAssociatePayload(devices=devices)
 
-        self.endpoint.associate(config_group_id=cg_id, payload=payload)
+        self._endpoints.associate(config_group_id=cg_id, payload=payload)
 
     def create(self, name: str, description: str, solution: Solution, profile_ids: list) -> ConfigGroupCreationResponse:
         """
         Creates new config-group
         """
         profiles = []
 
         for profile_id in profile_ids:
             profiles.append(ProfileId(id=profile_id))
         cg_payload = ConfigGroupCreationPayload(
             name=name, description=description, solution=solution, profiles=profiles
         )
 
-        return self.endpoint.create_config_group(cg_payload)
+        return self._endpoints.create_config_group(cg_payload)
 
     def create_variables(
         self, cg_id: str, device_ids: list, suggestions: bool = True
     ) -> ConfigGroupVariablesCreateResponse:
         """
         Creates device specific variable data in given config-group
         """
         payload = ConfigGroupVariablesCreatePayload(deviceIds=device_ids, suggestions=suggestions)
-        return self.endpoint.create_variables(config_group_id=cg_id, payload=payload)
+        return self._endpoints.create_variables(config_group_id=cg_id, payload=payload)
 
-    def delete(self, cg_id: str) -> None:
+    def delete(self, cg_id: UUID) -> None:
         """
         Deletes existing config-group with given ID
         """
-        self.endpoint.delete_config_group(cg_id)
+        self._endpoints.delete_config_group(cg_id)
 
     def deploy(self, cg_id: str, device_ids: list) -> ConfigGroupDeployResponse:
         """
         Deploys specified config-group config to given list of devices
         """
         devices = []
         for device_id in device_ids:
             devices.append(DeviceId(id=device_id))
 
         payload = ConfigGroupDeployPayload(devices=devices)
-        return self.endpoint.deploy(config_group_id=cg_id, payload=payload)
+        return self._endpoints.deploy(config_group_id=cg_id, payload=payload)
 
     def disassociate(self, cg_id: str, device_ids: list) -> ConfigGroupDisassociateResponse:
         """
         Disassociates given list of devices from the specified config-group
         """
         devices = []
         for device_id in device_ids:
             devices.append(DeviceId(id=device_id))
 
         payload = ConfigGroupAssociatePayload(devices=devices)
-        return self.endpoint.disassociate(config_group_id=cg_id, payload=payload)
+        return self._endpoints.disassociate(config_group_id=cg_id, payload=payload)
 
     def edit(
         self, cg_id: str, name: str, description: str, solution: Solution, profile_ids: list
     ) -> ConfigGroupEditResponse:
         """
         Modifies feature profiles in existing config-group
         """
         profiles = []
 
         for profile_id in profile_ids:
             profiles.append(ProfileId(id=profile_id))
         payload = ConfigGroupEditPayload(name=name, description=description, solution=solution, profiles=profiles)
 
-        return self.endpoint.edit_config_group(config_group_id=cg_id, payload=payload)
+        return self._endpoints.edit_config_group(config_group_id=cg_id, payload=payload)
+
+    @overload
+    def get(self) -> DataSequence[ConfigGroup]:
+        ...
+
+    @overload
+    def get(self, group_id: UUID) -> ConfigGroup:
+        ...
 
-    def get(self) -> ConfigGroupResponsePayload:
+    def get(self, group_id: Optional[UUID] = None) -> Any:
         """
-        Gets list of existing config-groups
+        Gets list of existing config-groups or single config-group with given ID
+        If given ID is not correct return None
         """
-        return self.endpoint.get()
+        if group_id is None:
+            return self._endpoints.get()
+        return self._endpoints.get().filter(id=group_id).single_or_default()
 
     def update_variables(self, cg_id: str, solution: Solution, device_variables: list) -> None:
         """
         Updates device specific variable data in given config-group
         """
         payload = ConfigGroupVariablesEditPayload(solution=solution, devices=device_variables)
 
-        self.endpoint.update_variables(config_group_id=cg_id, payload=payload)
+        self._endpoints.update_variables(config_group_id=cg_id, payload=payload)
```

### Comparing `catalystwan-0.33.7/catalystwan/api/configuration_groups/parcel.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,139 +1,112 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from enum import Enum
-from typing import Any, Dict, Generic, Literal, Optional, TypeVar, get_origin
+from typing import List, Literal, Optional, Union
 
-from pydantic import AliasPath, BaseModel, ConfigDict, Field, PrivateAttr, model_serializer
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-T = TypeVar("T")
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default
+from catalystwan.models.common import Duplex, Speed
 
 
-class _ParcelBase(BaseModel):
-    model_config = ConfigDict(extra="forbid", arbitrary_types_allowed=True, populate_by_name=True)
-    parcel_name: str = Field(
-        min_length=1,
-        max_length=128,
-        pattern=r'^[^&<>! "]+$',
-        serialization_alias="name",
-        validation_alias="name",
-    )
-    parcel_description: Optional[str] = Field(
-        default=None,
-        serialization_alias="description",
-        validation_alias="description",
-        description="Set the parcel description",
-    )
-    data: Optional[Any] = None
-    _parcel_data_key: str = PrivateAttr(default="data")
-
-    @model_serializer(mode="wrap")
-    def envelope_parcel_data(self, handler) -> Dict[str, Any]:
-        model_dict = handler(self)
-        model_dict[self._parcel_data_key] = {}
-        remove_keys = []
-
-        for key in model_dict.keys():
-            field_info = self.model_fields.get(key)
-            if field_info and isinstance(field_info.validation_alias, AliasPath):
-                aliases = field_info.validation_alias.convert_to_aliases()
-                if aliases and aliases[0] == self._parcel_data_key and len(aliases) == 2:
-                    model_dict[self._parcel_data_key][aliases[1]] = model_dict[key]
-                    remove_keys.append(key)
-        for key in remove_keys:
-            del model_dict[key]
-        return model_dict
-
+class StaticMacAddress(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-class OptionType(str, Enum):
-    GLOBAL = "global"
-    DEFAULT = "default"
-    VARIABLE = "variable"
-
-
-class ParcelAttribute(BaseModel):
-    model_config = ConfigDict(extra="forbid")
-    option_type: OptionType = Field(serialization_alias="optionType", validation_alias="optionType")
-
-
-# https://github.com/pydantic/pydantic/discussions/6090
-# Usage: Global[str](value="test")
-class Global(ParcelAttribute, Generic[T]):
-    option_type: OptionType = Field(
-        default=OptionType.GLOBAL, serialization_alias="optionType", validation_alias="optionType"
+    mac_address: Union[Global[str], Variable] = Field(serialization_alias="macaddr", validation_alias="macaddr")
+    vlan: Union[Global[int], Variable]
+    interface_name: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="ifName", validation_alias="ifName", default=None
     )
-    value: T
-
-    def __len__(self) -> int:
-        if isinstance(self.value, (str, list)):
-            return len(self.value)
-        return -1
 
-    def __ge__(self, other: Any) -> bool:
-        if isinstance(self.value, int):
-            return self.value >= other
-        return False
 
-    def __le__(self, other: Any) -> bool:
-        if isinstance(self.value, int):
-            return self.value <= other
-        return False
-
-
-class Variable(ParcelAttribute):
-    option_type: OptionType = Field(
-        default=OptionType.VARIABLE, serialization_alias="optionType", validation_alias="optionType"
+SwitchportMode = Literal[
+    "access",
+    "trunk",
+]
+
+
+PortControl = Literal[
+    "auto",
+    "force-unauthorized",
+    "force-authorized",
+]
+
+HostMode = Literal[
+    "single-host",
+    "multi-auth",
+    "multi-host",
+    "multi-domain",
+]
+
+ControlDirection = Literal[
+    "both",
+    "in",
+]
+
+
+class SwitchportInterface(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    interface_name: Union[Global[str], Variable] = Field(serialization_alias="ifName", validation_alias="ifName")
+    mode: Global[SwitchportMode] = as_default("access", SwitchportMode)
+    shutdown: Union[Global[bool], Variable, Default[bool]] = Default[bool](value=True)
+    speed: Union[Global[Speed], Variable, Default[None]] = Default[None](value=None)
+    duplex: Union[Global[Duplex], Variable, Default[None]] = Default[None](value=None)
+    switchport_access_vlan: Union[Global[int], Variable, Default[None]] = Field(
+        serialization_alias="switchportAccessVlan",
+        validation_alias="switchportAccessVlan",
+        default=Default[None](value=None),
     )
-    value: str = Field(pattern=r"^\{\{[.\/\[\]a-zA-Z0-9_-]+\}\}$", min_length=1, max_length=64)
-
-
-class Default(ParcelAttribute, Generic[T]):
-    option_type: OptionType = Field(
-        default=OptionType.DEFAULT, serialization_alias="optionType", validation_alias="optionType"
+    switchport_trunk_allowed_vlans: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="switchportTrunkAllowedVlans", validation_alias="switchportTrunkAllowedVlans", default=None
+    )
+    switchport_trunk_native_vlan: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="switchportTrunkNativeVlan", validation_alias="switchportTrunkNativeVlan", default=None
+    )
+    port_control: Optional[Union[Global[PortControl], Variable, Default[None]]] = Field(
+        serialization_alias="portControl", validation_alias="portControl", default=None
+    )
+    voice_vlan: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="voiceVlan", validation_alias="voiceVlan", default=None
+    )
+    pae_enable: Optional[Union[Global[bool], Variable, Default[None]]] = Field(
+        serialization_alias="paeEnable", validation_alias="paeEnable", default=None
+    )
+    mac_authentication_bypass: Optional[Union[Global[bool], Variable, Default[None]]] = Field(
+        serialization_alias="macAuthenticationBypass", validation_alias="macAuthenticationBypass", default=None
+    )
+    host_mode: Optional[Union[Global[HostMode], Variable, Default[None]]] = Field(
+        serialization_alias="hostMode", validation_alias="hostMode", default=None
+    )
+    enable_periodic_reauth: Optional[Union[Global[bool], Variable, Default[None]]] = Field(
+        serialization_alias="enablePeriodicReauth", validation_alias="enablePeriodicReauth", default=None
+    )
+    inactivity: Union[Global[int], Variable, Default[None]] = Default[None](value=None)
+    reauthentication: Union[Global[int], Variable, Default[int]] = as_default(3600)
+    control_direction: Optional[Union[Global[ControlDirection], Variable, Default[None]]] = Field(
+        serialization_alias="controlDirection", validation_alias="controlDirection", default=None
+    )
+    restricted_vlan: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="restrictedVlan", validation_alias="restrictedVlan", default=None
+    )
+    guest_vlan: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="guestVlan", validation_alias="guestVlan", default=None
+    )
+    critical_vlan: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="criticalVlan", validation_alias="criticalVlan", default=None
+    )
+    enable_voice: Optional[Union[Global[bool], Variable, Default[None]]] = Field(
+        serialization_alias="enableVoice", validation_alias="enableVoice", default=None
     )
-    value: Any
-
-
-def as_global(value: Any, generic_alias: Any = None):
-    """Produces Global object given only value (type is induced from value)
-
-    Args:
-        value (Any): value of Global object to be produced
-        generic_alias (Any, optional): specify alias type like Literal. Defaults to None.
-
-    Returns:
-        Global[Any]: global option type object
-    """
-    if generic_alias is None:
-        return Global[type(value)](value=value)  # type: ignore
-    elif get_origin(generic_alias) is Literal:
-        return Global[generic_alias](value=value)  # type: ignore
-    TypeError("Inappropriate type for argument generic_alias")
-
-
-def as_variable(value: str):
-    """Produces Variable object from variable name string
-
-    Args:
-        value (str): value of Variable object to be produced
-
-    Returns:
-        Variable: variable option type object
-    """
-    return Variable(value=value)
-
-
-def as_default(value: Any, generic_alias: Any = None):
-    """Produces Default object given only value (type is induced from value)
 
-    Args:
-        value (Any): value of Default object to be produced
-        generic_alias (Any, optional): specify alias type like Literal. Defaults to None.
 
-    Returns:
-        Default[Any]: default option type object
-    """
-    if generic_alias is None:
-        return Default[type(value)](value=value)  # type: ignore
-    elif get_origin(generic_alias) is Literal:
-        return Default[generic_alias](value=value)  # type: ignore
-    TypeError("Inappropriate type for argument generic_alias")
+class SwitchportParcel(_ParcelBase):
+    type_: Literal["switchport"] = Field(default="switchport", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    interface: List[SwitchportInterface] = Field(default_factory=list, validation_alias=AliasPath("data", "interface"))
+    age_time: Union[Global[int], Variable, Default[int]] = Field(
+        default=Default[int](value=300), validation_alias=AliasPath("data", "ageTime")
+    )
+    static_mac_address: List[StaticMacAddress] = Field(
+        default_factory=list, validation_alias=AliasPath("data", "staticMacAddress")
+    )
```

### Comparing `catalystwan-0.33.7/catalystwan/api/dashboard_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/dashboard_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/device_action_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/logs_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/monitoring_status_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/mtt_aaa_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/omp_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/packet_capture_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/packet_capture_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/parcel_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/parcel_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/partition_manager_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/policy_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/policy_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,73 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Type, overload
+from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Tuple, Type, overload
 from uuid import UUID
 
 from catalystwan.api.task_status_api import Task
-from catalystwan.endpoints.configuration.policy.definition.access_control_list import (
-    AclPolicyGetResponse,
-    ConfigurationPolicyAclDefinition,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints, PolicyListEndpoints
+from catalystwan.endpoints.configuration.policy.definition.access_control_list import ConfigurationPolicyAclDefinition
 from catalystwan.endpoints.configuration.policy.definition.access_control_list_ipv6 import (
-    AclIPv6PolicyGetResponse,
     ConfigurationPolicyAclIPv6Definition,
 )
-from catalystwan.endpoints.configuration.policy.definition.control import (
-    ConfigurationPolicyControlDefinition,
-    ControlPolicyGetResponse,
-)
+from catalystwan.endpoints.configuration.policy.definition.aip import ConfigurationPolicyAIPDefinition
+from catalystwan.endpoints.configuration.policy.definition.amp import ConfigurationPolicyAMPDefinition
+from catalystwan.endpoints.configuration.policy.definition.cflowd import ConfigurationPolicyCflowdDefinition
+from catalystwan.endpoints.configuration.policy.definition.control import ConfigurationPolicyControlDefinition
 from catalystwan.endpoints.configuration.policy.definition.device_access import (
     ConfigurationPolicyDeviceAccessDefinition,
-    DeviceAccessPolicyGetResponse,
 )
 from catalystwan.endpoints.configuration.policy.definition.device_access_ipv6 import (
     ConfigurationPolicyDeviceAccessIPv6Definition,
-    DeviceAccessIPv6PolicyGetResponse,
-)
-from catalystwan.endpoints.configuration.policy.definition.hub_and_spoke import (
-    ConfigurationPolicyHubAndSpokeDefinition,
-    HubAndSpokePolicyGetResponse,
-)
-from catalystwan.endpoints.configuration.policy.definition.mesh import (
-    ConfigurationPolicyMeshDefinition,
-    MeshPolicyGetResponse,
-)
-from catalystwan.endpoints.configuration.policy.definition.qos_map import (
-    ConfigurationPolicyQoSMapDefinition,
-    QoSMapPolicyGetResponse,
-)
-from catalystwan.endpoints.configuration.policy.definition.rewrite import (
-    ConfigurationPolicyRewriteRuleDefinition,
-    RewritePolicyGetResponse,
-)
-from catalystwan.endpoints.configuration.policy.definition.rule_set import (
-    ConfigurationPolicyRuleSetDefinition,
-    RuleSetGetResponse,
 )
+from catalystwan.endpoints.configuration.policy.definition.dns_security import ConfigurationPolicyDnsSecurityDefinition
+from catalystwan.endpoints.configuration.policy.definition.hub_and_spoke import ConfigurationPolicyHubAndSpokeDefinition
+from catalystwan.endpoints.configuration.policy.definition.intrusion_prevention import (
+    ConfigurationPolicyIntrusionPreventionDefinition,
+)
+from catalystwan.endpoints.configuration.policy.definition.mesh import ConfigurationPolicyMeshDefinition
+from catalystwan.endpoints.configuration.policy.definition.qos_map import ConfigurationPolicyQoSMapDefinition
+from catalystwan.endpoints.configuration.policy.definition.rewrite import ConfigurationPolicyRewriteRuleDefinition
+from catalystwan.endpoints.configuration.policy.definition.route_policy import ConfigurationPolicyRouteDefinition
+from catalystwan.endpoints.configuration.policy.definition.rule_set import ConfigurationPolicyRuleSetDefinition
 from catalystwan.endpoints.configuration.policy.definition.security_group import (
     ConfigurationPolicySecurityGroupDefinition,
-    SecurityGroupGetResponse,
 )
-from catalystwan.endpoints.configuration.policy.definition.traffic_data import (
-    ConfigurationPolicyDataDefinition,
-    TrafficDataPolicy,
-    TrafficDataPolicyGetResponse,
+from catalystwan.endpoints.configuration.policy.definition.ssl_decryption import ConfigurationSslDecryptionDefinition
+from catalystwan.endpoints.configuration.policy.definition.ssl_decryption_utd_profile import (
+    ConfigurationSslDecryptionUtdProfileDefinition,
+)
+from catalystwan.endpoints.configuration.policy.definition.traffic_data import ConfigurationPolicyDataDefinition
+from catalystwan.endpoints.configuration.policy.definition.url_filtering import (
+    ConfigurationPolicyUrlFilteringDefinition,
 )
 from catalystwan.endpoints.configuration.policy.definition.vpn_membership import (
     ConfigurationPolicyVPNMembershipGroupDefinition,
-    VPNMembershipPolicyGetResponse,
 )
 from catalystwan.endpoints.configuration.policy.definition.zone_based_firewall import (
     ConfigurationPolicyZoneBasedFirewallDefinition,
-    ZoneBasedFWPolicyGetResponse,
 )
 from catalystwan.endpoints.configuration.policy.list.app import AppListInfo, ConfigurationPolicyApplicationList
-from catalystwan.endpoints.configuration.policy.list.app_probe import (
-    AppProbeClassListInfo,
-    ConfigurationPolicyAppProbeClassList,
-)
+from catalystwan.endpoints.configuration.policy.list.app_probe import ConfigurationPolicyAppProbeClassList
 from catalystwan.endpoints.configuration.policy.list.as_path import ASPathListInfo, ConfigurationPolicyASPathList
-from catalystwan.endpoints.configuration.policy.list.class_map import (
-    ClassMapListInfo,
-    ConfigurationPolicyForwardingClassList,
-)
+from catalystwan.endpoints.configuration.policy.list.class_map import ConfigurationPolicyForwardingClassList
 from catalystwan.endpoints.configuration.policy.list.color import ColorListInfo, ConfigurationPolicyColorList
-from catalystwan.endpoints.configuration.policy.list.community import (
-    CommunityListInfo,
-    ConfigurationPolicyCommunityList,
-)
-from catalystwan.endpoints.configuration.policy.list.data_ipv6_prefix import (
-    ConfigurationPolicyDataIPv6PrefixList,
-    DataIPv6PrefixListInfo,
-)
-from catalystwan.endpoints.configuration.policy.list.data_prefix import (
-    ConfigurationPolicyDataPrefixList,
-    DataPrefixListInfo,
-)
-from catalystwan.endpoints.configuration.policy.list.expanded_community import (
-    ConfigurationPolicyExpandedCommunityList,
-    ExpandedCommunityListInfo,
-)
+from catalystwan.endpoints.configuration.policy.list.community import ConfigurationPolicyCommunityList
+from catalystwan.endpoints.configuration.policy.list.data_ipv6_prefix import ConfigurationPolicyDataIPv6PrefixList
+from catalystwan.endpoints.configuration.policy.list.data_prefix import ConfigurationPolicyDataPrefixList
+from catalystwan.endpoints.configuration.policy.list.expanded_community import ConfigurationPolicyExpandedCommunityList
+from catalystwan.endpoints.configuration.policy.list.extended_community import ConfigurationPolicyExtendedCommunityList
 from catalystwan.endpoints.configuration.policy.list.fqdn import ConfigurationPolicyFQDNList, FQDNListInfo
-from catalystwan.endpoints.configuration.policy.list.geo_location import (
-    ConfigurationPolicyGeoLocationList,
-    GeoLocationListInfo,
-)
-from catalystwan.endpoints.configuration.policy.list.ips_signature import (
-    ConfigurationPolicyIPSSignatureList,
-    IPSSignatureListInfo,
-)
-from catalystwan.endpoints.configuration.policy.list.ipv6_prefix import (
-    ConfigurationPolicyIPv6PrefixList,
-    IPv6PrefixListInfo,
-)
+from catalystwan.endpoints.configuration.policy.list.geo_location import ConfigurationPolicyGeoLocationList
+from catalystwan.endpoints.configuration.policy.list.ips_signature import ConfigurationPolicyIPSSignatureList
+from catalystwan.endpoints.configuration.policy.list.ipv6_prefix import ConfigurationPolicyIPv6PrefixList
 from catalystwan.endpoints.configuration.policy.list.local_app import ConfigurationPolicyLocalAppList, LocalAppListInfo
-from catalystwan.endpoints.configuration.policy.list.local_domain import (
-    ConfigurationPolicyLocalDomainList,
-    LocalDomainListInfo,
-)
+from catalystwan.endpoints.configuration.policy.list.local_domain import ConfigurationPolicyLocalDomainList
 from catalystwan.endpoints.configuration.policy.list.mirror import ConfigurationPolicyMirrorList, MirrorListInfo
 from catalystwan.endpoints.configuration.policy.list.policer import ConfigurationPolicyPolicerClassList, PolicerListInfo
 from catalystwan.endpoints.configuration.policy.list.port import ConfigurationPolicyPortList, PortListInfo
 from catalystwan.endpoints.configuration.policy.list.preferred_color_group import (
     ConfigurationPreferredColorGroupList,
     PreferredColorGroupListInfo,
 )
@@ -119,15 +75,18 @@
 from catalystwan.endpoints.configuration.policy.list.protocol_name import (
     ConfigurationPolicyProtocolNameList,
     ProtocolNameListInfo,
 )
 from catalystwan.endpoints.configuration.policy.list.region import ConfigurationPolicyRegionList, RegionListInfo
 from catalystwan.endpoints.configuration.policy.list.site import ConfigurationPolicySiteList, SiteListInfo
 from catalystwan.endpoints.configuration.policy.list.sla import ConfigurationPolicySLAClassList, SLAClassListInfo
+from catalystwan.endpoints.configuration.policy.list.threat_grid_api_key import ConfigurationPolicyThreatGridApiKeyList
 from catalystwan.endpoints.configuration.policy.list.tloc import ConfigurationPolicyTLOCList, TLOCListInfo
+from catalystwan.endpoints.configuration.policy.list.trunkgroup import ConfigurationPolicyTrunkGroupList
+from catalystwan.endpoints.configuration.policy.list.umbrella_data import ConfigurationPolicyUmbrellaDataList
 from catalystwan.endpoints.configuration.policy.list.url_allow_list import (
     ConfigurationPolicyURLAllowList,
     URLAllowListInfo,
 )
 from catalystwan.endpoints.configuration.policy.list.url_block_list import (
     ConfigurationPolicyURLBlockList,
     URLBlockListInfo,
@@ -137,77 +96,118 @@
 from catalystwan.endpoints.configuration.policy.security_template import ConfigurationSecurityTemplatePolicy
 from catalystwan.endpoints.configuration.policy.vedge_template import ConfigurationVEdgeTemplatePolicy
 from catalystwan.endpoints.configuration.policy.vsmart_template import (
     ConfigurationVSmartTemplatePolicy,
     VSmartConnectivityStatus,
 )
 from catalystwan.models.misc.application_protocols import ApplicationProtocol
-from catalystwan.models.policy import AnyPolicyDefinition, AnyPolicyList
-from catalystwan.models.policy.centralized import CentralizedPolicy, CentralizedPolicyEditPayload, CentralizedPolicyInfo
-from catalystwan.models.policy.definitions.access_control_list import AclPolicy
-from catalystwan.models.policy.definitions.access_control_list_ipv6 import AclIPv6Policy
-from catalystwan.models.policy.definitions.control import ControlPolicy
-from catalystwan.models.policy.definitions.device_access import DeviceAccessPolicy
-from catalystwan.models.policy.definitions.device_access_ipv6 import DeviceAccessIPv6Policy
-from catalystwan.models.policy.definitions.hub_and_spoke import HubAndSpokePolicy
-from catalystwan.models.policy.definitions.mesh import MeshPolicy
-from catalystwan.models.policy.definitions.qos_map import QoSMapPolicy
-from catalystwan.models.policy.definitions.rewrite import RewritePolicy
-from catalystwan.models.policy.definitions.rule_set import RuleSet
-from catalystwan.models.policy.definitions.security_group import SecurityGroup
-from catalystwan.models.policy.definitions.vpn_membership import VPNMembershipPolicy
-from catalystwan.models.policy.definitions.zone_based_firewall import ZoneBasedFWPolicy
-from catalystwan.models.policy.lists import (
+from catalystwan.models.policy import (
+    AnyPolicyDefinition,
+    AnyPolicyList,
     AppList,
     AppProbeClassList,
     ASPathList,
     ClassMapList,
     ColorList,
     CommunityList,
     DataIPv6PrefixList,
     DataPrefixList,
     ExpandedCommunityList,
+    ExtendedCommunityList,
     FQDNList,
     GeoLocationList,
     IPSSignatureList,
     IPv6PrefixList,
     LocalAppList,
     LocalDomainList,
     MirrorList,
     PolicerList,
-    PolicyListBase,
     PortList,
     PreferredColorGroupList,
     PrefixList,
     ProtocolNameList,
     RegionList,
     SiteList,
     SLAClassList,
     TLOCList,
     URLAllowList,
     URLBlockList,
     VPNList,
     ZoneList,
 )
+from catalystwan.models.policy.centralized import CentralizedPolicy, CentralizedPolicyEditPayload, CentralizedPolicyInfo
+from catalystwan.models.policy.definition.access_control_list import AclPolicy, AclPolicyGetResponse
+from catalystwan.models.policy.definition.access_control_list_ipv6 import AclIPv6Policy, AclIPv6PolicyGetResponse
+from catalystwan.models.policy.definition.aip import (
+    AdvancedInspectionProfilePolicy,
+    AdvancedInspectionProfilePolicyGetResponse,
+)
+from catalystwan.models.policy.definition.amp import (
+    AdvancedMalwareProtectionPolicy,
+    AdvancedMalwareProtectionPolicyGetResponse,
+)
+from catalystwan.models.policy.definition.cflowd import CflowdPolicy, CflowdPolicyGetResponse
+from catalystwan.models.policy.definition.control import ControlPolicy, ControlPolicyGetResponse
+from catalystwan.models.policy.definition.device_access import DeviceAccessPolicy, DeviceAccessPolicyGetResponse
+from catalystwan.models.policy.definition.device_access_ipv6 import (
+    DeviceAccessIPv6Policy,
+    DeviceAccessIPv6PolicyGetResponse,
+)
+from catalystwan.models.policy.definition.dns_security import DnsSecurityPolicy, DnsSecurityPolicyGetResponse
+from catalystwan.models.policy.definition.hub_and_spoke import HubAndSpokePolicy, HubAndSpokePolicyGetResponse
+from catalystwan.models.policy.definition.intrusion_prevention import (
+    IntrusionPreventionPolicy,
+    IntrusionPreventionPolicyGetResponse,
+)
+from catalystwan.models.policy.definition.mesh import MeshPolicy, MeshPolicyGetResponse
+from catalystwan.models.policy.definition.qos_map import QoSMapPolicy, QoSMapPolicyGetResponse
+from catalystwan.models.policy.definition.rewrite import RewritePolicy, RewritePolicyGetResponse
+from catalystwan.models.policy.definition.route_policy import RoutePolicy, RoutePolicyGetResponse
+from catalystwan.models.policy.definition.rule_set import RuleSet, RuleSetGetResponse
+from catalystwan.models.policy.definition.security_group import SecurityGroup, SecurityGroupGetResponse
+from catalystwan.models.policy.definition.ssl_decryption import SslDecryptionPolicy, SslDecryptionPolicyGetResponse
+from catalystwan.models.policy.definition.ssl_decryption_utd_profile import (
+    SslDecryptionUtdProfilePolicy,
+    SslDecryptionUtdProfilePolicyGetResponse,
+)
+from catalystwan.models.policy.definition.traffic_data import TrafficDataPolicy, TrafficDataPolicyGetResponse
+from catalystwan.models.policy.definition.url_filtering import UrlFilteringPolicy, UrlFilteringPolicyGetResponse
+from catalystwan.models.policy.definition.vpn_membership import VPNMembershipPolicy, VPNMembershipPolicyGetResponse
+from catalystwan.models.policy.definition.zone_based_firewall import ZoneBasedFWPolicy, ZoneBasedFWPolicyGetResponse
+from catalystwan.models.policy.list.app_probe import AppProbeClassListInfo
+from catalystwan.models.policy.list.class_map import ClassMapListInfo
+from catalystwan.models.policy.list.communities import (
+    CommunityListInfo,
+    ExpandedCommunityListInfo,
+    ExtendedCommunityListInfo,
+)
+from catalystwan.models.policy.list.data_ipv6_prefix import DataIPv6PrefixListInfo
+from catalystwan.models.policy.list.data_prefix import DataPrefixListInfo
+from catalystwan.models.policy.list.geo_location import GeoLocationListInfo
+from catalystwan.models.policy.list.ips_signature import IPSSignatureListInfo
+from catalystwan.models.policy.list.ipv6_prefix import IPv6PrefixListInfo
+from catalystwan.models.policy.list.local_domain import LocalDomainListInfo
+from catalystwan.models.policy.list.threat_grid_api_key import ThreatGridApiKeyList, ThreatGridApiKeyListInfo
+from catalystwan.models.policy.list.trunkgroup import TrunkGroupList, TrunkGroupListInfo
+from catalystwan.models.policy.list.umbrella_data import UmbrellaDataList, UmbrellaDataListInfo
 from catalystwan.models.policy.localized import (
     LocalizedPolicy,
     LocalizedPolicyDeviceInfo,
     LocalizedPolicyEditResponse,
     LocalizedPolicyInfo,
 )
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionBase,
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
     PolicyDefinitionInfo,
 )
-from catalystwan.models.policy.policy_list import PolicyListEndpoints
+from catalystwan.models.policy.policy_list import PolicyListBase
 from catalystwan.models.policy.security import (
     AnySecurityPolicy,
-    AnySecurityPolicyInfo,
+    AnySecurityPolicyInfoList,
     SecurityPolicy,
     SecurityPolicyEditResponse,
     UnifiedSecurityPolicy,
 )
 from catalystwan.typed_list import DataSequence
 
 if TYPE_CHECKING:
@@ -220,14 +220,15 @@
     ASPathList: ConfigurationPolicyASPathList,
     ClassMapList: ConfigurationPolicyForwardingClassList,
     ColorList: ConfigurationPolicyColorList,
     CommunityList: ConfigurationPolicyCommunityList,
     DataIPv6PrefixList: ConfigurationPolicyDataIPv6PrefixList,
     DataPrefixList: ConfigurationPolicyDataPrefixList,
     ExpandedCommunityList: ConfigurationPolicyExpandedCommunityList,
+    ExtendedCommunityList: ConfigurationPolicyExtendedCommunityList,
     FQDNList: ConfigurationPolicyFQDNList,
     GeoLocationList: ConfigurationPolicyGeoLocationList,
     IPSSignatureList: ConfigurationPolicyIPSSignatureList,
     IPv6PrefixList: ConfigurationPolicyIPv6PrefixList,
     LocalAppList: ConfigurationPolicyLocalAppList,
     LocalDomainList: ConfigurationPolicyLocalDomainList,
     MirrorList: ConfigurationPolicyMirrorList,
@@ -235,15 +236,18 @@
     PortList: ConfigurationPolicyPortList,
     PreferredColorGroupList: ConfigurationPreferredColorGroupList,
     PrefixList: ConfigurationPolicyPrefixList,
     ProtocolNameList: ConfigurationPolicyProtocolNameList,
     RegionList: ConfigurationPolicyRegionList,
     SiteList: ConfigurationPolicySiteList,
     SLAClassList: ConfigurationPolicySLAClassList,
+    ThreatGridApiKeyList: ConfigurationPolicyThreatGridApiKeyList,
     TLOCList: ConfigurationPolicyTLOCList,
+    TrunkGroupList: ConfigurationPolicyTrunkGroupList,
+    UmbrellaDataList: ConfigurationPolicyUmbrellaDataList,
     URLBlockList: ConfigurationPolicyURLBlockList,
     URLAllowList: ConfigurationPolicyURLAllowList,
     VPNList: ConfigurationPolicyVPNList,
     ZoneList: ConfigurationPolicyZoneList,
 }
 
 POLICY_DEFINITION_ENDPOINTS_MAP: Mapping[type, type] = {
@@ -257,14 +261,23 @@
     VPNMembershipPolicy: ConfigurationPolicyVPNMembershipGroupDefinition,
     HubAndSpokePolicy: ConfigurationPolicyHubAndSpokeDefinition,
     MeshPolicy: ConfigurationPolicyMeshDefinition,
     AclPolicy: ConfigurationPolicyAclDefinition,
     AclIPv6Policy: ConfigurationPolicyAclIPv6Definition,
     DeviceAccessPolicy: ConfigurationPolicyDeviceAccessDefinition,
     DeviceAccessIPv6Policy: ConfigurationPolicyDeviceAccessIPv6Definition,
+    AdvancedInspectionProfilePolicy: ConfigurationPolicyAIPDefinition,
+    AdvancedMalwareProtectionPolicy: ConfigurationPolicyAMPDefinition,
+    IntrusionPreventionPolicy: ConfigurationPolicyIntrusionPreventionDefinition,
+    SslDecryptionPolicy: ConfigurationSslDecryptionDefinition,
+    SslDecryptionUtdProfilePolicy: ConfigurationSslDecryptionUtdProfileDefinition,
+    UrlFilteringPolicy: ConfigurationPolicyUrlFilteringDefinition,
+    DnsSecurityPolicy: ConfigurationPolicyDnsSecurityDefinition,
+    CflowdPolicy: ConfigurationPolicyCflowdDefinition,
+    RoutePolicy: ConfigurationPolicyRouteDefinition,
 }
 
 
 class CentralizedPolicyAPI:
     def __init__(self, session: ManagerSession):
         self._session = session
         self._endpoints = ConfigurationVSmartTemplatePolicy(session)
@@ -360,25 +373,25 @@
     def edit(self, id: UUID, policy: AnySecurityPolicy) -> SecurityPolicyEditResponse:
         return self._endpoints.edit_security_template(id, policy)
 
     def delete(self, id: UUID) -> None:
         self._endpoints.delete_security_template(id)
 
     @overload
-    def get(self) -> List[AnySecurityPolicyInfo]:
+    def get(self) -> AnySecurityPolicyInfoList:
         ...
 
     @overload
     def get(self, id: UUID) -> AnySecurityPolicy:
         ...
 
     def get(self, id: Optional[UUID] = None) -> Any:
         if id is not None:
             return self._endpoints.get_security_template(id).root
-        return [info.root for info in self._endpoints.generate_security_template_list()]
+        return self._endpoints.generate_security_template_list()
 
 
 class PolicyListsAPI:
     def __init__(self, session: ManagerSession):
         self._session = session
 
     def __get_list_endpoints_instance(self, payload_type: type) -> PolicyListEndpoints:
@@ -432,14 +445,18 @@
         ...
 
     @overload
     def get(self, type: Type[ExpandedCommunityList]) -> DataSequence[ExpandedCommunityListInfo]:
         ...
 
     @overload
+    def get(self, type: Type[ExtendedCommunityList]) -> DataSequence[ExtendedCommunityListInfo]:
+        ...
+
+    @overload
     def get(self, type: Type[FQDNList]) -> DataSequence[FQDNListInfo]:
         ...
 
     @overload
     def get(self, type: Type[GeoLocationList]) -> DataSequence[GeoLocationListInfo]:
         ...
 
@@ -492,18 +509,30 @@
         ...
 
     @overload
     def get(self, type: Type[SLAClassList]) -> DataSequence[SLAClassListInfo]:
         ...
 
     @overload
+    def get(self, type: Type[ThreatGridApiKeyList]) -> DataSequence[ThreatGridApiKeyListInfo]:
+        ...
+
+    @overload
     def get(self, type: Type[TLOCList]) -> DataSequence[TLOCListInfo]:
         ...
 
     @overload
+    def get(self, type: Type[TrunkGroupList]) -> DataSequence[TrunkGroupListInfo]:
+        ...
+
+    @overload
+    def get(self, type: Type[UmbrellaDataList]) -> DataSequence[UmbrellaDataListInfo]:
+        ...
+
+    @overload
     def get(self, type: Type[URLBlockList]) -> DataSequence[URLBlockListInfo]:
         ...
 
     @overload
     def get(self, type: Type[URLAllowList]) -> DataSequence[URLAllowListInfo]:
         ...
 
@@ -550,14 +579,18 @@
         ...
 
     @overload
     def get(self, type: Type[ExpandedCommunityList], id: UUID) -> ExpandedCommunityListInfo:
         ...
 
     @overload
+    def get(self, type: Type[ExtendedCommunityList], id: UUID) -> ExtendedCommunityListInfo:
+        ...
+
+    @overload
     def get(self, type: Type[FQDNList], id: UUID) -> FQDNListInfo:
         ...
 
     @overload
     def get(self, type: Type[GeoLocationList], id: UUID) -> GeoLocationListInfo:
         ...
 
@@ -610,18 +643,30 @@
         ...
 
     @overload
     def get(self, type: Type[SLAClassList], id: UUID) -> SLAClassListInfo:
         ...
 
     @overload
+    def get(self, type: Type[ThreatGridApiKeyList], id: UUID) -> ThreatGridApiKeyListInfo:
+        ...
+
+    @overload
     def get(self, type: Type[TLOCList], id: UUID) -> TLOCListInfo:
         ...
 
     @overload
+    def get(self, type: Type[TrunkGroupList], id: UUID) -> TrunkGroupListInfo:
+        ...
+
+    @overload
+    def get(self, type: Type[UmbrellaDataList], id: UUID) -> UmbrellaDataListInfo:
+        ...
+
+    @overload
     def get(self, type: Type[URLBlockList], id: UUID) -> URLBlockListInfo:
         ...
 
     @overload
     def get(self, type: Type[URLAllowList], id: UUID) -> URLAllowListInfo:
         ...
 
@@ -635,14 +680,20 @@
 
     def get(self, type: Type[AnyPolicyList], id: Optional[UUID] = None) -> Any:
         endpoints = self.__get_list_endpoints_instance(type)
         if id is not None:
             return endpoints.get_lists_by_id(id=id)
         return endpoints.get_policy_lists()
 
+    def get_all(self) -> List[AnyPolicyList]:
+        infos: List[AnyPolicyList] = []
+        for list_type, _ in POLICY_LIST_ENDPOINTS_MAP.items():
+            infos.extend(self.get(list_type))
+        return infos
+
 
 class PolicyDefinitionsAPI:
     def __init__(self, session: ManagerSession):
         self._session = session
 
     def __get_definition_endpoints_instance(self, payload_type: type) -> PolicyDefinitionEndpoints:
         endpoints_class = POLICY_DEFINITION_ENDPOINTS_MAP.get(payload_type)
@@ -659,26 +710,62 @@
         return endpoints.edit_policy_definition(id=id, payload=policy_definition)
 
     def delete(self, type: Type[AnyPolicyDefinition], id: UUID) -> None:
         endpoints = self.__get_definition_endpoints_instance(type)
         endpoints.delete_policy_definition(id=id)
 
     @overload
+    def get(self, type: Type[IntrusionPreventionPolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
     def get(self, type: Type[TrafficDataPolicy]) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
     @overload
+    def get(self, type: Type[UrlFilteringPolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
+    def get(self, type: Type[AdvancedInspectionProfilePolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
+    def get(self, type: Type[AdvancedMalwareProtectionPolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
+    def get(self, type: Type[CflowdPolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
+    def get(self, type: Type[DnsSecurityPolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
+    def get(self, type: Type[RoutePolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
     def get(self, type: Type[RuleSet]) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
     @overload
     def get(self, type: Type[SecurityGroup]) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
     @overload
+    def get(self, type: Type[SslDecryptionPolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
+    def get(self, type: Type[SslDecryptionUtdProfilePolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
     def get(self, type: Type[ZoneBasedFWPolicy]) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
     @overload
     def get(self, type: Type[QoSMapPolicy]) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
@@ -715,28 +802,63 @@
         ...
 
     @overload
     def get(self, type: Type[DeviceAccessIPv6Policy]) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
     # get by id
+    @overload
+    def get(self, type: Type[IntrusionPreventionPolicy], id: UUID) -> IntrusionPreventionPolicyGetResponse:
+        ...
 
     @overload
     def get(self, type: Type[TrafficDataPolicy], id: UUID) -> TrafficDataPolicyGetResponse:
         ...
 
     @overload
+    def get(self, type: Type[UrlFilteringPolicy], id: UUID) -> UrlFilteringPolicyGetResponse:
+        ...
+
+    @overload
+    def get(self, type: Type[AdvancedInspectionProfilePolicy], id: UUID) -> AdvancedInspectionProfilePolicyGetResponse:
+        ...
+
+    @overload
+    def get(self, type: Type[AdvancedMalwareProtectionPolicy], id: UUID) -> AdvancedMalwareProtectionPolicyGetResponse:
+        ...
+
+    @overload
+    def get(self, type: Type[CflowdPolicy], id: UUID) -> CflowdPolicyGetResponse:
+        ...
+
+    @overload
+    def get(self, type: Type[DnsSecurityPolicy], id: UUID) -> DnsSecurityPolicyGetResponse:
+        ...
+
+    @overload
+    def get(self, type: Type[RoutePolicy], id: UUID) -> RoutePolicyGetResponse:
+        ...
+
+    @overload
     def get(self, type: Type[RuleSet], id: UUID) -> RuleSetGetResponse:
         ...
 
     @overload
     def get(self, type: Type[SecurityGroup], id: UUID) -> SecurityGroupGetResponse:
         ...
 
     @overload
+    def get(self, type: Type[SslDecryptionPolicy], id: UUID) -> SslDecryptionPolicyGetResponse:
+        ...
+
+    @overload
+    def get(self, type: Type[SslDecryptionUtdProfilePolicy], id: UUID) -> SslDecryptionUtdProfilePolicyGetResponse:
+        ...
+
+    @overload
     def get(self, type: Type[ZoneBasedFWPolicy], id: UUID) -> ZoneBasedFWPolicyGetResponse:
         ...
 
     @overload
     def get(self, type: Type[QoSMapPolicy], id: UUID) -> QoSMapPolicyGetResponse:
         ...
 
@@ -778,14 +900,20 @@
 
     def get(self, type: Type[AnyPolicyDefinition], id: Optional[UUID] = None) -> Any:
         endpoints = self.__get_definition_endpoints_instance(type)
         if id is not None:
             return endpoints.get_policy_definition(id=id)
         return endpoints.get_definitions()
 
+    def get_all(self) -> List[Tuple[type, PolicyDefinitionInfo]]:
+        all_items: List[Tuple[type, PolicyDefinitionInfo]] = []
+        for definition_type, _ in POLICY_DEFINITION_ENDPOINTS_MAP.items():
+            all_items.extend([(definition_type, info) for info in self.get(definition_type)])
+        return all_items
+
 
 class PolicyAPI:
     """This is exposing so called 'UX 1.0' API"""
 
     def __init__(self, session: ManagerSession):
         self._session = session
         self.centralized = CentralizedPolicyAPI(session)
```

### Comparing `catalystwan-0.33.7/catalystwan/api/resource_pool_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/resource_pool_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/software_action_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/speedtest_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/speedtest_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/task_status_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/template_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/template_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from catalystwan.api.templates.models.cli_template import CliTemplateModel
 from catalystwan.api.templates.models.omp_vsmart_model import OMPvSmart
 from catalystwan.api.templates.models.security_vsmart_model import SecurityvSmart
 from catalystwan.api.templates.models.system_vsmart_model import SystemVsmart
 from catalystwan.dataclasses import Device, DeviceTemplateInfo, FeatureTemplateInfo, FeatureTemplatesTypes, TemplateInfo
 from catalystwan.endpoints.configuration_device_template import FeatureToCLIPayload
 from catalystwan.exceptions import AttachedError, TemplateNotFoundError
+from catalystwan.models.templates import DeviceTemplateInformation, FeatureTemplateInformation
 from catalystwan.response import ManagerResponse
 from catalystwan.typed_list import DataSequence
 from catalystwan.utils.device_model import DeviceModel
 from catalystwan.utils.dict import merge
 from catalystwan.utils.pydantic_field import get_extra_field
 from catalystwan.utils.template_type import TemplateType
 
@@ -694,7 +695,23 @@
         """
         encoded_uuid = device.uuid.replace("/", "%2F")
         endpoint = f"/dataservice/template/config/running/{encoded_uuid}"
         response = self.session.get_json(endpoint)
         config = CiscoConfParse(response["config"].splitlines())
         logger.debug(f"Template loaded from {device.hostname}.")
         return config
+
+    def get_feature_templates(self) -> DataSequence[FeatureTemplateInformation]:
+        endpoint = "/dataservice/template/feature"
+        fr_templates = self.session.get(endpoint)
+        return fr_templates.dataseq(FeatureTemplateInformation)
+
+    def get_device_templates(self) -> DataSequence[DeviceTemplateInformation]:
+        endpoint = "/dataservice/template/device"
+        params = {"feature": "all"}
+        templates = self.session.get(url=endpoint, params=params)
+        return templates.dataseq(DeviceTemplateInformation)
+
+    def get_device_template(self, template_id: str) -> DeviceTemplate:
+        endpoint = f"/dataservice/template/device/object/{template_id}"
+        response = self.session.get(endpoint)
+        return DeviceTemplate(**response.json())
```

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/README.md` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/cli_template.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/device_template/device_template.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/device_template/device_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
 import logging
 from pathlib import Path
-from typing import TYPE_CHECKING, Final, List
+from typing import TYPE_CHECKING, ClassVar, List
 
 from jinja2 import DebugUndefined, Environment, FileSystemLoader, meta  # type: ignore
 from pydantic import BaseModel, ConfigDict, Field, field_validator
 
-from catalystwan.utils.device_model import DeviceModel
-
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
 logger = logging.getLogger(__name__)
 
 
 class GeneralTemplate(BaseModel):
@@ -40,21 +38,25 @@
             template_name="python",
             template_description="python",
             general_templates=templates
         )
     >>> session.api.templates.create(device_template)
     """
 
-    template_name: str = Field(alias="templateName")
-    template_description: str = Field(alias="templateDescription")
-    general_templates: List[GeneralTemplate] = Field(alias="generalTemplates")
-    device_role: str = Field(default="sdwan-edge", alias="deviceRole")
-    device_type: DeviceModel = Field(alias="deviceType")
-    security_policy_id: str = Field(default="", alias="securityPolicyId")
-    policy_id: str = Field(default="", alias="policyId")
+    template_name: str = Field(serialization_alias="templateName", validation_alias="templateName")
+    template_description: str = Field(serialization_alias="templateDescription", validation_alias="templateDescription")
+    general_templates: List[GeneralTemplate] = Field(
+        default=[], serialization_alias="generalTemplates", validation_alias="generalTemplates"
+    )
+    device_role: str = Field(default="sdwan-edge", serialization_alias="deviceRole", validation_alias="deviceRole")
+    device_type: str = Field(serialization_alias="deviceType", validation_alias="deviceType")
+    security_policy_id: str = Field(
+        default="", serialization_alias="securityPolicyId", validation_alias="securityPolicyId"
+    )
+    policy_id: str = Field(default="", serialization_alias="policyId", validation_alias="policyId")
 
     def generate_payload(self) -> str:
         env = Environment(
             loader=FileSystemLoader(self.payload_path.parent),
             trim_blocks=True,
             lstrip_blocks=True,
             undefined=DebugUndefined,
@@ -75,15 +77,15 @@
         for template in value:
             if isinstance(template, str):
                 output.append(GeneralTemplate(name=template))
             else:
                 output.append(template)
         return output
 
-    payload_path: Final[Path] = Path(__file__).parent / "device_template_payload.json.j2"
+    payload_path: ClassVar[Path] = Path(__file__).parent / "device_template_payload.json.j2"
 
     @classmethod
     def get(self, name: str, session: ManagerSession) -> DeviceTemplate:
         device_template = session.api.templates.get(DeviceTemplate).filter(name=name).single_or_default()
         resp = session.get(f"dataservice/template/device/object/{device_template.id}").json()
         return DeviceTemplate(**resp)
```

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/device_template/device_template_payload.json.j2` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/device_template/device_template_payload.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/feature_template.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/feature_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/feature_template_field.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/feature_template_payload.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/feature_template_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_aaa_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_banner_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_banner_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_bfd_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_bfd_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_bgp_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_bgp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_logging_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_logging_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_ntp_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_ntp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_omp_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_omp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_ospf.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_ospfv3.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_secure_internet_gateway.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_secure_internet_gateway.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_snmp_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_snmp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_system.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_vpn_interface_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_vpn_interface_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_vpn_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/omp_vsmart_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/omp_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/security_vsmart_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/security_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/supported.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/supported.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/models/system_vsmart_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/models/system_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/aaa_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/aaa/aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/user.json.j2` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/aaa/feature/user.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/tenant/tenant.json.j2` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/tenant/tenant.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/templates/payloads/tenant/tenant_model.py` & `catalystwan-0.33.7.dev0/catalystwan/api/templates/payloads/tenant/tenant_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/tenant_backup_restore_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/tenant_management_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/tenant_migration_api.py` & `catalystwan-0.33.7.dev0/catalystwan/api/tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/api/versions_utils.py` & `catalystwan-0.33.7.dev0/catalystwan/api/versions_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,15 @@
 import logging
 from pathlib import PurePath
 from typing import TYPE_CHECKING, Dict, List, Union
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from catalystwan.endpoints.configuration.software_actions import SoftwareImageDetails
-from catalystwan.endpoints.configuration_device_actions import (
-    InstallLxcImage,
-    LxcActivateDevice,
-    LxcUpgradeDevice,
-    PartitionDevice,
-)
+from catalystwan.endpoints.configuration_device_actions import PartitionDevice
 from catalystwan.endpoints.configuration_device_inventory import DeviceDetailsResponse
 from catalystwan.exceptions import ImageNotInRepositoryError
 from catalystwan.typed_list import DataSequence
 from catalystwan.utils.upgrades_helper import SoftwarePackageUploadPayload
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
@@ -68,26 +63,14 @@
 
         Returns:
             list: software images list
         """
         software_images = self.session.endpoints.configuration_software_actions.get_list_of_all_images()
         return software_images
 
-    def get_all_virtual_images(self) -> DataSequence[SoftwareImageDetails]:
-        """
-        Get all info about all software images stored in Vmanage repository
-
-        Returns:
-            list: software images list
-        """
-        software_images = self.session.endpoints.configuration_software_actions.get_list_of_all_images(
-            "imageType=virtualmachine"
-        )
-        return software_images
-
     def get_devices_versions_repository(self) -> Dict[str, DeviceSoftwareRepository]:
         """
         Create DeviceSoftwareRepository dataclass,
         which cointains information about all possible version types for certain devices
 
         Returns:
             Dict[str, DeviceSoftwareRepository]: Dictionary containing all versions
@@ -222,62 +205,14 @@
             if not device.uuid or not device.local_system_ip:
                 raise ValueError(
                     f"Provided device '{device.host_name}' doesn't include required fields for this operation:"
                     f"device.uuid (current value: {device.uuid})"
                     f"device.device_ip (current value: {device.device_ip})"
                 )
 
-    def get_lxcactivate_device_list(
-        self,
-        version_to_set_up: str,
-        devices: DataSequence[DeviceDetailsResponse],
-    ) -> DataSequence[LxcActivateDevice]:
-        self._validate_devices_required_fields(devices)
-        install_image_payload = [
-            InstallLxcImage(
-                network_function_type="app-hosting",
-                version_name=version_to_set_up,
-                version_type_name="UTD-Snort-Feature",
-            )
-        ]
-        devices_payload = DataSequence(
-            LxcActivateDevice,
-            [
-                LxcActivateDevice(
-                    device_id=str(device.uuid),
-                    device_ip=str(device.local_system_ip),
-                    install_images=install_image_payload,
-                )
-                for device in devices
-            ],  # type: ignore
-        )
-
-        return devices_payload
-
-    def get_lxcupgrade_device_list(
-        self,
-        version_to_set_up: str,
-        devices: DataSequence[DeviceDetailsResponse],
-    ) -> DataSequence[LxcUpgradeDevice]:
-        self._validate_devices_required_fields(devices)
-        install_image_payload = [InstallLxcImage(version_name=version_to_set_up)]
-        devices_payload = DataSequence(
-            LxcUpgradeDevice,
-            [
-                LxcUpgradeDevice(
-                    device_id=str(device.uuid),
-                    device_ip=str(device.local_system_ip),
-                    install_images=install_image_payload,
-                )
-                for device in devices
-            ],  # type: ignore
-        )
-
-        return devices_payload
-
     def _get_device_list_in(
         self, version_to_set_up: str, devices: DataSequence[DeviceDetailsResponse], version_type: str
     ) -> DataSequence[PartitionDevice]:
         """
         Create devices payload list included requested version, if requested version
         is in specified version type
 
@@ -288,18 +223,16 @@
 
         Returns:
             list : list of devices
         """
         self._validate_devices_required_fields(devices)
         devices_payload = DataSequence(
             PartitionDevice,
-            [PartitionDevice(device_id=str(device.uuid), device_ip=str(device.local_system_ip)) for device in devices],
-            # type: ignore
+            [PartitionDevice(device_id=device.uuid, device_ip=device.device_ip) for device in devices],  # type: ignore
         )
-
         all_dev_versions = self.repository.get_devices_versions_repository()
         for device in devices_payload:
             device_versions = getattr(all_dev_versions[device.device_id], version_type)
             try:
                 for version in device_versions:
                     if version_to_set_up in version:
                         device.version = version
@@ -358,18 +291,17 @@
         Returns:
             list : list of devices
         """
         self._validate_devices_required_fields(devices)
 
         devices_payload = DataSequence(
             PartitionDevice,
-            [
-                PartitionDevice(device_id=device.uuid, device_ip=device.local_system_ip)  # type: ignore
-                for device in devices
-            ],  # type: ignore
+            [PartitionDevice(
+                device_id=device.uuid, device_ip=device.local_system_ip  # type: ignore
+            ) for device in devices],  # type: ignore
         )
         all_dev_versions = self.repository.get_devices_versions_repository()
         for device in devices_payload:
             device.version = getattr(all_dev_versions[device.device_id], version_type)
         return devices_payload
 
     def get_devices_current_version(
```

### Comparing `catalystwan-0.33.7/catalystwan/dataclasses.py` & `catalystwan-0.33.7.dev0/catalystwan/dataclasses.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/__init__.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     Literal,
     Mapping,
     Optional,
     Protocol,
     Sequence,
     Set,
     Tuple,
+    Type,
     TypeVar,
     Union,
     runtime_checkable,
 )
 from uuid import UUID
 
 from packaging.specifiers import SpecifierSet  # type: ignore
@@ -109,14 +110,53 @@
     def json(cls) -> TypeSpecifier:
         return TypeSpecifier(present=True, is_json=True)
 
     @classmethod
     def model_union(cls, models: Sequence[type]) -> TypeSpecifier:
         return TypeSpecifier(present=True, payload_union_model_types=models)
 
+    @classmethod
+    def resolve_nested_base_model_unions(
+        cls, annotation: Any, models_types: List[Type[BaseModel]]
+    ) -> List[Type[BaseModel]]:
+        type_origin = get_origin(annotation)
+        if isclass(annotation):
+            try:
+                if issubclass(annotation, BaseModel):
+                    return [annotation]
+                raise APIEndpointError(f"Expected: {PayloadType}")
+            except TypeError:
+                raise APIEndpointError(f"Expected: {PayloadType}")
+        # Check if Annnotated[Union[PayloadModelType, ...]], only unions of pydantic models allowed
+        elif type_origin == Annotated:
+            if annotated_origin := get_args(annotation):
+                if (len(annotated_origin) >= 1) and get_origin(annotated_origin[0]) == Union:
+                    type_args = get_args(annotated_origin[0])
+                    if all(isclass(t) for t in type_args) and all(issubclass(t, BaseModel) for t in type_args):
+                        models_types.extend(list(type_args))
+                        return models_types
+                    else:
+                        non_models = [t for t in type_args if not isclass(t)]
+                        for non_model in non_models:
+                            models_types.extend(cls.resolve_nested_base_model_unions(non_model, models_types))
+                        return models_types
+
+        # Check if Union[PayloadModelType, ...], only unions of pydantic models allowed
+        elif type_origin == Union:
+            type_args = get_args(annotation)
+            if all(isclass(t) for t in type_args) and all(issubclass(t, BaseModel) for t in type_args):
+                models_types.extend(list(type_args))
+                return models_types
+            else:
+                non_models = [t for t in type_args if not isclass(t)]
+                for non_model in non_models:
+                    models_types.extend(cls.resolve_nested_base_model_unions(non_model, models_types))
+                return models_types
+        raise APIEndpointError(f"Expected: {PayloadType}")
+
 
 @dataclass
 class APIEndpointRequestMeta:
     """Holds data for endpoints exctracted during decorating. Used for documentation"""
 
     func: Any
     http_request: str
@@ -157,51 +197,54 @@
     """
     Class to be used as base for all API endpoints.
     Injects BASE_PATH url prefix as it is common for all known vManage API endpoints.
     Introduces special keyword argument 'payload' in request call and handles sending of such object.
     """
 
     @classmethod
-    def _prepare_payload(cls, payload: PayloadType, force_json: bool = False) -> PreparedPayload:
+    def _prepare_payload(
+        cls, payload: PayloadType, force_json: bool = False, context: Dict[str, Any] = {}
+    ) -> PreparedPayload:
         """Helper method to prepare data for sending based on type"""
         if force_json or isinstance(payload, dict):
             return PreparedPayload(data=json.dumps(payload), headers={"content-type": "application/json"})
         if isinstance(payload, (str, bytes)):
             return PreparedPayload(data=payload)
         elif isinstance(payload, (BaseModel)):
-            return cls._prepare_basemodel_payload(payload)
+            return cls._prepare_basemodel_payload(payload, context)
         elif isinstance(payload, Sequence) and not isinstance(payload, (str, bytes)):
-            return cls._prepare_sequence_payload(payload)  # type: ignore[arg-type]
+            return cls._prepare_sequence_payload(payload, context)  # type: ignore[arg-type]
             # offender is List[JSON] which is also a Sequence can be ignored as long as force_json is passed correctly
         elif isinstance(payload, CustomPayloadType):
             return payload.prepared()
         else:
             raise APIRequestPayloadTypeError(payload)
 
     @classmethod
-    def _prepare_basemodel_payload(cls, payload: BaseModel) -> PreparedPayload:
+    def _prepare_basemodel_payload(cls, payload: BaseModel, context: Dict[str, Any] = {}) -> PreparedPayload:
         """Helper method to prepare BaseModel instance for sending"""
         return PreparedPayload(
-            data=payload.model_dump_json(exclude_none=True, by_alias=True), headers={"content-type": "application/json"}
+            data=payload.model_dump_json(exclude_none=True, by_alias=True, context=context),
+            headers={"content-type": "application/json"},
         )
 
     @classmethod
-    def _prepare_sequence_payload(cls, payload: Iterable[BaseModel]) -> PreparedPayload:
+    def _prepare_sequence_payload(cls, payload: Iterable[BaseModel], context: Dict[str, Any] = {}) -> PreparedPayload:
         """Helper method to prepare sequences for sending"""
         items = []
         for item in payload:
-            items.append(item.model_dump(exclude_none=True, by_alias=True))
+            items.append(item.model_dump(exclude_none=True, by_alias=True, context=context))
         data = json.dumps(items)
         return PreparedPayload(data=data, headers={"content-type": "application/json"})
 
     @classmethod
-    def _prepare_params(cls, params: RequestParamsType) -> Dict[str, Any]:
+    def _prepare_params(cls, params: RequestParamsType, context: Dict[str, Any] = {}) -> Dict[str, Any]:
         """Helper method to prepare params for sending"""
         if isinstance(params, BaseModel):
-            return params.model_dump(exclude_none=True, by_alias=True)
+            return params.model_dump(exclude_none=True, by_alias=True, context=context)
         return params
 
     def __init__(self, client: APIEndpointClient):
         self._client = client
         self._basepath = BASE_PATH
 
     def _request(
@@ -211,18 +254,19 @@
         payload: Optional[ModelPayloadType] = None,
         params: Optional[RequestParamsType] = None,
         force_json_payload: bool = False,
         **kwargs,
     ) -> APIEndpointClientResponse:
         """Prepares and sends request using client protocol"""
         _kwargs = dict(kwargs)
+        context = dict(api_version=self._api_version)
         if payload is not None:
-            _kwargs.update(self._prepare_payload(payload, force_json_payload).asdict())
+            _kwargs.update(self._prepare_payload(payload, force_json_payload, context).asdict())
         if params is not None:
-            _kwargs.update({"params": self._prepare_params(params)})
+            _kwargs.update({"params": self._prepare_params(params, context)})
         return self._client.request(method, self._basepath + url, **_kwargs)
 
     @property
     def _api_version(self) -> Optional[Version]:
         return self._client.api_version
 
     @property
@@ -437,35 +481,18 @@
                 if (
                     (type_args := get_args(annotation))
                     and (len(type_args) == 1)
                     and isclass(type_args[0])
                     and issubclass(type_args[0], BaseModel)
                 ):
                     return TypeSpecifier(True, type_origin, type_args[0], None, False, is_optional)
-            # Check if Annnotated[Union[PayloadModelType, ...]], only unions of pydantic models allowed
-            elif type_origin == Annotated:
-                if annotated_origin := get_args(annotation):
-                    if (len(annotated_origin) >= 1) and get_origin(annotated_origin[0]) == Union:
-                        if (
-                            (type_args := get_args(annotated_origin[0]))
-                            and all(isclass(t) for t in type_args)
-                            and all(issubclass(t, BaseModel) for t in type_args)
-                        ):
-                            return TypeSpecifier.model_union(models=list(type_args))
-            # Check if Union[PayloadModelType, ...], only unions of pydantic models allowed
-            elif type_origin == Union:
-                if (
-                    (type_args := get_args(annotation))
-                    and all(isclass(t) for t in type_args)
-                    and all(issubclass(t, BaseModel) for t in type_args)
-                ):
-                    return TypeSpecifier.model_union(models=list(type_args))
-            raise APIEndpointError(f"Expected: {PayloadType} but found payload {annotation}")
-        else:
-            raise APIEndpointError(f"Expected: {PayloadType} but found payload {annotation}")
+            else:
+                models = TypeSpecifier.resolve_nested_base_model_unions(annotation, [])
+                return TypeSpecifier.model_union(models)
+        raise APIEndpointError(f"'payload' param must be annotated with supported type: {PayloadType}")
 
     def check_params(self):
         """Checks params in decorated method definition
 
         Raises:
             APIEndpointError: when decorated params not matching specification
         """
@@ -564,19 +591,19 @@
                 if self.return_spec.payload_type is None:
                     pass
                 elif issubclass(self.return_spec.payload_type, BaseModel):
                     if self.return_spec.sequence_type == DataSequence:
                         return response.dataseq(
                             cls=self.return_spec.payload_type,
                             sourcekey=self.resp_json_key,
-                            validate=_self._client.validate_responses,
+                            validate=_self._client.validate_response,
                         )
                     else:
                         return response.dataobj(
-                            self.return_spec.payload_type, self.resp_json_key, validate=_self._client.validate_responses
+                            self.return_spec.payload_type, self.resp_json_key, validate=_self._client.validate_response
                         )
                 elif issubclass(self.return_spec.payload_type, str):
                     return response.text
                 elif issubclass(self.return_spec.payload_type, bytes):
                     return response.content
                 elif issubclass(self.return_spec.payload_type, dict):
                     return response.json()
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/administration_user_and_group.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/administration_user_and_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/certificate_management_device.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/certificate_management_device.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/certificate_management_vmanage.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/certificate_management_vmanage.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/client.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/client.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/cluster_management.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/cluster_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/device/software_update.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/device/software_update.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/disaster_recovery.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/disaster_recovery.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
-from catalystwan.models.configuration.feature_profile.common import Parcel, ParcelCreationResponse
+from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse
 from catalystwan.models.configuration.feature_profile.sdwan.policy_object import AnyPolicyObjectParcel
 from catalystwan.typed_list import DataSequence
 
 
 class PolicyObjectFeatureProfile(APIEndpoints):
     @versions(supported_versions=(">=20.13"), raises=False)
     @post("/v1/feature-profile/sdwan/policy-object/{profile_id}/{policy_object_list_type}")
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,62 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from typing import Optional
+from uuid import UUID
 
 from catalystwan.api.configuration_groups.parcel import _ParcelBase
-from catalystwan.endpoints import JSON, APIEndpoints, delete, get, post, put, versions
+from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileInfo,
     GetFeatureProfilesPayload,
-    ParcelId,
-    SchemaTypeQuery,
 )
+from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelId
 from catalystwan.typed_list import DataSequence
 
 
-class SystemFeatureProfile(APIEndpoints):
+class OtherFeatureProfile(APIEndpoints):
     @versions(supported_versions=(">=20.9"), raises=False)
-    @get("/v1/feature-profile/sdwan/system/aaa/schema", resp_json_key="request")
-    def get_sdwan_system_aaa_parcel_schema(self, params: SchemaTypeQuery) -> JSON:
-        ...
-
-    @versions(supported_versions=(">=20.9"), raises=False)
-    @get("/v1/feature-profile/sdwan/system")
-    def get_sdwan_system_feature_profiles(
+    @get("/v1/feature-profile/sdwan/other")
+    def get_sdwan_other_feature_profiles(
         self, payload: Optional[GetFeatureProfilesPayload]
     ) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
-    @post("/v1/feature-profile/sdwan/system")
-    def create_sdwan_system_feature_profile(
+    @post("/v1/feature-profile/sdwan/other")
+    def create_sdwan_other_feature_profile(
         self, payload: FeatureProfileCreationPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
-    @delete("/v1/feature-profile/sdwan/system/{system_id}")
-    def delete_sdwan_system_feature_profile(self, system_id: str) -> None:
+    @delete("/v1/feature-profile/sdwan/other/{profile_id}")
+    def delete_sdwan_other_feature_profile(self, profile_id: UUID) -> None:
+        ...
+
+    @versions(supported_versions=(">=20.9"), raises=False)
+    @get("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}")
+    def get_all(self, profile_id: UUID, parcel_type: UUID) -> DataSequence[Parcel]:
+        ...
+
+    @versions(supported_versions=(">=20.9"), raises=False)
+    @get("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}/{parcel_id}")
+    def get_by_id(self, profile_id: UUID, parcel_type: str, parcel_id: UUID) -> Parcel:
+        ...
+
+    @versions(supported_versions=(">=20.9"), raises=False)
+    @put("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}/{parcel_id}")
+    def update(self, profile_id: UUID, parcel_type: str, parcel_id: UUID, payload: _ParcelBase) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
-    @post("/v1/feature-profile/sdwan/system/{system_id}/aaa")
-    def create_aaa_profile_parcel_for_system(self, system_id: str, payload: _ParcelBase) -> ParcelId:
+    @delete("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}/{parcel_id}")
+    def delete(self, profile_id: UUID, parcel_type: str, parcel_id: UUID) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
-    @put("/v1/feature-profile/sdwan/system/{system_id}/aaa/{parcel_id}")
-    def edit_aaa_profile_parcel_for_system(self, system_id: str, parcel_id: str, payload: _ParcelBase) -> ParcelId:
+    @post("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}")
+    def create(self, profile_id: UUID, parcel_type: str, payload: _ParcelBase) -> ParcelId:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from typing import Optional
+from uuid import UUID
 
 from catalystwan.api.configuration_groups.parcel import _ParcelBase
 from catalystwan.endpoints import JSON, APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileDetail,
     FeatureProfileEditPayload,
     FeatureProfileInfo,
     GetFeatureProfilesPayload,
-    ParcelCreationResponse,
-    ParcelId,
     SchemaTypeQuery,
 )
-from catalystwan.models.configuration.feature_profile.sdwan.management.vpn import ManagementVPN
-from catalystwan.models.configuration.feature_profile.sdwan.transport.cellular_controller import CellularController
+from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse, ParcelId
+from catalystwan.models.configuration.feature_profile.sdwan.transport import (
+    AnyTransportParcel,
+    CellularControllerParcel,
+)
+from catalystwan.models.configuration.feature_profile.sdwan.transport.vpn import ManagementVpnParcel
 from catalystwan.typed_list import DataSequence
 
 
 class TransportFeatureProfile(APIEndpoints):
     @versions(supported_versions=(">=20.13"), raises=False)
     @post("/v1/feature-profile/sdwan/transport")
     def create_transport_feature_profile(
@@ -32,57 +35,90 @@
     @versions(supported_versions=(">=20.13"), raises=False)
     @get("/v1/feature-profile/sdwan/transport")
     def get_transport_feature_profiles(self, params: GetFeatureProfilesPayload) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.13"), raises=False)
     @get("/v1/feature-profile/sdwan/transport/{profile_id}")
-    def get_transport_feature_profile(self, profile_id: str, params: GetFeatureProfilesPayload) -> FeatureProfileDetail:
+    def get_transport_feature_profile(
+        self, profile_id: UUID, params: GetFeatureProfilesPayload
+    ) -> FeatureProfileDetail:
         ...
 
     @versions(supported_versions=(">=20.13"), raises=False)
     @put("/v1/feature-profile/sdwan/transport/{profile_id}")
     def edit_transport_feature_profile(
-        self, profile_id: str, payload: FeatureProfileEditPayload
+        self, profile_id: UUID, payload: FeatureProfileEditPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
     @versions(supported_versions=(">=20.13"), raises=False)
     @delete("/v1/feature-profile/sdwan/transport/{profile_id}")
-    def delete_transport_feature_profile(self, profile_id: str) -> None:
+    def delete_transport_feature_profile(self, profile_id: UUID) -> None:
+        ...
+
+    @versions(supported_versions=(">=20.13"), raises=False)
+    @post("/v1/feature-profile/sdwan/transport/{profile_id}/{parcel_type}")
+    def create_transport_parcel(
+        self, profile_id: UUID, parcel_type: str, payload: _ParcelBase
+    ) -> ParcelCreationResponse:
+        ...
+
+    @versions(supported_versions=(">=20.13"), raises=False)
+    @post("/v1/feature-profile/sdwan/transport/{profile_id}/wan/vpn/{vpn_id}/{parcel_type}")
+    def create_transport_vpn_sub_parcel(
+        self, profile_id: UUID, vpn_id: UUID, parcel_type: str, payload: _ParcelBase
+    ) -> ParcelCreationResponse:
+        ...
+
+    @versions(supported_versions=(">=20.13"), raises=False)
+    @post("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn/{vpn_id}/{parcel_type}")
+    def create_management_vpn_sub_parcel(
+        self, profile_id: UUID, vpn_id: UUID, parcel_type: str, payload: _ParcelBase
+    ) -> ParcelCreationResponse:
+        ...
+
+    @versions(supported_versions=(">=20.13"), raises=False)
+    @get("/v1/feature-profile/sdwan/transport/{profile_id}/{parcel_type}")
+    def get_transport_parcels(self, profile_id: UUID, parcel_type: str) -> DataSequence[Parcel[AnyTransportParcel]]:
+        ...
+
+    @versions(supported_versions=(">=20.13"), raises=False)
+    @get("/v1/feature-profile/sdwan/transport/{profile_id}/{parcel_type}/{parcel_id}")
+    def get_transport_parcel(self, profile_id: UUID, parcel_type: str, parcel_id: UUID) -> Parcel[AnyTransportParcel]:
         ...
 
     #
     # ManagementVPN parcel
     #
     @versions(supported_versions=(">=20.13"), raises=False)
     @post("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn")
-    def create_management_vpn_parcel(self, profile_id: str, payload: _ParcelBase) -> ParcelCreationResponse:
+    def create_management_vpn_parcel(self, profile_id: UUID, payload: _ParcelBase) -> ParcelCreationResponse:
         ...
 
     # @versions(supported_versions=(">=20.13"), raises=False)
     # @get("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn")
-    # def get_management_vpn_parcels(self, profile_id: str) -> ParcelSequence[ManagementVPN]:
+    # def get_management_vpn_parcels(self, profile_id: UUID) -> ParcelSequence[ManagementVPN]:
     #     ...
 
     # @versions(supported_versions=(">=20.13"), raises=False)
     # @get("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn/{parcel_id}")
-    # def get_management_vpn_parcel(self, profile_id: str, parcel_id: str) -> Parcel[ManagementVPN]:
+    # def get_management_vpn_parcel(self, profile_id: UUID, parcel_id: str) -> Parcel[ManagementVPN]:
     #     ...
 
     @versions(supported_versions=(">=20.13"), raises=False)
     @put("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn/{parcel_id}")
     def edit_management_vpn_parcel(
-        self, profile_id: str, parcel_id: str, payload: ManagementVPN
+        self, profile_id: UUID, parcel_id: str, payload: ManagementVpnParcel
     ) -> ParcelCreationResponse:
         ...
 
     @versions(supported_versions=(">=20.13"), raises=False)
     @delete("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn/{parcel_id}")
-    def delete_management_vpn_parcel(self, profile_id: str, parcel_id: str) -> None:
+    def delete_management_vpn_parcel(self, profile_id: UUID, parcel_id: str) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @get("/v1/feature-profile/sdwan/transport")
     def get_sdwan_transport_feature_profiles(
         self, payload: Optional[GetFeatureProfilesPayload]
     ) -> DataSequence[FeatureProfileInfo]:
@@ -104,10 +140,10 @@
     @delete("/v1/feature-profile/sdwan/transport/{transport_id}")
     def delete_sdwan_transport_feature_profile(self, transport_id: str) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @post("/v1/feature-profile/sdwan/transport/{transport_id}/cellular-controller")
     def create_cellular_controller_profile_parcel_for_transport(
-        self, transport_id: str, payload: CellularController
+        self, transport_id: str, payload: CellularControllerParcel
     ) -> ParcelId:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/access_control_list.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/qos_map.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,53 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.access_control_list import AclPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.qos_map import QoSMapPolicy, QoSMapPolicyEditPayload, QoSMapPolicyGetResponse
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class AclPolicyEditPayload(AclPolicy, PolicyDefinitionId):
-    pass
-
-
-class AclPolicyGetResponse(AclPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyAclDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/acl")
-    def create_policy_definition(self, payload: AclPolicy) -> PolicyDefinitionId:
+class ConfigurationPolicyQoSMapDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/qosmap")
+    def create_policy_definition(self, payload: QoSMapPolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/acl/{id}")
+    @delete("/template/policy/definition/qosmap/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/acl/multiple/{id}
+        # PUT /template/policy/definition/qosmap/multiple/{id}
         ...
 
-    @put("/template/policy/definition/acl/{id}")
-    def edit_policy_definition(self, id: UUID, payload: AclPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/qosmap/{id}")
+    def edit_policy_definition(self, id: UUID, payload: QoSMapPolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/acl", "data")
+    @get("/template/policy/definition/qosmap", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/acl/{id}")
-    def get_policy_definition(self, id: UUID) -> AclPolicyGetResponse:
+    @get("/template/policy/definition/qosmap/{id}")
+    def get_policy_definition(self, id: UUID) -> QoSMapPolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/acl/preview")
-    def preview_policy_definition(self, payload: AclPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/qosmap/preview")
+    def preview_policy_definition(self, payload: QoSMapPolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/acl/preview/{id}")
+    @get("/template/policy/definition/qosmap/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/acl/bulk
+        # PUT /template/policy/definition/qosmap/bulk
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.access_control_list_ipv6 import AclIPv6Policy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.access_control_list_ipv6 import (
+    AclIPv6Policy,
+    AclIPv6PolicyEditPayload,
+    AclIPv6PolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class AclIPv6PolicyEditPayload(AclIPv6Policy, PolicyDefinitionId):
-    pass
-
-
-class AclIPv6PolicyGetResponse(AclIPv6Policy, PolicyDefinitionGetResponse):
-    pass
-
-
 class ConfigurationPolicyAclIPv6Definition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/aclv6")
     def create_policy_definition(self, payload: AclIPv6Policy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/aclv6/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/control.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/access_control_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.control import ControlPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.access_control_list import (
+    AclPolicy,
+    AclPolicyEditPayload,
+    AclPolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class ControlPolicyEditPayload(ControlPolicy, PolicyDefinitionId):
-    pass
-
-
-class ControlPolicyGetResponse(ControlPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyControlDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/control")
-    def create_policy_definition(self, payload: ControlPolicy) -> PolicyDefinitionId:
+class ConfigurationPolicyAclDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/acl")
+    def create_policy_definition(self, payload: AclPolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/control/{id}")
+    @delete("/template/policy/definition/acl/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/control/multiple/{id}
+        # PUT /template/policy/definition/acl/multiple/{id}
         ...
 
-    @put("/template/policy/definition/control/{id}")
-    def edit_policy_definition(self, id: UUID, payload: ControlPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/acl/{id}")
+    def edit_policy_definition(self, id: UUID, payload: AclPolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/control", "data")
+    @get("/template/policy/definition/acl", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/control/{id}")
-    def get_policy_definition(self, id: UUID) -> ControlPolicyGetResponse:
+    @get("/template/policy/definition/acl/{id}")
+    def get_policy_definition(self, id: UUID) -> AclPolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/control/preview")
-    def preview_policy_definition(self, payload: ControlPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/acl/preview")
+    def preview_policy_definition(self, payload: AclPolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/control/preview/{id}")
+    @get("/template/policy/definition/acl/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/control/bulk
+        # PUT /template/policy/definition/acl/bulk
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/device_access.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/device_access.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.device_access import DeviceAccessPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.device_access import (
+    DeviceAccessPolicy,
+    DeviceAccessPolicyEditPayload,
+    DeviceAccessPolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class DeviceAccessPolicyEditPayload(DeviceAccessPolicy, PolicyDefinitionId):
-    pass
-
-
-class DeviceAccessPolicyGetResponse(DeviceAccessPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
 class ConfigurationPolicyDeviceAccessDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/deviceaccesspolicy")
     def create_policy_definition(self, payload: DeviceAccessPolicy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/deviceaccesspolicy/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/rewrite.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,57 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.device_access_ipv6 import DeviceAccessIPv6Policy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.rewrite import (
+    RewritePolicy,
+    RewritePolicyEditPayload,
+    RewritePolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class DeviceAccessIPv6PolicyEditPayload(DeviceAccessIPv6Policy, PolicyDefinitionId):
-    pass
-
-
-class DeviceAccessIPv6PolicyGetResponse(DeviceAccessIPv6Policy, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyDeviceAccessIPv6Definition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/deviceaccesspolicyv6")
-    def create_policy_definition(self, payload: DeviceAccessIPv6Policy) -> PolicyDefinitionId:
+class ConfigurationPolicyRewriteRuleDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/rewriterule")
+    def create_policy_definition(self, payload: RewritePolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/deviceaccesspolicyv6/{id}")
+    @delete("/template/policy/definition/rewriterule/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/deviceaccesspolicyv6/multiple/{id}
+        # PUT /template/policy/definition/rewriterule/multiple/{id}
         ...
 
-    @put("/template/policy/definition/deviceaccesspolicyv6/{id}")
-    def edit_policy_definition(
-        self, id: UUID, payload: DeviceAccessIPv6PolicyEditPayload
-    ) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/rewriterule/{id}")
+    def edit_policy_definition(self, id: UUID, payload: RewritePolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/deviceaccesspolicyv6", "data")
+    @get("/template/policy/definition/rewriterule", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/deviceaccesspolicyv6/{id}")
-    def get_policy_definition(self, id: UUID) -> DeviceAccessIPv6PolicyGetResponse:
+    @get("/template/policy/definition/rewriterule/{id}")
+    def get_policy_definition(self, id: UUID) -> RewritePolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/deviceaccesspolicyv6/preview")
-    def preview_policy_definition(self, payload: DeviceAccessIPv6Policy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/rewriterule/preview")
+    def preview_policy_definition(self, payload: RewritePolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/deviceaccesspolicyv6/preview/{id}")
+    @get("/template/policy/definition/rewriterule/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/deviceaccesspolicyv6/bulk
+        # PUT /template/policy/definition/rewriterule/bulk
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.hub_and_spoke import HubAndSpokePolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.hub_and_spoke import (
+    HubAndSpokePolicy,
+    HubAndSpokePolicyEditPayload,
+    HubAndSpokePolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class HubAndSpokePolicyEditPayload(HubAndSpokePolicy, PolicyDefinitionId):
-    pass
-
-
-class HubAndSpokePolicyGetResponse(HubAndSpokePolicy, PolicyDefinitionGetResponse):
-    pass
-
-
 class ConfigurationPolicyHubAndSpokeDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/hubandspoke")
     def create_policy_definition(self, payload: HubAndSpokePolicy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/hubandspoke/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/mesh.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/mesh.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.mesh import MeshPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.mesh import MeshPolicy, MeshPolicyEditPayload, MeshPolicyGetResponse
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class MeshPolicyEditPayload(MeshPolicy, PolicyDefinitionId):
-    pass
-
-
-class MeshPolicyGetResponse(MeshPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
 class ConfigurationPolicyMeshDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/mesh")
     def create_policy_definition(self, payload: MeshPolicy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/mesh/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/qos_map.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.qos_map import QoSMapPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.zone_based_firewall import (
+    ZoneBasedFWPolicy,
+    ZoneBasedFWPolicyEditPayload,
+    ZoneBasedFWPolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class QoSMapPolicyEditPayload(QoSMapPolicy, PolicyDefinitionId):
-    pass
-
-
-class QoSMapPolicyGetResponse(QoSMapPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyQoSMapDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/qosmap")
-    def create_policy_definition(self, payload: QoSMapPolicy) -> PolicyDefinitionId:
+class ConfigurationPolicyZoneBasedFirewallDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/zonebasedfw")
+    def create_policy_definition(self, payload: ZoneBasedFWPolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/qosmap/{id}")
+    @delete("/template/policy/definition/zonebasedfw/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/qosmap/multiple/{id}
+        # PUT /template/policy/definition/zonebasedfw/multiple/{id}
         ...
 
-    @put("/template/policy/definition/qosmap/{id}")
-    def edit_policy_definition(self, id: UUID, payload: QoSMapPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/zonebasedfw/{id}")
+    def edit_policy_definition(self, id: UUID, payload: ZoneBasedFWPolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/qosmap", "data")
+    @get("/template/policy/definition/zonebasedfw", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/qosmap/{id}")
-    def get_policy_definition(self, id: UUID) -> QoSMapPolicyGetResponse:
+    @get("/template/policy/definition/zonebasedfw/{id}")
+    def get_policy_definition(self, id: UUID) -> ZoneBasedFWPolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/qosmap/preview")
-    def preview_policy_definition(self, payload: QoSMapPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/zonebasedfw/preview")
+    def preview_policy_definition(self, payload: ZoneBasedFWPolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/qosmap/preview/{id}")
+    @get("/template/policy/definition/zonebasedfw/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/qosmap/bulk
+        # PUT /template/policy/definition/zonebasedfw/bulk
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/rule_set.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,59 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.rule_set import RuleSet
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.device_access_ipv6 import (
+    DeviceAccessIPv6Policy,
+    DeviceAccessIPv6PolicyEditPayload,
+    DeviceAccessIPv6PolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class RuleSetEditPayload(RuleSet, PolicyDefinitionId):
-    pass
-
-
-class RuleSetGetResponse(RuleSet, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyRuleSetDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/ruleset")
-    def create_policy_definition(self, payload: RuleSet) -> PolicyDefinitionId:
+class ConfigurationPolicyDeviceAccessIPv6Definition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/deviceaccesspolicyv6")
+    def create_policy_definition(self, payload: DeviceAccessIPv6Policy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/ruleset/{id}")
+    @delete("/template/policy/definition/deviceaccesspolicyv6/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/ruleset/multiple/{id}
+        # PUT /template/policy/definition/deviceaccesspolicyv6/multiple/{id}
         ...
 
-    @put("/template/policy/definition/ruleset/{id}")
-    def edit_policy_definition(self, id: UUID, payload: RuleSetEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/deviceaccesspolicyv6/{id}")
+    def edit_policy_definition(
+        self, id: UUID, payload: DeviceAccessIPv6PolicyEditPayload
+    ) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/ruleset", "data")
+    @get("/template/policy/definition/deviceaccesspolicyv6", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/ruleset/{id}")
-    def get_policy_definition(self, id: UUID) -> RuleSetGetResponse:
+    @get("/template/policy/definition/deviceaccesspolicyv6/{id}")
+    def get_policy_definition(self, id: UUID) -> DeviceAccessIPv6PolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/ruleset/preview")
-    def preview_policy_definition(self, payload: RuleSet) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/deviceaccesspolicyv6/preview")
+    def preview_policy_definition(self, payload: DeviceAccessIPv6Policy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/ruleset/preview/{id}")
+    @get("/template/policy/definition/deviceaccesspolicyv6/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/ruleset/bulk
+        # PUT /template/policy/definition/deviceaccesspolicyv6/bulk
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/security_group.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/security_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.security_group import SecurityGroup
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.security_group import (
+    SecurityGroup,
+    SecurityGroupEditPayload,
+    SecurityGroupGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class SecurityGroupEditPayload(SecurityGroup, PolicyDefinitionId):
-    pass
-
-
-class SecurityGroupGetResponse(SecurityGroup, PolicyDefinitionGetResponse):
-    pass
-
-
 class ConfigurationPolicySecurityGroupDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/securitygroup")
     def create_policy_definition(self, payload: SecurityGroup) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/securitygroup/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/traffic_data.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/traffic_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.traffic_data import TrafficDataPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.traffic_data import (
+    TrafficDataPolicy,
+    TrafficDataPolicyEditPayload,
+    TrafficDataPolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class TrafficDataPolicyEditPayload(TrafficDataPolicy, PolicyDefinitionId):
-    pass
-
-
-class TrafficDataPolicyGetResponse(TrafficDataPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
 class ConfigurationPolicyDataDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/data")
     def create_policy_definition(self, payload: TrafficDataPolicy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/data/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/rule_set.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,53 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.vpn_membership import VPNMembershipPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.rule_set import RuleSet, RuleSetEditPayload, RuleSetGetResponse
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class VPNMembershipPolicyEditPayload(VPNMembershipPolicy, PolicyDefinitionId):
-    pass
-
-
-class VPNMembershipPolicyGetResponse(VPNMembershipPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyVPNMembershipGroupDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/vpnmembershipgroup")
-    def create_policy_definition(self, payload: VPNMembershipPolicy) -> PolicyDefinitionId:
+class ConfigurationPolicyRuleSetDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/ruleset")
+    def create_policy_definition(self, payload: RuleSet) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/vpnmembershipgroup/{id}")
+    @delete("/template/policy/definition/ruleset/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/vpnmembershipgroup/multiple/{id}
+        # PUT /template/policy/definition/ruleset/multiple/{id}
         ...
 
-    @put("/template/policy/definition/vpnmembershipgroup/{id}")
-    def edit_policy_definition(self, id: UUID, payload: VPNMembershipPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/ruleset/{id}")
+    def edit_policy_definition(self, id: UUID, payload: RuleSetEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/vpnmembershipgroup", "data")
+    @get("/template/policy/definition/ruleset", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/vpnmembershipgroup/{id}")
-    def get_policy_definition(self, id: UUID) -> VPNMembershipPolicyGetResponse:
+    @get("/template/policy/definition/ruleset/{id}")
+    def get_policy_definition(self, id: UUID) -> RuleSetGetResponse:
         ...
 
-    @post("/template/policy/definition/vpnmembershipgroup/preview")
-    def preview_policy_definition(self, payload: VPNMembershipPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/ruleset/preview")
+    def preview_policy_definition(self, payload: RuleSet) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/vpnmembershipgroup/preview/{id}")
+    @get("/template/policy/definition/ruleset/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/vpnmembershipgroup/bulk
+        # PUT /template/policy/definition/ruleset/bulk
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/definition/dns_security.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,50 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
+
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.zone_based_firewall import ZoneBasedFWPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.dns_security import (
+    DnsSecurityPolicy,
+    DnsSecurityPolicyEditPayload,
+    DnsSecurityPolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class ZoneBasedFWPolicyEditPayload(ZoneBasedFWPolicy, PolicyDefinitionId):
-    pass
-
-
-class ZoneBasedFWPolicyGetResponse(ZoneBasedFWPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyZoneBasedFirewallDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/zonebasedfw")
-    def create_policy_definition(self, payload: ZoneBasedFWPolicy) -> PolicyDefinitionId:
+class ConfigurationPolicyDnsSecurityDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/dnssecurity")
+    def create_policy_definition(self, payload: DnsSecurityPolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/zonebasedfw/{id}")
+    @delete("/template/policy/definition/dnssecurity/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
-    def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/zonebasedfw/multiple/{id}
-        ...
-
-    @put("/template/policy/definition/zonebasedfw/{id}")
-    def edit_policy_definition(self, id: UUID, payload: ZoneBasedFWPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/dnssecurity/{id}")
+    def edit_policy_definition(self, id: UUID, payload: DnsSecurityPolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/zonebasedfw", "data")
+    @get("/template/policy/definition/dnssecurity", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/zonebasedfw/{id}")
-    def get_policy_definition(self, id: UUID) -> ZoneBasedFWPolicyGetResponse:
+    @get("/template/policy/definition/dnssecurity/{id}")
+    def get_policy_definition(self, id: UUID) -> DnsSecurityPolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/zonebasedfw/preview")
-    def preview_policy_definition(self, payload: ZoneBasedFWPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/dnssecurity/preview")
+    def preview_policy_definition(self, payload: DnsSecurityPolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/zonebasedfw/preview/{id}")
+    @get("/template/policy/definition/dnssecurity/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
-
-    def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/zonebasedfw/bulk
-        ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/app.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/port.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import AppList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.port import PortList, PortListEditPayload, PortListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class AppListEditPayload(AppList, PolicyListId):
-    pass
-
-
-class AppListInfo(AppList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyApplicationList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/app")
-    def create_policy_list(self, payload: AppList) -> PolicyListId:
+class ConfigurationPolicyPortList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/port")
+    def create_policy_list(self, payload: PortList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/app/{id}")
+    @delete("/template/policy/list/port/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/app")
+    @delete("/template/policy/list/port")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/app/{id}")
-    def edit_policy_list(self, id: UUID, payload: AppListEditPayload) -> None:
+    @put("/template/policy/list/port/{id}")
+    def edit_policy_list(self, id: UUID, payload: PortListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/app/{id}")
-    def get_lists_by_id(self, id: UUID) -> AppListInfo:
+    @get("/template/policy/list/port/{id}")
+    def get_lists_by_id(self, id: UUID) -> PortListInfo:
         ...
 
-    @get("/template/policy/list/app", "data")
-    def get_policy_lists(self) -> DataSequence[AppListInfo]:
+    @get("/template/policy/list/port", "data")
+    def get_policy_lists(self) -> DataSequence[PortListInfo]:
         ...
 
-    @get("/template/policy/list/app/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[AppListInfo]:
+    @get("/template/policy/list/port/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[PortListInfo]:
         ...
 
-    @post("/template/policy/list/app/preview")
-    def preview_policy_list(self, payload: AppList) -> PolicyListPreview:
+    @post("/template/policy/list/port/preview")
+    def preview_policy_list(self, payload: PortList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/app/preview/{id}")
+    @get("/template/policy/list/port/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/app_probe.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/app_probe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import AppProbeClassList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.app_probe import (
+    AppProbeClassList,
+    AppProbeClassListEditPayload,
+    AppProbeClassListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class AppProbeClassListEditPayload(AppProbeClassList, PolicyListId):
-    pass
-
-
-class AppProbeClassListInfo(AppProbeClassList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyAppProbeClassList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/appprobe")
     def create_policy_list(self, payload: AppProbeClassList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/appprobe/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/as_path.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/as_path.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import ASPathList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.as_path import ASPathList, ASPathListEditPayload, ASPathListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class ASPathListEditPayload(ASPathList, PolicyListId):
-    pass
-
-
-class ASPathListInfo(ASPathList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyASPathList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/aspath")
     def create_policy_list(self, payload: ASPathList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/aspath/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/class_map.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/site.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,52 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import ClassMapList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.site import SiteList, SiteListEditPayload, SiteListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class ClassMapListEditPayload(ClassMapList, PolicyListId):
-    pass
-
-
-class ClassMapListInfo(ClassMapList, PolicyListInfo):
-    pass
-
+class ConfigurationPolicySiteList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/site/defaultsite")
+    def create_default_site_list(self, payload: SiteList) -> PolicyListId:
+        ...
 
-class ConfigurationPolicyForwardingClassList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/class")
-    def create_policy_list(self, payload: ClassMapList) -> PolicyListId:
+    @post("/template/policy/list/site")
+    def create_policy_list(self, payload: SiteList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/class/{id}")
+    @delete("/template/policy/list/site/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/class")
+    @delete("/template/policy/list/site")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/class/{id}")
-    def edit_policy_list(self, id: UUID, payload: ClassMapListEditPayload) -> None:
+    @put("/template/policy/list/site/{id}")
+    def edit_policy_list(self, id: UUID, payload: SiteListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/class/{id}")
-    def get_lists_by_id(self, id: UUID) -> ClassMapListInfo:
+    @get("/template/policy/list/site/{id}")
+    def get_lists_by_id(self, id: UUID) -> SiteListInfo:
         ...
 
-    @get("/template/policy/list/class", "data")
-    def get_policy_lists(self) -> DataSequence[ClassMapListInfo]:
+    @get("/template/policy/list/site", "data")
+    def get_policy_lists(self) -> DataSequence[SiteListInfo]:
         ...
 
-    @get("/template/policy/list/class/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[ClassMapListInfo]:
+    @get("/template/policy/list/site/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[SiteListInfo]:
         ...
 
-    @post("/template/policy/list/class/preview")
-    def preview_policy_list(self, payload: ClassMapList) -> PolicyListPreview:
+    @post("/template/policy/list/site/preview")
+    def preview_policy_list(self, payload: SiteList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/class/preview/{id}")
+    @get("/template/policy/list/site/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/color.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/color.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import ColorList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.color import ColorList, ColorListEditPayload, ColorListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class ColorListEditPayload(ColorList, PolicyListId):
-    pass
-
-
-class ColorListInfo(ColorList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyColorList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/color")
     def create_policy_list(self, payload: ColorList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/color/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/community.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/community.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import CommunityList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.communities import CommunityList, CommunityListEditPayload, CommunityListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class CommunityListEditPayload(CommunityList, PolicyListId):
-    pass
-
-
-class CommunityListInfo(CommunityList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyCommunityList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/community")
     def create_policy_list(self, payload: CommunityList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/community/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import DataIPv6PrefixList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.data_ipv6_prefix import (
+    DataIPv6PrefixList,
+    DataIPv6PrefixListEditPayload,
+    DataIPv6PrefixListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class DataIPv6PrefixListEditPayload(DataIPv6PrefixList, PolicyListId):
-    pass
-
-
-class DataIPv6PrefixListInfo(DataIPv6PrefixList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyDataIPv6PrefixList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/dataipv6prefix")
     def create_policy_list(self, payload: DataIPv6PrefixList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/dataipv6prefix/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/data_prefix.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/data_prefix.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import DataPrefixList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.data_prefix import DataPrefixList, DataPrefixListEditPayload, DataPrefixListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class DataPrefixListEditPayload(DataPrefixList, PolicyListId):
-    pass
-
-
-class DataPrefixListInfo(DataPrefixList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyDataPrefixList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/dataprefix")
     def create_policy_list(self, payload: DataPrefixList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/dataprefix/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/expanded_community.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/expanded_community.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import ExpandedCommunityList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.communities import (
+    ExpandedCommunityList,
+    ExpandedCommunityListEditPayload,
+    ExpandedCommunityListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class ExpandedCommunityListEditPayload(ExpandedCommunityList, PolicyListId):
-    pass
-
-
-class ExpandedCommunityListInfo(ExpandedCommunityList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyExpandedCommunityList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/expandedcommunity")
     def create_policy_list(self, payload: ExpandedCommunityList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/expandedcommunity/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/fqdn.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/fqdn.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import FQDNList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.fqdn import FQDNList, FQDNListEditPayload, FQDNListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class FQDNListEditPayload(FQDNList, PolicyListId):
-    pass
-
-
-class FQDNListInfo(FQDNList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyFQDNList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/fqdn")
     def create_policy_list(self, payload: FQDNList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/fqdn/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/geo_location.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/url_block_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import GeoLocationList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.url import URLBlockList, URLBlockListEditPayload, URLBlockListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class GeoLocationListEditPayload(GeoLocationList, PolicyListId):
-    pass
-
-
-class GeoLocationListInfo(GeoLocationList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyGeoLocationList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/geolocation")
-    def create_policy_list(self, payload: GeoLocationList) -> PolicyListId:
+class ConfigurationPolicyURLBlockList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/urlblacklist")
+    def create_policy_list(self, payload: URLBlockList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/geolocation/{id}")
+    @delete("/template/policy/list/urlblacklist/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/geolocation")
+    @delete("/template/policy/list/urlblacklist")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/geolocation/{id}")
-    def edit_policy_list(self, id: UUID, payload: GeoLocationListEditPayload) -> None:
+    @put("/template/policy/list/urlblacklist/{id}")
+    def edit_policy_list(self, id: UUID, payload: URLBlockListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/geolocation/{id}")
-    def get_lists_by_id(self, id: UUID) -> GeoLocationListInfo:
+    @get("/template/policy/list/urlblacklist/{id}")
+    def get_lists_by_id(self, id: UUID) -> URLBlockListInfo:
         ...
 
-    @get("/template/policy/list/geolocation", "data")
-    def get_policy_lists(self) -> DataSequence[GeoLocationListInfo]:
+    @get("/template/policy/list/urlblacklist", "data")
+    def get_policy_lists(self) -> DataSequence[URLBlockListInfo]:
         ...
 
-    @get("/template/policy/list/geolocation/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[GeoLocationListInfo]:
+    @get("/template/policy/list/urlblacklist/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[URLBlockListInfo]:
         ...
 
-    @post("/template/policy/list/geolocation/preview")
-    def preview_policy_list(self, payload: GeoLocationList) -> PolicyListPreview:
+    @post("/template/policy/list/urlblacklist/preview")
+    def preview_policy_list(self, payload: URLBlockList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/geolocation/preview/{id}")
+    @get("/template/policy/list/urlblacklist/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/ips_signature.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/ips_signature.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import IPSSignatureList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.ips_signature import (
+    IPSSignatureList,
+    IPSSignatureListEditPayload,
+    IPSSignatureListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class IPSSignatureListEditPayload(IPSSignatureList, PolicyListId):
-    pass
-
-
-class IPSSignatureListInfo(IPSSignatureList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyIPSSignatureList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/ipssignature")
     def create_policy_list(self, payload: IPSSignatureList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/ipssignature/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/zone.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import IPv6PrefixList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.zone import ZoneList, ZoneListEditPayload, ZoneListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class IPv6PrefixListEditPayload(IPv6PrefixList, PolicyListId):
-    pass
-
-
-class IPv6PrefixListInfo(IPv6PrefixList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyIPv6PrefixList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/ipv6prefix")
-    def create_policy_list(self, payload: IPv6PrefixList) -> PolicyListId:
+class ConfigurationPolicyZoneList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/zone")
+    def create_policy_list(self, payload: ZoneList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/ipv6prefix/{id}")
+    @delete("/template/policy/list/zone/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/ipv6prefix")
+    @delete("/template/policy/list/zone")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/ipv6prefix/{id}")
-    def edit_policy_list(self, id: UUID, payload: IPv6PrefixListEditPayload) -> None:
+    @put("/template/policy/list/zone/{id}")
+    def edit_policy_list(self, id: UUID, payload: ZoneListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/ipv6prefix/{id}")
-    def get_lists_by_id(self, id: UUID) -> IPv6PrefixListInfo:
+    @get("/template/policy/list/zone/{id}")
+    def get_lists_by_id(self, id: UUID) -> ZoneListInfo:
         ...
 
-    @get("/template/policy/list/ipv6prefix", "data")
-    def get_policy_lists(self) -> DataSequence[IPv6PrefixListInfo]:
+    @get("/template/policy/list/zone", "data")
+    def get_policy_lists(self) -> DataSequence[ZoneListInfo]:
         ...
 
-    @get("/template/policy/list/ipv6prefix/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[IPv6PrefixListInfo]:
+    @get("/template/policy/list/zone/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[ZoneListInfo]:
         ...
 
-    @post("/template/policy/list/ipv6prefix/preview")
-    def preview_policy_list(self, payload: IPv6PrefixList) -> PolicyListPreview:
+    @post("/template/policy/list/zone/preview")
+    def preview_policy_list(self, payload: ZoneList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/ipv6prefix/preview/{id}")
+    @get("/template/policy/list/zone/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/local_app.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/local_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import LocalAppList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.local_app import LocalAppList, LocalAppListEditPayload, LocalAppListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class LocalAppListEditPayload(LocalAppList, PolicyListId):
-    pass
-
-
-class LocalAppListInfo(LocalAppList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyLocalAppList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/localapp")
     def create_policy_list(self, payload: LocalAppList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/localapp/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/local_domain.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/local_domain.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import LocalDomainList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.local_domain import LocalDomainList, LocalDomainListEditPayload, LocalDomainListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class LocalDomainListEditPayload(LocalDomainList, PolicyListId):
-    pass
-
-
-class LocalDomainListInfo(LocalDomainList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyLocalDomainList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/localdomain")
     def create_policy_list(self, payload: LocalDomainList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/localdomain/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/mirror.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/mirror.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import MirrorList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.mirror import MirrorList, MirrorListEditPayload, MirrorListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class MirrorListEditPayload(MirrorList, PolicyListId):
-    pass
-
-
-class MirrorListInfo(MirrorList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyMirrorList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/mirror")
     def create_policy_list(self, payload: MirrorList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/mirror/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/policer.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/policer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import PolicerList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.policer import PolicerList, PolicerListEditPayload, PolicerListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class PolicerListEditPayload(PolicerList, PolicyListId):
-    pass
-
-
-class PolicerListInfo(PolicerList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyPolicerClassList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/policer")
     def create_policy_list(self, payload: PolicerList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/policer/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/port.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/tloc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import PortList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.tloc import TLOCList, TLOCListEditPayload, TLOCListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class PortListEditPayload(PortList, PolicyListId):
-    pass
-
-
-class PortListInfo(PortList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyPortList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/port")
-    def create_policy_list(self, payload: PortList) -> PolicyListId:
+class ConfigurationPolicyTLOCList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/tloc")
+    def create_policy_list(self, payload: TLOCList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/port/{id}")
+    @delete("/template/policy/list/tloc/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/port")
+    @delete("/template/policy/list/tloc")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/port/{id}")
-    def edit_policy_list(self, id: UUID, payload: PortListEditPayload) -> None:
+    @put("/template/policy/list/tloc/{id}")
+    def edit_policy_list(self, id: UUID, payload: TLOCListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/port/{id}")
-    def get_lists_by_id(self, id: UUID) -> PortListInfo:
+    @get("/template/policy/list/tloc/{id}")
+    def get_lists_by_id(self, id: UUID) -> TLOCListInfo:
         ...
 
-    @get("/template/policy/list/port", "data")
-    def get_policy_lists(self) -> DataSequence[PortListInfo]:
+    @get("/template/policy/list/tloc", "data")
+    def get_policy_lists(self) -> DataSequence[TLOCListInfo]:
         ...
 
-    @get("/template/policy/list/port/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[PortListInfo]:
+    @get("/template/policy/list/tloc/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[TLOCListInfo]:
         ...
 
-    @post("/template/policy/list/port/preview")
-    def preview_policy_list(self, payload: PortList) -> PolicyListPreview:
+    @post("/template/policy/list/tloc/preview")
+    def preview_policy_list(self, payload: TLOCList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/port/preview/{id}")
+    @get("/template/policy/list/tloc/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import PreferredColorGroupList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.preferred_color_group import (
+    PreferredColorGroupList,
+    PreferredColorGroupListEditPayload,
+    PreferredColorGroupListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class PreferredColorGroupListEditPayload(PreferredColorGroupList, PolicyListId):
-    pass
-
-
-class PreferredColorGroupListInfo(PreferredColorGroupList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPreferredColorGroupList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/preferredcolorgroup")
     def create_policy_list(self, payload: PreferredColorGroupList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/preferredcolorgroup/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/prefix.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/prefix.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,20 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
+from catalystwan.api.templates.models.cisco_vpn_model import PrefixList
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import PrefixList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.prefix import PrefixListEditPayload, PrefixListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class PrefixListEditPayload(PrefixList, PolicyListId):
-    pass
-
-
-class PrefixListInfo(PrefixList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyPrefixList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/prefix")
     def create_policy_list(self, payload: PrefixList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/prefix/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/protocol_name.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/protocol_name.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import ProtocolNameList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.protocol_name import (
+    ProtocolNameList,
+    ProtocolNameListEditPayload,
+    ProtocolNameListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class ProtocolNameListEditPayload(ProtocolNameList, PolicyListId):
-    pass
-
-
-class ProtocolNameListInfo(ProtocolNameList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyProtocolNameList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/protocolname")
     def create_policy_list(self, payload: ProtocolNameList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/protocolname/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/region.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/region.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import RegionList
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListInfo, PolicyListPreview
+from catalystwan.models.policy.list.region import RegionList, RegionListEditPayload, RegionListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class RegionListEditPayload(RegionList, PolicyListId):
-    pass
-
-
-class RegionListInfo(RegionList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyRegionList(APIEndpoints):
     @post("/template/policy/list/region")
     def create_policy_list(self, payload: RegionList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/region/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/site.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/sla.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import SiteList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.sla import SLAClassList, SLAClassListEditPayload, SLAClassListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class SiteListEditPayload(SiteList, PolicyListId):
-    pass
-
-
-class SiteListInfo(SiteList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicySiteList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/site/defaultsite")
-    def create_default_site_list(self, payload: SiteList) -> PolicyListId:
-        ...
-
-    @post("/template/policy/list/site")
-    def create_policy_list(self, payload: SiteList) -> PolicyListId:
+class ConfigurationPolicySLAClassList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/sla")
+    def create_policy_list(self, payload: SLAClassList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/site/{id}")
+    @delete("/template/policy/list/sla/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/site")
+    @delete("/template/policy/list/sla")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/site/{id}")
-    def edit_policy_list(self, id: UUID, payload: SiteListEditPayload) -> None:
+    @put("/template/policy/list/sla/{id}")
+    def edit_policy_list(self, id: UUID, payload: SLAClassListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/site/{id}")
-    def get_lists_by_id(self, id: UUID) -> SiteListInfo:
+    @get("/template/policy/list/sla/{id}")
+    def get_lists_by_id(self, id: UUID) -> SLAClassListInfo:
         ...
 
-    @get("/template/policy/list/site", "data")
-    def get_policy_lists(self) -> DataSequence[SiteListInfo]:
+    @get("/template/policy/list/sla", "data")
+    def get_policy_lists(self) -> DataSequence[SLAClassListInfo]:
         ...
 
-    @get("/template/policy/list/site/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[SiteListInfo]:
+    @get("/template/policy/list/sla/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[SLAClassListInfo]:
         ...
 
-    @post("/template/policy/list/site/preview")
-    def preview_policy_list(self, payload: SiteList) -> PolicyListPreview:
+    @post("/template/policy/list/sla/preview")
+    def preview_policy_list(self, payload: SLAClassList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/site/preview/{id}")
+    @get("/template/policy/list/sla/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/sla.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/trunkgroup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,48 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import SLAClassList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.trunkgroup import TrunkGroupList, TrunkGroupListEditPayload, TrunkGroupListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class SLAClassListEditPayload(SLAClassList, PolicyListId):
-    pass
-
-
-class SLAClassListInfo(SLAClassList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicySLAClassList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/sla")
-    def create_policy_list(self, payload: SLAClassList) -> PolicyListId:
+class ConfigurationPolicyTrunkGroupList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/trunkgroup")
+    def create_policy_list(self, payload: TrunkGroupList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/sla/{id}")
+    @delete("/template/policy/list/trunkgroup/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/sla")
+    @delete("/template/policy/list/trunkgroup")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/sla/{id}")
-    def edit_policy_list(self, id: UUID, payload: SLAClassListEditPayload) -> None:
+    @put("/template/policy/list/trunkgroup/{id}")
+    def edit_policy_list(self, id: UUID, payload: TrunkGroupListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/sla/{id}")
-    def get_lists_by_id(self, id: UUID) -> SLAClassListInfo:
+    @get("/template/policy/list/trunkgroup/{id}")
+    def get_lists_by_id(self, id: UUID) -> TrunkGroupListInfo:
         ...
 
-    @get("/template/policy/list/sla", "data")
-    def get_policy_lists(self) -> DataSequence[SLAClassListInfo]:
+    @get("/template/policy/list/trunkgroup", "data")
+    def get_policy_lists(self) -> DataSequence[TrunkGroupListInfo]:
         ...
 
-    @get("/template/policy/list/sla/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[SLAClassListInfo]:
+    @get("/template/policy/list/trunkgroup/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[TrunkGroupListInfo]:
         ...
 
-    @post("/template/policy/list/sla/preview")
-    def preview_policy_list(self, payload: SLAClassList) -> PolicyListPreview:
+    @post("/template/policy/list/trunkgroup/preview")
+    def preview_policy_list(self, payload: TrunkGroupList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/sla/preview/{id}")
+    @get("/template/policy/list/trunkgroup/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/tloc.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import TLOCList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.ipv6_prefix import IPv6PrefixList, IPv6PrefixListEditPayload, IPv6PrefixListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class TLOCListEditPayload(TLOCList, PolicyListId):
-    pass
-
-
-class TLOCListInfo(TLOCList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyTLOCList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/tloc")
-    def create_policy_list(self, payload: TLOCList) -> PolicyListId:
+class ConfigurationPolicyIPv6PrefixList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/ipv6prefix")
+    def create_policy_list(self, payload: IPv6PrefixList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/tloc/{id}")
+    @delete("/template/policy/list/ipv6prefix/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/tloc")
+    @delete("/template/policy/list/ipv6prefix")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/tloc/{id}")
-    def edit_policy_list(self, id: UUID, payload: TLOCListEditPayload) -> None:
+    @put("/template/policy/list/ipv6prefix/{id}")
+    def edit_policy_list(self, id: UUID, payload: IPv6PrefixListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/tloc/{id}")
-    def get_lists_by_id(self, id: UUID) -> TLOCListInfo:
+    @get("/template/policy/list/ipv6prefix/{id}")
+    def get_lists_by_id(self, id: UUID) -> IPv6PrefixListInfo:
         ...
 
-    @get("/template/policy/list/tloc", "data")
-    def get_policy_lists(self) -> DataSequence[TLOCListInfo]:
+    @get("/template/policy/list/ipv6prefix", "data")
+    def get_policy_lists(self) -> DataSequence[IPv6PrefixListInfo]:
         ...
 
-    @get("/template/policy/list/tloc/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[TLOCListInfo]:
+    @get("/template/policy/list/ipv6prefix/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[IPv6PrefixListInfo]:
         ...
 
-    @post("/template/policy/list/tloc/preview")
-    def preview_policy_list(self, payload: TLOCList) -> PolicyListPreview:
+    @post("/template/policy/list/ipv6prefix/preview")
+    def preview_policy_list(self, payload: IPv6PrefixList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/tloc/preview/{id}")
+    @get("/template/policy/list/ipv6prefix/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/url_allow_list.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/url_allow_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import URLAllowList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.url import URLAllowList, URLAllowListEditPayload, URLAllowListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class URLAllowListEditPayload(URLAllowList, PolicyListId):
-    pass
-
-
-class URLAllowListInfo(URLAllowList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyURLAllowList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/urlwhitelist")
     def create_policy_list(self, payload: URLAllowList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/urlwhitelist/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/url_block_list.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/app.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import URLBlockList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.app import AppList, AppListEditPayload, AppListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class URLBlockListEditPayload(URLBlockList, PolicyListId):
-    pass
-
-
-class URLBlockListInfo(URLBlockList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyURLBlockList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/urlblacklist")
-    def create_policy_list(self, payload: URLBlockList) -> PolicyListId:
+class ConfigurationPolicyApplicationList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/app")
+    def create_policy_list(self, payload: AppList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/urlblacklist/{id}")
+    @delete("/template/policy/list/app/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/urlblacklist")
+    @delete("/template/policy/list/app")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/urlblacklist/{id}")
-    def edit_policy_list(self, id: UUID, payload: URLBlockListEditPayload) -> None:
+    @put("/template/policy/list/app/{id}")
+    def edit_policy_list(self, id: UUID, payload: AppListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/urlblacklist/{id}")
-    def get_lists_by_id(self, id: UUID) -> URLBlockListInfo:
+    @get("/template/policy/list/app/{id}")
+    def get_lists_by_id(self, id: UUID) -> AppListInfo:
         ...
 
-    @get("/template/policy/list/urlblacklist", "data")
-    def get_policy_lists(self) -> DataSequence[URLBlockListInfo]:
+    @get("/template/policy/list/app", "data")
+    def get_policy_lists(self) -> DataSequence[AppListInfo]:
         ...
 
-    @get("/template/policy/list/urlblacklist/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[URLBlockListInfo]:
+    @get("/template/policy/list/app/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[AppListInfo]:
         ...
 
-    @post("/template/policy/list/urlblacklist/preview")
-    def preview_policy_list(self, payload: URLBlockList) -> PolicyListPreview:
+    @post("/template/policy/list/app/preview")
+    def preview_policy_list(self, payload: AppList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/urlblacklist/preview/{id}")
+    @get("/template/policy/list/app/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/vpn.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/vpn.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,20 @@
 
 # mypy: disable-error-code="empty-body"
 
 
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import VPNList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.vpn import VPNList, VPNListEditPayload, VPNListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class VPNListEditPayload(VPNList, PolicyListId):
-    pass
-
-
-class VPNListInfo(VPNList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyVPNList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/vpn")
     def create_policy_list(self, payload: VPNList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/vpn/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/zone.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/list/extended_community.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,52 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import ZoneList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.communities import (
+    ExtendedCommunityList,
+    ExtendedCommunityListEditPayload,
+    ExtendedCommunityListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class ZoneListEditPayload(ZoneList, PolicyListId):
-    pass
-
-
-class ZoneListInfo(ZoneList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyZoneList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/zone")
-    def create_policy_list(self, payload: ZoneList) -> PolicyListId:
+class ConfigurationPolicyExtendedCommunityList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/extcommunity")
+    def create_policy_list(self, payload: ExtendedCommunityList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/zone/{id}")
+    @delete("/template/policy/list/extcommunity/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/zone")
+    @delete("/template/policy/list/extcommunity")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/zone/{id}")
-    def edit_policy_list(self, id: UUID, payload: ZoneListEditPayload) -> None:
+    @put("/template/policy/list/extcommunity/{id}")
+    def edit_policy_list(self, id: UUID, payload: ExtendedCommunityListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/zone/{id}")
-    def get_lists_by_id(self, id: UUID) -> ZoneListInfo:
+    @get("/template/policy/list/extcommunity/{id}")
+    def get_lists_by_id(self, id: UUID) -> ExtendedCommunityListInfo:
         ...
 
-    @get("/template/policy/list/zone", "data")
-    def get_policy_lists(self) -> DataSequence[ZoneListInfo]:
+    @get("/template/policy/list/extcommunity", "data")
+    def get_policy_lists(self) -> DataSequence[ExtendedCommunityListInfo]:
         ...
 
-    @get("/template/policy/list/zone/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[ZoneListInfo]:
+    @get("/template/policy/list/extcommunity/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[ExtendedCommunityListInfo]:
         ...
 
-    @post("/template/policy/list/zone/preview")
-    def preview_policy_list(self, payload: ZoneList) -> PolicyListPreview:
+    @post("/template/policy/list/extcommunity/preview")
+    def preview_policy_list(self, payload: ExtendedCommunityList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/zone/preview/{id}")
+    @get("/template/policy/list/extcommunity/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/security_template.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/security_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import JSON, APIEndpoints, delete, get, post, put
 from catalystwan.models.policy.security import (
     AnySecurityPolicy,
+    AnySecurityPolicyInfoList,
     SecurityPolicyEditResponse,
-    SecurityPolicyInfoRoot,
     SecurityPolicyRoot,
 )
-from catalystwan.typed_list import DataSequence
 
 
 class ConfigurationSecurityTemplatePolicy(APIEndpoints):
     @post("/template/policy/security")
     def create_security_template(self, payload: AnySecurityPolicy) -> None:
         ...
 
@@ -32,15 +31,15 @@
         ...
 
     def generate_security_policy_summary(self):
         # GET /template/policy/security/summary
         ...
 
     @get("/template/policy/security", "data")
-    def generate_security_template_list(self) -> DataSequence[SecurityPolicyInfoRoot]:
+    def generate_security_template_list(self) -> AnySecurityPolicyInfoList:
         ...
 
     def get_device_list_by_id(self):
         # GET /template/policy/security/devices/{policyId}
         ...
 
     def get_security_policy_device_list(self):
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/vedge_template.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/vedge_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/vsmart_template.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/policy/vsmart_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration/software_actions.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration/software_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration_dashboard_status.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_dashboard_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration_device_actions.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_device_actions.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 
 DeviceType = Literal["vedge", "controller", "vmanage"]
 
 VersionType = Literal["vmanage", "remote"]
 
 PartitionActionType = Literal["removepartition", "defaultpartition", "changepartition"]
-LxcActionType = Literal["lxc_activate", "lxc_upgrade", "lxc_delete"]
 
 
 class ActionId(BaseModel):
     id: str
 
 
 class GroupId(BaseModel):
@@ -47,44 +46,14 @@
     device_ip: str = Field(serialization_alias="deviceIP", validation_alias="deviceIP")
     version: Union[str, List[str]] = Field(default="")
 
 
 VersionList = Annotated[Union[str, List[str]], BeforeValidator(convert_to_list)]
 
 
-class InstallLxcImage(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    network_function_type: str = Field(
-        default="app-hosting", serialization_alias="networkFunctionType", validation_alias="networkFunctionType"
-    )
-    version_name: str = Field(serialization_alias="versionName", validation_alias="versionName")
-    version_type_name: str = Field(
-        default="UTD-Snort-Feature", serialization_alias="versionTypeName", validation_alias="versionTypeName"
-    )
-
-
-class LxcActivateDevice(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    device_id: str = Field(serialization_alias="deviceId", validation_alias="deviceId")
-    device_ip: str = Field(serialization_alias="deviceIP", validation_alias="deviceIP")
-    install_images: List[InstallLxcImage] = Field(serialization_alias="installImages", validation_alias="installImages")
-    vedge_vpn: str = Field(default="0", serialization_alias="vEdgeVPN", validation_alias="vEdgeVPN")
-    version_type: str = Field(default="vmanage", serialization_alias="versionType", validation_alias="versionType")
-
-
-class LxcUpgradeDevice(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    device_id: str = Field(serialization_alias="deviceId", validation_alias="deviceId")
-    device_ip: str = Field(serialization_alias="deviceIP", validation_alias="deviceIP")
-    install_images: List[InstallLxcImage] = Field(serialization_alias="installImages", validation_alias="installImages")
-
-
 class RemovePartitionDevice(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
 
     device_id: str = Field(serialization_alias="deviceId", validation_alias="deviceId")
     device_ip: str = Field(serialization_alias="deviceIP", validation_alias="deviceIP")
     version: VersionList
 
@@ -93,47 +62,14 @@
     model_config = ConfigDict(populate_by_name=True)
 
     action: PartitionActionType
     device_type: str = Field(serialization_alias="deviceType", validation_alias="deviceType")
     devices: List[PartitionDevice]
 
 
-class LxcInstallInput(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    v_edge_vpn: str = Field(serialization_alias="vEdgeVPN", validation_alias="vEdgeVPN")
-    version_type: VersionType = Field(serialization_alias="versionType", validation_alias="versionType")
-
-
-class LxcImageActivatePayload(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    action: LxcActionType
-    device_type: str = Field(serialization_alias="deviceType", validation_alias="deviceType")
-    devices: List[LxcActivateDevice]
-    input: LxcInstallInput
-
-
-class LxcImageUpgradePayload(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    action: LxcActionType
-    device_type: str = Field(serialization_alias="deviceType", validation_alias="deviceType")
-    devices: List[LxcUpgradeDevice]
-    input: LxcInstallInput
-
-
-class LxcImageDeletePayload(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    action: LxcActionType
-    device_type: str = Field(serialization_alias="deviceType", validation_alias="deviceType")
-    devices: List[LxcUpgradeDevice]
-
-
 class RemovePartitionActionPayload(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
 
     action: PartitionActionType
     device_type: str = Field(serialization_alias="deviceType", validation_alias="deviceType")
     devices: List[RemovePartitionDevice]
 
@@ -309,21 +245,19 @@
         # DELETE /device/action/security/amp/apikey/{uuid}
         ...
 
     @post("/device/action/install")
     def process_install_operation(self, payload: InstallActionPayload) -> ActionId:
         ...
 
-    @post("/device/action/lxcactivate")
-    def process_lxc_activate(self, payload: PartitionActionPayload) -> ActionId:
+    def process_lxc_activate(self):
         # POST /device/action/lxcactivate
         ...
 
-    @post("/device/action/lxcdelete")
-    def process_lxc_delete(self, payload: PartitionActionPayload) -> ActionId:
+    def process_lxc_delete(self):
         # POST /device/action/lxcdelete
         ...
 
     def process_lxc_install(self):
         # POST /device/action/lxcinstall
         ...
 
@@ -331,16 +265,15 @@
         # POST /device/action/lxcreload
         ...
 
     def process_lxc_reset(self):
         # POST /device/action/lxcreset
         ...
 
-    @post("/device/action/lxcupgrade")
-    def process_lxc_upgrade(self, payload: PartitionActionPayload) -> ActionId:
+    def process_lxc_upgrade(self):
         # POST /device/action/lxcupgrade
         ...
 
     def process_reboot(self):
         # POST /device/action/reboot
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration_device_inventory.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration_device_template.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_device_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration_feature_profile.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_feature_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration_group.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_group.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from datetime import datetime
-from typing import List, Optional
+from typing import Any, List, Optional, Union
+from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.common import Solution
 from catalystwan.models.configuration.feature_profile.common import ProfileType
 from catalystwan.typed_list import DataSequence
 
 
 class ProfileId(BaseModel):
-    id: str
+    id: UUID
 
 
 # TODO Get mode from schema
 class ConfigGroupCreationPayload(BaseModel):
     name: str
     description: str
     solution: Solution
@@ -34,18 +35,37 @@
     created_by: str = Field(serialization_alias="createdBy", validation_alias="createdBy")
     last_updated_by: str = Field(serialization_alias="lastUpdatedBy", validation_alias="lastUpdatedBy")
     created_on: datetime = Field(serialization_alias="createdOn", validation_alias="createdOn")
     last_updated_on: datetime = Field(serialization_alias="lastUpdatedOn", validation_alias="lastUpdatedOn")
 
 
 class ConfigGroup(BaseModel):
+    model_config = ConfigDict(populate_by_name=True)
+    id: UUID
     name: str
     description: Optional[str]
     solution: Solution
     profiles: Optional[List[FeatureProfile]]
+    source: Optional[str] = None
+    state: Optional[str] = None
+    devices: Optional[List] = Field(default=[])
+    created_by: Optional[str] = Field(serialization_alias="createdBy", validation_alias="createdBy")
+    last_updated_by: Optional[str] = Field(serialization_alias="lastUpdatedBy", validation_alias="lastUpdatedBy")
+    created_on: Optional[datetime] = Field(serialization_alias="createdOn", validation_alias="createdOn")
+    last_updated_on: Optional[datetime] = Field(serialization_alias="lastUpdatedOn", validation_alias="lastUpdatedOn")
+    version: int
+    number_of_devices: int = Field(serialization_alias="numberOfDevices", validation_alias="numberOfDevices")
+    number_of_devices_up_to_date: int = Field(
+        serialization_alias="numberOfDevicesUpToDate", validation_alias="numberOfDevicesUpToDate"
+    )
+    origin: Optional[str] = None
+    topology: Any = None
+    full_config_cli: Optional[bool] = Field(
+        default=None, serialization_alias="fullConfigCli", validation_alias="fullConfigCli"
+    )
 
 
 class ConfigGroupResponsePayload(BaseModel):
     config_groups: List[ConfigGroup]
 
 
 class ConfigGroupEditPayload(BaseModel):
@@ -64,17 +84,20 @@
 
 
 class ConfigGroupVariablesCreatePayload(BaseModel):
     deviceIds: List[str]
     suggestions: bool = True
 
 
+VariableType = Union[str, int, bool, List[Union[str, int, bool]]]
+
+
 class VariableData(BaseModel):
     name: str
-    value: str
+    value: Optional[VariableType] = None
 
 
 class DeviceVariables(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     device_id: str = Field(serialization_alias="device-id", validation_alias="device-id")
     variables: List[VariableData]
 
@@ -107,15 +130,15 @@
 
 
 class ConfigGroupDisassociateResponse(BaseModel):
     parentTaskId: str
 
 
 class ConfigGroupCreationResponse(BaseModel):
-    id: str
+    id: UUID
 
 
 class EditedProfileId(BaseModel):
     profileId: str
 
 
 class ConfigGroupEditResponse(BaseModel):
@@ -139,15 +162,15 @@
     def create_variables(
         self, config_group_id: str, payload: ConfigGroupVariablesCreatePayload
     ) -> ConfigGroupVariablesCreateResponse:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @delete("/v1/config-group/{config_group_id}")
-    def delete_config_group(self, config_group_id: str) -> None:
+    def delete_config_group(self, config_group_id: UUID) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @post("/v1/config-group/{config_group_id}/device/deploy")
     def deploy(self, config_group_id: str, payload: ConfigGroupDeployPayload) -> ConfigGroupDeployResponse:
         ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/configuration_settings.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/configuration_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -331,14 +331,60 @@
     def check_vpn(cls, vpn_str: str):
         vpn = int(vpn_str)
         if vpn < 0 or vpn > 65530:
             raise ValueError("vpn should be in range 0-65530")
         return vpn_str
 
 
+class CloudCredentials(BaseModel):
+    model_config = ConfigDict(populate_by_name=True)
+
+    umbrella_org_id: Optional[str] = Field(
+        default=None, validation_alias="umbrellaOrgId", serialization_alias="umbrellaOrgId"
+    )
+    umbrella_sig_auth_key: Optional[str] = Field(
+        default=None, validation_alias="umbrellaSIGAuthKey", serialization_alias="umbrellaSIGAuthKey"
+    )
+    umbrella_sig_auth_secret: Optional[str] = Field(
+        default=None, validation_alias="umbrellaSIGAuthSecret", serialization_alias="umbrellaSIGAuthSecret"
+    )
+    umbrella_dns_auth_key: Optional[str] = Field(
+        default=None, validation_alias="umbrellaDNSAuthKey", serialization_alias="umbrellaDNSAuthKey"
+    )
+    umbrella_dns_auth_secret: Optional[str] = Field(
+        default=None, validation_alias="umbrellaDNSAuthSecret", serialization_alias="umbrellaDNSAuthSecret"
+    )
+
+    zscaler_organization: Optional[str] = Field(
+        default=None, validation_alias="zscalerOrganization", serialization_alias="zscalerOrganization"
+    )
+    zscaler_partner_base_uri: Optional[str] = Field(
+        default=None, validation_alias="zscalerPartnerBaseUri", serialization_alias="zscalerPartnerBaseUri"
+    )
+    zscaler_partner_key: Optional[str] = Field(
+        default=None, validation_alias="zscalerPartnerKey", serialization_alias="zscalerPartnerKey"
+    )
+    zscaler_username: Optional[str] = Field(
+        default=None, validation_alias="zscalerUsername", serialization_alias="zscalerUsername"
+    )
+    zscaler_password: Optional[str] = Field(
+        default=None, validation_alias="zscalerPassword", serialization_alias="zscalerPassword"
+    )
+
+    cisco_sse_org_id: Optional[str] = Field(
+        default=None, validation_alias="ciscoSSEOrgId", serialization_alias="ciscoSSEOrgId"
+    )
+    cisco_sse_auth_key: Optional[str] = Field(
+        default=None, validation_alias="ciscoSSEAuthKey", serialization_alias="ciscoSSEAuthKey"
+    )
+    cisco_sse_auth_secret: Optional[str] = Field(
+        default=None, validation_alias="ciscoSSEAuthSecret", serialization_alias="ciscoSSEAuthSecret"
+    )
+
+
 class ConfigurationSettings(APIEndpoints):
     def create_analytics_data_file(self):
         # POST /settings/configuration/analytics/dca
         ...
 
     def edit_cert_configuration(self):
         # PUT /settings/configuration/certificate/{settingType}
@@ -498,14 +544,18 @@
         ...
 
     @view({SingleTenantView, ProviderView})
     @get("/settings/configuration/smartLicensing", "data")
     def get_smart_licensing_settings(self) -> DataSequence[SmartLicensingSetting]:
         ...
 
+    @get("/settings/configuration/cloudProviderSetting", "data")
+    def get_cloud_credentials(self) -> DataSequence[CloudCredentials]:
+        ...
+
     def new_cert_configuration(self):
         # POST /settings/configuration/certificate/{settingType}
         ...
 
     def new_configuration(self):
         # POST /settings/configuration/{settingType}
         ...
@@ -654,7 +704,15 @@
     def edit_walkme(self, payload: WalkMe) -> DataSequence[WalkMe]:
         ...
 
     @view({SingleTenantView, ProviderView})
     @put("/settings/configuration/smartLicensing", "data")
     def edit_smart_licensing_settings(self, payload: SmartLicensingSetting) -> DataSequence[SmartLicensingSetting]:
         ...
+
+    @put("/settings/configuration/cloudProviderSetting", "data")
+    def edit_cloud_credentials(self, payload: CloudCredentials) -> DataSequence[CloudCredentials]:
+        ...
+
+    @post("/settings/configuration/cloudProviderSetting", "data")
+    def create_cloud_credentials(self, payload: CloudCredentials) -> DataSequence[CloudCredentials]:
+        ...
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/endpoints_container.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/endpoints_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 from catalystwan.endpoints.administration_user_and_group import AdministrationUserAndGroup
 from catalystwan.endpoints.certificate_management_device import CertificateManagementDevice
 from catalystwan.endpoints.certificate_management_vmanage import CertificateManagementVManage
 from catalystwan.endpoints.client import Client
 from catalystwan.endpoints.cluster_management import ClusterManagement
 from catalystwan.endpoints.configuration.device.software_update import ConfigurationDeviceSoftwareUpdate
 from catalystwan.endpoints.configuration.disaster_recovery import ConfigurationDisasterRecovery
+from catalystwan.endpoints.configuration.feature_profile.sdwan.cli import CliFeatureProfile
+from catalystwan.endpoints.configuration.feature_profile.sdwan.sig_security import SIGSecurity
 from catalystwan.endpoints.configuration.feature_profile.sdwan.system import SystemFeatureProfile
+from catalystwan.endpoints.configuration.feature_profile.sdwan.topology import TopologyFeatureProfile
 from catalystwan.endpoints.configuration.feature_profile.sdwan.transport import TransportFeatureProfile
 from catalystwan.endpoints.configuration.policy.definition.access_control_list import ConfigurationPolicyAclDefinition
 from catalystwan.endpoints.configuration.policy.definition.access_control_list_ipv6 import (
     ConfigurationPolicyAclIPv6Definition,
 )
 from catalystwan.endpoints.configuration.policy.definition.control import ConfigurationPolicyControlDefinition
 from catalystwan.endpoints.configuration.policy.definition.device_access import (
@@ -60,14 +63,15 @@
 from catalystwan.endpoints.configuration.policy.list.preferred_color_group import ConfigurationPreferredColorGroupList
 from catalystwan.endpoints.configuration.policy.list.prefix import ConfigurationPolicyPrefixList
 from catalystwan.endpoints.configuration.policy.list.protocol_name import ConfigurationPolicyProtocolNameList
 from catalystwan.endpoints.configuration.policy.list.region import ConfigurationPolicyRegionList
 from catalystwan.endpoints.configuration.policy.list.site import ConfigurationPolicySiteList
 from catalystwan.endpoints.configuration.policy.list.sla import ConfigurationPolicySLAClassList
 from catalystwan.endpoints.configuration.policy.list.tloc import ConfigurationPolicyTLOCList
+from catalystwan.endpoints.configuration.policy.list.trunkgroup import ConfigurationPolicyTrunkGroupList
 from catalystwan.endpoints.configuration.policy.list.url_allow_list import ConfigurationPolicyURLAllowList
 from catalystwan.endpoints.configuration.policy.list.url_block_list import ConfigurationPolicyURLBlockList
 from catalystwan.endpoints.configuration.policy.list.vpn import ConfigurationPolicyVPNList
 from catalystwan.endpoints.configuration.policy.list.zone import ConfigurationPolicyZoneList
 from catalystwan.endpoints.configuration.policy.security_template import ConfigurationSecurityTemplatePolicy
 from catalystwan.endpoints.configuration.policy.vedge_template import ConfigurationVEdgeTemplatePolicy
 from catalystwan.endpoints.configuration.policy.vsmart_template import ConfigurationVSmartTemplatePolicy
@@ -80,24 +84,22 @@
     ConfigurationFeatureProfile,
     SDRoutingConfigurationFeatureProfile,
 )
 from catalystwan.endpoints.configuration_group import ConfigurationGroup
 from catalystwan.endpoints.configuration_settings import ConfigurationSettings
 from catalystwan.endpoints.misc import MiscellaneousEndpoints
 from catalystwan.endpoints.monitoring.device_details import MonitoringDeviceDetails
-from catalystwan.endpoints.monitoring.security_policy import MonitoringSecurityPolicy
 from catalystwan.endpoints.monitoring.server_info import ServerInfo
 from catalystwan.endpoints.monitoring.status import MonitoringStatus
 from catalystwan.endpoints.real_time_monitoring.reboot_history import RealTimeMonitoringRebootHistory
 from catalystwan.endpoints.sdavc_cloud_connector import SDAVCCloudConnector
 from catalystwan.endpoints.tenant_backup_restore import TenantBackupRestore
 from catalystwan.endpoints.tenant_management import TenantManagement
 from catalystwan.endpoints.tenant_migration import TenantMigration
 from catalystwan.endpoints.troubleshooting_tools.device_connectivity import TroubleshootingToolsDeviceConnectivity
-from catalystwan.endpoints.url_monitoring import UrlMonitoring
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
 
 class ConfigurationPolicyListContainer:
     def __init__(self, session: ManagerSession):
@@ -122,14 +124,15 @@
         self.preferred_color_group = ConfigurationPreferredColorGroupList(session)
         self.prefix = ConfigurationPolicyPrefixList(session)
         self.protocol_name = ConfigurationPolicyProtocolNameList(session)
         self.region = ConfigurationPolicyRegionList(session)
         self.site = ConfigurationPolicySiteList(session)
         self.sla = ConfigurationPolicySLAClassList(session)
         self.tloc = ConfigurationPolicyTLOCList(session)
+        self.trunkgroup = ConfigurationPolicyTrunkGroupList(session)
         self.url_block_list = ConfigurationPolicyURLBlockList(session)
         self.url_allow_list = ConfigurationPolicyURLAllowList(session)
         self.vpn = ConfigurationPolicyVPNList(session)
         self.zone = ConfigurationPolicyZoneList(session)
 
 
 class ConfigurationPolicyDefinitionContainer:
@@ -159,14 +162,16 @@
         self.security_template = ConfigurationSecurityTemplatePolicy(session)
 
 
 class ConfigurationSDWANFeatureProfileContainer:
     def __init__(self, session: ManagerSession):
         self.transport = TransportFeatureProfile(client=session)
         self.system = SystemFeatureProfile(client=session)
+        self.cli = CliFeatureProfile(client=session)
+        self.topology = TopologyFeatureProfile(client=session)
 
 
 class ConfigurationFeatureProfileContainer:
     def __init__(self, session: ManagerSession):
         self.sdwan = ConfigurationSDWANFeatureProfileContainer(session=session)
 
 
@@ -197,23 +202,22 @@
         self.configuration_device_actions = ConfigurationDeviceActions(session)
         self.configuration_device_software_update = ConfigurationDeviceSoftwareUpdate(session)
         self.configuration_device_template = ConfigurationDeviceTemplate(session)
         self.configuration_settings = ConfigurationSettings(session)
         self.configuration_software_actions = ConfigurationSoftwareActions(session)
         self.configuration_disaster_recovery = ConfigurationDisasterRecovery(session)
         self.monitoring_device_details = MonitoringDeviceDetails(session)
-        self.monitoring_security_policy = MonitoringSecurityPolicy(session)
         self.monitoring_server_info = ServerInfo(session)
         self.monitoring_status = MonitoringStatus(session)
         self.sdavc_cloud_connector = SDAVCCloudConnector(session)
         self.tenant_backup_restore = TenantBackupRestore(session)
         self.tenant_management = TenantManagement(session)
         self.tenant_migration = TenantMigration(session)
         self.configuration_feature_profile = ConfigurationFeatureProfile(session)
         self.configuration_group = ConfigurationGroup(session)
         self.sd_routing_configuration_feature_profile = SDRoutingConfigurationFeatureProfile(session)
         self.configuration_device_inventory = ConfigurationDeviceInventory(session)
         self.troubleshooting_tools = TroubleshootingToolsContainer(session)
         self.misc = MiscellaneousEndpoints(session)
         self.real_time_monitoring = RealTimeMonitoringContainer(session)
         self.certificate_management_device = CertificateManagementDevice(session)
-        self.url_monitoring = UrlMonitoring(session)
+        self.sig_security = SIGSecurity(session)
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/misc.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/monitoring/device_details.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/monitoring/device_details.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/monitoring/status.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/monitoring/status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/real_time_monitoring/reboot_history.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/real_time_monitoring/reboot_history.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/sdavc_cloud_connector.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/sdavc_cloud_connector.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/tenant_backup_restore.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/tenant_backup_restore.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/tenant_management.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/tenant_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/tenant_migration.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/tenant_migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 class MigrationTokenQueryParams(BaseModel):
     model_config = ConfigDict(populate_by_name=True, extra="allow")
     migration_id: str = Field(serialization_alias="migrationId", validation_alias="migrationId")
 
     @model_validator(mode="before")
     @classmethod
     def single_migration_id_required(cls, values: Any):
+        if not isinstance(values, dict):
+            return values
         migration_id = values.get("migrationId")
         if isinstance(migration_id, list) and len(migration_id) == 1:
             values["migrationId"] = migration_id[0]
         return values
 
 
 class ExportInfo(BaseModel):
```

### Comparing `catalystwan-0.33.7/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py` & `catalystwan-0.33.7.dev0/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/exceptions.py` & `catalystwan-0.33.7.dev0/catalystwan/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,25 @@
         _args = args
         if not _args:
             _args = (info_str,)
         else:
             _args = (str(_args[0]) + "\n" + info_str,) + _args[1:]
         super().__init__(*_args, **kwargs)
 
+    def __str__(self):
+        error_info_str = str(self.info) if self.info else "No error information"
+        request_str = (
+            f"Request: Method: {self.request.method}, URL: {self.request.url},"
+            f"Headers: {self.request.headers}, Body: {self.request.body}"
+        )
+        response_str = (
+            f"Response: {str(self.response.json())}" if self.response else "Response: No response information"
+        )
+        return f"{error_info_str}\n\n {request_str}\n\n {response_str}"
+
 
 class DefaultPasswordError(CatalystwanException):
     """Default password for SDWAN Manager user was detected and needs to be changed."""
 
     pass
```

### Comparing `catalystwan-0.33.7/catalystwan/integration_tests/test_find_template_values.py` & `catalystwan-0.33.7.dev0/catalystwan/integration_tests/test_find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/logging.conf` & `catalystwan-0.33.7.dev0/catalystwan/logging.conf`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/README.md` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/builder.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/builder.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,123 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Mapping, Union
+from typing import List, Union
 
 from pydantic import Field
 from typing_extensions import Annotated
 
 from .policy.app_probe import AppProbeMapItem, AppProbeParcel
 from .policy.application_list import ApplicationFamilyListEntry, ApplicationListEntry, ApplicationListParcel
+from .policy.as_path import AsPathParcel
 from .policy.color_list import ColorEntry, ColorParcel
 from .policy.data_prefix import DataPrefixEntry, DataPrefixParcel
 from .policy.expanded_community_list import ExpandedCommunityParcel
 from .policy.fowarding_class import FowardingClassParcel, FowardingClassQueueEntry
 from .policy.ipv6_data_prefix import IPv6DataPrefixEntry, IPv6DataPrefixParcel
 from .policy.ipv6_prefix_list import IPv6PrefixListEntry, IPv6PrefixListParcel
-from .policy.policier import PolicierEntry, PolicierParcel
+from .policy.mirror import MirrorParcel
+from .policy.policer import PolicerEntry, PolicerParcel
 from .policy.prefered_group_color import Preference, PreferredColorGroupEntry, PreferredColorGroupParcel
 from .policy.prefix_list import PrefixListEntry, PrefixListParcel
 from .policy.sla_class import FallbackBestTunnel, SLAAppProbeClass, SLAClassCriteria, SLAClassListEntry, SLAClassParcel
 from .policy.standard_community import StandardCommunityEntry, StandardCommunityParcel
 from .policy.tloc_list import TlocEntry, TlocParcel
+from .security.aip import AdvancedInspectionProfileParcel
+from .security.amp import AdvancedMalwareProtectionParcel
 from .security.application_list import (
     SecurityApplicationFamilyListEntry,
     SecurityApplicationListEntry,
     SecurityApplicationListParcel,
 )
 from .security.data_prefix import SecurityDataPrefixEntry, SecurityDataPrefixParcel
 from .security.fqdn import FQDNDomainParcel, FQDNListEntry
 from .security.geolocation_list import GeoLocationListEntry, GeoLocationListParcel
+from .security.intrusion_prevention import IntrusionPreventionParcel
 from .security.ips_signature import IPSSignatureListEntry, IPSSignatureParcel
 from .security.local_domain import LocalDomainListEntry, LocalDomainParcel
 from .security.protocol_list import ProtocolListEntry, ProtocolListParcel
 from .security.security_port import SecurityPortListEntry, SecurityPortParcel
-from .security.url import BaseURLListEntry, URLAllowParcel, URLBlockParcel
+from .security.ssl_decryption import SslDecryptionParcel
+from .security.ssl_decryption_profile import SslDecryptionProfileParcel
+from .security.url import BaseURLListEntry, URLAllowParcel, URLBlockParcel, URLParcel
 from .security.zone import SecurityZoneListEntry, SecurityZoneListParcel
 
 AnyPolicyObjectParcel = Annotated[
     Union[
-        AppProbeParcel,
+        AdvancedInspectionProfileParcel,
+        AdvancedMalwareProtectionParcel,
+        URLParcel,
         ApplicationListParcel,
+        AppProbeParcel,
+        AsPathParcel,
         ColorParcel,
         DataPrefixParcel,
         ExpandedCommunityParcel,
         FowardingClassParcel,
+        FQDNDomainParcel,
+        GeoLocationListParcel,
+        IntrusionPreventionParcel,
+        IPSSignatureParcel,
         IPv6DataPrefixParcel,
         IPv6PrefixListParcel,
-        PrefixListParcel,
-        PolicierParcel,
-        PreferredColorGroupParcel,
-        SLAClassParcel,
-        TlocParcel,
-        StandardCommunityParcel,
         LocalDomainParcel,
-        FQDNDomainParcel,
-        IPSSignatureParcel,
-        URLAllowParcel,
-        URLBlockParcel,
-        SecurityPortParcel,
+        MirrorParcel,
+        PolicerParcel,
+        PreferredColorGroupParcel,
+        PrefixListParcel,
         ProtocolListParcel,
-        GeoLocationListParcel,
-        SecurityZoneListParcel,
         SecurityApplicationListParcel,
         SecurityDataPrefixParcel,
+        SecurityPortParcel,
+        SecurityZoneListParcel,
+        SLAClassParcel,
+        SslDecryptionParcel,
+        SslDecryptionProfileParcel,
+        StandardCommunityParcel,
+        TlocParcel,
     ],
-    Field(discriminator="type"),
+    Field(discriminator="type_"),
 ]
 
-POLICY_OBJECT_PAYLOAD_ENDPOINT_MAPPING: Mapping[type, str] = {
-    AppProbeParcel: "app-probe",
-    ApplicationListParcel: "app-list",
-    ColorParcel: "color",
-    DataPrefixParcel: "data-prefix",
-    ExpandedCommunityParcel: "expanded-community",
-    FowardingClassParcel: "class",
-    IPv6DataPrefixParcel: "data-ipv6-prefix",
-    IPv6PrefixListParcel: "ipv6-prefix",
-    PrefixListParcel: "prefix",
-    PolicierParcel: "policer",
-    PreferredColorGroupParcel: "preferred-color-group",
-    SLAClassParcel: "sla-class",
-    TlocParcel: "tloc",
-    StandardCommunityParcel: "standard-community",
-    LocalDomainParcel: "security-localdomain",
-    FQDNDomainParcel: "security-fqdn",
-    IPSSignatureParcel: "security-ipssignature",
-    URLAllowParcel: "security-urllist",
-    URLBlockParcel: "security-urllist",
-    SecurityPortParcel: "security-port",
-    ProtocolListParcel: "security-protocolname",
-    GeoLocationListParcel: "security-geolocation",
-    SecurityZoneListParcel: "security-zone",
-    SecurityApplicationListParcel: "security-localapp",
-    SecurityDataPrefixParcel: "security-data-ip-prefix",
-}
-
 __all__ = (
+    "AdvancedInspectionProfileParcel",
+    "AdvancedMalwareProtectionParcel",
     "AnyPolicyObjectParcel",
     "ApplicationFamilyListEntry",
     "ApplicationListEntry",
     "ApplicationListParcel",
     "AppProbeEntry",
     "AppProbeMapItem",
     "AppProbeParcel",
+    "AsPathParcel",
     "BaseURLListEntry",
     "ColorEntry",
     "ColorParcel",
     "DataPrefixEntry",
     "DataPrefixParcel",
     "ExpandedCommunityParcel",
     "FallbackBestTunnel",
     "FowardingClassParcel",
     "FowardingClassQueueEntry",
     "FQDNDomainParcel",
     "FQDNListEntry",
     "GeoLocationListEntry",
     "GeoLocationListParcel",
+    "IntrusionPreventionParcel",
     "IPSSignatureListEntry",
     "IPSSignatureParcel",
     "IPv6DataPrefixEntry",
     "IPv6DataPrefixParcel",
     "IPv6PrefixListEntry",
     "IPv6PrefixListParcel",
     "LocalDomainListEntry",
     "LocalDomainParcel",
-    "PolicierEntry",
-    "PolicierParcel",
+    "MirrorParcel",
+    "PolicerEntry",
+    "PolicerParcel",
     "Preference",
     "PreferredColorGroupEntry",
     "PreferredColorGroupParcel",
     "PrefixListEntry",
     "PrefixListParcel",
     "ProtocolListEntry",
     "ProtocolListParcel",
@@ -140,18 +130,21 @@
     "SecurityPortParcel",
     "SecurityZoneListEntry",
     "SecurityZoneListParcel",
     "SLAAppProbeClass",
     "SLAClassCriteria",
     "SLAClassListEntry",
     "SLAClassParcel",
+    "SslDecryptionParcel",
+    "SslDecryptionProfileParcel",
     "StandardCommunityEntry",
     "StandardCommunityParcel",
     "TlocEntry",
     "TlocParcel",
+    "URLParcel",
     "URLAllowParcel",
     "URLBlockParcel",
 )
 
 
 def __dir__() -> "List[str]":
     return list(__all__)
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import TLOCColor
 
 
@@ -24,14 +24,15 @@
     map: List[AppProbeMapItem] = Field(default=[])
     forwarding_class_name: Global[str] = Field(
         serialization_alias="forwardingClass", validation_alias="forwardingClass"
     )
 
 
 class AppProbeParcel(_ParcelBase):
+    type_: Literal["app-probe"] = Field(default="app-probe", exclude=True)
     entries: List[AppProbeEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_fowarding_class(self, forwarding_class_name: str):
         self.entries.append(
             AppProbeEntry(
                 forwarding_class_name=as_global(forwarding_class_name),
             )
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Union
+from typing import List, Literal, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class ApplicationListEntry(BaseModel):
@@ -14,14 +14,15 @@
 
 class ApplicationFamilyListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     app_list_family: Global[str] = Field(serialization_alias="appFamily", validation_alias="appFamily")
 
 
 class ApplicationListParcel(_ParcelBase):
+    type_: Literal["app-list"] = Field(default="app-list", exclude=True)
     entries: List[Union[ApplicationListEntry, ApplicationFamilyListEntry]] = Field(
         default=[], validation_alias=AliasPath("data", "entries")
     )
 
     def add_application(self, application: str):
         self.entries.append(ApplicationListEntry(app_list=as_global(application)))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from ipaddress import IPv4Address, IPv4Network
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class DataPrefixEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     ipv4_address: Global[IPv4Address] = Field(serialization_alias="ipv4Address", validation_alias="ipv4Address")
     ipv4_prefix_length: Global[int] = Field(serialization_alias="ipv4PrefixLength", validation_alias="ipv4PrefixLength")
 
+    @staticmethod
+    def from_ipv4_network(ipv4_network: IPv4Network) -> "DataPrefixEntry":
+        return DataPrefixEntry(
+            ipv4_address=as_global(ipv4_network.network_address),
+            ipv4_prefix_length=as_global(ipv4_network.prefixlen),
+        )
+
 
 class DataPrefixParcel(_ParcelBase):
+    type_: Literal["data-prefix"] = Field(default="data-prefix", exclude=True)
     entries: List[DataPrefixEntry] = Field(default_factory=list, validation_alias=AliasPath("data", "entries"))
 
     def add_data_prefix(self, ipv4_network: IPv4Network):
-        self.entries.append(
-            DataPrefixEntry(
-                ipv4_address=as_global(ipv4_network.network_address),
-                ipv4_prefix_length=as_global(ipv4_network.prefixlen),
-            )
-        )
+        self.entries.append(DataPrefixEntry.from_ipv4_network(ipv4_network))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from typing import List, Literal
+
 from pydantic import AliasPath, ConfigDict, Field, field_validator
 
-from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
+from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase
 
 
 class ExpandedCommunityParcel(_ParcelBase):
+    type_: Literal["expanded-community"] = Field(default="expanded-community", exclude=True)
     model_config = ConfigDict(populate_by_name=True)
-    expandedCommunityList: Global[list] = Field(
-        default=as_global([]),
+    expanded_community_list: Global[List[str]] = Field(
+        default=Global[List[str]](value=list()),
         serialization_alias="expandedCommunityList",
         validation_alias=AliasPath("data", "expandedCommunityList"),
     )
 
     def add_community(self, expanded_community: str):
-        self.expandedCommunityList.value.append(expanded_community)
+        self.expanded_community_list.value.append(expanded_community)
 
-    @field_validator("expandedCommunityList")
+    @field_validator("expanded_community_list")
     @classmethod
-    def check_rate(cls, expanded_community_list: Global):
+    def check_list_str(cls, expanded_community_list: Global):
         assert all([isinstance(ec, str) for ec in expanded_community_list.value])
         return expanded_community_list
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class FowardingClassQueueEntry(BaseModel):
@@ -14,11 +14,12 @@
     @classmethod
     def check_burst(cls, queue: Global):
         assert 0 <= int(queue.value) <= 7
         return queue
 
 
 class FowardingClassParcel(_ParcelBase):
+    type_: Literal["class"] = Field(default="class", exclude=True)
     entries: List[FowardingClassQueueEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_queue(self, queue: int):
         self.entries.append(FowardingClassQueueEntry(queue=as_global(str(queue))))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from ipaddress import IPv6Address, IPv6Network
-from typing import List
+from ipaddress import IPv6Address, IPv6Interface
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class IPv6DataPrefixEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     ipv6_address: Global[IPv6Address] = Field(serialization_alias="ipv6Address", validation_alias="ipv6Address")
     ipv6_prefix_length: Global[int] = Field(serialization_alias="ipv6PrefixLength", validation_alias="ipv6PrefixLength")
 
 
 class IPv6DataPrefixParcel(_ParcelBase):
+    type_: Literal["data-ipv6-prefix"] = Field(default="data-ipv6-prefix", exclude=True)
     entries: List[IPv6DataPrefixEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
-    def add_prefix(self, ipv6_network: IPv6Network):
+    def add_prefix(self, ipv6_network: IPv6Interface):
         self.entries.append(
             IPv6DataPrefixEntry(
-                ipv6_address=as_global(ipv6_network.network_address),
-                ipv6_prefix_length=as_global(ipv6_network.prefixlen),
+                ipv6_address=as_global(ipv6_network.network.network_address),
+                ipv6_prefix_length=as_global(ipv6_network.network.prefixlen),
             )
         )
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from ipaddress import IPv6Address, IPv6Network
-from typing import List
+from ipaddress import IPv4Address, IPv4Network
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
-class IPv6PrefixListEntry(BaseModel):
+class PrefixListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    ipv6_address: Global[IPv6Address] = Field(serialization_alias="ipv6Address", validation_alias="ipv6Address")
-    ipv6_prefix_length: Global[int] = Field(serialization_alias="ipv6PrefixLength", validation_alias="ipv6PrefixLength")
+    ipv4_address: Global[IPv4Address] = Field(serialization_alias="ipv4Address", validation_alias="ipv4Address")
+    ipv4_prefix_length: Global[int] = Field(serialization_alias="ipv4PrefixLength", validation_alias="ipv4PrefixLength")
 
 
-class IPv6PrefixListParcel(_ParcelBase):
-    entries: List[IPv6PrefixListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
+class PrefixListParcel(_ParcelBase):
+    type_: Literal["prefix"] = Field(default="prefix", exclude=True)
+    entries: List[PrefixListEntry] = Field(default_factory=list, validation_alias=AliasPath("data", "entries"))
 
-    def add_prefix(self, ipv6_network: IPv6Network):
+    def add_prefix(self, ipv4_network: IPv4Network):
         self.entries.append(
-            IPv6PrefixListEntry(
-                ipv6_address=as_global(ipv6_network.network_address),
-                ipv6_prefix_length=as_global(ipv6_network.prefixlen),
+            PrefixListEntry(
+                ipv4_address=as_global(ipv4_network.network_address),
+                ipv4_prefix_length=as_global(ipv4_network.prefixlen),
             )
         )
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
-from catalystwan.models.policy.lists_entries import PolicerExceedAction
 
+PolicerExceedAction = Literal[
+    "drop",
+    "remark",
+]
 
-class PolicierEntry(BaseModel):
+
+class PolicerEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     burst: Global[int]
     exceed: Global[PolicerExceedAction]
     rate: Global[int]
 
     @field_validator("burst")
     @classmethod
@@ -23,18 +27,19 @@
     @field_validator("rate")
     @classmethod
     def check_rate(cls, rate_str: Global):
         assert 8 <= rate_str.value <= 100_000_000_000
         return rate_str
 
 
-class PolicierParcel(_ParcelBase):
-    entries: List[PolicierEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
+class PolicerParcel(_ParcelBase):
+    type_: Literal["policer"] = Field(default="policer", exclude=True)
+    entries: List[PolicerEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_entry(self, burst: int, exceed: PolicerExceedAction, rate: int):
         self.entries.append(
-            PolicierEntry(
+            PolicerEntry(
                 burst=as_global(burst),
                 exceed=as_global(exceed, PolicerExceedAction),
                 rate=as_global(rate),
             )
         )
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Optional
+from typing import List, Literal, Optional
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, model_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import TLOCColor
-from catalystwan.models.policy.lists_entries import PathPreference
+
+PathPreference = Literal[
+    "direct-path",
+    "multi-hop-path",
+    "all-paths",
+]
 
 
 class Preference(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    color_preference: Global[list] = Field(serialization_alias="colorPreference", validation_alias="colorPreference")
+    color_preference: Global[List[TLOCColor]] = Field(
+        serialization_alias="colorPreference", validation_alias="colorPreference"
+    )
     path_preference: Global[PathPreference] = Field(
         serialization_alias="pathPreference", validation_alias="pathPreference"
     )
 
 
 class PreferredColorGroupEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
@@ -33,32 +40,35 @@
     def check_passwords_match(self) -> "PreferredColorGroupEntry":
         if not self.secondary_preference and self.tertiary_preference:
             raise ValueError("Preference Entry has to have a secondary prefrence when assigning tertiary preference.")
         return self
 
 
 class PreferredColorGroupParcel(_ParcelBase):
+    type_: Literal["preferred-color-group"] = Field(default="preferred-color-group", exclude=True)
     entries: List[PreferredColorGroupEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_primary(self, color_preference: List[TLOCColor], path_preference: PathPreference):
         self.entries.append(
             PreferredColorGroupEntry(
                 primary_preference=Preference(
-                    color_preference=as_global(color_preference),
+                    color_preference=Global[List[TLOCColor]](value=color_preference),
                     path_preference=as_global(path_preference, PathPreference),
                 ),
                 secondary_preference=None,
                 tertiary_preference=None,
             )
         )
 
     def add_secondary(self, color_preference: List[TLOCColor], path_preference: PathPreference):
         preferred_color = self.entries[0]
         preferred_color.secondary_preference = Preference(
-            color_preference=as_global(color_preference), path_preference=as_global(path_preference, PathPreference)
+            color_preference=Global[List[TLOCColor]](value=color_preference),
+            path_preference=as_global(path_preference, PathPreference),
         )
 
     def add_tertiary(self, color_preference: List[TLOCColor], path_preference: PathPreference):
         preferred_color = self.entries[0]
         preferred_color.tertiary_preference = Preference(
-            color_preference=as_global(color_preference), path_preference=as_global(path_preference, PathPreference)
+            color_preference=Global[List[TLOCColor]](value=color_preference),
+            path_preference=as_global(path_preference, PathPreference),
         )
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from ipaddress import IPv4Address, IPv4Network
-from typing import List
+from typing import List, Literal, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
-class PrefixListEntry(BaseModel):
+class SecurityApplicationListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    ipv4_address: Global[IPv4Address] = Field(serialization_alias="ipv4Address", validation_alias="ipv4Address")
-    ipv4_prefix_length: Global[int] = Field(serialization_alias="ipv4PrefixLength", validation_alias="ipv4PrefixLength")
+    app_list: Global[str] = Field(serialization_alias="app", validation_alias="app")
 
 
-class PrefixListParcel(_ParcelBase):
-    entries: List[PrefixListEntry] = Field(default_factory=list, validation_alias=AliasPath("data", "entries"))
+class SecurityApplicationFamilyListEntry(BaseModel):
+    model_config = ConfigDict(populate_by_name=True)
+    app_list_family: Global[str] = Field(serialization_alias="appFamily", validation_alias="appFamily")
+
+
+class SecurityApplicationListParcel(_ParcelBase):
+    type_: Literal["security-localapp"] = Field(default="security-localapp", exclude=True)
+    entries: List[Union[SecurityApplicationFamilyListEntry, SecurityApplicationListEntry]] = Field(
+        default=[], validation_alias=AliasPath("data", "entries")
+    )
+
+    def add_application(self, application: str):
+        self.entries.append(SecurityApplicationListEntry(app_list=as_global(application)))
 
-    def add_prefix(self, ipv4_network: IPv4Network):
-        self.entries.append(
-            PrefixListEntry(
-                ipv4_address=as_global(ipv4_network.network_address),
-                ipv4_prefix_length=as_global(ipv4_network.prefixlen),
-            )
-        )
+    def add_application_family(self, application_family: str):
+        self.entries.append(SecurityApplicationFamilyListEntry(app_list_family=as_global(application_family)))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     # validators
     _jitter_validator = field_validator("jitter")(check_jitter_ms)
     _latency_validator = field_validator("latency")(check_latency_ms)
     _loss_validator = field_validator("loss")(check_loss_percent)
 
 
 class SLAClassParcel(_ParcelBase):
+    type_: Literal["sla-class"] = Field(default="sla-class", exclude=True)
     entries: List[SLAClassListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_entry(
         self,
         app_probe_class_id: UUID,
         loss: Optional[int] = None,
         jitter: Optional[int] = None,
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import WellKnownBGPCommunities
 
 
 class StandardCommunityEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    standard_community: Global[WellKnownBGPCommunities] = Field(
+    standard_community: Global[str] = Field(
         serialization_alias="standardCommunity", validation_alias="standardCommunity"
     )
 
 
 class StandardCommunityParcel(_ParcelBase):
+    type_: Literal["standard-community"] = Field(default="standard-community", exclude=True)
     entries: List[StandardCommunityEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
-    def add_community(self, standard_community: WellKnownBGPCommunities):
-        self.entries.append(
-            StandardCommunityEntry(standard_community=as_global(standard_community, WellKnownBGPCommunities))
-        )
+    def _add_community(self, standard_community: str):
+        self.entries.append(StandardCommunityEntry(standard_community=as_global(standard_community)))
+
+    def add_well_known_community(self, standard_community: WellKnownBGPCommunities):
+        self._add_community(standard_community)
+
+    def add_community(self, as_number: int, community_number: int) -> None:
+        self._add_community(f"{as_number}:{community_number}")
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from ipaddress import IPv4Address
-from typing import List, Optional
+from typing import List, Literal, Optional
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import TLOCColor
-from catalystwan.models.policy.lists_entries import EncapType
+
+EncapType = Literal[
+    "ipsec",
+    "gre",
+]
 
 
 class TlocEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     tloc: Global[IPv4Address]
     color: Global[TLOCColor]
     encapsulation: Global[EncapType] = Field(serialization_alias="encap", validation_alias="encap")
@@ -24,14 +28,15 @@
             return v
         if not (0 <= int(v.value) < 4_294_967_295):
             raise ValueError('"preference" not in range 0 - 4 294 967 295 (2 ** 32 - 1)')
         return v
 
 
 class TlocParcel(_ParcelBase):
+    type_: Literal["tloc"] = Field(default="tloc", exclude=True)
     entries: List[TlocEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_entry(
         self, tloc: IPv4Address, color: TLOCColor, encapsulation: EncapType, preference: Optional[str] = None
     ):
         self.entries.append(
             TlocEntry(
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from ipaddress import IPv4Network
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
-class SecurityDataPrefixEntry(BaseModel):
+class AsPathEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    ip_prefix: Global[IPv4Network] = Field(serialization_alias="ipPrefix", validation_alias="ipPrefix")
+    as_path: Global[str] = Field(validation_alias="asPath", serialization_alias="asPath")
 
 
-class SecurityDataPrefixParcel(_ParcelBase):
-    entries: List[SecurityDataPrefixEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
+class AsPathParcel(_ParcelBase):
+    type_: Literal["as-path"] = Field(default="as-path", exclude=True)
+    as_path_list_num: Global[int] = Field(validation_alias=AliasPath("data", "asPathListNum"))
+    entries: List[AsPathEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
-    def add_prefix(self, ip_prefix: IPv4Network):
-        self.entries.append(SecurityDataPrefixEntry(ip_prefix=as_global(ip_prefix)))
+    def add_as_path(self, as_path: str):
+        self.entries.append(AsPathEntry(as_path=as_global(as_path)))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
+from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase
 
 
-class FQDNListEntry(BaseModel):
+class MirrorEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    pattern: Global[str] = Field(
-        description="Ex: cisco.com, .*cisco.com, .*.cisco.com. Should not start with '*' or '+'"
-    )
+    remote_dest_ip: Global[str] = Field(validation_alias="remoteDestIp", serialization_alias="remoteDestIp")
+    source_ip: Global[str] = Field(validation_alias="sourceIp", serialization_alias="sourceIp")
 
 
-class FQDNDomainParcel(_ParcelBase):
-    entries: List[FQDNListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
-
-    def from_fqdns(self, fqdns: List[str]):
-        for fqdn in fqdns:
-            self.entries.append(FQDNListEntry(pattern=as_global(fqdn)))
+class MirrorParcel(_ParcelBase):
+    type_: Literal["mirror"] = Field(default="mirror", exclude=True)
+    entries: List[MirrorEntry] = Field(validation_alias=AliasPath("data", "entries"), min_length=1, max_length=1)
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Optional
+from typing import List, Literal, Optional
 
 from pydantic import AliasPath, BaseModel, Field, model_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import check_fields_exclusive
 
 
@@ -17,14 +17,15 @@
     @model_validator(mode="after")
     def check_country_xor_continent(self):
         check_fields_exclusive(self.__dict__, {"country", "continent"}, True)
         return self
 
 
 class GeoLocationListParcel(_ParcelBase):
+    type_: Literal["security-geolocation"] = Field(default="security-geolocation", exclude=True)
     entries: List[GeoLocationListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_country(self, country: str):
         self.entries.append(GeoLocationListEntry(country=as_global(country)))
 
     def add_continent(self, continent: str):
         self.entries.append(GeoLocationListEntry(continent=as_global(continent)))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class IPSSignatureListEntry(BaseModel):
@@ -26,14 +26,15 @@
     @classmethod
     def check_signature_id(cls, signature_id: Global):
         assert 0 <= int(signature_id.value) <= 4294967295
         return signature_id
 
 
 class IPSSignatureParcel(_ParcelBase):
+    type_: Literal["security-ipssignature"] = Field(default="security-ipssignature", exclude=True)
     entries: List[IPSSignatureListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_signature(self, signature: str):
         generator_id, signature_id = signature.split(":")
         self.entries.append(
             IPSSignatureListEntry(
                 generator_id=as_global(generator_id),
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class LocalDomainListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     name_server: Global[str] = Field(
         serialization_alias="nameServer", validation_alias="nameServer", description="Ex: cisco.com, *.cisco.com"
     )
 
 
 class LocalDomainParcel(_ParcelBase):
+    type_: Literal["security-localdomain"] = Field(default="security-localdomain", exclude=True)
     entries: List[LocalDomainListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def from_local_domains(self, domains: List[str]):
         for domain in domains:
             self.entries.append(LocalDomainListEntry(name_server=as_global(domain)))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class ProtocolListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     protocol: Global[str] = Field(serialization_alias="protocolName", validation_alias="protocolName")
 
 
 class ProtocolListParcel(_ParcelBase):
+    type_: Literal["security-protocolname"] = Field(default="security-protocolname", exclude=True)
     entries: List[ProtocolListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_protocol(self, protocol: str):
         self.entries.append(ProtocolListEntry(protocol=as_global(protocol)))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class BaseURLListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     pattern: Global[str]
 
 
-class BaseURLParcel(_ParcelBase):
+class URLParcel(_ParcelBase):
+    type_: Literal["security-urllist"] = Field(default="security-urllist", exclude=True)
+    type: Literal["urlallowed", "urlblocked"]
     entries: List[BaseURLListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_url(self, pattern: str):
         self.entries.append(BaseURLListEntry(pattern=as_global(pattern)))
 
 
-class URLAllowParcel(BaseURLParcel):
-    parcel_type: str = Field(default="urlallowed", validation_alias="type", serialization_alias="type")
+class URLAllowParcel(URLParcel):
+    type_: Literal["security-urllist"] = Field(default="security-urllist", exclude=True)
+    type: Literal["urlallowed"] = "urlallowed"
 
 
-class URLBlockParcel(BaseURLParcel):
-    parcel_type: str = Field(default="urlblocked", validation_alias="type", serialization_alias="type")
+class URLBlockParcel(URLParcel):
+    type_: Literal["security-urllist"] = Field(default="security-urllist", exclude=True)
+    type: Literal["urlblocked"] = "urlblocked"
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Optional
+from typing import List, Literal, Optional
 
 from pydantic import AliasPath, BaseModel, Field, field_validator, model_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import InterfaceType, check_fields_exclusive
 
 
@@ -21,22 +21,23 @@
     @model_validator(mode="after")
     def check_vpn_xor_interface(self):
         check_fields_exclusive(self.__dict__, {"vpn", "interface"}, True)
         return self
 
 
 class SecurityZoneListParcel(_ParcelBase):
+    type_: Literal["security-zone"] = Field(default="security-zone", exclude=True)
     entries: List[SecurityZoneListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_interface(self, interface: InterfaceType):
         self.entries.append(
             SecurityZoneListEntry(
                 interface=as_global(interface, InterfaceType),
             )
         )
 
     def add_vpn(self, vpn: str):
         self.entries.append(
             SecurityZoneListEntry(
-                vpn=as_global(vpn, InterfaceType),
+                vpn=as_global(vpn),
             )
         )
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,20 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
+from __future__ import annotations
 
+from ipaddress import IPv4Address, IPv6Address, IPv6Interface
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field, model_validator
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.common import ServiceChainNumber
+from catalystwan.api.configuration_groups.parcel import Default, Global, _ParcelBase, as_default
 
-Action = Literal[
-    "drop",
-    "accept",
-]
-
-IcmpMessage = Literal[
-    "administratively-prohibited",
-    "dod-host-prohibited",
-    "dod-net-prohibited",
-    "echo",
-    "echo-reply",
-    "echo-reply-no-error",
-    "extended-echo",
-    "extended-echo-reply",
-    "general-parameter-problem",
-    "host-isolated",
-    "host-precedence-unreachable",
-    "host-redirect",
-    "host-tos-redirect",
-    "host-tos-unreachable",
-    "host-unknown",
-    "host-unreachable",
-    "interface-error",
-    "malformed-query",
-    "multiple-interface-match",
-    "net-redirect",
-    "net-tos-redirect",
-    "net-tos-unreachable",
-    "net-unreachable",
-    "network-unknown",
-    "no-room-for-option",
-    "option-missing",
-    "packet-too-big",
-    "parameter-problem",
-    "photuris",
-    "port-unreachable",
-    "precedence-unreachable",
-    "protocol-unreachable",
-    "reassembly-timeout",
-    "redirect",
-    "router-advertisement",
-    "router-solicitation",
-    "source-route-failed",
-    "table-entry-error",
-    "time-exceeded",
-    "timestamp-reply",
-    "timestamp-request",
-    "ttl-exceeded",
-    "unreachable",
-]
-
-Icmp6Message = Literal[
+Action = Literal["drop", "accept"]
+Icmp6Msg = Literal[
     "beyond-scope",
     "cp-advertisement",
     "cp-solicitation",
     "destination-unreachable",
     "dhaad-reply",
     "dhaad-request",
     "echo-reply",
@@ -109,301 +60,383 @@
     "router-solicitation",
     "rpl-control",
     "source-policy",
     "source-route-header",
     "time-exceeded",
     "unreachable",
 ]
+IcmpMsg = Literal[
+    "administratively-prohibited",
+    "dod-host-prohibited",
+    "dod-net-prohibited",
+    "echo",
+    "echo-reply",
+    "echo-reply-no-error",
+    "extended-echo",
+    "extended-echo-reply",
+    "general-parameter-problem",
+    "host-isolated",
+    "host-precedence-unreachable",
+    "host-redirect",
+    "host-tos-redirect",
+    "host-tos-unreachable",
+    "host-unknown",
+    "host-unreachable",
+    "interface-error",
+    "malformed-query",
+    "multiple-interface-match",
+    "net-redirect",
+    "net-tos-redirect",
+    "net-tos-unreachable",
+    "net-unreachable",
+    "network-unknown",
+    "no-room-for-option",
+    "option-missing",
+    "packet-too-big",
+    "parameter-problem",
+    "photuris",
+    "port-unreachable",
+    "precedence-unreachable",
+    "protocol-unreachable",
+    "reassembly-timeout",
+    "redirect",
+    "router-advertisement",
+    "router-solicitation",
+    "source-route-failed",
+    "table-entry-error",
+    "time-exceeded",
+    "timestamp-reply",
+    "timestamp-request",
+    "ttl-exceeded",
+    "unreachable",
+]
+Tcp = Literal["syn"]
 
 
-class SourceDataIPv4Prefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    source_ip_prefix: Union[Global[str], Variable] = Field(
-        serialization_alias="sourceIpPrefix", validation_alias="sourceIpPrefix"
+class ReferenceId(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
+    ref_id: Global[UUID] = Field(..., serialization_alias="refId", validation_alias="refId")
 
 
-class SourceDataIPv6Prefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    source_ip_prefix: Union[Global[str], Variable] = Field(
-        serialization_alias="sourceIpPrefix", validation_alias="sourceIpPrefix"
+class SourceDataPrefixListReference(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-
-
-class SourceDataIPv4PrefixParcel(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    source_data_prefix_list: Global[UUID] = Field(
-        serialization_alias="sourceDataPrefixList", validation_alias="sourceDataPrefixList"
+    source_data_prefix_list: ReferenceId = Field(
+        ...,
+        serialization_alias="sourceDataPrefixList",
+        validation_alias="sourceDataPrefixList",
+        description="Source Data Prefix Parcel",
     )
 
 
-class SourceDataIPv6PrefixParcel(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    source_data_prefix_list: Global[UUID] = Field(
-        serialization_alias="sourceDataPrefixList", validation_alias="sourceDataPrefixList"
+class SourceDataPrefixIp(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    source_ip_prefix: Global[str] = Field(
+        ...,
+        serialization_alias="sourceIpPrefix",
+        validation_alias="sourceIpPrefix",
+        description="Source Data IP Prefix",
     )
 
 
 class SourcePort(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    source_port: Global[int] = Field(serialization_alias="sourcePort", validation_alias="sourcePort")
-
-
-class DestinationDataIPv4Prefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    destination_ip_prefix: Union[Global[str], Variable] = Field(
-        serialization_alias="destinationIpPrefix", validation_alias="destinationIpPrefix"
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-
-
-class DestinationDataIPv6Prefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    destination_ip_prefix: Union[Global[str], Variable] = Field(
-        serialization_alias="destinationIpPrefix", validation_alias="destinationIpPrefix"
+    source_port: Union[Global[int], Global[str]] = Field(
+        ...,
+        serialization_alias="sourcePort",
+        validation_alias="sourcePort",
+        description="source port range or individual port number",
     )
 
 
-class DestinationDataIPv4PrefixParcel(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    destination_data_prefix_list: Global[UUID] = Field(
-        serialization_alias="destinationDataPrefixList", validation_alias="destinationDataPrefixList"
+class DestinationDataPrefixListReference(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    destination_data_prefix_list: ReferenceId = Field(
+        ...,
+        serialization_alias="destinationDataPrefixList",
+        validation_alias="destinationDataPrefixList",
+        description="Destination Data Prefix Parcel",
     )
 
 
-class DestinationDataIPv6PrefixParcel(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    destination_data_prefix_list: Global[UUID] = Field(
-        serialization_alias="destinationDataPrefixList", validation_alias="destinationDataPrefixList"
+class DestinationDataPrefixIp(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    destination_ip_prefix: Global[IPv6Interface] = Field(
+        ...,
+        serialization_alias="destinationIpPrefix",
+        validation_alias="destinationIpPrefix",
+        description="Destination Data IP Prefix",
     )
 
 
 class DestinationPort(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    destination_port: Global[int] = Field(serialization_alias="destinationPort", validation_alias="destinationPort")
-
-
-TcpState = Literal["syn"]
-
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    destination_port: Union[Global[int], Global[str]] = Field(
+        ...,
+        serialization_alias="destinationPort",
+        validation_alias="destinationPort",
+        description="destination port range or individual port number",
+    )
 
-class IPv4Match(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    dscp: Optional[Global[List[int]]] = None
-    packet_length: Optional[Global[int]] = Field(
-        serialization_alias="packetLength", validation_alias="packetLength", default=None
+class Ipv4MatchEntry(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    dscp: Optional[Global[List[int]]] = Field(default=None, description="DSCP number")
+    packet_length: Optional[Union[Global[int], Global[str]]] = Field(
+        default=None, serialization_alias="packetLength", validation_alias="packetLength", description="Packet Length"
     )
-    protocol: Optional[Global[List[int]]] = None
-    icmp_message: Optional[Global[List[IcmpMessage]]] = Field(
-        serialization_alias="icmpMsg", validation_alias="icmpMsg", default=None
+    protocol: Optional[Global[List[int]]] = Field(
+        default=None, description="protocol number list with at least one item"
     )
-    source_data_prefix: Optional[Union[SourceDataIPv4Prefix, SourceDataIPv4PrefixParcel]] = Field(
-        serialization_alias="sourceDataPrefix", validation_alias="sourceDataPrefix", default=None
+    icmp_msg: Optional[IcmpMsg] = Field(
+        default=None, serialization_alias="icmpMsg", validation_alias="icmpMsg", description="ICMP Message"
+    )
+    source_data_prefix: Optional[Union[SourceDataPrefixListReference, SourceDataPrefixIp]] = Field(
+        default=None, serialization_alias="sourceDataPrefix", validation_alias="sourceDataPrefix"
     )
     source_ports: Optional[List[SourcePort]] = Field(
-        serialization_alias="sourcePorts", validation_alias="sourcePorts", default=None
+        default=None, serialization_alias="sourcePorts", validation_alias="sourcePorts", description="Source Port List"
     )
-    destination_data_prefix: Optional[Union[DestinationDataIPv4Prefix, DestinationDataIPv4PrefixParcel]] = Field(
-        serialization_alias="destinationDataPrefix", validation_alias="destinationDataPrefix", default=None
+    destination_data_prefix: Optional[Union[DestinationDataPrefixListReference, DestinationDataPrefixIp]] = Field(
+        default=None, serialization_alias="destinationDataPrefix", validation_alias="destinationDataPrefix"
     )
     destination_ports: Optional[List[DestinationPort]] = Field(
-        serialization_alias="destinationPorts", validation_alias="destinationPorts", default=None
-    )
-    tcp: Optional[Global[TcpState]] = None
+        default=None,
+        serialization_alias="destinationPorts",
+        validation_alias="destinationPorts",
+        description="Destination Port List",
+    )
+    tcp: Optional[Tcp] = Field(default=None, description="TCP States")
 
 
-class IPv6Match(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
+class Ipv6MatchEntry(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
     next_header: Optional[Global[int]] = Field(
-        serialization_alias="nextHeader", validation_alias="nextHeader", default=None
+        default=None, serialization_alias="nextHeader", validation_alias="nextHeader", description="next header number"
     )
-    packet_length: Optional[Global[int]] = Field(
-        serialization_alias="packetLength", validation_alias="packetLength", default=None
+    packet_length: Optional[Union[Global[int], Global[str]]] = Field(
+        default=None, serialization_alias="packetLength", validation_alias="packetLength", description="Packet Length"
     )
-    source_data_prefix: Optional[Union[SourceDataIPv6Prefix, SourceDataIPv6PrefixParcel]] = Field(
-        serialization_alias="sourceDataPrefix", validation_alias="sourceDataPrefix", default=None
+    source_data_prefix: Optional[Union[SourceDataPrefixListReference, SourceDataPrefixIp]] = Field(
+        default=None, serialization_alias="sourceDataPrefix", validation_alias="sourceDataPrefix"
     )
     source_ports: Optional[List[SourcePort]] = Field(
-        serialization_alias="sourcePorts", validation_alias="sourcePorts", default=None
+        default=None, serialization_alias="sourcePorts", validation_alias="sourcePorts", description="Source Port List"
     )
-    destination_data_prefix: Optional[Union[DestinationDataIPv6Prefix, DestinationDataIPv6PrefixParcel]] = Field(
-        serialization_alias="destinationDataPrefix", validation_alias="destinationDataPrefix", default=None
+    destination_data_prefix: Optional[Union[DestinationDataPrefixListReference, DestinationDataPrefixIp]] = Field(
+        default=None, serialization_alias="destinationDataPrefix", validation_alias="destinationDataPrefix"
     )
     destination_ports: Optional[List[DestinationPort]] = Field(
-        serialization_alias="destinationPorts", validation_alias="destinationPorts", default=None
-    )
-    tcp: Optional[Global[TcpState]] = None
-    traffic_class: Optional[Global[int]] = None
-    icmp6_message: Optional[Global[List[Icmp6Message]]] = Field(
-        serialization_alias="icmpMsg", validation_alias="icmpMsg", default=None
+        default=None,
+        serialization_alias="destinationPorts",
+        validation_alias="destinationPorts",
+        description="Destination Port List",
+    )
+    tcp: Optional[Global[Tcp]] = Field(default=None, description="TCP States")
+    traffic_class: Optional[Global[List[int]]] = Field(
+        default=None,
+        serialization_alias="trafficClass",
+        validation_alias="trafficClass",
+        description="Select Traffic Class",
+    )
+    icmp6_msg: Optional[Global[List[Icmp6Msg]]] = Field(
+        default=None, serialization_alias="icmp6Msg", validation_alias="icmp6Msg", description="ICMP6 Message"
     )
 
 
-class ServiceChain(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    service_chain_number: Union[Global[ServiceChainNumber], Variable] = Field(
-        serialization_alias="serviceChainNumber", validation_alias="serviceChainNumber"
+class Ipv4AcceptAction(BaseModel):
+    """
+    Accept Action
+    """
+
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    vpn: Optional[Union[Global[int], Variable]] = None
-    fallback: Optional[Union[Global[bool], Variable, Default[bool]]] = None
-
-
-class AcceptActionIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    set_dscp: Optional[Global[int]] = Field(serialization_alias="setDscp", validation_alias="setDscp", default=None)
-    counter_name: Optional[Global[str]] = Field(
-        serialization_alias="counterName", validation_alias="counterName", default=None
+    set_dscp: Optional[Global[int]] = Field(
+        default=None, serialization_alias="setDscp", validation_alias="setDscp", description="DSCP number"
     )
-    log: Optional[Union[Global[bool], Default[bool]]] = None
-    set_next_hop: Optional[Global[str]] = Field(
-        serialization_alias="setNextHop", validation_alias="setNextHop", default=None
+    counter_name: Optional[Global[str]] = Field(
+        default=None, serialization_alias="counterName", validation_alias="counterName", description="Counter Name"
     )
-    set_service_chain: Optional[ServiceChain] = Field(
-        serialization_alias="setServiceChain", validation_alias="setServiceChain", default=None
+    log: Union[Global[bool], Default[bool]] = Field(default=as_default(False), description="Enable log")
+    set_next_hop: Optional[Global[IPv4Address]] = Field(
+        default=None,
+        serialization_alias="setNextHop",
+        validation_alias="setNextHop",
+        description="Set Next Hop (IPV4 address)",
+    )
+    mirror: Optional[ReferenceId] = Field(default=None, description="Select a Mirror Parcel UUID")
+    policer: Optional[ReferenceId] = Field(default=None, description="Select a Policer Parcel")
+
+
+class Ipv6AcceptAction(BaseModel):
+    """
+    Accept Action
+    """
+
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    mirror: Optional[Global[UUID]] = None
-    policer: Optional[Global[UUID]] = None
-
-
-class AcceptActionIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
     counter_name: Optional[Global[str]] = Field(
-        serialization_alias="counterName", validation_alias="counterName", default=None
-    )
-    log: Optional[Union[Global[bool], Default[bool]]] = None
-    set_next_hop: Optional[Global[str]] = Field(
-        serialization_alias="setNextHop", validation_alias="setNextHop", default=None
+        default=None, serialization_alias="counterName", validation_alias="counterName", description="Counter Name"
     )
-    set_service_chain: Optional[ServiceChain] = Field(
-        serialization_alias="setServiceChain", validation_alias="setServiceChain", default=None
+    log: Union[Global[bool], Default[bool]] = Field(default=as_default(False), description="Enable log")
+    set_next_hop: Optional[Global[IPv6Address]] = Field(
+        default=None,
+        serialization_alias="setNextHop",
+        validation_alias="setNextHop",
+        description="Set Next Hop (IPV6 address)",
     )
     set_traffic_class: Optional[Global[int]] = Field(
-        serialization_alias="setTrafficClass", validation_alias="setTrafficClass", default=None
+        default=None,
+        serialization_alias="setTrafficClass",
+        validation_alias="setTrafficClass",
+        description="set traffic class number",
     )
-    mirror: Optional[Global[UUID]] = None
-    policer: Optional[Global[UUID]] = None
+    mirror: Optional[ReferenceId] = Field(default=None, description="Select a Mirror Parcel UUID")
+    policer: Optional[ReferenceId] = Field(default=None, description="Select a Policer Parcel")
 
 
-class DropAction(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    counter_name: Optional[Global[str]] = Field(
-        serialization_alias="counterName", validation_alias="counterName", default=None
+class Ipv4AcceptActions(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    log: Optional[Union[Global[bool], Default[bool]]] = None
-
-
-class AcceptActionsIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    accept: AcceptActionIPv4
-
-
-class AcceptActionsIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    accept: AcceptActionIPv6
-
-
-class DropActions(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    accept: Ipv4AcceptAction = Field(..., description="Accept Action")
 
-    drop: DropAction
 
+class Ipv6AcceptActions(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    accept: Ipv6AcceptAction = Field(..., description="Accept Action")
 
-class IPv4SequenceBaseAction(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    sequence_id: Global[int] = Field(serialization_alias="sequenceId", validation_alias="sequenceId")
-    sequence_name: Global[str] = Field(serialization_alias="sequenceName", validation_alias="sequenceName")
-    base_action: Union[Global[Action], Default[Action]] = Field(
-        serialization_alias="baseAction", validation_alias="baseAction", default=Default[Action](value="accept")
+class DropAction(BaseModel):
+    """
+    Drop Action
+    """
+
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    match_entries: Optional[List[IPv4Match]] = Field(
-        serialization_alias="matchEntries", validation_alias="matchEntries", default=None
+    counter_name: Optional[Global[str]] = Field(
+        default=None, serialization_alias="counterName", validation_alias="counterName", description="Counter Name"
     )
+    log: Union[Global[bool], Default[bool]] = Field(default=as_default(False), description="Enable log")
 
 
-class IPv6SequenceBaseAction(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    sequence_id: Global[int] = Field(serialization_alias="sequenceId", validation_alias="sequenceId")
-    sequence_name: Global[str] = Field(serialization_alias="sequenceName", validation_alias="sequenceName")
-    base_action: Union[Global[Action], Default[Action]] = Field(
-        serialization_alias="baseAction", validation_alias="baseAction", default=Default[Action](value="accept")
-    )
-    match_entries: Optional[List[IPv6Match]] = Field(
-        serialization_alias="matchEntries", validation_alias="matchEntries", default=None
+class DropActions(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
+    drop: DropAction = Field(..., description="Drop Action")
 
 
-class IPv4SequenceActions(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    sequence_id: Global[int] = Field(serialization_alias="sequenceId", validation_alias="sequenceId")
-    sequence_name: Global[str] = Field(serialization_alias="sequenceName", validation_alias="sequenceName")
-    actions: List[Union[AcceptActionsIPv4, DropActions]] = Field(
-        serialization_alias="actions", validation_alias="actions"
+class Sequences(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    match_entries: Optional[List[IPv4Match]] = Field(
-        serialization_alias="matchEntries", validation_alias="matchEntries", default=None
+    sequence_id: Global[int] = Field(
+        ..., serialization_alias="sequenceId", validation_alias="sequenceId", description="Sequence Id"
     )
-
-
-class IPv6SequenceActions(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    sequence_id: Global[int] = Field(serialization_alias="sequenceId", validation_alias="sequenceId")
-    sequence_name: Global[str] = Field(serialization_alias="sequenceName", validation_alias="sequenceName")
-    actions: List[Union[AcceptActionsIPv6, DropActions]] = Field(
-        serialization_alias="actions", validation_alias="actions"
+    sequence_name: Global[str] = Field(
+        ..., serialization_alias="sequenceName", validation_alias="sequenceName", description="Sequence Name"
     )
-    match_entries: Optional[List[IPv6Match]] = Field(
-        serialization_alias="matchEntries", validation_alias="matchEntries", default=None
+    base_action: Optional[Union[Global[Action], Default[Action]]] = Field(
+        default=None, serialization_alias="baseAction", validation_alias="baseAction", description="Base Action"
+    )
+    match_entries: Optional[List[Ipv6MatchEntry]] = Field(
+        default=None,
+        serialization_alias="matchEntries",
+        validation_alias="matchEntries",
+        description="Define match conditions",
+        max_length=1,
+        min_length=1,
     )
 
+    @model_validator(mode="after")
+    def check_fields_at_least_one_assigned(self):
+        """There are two Sequence models in schema,
+        one with set base_action and empty actions,
+        and one with set actions and empty base_action,
+        so we combine two models into one model with check if
+        at least one field assigned
+        """
+        if self.base_action is None and self.actions is None:
+            self.base_action = as_default("accept", Action)
 
-class IPv4AclData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    defautl_action: Union[Global[Action], Default[Action]] = Field(
-        serialization_alias="defaultAction", validation_alias="defaultAction", default=Default[Action](value="drop")
+class Ipv6Sequences(Sequences):
+    actions: Optional[List[Union[Ipv6AcceptActions, DropActions]]] = Field(
+        default=None, description="Define list of actions", max_length=1, min_length=1
     )
-    sequences: List[Union[IPv4SequenceBaseAction, IPv4SequenceActions]]
-
-
-class IPv4AclCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    name: str
-    description: Optional[str] = None
-    data: IPv4AclData
 
+class Ipv4Sequences(Sequences):
+    actions: Optional[List[Union[Ipv4AcceptActions, DropActions]]] = Field(
+        default=None, description="Define list of actions", max_length=1, min_length=1
+    )
 
-class IPv6AclData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    defautl_action: Union[Global[Action], Default[Action]] = Field(
-        serialization_alias="defaultAction", validation_alias="defaultAction", default=Default[Action](value="drop")
+class Ipv4AclParcel(_ParcelBase):
+    type_: Literal["ipv4-acl"] = Field(default="ipv4-acl", exclude=True)
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    default_action: Union[Global[Action], Global[Action]] = Field(
+        as_default("drop", Action),
+        validation_alias=AliasPath("data", "defaultAction"),
+        description="Default Action",
+    )
+    sequences: List[Union[Ipv4Sequences]] = Field(
+        default_factory=list, validation_alias=AliasPath("data", "sequences"), description="Access Control List"
     )
-    sequences: List[Union[IPv6SequenceBaseAction, IPv6SequenceActions]]
-
 
-class IPv6AclCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    name: str
-    description: Optional[str] = None
-    data: IPv6AclData
+class Ipv6AclParcel(_ParcelBase):
+    type_: Literal["ipv6-acl"] = Field(default="ipv6-acl", exclude=True)
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    default_action: Union[Global[Action], Global[Action]] = Field(
+        as_default("drop", Action),
+        validation_alias=AliasPath("data", "defaultAction"),
+        description="Default Action",
+    )
+    sequences: List[Union[Ipv6Sequences]] = Field(
+        default_factory=list, validation_alias=AliasPath("data", "sequences"), description="Access Control List"
+    )
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,235 +1,172 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Address, IPv6Interface
 from typing import List, Literal, Optional, Union
+from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.configuration.feature_profile.common import Arp, StaticIPv4Address, StaticIPv6Address
+from catalystwan.models.configuration.feature_profile.sdwan.service.lan.common import (
+    VrrpIPv6Address,
+    VrrpTrackingObject,
+)
 
-VirtualApplicationType = Literal["dreopt"]
 
-ResourceProfile = Literal[
-    "small",
-    "medium",
-    "large",
-    "extra-large",
-    "default",
-]
+class VrrpIPv4SecondaryAddress(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-AppqoeDeviceRole = Literal[
-    "forwarder",
-    "forwarderAndServiceNode",
-    "serviceNode",
-    "serviceNodeWithDre",
-    "forwarderAndServiceNodeWithDre",
-]
+    address: Union[Variable, Global[str]]
 
-AppnavControllerGroupName = Literal["ACG-APPQOE"]
-ServiceNodeGroupName = Literal["SNG-APPQOE"]
-ForwarderAndServiceNodeAddress = Literal["192.168.2.2"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
-ForwarderAndServiceNodeControllerAddress = Literal[
-    "192.168.2.1"
-]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
-ServiceNodeExternalAddress = Literal["192.168.2.2"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
-ServiceNodeExternalVpgIp = Literal["192.168.2.1/24"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
 
+class VrrpIPv6SecondaryAddress(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-class VirtualApplication(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    prefix: Union[Global[str], Global[IPv6Interface], Variable]
 
-    instance_id: Global[int] = Field(
-        default=Global(value=1), serialization_alias="instanceId", validation_alias="instanceId"
+
+class VrrpIPv4(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    group_id: Union[Variable, Global[int]] = Field(serialization_alias="groupId", validation_alias="groupId")
+    priority: Union[Variable, Global[int], Default[int]] = Default[int](value=100)
+    timer: Union[Variable, Global[int], Default[int]] = Default[int](value=1000)
+    track_omp: Union[Global[bool], Default[bool]] = Field(
+        serialization_alias="trackOmp", validation_alias="trackOmp", default=Default[bool](value=False)
     )
-    application_type: Global[VirtualApplicationType] = Field(
-        default=Global[VirtualApplicationType](value="dreopt"),
-        serialization_alias="applicationType",
-        validation_alias="applicationType",
+    ip_address: Union[Global[str], Global[IPv4Address], Variable] = Field(
+        serialization_alias="ipAddress", validation_alias="ipAddress"
     )
-    resource_profile: Union[Global[ResourceProfile], Default[str]] = Field(
-        default=Global[ResourceProfile](value="default"),
-        serialization_alias="resourceProfile",
-        validation_alias="resourceProfile",
+    ip_address_secondary: Optional[List[VrrpIPv4SecondaryAddress]] = Field(
+        serialization_alias="ipAddressSecondary", validation_alias="ipAddressSecondary", default=None
     )
-
-
-class Appqoe(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: Default[str] = Default(value="/1")
-    appnav_controller_group: Global[AppnavControllerGroupName] = Field(
-        default=Global[AppnavControllerGroupName](value="ACG-APPQOE"),
-        serialization_alias="appnavControllerGroup",
-        validation_alias="appnavControllerGroup",
+    tloc_pref_change: Union[Global[bool], Default[bool]] = Field(
+        serialization_alias="tlocPrefChange", validation_alias="tlocPrefChange", default=Default[bool](value=False)
     )
-    service_node_group: Global[ServiceNodeGroupName] = Field(
-        default=Global[ServiceNodeGroupName](value="SNG-APPQOE"),
-        serialization_alias="serviceNodeGroup",
-        validation_alias="serviceNodeGroup",
+    tloc_pref_change_value: Optional[Union[Global[int], Variable]] = Field(
+        serialization_alias="tlocPrefChangeValue", validation_alias="tlocPrefChangeValue", default=None
     )
-    service_node_groups: List[Global[ServiceNodeGroupName]] = Field(
-        default=[Global[ServiceNodeGroupName](value="SNG-APPQOE")],
-        serialization_alias="serviceNodeGroups",
-        validation_alias="serviceNodeGroups",
+    tracking_object: Optional[List[VrrpTrackingObject]] = Field(
+        serialization_alias="trackingObject", validation_alias="trackingObject", default=None
     )
-    enable: Global[bool] = Global[bool](value=True)
-    vpn: Union[Global[int], Default[None], Variable] = Field(default=Global[int](value=0))
 
+    prefix_list: Optional[Union[Global[str], Variable, Default[None]]] = Default[None](value=None)
 
-class ServiceContext(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True)
-    appqoe: List[Appqoe]
 
+class VrrpIPv6(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-# Frowarder
-
-
-class ServiceNodeInformation(BaseModel):
-    address: Global[str]
+    group_id: Union[Variable, Global[int]] = Field(serialization_alias="groupId", validation_alias="groupId")
+    priority: Union[Variable, Global[int], Default[int]] = Default[int](value=100)
+    timer: Union[Variable, Global[int], Default[int]] = Default[int](value=1000)
+    track_omp: Union[Global[bool], Default[bool]] = Field(
+        serialization_alias="trackOmp", validation_alias="trackOmp", default=Default[bool](value=False)
+    )
+    track_prefix_list: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="trackPrefixList", validation_alias="trackPrefixList"
+    )
+    ipv6: List[VrrpIPv6Address]
+    ipv6_secondary: Optional[List[VrrpIPv6SecondaryAddress]]
 
 
-class ForwarderController(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class Dhcpv6Helper(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    address: Union[Global[str], Variable]
-    vpn: Global[int] = Global[int](value=1)
+    address: Union[Global[str], Variable] = Field(serialization_alias="address", validation_alias="address")
+    vpn: Optional[Union[Global[int], Variable, Default[None]]] = None
 
 
-class ForwarderAppnavControllerGroup(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class AdvancedSviAttributes(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    group_name: Default[AppnavControllerGroupName] = Field(
-        default=Default(value="ACG-APPQOE"), serialization_alias="groupName", validation_alias="groupName"
+    tcp_mss: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="tcpMss", validation_alias="tcpMss", default=Default[None](value=None)
     )
-    appnav_controllers: List[ForwarderController] = Field(
-        serialization_alias="appnavControllers", validation_alias="appnavControllers"
+    arp_timeout: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="arpTimeout", validation_alias="arpTimeout", default=Default[int](value=1200)
     )
-
-
-class ForwarderNodeGroup(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: Union[Global[str], Default[ServiceNodeGroupName]]
-    internal: Default[bool] = Default[bool](value=False)
-    service_node: List[ServiceNodeInformation] = Field(
-        serialization_alias="serviceNode", validation_alias="serviceNode"
+    ip_directed_broadcast: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="ipDirectedBroadcast",
+        validation_alias="ipDirectedBroadcast",
+        default=Default[bool](value=False),
+    )
+    icmp_redirect_disable: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="icmpRedirectDisable",
+        validation_alias="icmpRedirectDisable",
+        default=Default[bool](value=True),
     )
 
 
-class ForwarderRole(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class IPv4AddressConfiguration(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    appnav_controller_group: List[ForwarderAppnavControllerGroup] = Field(
-        serialization_alias="appnavControllerGroup", validation_alias="appnavControllerGroup"
+    address: StaticIPv4Address = Field(serialization_alias="addressV4", validation_alias="addressV4")
+    secondary_address: Optional[List[StaticIPv4Address]] = Field(
+        serialization_alias="secondaryAddressV4", validation_alias="secondaryAddressV4", default=None
     )
-    service_node_group: List[ForwarderNodeGroup] = Field(
-        serialization_alias="serviceNodeGroup", validation_alias="serviceNodeGroup"
+    dhcp_helper: Optional[Union[Global[List[str]], Variable, Default[None]]] = Field(
+        serialization_alias="dhcpHelperV4", validation_alias="dhcpHelperV4", default=None
     )
-    service_context: ServiceContext = Field(serialization_alias="serviceContext", validation_alias="serviceContext")
-
-
-# Forwarder and Service
 
 
-class ServiceNodeInformationDefault(BaseModel):
-    address: Default[ForwarderAndServiceNodeAddress] = Default[ForwarderAndServiceNodeAddress](value="192.168.2.2")
+class IPv6AddressConfiguration(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-
-class ForwarderAndServiceNodeController(BaseModel):
-    address: Default[ForwarderAndServiceNodeControllerAddress] = Default[ForwarderAndServiceNodeControllerAddress](
-        value="192.168.2.1"
+    address: Union[Global[str], Global[IPv6Interface], Variable, Default[None]] = Field(
+        serialization_alias="addressV6", validation_alias="addressV6"
     )
-
-
-class ForwarderAndServiceNodeAppnavControllerGroup(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    group_name: Default[AppnavControllerGroupName] = Field(
-        default=Default[AppnavControllerGroupName](value="ACG-APPQOE"),
-        serialization_alias="groupName",
-        validation_alias="groupName",
+    secondary_address: Optional[List[StaticIPv6Address]] = Field(
+        serialization_alias="secondaryAddressV6", validation_alias="secondaryAddressV6", default=None
     )
-    appnav_controllers: List[ForwarderAndServiceNodeController] = Field(
-        serialization_alias="appnavControllers", validation_alias="appnavControllers"
+    dhcp_helper: Optional[List[Dhcpv6Helper]] = Field(
+        serialization_alias="dhcpHelperV6", validation_alias="dhcpHelperV6", default=None
     )
 
 
-class ForwarderAndServiceNodeGroup(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class AclQos(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    name: Default[ServiceNodeGroupName] = Default[ServiceNodeGroupName](value="SNG-APPQOE")
-    internal: Default[bool] = Default[bool](value=True)
-    service_node: List[ServiceNodeInformationDefault] = Field(
-        serialization_alias="serviceNode", validation_alias="serviceNode"
+    ipv4_acl_egress: Optional[Global[UUID]] = Field(
+        serialization_alias="ipv4AclEgress", validation_alias="ipv4AclEgress", default=None
     )
-
-
-class ForwarderAndServiceNodeRole(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    appnav_controller_group: List[ForwarderAndServiceNodeAppnavControllerGroup] = Field(
-        serialization_alias="appnavControllerGroup", validation_alias="appnavControllerGroup"
+    ipv4_acl_ingress: Optional[Global[UUID]] = Field(
+        serialization_alias="ipv4AclIngress", validation_alias="ipv4AclIngress", default=None
     )
-    service_node_group: List[ForwarderAndServiceNodeGroup] = Field(
-        serialization_alias="serviceNodeGroup", validation_alias="serviceNodeGroup"
+    ipv6_acl_egress: Optional[Global[UUID]] = Field(
+        serialization_alias="ipv6AclEgress", validation_alias="ipv6AclEgress", default=None
     )
-
-    service_context: ServiceContext = Field(serialization_alias="serviceContext", validation_alias="serviceContext")
-
-
-# Service
-
-
-class ServiceNodeInformationExternal(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    address: Default[ServiceNodeExternalAddress] = Default[ServiceNodeExternalAddress](value="192.168.2.2")
-    vpg_ip: Default[ServiceNodeExternalVpgIp] = Field(
-        default=Default[ServiceNodeExternalVpgIp](value="192.168.2.1"),
-        serialization_alias="vpgIp",
-        validation_alias="vpgIp",
+    ipv6_acl_ingress: Optional[Global[UUID]] = Field(
+        serialization_alias="ipv6AclIngress", validation_alias="ipv6AclIngress", default=None
     )
 
 
-class ServiceNodeGroup(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class InterfaceSviParcel(_ParcelBase):
+    type_: Literal["lan/vpn/interface/svi"] = Field(default="lan/vpn/interface/svi", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    name: Default[ServiceNodeGroupName] = Default[ServiceNodeGroupName](value="SNG-APPQOE")
-    external_node: Default[bool] = Field(
-        default=Default[bool](value=True), serialization_alias="externalNode", validation_alias="externalNode"
+    shutdown: Union[Global[bool], Variable, Default[bool]] = Field(
+        default=Default[bool](value=True), validation_alias=AliasPath("data", "shutdown")
     )
-    service_node: List[ServiceNodeInformationExternal] = Field(
-        default=[ServiceNodeInformationExternal()], serialization_alias="serviceNode", validation_alias="serviceNode"
+    interface_name: Union[Global[str], Variable] = Field(validation_alias=AliasPath("data", "interfaceName"))
+    svi_description: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        default=Default[None](value=None), validation_alias=AliasPath("data", "description")
     )
-
-
-class ServiceNodeRole(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    service_node_group: List[ServiceNodeGroup] = Field(
-        default=[ServiceNodeGroup()], serialization_alias="serviceNodeGroup", validation_alias="serviceNodeGroup"
+    interface_mtu: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "ifMtu"), default=Default[int](value=1500)
     )
-
-
-class AppqoeData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    dreopt: Optional[Union[Global[bool], Default[bool]]] = Default[bool](value=False)
-    virtual_application: Optional[List[VirtualApplication]] = Field(
-        serialization_alias="virtualApplication", validation_alias="virtualApplication"
+    ip_mtu: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "ipMtu"), default=Default[int](value=1500)
     )
-    appqoe_device_role: Global[str] = Field(
-        default=Global(value="forwarder"), serialization_alias="appqoeDeviceRole", validation_alias="appqoeDeviceRole"
+    ipv4: Optional[IPv4AddressConfiguration] = Field(default=None, validation_alias=AliasPath("data", "ipv4"))
+    ipv6: Optional[IPv6AddressConfiguration] = Field(default=None, validation_alias=AliasPath("data", "ipv6"))
+    acl_qos: Optional[AclQos] = Field(validation_alias=AliasPath("data", "aclQos"), default=None)
+    arp: Optional[List[Arp]] = Field(default=None, validation_alias=AliasPath("data", "arp"))
+    vrrp: Optional[List[VrrpIPv4]] = Field(default=None, validation_alias=AliasPath("data", "vrrp"))
+    vrrp_ipv6: Optional[List[VrrpIPv6]] = Field(validation_alias=AliasPath("data", "vrrpIpv6"), default=None)
+    dhcp_client_v6: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        validation_alias=AliasPath("data", "dhcpClientV6"), default=Default[bool](value=False)
     )
-
-    forwarder: Optional[ForwarderRole]
-    forwarder_and_service_node: Optional[ForwarderAndServiceNodeRole] = Field(
-        serialization_alias="forwarderAndServiceNode", validation_alias="forwarderAndServiceNode"
+    advanced: AdvancedSviAttributes = Field(
+        default_factory=AdvancedSviAttributes, validation_alias=AliasPath("data", "advanced")
     )
-    service_node: Optional[ServiceNodeRole] = Field(serialization_alias="serviceNode", validation_alias="serviceNode")
-
-
-class AppqoeCreationPayload(BaseModel):
-    name: str
-    description: Optional[str] = None
-    data: AppqoeData
-    metadata: Optional[dict] = None
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.common import Prefix
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask
 
 
 class AggregatePrefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    prefix: Prefix
+    prefix: AddressWithMask
     as_set: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="asSet", validation_alias="asSet", default=Default[bool](value=False)
     )
     summary_only: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="summaryOnly", validation_alias="summaryOnly", default=Default[bool](value=False)
     )
 
 
 class AggregatePrefixIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     prefix: Union[Global[str], Variable]
     as_set: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="asSet", validation_alias="asSet", default=Default[bool](value=False)
     )
     summary_only: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="summaryOnly", validation_alias="summaryOnly", default=Default[bool](value=False)
     )
 
 
 class NetworkPrefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    prefix: Prefix
+    prefix: AddressWithMask
 
 
 class NetworkPrefixIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     prefix: Union[Global[str], Variable]
 
 
 RedistributeProtocol = Literal[
     "static",
     "connected",
@@ -61,70 +61,70 @@
     "connected",
     "omp",
     "ospf",
 ]
 
 
 class RedistributedRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     protocol: Union[Global[RedistributeProtocol], Variable]
     route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="routePolicy", validation_alias="routePolicy"
     )
 
 
 class RedistributedRouteIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     protocol: Union[Global[RedistributeProtocolIPv6], Variable]
     route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="routePolicy", validation_alias="routePolicy"
     )
 
 
 class AddressFamilyIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     aggregate_address: Optional[List[AggregatePrefix]] = Field(
         serialization_alias="aggregateAddress", validation_alias="aggregateAddress"
     )
     network: Optional[List[NetworkPrefix]] = None
     paths: Optional[Union[Global[int], Variable, Default[None]]] = None
     originate: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     name: Optional[Union[Default[None], Global[UUID]]] = None
     filter: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     redistribute: Optional[List[RedistributedRoute]] = None
 
 
 class PolicyType(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     policy_type: Global[str] = Field(serialization_alias="policyType", validation_alias="policyType")
 
 
 class PolicyTypeWithThreshold(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     policy_type: Global[str] = Field(serialization_alias="policyType", validation_alias="policyType")
     prefix_number: Union[Global[int], Variable] = Field(serialization_alias="prefixNum", validation_alias="prefixNum")
     threshold: Union[Global[int], Variable, Default[int]] = Default[int](value=75)
 
 
 class PolicyTypeWithRestart(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     policy_type: Global[str] = Field(serialization_alias="policyType", validation_alias="policyType")
     prefix_number: Union[Global[int], Variable] = Field(serialization_alias="prefixNum", validation_alias="prefixNum")
     threshold: Union[Global[int], Variable, Default[int]] = Default[int](value=75)
     restart_interval: Union[Global[int], Variable]
 
 
 class AddressFamilyIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     aggregate_address: Optional[List[AggregatePrefixIPv6]] = Field(
         serialization_alias="ipv6AggregateAddress", validation_alias="ipv6AggregateAddress"
     )
     network: Optional[List[NetworkPrefixIPv6]] = Field(
         serialization_alias="ipv6Network", validation_alias="ipv6Network"
     )
@@ -132,30 +132,30 @@
     originate: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     name: Optional[Union[Default[None], Global[UUID]]] = None
     filter: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     redistribute: Optional[List[RedistributedRouteIPv6]] = None
 
 
 class BgpAddressFamily(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     family_type: Global[str] = Field(serialization_alias="familyType", validation_alias="familyType")
     max_prefix_config: Optional[Union[PolicyType, PolicyTypeWithRestart, PolicyTypeWithThreshold]] = Field(
         serialization_alias="maxPrefixConfig", validation_alias="maxPrefixConfig"
     )
     in_route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="inRoutePolicy", validation_alias="inRoutePolicy"
     )
     out_route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="outRoutePolicy", validation_alias="outRoutePolicy"
     )
 
 
 class BgpIPv4Neighbor(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     address: Union[Global[str], Variable]
     description: Optional[Union[Global[str], Variable, Default[None]]] = None
     shutdown: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     remote_as: Union[Global[int], Variable] = Field(serialization_alias="remoteAs", validation_alias="remoteAs")
     local_as: Union[Global[int], Variable] = Field(
         serialization_alias="localAs", validation_alias="localAs", default=None
@@ -189,15 +189,15 @@
     )
     address_family: Optional[BgpAddressFamily] = Field(
         serialization_alias="addressFamily", validation_alias="addressFamily"
     )
 
 
 class BgpIPv6Neighbor(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     address: Union[Global[str], Variable]
     description: Optional[Union[Global[str], Variable, Default[None]]] = None
     shutdown: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     remote_as: Union[Global[int], Variable] = Field(serialization_alias="remoteAs", validation_alias="remoteAs")
     local_as: Union[Global[int], Variable] = Field(
         serialization_alias="localAs", validation_alias="localAs", default=None
@@ -230,59 +230,61 @@
         serialization_alias="asNumber", validation_alias="asNumber", default=None
     )
     address_family: Optional[BgpAddressFamily] = Field(
         serialization_alias="addressFamily", validation_alias="addressFamily"
     )
 
 
-class BgpData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    as_num: Union[Global[int], Variable] = Field(serialization_alias="asNum", validation_alias="asNum")
+class BgpParcel(_ParcelBase):
+    type_: Literal["routing/bgp"] = Field(default="routing/bgp", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+    as_num: Union[Global[int], Variable] = Field(validation_alias=AliasPath("data", "asNum"))
     router_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="routerId", validation_alias="routerId", default=None
+        validation_alias=AliasPath("data", "routerId"), default=None
     )
     propagate_aspath: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="propagateAspath", validation_alias="propagateAspath", default=Default[bool](value=False)
+        validation_alias=AliasPath("data", "propagateAspath"), default=Default[bool](value=False)
     )
     propagate_community: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="propagateCommunity",
-        validation_alias="propagateCommunity",
+        validation_alias=AliasPath("data", "propagateCommunity"),
         default=Default[bool](value=False),
     )
-    external: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=20)
-    internal: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=200)
-    local: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=20)
-    keepalive: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=60)
-    holdtime: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=180)
+    external: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "external"), default=Default[int](value=20)
+    )
+    internal: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "internal"), default=Default[int](value=200)
+    )
+    local: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "local"), default=Default[int](value=20)
+    )
+    keepalive: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "keepalive"), default=Default[int](value=60)
+    )
+    holdtime: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "holdtime"), default=Default[int](value=180)
+    )
     always_compare: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="alwaysCompare", validation_alias="alwaysCompare", default=Default[bool](value=False)
+        validation_alias=AliasPath("data", "alwaysCompare"), default=Default[bool](value=False)
+    )
+    deterministic: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        validation_alias=AliasPath("data", "deterministic"), default=Default[bool](value=False)
     )
-    deterministic: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     missing_as_worst: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="missingAsWorst", validation_alias="missingAsWorst", default=Default[bool](value=False)
+        validation_alias=AliasPath("data", "missingAsWorst"), default=Default[bool](value=False)
     )
     compare_router_id: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="compareRouterId", validation_alias="compareRouterId", default=Default[bool](value=False)
+        validation_alias=AliasPath("data", "compareRouterId"), default=Default[bool](value=False)
     )
     multipath_relax: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="multipathRelax", validation_alias="multipathRelax", default=Default[bool](value=False)
+        validation_alias=AliasPath("data", "multipathRelax"), default=Default[bool](value=False)
     )
-    neighbor: Optional[List[BgpIPv4Neighbor]] = None
+    neighbor: Optional[List[BgpIPv4Neighbor]] = Field(validation_alias=AliasPath("data", "neighbor"), default=None)
     ipv6_neighbor: Optional[List[BgpIPv6Neighbor]] = Field(
-        serialization_alias="ipv6Neighbor", validation_alias="ipv6Neighbor", default=None
+        validation_alias=AliasPath("data", "ipv6Neighbor"), default=None
     )
     address_family: Optional[AddressFamilyIPv4] = Field(
-        serialization_alias="addressFamily", validation_alias="addressFamily", default=None
+        validation_alias=AliasPath("data", "addressFamily"), default=None
     )
     ipv6_address_family: Optional[AddressFamilyIPv6] = Field(
-        serialization_alias="ipv6AddressFamily", validation_alias="ipv6AddressFamily", default=None
+        validation_alias=AliasPath("data", "ipv6AddressFamily"), default=None
     )
-
-
-class BgpCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: BgpData
-    metadata: Optional[dict] = None
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,74 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
+from __future__ import annotations
 
-from typing import List, Optional, Union
+from typing import List, Literal, Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default
 
+EnableMrfMigration = Literal["enabled", "enabled-from-bgp-core"]
+Role = Literal["edge-router", "border-router"]
 
-class OptionCodeAscii(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    code: Union[Global[int], Variable]
-    ascii: Union[Global[str], Variable]
-
-
-class OptionCodeHex(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    code: Union[Global[int], Variable]
-    hex: Union[Global[str], Variable]
-
-
-class OptionCodeIP(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    code: Union[Global[int], Variable]
-    ip: Union[Global[List[str]], Variable]
-
-
-class StaticLease(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    mac_address: Union[Global[str], Variable] = Field(serialization_alias="macAddress", validation_alias="macAddress")
-    ip: Union[Global[str], Variable]
-
-
-class DhcpAddressPool(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    network_address: Union[Global[str], Variable] = Field(
-        serialization_alias="networkAddress", validation_alias="networkAddress"
+class ManagementRegion(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    vrf_id: Union[Global[int], Default[None], Variable] = Field(
+        default=Default[None](value=None),
+        serialization_alias="vrfId",
+        validation_alias="vrfId",
+        description="VRF name for management region",
+    )
+    gateway_preference: Optional[Union[Global[List[int]], Default[None], Variable]] = Field(
+        default=Default[None](value=None),
+        serialization_alias="gatewayPreference",
+        validation_alias="gatewayPreference",
+        description="List of affinity group preferences for VRF",
+    )
+    management_gateway: Union[Global[bool], Default[bool], Variable] = Field(
+        default=as_default(False),
+        serialization_alias="managementGateway",
+        validation_alias="managementGateway",
+        description="Enable management gateway",
     )
-    subnet_mask: Union[Global[str], Variable] = Field(serialization_alias="subnetMask", validation_alias="subnetMask")
 
 
-class DhcpServerData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class MRFParcel(_ParcelBase):
+    type_: Literal["mrf"] = Field(default="mrf", exclude=True)
 
-    address_pool: DhcpAddressPool = Field(serialization_alias="addressPool", validation_alias="addressPool")
-    exclude: Optional[Union[Global[List[str]], Variable, Default[None]]] = None
-    lease_time: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="leaseTime", validation_alias="leaseTime", default=Default[int](value=86400)
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    interface_mtu: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="interfaceMtu", validation_alias="interfaceMtu", default=None
+    secondary_region: Union[Global[int], Variable, Default[None]] = Field(
+        default=Default[None](value=None),
+        validation_alias=AliasPath("data", "secondaryRegion"),
+        description="Set secondary region ID",
     )
-    domain_name: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="domainName", validation_alias="domainName", default=None
+    role: Union[Global[Role], Variable, Default[None]] = Field(
+        default=Default[None](value=None),
+        validation_alias=AliasPath("data", "role"),
+        description="Set the role for router",
     )
-    default_gateway: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="defaultGateway", validation_alias="defaultGateway", default=None
+    enable_mrf_migration: Union[Global[EnableMrfMigration], Default[None]] = Field(
+        default=Default[None](value=None),
+        validation_alias=AliasPath("data", "enableMrfMigration"),
+        description="Enable migration mode to Multi-Region Fabric",
     )
-    dns_servers: Optional[Union[Global[List[str]], Variable, Default[None]]] = Field(
-        serialization_alias="dnsServers", validation_alias="dnsServers", default=None
+    migration_bgp_community: Optional[Union[Global[int], Default[None]]] = Field(
+        default=Default[None](value=None),
+        validation_alias=AliasPath("data", "migrationBgpCommunity"),
+        description="Set BGP community during migration from BGP-core based network",
     )
-    tftp_servers: Optional[Union[Global[List[str]], Variable, Default[None]]] = Field(
-        serialization_alias="tftpServers", validation_alias="tftpServers", default=None
+    enable_management_region: Union[Global[bool], Default[bool], Variable] = Field(
+        default=as_default(False),
+        validation_alias=AliasPath("data", "enableManagementRegion"),
+        description="Enable management region",
     )
-    static_lease: Optional[List[StaticLease]] = Field(
-        serialization_alias="staticLease", validation_alias="staticLease", default=None
+    management_region: ManagementRegion = Field(
+        default_factory=ManagementRegion,
+        validation_alias=AliasPath("data", "managementRegion"),
+        description="Management Region",
     )
-    option_code: Optional[List[Union[OptionCodeAscii, OptionCodeHex, OptionCodeIP]]] = Field(
-        serialization_alias="optionCode", validation_alias="optionCode", default=None
-    )
-
-
-class DhcpSeverCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: DhcpServerData
-    metadata: Optional[dict] = None
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.common import Prefix
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask
 
 EigrpAuthType = Literal[
     "md5",
     "hmac-sha-256",
 ]
 
 
@@ -22,85 +22,81 @@
     "ospf",
     "ospfv3",
     "static",
 ]
 
 
 class KeychainDetails(BaseModel):
-    key_id: Union[Global[int], Variable, Default[None]] = Field(serialization_alias="keyId", validation_alias="keyId")
-    keystring: Union[Global[str], Variable, Default[None]]
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    key_id: Union[Global[int], Variable, Default[None]] = Field(
+        default=Default[None](value=None), serialization_alias="keyId", validation_alias="keyId"
+    )
+    keystring: Union[Global[str], Variable, Default[None]] = Field(default=Default[None](value=None))
 
 
 class EigrpAuthentication(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    auth_type: Union[Global[EigrpAuthType], Variable, Default[None]] = Field(
-        serialization_alias="type", validation_alias="type"
-    )
+    auth_type: Union[Global[EigrpAuthType], Variable, Default[None]] = Default[None](value=None)
     auth_key: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="authKey", validation_alias="authKey"
+        serialization_alias="authKey", validation_alias="authKey", default=Default[None](value=None)
     )
-    key: Optional[List[KeychainDetails]] = Field(serialization_alias="key", validation_alias="key")
+    key: Optional[List[KeychainDetails]] = None
 
 
 class TableMap(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     name: Optional[Union[Default[None], Global[UUID]]] = Default[None](value=None)
     filter: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
 
 
 class SummaryAddress(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    prefix: Prefix
+    prefix: AddressWithMask
 
 
 class IPv4StaticRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     name: Union[Global[str], Variable]
-    shutdown: Optional[Union[Global[int], Variable, Default[bool]]] = Default[bool](value=False)
-    summary_address: Optional[List[SummaryAddress]] = Field(
-        serialization_alias="summaryAddress", validation_alias="summaryAddress"
+    shutdown: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
+    summary_address: List[SummaryAddress] = Field(
+        serialization_alias="summaryAddress", validation_alias="summaryAddress", default_factory=list
     )
 
 
 class RedistributeIntoEigrp(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     protocol: Union[Global[RedistributeProtocol], Variable]
     route_policy: Optional[Union[Default[None], Global[UUID]]] = Default[None](value=None)
 
 
 class AddressFamily(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     redistribute: Optional[List[RedistributeIntoEigrp]] = None
-    network: List[SummaryAddress]
+    network: List[SummaryAddress] = Field(min_length=1)
 
 
-class EigrpData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class EigrpParcel(_ParcelBase):
+    type_: Literal["routing/eigrp"] = Field(default="routing/eigrp", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    as_number: Union[Global[int], Variable] = Field(serialization_alias="asNum", validation_alias="asNum")
-    address_family: AddressFamily = Field(serialization_alias="addressFamily", validation_alias="addressFamily")
+    as_number: Union[Global[int], Variable] = Field(validation_alias=AliasPath("data", "asNum"))
+    address_family: AddressFamily = Field(validation_alias=AliasPath("data", "addressFamily"))
     hello_interval: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="helloInterval", validation_alias="helloInterval", default=Default[int](value=5)
+        validation_alias=AliasPath("data", "helloInterval"), default=Default[int](value=5)
     )
     hold_time: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="holdTime", validation_alias="holdTime", default=Default[int](value=15)
+        validation_alias=AliasPath("data", "holdTime"), default=Default[int](value=15)
+    )
+    authentication: Optional[EigrpAuthentication] = Field(
+        validation_alias=AliasPath("data", "authentication"), default=None
     )
-    authentication: Optional[EigrpAuthentication] = None
     af_interface: Optional[List[IPv4StaticRoute]] = Field(
-        serialization_alias="afInterface", validation_alias="afInterface", default=None
+        validation_alias=AliasPath("data", "afInterface"), default=None
     )
-    table_map: TableMap = Field(serialization_alias="tableMap", validation_alias="tableMap", default=TableMap())
-
-
-class EigrpCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: EigrpData
-    metadata: Optional[dict] = None
+    table_map: TableMap = Field(validation_alias=AliasPath("data", "tableMap"), default=TableMap())
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,84 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import Literal, Optional, Union
+from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
 
-IkeMode = Literal[
-    "main",
-    "aggresive",
+ObjectTrackerType = Literal[
+    "Interface",
+    "SIG",
+    "Route",
 ]
 
-IkeCiphersuite = Literal[
-    "aes256-cbc-sha1",
-    "aes256-cbc-sha2",
-    "aes128-cbc-sha1",
-    "aes128-cbc-sha2",
-]
 
-IkeGroup = Literal[
-    "2",
-    "14",
-    "15",
-    "16",
-    "19",
-    "20",
-    "21",
-    "24",
+Criteria = Literal[
+    "and",
+    "or",
 ]
 
-IpsecCiphersuite = Literal[
-    "aes256-cbc-sha1",
-    "aes256-cbc-sha384",
-    "aes256-cbc-sha256",
-    "aes256-cbc-sha512",
-    "aes256-gcm",
-    "null-sha1",
-    "null-sha384",
-    "null-sha256",
-    "null-sha512",
-]
 
-PfsGroup = Literal[
-    "group-1",
-    "group-2",
-    "group-5",
-    "group-14",
-    "group-15",
-    "group-16",
-    "group-19",
-    "group-20",
-    "group-21",
-    "group-24",
-    "none",
-]
+class SigTracker(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-TunnelApplication = Literal[
-    "none",
-    "sig",
-]
-
-VrrpTrackerAction = Literal[
-    "Decrement",
-    "Shutdown",
-]
+    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
+    object_tracker_type: Global[ObjectTrackerType] = Field(
+        serialization_alias="objectTrackerType",
+        validation_alias="objectTrackerType",
+        default=Global[ObjectTrackerType](value="SIG"),
+    )
 
 
-class Arp(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class InterfaceTracker(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    ip_address: Union[Variable, Global[str], Default[None]]
-    mac_address: Union[Global[str], Variable]
+    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
+    object_tracker_type: Global[ObjectTrackerType] = Field(
+        serialization_alias="objectTrackerType",
+        validation_alias="objectTrackerType",
+        default=Global[ObjectTrackerType](value="Interface"),
+    )
+    interface: Union[Global[str], Variable]
 
 
-class VrrpTrackingObject(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class RouteTracker(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    tracker_id: Union[Default[None], Global[UUID]] = Field(
-        serialization_alias="trackerId", validation_alias="trackerId"
-    )
-    tracker_action: Union[Global[VrrpTrackerAction], Variable] = Field(
-        serialization_alias="trackerAction", validation_alias="trackerAction"
+    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
+    object_tracker_type: Global[ObjectTrackerType] = Field(
+        serialization_alias="objectTrackerType",
+        validation_alias="objectTrackerType",
+        default=Global[ObjectTrackerType](value="Route"),
     )
-    decrement_value: Optional[Union[Variable, Global[int]]] = Field(
-        serialization_alias="decrementValue", validation_alias="decrementValue", default=None
+    route_ip: Union[Global[str], Variable] = Field(serialization_alias="routeIp", validation_alias="routeIp")
+    route_mask: Union[Global[str], Variable, Default[str]] = Field(
+        serialization_alias="routeMask", validation_alias="routeMask"
     )
+    vpn: Union[Global[int], Variable, Default[None]] = Default[None](value=None)
 
 
-class VrrpIPv6Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ObjectTrackerCreationPayload(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    ipv6_link_local: Union[Global[str], Variable] = Field(
-        serialization_alias="ipv6LinkLocal", validation_alias="ipv6LinkLocal"
-    )
-    prefix: Optional[Union[Global[str], Variable, Default[None]]] = None
+    name: str
+    description: Optional[str] = None
+    data: Union[InterfaceTracker, RouteTracker, SigTracker]
 
 
-class StaticIPv4Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ObjectTrackerRef(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    ip_address: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="ipAddress", validation_alias="ipAddress"
-    )
-    subnet_mask: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="subnetMask", validation_alias="subnetMask"
-    )
+    tracker_ref: Global[UUID] = Field(serialization_alias="trackerRef", validation_alias="trackerRef")
 
 
-class StaticIPv6Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ObjectTrackerGroupParcel(_ParcelBase):
+    type_: Literal["trackergroup"] = Field(default="trackergroup", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    address: Union[Global[str], Variable]
+    object_id: Union[Global[int], Variable] = Field(validation_alias=AliasPath("data", "objectId"))
+    tracker_refs: List[ObjectTrackerRef] = Field(validation_alias=AliasPath("data", "trackerRefs"))
+    criteria: Union[Global[Criteria], Variable, Default[Criteria]] = Field(
+        validation_alias=AliasPath("data", "trackerRefs"), default=Default[Criteria](value="or")
+    )
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,175 +1,69 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Address
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.common import (
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.common import EthernetDuplexMode, MediaType
+from catalystwan.models.configuration.feature_profile.common import (
     Arp,
+    DynamicDhcpDistance,
+    EthernetNatAttributesIpv4,
+    InterfaceDynamicIPv4Address,
+    InterfaceDynamicIPv6Address,
+    InterfaceStaticIPv4Address,
     StaticIPv4Address,
+    StaticIPv4AddressConfig,
     StaticIPv6Address,
+)
+from catalystwan.models.configuration.feature_profile.sdwan.service.lan.common import (
     VrrpIPv6Address,
     VrrpTrackingObject,
 )
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.vpn import Direction
-
-NatType = Literal[
-    "pool",
-    "loopback",
-]
-
-DuplexMode = Literal[
-    "full",
-    "half",
-    "auto",
-]
-
-MediaType = Literal[
-    "auto-select",
-    "rj45",
-    "sfp",
-]
-
-
-class DynamicDhcpDistance(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    dynamic_dhcp_distance: Union[Variable, Global[int], Default[int]] = Default[int](value=1)
-
-
-class InterfaceDynamicIPv4Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    dynamic: DynamicDhcpDistance
-
-
-class StaticIPv4AddressConfig(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    primary_ip_address: StaticIPv4Address = Field(
-        serialization_alias="staticIpV4AddressPrimary", validation_alias="staticIpV4AddressPrimary"
-    )
-    secondary_ip_address: Optional[StaticIPv4Address] = Field(
-        serialization_alias="staticIpV4AddressSecondary", validation_alias="staticIpV4AddressSecondary", default=None
-    )
-
-
-class InterfaceStaticIPv4Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    static: StaticIPv4AddressConfig
-
-
-class DynamicIPv6Dhcp(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    dhcp_client: Global[dict] = Field(
-        serialization_alias="dhcpClient", validation_alias="dhcpClient", default=Global[dict](value={})
-    )
-    secondary_ipv6_address: Optional[List[StaticIPv6Address]] = Field(
-        serialization_alias="secondaryIpV6Address", validation_alias="secondaryIpV6Address"
-    )
-
-
-class InterfaceDynamicIPv6Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    dynamic: DynamicIPv6Dhcp
 
 
 class Dhcpv6Helper(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     ip_address: Union[Global[str], Variable] = Field(serialization_alias="ipAddress", validation_alias="ipAddress")
     vpn: Optional[Union[Global[int], Variable, Default[None]]] = None
 
 
 class StaticIPv6AddressConfig(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     primary_ip_address: StaticIPv6Address = Field(
         serialization_alias="staticIpV6AddressPrimary", validation_alias="staticIpV6AddressPrimary"
     )
     secondary_ip_address: Optional[List[StaticIPv6Address]] = Field(
         serialization_alias="staticIpV6AddressSecondary", validation_alias="staticIpV6AddressSecondary", default=None
     )
     dhcp_helper_v6: Optional[List[Dhcpv6Helper]] = Field(
         serialization_alias="dhcpHelperV6", validation_alias="dhcpHelperV6", default=None
     )
 
 
 class InterfaceStaticIPv6Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     static: StaticIPv6AddressConfig
 
 
-class NatPool(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    range_start: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="rangeStart", validation_alias="rangeStart"
-    )
-    range_end: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="rangeEnd", validation_alias="rangeEnd"
-    )
-    prefix_length: Union[Variable, Global[int], Default[None]] = Field(
-        serialization_alias="prefixLength", validation_alias="prefixLength"
-    )
-    overload: Union[Variable, Global[bool], Default[bool]] = Default[bool](value=True)
-
-
-class StaticNat(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    source_ip: Union[Global[str], Variable] = Field(serialization_alias="sourceIp", validation_alias="sourceIp")
-
-    translate_ip: Union[Global[str], Variable] = Field(
-        serialization_alias="translateIp", validation_alias="translateIp"
-    )
-    static_nat_direction: Union[Global[Direction], Default[Direction]] = Field(
-        serialization_alias="staticNatDirection",
-        validation_alias="staticNatDirection",
-        default=Default[Direction](value="inside"),
-    )
-    source_vpn: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="sourceVpn", validation_alias="sourceVpn", default=Default[int](value=0)
-    )
-
-
-class NatAttributesIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    nat_type: Union[Global[NatType], Variable] = Field(serialization_alias="natType", validation_alias="natType")
-    nat_pool: Optional[NatPool] = Field(serialization_alias="natPool", validation_alias="natPool", default=None)
-    nat_loopback: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="natLoopbakc", validation_alias="natLoopbakc", default=None
-    )
-    udp_timeout: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="udpTimeout", validation_alias="udpTimeout", default=Default[int](value=1)
-    )
-    tcp_timeout: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="tcpTimeout", validation_alias="tcpTimeout", default=Default[int](value=1)
-    )
-    new_static_nat: Optional[List[StaticNat]] = Field(
-        serialization_alias="newStaticNat", validation_alias="newStaticNat", default=None
-    )
-
-
 class NatAttributesIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     nat64: Optional[Union[Global[bool], Default[bool]]] = Default[bool](value=False)
 
 
 class AclQos(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     shaping_rate: Optional[Union[Global[int], Variable, Default[None]]] = Field(
         serialization_alias="shapingRate", validation_alias="shapingRate", default=None
     )
     ipv4_acl_egress: Optional[Global[UUID]] = Field(
         serialization_alias="ipv4AclEgress", validation_alias="ipv4AclEgress", default=None
     )
@@ -181,51 +75,55 @@
     )
     ipv6_acl_ingress: Optional[Global[UUID]] = Field(
         serialization_alias="ipv6AclIngress", validation_alias="ipv6AclIngress", default=None
     )
 
 
 class VrrpIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     group_id: Union[Variable, Global[int]] = Field(serialization_alias="groupId", validation_alias="groupId")
     priority: Union[Variable, Global[int], Default[int]] = Default[int](value=100)
     timer: Union[Variable, Global[int], Default[int]] = Default[int](value=1000)
     track_omp: Union[Global[bool], Default[bool]] = Field(
         serialization_alias="trackOmp", validation_alias="trackOmp", default=Default[bool](value=False)
     )
     ipv6: List[VrrpIPv6Address]
 
 
 class VrrpIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     group_id: Union[Variable, Global[int]] = Field(serialization_alias="groupId", validation_alias="groupId")
     priority: Union[Variable, Global[int], Default[int]] = Default[int](value=100)
     timer: Union[Variable, Global[int], Default[int]] = Default[int](value=1000)
     track_omp: Union[Global[bool], Default[bool]] = Field(
         serialization_alias="trackOmp", validation_alias="trackOmp", default=Default[bool](value=False)
     )
-    ip_address: Union[Global[str], Variable] = Field(serialization_alias="ipAddress", validation_alias="ipAddress")
+    ip_address: Union[Global[str], Global[IPv4Address], Variable] = Field(
+        serialization_alias="ipAddress", validation_alias="ipAddress"
+    )
     ip_address_secondary: Optional[List[StaticIPv4Address]] = Field(
-        serialization_alias="ipAddressSecondary", validation_alias="ipAddressSecondary"
+        serialization_alias="ipAddressSecondary",
+        validation_alias="ipAddressSecondary",
+        default=None,
     )
     tloc_pref_change: Union[Global[bool], Default[bool]] = Field(
         serialization_alias="tlocPrefChange", validation_alias="tlocPrefChange", default=Default[bool](value=False)
     )
     tloc_pref_change_value: Optional[Union[Global[int], Default[None]]] = Field(
         serialization_alias="tlocPrefChangeValue", validation_alias="tlocPrefChangeValue", default=None
     )
     tracking_object: Optional[List[VrrpTrackingObject]] = Field(
         serialization_alias="trackingObject", validation_alias="trackingObject", default=None
     )
 
 
 class Trustsec(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     enable_sgt_propagation: Union[Global[bool], Default[bool]] = Field(
         serialization_alias="enableSGTPropagation",
         validation_alias="enableSGTPropagation",
         default=Default[bool](value=False),
     )
     propagate: Optional[Union[Global[bool], Default[bool]]] = Default[bool](value=True)
@@ -236,18 +134,18 @@
         serialization_alias="enableEnforcedPropagation", validation_alias="enableEnforcedPropagation"
     )
     enforced_security_group_tag: Union[Global[int], Variable, Default[None]] = Field(
         serialization_alias="enforcedSecurityGroupTag", validation_alias="enforcedSecurityGroupTag"
     )
 
 
-class AdvancedAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class AdvancedEthernetAttributes(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    duplex: Optional[Union[Global[DuplexMode], Variable, Default[None]]] = None
+    duplex: Optional[Union[Global[EthernetDuplexMode], Variable, Default[None]]] = None
     mac_address: Optional[Union[Global[str], Variable, Default[None]]] = Field(
         serialization_alias="macAddress", validation_alias="macAddress", default=None
     )
     ip_mtu: Union[Global[int], Variable, Default[int]] = Field(
         serialization_alias="ipMtu", validation_alias="ipMtu", default=Default[int](value=1500)
     )
     interface_mtu: Optional[Union[Global[int], Variable, Default[int]]] = Field(
@@ -269,59 +167,86 @@
     )
     tracker: Optional[Union[Global[str], Variable, Default[None]]] = None
     icmp_redirect_disable: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="icmpRedirectDisable",
         validation_alias="icmpRedirectDisable",
         default=Default[bool](value=True),
     )
-    xconnect: Optional[Union[Global[str], Variable, Default[None]]] = None
+    xconnect: Optional[Union[Global[str], Global[IPv4Address], Variable, Default[None]]] = None
     ip_directed_broadcast: Union[Global[bool], Variable, Default[bool]] = Field(
         serialization_alias="ipDirectedBroadcast",
         validation_alias="ipDirectedBroadcast",
         default=Default[bool](value=False),
     )
 
 
-class InterfaceEthernetData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    shutdown: Union[Global[bool], Variable, Default[bool]] = Default[bool](value=True)
-    interface_name: Union[Global[str], Variable] = Field(
-        serialization_alias="interfaceName", validation_alias="interfaceName"
+class InterfaceEthernetParcel(_ParcelBase):
+    type_: Literal["lan/vpn/interface/ethernet"] = Field(default="lan/vpn/interface/ethernet", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    shutdown: Union[Global[bool], Variable, Default[bool]] = Field(
+        default=Default[bool](value=True), validation_alias=AliasPath("data", "shutdown")
+    )
+    interface_name: Union[Global[str], Variable] = Field(validation_alias=AliasPath("data", "interfaceName"))
+    ethernet_description: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        default=Default[None](value=None), validation_alias=AliasPath("data", "description")
     )
-    description: Optional[Union[Global[str], Variable, Default[None]]] = None
     interface_ip_address: Union[InterfaceDynamicIPv4Address, InterfaceStaticIPv4Address] = Field(
-        serialization_alias="intfIpAddress", validation_alias="intfIpAddress"
+        validation_alias=AliasPath("data", "intfIpAddress"), default_factory=InterfaceStaticIPv4Address
     )
     dhcp_helper: Optional[Union[Variable, Global[List[str]], Default[None]]] = Field(
-        serialization_alias="dhcpHelper", validation_alias="dhcpHelper", default=None
+        validation_alias=AliasPath("data", "dhcpHelper"), default=None
     )
     interface_ipv6_address: Optional[Union[InterfaceDynamicIPv6Address, InterfaceStaticIPv6Address]] = Field(
-        serialization_alias="intfIpV6Address", validation_alias="intfIpV6Address", default=None
+        validation_alias=AliasPath("data", "intfIpV6Address"), default=None
     )
-    nat: Union[Global[bool], Default[bool]] = Default[bool](value=False)
-    nat_attributes_ipv4: Optional[NatAttributesIPv4] = Field(
-        serialization_alias="natAttributesIpv4", validation_alias="natAttributesIpv4", default=None
+    nat: Union[Global[bool], Default[bool]] = Field(
+        validation_alias=AliasPath("data", "nat"), default=Default[bool](value=False)
+    )
+    nat_attributes_ipv4: Optional[EthernetNatAttributesIpv4] = Field(
+        validation_alias=AliasPath("data", "natAttributesIpv4"), default=None
     )
     nat_ipv6: Optional[Union[Global[bool], Default[bool]]] = Field(
-        serialization_alias="natIpv6", validation_alias="natIpv6", default=Default[bool](value=False)
+        validation_alias=AliasPath("data", "natIpv6"), default=Default[bool](value=False)
     )
     nat_attributes_ipv6: Optional[NatAttributesIPv6] = Field(
-        serialization_alias="natAttributesIpv6", validation_alias="natAttributesIpv6", default=None
-    )
-    acl_qos: Optional[AclQos] = Field(serialization_alias="aclQos", validation_alias="aclQos", default=None)
-    vrrp_ipv6: Optional[List[VrrpIPv6]] = Field(
-        serialization_alias="vrrpIpv6", validation_alias="vrrpIpv6", default=None
+        validation_alias=AliasPath("data", "natAttributesIpv6"), default=None
     )
-    vrrp: Optional[List[VrrpIPv4]] = None
-    arp: Optional[List[Arp]] = None
-    trustsec: Optional[Trustsec] = None
-    advanced: AdvancedAttributes = AdvancedAttributes()
-
-
-class InterfaceEthernetCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: InterfaceEthernetData
-    metadata: Optional[dict] = None
+    acl_qos: Optional[AclQos] = Field(validation_alias=AliasPath("data", "aclQos"), default=None)
+    vrrp_ipv6: Optional[List[VrrpIPv6]] = Field(validation_alias=AliasPath("data", "vrrpIpv6"), default=None)
+    vrrp: Optional[List[VrrpIPv4]] = Field(validation_alias=AliasPath("data", "vrrp"), default=None)
+    arp: Optional[List[Arp]] = Field(validation_alias=AliasPath("data", "arp"), default=None)
+    trustsec: Optional[Trustsec] = Field(validation_alias=AliasPath("data", "trustsec"), default=None)
+    advanced: AdvancedEthernetAttributes = Field(
+        validation_alias=AliasPath("data", "advanced"), default_factory=AdvancedEthernetAttributes
+    )
+
+    def set_dynamic_interface_ip_address(self, dhcp_distance: Union[Global[int], Variable]) -> None:
+        self.interface_ip_address = InterfaceDynamicIPv4Address(
+            dynamic=DynamicDhcpDistance(dynamic_dhcp_distance=dhcp_distance)
+        )
+
+    def set_static_primary_interface_ip_address(
+        self,
+        ip_address: Union[Global[str], Global[IPv4Address], Variable],
+        subnet_mask: Optional[Union[Global[str], Variable]] = None,
+    ) -> None:
+        if subnet_mask is None:
+            primary_ip_address = StaticIPv4Address(ip_address=ip_address)
+        else:
+            primary_ip_address = StaticIPv4Address(ip_address=ip_address, subnet_mask=subnet_mask)
+        self.interface_ip_address = InterfaceStaticIPv4Address(
+            static=StaticIPv4AddressConfig(primary_ip_address=primary_ip_address)
+        )
+
+    def add_static_secondary_interface_ip_address(
+        self, ip_address: Union[Global[str], Global[IPv4Address], Variable], subnet_mask: Union[Global[str], Variable]
+    ) -> None:
+        if self.interface_ip_address is None:
+            raise ValueError("Missing static primary IP Address")
+        if isinstance(self.interface_ip_address, InterfaceDynamicIPv4Address):
+            raise ValueError("Interface IP Address is already dynamic")
+
+        secondary_ip_address = StaticIPv4Address(ip_address=ip_address, subnet_mask=subnet_mask)
+        if self.interface_ip_address.static.secondary_ip_address is None:
+            self.interface_ip_address.static.secondary_ip_address = []
+        self.interface_ip_address.static.secondary_ip_address.append(secondary_ip_address)
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,206 +1,270 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import Literal, Optional, Union
+from ipaddress import IPv4Address
+from typing import List, Literal, Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.common import (
-    IkeCiphersuite,
-    IkeGroup,
-    IkeMode,
-    IpsecCiphersuite,
-    PfsGroup,
-    TunnelApplication,
-)
-
-GreTunnelMode = Literal[
-    "ipv4",
-    "ipv6",
-]
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default, as_global
 
+VirtualApplicationType = Literal["dreopt"]
 
-class GreAddress(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+ResourceProfile = Literal[
+    "small",
+    "medium",
+    "large",
+    "extra-large",
+    "default",
+]
 
-    address: Union[Variable, Global[str]]
-    mask: Union[Variable, Global[str]]
+AppqoeDeviceRole = Literal[
+    "forwarder",
+    "forwarderAndServiceNode",
+    "serviceNode",
+    "serviceNodeWithDre",
+    "forwarderAndServiceNodeWithDre",
+]
 
+AppnavControllerGroupName = Literal["ACG-APPQOE"]
+ServiceNodeGroupName = Literal["SNG-APPQOE"]
+ServiceNodeGroupsNames = Literal[
+    "SNG-APPQOE",
+    "SNG-APPQOE1",
+    "SNG-APPQOE2",
+    "SNG-APPQOE3",
+    "SNG-APPQOE4",
+    "SNG-APPQOE5",
+    "SNG-APPQOE6",
+    "SNG-APPQOE7",
+    "SNG-APPQOE8",
+    "SNG-APPQOE9",
+    "SNG-APPQOE10",
+    "SNG-APPQOE11",
+    "SNG-APPQOE12",
+    "SNG-APPQOE13",
+    "SNG-APPQOE14",
+    "SNG-APPQOE15",
+    "SNG-APPQOE16",
+    "SNG-APPQOE17",
+    "SNG-APPQOE18",
+    "SNG-APPQOE19",
+    "SNG-APPQOE20",
+    "SNG-APPQOE21",
+    "SNG-APPQOE22",
+    "SNG-APPQOE23",
+    "SNG-APPQOE24",
+    "SNG-APPQOE25",
+    "SNG-APPQOE26",
+    "SNG-APPQOE27",
+    "SNG-APPQOE28",
+    "SNG-APPQOE29",
+    "SNG-APPQOE30",
+    "SNG-APPQOE31",
+]
+ForwarderAndServiceNodeAddress = Literal["192.168.2.2"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
+ForwarderAndServiceNodeControllerAddress = Literal[
+    "192.168.2.1"
+]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
+ServiceNodeExternalAddress = Literal["192.168.2.2"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
+ServiceNodeExternalVpgIp = Literal["192.168.2.1/24"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
 
-class TunnelSourceIP(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    tunnel_source: Union[Global[str], Variable] = Field(
-        serialization_alias="tunnelSource", validation_alias="tunnelSource"
+class VirtualApplication(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    instance_id: Global[int] = Field(
+        default=Global(value=1), serialization_alias="instanceId", validation_alias="instanceId"
+    )
+    application_type: Global[VirtualApplicationType] = Field(
+        default=Global[VirtualApplicationType](value="dreopt"),
+        serialization_alias="applicationType",
+        validation_alias="applicationType",
     )
-    tunnel_route_via: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="tunnelRouteVia", validation_alias="tunnelRouteVia", default=None
+    resource_profile: Union[Global[ResourceProfile], Default[ResourceProfile]] = Field(
+        default=Default[ResourceProfile](value="default"),
+        serialization_alias="resourceProfile",
+        validation_alias="resourceProfile",
     )
 
 
-class TunnelSourceIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class Appqoe(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    tunnel_source_v6: Union[Global[str], Variable] = Field(
-        serialization_alias="tunnelSourceV6", validation_alias="tunnelSourceV6"
+    name: Default[str] = Default(value="/1")
+    appnav_controller_group: Global[AppnavControllerGroupName] = Field(
+        default=Global[AppnavControllerGroupName](value="ACG-APPQOE"),
+        serialization_alias="appnavControllerGroup",
+        validation_alias="appnavControllerGroup",
+    )
+    service_node_group: Global[ServiceNodeGroupName] = Field(
+        default=Global[ServiceNodeGroupName](value="SNG-APPQOE"),
+        serialization_alias="serviceNodeGroup",
+        validation_alias="serviceNodeGroup",
     )
-    tunnel_route_via: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="tunnelRouteVia", validation_alias="tunnelRouteVia", default=None
+    service_node_groups: List[Global[ServiceNodeGroupsNames]] = Field(
+        default=[Global[ServiceNodeGroupsNames](value="SNG-APPQOE")],
+        serialization_alias="serviceNodeGroups",
+        validation_alias="serviceNodeGroups",
     )
+    enable: Global[bool] = Global[bool](value=True)
+    vpn: Union[Global[int], Default[None], Variable] = Field(default=Global[int](value=0))
 
 
-class TunnelSourceInterface(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ServiceContext(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+    appqoe: List[Appqoe] = Field(default_factory=lambda: [Appqoe()])
 
-    tunnel_source_interface: Union[Global[str], Variable] = Field(
-        serialization_alias="tunnelSourceInterface", validation_alias="tunnelSourceInterface"
-    )
-    tunnel_route_via: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="tunnelRouteVia", validation_alias="tunnelRouteVia", default=None
-    )
 
+# Frowarder
 
-class GreSourceIp(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    source_ip: TunnelSourceIP = Field(serialization_alias="sourceIp", validation_alias="sourceIp")
+class ServiceNodeInformation(BaseModel):
+    address: Global[IPv4Address]
 
 
-class GreSourceNotLoopback(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ForwarderController(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    source_not_loopback: TunnelSourceInterface = Field(
-        serialization_alias="sourceNotLoopback", validation_alias="sourceNotLoopback"
+    address: Union[Global[str], Global[IPv4Address], Variable]
+    vpn: Global[int] = Field(
+        default=Global[int](value=1), description="This is field is a depended on the Service VPN value."
     )
 
 
-class GreSourceLoopback(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ForwarderAppnavControllerGroup(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    source_loopback: TunnelSourceInterface = Field(
-        serialization_alias="sourceLoopback", validation_alias="sourceLoopback"
+    group_name: Default[AppnavControllerGroupName] = Field(
+        default=Default(value="ACG-APPQOE"), serialization_alias="groupName", validation_alias="groupName"
+    )
+    appnav_controllers: List[ForwarderController] = Field(
+        serialization_alias="appnavControllers", validation_alias="appnavControllers"
     )
 
 
-class GreSourceIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ForwarderNodeGroup(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    source_ipv6: TunnelSourceIPv6 = Field(serialization_alias="sourceIpv6", validation_alias="sourceIpv6")
+    name: Union[Global[str], Default[ServiceNodeGroupName]] = Default[ServiceNodeGroupName](value="SNG-APPQOE")
+    internal: Union[Default[bool], Global[bool]] = Default[bool](value=False)
+    service_node: List[ServiceNodeInformation] = Field(
+        serialization_alias="serviceNode", validation_alias="serviceNode"
+    )
 
 
-class BasicGre(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ForwarderRole(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    interface_name: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="ifName", validation_alias="ifName", default=None
-    )
-    description: Optional[Union[Global[str], Variable, Default[None]]] = None
-    address: Optional[GreAddress] = None
-    ipv6_address: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="ipv6Address", validation_alias="ipv6Address", default=None
-    )
-    shutdown: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
-    tunnel_protection: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="tunnelProtection", validation_alias="tunnelProtection", default=Default[bool](value=False)
-    )
-    tunnel_mode: Optional[Union[Global[GreTunnelMode], Default[GreTunnelMode]]] = Field(
-        serialization_alias="tunnelMode",
-        validation_alias="tunnelMode",
-        default=Default[GreTunnelMode](value="ipv4"),
+    appnav_controller_group: List[ForwarderAppnavControllerGroup] = Field(
+        serialization_alias="appnavControllerGroup", validation_alias="appnavControllerGroup"
     )
-    tunnel_source_type: Optional[Union[GreSourceIp, GreSourceNotLoopback, GreSourceLoopback, GreSourceIPv6]] = Field(
-        serialization_alias="tunnelSourceType", validation_alias="tunnelSourceType", default=None
+    service_node_group: List[ForwarderNodeGroup] = Field(
+        serialization_alias="serviceNodeGroup", validation_alias="serviceNodeGroup"
     )
-    tunnel_destination: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="tunnelDestination", validation_alias="tunnelDestination", default=None
+    service_context: ServiceContext = Field(
+        default_factory=ServiceContext, serialization_alias="serviceContext", validation_alias="serviceContext"
     )
-    tunnel_destination_v6: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="tunnelDestinationV6", validation_alias="tunnelDestinationV6", default=None
-    )
-    mtu: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=1500)
-    mtu_v6: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="mtuV6", validation_alias="mtuV6", default=None
-    )
-    tcp_mss_adjust: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="tcpMssAdjust", validation_alias="tcpMssAdjust", default=None
-    )
-    tcp_mss_adjust_v6: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="tcpMssAdjustV6", validation_alias="tcpMssAdjustV6", default=None
-    )
-    clear_dont_fragment: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="clearDontFragment",
-        validation_alias="clearDontFragment",
-        default=Default[bool](value=False),
-    )
-    dpd_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="dpdInterval", validation_alias="dpdInterval", default=Default[int](value=10)
-    )
-    dpd_retries: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="dpdRetries", validation_alias="dpdRetries", default=Default[int](value=3)
-    )
-    ike_version: Optional[Union[Global[int], Default[int]]] = Field(
-        serialization_alias="ikeVersion", validation_alias="ikeVersion", default=Default[int](value=1)
-    )
-    ike_mode: Optional[Union[Global[IkeMode], Variable, Default[IkeMode]]] = Field(
-        serialization_alias="ikeMode", validation_alias="ikeMode", default=Default[IkeMode](value="main")
-    )
-    ike_rekey_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="ikeRekeyInterval", validation_alias="ikeRekeyInterval", default=Default[int](value=14400)
-    )
-    ike_ciphersuite: Optional[Union[Global[IkeCiphersuite], Variable, Default[IkeCiphersuite]]] = Field(
-        serialization_alias="ikeCiphersuite",
-        validation_alias="ikeCiphersuite",
-        default=Default[IkeCiphersuite](value="aes256-cbc-sha1"),
-    )
-    ike_group: Optional[Union[Global[IkeGroup], Variable, Default[IkeGroup]]] = Field(
-        serialization_alias="ikeGroup", validation_alias="ikeGroup", default=Default[IkeGroup](value="16")
-    )
-    pre_shared_secret: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="preSharedSecret", validation_alias="preSharedSecret", default=None
+
+
+# Forwarder and Service
+
+
+class ServiceNodeInformationDefault(BaseModel):
+    address: Default[ForwarderAndServiceNodeAddress] = Default[ForwarderAndServiceNodeAddress](value="192.168.2.2")
+
+
+class ForwarderAndServiceNodeController(BaseModel):
+    address: Default[ForwarderAndServiceNodeControllerAddress] = Default[ForwarderAndServiceNodeControllerAddress](
+        value="192.168.2.1"
     )
-    ike_local_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="ikeLocalId", validation_alias="ikeLocalId", default=None
+
+
+class ForwarderAndServiceNodeAppnavControllerGroup(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    group_name: Default[AppnavControllerGroupName] = Field(
+        default=Default[AppnavControllerGroupName](value="ACG-APPQOE"),
+        serialization_alias="groupName",
+        validation_alias="groupName",
     )
-    ike_remote_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="ikeRemoteId", validation_alias="ikeRemoteId", default=None
+    appnav_controllers: List[ForwarderAndServiceNodeController] = Field(
+        serialization_alias="appnavControllers", validation_alias="appnavControllers"
     )
-    ipsec_rekey_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="ipsecRekeyInterval",
-        validation_alias="ipsecRekeyInterval",
-        default=Default[int](value=3600),
+
+
+class ForwarderAndServiceNodeGroup(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    name: Default[ServiceNodeGroupName] = Default[ServiceNodeGroupName](value="SNG-APPQOE")
+    internal: Default[bool] = Default[bool](value=True)
+    service_node: List[ServiceNodeInformationDefault] = Field(
+        serialization_alias="serviceNode", validation_alias="serviceNode"
     )
-    ipsec_replay_window: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="ipsecReplayWindow", validation_alias="ipsecReplayWindow", default=Default[int](value=512)
+
+
+class ForwarderAndServiceNodeRole(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    appnav_controller_group: List[ForwarderAndServiceNodeAppnavControllerGroup] = Field(
+        serialization_alias="appnavControllerGroup", validation_alias="appnavControllerGroup"
     )
-    ipsec_ciphersuite: Optional[Union[Global[IpsecCiphersuite], Variable, Default[IpsecCiphersuite]]] = Field(
-        serialization_alias="ipsecCiphersuite",
-        validation_alias="ipsecCiphersuite",
-        default=Default[IpsecCiphersuite](value="aes256-gcm"),
+    service_node_group: List[ForwarderAndServiceNodeGroup] = Field(
+        serialization_alias="serviceNodeGroup", validation_alias="serviceNodeGroup"
     )
-    perfect_forward_secrecy: Optional[Union[Global[PfsGroup], Variable, Default[PfsGroup]]] = Field(
-        serialization_alias="perfectForwardSecrecy",
-        validation_alias="perfectForwardSecrecy",
-        default=Default[PfsGroup](value="group-16"),
+
+    service_context: ServiceContext = Field(serialization_alias="serviceContext", validation_alias="serviceContext")
+
+
+# Service
+
+
+class ServiceNodeInformationExternal(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    address: Default[ServiceNodeExternalAddress] = Default[ServiceNodeExternalAddress](value="192.168.2.2")
+    vpg_ip: Default[ServiceNodeExternalVpgIp] = Field(
+        default=Default[ServiceNodeExternalVpgIp](value="192.168.2.1/24"),
+        serialization_alias="vpgIp",
+        validation_alias="vpgIp",
     )
 
 
-class AdvancedGre(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ServiceNodeGroup(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    application: Optional[Union[Global[TunnelApplication], Variable]] = None
+    name: Default[ServiceNodeGroupName] = Default[ServiceNodeGroupName](value="SNG-APPQOE")
+    external_node: Default[bool] = Field(
+        default=Default[bool](value=True), serialization_alias="externalNode", validation_alias="externalNode"
+    )
+    service_node: List[ServiceNodeInformationExternal] = Field(
+        default=[ServiceNodeInformationExternal()], serialization_alias="serviceNode", validation_alias="serviceNode"
+    )
 
 
-class InterfaceGreData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ServiceNodeRole(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    service_node_group: List[ServiceNodeGroup] = Field(
+        default=[ServiceNodeGroup()], serialization_alias="serviceNodeGroup", validation_alias="serviceNodeGroup"
+    )
 
-    basic: BasicGre
-    advanced: Optional[AdvancedGre] = None
 
+class AppqoeParcel(_ParcelBase):
+    type_: Literal["appqoe"] = Field(default="appqoe", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-class InterfaceGreCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    dreopt: Optional[Union[Global[bool], Default[bool]]] = Field(
+        default=as_default(False), validation_alias=AliasPath("data", "dreopt")
+    )
+    virtual_application: Optional[List[VirtualApplication]] = Field(
+        default=None, validation_alias=AliasPath("data", "virtualApplication")
+    )
+    appqoe_device_role: Global[str] = Field(
+        default=as_global("forwarder"), validation_alias=AliasPath("data", "appqoeDeviceRole")
+    )
 
-    name: str
-    description: Optional[str] = None
-    data: InterfaceGreData
-    metadata: Optional[dict] = None
+    forwarder: Optional[ForwarderRole] = Field(default=None, validation_alias=AliasPath("data", "forwarder"))
+    forwarder_and_service_node: Optional[ForwarderAndServiceNodeRole] = Field(
+        default=None, validation_alias=AliasPath("data", "forwarderAndServiceNode")
+    )
+    service_node: Optional[ServiceNodeRole] = Field(default=None, validation_alias=AliasPath("data", "serviceNode"))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,138 +1,119 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Interface, IPv6Address, IPv6Interface
 from typing import Literal, Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.common import (
-    IkeCiphersuite,
-    IkeGroup,
-    IkeMode,
-    IpsecCiphersuite,
-    PfsGroup,
-    TunnelApplication,
-)
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.common import IkeCiphersuite, IkeGroup, IkeMode, IpsecCiphersuite, PfsGroup
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask, TunnelApplication
 
 IpsecTunnelMode = Literal[
     "ipv4",
     "ipv6",
     "ipv4-v6overlay",
 ]
 
 
-class IpsecAddress(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    address: Union[Variable, Global[str]]
-    mask: Union[Variable, Global[str]]
-
-
-class InterfaceIpsecData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    interface_name: Union[Global[str], Variable] = Field(serialization_alias="ifName", validation_alias="ifName")
-    shutdown: Union[Global[bool], Variable, Default[bool]] = Default[bool](value=True)
+class InterfaceIpsecParcel(_ParcelBase):
+    type_: Literal["lan/vpn/interface/ipsec"] = Field(default="lan/vpn/interface/ipsec", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    interface_name: Union[Global[str], Variable] = Field(validation_alias=AliasPath("data", "ifName"))
+    shutdown: Union[Global[bool], Variable, Default[bool]] = Field(
+        default=Default[bool](value=True), validation_alias=AliasPath("data", "shutdown")
+    )
     tunnel_mode: Optional[Union[Global[IpsecTunnelMode], Default[IpsecTunnelMode]]] = Field(
-        serialization_alias="tunnelMode",
-        validation_alias="tunnelMode",
-        default=Default[IpsecTunnelMode](value="ipv4"),
-    )
-    description: Union[Global[str], Variable, Default[None]] = Default[None](value=None)
-    address: Optional[IpsecAddress] = None
-    ipv6_address: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="ipv6Address", validation_alias="ipv6Address", default=None
+        validation_alias=AliasPath("data", "tunnelMode"),
+        default=None,
+    )
+    ipsec_description: Union[Global[str], Variable, Default[None]] = Field(
+        default=Default[None](value=None), validation_alias=AliasPath("data", "description")
     )
-    tunnel_source: Optional[IpsecAddress] = Field(
-        serialization_alias="tunnelSource", validation_alias="tunnelSource", default=None
+    address: Optional[AddressWithMask] = Field(default=None, validation_alias=AliasPath("data", "address"))
+    ipv6_address: Optional[Union[Global[str], Global[IPv6Interface], Variable]] = Field(
+        validation_alias=AliasPath("data", "ipv6Address"), default=None
     )
+    tunnel_source: Optional[AddressWithMask] = Field(validation_alias=AliasPath("data", "tunnelSource"), default=None)
     tunnel_source_v6: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="tunnelSourceV6", validation_alias="tunnelSourceV6", default=None
+        validation_alias=AliasPath("data", "tunnelSourceV6"), default=None
     )
-    tunnel_source_interface: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="tunnelSourceInterface", validation_alias="tunnelSourceInterface", default=None
+    tunnel_source_interface: Optional[Union[Global[str], Global[IPv4Interface], Variable]] = Field(
+        validation_alias=AliasPath("data", "tunnelSourceInterface"), default=None
     )
-    tunnel_destination: Optional[IpsecAddress] = Field(
-        serialization_alias="tunnelDestination", validation_alias="tunnelDestination", default=None
+    tunnel_destination: Optional[AddressWithMask] = Field(
+        validation_alias=AliasPath("data", "tunnelDestination"), default=None
     )
-    tunnel_destination_v6: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="tunnelDestinationV6", validation_alias="tunnelDestinationV6", default=None
+    tunnel_destination_v6: Optional[Union[Global[str], Global[IPv6Address], Variable]] = Field(
+        validation_alias=AliasPath("data", "tunnelDestinationV6"), default=None
     )
-    application: Union[Global[TunnelApplication], Variable]
+    application: Union[Global[TunnelApplication], Variable] = Field(validation_alias=AliasPath("data", "application"))
     tcp_mss_adjust: Union[Global[int], Variable, Default[None]] = Field(
-        serialization_alias="tcpMssAdjust", validation_alias="tcpMssAdjust", default=Default[None](value=None)
+        validation_alias=AliasPath("data", "tcpMssAdjust"), default=Default[None](value=None)
     )
-    tcp_mss_adjust_v6: Union[Global[int], Variable, Default[None]] = Field(
-        serialization_alias="tcpMssAdjustV6", validation_alias="tcpMssAdjustV6", default=Default[None](value=None)
+    tcp_mss_adjust_v6: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        validation_alias=AliasPath("data", "tcpMssAdjustV6"), default=None
     )
     clear_dont_fragment: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="clearDontFragment",
-        validation_alias="clearDontFragment",
+        validation_alias=AliasPath("data", "clearDontFragment"),
         default=Default[bool](value=False),
     )
-    mtu: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=1500)
+    mtu: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        default=Default[int](value=1500), validation_alias=AliasPath("data", "mtu")
+    )
     mtu_v6: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="mtuV6", validation_alias="mtuV6", default=None
+        validation_alias=AliasPath("data", "mtuV6"), default=None
     )
     dpd_interval: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="dpdInterval", validation_alias="dpdInterval", default=Default[int](value=10)
+        validation_alias=AliasPath("data", "dpdInterval"), default=Default[int](value=10)
     )
     dpd_retries: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="dpdRetries", validation_alias="dpdRetries", default=Default[int](value=3)
+        validation_alias=AliasPath("data", "dpdRetries"), default=Default[int](value=3)
     )
     ike_version: Union[Global[int], Default[int]] = Field(
-        serialization_alias="ikeVersion", validation_alias="ikeVersion", default=Default[int](value=1)
+        validation_alias=AliasPath("data", "ikeVersion"), default=Default[int](value=1)
     )
     ike_mode: Optional[Union[Global[IkeMode], Variable, Default[IkeMode]]] = Field(
-        serialization_alias="ikeMode", validation_alias="ikeMode", default=Default[IkeMode](value="main")
+        validation_alias=AliasPath("data", "ikeMode"), default=Default[IkeMode](value="main")
     )
     ike_rekey_interval: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="ikeRekeyInterval", validation_alias="ikeRekeyInterval", default=Default[int](value=14400)
+        validation_alias=AliasPath("data", "ikeRekeyInterval"), default=Default[int](value=14400)
     )
     ike_ciphersuite: Union[Global[IkeCiphersuite], Variable, Default[IkeCiphersuite]] = Field(
-        serialization_alias="ikeCiphersuite",
-        validation_alias="ikeCiphersuite",
+        validation_alias=AliasPath("data", "ikeCiphersuite"),
         default=Default[IkeCiphersuite](value="aes256-cbc-sha1"),
     )
     ike_group: Union[Global[IkeGroup], Variable, Default[IkeGroup]] = Field(
-        serialization_alias="ikeGroup", validation_alias="ikeGroup", default=Default[IkeGroup](value="16")
+        validation_alias=AliasPath("data", "ikeGroup"), default=Default[IkeGroup](value="16")
     )
     pre_shared_secret: Union[Global[str], Variable] = Field(
-        serialization_alias="preSharedSecret", validation_alias="preSharedSecret"
+        validation_alias=AliasPath("data", "preSharedSecret"),
     )
     ike_local_id: Union[Global[str], Variable, Default[None]] = Field(
-        serialization_alias="ikeLocalId", validation_alias="ikeLocalId"
+        validation_alias=AliasPath("data", "ikeLocalId"), default=Default[None](value=None)
     )
     ike_remote_id: Union[Global[str], Variable, Default[None]] = Field(
-        serialization_alias="ikeRemoteId", validation_alias="ikeRemoteId"
+        validation_alias=AliasPath("data", "ikeRemoteId"), default=Default[None](value=None)
     )
     ipsec_rekey_interval: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="ipsecRekeyInterval",
-        validation_alias="ipsecRekeyInterval",
+        validation_alias=AliasPath("data", "ipsecRekeyInterval"),
         default=Default[int](value=3600),
     )
     ipsec_replay_window: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="ipsecReplayWindow", validation_alias="ipsecReplayWindow", default=Default[int](value=512)
+        validation_alias=AliasPath("data", "ipsecReplayWindow"), default=Default[int](value=512)
     )
     ipsec_ciphersuite: Union[Global[IpsecCiphersuite], Variable, Default[IpsecCiphersuite]] = Field(
-        serialization_alias="ipsecCiphersuite",
-        validation_alias="ipsecCiphersuite",
+        validation_alias=AliasPath("data", "ipsecCiphersuite"),
         default=Default[IpsecCiphersuite](value="aes256-gcm"),
     )
     perfect_forward_secrecy: Union[Global[PfsGroup], Variable, Default[PfsGroup]] = Field(
-        serialization_alias="perfectForwardSecrecy",
-        validation_alias="perfectForwardSecrecy",
+        validation_alias=AliasPath("data", "perfectForwardSecrecy"),
         default=Default[PfsGroup](value="group-16"),
     )
-    tracker: Optional[Union[Global[str], Variable, Default[None]]] = None
+    tracker: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        default=None, validation_alias=AliasPath("data", "tracker")
+    )
     tunnel_route_via: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="tunnelRouteVia", validation_alias="tunnelRouteVia", default=None
+        validation_alias=AliasPath("data", "tunnelRouteVia"), default=None
     )
-
-
-class InterfaceIpsecCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: InterfaceIpsecData
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,177 +1,136 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Optional, Union
-from uuid import UUID
+from ipaddress import IPv4Address, IPv6Address, IPv6Interface
+from typing import Literal, Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.common import (
-    Arp,
-    StaticIPv4Address,
-    StaticIPv6Address,
-    VrrpIPv6Address,
-    VrrpTrackingObject,
-)
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.common import IkeCiphersuite, IkeGroup, IkeMode, IpsecCiphersuite, PfsGroup
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask, AdvancedGre, TunnelSourceType
 
+GreTunnelMode = Literal[
+    "ipv4",
+    "ipv6",
+]
 
-class VrrpIPv4SecondaryAddress(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    address: Union[Variable, Global[str]]
+class TunnelSourceIPv6(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
+    tunnel_source_v6: Union[Global[str], Global[IPv6Address], Variable] = Field(
+        serialization_alias="tunnelSourceV6", validation_alias="tunnelSourceV6"
+    )
+    tunnel_route_via: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="tunnelRouteVia", validation_alias="tunnelRouteVia", default=None
+    )
 
-class VrrpIPv6SecondaryAddress(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    prefix: Union[Global[str], Variable]
+class GreSourceIPv6(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
+    source_ipv6: TunnelSourceIPv6 = Field(serialization_alias="sourceIpv6", validation_alias="sourceIpv6")
 
-class VrrpIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    group_id: Union[Variable, Global[int]] = Field(serialization_alias="groupId", validation_alias="groupId")
-    priority: Union[Variable, Global[int], Default[int]] = Default[int](value=100)
-    timer: Union[Variable, Global[int], Default[int]] = Default[int](value=1000)
-    track_omp: Union[Global[bool], Default[bool]] = Field(
-        serialization_alias="trackOmp", validation_alias="trackOmp", default=Default[bool](value=False)
+class BasicGre(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    if_name: Union[Global[str], Variable] = Field(
+        serialization_alias="ifName", validation_alias="ifName", description="Minimum length of the value should be 4."
     )
-    ip_address: Union[Global[str], Variable] = Field(serialization_alias="ipAddress", validation_alias="ipAddress")
-    ip_address_secondary: Optional[List[VrrpIPv4SecondaryAddress]] = Field(
-        serialization_alias="ipAddressSecondary", validation_alias="ipAddressSecondary"
+    description: Union[Global[str], Variable, Default[None]] = Field(default=Default[None](value=None))
+    address: Optional[AddressWithMask] = None
+    ipv6_address: Optional[Union[Global[str], Global[IPv6Interface], Variable, Default[None]]] = Field(
+        serialization_alias="ipv6Address", validation_alias="ipv6Address", default=None
     )
-    tloc_pref_change: Union[Global[bool], Default[bool]] = Field(
-        serialization_alias="tlocPrefChange", validation_alias="tlocPrefChange", default=Default[bool](value=False)
+    shutdown: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
+    tunnel_protection: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="tunnelProtection", validation_alias="tunnelProtection", default=None
     )
-    tloc_pref_change_value: Optional[Union[Global[int], Variable]] = Field(
-        serialization_alias="tlocPrefChangeValue", validation_alias="tlocPrefChangeValue", default=None
+    tunnel_mode: Optional[Union[Global[GreTunnelMode], Default[GreTunnelMode]]] = Field(
+        default=None,
+        serialization_alias="tunnelMode",
+        validation_alias="tunnelMode",
     )
-    tracking_object: Optional[List[VrrpTrackingObject]] = Field(
-        serialization_alias="trackingObject", validation_alias="trackingObject", default=None
+    tunnel_source_type: Optional[Union[TunnelSourceType, GreSourceIPv6]] = Field(
+        serialization_alias="tunnelSourceType", validation_alias="tunnelSourceType", default=None
     )
-
-    prefix_list: Optional[Union[Global[str], Variable, Default[None]]] = Default[None](value=None)
-
-
-class VrrpIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    group_id: Union[Variable, Global[int]] = Field(serialization_alias="groupId", validation_alias="groupId")
-    priority: Union[Variable, Global[int], Default[int]] = Default[int](value=100)
-    timer: Union[Variable, Global[int], Default[int]] = Default[int](value=1000)
-    track_omp: Union[Global[bool], Default[bool]] = Field(
-        serialization_alias="trackOmp", validation_alias="trackOmp", default=Default[bool](value=False)
+    tunnel_destination: Union[Global[str], Global[IPv4Address], Variable] = Field(
+        serialization_alias="tunnelDestination", validation_alias="tunnelDestination"
     )
-    track_prefix_list: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="trackPrefixList", validation_alias="trackPrefixList"
+    tunnel_destination_v6: Optional[Union[Global[str], Global[IPv6Address], Variable]] = Field(
+        default=None, serialization_alias="tunnelDestinationV6", validation_alias="tunnelDestinationV6"
     )
-    ipv6: List[VrrpIPv6Address]
-    ipv6_secondary: Optional[List[VrrpIPv6SecondaryAddress]]
-
-
-class Dhcpv6Helper(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    address: Union[Global[str], Variable] = Field(serialization_alias="address", validation_alias="address")
-    vpn: Optional[Union[Global[int], Variable, Default[None]]] = None
-
-
-class AdvancedSviAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    tcp_mss: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="tcpMss", validation_alias="tcpMss", default=Default[None](value=None)
+    mtu: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=1500)
+    mtu_v6: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="mtuV6", validation_alias="mtuV6", default=None
     )
-    arp_timeout: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="arpTimeout", validation_alias="arpTimeout", default=Default[int](value=1200)
+    tcp_mss_adjust: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="tcpMssAdjust", validation_alias="tcpMssAdjust", default=None
     )
-    ip_directed_broadcast: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="ipDirectedBroadcast",
-        validation_alias="ipDirectedBroadcast",
-        default=Default[bool](value=False),
+    tcp_mss_adjust_v6: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="tcpMssAdjustV6", validation_alias="tcpMssAdjustV6", default=None
     )
-    icmp_redirect_disable: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="icmpRedirectDisable",
-        validation_alias="icmpRedirectDisable",
-        default=Default[bool](value=True),
+    clear_dont_fragment: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="clearDontFragment",
+        validation_alias="clearDontFragment",
+        default=None,
     )
-
-
-class IPv4Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    address: StaticIPv4Address = Field(serialization_alias="addressV4", validation_alias="addressV4")
-    secondary_address: Optional[List[StaticIPv4Address]] = Field(
-        serialization_alias="secondaryAddressV4", validation_alias="secondaryAddressV4", default=None
+    dpd_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="dpdInterval", validation_alias="dpdInterval", default=None
     )
-    dhcp_helper: Optional[Union[Global[List[str]], Variable, Default[None]]] = Field(
-        serialization_alias="dhcpHelperV4", validation_alias="dhcpHelperV4", default=None
+    dpd_retries: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="dpdRetries", validation_alias="dpdRetries", default=None
     )
-
-
-class IPv6Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    address: Union[Global[str], Variable, Default[None]] = Field(
-        serialization_alias="addressV6", validation_alias="addressV6"
+    ike_version: Optional[Union[Global[int], Default[int]]] = Field(
+        serialization_alias="ikeVersion", validation_alias="ikeVersion", default=None
     )
-    secondary_address: Optional[List[StaticIPv6Address]] = Field(
-        serialization_alias="secondaryAddressV6", validation_alias="secondaryAddressV6", default=None
+    ike_mode: Optional[Union[Global[IkeMode], Variable, Default[IkeMode]]] = Field(
+        serialization_alias="ikeMode", validation_alias="ikeMode", default=None
     )
-    dhcp_helper: Optional[List[Dhcpv6Helper]] = Field(
-        serialization_alias="dhcpHelperV6", validation_alias="dhcpHelperV6", default=None
+    ike_rekey_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="ikeRekeyInterval", validation_alias="ikeRekeyInterval", default=None
     )
-
-
-class AclQos(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    ipv4_acl_egress: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv4AclEgress", validation_alias="ipv4AclEgress", default=None
+    ike_ciphersuite: Optional[Union[Global[IkeCiphersuite], Variable, Default[IkeCiphersuite]]] = Field(
+        serialization_alias="ikeCiphersuite",
+        validation_alias="ikeCiphersuite",
+        default=None,
     )
-    ipv4_acl_ingress: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv4AclIngress", validation_alias="ipv4AclIngress", default=None
+    ike_group: Optional[Union[Global[IkeGroup], Variable, Default[IkeGroup]]] = Field(
+        serialization_alias="ikeGroup", validation_alias="ikeGroup", default=None
     )
-    ipv6_acl_egress: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv6AclEgress", validation_alias="ipv6AclEgress", default=None
+    pre_shared_secret: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="preSharedSecret", validation_alias="preSharedSecret", default=None
     )
-    ipv6_acl_ingress: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv6AclIngress", validation_alias="ipv6AclIngress", default=None
+    ike_local_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="ikeLocalId", validation_alias="ikeLocalId", default=None
     )
-
-
-class InterfaceSviData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    shutdown: Union[Global[bool], Variable, Default[bool]] = Default[bool](value=True)
-    interface_name: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="interfaceName", validation_alias="interfaceName"
+    ike_remote_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="ikeRemoteId", validation_alias="ikeRemoteId", default=None
     )
-    description: Optional[Union[Global[str], Variable, Default[None]]] = Default[None](value=None)
-    interface_mtu: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="ifMtu", validation_alias="ifMtu", default=Default[int](value=1500)
+    ipsec_rekey_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="ipsecRekeyInterval",
+        validation_alias="ipsecRekeyInterval",
+        default=None,
     )
-    ip_mtu: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="ipMtu", validation_alias="ipMtu", default=Default[int](value=1500)
+    ipsec_replay_window: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="ipsecReplayWindow", validation_alias="ipsecReplayWindow", default=None
     )
-    ipv4: Optional[IPv4Address] = None
-    ipv6: Optional[IPv6Address] = None
-    acl_qos: Optional[AclQos] = Field(serialization_alias="aclQos", validation_alias="aclQos", default=None)
-    arp: Optional[List[Arp]] = None
-    vrrp: Optional[List[VrrpIPv4]] = None
-    vrrp_ipv6: Optional[List[VrrpIPv6]] = Field(
-        serialization_alias="vrrpIpv6", validation_alias="vrrpIpv6", default=None
+    ipsec_ciphersuite: Optional[Union[Global[IpsecCiphersuite], Variable, Default[IpsecCiphersuite]]] = Field(
+        serialization_alias="ipsecCiphersuite",
+        validation_alias="ipsecCiphersuite",
+        default=None,
     )
-    dhcp_client_v6: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="dhcpClientV6", validation_alias="dhcpClientV6", default=Default[bool](value=False)
+    perfect_forward_secrecy: Optional[Union[Global[PfsGroup], Variable, Default[PfsGroup]]] = Field(
+        serialization_alias="perfectForwardSecrecy",
+        validation_alias="perfectForwardSecrecy",
+        default=None,
     )
-    advanced: AdvancedSviAttributes = AdvancedSviAttributes()
 
 
-class InterfaceSviCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class InterfaceGreParcel(_ParcelBase):
+    type_: Literal["lan/vpn/interface/gre"] = Field(default="lan/vpn/interface/gre", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    name: str
-    description: Optional[str] = None
-    data: InterfaceSviData
-    metadata: Optional[dict] = None
+    basic: BasicGre = Field(validation_alias=AliasPath("data", "basic"))
+    advanced: Optional[AdvancedGre] = Field(default=None, validation_alias=AliasPath("data", "advanced"))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Address, IPv6Address, IPv6Interface
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field, IPvAnyAddress
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.common import Prefix
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask
 
 ProtocolIPv4 = Literal[
     "bgp",
     "ospf",
     "opsfv3",
     "connected",
     "static",
@@ -93,18 +94,22 @@
 ]
 
 
 class DnsIPv4(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     primary_dns_address_ipv4: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="primaryDnsAddressIpv4", validation_alias="primaryDnsAddressIpv4"
+        default=Default[None](value=None),
+        serialization_alias="primaryDnsAddressIpv4",
+        validation_alias="primaryDnsAddressIpv4",
     )
     secondary_dns_address_ipv4: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="secondaryDnsAddressIpv4", validation_alias="secondaryDnsAddressIpv4"
+        default=Default[None](value=None),
+        serialization_alias="secondaryDnsAddressIpv4",
+        validation_alias="secondaryDnsAddressIpv4",
     )
 
 
 class DnsIPv6(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     primary_dns_address_ipv6: Union[Variable, Global[str], Default[None]] = Field(
@@ -115,40 +120,46 @@
     )
 
 
 class HostMapping(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     host_name: Union[Variable, Global[str]] = Field(serialization_alias="hostName", validation_alias="hostName")
-    list_of_ip: Union[Variable, Global[str]] = Field(serialization_alias="listOfIp", validation_alias="listOfIp")
+    list_of_ip: Union[Variable, Global[List[IPvAnyAddress]]] = Field(
+        serialization_alias="listOfIp", validation_alias="listOfIp"
+    )
 
 
 class RoutePrefix(BaseModel):
-    ip_address: Union[Variable, Global[str]] = Field(serialization_alias="ipAddress", validation_alias="ipAddress")
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+
+    ip_address: Union[Variable, Global[str], Global[IPv4Address], Global[IPv6Address]] = Field(
+        serialization_alias="ipAddress", validation_alias="ipAddress"
+    )
     subnet_mask: Union[Variable, Global[str]] = Field(serialization_alias="subnetMask", validation_alias="subnetMask")
 
 
 class IPv4Prefix(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    prefix: Prefix
+    prefix: AddressWithMask
     aggregate_only: Optional[Union[Global[bool], Default[bool]]] = Field(
         serialization_alias="aggregateOnly", validation_alias="aggregateOnly", default=None
     )
-    region: Optional[Union[Variable, Global[Region], Default[str]]] = None
+    region: Optional[Union[Variable, Global[Region], Default[Region]]] = None
 
 
 class IPv6Prefix(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    prefix: Union[Global[str], Variable]
+    prefix: Union[Global[str], Global[IPv6Interface], Variable]
     aggregate_only: Optional[Union[Global[bool], Default[bool]]] = Field(
         serialization_alias="aggregateOnly", validation_alias="aggregateOnly", default=None
     )
-    region: Optional[Union[Variable, Global[Region], Default[str]]] = None
+    region: Optional[Union[Variable, Global[Region], Default[Region]]] = None
 
 
 class OmpAdvertiseIPv4(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     omp_protocol: Union[Variable, Global[ProtocolIPv4]] = Field(
         serialization_alias="ompProtocol", validation_alias="ompProtocol"
@@ -170,24 +181,24 @@
     )
     prefix_list: Optional[List[IPv6Prefix]] = None
 
 
 class IPv4RouteGatewayNextHop(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    address: Union[Variable, Global[str]]
+    address: Union[Variable, Global[str], Global[IPv4Address]]
     distance: Union[Variable, Global[int], Default[int]] = Default[int](value=1)
 
 
 class IPv4RouteGatewayNextHopWithTracker(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     address: Union[Variable, Global[str]]
     distance: Union[Variable, Global[int], Default[int]] = Default[int](value=1)
-    tracker: Union[Global[UUID], Default[None]]
+    tracker: Union[Global[UUID], Default[None]] = as_default(None)
 
 
 class NextHopContainer(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     next_hop: Optional[List[IPv4RouteGatewayNextHop]] = Field(
         serialization_alias="nextHop", validation_alias="nextHop", default=None
@@ -265,15 +276,15 @@
     address: Union[Variable, Global[str], Default[None]] = Default[None](value=None)
     distance: Union[Variable, Global[int], Default[int]] = Default[int](value=1)
 
 
 class NextHopInterfaceRouteIPv6(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    address: Union[Variable, Global[str], Default[None]] = Default[None](value=None)
+    address: Union[Variable, Global[str], Global[IPv6Address], Default[None]] = Default[None](value=None)
     distance: Union[Variable, Global[int], Default[int]] = Default[int](value=1)
 
 
 class IPStaticRouteInterface(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     interface_name: Union[Variable, Global[str]] = Field(
@@ -284,15 +295,17 @@
 
 class IPv6StaticRouteInterface(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     interface_name: Union[Variable, Global[str]] = Field(
         serialization_alias="interfaceName", validation_alias="interfaceName"
     )
-    next_hop: List[NextHopInterfaceRouteIPv6] = Field(serialization_alias="nextHop", validation_alias="nextHop")
+    interface_next_hop: List[NextHopInterfaceRouteIPv6] = Field(
+        serialization_alias="nextHop", validation_alias="nextHop"
+    )
 
 
 class InterfaceContainer(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     ip_static_route_interface: List[IPStaticRouteInterface] = Field(
         serialization_alias="ipStaticRouteInterface", validation_alias="ipStaticRouteInterface"
@@ -352,50 +365,54 @@
     )
     tracking: Union[Variable, Global[bool], Default[bool]] = Default[bool](value=True)
 
 
 class ServiceRoute(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    prefix: Prefix
+    prefix: AddressWithMask
     service: Union[Variable, Global[ServiceRouteType], Default[ServiceRouteType]] = Default[ServiceRouteType](
         value="SIG"
     )
     vpn: Global[int] = Global[int](value=0)
     sse_instance: Optional[Union[Variable, Global[str]]] = Field(
         serialization_alias="sseInstance", validation_alias="sseInstance", default=None
     )
 
 
 class StaticGreRouteIPv4(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    prefix: Prefix
-    interface: Union[Variable, Global[List[str]], Default[None]]
+    prefix: AddressWithMask
+    interface: Union[Variable, Global[List[str]], Default[None]] = Default[None](value=None)
     vpn: Global[int] = Global[int](value=0)
 
 
 class StaticIpsecRouteIPv4(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    prefix: Prefix
-    interface: Union[Variable, Global[List[str]], Default[None]]
+    prefix: AddressWithMask
+    interface: Union[Variable, Global[List[str]], Default[None]] = Default[None](value=None)
 
 
 class NatPool(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     nat_pool_name: Union[Variable, Global[int]] = Field(
         serialization_alias="natPoolName", validation_alias="natPoolName"
     )
     prefix_length: Union[Variable, Global[int]] = Field(
         serialization_alias="prefixLength", validation_alias="prefixLength"
     )
-    range_start: Union[Variable, Global[str]] = Field(serialization_alias="rangeStart", validation_alias="rangeStart")
-    range_end: Union[Variable, Global[str]] = Field(serialization_alias="rangeEnd", validation_alias="rangeEnd")
+    range_start: Union[Variable, Global[str], Global[IPv4Address]] = Field(
+        serialization_alias="rangeStart", validation_alias="rangeStart"
+    )
+    range_end: Union[Variable, Global[str], Global[IPv4Address]] = Field(
+        serialization_alias="rangeEnd", validation_alias="rangeEnd"
+    )
     overload: Union[Variable, Global[bool], Default[bool]] = Default[bool](value=True)
     direction: Union[Variable, Global[Direction]]
     tracking_object: Optional[dict] = Field(
         serialization_alias="trackingObject", validation_alias="trackingObject", default=None
     )
 
 
@@ -405,30 +422,34 @@
     nat_pool_name: Union[Variable, Global[int], Default[None]] = Field(
         serialization_alias="natPoolName", validation_alias="natPoolName"
     )
     source_port: Union[Variable, Global[int]] = Field(serialization_alias="sourcePort", validation_alias="sourcePort")
     translate_port: Union[Variable, Global[int]] = Field(
         serialization_alias="translatePort", validation_alias="translatePort"
     )
-    source_ip: Union[Variable, Global[str]] = Field(serialization_alias="sourceIp", validation_alias="sourceIp")
-    translated_source_ip: Union[Variable, Global[str]] = Field(
-        serialization_alias="TranslatedSourceIp", validation_alias="TranslatedSourceIp"
+    source_ip: Union[Variable, Global[str], Global[IPv4Address]] = Field(
+        serialization_alias="sourceIp", validation_alias="sourceIp"
+    )
+    translated_source_ip: Union[Variable, Global[str], Global[IPv4Address]] = Field(
+        serialization_alias="translatedSourceIp", validation_alias="translatedSourceIp"
     )
     protocol: Union[Variable, Global[NATPortForwardProtocol]]
 
 
 class StaticNat(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     nat_pool_name: Union[Variable, Global[int], Default[None]] = Field(
         serialization_alias="natPoolName", validation_alias="natPoolName"
     )
-    source_ip: Union[Variable, Global[str]] = Field(serialization_alias="sourceIp", validation_alias="sourceIp")
-    translated_source_ip: Union[Variable, Global[str]] = Field(
-        serialization_alias="TranslatedSourceIP", validation_alias="TranslatedSourceIP"
+    source_ip: Union[Variable, Global[str], Global[IPv4Address]] = Field(
+        serialization_alias="sourceIp", validation_alias="sourceIp"
+    )
+    translated_source_ip: Union[Variable, Global[str], Global[IPv4Address]] = Field(
+        serialization_alias="TranslatedSourceIp", validation_alias="TranslatedSourceIp"
     )
     static_nat_direction: Union[Variable, Global[Direction]] = Field(
         serialization_alias="staticNatDirection", validation_alias="staticNatDirection"
     )
     tracking_object: Optional[dict] = Field(
         serialization_alias="trackingObject", validation_alias="trackingObject", default=None
     )
@@ -437,15 +458,15 @@
 class StaticNatSubnet(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     source_ip_subnet: Union[Variable, Global[str]] = Field(
         serialization_alias="sourceIpSubnet", validation_alias="sourceIpSubnet"
     )
     translated_source_ip_subnet: Union[Variable, Global[str]] = Field(
-        serialization_alias="TranslatedSourceIpSubnet", validation_alias="TranslatedSourceIpSubnet"
+        serialization_alias="translatedSourceIpSubnet", validation_alias="translatedSourceIpSubnet"
     )
     prefix_length: Union[Variable, Global[int]] = Field(
         serialization_alias="prefixLength", validation_alias="prefixLength"
     )
     static_nat_direction: Union[Variable, Global[Direction]] = Field(
         serialization_alias="staticNatDirection", validation_alias="staticNatDirection"
     )
@@ -456,39 +477,39 @@
 
 class Nat64v4Pool(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     nat64_v4_pool_name: Union[Variable, Global[str]] = Field(
         serialization_alias="nat64V4PoolName", validation_alias="nat64V4PoolName"
     )
-    nat64_v4_pool_range_start: Union[Variable, Global[str]] = Field(
+    nat64_v4_pool_range_start: Union[Variable, Global[str], Global[IPv4Address]] = Field(
         serialization_alias="nat64V4PoolRangeStart", validation_alias="nat64V4PoolRangeStart"
     )
-    nat64_v4_pool_range_end: Union[Variable, Global[str]] = Field(
+    nat64_v4_pool_range_end: Union[Variable, Global[str], Global[IPv4Address]] = Field(
         serialization_alias="nat64V4PoolRangeEnd", validation_alias="nat64V4PoolRangeEnd"
     )
     nat64_v4_pool_overload: Union[Variable, Global[bool], Default[bool]] = Field(
         serialization_alias="nat64V4PoolOverload",
         validation_alias="nat64V4PoolOverload",
         default=Default[bool](value=False),
     )
 
 
 class RedistributeToService(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     protocol: Union[Variable, Global[RedistributeToServiceProtocol]]
-    policy: Union[Default[None], Global[UUID]]
+    policy: Union[Default[None], Global[UUID]] = Default[None](value=None)
 
 
 class RedistributeToGlobal(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     protocol: Union[Variable, Global[RedistributeToGlobalProtocol]]
-    policy: Union[Default[None], Global[UUID]]
+    policy: Union[Default[None], Global[UUID]] = Default[None](value=None)
 
 
 class RouteLeakFromGlobal(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     route_protocol: Union[Variable, Global[RouteLeakFromGlobalProtocol]] = Field(
         serialization_alias="routeProtocol", validation_alias="routeProtocol"
@@ -554,83 +575,69 @@
         serialization_alias="importRtList", validation_alias="importRtList", default=None
     )
     export_rt_list: Optional[List[RouteTarget]] = Field(
         serialization_alias="exportRtList", validation_alias="exportRtList", default=None
     )
 
 
-class LanVpnData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    vpn_id: Union[Variable, Global[int], Default[int]] = Field(serialization_alias="vpnId", validation_alias="vpnId")
-    name: Union[Variable, Global[str], Default[None]]
-    omp_admin_distance: Optional[Union[Variable, Global[int], Default[None]]] = Field(
-        serialization_alias="ompAdminDistance", validation_alias="ompAdminDistance", default=None
+class LanVpnParcel(_ParcelBase):
+    type_: Literal["lan/vpn"] = Field(default="lan/vpn", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    vpn_id: Union[Variable, Global[int]] = Field(validation_alias=AliasPath("data", "vpnId"))
+    vpn_name: Union[Variable, Global[str], Default[None]] = Field(
+        default=Default[None](value=None), validation_alias=AliasPath("data", "name")
+    )
+    omp_admin_distance_ipv4: Optional[Union[Variable, Global[int], Default[None]]] = Field(
+        validation_alias=AliasPath("data", "ompAdminDistance"), default=None
     )
     omp_admin_distance_ipv6: Optional[Union[Variable, Global[int], Default[None]]] = Field(
-        serialization_alias="ompAdminDistanceIpv6", validation_alias="ompAdminDistanceIpv6", default=None
+        validation_alias=AliasPath("data", "ompAdminDistanceIpv6"), default=None
     )
-    dns_ipv4: Optional[DnsIPv4] = Field(serialization_alias="dnsIpv4", validation_alias="dnsIpv4", default=None)
-    dns_ipv6: Optional[DnsIPv6] = Field(serialization_alias="dnsIpv6", validation_alias="dnsIpv6", default=None)
+    dns_ipv4: Optional[DnsIPv4] = Field(validation_alias=AliasPath("data", "dnsIpv4"), default=None)
+    dns_ipv6: Optional[DnsIPv6] = Field(validation_alias=AliasPath("data", "dnsIpv6"), default=None)
     new_host_mapping: Optional[List[HostMapping]] = Field(
-        serialization_alias="newHostMapping", validation_alias="newHostMapping", default=None
+        validation_alias=AliasPath("data", "newHostMapping"), default=None
     )
     omp_advertise_ipv4: Optional[List[OmpAdvertiseIPv4]] = Field(
-        serialization_alias="ompAdvertiseIpv4", validation_alias="ompAdvertiseIpv4", default=None
+        validation_alias=AliasPath("data", "ompAdvertiseIp4"), default=None  # API typo
     )
     omp_advertise_ipv6: Optional[List[OmpAdvertiseIPv6]] = Field(
-        serialization_alias="ompAdvertiseIpv6", validation_alias="ompAdvertiseIpv6", default=None
-    )
-    ipv4_route: Optional[List[StaticRouteIPv4]] = Field(
-        serialization_alias="ipv4Route", validation_alias="ipv4Route", default=None
-    )
-    ipv6_route: Optional[List[StaticRouteIPv6]] = Field(
-        serialization_alias="ipv6Route", validation_alias="ipv6Route", default=None
+        validation_alias=AliasPath("data", "ompAdvertiseIpv6"), default=None
     )
-    service: Optional[List[Service]] = None
+    ipv4_route: Optional[List[StaticRouteIPv4]] = Field(validation_alias=AliasPath("data", "ipv4Route"), default=None)
+    ipv6_route: Optional[List[StaticRouteIPv6]] = Field(validation_alias=AliasPath("data", "ipv6Route"), default=None)
+    service: Optional[List[Service]] = Field(default=None, validation_alias=AliasPath("data", "service"))
     service_route: Optional[List[ServiceRoute]] = Field(
-        serialization_alias="serviceRoute", validation_alias="serviceRoute", default=None
-    )
-    gre_route: Optional[List[StaticGreRouteIPv4]] = Field(
-        serialization_alias="greRoute", validation_alias="greRoute", default=None
+        validation_alias=AliasPath("data", "serviceRoute"), default=None
     )
+    gre_route: Optional[List[StaticGreRouteIPv4]] = Field(validation_alias=AliasPath("data", "greRoute"), default=None)
     ipsec_route: Optional[List[StaticIpsecRouteIPv4]] = Field(
-        serialization_alias="ipsecRoute", validation_alias="ipsecRoute", default=None
+        validation_alias=AliasPath("data", "ipsecRoute"), default=None
     )
-    nat_pool: Optional[List[NatPool]] = Field(serialization_alias="natPool", validation_alias="natPool", default=None)
+    nat_pool: Optional[List[NatPool]] = Field(validation_alias=AliasPath("data", "natPool"), default=None)
     nat_port_forwarding: Optional[List[NatPortForward]] = Field(
-        serialization_alias="natPortForwarding", validation_alias="natPortForwarding", default=None
-    )
-    static_nat: Optional[List[StaticNat]] = Field(
-        serialization_alias="staticNat", validation_alias="staticNat", default=None
+        validation_alias=AliasPath("data", "natPortForwarding"), default=None
     )
+    static_nat: Optional[List[StaticNat]] = Field(validation_alias=AliasPath("data", "staticNat"), default=None)
     static_nat_subnet: Optional[List[StaticNatSubnet]] = Field(
-        serialization_alias="staticNatSubnet", validation_alias="staticNatSubnet", default=None
-    )
-    nat64_v4_pool: Optional[List[Nat64v4Pool]] = Field(
-        serialization_alias="nat64V4Pool", validation_alias="nat64V4Pool", default=None
+        validation_alias=AliasPath("data", "staticNatSubnet"), default=None
     )
+    nat64_v4_pool: Optional[List[Nat64v4Pool]] = Field(validation_alias=AliasPath("data", "nat64V4Pool"), default=None)
     route_leak_from_global: Optional[List[RouteLeakFromGlobal]] = Field(
-        serialization_alias="routeLeakFromGlobal", validation_alias="routeLeakFromGlobal", default=None
+        validation_alias=AliasPath("data", "routeLeakFromGlobal"), default=None
     )
     route_leak_from_service: Optional[List[RouteLeakFromService]] = Field(
-        serialization_alias="routeLeakFromService", validation_alias="routeLeakFromService", default=None
+        validation_alias=AliasPath("data", "routeLeakFromService"), default=None
     )
     route_leak_between_services: Optional[List[RouteLeakBetweenServices]] = Field(
-        serialization_alias="routeLeakBetweenServices", validation_alias="routeLeakBetweenServices", default=None
+        validation_alias=AliasPath("data", "routeLeakBetweenServices"), default=None
     )
     mpls_vpn_ipv4_route_target: Optional[MplsVpnIPv4RouteTarget] = Field(
-        serialization_alias="mplsVpnIpv4RouteTarget", validation_alias="mplsVpnIpv4RouteTarget", default=None
+        validation_alias=AliasPath("data", "mplsVpnIpv4RouteTarget"), default=None
     )
     mpls_vpn_ipv6_route_target: Optional[MplsVpnIPv6RouteTarget] = Field(
-        serialization_alias="mplsVpnIpv6RouteTarget", validation_alias="mplsVpnIpv6RouteTarget", default=None
+        validation_alias=AliasPath("data", "mplsVpnIpv6RouteTarget"), default=None
     )
     enable_sdra: Optional[Union[Global[bool], Default[bool]]] = Field(
-        serialization_alias="enableSdra", validation_alias="enableSdra", default=None
+        validation_alias=AliasPath("data", "enableSdra"), default=None
     )
-
-
-class LanVpnCreationPayload(BaseModel):
-    name: str
-    description: Optional[str] = None
-    data: LanVpnData
-    metadata: Optional[dict] = None
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,243 +1,242 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Optional, Union
+from ipaddress import IPv4Address
+from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+
+SptThreshold = Literal["infinity", "0"]
 
 
 class LocalConfig(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     local: Union[Global[bool], Variable, Default[bool]] = Default[bool](value=False)
     threshold: Optional[Union[Global[int], Variable, Default[None]]] = Default[None](value=None)
 
 
 class MulticastBasicAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     spt_only: Union[Global[bool], Variable, Default[bool]] = Field(
         serialization_alias="sptOnly", validation_alias="sptOnly", default=Default[bool](value=False)
     )
     local_config: LocalConfig = Field(
         serialization_alias="localConfig", validation_alias="localConfig", default=LocalConfig()
     )
 
 
 class StaticJoin(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    group_address: Union[Global[str], Variable] = Field(
-        serialization_alias="groupAddress", validation_alias="groupAddress"
+    group_address: Union[Global[IPv4Address], Variable] = Field(
+        serialization_alias="groupAddress",
+        validation_alias="groupAddress",
+        description="Address range: 224.0.0.0 ~ 239.255.255.255",
     )
-    source_address: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+    source_address: Optional[Union[Global[IPv4Address], Variable, Default[None]]] = Field(
         serialization_alias="sourceAddress", validation_alias="sourceAddress", default=Default[None](value=None)
     )
 
 
 class IgmpInterfaceParameters(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     interface_name: Union[Global[str], Variable] = Field(
         serialization_alias="interfaceName", validation_alias="interfaceName"
     )
     version: Union[Global[int], Default[int]] = Default[int](value=2)
     join_group: Optional[List[StaticJoin]] = Field(
         serialization_alias="joinGroup", validation_alias="joinGroup", default=None
     )
 
 
 class IgmpAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     interface: List[IgmpInterfaceParameters]
 
 
-class SmmFlag(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    enable_ssm_flag: Global[bool] = Global[bool](value=True)
-    range: Optional[Union[Global[str], Variable, Default[None]]] = Default[None](value=None)
-
+class SsmFlag(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-class SptThreshold:
-    INFINITY = "infinity"
-    ZERO = "0"
+    enable_ssm_flag: Global[bool] = Field(
+        default=Global[bool](value=True), serialization_alias="enableSSMFlag", validation_alias="enableSSMFlag"
+    )
+    range: Union[Global[str], Variable, Default[None]] = Default[None](value=None)
 
 
-class SsmAttrubutes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class SsmAttributes(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    ssm_range_config: SmmFlag = Field(serialization_alias="ssmRangeConfig", validation_alias="ssmRangeConfig")
+    ssm_range_config: SsmFlag = Field(serialization_alias="ssmRangeConfig", validation_alias="ssmRangeConfig")
     spt_threshold: Optional[Union[Global[SptThreshold], Variable, Default[SptThreshold]]] = Field(
         serialization_alias="sptThreshold",
         validation_alias="sptThreshold",
-        default=Default[SptThreshold](value=SptThreshold.ZERO),
+        default=Default[SptThreshold](value="0"),
     )
 
 
 class PimInterfaceParameters(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     interface_name: Union[Global[str], Variable] = Field(
         serialization_alias="interfaceName", validation_alias="interfaceName"
     )
     query_interval: Union[Global[int], Variable, Default[int]] = Field(
         serialization_alias="queryInterval", validation_alias="queryInterval", default=Default[int](value=30)
     )
     join_prune_interval: Union[Global[int], Variable, Default[int]] = Field(
         serialization_alias="joinPruneInterval", validation_alias="joinPruneInterval", default=Default[int](value=60)
     )
 
 
 class StaticRpAddress(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    address: Union[Global[str], Variable]
+    address: Union[Global[IPv4Address], Variable]
     access_list: Union[Global[str], Variable] = Field(serialization_alias="accessList", validation_alias="accessList")
     override: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
 
 
 class RPAnnounce(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     interface_name: Union[Global[str], Variable] = Field(
         serialization_alias="interfaceName", validation_alias="interfaceName"
     )
     scope: Union[Global[int], Variable]
 
 
 class AutoRpAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     enable_auto_rp_flag: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="enableAutoRPFlag", validation_alias="enableAutoRPFlag", default=Default[bool](value=False)
     )
     send_rp_announce_list: Optional[List[RPAnnounce]] = Field(
         serialization_alias="sendRpAnnounceList", validation_alias="sendRpAnnounceList", default=None
     )
     send_rp_discovery: Optional[List[RPAnnounce]] = Field(
         serialization_alias="sendRpDiscovery", validation_alias="sendRpDiscovery", default=None
     )
 
 
 class RpDiscoveryScope(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     interface_name: Union[Global[str], Variable] = Field(
         serialization_alias="interfaceName", validation_alias="interfaceName"
     )
     group_list: Optional[Union[Global[str], Variable, Default[None]]] = Field(
         serialization_alias="groupList", validation_alias="groupList", default=None
     )
     interval: Optional[Union[Global[int], Variable, Default[None]]] = None
     priority: Optional[Union[Global[int], Variable, Default[None]]] = None
 
 
 class BsrCandidateAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     interface_name: Union[Global[str], Variable] = Field(
         serialization_alias="interfaceName", validation_alias="interfaceName"
     )
     mask: Optional[Union[Global[int], Variable, Default[None]]] = None
     priority: Optional[Union[Global[int], Variable, Default[None]]] = None
     accept_rp_candidate: Optional[Union[Global[str], Variable, Default[None]]] = Field(
         serialization_alias="acceptRpCandidate", validation_alias="acceptRpCandidate", default=None
     )
 
 
 class PimBsrAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     rp_candidate: Optional[List[RpDiscoveryScope]] = Field(
         serialization_alias="rpCandidate", validation_alias="rpCandidate", default=None
     )
     bsr_candidate: Optional[List[BsrCandidateAttributes]] = Field(
-        serialization_alias="bsdCandidate", validation_alias="bsdCandidate", default=None
+        serialization_alias="bsrCandidate", validation_alias="bsrCandidate", default=None
     )
 
 
 class PimAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    ssm: SsmAttrubutes
+    ssm: SsmAttributes
     interface: Optional[List[PimInterfaceParameters]] = None
-    rp_addres: Optional[List[StaticRpAddress]] = Field(
+    rp_address: Optional[List[StaticRpAddress]] = Field(
         serialization_alias="rpAddr", validation_alias="rpAddr", default=None
     )
     auto_rp: Optional[AutoRpAttributes] = Field(serialization_alias="autoRp", validation_alias="autoRp", default=None)
     pim_bsr: Optional[PimBsrAttributes] = Field(serialization_alias="pimBsr", validation_alias="pimBsr", default=None)
 
 
 class DefaultMsdpPeer(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     default_peer: Union[Global[bool], Default[bool]]
     prefix_list: Optional[Global[UUID]] = None
 
 
 class MsdpPeerAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    peer_ip: Union[Global[str], Variable] = Field(serialization_alias="peerIp", validation_alias="peerIp")
+    peer_ip: Union[Global[IPv4Address], Variable] = Field(serialization_alias="peerIp", validation_alias="peerIp")
     connect_source_intf: Optional[Union[Global[str], Variable, Default[None]]] = Field(
         serialization_alias="connectSourceIntf", validation_alias="connectSourceIntf", default=None
     )
     remote_as: Optional[Union[Global[int], Variable, Default[None]]] = Field(
         serialization_alias="remoteAs", validation_alias="remoteAs", default=None
     )
     password: Optional[Union[Global[str], Variable, Default[None]]] = None
     keepalive_interval: Optional[Union[Global[int], Variable, Default[None]]] = Field(
         serialization_alias="keepaliveInterval", validation_alias="keepaliveInterval", default=None
     )
     keepalive_holdtime: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="keepaliveHoldTime", validation_alias="keepaliveHoldTime", default=None
+        serialization_alias="keepaliveHoldTime",
+        validation_alias="keepaliveHoldTime",
+        default=None,
+        description="Hold-Time must be higher than Keep Alive",
     )
     sa_limit: Optional[Union[Global[int], Variable, Default[None]]] = Field(
         serialization_alias="saLimit", validation_alias="saLimit", default=None
     )
     default: Optional[DefaultMsdpPeer] = None
 
 
 class MsdpPeer(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     mesh_group: Optional[Union[Global[str], Variable, Default[None]]] = Field(
         serialization_alias="meshGroup", validation_alias="meshGroup", default=None
     )
     peer: List[MsdpPeerAttributes]
 
 
 class MsdpAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     msdp_list: Optional[List[MsdpPeer]] = Field(
         serialization_alias="msdpList", validation_alias="msdpList", default=None
     )
     originator_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
         serialization_alias="originatorId", validation_alias="originatorId", default=None
     )
     refresh_timer: Optional[Union[Global[int], Variable, Default[None]]] = Field(
         serialization_alias="refreshTimer", validation_alias="refreshTimer", default=None
     )
 
 
-class MulticastData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    basic: MulticastBasicAttributes = MulticastBasicAttributes()
-    igmp: Optional[IgmpAttributes] = None
-    pim: Optional[PimAttributes] = None
-    msdp: Optional[MsdpAttributes] = None
-
-
-class MulticastCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: MulticastData
-    metadata: Optional[dict] = None
+class MulticastParcel(_ParcelBase):
+    type_: Literal["routing/multicast"] = Field(default="routing/multicast", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    basic: MulticastBasicAttributes = Field(
+        validation_alias=AliasPath("data", "basic"), default_factory=MulticastBasicAttributes
+    )
+    igmp: Optional[IgmpAttributes] = Field(default=None, validation_alias=AliasPath("data", "igmp"))
+    pim: Optional[PimAttributes] = Field(default=None, validation_alias=AliasPath("data", "pim"))
+    msdp: Optional[MsdpAttributes] = Field(default=None, validation_alias=AliasPath("data", "msdp"))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
 
-ObjectTrackerType = Literal[
-    "Interface",
-    "SIG",
-    "Route",
+EndpointProtocol = Literal[
+    "tcp",
+    "udp",
 ]
 
+TrackerType = Literal["endpoint"]
 
-Criteria = Literal[
+EndpointTrackerType = Literal["static-route"]
+
+CombineBoolean = Literal[
     "and",
     "or",
 ]
 
 
-class SigTracker(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class EndpointTcpUdp(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
-    object_tracker_type: Global[ObjectTrackerType] = Field(
-        serialization_alias="objectTrackerType",
-        validation_alias="objectTrackerType",
-        default=Global[ObjectTrackerType](value="SIG"),
-    )
+    protocol: Optional[Union[Variable, Global[EndpointProtocol]]] = None
+    port: Optional[Union[Variable, Global[int]]] = None
 
 
-class InterfaceTracker(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class TrackerData(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
-    object_tracker_type: Global[ObjectTrackerType] = Field(
-        serialization_alias="objectTrackerType",
-        validation_alias="objectTrackerType",
-        default=Global[ObjectTrackerType](value="Interface"),
+    name: Union[Variable, Global[str]] = Field(serialization_alias="trackerName", validation_alias="trackerName")
+    endpoint_api_url: Optional[Union[Variable, Global[str]]] = Field(
+        serialization_alias="endpointApiUrl", validation_alias="endpointApiUrl", default=None
     )
-    interface: Union[Global[str], Variable]
-
-
-class RouteTracker(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
-    object_tracker_type: Global[ObjectTrackerType] = Field(
-        serialization_alias="objectTrackerType",
-        validation_alias="objectTrackerType",
-        default=Global[ObjectTrackerType](value="Route"),
+    endpoint_dns_name: Optional[Union[Variable, Global[str]]] = Field(
+        serialization_alias="endpointDnsName", validation_alias="endpointDnsName", default=None
+    )
+    endpoint_ip: Optional[Union[Variable, Global[str]]] = Field(
+        serialization_alias="endpointIp", validation_alias="endpointIp", default=None
+    )
+    endpoint_tcp_udp: Optional[EndpointTcpUdp] = Field(
+        serialization_alias="endpointTcpUdp", validation_alias="endpointTcpUdp", default=None
     )
-    route_ip: Union[Global[str], Variable] = Field(serialization_alias="routeIp", validation_alias="routeIp")
-    route_mask: Union[Global[str], Variable, Default[str]] = Field(
-        serialization_alias="routeMask", validation_alias="routeMask"
+    interval: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=60)
+    multiplier: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=3)
+    threshold: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=300)
+    endpoint_tracker_type: Optional[Union[Global[EndpointTrackerType], Variable, Default[EndpointTrackerType]]] = Field(
+        serialization_alias="endpointTrackerType",
+        validation_alias="endpointTrackerType",
+        default=Default[EndpointTrackerType](value="static-route"),
+    )
+    tracker_type: Optional[Union[Global[TrackerType], Variable, Default[TrackerType]]] = Field(
+        serialization_alias="trackerType",
+        validation_alias="trackerType",
+        default=Default[TrackerType](value="endpoint"),
     )
-    vpn: Union[Global[int], Variable, Default[None]] = Default[None](value=None)
 
 
-class ObjectTrackerCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class TrackerCreationPayload(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     name: str
     description: Optional[str] = None
-    data: Union[InterfaceTracker, RouteTracker, SigTracker]
+    data: TrackerData
+    metadata: Optional[dict] = None
 
 
-class ObjectTrackerRef(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class TrackerRef(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     tracker_ref: Global[UUID] = Field(serialization_alias="trackerRef", validation_alias="trackerRef")
 
 
-class ObjectTrackerGroupData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
-    tracker_refs: List[ObjectTrackerRef] = Field(serialization_alias="trackerRefs", validation_alias="trackerRefs")
-    criteria: Union[Global[Criteria], Variable, Default[Criteria]] = Default[Criteria](value="or")
+class TrackerGroupParcel(_ParcelBase):
+    type_: Literal["trackergroup"] = Field(default="trackergroup", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    tracker_refs: List[TrackerRef] = Field(validation_alias=AliasPath("data", "trackerRefs"))
+    combine_boolean: Union[Global[CombineBoolean], Variable, Default[CombineBoolean]] = Field(
+        validation_alias=AliasPath("data", "combineBoolean"),
+        default=Default[CombineBoolean](value="or"),
+    )
 
 
-class ObjectTrackerGroupCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class TrackerAssociationPayload(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    name: str
-    description: Optional[str] = None
-    data: ObjectTrackerGroupData
-    metadata: Optional[dict] = None
+    parcel_id: str = Field(serialization_alias="parcelId", validation_alias="parcelId")
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Address
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default
+from catalystwan.models.common import MetricType
 
 NetworkType = Literal[
     "broadcast",
     "point-to-point",
     "non-broadcast",
     "point-to-multipoint",
 ]
@@ -22,45 +24,43 @@
 ]
 
 AdvertiseType = Literal[
     "administrative",
     "on-startup",
 ]
 
-RedistributeProtocol = Literal[
+RedistributeProtocolOspf = Literal[
     "static",
     "connected",
     "bgp",
     "omp",
     "nat",
     "eigrp",
 ]
 
-MetricType = Literal["type1", "type2"]
-
 
 class SummaryPrefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     ip_address: Optional[Union[Global[str], Variable]] = None
     subnet_mask: Optional[Union[Global[str], Variable]] = None
 
 
 class SummaryRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     address: Optional[SummaryPrefix] = None
     cost: Optional[Union[Global[int], Variable, Default[None]]] = None
     no_advertise: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="noAdvertise", validation_alias="noAdvertise", default=None
     )
 
 
 class OspfInterfaceParametres(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     name: Optional[Union[Global[str], Variable]]
     hello_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="helloInterval", validation_alias="helloInterval", default=None
     )
     dead_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="deadInterval", validation_alias="deadInterval", default=None
@@ -82,84 +82,88 @@
     message_digest_key: Optional[Union[Global[int], Variable, Default[None]]] = Field(
         serialization_alias="messageDigestKey", validation_alias="messageDigestKey", default=None
     )
     md5: Optional[Union[Global[str], Variable, Default[None]]] = None
 
 
 class OspfArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_number: Union[Global[int], Variable] = Field(serialization_alias="aNum", validation_alias="aNum")
     area_type: Optional[Union[Global[AreaType], Default[None]]] = Field(
         serialization_alias="aType", validation_alias="aType", default=None
     )
     no_summary: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="noSummary", validation_alias="noSummary", default=None
     )
     interface: Optional[List[OspfInterfaceParametres]] = None
-    range: Optional[List[SummaryRoute]]
+    range: Optional[List[SummaryRoute]] = None
 
 
 class RouterLsa(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     ad_type: Global[AdvertiseType] = Field(serialization_alias="adType", validation_alias="adType")
     time: Optional[Union[Global[int], Variable]] = None
 
 
 class RedistributedRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    protocol: Union[Global[RedistributeProtocol], Variable]
+    protocol: Union[Global[RedistributeProtocolOspf], Variable]
     dia: Optional[Union[Global[bool], Variable, Default[bool]]] = None
-    route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
+    route_policy: Optional[Union[Default[None], Global[str], Global[UUID]]] = Field(
         serialization_alias="routePolicy", validation_alias="routePolicy", default=None
     )
 
 
-class OspfData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class OspfParcel(_ParcelBase):
+    type_: Literal["routing/ospf"] = Field(default="routing/ospf", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    router_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="routerId", validation_alias="routerId", default=None
+    router_id: Union[Global[str], Global[IPv4Address], Variable, Default[None]] = Field(
+        validation_alias=AliasPath("data", "routerId"), default=Default[None](value=None)
+    )
+    reference_bandwidth: Union[Global[int], Variable, Default[int]] = Field(
+        validation_alias=AliasPath("data", "referenceBandwidth"), default=as_default(100)
+    )
+    rfc1583: Union[Global[bool], Variable, Default[bool]] = Field(
+        validation_alias=AliasPath("data", "rfc1583"), default=as_default(True)
     )
-    reference_bandwidth: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="referenceBandwidth", validation_alias="referenceBandwidth", default=None
+    originate: Union[Global[bool], Default[bool]] = Field(
+        validation_alias=AliasPath("data", "originate"), default=as_default(False)
+    )
+    always: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        validation_alias=AliasPath("data", "always"), default=None
+    )
+    metric: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        validation_alias=AliasPath("data", "metric"), default=None
     )
-    rfc1583: Optional[Union[Global[bool], Variable, Default[bool]]] = None
-    originate: Optional[Union[Global[bool], Default[bool]]] = None
-    always: Optional[Union[Global[bool], Variable, Default[bool]]] = None
-    metric: Optional[Union[Global[int], Variable, Default[None]]] = None
     metric_type: Optional[Union[Global[MetricType], Variable, Default[None]]] = Field(
-        serialization_alias="metricType", validation_alias="metricType", default=None
+        validation_alias=AliasPath("data", "metricType"), default=None
+    )
+    external: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        default=as_default(110), validation_alias=AliasPath("data", "external")
     )
-    external: Optional[Union[Global[int], Variable, Default[int]]] = None
     inter_area: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="interArea", validation_alias="interArea", default=None
+        validation_alias=AliasPath("data", "interArea"), default=as_default(110)
     )
     intra_area: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="intraArea", validation_alias="intraArea", default=None
+        validation_alias=AliasPath("data", "intraArea"), default=as_default(110)
+    )
+    delay: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "delay"), default=as_default(200)
     )
-    delay: Optional[Union[Global[int], Variable, Default[int]]] = None
     initial_hold: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="initialHold", validation_alias="initialHold", default=None
+        validation_alias=AliasPath("data", "initialHold"), default=as_default(1000)
     )
     max_hold: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="maxHold", validation_alias="maxHold", default=None
+        validation_alias=AliasPath("data", "maxHold"), default=as_default(10000)
     )
-    redistribute: Optional[List[RedistributedRoute]] = None
-    router_lsa: Optional[List[RouterLsa]] = Field(
-        serialization_alias="routerLsa", validation_alias="routerLsa", default=None
+    redistribute: Optional[List[RedistributedRoute]] = Field(
+        validation_alias=AliasPath("data", "redistribute"), default=None
     )
-    route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
-        serialization_alias="routePolicy", validation_alias="routePolicy", default=None
+    router_lsa: Optional[List[RouterLsa]] = Field(validation_alias=AliasPath("data", "routerLsa"), default=None)
+    route_policy: Optional[Union[Default[None], Global[str], Global[UUID]]] = Field(
+        validation_alias=AliasPath("data", "routePolicy"), default=None
     )
-    area: Optional[List[OspfArea]] = None
-
-
-class OspfCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: OspfData
-    metadata: Optional[dict] = None
+    area: Optional[List[OspfArea]] = Field(validation_alias=AliasPath("data", "area"), default=None)
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Address, IPv6Interface
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.common import Prefix
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.common import MetricType
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask
 
 NetworkType = Literal[
     "broadcast",
     "point-to-point",
     "non-broadcast",
     "point-to-multipoint",
 ]
@@ -36,41 +38,40 @@
 RedistributeProtocolIPv6 = Literal[
     "static",
     "connected",
     "bgp",
     "omp",
     "eigrp",
 ]
-MetricType = Literal["type1", "type2"]
 
 
 class NoAuth(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     auth_type: Union[Global[NoAuthType], Default[NoAuthType]] = Field(
         serialization_alias="authType",
         validation_alias="authType",
         default=Default[NoAuthType](value="no-auth"),
     )
 
 
 class IpsecSha1Auth(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     auth_type: Global[IpsecSha1AuthType] = Field(
         serialization_alias="authType",
         validation_alias="authType",
         default=Global[IpsecSha1AuthType](value="ipsec-sha1"),
     )
     spi: Union[Global[int], Variable]
     auth_key: Union[Global[str], Variable] = Field(serialization_alias="authKey", validation_alias="authKey")
 
 
 class Ospfv3InterfaceParametres(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     name: Optional[Union[Global[str], Variable]] = Field(serialization_alias="ifName", validation_alias="ifName")
     hello_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="helloInterval", validation_alias="helloInterval", default=None
     )
     dead_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="deadInterval", validation_alias="deadInterval", default=None
@@ -88,145 +89,147 @@
     )
     authentication_config: Optional[Union[NoAuth, IpsecSha1Auth]] = Field(
         serialization_alias="authenticationConfig", validation_alias="authenticationConfig", default=None
     )
 
 
 class SummaryRouteIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    network: Union[Global[str], Variable]
+    network: Union[Global[str], Global[IPv6Interface], Variable]
     no_advertise: Union[Global[bool], Variable, Default[bool]] = Field(
-        serialization_alias="noAdvertise", validation_alias="noAdvertise"
+        serialization_alias="noAdvertise", validation_alias="noAdvertise", default=Default[bool](value=False)
     )
     cost: Optional[Union[Global[int], Variable, Default[None]]] = None
 
 
 class SummaryRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    network: Optional[Prefix] = None
+    network: Optional[AddressWithMask] = None
     cost: Optional[Union[Global[int], Variable, Default[None]]] = None
     no_advertise: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="noAdvertise", validation_alias="noAdvertise", default=None
     )
 
 
 class StubArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_type: Global[str] = Field(
         serialization_alias="areaType", validation_alias="areaType", default=Global[str](value="stub")
     )
     no_summary: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="noSummary", validation_alias="noSummary", default=None
     )
 
 
 class NssaArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_type: Global[str] = Field(
         serialization_alias="areaType", validation_alias="areaType", default=Global[str](value="nssa")
     )
     no_summary: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="noSummary", validation_alias="noSummary", default=None
     )
     always_translate: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="alwaysTranslate", validation_alias="alwaysTranslate", default=None
     )
 
 
 class NormalArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_type: Global[str] = Field(
         serialization_alias="areaType", validation_alias="areaType", default=Global[str](value="normal")
     )
 
 
 class DefaultArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_type: Default[None] = Field(
         serialization_alias="areaType", validation_alias="areaType", default=Default[None](value=None)
     )
 
 
 class Ospfv3IPv4Area(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_number: Union[Global[int], Variable] = Field(serialization_alias="areaNum", validation_alias="areaNum")
     area_type_config: Optional[Union[StubArea, NssaArea, NormalArea, DefaultArea]] = Field(
         serialization_alias="areaTypeConfig", validation_alias="areaTypeConfig", default=None
     )
-    interfaces: List[Ospfv3InterfaceParametres]
+    interfaces: List[Ospfv3InterfaceParametres] = Field(min_length=1)
     ranges: Optional[List[SummaryRoute]] = None
 
 
 class Ospfv3IPv6Area(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_number: Union[Global[int], Variable] = Field(serialization_alias="areaNum", validation_alias="areaNum")
     area_type_config: Optional[Union[StubArea, NssaArea, NormalArea, DefaultArea]] = Field(
         serialization_alias="areaTypeConfig", validation_alias="areaTypeConfig", default=None
     )
-    interfaces: List[Ospfv3InterfaceParametres]
-    ranges: Optional[List[SummaryRoute]] = None
+    interfaces: List[Ospfv3InterfaceParametres] = Field(min_length=1)
+    ranges: Optional[List[SummaryRouteIPv6]] = None
 
 
 class MaxMetricRouterLsa(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     action: Global[MaxMetricRouterLsaAction]
     on_startup_time: Optional[Union[Global[int], Variable]] = Field(
         serialization_alias="onStartUpTime", validation_alias="onStartUpTime", default=None
     )
 
 
 class RedistributedRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     protocol: Union[Global[RedistributeProtocol], Variable]
     nat_dia: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="natDia", validation_alias="natDia", default=None
     )
     route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="routePolicy", validation_alias="routePolicy", default=None
     )
 
 
 class RedistributedRouteIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     protocol: Union[Global[RedistributeProtocolIPv6], Variable]
     route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="routePolicy", validation_alias="routePolicy", default=None
     )
 
 
 class DefaultOriginate(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     originate: Union[Global[bool], Default[bool]]
     always: Optional[Union[Global[bool], Variable, Default[bool]]] = None
     metric: Optional[Union[Global[str], Variable, Default[None]]] = None
-    metricType: Optional[Union[Global[MetricType], Variable, Default[None]]] = None
+    metric_type: Optional[Union[Global[MetricType], Variable, Default[None]]] = Field(
+        default=None, serialization_alias="metricType", validation_alias="metricType"
+    )
 
 
 class SpfTimers(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     delay: Optional[Union[Global[int], Variable, Default[int]]] = None
     initial_hold: Optional[Union[Global[int], Variable, Default[int]]] = None
     max_hold: Optional[Union[Global[int], Variable, Default[int]]] = None
 
 
 class AdvancedOspfv3Attributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     reference_bandwidth: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="referenceBandwidth", validation_alias="referenceBandwidth", default=None
     )
     compatible_rfc1583: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="compatibleRfc1583", validation_alias="compatibleRfc1583", default=None
     )
@@ -237,63 +240,52 @@
     policy_name: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="policyName", validation_alias="policyName", default=None
     )
     filter: Optional[Union[Global[bool], Variable, Default[bool]]] = None
 
 
 class BasicOspfv3Attributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    router_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+    router_id: Optional[Union[Global[str], Global[IPv4Address], Variable, Default[None]]] = Field(
         serialization_alias="routerId", validation_alias="routerId", default=None
     )
     distance: Optional[Union[Global[int], Variable, Default[int]]] = None
     external_distance: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="externalDistance", validation_alias="externalDistance", default=None
     )
     inter_area_distance: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="interAreaDistance", validation_alias="interAreaDistance", default=None
     )
     intra_area_distance: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="intraAreaDistance", validation_alias="intraAreaDistance", default=None
     )
 
 
-class Ospfv3IPv4Data(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    basic: Optional[BasicOspfv3Attributes] = None
-    advanced: Optional[AdvancedOspfv3Attributes] = None
-    redistribute: Optional[RedistributedRoute] = None
+class Ospfv3IPv4Parcel(_ParcelBase):
+    type_: Literal["routing/ospfv3/ipv4"] = Field(default="routing/ospfv3/ipv4", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    basic: Optional[BasicOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "basic"))
+    advanced: Optional[AdvancedOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "advanced"))
+    redistribute: Optional[List[RedistributedRoute]] = Field(
+        default=None, validation_alias=AliasPath("data", "redistribute")
+    )
     max_metric_router_lsa: Optional[MaxMetricRouterLsa] = Field(
-        serialization_alias="maxMetricRouterLsa", validation_alias="maxMetricRouterLsa", default=None
+        validation_alias=AliasPath("data", "maxMetricRouterLsa"), default=None
     )
-    area: List[Ospfv3IPv4Area]
+    area: List[Ospfv3IPv4Area] = Field(validation_alias=AliasPath("data", "area"))
 
 
-class Ospfv3IPv6Data(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class Ospfv3IPv6Parcel(_ParcelBase):
+    type_: Literal["routing/ospfv3/ipv6"] = Field(default="routing/ospfv3/ipv6", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    basic: Optional[BasicOspfv3Attributes] = None
-    advanced: Optional[AdvancedOspfv3Attributes] = None
-    redistribute: Optional[RedistributedRouteIPv6] = None
+    basic: Optional[BasicOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "basic"))
+    advanced: Optional[AdvancedOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "advanced"))
+    redistribute: Optional[List[RedistributedRouteIPv6]] = Field(
+        default=None, validation_alias=AliasPath("data", "redistribute")
+    )
     max_metric_router_lsa: Optional[MaxMetricRouterLsa] = Field(
-        serialization_alias="maxMetricRouterLsa", validation_alias="maxMetricRouterLsa", default=None
+        validation_alias=AliasPath("data", "maxMetricRouterLsa"), default=None
     )
-    area: List[Ospfv3IPv6Area]
-
-
-class Ospfv3IPv4CreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: Ospfv3IPv4Data
-
-
-class Ospfv3IPv6CreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: Ospfv3IPv6Data
-    metadata: Optional[dict] = None
+    area: List[Ospfv3IPv6Area] = Field(validation_alias=AliasPath("data", "area"))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,171 +1,184 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
 
-Action = Literal[
-    "reject",
-    "accept",
+AttachmentType = Literal[
+    "custom",
+    "auto",
 ]
 
-Protocol = Literal[
-    "IPV4",
-    "IPV6",
-    "BOTH",
+TrafficDirection = Literal[
+    "UNIDIR",
+    "BIDIR",
 ]
 
-Criteria = Literal[
-    "or",
-    "and",
-    "exact",
+ReachableInterfaceType = Literal[
+    "ipv4",
+    "ipv6",
+    "tunnel",
 ]
 
-MetricType = Literal[
-    "type1",
-    "type2",
+TrackType = Literal[
+    "service-icmp",
+    "ipv6-service-icmp",
 ]
 
-Origin = Literal[
-    "egp",
-    "igp",
-    "incomplete",
+InterfaceType = Literal[
+    "fromservice",
+    "toservice",
 ]
 
+RedundancyType = Literal[
+    "active",
+    "backup",
+]
 
-class StandardCommunityList(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    criteria: Union[Global[Criteria], Default[Criteria]] = Default[Criteria](value="or")
-    standard_community_list: List[Global[UUID]] = Field(
-        serialization_alias="standardCommunityList", validation_alias="standardCommunityList"
-    )
+ServiceType = Literal[
+    "Firewall",
+    "Intrusion-detection",
+    "Intrusion-detection-prevention",
+    "NETSVC1",
+    "NETSVC2",
+    "NETSVC3",
+    "NETSVC4",
+    "NETSVC5",
+    "NETSVC6",
+    "NETSVC7",
+]
 
 
-class ExpandedCommunityList(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class GatewayInterface(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    expanded_community_list: Global[UUID] = Field(
-        serialization_alias="expandedCommunityList", validation_alias="expandedCommunityList"
+    interface_name: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="gatewayInterfaceName", validation_alias="gatewayInterfaceName", default=None
+    )
+    ip_address: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="gatewayIpAddress", validation_alias="gatewayIpAddress", default=None
+    )
+    ipv6_address: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="gatewayIpv6Address", validation_alias="gatewayIpv6Address", default=None
     )
 
 
-class RoutePolicyMatch(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ServiceInterface(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    as_path_list: Optional[Global[UUID]] = Field(
-        serialization_alias="asPathList", validation_alias="asPathList", default=None
-    )
-    community_list: Optional[Union[StandardCommunityList, ExpandedCommunityList]] = Field(
-        serialization_alias="communityList", validation_alias="communityList", default=None
+    interface_name: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="serviceInterfaceName", validation_alias="serviceInterfaceName", default=None
     )
-    ext_community_list: Optional[Global[UUID]] = Field(
-        serialization_alias="extCommunityList", validation_alias="extCommunityList", default=None
+    ip_address: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="serviceIpAddress", validation_alias="serviceIpAddress", default=None
     )
-    bgp_local_preference: Optional[Global[int]] = Field(
-        serialization_alias="bgpLocalPreference", validation_alias="bgpLocalPreference", default=None
-    )
-    metric: Optional[Global[int]] = None
-    omp_tag: Optional[Global[int]] = Field(serialization_alias="ompTag", validation_alias="ompTag", default=None)
-    ospf_tag: Optional[Global[int]] = Field(serialization_alias="ospfTag", validation_alias="ospfTag", default=None)
-    ipv4_address: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv4Address", validation_alias="ipv4Address", default=None
-    )
-    ipv4_nexthop: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv4NextHop", validation_alias="ipv4NextHop", default=None
-    )
-    ipv6_address: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv6Address", validation_alias="ipv6Address", default=None
-    )
-    ipv6_nexthop: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv6NextHop", validation_alias="ipv6NextHop", default=None
+    ipv6_address: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="serviceIpv6Address", validation_alias="serviceIpv6Address", default=None
     )
 
 
-class AcceptAction(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class TrackingIP(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    ipv4: Optional[Union[Global[str], Variable]] = None
+    ipv6: Optional[Union[Global[str], Variable]] = None
+
 
-    enable_accept_action: Default[bool] = Default[bool](value=True)
-    set_as_path: Optional[Global[int]] = Field(
-        serialization_alias="setAsPath", validation_alias="setAsPath", default=None
+class ReachableInterface(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    type: Global[ReachableInterfaceType] = Field(
+        serialization_alias="reachableInterfaceType", validation_alias="reachableInterfaceType"
     )
-    set_community: Optional[Union[Global[bool], Default[bool]]] = Field(
-        serialization_alias="setCommunity", validation_alias="setCommunity", default=None
+    name: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="reachableInterfaceName", validation_alias="reachableInterfaceName"
     )
-    set_local_preference: Optional[Global[int]] = Field(
-        serialization_alias="setLocalPreference", validation_alias="setLocalPreference", default=None
+    ip_address: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="reachableIpAddress", validation_alias="reachableIpAddress", default=None
     )
-    set_metric: Optional[Global[int]] = Field(
-        serialization_alias="setMetric", validation_alias="setMetric", default=None
+    ipv6_address: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="reachableIpv6Address", validation_alias="reachableIpv6Address", default=None
     )
-    set_metric_type: Optional[Global[MetricType]] = Field(
-        serialization_alias="setMetricType", validation_alias="setMetricType", default=None
+    tracking_ip: Optional[TrackingIP] = Field(
+        serialization_alias="trackingIp", validation_alias="trackingIp", default=None
     )
-    set_omp_tag: Optional[Global[int]] = Field(
-        serialization_alias="setOmpTag", validation_alias="setOmpTag", default=None
+    track_name: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="trackName", validation_alias="trackName", default=None
     )
-    set_origin: Optional[Global[Origin]] = Field(
-        serialization_alias="setOrigin", validation_alias="setOrigin", default=None
+    track_type: Optional[Union[Global[TrackType], Variable]] = Field(
+        serialization_alias="trackType", validation_alias="trackType", default=None
     )
-    set_ospf_tag: Optional[Global[int]] = Field(
-        serialization_alias="setOspfTag", validation_alias="setOspfTag", default=None
+
+
+class InterfaceProperties(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    gateway_interface: Optional[GatewayInterface] = Field(
+        serialization_alias="gatewayInterface", validation_alias="gatewayInterface", default=None
     )
-    set_weight: Optional[Global[int]] = Field(
-        serialization_alias="setWeight", validation_alias="setWeight", default=None
+    service_interface: Optional[ServiceInterface] = Field(
+        serialization_alias="serviceInterface", validation_alias="serviceInterface", default=None
     )
-    set_ipv4_nexthop: Optional[Global[str]] = Field(
-        serialization_alias="setIpv4NextHop", validation_alias="setIpv4NextHop", default=None
+    reachable_interface: Optional[ReachableInterface] = Field(
+        serialization_alias="reachableInterface", validation_alias="reachableInterface", default=None
     )
-    set_ipv6_nexthop: Optional[Global[str]] = Field(
-        serialization_alias="setIpv6NextHop", validation_alias="setIpv6NextHop", default=None
+    interface_type: Optional[Union[Global[InterfaceType], Variable]] = Field(
+        serialization_alias="interfaceType", validation_alias="interfaceType", default=None
+    )
+    redundancy_type: Optional[Union[Global[RedundancyType], Variable]] = Field(
+        serialization_alias="redundancyType", validation_alias="redundancyType", default=None
     )
 
 
-class AcceptActions(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class Attachment(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    accept: AcceptAction
+    interface_properties: List[InterfaceProperties] = Field(
+        serialization_alias="interfaceProperties", validation_alias="interfaceProperties"
+    )
+    traffic_direction: Optional[Union[Global[TrafficDirection], Variable]] = Field(
+        serialization_alias="trafficDirection", validation_alias="trafficDirection", default=None
+    )
 
 
-class RejectActions(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class TrackConfig(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    reject: Default[bool] = Default[bool](value=True)
+    interval: Optional[Union[Global[int], Variable]] = None
+    threshold: Optional[Union[Global[int], Variable]] = None
+    multiplier: Optional[Union[Global[int], Variable]] = None
 
 
-class RoutePolicySequence(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class Service(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    sequence_id: Global[int] = Field(serialization_alias="sequenceId", validation_alias="sequenceId")
-    sequence_name: Global[str] = Field(serialization_alias="sequenceName", validation_alias="sequenceName")
-    base_action: Union[Global[Action], Default[Action]] = Field(
-        serialization_alias="baseAction", validation_alias="baseAction", default=Default[Action](value="reject")
+    service_type: Union[Global[ServiceType], Variable] = Field(
+        serialization_alias="serviceType", validation_alias="serviceType"
     )
-    protocol: Union[Global[Protocol], Default[Protocol]] = Default[Protocol](value="IPV4")
-    match_entries: Optional[List[RoutePolicyMatch]] = Field(
-        serialization_alias="matchEntries", validation_alias="matchEntries", default=None
+    default_track: Optional[Union[Global[bool], Default[bool]]] = Field(
+        serialization_alias="defaultTrack", validation_alias="defaultTrack", default=None
     )
-    actions: Optional[List[Union[AcceptActions, RejectActions]]] = None
-
-
-class RoutePolicyData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    defautl_action: Union[Global[Action], Default[Action]] = Field(
-        serialization_alias="defaultAction",
-        validation_alias="defaultAction",
-        default=Default[Action](value="reject"),
+    track: Optional[Global[bool]] = None
+    track_config: Optional[TrackConfig] = Field(
+        serialization_alias="trackConfig", validation_alias="trackConfig", default=None
     )
-    sequences: List[RoutePolicySequence] = []
+    attachments: Optional[List[Attachment]] = None
 
 
-class RoutePolicyCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ServiceInsertionAttachmentParcel(_ParcelBase):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    name: str
-    description: Optional[str] = None
-    data: RoutePolicyData
-    metadata: Optional[dict] = None
+    attachment_type: Optional[Union[Global[AttachmentType], Variable]] = Field(
+        validation_alias=AliasPath("data", "attachmentType"), default=None
+    )
+    service_chain_instance_id: Optional[Union[Global[str], Variable]] = Field(
+        validation_alias=AliasPath("data", "serviceChainInstanceID"), default=None
+    )
+    service_chain_definition_id: Global[UUID] = Field(
+        validation_alias=AliasPath("data", "serviceChainDefinitionID"),
+    )
+    vpn: Union[Global[int], Variable] = Field(validation_alias=AliasPath("data", "vpn"))
+    services: Optional[List[Service]] = Field(default=None, validation_alias=AliasPath("data", "services"))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/policy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,86 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
-
-from typing import List, Literal, Optional, Union
+from typing import List, Literal, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Global, Variable, _ParcelBase
+from catalystwan.models.configuration.feature_profile.sdwan.transport.bgp import RefIdItem
 
-EndpointProtocol = Literal[
-    "tcp",
-    "udp",
-]
+PredefinedZone = Literal["self", "default", "untrusted"]
+SettingOn = Literal["on"]
+FailureMode = Literal["close", "open"]
 
-TrackerType = Literal["endpoint"]
 
-EndpointTrackerType = Literal["static-route"]
+class AppHosting(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    nat: Union[Global[bool], Variable]
+    database_url: Union[Global[bool], Variable] = Field(validation_alias="databaseUrl")
+    resource_profile: Union[Global[bool], Variable] = Field(validation_alias="resourceProfile")
 
-CombineBoolean = Literal[
-    "and",
-    "or",
-]
 
+class NetworkSettings(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    option_type: str = Field(default="network-settings", validation_alias="optionType")
+    value: bool
 
-class EndpointTcpUdp(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    protocol: Optional[Union[Variable, Global[EndpointProtocol]]] = None
-    port: Optional[Union[Variable, Global[int]]] = None
+class PolicySettings(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    tcp_syn_flood_limit: Global[str] = Field(default=None, validation_alias="tcpSynFloodLimit")
+    max_incomplete_tcp_limit: Global[str] = Field(default=None, validation_alias="maxIncompleteTcpLimit")
+    max_incomplete_udp_limit: Global[str] = Field(default=None, validation_alias="maxIncompleteUdpLimit")
 
+    max_incomplete_icmp_limit: Global[str] = Field(default=None, validation_alias="maxIncompleteIcmpLimit")
+    audit_trail: Global[SettingOn] = Field(default=None, validation_alias="auditTrail")
+    unified_logging: Global[SettingOn] = Field(default=None, validation_alias="unifiedLogging")
+    session_reclassify_allow: Global[SettingOn] = Field(default=None, validation_alias="sessionReclassifyAllow")
+    icmp_unreachable_allow: Global[SettingOn] = Field(default=None, validation_alias="icmpUnreachableAllow")
+    failure_mode: Global[FailureMode] = Field(default=None, validation_alias="failureMode")
+    security_logging: NetworkSettings = Field(default=None, validation_alias="securityLogging")
 
-class TrackerData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    name: Union[Variable, Global[str]] = Field(serialization_alias="trackerName", validation_alias="trackerName")
-    endpoint_api_url: Optional[Union[Variable, Global[str]]] = Field(
-        serialization_alias="endpointApiUrl", validation_alias="endpointApiUrl", default=None
-    )
-    endpoint_dns_name: Optional[Union[Variable, Global[str]]] = Field(
-        serialization_alias="endpointDnsName", validation_alias="endpointDnsName", default=None
-    )
-    endpoint_ip: Optional[Union[Variable, Global[str]]] = Field(
-        serialization_alias="endpointIp", validation_alias="endpointIp", default=None
-    )
-    endpoint_tcp_udp: Optional[EndpointTcpUdp] = Field(
-        serialization_alias="endpointTcpUdp", validation_alias="endpointTcpUdp", default=None
+class NgFirewallEntry(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    src_zone: Union[RefIdItem, Global[PredefinedZone]] = Field(
+        validation_alias="srcZone", serialization_alias="srcZone"
     )
-    interval: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=60)
-    multiplier: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=3)
-    threshold: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=300)
-    endpoint_tracker_type: Optional[Union[Global[EndpointTrackerType], Variable, Default[EndpointTrackerType]]] = Field(
-        serialization_alias="endpointTrackerType",
-        validation_alias="endpointTrackerType",
-        default=Default[EndpointTrackerType](value="static-route"),
+    dst_zone: Union[RefIdItem, Global[PredefinedZone]] = Field(
+        validation_alias="dstZone", serialization_alias="dstZone"
     )
-    tracker_type: Optional[Union[Global[TrackerType], Variable, Default[TrackerType]]] = Field(
-        serialization_alias="trackerType",
-        validation_alias="trackerType",
-        default=Default[TrackerType](value="endpoint"),
-    )
-
 
-class TrackerCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    name: str
-    description: Optional[str] = None
-    data: TrackerData
-    metadata: Optional[dict] = None
+class NgFirewall(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    ref_id: Union[Global[UUID], Global[str]] = Field(validation_alias="refId", serialization_alias="refId")
+    entries: List[NgFirewallEntry] = Field(validation_alias="entries", min_length=1)
 
 
-class TrackerRef(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class NgFirewallContainer(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    ngfirewall: NgFirewall = Field(validation_alias="ngfirewall", serialization_alias="ngfirewall")
 
-    tracker_ref: Global[UUID] = Field(serialization_alias="trackerRef", validation_alias="trackerRef")
 
+class SslDecryption(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    ssl_decryption: RefIdItem = Field(validation_alias="sslDecryption", serialization_alias="sslDecryption")
 
-class TrackerGroupData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    tracker_refs: List[TrackerRef] = Field(serialization_alias="trackerRefs", validation_alias="trackerRefs")
-    combine_boolean: Union[Global[CombineBoolean], Variable, Default[CombineBoolean]] = Field(
-        serialization_alias="combineBoolean",
-        validation_alias="combineBoolean",
-        default=Default[CombineBoolean](value="or"),
-    )
+class AdvancedInspectionProfile(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    advanced_inspection_profile: RefIdItem = Field(validation_alias="advancedInspectionProfile")
 
 
-class TrackerGroupCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: TrackerGroupData
-    metadata: Optional[dict] = None
-
-
-class TrackerAssociationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    parcel_id: str = Field(serialization_alias="parcelId", validation_alias="parcelId")
+class PolicyParcel(_ParcelBase):
+    type_: Literal["policy"] = Field(default="policy", exclude=True)
+    parcel_description: str = Field(
+        default="",
+        serialization_alias="description",
+        validation_alias="description",
+        description="Set the parcel description",
+    )
+    assembly: List[Union[NgFirewallContainer, SslDecryption, AdvancedInspectionProfile]] = Field(
+        validation_alias=AliasPath("data", "assembly"), min_length=1
+    )
+    settings: PolicySettings = Field(default=None, validation_alias=AliasPath("data", "settings"))
+    app_hosting: AppHosting = Field(default=None, validation_alias=AliasPath("data", "appHosting"))
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Address
 from typing import List, Literal, Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.common import SubnetMask
 
 CountryCode = Literal[
     "AE",
     "AR",
     "AT",
     "AU",
     "BA",
@@ -131,52 +133,56 @@
     "open",
     "personal",
     "enterprise",
 ]
 
 
 class MeStaticIpConfig(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    me_ipv4_address: Union[Global[str], Variable]
-    netmask: Union[Global[str], Variable]
-    default_gateway: Union[Global[str], Variable] = Field(
+    me_ipv4_address: Union[Global[IPv4Address], Variable] = Field(
+        serialization_alias="meIpv4Address", validation_alias="meIpv4Address"
+    )
+    netmask: Union[Global[SubnetMask], Variable]
+    default_gateway: Union[Global[IPv4Address], Variable] = Field(
         serialization_alias="defaultGateway", validation_alias="defaultGateway"
     )
 
 
 class MeIpConfig(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     me_dynamic_ip_enabled: Union[Global[bool], Default[bool]] = Field(
         serialization_alias="meDynamicIpEnabled",
         validation_alias="meDynamicIpEnabled",
         default=Default[bool](value=True),
     )
-    me_static_ip_config: Optional[MeStaticIpConfig] = None
+    me_static_ip_config: Optional[MeStaticIpConfig] = Field(
+        default=None, serialization_alias="meStaticIpCfg", validation_alias="meStaticIpCfg"
+    )
 
 
 class SecurityConfig(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     security_type: Global[SecurityType] = Field(serialization_alias="securityType", validation_alias="securityType")
-    radius_server_ip: Optional[Union[Global[str], Variable]] = Field(
+    radius_server_ip: Optional[Union[Global[IPv4Address], Variable]] = Field(
         serialization_alias="radiusServerIp", validation_alias="radiusServerIp", default=None
     )
     radius_server_port: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="radiusServerPort", validation_alias="radiusServerPort", default=None
     )
     radius_server_secret: Optional[Union[Global[str], Variable]] = Field(
         serialization_alias="radiusServerSecret", validation_alias="radiusServerSecret", default=None
     )
     passphrase: Optional[Union[Global[str], Variable]] = None
 
 
 class SSID(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     name: Global[str]
     admin_state: Union[Global[bool], Variable, Default[bool]] = Field(
         serialization_alias="adminState", validation_alias="adminState", default=Default[bool](value=True)
     )
     broadcast_ssid: Union[Global[bool], Variable, Default[bool]] = Field(
         serialization_alias="broadcastSsid", validation_alias="broadcastSsid", default=Default[bool](value=True)
@@ -189,32 +195,22 @@
     qos_profile: Union[Global[QosProfile], Variable, Default[QosProfile]] = Field(
         serialization_alias="qosProfile",
         validation_alias="qosProfile",
         default=Default[QosProfile](value="silver"),
     )
 
 
-class WirelessLanData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class WirelessLanParcel(_ParcelBase):
+    type_: Literal["wirelesslan"] = Field(default="wirelesslan", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     enable_2_4G: Union[Global[bool], Variable, Default[bool]] = Field(
-        serialization_alias="enable24G", validation_alias="enable24G", default=Default[bool](value=True)
+        validation_alias=AliasPath("data", "enable24G"), default=Default[bool](value=True)
     )
     enable_5G: Union[Global[bool], Variable, Default[bool]] = Field(
-        serialization_alias="enable5G", validation_alias="enable5G", default=Default[bool](value=True)
-    )
-    ssid: List[SSID]
-    country: Union[Global[CountryCode], Variable]
-    username: Union[Global[str], Variable]
-    password: Union[Global[str], Variable]
-    me_ip_config: MeIpConfig = Field(
-        serialization_alias="meIpConfig", validation_alias="meIpConfig", default=MeIpConfig()
+        validation_alias=AliasPath("data", "enable5G"), default=Default[bool](value=True)
     )
-
-
-class WirelessLanCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: WirelessLanData
-    metadata: Optional[dict] = None
+    ssid: List[SSID] = Field(validation_alias=AliasPath("data", "ssid"))
+    country: Union[Global[CountryCode], Variable] = Field(validation_alias=AliasPath("data", "country"))
+    username: Union[Global[str], Variable] = Field(validation_alias=AliasPath("data", "username"))
+    password: Union[Global[str], Variable] = Field(validation_alias=AliasPath("data", "password"))
+    me_ip_config: MeIpConfig = Field(validation_alias=AliasPath("data", "meIpConfig"), default=MeIpConfig())
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from ipaddress import IPv4Address, IPv6Address
-from typing import List, Optional, Union
+from typing import List, Literal, Optional, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default, as_global
 
+DEFAULT_USER_PRIVILEGE = "15"
+
 
 class PubkeyChainItem(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-    )
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
     key_string: Global[str] = Field(
         validation_alias="keyString",
         serialization_alias="keyString",
-        pattern="^AAAA[0-9A-Za-z+/]+[=]{0,3}$",
         description="Set the RSA key string",
     )
 
     # Literal["ssh-rsa"]
     key_type: Global[str] = Field(
         default=Global[str](value="ssh-rsa"),
         serialization_alias="keyType",
         validation_alias="keyType",
         description="Only RSA is supported",
     )
 
 
 class UserItem(BaseModel):
-    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    model_config = ConfigDict(extra="ignore", populate_by_name=True)
 
     name: Union[Global[str], Variable] = Field(description="Set the username")
     password: Union[Global[str], Variable] = Field(
         description=(
             "Set the user password [Note: Catalyst SD-WAN Manager will encrypt this field before saving."
             "Cleartext strings will not be returned back to the user in GET responses for sensitive fields.]"
         )
     )
     privilege: Union[Global[str], Variable, Default[str], None] = Field(
-        None, description="Set Privilege Level for this user"
+        default=as_default(DEFAULT_USER_PRIVILEGE), description="Set Privilege Level for this user"
     )
     pubkey_chain: Optional[List[PubkeyChainItem]] = Field(
         default=None,
         validation_alias="pubkeyChain",
         serialization_alias="pubkeyChain",
         description="List of RSA public-keys per user",
         max_length=2,
@@ -256,33 +255,38 @@
         default=None,
         validation_alias="ifAuthenticated",
         serialization_alias="ifAuthenticated",
         description="Succeed if user has authenticated",
     )
 
 
-class AAA(_ParcelBase):
+class AAAParcel(_ParcelBase):
+    type_: Literal["aaa"] = Field(default="aaa", exclude=True)
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+
     authentication_group: Union[Variable, Global[bool], Default[bool]] = Field(
         default=as_default(False),
         validation_alias=AliasPath("data", "authenticationGroup"),
         description="Authentication configurations parameters",
     )
     accounting_group: Union[Variable, Global[bool], Default[bool]] = Field(
         default=as_default(False),
         validation_alias=AliasPath("data", "accountingGroup"),
         description="Accounting configurations parameters",
     )
-    # local, radius, tacacs
     server_auth_order: Global[List[str]] = Field(
+        # local, radius, tacacs
         validation_alias=AliasPath("data", "serverAuthOrder"),
         min_length=1,
         max_length=4,
         description="ServerGroups priority order",
     )
-    user: Optional[List[UserItem]] = Field(default=None, description="Create local login account", min_length=1)
+    user: Optional[List[UserItem]] = Field(
+        default=None, validation_alias=AliasPath("data", "user"), description="Create local login account", min_length=1
+    )
     radius: Optional[List[Radius]] = Field(
         default=None, validation_alias=AliasPath("data", "radius"), description="Configure the Radius serverGroup"
     )
     tacacs: Optional[List[Tacacs]] = Field(
         default=None, validation_alias=AliasPath("data", "tacacs"), description="Configure the TACACS serverGroup"
     )
     accounting_rule: Optional[List[AccountingRuleItem]] = Field(
@@ -300,14 +304,56 @@
     )
     authorization_rule: Optional[List[AuthorizationRuleItem]] = Field(
         default=None,
         validation_alias=AliasPath("data", "authorizationRule"),
         description="Configure the Authorization Rules",
     )
 
+    @classmethod
+    def new(
+        cls,
+        parcel_name: str,
+        server_auth_order: List[str],
+        *,
+        parcel_description: Optional[str] = None,
+        accounting_group: bool = False,
+        authorization_console: bool = False,
+        authorization_config_commands: bool = False
+    ) -> "AAAParcel":
+        return cls(
+            parcel_name=parcel_name,
+            parcel_description=parcel_description,
+            server_auth_order=as_global(server_auth_order),
+            accounting_group=as_global(accounting_group),
+            authorization_console=as_global(authorization_console),
+            authorization_config_commands=as_global(authorization_config_commands),
+        )
+
+    def add_user(
+        self,
+        name: str,
+        password: str,
+        *,
+        privilege: str = DEFAULT_USER_PRIVILEGE,
+        pubkey_chain: Optional[List[PubkeyChainItem]] = None
+    ) -> UserItem:
+        user = UserItem(
+            name=as_global(name),
+            password=as_global(password),
+            privilege=as_global(privilege),
+            pubkey_chain=pubkey_chain,
+        )
+        if self.user is None:
+            self.user = []
+        self.user.append(user)
+        return user
+
+    def set_server_auth_order(self, server_auth_order: List[str]) -> None:
+        self.server_auth_order = as_global(server_auth_order)
+
     def add_authorization_rule(
         self, rule_id: str, method: str, level: str, group: List[str], if_authenticated: bool
     ) -> AuthorizationRuleItem:
         item = AuthorizationRuleItem(
             rule_id=as_global(rule_id),
             method=as_global(method),
             level=as_global(level),
```

### Comparing `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py` & `catalystwan-0.33.7.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_profile.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,70 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import Literal, Union
+from typing import Literal, Optional, Union
 
-from pydantic import AliasPath, BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field, model_validator
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
 
-ConfigTypeValue = Literal["non-eSim"]
-
-
-class ControllerConfig(BaseModel):
-    model_config = ConfigDict(extra="forbid", arbitrary_types_allowed=True, populate_by_name=True)
-    id: Union[Variable, Global[str]] = Field(min_length=1, max_length=5, description="Cellular ID")
-    slot: Union[Variable, Global[int], Default[int], None] = Field(
-        default=None, description="Set primary SIM slot", ge=0, le=1
+AuthenticationType = Literal[
+    "chap",
+    "pap",
+    "pap_chap",
+]
+
+
+class NeedAuthentication(BaseModel):
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    password: Union[Variable, Global[str]] = Field()
+    type: Union[Variable, Global[AuthenticationType]] = Field()
+    username: Union[Variable, Global[str]] = Field()
+
+
+class Authentication(BaseModel):
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    need_authentication: Optional[NeedAuthentication] = Field(
+        default=None, validation_alias="needAuthentication", serialization_alias="needAuthentication"
     )
-    max_retry: Union[Variable, Global[int], Default[None], None] = Field(
-        default=None,
-        description="Set SIM failover retries",
-        ge=0,
-        le=65535,
-        serialization_alias="maxRetry",
-        validation_alias="maxRetry",
+    no_authentication: Optional[Default[Literal["none"]]] = Field(
+        default=None, validation_alias="noAuthentication", serialization_alias="noAuthentication"
     )
-    failover_timer: Union[Variable, Global[int], Default[None], None] = Field(
-        default=None,
-        description="Set SIM failover timeout in minutes",
-        ge=3,
-        le=7,
-        serialization_alias="failovertimer",
-        validation_alias="failovertimer",
+
+    @model_validator(mode="after")
+    def validate_authentication_exclusive(self):
+        if self.need_authentication and self.no_authentication:
+            raise ValueError("Only one of need_authentication and no_authentication can be set")
+        return self
+
+
+PdnType = Literal[
+    "ipv4",
+    "ipv4v6",
+    "ipv6",
+]
+
+
+class ProfileInfo(BaseModel):
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    apn: Union[Variable, Global[str]] = Field()
+    authentication: Optional[Authentication] = Field(default=None)
+    no_overwrite: Optional[Union[Variable, Global[bool], Default[None]]] = Field(
+        default=None, validation_alias="noOverwrite", serialization_alias="noOverwrite"
     )
-    auto_sim: Union[Variable, Global[bool], Default[None], None] = Field(
-        default=None,
-        description="Enable/Disable Firmware Auto Sim",
-        serialization_alias="autoSim",
-        validation_alias="autoSim",
+    pdn_type: Optional[Union[Variable, Default[PdnType], Global[PdnType]]] = Field(
+        default=None, validation_alias="pdnType", serialization_alias="pdnType"
     )
 
 
-class CellularController(_ParcelBase):
-    config_type: Default[ConfigTypeValue] = Field(
-        default=Default(value="non-eSim"), validation_alias=AliasPath("data", "configType")
-    )
-    controller_config: ControllerConfig = Field(validation_alias=AliasPath("data", "controllerConfig"))
+class ProfileConfig(BaseModel):
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    id: Union[Variable, Global[int]] = Field()
+    profile_info: ProfileInfo = Field(validation_alias="profileInfo", serialization_alias="profileInfo")
+
 
-    @staticmethod
-    def add_controller_config(
-        id: Union[Variable, Global[str]],
-        max_retry: Union[Variable, Global[int], Default[None], None] = None,
-        failover_timer: Union[Variable, Global[int], Default[None], None] = None,
-        auto_sim: Union[Variable, Global[bool], Default[None], None] = None,
-    ):
-        return ControllerConfig(id=id, max_retry=max_retry, failover_timer=failover_timer, auto_sim=auto_sim)
+class CellularProfileParcel(_ParcelBase):
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    type_: Literal["cellular-profile"] = Field(default="cellular-profile", exclude=True, frozen=True)
+    profile_config: ProfileConfig = Field(validation_alias=AliasPath("data", "profileConfig"))
+    config_type: Optional[Default[Literal["non-eSim"]]] = Field(
+        default=None, validation_alias=AliasPath("data", "configType")
+    )
```

### Comparing `catalystwan-0.33.7/catalystwan/models/device_inventory.py` & `catalystwan-0.33.7.dev0/catalystwan/models/device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/models/misc/application_protocols.py` & `catalystwan-0.33.7.dev0/catalystwan/models/misc/application_protocols.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/centralized.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/centralized.py`

 * *Files 10% similar despite different names*

```diff
@@ -229,40 +229,26 @@
     def add_hub_and_spoke_policy(self, hub_and_spoke_policy_id: UUID) -> None:
         policy_definition = assert_feature_defintion(self.policy_definition)
         policy_definition.assembly.append(HubAndSpokePolicyItem(definition_id=hub_and_spoke_policy_id))
 
     @model_validator(mode="before")
     @classmethod
     def try_parse_policy_definition_string(cls, values):
-        # GET /template/policy/vsmart contains string in policyDefinition field
+        # this is needed because GET /template/policy/vsmart contains string in policyDefinition field
         # while POST /template/policy/vsmart requires a regular object
         # it makes sense to reuse that model for both requests and present parsed data to the user
-        # This is only applicable for "feature" policy type
-        # when we are trying to deserialize "policyDefinition" field obtained from remote as string
-        json_policy_type = values.get("policyType")
-        json_policy_definition = values.get("policyDefinition")
-        if json_policy_type == "feature":
-            if isinstance(json_policy_definition, str):
-                values["policyDefinition"] = CentralizedPolicyDefinition.model_validate_json(json_policy_definition)
-            else:
-                values["policyDefinition"] = CentralizedPolicyDefinition()
+        if not isinstance(values, dict):
+            return values
+        if (policy_definition := values.get("policyDefinition")) and values.get("policyType") != "cli":
+            if isinstance(policy_definition, str):
+                values["policyDefinition"] = CentralizedPolicyDefinition.model_validate_json(policy_definition)
+        else:
+            values["policyDefinition"] = CentralizedPolicyDefinition()
         return values
 
-    @model_validator(mode="after")
-    def check_definition_content_by_type(self):
-        if self.policy_type == "cli":
-            assert isinstance(
-                self.policy_definition, str
-            ), "policy definition must be provided as string for cli policy"
-        elif self.policy_type == "feature":
-            assert isinstance(
-                self.policy_definition, CentralizedPolicyDefinition
-            ), "policy definition must be provided as CentralizedPolicyDefinition object for feature policy"
-        return self
-
 
 class CentralizedPolicyEditPayload(PolicyEditPayload, CentralizedPolicy):
     rid: Optional[int] = Field(default=None, serialization_alias="@rid", validation_alias="@rid")
 
 
 class CentralizedPolicyInfo(PolicyInfo, CentralizedPolicyEditPayload):
     pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/access_control_list.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/access_control_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 from typing import Any, List, Literal, Set, Tuple, Union
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
 from catalystwan.models.policy.policy_definition import (
+    BasicPolicyAction,
+    BasicPolicyActionType,
     ClassMapAction,
     ClassMapListEntry,
     CountAction,
-    DefaultAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataPrefixListEntry,
     DestinationIPEntry,
     DestinationPortEntry,
     DSCPEntry,
     LogAction,
     Match,
     MirrorAction,
-    NextHopEntry,
+    NextHopActionEntry,
     PacketLengthEntry,
     PLPEntry,
     PolicerAction,
-    PolicyActionType,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     ProtocolEntry,
     Reference,
     SourceDataPrefixListEntry,
     SourceIPEntry,
     SourcePortEntry,
     TCPEntry,
@@ -65,15 +67,15 @@
     entries: List[AclPolicySequenceMatchEntry] = []
 
 
 class AclPolicySequence(PolicyDefinitionSequenceBase):
     sequence_type: Literal["acl"] = Field(
         default="acl", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
-    base_action: PolicyActionType = Field(
+    base_action: BasicPolicyActionType = Field(
         default="accept", serialization_alias="baseAction", validation_alias="baseAction"
     )
     match: AclPolicySequenceMatch = AclPolicySequenceMatch()
     actions: List[AclPolicySequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_dscp(self, dscp: int) -> None:
@@ -87,25 +89,25 @@
 
     def match_high_plp(self) -> None:
         self._insert_match(PLPEntry(value="high"))
 
     def match_protocols(self, protocols: Set[int]) -> None:
         self._insert_match(ProtocolEntry.from_protocol_set(protocols))
 
-    def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_list_id))
+    def match_source_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
+        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_lists))
 
     def match_source_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(SourceIPEntry.from_ipv4_networks(networks))
 
     def match_source_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(SourcePortEntry.from_port_set_and_ranges(ports, port_ranges))
 
     def match_destination_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(DestinationDataPrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(DestinationDataPrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_destination_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(DestinationIPEntry.from_ipv4_networks(networks))
 
     def match_destination_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(DestinationPortEntry.from_port_set_and_ranges(ports, port_ranges))
 
@@ -123,15 +125,15 @@
 
     @accept_action
     def associate_dscp_action(self, dscp: int) -> None:
         self._insert_action_in_set(DSCPEntry(value=str(dscp)))
 
     @accept_action
     def associate_next_hop_action(self, next_hop: IPv4Address) -> None:
-        self._insert_action_in_set(NextHopEntry(value=next_hop))
+        self._insert_action_in_set(NextHopActionEntry(value=next_hop))
 
     @accept_action
     def associate_mirror_action(self, mirror_list_id: UUID) -> None:
         self._insert_action(MirrorAction(parameter=Reference(ref=mirror_list_id)))
 
     @accept_action
     def associate_class_map_list_action(self, class_map_list_id: UUID) -> None:
@@ -140,24 +142,32 @@
     @accept_action
     def associate_policer_list_action(self, policer_list_id: UUID) -> None:
         self._insert_action(PolicerAction(parameter=Reference(ref=policer_list_id)))
 
 
 class AclPolicy(AclPolicyHeader, DefinitionWithSequencesCommonBase):
     sequences: List[AclPolicySequence] = []
-    default_action: DefaultAction = Field(
-        default=DefaultAction(type="drop"),
+    default_action: BasicPolicyAction = Field(
+        default=BasicPolicyAction(type="drop"),
         serialization_alias="defaultAction",
         validation_alias="defaultAction",
     )
     model_config = ConfigDict(populate_by_name=True)
 
     def add_acl_sequence(
-        self, name: str = "Access Control List", base_action: PolicyActionType = "accept"
+        self, name: str = "Access Control List", base_action: BasicPolicyActionType = "accept"
     ) -> AclPolicySequence:
         seq = AclPolicySequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         self.add(seq)
         return seq
+
+
+class AclPolicyEditPayload(AclPolicy, PolicyDefinitionId):
+    pass
+
+
+class AclPolicyGetResponse(AclPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/access_control_list_ipv6.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/access_control_list_ipv6.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 from typing import Any, List, Literal, Set, Tuple, Union
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
 from catalystwan.models.policy.policy_definition import (
+    BasicPolicyAction,
+    BasicPolicyActionType,
     ClassMapAction,
     ClassMapListEntry,
     CountAction,
-    DefaultAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataIPv6PrefixListEntry,
     DestinationIPv6Entry,
     DestinationPortEntry,
     LogAction,
     Match,
     MirrorAction,
     NextHeaderEntry,
-    NextHopEntry,
+    NextHopActionEntry,
     PacketLengthEntry,
     PLPEntry,
     PolicerAction,
-    PolicyActionType,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     Reference,
     SourceDataIPv6PrefixListEntry,
     SourceIPv6Entry,
     SourcePortEntry,
     TCPEntry,
     TrafficClassEntry,
@@ -65,15 +67,15 @@
     entries: List[AclIPv6PolicySequenceMatchEntry] = []
 
 
 class AclIPv6PolicySequence(PolicyDefinitionSequenceBase):
     sequence_type: Literal["aclv6"] = Field(
         default="aclv6", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
-    base_action: PolicyActionType = Field(
+    base_action: BasicPolicyActionType = Field(
         default="accept", serialization_alias="baseAction", validation_alias="baseAction"
     )
     match: AclIPv6PolicySequenceMatch = AclIPv6PolicySequenceMatch()
     actions: List[AclIPv6PolicySequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_next_header(self, next_header: int) -> None:
@@ -85,24 +87,24 @@
     def match_low_plp(self) -> None:
         self._insert_match(PLPEntry(value="low"))
 
     def match_high_plp(self) -> None:
         self._insert_match(PLPEntry(value="high"))
 
     def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(SourceDataIPv6PrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(SourceDataIPv6PrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_source_ip(self, networks: List[IPv6Network]) -> None:
         self._insert_match(SourceIPv6Entry.from_ipv6_networks(networks))
 
     def match_source_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(SourcePortEntry.from_port_set_and_ranges(ports, port_ranges))
 
     def match_destination_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(DestinationDataIPv6PrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(DestinationDataIPv6PrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_destination_ip(self, networks: List[IPv6Network]) -> None:
         self._insert_match(DestinationIPv6Entry.from_ipv6_networks(networks))
 
     def match_destination_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(DestinationPortEntry.from_port_set_and_ranges(ports, port_ranges))
 
@@ -119,15 +121,15 @@
         self._insert_action(CountAction(parameter=counter_name))
 
     def associate_log_action(self) -> None:
         self._insert_action(LogAction())
 
     @accept_action
     def associate_next_hop_action(self, next_hop: IPv4Address) -> None:
-        self._insert_action_in_set(NextHopEntry(value=next_hop))
+        self._insert_action_in_set(NextHopActionEntry(value=next_hop))
 
     @accept_action
     def associate_traffic_class_action(self, traffic_class: int) -> None:
         self._insert_action_in_set(TrafficClassEntry(value=str(traffic_class)))
 
     @accept_action
     def associate_mirror_action(self, mirror_list_id: UUID) -> None:
@@ -140,24 +142,32 @@
     @accept_action
     def associate_policer_list_action(self, policer_list_id: UUID) -> None:
         self._insert_action(PolicerAction(parameter=Reference(ref=policer_list_id)))
 
 
 class AclIPv6Policy(AclIPv6PolicyHeader, DefinitionWithSequencesCommonBase):
     sequences: List[AclIPv6PolicySequence] = []
-    default_action: DefaultAction = Field(
-        default=DefaultAction(type="drop"),
+    default_action: BasicPolicyAction = Field(
+        default=BasicPolicyAction(type="drop"),
         serialization_alias="defaultAction",
         validation_alias="defaultAction",
     )
     model_config = ConfigDict(populate_by_name=True)
 
     def add_acl_sequence(
-        self, name: str = "Access Control List", base_action: PolicyActionType = "accept"
+        self, name: str = "Access Control List", base_action: BasicPolicyActionType = "accept"
     ) -> AclIPv6PolicySequence:
         seq = AclIPv6PolicySequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv6",
         )
         self.add(seq)
         return seq
+
+
+class AclIPv6PolicyEditPayload(AclIPv6Policy, PolicyDefinitionId):
+    pass
+
+
+class AclIPv6PolicyGetResponse(AclIPv6Policy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/control.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/control.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,40 +3,41 @@
 from ipaddress import IPv4Address
 from typing import Any, List, Literal, Optional, Union, overload
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
-from catalystwan.models.common import TLOCColor
-from catalystwan.models.policy.lists_entries import EncapType
+from catalystwan.models.common import EncapType, TLOCColor
 from catalystwan.models.policy.policy_definition import (
     AffinityEntry,
-    Carrier,
     CarrierEntry,
+    CarrierType,
     ColorListEntry,
     CommunityAdditiveEntry,
     CommunityEntry,
     CommunityListEntry,
-    DefaultAction,
+    ControlPathType,
     DefinitionWithSequencesCommonBase,
     DomainIDEntry,
     ExpandedCommunityListEntry,
     ExportToAction,
     GroupIDEntry,
     Match,
     MultiRegionRole,
     OMPTagEntry,
     OriginatorEntry,
     OriginEntry,
     OriginProtocol,
-    PathType,
     PathTypeEntry,
-    PolicyActionType,
+    PolicyAcceptRejectAction,
+    PolicyAcceptRejectActionType,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     PreferenceEntry,
     PrefixListEntry,
     RegionEntry,
     RegionListEntry,
     RoleEntry,
     ServiceEntry,
@@ -115,15 +116,15 @@
     entries: List[AnyControlPolicyTLOCSequenceMatchEntry] = []
 
 
 class ControlPolicyRouteSequence(PolicyDefinitionSequenceBase):
     sequence_type: Literal["route"] = Field(
         default="route", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
-    base_action: PolicyActionType = Field(
+    base_action: PolicyAcceptRejectActionType = Field(
         default="reject", serialization_alias="baseAction", validation_alias="baseAction"
     )
     match: ControlPolicyRouteSequenceMatch = ControlPolicyRouteSequenceMatch()
     actions: List[ControlPolicyRouteSequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_color_list(self, color_list_id: UUID) -> None:
@@ -132,23 +133,23 @@
     def match_community_list(self, community_list_id: UUID) -> None:
         self._insert_match(CommunityListEntry(ref=community_list_id))
 
     def match_expanded_community_list(self, expanded_community_list_id: UUID) -> None:
         self._insert_match(ExpandedCommunityListEntry(ref=expanded_community_list_id))
 
     def match_omp_tag(self, omp_tag: int) -> None:
-        self._insert_match(OMPTagEntry(value=str(omp_tag)))
+        self._insert_match(OMPTagEntry(value=omp_tag))
 
     def match_origin(self, origin: OriginProtocol) -> None:
         self._insert_match(OriginEntry(value=origin))
 
     def match_originator(self, originator: IPv4Address) -> None:
         self._insert_match(OriginatorEntry(value=originator))
 
-    def match_path_type(self, path_type: PathType) -> None:
+    def match_path_type(self, path_type: ControlPathType) -> None:
         self._insert_match(PathTypeEntry(value=path_type))
 
     def match_preference(self, preference: int) -> None:
         self._insert_match(PreferenceEntry(value=str(preference)))
 
     def match_region(self, region_id: int, role: Optional[MultiRegionRole] = None) -> None:
         self._insert_match(RegionEntry(value=str(region_id)))
@@ -188,15 +189,15 @@
         if additive:
             self._insert_action_in_set(CommunityAdditiveEntry())
         else:
             self._remove_action_from_set(CommunityAdditiveEntry().field)
 
     @accept_action
     def associate_omp_tag_action(self, omp_tag: int) -> None:
-        self._insert_action_in_set(OMPTagEntry(value=str(omp_tag)))
+        self._insert_action_in_set(OMPTagEntry(value=omp_tag))
 
     @accept_action
     def associate_preference_action(self, preference: int) -> None:
         self._insert_action_in_set(PreferenceEntry(value=str(preference)))
 
     @overload
     def associate_service_action(self, service_type: ServiceType, vpn: int, *, tloc_list_id: UUID) -> None:
@@ -234,35 +235,35 @@
         self._insert_action(ExportToAction(parameter=VPNListEntry(ref=vpn_list_id)))
 
 
 class ControlPolicyTLOCSequence(PolicyDefinitionSequenceBase):
     sequence_type: Literal["tloc"] = Field(
         default="tloc", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
-    base_action: PolicyActionType = Field(
+    base_action: PolicyAcceptRejectActionType = Field(
         default="reject", serialization_alias="baseAction", validation_alias="baseAction"
     )
     match: ControlPolicyTLOCSequenceMatch = ControlPolicyTLOCSequenceMatch()
     actions: List[ControlPolicyTLOCSequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
-    def match_carrier(self, carrier: Carrier) -> None:
+    def match_carrier(self, carrier: CarrierType) -> None:
         self._insert_match(CarrierEntry(value=carrier))
 
     def match_color_list(self, color_list_id: UUID) -> None:
         self._insert_match(ColorListEntry(ref=color_list_id))
 
     def match_domain_id(self, domain_id: int) -> None:
         self._insert_match(DomainIDEntry(value=str(domain_id)))
 
     def match_group_id(self, group_id: int) -> None:
         self._insert_match(GroupIDEntry(value=str(group_id)))
 
     def match_omp_tag(self, omp_tag: int) -> None:
-        self._insert_match(OMPTagEntry(value=str(omp_tag)))
+        self._insert_match(OMPTagEntry(value=omp_tag))
 
     def match_originator(self, originator: IPv4Address) -> None:
         self._insert_match(OriginatorEntry(value=originator))
 
     def match_preference(self, preference: int) -> None:
         self._insert_match(PreferenceEntry(value=str(preference)))
 
@@ -290,15 +291,15 @@
         self._insert_match(TLOCListEntry(ref=tloc_list_id))
 
     def match_tloc(self, ip: IPv4Address, color: TLOCColor, encap: EncapType) -> None:
         self._insert_match(TLOCEntry(value=TLOCEntryValue(ip=ip, color=color, encap=encap)))
 
     @accept_action
     def associate_omp_tag_action(self, omp_tag: int) -> None:
-        self._insert_action_in_set(OMPTagEntry(value=str(omp_tag)))
+        self._insert_action_in_set(OMPTagEntry(value=omp_tag))
 
     @accept_action
     def associate_preference_action(self, preference: int) -> None:
         self._insert_action_in_set(PreferenceEntry(value=str(preference)))
 
     @accept_action
     def associate_affinity_action(self, affinity: int) -> None:
@@ -309,35 +310,43 @@
     Union[ControlPolicyRouteSequence, ControlPolicyTLOCSequence],
     Field(discriminator="sequence_type"),
 ]
 
 
 class ControlPolicy(ControlPolicyHeader, DefinitionWithSequencesCommonBase):
     sequences: List[AnyControlPolicySequence] = []
-    default_action: DefaultAction = Field(
-        default=DefaultAction(type="reject"),
+    default_action: PolicyAcceptRejectAction = Field(
+        default=PolicyAcceptRejectAction(type="reject"),
         serialization_alias="defaultAction",
         validation_alias="defaultAction",
     )
     model_config = ConfigDict(populate_by_name=True)
 
     def add_route_sequence(
-        self, name: str = "Route", base_action: PolicyActionType = "reject"
+        self, name: str = "Route", base_action: PolicyAcceptRejectActionType = "reject"
     ) -> ControlPolicyRouteSequence:
         seq = ControlPolicyRouteSequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         self.add(seq)
         return seq
 
     def add_tloc_sequence(
-        self, name: str = "TLOC", base_action: PolicyActionType = "reject"
+        self, name: str = "TLOC", base_action: PolicyAcceptRejectActionType = "reject"
     ) -> ControlPolicyTLOCSequence:
         seq = ControlPolicyTLOCSequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         self.add(seq)
         return seq
+
+
+class ControlPolicyEditPayload(ControlPolicy, PolicyDefinitionId):
+    pass
+
+
+class ControlPolicyGetResponse(ControlPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/device_access.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/device_access.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 from typing import Any, List, Literal, Optional, Set, Tuple, Union
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
 from catalystwan.models.policy.policy_definition import (
+    BasicPolicyAction,
+    BasicPolicyActionType,
     CountAction,
-    DefaultAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataPrefixListEntry,
     DestinationIPEntry,
     DestinationPortEntry,
     DeviceAccessProtocol,
     Match,
-    PolicyActionType,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     SourceDataPrefixListEntry,
     SourceIPEntry,
     SourcePortEntry,
 )
 
 DeviceAccessPolicySequenceMatchEntry = Annotated[
@@ -47,60 +49,68 @@
     entries: List[DeviceAccessPolicySequenceMatchEntry] = []
 
 
 class DeviceAccessPolicySequence(PolicyDefinitionSequenceBase):
     sequence_type: Literal["deviceaccesspolicy"] = Field(
         default="deviceaccesspolicy", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
-    base_action: PolicyActionType = Field(
+    base_action: BasicPolicyActionType = Field(
         default="accept", serialization_alias="baseAction", validation_alias="baseAction"
     )
     match: DeviceAccessPolicySequenceMatch = DeviceAccessPolicySequenceMatch()
     actions: List[DeviceAccessPolicySequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_device_access_protocol(self, port: DeviceAccessProtocol) -> None:
         self._insert_match(DestinationPortEntry.from_port_set_and_ranges(ports={port}))
 
-    def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_list_id))
+    def match_source_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
+        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_lists))
 
     def match_source_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(SourceIPEntry.from_ipv4_networks(networks))
 
     def match_source_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(SourcePortEntry.from_port_set_and_ranges(ports, port_ranges))
 
     def match_destination_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(DestinationDataPrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(DestinationDataPrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_destination_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(DestinationIPEntry.from_ipv4_networks(networks))
 
     def associate_count_action(self, counter_name: str) -> None:
         self._insert_action(CountAction(parameter=counter_name))
 
 
 class DeviceAccessPolicy(DeviceAccessPolicyHeader, DefinitionWithSequencesCommonBase):
     sequences: List[DeviceAccessPolicySequence] = []
-    default_action: DefaultAction = Field(
-        default=DefaultAction(type="drop"),
+    default_action: BasicPolicyAction = Field(
+        default=BasicPolicyAction(type="drop"),
         serialization_alias="defaultAction",
         validation_alias="defaultAction",
     )
     model_config = ConfigDict(populate_by_name=True)
 
     def add_acl_sequence(
         self,
         name: str = "Device Access Control List",
-        base_action: PolicyActionType = "accept",
+        base_action: BasicPolicyActionType = "accept",
         device_access_protocol: Optional[DeviceAccessProtocol] = None,
     ) -> DeviceAccessPolicySequence:
         seq = DeviceAccessPolicySequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         if device_access_protocol is not None:
             seq.match_device_access_protocol(port=device_access_protocol)
         self.add(seq)
         return seq
+
+
+class DeviceAccessPolicyEditPayload(DeviceAccessPolicy, PolicyDefinitionId):
+    pass
+
+
+class DeviceAccessPolicyGetResponse(DeviceAccessPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/device_access_ipv6.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/device_access_ipv6.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 from typing import Any, List, Literal, Optional, Set, Tuple, Union
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
 from catalystwan.models.policy.policy_definition import (
+    BasicPolicyAction,
+    BasicPolicyActionType,
     CountAction,
-    DefaultAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataIPv6PrefixListEntry,
     DestinationIPv6Entry,
     DestinationPortEntry,
     DeviceAccessProtocol,
     Match,
-    PolicyActionType,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     SourceDataIPv6PrefixListEntry,
     SourceIPv6Entry,
     SourcePortEntry,
 )
 
 DeviceAccessIPv6PolicySequenceMatchEntry = Annotated[
@@ -47,60 +49,68 @@
     entries: List[DeviceAccessIPv6PolicySequenceMatchEntry] = []
 
 
 class DeviceAccessIPv6PolicySequence(PolicyDefinitionSequenceBase):
     sequence_type: Literal["deviceaccesspolicyv6"] = Field(
         default="deviceaccesspolicyv6", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
-    base_action: PolicyActionType = Field(
+    base_action: BasicPolicyActionType = Field(
         default="accept", serialization_alias="baseAction", validation_alias="baseAction"
     )
     match: DeviceAccessIPv6PolicySequenceMatch = DeviceAccessIPv6PolicySequenceMatch()
     actions: List[DeviceAccessIPv6PolicySequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_device_access_protocol(self, port: DeviceAccessProtocol) -> None:
         self._insert_match(DestinationPortEntry.from_port_set_and_ranges(ports={port}))
 
     def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(SourceDataIPv6PrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(SourceDataIPv6PrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_source_ip(self, networks: List[IPv6Network]) -> None:
         self._insert_match(SourceIPv6Entry.from_ipv6_networks(networks))
 
     def match_source_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(SourcePortEntry.from_port_set_and_ranges(ports, port_ranges))
 
     def match_destination_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(DestinationDataIPv6PrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(DestinationDataIPv6PrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_destination_ip(self, networks: List[IPv6Network]) -> None:
         self._insert_match(DestinationIPv6Entry.from_ipv6_networks(networks))
 
     def associate_count_action(self, counter_name: str) -> None:
         self._insert_action(CountAction(parameter=counter_name))
 
 
 class DeviceAccessIPv6Policy(DeviceAccessIPv6PolicyHeader, DefinitionWithSequencesCommonBase):
     sequences: List[DeviceAccessIPv6PolicySequence] = []
-    default_action: DefaultAction = Field(
-        default=DefaultAction(type="drop"),
+    default_action: BasicPolicyAction = Field(
+        default=BasicPolicyAction(type="drop"),
         serialization_alias="defaultAction",
         validation_alias="defaultAction",
     )
     model_config = ConfigDict(populate_by_name=True)
 
     def add_acl_sequence(
         self,
         name: str = "Device Access Control List",
-        base_action: PolicyActionType = "accept",
+        base_action: BasicPolicyActionType = "accept",
         device_access_protocol: Optional[DeviceAccessProtocol] = None,
     ) -> DeviceAccessIPv6PolicySequence:
         seq = DeviceAccessIPv6PolicySequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         if device_access_protocol is not None:
             seq.match_device_access_protocol(port=device_access_protocol)
         self.add(seq)
         return seq
+
+
+class DeviceAccessIPv6PolicyEditPayload(DeviceAccessIPv6Policy, PolicyDefinitionId):
+    pass
+
+
+class DeviceAccessIPv6PolicyGetResponse(DeviceAccessIPv6Policy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/hub_and_spoke.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/hub_and_spoke.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
-from catalystwan.models.policy.policy_definition import PolicyDefinitionBase
+from catalystwan.models.policy.policy_definition import (
+    PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
+)
 
 
 class Hub(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     site_list: UUID = Field(validation_alias="siteList", serialization_alias="siteList")
     preference: Optional[str] = None
     prefix_lists: List[UUID] = Field(default=[], validation_alias="prefixLists", serialization_alias="prefixLists")
@@ -67,7 +71,15 @@
             equal_preference=True,
             advertise_tloc=(advertise_tloc_list is not None),
             tloc_list=advertise_tloc_list,
             spokes=spokes,
         )
         self.definition.sub_definitions.append(sub_definition)
         return sub_definition
+
+
+class HubAndSpokePolicyEditPayload(HubAndSpokePolicy, PolicyDefinitionId):
+    pass
+
+
+class HubAndSpokePolicyGetResponse(HubAndSpokePolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/mesh.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/mesh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
-from catalystwan.models.policy.policy_definition import PolicyDefinitionBase
+from catalystwan.models.policy.policy_definition import (
+    PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
+)
 
 
 class Region(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     name: str
     site_lists: List[UUID] = Field(validation_alias="siteLists", serialization_alias="siteLists")
 
@@ -29,7 +33,15 @@
     def from_vpn_list(name: str, vpn_list: UUID) -> "MeshPolicy":
         return MeshPolicy(name=name, definition=MeshPolicyDefinition(vpn_list=vpn_list))
 
     def add_region(self, name: str, site_lists: List[UUID]) -> Region:
         region = Region(name=name, site_lists=site_lists)
         self.definition.regions.append(region)
         return region
+
+
+class MeshPolicyEditPayload(MeshPolicy, PolicyDefinitionId):
+    pass
+
+
+class MeshPolicyGetResponse(MeshPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/qos_map.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/qos_map.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,70 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field, field_validator, model_validator
 
-from catalystwan.models.policy.policy_definition import PolicyDefinitionBase
+from catalystwan.models.common import IntStr
+from catalystwan.models.policy.policy_definition import (
+    PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
+)
 
 QoSScheduling = Literal[
     "llq",
     "wrr",
 ]
 
 QoSDropType = Literal[
     "tail-drop",
     "red-drop",
 ]
 
 
 class QoSScheduler(BaseModel):
-    queue: str
-    class_map_ref: Union[UUID, Literal[""]] = Field(serialization_alias="classMapRef", validation_alias="classMapRef")
-    bandwidth_percent: str = Field("1", serialization_alias="bandwidthPercent", validation_alias="bandwidthPercent")
-    buffer_percent: str = Field("1", serialization_alias="bufferPercent", validation_alias="bufferPercent")
-    burst: Optional[str] = None
+    queue: IntStr = Field(ge=0, le=8)
+    class_map_ref: Optional[UUID] = Field(
+        default=None, serialization_alias="classMapRef", validation_alias="classMapRef"
+    )
+    bandwidth_percent: IntStr = Field(
+        default=1, ge=1, le=100, serialization_alias="bandwidthPercent", validation_alias="bandwidthPercent"
+    )
+    buffer_percent: IntStr = Field(
+        default=1, ge=1, le=100, serialization_alias="bufferPercent", validation_alias="bufferPercent"
+    )
+    burst: Optional[IntStr] = Field(default=None, ge=5000, le=10_000_000)
     scheduling: QoSScheduling = "wrr"
     drops: QoSDropType = "tail-drop"
     temp_key_values: Optional[str] = Field(
         default=None, serialization_alias="tempKeyValues", validation_alias="tempKeyValues"
     )
 
     @staticmethod
     def get_default_control_scheduler() -> "QoSScheduler":
         return QoSScheduler(
-            queue="0",
-            class_map_ref="",
-            bandwidth_percent="100",
-            buffer_percent="100",
-            burst="15000",
+            queue=0,
+            bandwidth_percent=100,
+            buffer_percent=100,
+            burst=15000,
             scheduling="llq",
             drops="tail-drop",
         )
 
     model_config = ConfigDict(populate_by_name=True)
 
-    @field_validator("queue")
+    @field_validator("class_map_ref", mode="before")
     @classmethod
-    def check_queue(cls, queue_str: str):
-        assert 0 <= int(queue_str) <= 7
-        return queue_str
-
-    @field_validator("bandwidth_percent", "buffer_percent")
-    @classmethod
-    def check_bandwidth_and_buffer_percent(cls, percent_str: str):
-        assert 1 <= int(percent_str) <= 100
-        return percent_str
-
-    @field_validator("burst")
-    @classmethod
-    def check_burst(cls, burst_val: Union[str, None]):
-        if burst_val is not None:
-            assert 5000 <= int(burst_val) <= 10_000_000
-        return burst_val
+    def check_optional_class_map_ref(cls, class_map_ref: Union[str, None]):
+        # None and "" indicates missing value, both can be found in server responses
+        if not class_map_ref:
+            return None
+        return class_map_ref
 
 
 class QoSMapDefinition(BaseModel):
     qos_schedulers: List[QoSScheduler] = Field(serialization_alias="qosSchedulers", validation_alias="qosSchedulers")
     model_config = ConfigDict(populate_by_name=True)
 
 
@@ -82,23 +81,31 @@
         buffer: int = 1,
         scheduling: QoSScheduling = "wrr",
         drops: QoSDropType = "tail-drop",
         burst: Optional[int] = None,
     ) -> None:
         self.definition.qos_schedulers.append(
             QoSScheduler(
-                queue=str(queue),
+                queue=queue,
                 class_map_ref=class_map_ref,
-                bandwidth_percent=str(bandwidth),
-                buffer_percent=str(buffer),
-                burst=str(burst) if burst is not None else None,
+                bandwidth_percent=bandwidth,
+                buffer_percent=buffer,
+                burst=burst,
                 scheduling=scheduling,
                 drops=drops,
             )
         )
 
     @model_validator(mode="after")
     def generate_default_control_scheduler(self):
         if not self.definition.qos_schedulers:
             # Only when creating (not when value obtained from remote is present)
             self.definition = QoSMapDefinition(qos_schedulers=[QoSScheduler.get_default_control_scheduler()])
         return self
+
+
+class QoSMapPolicyEditPayload(QoSMapPolicy, PolicyDefinitionId):
+    pass
+
+
+class QoSMapPolicyGetResponse(QoSMapPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/rewrite.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/rewrite.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,33 +5,43 @@
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from catalystwan.models.policy.policy_definition import (
     DefinitionWithSequencesCommonBase,
     PLPEntryType,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
 )
 
 
 class RewritePolicyHeader(PolicyDefinitionBase):
     type: Literal["rewriteRule"] = "rewriteRule"
 
 
 class RewritePolicyRule(BaseModel):
     class_: UUID = Field(serialization_alias="class", validation_alias="class")
     plp: str
     dscp: str
-    l2cos: str = Field(serialization_alias="layer2Cos", validation_alias="layer2Cos")
+    l2cos: int = Field(serialization_alias="layer2Cos", validation_alias="layer2Cos")
     model_config = ConfigDict(populate_by_name=True)
 
 
 class RewritePolicyDefinition(BaseModel):
     rules: List[RewritePolicyRule] = []
 
 
 class RewritePolicy(RewritePolicyHeader, DefinitionWithSequencesCommonBase):
     definition: RewritePolicyDefinition = RewritePolicyDefinition()
 
     def add_rule(self, class_map_ref: UUID, dscp: int, l2cos: int, plp: PLPEntryType) -> None:
-        self.definition.rules.append(RewritePolicyRule(class_=class_map_ref, plp=plp, dscp=str(dscp), l2cos=str(l2cos)))
+        self.definition.rules.append(RewritePolicyRule(class_=class_map_ref, plp=plp, dscp=str(dscp), l2cos=l2cos))
 
     model_config = ConfigDict(populate_by_name=True)
+
+
+class RewritePolicyEditPayload(RewritePolicy, PolicyDefinitionId):
+    pass
+
+
+class RewritePolicyGetResponse(RewritePolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/rule_set.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/rule_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from ipaddress import IPv4Network, IPv6Network
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field, model_validator
-from typing_extensions import Annotated
 
 from catalystwan.models.common import check_fields_exclusive
-from catalystwan.models.policy.policy_definition import PolicyDefinitionBase, Reference, VariableName
+from catalystwan.models.policy.policy_definition import (
+    PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
+    Reference,
+    VariableName,
+)
 
 
 class RuleBase(BaseModel):
     rule: str = ""
     order: str = ""
     action: str = "permit"
     source_security_group: Optional[Reference] = Field(
@@ -33,15 +38,15 @@
     @model_validator(mode="after")
     def check_exclusive_fields(self):
         check_fields_exclusive(self.__dict__, {"protocol", "protocol_name", "protocol_name_list"}, False)
         return self
 
 
 class IPv4Rule(RuleBase):
-    sequence_ip_type: Literal["ipv4"] = Field(
+    sequence_ip_type: Literal[None, "ipv4"] = Field(
         default="ipv4", serialization_alias="sequenceIpType", validation_alias="sequenceIpType"
     )
     source_ip: Union[IPv4Network, VariableName, None] = Field(
         default=None, serialization_alias="sourceIP", validation_alias="sourceIP"
     )
     source_data_prefix_list: Optional[Reference] = Field(
         default=None, serialization_alias="sourceDataPrefixList", validation_alias="sourceDataPrefixList"
@@ -140,15 +145,15 @@
             self.__dict__,
             {"destination_security_group", "destination_ipv6", "destination_ipv6_data_prefix_list"},
             False,
         )
         return self
 
 
-Rule = Annotated[Union[IPv4Rule, IPv6Rule], Field(discriminator="sequence_ip_type")]
+Rule = Union[IPv4Rule, IPv6Rule]
 
 
 class RuleSetDefinition(BaseModel):
     rules: List[Rule] = []
 
 
 class RuleSet(PolicyDefinitionBase):
@@ -250,7 +255,15 @@
             destination_port=destination_port,
             destination_port_list=Reference(ref=destination_port_list_id) if destination_port_list_id else None,
             protocol=" ".join(str(p) for p in protocols) if protocols else None,
             protocol_name=" ".join(p for p in protocol_names) if protocol_names else None,
             protocol_name_list=Reference(ref=protocol_name_list_id) if protocol_name_list_id else None,
         )
         self.add(ipv4_rule)
+
+
+class RuleSetEditPayload(RuleSet, PolicyDefinitionId):
+    pass
+
+
+class RuleSetGetResponse(RuleSet, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/security_group.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/security_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 
 from ipaddress import IPv4Network, IPv6Network
 from typing import Literal, Optional, Union
 
 from pydantic import BaseModel, ConfigDict, Field, model_validator
 
 from catalystwan.models.common import check_any_of_exclusive_field_sets, check_fields_exclusive
-from catalystwan.models.policy.policy_definition import PolicyDefinitionBase, Reference, VariableName
+from catalystwan.models.policy.policy_definition import (
+    PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
+    Reference,
+    VariableName,
+)
 
 SequenceIPType = Literal[
     "ipv4",
     "ipv6",
 ]
 
 
@@ -56,14 +62,20 @@
     type: Literal["securityGroup"] = "securityGroup"
     mode: Literal["unified"] = "unified"
     sequence_ip_type: SequenceIPType = Field(alias="sequenceIpType")
     definition: Union[SecurityGroupIPv4Definition, SecurityGroupIPv6Definition]
 
     @model_validator(mode="after")
     def validate_by_sequence_ip_type(self):
-        if (
-            self.sequence_ip_type == SequenceIPType.IPV4 and isinstance(self.definition, SecurityGroupIPv6Definition)
-        ) or (
-            self.sequence_ip_type == SequenceIPType.IPV6 and isinstance(self.definition, SecurityGroupIPv4Definition)
+        if (self.sequence_ip_type == "ipv6" and not isinstance(self.definition, SecurityGroupIPv6Definition)) or (
+            self.sequence_ip_type == "ipv4" and not isinstance(self.definition, SecurityGroupIPv4Definition)
         ):
             raise ValueError(f"Incompatible definition for {self.sequence_ip_type} sequence")
         return self
+
+
+class SecurityGroupEditPayload(SecurityGroup, PolicyDefinitionId):
+    pass
+
+
+class SecurityGroupGetResponse(SecurityGroup, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/traffic_data.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/traffic_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from ipaddress import IPv4Address, IPv4Network
 from typing import Any, List, Literal, Optional, Set, Tuple, Union, overload
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
-from catalystwan.models.common import ServiceChainNumber, TLOCColor
-from catalystwan.models.policy.lists_entries import EncapType
+from catalystwan.models.common import EncapType, ICMPMessageType, ServiceChainNumber, TLOCColor
 from catalystwan.models.policy.policy_definition import (
     AppListEntry,
+    BasicPolicyAction,
+    BasicPolicyActionType,
     CFlowDAction,
     CountAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataIPv6PrefixListEntry,
     DestinationDataPrefixListEntry,
     DestinationIPEntry,
     DestinationPortEntry,
@@ -22,30 +23,32 @@
     DNSAppListEntry,
     DNSEntry,
     DNSTypeEntryType,
     DREOptimizationAction,
     DSCPEntry,
     FallBackToRoutingAction,
     ForwardingClassEntry,
+    ICMPMessageEntry,
     LocalTLOCListEntry,
     LocalTLOCListEntryValue,
     LogAction,
     LossProtectionAction,
     LossProtectionFECAction,
     LossProtectionPacketDuplicationAction,
     LossProtectionType,
     Match,
     NATAction,
-    NextHopEntry,
+    NextHopActionEntry,
     NextHopLooseEntry,
     PacketLengthEntry,
     PLPEntry,
     PolicerListEntry,
-    PolicyActionType,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     PrefferedColorGroupListEntry,
     ProtocolEntry,
     RedirectDNSAction,
     SecureInternetGatewayAction,
     ServiceChainEntry,
     ServiceChainEntryValue,
@@ -62,32 +65,33 @@
     TrafficToEntry,
     VPNEntry,
     accept_action,
 )
 
 TrafficDataPolicySequenceEntry = Annotated[
     Union[
+        AppListEntry,
+        DestinationDataIPv6PrefixListEntry,
+        DestinationDataPrefixListEntry,
+        DestinationIPEntry,
+        DestinationPortEntry,
+        DestinationRegionEntry,
+        DNSAppListEntry,
+        DNSEntry,
+        DSCPEntry,
+        ICMPMessageEntry,
         PacketLengthEntry,
         PLPEntry,
         ProtocolEntry,
-        DSCPEntry,
+        SourceDataIPv6PrefixListEntry,
+        SourceDataPrefixListEntry,
         SourceIPEntry,
         SourcePortEntry,
-        DestinationIPEntry,
-        DestinationPortEntry,
         TCPEntry,
-        DNSEntry,
         TrafficToEntry,
-        SourceDataPrefixListEntry,
-        DestinationDataPrefixListEntry,
-        SourceDataIPv6PrefixListEntry,
-        DestinationDataIPv6PrefixListEntry,
-        DestinationRegionEntry,
-        DNSAppListEntry,
-        AppListEntry,
     ],
     Field(discriminator="field"),
 ]
 
 TrafficDataPolicySequenceActions = Any  # TODO
 
 
@@ -96,15 +100,15 @@
 
 
 class TrafficDataPolicySequenceMatch(Match):
     entries: List[TrafficDataPolicySequenceEntry] = []
 
 
 class TrafficDataPolicySequence(PolicyDefinitionSequenceBase):
-    sequence_type: Literal["data"] = Field(
+    sequence_type: Literal["applicationFirewall", "qos", "serviceChaining", "trafficEngineering", "data"] = Field(
         default="data", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
     match: TrafficDataPolicySequenceMatch = TrafficDataPolicySequenceMatch()
     actions: List[TrafficDataPolicySequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_app_list(self, app_list_id: UUID) -> None:
@@ -118,37 +122,40 @@
 
     def match_dns_response(self) -> None:
         self._insert_match(DNSEntry(value="response"))
 
     def match_dscp(self, dscp: int) -> None:
         self._insert_match(DSCPEntry(value=str(dscp)))
 
+    def match_icmp(self, icmp_message_types: List[ICMPMessageType]) -> None:
+        self._insert_match(ICMPMessageEntry(value=icmp_message_types))
+
     def match_packet_length(self, packet_lengths: Tuple[int, int]) -> None:
         self._insert_match(PacketLengthEntry.from_range(packet_lengths))
 
     def match_low_plp(self) -> None:
         self._insert_match(PLPEntry(value="low"))
 
     def match_high_plp(self) -> None:
         self._insert_match(PLPEntry(value="high"))
 
     def match_protocols(self, protocols: Set[int]) -> None:
         self._insert_match(ProtocolEntry.from_protocol_set(protocols))
 
-    def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_list_id))
+    def match_source_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
+        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_lists))
 
     def match_source_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(SourceIPEntry.from_ipv4_networks(networks))
 
     def match_source_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(SourcePortEntry.from_port_set_and_ranges(ports, port_ranges))
 
     def match_destination_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(DestinationDataPrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(DestinationDataPrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_destination_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(DestinationIPEntry.from_ipv4_networks(networks))
 
     def match_primary_destination_region(self) -> None:
         self._insert_match(DestinationRegionEntry(value="primary-region"))
 
@@ -220,15 +227,15 @@
             nat_action = NATAction.from_nat_pool(nat_pool=nat_pool)
         else:
             nat_action = NATAction.from_nat_vpn(fallback=vpn_fallback, vpn=vpn)
         self._insert_action(nat_action)
 
     @accept_action
     def associate_next_hop_action(self, next_hop: IPv4Address, loose: bool = False) -> None:
-        self._insert_action_in_set(NextHopEntry(value=next_hop))
+        self._insert_action_in_set(NextHopActionEntry(value=next_hop))
         self._insert_action_in_set(NextHopLooseEntry(value="true" if loose else "false"))
 
     @accept_action
     def associate_policer_list_action(self, policer_list_id: UUID) -> None:
         self._insert_action_in_set(PolicerListEntry(ref=policer_list_id))
 
     @overload
@@ -355,19 +362,32 @@
             self._insert_action(FallBackToRoutingAction())
         else:
             self._remove_action(FallBackToRoutingAction().type)
 
 
 class TrafficDataPolicy(TrafficDataPolicyHeader, DefinitionWithSequencesCommonBase):
     sequences: List[TrafficDataPolicySequence] = []
+    default_action: BasicPolicyAction = Field(
+        default=BasicPolicyAction(type="drop"),
+        serialization_alias="defaultAction",
+        validation_alias="defaultAction",
+    )
     model_config = ConfigDict(populate_by_name=True)
 
     def add_ipv4_sequence(
-        self, name: str = "Custom", base_action: PolicyActionType = "drop", log: bool = False
+        self, name: str = "Custom", base_action: BasicPolicyActionType = "drop", log: bool = False
     ) -> TrafficDataPolicySequence:
         seq = TrafficDataPolicySequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         self.add(seq)
         return seq
+
+
+class TrafficDataPolicyEditPayload(TrafficDataPolicy, PolicyDefinitionId):
+    pass
+
+
+class TrafficDataPolicyGetResponse(TrafficDataPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/vpn_membership.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/vpn_membership.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
-from catalystwan.models.policy.policy_definition import PolicyDefinitionBase
+from catalystwan.models.policy.policy_definition import (
+    PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
+)
 
 
 class Site(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     site_list: UUID = Field(validation_alias="siteList", serialization_alias="siteList")
     vpn_list: List[UUID] = Field(validation_alias="vpnList", serialization_alias="vpnList")
 
@@ -24,7 +28,15 @@
     type: Literal["vpnMembershipGroup"] = "vpnMembershipGroup"
     definition: VPNMembershipPolicyDefinition = VPNMembershipPolicyDefinition()
 
     def add_site(self, site_list: UUID, vpn_lists: List[UUID]) -> Site:
         site = Site(site_list=site_list, vpn_list=vpn_lists)
         self.definition.sites.append(site)
         return site
+
+
+class VPNMembershipPolicyEditPayload(VPNMembershipPolicy, PolicyDefinitionId):
+    pass
+
+
+class VPNMembershipPolicyGetResponse(VPNMembershipPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/definitions/zone_based_firewall.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/definition/zone_based_firewall.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,88 +5,114 @@
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from catalystwan.models.misc.application_protocols import ApplicationProtocol
 from catalystwan.models.policy.policy_definition import (
+    AdvancedInspectionProfileAction,
     AppListEntry,
+    AppListFlatEntry,
+    ConnectionEventsAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataPrefixListEntry,
     DestinationFQDNEntry,
     DestinationGeoLocationEntry,
     DestinationGeoLocationListEntry,
     DestinationIPEntry,
     DestinationPortEntry,
     DestinationPortListEntry,
+    DestinationScalableGroupTagListEntry,
     LogAction,
     Match,
-    PolicyActionType,
+    PolicyActionBase,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     ProtocolEntry,
     ProtocolNameEntry,
     ProtocolNameListEntry,
     RuleSetListEntry,
     SourceDataPrefixListEntry,
     SourceFQDNEntry,
     SourceFQDNListEntry,
     SourceGeoLocationEntry,
     SourceGeoLocationListEntry,
     SourceIPEntry,
     SourcePortEntry,
     SourcePortListEntry,
+    SourceScalableGroupTagListEntry,
 )
 
 ZoneBasedFWPolicySequenceEntry = Annotated[
     Union[
         AppListEntry,
+        AppListFlatEntry,
         DestinationDataPrefixListEntry,
         DestinationFQDNEntry,
         DestinationGeoLocationEntry,
         DestinationGeoLocationListEntry,
         DestinationIPEntry,
         DestinationPortEntry,
         DestinationPortListEntry,
+        DestinationScalableGroupTagListEntry,
         ProtocolEntry,
         ProtocolNameEntry,
         ProtocolNameListEntry,
         RuleSetListEntry,
         SourceDataPrefixListEntry,
         SourceFQDNEntry,
         SourceFQDNListEntry,
         SourceGeoLocationEntry,
         SourceGeoLocationListEntry,
         SourceIPEntry,
         SourcePortEntry,
         SourcePortListEntry,
+        SourceScalableGroupTagListEntry,
     ],
     Field(discriminator="field"),
 ]
 
 ZoneBasedFWPolicySequenceEntryWithRuleSets = Annotated[
     Union[
         AppListEntry,
         RuleSetListEntry,
     ],
     Field(discriminator="field"),
 ]
 
+ZoneBasedFWPolicyActions = Annotated[
+    Union[
+        AdvancedInspectionProfileAction,
+        ConnectionEventsAction,
+        LogAction,
+    ],
+    Field(discriminator="type"),
+]
+
+ZoneBasedFirewallDefaultActionType = Literal["drop", "pass"]
+ZoneBasedFirewallBaseActionType = Literal["drop", "pass", "inspect"]
+
+
+class ZoneBasedFirewallDefaultAction(PolicyActionBase):
+    type: ZoneBasedFirewallDefaultActionType
+
 
 class ZoneBasedFWPolicyMatches(Match):
     entries: List[ZoneBasedFWPolicySequenceEntry] = []
 
 
 class ZoneBasedFWPolicySequenceWithRuleSets(PolicyDefinitionSequenceBase):
     sequence_type: Literal["zoneBasedFW"] = Field(
         default="zoneBasedFW", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
     match: ZoneBasedFWPolicyMatches
     ruleset: bool = True
-    actions: List[LogAction] = []
+    actions: List[ZoneBasedFWPolicyActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_rule_set_lists(self, rule_set_ids: Set[UUID]) -> None:
         self._insert_match(RuleSetListEntry.from_rule_set_ids(rule_set_ids))
 
     def match_app_list(self, app_list_id: UUID) -> None:
         if self.base_action != "inspect":
@@ -103,16 +129,16 @@
     model_config = ConfigDict(populate_by_name=True)
 
     def match_app_list(self, app_list_id: UUID) -> None:
         if self.base_action != "inspect":
             raise ValueError("Action must be inspect when Application/Application Family List is selected.")
         self._insert_match(AppListEntry(ref=app_list_id))
 
-    def match_destination_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(DestinationDataPrefixListEntry(ref=data_prefix_list_id))
+    def match_destination_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
+        self._insert_match(DestinationDataPrefixListEntry(ref=data_prefix_lists))
 
     def match_destination_fqdn(self, fqdn: str) -> None:
         self._insert_match(DestinationFQDNEntry(value=fqdn))
 
     def match_destination_geo_location(self, geo_location: str) -> None:
         self._insert_match(DestinationGeoLocationEntry(value=geo_location))
 
@@ -121,36 +147,36 @@
 
     def match_destination_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(DestinationIPEntry.from_ipv4_networks(networks))
 
     def match_destination_ports(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(DestinationPortEntry.from_port_set_and_ranges(ports, port_ranges))
 
-    def match_destination_port_list(self, port_list_id: UUID) -> None:
-        self._insert_match(DestinationPortListEntry(ref=port_list_id))
+    def match_destination_port_list(self, data_prefix_lists: List[UUID]) -> None:
+        self._insert_match(DestinationPortListEntry(ref=data_prefix_lists))
 
     def match_protocols(self, protocols: Set[int]) -> None:
         self._insert_match(ProtocolEntry.from_protocol_set(protocols))
 
     def match_protocol_names(self, names: Set[str], protocol_map: Dict[str, ApplicationProtocol]) -> None:
         app_protocols = []
         for name in names:
             app_protocol = protocol_map.get(name, None)
             if app_protocol is None:
-                raise ValueError(f"{name} not found in protocol map keys: {protocol_map.keys()}")
+                raise ValueError(f"{name} not found in protocol map keys: {protocol_map.keys()}")  # noqa: E713
             app_protocols.append(app_protocol)
         self._insert_match(ProtocolNameEntry.from_application_protocols(app_protocols))
         self._insert_match(DestinationPortEntry.from_application_protocols(app_protocols), False)
         self._insert_match(ProtocolEntry.from_application_protocols(app_protocols), False)
 
     def match_protocol_name_list(self, protocol_name_list_id: UUID) -> None:
         self._insert_match(ProtocolNameListEntry(ref=protocol_name_list_id))
 
-    def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_list_id))
+    def match_source_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
+        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_lists))
 
     def match_source_fqdn(self, fqdn: str) -> None:
         self._insert_match(SourceFQDNEntry(value=fqdn))
 
     def match_source_fqdn_list(self, fqdn_list_id: UUID) -> None:
         self._insert_match(SourceFQDNListEntry(ref=fqdn_list_id))
 
@@ -181,25 +207,30 @@
 class ZoneBasedFWPolicyHeader(PolicyDefinitionBase):
     type: Literal["zoneBasedFW"] = "zoneBasedFW"
     mode: str = Field(default="security")
     model_config = ConfigDict(populate_by_name=True)
 
 
 class ZoneBasedFWPolicyDefinition(DefinitionWithSequencesCommonBase):
+    default_action: ZoneBasedFirewallDefaultAction = Field(
+        default=ZoneBasedFirewallDefaultAction(type="drop"),
+        serialization_alias="defaultAction",
+        validation_alias="defaultAction",
+    )
     sequences: List[Union[ZoneBasedFWPolicySequence, ZoneBasedFWPolicySequenceWithRuleSets]] = []
     entries: List[ZoneBasedFWPolicyEntry] = []
 
 
 class ZoneBasedFWPolicy(ZoneBasedFWPolicyHeader):
     type: Literal["zoneBasedFW"] = "zoneBasedFW"
-    mode: Literal["security"] = "security"
+    mode: Literal["security", "unified"] = "security"
     definition: ZoneBasedFWPolicyDefinition = ZoneBasedFWPolicyDefinition()
 
     def add_ipv4_rule(
-        self, name: str, base_action: PolicyActionType = "drop", log: bool = False
+        self, name: str, base_action: ZoneBasedFirewallBaseActionType = "drop", log: bool = False
     ) -> ZoneBasedFWPolicySequence:
         """Adds new IPv4 Rule to Zone Based Firewall Policy
 
         Args:
             name (str): Rule name
             base_action (BaseAction, optional): Rule base action (drop, pass, inspect) Defaults to BaseAction.DROP.
             log (bool, optional): If true sets log action
@@ -215,15 +246,15 @@
         )
         if log:
             sequence.actions.append(LogAction())
         self.definition.add(sequence)
         return sequence
 
     def add_ipv4_rule_sets(
-        self, name: str, base_action: PolicyActionType = "drop", log: bool = False
+        self, name: str, base_action: ZoneBasedFirewallBaseActionType = "drop", log: bool = False
     ) -> ZoneBasedFWPolicySequenceWithRuleSets:
         sequence = ZoneBasedFWPolicySequenceWithRuleSets(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
             match=ZoneBasedFWPolicyMatches(),
         )
@@ -234,7 +265,15 @@
 
     def add_zone_pair(self, source_zone_id: UUID, destination_zone_id: UUID) -> None:
         entry = ZoneBasedFWPolicyEntry(
             source_zone_id=source_zone_id,
             destination_zone_id=destination_zone_id,
         )
         self.definition.entries.append(entry)
+
+
+class ZoneBasedFWPolicyEditPayload(ZoneBasedFWPolicy, PolicyDefinitionId):
+    pass
+
+
+class ZoneBasedFWPolicyGetResponse(ZoneBasedFWPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/localized.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/localized.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal, Optional
+from typing import Any, List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field, IPvAnyAddress, field_validator
+from pydantic import BaseModel, ConfigDict, Field, IPvAnyAddress, model_validator
 
 from catalystwan.models.policy.policy import AssemblyItemBase, PolicyCreationPayload, PolicyDefinition, PolicyInfo
 
 LocalizedPolicySupportedItemType = Literal[
     "qosMap",
     "rewriteRule",
     "vpnQoSMap",
@@ -17,14 +17,19 @@
     "deviceAccessPolicy",
     "deviceaccesspolicyv6",
     "deviceAccessPolicyv6",
     "vedgeRoute",
 ]
 
 
+def assert_feature_defintion(definition: Any) -> "LocalizedPolicyDefinition":
+    assert isinstance(definition, LocalizedPolicyDefinition)
+    return definition
+
+
 class LocalizedPolicySettings(BaseModel):
     flow_visibility: Optional[bool] = Field(
         default=None, serialization_alias="flowVisibility", validation_alias="flowVisibility"
     )
     flow_visibility_ipv6: Optional[bool] = Field(
         default=None, serialization_alias="flowVisibilityIPv6", validation_alias="flowVisibilityIPv6"
     )
@@ -64,28 +69,33 @@
 class LocalizedPolicyAssemblyItem(AssemblyItemBase):
     type: LocalizedPolicySupportedItemType
     definition_id: UUID = Field(serialization_alias="definitionId", validation_alias="definitionId")
     model_config = ConfigDict(populate_by_name=True)
 
 
 class LocalizedPolicyDefinition(PolicyDefinition):
-    assembly: List[LocalizedPolicyAssemblyItem]
-    settings: LocalizedPolicySettings
+    assembly: List[LocalizedPolicyAssemblyItem] = []
+    settings: Optional[LocalizedPolicySettings] = None
 
 
 class LocalizedPolicy(PolicyCreationPayload):
-    policy_definition: LocalizedPolicyDefinition = Field(
+    policy_definition: Union[LocalizedPolicyDefinition, str] = Field(
         default=LocalizedPolicyDefinition(assembly=[], settings=LocalizedPolicySettings()),
         serialization_alias="policyDefinition",
         validation_alias="policyDefinition",
     )
-    policy_type: str = Field(default="feature", serialization_alias="policyType", validation_alias="policyType")
+    policy_type: Literal["feature", "cli"] = Field(
+        default="feature", serialization_alias="policyType", validation_alias="policyType"
+    )
 
-    def _add_item(self, type: LocalizedPolicySupportedItemType, id: UUID) -> None:
-        self.policy_definition.assembly.append(LocalizedPolicyAssemblyItem(type=type, definition_id=id))
+    def _add_item(self, type: LocalizedPolicySupportedItemType, id: UUID) -> LocalizedPolicyAssemblyItem:
+        policy_definition = assert_feature_defintion(self.policy_definition)
+        item = LocalizedPolicyAssemblyItem(type=type, definition_id=id)
+        policy_definition.assembly.append(item)
+        return item
 
     def add_qos_map(self, definition_id: UUID) -> None:
         self._add_item("qosMap", definition_id)
 
     def add_rewrite_rule(self, definition_id: UUID) -> None:
         self._add_item("rewriteRule", definition_id)
 
@@ -103,23 +113,28 @@
 
     def add_device_access_policy_ipv6(self, definition_id: UUID) -> None:
         self._add_item("deviceAccessPolicyv6", definition_id)
 
     def add_route_policy(self, definition_id: UUID) -> None:
         self._add_item("vedgeRoute", definition_id)
 
-    @field_validator("policy_definition", mode="before")
+    @model_validator(mode="before")
     @classmethod
-    def try_parse(cls, policy_definition):
+    def try_parse_policy_definition_string(cls, values):
         # this is needed because GET /template/policy/vedge contains string in policyDefinition field
         # while POST /template/policy/vedge requires a regular object
         # it makes sense to reuse that model for both requests and present parsed data to the user
-        if isinstance(policy_definition, str):
-            return LocalizedPolicyDefinition.model_validate_json(policy_definition)
-        return policy_definition
+        if not isinstance(values, dict):
+            return values
+        if (policy_definition := values.get("policyDefinition")) and values.get("policyType") != "cli":
+            if isinstance(policy_definition, str):
+                values["policyDefinition"] = LocalizedPolicyDefinition.model_validate_json(policy_definition)
+        else:
+            values["policyDefinition"] = LocalizedPolicyDefinition()
+        return values
 
 
 class LocalizedPolicyInfo(PolicyInfo, LocalizedPolicy):
     pass
 
 
 class LocalizedPolicyEditResponse(BaseModel):
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/policy.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 import datetime
 from typing import List, Literal, Optional, Sequence, Union
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
+ZoneListId = Union[UUID, Literal["self", "default"]]
+
 
 class PolicyId(BaseModel):
     policy_id: UUID = Field(serialization_alias="policyId", validation_alias="policyId")
 
 
 class NGFirewallZoneListEntry(BaseModel):
-    src_zone_list_id: UUID = Field(serialization_alias="srcZoneListId", validation_alias="srcZoneListId")
-    dst_zone_list_id: UUID = Field(serialization_alias="dstZoneListId", validation_alias="dstZoneListId")
+    src_zone_list_id: ZoneListId = Field(serialization_alias="srcZoneListId", validation_alias="srcZoneListId")
+    dst_zone_list_id: ZoneListId = Field(serialization_alias="dstZoneListId", validation_alias="dstZoneListId")
     model_config = ConfigDict(populate_by_name=True)
 
 
 class AssemblyItemBase(BaseModel):
     definition_id: UUID = Field(serialization_alias="definitionId", validation_alias="definitionId")
     type: str
     model_config = ConfigDict(populate_by_name=True)
@@ -43,14 +45,18 @@
     type: Literal["intrusionPrevention"] = "intrusionPrevention"
 
 
 class URLFilteringAssemblyItem(AssemblyItemBase):
     type: Literal["urlFiltering"] = "urlFiltering"
 
 
+class AdvancedInspectionProfileAssemblyItem(AssemblyItemBase):
+    type: Literal["advancedInspectionProfile"] = "advancedInspectionProfile"
+
+
 class AdvancedMalwareProtectionAssemblyItem(AssemblyItemBase):
     type: Literal["advancedMalwareProtection"] = "advancedMalwareProtection"
 
 
 class SSLDecryptionAssemblyItem(AssemblyItemBase):
     type: Literal["sslDecryption"] = "sslDecryption"
 
@@ -59,24 +65,23 @@
     assembly: Sequence[AssemblyItemBase] = []
 
 
 class PolicyCreationPayload(BaseModel):
     policy_name: str = Field(
         serialization_alias="policyName",
         validation_alias="policyName",
-        pattern="^[a-zA-Z0-9_-]{1,127}$",
+        pattern="^[a-zA-Z0-9_-]{0,127}$",
         description="Can include only alpha-numeric characters, hyphen '-' or underscore '_'; maximum 127 characters",
     )
     policy_description: str = Field(
         default="default description", serialization_alias="policyDescription", validation_alias="policyDescription"
     )
     policy_type: str = Field(serialization_alias="policyType", validation_alias="policyType")
     policy_definition: Union[PolicyDefinition, str] = Field(
-        serialization_alias="policyDefinition",
-        validation_alias="policyDefinition",
+        serialization_alias="policyDefinition", validation_alias="policyDefinition"
     )
     is_policy_activated: bool = Field(
         default=False, serialization_alias="isPolicyActivated", validation_alias="isPolicyActivated"
     )
     model_config = ConfigDict(populate_by_name=True)
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/policy_definition.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/policy_definition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 import datetime
 from functools import wraps
-from ipaddress import IPv4Address, IPv4Network, IPv6Network
-from typing import Any, Dict, List, MutableSequence, Optional, Protocol, Sequence, Set, Tuple, Union
+from ipaddress import IPv4Address, IPv4Network, IPv6Address, IPv6Network
+from typing import Any, Dict, List, MutableSequence, Optional, Sequence, Set, Tuple, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field, RootModel, model_validator
+from pydantic import BaseModel, ConfigDict, Field, RootModel, field_validator, model_validator
 from typing_extensions import Annotated, Literal
 
-from catalystwan.models.common import ServiceChainNumber, TLOCColor, check_fields_exclusive
+from catalystwan.models.common import (
+    CarrierType,
+    ControlPathType,
+    EncapType,
+    ICMPMessageType,
+    IntStr,
+    MultiRegionRole,
+    OriginProtocol,
+    SequenceIpType,
+    ServiceChainNumber,
+    ServiceType,
+    SpaceSeparatedPositiveIntList,
+    SpaceSeparatedUUIDList,
+    TLOCActionType,
+    TLOCColor,
+    check_fields_exclusive,
+    str_as_str_list,
+)
 from catalystwan.models.misc.application_protocols import ApplicationProtocol
-from catalystwan.models.policy.lists_entries import EncapType
-from catalystwan.typed_list import DataSequence
 
 
 def port_set_and_ranges_to_str(ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> str:
     assert ports or port_ranges
     ports_str = " ".join(f"{port_begin}-{port_end}" for port_begin, port_end in port_ranges)
     ports_str += " " if ports_str else ""
     ports_str += " ".join(str(p) for p in ports)
@@ -45,72 +60,39 @@
 
 DestinationRegion = Literal[
     "primary-region",
     "secondary-region",
     "other-region",
 ]
 
-OriginProtocol = Literal[
-    "aggregate",
-    "bgp",
-    "bgp-external",
-    "bgp-internal",
-    "connected",
-    "eigrp",
-    "ospf",
-    "ospf-inter-area",
-    "ospf-intra-area",
-    "ospf-external1",
-    "ospf-external2",
-    "rip",
-    "static",
-    "eigrp-summary",
-    "eigrp-internal",
-    "eigrp-external",
-    "lisp",
-    "nat-dia",
-    "natpool",
-    "isis",
-    "isis-level1",
-    "isis-level2",
-]
 
 PathType = Literal[
     "hierarchical-path",
     "direct-path",
     "transport-gateway-path",
 ]
 
-SequenceIpType = Literal[
-    "ipv4",
-    "ipv6",
-    "all",
-]
 
-PolicyActionType = Literal[
-    "drop",
-    "accept",
-    "pass",
-    "inspect",
-    "reject",
-]
+BasicPolicyActionType = Literal["accept", "drop"]
 
 SequenceType = Literal[
     "applicationFirewall",
     "data",
     "serviceChaining",
     "trafficEngineering",
     "qos",
     "zoneBasedFW",
     "tloc",
     "route",
     "acl",
     "aclv6",
     "deviceaccesspolicy",
     "deviceaccesspolicyv6",
+    "sslDecryption",
+    "vedgeRoute",
 ]
 
 
 Optimized = Literal[
     "true",
     "false",
 ]
@@ -122,49 +104,19 @@
 
 LossProtectionType = Literal[
     "fecAdaptive",
     "fecAlways",
     "packetDuplication",
 ]
 
-MultiRegionRole = Literal[
-    "border-router",
-    "edge-router",
-]
-
-ServiceType = Literal[
-    "FW",
-    "IDP",
-    "IDS",
-    "netsvc1",
-    "netsvc2",
-    "netsvc3",
-    "netsvc4",
-]
-
-TLOCActionType = Literal[
-    "strict",
-    "primary",
-    "backup",
-    "ecmp",
-]
+DeviceAccessProtocol = Literal[22, 161]
 
-Carrier = Literal[
-    "default",
-    "carrier1",
-    "carrier2",
-    "carrier3",
-    "carrier4",
-    "carrier5",
-    "carrier6",
-    "carrier7",
-    "carrier8",
-]
+AdvancedCommunityMatchFlag = Literal["or", "and", "exact"]
 
-DeviceAccessProtocol = Literal[22, 161]
+MetricType = Literal["type1", "type2"]
 
 
 class Reference(BaseModel):
     ref: UUID
 
 
 class VariableName(BaseModel):
@@ -227,15 +179,18 @@
 class DSCPEntry(BaseModel):
     field: Literal["dscp"] = "dscp"
     value: str = Field(description="0-63 single numbers separate by space")
 
 
 class SourceIPEntry(BaseModel):
     field: Literal["sourceIp"] = "sourceIp"
-    value: str = Field(description="IP network specifiers separate by space")
+    value: Optional[str] = Field(default=None, description="IP network specifiers separate by space")
+    vipVariableName: Optional[str] = Field(
+        default=None, serialization_alias="vipVariableName", validation_alias="vipVariableName"
+    )
 
     @staticmethod
     def from_ipv4_networks(networks: List[IPv4Network]) -> "SourceIPEntry":
         return SourceIPEntry(value=networks_to_str(networks))
 
 
 class SourceIPv6Entry(BaseModel):
@@ -259,15 +214,18 @@
     @staticmethod
     def from_port_set_and_ranges(ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> "SourcePortEntry":
         return SourcePortEntry(value=port_set_and_ranges_to_str(ports, port_ranges))
 
 
 class DestinationIPEntry(BaseModel):
     field: Literal["destinationIp"] = "destinationIp"
-    value: str
+    value: Optional[str] = Field(default=None)
+    vipVariableName: Optional[str] = Field(
+        default=None, serialization_alias="vipVariableName", validation_alias="vipVariableName"
+    )
 
     @staticmethod
     def from_ipv4_networks(networks: List[IPv4Network]) -> "DestinationIPEntry":
         return DestinationIPEntry(value=networks_to_str(networks))
 
 
 class DestinationIPv6Entry(BaseModel):
@@ -314,14 +272,34 @@
 
 
 class DestinationRegionEntry(BaseModel):
     field: Literal["destinationRegion"] = "destinationRegion"
     value: DestinationRegion
 
 
+class AddressEntry(BaseModel):
+    field: Literal["address"] = "address"
+    ref: UUID
+
+
+class AsPathListMatchEntry(BaseModel):
+    field: Literal["asPath"] = "asPath"
+    ref: UUID
+
+
+class AsPathActionEntryValue(BaseModel):
+    prepend: SpaceSeparatedPositiveIntList
+    exclude: SpaceSeparatedPositiveIntList
+
+
+class AsPathActionEntry(BaseModel):
+    field: Literal["asPath"] = "asPath"
+    value: AsPathActionEntryValue
+
+
 class SourceFQDNEntry(BaseModel):
     field: Literal["sourceFqdn"] = "sourceFqdn"
     value: str = Field(max_length=120)
 
 
 class DestinationFQDNEntry(BaseModel):
     field: Literal["destinationFqdn"] = "destinationFqdn"
@@ -363,27 +341,32 @@
 
 
 class FallBackEntry(BaseModel):
     field: Literal["fallback"] = "fallback"
     value: str = ""
 
 
-class NextHopEntry(BaseModel):
+class NextHopActionEntry(BaseModel):
     field: Literal["nextHop"] = "nextHop"
-    value: IPv4Address
+    value: Union[IPv4Address, IPv6Address]
+
+
+class NextHopMatchEntry(BaseModel):
+    field: Literal["nextHop"] = "nextHop"
+    ref: UUID
 
 
 class NextHopLooseEntry(BaseModel):
     field: Literal["nextHopLoose"] = "nextHopLoose"
     value: str
 
 
 class OMPTagEntry(BaseModel):
     field: Literal["ompTag"] = "ompTag"
-    value: str = Field(description="Number in range 0-4294967295")
+    value: IntStr = Field(description="Number in range 0-4294967295", ge=0, le=4294967295)
 
 
 class OriginEntry(BaseModel):
     field: Literal["origin"] = "origin"
     value: OriginProtocol
 
 
@@ -395,15 +378,15 @@
 class PreferenceEntry(BaseModel):
     field: Literal["preference"] = "preference"
     value: str = Field(description="Number in range 0-4294967295")
 
 
 class PathTypeEntry(BaseModel):
     field: Literal["pathType"] = "pathType"
-    value: PathType
+    value: ControlPathType
 
 
 class RegionEntry(BaseModel):
     field: Literal["regionId"] = "regionId"
     value: str
 
 
@@ -439,26 +422,35 @@
 
 class TLOCEntry(BaseModel):
     field: Literal["tloc"] = "tloc"
     value: TLOCEntryValue
 
 
 class CommunityEntry(BaseModel):
+    model_config = ConfigDict(populate_by_name=True)
     field: Literal["community"] = "community"
-    value: str = Field(description="Example: 1000:10000 or internet or local-AS or no advertise or no-export")
+    value: Optional[str] = Field(
+        default=None, description="Example: 1000:10000 or internet or local-AS or no advertise or no-export"
+    )
+    vip_variable_name: Optional[str] = Field(
+        default=None,
+        serialization_alias="vipVariableName",
+        validation_alias="vipVariableName",
+        description="Example: 1000:10000 or internet or local-AS or no advertise or no-export",
+    )
 
 
 class CommunityAdditiveEntry(BaseModel):
     field: Literal["communityAdditive"] = "communityAdditive"
     value: Literal["true"] = "true"
 
 
 class CarrierEntry(BaseModel):
     field: Literal["carrier"] = "carrier"
-    value: Carrier
+    value: CarrierType
 
 
 class DomainIDEntry(BaseModel):
     field: Literal["domainId"] = "domainId"
     value: str = Field(description="Number in range 1-4294967295")
 
 
@@ -468,59 +460,144 @@
 
 
 class NextHeaderEntry(BaseModel):
     field: Literal["nextHeader"] = "nextHeader"
     value: str = Field(description="0-63 single numbers separate by space")
 
 
+class AggregatorActionEntryValue(BaseModel):
+    model_config = ConfigDict(populate_by_name=True)
+    aggregator: IntStr = Field(description="Number in range 1-4294967295", ge=0, le=4294967295)
+    ip_address: Union[IPv4Address, IPv6Address] = Field(serialization_alias="ipAddress", validation_alias="ipAddress")
+
+
+class AggregatorActionEntry(BaseModel):
+    field: Literal["aggregator"] = "aggregator"
+    value: AggregatorActionEntryValue
+
+
 class TrafficClassEntry(BaseModel):
     field: Literal["trafficClass"] = "trafficClass"
     value: str = Field(description="Number in range 0-63")
 
 
+class LocalPreferenceEntry(BaseModel):
+    field: Literal["localPreference"] = "localPreference"
+    value: IntStr = Field(ge=0, le=4294967295, description="Number in range 0-4294967295")
+
+
+class MetricEntry(BaseModel):
+    field: Literal["metric"] = "metric"
+    value: IntStr = Field(ge=0, le=4294967295, description="Number in range 0-4294967295")
+
+
+class MetricTypeEntry(BaseModel):
+    field: Literal["metricType"] = "metricType"
+    value: MetricType
+
+
+class OspfTagEntry(BaseModel):
+    field: Literal["ospfTag"] = "ospfTag"
+    value: IntStr = Field(ge=0, le=4294967295, description="Number in range 0-4294967295")
+
+
+class PeerEntry(BaseModel):
+    field: Literal["peer"] = "peer"
+    value: Union[IPv4Address, IPv6Address]
+
+
+class AtomicAggregateActionEntry(BaseModel):
+    field: Literal["atomicAggregate"] = "atomicAggregate"
+    value: Literal["true"] = "true"
+
+
+class WeightEntry(BaseModel):
+    field: Literal["weight"] = "weight"
+    value: IntStr = Field(ge=0, le=4294967295, description="Number in range 0-4294967295")
+
+
+class AdvancedCommunityEntry(BaseModel):
+    model_config = ConfigDict(populate_by_name=True)
+
+    field: Literal["advancedCommunity"] = "advancedCommunity"
+
+    match_flag: AdvancedCommunityMatchFlag = Field(
+        default="or",
+        serialization_alias="matchFlag",
+        validation_alias="matchFlag",
+        description="The 'and' and 'exact' conditions are applicable to only one community list",
+    )
+
+    refs: List[UUID] = []
+
+
+class ExpandedCommunityInLineEntry(BaseModel):
+    model_config = ConfigDict(populate_by_name=True)
+
+    field: Literal["expandedCommunityInline"] = "expandedCommunityInline"
+    vip_variable_name: str = Field(serialization_alias="vipVariableName", validation_alias="vipVariableName")
+
+
+class ExtendedCommunityEntry(BaseModel):
+    field: Literal["extCommunity"] = "extCommunity"
+    ref: UUID
+
+
 class NATVPNEntry(RootModel):
     root: List[Union[UseVPNEntry, FallBackEntry]]
 
     @staticmethod
     def from_nat_vpn(fallback: bool, vpn: int = 0) -> "NATVPNEntry":
         if fallback:
             return NATVPNEntry(root=[UseVPNEntry(value=str(vpn)), FallBackEntry()])
         return NATVPNEntry(root=[UseVPNEntry(value=str(vpn))])
 
 
+class ICMPMessageEntry(BaseModel):
+    field: Literal["icmpMessage"] = "icmpMessage"
+    value: List[ICMPMessageType]
+
+    _value = field_validator("value", mode="before")(str_as_str_list)
+
+
 class SourceDataPrefixListEntry(BaseModel):
     field: Literal["sourceDataPrefixList"] = "sourceDataPrefixList"
-    ref: UUID
+    ref: SpaceSeparatedUUIDList  # usually single id but zone based firewall can use multiple ids separated by space
 
 
 class SourceDataIPv6PrefixListEntry(BaseModel):
     field: Literal["sourceDataIpv6PrefixList"] = "sourceDataIpv6PrefixList"
-    ref: UUID
+    ref: SpaceSeparatedUUIDList  # usually single id but zone based firewall can use multiple ids separated by space
 
 
 class DestinationDataPrefixListEntry(BaseModel):
     field: Literal["destinationDataPrefixList"] = "destinationDataPrefixList"
-    ref: UUID
+    ref: SpaceSeparatedUUIDList  # usually single id but zone based firewall can use multiple ids separated by space
 
 
 class DestinationDataIPv6PrefixListEntry(BaseModel):
     field: Literal["destinationDataIpv6PrefixList"] = "destinationDataIpv6PrefixList"
-    ref: UUID
+    ref: SpaceSeparatedUUIDList  # usually single id but zone based firewall can use multiple ids separated by space
 
 
 class DNSAppListEntry(BaseModel):
     field: Literal["dnsAppList"] = "dnsAppList"
     ref: UUID
 
 
 class AppListEntry(BaseModel):
     field: Literal["appList"] = "appList"
     ref: UUID
 
 
+class AppListFlatEntry(BaseModel):
+    field: Literal["appListFlat"] = "appListFlat"
+    ref: UUID
+
+
 class SourceFQDNListEntry(BaseModel):
     field: Literal["sourceFqdnList"] = "sourceFqdnList"
     ref: UUID
 
 
 class DestinationFQDNListEntry(BaseModel):
     field: Literal["destinationFqdnList"] = "destinationFqdnList"
@@ -543,16 +620,26 @@
 
 
 class SourcePortListEntry(BaseModel):
     field: Literal["sourcePortList"] = "sourcePortList"
     ref: UUID
 
 
+class SourceScalableGroupTagListEntry(BaseModel):
+    field: Literal["sourceScalableGroupTagList"] = "sourceScalableGroupTagList"
+    ref: UUID
+
+
 class DestinationPortListEntry(BaseModel):
     field: Literal["destinationPortList"] = "destinationPortList"
+    ref: SpaceSeparatedUUIDList  # usually single id but zone based firewall can use multiple ids separated by space
+
+
+class DestinationScalableGroupTagListEntry(BaseModel):
+    field: Literal["destinationScalableGroupTagList"] = "destinationScalableGroupTagList"
     ref: UUID
 
 
 class RuleSetListEntry(BaseModel):
     field: Literal["ruleSetList"] = "ruleSetList"
     ref: str
 
@@ -567,14 +654,24 @@
 
 
 class TLOCListEntry(BaseModel):
     field: Literal["tlocList"] = "tlocList"
     ref: UUID
 
 
+class SourceVpnEntry(BaseModel):
+    field: Literal["sourceVpn"] = "sourceVpn"
+    value: str = Field(description="VPN ids numbers separated by space")
+
+
+class DestinationVpnEntry(BaseModel):
+    field: Literal["destinationVpn"] = "destinationVpn"
+    value: str = Field(description="VPN ids numbers separated by space")
+
+
 class PrefferedColorGroupListEntry(BaseModel):
     field: Literal["preferredColorGroup"] = "preferredColorGroup"
     ref: UUID
     color_restrict: bool = Field(False, serialization_alias="colorRestrict", validation_alias="colorRestrict")
     model_config = ConfigDict(populate_by_name=True)
 
 
@@ -748,50 +845,72 @@
 
 
 class PolicerAction(BaseModel):
     type: Literal["policer"] = "policer"
     parameter: Reference
 
 
+class ConnectionEventsAction(BaseModel):
+    type: Literal["connectionEvents"] = "connectionEvents"
+    parameter: str = ""
+
+
+class AdvancedInspectionProfileAction(BaseModel):
+    type: Literal["advancedInspectionProfile"] = "advancedInspectionProfile"
+    parameter: Reference
+
+
 ActionSetEntry = Annotated[
     Union[
         AffinityEntry,
         CommunityAdditiveEntry,
         CommunityEntry,
         DSCPEntry,
         ForwardingClassEntry,
         LocalTLOCListEntry,
-        NextHopEntry,
+        NextHopActionEntry,
         NextHopLooseEntry,
         OMPTagEntry,
         PolicerListEntry,
         PreferenceEntry,
         PrefferedColorGroupListEntry,
         ServiceChainEntry,
         ServiceEntry,
         TLOCActionEntry,
         TLOCEntry,
         TLOCListEntry,
         TrafficClassEntry,
         VPNEntry,
+        AggregatorActionEntry,
+        AsPathActionEntry,
+        AtomicAggregateActionEntry,
+        LocalPreferenceEntry,
+        MetricEntry,
+        MetricTypeEntry,
+        OriginEntry,
+        OriginatorEntry,
+        OspfTagEntry,
+        WeightEntry,
     ],
     Field(discriminator="field"),
 ]
 
 
 class ActionSet(BaseModel):
     type: Literal["set"] = "set"
     parameter: List[ActionSetEntry] = []
 
 
 ActionEntry = Annotated[
     Union[
         ActionSet,
+        AdvancedInspectionProfileAction,
         CFlowDAction,
         ClassMapAction,
+        ConnectionEventsAction,
         CountAction,
         DREOptimizationAction,
         FallBackToRoutingAction,
         LogAction,
         LossProtectionAction,
         LossProtectionFECAction,
         LossProtectionPacketDuplicationAction,
@@ -805,15 +924,22 @@
         ExportToAction,
     ],
     Field(discriminator="type"),
 ]
 
 MatchEntry = Annotated[
     Union[
+        AdvancedCommunityEntry,
+        ExpandedCommunityListEntry,
+        ExpandedCommunityInLineEntry,
+        AddressEntry,
         AppListEntry,
+        AppListFlatEntry,
+        AsPathListMatchEntry,
+        LocalPreferenceEntry,
         CarrierEntry,
         ClassMapListEntry,
         ColorListEntry,
         CommunityListEntry,
         DestinationDataIPv6PrefixListEntry,
         DestinationDataPrefixListEntry,
         DestinationFQDNEntry,
@@ -821,21 +947,25 @@
         DestinationGeoLocationEntry,
         DestinationGeoLocationListEntry,
         DestinationIPEntry,
         DestinationIPv6Entry,
         DestinationPortEntry,
         DestinationPortListEntry,
         DestinationRegionEntry,
+        DestinationScalableGroupTagListEntry,
+        DestinationVpnEntry,
         DNSAppListEntry,
         DNSEntry,
         DomainIDEntry,
         DSCPEntry,
         ExpandedCommunityListEntry,
         GroupIDEntry,
+        ICMPMessageEntry,
         NextHeaderEntry,
+        MetricEntry,
         OMPTagEntry,
         OriginatorEntry,
         OriginEntry,
         PacketLengthEntry,
         PathTypeEntry,
         PLPEntry,
         PreferenceEntry,
@@ -856,20 +986,26 @@
         SourceFQDNListEntry,
         SourceGeoLocationEntry,
         SourceGeoLocationListEntry,
         SourceIPEntry,
         SourceIPv6Entry,
         SourcePortEntry,
         SourcePortListEntry,
+        SourceScalableGroupTagListEntry,
+        SourceVpnEntry,
         TCPEntry,
         TLOCEntry,
         TLOCListEntry,
         TrafficClassEntry,
         TrafficToEntry,
         VPNListEntry,
+        NextHopMatchEntry,
+        OspfTagEntry,
+        PeerEntry,
+        ExtendedCommunityEntry,
     ],
     Field(discriminator="field"),
 ]
 
 MUTUALLY_EXCLUSIVE_FIELDS = [
     {"destinationDataPrefixList", "destinationIp"},
     {"destinationDataIpv6PrefixList", "destinationIpv6"},
@@ -900,25 +1036,28 @@
     entries: Sequence[MatchEntry]
 
 
 class Action(BaseModel):
     pass
 
 
+PolicyAcceptRejectActionType = Literal["accept", "reject"]
+
+
 class PolicyDefinitionSequenceBase(BaseModel):
     sequence_id: int = Field(default=0, serialization_alias="sequenceId", validation_alias="sequenceId")
     sequence_name: str = Field(serialization_alias="sequenceName", validation_alias="sequenceName")
-    base_action: PolicyActionType = Field(
-        default="drop", serialization_alias="baseAction", validation_alias="baseAction"
-    )
+    base_action: str = Field(serialization_alias="baseAction", validation_alias="baseAction")
     sequence_type: SequenceType = Field(serialization_alias="sequenceType", validation_alias="sequenceType")
-    sequence_ip_type: SequenceIpType = Field(serialization_alias="sequenceIpType", validation_alias="sequenceIpType")
+    sequence_ip_type: Optional[SequenceIpType] = Field(
+        default="ipv4", serialization_alias="sequenceIpType", validation_alias="sequenceIpType"
+    )
     ruleset: Optional[bool] = None
     match: Match
-    actions: Sequence[ActionEntry]
+    actions: Optional[Sequence[ActionEntry]] = None
 
     @staticmethod
     def _check_field_collision(field: str, fields: Sequence[str]) -> None:
         existing_fields = set(fields)
         forbidden_fields = set(MUTUALLY_EXCLUSIVE_FIELD_LOOKUP.get(field, []))
         colliding_fields = set(existing_fields) & set(forbidden_fields)
         assert not colliding_fields, f"{field} is mutually exclusive with {colliding_fields}"
@@ -1002,16 +1141,24 @@
     def wrapper(self: PolicyDefinitionSequenceBase, *args, **kwargs):
         assert self.base_action == "accept", f"{method.__name__} only allowed when base_action is accept"
         return method(self, *args, **kwargs)
 
     return wrapper
 
 
-class DefaultAction(BaseModel):
-    type: PolicyActionType
+class PolicyActionBase(BaseModel):
+    type: str
+
+
+class PolicyAcceptRejectAction(PolicyActionBase):
+    type: PolicyAcceptRejectActionType
+
+
+class BasicPolicyAction(PolicyActionBase):
+    type: BasicPolicyActionType
 
 
 class InfoTag(BaseModel):
     info_tag: Optional[str] = Field("", serialization_alias="infoTag", validation_alias="infoTag")
 
 
 class PolicyDefinitionId(BaseModel):
@@ -1020,16 +1167,16 @@
 
 class PolicyReference(BaseModel):
     id: UUID
     property: str
 
 
 class DefinitionWithSequencesCommonBase(BaseModel):
-    default_action: Optional[DefaultAction] = Field(
-        default=DefaultAction(type="drop"),
+    default_action: Optional[PolicyActionBase] = Field(
+        default=None,
         serialization_alias="defaultAction",
         validation_alias="defaultAction",
     )
     sequences: Optional[Sequence[PolicyDefinitionSequenceBase]] = None
 
     def _enumerate_sequences(self, from_index: int = 0) -> None:
         """Updates sequence entries with appropriate index.
@@ -1105,24 +1252,7 @@
     master_templates_affected: List[str] = Field(
         default=[], serialization_alias="masterTemplatesAffected", validation_alias="masterTemplatesAffected"
     )
 
 
 class PolicyDefinitionPreview(BaseModel):
     preview: str
-
-
-class PolicyDefinitionEndpoints(Protocol):
-    def create_policy_definition(self, payload: BaseModel) -> PolicyDefinitionId:
-        ...
-
-    def delete_policy_definition(self, id: UUID) -> None:
-        ...
-
-    def edit_policy_definition(self, id: UUID, payload: BaseModel) -> PolicyDefinitionEditResponse:
-        ...
-
-    def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
-        ...
-
-    def get_policy_definition(self, id: UUID) -> PolicyDefinitionGetResponse:
-        ...
```

### Comparing `catalystwan-0.33.7/catalystwan/models/policy/policy_list.py` & `catalystwan-0.33.7.dev0/catalystwan/models/policy/list/vpn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,40 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2022 Cisco Systems, Inc. and its affiliates
 
-import datetime
-from typing import List, Optional, Protocol
-from uuid import UUID
+from typing import List, Literal, Set, Tuple
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, field_validator
 
-from catalystwan.models.policy import AnyPolicyList
-from catalystwan.typed_list import DataSequence
+from catalystwan.models.common import IntRangeStr
+from catalystwan.models.policy.policy_list import PolicyListBase, PolicyListId, PolicyListInfo
 
 
-class InfoTag(BaseModel):
-    info_tag: Optional[str] = Field("", alias="infoTag")
+class VPNListEntry(BaseModel):
+    vpn: IntRangeStr = Field(description="0-65530 range or single number")
 
+    @field_validator("vpn")
+    @classmethod
+    def check_vpn_range(cls, vpn: IntRangeStr):
+        for i in vpn:
+            if i is not None:
+                assert 0 <= i <= 65_530
+        return vpn
 
-class PolicyListId(BaseModel):
-    list_id: UUID = Field(alias="listId")
 
+class VPNList(PolicyListBase):
+    type: Literal["vpn"] = "vpn"
+    entries: List[VPNListEntry] = []
 
-class PolicyListInfo(PolicyListId, InfoTag):
-    last_updated: datetime.datetime = Field(alias="lastUpdated")
-    owner: str
-    read_only: bool = Field(alias="readOnly")
-    version: str
-    reference_count: int = Field(alias="referenceCount")
-    references: List
-    is_activated_by_vsmart: Optional[bool] = Field(None, alias="isActivatedByVsmart")
+    def add_vpns(self, vpns: Set[int]):
+        for vpn in vpns:
+            self._add_entry(VPNListEntry(vpn=(vpn, None)))
 
+    def add_vpn_range(self, vpn_range: Tuple[int, int]):
+        self._add_entry(VPNListEntry(vpn=vpn_range))
 
-class PolicyListPreview(BaseModel):
-    preview: str
 
+class VPNListEditPayload(VPNList, PolicyListId):
+    pass
 
-class PolicyListEndpoints(Protocol):
-    def create_policy_list(self, payload: AnyPolicyList) -> PolicyListId:
-        ...
 
-    def delete_policy_list(self, id: UUID) -> None:
-        ...
-
-    def edit_policy_list(self, id: UUID, payload: AnyPolicyList) -> None:
-        ...
-
-    def get_lists_by_id(self, id: UUID) -> PolicyListInfo:
-        ...
-
-    def get_policy_lists(self) -> DataSequence[PolicyListInfo]:
-        ...
+class VPNListInfo(VPNList, PolicyListInfo):
+    pass
```

### Comparing `catalystwan-0.33.7/catalystwan/models/tenant.py` & `catalystwan-0.33.7.dev0/catalystwan/models/tenant.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/response.py` & `catalystwan-0.33.7.dev0/catalystwan/response.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/session.py` & `catalystwan-0.33.7.dev0/catalystwan/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         url: str,
         username: str,
         password: str,
         verify: bool = False,
         port: Optional[int] = None,
         subdomain: Optional[str] = None,
         auth: Optional[AuthBase] = None,
-        validate_responses: bool = True,
+        validate_response: bool = True,
     ):
         self.url = url
         self.port = port
         self.base_url = self.__create_base_url()
         self.username = username
         self.password = password
         self.subdomain = subdomain
@@ -171,19 +171,19 @@
         self.response_trace: Callable[
             [Optional[Response], Union[Request, PreparedRequest, None]], str
         ] = response_history_debug
         super(ManagerSession, self).__init__()
         self.headers.update({"User-Agent": USER_AGENT})
         self.__prepare_session(verify, auth)
         self._platform_version: str = ""
-        self._api_version: Version
+        self._api_version: Version = NullVersion  # type: ignore
         self._state: ManagerSessionState = ManagerSessionState.OPERATIVE
         self.restart_timeout: int = 1200
         self.polling_requests_timeout: int = 10
-        self._validate_responses = validate_responses
+        self._validate_response = validate_response
 
     @cached_property
     def api(self) -> APIContainer:
         from catalystwan.api.api_container import APIContainer
 
         self._api = APIContainer(self)
         return self._api
@@ -440,43 +440,32 @@
             Virtual session token
         """
         url_path = f"/dataservice/tenant/{tenant_id}/vsessionid"
         response = self.post(url_path)
         return response.json()["VSessionId"]
 
     def logout(self) -> Optional[ManagerResponse]:
-        response = None
         if isinstance((version := self.api_version), NullVersion):
             self.logger.warning("Cannot perform logout operation without known api_version.")
-            return response
+            return None
         else:
-            # disable automatic relogin before performing logout request
-            _relogin = self.enable_relogin
-            try:
-                self.enable_relogin = False
-                if version >= Version("20.12"):
-                    response = self.post("/logout")
-                else:
-                    response = self.get("/logout")
-            finally:
-                # restore original setting after performing logout request
-                self.enable_relogin = _relogin
-        return response
+            return self.post("/logout") if version >= Version("20.12") else self.get("/logout")
 
     def close(self) -> None:
         """Closes the ManagerSession.
 
         This method is overrided from requests.Session.
         Firstly it cleans up any resources associated with vManage.
         Then it closes all adapters and as such the session.
 
         Note: It is generally recommended to use the session as a context manager
         using the `with` statement, which ensures that the session is properly
         closed and resources are cleaned up even in case of exceptions.
         """
+        self.enable_relogin = False
         self.logout()
         super().close()
 
     def __prepare_session(self, verify: bool, auth: Optional[AuthBase]) -> None:
         self.auth = auth
         self.verify = verify
 
@@ -494,20 +483,20 @@
         self._api_version = parse_api_version(version)
 
     @property
     def api_version(self) -> Version:
         return self._api_version
 
     @property
-    def validate_responses(self) -> bool:
-        return self._validate_responses
+    def validate_response(self) -> bool:
+        return self._validate_response
 
-    @validate_responses.setter
-    def validate_responses(self, value: bool):
-        self._validate_responses = value
+    @validate_response.setter
+    def validate_response(self, value: bool):
+        self._validate_response = value
 
     def __str__(self) -> str:
         return f"{self.username}@{self.base_url}"
 
     def __repr__(self):
         return (
             f"{self.__class__.__name__}('{self.url}', '{self.username}', '{self.password}', port={self.port}, "
```

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/definitions/banner_1.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/banner_1.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/children.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/children_nested.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/definitions/cisco_bfd.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/definitions/complex_aaa.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/complex_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/definitions/complex_cisco_vpn.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/complex_cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/definitions/default_cisco_system.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/default_cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/definitions/iuo.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/iuo.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/definitions/omp_2.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/omp_2.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/definitions/omp_3.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/definitions/omp_3.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/models/__init__.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/models/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_aaa.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/models/cisco_aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_bfd.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/models/cisco_bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_vpn.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/models/cisco_vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/models/omp_vsmart.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/models/omp_vsmart.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/alias.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/basic/alias.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/basic.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/basic/basic.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/children.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/children_nested.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/data_path.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/basic/data_path.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/schemas/cedge_aaa.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/cedge_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_banner.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/cisco_banner.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_bfd.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_system.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_vpn.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/schemas/omp-vsmart.json` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/schemas/omp-vsmart.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/test_chose_model.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/test_chose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/test_deserialize_model.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/test_deserialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/test_find_template_values.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/test_find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/test_generate_payload.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/test_generate_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/templates/test_serialize_model.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/templates/test_serialize_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         with open(Path(__file__).resolve().parents[0] / Path("schemas") / Path(template.type + ".json")) as f:
             schema = json.load(f)
 
         with open(
             Path(__file__).resolve().parents[0] / Path("definitions") / Path(f"{template.template_name}.json")
         ) as f:
             definition = json.load(f)
-
         # Act
         feature_template_payload = templates_api.generate_feature_template_payload(
             template=template, schema=schema, debug=False
         )
         # Assert
         # self.assertDictEqual
         self.maxDiff = 10000
```

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_admin_tech_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_administration.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_alarms_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_cli_template.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_creation_tools.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_device_action_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_devices_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_endpoints.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Dict, List, Literal, Optional, Union
 from unittest.mock import MagicMock
 from uuid import UUID, uuid4
 
 import pytest  # type: ignore
 from packaging.version import Version  # type: ignore
 from parameterized import parameterized  # type: ignore
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field, model_serializer
 from typing_extensions import Annotated
 
 from catalystwan.endpoints import (
     BASE_PATH,
     JSON,
     APIEndpoints,
     CustomPayloadType,
@@ -25,14 +25,15 @@
     TypeSpecifier,
     delete,
     get,
 )
 from catalystwan.endpoints import logger as endpoints_logger
 from catalystwan.endpoints import post, put, request, versions, view
 from catalystwan.exceptions import APIEndpointError, APIRequestPayloadTypeError, APIVersionError, APIViewError
+from catalystwan.models.common import VersionedField
 from catalystwan.typed_list import DataSequence
 from catalystwan.utils.session_type import ProviderAsTenantView, ProviderView, TenantView
 
 
 class BaseModelExample(BaseModel):
     id: str
     size: int
@@ -870,7 +871,40 @@
 
         AnyBaseModel = Annotated[Union[BaseModel_A, BaseModel_B], Field(discriminator="field")]
 
         class TestAPI(APIEndpoints):
             @request("POST", "/v1/data")
             def create(self, payload: AnyBaseModel) -> None:  # type: ignore [empty-body]
                 ...
+
+    @parameterized.expand(
+        [
+            ("1.3", '{"name":"John"}'),
+            ("1.9", '{"newName":"John"}'),
+        ]
+    )
+    def test_api_version_passed_in_dump_context(self, version, expected_payload_json):
+        # Arrange
+        class Payload(BaseModel):
+            model_config = ConfigDict(populate_by_name=True)
+            name: Annotated[str, VersionedField(versions=">1.6", serialization_alias="newName")]
+
+            @model_serializer(mode="wrap")
+            def serialize(self, handler, info):
+                return VersionedField.dump(self.model_fields, handler(self), info)
+
+        class ExampleAPI(APIEndpoints):
+            @request("POST", "/v1/data")
+            def create(self, payload: Payload) -> None:  # type: ignore [empty-body]
+                ...
+
+        self.session_mock.api_version = Version(version)
+        api = ExampleAPI(self.session_mock)
+        # Act
+        api.create(Payload(name="John"))
+        # Assert
+        self.session_mock.request.assert_called_once_with(
+            "POST",
+            self.base_path + "/v1/data",
+            data=expected_payload_json,
+            headers={"content-type": "application/json"},
+        )
```

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_feature_template_field.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_logs_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_monitoring_server_info.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_monitoring_server_info.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_monitoring_status_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_mtt_aaa_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_omp_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_packet_capture.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_packet_capture.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_partition_manager_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_response.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,25 +152,27 @@
         # Arrange
         self.response_mock.json.return_value = VALIDATE_DATASEQ_TEST_DATA[0]
         vmng_response = ManagerResponse(self.response_mock)
         # Act
         data = vmng_response.dataobj(DataForValidateTest, sourcekey=None, validate=False)
         # Assert
         assert isinstance(data, DataForValidateTest)
+        print(data)
         assert data.important == VALIDATE_DATASEQ_TEST_DATA[0]["important"]
         with self.assertRaises(ValidationError):
             vmng_response.dataobj(DataForValidateTest, sourcekey=None, validate=True)
 
     def test_dataseq_optional_validate(self):
         self.response_mock.json.return_value = VALIDATE_DATASEQ_TEST_DATA
         vmng_response = ManagerResponse(self.response_mock)
         # Act
         dataseq = vmng_response.dataseq(DataForValidateTest, sourcekey=None, validate=False)
         # Assert
         assert isinstance(dataseq, DataSequence)
+        print(dataseq)
         for i, data in enumerate(dataseq):
             assert isinstance(data, DataForValidateTest)
             assert data.important == VALIDATE_DATASEQ_TEST_DATA[i]["important"]
         with self.assertRaises(ValidationError):
             vmng_response.dataseq(DataForValidateTest, sourcekey=None, validate=True)
 
     def test_dataseq_with_misisng_data(self):
```

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_session.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_software_action_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_speed_test_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_speed_test_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_task_status_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_templates.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             reachability=Reachability.REACHABLE,
             local_system_ip="192.168.0.1",
             memUsage=1.0,
             connected_vManages=["192.168.0.1"],
             model="vedge-cloud",
             status="normal",
         )
-        sub_tasks_data = SubTaskData.parse_obj(
+        sub_tasks_data = SubTaskData.model_validate(
             {
                 "status": "Success",
                 "statusId": "success",
                 "action": "",
                 "activity": [],
                 "currentActivity": "",
                 "actionConfig": "",
```

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_tenant_backup_restore_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_tenant_management_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_tenant_migration_api.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_typed_list.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_version.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_version_utils.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/tests/test_vmanage_auth.py` & `catalystwan-0.33.7.dev0/catalystwan/tests/test_vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/typed_list.py` & `catalystwan-0.33.7.dev0/catalystwan/typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/utils/creation_tools.py` & `catalystwan-0.33.7.dev0/catalystwan/utils/creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/utils/dashboard.py` & `catalystwan-0.33.7.dev0/catalystwan/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/utils/device_model.py` & `catalystwan-0.33.7.dev0/catalystwan/utils/device_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/utils/dict.py` & `catalystwan-0.33.7.dev0/catalystwan/utils/dict.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/utils/feature_template/choose_model.py` & `catalystwan-0.33.7.dev0/catalystwan/utils/feature_template/choose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/utils/feature_template/find_template_values.py` & `catalystwan-0.33.7.dev0/catalystwan/utils/feature_template/find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/utils/operation_status.py` & `catalystwan-0.33.7.dev0/catalystwan/utils/operation_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/utils/upgrades_helper.py` & `catalystwan-0.33.7.dev0/catalystwan/utils/upgrades_helper.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/version.py` & `catalystwan-0.33.7.dev0/catalystwan/version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/vmanage_auth.py` & `catalystwan-0.33.7.dev0/catalystwan/vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/catalystwan/workflows/tenant_migration.py` & `catalystwan-0.33.7.dev0/catalystwan/workflows/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7/pyproject.toml` & `catalystwan-0.33.7.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "catalystwan"
-version = "0.33.7"
+version = "0.33.7dev0"
 description = "Cisco Catalyst WAN SDK for Python"
 authors = ["kagorski <kagorski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/cisco-open/cisco-catalyst-wan-sdk"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
@@ -14,15 +14,15 @@
 ciscoconfparse = "1.9.41"
 tenacity = "^8.1.0"
 Jinja2 = "^3.1.2"
 flake8-quotes = "^3.3.1"
 clint = "^0.5.1"
 requests-toolbelt = "^1.0.0"
 packaging = "^23.0"
-pydantic = "^2.5"
+pydantic = "^2.7"
 typing-extensions = "^4.6.1"
 
 [tool.poetry.dev-dependencies]
 parameterized = "^0.8.1"
 pytest = "^7.1.2"
 pytest-mock = "^3.7.0"
 pytest-subtests = "^0.11.0"
```

### Comparing `catalystwan-0.33.7/setup.py` & `catalystwan-0.33.7.dev0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,1080 +1,1170 @@
 00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
 00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
 00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
 00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
 00000040: 205c 0a5b 2763 6174 616c 7973 7477 616e   \.['catalystwan
 00000050: 272c 0a20 2763 6174 616c 7973 7477 616e  ',. 'catalystwan
 00000060: 2e61 7069 272c 0a20 2763 6174 616c 7973  .api',. 'catalys
-00000070: 7477 616e 2e61 7069 2e63 6f6e 6669 6775  twan.api.configu
-00000080: 7261 7469 6f6e 5f67 726f 7570 7327 2c0a  ration_groups',.
-00000090: 2027 6361 7461 6c79 7374 7761 6e2e 6170   'catalystwan.ap
-000000a0: 692e 636f 6e66 6967 7572 6174 696f 6e5f  i.configuration_
-000000b0: 6772 6f75 7073 2e70 6172 6365 6c73 272c  groups.parcels',
-000000c0: 0a20 2763 6174 616c 7973 7477 616e 2e61  . 'catalystwan.a
-000000d0: 7069 2e74 656d 706c 6174 6573 272c 0a20  pi.templates',. 
-000000e0: 2763 6174 616c 7973 7477 616e 2e61 7069  'catalystwan.api
-000000f0: 2e74 656d 706c 6174 6573 2e64 6576 6963  .templates.devic
-00000100: 655f 7465 6d70 6c61 7465 272c 0a20 2763  e_template',. 'c
-00000110: 6174 616c 7973 7477 616e 2e61 7069 2e74  atalystwan.api.t
-00000120: 656d 706c 6174 6573 2e6d 6f64 656c 7327  emplates.models'
-00000130: 2c0a 2027 6361 7461 6c79 7374 7761 6e2e  ,. 'catalystwan.
-00000140: 6170 692e 7465 6d70 6c61 7465 732e 7061  api.templates.pa
-00000150: 796c 6f61 6473 2e61 6161 272c 0a20 2763  yloads.aaa',. 'c
-00000160: 6174 616c 7973 7477 616e 2e61 7069 2e74  atalystwan.api.t
-00000170: 656d 706c 6174 6573 2e70 6179 6c6f 6164  emplates.payload
-00000180: 732e 6369 7363 6f5f 7670 6e27 2c0a 2027  s.cisco_vpn',. '
-00000190: 6361 7461 6c79 7374 7761 6e2e 6170 692e  catalystwan.api.
-000001a0: 7465 6d70 6c61 7465 732e 7061 796c 6f61  templates.payloa
-000001b0: 6473 2e74 656e 616e 7427 2c0a 2027 6361  ds.tenant',. 'ca
-000001c0: 7461 6c79 7374 7761 6e2e 656e 6470 6f69  talystwan.endpoi
-000001d0: 6e74 7327 2c0a 2027 6361 7461 6c79 7374  nts',. 'catalyst
-000001e0: 7761 6e2e 656e 6470 6f69 6e74 732e 636f  wan.endpoints.co
-000001f0: 6e66 6967 7572 6174 696f 6e27 2c0a 2027  nfiguration',. '
-00000200: 6361 7461 6c79 7374 7761 6e2e 656e 6470  catalystwan.endp
-00000210: 6f69 6e74 732e 636f 6e66 6967 7572 6174  oints.configurat
-00000220: 696f 6e2e 6465 7669 6365 272c 0a20 2763  ion.device',. 'c
-00000230: 6174 616c 7973 7477 616e 2e65 6e64 706f  atalystwan.endpo
-00000240: 696e 7473 2e63 6f6e 6669 6775 7261 7469  ints.configurati
-00000250: 6f6e 2e66 6561 7475 7265 5f70 726f 6669  on.feature_profi
-00000260: 6c65 2e73 6477 616e 272c 0a20 2763 6174  le.sdwan',. 'cat
-00000270: 616c 7973 7477 616e 2e65 6e64 706f 696e  alystwan.endpoin
-00000280: 7473 2e63 6f6e 6669 6775 7261 7469 6f6e  ts.configuration
-00000290: 2e70 6f6c 6963 7927 2c0a 2027 6361 7461  .policy',. 'cata
-000002a0: 6c79 7374 7761 6e2e 656e 6470 6f69 6e74  lystwan.endpoint
-000002b0: 732e 636f 6e66 6967 7572 6174 696f 6e2e  s.configuration.
-000002c0: 706f 6c69 6379 2e64 6566 696e 6974 696f  policy.definitio
-000002d0: 6e27 2c0a 2027 6361 7461 6c79 7374 7761  n',. 'catalystwa
-000002e0: 6e2e 656e 6470 6f69 6e74 732e 636f 6e66  n.endpoints.conf
-000002f0: 6967 7572 6174 696f 6e2e 706f 6c69 6379  iguration.policy
-00000300: 2e6c 6973 7427 2c0a 2027 6361 7461 6c79  .list',. 'cataly
-00000310: 7374 7761 6e2e 656e 6470 6f69 6e74 732e  stwan.endpoints.
-00000320: 6d6f 6e69 746f 7269 6e67 272c 0a20 2763  monitoring',. 'c
-00000330: 6174 616c 7973 7477 616e 2e65 6e64 706f  atalystwan.endpo
-00000340: 696e 7473 2e72 6561 6c5f 7469 6d65 5f6d  ints.real_time_m
-00000350: 6f6e 6974 6f72 696e 6727 2c0a 2027 6361  onitoring',. 'ca
-00000360: 7461 6c79 7374 7761 6e2e 656e 6470 6f69  talystwan.endpoi
-00000370: 6e74 732e 7472 6f75 626c 6573 686f 6f74  nts.troubleshoot
-00000380: 696e 675f 746f 6f6c 7327 2c0a 2027 6361  ing_tools',. 'ca
-00000390: 7461 6c79 7374 7761 6e2e 696e 7465 6772  talystwan.integr
-000003a0: 6174 696f 6e5f 7465 7374 7327 2c0a 2027  ation_tests',. '
-000003b0: 6361 7461 6c79 7374 7761 6e2e 6d6f 6465  catalystwan.mode
-000003c0: 6c73 272c 0a20 2763 6174 616c 7973 7477  ls',. 'catalystw
-000003d0: 616e 2e6d 6f64 656c 732e 636f 6e66 6967  an.models.config
-000003e0: 7572 6174 696f 6e27 2c0a 2027 6361 7461  uration',. 'cata
-000003f0: 6c79 7374 7761 6e2e 6d6f 6465 6c73 2e63  lystwan.models.c
-00000400: 6f6e 6669 6775 7261 7469 6f6e 2e66 6561  onfiguration.fea
-00000410: 7475 7265 5f70 726f 6669 6c65 272c 0a20  ture_profile',. 
-00000420: 2763 6174 616c 7973 7477 616e 2e6d 6f64  'catalystwan.mod
-00000430: 656c 732e 636f 6e66 6967 7572 6174 696f  els.configuratio
-00000440: 6e2e 6665 6174 7572 655f 7072 6f66 696c  n.feature_profil
-00000450: 652e 7364 7761 6e2e 6d61 6e61 6765 6d65  e.sdwan.manageme
-00000460: 6e74 272c 0a20 2763 6174 616c 7973 7477  nt',. 'catalystw
-00000470: 616e 2e6d 6f64 656c 732e 636f 6e66 6967  an.models.config
-00000480: 7572 6174 696f 6e2e 6665 6174 7572 655f  uration.feature_
-00000490: 7072 6f66 696c 652e 7364 7761 6e2e 706f  profile.sdwan.po
-000004a0: 6c69 6379 5f6f 626a 6563 7427 2c0a 2027  licy_object',. '
-000004b0: 6361 7461 6c79 7374 7761 6e2e 6d6f 6465  catalystwan.mode
-000004c0: 6c73 2e63 6f6e 6669 6775 7261 7469 6f6e  ls.configuration
-000004d0: 2e66 6561 7475 7265 5f70 726f 6669 6c65  .feature_profile
-000004e0: 2e73 6477 616e 2e70 6f6c 6963 795f 6f62  .sdwan.policy_ob
-000004f0: 6a65 6374 2e70 6f6c 6963 7927 2c0a 2027  ject.policy',. '
-00000500: 6361 7461 6c79 7374 7761 6e2e 6d6f 6465  catalystwan.mode
-00000510: 6c73 2e63 6f6e 6669 6775 7261 7469 6f6e  ls.configuration
-00000520: 2e66 6561 7475 7265 5f70 726f 6669 6c65  .feature_profile
-00000530: 2e73 6477 616e 2e70 6f6c 6963 795f 6f62  .sdwan.policy_ob
-00000540: 6a65 6374 2e73 6563 7572 6974 7927 2c0a  ject.security',.
-00000550: 2027 6361 7461 6c79 7374 7761 6e2e 6d6f   'catalystwan.mo
-00000560: 6465 6c73 2e63 6f6e 6669 6775 7261 7469  dels.configurati
-00000570: 6f6e 2e66 6561 7475 7265 5f70 726f 6669  on.feature_profi
-00000580: 6c65 2e73 6477 616e 2e73 6572 7669 6365  le.sdwan.service
-00000590: 272c 0a20 2763 6174 616c 7973 7477 616e  ',. 'catalystwan
-000005a0: 2e6d 6f64 656c 732e 636f 6e66 6967 7572  .models.configur
-000005b0: 6174 696f 6e2e 6665 6174 7572 655f 7072  ation.feature_pr
-000005c0: 6f66 696c 652e 7364 7761 6e2e 7365 7276  ofile.sdwan.serv
-000005d0: 6963 652e 6c61 6e27 2c0a 2027 6361 7461  ice.lan',. 'cata
-000005e0: 6c79 7374 7761 6e2e 6d6f 6465 6c73 2e63  lystwan.models.c
-000005f0: 6f6e 6669 6775 7261 7469 6f6e 2e66 6561  onfiguration.fea
-00000600: 7475 7265 5f70 726f 6669 6c65 2e73 6477  ture_profile.sdw
-00000610: 616e 2e73 7973 7465 6d27 2c0a 2027 6361  an.system',. 'ca
-00000620: 7461 6c79 7374 7761 6e2e 6d6f 6465 6c73  talystwan.models
-00000630: 2e63 6f6e 6669 6775 7261 7469 6f6e 2e66  .configuration.f
-00000640: 6561 7475 7265 5f70 726f 6669 6c65 2e73  eature_profile.s
-00000650: 6477 616e 2e74 7261 6e73 706f 7274 272c  dwan.transport',
-00000660: 0a20 2763 6174 616c 7973 7477 616e 2e6d  . 'catalystwan.m
-00000670: 6f64 656c 732e 6d69 7363 272c 0a20 2763  odels.misc',. 'c
-00000680: 6174 616c 7973 7477 616e 2e6d 6f64 656c  atalystwan.model
-00000690: 732e 6d6f 6e69 746f 7269 6e67 272c 0a20  s.monitoring',. 
-000006a0: 2763 6174 616c 7973 7477 616e 2e6d 6f64  'catalystwan.mod
-000006b0: 656c 732e 706f 6c69 6379 272c 0a20 2763  els.policy',. 'c
-000006c0: 6174 616c 7973 7477 616e 2e6d 6f64 656c  atalystwan.model
-000006d0: 732e 706f 6c69 6379 2e64 6566 696e 6974  s.policy.definit
-000006e0: 696f 6e73 272c 0a20 2763 6174 616c 7973  ions',. 'catalys
-000006f0: 7477 616e 2e74 6573 7473 272c 0a20 2763  twan.tests',. 'c
-00000700: 6174 616c 7973 7477 616e 2e74 6573 7473  atalystwan.tests
-00000710: 2e74 656d 706c 6174 6573 272c 0a20 2763  .templates',. 'c
-00000720: 6174 616c 7973 7477 616e 2e74 6573 7473  atalystwan.tests
-00000730: 2e74 656d 706c 6174 6573 2e6d 6f64 656c  .templates.model
-00000740: 7327 2c0a 2027 6361 7461 6c79 7374 7761  s',. 'catalystwa
-00000750: 6e2e 7574 696c 7327 2c0a 2027 6361 7461  n.utils',. 'cata
-00000760: 6c79 7374 7761 6e2e 7574 696c 732e 6665  lystwan.utils.fe
-00000770: 6174 7572 655f 7465 6d70 6c61 7465 272c  ature_template',
-00000780: 0a20 2763 6174 616c 7973 7477 616e 2e77  . 'catalystwan.w
-00000790: 6f72 6b66 6c6f 7773 275d 0a0a 7061 636b  orkflows']..pack
-000007a0: 6167 655f 6461 7461 203d 205c 0a7b 2727  age_data = \.{''
-000007b0: 3a20 5b27 2a27 5d2c 0a20 2763 6174 616c  : ['*'],. 'catal
-000007c0: 7973 7477 616e 2e61 7069 2e74 656d 706c  ystwan.api.templ
-000007d0: 6174 6573 2e70 6179 6c6f 6164 732e 6161  ates.payloads.aa
-000007e0: 6127 3a20 5b27 6665 6174 7572 652f 2a27  a': ['feature/*'
-000007f0: 5d2c 0a20 2763 6174 616c 7973 7477 616e  ],. 'catalystwan
-00000800: 2e61 7069 2e74 656d 706c 6174 6573 2e70  .api.templates.p
-00000810: 6179 6c6f 6164 732e 6369 7363 6f5f 7670  ayloads.cisco_vp
-00000820: 6e27 3a20 5b27 6665 6174 7572 652f 2a27  n': ['feature/*'
-00000830: 5d2c 0a20 2763 6174 616c 7973 7477 616e  ],. 'catalystwan
-00000840: 2e74 6573 7473 2e74 656d 706c 6174 6573  .tests.templates
-00000850: 273a 205b 2764 6566 696e 6974 696f 6e73  ': ['definitions
-00000860: 2f2a 272c 0a20 2020 2020 2020 2020 2020  /*',.           
-00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000880: 2020 2020 2020 2764 6566 696e 6974 696f        'definitio
-00000890: 6e73 2f62 6173 6963 2f2a 272c 0a20 2020  ns/basic/*',.   
-000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-000008c0: 6368 656d 6173 2f2a 272c 0a20 2020 2020  chemas/*',.     
-000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008e0: 2020 2020 2020 2020 2020 2020 2773 6368              'sch
-000008f0: 656d 6173 2f62 6173 6963 2f2a 275d 7d0a  emas/basic/*']}.
-00000900: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-00000910: 7320 3d20 5c0a 5b27 4a69 6e6a 6132 3e3d  s = \.['Jinja2>=
-00000920: 332e 312e 322c 3c34 2e30 2e30 272c 0a20  3.1.2,<4.0.0',. 
-00000930: 2761 7474 7273 3e3d 3231 2e34 2e30 2c3c  'attrs>=21.4.0,<
-00000940: 3232 2e30 2e30 272c 0a20 2763 6973 636f  22.0.0',. 'cisco
-00000950: 636f 6e66 7061 7273 653d 3d31 2e39 2e34  confparse==1.9.4
-00000960: 3127 2c0a 2027 636c 696e 743e 3d30 2e35  1',. 'clint>=0.5
-00000970: 2e31 2c3c 302e 362e 3027 2c0a 2027 666c  .1,<0.6.0',. 'fl
-00000980: 616b 6538 2d71 756f 7465 733e 3d33 2e33  ake8-quotes>=3.3
-00000990: 2e31 2c3c 342e 302e 3027 2c0a 2027 7061  .1,<4.0.0',. 'pa
-000009a0: 636b 6167 696e 673e 3d32 332e 302c 3c32  ckaging>=23.0,<2
-000009b0: 342e 3027 2c0a 2027 7079 6461 6e74 6963  4.0',. 'pydantic
-000009c0: 3e3d 322e 352c 3c33 2e30 272c 0a20 2770  >=2.5,<3.0',. 'p
-000009d0: 7974 686f 6e2d 6461 7465 7574 696c 3e3d  ython-dateutil>=
-000009e0: 322e 382e 322c 3c33 2e30 2e30 272c 0a20  2.8.2,<3.0.0',. 
-000009f0: 2772 6571 7565 7374 732d 746f 6f6c 6265  'requests-toolbe
-00000a00: 6c74 3e3d 312e 302e 302c 3c32 2e30 2e30  lt>=1.0.0,<2.0.0
-00000a10: 272c 0a20 2772 6571 7565 7374 733e 3d32  ',. 'requests>=2
-00000a20: 2e32 372e 312c 3c33 2e30 2e30 272c 0a20  .27.1,<3.0.0',. 
-00000a30: 2774 656e 6163 6974 793e 3d38 2e31 2e30  'tenacity>=8.1.0
-00000a40: 2c3c 392e 302e 3027 2c0a 2027 7479 7069  ,<9.0.0',. 'typi
-00000a50: 6e67 2d65 7874 656e 7369 6f6e 733e 3d34  ng-extensions>=4
-00000a60: 2e36 2e31 2c3c 352e 302e 3027 5d0a 0a73  .6.1,<5.0.0']..s
-00000a70: 6574 7570 5f6b 7761 7267 7320 3d20 7b0a  etup_kwargs = {.
-00000a80: 2020 2020 276e 616d 6527 3a20 2763 6174      'name': 'cat
-00000a90: 616c 7973 7477 616e 272c 0a20 2020 2027  alystwan',.    '
-00000aa0: 7665 7273 696f 6e27 3a20 2730 2e33 332e  version': '0.33.
-00000ab0: 3727 2c0a 2020 2020 2764 6573 6372 6970  7',.    'descrip
-00000ac0: 7469 6f6e 273a 2027 4369 7363 6f20 4361  tion': 'Cisco Ca
-00000ad0: 7461 6c79 7374 2057 414e 2053 444b 2066  talyst WAN SDK f
-00000ae0: 6f72 2050 7974 686f 6e27 2c0a 2020 2020  or Python',.    
-00000af0: 276c 6f6e 675f 6465 7363 7269 7074 696f  'long_descriptio
-00000b00: 6e27 3a20 273c 7020 616c 6967 6e3d 2263  n': '<p align="c
-00000b10: 656e 7465 7222 3e5c 6e20 203c 6120 6872  enter">\n  <a hr
-00000b20: 6566 3d22 2322 3e3c 696d 6720 7372 633d  ef="#"><img src=
-00000b30: 2264 6f63 732f 696d 6167 6573 2f63 6174  "docs/images/cat
-00000b40: 616c 7973 7477 616e 2e73 7667 2220 616c  alystwan.svg" al
-00000b50: 743d 2243 6973 636f 2043 6174 616c 7973  t="Cisco Catalys
-00000b60: 7420 5741 4e20 5344 4b20 4c6f 676f 2220  t WAN SDK Logo" 
-00000b70: 7374 796c 653d 2268 6569 6768 743a 3135  style="height:15
-00000b80: 3070 7822 202f 3e5c 6e3c 2f70 3e5c 6e5c  0px" />\n</p>\n\
-00000b90: 6e5b 215b 5079 7468 6f6e 2d53 7570 706f  n[![Python-Suppo
-00000ba0: 7274 6564 5d28 6874 7470 733a 2f2f 696d  rted](https://im
-00000bb0: 672e 7368 6965 6c64 732e 696f 2f73 7461  g.shields.io/sta
-00000bc0: 7469 632f 7631 3f6c 6162 656c 3d50 7974  tic/v1?label=Pyt
-00000bd0: 686f 6e26 6c6f 676f 3d50 7974 686f 6e26  hon&logo=Python&
-00000be0: 636f 6c6f 723d 3337 3736 4142 266d 6573  color=3776AB&mes
-00000bf0: 7361 6765 3d33 2e38 2532 307c 2532 3033  sage=3.8%20|%203
-00000c00: 2e39 2532 307c 2532 3033 2e31 3025 3230  .9%20|%203.10%20
-00000c10: 7c25 3230 332e 3131 2532 307c 2532 3033  |%203.11%20|%203
-00000c20: 2e31 3229 5d28 6874 7470 733a 2f2f 7777  .12)](https://ww
-00000c30: 772e 7079 7468 6f6e 2e6f 7267 2f29 5c6e  w.python.org/)\n
-00000c40: 5c6e 4369 7363 6f20 4361 7461 6c79 7374  \nCisco Catalyst
-00000c50: 2057 414e 2053 444b 2069 7320 6120 7061   WAN SDK is a pa
-00000c60: 636b 6167 6520 666f 7220 6372 6561 7469  ckage for creati
-00000c70: 6e67 2073 696d 706c 6520 616e 6420 7061  ng simple and pa
-00000c80: 7261 6c6c 656c 2061 7574 6f6d 6174 6963  rallel automatic
-00000c90: 2072 6571 7565 7374 7320 7669 6120 6f66   requests via of
-00000ca0: 6669 6369 616c 2053 442d 5741 4e20 4d61  ficial SD-WAN Ma
-00000cb0: 6e61 6765 7220 4150 492e 2049 7420 6973  nager API. It is
-00000cc0: 2069 6e74 656e 6465 6420 746f 2073 6572   intended to ser
-00000cd0: 7665 2061 7320 6120 6d75 6c74 6970 6c65  ve as a multiple
-00000ce0: 2073 6573 7369 6f6e 2068 616e 646c 6572   session handler
-00000cf0: 2028 7072 6f76 6964 6572 2c20 7072 6f76   (provider, prov
-00000d00: 6964 6572 2061 7320 6120 7465 6e61 6e74  ider as a tenant
-00000d10: 2c20 7465 6e61 6e74 292e 2054 6865 206c  , tenant). The l
-00000d20: 6962 7261 7279 2069 7320 6e6f 7420 6465  ibrary is not de
-00000d30: 7065 6e64 656e 7420 6f6e 2065 6e76 6972  pendent on envir
-00000d40: 6f6e 6d65 6e74 2077 6869 6368 2069 7320  onment which is 
-00000d50: 6265 696e 6720 7275 6e20 696e 2c20 796f  being run in, yo
-00000d60: 7520 6a75 7374 206e 6565 6420 6120 636f  u just need a co
-00000d70: 6e6e 6563 7469 6f6e 2074 6f20 616e 7920  nnection to any 
-00000d80: 5344 2d57 414e 204d 616e 6167 6572 2e5c  SD-WAN Manager.\
-00000d90: 6e5c 6e23 2320 496d 706f 7274 616e 7420  n\n## Important 
-00000da0: 4e6f 7469 6365 3a20 4561 726c 7920 4265  Notice: Early Be
-00000db0: 7461 2052 656c 6561 7365 5c6e 5c6e 5765  ta Release\n\nWe
-00000dc0: 6c63 6f6d 6520 746f 2074 6865 2043 6973  lcome to the Cis
-00000dd0: 636f 2043 6174 616c 7973 7420 5741 4e20  co Catalyst WAN 
-00000de0: 5344 4b21 5c6e 5c6e 5765 2061 7265 2074  SDK!\n\nWe are t
-00000df0: 6872 696c 6c65 6420 746f 2061 6e6e 6f75  hrilled to annou
-00000e00: 6e63 6520 7468 6174 2043 6973 636f 2043  nce that Cisco C
-00000e10: 6174 616c 7973 7420 5741 4e20 5344 4b20  atalyst WAN SDK 
-00000e20: 6973 206e 6f77 2061 7661 696c 6162 6c65  is now available
-00000e30: 2069 6e20 6561 726c 7920 6265 7461 2e20   in early beta. 
-00000e40: 5468 6973 2069 7320 616e 2065 7863 6974  This is an excit
-00000e50: 696e 6720 7374 6570 2066 6f72 7761 7264  ing step forward
-00000e60: 2069 6e20 656e 6162 6c69 6e67 2064 6576   in enabling dev
-00000e70: 656c 6f70 6572 7320 746f 2068 6172 6e65  elopers to harne
-00000e80: 7373 2074 6865 2066 756c 6c20 706f 7465  ss the full pote
-00000e90: 6e74 6961 6c20 6f66 2043 6973 636f 5c27  ntial of Cisco\'
-00000ea0: 7320 6e65 7477 6f72 6b69 6e67 2073 6f6c  s networking sol
-00000eb0: 7574 696f 6e73 2e20 2050 6c65 6173 6520  utions.  Please 
-00000ec0: 6265 2061 7761 7265 2074 6861 742c 2061  be aware that, a
-00000ed0: 7320 616e 2065 6172 6c79 2062 6574 6120  s an early beta 
-00000ee0: 7265 6c65 6173 652c 2074 6869 7320 7665  release, this ve
-00000ef0: 7273 696f 6e20 6f66 2074 6865 2053 444b  rsion of the SDK
-00000f00: 2069 7320 7374 696c 6c20 756e 6465 7267   is still underg
-00000f10: 6f69 6e67 2064 6576 656c 6f70 6d65 6e74  oing development
-00000f20: 2061 6e64 2074 6573 7469 6e67 2e20 4173   and testing. As
-00000f30: 2073 7563 682c 2069 7420 6973 2070 726f   such, it is pro
-00000f40: 7669 6465 6420 2261 7320 6973 2220 616e  vided "as is" an
-00000f50: 6420 7375 7070 6f72 7420 746f 2061 6464  d support to add
-00000f60: 7265 7373 2061 6e79 2069 7373 7565 7320  ress any issues 
-00000f70: 6172 6520 6c69 6d69 7465 6420 616e 6420  are limited and 
-00000f80: 6265 7374 2065 6666 6f72 742e 5c6e 5c6e  best effort.\n\n
-00000f90: 2323 204e 6f74 2072 6563 6f6d 6d65 6e64  ## Not recommend
-00000fa0: 2074 6f20 7573 6520 696e 2070 726f 6475   to use in produ
-00000fb0: 6374 696f 6e20 656e 7669 726f 6e6d 656e  ction environmen
-00000fc0: 7473 2e5c 6e57 6520 656e 636f 7572 6167  ts.\nWe encourag
-00000fd0: 6520 6465 7665 6c6f 7065 7273 2074 6f20  e developers to 
-00000fe0: 6578 706c 6f72 6520 616e 6420 7465 7374  explore and test
-00000ff0: 2074 6865 2053 444b 5c27 7320 6361 7061   the SDK\'s capa
-00001000: 6269 6c69 7469 6573 2c20 6275 7420 706c  bilities, but pl
-00001010: 6561 7365 2065 7865 7263 6973 6520 6361  ease exercise ca
-00001020: 7574 696f 6e20 7768 656e 2075 7369 6e67  ution when using
-00001030: 2069 7420 696e 2070 726f 6475 6374 696f   it in productio
-00001040: 6e20 656e 7669 726f 6e6d 656e 7473 2e20  n environments. 
-00001050: 2057 6520 6172 6520 6465 6469 6361 7465   We are dedicate
-00001060: 6420 746f 2069 6d70 726f 7669 6e67 2074  d to improving t
-00001070: 6865 2043 6973 636f 2043 6174 616c 7973  he Cisco Catalys
-00001080: 7420 5741 4e20 5344 4b20 616e 6420 7765  t WAN SDK and we
-00001090: 2076 616c 7565 2079 6f75 7220 696e 7075   value your inpu
-000010a0: 742e 2059 6f75 7220 6665 6564 6261 636b  t. Your feedback
-000010b0: 2069 7320 6372 7563 6961 6c20 746f 2075   is crucial to u
-000010c0: 732d 6974 2077 696c 6c20 6775 6964 6520  s-it will guide 
-000010d0: 7573 2069 6e20 7265 6669 6e69 6e67 2061  us in refining a
-000010e0: 6e64 2065 6e68 616e 6369 6e67 2074 6865  nd enhancing the
-000010f0: 2053 444b 2074 6f20 6265 7474 6572 206d   SDK to better m
-00001100: 6565 7420 796f 7572 206e 6565 6473 2e5c  eet your needs.\
-00001110: 6e54 6f20 7265 706f 7274 2061 6e79 2069  nTo report any i
-00001120: 7373 7565 732c 2073 6861 7265 2079 6f75  ssues, share you
-00001130: 7220 696e 7369 6768 7473 2c20 6f72 2073  r insights, or s
-00001140: 7567 6765 7374 2069 6d70 726f 7665 6d65  uggest improveme
-00001150: 6e74 732c 2070 6c65 6173 6520 7669 7369  nts, please visi
-00001160: 7420 6f75 7220 4973 7375 6573 2070 6167  t our Issues pag
-00001170: 6520 6f6e 2047 6974 4875 6220 6f72 2072  e on GitHub or r
-00001180: 6561 6368 206f 7574 2074 6f20 7573 2074  each out to us t
-00001190: 6872 6f75 6768 2074 6865 2070 726f 7669  hrough the provi
-000011a0: 6465 6420 636f 6d6d 756e 6963 6174 696f  ded communicatio
-000011b0: 6e20 6368 616e 6e65 6c73 2e5c 6e5c 6e54  n channels.\n\nT
-000011c0: 6861 6e6b 2079 6f75 2066 6f72 2062 6569  hank you for bei
-000011d0: 6e67 2061 2070 6172 7420 6f66 206f 7572  ng a part of our
-000011e0: 2064 6576 656c 6f70 6d65 6e74 206a 6f75   development jou
-000011f0: 726e 6579 215c 6e5c 6e23 2320 496e 7374  rney!\n\n## Inst
-00001200: 616c 6c61 7469 6f6e 5c6e 6060 6063 6f6e  allation\n```con
-00001210: 736f 6c65 5c6e 7069 7020 696e 7374 616c  sole\npip instal
-00001220: 6c20 6361 7461 6c79 7374 7761 6e5c 6e60  l catalystwan\n`
-00001230: 6060 5c6e 5c6e 2323 204d 616e 6167 6572  ``\n\n## Manager
-00001240: 2053 6573 7369 6f6e 5c6e 496e 206f 7264   Session\nIn ord
-00001250: 6572 2074 6f20 6578 6563 7574 6520 5344  er to execute SD
-00001260: 4b20 4150 4973 202a 2a4d 616e 6167 6572  K APIs **Manager
-00001270: 5365 7373 696f 6e2a 2a20 6e65 6564 7320  Session** needs 
-00001280: 746f 2062 6520 6372 6561 7465 642e 2054  to be created. T
-00001290: 6865 2066 6173 7465 7374 2077 6179 2074  he fastest way t
-000012a0: 6f20 6765 7420 7374 6172 7465 6420 6973  o get started is
-000012b0: 2074 6f20 7573 6520 6063 7265 6174 655f   to use `create_
-000012c0: 6d61 6e61 6765 725f 7365 7373 696f 6e28  manager_session(
-000012d0: 2960 206d 6574 686f 6420 7768 6963 6820  )` method which 
-000012e0: 636f 6e66 6967 7572 6573 2073 6573 7369  configures sessi
-000012f0: 6f6e 2c20 7065 7266 6f72 6d73 2061 7574  on, performs aut
-00001300: 6865 6e74 6963 6174 696f 6e20 666f 7220  hentication for 
-00001310: 6769 7665 6e20 6372 6564 656e 7469 616c  given credential
-00001320: 7320 616e 6420 7265 7475 726e 7320 2a2a  s and returns **
-00001330: 4d61 6e61 6765 7253 6573 7369 6f6e 2a2a  ManagerSession**
-00001340: 2069 6e73 7461 6e63 6520 696e 206f 7065   instance in ope
-00001350: 7261 7469 6f6e 616c 2073 7461 7465 2e20  rational state. 
-00001360: 2a2a 4d61 6e61 6765 7253 6573 7369 6f6e  **ManagerSession
-00001370: 2a2a 2070 726f 7669 6465 7320 6120 636f  ** provides a co
-00001380: 6c6c 6563 7469 6f6e 206f 6620 7375 7070  llection of supp
-00001390: 6f72 7465 6420 4150 4973 2069 6e20 6061  orted APIs in `a
-000013a0: 7069 6020 696e 7374 616e 6365 2076 6172  pi` instance var
-000013b0: 6961 626c 652e 5c6e 506c 6561 7365 2063  iable.\nPlease c
-000013c0: 6865 636b 2065 7861 6d70 6c65 2062 656c  heck example bel
-000013d0: 6f77 3a5c 6e5c 6e60 6060 7079 7468 6f6e  ow:\n\n```python
-000013e0: 5c6e 6672 6f6d 2063 6174 616c 7973 7477  \nfrom catalystw
-000013f0: 616e 2e73 6573 7369 6f6e 2069 6d70 6f72  an.session impor
-00001400: 7420 6372 6561 7465 5f6d 616e 6167 6572  t create_manager
-00001410: 5f73 6573 7369 6f6e 5c6e 5c6e 7572 6c20  _session\n\nurl 
-00001420: 3d20 2265 7861 6d70 6c65 2e63 6f6d 225c  = "example.com"\
-00001430: 6e75 7365 726e 616d 6520 3d20 2261 646d  nusername = "adm
-00001440: 696e 225c 6e70 6173 7377 6f72 6420 3d20  in"\npassword = 
-00001450: 2270 6173 7377 6f72 6431 3233 225c 6e5c  "password123"\n\
-00001460: 6e77 6974 6820 6372 6561 7465 5f6d 616e  nwith create_man
-00001470: 6167 6572 5f73 6573 7369 6f6e 2875 726c  ager_session(url
-00001480: 3d75 726c 2c20 7573 6572 6e61 6d65 3d75  =url, username=u
-00001490: 7365 726e 616d 652c 2070 6173 7377 6f72  sername, passwor
-000014a0: 643d 7061 7373 776f 7264 2920 6173 2073  d=password) as s
-000014b0: 6573 7369 6f6e 3a5c 6e20 2020 2064 6576  ession:\n    dev
-000014c0: 6963 6573 203d 2073 6573 7369 6f6e 2e61  ices = session.a
-000014d0: 7069 2e64 6576 6963 6573 2e67 6574 2829  pi.devices.get()
-000014e0: 5c6e 2020 2020 7072 696e 7428 6465 7669  \n    print(devi
-000014f0: 6365 7329 5c6e 6060 605c 6e2a 2a4d 616e  ces)\n```\n**Man
-00001500: 6167 6572 5365 7373 696f 6e2a 2a20 6578  agerSession** ex
-00001510: 7465 6e64 7320 5b72 6571 7565 7374 732e  tends [requests.
-00001520: 5365 7373 696f 6e5d 2868 7474 7073 3a2f  Session](https:/
-00001530: 2f72 6571 7565 7374 732e 7265 6164 7468  /requests.readth
-00001540: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00001550: 7374 2f75 7365 722f 6164 7661 6e63 6564  st/user/advanced
-00001560: 2f23 7365 7373 696f 6e2d 6f62 6a65 6374  /#session-object
-00001570: 7329 2073 6f20 616c 6c20 6675 6e63 7469  s) so all functi
-00001580: 6f6e 616c 6974 7920 6672 6f6d 205b 7265  onality from [re
-00001590: 7175 6573 7473 5d28 6874 7470 733a 2f2f  quests](https://
-000015a0: 7265 7175 6573 7473 2e72 6561 6474 6865  requests.readthe
-000015b0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-000015c0: 742f 2920 6c69 6272 6172 7920 6973 2061  t/) library is a
-000015d0: 7661 6961 626c 6520 746f 2075 7365 722c  vaiable to user,
-000015e0: 2069 7420 616c 736f 2069 6d70 6c65 6d65   it also impleme
-000015f0: 6e74 7320 7079 7468 6f6e 205b 636f 6e74  nts python [cont
-00001600: 6578 746d 616e 6167 6572 5d28 6874 7470  extmanager](http
-00001610: 733a 2f2f 646f 6373 2e70 7974 686f 6e2e  s://docs.python.
-00001620: 6f72 672f 332e 382f 6c69 6272 6172 792f  org/3.8/library/
-00001630: 636f 6e74 6578 746c 6962 2e68 746d 6c23  contextlib.html#
-00001640: 636f 6e74 6578 746c 6962 2e63 6f6e 7465  contextlib.conte
-00001650: 7874 6d61 6e61 6765 7229 2061 6e64 2061  xtmanager) and a
-00001660: 7574 6f6d 6174 6963 616c 6c79 2066 7265  utomatically fre
-00001670: 6573 2073 6572 7665 7220 7265 736f 7572  es server resour
-00001680: 6365 7320 6f6e 2065 7869 742e 5c6e 5c6e  ces on exit.\n\n
-00001690: 3c64 6574 6169 6c73 3e5c 6e20 2020 203c  <details>\n    <
-000016a0: 7375 6d6d 6172 793e 203c 623e 436f 6e66  summary> <b>Conf
-000016b0: 6967 7572 6520 4d61 6e61 6765 7220 5365  igure Manager Se
-000016c0: 7373 696f 6e20 6265 666f 7265 2075 7369  ssion before usi
-000016d0: 6e67 3c2f 623e 203c 693e 2863 6c69 636b  ng</b> <i>(click
-000016e0: 2074 6f20 6578 7061 6e64 293c 2f69 3e3c   to expand)</i><
-000016f0: 2f73 756d 6d61 7279 3e5c 6e5c 6e49 7420  /summary>\n\nIt 
-00001700: 6973 2070 6f73 7369 626c 6520 746f 2063  is possible to c
-00001710: 6f6e 6669 6775 7265 202a 2a4d 616e 6167  onfigure **Manag
-00001720: 6572 5365 7373 696f 6e2a 2a20 7072 696f  erSession** prio
-00001730: 7220 7365 6e64 696e 6720 616e 7920 7265  r sending any re
-00001740: 7175 6573 742e 5c6e 5c6e 6060 6070 7974  quest.\n\n```pyt
-00001750: 686f 6e5c 6e66 726f 6d20 6361 7461 6c79  hon\nfrom cataly
-00001760: 7374 7761 6e2e 7365 7373 696f 6e20 696d  stwan.session im
-00001770: 706f 7274 204d 616e 6167 6572 5365 7373  port ManagerSess
-00001780: 696f 6e5c 6e5c 6e75 726c 203d 2022 6578  ion\n\nurl = "ex
-00001790: 616d 706c 652e 636f 6d22 5c6e 7573 6572  ample.com"\nuser
-000017a0: 6e61 6d65 203d 2022 6164 6d69 6e22 5c6e  name = "admin"\n
-000017b0: 7061 7373 776f 7264 203d 2022 7061 7373  password = "pass
-000017c0: 776f 7264 3132 3322 5c6e 5c6e 2320 636f  word123"\n\n# co
-000017d0: 6e66 6967 7572 6520 7365 7373 696f 6e20  nfigure session 
-000017e0: 7573 696e 6720 636f 6e73 7472 7563 746f  using constructo
-000017f0: 7220 2d20 6e6f 7468 696e 6720 7769 6c6c  r - nothing will
-00001800: 2062 6520 7365 6e74 2074 6f20 7461 7267   be sent to targ
-00001810: 6574 2073 6572 7665 7220 7965 745c 6e73  et server yet\ns
-00001820: 6573 7369 6f6e 203d 204d 616e 6167 6572  ession = Manager
-00001830: 5365 7373 696f 6e28 7572 6c3d 7572 6c2c  Session(url=url,
-00001840: 2075 7365 726e 616d 653d 7573 6572 6e61   username=userna
-00001850: 6d65 2c20 7061 7373 776f 7264 3d70 6173  me, password=pas
-00001860: 7377 6f72 6429 5c6e 2320 6c6f 6769 6e20  sword)\n# login 
-00001870: 616e 6420 7365 6e64 2072 6571 7565 7374  and send request
-00001880: 735c 6e73 6573 7369 6f6e 2e6c 6f67 696e  s\nsession.login
-00001890: 2829 5c6e 7365 7373 696f 6e2e 6765 7428  ()\nsession.get(
-000018a0: 222f 6461 7461 7365 7276 6963 652f 6465  "/dataservice/de
-000018b0: 7669 6365 2229 5c6e 7365 7373 696f 6e2e  vice")\nsession.
-000018c0: 636c 6f73 6528 295c 6e60 6060 5c6e 5768  close()\n```\nWh
-000018d0: 656e 2069 6e74 6572 6163 7469 6e67 2077  en interacting w
-000018e0: 6974 6820 7468 6520 5344 5741 4e20 4d61  ith the SDWAN Ma
-000018f0: 6e61 6765 7220 4150 4920 7769 7468 6f75  nager API withou
-00001900: 7420 7573 696e 6720 6120 636f 6e74 6578  t using a contex
-00001910: 7420 6d61 6e61 6765 722c 2069 745c 2773  t manager, it\'s
-00001920: 2069 6d70 6f72 7461 6e74 205c 6e74 6f20   important \nto 
-00001930: 6d61 6e75 616c 6c79 2065 7865 6375 7465  manually execute
-00001940: 2074 6865 2060 636c 6f73 6528 2960 206d   the `close()` m
-00001950: 6574 686f 6420 746f 2072 656c 6561 7365  ethod to release
-00001960: 2074 6865 2075 7365 7220 7365 7373 696f   the user sessio
-00001970: 6e20 7265 736f 7572 6365 2e5c 6e45 6e73  n resource.\nEns
-00001980: 7572 6520 7468 6174 2074 6865 2060 636c  ure that the `cl
-00001990: 6f73 6528 2960 206d 6574 686f 6420 6973  ose()` method is
-000019a0: 2063 616c 6c65 6420 6166 7465 7220 796f   called after yo
-000019b0: 7520 6861 7665 2066 696e 6973 6865 6420  u have finished 
-000019c0: 7573 696e 6720 7468 6520 7365 7373 696f  using the sessio
-000019d0: 6e20 746f 206d 6169 6e74 6169 6e20 6f70  n to maintain op
-000019e0: 7469 6d61 6c20 7265 736f 7572 6365 206d  timal resource m
-000019f0: 616e 6167 656d 656e 7420 616e 6420 6176  anagement and av
-00001a00: 6f69 6420 706f 7465 6e74 6961 6c20 6572  oid potential er
-00001a10: 726f 7273 2e5c 6e5c 6e3c 2f64 6574 6169  rors.\n\n</detai
-00001a20: 6c73 3e5c 6e5c 6e3c 6465 7461 696c 733e  ls>\n\n<details>
-00001a30: 5c6e 2020 2020 3c73 756d 6d61 7279 3e20  \n    <summary> 
-00001a40: 3c62 3e4c 6f67 696e 2061 7320 5465 6e61  <b>Login as Tena
-00001a50: 6e74 3c2f 623e 203c 693e 2863 6c69 636b  nt</b> <i>(click
-00001a60: 2074 6f20 6578 7061 6e64 293c 2f69 3e3c   to expand)</i><
-00001a70: 2f73 756d 6d61 7279 3e5c 6e5c 6e54 656e  /summary>\n\nTen
-00001a80: 616e 7420 646f 6d61 696e 206e 6565 6473  ant domain needs
-00001a90: 2074 6f20 6265 2070 726f 7669 6465 6420   to be provided 
-00001aa0: 696e 2075 726c 2074 6f67 6574 6865 7220  in url together 
-00001ab0: 7769 7468 2054 656e 616e 7420 6372 6564  with Tenant cred
-00001ac0: 656e 7469 616c 732e 5c6e 5c6e 6060 6070  entials.\n\n```p
-00001ad0: 7974 686f 6e5c 6e66 726f 6d20 6361 7461  ython\nfrom cata
-00001ae0: 6c79 7374 7761 6e2e 7365 7373 696f 6e20  lystwan.session 
-00001af0: 696d 706f 7274 2063 7265 6174 655f 6d61  import create_ma
-00001b00: 6e61 6765 725f 7365 7373 696f 6e5c 6e5c  nager_session\n\
-00001b10: 6e75 726c 203d 2022 7465 6e61 6e74 2e65  nurl = "tenant.e
-00001b20: 7861 6d70 6c65 2e63 6f6d 225c 6e75 7365  xample.com"\nuse
-00001b30: 726e 616d 6520 3d20 2274 656e 616e 745f  rname = "tenant_
-00001b40: 7573 6572 225c 6e70 6173 7377 6f72 6420  user"\npassword 
-00001b50: 3d20 2270 6173 7377 6f72 6431 3233 225c  = "password123"\
-00001b60: 6e5c 6e77 6974 6820 6372 6561 7465 5f6d  n\nwith create_m
-00001b70: 616e 6167 6572 5f73 6573 7369 6f6e 2875  anager_session(u
-00001b80: 726c 3d75 726c 2c20 7573 6572 6e61 6d65  rl=url, username
-00001b90: 3d75 7365 726e 616d 652c 2070 6173 7377  =username, passw
-00001ba0: 6f72 643d 7061 7373 776f 7264 2920 6173  ord=password) as
-00001bb0: 2073 6573 7369 6f6e 3a5c 6e20 2020 2070   session:\n    p
-00001bc0: 7269 6e74 2873 6573 7369 6f6e 2e73 6573  rint(session.ses
-00001bd0: 7369 6f6e 5f74 7970 6529 5c6e 6060 605c  sion_type)\n```\
-00001be0: 6e5c 6e3c 2f64 6574 6169 6c73 3e5c 6e5c  n\n</details>\n\
-00001bf0: 6e3c 6465 7461 696c 733e 5c6e 2020 2020  n<details>\n    
-00001c00: 3c73 756d 6d61 7279 3e20 3c62 3e4c 6f67  <summary> <b>Log
-00001c10: 696e 2061 7320 5072 6f76 6964 6572 2d61  in as Provider-a
-00001c20: 732d 5465 6e61 6e74 3c2f 623e 203c 693e  s-Tenant</b> <i>
-00001c30: 2863 6c69 636b 2074 6f20 6578 7061 6e64  (click to expand
-00001c40: 293c 2f69 3e3c 2f73 756d 6d61 7279 3e5c  )</i></summary>\
-00001c50: 6e5c 6e54 656e 616e 7420 6073 7562 646f  n\nTenant `subdo
-00001c60: 6d61 696e 6020 6e65 6564 7320 746f 2062  main` needs to b
-00001c70: 6520 7072 6f76 6964 6564 2061 7320 6164  e provided as ad
-00001c80: 6469 7469 6f6e 616c 2061 7267 756d 656e  ditional argumen
-00001c90: 7420 746f 6765 7468 6572 2077 6974 6820  t together with 
-00001ca0: 5072 6f76 6964 6572 2063 7265 6465 6e74  Provider credent
-00001cb0: 6961 6c73 2e5c 6e5c 6e60 6060 7079 7468  ials.\n\n```pyth
-00001cc0: 6f6e 5c6e 6672 6f6d 2063 6174 616c 7973  on\nfrom catalys
-00001cd0: 7477 616e 2e73 6573 7369 6f6e 2069 6d70  twan.session imp
-00001ce0: 6f72 7420 6372 6561 7465 5f6d 616e 6167  ort create_manag
-00001cf0: 6572 5f73 6573 7369 6f6e 5c6e 5c6e 7572  er_session\n\nur
-00001d00: 6c20 3d20 2265 7861 6d70 6c65 2e63 6f6d  l = "example.com
-00001d10: 225c 6e75 7365 726e 616d 6520 3d20 2270  "\nusername = "p
-00001d20: 726f 7669 6465 7222 5c6e 7061 7373 776f  rovider"\npasswo
-00001d30: 7264 203d 2022 7061 7373 776f 7264 3132  rd = "password12
-00001d40: 3322 5c6e 7375 6264 6f6d 6169 6e20 3d20  3"\nsubdomain = 
-00001d50: 2274 656e 616e 742e 6578 616d 706c 652e  "tenant.example.
-00001d60: 636f 6d22 5c6e 5c6e 7769 7468 2063 7265  com"\n\nwith cre
-00001d70: 6174 655f 6d61 6e61 6765 725f 7365 7373  ate_manager_sess
-00001d80: 696f 6e28 7572 6c3d 7572 6c2c 2075 7365  ion(url=url, use
-00001d90: 726e 616d 653d 7573 6572 6e61 6d65 2c20  rname=username, 
-00001da0: 7061 7373 776f 7264 3d70 6173 7377 6f72  password=passwor
-00001db0: 642c 2073 7562 646f 6d61 696e 3d73 7562  d, subdomain=sub
-00001dc0: 646f 6d61 696e 2920 6173 2073 6573 7369  domain) as sessi
-00001dd0: 6f6e 3a5c 6e20 2020 2070 7269 6e74 2873  on:\n    print(s
-00001de0: 6573 7369 6f6e 2e73 6573 7369 6f6e 5f74  ession.session_t
-00001df0: 7970 6529 5c6e 6060 605c 6e5c 6e3c 2f64  ype)\n```\n\n</d
-00001e00: 6574 6169 6c73 3e5c 6e5c 6e5c 6e5c 6e23  etails>\n\n\n\n#
-00001e10: 2320 4150 4920 7573 6167 6520 6578 616d  # API usage exam
-00001e20: 706c 6573 5c6e 416c 6c20 6578 616d 706c  ples\nAll exampl
-00001e30: 6573 2062 656c 6f77 2061 7373 756d 6573  es below assumes
-00001e40: 2060 7365 7373 696f 6e60 2076 6172 6961   `session` varia
-00001e50: 626c 6520 636f 6e74 6169 6e73 206c 6f67  ble contains log
-00001e60: 6765 642d 696e 205b 4d61 6e61 6765 7220  ged-in [Manager 
-00001e70: 5365 7373 696f 6e5d 2823 4d61 6e61 6765  Session](#Manage
-00001e80: 722d 5365 7373 696f 6e29 2069 6e73 7461  r-Session) insta
-00001e90: 6e63 652e 5c6e 5c6e 3c64 6574 6169 6c73  nce.\n\n<details
-00001ea0: 3e5c 6e20 2020 203c 7375 6d6d 6172 793e  >\n    <summary>
-00001eb0: 203c 623e 4765 7420 6465 7669 6365 733c   <b>Get devices<
-00001ec0: 2f62 3e20 3c69 3e28 636c 6963 6b20 746f  /b> <i>(click to
-00001ed0: 2065 7870 616e 6429 3c2f 693e 3c2f 7375   expand)</i></su
-00001ee0: 6d6d 6172 793e 5c6e 5c6e 6060 6070 7974  mmary>\n\n```pyt
-00001ef0: 686f 6e5c 6e64 6576 6963 6573 203d 2073  hon\ndevices = s
-00001f00: 6573 7369 6f6e 2e61 7069 2e64 6576 6963  ession.api.devic
-00001f10: 6573 2e67 6574 2829 5c6e 6060 605c 6e5c  es.get()\n```\n\
-00001f20: 6e3c 2f64 6574 6169 6c73 3e5c 6e5c 6e3c  n</details>\n\n<
-00001f30: 6465 7461 696c 733e 5c6e 2020 2020 3c73  details>\n    <s
-00001f40: 756d 6d61 7279 3e20 3c62 3e41 646d 696e  ummary> <b>Admin
-00001f50: 2054 6563 683c 2f62 3e20 3c69 3e28 636c   Tech</b> <i>(cl
-00001f60: 6963 6b20 746f 2065 7870 616e 6429 3c2f  ick to expand)</
-00001f70: 693e 3c2f 7375 6d6d 6172 793e 5c6e 5c6e  i></summary>\n\n
-00001f80: 6060 6050 7974 686f 6e5c 6e61 646d 696e  ```Python\nadmin
-00001f90: 5f74 6563 685f 6669 6c65 203d 2073 6573  _tech_file = ses
-00001fa0: 7369 6f6e 2e61 7069 2e61 646d 696e 5f74  sion.api.admin_t
-00001fb0: 6563 682e 6765 6e65 7261 7465 2822 3137  ech.generate("17
-00001fc0: 322e 3136 2e32 3535 2e31 3122 295c 6e73  2.16.255.11")\ns
-00001fd0: 6573 7369 6f6e 2e61 7069 2e61 646d 696e  ession.api.admin
-00001fe0: 5f74 6563 682e 646f 776e 6c6f 6164 2861  _tech.download(a
-00001ff0: 646d 696e 5f74 6563 685f 6669 6c65 295c  dmin_tech_file)\
-00002000: 6e73 6573 7369 6f6e 2e61 7069 2e61 646d  nsession.api.adm
-00002010: 696e 5f74 6563 682e 6465 6c65 7465 2861  in_tech.delete(a
-00002020: 646d 696e 5f74 6563 685f 6669 6c65 295c  dmin_tech_file)\
-00002030: 6e60 6060 5c6e 3c2f 6465 7461 696c 733e  n```\n</details>
-00002040: 5c6e 5c6e 3c64 6574 6169 6c73 3e5c 6e20  \n\n<details>\n 
-00002050: 2020 203c 7375 6d6d 6172 793e 203c 623e     <summary> <b>
-00002060: 5370 6565 6420 7465 7374 3c2f 623e 203c  Speed test</b> <
-00002070: 693e 2863 6c69 636b 2074 6f20 6578 7061  i>(click to expa
-00002080: 6e64 293c 2f69 3e3c 2f73 756d 6d61 7279  nd)</i></summary
-00002090: 3e5c 6e5c 6e60 6060 7079 7468 6f6e 5c6e  >\n\n```python\n
-000020a0: 6465 7669 6365 7320 3d20 7365 7373 696f  devices = sessio
-000020b0: 6e2e 6170 692e 6465 7669 6365 732e 6765  n.api.devices.ge
-000020c0: 7428 295c 6e73 7065 6564 7465 7374 203d  t()\nspeedtest =
-000020d0: 2073 6573 7369 6f6e 2e61 7069 2e73 7065   session.api.spe
-000020e0: 6564 7465 7374 2e73 7065 6564 7465 7374  edtest.speedtest
-000020f0: 2864 6576 6963 6573 5b30 5d2c 2064 6576  (devices[0], dev
-00002100: 6963 6573 5b31 5d29 5c6e 6060 605c 6e5c  ices[1])\n```\n\
-00002110: 6e3c 2f64 6574 6169 6c73 3e5c 6e5c 6e3c  n</details>\n\n<
-00002120: 6465 7461 696c 733e 5c6e 2020 2020 3c73  details>\n    <s
-00002130: 756d 6d61 7279 3e20 3c62 3e55 7067 7261  ummary> <b>Upgra
-00002140: 6465 2064 6576 6963 653c 2f62 3e20 3c69  de device</b> <i
-00002150: 3e28 636c 6963 6b20 746f 2065 7870 616e  >(click to expan
-00002160: 6429 3c2f 693e 3c2f 7375 6d6d 6172 793e  d)</i></summary>
-00002170: 5c6e 5c6e 6060 6070 7974 686f 6e5c 6e23  \n\n```python\n#
-00002180: 2050 7265 7061 7265 2064 6576 6963 6573   Prepare devices
-00002190: 206c 6973 745c 6e63 6f6e 7472 6f6c 6c65   list\ncontrolle
-000021a0: 7273 203d 2073 6573 7369 6f6e 2e65 6e64  rs = session.end
-000021b0: 706f 696e 7473 2e63 6f6e 6669 6775 7261  points.configura
-000021c0: 7469 6f6e 5f64 6576 6963 655f 696e 7665  tion_device_inve
-000021d0: 6e74 6f72 792e 6765 745f 6465 7669 6365  ntory.get_device
-000021e0: 5f64 6574 6169 6c73 285c 2763 6f6e 7472  _details(\'contr
-000021f0: 6f6c 6c65 7273 5c27 295c 6e76 736d 6172  ollers\')\nvsmar
-00002200: 7473 203d 2063 6f6e 7472 6f6c 6c65 7273  ts = controllers
-00002210: 2e66 696c 7465 7228 7065 7273 6f6e 616c  .filter(personal
-00002220: 6974 793d 5065 7273 6f6e 616c 6974 792e  ity=Personality.
-00002230: 5653 4d41 5254 295c 6e69 6d61 6765 203d  VSMART)\nimage =
-00002240: 2022 7669 7074 656c 612d 3230 2e37 2e32   "viptela-20.7.2
-00002250: 2d78 3836 5f36 342e 7461 722e 677a 225c  -x86_64.tar.gz"\
-00002260: 6e5c 6e23 2055 706c 6f61 6420 696d 6167  n\n# Upload imag
-00002270: 655c 6e73 6573 7369 6f6e 2e61 7069 2e72  e\nsession.api.r
-00002280: 6570 6f73 6974 6f72 792e 7570 6c6f 6164  epository.upload
-00002290: 5f69 6d61 6765 2869 6d61 6765 295c 6e5c  _image(image)\n\
-000022a0: 6e23 2049 6e73 7461 6c6c 2073 6f66 7477  n# Install softw
-000022b0: 6172 655c 6e5c 6e69 6e73 7461 6c6c 5f74  are\n\ninstall_t
-000022c0: 6173 6b20 3d20 7365 7373 696f 6e2e 6170  ask = session.ap
-000022d0: 692e 736f 6674 7761 7265 2e69 6e73 7461  i.software.insta
-000022e0: 6c6c 2864 6576 6963 6573 3d76 736d 6172  ll(devices=vsmar
-000022f0: 7473 2c20 696d 6167 653d 696d 6167 6529  ts, image=image)
-00002300: 5c6e 5c6e 2320 4368 6563 6b20 6163 7469  \n\n# Check acti
-00002310: 6f6e 2073 7461 7475 735c 6e69 6e73 7461  on status\ninsta
-00002320: 6c6c 5f74 6173 6b2e 7761 6974 5f66 6f72  ll_task.wait_for
-00002330: 5f63 6f6d 706c 6574 6564 2829 5c6e 6060  _completed()\n``
-00002340: 605c 6e5c 6e3c 2f64 6574 6169 6c73 3e5c  `\n\n</details>\
-00002350: 6e5c 6e3c 6465 7461 696c 733e 5c6e 2020  n\n<details>\n  
-00002360: 2020 3c73 756d 6d61 7279 3e20 3c62 3e47    <summary> <b>G
-00002370: 6574 2061 6c61 726d 733c 2f62 3e20 3c69  et alarms</b> <i
-00002380: 3e28 636c 6963 6b20 746f 2065 7870 616e  >(click to expan
-00002390: 6429 3c2f 693e 3c2f 7375 6d6d 6172 793e  d)</i></summary>
-000023a0: 5c6e 546f 2067 6574 2061 6c6c 2061 6c61  \nTo get all ala
-000023b0: 726d 733a 5c6e 5c6e 6060 6070 7974 686f  rms:\n\n```pytho
-000023c0: 6e5c 6e61 6c61 726d 7320 3d20 7365 7373  n\nalarms = sess
-000023d0: 696f 6e2e 6170 692e 616c 6172 6d73 2e67  ion.api.alarms.g
-000023e0: 6574 2829 5c6e 6060 605c 6e5c 6e54 6f20  et()\n```\n\nTo 
-000023f0: 6765 7420 616c 6c20 6e6f 7420 7669 6577  get all not view
-00002400: 6564 2061 6c61 726d 733a 5c6e 5c6e 6060  ed alarms:\n\n``
-00002410: 6070 7974 686f 6e5c 6e6e 6f74 5f76 6965  `python\nnot_vie
-00002420: 7765 645f 616c 6172 6d73 203d 2073 6573  wed_alarms = ses
-00002430: 7369 6f6e 2e61 7069 2e61 6c61 726d 732e  sion.api.alarms.
-00002440: 6765 7428 292e 6669 6c74 6572 2876 6965  get().filter(vie
-00002450: 7765 643d 4661 6c73 6529 5c6e 6060 605c  wed=False)\n```\
-00002460: 6e5c 6e54 6f20 6765 7420 616c 6c20 616c  n\nTo get all al
-00002470: 6172 6d73 2066 726f 6d20 7061 7374 2060  arms from past `
-00002480: 6e60 2068 6f75 7273 3a5c 6e5c 6e60 6060  n` hours:\n\n```
-00002490: 7079 7468 6f6e 5c6e 6e20 3d20 3234 5c6e  python\nn = 24\n
-000024a0: 616c 6172 6d73 5f66 726f 6d5f 6e5f 686f  alarms_from_n_ho
-000024b0: 7572 7320 3d20 7365 7373 696f 6e2e 6170  urs = session.ap
-000024c0: 692e 616c 6172 6d73 2e67 6574 2866 726f  i.alarms.get(fro
-000024d0: 6d5f 7469 6d65 3d6e 295c 6e60 6060 5c6e  m_time=n)\n```\n
-000024e0: 5c6e 546f 2067 6574 2061 6c6c 2063 7269  \nTo get all cri
-000024f0: 7469 6361 6c20 616c 6172 6d73 2066 726f  tical alarms fro
-00002500: 6d20 7061 7374 2060 6e60 2068 6f75 7273  m past `n` hours
-00002510: 3a5c 6e5c 6e60 6060 7079 7468 6f6e 5c6e  :\n\n```python\n
-00002520: 6672 6f6d 2063 6174 616c 7973 7477 616e  from catalystwan
-00002530: 2e75 7469 6c73 2e61 6c61 726d 5f73 7461  .utils.alarm_sta
-00002540: 7475 7320 696d 706f 7274 2053 6576 6572  tus import Sever
-00002550: 6974 795c 6e6e 203d 2034 385c 6e63 7269  ity\nn = 48\ncri
-00002560: 7469 6361 6c5f 616c 6172 6d73 203d 2073  tical_alarms = s
-00002570: 6573 7369 6f6e 2e61 7069 2e61 6c61 726d  ession.api.alarm
-00002580: 732e 6765 7428 6672 6f6d 5f74 696d 653d  s.get(from_time=
-00002590: 6e29 2e66 696c 7465 7228 7365 7665 7269  n).filter(severi
-000025a0: 7479 3d53 6576 6572 6974 792e 4352 4954  ty=Severity.CRIT
-000025b0: 4943 414c 295c 6e60 6060 5c6e 5c6e 3c2f  ICAL)\n```\n\n</
-000025c0: 6465 7461 696c 733e 5c6e 5c6e 3c64 6574  details>\n\n<det
-000025d0: 6169 6c73 3e5c 6e20 2020 203c 7375 6d6d  ails>\n    <summ
-000025e0: 6172 793e 203c 623e 5573 6572 733c 2f62  ary> <b>Users</b
-000025f0: 3e20 3c69 3e28 636c 6963 6b20 746f 2065  > <i>(click to e
-00002600: 7870 616e 6429 3c2f 693e 3c2f 7375 6d6d  xpand)</i></summ
-00002610: 6172 793e 5c6e 5c6e 6060 6070 7974 686f  ary>\n\n```pytho
-00002620: 6e5c 6e23 2047 6574 2061 6c6c 2075 7365  n\n# Get all use
-00002630: 7273 5c6e 7365 7373 696f 6e2e 6170 692e  rs\nsession.api.
-00002640: 7573 6572 732e 6765 7428 295c 6e5c 6e23  users.get()\n\n#
-00002650: 2043 7265 6174 6520 7573 6572 5c6e 6672   Create user\nfr
-00002660: 6f6d 2063 6174 616c 7973 7477 616e 2e65  om catalystwan.e
-00002670: 6e64 706f 696e 7473 2e61 646d 696e 6973  ndpoints.adminis
-00002680: 7472 6174 696f 6e5f 7573 6572 5f61 6e64  tration_user_and
-00002690: 5f67 726f 7570 2069 6d70 6f72 7420 5573  _group import Us
-000026a0: 6572 5c6e 6e65 775f 7573 6572 203d 2055  er\nnew_user = U
-000026b0: 7365 7228 7573 6572 6e61 6d65 3d22 6e65  ser(username="ne
-000026c0: 775f 7573 6572 222c 2070 6173 7377 6f72  w_user", passwor
-000026d0: 643d 226e 6577 5f75 7365 7222 2c20 6772  d="new_user", gr
-000026e0: 6f75 703d 5b22 6e65 7461 646d 696e 225d  oup=["netadmin"]
-000026f0: 2c20 6465 7363 7269 7074 696f 6e3d 226e  , description="n
-00002700: 6577 2075 7365 7222 295c 6e73 6573 7369  ew user")\nsessi
-00002710: 6f6e 2e61 7069 2e75 7365 7273 2e63 7265  on.api.users.cre
-00002720: 6174 6528 6e65 775f 7573 6572 295c 6e5c  ate(new_user)\n\
-00002730: 6e23 2055 7064 6174 6520 7573 6572 2064  n# Update user d
-00002740: 6174 615c 6e6e 6577 5f75 7365 725f 7570  ata\nnew_user_up
-00002750: 6461 7465 203d 2055 7365 7255 7064 6174  date = UserUpdat
-00002760: 6552 6571 7565 7374 2875 7365 726e 616d  eRequest(usernam
-00002770: 653d 226e 6577 5f75 7365 7222 2c20 6772  e="new_user", gr
-00002780: 6f75 703d 5b22 6e65 7461 646d 696e 222c  oup=["netadmin",
-00002790: 2022 6e65 746f 7073 225d 2c20 6c6f 6361   "netops"], loca
-000027a0: 6c65 3d22 656e 5f55 5322 2c20 6465 7363  le="en_US", desc
-000027b0: 7269 7074 696f 6e3d 2275 7064 6174 6564  ription="updated
-000027c0: 2d6e 6577 5f75 7365 722d 6465 7363 7269  -new_user-descri
-000027d0: 7074 696f 6e22 295c 6e73 6573 7369 6f6e  ption")\nsession
-000027e0: 2e61 7069 2e75 7365 7273 2e75 7064 6174  .api.users.updat
-000027f0: 6528 6e65 775f 7573 6572 5f75 7064 6174  e(new_user_updat
-00002800: 6529 5c6e 5c6e 2320 5570 6461 7465 2075  e)\n\n# Update u
-00002810: 7365 7220 7061 7373 776f 7264 5c6e 7365  ser password\nse
-00002820: 7373 696f 6e2e 6170 692e 7573 6572 732e  ssion.api.users.
-00002830: 7570 6461 7465 5f70 6173 7377 6f72 6428  update_password(
-00002840: 226e 6577 5f75 7365 7222 2c20 226e 3357  "new_user", "n3W
-00002850: 2d50 3473 2477 3072 6422 295c 6e5c 6e23  -P4s$w0rd")\n\n#
-00002860: 2052 6573 6574 2075 7365 725c 6e73 6573   Reset user\nses
-00002870: 7369 6f6e 2e61 7069 2e75 7365 7273 2e72  sion.api.users.r
-00002880: 6573 6574 2822 6e65 775f 7573 6572 2229  eset("new_user")
-00002890: 5c6e 5c6e 2320 4465 6c65 7465 2075 7365  \n\n# Delete use
-000028a0: 725c 6e73 6573 7369 6f6e 2e61 7069 2e75  r\nsession.api.u
-000028b0: 7365 7273 2e64 656c 6574 6528 226e 6577  sers.delete("new
-000028c0: 5f75 7365 7222 295c 6e5c 6e23 2047 6574  _user")\n\n# Get
-000028d0: 2063 7572 7265 6e74 2075 7365 7220 6175   current user au
-000028e0: 7468 656e 7469 6361 7469 6f6e 2074 7970  thentication typ
-000028f0: 6520 616e 6420 726f 6c65 5c6e 7365 7373  e and role\nsess
-00002900: 696f 6e2e 6170 692e 7573 6572 732e 6765  ion.api.users.ge
-00002910: 745f 6175 7468 5f74 7970 6528 295c 6e73  t_auth_type()\ns
-00002920: 6573 7369 6f6e 2e61 7069 2e75 7365 7273  ession.api.users
-00002930: 2e67 6574 5f72 6f6c 6528 295c 6e60 6060  .get_role()\n```
-00002940: 5c6e 5c6e 3c2f 6465 7461 696c 733e 5c6e  \n\n</details>\n
-00002950: 5c6e 3c64 6574 6169 6c73 3e5c 6e20 2020  \n<details>\n   
-00002960: 203c 7375 6d6d 6172 793e 203c 623e 5573   <summary> <b>Us
-00002970: 6572 2047 726f 7570 733c 2f62 3e20 3c69  er Groups</b> <i
-00002980: 3e28 636c 6963 6b20 746f 2065 7870 616e  >(click to expan
-00002990: 6429 3c2f 693e 3c2f 7375 6d6d 6172 793e  d)</i></summary>
-000029a0: 5c6e 5c6e 6060 6070 7974 686f 6e5c 6e23  \n\n```python\n#
-000029b0: 2047 6574 2061 6c6c 2075 7365 7220 6772   Get all user gr
-000029c0: 6f75 7073 5c6e 7365 7373 696f 6e2e 6170  oups\nsession.ap
-000029d0: 692e 7573 6572 5f67 726f 7570 732e 6765  i.user_groups.ge
-000029e0: 7428 295c 6e5c 6e23 2043 7265 6174 6520  t()\n\n# Create 
-000029f0: 7573 6572 2067 726f 7570 5c6e 6772 6f75  user group\ngrou
-00002a00: 7020 3d20 5573 6572 4772 6f75 7028 226e  p = UserGroup("n
-00002a10: 6577 5f75 7365 725f 6772 6f75 7022 2c20  ew_user_group", 
-00002a20: 5b5d 295c 6e67 726f 7570 2e65 6e61 626c  [])\ngroup.enabl
-00002a30: 655f 7265 6164 287b 2241 7564 6974 204c  e_read({"Audit L
-00002a40: 6f67 222c 2022 416c 6172 6d73 227d 295c  og", "Alarms"})\
-00002a50: 6e67 726f 7570 2e65 6e61 626c 655f 7265  ngroup.enable_re
-00002a60: 6164 5f61 6e64 5f77 7269 7465 287b 2244  ad_and_write({"D
-00002a70: 6576 6963 6520 496e 7665 6e74 6f72 7922  evice Inventory"
-00002a80: 7d29 5c6e 7365 7373 696f 6e2e 6170 692e  })\nsession.api.
-00002a90: 7573 6572 5f67 726f 7570 732e 6372 6561  user_groups.crea
-00002aa0: 7465 2867 726f 7570 295c 6e5c 6e23 2055  te(group)\n\n# U
-00002ab0: 7064 6174 6520 7573 6572 2067 726f 7570  pdate user group
-00002ac0: 5c6e 6772 6f75 702e 6469 7361 626c 6528  \ngroup.disable(
-00002ad0: 7b22 416c 6172 6d73 227d 295c 6e73 6573  {"Alarms"})\nses
-00002ae0: 7369 6f6e 2e61 7069 2e75 7365 725f 6772  sion.api.user_gr
-00002af0: 6f75 7073 2e75 7064 6174 6528 6772 6f75  oups.update(grou
-00002b00: 7029 5c6e 5c6e 2320 4465 6c65 7465 2075  p)\n\n# Delete u
-00002b10: 7365 7220 6772 6f75 705c 6e73 6573 7369  ser group\nsessi
-00002b20: 6f6e 2e61 7069 2e75 7365 725f 6772 6f75  on.api.user_grou
-00002b30: 7073 2e64 656c 6574 6528 6772 6f75 702e  ps.delete(group.
-00002b40: 6772 6f75 705f 6e61 6d65 295c 6e60 6060  group_name)\n```
-00002b50: 5c6e 5c6e 3c2f 6465 7461 696c 733e 5c6e  \n\n</details>\n
-00002b60: 5c6e 3c2f 6465 7461 696c 733e 5c6e 5c6e  \n</details>\n\n
-00002b70: 3c64 6574 6169 6c73 3e5c 6e20 2020 203c  <details>\n    <
-00002b80: 7375 6d6d 6172 793e 203c 623e 5365 7373  summary> <b>Sess
-00002b90: 696f 6e73 3c2f 623e 203c 693e 2863 6c69  ions</b> <i>(cli
-00002ba0: 636b 2074 6f20 6578 7061 6e64 293c 2f69  ck to expand)</i
-00002bb0: 3e3c 2f73 756d 6d61 7279 3e5c 6e5c 6e60  ></summary>\n\n`
-00002bc0: 6060 7079 7468 6f6e 5c6e 2320 4765 7420  ``python\n# Get 
-00002bd0: 616c 6c20 6163 7469 7665 2073 6573 7369  all active sessi
-00002be0: 6f6e 735c 6e61 6374 6976 655f 7365 7373  ons\nactive_sess
-00002bf0: 696f 6e73 203d 2073 6573 7369 6f6e 2e61  ions = session.a
-00002c00: 7069 2e73 6573 7369 6f6e 732e 6765 7428  pi.sessions.get(
-00002c10: 295c 6e5c 6e23 2049 6e76 616c 6964 6174  )\n\n# Invalidat
-00002c20: 6520 7365 7373 696f 6e73 2066 6f72 2067  e sessions for g
-00002c30: 6976 656e 2075 7365 725c 6e6e 6577 5f75  iven user\nnew_u
-00002c40: 7365 725f 7365 7373 696f 6e73 203d 2061  ser_sessions = a
-00002c50: 6374 6976 655f 7365 7373 696f 6e73 2e66  ctive_sessions.f
-00002c60: 696c 7465 7228 7261 775f 7573 6572 6e61  ilter(raw_userna
-00002c70: 6d65 3d22 6e65 775f 7573 6572 2229 5c6e  me="new_user")\n
-00002c80: 7365 7373 696f 6e2e 6170 692e 7365 7373  session.api.sess
-00002c90: 696f 6e73 2e69 6e76 616c 6964 6174 6528  ions.invalidate(
-00002ca0: 6e65 775f 7573 6572 5f73 6573 7369 6f6e  new_user_session
-00002cb0: 7329 5c6e 6060 605c 6e5c 6e3c 2f64 6574  s)\n```\n\n</det
-00002cc0: 6169 6c73 3e5c 6e5c 6e3c 6465 7461 696c  ails>\n\n<detail
-00002cd0: 733e 5c6e 2020 2020 3c73 756d 6d61 7279  s>\n    <summary
-00002ce0: 3e20 3c62 3e52 6573 6f75 7263 6520 4772  > <b>Resource Gr
-00002cf0: 6f75 7073 3c2f 623e 203c 693e 2863 6c69  oups</b> <i>(cli
-00002d00: 636b 2074 6f20 6578 7061 6e64 293c 2f69  ck to expand)</i
-00002d10: 3e3c 2f73 756d 6d61 7279 3e5c 6e5c 6e60  ></summary>\n\n`
-00002d20: 6060 7079 7468 6f6e 5c6e 2320 6765 7420  ``python\n# get 
-00002d30: 7265 736f 7572 6365 2067 726f 7570 735c  resource groups\
-00002d40: 6e73 6573 7369 6f6e 2e61 7069 2e72 6573  nsession.api.res
-00002d50: 6f75 7263 655f 6772 6f75 7073 2e67 6574  ource_groups.get
-00002d60: 2829 5c6e 5c6e 2320 6372 6561 7465 2072  ()\n\n# create r
-00002d70: 6573 6f75 7263 6520 6772 6f75 705c 6e6e  esource group\nn
-00002d80: 6577 5f72 6573 6f75 7263 655f 6772 6f75  ew_resource_grou
-00002d90: 7020 3d20 5265 736f 7572 6365 4772 6f75  p = ResourceGrou
-00002da0: 7028 5c6e 2020 2020 6e61 6d65 3d22 6e65  p(\n    name="ne
-00002db0: 775f 7265 736f 7572 6365 5f67 726f 7570  w_resource_group
-00002dc0: 222c 5c6e 2020 2020 6465 7363 3d22 4375  ",\n    desc="Cu
-00002dd0: 7374 6f6d 2052 6573 6f75 7263 6520 4772  stom Resource Gr
-00002de0: 6f75 7020 2331 222c 5c6e 2020 2020 7369  oup #1",\n    si
-00002df0: 7465 4964 733d 5b5d 5c6e 295c 6e73 6573  teIds=[]\n)\nses
-00002e00: 7369 6f6e 2e61 7069 2e72 6573 6f75 7263  sion.api.resourc
-00002e10: 655f 6772 6f75 7073 2e63 7265 6174 6528  e_groups.create(
-00002e20: 6e65 775f 7265 736f 7572 6365 5f67 726f  new_resource_gro
-00002e30: 7570 295c 6e5c 6e23 2075 7064 6174 6520  up)\n\n# update 
-00002e40: 7265 736f 7572 6365 2067 726f 7570 5c6e  resource group\n
-00002e50: 7265 736f 7572 6365 5f67 726f 7570 203d  resource_group =
-00002e60: 2073 6573 7369 6f6e 2e61 7069 2e72 6573   session.api.res
-00002e70: 6f75 7263 655f 6772 6f75 7073 2e67 6574  ource_groups.get
-00002e80: 2829 2e66 696c 7465 7228 6e61 6d65 3d22  ().filter(name="
-00002e90: 6e65 775f 7265 736f 7572 6365 5f67 726f  new_resource_gro
-00002ea0: 7570 2229 2e73 696e 676c 655f 6f72 5f64  up").single_or_d
-00002eb0: 6566 6175 6c74 2829 5c6e 7570 6461 7465  efault()\nupdate
-00002ec0: 645f 7265 736f 7572 6365 5f67 726f 7570  d_resource_group
-00002ed0: 203d 2052 6573 6f75 7263 6547 726f 7570   = ResourceGroup
-00002ee0: 5570 6461 7465 5265 7175 6573 7428 5c6e  UpdateRequest(\n
-00002ef0: 2020 2020 6964 3d72 6573 6f75 7263 655f      id=resource_
-00002f00: 6772 6f75 702e 6964 2c5c 6e20 2020 206e  group.id,\n    n
-00002f10: 616d 653d 7265 736f 7572 6365 5f67 726f  ame=resource_gro
-00002f20: 7570 2e6e 616d 652c 5c6e 2020 2020 6465  up.name,\n    de
-00002f30: 7363 3d22 4375 7374 6f6d 2052 6573 6f75  sc="Custom Resou
-00002f40: 7263 6520 4772 6f75 7020 2331 2077 6974  rce Group #1 wit
-00002f50: 6820 7570 6461 7465 6420 6465 7363 7269  h updated descri
-00002f60: 7074 696f 6e20 616e 6420 7369 7465 2069  ption and site i
-00002f70: 6473 222c 5c6e 2020 2020 7369 7465 4964  ds",\n    siteId
-00002f80: 733d 5b32 3030 5d5c 6e29 5c6e 5c6e 2320  s=[200]\n)\n\n# 
-00002f90: 7377 6974 6368 2074 6f20 7265 736f 7572  switch to resour
-00002fa0: 6365 2067 726f 7570 2076 6965 775c 6e73  ce group view\ns
-00002fb0: 6573 7369 6f6e 2e61 7069 2e72 6573 6f75  ession.api.resou
-00002fc0: 7263 655f 6772 6f75 7073 2e73 7769 7463  rce_groups.switc
-00002fd0: 6828 226e 6577 5f72 6573 6f75 7263 655f  h("new_resource_
-00002fe0: 6772 6f75 7022 295c 6e5c 6e23 2064 656c  group")\n\n# del
-00002ff0: 6574 6520 7265 736f 7572 6365 2067 726f  ete resource gro
-00003000: 7570 5c6e 7365 7373 696f 6e2e 6170 692e  up\nsession.api.
-00003010: 7265 736f 7572 6365 5f67 726f 7570 732e  resource_groups.
-00003020: 6465 6c65 7465 2872 6573 6f75 7263 655f  delete(resource_
-00003030: 6772 6f75 702e 6964 295c 6e60 6060 5c6e  group.id)\n```\n
-00003040: 5c6e 3c2f 6465 7461 696c 733e 5c6e 5c6e  \n</details>\n\n
-00003050: 3c64 6574 6169 6c73 3e5c 6e20 2020 203c  <details>\n    <
-00003060: 7375 6d6d 6172 793e 203c 623e 5465 6e61  summary> <b>Tena
-00003070: 6e74 206d 616e 6167 656d 656e 743c 2f62  nt management</b
-00003080: 3e20 3c69 3e28 636c 6963 6b20 746f 2065  > <i>(click to e
-00003090: 7870 616e 6429 3c2f 693e 3c2f 7375 6d6d  xpand)</i></summ
-000030a0: 6172 793e 5c6e 5c6e 6060 6070 7974 686f  ary>\n\n```pytho
-000030b0: 6e5c 6e61 7069 203d 2073 6573 7369 6f6e  n\napi = session
-000030c0: 2e61 7069 2e74 656e 616e 745f 6d61 6e61  .api.tenant_mana
-000030d0: 6765 6d65 6e74 5c6e 2320 6372 6561 7465  gement\n# create
-000030e0: 2074 656e 616e 7473 5c6e 7465 6e61 6e74   tenants\ntenant
-000030f0: 7320 3d20 5b5c 6e20 2020 2054 656e 616e  s = [\n    Tenan
-00003100: 7428 5c6e 2020 2020 2020 2020 6e61 6d65  t(\n        name
-00003110: 3d22 7465 6e61 6e74 3122 2c5c 6e20 2020  ="tenant1",\n   
-00003120: 2020 2020 206f 7267 5f6e 616d 653d 2243       org_name="C
-00003130: 6973 636f 4465 764e 6574 222c 5c6e 2020  iscoDevNet",\n  
-00003140: 2020 2020 2020 7375 6264 6f6d 6169 6e3d        subdomain=
-00003150: 2261 6c70 6861 2e62 7261 766f 2e6e 6574  "alpha.bravo.net
-00003160: 222c 5c6e 2020 2020 2020 2020 6465 7363  ",\n        desc
-00003170: 3d22 5468 6973 2069 7320 7465 6e61 6e74  ="This is tenant
-00003180: 2066 6f72 2075 6e69 7420 7465 7374 7322   for unit tests"
-00003190: 2c5c 6e20 2020 2020 2020 2065 6467 655f  ,\n        edge_
-000031a0: 636f 6e6e 6563 746f 725f 656e 6162 6c65  connector_enable
-000031b0: 3d54 7275 652c 5c6e 2020 2020 2020 2020  =True,\n        
-000031c0: 6564 6765 5f63 6f6e 6e65 6374 6f72 5f73  edge_connector_s
-000031d0: 7973 7465 6d5f 6970 3d22 3137 322e 3136  ystem_ip="172.16
-000031e0: 2e32 3535 2e38 3122 2c5c 6e20 2020 2020  .255.81",\n     
-000031f0: 2020 2065 6467 655f 636f 6e6e 6563 746f     edge_connecto
-00003200: 725f 7475 6e6e 656c 5f69 6e74 6572 6661  r_tunnel_interfa
-00003210: 6365 5f6e 616d 653d 2247 6967 6162 6974  ce_name="Gigabit
-00003220: 4574 6865 726e 6574 3122 2c5c 6e20 2020  Ethernet1",\n   
-00003230: 2020 2020 2077 616e 5f65 6467 655f 666f       wan_edge_fo
-00003240: 7265 6361 7374 3d31 2c5c 6e20 2020 2029  recast=1,\n    )
-00003250: 5c6e 5d5c 6e63 7265 6174 655f 7461 736b  \n]\ncreate_task
-00003260: 203d 2061 7069 2e63 7265 6174 6528 7465   = api.create(te
-00003270: 6e61 6e74 7329 5c6e 6372 6561 7465 5f74  nants)\ncreate_t
-00003280: 6173 6b2e 7761 6974 5f66 6f72 5f63 6f6d  ask.wait_for_com
-00003290: 706c 6574 6564 2829 5c6e 2320 6c69 7374  pleted()\n# list
-000032a0: 2061 6c6c 2074 656e 616e 7473 5c6e 7465   all tenants\nte
-000032b0: 6e61 6e74 735f 6461 7461 203d 2061 7069  nants_data = api
-000032c0: 2e67 6574 5f61 6c6c 2829 5c6e 2320 7069  .get_all()\n# pi
-000032d0: 636b 2074 656e 616e 7420 6672 6f6d 206c  ck tenant from l
-000032e0: 6973 7420 6279 206e 616d 655c 6e74 656e  ist by name\nten
-000032f0: 616e 7420 3d20 7465 6e61 6e74 735f 6461  ant = tenants_da
-00003300: 7461 2e66 696c 7465 7228 6e61 6d65 3d22  ta.filter(name="
-00003310: 7465 6e61 6e74 3122 292e 7369 6e67 6c65  tenant1").single
-00003320: 5f6f 725f 6465 6661 756c 7428 295c 6e23  _or_default()\n#
-00003330: 2067 6574 2073 656c 6563 7465 6420 7465   get selected te
-00003340: 6e61 6e74 2069 645c 6e74 656e 616e 745f  nant id\ntenant_
-00003350: 6964 203d 2074 656e 616e 742e 7465 6e61  id = tenant.tena
-00003360: 6e74 5f69 645c 6e23 2067 6574 2076 7365  nt_id\n# get vse
-00003370: 7373 696f 6e20 6964 206f 6620 7365 6c65  ssion id of sele
-00003380: 6374 6564 2074 656e 616e 745c 6e76 7365  cted tenant\nvse
-00003390: 7373 696f 6e69 6420 3d20 6170 692e 7673  ssionid = api.vs
-000033a0: 6573 7369 6f6e 5f69 6428 7465 6e61 6e74  ession_id(tenant
-000033b0: 5f69 6429 5c6e 2320 6465 6c65 7465 2074  _id)\n# delete t
-000033c0: 656e 616e 7420 6279 2069 6473 5c6e 6465  enant by ids\nde
-000033d0: 6c65 7465 5f74 6173 6b20 3d20 6170 692e  lete_task = api.
-000033e0: 6465 6c65 7465 285b 7465 6e61 6e74 5f69  delete([tenant_i
-000033f0: 645d 295c 6e64 656c 6574 655f 7461 736b  d])\ndelete_task
-00003400: 2e77 6169 745f 666f 725f 636f 6d70 6c65  .wait_for_comple
-00003410: 7465 6428 295c 6e23 206f 7468 6572 735c  ted()\n# others\
-00003420: 6e61 7069 2e67 6574 5f68 6f73 7469 6e67  napi.get_hosting
-00003430: 5f63 6170 6163 6974 795f 6f6e 5f76 736d  _capacity_on_vsm
-00003440: 6172 7473 2829 5c6e 6170 692e 6765 745f  arts()\napi.get_
-00003450: 7374 6174 7573 6573 2829 5c6e 6170 692e  statuses()\napi.
-00003460: 6765 745f 7673 6d61 7274 5f6d 6170 7069  get_vsmart_mappi
-00003470: 6e67 2829 5c6e 6060 605c 6e3c 2f64 6574  ng()\n```\n</det
-00003480: 6169 6c73 3e5c 6e5c 6e3c 6465 7461 696c  ails>\n\n<detail
-00003490: 733e 5c6e 2020 2020 3c73 756d 6d61 7279  s>\n    <summary
-000034a0: 3e20 3c62 3e54 656e 616e 7420 6d69 6772  > <b>Tenant migr
-000034b0: 6174 696f 6e3c 2f62 3e20 3c69 3e28 636c  ation</b> <i>(cl
-000034c0: 6963 6b20 746f 2065 7870 616e 6429 3c2f  ick to expand)</
-000034d0: 693e 3c2f 7375 6d6d 6172 793e 5c6e 5c6e  i></summary>\n\n
-000034e0: 6060 6070 7974 686f 6e5c 6e66 726f 6d20  ```python\nfrom 
-000034f0: 7061 7468 6c69 6220 696d 706f 7274 2050  pathlib import P
-00003500: 6174 685c 6e66 726f 6d20 6361 7461 6c79  ath\nfrom cataly
-00003510: 7374 7761 6e2e 7365 7373 696f 6e20 696d  stwan.session im
-00003520: 706f 7274 2063 7265 6174 655f 6d61 6e61  port create_mana
-00003530: 6765 725f 7365 7373 696f 6e5c 6e66 726f  ger_session\nfro
-00003540: 6d20 6361 7461 6c79 7374 7761 6e2e 6d6f  m catalystwan.mo
-00003550: 6465 6c73 2e74 656e 616e 7420 696d 706f  dels.tenant impo
-00003560: 7274 2054 656e 616e 7445 7870 6f72 745c  rt TenantExport\
-00003570: 6e66 726f 6d20 6361 7461 6c79 7374 7761  nfrom catalystwa
-00003580: 6e2e 776f 726b 666c 6f77 732e 7465 6e61  n.workflows.tena
-00003590: 6e74 5f6d 6967 7261 7469 6f6e 2069 6d70  nt_migration imp
-000035a0: 6f72 7420 6d69 6772 6174 696f 6e5f 776f  ort migration_wo
-000035b0: 726b 666c 6f77 5c6e 5c6e 7465 6e61 6e74  rkflow\n\ntenant
-000035c0: 203d 2054 656e 616e 7445 7870 6f72 7428   = TenantExport(
-000035d0: 5c6e 2020 2020 6e61 6d65 3d22 6d61 6e67  \n    name="mang
-000035e0: 6f22 2c5c 6e20 2020 2064 6573 633d 224d  o",\n    desc="M
-000035f0: 616e 676f 2074 656e 616e 7420 6465 7363  ango tenant desc
-00003600: 7269 7074 696f 6e22 2c5c 6e20 2020 206f  ription",\n    o
-00003610: 7267 5f6e 616d 653d 2250 726f 7669 6465  rg_name="Provide
-00003620: 7220 4f72 672d 4d61 6e67 6f20 496e 6322  r Org-Mango Inc"
-00003630: 2c5c 6e20 2020 2073 7562 646f 6d61 696e  ,\n    subdomain
-00003640: 3d22 6d61 6e67 6f2e 6672 7569 7473 2e63  ="mango.fruits.c
-00003650: 6f6d 222c 5c6e 2020 2020 7761 6e5f 6564  om",\n    wan_ed
-00003660: 6765 5f66 6f72 6563 6173 743d 3130 302c  ge_forecast=100,
-00003670: 5c6e 2020 2020 6d69 6772 6174 696f 6e5f  \n    migration_
-00003680: 6b65 793d 224d 616e 676f 5465 6e61 6e74  key="MangoTenant
-00003690: 4d69 6772 6174 696f 6e4b 6579 222c 2020  MigrationKey",  
-000036a0: 2023 206f 6e6c 7920 666f 7220 5344 5741   # only for SDWA
-000036b0: 4e20 4d61 6e61 6765 7220 3e3d 2032 302e  N Manager >= 20.
-000036c0: 3133 5c6e 2020 2020 6973 5f64 6573 7469  13\n    is_desti
-000036d0: 6e61 7469 6f6e 5f6f 7665 726c 6179 5f6d  nation_overlay_m
-000036e0: 743d 5472 7565 2c20 2020 2020 2020 2020  t=True,         
-000036f0: 2020 2023 206f 6e6c 7920 666f 7220 5344     # only for SD
-00003700: 5741 4e20 4d61 6e61 6765 7220 3e3d 2032  WAN Manager >= 2
-00003710: 302e 3133 5c6e 295c 6e5c 6e77 6974 6820  0.13\n)\n\nwith 
-00003720: 6372 6561 7465 5f6d 616e 6167 6572 5f73  create_manager_s
-00003730: 6573 7369 6f6e 2875 726c 3d22 3130 2e30  ession(url="10.0
-00003740: 2e31 2e31 3522 2c20 7573 6572 6e61 6d65  .1.15", username
-00003750: 3d22 7374 2d61 646d 696e 222c 2070 6173  ="st-admin", pas
-00003760: 7377 6f72 643d 2222 2920 6173 206f 7269  sword="") as ori
-00003770: 6769 6e5f 7365 7373 696f 6e2c 205c 5c5c  gin_session, \\\
-00003780: 6e20 2020 2020 6372 6561 7465 5f6d 616e  n     create_man
-00003790: 6167 6572 5f73 6573 7369 6f6e 2875 726c  ager_session(url
-000037a0: 3d22 3130 2e39 2e30 2e31 3622 2c20 7573  ="10.9.0.16", us
-000037b0: 6572 6e61 6d65 3d22 6d74 2d70 726f 7669  ername="mt-provi
-000037c0: 6465 722d 6164 6d69 6e22 2c20 7061 7373  der-admin", pass
-000037d0: 776f 7264 3d22 2229 2061 7320 7461 7267  word="") as targ
-000037e0: 6574 5f73 6573 7369 6f6e 3a5c 6e20 2020  et_session:\n   
-000037f0: 206d 6967 7261 7469 6f6e 5f77 6f72 6b66   migration_workf
-00003800: 6c6f 7728 5c6e 2020 2020 2020 2020 6f72  low(\n        or
-00003810: 6967 696e 5f73 6573 7369 6f6e 3d6f 7269  igin_session=ori
-00003820: 6769 6e5f 7365 7373 696f 6e2c 5c6e 2020  gin_session,\n  
-00003830: 2020 2020 2020 7461 7267 6574 5f73 6573        target_ses
-00003840: 7369 6f6e 3d74 6172 6765 745f 7365 7373  sion=target_sess
-00003850: 696f 6e2c 5c6e 2020 2020 2020 2020 776f  ion,\n        wo
-00003860: 726b 6469 723d 5061 7468 2822 776f 726b  rkdir=Path("work
-00003870: 6469 7222 292c 5c6e 2020 2020 2020 2020  dir"),\n        
-00003880: 7465 6e61 6e74 3d74 656e 616e 742c 5c6e  tenant=tenant,\n
-00003890: 2020 2020 2020 2020 7661 6c69 6461 746f          validato
-000038a0: 723d 2231 302e 392e 3132 2e32 3622 5c6e  r="10.9.12.26"\n
-000038b0: 2020 2020 295c 6e60 6060 5c6e 5c6e 606d      )\n```\n\n`m
-000038c0: 6967 7261 7469 6f6e 5f77 6f72 6b66 6c6f  igration_workflo
-000038d0: 7760 2070 6572 666f 726d 7320 6d75 6c74  w` performs mult
-000038e0: 692d 7374 6570 206d 6967 7261 7469 6f6e  i-step migration
-000038f0: 2070 726f 6365 6475 7265 2061 6363 6f72   procedure accor
-00003900: 6469 6e67 2074 6f20 5b4d 6967 7261 7465  ding to [Migrate
-00003910: 2053 696e 676c 652d 5465 6e61 6e74 2043   Single-Tenant C
-00003920: 6973 636f 2053 442d 5741 4e20 4f76 6572  isco SD-WAN Over
-00003930: 6c61 7920 746f 204d 756c 7469 7465 6e61  lay to Multitena
-00003940: 6e74 2043 6973 636f 2053 442d 5741 4e20  nt Cisco SD-WAN 
-00003950: 4465 706c 6f79 6d65 6e74 5d28 6874 7470  Deployment](http
-00003960: 733a 2f2f 7777 772e 6369 7363 6f2e 636f  s://www.cisco.co
-00003970: 6d2f 632f 656e 2f75 732f 7464 2f64 6f63  m/c/en/us/td/doc
-00003980: 732f 726f 7574 6572 732f 7364 7761 6e2f  s/routers/sdwan/
-00003990: 636f 6e66 6967 7572 6174 696f 6e2f 7379  configuration/sy
-000039a0: 7374 656d 2d69 6e74 6572 6661 6365 2f76  stem-interface/v
-000039b0: 6564 6765 2d32 302d 782f 7379 7374 656d  edge-20-x/system
-000039c0: 732d 696e 7465 7266 6163 6573 2d62 6f6f  s-interfaces-boo
-000039d0: 6b2f 7364 7761 6e2d 6d75 6c74 6974 656e  k/sdwan-multiten
-000039e0: 616e 6379 2e68 746d 6c23 636f 6e63 6570  ancy.html#concep
-000039f0: 745f 736a 6a5f 6a6d 6d5f 7a34 6229 5c6e  t_sjj_jmm_z4b)\n
-00003a00: 5c6e 5c6e 5369 6e63 6520 3230 2e31 3320  \n\nSince 20.13 
-00003a10: 616c 736f 204d 5420 746f 2053 5420 6973  also MT to ST is
-00003a20: 2073 7570 706f 7274 6564 2028 6a75 7374   supported (just
-00003a30: 2070 726f 7669 6465 2073 7569 7461 626c   provide suitabl
-00003a40: 6520 6f72 6967 696e 2f74 6172 6765 7420  e origin/target 
-00003a50: 7365 7373 696f 6e73 2c20 616e 6420 6069  sessions, and `i
-00003a60: 735f 6465 7374 696e 6174 696f 6e5f 6f76  s_destination_ov
-00003a70: 6572 6c61 795f 6d74 6020 7061 7261 6d65  erlay_mt` parame
-00003a80: 7465 7229 5c6e 5c6e 5c6e 4561 6368 2073  ter)\n\n\nEach s
-00003a90: 7465 7020 6f66 2074 6865 2060 6d69 6772  tep of the `migr
-00003aa0: 6174 696f 6e5f 776f 726b 666c 6f77 6020  ation_workflow` 
-00003ab0: 7072 6f63 6564 7572 6520 6361 6e20 6265  procedure can be
-00003ac0: 2065 7865 6375 7465 6420 696e 6465 7065   executed indepe
-00003ad0: 6e64 656e 746c 7920 7573 696e 6720 6170  ndently using ap
-00003ae0: 6920 6d65 7468 6f64 733a 2060 6578 706f  i methods: `expo
-00003af0: 7274 5f74 656e 616e 7460 2c20 6064 6f77  rt_tenant`, `dow
-00003b00: 6e6c 6f61 6460 2c20 6069 6d70 6f72 745f  nload`, `import_
-00003b10: 7465 6e61 6e74 602c 2060 7374 6f72 655f  tenant`, `store_
-00003b20: 746f 6b65 6e60 2c20 606d 6967 7261 7465  token`, `migrate
-00003b30: 5f6e 6574 776f 726b 605c 6e5c 6e60 6060  _network`\n\n```
-00003b40: 7079 7468 6f6e 5c6e 6f72 6967 696e 5f61  python\norigin_a
-00003b50: 7069 203d 206f 7269 6769 6e5f 7365 7373  pi = origin_sess
-00003b60: 696f 6e2e 6170 692e 7465 6e61 6e74 5f6d  ion.api.tenant_m
-00003b70: 6967 7261 7469 6f6e 5f61 7069 5c6e 7461  igration_api\nta
-00003b80: 7267 6574 5f61 7069 203d 2074 6172 6765  rget_api = targe
-00003b90: 745f 7365 7373 696f 6e2e 6170 692e 7465  t_session.api.te
-00003ba0: 6e61 6e74 5f6d 6967 7261 7469 6f6e 5f61  nant_migration_a
-00003bb0: 7069 5c6e 7465 6e61 6e74 5f66 696c 6520  pi\ntenant_file 
-00003bc0: 3d20 5061 7468 2822 7e2f 7465 6e61 6e74  = Path("~/tenant
-00003bd0: 2e74 6172 2e67 7a22 295c 6e74 6f6b 656e  .tar.gz")\ntoken
-00003be0: 5f66 696c 6520 3d20 5061 7468 2822 7e2f  _file = Path("~/
-00003bf0: 7465 6e61 6e74 2d74 6f6b 656e 2e74 7874  tenant-token.txt
-00003c00: 2229 5c6e 2320 6578 706f 7274 5c6e 6578  ")\n# export\nex
-00003c10: 706f 7274 5f74 6173 6b20 3d20 6f72 6967  port_task = orig
-00003c20: 696e 5f61 7069 2e65 7870 6f72 745f 7465  in_api.export_te
-00003c30: 6e61 6e74 2874 656e 616e 743d 7465 6e61  nant(tenant=tena
-00003c40: 6e74 295c 6e72 656d 6f74 655f 6669 6c65  nt)\nremote_file
-00003c50: 6e61 6d65 203d 2065 7870 6f72 745f 7461  name = export_ta
-00003c60: 736b 2e77 6169 745f 666f 725f 6669 6c65  sk.wait_for_file
-00003c70: 2829 5c6e 2320 646f 776e 6c6f 6164 5c6e  ()\n# download\n
-00003c80: 6f72 6967 696e 5f61 7069 2e64 6f77 6e6c  origin_api.downl
-00003c90: 6f61 6428 6578 706f 7274 5f70 6174 682c  oad(export_path,
-00003ca0: 2072 656d 6f74 655f 6669 6c65 6e61 6d65   remote_filename
-00003cb0: 295c 6e23 2069 6d70 6f72 745c 6e69 6d70  )\n# import\nimp
-00003cc0: 6f72 745f 7461 736b 203d 2074 6172 6765  ort_task = targe
-00003cd0: 745f 6170 692e 696d 706f 7274 5f74 656e  t_api.import_ten
-00003ce0: 616e 7428 6578 706f 7274 5f70 6174 682c  ant(export_path,
-00003cf0: 2074 656e 616e 742e 6d69 6772 6174 696f   tenant.migratio
-00003d00: 6e5f 6b65 7929 5c6e 696d 706f 7274 5f74  n_key)\nimport_t
-00003d10: 6173 6b2e 7761 6974 5f66 6f72 5f63 6f6d  ask.wait_for_com
-00003d20: 706c 6574 6564 2829 5c6e 2320 6765 7420  pleted()\n# get 
-00003d30: 746f 6b65 6e5c 6e6d 6967 7261 7469 6f6e  token\nmigration
-00003d40: 5f69 6420 3d20 696d 706f 7274 5f74 6173  _id = import_tas
-00003d50: 6b2e 696d 706f 7274 5f69 6e66 6f2e 6d69  k.import_info.mi
-00003d60: 6772 6174 696f 6e5f 746f 6b65 6e5f 7175  gration_token_qu
-00003d70: 6572 795f 7061 7261 6d73 2e6d 6967 7261  ery_params.migra
-00003d80: 7469 6f6e 5f69 645c 6e74 6172 6765 745f  tion_id\ntarget_
-00003d90: 6170 692e 7374 6f72 655f 746f 6b65 6e28  api.store_token(
-00003da0: 6d69 6772 6174 696f 6e5f 6964 2c20 746f  migration_id, to
-00003db0: 6b65 6e5f 7061 7468 295c 6e23 206d 6967  ken_path)\n# mig
-00003dc0: 7261 7465 206e 6574 776f 726b 5c6e 6d69  rate network\nmi
-00003dd0: 6772 6174 655f 7461 736b 203d 206f 7269  grate_task = ori
-00003de0: 6769 6e5f 6170 692e 6d69 6772 6174 655f  gin_api.migrate_
-00003df0: 6e65 7477 6f72 6b28 746f 6b65 6e5f 7061  network(token_pa
-00003e00: 7468 295c 6e6d 6967 7261 7465 5f74 6173  th)\nmigrate_tas
-00003e10: 6b2e 7761 6974 5f66 6f72 5f63 6f6d 706c  k.wait_for_compl
-00003e20: 6574 6564 2829 5c6e 6060 605c 6e3c 2f64  eted()\n```\n</d
-00003e30: 6574 6169 6c73 3e5c 6e5c 6e23 2323 204e  etails>\n\n### N
-00003e40: 6f74 653a 5c6e 546f 2072 656d 6f76 6520  ote:\nTo remove 
-00003e50: 6049 6e73 6563 7572 6552 6571 7565 7374  `InsecureRequest
-00003e60: 5761 726e 696e 6760 2c20 796f 7520 6361  Warning`, you ca
-00003e70: 6e20 696e 636c 7564 6520 696e 2079 6f75  n include in you
-00003e80: 7220 7363 7269 7074 7320 2877 6172 6e69  r scripts (warni
-00003e90: 6e67 2069 7320 7375 7070 7265 7373 6564  ng is suppressed
-00003ea0: 2077 6865 6e20 6063 6174 616c 7973 7477   when `catalystw
-00003eb0: 616e 5f64 6576 656c 6020 656e 7669 726f  an_devel` enviro
-00003ec0: 6e6d 656e 7420 7661 7269 6162 6c65 2069  nment variable i
-00003ed0: 7320 7365 7429 3a5c 6e60 6060 5079 7468  s set):\n```Pyth
-00003ee0: 6f6e 5c6e 696d 706f 7274 2075 726c 6c69  on\nimport urlli
-00003ef0: 6233 5c6e 7572 6c6c 6962 332e 6469 7361  b3\nurllib3.disa
-00003f00: 626c 655f 7761 726e 696e 6773 2875 726c  ble_warnings(url
-00003f10: 6c69 6233 2e65 7863 6570 7469 6f6e 732e  lib3.exceptions.
-00003f20: 496e 7365 6375 7265 5265 7175 6573 7457  InsecureRequestW
-00003f30: 6172 6e69 6e67 295c 6e60 6060 5c6e 5c6e  arning)\n```\n\n
-00003f40: 2323 2043 6174 6368 696e 6720 4578 6365  ## Catching Exce
-00003f50: 7074 696f 6e73 5c6e 6060 6070 7974 686f  ptions\n```pytho
-00003f60: 6e5c 6e74 7279 3a5c 6e20 2020 2073 6573  n\ntry:\n    ses
-00003f70: 7369 6f6e 2e61 7069 2e75 7365 7273 2e64  sion.api.users.d
-00003f80: 656c 6574 6528 2262 6f67 7573 2d75 7365  elete("bogus-use
-00003f90: 722d 6e61 6d65 2229 5c6e 6578 6365 7074  r-name")\nexcept
-00003fa0: 204d 616e 6167 6572 4854 5450 4572 726f   ManagerHTTPErro
-00003fb0: 7220 6173 2065 7272 6f72 3a5c 6e20 2020  r as error:\n   
-00003fc0: 2023 2050 726f 6365 7373 2061 6e20 6572   # Process an er
-00003fd0: 726f 722e 5c6e 2020 2020 7072 696e 7428  ror.\n    print(
-00003fe0: 6572 726f 722e 7265 7370 6f6e 7365 2e73  error.response.s
-00003ff0: 7461 7475 735f 636f 6465 295c 6e20 2020  tatus_code)\n   
-00004000: 2070 7269 6e74 2865 7272 6f72 2e69 6e66   print(error.inf
-00004010: 6f2e 636f 6465 295c 6e20 2020 2070 7269  o.code)\n    pri
-00004020: 6e74 2865 7272 6f72 2e69 6e66 6f2e 6d65  nt(error.info.me
-00004030: 7373 6167 6529 5c6e 2020 2020 7072 696e  ssage)\n    prin
-00004040: 7428 6572 726f 722e 696e 666f 2e64 6574  t(error.info.det
-00004050: 6169 6c73 295c 6e5c 6e60 6060 5c6e 5c6e  ails)\n\n```\n\n
-00004060: 2323 205b 5375 7070 6f72 7465 6420 4150  ## [Supported AP
-00004070: 4920 656e 6470 6f69 6e74 735d 2868 7474  I endpoints](htt
-00004080: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00004090: 6369 7363 6f2d 6f70 656e 2f63 6973 636f  cisco-open/cisco
-000040a0: 2d63 6174 616c 7973 742d 7761 6e2d 7364  -catalyst-wan-sd
-000040b0: 6b2f 626c 6f62 2f6d 6169 6e2f 454e 4450  k/blob/main/ENDP
-000040c0: 4f49 4e54 532e 6d64 295c 6e5c 6e5c 6e23  OINTS.md)\n\n\n#
-000040d0: 2320 5b43 6f6e 7472 6962 7574 696e 672c  # [Contributing,
-000040e0: 2062 7567 2072 6570 6f72 7469 6e67 2061   bug reporting a
-000040f0: 6e64 2066 6561 7475 7265 2072 6571 7565  nd feature reque
-00004100: 7374 735d 2868 7474 7073 3a2f 2f67 6974  sts](https://git
-00004110: 6875 622e 636f 6d2f 6369 7363 6f2d 6f70  hub.com/cisco-op
-00004120: 656e 2f63 6973 636f 2d63 6174 616c 7973  en/cisco-catalys
-00004130: 742d 7761 6e2d 7364 6b2f 626c 6f62 2f6d  t-wan-sdk/blob/m
-00004140: 6169 6e2f 434f 4e54 5249 4255 5449 4e47  ain/CONTRIBUTING
-00004150: 2e6d 6429 5c6e 5c6e 2323 2053 6565 6b69  .md)\n\n## Seeki
-00004160: 6e67 2073 7570 706f 7274 5c6e 5c6e 596f  ng support\n\nYo
-00004170: 7520 6361 6e20 636f 6e74 6163 7420 7573  u can contact us
-00004180: 2062 7920 7375 626d 6974 7469 6e67 205b   by submitting [
-00004190: 6973 7375 6573 5d28 6874 7470 733a 2f2f  issues](https://
-000041a0: 6769 7468 7562 2e63 6f6d 2f63 6973 636f  github.com/cisco
-000041b0: 2d6f 7065 6e2f 6369 7363 6f2d 6361 7461  -open/cisco-cata
-000041c0: 6c79 7374 2d77 616e 2d73 646b 2f69 7373  lyst-wan-sdk/iss
-000041d0: 7565 7329 2c20 6f72 2064 6972 6563 746c  ues), or directl
-000041e0: 7920 7669 6120 6d61 696c 206f 6e20 6361  y via mail on ca
-000041f0: 7461 6c79 7374 7761 6e40 6369 7363 6f2e  talystwan@cisco.
-00004200: 636f 6d2e 5c6e 272c 0a20 2020 2027 6175  com.\n',.    'au
-00004210: 7468 6f72 273a 2027 6b61 676f 7273 6b69  thor': 'kagorski
-00004220: 272c 0a20 2020 2027 6175 7468 6f72 5f65  ',.    'author_e
-00004230: 6d61 696c 273a 2027 6b61 676f 7273 6b69  mail': 'kagorski
-00004240: 4063 6973 636f 2e63 6f6d 272c 0a20 2020  @cisco.com',.   
-00004250: 2027 6d61 696e 7461 696e 6572 273a 2027   'maintainer': '
-00004260: 4e6f 6e65 272c 0a20 2020 2027 6d61 696e  None',.    'main
-00004270: 7461 696e 6572 5f65 6d61 696c 273a 2027  tainer_email': '
-00004280: 4e6f 6e65 272c 0a20 2020 2027 7572 6c27  None',.    'url'
-00004290: 3a20 2768 7474 7073 3a2f 2f67 6974 6875  : 'https://githu
-000042a0: 622e 636f 6d2f 6369 7363 6f2d 6f70 656e  b.com/cisco-open
-000042b0: 2f63 6973 636f 2d63 6174 616c 7973 742d  /cisco-catalyst-
-000042c0: 7761 6e2d 7364 6b27 2c0a 2020 2020 2770  wan-sdk',.    'p
-000042d0: 6163 6b61 6765 7327 3a20 7061 636b 6167  ackages': packag
-000042e0: 6573 2c0a 2020 2020 2770 6163 6b61 6765  es,.    'package
-000042f0: 5f64 6174 6127 3a20 7061 636b 6167 655f  _data': package_
-00004300: 6461 7461 2c0a 2020 2020 2769 6e73 7461  data,.    'insta
-00004310: 6c6c 5f72 6571 7569 7265 7327 3a20 696e  ll_requires': in
-00004320: 7374 616c 6c5f 7265 7175 6972 6573 2c0a  stall_requires,.
-00004330: 2020 2020 2770 7974 686f 6e5f 7265 7175      'python_requ
-00004340: 6972 6573 273a 2027 3e3d 332e 382e 302c  ires': '>=3.8.0,
-00004350: 3c34 2e30 2e30 272c 0a7d 0a0a 0a73 6574  <4.0.0',.}...set
-00004360: 7570 282a 2a73 6574 7570 5f6b 7761 7267  up(**setup_kwarg
-00004370: 7329 0a                                  s).
+00000070: 7477 616e 2e61 7069 2e62 7569 6c64 6572  twan.api.builder
+00000080: 7327 2c0a 2027 6361 7461 6c79 7374 7761  s',. 'catalystwa
+00000090: 6e2e 6170 692e 6275 696c 6465 7273 2e66  n.api.builders.f
+000000a0: 6561 7475 7265 5f70 726f 6669 6c65 7327  eature_profiles'
+000000b0: 2c0a 2027 6361 7461 6c79 7374 7761 6e2e  ,. 'catalystwan.
+000000c0: 6170 692e 636f 6e66 6967 7572 6174 696f  api.configuratio
+000000d0: 6e5f 6772 6f75 7073 272c 0a20 2763 6174  n_groups',. 'cat
+000000e0: 616c 7973 7477 616e 2e61 7069 2e74 656d  alystwan.api.tem
+000000f0: 706c 6174 6573 272c 0a20 2763 6174 616c  plates',. 'catal
+00000100: 7973 7477 616e 2e61 7069 2e74 656d 706c  ystwan.api.templ
+00000110: 6174 6573 2e64 6576 6963 655f 7465 6d70  ates.device_temp
+00000120: 6c61 7465 272c 0a20 2763 6174 616c 7973  late',. 'catalys
+00000130: 7477 616e 2e61 7069 2e74 656d 706c 6174  twan.api.templat
+00000140: 6573 2e6d 6f64 656c 7327 2c0a 2027 6361  es.models',. 'ca
+00000150: 7461 6c79 7374 7761 6e2e 6170 692e 7465  talystwan.api.te
+00000160: 6d70 6c61 7465 732e 7061 796c 6f61 6473  mplates.payloads
+00000170: 2e61 6161 272c 0a20 2763 6174 616c 7973  .aaa',. 'catalys
+00000180: 7477 616e 2e61 7069 2e74 656d 706c 6174  twan.api.templat
+00000190: 6573 2e70 6179 6c6f 6164 732e 6369 7363  es.payloads.cisc
+000001a0: 6f5f 7670 6e27 2c0a 2027 6361 7461 6c79  o_vpn',. 'cataly
+000001b0: 7374 7761 6e2e 6170 692e 7465 6d70 6c61  stwan.api.templa
+000001c0: 7465 732e 7061 796c 6f61 6473 2e74 656e  tes.payloads.ten
+000001d0: 616e 7427 2c0a 2027 6361 7461 6c79 7374  ant',. 'catalyst
+000001e0: 7761 6e2e 656e 6470 6f69 6e74 7327 2c0a  wan.endpoints',.
+000001f0: 2027 6361 7461 6c79 7374 7761 6e2e 656e   'catalystwan.en
+00000200: 6470 6f69 6e74 732e 636f 6e66 6967 7572  dpoints.configur
+00000210: 6174 696f 6e27 2c0a 2027 6361 7461 6c79  ation',. 'cataly
+00000220: 7374 7761 6e2e 656e 6470 6f69 6e74 732e  stwan.endpoints.
+00000230: 636f 6e66 6967 7572 6174 696f 6e2e 6465  configuration.de
+00000240: 7669 6365 272c 0a20 2763 6174 616c 7973  vice',. 'catalys
+00000250: 7477 616e 2e65 6e64 706f 696e 7473 2e63  twan.endpoints.c
+00000260: 6f6e 6669 6775 7261 7469 6f6e 2e66 6561  onfiguration.fea
+00000270: 7475 7265 5f70 726f 6669 6c65 2e73 6477  ture_profile.sdw
+00000280: 616e 272c 0a20 2763 6174 616c 7973 7477  an',. 'catalystw
+00000290: 616e 2e65 6e64 706f 696e 7473 2e63 6f6e  an.endpoints.con
+000002a0: 6669 6775 7261 7469 6f6e 2e70 6f6c 6963  figuration.polic
+000002b0: 7927 2c0a 2027 6361 7461 6c79 7374 7761  y',. 'catalystwa
+000002c0: 6e2e 656e 6470 6f69 6e74 732e 636f 6e66  n.endpoints.conf
+000002d0: 6967 7572 6174 696f 6e2e 706f 6c69 6379  iguration.policy
+000002e0: 2e64 6566 696e 6974 696f 6e27 2c0a 2027  .definition',. '
+000002f0: 6361 7461 6c79 7374 7761 6e2e 656e 6470  catalystwan.endp
+00000300: 6f69 6e74 732e 636f 6e66 6967 7572 6174  oints.configurat
+00000310: 696f 6e2e 706f 6c69 6379 2e6c 6973 7427  ion.policy.list'
+00000320: 2c0a 2027 6361 7461 6c79 7374 7761 6e2e  ,. 'catalystwan.
+00000330: 656e 6470 6f69 6e74 732e 6d6f 6e69 746f  endpoints.monito
+00000340: 7269 6e67 272c 0a20 2763 6174 616c 7973  ring',. 'catalys
+00000350: 7477 616e 2e65 6e64 706f 696e 7473 2e72  twan.endpoints.r
+00000360: 6561 6c5f 7469 6d65 5f6d 6f6e 6974 6f72  eal_time_monitor
+00000370: 696e 6727 2c0a 2027 6361 7461 6c79 7374  ing',. 'catalyst
+00000380: 7761 6e2e 656e 6470 6f69 6e74 732e 7472  wan.endpoints.tr
+00000390: 6f75 626c 6573 686f 6f74 696e 675f 746f  oubleshooting_to
+000003a0: 6f6c 7327 2c0a 2027 6361 7461 6c79 7374  ols',. 'catalyst
+000003b0: 7761 6e2e 696e 7465 6772 6174 696f 6e5f  wan.integration_
+000003c0: 7465 7374 7327 2c0a 2027 6361 7461 6c79  tests',. 'cataly
+000003d0: 7374 7761 6e2e 696e 7465 6772 6174 696f  stwan.integratio
+000003e0: 6e5f 7465 7374 732e 6665 6174 7572 655f  n_tests.feature_
+000003f0: 7072 6f66 696c 652e 7364 7761 6e27 2c0a  profile.sdwan',.
+00000400: 2027 6361 7461 6c79 7374 7761 6e2e 696e   'catalystwan.in
+00000410: 7465 6772 6174 696f 6e5f 7465 7374 732e  tegration_tests.
+00000420: 6665 6174 7572 655f 7072 6f66 696c 652e  feature_profile.
+00000430: 7364 7761 6e2e 746f 706f 6c6f 6779 272c  sdwan.topology',
+00000440: 0a20 2763 6174 616c 7973 7477 616e 2e6d  . 'catalystwan.m
+00000450: 6f64 656c 7327 2c0a 2027 6361 7461 6c79  odels',. 'cataly
+00000460: 7374 7761 6e2e 6d6f 6465 6c73 2e63 6f6e  stwan.models.con
+00000470: 6669 6775 7261 7469 6f6e 272c 0a20 2763  figuration',. 'c
+00000480: 6174 616c 7973 7477 616e 2e6d 6f64 656c  atalystwan.model
+00000490: 732e 636f 6e66 6967 7572 6174 696f 6e2e  s.configuration.
+000004a0: 6665 6174 7572 655f 7072 6f66 696c 6527  feature_profile'
+000004b0: 2c0a 2027 6361 7461 6c79 7374 7761 6e2e  ,. 'catalystwan.
+000004c0: 6d6f 6465 6c73 2e63 6f6e 6669 6775 7261  models.configura
+000004d0: 7469 6f6e 2e66 6561 7475 7265 5f70 726f  tion.feature_pro
+000004e0: 6669 6c65 2e73 6477 616e 2e61 7070 6c69  file.sdwan.appli
+000004f0: 6361 7469 6f6e 5f70 7269 6f72 6974 7927  cation_priority'
+00000500: 2c0a 2027 6361 7461 6c79 7374 7761 6e2e  ,. 'catalystwan.
+00000510: 6d6f 6465 6c73 2e63 6f6e 6669 6775 7261  models.configura
+00000520: 7469 6f6e 2e66 6561 7475 7265 5f70 726f  tion.feature_pro
+00000530: 6669 6c65 2e73 6477 616e 2e63 6c69 272c  file.sdwan.cli',
+00000540: 0a20 2763 6174 616c 7973 7477 616e 2e6d  . 'catalystwan.m
+00000550: 6f64 656c 732e 636f 6e66 6967 7572 6174  odels.configurat
+00000560: 696f 6e2e 6665 6174 7572 655f 7072 6f66  ion.feature_prof
+00000570: 696c 652e 7364 7761 6e2e 646e 735f 7365  ile.sdwan.dns_se
+00000580: 6375 7269 7479 272c 0a20 2763 6174 616c  curity',. 'catal
+00000590: 7973 7477 616e 2e6d 6f64 656c 732e 636f  ystwan.models.co
+000005a0: 6e66 6967 7572 6174 696f 6e2e 6665 6174  nfiguration.feat
+000005b0: 7572 655f 7072 6f66 696c 652e 7364 7761  ure_profile.sdwa
+000005c0: 6e2e 656d 6265 6464 6564 5f73 6563 7572  n.embedded_secur
+000005d0: 6974 7927 2c0a 2027 6361 7461 6c79 7374  ity',. 'catalyst
+000005e0: 7761 6e2e 6d6f 6465 6c73 2e63 6f6e 6669  wan.models.confi
+000005f0: 6775 7261 7469 6f6e 2e66 6561 7475 7265  guration.feature
+00000600: 5f70 726f 6669 6c65 2e73 6477 616e 2e6f  _profile.sdwan.o
+00000610: 7468 6572 272c 0a20 2763 6174 616c 7973  ther',. 'catalys
+00000620: 7477 616e 2e6d 6f64 656c 732e 636f 6e66  twan.models.conf
+00000630: 6967 7572 6174 696f 6e2e 6665 6174 7572  iguration.featur
+00000640: 655f 7072 6f66 696c 652e 7364 7761 6e2e  e_profile.sdwan.
+00000650: 706f 6c69 6379 5f6f 626a 6563 7427 2c0a  policy_object',.
+00000660: 2027 6361 7461 6c79 7374 7761 6e2e 6d6f   'catalystwan.mo
+00000670: 6465 6c73 2e63 6f6e 6669 6775 7261 7469  dels.configurati
+00000680: 6f6e 2e66 6561 7475 7265 5f70 726f 6669  on.feature_profi
+00000690: 6c65 2e73 6477 616e 2e70 6f6c 6963 795f  le.sdwan.policy_
+000006a0: 6f62 6a65 6374 2e70 6f6c 6963 7927 2c0a  object.policy',.
+000006b0: 2027 6361 7461 6c79 7374 7761 6e2e 6d6f   'catalystwan.mo
+000006c0: 6465 6c73 2e63 6f6e 6669 6775 7261 7469  dels.configurati
+000006d0: 6f6e 2e66 6561 7475 7265 5f70 726f 6669  on.feature_profi
+000006e0: 6c65 2e73 6477 616e 2e70 6f6c 6963 795f  le.sdwan.policy_
+000006f0: 6f62 6a65 6374 2e73 6563 7572 6974 7927  object.security'
+00000700: 2c0a 2027 6361 7461 6c79 7374 7761 6e2e  ,. 'catalystwan.
+00000710: 6d6f 6465 6c73 2e63 6f6e 6669 6775 7261  models.configura
+00000720: 7469 6f6e 2e66 6561 7475 7265 5f70 726f  tion.feature_pro
+00000730: 6669 6c65 2e73 6477 616e 2e73 6572 7669  file.sdwan.servi
+00000740: 6365 272c 0a20 2763 6174 616c 7973 7477  ce',. 'catalystw
+00000750: 616e 2e6d 6f64 656c 732e 636f 6e66 6967  an.models.config
+00000760: 7572 6174 696f 6e2e 6665 6174 7572 655f  uration.feature_
+00000770: 7072 6f66 696c 652e 7364 7761 6e2e 7365  profile.sdwan.se
+00000780: 7276 6963 652e 6c61 6e27 2c0a 2027 6361  rvice.lan',. 'ca
+00000790: 7461 6c79 7374 7761 6e2e 6d6f 6465 6c73  talystwan.models
+000007a0: 2e63 6f6e 6669 6775 7261 7469 6f6e 2e66  .configuration.f
+000007b0: 6561 7475 7265 5f70 726f 6669 6c65 2e73  eature_profile.s
+000007c0: 6477 616e 2e73 6967 5f73 6563 7572 6974  dwan.sig_securit
+000007d0: 7927 2c0a 2027 6361 7461 6c79 7374 7761  y',. 'catalystwa
+000007e0: 6e2e 6d6f 6465 6c73 2e63 6f6e 6669 6775  n.models.configu
+000007f0: 7261 7469 6f6e 2e66 6561 7475 7265 5f70  ration.feature_p
+00000800: 726f 6669 6c65 2e73 6477 616e 2e73 7973  rofile.sdwan.sys
+00000810: 7465 6d27 2c0a 2027 6361 7461 6c79 7374  tem',. 'catalyst
+00000820: 7761 6e2e 6d6f 6465 6c73 2e63 6f6e 6669  wan.models.confi
+00000830: 6775 7261 7469 6f6e 2e66 6561 7475 7265  guration.feature
+00000840: 5f70 726f 6669 6c65 2e73 6477 616e 2e74  _profile.sdwan.t
+00000850: 6f70 6f6c 6f67 7927 2c0a 2027 6361 7461  opology',. 'cata
+00000860: 6c79 7374 7761 6e2e 6d6f 6465 6c73 2e63  lystwan.models.c
+00000870: 6f6e 6669 6775 7261 7469 6f6e 2e66 6561  onfiguration.fea
+00000880: 7475 7265 5f70 726f 6669 6c65 2e73 6477  ture_profile.sdw
+00000890: 616e 2e74 7261 6e73 706f 7274 272c 0a20  an.transport',. 
+000008a0: 2763 6174 616c 7973 7477 616e 2e6d 6f64  'catalystwan.mod
+000008b0: 656c 732e 636f 6e66 6967 7572 6174 696f  els.configuratio
+000008c0: 6e2e 6665 6174 7572 655f 7072 6f66 696c  n.feature_profil
+000008d0: 652e 7364 7761 6e2e 7472 616e 7370 6f72  e.sdwan.transpor
+000008e0: 742e 6d61 6e61 6765 6d65 6e74 272c 0a20  t.management',. 
+000008f0: 2763 6174 616c 7973 7477 616e 2e6d 6f64  'catalystwan.mod
+00000900: 656c 732e 636f 6e66 6967 7572 6174 696f  els.configuratio
+00000910: 6e2e 6665 6174 7572 655f 7072 6f66 696c  n.feature_profil
+00000920: 652e 7364 7761 6e2e 7472 616e 7370 6f72  e.sdwan.transpor
+00000930: 742e 7761 6e2e 696e 7465 7266 6163 6527  t.wan.interface'
+00000940: 2c0a 2027 6361 7461 6c79 7374 7761 6e2e  ,. 'catalystwan.
+00000950: 6d6f 6465 6c73 2e6d 6973 6327 2c0a 2027  models.misc',. '
+00000960: 6361 7461 6c79 7374 7761 6e2e 6d6f 6465  catalystwan.mode
+00000970: 6c73 2e6d 6f6e 6974 6f72 696e 6727 2c0a  ls.monitoring',.
+00000980: 2027 6361 7461 6c79 7374 7761 6e2e 6d6f   'catalystwan.mo
+00000990: 6465 6c73 2e70 6f6c 6963 7927 2c0a 2027  dels.policy',. '
+000009a0: 6361 7461 6c79 7374 7761 6e2e 6d6f 6465  catalystwan.mode
+000009b0: 6c73 2e70 6f6c 6963 792e 6465 6669 6e69  ls.policy.defini
+000009c0: 7469 6f6e 272c 0a20 2763 6174 616c 7973  tion',. 'catalys
+000009d0: 7477 616e 2e6d 6f64 656c 732e 706f 6c69  twan.models.poli
+000009e0: 6379 2e6c 6973 7427 2c0a 2027 6361 7461  cy.list',. 'cata
+000009f0: 6c79 7374 7761 6e2e 7465 7374 7327 2c0a  lystwan.tests',.
+00000a00: 2027 6361 7461 6c79 7374 7761 6e2e 7465   'catalystwan.te
+00000a10: 7374 732e 636f 6e66 6967 5f6d 6967 7261  sts.config_migra
+00000a20: 7469 6f6e 272c 0a20 2763 6174 616c 7973  tion',. 'catalys
+00000a30: 7477 616e 2e74 6573 7473 2e63 6f6e 6669  twan.tests.confi
+00000a40: 675f 6d69 6772 6174 696f 6e2e 7465 7374  g_migration.test
+00000a50: 5f64 6174 6127 2c0a 2027 6361 7461 6c79  _data',. 'cataly
+00000a60: 7374 7761 6e2e 7465 7374 732e 636f 6e66  stwan.tests.conf
+00000a70: 6967 5f6d 6967 7261 7469 6f6e 2e74 6573  ig_migration.tes
+00000a80: 745f 6461 7461 2e66 6561 7475 7265 5f74  t_data.feature_t
+00000a90: 656d 706c 6174 6573 272c 0a20 2763 6174  emplates',. 'cat
+00000aa0: 616c 7973 7477 616e 2e74 6573 7473 2e6d  alystwan.tests.m
+00000ab0: 6f64 656c 7327 2c0a 2027 6361 7461 6c79  odels',. 'cataly
+00000ac0: 7374 7761 6e2e 7465 7374 732e 7465 6d70  stwan.tests.temp
+00000ad0: 6c61 7465 7327 2c0a 2027 6361 7461 6c79  lates',. 'cataly
+00000ae0: 7374 7761 6e2e 7465 7374 732e 7465 6d70  stwan.tests.temp
+00000af0: 6c61 7465 732e 6d6f 6465 6c73 272c 0a20  lates.models',. 
+00000b00: 2763 6174 616c 7973 7477 616e 2e75 7469  'catalystwan.uti
+00000b10: 6c73 272c 0a20 2763 6174 616c 7973 7477  ls',. 'catalystw
+00000b20: 616e 2e75 7469 6c73 2e63 6f6e 6669 675f  an.utils.config_
+00000b30: 6d69 6772 6174 696f 6e2e 636f 6e76 6572  migration.conver
+00000b40: 7465 7273 272c 0a20 2763 6174 616c 7973  ters',. 'catalys
+00000b50: 7477 616e 2e75 7469 6c73 2e63 6f6e 6669  twan.utils.confi
+00000b60: 675f 6d69 6772 6174 696f 6e2e 636f 6e76  g_migration.conv
+00000b70: 6572 7465 7273 2e66 6561 7475 7265 5f74  erters.feature_t
+00000b80: 656d 706c 6174 6527 2c0a 2027 6361 7461  emplate',. 'cata
+00000b90: 6c79 7374 7761 6e2e 7574 696c 732e 636f  lystwan.utils.co
+00000ba0: 6e66 6967 5f6d 6967 7261 7469 6f6e 2e63  nfig_migration.c
+00000bb0: 6f6e 7665 7274 6572 732e 6665 6174 7572  onverters.featur
+00000bc0: 655f 7465 6d70 6c61 7465 2e6c 616e 272c  e_template.lan',
+00000bd0: 0a20 2763 6174 616c 7973 7477 616e 2e75  . 'catalystwan.u
+00000be0: 7469 6c73 2e63 6f6e 6669 675f 6d69 6772  tils.config_migr
+00000bf0: 6174 696f 6e2e 636f 6e76 6572 7465 7273  ation.converters
+00000c00: 2e66 6561 7475 7265 5f74 656d 706c 6174  .feature_templat
+00000c10: 652e 7761 6e27 2c0a 2027 6361 7461 6c79  e.wan',. 'cataly
+00000c20: 7374 7761 6e2e 7574 696c 732e 636f 6e66  stwan.utils.conf
+00000c30: 6967 5f6d 6967 7261 7469 6f6e 2e63 6f6e  ig_migration.con
+00000c40: 7665 7274 6572 732e 706f 6c69 6379 272c  verters.policy',
+00000c50: 0a20 2763 6174 616c 7973 7477 616e 2e75  . 'catalystwan.u
+00000c60: 7469 6c73 2e63 6f6e 6669 675f 6d69 6772  tils.config_migr
+00000c70: 6174 696f 6e2e 6372 6561 746f 7273 272c  ation.creators',
+00000c80: 0a20 2763 6174 616c 7973 7477 616e 2e75  . 'catalystwan.u
+00000c90: 7469 6c73 2e63 6f6e 6669 675f 6d69 6772  tils.config_migr
+00000ca0: 6174 696f 6e2e 6372 6561 746f 7273 2e73  ation.creators.s
+00000cb0: 7472 6174 6567 7927 2c0a 2027 6361 7461  trategy',. 'cata
+00000cc0: 6c79 7374 7761 6e2e 7574 696c 732e 636f  lystwan.utils.co
+00000cd0: 6e66 6967 5f6d 6967 7261 7469 6f6e 2e66  nfig_migration.f
+00000ce0: 6163 746f 7269 6573 272c 0a20 2763 6174  actories',. 'cat
+00000cf0: 616c 7973 7477 616e 2e75 7469 6c73 2e63  alystwan.utils.c
+00000d00: 6f6e 6669 675f 6d69 6772 6174 696f 6e2e  onfig_migration.
+00000d10: 7265 7665 7274 6572 7327 2c0a 2027 6361  reverters',. 'ca
+00000d20: 7461 6c79 7374 7761 6e2e 7574 696c 732e  talystwan.utils.
+00000d30: 636f 6e66 6967 5f6d 6967 7261 7469 6f6e  config_migration
+00000d40: 2e73 7465 7073 272c 0a20 2763 6174 616c  .steps',. 'catal
+00000d50: 7973 7477 616e 2e75 7469 6c73 2e66 6561  ystwan.utils.fea
+00000d60: 7475 7265 5f74 656d 706c 6174 6527 2c0a  ture_template',.
+00000d70: 2027 6361 7461 6c79 7374 7761 6e2e 776f   'catalystwan.wo
+00000d80: 726b 666c 6f77 7327 5d0a 0a70 6163 6b61  rkflows']..packa
+00000d90: 6765 5f64 6174 6120 3d20 5c0a 7b27 273a  ge_data = \.{'':
+00000da0: 205b 272a 275d 2c0a 2027 6361 7461 6c79   ['*'],. 'cataly
+00000db0: 7374 7761 6e2e 6170 692e 7465 6d70 6c61  stwan.api.templa
+00000dc0: 7465 732e 7061 796c 6f61 6473 2e61 6161  tes.payloads.aaa
+00000dd0: 273a 205b 2766 6561 7475 7265 2f2a 275d  ': ['feature/*']
+00000de0: 2c0a 2027 6361 7461 6c79 7374 7761 6e2e  ,. 'catalystwan.
+00000df0: 6170 692e 7465 6d70 6c61 7465 732e 7061  api.templates.pa
+00000e00: 796c 6f61 6473 2e63 6973 636f 5f76 706e  yloads.cisco_vpn
+00000e10: 273a 205b 2766 6561 7475 7265 2f2a 275d  ': ['feature/*']
+00000e20: 2c0a 2027 6361 7461 6c79 7374 7761 6e2e  ,. 'catalystwan.
+00000e30: 6d6f 6465 6c73 2e63 6f6e 6669 6775 7261  models.configura
+00000e40: 7469 6f6e 273a 205b 2764 6f63 732f 2a27  tion': ['docs/*'
+00000e50: 5d2c 0a20 2763 6174 616c 7973 7477 616e  ],. 'catalystwan
+00000e60: 2e74 6573 7473 2e74 656d 706c 6174 6573  .tests.templates
+00000e70: 273a 205b 2764 6566 696e 6974 696f 6e73  ': ['definitions
+00000e80: 2f2a 272c 0a20 2020 2020 2020 2020 2020  /*',.           
+00000e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ea0: 2020 2020 2020 2764 6566 696e 6974 696f        'definitio
+00000eb0: 6e73 2f62 6173 6963 2f2a 272c 0a20 2020  ns/basic/*',.   
+00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ed0: 2020 2020 2020 2020 2020 2020 2020 2773                's
+00000ee0: 6368 656d 6173 2f2a 272c 0a20 2020 2020  chemas/*',.     
+00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f00: 2020 2020 2020 2020 2020 2020 2773 6368              'sch
+00000f10: 656d 6173 2f62 6173 6963 2f2a 275d 7d0a  emas/basic/*']}.
+00000f20: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+00000f30: 7320 3d20 5c0a 5b27 4a69 6e6a 6132 3e3d  s = \.['Jinja2>=
+00000f40: 332e 312e 322c 3c34 2e30 2e30 272c 0a20  3.1.2,<4.0.0',. 
+00000f50: 2761 7474 7273 3e3d 3231 2e34 2e30 2c3c  'attrs>=21.4.0,<
+00000f60: 3232 2e30 2e30 272c 0a20 2763 6973 636f  22.0.0',. 'cisco
+00000f70: 636f 6e66 7061 7273 653d 3d31 2e39 2e34  confparse==1.9.4
+00000f80: 3127 2c0a 2027 636c 696e 743e 3d30 2e35  1',. 'clint>=0.5
+00000f90: 2e31 2c3c 302e 362e 3027 2c0a 2027 666c  .1,<0.6.0',. 'fl
+00000fa0: 616b 6538 2d71 756f 7465 733e 3d33 2e33  ake8-quotes>=3.3
+00000fb0: 2e31 2c3c 342e 302e 3027 2c0a 2027 7061  .1,<4.0.0',. 'pa
+00000fc0: 636b 6167 696e 673e 3d32 332e 302c 3c32  ckaging>=23.0,<2
+00000fd0: 342e 3027 2c0a 2027 7079 6461 6e74 6963  4.0',. 'pydantic
+00000fe0: 3e3d 322e 372c 3c33 2e30 272c 0a20 2770  >=2.7,<3.0',. 'p
+00000ff0: 7974 686f 6e2d 6461 7465 7574 696c 3e3d  ython-dateutil>=
+00001000: 322e 382e 322c 3c33 2e30 2e30 272c 0a20  2.8.2,<3.0.0',. 
+00001010: 2772 6571 7565 7374 732d 746f 6f6c 6265  'requests-toolbe
+00001020: 6c74 3e3d 312e 302e 302c 3c32 2e30 2e30  lt>=1.0.0,<2.0.0
+00001030: 272c 0a20 2772 6571 7565 7374 733e 3d32  ',. 'requests>=2
+00001040: 2e32 372e 312c 3c33 2e30 2e30 272c 0a20  .27.1,<3.0.0',. 
+00001050: 2774 656e 6163 6974 793e 3d38 2e31 2e30  'tenacity>=8.1.0
+00001060: 2c3c 392e 302e 3027 2c0a 2027 7479 7069  ,<9.0.0',. 'typi
+00001070: 6e67 2d65 7874 656e 7369 6f6e 733e 3d34  ng-extensions>=4
+00001080: 2e36 2e31 2c3c 352e 302e 3027 5d0a 0a73  .6.1,<5.0.0']..s
+00001090: 6574 7570 5f6b 7761 7267 7320 3d20 7b0a  etup_kwargs = {.
+000010a0: 2020 2020 276e 616d 6527 3a20 2763 6174      'name': 'cat
+000010b0: 616c 7973 7477 616e 272c 0a20 2020 2027  alystwan',.    '
+000010c0: 7665 7273 696f 6e27 3a20 2730 2e33 332e  version': '0.33.
+000010d0: 372e 6465 7630 272c 0a20 2020 2027 6465  7.dev0',.    'de
+000010e0: 7363 7269 7074 696f 6e27 3a20 2743 6973  scription': 'Cis
+000010f0: 636f 2043 6174 616c 7973 7420 5741 4e20  co Catalyst WAN 
+00001100: 5344 4b20 666f 7220 5079 7468 6f6e 272c  SDK for Python',
+00001110: 0a20 2020 2027 6c6f 6e67 5f64 6573 6372  .    'long_descr
+00001120: 6970 7469 6f6e 273a 2027 3c70 2061 6c69  iption': '<p ali
+00001130: 676e 3d22 6365 6e74 6572 223e 5c6e 2020  gn="center">\n  
+00001140: 3c61 2068 7265 663d 2223 223e 3c69 6d67  <a href="#"><img
+00001150: 2073 7263 3d22 646f 6373 2f69 6d61 6765   src="docs/image
+00001160: 732f 6361 7461 6c79 7374 7761 6e2e 7376  s/catalystwan.sv
+00001170: 6722 2061 6c74 3d22 4369 7363 6f20 4361  g" alt="Cisco Ca
+00001180: 7461 6c79 7374 2057 414e 2053 444b 204c  talyst WAN SDK L
+00001190: 6f67 6f22 2073 7479 6c65 3d22 6865 6967  ogo" style="heig
+000011a0: 6874 3a31 3530 7078 2220 2f3e 5c6e 3c2f  ht:150px" />\n</
+000011b0: 703e 5c6e 5c6e 5b21 5b50 7974 686f 6e2d  p>\n\n[![Python-
+000011c0: 5375 7070 6f72 7465 645d 2868 7474 7073  Supported](https
+000011d0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000011e0: 6f2f 7374 6174 6963 2f76 313f 6c61 6265  o/static/v1?labe
+000011f0: 6c3d 5079 7468 6f6e 266c 6f67 6f3d 5079  l=Python&logo=Py
+00001200: 7468 6f6e 2663 6f6c 6f72 3d33 3737 3641  thon&color=3776A
+00001210: 4226 6d65 7373 6167 653d 332e 3825 3230  B&message=3.8%20
+00001220: 7c25 3230 332e 3925 3230 7c25 3230 332e  |%203.9%20|%203.
+00001230: 3130 2532 307c 2532 3033 2e31 3125 3230  10%20|%203.11%20
+00001240: 7c25 3230 332e 3132 295d 2868 7474 7073  |%203.12)](https
+00001250: 3a2f 2f77 7777 2e70 7974 686f 6e2e 6f72  ://www.python.or
+00001260: 672f 295c 6e5c 6e43 6973 636f 2043 6174  g/)\n\nCisco Cat
+00001270: 616c 7973 7420 5741 4e20 5344 4b20 6973  alyst WAN SDK is
+00001280: 2061 2070 6163 6b61 6765 2066 6f72 2063   a package for c
+00001290: 7265 6174 696e 6720 7369 6d70 6c65 2061  reating simple a
+000012a0: 6e64 2070 6172 616c 6c65 6c20 6175 746f  nd parallel auto
+000012b0: 6d61 7469 6320 7265 7175 6573 7473 2076  matic requests v
+000012c0: 6961 206f 6666 6963 6961 6c20 5344 2d57  ia official SD-W
+000012d0: 414e 204d 616e 6167 6572 2041 5049 2e20  AN Manager API. 
+000012e0: 4974 2069 7320 696e 7465 6e64 6564 2074  It is intended t
+000012f0: 6f20 7365 7276 6520 6173 2061 206d 756c  o serve as a mul
+00001300: 7469 706c 6520 7365 7373 696f 6e20 6861  tiple session ha
+00001310: 6e64 6c65 7220 2870 726f 7669 6465 722c  ndler (provider,
+00001320: 2070 726f 7669 6465 7220 6173 2061 2074   provider as a t
+00001330: 656e 616e 742c 2074 656e 616e 7429 2e20  enant, tenant). 
+00001340: 5468 6520 6c69 6272 6172 7920 6973 206e  The library is n
+00001350: 6f74 2064 6570 656e 6465 6e74 206f 6e20  ot dependent on 
+00001360: 656e 7669 726f 6e6d 656e 7420 7768 6963  environment whic
+00001370: 6820 6973 2062 6569 6e67 2072 756e 2069  h is being run i
+00001380: 6e2c 2079 6f75 206a 7573 7420 6e65 6564  n, you just need
+00001390: 2061 2063 6f6e 6e65 6374 696f 6e20 746f   a connection to
+000013a0: 2061 6e79 2053 442d 5741 4e20 4d61 6e61   any SD-WAN Mana
+000013b0: 6765 722e 5c6e 5c6e 2323 2049 6d70 6f72  ger.\n\n## Impor
+000013c0: 7461 6e74 204e 6f74 6963 653a 2045 6172  tant Notice: Ear
+000013d0: 6c79 2042 6574 6120 5265 6c65 6173 655c  ly Beta Release\
+000013e0: 6e5c 6e57 656c 636f 6d65 2074 6f20 7468  n\nWelcome to th
+000013f0: 6520 4369 7363 6f20 4361 7461 6c79 7374  e Cisco Catalyst
+00001400: 2057 414e 2053 444b 215c 6e5c 6e57 6520   WAN SDK!\n\nWe 
+00001410: 6172 6520 7468 7269 6c6c 6564 2074 6f20  are thrilled to 
+00001420: 616e 6e6f 756e 6365 2074 6861 7420 4369  announce that Ci
+00001430: 7363 6f20 4361 7461 6c79 7374 2057 414e  sco Catalyst WAN
+00001440: 2053 444b 2069 7320 6e6f 7720 6176 6169   SDK is now avai
+00001450: 6c61 626c 6520 696e 2065 6172 6c79 2062  lable in early b
+00001460: 6574 612e 2054 6869 7320 6973 2061 6e20  eta. This is an 
+00001470: 6578 6369 7469 6e67 2073 7465 7020 666f  exciting step fo
+00001480: 7277 6172 6420 696e 2065 6e61 626c 696e  rward in enablin
+00001490: 6720 6465 7665 6c6f 7065 7273 2074 6f20  g developers to 
+000014a0: 6861 726e 6573 7320 7468 6520 6675 6c6c  harness the full
+000014b0: 2070 6f74 656e 7469 616c 206f 6620 4369   potential of Ci
+000014c0: 7363 6f5c 2773 206e 6574 776f 726b 696e  sco\'s networkin
+000014d0: 6720 736f 6c75 7469 6f6e 732e 2020 506c  g solutions.  Pl
+000014e0: 6561 7365 2062 6520 6177 6172 6520 7468  ease be aware th
+000014f0: 6174 2c20 6173 2061 6e20 6561 726c 7920  at, as an early 
+00001500: 6265 7461 2072 656c 6561 7365 2c20 7468  beta release, th
+00001510: 6973 2076 6572 7369 6f6e 206f 6620 7468  is version of th
+00001520: 6520 5344 4b20 6973 2073 7469 6c6c 2075  e SDK is still u
+00001530: 6e64 6572 676f 696e 6720 6465 7665 6c6f  ndergoing develo
+00001540: 706d 656e 7420 616e 6420 7465 7374 696e  pment and testin
+00001550: 672e 2041 7320 7375 6368 2c20 6974 2069  g. As such, it i
+00001560: 7320 7072 6f76 6964 6564 2022 6173 2069  s provided "as i
+00001570: 7322 2061 6e64 2073 7570 706f 7274 2074  s" and support t
+00001580: 6f20 6164 6472 6573 7320 616e 7920 6973  o address any is
+00001590: 7375 6573 2061 7265 206c 696d 6974 6564  sues are limited
+000015a0: 2061 6e64 2062 6573 7420 6566 666f 7274   and best effort
+000015b0: 2e5c 6e5c 6e23 2320 4e6f 7420 7265 636f  .\n\n## Not reco
+000015c0: 6d6d 656e 6420 746f 2075 7365 2069 6e20  mmend to use in 
+000015d0: 7072 6f64 7563 7469 6f6e 2065 6e76 6972  production envir
+000015e0: 6f6e 6d65 6e74 732e 5c6e 5765 2065 6e63  onments.\nWe enc
+000015f0: 6f75 7261 6765 2064 6576 656c 6f70 6572  ourage developer
+00001600: 7320 746f 2065 7870 6c6f 7265 2061 6e64  s to explore and
+00001610: 2074 6573 7420 7468 6520 5344 4b5c 2773   test the SDK\'s
+00001620: 2063 6170 6162 696c 6974 6965 732c 2062   capabilities, b
+00001630: 7574 2070 6c65 6173 6520 6578 6572 6369  ut please exerci
+00001640: 7365 2063 6175 7469 6f6e 2077 6865 6e20  se caution when 
+00001650: 7573 696e 6720 6974 2069 6e20 7072 6f64  using it in prod
+00001660: 7563 7469 6f6e 2065 6e76 6972 6f6e 6d65  uction environme
+00001670: 6e74 732e 2020 5765 2061 7265 2064 6564  nts.  We are ded
+00001680: 6963 6174 6564 2074 6f20 696d 7072 6f76  icated to improv
+00001690: 696e 6720 7468 6520 4369 7363 6f20 4361  ing the Cisco Ca
+000016a0: 7461 6c79 7374 2057 414e 2053 444b 2061  talyst WAN SDK a
+000016b0: 6e64 2077 6520 7661 6c75 6520 796f 7572  nd we value your
+000016c0: 2069 6e70 7574 2e20 596f 7572 2066 6565   input. Your fee
+000016d0: 6462 6163 6b20 6973 2063 7275 6369 616c  dback is crucial
+000016e0: 2074 6f20 7573 2d69 7420 7769 6c6c 2067   to us-it will g
+000016f0: 7569 6465 2075 7320 696e 2072 6566 696e  uide us in refin
+00001700: 696e 6720 616e 6420 656e 6861 6e63 696e  ing and enhancin
+00001710: 6720 7468 6520 5344 4b20 746f 2062 6574  g the SDK to bet
+00001720: 7465 7220 6d65 6574 2079 6f75 7220 6e65  ter meet your ne
+00001730: 6564 732e 5c6e 546f 2072 6570 6f72 7420  eds.\nTo report 
+00001740: 616e 7920 6973 7375 6573 2c20 7368 6172  any issues, shar
+00001750: 6520 796f 7572 2069 6e73 6967 6874 732c  e your insights,
+00001760: 206f 7220 7375 6767 6573 7420 696d 7072   or suggest impr
+00001770: 6f76 656d 656e 7473 2c20 706c 6561 7365  ovements, please
+00001780: 2076 6973 6974 206f 7572 2049 7373 7565   visit our Issue
+00001790: 7320 7061 6765 206f 6e20 4769 7448 7562  s page on GitHub
+000017a0: 206f 7220 7265 6163 6820 6f75 7420 746f   or reach out to
+000017b0: 2075 7320 7468 726f 7567 6820 7468 6520   us through the 
+000017c0: 7072 6f76 6964 6564 2063 6f6d 6d75 6e69  provided communi
+000017d0: 6361 7469 6f6e 2063 6861 6e6e 656c 732e  cation channels.
+000017e0: 5c6e 5c6e 5468 616e 6b20 796f 7520 666f  \n\nThank you fo
+000017f0: 7220 6265 696e 6720 6120 7061 7274 206f  r being a part o
+00001800: 6620 6f75 7220 6465 7665 6c6f 706d 656e  f our developmen
+00001810: 7420 6a6f 7572 6e65 7921 5c6e 5c6e 2323  t journey!\n\n##
+00001820: 2049 6e73 7461 6c6c 6174 696f 6e5c 6e60   Installation\n`
+00001830: 6060 636f 6e73 6f6c 655c 6e70 6970 2069  ``console\npip i
+00001840: 6e73 7461 6c6c 2063 6174 616c 7973 7477  nstall catalystw
+00001850: 616e 5c6e 6060 605c 6e5c 6e23 2320 4d61  an\n```\n\n## Ma
+00001860: 6e61 6765 7220 5365 7373 696f 6e5c 6e49  nager Session\nI
+00001870: 6e20 6f72 6465 7220 746f 2065 7865 6375  n order to execu
+00001880: 7465 2053 444b 2041 5049 7320 2a2a 4d61  te SDK APIs **Ma
+00001890: 6e61 6765 7253 6573 7369 6f6e 2a2a 206e  nagerSession** n
+000018a0: 6565 6473 2074 6f20 6265 2063 7265 6174  eeds to be creat
+000018b0: 6564 2e20 5468 6520 6661 7374 6573 7420  ed. The fastest 
+000018c0: 7761 7920 746f 2067 6574 2073 7461 7274  way to get start
+000018d0: 6564 2069 7320 746f 2075 7365 2060 6372  ed is to use `cr
+000018e0: 6561 7465 5f6d 616e 6167 6572 5f73 6573  eate_manager_ses
+000018f0: 7369 6f6e 2829 6020 6d65 7468 6f64 2077  sion()` method w
+00001900: 6869 6368 2063 6f6e 6669 6775 7265 7320  hich configures 
+00001910: 7365 7373 696f 6e2c 2070 6572 666f 726d  session, perform
+00001920: 7320 6175 7468 656e 7469 6361 7469 6f6e  s authentication
+00001930: 2066 6f72 2067 6976 656e 2063 7265 6465   for given crede
+00001940: 6e74 6961 6c73 2061 6e64 2072 6574 7572  ntials and retur
+00001950: 6e73 202a 2a4d 616e 6167 6572 5365 7373  ns **ManagerSess
+00001960: 696f 6e2a 2a20 696e 7374 616e 6365 2069  ion** instance i
+00001970: 6e20 6f70 6572 6174 696f 6e61 6c20 7374  n operational st
+00001980: 6174 652e 202a 2a4d 616e 6167 6572 5365  ate. **ManagerSe
+00001990: 7373 696f 6e2a 2a20 7072 6f76 6964 6573  ssion** provides
+000019a0: 2061 2063 6f6c 6c65 6374 696f 6e20 6f66   a collection of
+000019b0: 2073 7570 706f 7274 6564 2041 5049 7320   supported APIs 
+000019c0: 696e 2060 6170 6960 2069 6e73 7461 6e63  in `api` instanc
+000019d0: 6520 7661 7269 6162 6c65 2e5c 6e50 6c65  e variable.\nPle
+000019e0: 6173 6520 6368 6563 6b20 6578 616d 706c  ase check exampl
+000019f0: 6520 6265 6c6f 773a 5c6e 5c6e 6060 6070  e below:\n\n```p
+00001a00: 7974 686f 6e5c 6e66 726f 6d20 6361 7461  ython\nfrom cata
+00001a10: 6c79 7374 7761 6e2e 7365 7373 696f 6e20  lystwan.session 
+00001a20: 696d 706f 7274 2063 7265 6174 655f 6d61  import create_ma
+00001a30: 6e61 6765 725f 7365 7373 696f 6e5c 6e5c  nager_session\n\
+00001a40: 6e75 726c 203d 2022 6578 616d 706c 652e  nurl = "example.
+00001a50: 636f 6d22 5c6e 7573 6572 6e61 6d65 203d  com"\nusername =
+00001a60: 2022 6164 6d69 6e22 5c6e 7061 7373 776f   "admin"\npasswo
+00001a70: 7264 203d 2022 7061 7373 776f 7264 3132  rd = "password12
+00001a80: 3322 5c6e 5c6e 7769 7468 2063 7265 6174  3"\n\nwith creat
+00001a90: 655f 6d61 6e61 6765 725f 7365 7373 696f  e_manager_sessio
+00001aa0: 6e28 7572 6c3d 7572 6c2c 2075 7365 726e  n(url=url, usern
+00001ab0: 616d 653d 7573 6572 6e61 6d65 2c20 7061  ame=username, pa
+00001ac0: 7373 776f 7264 3d70 6173 7377 6f72 6429  ssword=password)
+00001ad0: 2061 7320 7365 7373 696f 6e3a 5c6e 2020   as session:\n  
+00001ae0: 2020 6465 7669 6365 7320 3d20 7365 7373    devices = sess
+00001af0: 696f 6e2e 6170 692e 6465 7669 6365 732e  ion.api.devices.
+00001b00: 6765 7428 295c 6e20 2020 2070 7269 6e74  get()\n    print
+00001b10: 2864 6576 6963 6573 295c 6e60 6060 5c6e  (devices)\n```\n
+00001b20: 2a2a 4d61 6e61 6765 7253 6573 7369 6f6e  **ManagerSession
+00001b30: 2a2a 2065 7874 656e 6473 205b 7265 7175  ** extends [requ
+00001b40: 6573 7473 2e53 6573 7369 6f6e 5d28 6874  ests.Session](ht
+00001b50: 7470 733a 2f2f 7265 7175 6573 7473 2e72  tps://requests.r
+00001b60: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00001b70: 2f6c 6174 6573 742f 7573 6572 2f61 6476  /latest/user/adv
+00001b80: 616e 6365 642f 2373 6573 7369 6f6e 2d6f  anced/#session-o
+00001b90: 626a 6563 7473 2920 736f 2061 6c6c 2066  bjects) so all f
+00001ba0: 756e 6374 696f 6e61 6c69 7479 2066 726f  unctionality fro
+00001bb0: 6d20 5b72 6571 7565 7374 735d 2868 7474  m [requests](htt
+00001bc0: 7073 3a2f 2f72 6571 7565 7374 732e 7265  ps://requests.re
+00001bd0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00001be0: 6c61 7465 7374 2f29 206c 6962 7261 7279  latest/) library
+00001bf0: 2069 7320 6176 6169 6162 6c65 2074 6f20   is avaiable to 
+00001c00: 7573 6572 2c20 6974 2061 6c73 6f20 696d  user, it also im
+00001c10: 706c 656d 656e 7473 2070 7974 686f 6e20  plements python 
+00001c20: 5b63 6f6e 7465 7874 6d61 6e61 6765 725d  [contextmanager]
+00001c30: 2868 7474 7073 3a2f 2f64 6f63 732e 7079  (https://docs.py
+00001c40: 7468 6f6e 2e6f 7267 2f33 2e38 2f6c 6962  thon.org/3.8/lib
+00001c50: 7261 7279 2f63 6f6e 7465 7874 6c69 622e  rary/contextlib.
+00001c60: 6874 6d6c 2363 6f6e 7465 7874 6c69 622e  html#contextlib.
+00001c70: 636f 6e74 6578 746d 616e 6167 6572 2920  contextmanager) 
+00001c80: 616e 6420 6175 746f 6d61 7469 6361 6c6c  and automaticall
+00001c90: 7920 6672 6565 7320 7365 7276 6572 2072  y frees server r
+00001ca0: 6573 6f75 7263 6573 206f 6e20 6578 6974  esources on exit
+00001cb0: 2e5c 6e5c 6e3c 6465 7461 696c 733e 5c6e  .\n\n<details>\n
+00001cc0: 2020 2020 3c73 756d 6d61 7279 3e20 3c62      <summary> <b
+00001cd0: 3e43 6f6e 6669 6775 7265 204d 616e 6167  >Configure Manag
+00001ce0: 6572 2053 6573 7369 6f6e 2062 6566 6f72  er Session befor
+00001cf0: 6520 7573 696e 673c 2f62 3e20 3c69 3e28  e using</b> <i>(
+00001d00: 636c 6963 6b20 746f 2065 7870 616e 6429  click to expand)
+00001d10: 3c2f 693e 3c2f 7375 6d6d 6172 793e 5c6e  </i></summary>\n
+00001d20: 5c6e 4974 2069 7320 706f 7373 6962 6c65  \nIt is possible
+00001d30: 2074 6f20 636f 6e66 6967 7572 6520 2a2a   to configure **
+00001d40: 4d61 6e61 6765 7253 6573 7369 6f6e 2a2a  ManagerSession**
+00001d50: 2070 7269 6f72 2073 656e 6469 6e67 2061   prior sending a
+00001d60: 6e79 2072 6571 7565 7374 2e5c 6e5c 6e60  ny request.\n\n`
+00001d70: 6060 7079 7468 6f6e 5c6e 6672 6f6d 2063  ``python\nfrom c
+00001d80: 6174 616c 7973 7477 616e 2e73 6573 7369  atalystwan.sessi
+00001d90: 6f6e 2069 6d70 6f72 7420 4d61 6e61 6765  on import Manage
+00001da0: 7253 6573 7369 6f6e 5c6e 5c6e 7572 6c20  rSession\n\nurl 
+00001db0: 3d20 2265 7861 6d70 6c65 2e63 6f6d 225c  = "example.com"\
+00001dc0: 6e75 7365 726e 616d 6520 3d20 2261 646d  nusername = "adm
+00001dd0: 696e 225c 6e70 6173 7377 6f72 6420 3d20  in"\npassword = 
+00001de0: 2270 6173 7377 6f72 6431 3233 225c 6e5c  "password123"\n\
+00001df0: 6e23 2063 6f6e 6669 6775 7265 2073 6573  n# configure ses
+00001e00: 7369 6f6e 2075 7369 6e67 2063 6f6e 7374  sion using const
+00001e10: 7275 6374 6f72 202d 206e 6f74 6869 6e67  ructor - nothing
+00001e20: 2077 696c 6c20 6265 2073 656e 7420 746f   will be sent to
+00001e30: 2074 6172 6765 7420 7365 7276 6572 2079   target server y
+00001e40: 6574 5c6e 7365 7373 696f 6e20 3d20 4d61  et\nsession = Ma
+00001e50: 6e61 6765 7253 6573 7369 6f6e 2875 726c  nagerSession(url
+00001e60: 3d75 726c 2c20 7573 6572 6e61 6d65 3d75  =url, username=u
+00001e70: 7365 726e 616d 652c 2070 6173 7377 6f72  sername, passwor
+00001e80: 643d 7061 7373 776f 7264 295c 6e23 206c  d=password)\n# l
+00001e90: 6f67 696e 2061 6e64 2073 656e 6420 7265  ogin and send re
+00001ea0: 7175 6573 7473 5c6e 7365 7373 696f 6e2e  quests\nsession.
+00001eb0: 6c6f 6769 6e28 295c 6e73 6573 7369 6f6e  login()\nsession
+00001ec0: 2e67 6574 2822 2f64 6174 6173 6572 7669  .get("/dataservi
+00001ed0: 6365 2f64 6576 6963 6522 295c 6e73 6573  ce/device")\nses
+00001ee0: 7369 6f6e 2e63 6c6f 7365 2829 5c6e 6060  sion.close()\n``
+00001ef0: 605c 6e57 6865 6e20 696e 7465 7261 6374  `\nWhen interact
+00001f00: 696e 6720 7769 7468 2074 6865 2053 4457  ing with the SDW
+00001f10: 414e 204d 616e 6167 6572 2041 5049 2077  AN Manager API w
+00001f20: 6974 686f 7574 2075 7369 6e67 2061 2063  ithout using a c
+00001f30: 6f6e 7465 7874 206d 616e 6167 6572 2c20  ontext manager, 
+00001f40: 6974 5c27 7320 696d 706f 7274 616e 7420  it\'s important 
+00001f50: 5c6e 746f 206d 616e 7561 6c6c 7920 6578  \nto manually ex
+00001f60: 6563 7574 6520 7468 6520 6063 6c6f 7365  ecute the `close
+00001f70: 2829 6020 6d65 7468 6f64 2074 6f20 7265  ()` method to re
+00001f80: 6c65 6173 6520 7468 6520 7573 6572 2073  lease the user s
+00001f90: 6573 7369 6f6e 2072 6573 6f75 7263 652e  ession resource.
+00001fa0: 5c6e 456e 7375 7265 2074 6861 7420 7468  \nEnsure that th
+00001fb0: 6520 6063 6c6f 7365 2829 6020 6d65 7468  e `close()` meth
+00001fc0: 6f64 2069 7320 6361 6c6c 6564 2061 6674  od is called aft
+00001fd0: 6572 2079 6f75 2068 6176 6520 6669 6e69  er you have fini
+00001fe0: 7368 6564 2075 7369 6e67 2074 6865 2073  shed using the s
+00001ff0: 6573 7369 6f6e 2074 6f20 6d61 696e 7461  ession to mainta
+00002000: 696e 206f 7074 696d 616c 2072 6573 6f75  in optimal resou
+00002010: 7263 6520 6d61 6e61 6765 6d65 6e74 2061  rce management a
+00002020: 6e64 2061 766f 6964 2070 6f74 656e 7469  nd avoid potenti
+00002030: 616c 2065 7272 6f72 732e 5c6e 5c6e 3c2f  al errors.\n\n</
+00002040: 6465 7461 696c 733e 5c6e 5c6e 3c64 6574  details>\n\n<det
+00002050: 6169 6c73 3e5c 6e20 2020 203c 7375 6d6d  ails>\n    <summ
+00002060: 6172 793e 203c 623e 4c6f 6769 6e20 6173  ary> <b>Login as
+00002070: 2054 656e 616e 743c 2f62 3e20 3c69 3e28   Tenant</b> <i>(
+00002080: 636c 6963 6b20 746f 2065 7870 616e 6429  click to expand)
+00002090: 3c2f 693e 3c2f 7375 6d6d 6172 793e 5c6e  </i></summary>\n
+000020a0: 5c6e 5465 6e61 6e74 2064 6f6d 6169 6e20  \nTenant domain 
+000020b0: 6e65 6564 7320 746f 2062 6520 7072 6f76  needs to be prov
+000020c0: 6964 6564 2069 6e20 7572 6c20 746f 6765  ided in url toge
+000020d0: 7468 6572 2077 6974 6820 5465 6e61 6e74  ther with Tenant
+000020e0: 2063 7265 6465 6e74 6961 6c73 2e5c 6e5c   credentials.\n\
+000020f0: 6e60 6060 7079 7468 6f6e 5c6e 6672 6f6d  n```python\nfrom
+00002100: 2063 6174 616c 7973 7477 616e 2e73 6573   catalystwan.ses
+00002110: 7369 6f6e 2069 6d70 6f72 7420 6372 6561  sion import crea
+00002120: 7465 5f6d 616e 6167 6572 5f73 6573 7369  te_manager_sessi
+00002130: 6f6e 5c6e 5c6e 7572 6c20 3d20 2274 656e  on\n\nurl = "ten
+00002140: 616e 742e 6578 616d 706c 652e 636f 6d22  ant.example.com"
+00002150: 5c6e 7573 6572 6e61 6d65 203d 2022 7465  \nusername = "te
+00002160: 6e61 6e74 5f75 7365 7222 5c6e 7061 7373  nant_user"\npass
+00002170: 776f 7264 203d 2022 7061 7373 776f 7264  word = "password
+00002180: 3132 3322 5c6e 5c6e 7769 7468 2063 7265  123"\n\nwith cre
+00002190: 6174 655f 6d61 6e61 6765 725f 7365 7373  ate_manager_sess
+000021a0: 696f 6e28 7572 6c3d 7572 6c2c 2075 7365  ion(url=url, use
+000021b0: 726e 616d 653d 7573 6572 6e61 6d65 2c20  rname=username, 
+000021c0: 7061 7373 776f 7264 3d70 6173 7377 6f72  password=passwor
+000021d0: 6429 2061 7320 7365 7373 696f 6e3a 5c6e  d) as session:\n
+000021e0: 2020 2020 7072 696e 7428 7365 7373 696f      print(sessio
+000021f0: 6e2e 7365 7373 696f 6e5f 7479 7065 295c  n.session_type)\
+00002200: 6e60 6060 5c6e 5c6e 3c2f 6465 7461 696c  n```\n\n</detail
+00002210: 733e 5c6e 5c6e 3c64 6574 6169 6c73 3e5c  s>\n\n<details>\
+00002220: 6e20 2020 203c 7375 6d6d 6172 793e 203c  n    <summary> <
+00002230: 623e 4c6f 6769 6e20 6173 2050 726f 7669  b>Login as Provi
+00002240: 6465 722d 6173 2d54 656e 616e 743c 2f62  der-as-Tenant</b
+00002250: 3e20 3c69 3e28 636c 6963 6b20 746f 2065  > <i>(click to e
+00002260: 7870 616e 6429 3c2f 693e 3c2f 7375 6d6d  xpand)</i></summ
+00002270: 6172 793e 5c6e 5c6e 5465 6e61 6e74 2060  ary>\n\nTenant `
+00002280: 7375 6264 6f6d 6169 6e60 206e 6565 6473  subdomain` needs
+00002290: 2074 6f20 6265 2070 726f 7669 6465 6420   to be provided 
+000022a0: 6173 2061 6464 6974 696f 6e61 6c20 6172  as additional ar
+000022b0: 6775 6d65 6e74 2074 6f67 6574 6865 7220  gument together 
+000022c0: 7769 7468 2050 726f 7669 6465 7220 6372  with Provider cr
+000022d0: 6564 656e 7469 616c 732e 5c6e 5c6e 6060  edentials.\n\n``
+000022e0: 6070 7974 686f 6e5c 6e66 726f 6d20 6361  `python\nfrom ca
+000022f0: 7461 6c79 7374 7761 6e2e 7365 7373 696f  talystwan.sessio
+00002300: 6e20 696d 706f 7274 2063 7265 6174 655f  n import create_
+00002310: 6d61 6e61 6765 725f 7365 7373 696f 6e5c  manager_session\
+00002320: 6e5c 6e75 726c 203d 2022 6578 616d 706c  n\nurl = "exampl
+00002330: 652e 636f 6d22 5c6e 7573 6572 6e61 6d65  e.com"\nusername
+00002340: 203d 2022 7072 6f76 6964 6572 225c 6e70   = "provider"\np
+00002350: 6173 7377 6f72 6420 3d20 2270 6173 7377  assword = "passw
+00002360: 6f72 6431 3233 225c 6e73 7562 646f 6d61  ord123"\nsubdoma
+00002370: 696e 203d 2022 7465 6e61 6e74 2e65 7861  in = "tenant.exa
+00002380: 6d70 6c65 2e63 6f6d 225c 6e5c 6e77 6974  mple.com"\n\nwit
+00002390: 6820 6372 6561 7465 5f6d 616e 6167 6572  h create_manager
+000023a0: 5f73 6573 7369 6f6e 2875 726c 3d75 726c  _session(url=url
+000023b0: 2c20 7573 6572 6e61 6d65 3d75 7365 726e  , username=usern
+000023c0: 616d 652c 2070 6173 7377 6f72 643d 7061  ame, password=pa
+000023d0: 7373 776f 7264 2c20 7375 6264 6f6d 6169  ssword, subdomai
+000023e0: 6e3d 7375 6264 6f6d 6169 6e29 2061 7320  n=subdomain) as 
+000023f0: 7365 7373 696f 6e3a 5c6e 2020 2020 7072  session:\n    pr
+00002400: 696e 7428 7365 7373 696f 6e2e 7365 7373  int(session.sess
+00002410: 696f 6e5f 7479 7065 295c 6e60 6060 5c6e  ion_type)\n```\n
+00002420: 5c6e 3c2f 6465 7461 696c 733e 5c6e 5c6e  \n</details>\n\n
+00002430: 5c6e 5c6e 2323 2041 5049 2075 7361 6765  \n\n## API usage
+00002440: 2065 7861 6d70 6c65 735c 6e41 6c6c 2065   examples\nAll e
+00002450: 7861 6d70 6c65 7320 6265 6c6f 7720 6173  xamples below as
+00002460: 7375 6d65 7320 6073 6573 7369 6f6e 6020  sumes `session` 
+00002470: 7661 7269 6162 6c65 2063 6f6e 7461 696e  variable contain
+00002480: 7320 6c6f 6767 6564 2d69 6e20 5b4d 616e  s logged-in [Man
+00002490: 6167 6572 2053 6573 7369 6f6e 5d28 234d  ager Session](#M
+000024a0: 616e 6167 6572 2d53 6573 7369 6f6e 2920  anager-Session) 
+000024b0: 696e 7374 616e 6365 2e5c 6e5c 6e3c 6465  instance.\n\n<de
+000024c0: 7461 696c 733e 5c6e 2020 2020 3c73 756d  tails>\n    <sum
+000024d0: 6d61 7279 3e20 3c62 3e47 6574 2064 6576  mary> <b>Get dev
+000024e0: 6963 6573 3c2f 623e 203c 693e 2863 6c69  ices</b> <i>(cli
+000024f0: 636b 2074 6f20 6578 7061 6e64 293c 2f69  ck to expand)</i
+00002500: 3e3c 2f73 756d 6d61 7279 3e5c 6e5c 6e60  ></summary>\n\n`
+00002510: 6060 7079 7468 6f6e 5c6e 6465 7669 6365  ``python\ndevice
+00002520: 7320 3d20 7365 7373 696f 6e2e 6170 692e  s = session.api.
+00002530: 6465 7669 6365 732e 6765 7428 295c 6e60  devices.get()\n`
+00002540: 6060 5c6e 5c6e 3c2f 6465 7461 696c 733e  ``\n\n</details>
+00002550: 5c6e 5c6e 3c64 6574 6169 6c73 3e5c 6e20  \n\n<details>\n 
+00002560: 2020 203c 7375 6d6d 6172 793e 203c 623e     <summary> <b>
+00002570: 4164 6d69 6e20 5465 6368 3c2f 623e 203c  Admin Tech</b> <
+00002580: 693e 2863 6c69 636b 2074 6f20 6578 7061  i>(click to expa
+00002590: 6e64 293c 2f69 3e3c 2f73 756d 6d61 7279  nd)</i></summary
+000025a0: 3e5c 6e5c 6e60 6060 5079 7468 6f6e 5c6e  >\n\n```Python\n
+000025b0: 6164 6d69 6e5f 7465 6368 5f66 696c 6520  admin_tech_file 
+000025c0: 3d20 7365 7373 696f 6e2e 6170 692e 6164  = session.api.ad
+000025d0: 6d69 6e5f 7465 6368 2e67 656e 6572 6174  min_tech.generat
+000025e0: 6528 2231 3732 2e31 362e 3235 352e 3131  e("172.16.255.11
+000025f0: 2229 5c6e 7365 7373 696f 6e2e 6170 692e  ")\nsession.api.
+00002600: 6164 6d69 6e5f 7465 6368 2e64 6f77 6e6c  admin_tech.downl
+00002610: 6f61 6428 6164 6d69 6e5f 7465 6368 5f66  oad(admin_tech_f
+00002620: 696c 6529 5c6e 7365 7373 696f 6e2e 6170  ile)\nsession.ap
+00002630: 692e 6164 6d69 6e5f 7465 6368 2e64 656c  i.admin_tech.del
+00002640: 6574 6528 6164 6d69 6e5f 7465 6368 5f66  ete(admin_tech_f
+00002650: 696c 6529 5c6e 6060 605c 6e3c 2f64 6574  ile)\n```\n</det
+00002660: 6169 6c73 3e5c 6e5c 6e3c 6465 7461 696c  ails>\n\n<detail
+00002670: 733e 5c6e 2020 2020 3c73 756d 6d61 7279  s>\n    <summary
+00002680: 3e20 3c62 3e53 7065 6564 2074 6573 743c  > <b>Speed test<
+00002690: 2f62 3e20 3c69 3e28 636c 6963 6b20 746f  /b> <i>(click to
+000026a0: 2065 7870 616e 6429 3c2f 693e 3c2f 7375   expand)</i></su
+000026b0: 6d6d 6172 793e 5c6e 5c6e 6060 6070 7974  mmary>\n\n```pyt
+000026c0: 686f 6e5c 6e64 6576 6963 6573 203d 2073  hon\ndevices = s
+000026d0: 6573 7369 6f6e 2e61 7069 2e64 6576 6963  ession.api.devic
+000026e0: 6573 2e67 6574 2829 5c6e 7370 6565 6474  es.get()\nspeedt
+000026f0: 6573 7420 3d20 7365 7373 696f 6e2e 6170  est = session.ap
+00002700: 692e 7370 6565 6474 6573 742e 7370 6565  i.speedtest.spee
+00002710: 6474 6573 7428 6465 7669 6365 735b 305d  dtest(devices[0]
+00002720: 2c20 6465 7669 6365 735b 315d 295c 6e60  , devices[1])\n`
+00002730: 6060 5c6e 5c6e 3c2f 6465 7461 696c 733e  ``\n\n</details>
+00002740: 5c6e 5c6e 3c64 6574 6169 6c73 3e5c 6e20  \n\n<details>\n 
+00002750: 2020 203c 7375 6d6d 6172 793e 203c 623e     <summary> <b>
+00002760: 5570 6772 6164 6520 6465 7669 6365 3c2f  Upgrade device</
+00002770: 623e 203c 693e 2863 6c69 636b 2074 6f20  b> <i>(click to 
+00002780: 6578 7061 6e64 293c 2f69 3e3c 2f73 756d  expand)</i></sum
+00002790: 6d61 7279 3e5c 6e5c 6e60 6060 7079 7468  mary>\n\n```pyth
+000027a0: 6f6e 5c6e 2320 5072 6570 6172 6520 6465  on\n# Prepare de
+000027b0: 7669 6365 7320 6c69 7374 5c6e 636f 6e74  vices list\ncont
+000027c0: 726f 6c6c 6572 7320 3d20 7365 7373 696f  rollers = sessio
+000027d0: 6e2e 656e 6470 6f69 6e74 732e 636f 6e66  n.endpoints.conf
+000027e0: 6967 7572 6174 696f 6e5f 6465 7669 6365  iguration_device
+000027f0: 5f69 6e76 656e 746f 7279 2e67 6574 5f64  _inventory.get_d
+00002800: 6576 6963 655f 6465 7461 696c 7328 5c27  evice_details(\'
+00002810: 636f 6e74 726f 6c6c 6572 735c 2729 5c6e  controllers\')\n
+00002820: 7673 6d61 7274 7320 3d20 636f 6e74 726f  vsmarts = contro
+00002830: 6c6c 6572 732e 6669 6c74 6572 2870 6572  llers.filter(per
+00002840: 736f 6e61 6c69 7479 3d50 6572 736f 6e61  sonality=Persona
+00002850: 6c69 7479 2e56 534d 4152 5429 5c6e 696d  lity.VSMART)\nim
+00002860: 6167 6520 3d20 2276 6970 7465 6c61 2d32  age = "viptela-2
+00002870: 302e 372e 322d 7838 365f 3634 2e74 6172  0.7.2-x86_64.tar
+00002880: 2e67 7a22 5c6e 5c6e 2320 5570 6c6f 6164  .gz"\n\n# Upload
+00002890: 2069 6d61 6765 5c6e 7365 7373 696f 6e2e   image\nsession.
+000028a0: 6170 692e 7265 706f 7369 746f 7279 2e75  api.repository.u
+000028b0: 706c 6f61 645f 696d 6167 6528 696d 6167  pload_image(imag
+000028c0: 6529 5c6e 5c6e 2320 496e 7374 616c 6c20  e)\n\n# Install 
+000028d0: 736f 6674 7761 7265 5c6e 5c6e 696e 7374  software\n\ninst
+000028e0: 616c 6c5f 7461 736b 203d 2073 6573 7369  all_task = sessi
+000028f0: 6f6e 2e61 7069 2e73 6f66 7477 6172 652e  on.api.software.
+00002900: 696e 7374 616c 6c28 6465 7669 6365 733d  install(devices=
+00002910: 7673 6d61 7274 732c 2069 6d61 6765 3d69  vsmarts, image=i
+00002920: 6d61 6765 295c 6e5c 6e23 2043 6865 636b  mage)\n\n# Check
+00002930: 2061 6374 696f 6e20 7374 6174 7573 5c6e   action status\n
+00002940: 696e 7374 616c 6c5f 7461 736b 2e77 6169  install_task.wai
+00002950: 745f 666f 725f 636f 6d70 6c65 7465 6428  t_for_completed(
+00002960: 295c 6e60 6060 5c6e 5c6e 3c2f 6465 7461  )\n```\n\n</deta
+00002970: 696c 733e 5c6e 5c6e 3c64 6574 6169 6c73  ils>\n\n<details
+00002980: 3e5c 6e20 2020 203c 7375 6d6d 6172 793e  >\n    <summary>
+00002990: 203c 623e 4765 7420 616c 6172 6d73 3c2f   <b>Get alarms</
+000029a0: 623e 203c 693e 2863 6c69 636b 2074 6f20  b> <i>(click to 
+000029b0: 6578 7061 6e64 293c 2f69 3e3c 2f73 756d  expand)</i></sum
+000029c0: 6d61 7279 3e5c 6e54 6f20 6765 7420 616c  mary>\nTo get al
+000029d0: 6c20 616c 6172 6d73 3a5c 6e5c 6e60 6060  l alarms:\n\n```
+000029e0: 7079 7468 6f6e 5c6e 616c 6172 6d73 203d  python\nalarms =
+000029f0: 2073 6573 7369 6f6e 2e61 7069 2e61 6c61   session.api.ala
+00002a00: 726d 732e 6765 7428 295c 6e60 6060 5c6e  rms.get()\n```\n
+00002a10: 5c6e 546f 2067 6574 2061 6c6c 206e 6f74  \nTo get all not
+00002a20: 2076 6965 7765 6420 616c 6172 6d73 3a5c   viewed alarms:\
+00002a30: 6e5c 6e60 6060 7079 7468 6f6e 5c6e 6e6f  n\n```python\nno
+00002a40: 745f 7669 6577 6564 5f61 6c61 726d 7320  t_viewed_alarms 
+00002a50: 3d20 7365 7373 696f 6e2e 6170 692e 616c  = session.api.al
+00002a60: 6172 6d73 2e67 6574 2829 2e66 696c 7465  arms.get().filte
+00002a70: 7228 7669 6577 6564 3d46 616c 7365 295c  r(viewed=False)\
+00002a80: 6e60 6060 5c6e 5c6e 546f 2067 6574 2061  n```\n\nTo get a
+00002a90: 6c6c 2061 6c61 726d 7320 6672 6f6d 2070  ll alarms from p
+00002aa0: 6173 7420 606e 6020 686f 7572 733a 5c6e  ast `n` hours:\n
+00002ab0: 5c6e 6060 6070 7974 686f 6e5c 6e6e 203d  \n```python\nn =
+00002ac0: 2032 345c 6e61 6c61 726d 735f 6672 6f6d   24\nalarms_from
+00002ad0: 5f6e 5f68 6f75 7273 203d 2073 6573 7369  _n_hours = sessi
+00002ae0: 6f6e 2e61 7069 2e61 6c61 726d 732e 6765  on.api.alarms.ge
+00002af0: 7428 6672 6f6d 5f74 696d 653d 6e29 5c6e  t(from_time=n)\n
+00002b00: 6060 605c 6e5c 6e54 6f20 6765 7420 616c  ```\n\nTo get al
+00002b10: 6c20 6372 6974 6963 616c 2061 6c61 726d  l critical alarm
+00002b20: 7320 6672 6f6d 2070 6173 7420 606e 6020  s from past `n` 
+00002b30: 686f 7572 733a 5c6e 5c6e 6060 6070 7974  hours:\n\n```pyt
+00002b40: 686f 6e5c 6e6e 203d 2034 385c 6e63 7269  hon\nn = 48\ncri
+00002b50: 7469 6361 6c5f 616c 6172 6d73 203d 2073  tical_alarms = s
+00002b60: 6573 7369 6f6e 2e61 7069 2e61 6c61 726d  ession.api.alarm
+00002b70: 732e 6765 7428 6672 6f6d 5f74 696d 653d  s.get(from_time=
+00002b80: 6e29 2e66 696c 7465 7228 7365 7665 7269  n).filter(severi
+00002b90: 7479 3d53 6576 6572 6974 792e 4352 4954  ty=Severity.CRIT
+00002ba0: 4943 414c 295c 6e60 6060 5c6e 5c6e 3c2f  ICAL)\n```\n\n</
+00002bb0: 6465 7461 696c 733e 5c6e 5c6e 3c64 6574  details>\n\n<det
+00002bc0: 6169 6c73 3e5c 6e20 2020 203c 7375 6d6d  ails>\n    <summ
+00002bd0: 6172 793e 203c 623e 5573 6572 733c 2f62  ary> <b>Users</b
+00002be0: 3e20 3c69 3e28 636c 6963 6b20 746f 2065  > <i>(click to e
+00002bf0: 7870 616e 6429 3c2f 693e 3c2f 7375 6d6d  xpand)</i></summ
+00002c00: 6172 793e 5c6e 5c6e 6060 6070 7974 686f  ary>\n\n```pytho
+00002c10: 6e5c 6e23 2047 6574 2061 6c6c 2075 7365  n\n# Get all use
+00002c20: 7273 5c6e 7365 7373 696f 6e2e 6170 692e  rs\nsession.api.
+00002c30: 7573 6572 732e 6765 7428 295c 6e5c 6e23  users.get()\n\n#
+00002c40: 2043 7265 6174 6520 7573 6572 5c6e 6e65   Create user\nne
+00002c50: 775f 7573 6572 203d 2055 7365 7228 7573  w_user = User(us
+00002c60: 6572 6e61 6d65 3d22 6e65 775f 7573 6572  ername="new_user
+00002c70: 222c 2070 6173 7377 6f72 643d 226e 6577  ", password="new
+00002c80: 5f75 7365 7222 2c20 6772 6f75 703d 5b22  _user", group=["
+00002c90: 6e65 7461 646d 696e 225d 2c20 6465 7363  netadmin"], desc
+00002ca0: 7269 7074 696f 6e3d 226e 6577 2075 7365  ription="new use
+00002cb0: 7222 295c 6e73 6573 7369 6f6e 2e61 7069  r")\nsession.api
+00002cc0: 2e75 7365 7273 2e63 7265 6174 6528 6e65  .users.create(ne
+00002cd0: 775f 7573 6572 295c 6e5c 6e23 2055 7064  w_user)\n\n# Upd
+00002ce0: 6174 6520 7573 6572 2064 6174 615c 6e6e  ate user data\nn
+00002cf0: 6577 5f75 7365 725f 7570 6461 7465 203d  ew_user_update =
+00002d00: 2055 7365 7255 7064 6174 6552 6571 7565   UserUpdateReque
+00002d10: 7374 2875 7365 726e 616d 653d 226e 6577  st(username="new
+00002d20: 5f75 7365 7222 2c20 6772 6f75 703d 5b22  _user", group=["
+00002d30: 6e65 7461 646d 696e 222c 2022 6e65 746f  netadmin", "neto
+00002d40: 7073 225d 2c20 6c6f 6361 6c65 3d22 656e  ps"], locale="en
+00002d50: 5f55 5322 2c20 6465 7363 7269 7074 696f  _US", descriptio
+00002d60: 6e3d 2275 7064 6174 6564 2d6e 6577 5f75  n="updated-new_u
+00002d70: 7365 722d 6465 7363 7269 7074 696f 6e22  ser-description"
+00002d80: 295c 6e73 6573 7369 6f6e 2e61 7069 2e75  )\nsession.api.u
+00002d90: 7365 7273 2e75 7064 6174 6528 6e65 775f  sers.update(new_
+00002da0: 7573 6572 5f75 7064 6174 6529 5c6e 5c6e  user_update)\n\n
+00002db0: 2320 5570 6461 7465 2075 7365 7220 7061  # Update user pa
+00002dc0: 7373 776f 7264 5c6e 7365 7373 696f 6e2e  ssword\nsession.
+00002dd0: 6170 692e 7573 6572 732e 7570 6461 7465  api.users.update
+00002de0: 5f70 6173 7377 6f72 6428 226e 6577 5f75  _password("new_u
+00002df0: 7365 7222 2c20 226e 3357 2d50 3473 2477  ser", "n3W-P4s$w
+00002e00: 3072 6422 295c 6e5c 6e23 2052 6573 6574  0rd")\n\n# Reset
+00002e10: 2075 7365 725c 6e73 6573 7369 6f6e 2e61   user\nsession.a
+00002e20: 7069 2e75 7365 7273 2e72 6573 6574 2822  pi.users.reset("
+00002e30: 6e65 775f 7573 6572 2229 5c6e 5c6e 2320  new_user")\n\n# 
+00002e40: 4465 6c65 7465 2075 7365 725c 6e73 6573  Delete user\nses
+00002e50: 7369 6f6e 2e61 7069 2e75 7365 7273 2e64  sion.api.users.d
+00002e60: 656c 6574 6528 226e 6577 5f75 7365 7222  elete("new_user"
+00002e70: 295c 6e5c 6e23 2047 6574 2063 7572 7265  )\n\n# Get curre
+00002e80: 6e74 2075 7365 7220 6175 7468 656e 7469  nt user authenti
+00002e90: 6361 7469 6f6e 2074 7970 6520 616e 6420  cation type and 
+00002ea0: 726f 6c65 5c6e 7365 7373 696f 6e2e 6170  role\nsession.ap
+00002eb0: 692e 7573 6572 732e 6765 745f 6175 7468  i.users.get_auth
+00002ec0: 5f74 7970 6528 295c 6e73 6573 7369 6f6e  _type()\nsession
+00002ed0: 2e61 7069 2e75 7365 7273 2e67 6574 5f72  .api.users.get_r
+00002ee0: 6f6c 6528 295c 6e60 6060 5c6e 5c6e 3c2f  ole()\n```\n\n</
+00002ef0: 6465 7461 696c 733e 5c6e 5c6e 3c64 6574  details>\n\n<det
+00002f00: 6169 6c73 3e5c 6e20 2020 203c 7375 6d6d  ails>\n    <summ
+00002f10: 6172 793e 203c 623e 5573 6572 2047 726f  ary> <b>User Gro
+00002f20: 7570 733c 2f62 3e20 3c69 3e28 636c 6963  ups</b> <i>(clic
+00002f30: 6b20 746f 2065 7870 616e 6429 3c2f 693e  k to expand)</i>
+00002f40: 3c2f 7375 6d6d 6172 793e 5c6e 5c6e 6060  </summary>\n\n``
+00002f50: 6070 7974 686f 6e5c 6e23 2047 6574 2061  `python\n# Get a
+00002f60: 6c6c 2075 7365 7220 6772 6f75 7073 5c6e  ll user groups\n
+00002f70: 7365 7373 696f 6e2e 6170 692e 7573 6572  session.api.user
+00002f80: 5f67 726f 7570 732e 6765 7428 295c 6e5c  _groups.get()\n\
+00002f90: 6e23 2043 7265 6174 6520 7573 6572 2067  n# Create user g
+00002fa0: 726f 7570 5c6e 6772 6f75 7020 3d20 5573  roup\ngroup = Us
+00002fb0: 6572 4772 6f75 7028 226e 6577 5f75 7365  erGroup("new_use
+00002fc0: 725f 6772 6f75 7022 2c20 5b5d 295c 6e67  r_group", [])\ng
+00002fd0: 726f 7570 2e65 6e61 626c 655f 7265 6164  roup.enable_read
+00002fe0: 287b 2241 7564 6974 204c 6f67 222c 2022  ({"Audit Log", "
+00002ff0: 416c 6172 6d73 227d 295c 6e67 726f 7570  Alarms"})\ngroup
+00003000: 2e65 6e61 626c 655f 7265 6164 5f61 6e64  .enable_read_and
+00003010: 5f77 7269 7465 287b 2244 6576 6963 6520  _write({"Device 
+00003020: 496e 7665 6e74 6f72 7922 7d29 5c6e 7365  Inventory"})\nse
+00003030: 7373 696f 6e2e 6170 692e 7573 6572 5f67  ssion.api.user_g
+00003040: 726f 7570 732e 6372 6561 7465 2867 726f  roups.create(gro
+00003050: 7570 295c 6e5c 6e23 2055 7064 6174 6520  up)\n\n# Update 
+00003060: 7573 6572 2067 726f 7570 5c6e 6772 6f75  user group\ngrou
+00003070: 702e 6469 7361 626c 6528 7b22 416c 6172  p.disable({"Alar
+00003080: 6d73 227d 295c 6e73 6573 7369 6f6e 2e61  ms"})\nsession.a
+00003090: 7069 2e75 7365 725f 6772 6f75 7073 2e75  pi.user_groups.u
+000030a0: 7064 6174 6528 6772 6f75 7029 5c6e 5c6e  pdate(group)\n\n
+000030b0: 2320 4465 6c65 7465 2075 7365 7220 6772  # Delete user gr
+000030c0: 6f75 705c 6e73 6573 7369 6f6e 2e61 7069  oup\nsession.api
+000030d0: 2e75 7365 725f 6772 6f75 7073 2e64 656c  .user_groups.del
+000030e0: 6574 6528 6772 6f75 702e 6772 6f75 705f  ete(group.group_
+000030f0: 6e61 6d65 295c 6e60 6060 5c6e 5c6e 3c2f  name)\n```\n\n</
+00003100: 6465 7461 696c 733e 5c6e 5c6e 3c2f 6465  details>\n\n</de
+00003110: 7461 696c 733e 5c6e 5c6e 3c64 6574 6169  tails>\n\n<detai
+00003120: 6c73 3e5c 6e20 2020 203c 7375 6d6d 6172  ls>\n    <summar
+00003130: 793e 203c 623e 5365 7373 696f 6e73 3c2f  y> <b>Sessions</
+00003140: 623e 203c 693e 2863 6c69 636b 2074 6f20  b> <i>(click to 
+00003150: 6578 7061 6e64 293c 2f69 3e3c 2f73 756d  expand)</i></sum
+00003160: 6d61 7279 3e5c 6e5c 6e60 6060 7079 7468  mary>\n\n```pyth
+00003170: 6f6e 5c6e 2320 4765 7420 616c 6c20 6163  on\n# Get all ac
+00003180: 7469 7665 2073 6573 7369 6f6e 735c 6e61  tive sessions\na
+00003190: 6374 6976 655f 7365 7373 696f 6e73 203d  ctive_sessions =
+000031a0: 2073 6573 7369 6f6e 2e61 7069 2e73 6573   session.api.ses
+000031b0: 7369 6f6e 732e 6765 7428 295c 6e5c 6e23  sions.get()\n\n#
+000031c0: 2049 6e76 616c 6964 6174 6520 7365 7373   Invalidate sess
+000031d0: 696f 6e73 2066 6f72 2067 6976 656e 2075  ions for given u
+000031e0: 7365 725c 6e6e 6577 5f75 7365 725f 7365  ser\nnew_user_se
+000031f0: 7373 696f 6e73 203d 2061 6374 6976 655f  ssions = active_
+00003200: 7365 7373 696f 6e73 2e66 696c 7465 7228  sessions.filter(
+00003210: 7261 775f 7573 6572 6e61 6d65 3d22 6e65  raw_username="ne
+00003220: 775f 7573 6572 2229 5c6e 7365 7373 696f  w_user")\nsessio
+00003230: 6e2e 6170 692e 7365 7373 696f 6e73 2e69  n.api.sessions.i
+00003240: 6e76 616c 6964 6174 6528 6e65 775f 7573  nvalidate(new_us
+00003250: 6572 5f73 6573 7369 6f6e 7329 5c6e 6060  er_sessions)\n``
+00003260: 605c 6e5c 6e3c 2f64 6574 6169 6c73 3e5c  `\n\n</details>\
+00003270: 6e5c 6e3c 6465 7461 696c 733e 5c6e 2020  n\n<details>\n  
+00003280: 2020 3c73 756d 6d61 7279 3e20 3c62 3e52    <summary> <b>R
+00003290: 6573 6f75 7263 6520 4772 6f75 7073 3c2f  esource Groups</
+000032a0: 623e 203c 693e 2863 6c69 636b 2074 6f20  b> <i>(click to 
+000032b0: 6578 7061 6e64 293c 2f69 3e3c 2f73 756d  expand)</i></sum
+000032c0: 6d61 7279 3e5c 6e5c 6e60 6060 7079 7468  mary>\n\n```pyth
+000032d0: 6f6e 5c6e 2320 6765 7420 7265 736f 7572  on\n# get resour
+000032e0: 6365 2067 726f 7570 735c 6e73 6573 7369  ce groups\nsessi
+000032f0: 6f6e 2e61 7069 2e72 6573 6f75 7263 655f  on.api.resource_
+00003300: 6772 6f75 7073 2e67 6574 2829 5c6e 5c6e  groups.get()\n\n
+00003310: 2320 6372 6561 7465 2072 6573 6f75 7263  # create resourc
+00003320: 6520 6772 6f75 705c 6e6e 6577 5f72 6573  e group\nnew_res
+00003330: 6f75 7263 655f 6772 6f75 7020 3d20 5265  ource_group = Re
+00003340: 736f 7572 6365 4772 6f75 7028 5c6e 2020  sourceGroup(\n  
+00003350: 2020 6e61 6d65 3d22 6e65 775f 7265 736f    name="new_reso
+00003360: 7572 6365 5f67 726f 7570 222c 5c6e 2020  urce_group",\n  
+00003370: 2020 6465 7363 3d22 4375 7374 6f6d 2052    desc="Custom R
+00003380: 6573 6f75 7263 6520 4772 6f75 7020 2331  esource Group #1
+00003390: 222c 5c6e 2020 2020 7369 7465 4964 733d  ",\n    siteIds=
+000033a0: 5b5d 5c6e 295c 6e73 6573 7369 6f6e 2e61  []\n)\nsession.a
+000033b0: 7069 2e72 6573 6f75 7263 655f 6772 6f75  pi.resource_grou
+000033c0: 7073 2e63 7265 6174 6528 6e65 775f 7265  ps.create(new_re
+000033d0: 736f 7572 6365 5f67 726f 7570 295c 6e5c  source_group)\n\
+000033e0: 6e23 2075 7064 6174 6520 7265 736f 7572  n# update resour
+000033f0: 6365 2067 726f 7570 5c6e 7265 736f 7572  ce group\nresour
+00003400: 6365 5f67 726f 7570 203d 2073 6573 7369  ce_group = sessi
+00003410: 6f6e 2e61 7069 2e72 6573 6f75 7263 655f  on.api.resource_
+00003420: 6772 6f75 7073 2e67 6574 2829 2e66 696c  groups.get().fil
+00003430: 7465 7228 6e61 6d65 3d22 6e65 775f 7265  ter(name="new_re
+00003440: 736f 7572 6365 5f67 726f 7570 2229 2e73  source_group").s
+00003450: 696e 676c 655f 6f72 5f64 6566 6175 6c74  ingle_or_default
+00003460: 2829 5c6e 7570 6461 7465 645f 7265 736f  ()\nupdated_reso
+00003470: 7572 6365 5f67 726f 7570 203d 2052 6573  urce_group = Res
+00003480: 6f75 7263 6547 726f 7570 5570 6461 7465  ourceGroupUpdate
+00003490: 5265 7175 6573 7428 5c6e 2020 2020 6964  Request(\n    id
+000034a0: 3d72 6573 6f75 7263 655f 6772 6f75 702e  =resource_group.
+000034b0: 6964 2c5c 6e20 2020 206e 616d 653d 7265  id,\n    name=re
+000034c0: 736f 7572 6365 5f67 726f 7570 2e6e 616d  source_group.nam
+000034d0: 652c 5c6e 2020 2020 6465 7363 3d22 4375  e,\n    desc="Cu
+000034e0: 7374 6f6d 2052 6573 6f75 7263 6520 4772  stom Resource Gr
+000034f0: 6f75 7020 2331 2077 6974 6820 7570 6461  oup #1 with upda
+00003500: 7465 6420 6465 7363 7269 7074 696f 6e20  ted description 
+00003510: 616e 6420 7369 7465 2069 6473 222c 5c6e  and site ids",\n
+00003520: 2020 2020 7369 7465 4964 733d 5b32 3030      siteIds=[200
+00003530: 5d5c 6e29 5c6e 5c6e 2320 7377 6974 6368  ]\n)\n\n# switch
+00003540: 2074 6f20 7265 736f 7572 6365 2067 726f   to resource gro
+00003550: 7570 2076 6965 775c 6e73 6573 7369 6f6e  up view\nsession
+00003560: 2e61 7069 2e72 6573 6f75 7263 655f 6772  .api.resource_gr
+00003570: 6f75 7073 2e73 7769 7463 6828 226e 6577  oups.switch("new
+00003580: 5f72 6573 6f75 7263 655f 6772 6f75 7022  _resource_group"
+00003590: 295c 6e5c 6e23 2064 656c 6574 6520 7265  )\n\n# delete re
+000035a0: 736f 7572 6365 2067 726f 7570 5c6e 7365  source group\nse
+000035b0: 7373 696f 6e2e 6170 692e 7265 736f 7572  ssion.api.resour
+000035c0: 6365 5f67 726f 7570 732e 6465 6c65 7465  ce_groups.delete
+000035d0: 2872 6573 6f75 7263 655f 6772 6f75 702e  (resource_group.
+000035e0: 6964 295c 6e60 6060 5c6e 5c6e 3c2f 6465  id)\n```\n\n</de
+000035f0: 7461 696c 733e 5c6e 5c6e 3c64 6574 6169  tails>\n\n<detai
+00003600: 6c73 3e5c 6e20 2020 203c 7375 6d6d 6172  ls>\n    <summar
+00003610: 793e 203c 623e 5465 6e61 6e74 206d 616e  y> <b>Tenant man
+00003620: 6167 656d 656e 743c 2f62 3e20 3c69 3e28  agement</b> <i>(
+00003630: 636c 6963 6b20 746f 2065 7870 616e 6429  click to expand)
+00003640: 3c2f 693e 3c2f 7375 6d6d 6172 793e 5c6e  </i></summary>\n
+00003650: 5c6e 6060 6070 7974 686f 6e5c 6e61 7069  \n```python\napi
+00003660: 203d 2073 6573 7369 6f6e 2e61 7069 2e74   = session.api.t
+00003670: 656e 616e 745f 6d61 6e61 6765 6d65 6e74  enant_management
+00003680: 5c6e 2320 6372 6561 7465 2074 656e 616e  \n# create tenan
+00003690: 7473 5c6e 7465 6e61 6e74 7320 3d20 5b5c  ts\ntenants = [\
+000036a0: 6e20 2020 2054 656e 616e 7428 5c6e 2020  n    Tenant(\n  
+000036b0: 2020 2020 2020 6e61 6d65 3d22 7465 6e61        name="tena
+000036c0: 6e74 3122 2c5c 6e20 2020 2020 2020 206f  nt1",\n        o
+000036d0: 7267 5f6e 616d 653d 2243 6973 636f 4465  rg_name="CiscoDe
+000036e0: 764e 6574 222c 5c6e 2020 2020 2020 2020  vNet",\n        
+000036f0: 7375 6264 6f6d 6169 6e3d 2261 6c70 6861  subdomain="alpha
+00003700: 2e62 7261 766f 2e6e 6574 222c 5c6e 2020  .bravo.net",\n  
+00003710: 2020 2020 2020 6465 7363 3d22 5468 6973        desc="This
+00003720: 2069 7320 7465 6e61 6e74 2066 6f72 2075   is tenant for u
+00003730: 6e69 7420 7465 7374 7322 2c5c 6e20 2020  nit tests",\n   
+00003740: 2020 2020 2065 6467 655f 636f 6e6e 6563       edge_connec
+00003750: 746f 725f 656e 6162 6c65 3d54 7275 652c  tor_enable=True,
+00003760: 5c6e 2020 2020 2020 2020 6564 6765 5f63  \n        edge_c
+00003770: 6f6e 6e65 6374 6f72 5f73 7973 7465 6d5f  onnector_system_
+00003780: 6970 3d22 3137 322e 3136 2e32 3535 2e38  ip="172.16.255.8
+00003790: 3122 2c5c 6e20 2020 2020 2020 2065 6467  1",\n        edg
+000037a0: 655f 636f 6e6e 6563 746f 725f 7475 6e6e  e_connector_tunn
+000037b0: 656c 5f69 6e74 6572 6661 6365 5f6e 616d  el_interface_nam
+000037c0: 653d 2247 6967 6162 6974 4574 6865 726e  e="GigabitEthern
+000037d0: 6574 3122 2c5c 6e20 2020 2020 2020 2077  et1",\n        w
+000037e0: 616e 5f65 6467 655f 666f 7265 6361 7374  an_edge_forecast
+000037f0: 3d31 2c5c 6e20 2020 2029 5c6e 5d5c 6e63  =1,\n    )\n]\nc
+00003800: 7265 6174 655f 7461 736b 203d 2061 7069  reate_task = api
+00003810: 2e63 7265 6174 6528 7465 6e61 6e74 7329  .create(tenants)
+00003820: 5c6e 6372 6561 7465 5f74 6173 6b2e 7761  \ncreate_task.wa
+00003830: 6974 5f66 6f72 5f63 6f6d 706c 6574 6564  it_for_completed
+00003840: 2829 5c6e 2320 6c69 7374 2061 6c6c 2074  ()\n# list all t
+00003850: 656e 616e 7473 5c6e 7465 6e61 6e74 735f  enants\ntenants_
+00003860: 6461 7461 203d 2061 7069 2e67 6574 5f61  data = api.get_a
+00003870: 6c6c 2829 5c6e 2320 7069 636b 2074 656e  ll()\n# pick ten
+00003880: 616e 7420 6672 6f6d 206c 6973 7420 6279  ant from list by
+00003890: 206e 616d 655c 6e74 656e 616e 7420 3d20   name\ntenant = 
+000038a0: 7465 6e61 6e74 735f 6461 7461 2e66 696c  tenants_data.fil
+000038b0: 7465 7228 6e61 6d65 3d22 7465 6e61 6e74  ter(name="tenant
+000038c0: 3122 292e 7369 6e67 6c65 5f6f 725f 6465  1").single_or_de
+000038d0: 6661 756c 7428 295c 6e23 2067 6574 2073  fault()\n# get s
+000038e0: 656c 6563 7465 6420 7465 6e61 6e74 2069  elected tenant i
+000038f0: 645c 6e74 656e 616e 745f 6964 203d 2074  d\ntenant_id = t
+00003900: 656e 616e 742e 7465 6e61 6e74 5f69 645c  enant.tenant_id\
+00003910: 6e23 2067 6574 2076 7365 7373 696f 6e20  n# get vsession 
+00003920: 6964 206f 6620 7365 6c65 6374 6564 2074  id of selected t
+00003930: 656e 616e 745c 6e76 7365 7373 696f 6e69  enant\nvsessioni
+00003940: 6420 3d20 6170 692e 7673 6573 7369 6f6e  d = api.vsession
+00003950: 5f69 6428 7465 6e61 6e74 5f69 6429 5c6e  _id(tenant_id)\n
+00003960: 2320 6465 6c65 7465 2074 656e 616e 7420  # delete tenant 
+00003970: 6279 2069 6473 5c6e 6465 6c65 7465 5f74  by ids\ndelete_t
+00003980: 6173 6b20 3d20 6170 692e 6465 6c65 7465  ask = api.delete
+00003990: 285b 7465 6e61 6e74 5f69 645d 295c 6e64  ([tenant_id])\nd
+000039a0: 656c 6574 655f 7461 736b 2e77 6169 745f  elete_task.wait_
+000039b0: 666f 725f 636f 6d70 6c65 7465 6428 295c  for_completed()\
+000039c0: 6e23 206f 7468 6572 735c 6e61 7069 2e67  n# others\napi.g
+000039d0: 6574 5f68 6f73 7469 6e67 5f63 6170 6163  et_hosting_capac
+000039e0: 6974 795f 6f6e 5f76 736d 6172 7473 2829  ity_on_vsmarts()
+000039f0: 5c6e 6170 692e 6765 745f 7374 6174 7573  \napi.get_status
+00003a00: 6573 2829 5c6e 6170 692e 6765 745f 7673  es()\napi.get_vs
+00003a10: 6d61 7274 5f6d 6170 7069 6e67 2829 5c6e  mart_mapping()\n
+00003a20: 6060 605c 6e3c 2f64 6574 6169 6c73 3e5c  ```\n</details>\
+00003a30: 6e5c 6e3c 6465 7461 696c 733e 5c6e 2020  n\n<details>\n  
+00003a40: 2020 3c73 756d 6d61 7279 3e20 3c62 3e54    <summary> <b>T
+00003a50: 656e 616e 7420 6d69 6772 6174 696f 6e3c  enant migration<
+00003a60: 2f62 3e20 3c69 3e28 636c 6963 6b20 746f  /b> <i>(click to
+00003a70: 2065 7870 616e 6429 3c2f 693e 3c2f 7375   expand)</i></su
+00003a80: 6d6d 6172 793e 5c6e 5c6e 6060 6070 7974  mmary>\n\n```pyt
+00003a90: 686f 6e5c 6e66 726f 6d20 7061 7468 6c69  hon\nfrom pathli
+00003aa0: 6220 696d 706f 7274 2050 6174 685c 6e66  b import Path\nf
+00003ab0: 726f 6d20 6361 7461 6c79 7374 7761 6e2e  rom catalystwan.
+00003ac0: 7365 7373 696f 6e20 696d 706f 7274 2063  session import c
+00003ad0: 7265 6174 655f 6d61 6e61 6765 725f 7365  reate_manager_se
+00003ae0: 7373 696f 6e5c 6e66 726f 6d20 6361 7461  ssion\nfrom cata
+00003af0: 6c79 7374 7761 6e2e 6d6f 6465 6c73 2e74  lystwan.models.t
+00003b00: 656e 616e 7420 696d 706f 7274 2054 656e  enant import Ten
+00003b10: 616e 7445 7870 6f72 745c 6e66 726f 6d20  antExport\nfrom 
+00003b20: 6361 7461 6c79 7374 7761 6e2e 776f 726b  catalystwan.work
+00003b30: 666c 6f77 732e 7465 6e61 6e74 5f6d 6967  flows.tenant_mig
+00003b40: 7261 7469 6f6e 2069 6d70 6f72 7420 6d69  ration import mi
+00003b50: 6772 6174 696f 6e5f 776f 726b 666c 6f77  gration_workflow
+00003b60: 5c6e 5c6e 7465 6e61 6e74 203d 2054 656e  \n\ntenant = Ten
+00003b70: 616e 7445 7870 6f72 7428 5c6e 2020 2020  antExport(\n    
+00003b80: 6e61 6d65 3d22 6d61 6e67 6f22 2c5c 6e20  name="mango",\n 
+00003b90: 2020 2064 6573 633d 224d 616e 676f 2074     desc="Mango t
+00003ba0: 656e 616e 7420 6465 7363 7269 7074 696f  enant descriptio
+00003bb0: 6e22 2c5c 6e20 2020 206f 7267 5f6e 616d  n",\n    org_nam
+00003bc0: 653d 2250 726f 7669 6465 7220 4f72 672d  e="Provider Org-
+00003bd0: 4d61 6e67 6f20 496e 6322 2c5c 6e20 2020  Mango Inc",\n   
+00003be0: 2073 7562 646f 6d61 696e 3d22 6d61 6e67   subdomain="mang
+00003bf0: 6f2e 6672 7569 7473 2e63 6f6d 222c 5c6e  o.fruits.com",\n
+00003c00: 2020 2020 7761 6e5f 6564 6765 5f66 6f72      wan_edge_for
+00003c10: 6563 6173 743d 3130 302c 5c6e 2020 2020  ecast=100,\n    
+00003c20: 6d69 6772 6174 696f 6e5f 6b65 793d 224d  migration_key="M
+00003c30: 616e 676f 5465 6e61 6e74 4d69 6772 6174  angoTenantMigrat
+00003c40: 696f 6e4b 6579 222c 2020 2023 206f 6e6c  ionKey",   # onl
+00003c50: 7920 666f 7220 5344 5741 4e20 4d61 6e61  y for SDWAN Mana
+00003c60: 6765 7220 3e3d 2032 302e 3133 5c6e 2020  ger >= 20.13\n  
+00003c70: 2020 6973 5f64 6573 7469 6e61 7469 6f6e    is_destination
+00003c80: 5f6f 7665 726c 6179 5f6d 743d 5472 7565  _overlay_mt=True
+00003c90: 2c20 2020 2020 2020 2020 2020 2023 206f  ,            # o
+00003ca0: 6e6c 7920 666f 7220 5344 5741 4e20 4d61  nly for SDWAN Ma
+00003cb0: 6e61 6765 7220 3e3d 2032 302e 3133 5c6e  nager >= 20.13\n
+00003cc0: 295c 6e5c 6e77 6974 6820 6372 6561 7465  )\n\nwith create
+00003cd0: 5f6d 616e 6167 6572 5f73 6573 7369 6f6e  _manager_session
+00003ce0: 2875 726c 3d22 3130 2e30 2e31 2e31 3522  (url="10.0.1.15"
+00003cf0: 2c20 7573 6572 6e61 6d65 3d22 7374 2d61  , username="st-a
+00003d00: 646d 696e 222c 2070 6173 7377 6f72 643d  dmin", password=
+00003d10: 2222 2920 6173 206f 7269 6769 6e5f 7365  "") as origin_se
+00003d20: 7373 696f 6e2c 205c 5c5c 6e20 2020 2020  ssion, \\\n     
+00003d30: 6372 6561 7465 5f6d 616e 6167 6572 5f73  create_manager_s
+00003d40: 6573 7369 6f6e 2875 726c 3d22 3130 2e39  ession(url="10.9
+00003d50: 2e30 2e31 3622 2c20 7573 6572 6e61 6d65  .0.16", username
+00003d60: 3d22 6d74 2d70 726f 7669 6465 722d 6164  ="mt-provider-ad
+00003d70: 6d69 6e22 2c20 7061 7373 776f 7264 3d22  min", password="
+00003d80: 2229 2061 7320 7461 7267 6574 5f73 6573  ") as target_ses
+00003d90: 7369 6f6e 3a5c 6e20 2020 206d 6967 7261  sion:\n    migra
+00003da0: 7469 6f6e 5f77 6f72 6b66 6c6f 7728 5c6e  tion_workflow(\n
+00003db0: 2020 2020 2020 2020 6f72 6967 696e 5f73          origin_s
+00003dc0: 6573 7369 6f6e 3d6f 7269 6769 6e5f 7365  ession=origin_se
+00003dd0: 7373 696f 6e2c 5c6e 2020 2020 2020 2020  ssion,\n        
+00003de0: 7461 7267 6574 5f73 6573 7369 6f6e 3d74  target_session=t
+00003df0: 6172 6765 745f 7365 7373 696f 6e2c 5c6e  arget_session,\n
+00003e00: 2020 2020 2020 2020 776f 726b 6469 723d          workdir=
+00003e10: 5061 7468 2822 776f 726b 6469 7222 292c  Path("workdir"),
+00003e20: 5c6e 2020 2020 2020 2020 7465 6e61 6e74  \n        tenant
+00003e30: 3d74 656e 616e 742c 5c6e 2020 2020 2020  =tenant,\n      
+00003e40: 2020 7661 6c69 6461 746f 723d 2231 302e    validator="10.
+00003e50: 392e 3132 2e32 3622 5c6e 2020 2020 295c  9.12.26"\n    )\
+00003e60: 6e60 6060 5c6e 5c6e 606d 6967 7261 7469  n```\n\n`migrati
+00003e70: 6f6e 5f77 6f72 6b66 6c6f 7760 2070 6572  on_workflow` per
+00003e80: 666f 726d 7320 6d75 6c74 692d 7374 6570  forms multi-step
+00003e90: 206d 6967 7261 7469 6f6e 2070 726f 6365   migration proce
+00003ea0: 6475 7265 2061 6363 6f72 6469 6e67 2074  dure according t
+00003eb0: 6f20 5b4d 6967 7261 7465 2053 696e 676c  o [Migrate Singl
+00003ec0: 652d 5465 6e61 6e74 2043 6973 636f 2053  e-Tenant Cisco S
+00003ed0: 442d 5741 4e20 4f76 6572 6c61 7920 746f  D-WAN Overlay to
+00003ee0: 204d 756c 7469 7465 6e61 6e74 2043 6973   Multitenant Cis
+00003ef0: 636f 2053 442d 5741 4e20 4465 706c 6f79  co SD-WAN Deploy
+00003f00: 6d65 6e74 5d28 6874 7470 733a 2f2f 7777  ment](https://ww
+00003f10: 772e 6369 7363 6f2e 636f 6d2f 632f 656e  w.cisco.com/c/en
+00003f20: 2f75 732f 7464 2f64 6f63 732f 726f 7574  /us/td/docs/rout
+00003f30: 6572 732f 7364 7761 6e2f 636f 6e66 6967  ers/sdwan/config
+00003f40: 7572 6174 696f 6e2f 7379 7374 656d 2d69  uration/system-i
+00003f50: 6e74 6572 6661 6365 2f76 6564 6765 2d32  nterface/vedge-2
+00003f60: 302d 782f 7379 7374 656d 732d 696e 7465  0-x/systems-inte
+00003f70: 7266 6163 6573 2d62 6f6f 6b2f 7364 7761  rfaces-book/sdwa
+00003f80: 6e2d 6d75 6c74 6974 656e 616e 6379 2e68  n-multitenancy.h
+00003f90: 746d 6c23 636f 6e63 6570 745f 736a 6a5f  tml#concept_sjj_
+00003fa0: 6a6d 6d5f 7a34 6229 5c6e 5c6e 5c6e 5369  jmm_z4b)\n\n\nSi
+00003fb0: 6e63 6520 3230 2e31 3320 616c 736f 204d  nce 20.13 also M
+00003fc0: 5420 746f 2053 5420 6973 2073 7570 706f  T to ST is suppo
+00003fd0: 7274 6564 2028 6a75 7374 2070 726f 7669  rted (just provi
+00003fe0: 6465 2073 7569 7461 626c 6520 6f72 6967  de suitable orig
+00003ff0: 696e 2f74 6172 6765 7420 7365 7373 696f  in/target sessio
+00004000: 6e73 2c20 616e 6420 6069 735f 6465 7374  ns, and `is_dest
+00004010: 696e 6174 696f 6e5f 6f76 6572 6c61 795f  ination_overlay_
+00004020: 6d74 6020 7061 7261 6d65 7465 7229 5c6e  mt` parameter)\n
+00004030: 5c6e 5c6e 4561 6368 2073 7465 7020 6f66  \n\nEach step of
+00004040: 2074 6865 2060 6d69 6772 6174 696f 6e5f   the `migration_
+00004050: 776f 726b 666c 6f77 6020 7072 6f63 6564  workflow` proced
+00004060: 7572 6520 6361 6e20 6265 2065 7865 6375  ure can be execu
+00004070: 7465 6420 696e 6465 7065 6e64 656e 746c  ted independentl
+00004080: 7920 7573 696e 6720 6170 6920 6d65 7468  y using api meth
+00004090: 6f64 733a 2060 6578 706f 7274 5f74 656e  ods: `export_ten
+000040a0: 616e 7460 2c20 6064 6f77 6e6c 6f61 6460  ant`, `download`
+000040b0: 2c20 6069 6d70 6f72 745f 7465 6e61 6e74  , `import_tenant
+000040c0: 602c 2060 7374 6f72 655f 746f 6b65 6e60  `, `store_token`
+000040d0: 2c20 606d 6967 7261 7465 5f6e 6574 776f  , `migrate_netwo
+000040e0: 726b 605c 6e5c 6e60 6060 7079 7468 6f6e  rk`\n\n```python
+000040f0: 5c6e 6f72 6967 696e 5f61 7069 203d 206f  \norigin_api = o
+00004100: 7269 6769 6e5f 7365 7373 696f 6e2e 6170  rigin_session.ap
+00004110: 692e 7465 6e61 6e74 5f6d 6967 7261 7469  i.tenant_migrati
+00004120: 6f6e 5f61 7069 5c6e 7461 7267 6574 5f61  on_api\ntarget_a
+00004130: 7069 203d 2074 6172 6765 745f 7365 7373  pi = target_sess
+00004140: 696f 6e2e 6170 692e 7465 6e61 6e74 5f6d  ion.api.tenant_m
+00004150: 6967 7261 7469 6f6e 5f61 7069 5c6e 7465  igration_api\nte
+00004160: 6e61 6e74 5f66 696c 6520 3d20 5061 7468  nant_file = Path
+00004170: 2822 7e2f 7465 6e61 6e74 2e74 6172 2e67  ("~/tenant.tar.g
+00004180: 7a22 295c 6e74 6f6b 656e 5f66 696c 6520  z")\ntoken_file 
+00004190: 3d20 5061 7468 2822 7e2f 7465 6e61 6e74  = Path("~/tenant
+000041a0: 2d74 6f6b 656e 2e74 7874 2229 5c6e 2320  -token.txt")\n# 
+000041b0: 6578 706f 7274 5c6e 6578 706f 7274 5f74  export\nexport_t
+000041c0: 6173 6b20 3d20 6f72 6967 696e 5f61 7069  ask = origin_api
+000041d0: 2e65 7870 6f72 745f 7465 6e61 6e74 2874  .export_tenant(t
+000041e0: 656e 616e 743d 7465 6e61 6e74 295c 6e72  enant=tenant)\nr
+000041f0: 656d 6f74 655f 6669 6c65 6e61 6d65 203d  emote_filename =
+00004200: 2065 7870 6f72 745f 7461 736b 2e77 6169   export_task.wai
+00004210: 745f 666f 725f 6669 6c65 2829 5c6e 2320  t_for_file()\n# 
+00004220: 646f 776e 6c6f 6164 5c6e 6f72 6967 696e  download\norigin
+00004230: 5f61 7069 2e64 6f77 6e6c 6f61 6428 6578  _api.download(ex
+00004240: 706f 7274 5f70 6174 682c 2072 656d 6f74  port_path, remot
+00004250: 655f 6669 6c65 6e61 6d65 295c 6e23 2069  e_filename)\n# i
+00004260: 6d70 6f72 745c 6e69 6d70 6f72 745f 7461  mport\nimport_ta
+00004270: 736b 203d 2074 6172 6765 745f 6170 692e  sk = target_api.
+00004280: 696d 706f 7274 5f74 656e 616e 7428 6578  import_tenant(ex
+00004290: 706f 7274 5f70 6174 682c 2074 656e 616e  port_path, tenan
+000042a0: 742e 6d69 6772 6174 696f 6e5f 6b65 7929  t.migration_key)
+000042b0: 5c6e 696d 706f 7274 5f74 6173 6b2e 7761  \nimport_task.wa
+000042c0: 6974 5f66 6f72 5f63 6f6d 706c 6574 6564  it_for_completed
+000042d0: 2829 5c6e 2320 6765 7420 746f 6b65 6e5c  ()\n# get token\
+000042e0: 6e6d 6967 7261 7469 6f6e 5f69 6420 3d20  nmigration_id = 
+000042f0: 696d 706f 7274 5f74 6173 6b2e 696d 706f  import_task.impo
+00004300: 7274 5f69 6e66 6f2e 6d69 6772 6174 696f  rt_info.migratio
+00004310: 6e5f 746f 6b65 6e5f 7175 6572 795f 7061  n_token_query_pa
+00004320: 7261 6d73 2e6d 6967 7261 7469 6f6e 5f69  rams.migration_i
+00004330: 645c 6e74 6172 6765 745f 6170 692e 7374  d\ntarget_api.st
+00004340: 6f72 655f 746f 6b65 6e28 6d69 6772 6174  ore_token(migrat
+00004350: 696f 6e5f 6964 2c20 746f 6b65 6e5f 7061  ion_id, token_pa
+00004360: 7468 295c 6e23 206d 6967 7261 7465 206e  th)\n# migrate n
+00004370: 6574 776f 726b 5c6e 6d69 6772 6174 655f  etwork\nmigrate_
+00004380: 7461 736b 203d 206f 7269 6769 6e5f 6170  task = origin_ap
+00004390: 692e 6d69 6772 6174 655f 6e65 7477 6f72  i.migrate_networ
+000043a0: 6b28 746f 6b65 6e5f 7061 7468 295c 6e6d  k(token_path)\nm
+000043b0: 6967 7261 7465 5f74 6173 6b2e 7761 6974  igrate_task.wait
+000043c0: 5f66 6f72 5f63 6f6d 706c 6574 6564 2829  _for_completed()
+000043d0: 5c6e 6060 605c 6e3c 2f64 6574 6169 6c73  \n```\n</details
+000043e0: 3e5c 6e5c 6e23 2323 204e 6f74 653a 5c6e  >\n\n### Note:\n
+000043f0: 546f 2072 656d 6f76 6520 6049 6e73 6563  To remove `Insec
+00004400: 7572 6552 6571 7565 7374 5761 726e 696e  ureRequestWarnin
+00004410: 6760 2c20 796f 7520 6361 6e20 696e 636c  g`, you can incl
+00004420: 7564 6520 696e 2079 6f75 7220 7363 7269  ude in your scri
+00004430: 7074 7320 2877 6172 6e69 6e67 2069 7320  pts (warning is 
+00004440: 7375 7070 7265 7373 6564 2077 6865 6e20  suppressed when 
+00004450: 6063 6174 616c 7973 7477 616e 5f64 6576  `catalystwan_dev
+00004460: 656c 6020 656e 7669 726f 6e6d 656e 7420  el` environment 
+00004470: 7661 7269 6162 6c65 2069 7320 7365 7429  variable is set)
+00004480: 3a5c 6e60 6060 5079 7468 6f6e 5c6e 696d  :\n```Python\nim
+00004490: 706f 7274 2075 726c 6c69 6233 5c6e 7572  port urllib3\nur
+000044a0: 6c6c 6962 332e 6469 7361 626c 655f 7761  llib3.disable_wa
+000044b0: 726e 696e 6773 2875 726c 6c69 6233 2e65  rnings(urllib3.e
+000044c0: 7863 6570 7469 6f6e 732e 496e 7365 6375  xceptions.Insecu
+000044d0: 7265 5265 7175 6573 7457 6172 6e69 6e67  reRequestWarning
+000044e0: 295c 6e60 6060 5c6e 5c6e 2323 2043 6174  )\n```\n\n## Cat
+000044f0: 6368 696e 6720 4578 6365 7074 696f 6e73  ching Exceptions
+00004500: 5c6e 6060 6070 7974 686f 6e5c 6e74 7279  \n```python\ntry
+00004510: 3a5c 6e20 2020 2073 6573 7369 6f6e 2e61  :\n    session.a
+00004520: 7069 2e75 7365 7273 2e64 656c 6574 6528  pi.users.delete(
+00004530: 2262 6f67 7573 2d75 7365 722d 6e61 6d65  "bogus-user-name
+00004540: 2229 5c6e 6578 6365 7074 204d 616e 6167  ")\nexcept Manag
+00004550: 6572 4854 5450 4572 726f 7220 6173 2065  erHTTPError as e
+00004560: 7272 6f72 3a5c 6e20 2020 2023 2050 726f  rror:\n    # Pro
+00004570: 6365 7373 2061 6e20 6572 726f 722e 5c6e  cess an error.\n
+00004580: 2020 2020 7072 696e 7428 6572 726f 722e      print(error.
+00004590: 7265 7370 6f6e 7365 2e73 7461 7475 735f  response.status_
+000045a0: 636f 6465 295c 6e20 2020 2070 7269 6e74  code)\n    print
+000045b0: 2865 7272 6f72 2e69 6e66 6f2e 636f 6465  (error.info.code
+000045c0: 295c 6e20 2020 2070 7269 6e74 2865 7272  )\n    print(err
+000045d0: 6f72 2e69 6e66 6f2e 6d65 7373 6167 6529  or.info.message)
+000045e0: 5c6e 2020 2020 7072 696e 7428 6572 726f  \n    print(erro
+000045f0: 722e 696e 666f 2e64 6574 6169 6c73 295c  r.info.details)\
+00004600: 6e5c 6e60 6060 5c6e 5c6e 2323 205b 5375  n\n```\n\n## [Su
+00004610: 7070 6f72 7465 6420 4150 4920 656e 6470  pported API endp
+00004620: 6f69 6e74 735d 2868 7474 7073 3a2f 2f67  oints](https://g
+00004630: 6974 6875 622e 636f 6d2f 6369 7363 6f2d  ithub.com/cisco-
+00004640: 6f70 656e 2f63 6973 636f 2d63 6174 616c  open/cisco-catal
+00004650: 7973 742d 7761 6e2d 7364 6b2f 626c 6f62  yst-wan-sdk/blob
+00004660: 2f6d 6169 6e2f 454e 4450 4f49 4e54 532e  /main/ENDPOINTS.
+00004670: 6d64 295c 6e5c 6e5c 6e23 2320 5b43 6f6e  md)\n\n\n## [Con
+00004680: 7472 6962 7574 696e 672c 2062 7567 2072  tributing, bug r
+00004690: 6570 6f72 7469 6e67 2061 6e64 2066 6561  eporting and fea
+000046a0: 7475 7265 2072 6571 7565 7374 735d 2868  ture requests](h
+000046b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000046c0: 6d2f 6369 7363 6f2d 6f70 656e 2f63 6973  m/cisco-open/cis
+000046d0: 636f 2d63 6174 616c 7973 742d 7761 6e2d  co-catalyst-wan-
+000046e0: 7364 6b2f 626c 6f62 2f6d 6169 6e2f 434f  sdk/blob/main/CO
+000046f0: 4e54 5249 4255 5449 4e47 2e6d 6429 5c6e  NTRIBUTING.md)\n
+00004700: 5c6e 2323 2053 6565 6b69 6e67 2073 7570  \n## Seeking sup
+00004710: 706f 7274 5c6e 5c6e 596f 7520 6361 6e20  port\n\nYou can 
+00004720: 636f 6e74 6163 7420 7573 2062 7920 7375  contact us by su
+00004730: 626d 6974 7469 6e67 205b 6973 7375 6573  bmitting [issues
+00004740: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004750: 2e63 6f6d 2f63 6973 636f 2d6f 7065 6e2f  .com/cisco-open/
+00004760: 6369 7363 6f2d 6361 7461 6c79 7374 2d77  cisco-catalyst-w
+00004770: 616e 2d73 646b 2f69 7373 7565 7329 2c20  an-sdk/issues), 
+00004780: 6f72 2064 6972 6563 746c 7920 7669 6120  or directly via 
+00004790: 6d61 696c 206f 6e20 6361 7461 6c79 7374  mail on catalyst
+000047a0: 7761 6e40 6369 7363 6f2e 636f 6d2e 5c6e  wan@cisco.com.\n
+000047b0: 272c 0a20 2020 2027 6175 7468 6f72 273a  ',.    'author':
+000047c0: 2027 6b61 676f 7273 6b69 272c 0a20 2020   'kagorski',.   
+000047d0: 2027 6175 7468 6f72 5f65 6d61 696c 273a   'author_email':
+000047e0: 2027 6b61 676f 7273 6b69 4063 6973 636f   'kagorski@cisco
+000047f0: 2e63 6f6d 272c 0a20 2020 2027 6d61 696e  .com',.    'main
+00004800: 7461 696e 6572 273a 2027 4e6f 6e65 272c  tainer': 'None',
+00004810: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
+00004820: 5f65 6d61 696c 273a 2027 4e6f 6e65 272c  _email': 'None',
+00004830: 0a20 2020 2027 7572 6c27 3a20 2768 7474  .    'url': 'htt
+00004840: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004850: 6369 7363 6f2d 6f70 656e 2f63 6973 636f  cisco-open/cisco
+00004860: 2d63 6174 616c 7973 742d 7761 6e2d 7364  -catalyst-wan-sd
+00004870: 6b27 2c0a 2020 2020 2770 6163 6b61 6765  k',.    'package
+00004880: 7327 3a20 7061 636b 6167 6573 2c0a 2020  s': packages,.  
+00004890: 2020 2770 6163 6b61 6765 5f64 6174 6127    'package_data'
+000048a0: 3a20 7061 636b 6167 655f 6461 7461 2c0a  : package_data,.
+000048b0: 2020 2020 2769 6e73 7461 6c6c 5f72 6571      'install_req
+000048c0: 7569 7265 7327 3a20 696e 7374 616c 6c5f  uires': install_
+000048d0: 7265 7175 6972 6573 2c0a 2020 2020 2770  requires,.    'p
+000048e0: 7974 686f 6e5f 7265 7175 6972 6573 273a  ython_requires':
+000048f0: 2027 3e3d 332e 382e 302c 3c34 2e30 2e30   '>=3.8.0,<4.0.0
+00004900: 272c 0a7d 0a0a 0a73 6574 7570 282a 2a73  ',.}...setup(**s
+00004910: 6574 7570 5f6b 7761 7267 7329 0a         etup_kwargs).
```

### Comparing `catalystwan-0.33.7/PKG-INFO` & `catalystwan-0.33.7.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystwan
-Version: 0.33.7
+Version: 0.33.7.dev0
 Summary: Cisco Catalyst WAN SDK for Python
 Home-page: https://github.com/cisco-open/cisco-catalyst-wan-sdk
 Author: kagorski
 Author-email: kagorski@cisco.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: attrs (>=21.4.0,<22.0.0)
 Requires-Dist: ciscoconfparse (==1.9.41)
 Requires-Dist: clint (>=0.5.1,<0.6.0)
 Requires-Dist: flake8-quotes (>=3.3.1,<4.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
-Requires-Dist: pydantic (>=2.5,<3.0)
+Requires-Dist: pydantic (>=2.7,<3.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Requires-Dist: typing-extensions (>=4.6.1,<5.0.0)
 Project-URL: Repository, https://github.com/cisco-open/cisco-catalyst-wan-sdk
 Description-Content-Type: text/markdown
@@ -206,30 +206,28 @@
 n = 24
 alarms_from_n_hours = session.api.alarms.get(from_time=n)
 ```
 
 To get all critical alarms from past `n` hours:
 
 ```python
-from catalystwan.utils.alarm_status import Severity
 n = 48
 critical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)
 ```
 
 </details>
 
 <details>
     <summary> <b>Users</b> <i>(click to expand)</i></summary>
 
 ```python
 # Get all users
 session.api.users.get()
 
 # Create user
-from catalystwan.endpoints.administration_user_and_group import User
 new_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")
 session.api.users.create(new_user)
 
 # Update user data
 new_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")
 session.api.users.update(new_user_update)
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: catalystwan Version: 0.33.7 Summary: Cisco Catalyst
-WAN SDK for Python Home-page: https://github.com/cisco-open/cisco-catalyst-wan-
-sdk Author: kagorski Author-email: kagorski@cisco.com Requires-Python:
->=3.8.0,<4.0.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: attrs (>=21.4.0,<22.0.0) Requires-Dist: ciscoconfparse
-(==1.9.41) Requires-Dist: clint (>=0.5.1,<0.6.0) Requires-Dist: flake8-quotes
-(>=3.3.1,<4.0.0) Requires-Dist: packaging (>=23.0,<24.0) Requires-Dist:
-pydantic (>=2.5,<3.0) Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-
-Dist: requests (>=2.27.1,<3.0.0) Requires-Dist: requests-toolbelt
-(>=1.0.0,<2.0.0) Requires-Dist: tenacity (>=8.1.0,<9.0.0) Requires-Dist:
-typing-extensions (>=4.6.1,<5.0.0) Project-URL: Repository, https://github.com/
-cisco-open/cisco-catalyst-wan-sdk Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: catalystwan Version: 0.33.7.dev0 Summary: Cisco
+Catalyst WAN SDK for Python Home-page: https://github.com/cisco-open/cisco-
+catalyst-wan-sdk Author: kagorski Author-email: kagorski@cisco.com Requires-
+Python: >=3.8.0,<4.0.0 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Jinja2
+(>=3.1.2,<4.0.0) Requires-Dist: attrs (>=21.4.0,<22.0.0) Requires-Dist:
+ciscoconfparse (==1.9.41) Requires-Dist: clint (>=0.5.1,<0.6.0) Requires-Dist:
+flake8-quotes (>=3.3.1,<4.0.0) Requires-Dist: packaging (>=23.0,<24.0)
+Requires-Dist: pydantic (>=2.7,<3.0) Requires-Dist: python-dateutil
+(>=2.8.2,<3.0.0) Requires-Dist: requests (>=2.27.1,<3.0.0) Requires-Dist:
+requests-toolbelt (>=1.0.0,<2.0.0) Requires-Dist: tenacity (>=8.1.0,<9.0.0)
+Requires-Dist: typing-extensions (>=4.6.1,<5.0.0) Project-URL: Repository,
+https://github.com/cisco-open/cisco-catalyst-wan-sdk Description-Content-Type:
+text/markdown
                          _[_C_i_s_c_o_ _C_a_t_a_l_y_s_t_ _W_A_N_ _S_D_K_ _L_o_g_o_]
 [![Python-Supported](https://img.shields.io/static/
 v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)]
 (https://www.python.org/) Cisco Catalyst WAN SDK is a package for creating
 simple and parallel automatic requests via official SD-WAN Manager API. It is
 intended to serve as a multiple session handler (provider, provider as a
 tenant, tenant). The library is not dependent on environment which is being run
@@ -87,20 +88,18 @@
 session.api.repository.upload_image(image) # Install software install_task =
 session.api.software.install(devices=vsmarts, image=image) # Check action
 status install_task.wait_for_completed() ``` GGeett aallaarrmmss (click to expand) To
 get all alarms: ```python alarms = session.api.alarms.get() ``` To get all not
 viewed alarms: ```python not_viewed_alarms = session.api.alarms.get().filter
 (viewed=False) ``` To get all alarms from past `n` hours: ```python n = 24
 alarms_from_n_hours = session.api.alarms.get(from_time=n) ``` To get all
-critical alarms from past `n` hours: ```python from
-catalystwan.utils.alarm_status import Severity n = 48 critical_alarms =
+critical alarms from past `n` hours: ```python n = 48 critical_alarms =
 session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL) ```
 UUsseerrss (click to expand) ```python # Get all users session.api.users.get() #
-Create user from catalystwan.endpoints.administration_user_and_group import
-User new_user = User(username="new_user", password="new_user", group=
+Create user new_user = User(username="new_user", password="new_user", group=
 ["netadmin"], description="new user") session.api.users.create(new_user) #
 Update user data new_user_update = UserUpdateRequest(username="new_user",
 group=["netadmin", "netops"], locale="en_US", description="updated-new_user-
 description") session.api.users.update(new_user_update) # Update user password
 session.api.users.update_password("new_user", "n3W-P4s$w0rd") # Reset user
 session.api.users.reset("new_user") # Delete user session.api.users.delete
 ("new_user") # Get current user authentication type and role
```

