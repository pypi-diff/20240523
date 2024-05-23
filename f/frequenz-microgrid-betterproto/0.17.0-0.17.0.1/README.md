# Comparing `tmp/frequenz-microgrid-betterproto-0.17.0.tar.gz` & `tmp/frequenz-microgrid-betterproto-0.17.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-microgrid-betterproto-0.17.0.tar", last modified: Thu May 16 13:13:26 2024, max compression
+gzip compressed data, was "frequenz-microgrid-betterproto-0.17.0.1.tar", last modified: Thu May 23 10:06:29 2024, max compression
```

## Comparing `frequenz-microgrid-betterproto-0.17.0.tar` & `frequenz-microgrid-betterproto-0.17.0.1.tar`

### file list

```diff
@@ -1,137 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.591244 frequenz-microgrid-betterproto-0.17.0/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-16 13:13:10.000000 frequenz-microgrid-betterproto-0.17.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 13:13:10.000000 frequenz-microgrid-betterproto-0.17.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 13:13:10.000000 frequenz-microgrid-betterproto-0.17.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-16 13:13:26.591244 frequenz-microgrid-betterproto-0.17.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 13:13:10.000000 frequenz-microgrid-betterproto-0.17.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-16 13:13:10.000000 frequenz-microgrid-betterproto-0.17.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/proto/frequenz/api/microgrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.579244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/proto/frequenz/api/microgrid/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-05-16 13:13:11.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/proto/frequenz/api/microgrid/v1/microgrid.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.583244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.583244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.583244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    41483 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.583244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.583244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.583244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.587244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.587244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.587244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.587244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/timeofday.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.575245 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.587244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.587244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.587244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.587244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.587244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.591244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.591244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.591244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
--rw-r--r--   0 runner    (1001) docker     (127)    17610 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.591244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.591244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.591244 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-16 13:13:12.000000 frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/decimal.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-16 13:13:10.000000 frequenz-microgrid-betterproto-0.17.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:13:26.591244 frequenz-microgrid-betterproto-0.17.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.579244 frequenz-microgrid-betterproto-0.17.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.579244 frequenz-microgrid-betterproto-0.17.0/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.579244 frequenz-microgrid-betterproto-0.17.0/src/frequenz/microgrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.591244 frequenz-microgrid-betterproto-0.17.0/src/frequenz/microgrid/betterproto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:10.000000 frequenz-microgrid-betterproto-0.17.0/src/frequenz/microgrid/betterproto/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:13:26.591244 frequenz-microgrid-betterproto-0.17.0/src/frequenz_microgrid_betterproto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-16 13:13:26.000000 frequenz-microgrid-betterproto-0.17.0/src/frequenz_microgrid_betterproto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-05-16 13:13:26.000000 frequenz-microgrid-betterproto-0.17.0/src/frequenz_microgrid_betterproto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:13:26.000000 frequenz-microgrid-betterproto-0.17.0/src/frequenz_microgrid_betterproto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-16 13:13:26.000000 frequenz-microgrid-betterproto-0.17.0/src/frequenz_microgrid_betterproto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 13:13:26.000000 frequenz-microgrid-betterproto-0.17.0/src/frequenz_microgrid_betterproto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.521395 frequenz-microgrid-betterproto-0.17.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-23 10:06:17.000000 frequenz-microgrid-betterproto-0.17.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-23 10:06:17.000000 frequenz-microgrid-betterproto-0.17.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-23 10:06:29.521395 frequenz-microgrid-betterproto-0.17.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-23 10:06:17.000000 frequenz-microgrid-betterproto-0.17.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-23 10:06:17.000000 frequenz-microgrid-betterproto-0.17.0.1/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.477395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.477395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.477395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.477395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.477395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/proto/frequenz/api/microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.477395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/proto/frequenz/api/microgrid/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-05-23 10:06:29.477395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/proto/frequenz/api/microgrid/v1/microgrid.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.477395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/backend.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/billing.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/client.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/config_change.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/consumer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/control.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/distribution.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/documentation.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/endpoint.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/field_behavior.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/httpbody.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/label.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/launch_stage.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/log.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/logging.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/metric.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitored_resource.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitoring.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/quota.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/resource.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/routing.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/service.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/source_info.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/system_parameter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/usage.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/cloud/extended_operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    41483 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/v1/iam.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/iam_policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/options.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/logging/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/http_request.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/log_severity.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/longrunning/
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/longrunning/operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/code.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/context/
+-rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/context/attribute_context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/error_details.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/status.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/calendar_period.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/color.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/date.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/datetime.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/dayofweek.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/expr.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/fraction.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-23 10:06:29.481395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/latlng.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/money.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/month.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/postal_address.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/quaternion.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-23 10:06:29.485395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    17610 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-23 10:06:29.489395 frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/decimal.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-23 10:06:17.000000 frequenz-microgrid-betterproto-0.17.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 10:06:29.521395 frequenz-microgrid-betterproto-0.17.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.517395 frequenz-microgrid-betterproto-0.17.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.517395 frequenz-microgrid-betterproto-0.17.0.1/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.517395 frequenz-microgrid-betterproto-0.17.0.1/src/frequenz/microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.517395 frequenz-microgrid-betterproto-0.17.0.1/src/frequenz/microgrid/betterproto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:17.000000 frequenz-microgrid-betterproto-0.17.0.1/src/frequenz/microgrid/betterproto/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:06:29.521395 frequenz-microgrid-betterproto-0.17.0.1/src/frequenz_microgrid_betterproto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-23 10:06:29.000000 frequenz-microgrid-betterproto-0.17.0.1/src/frequenz_microgrid_betterproto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-23 10:06:29.000000 frequenz-microgrid-betterproto-0.17.0.1/src/frequenz_microgrid_betterproto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:06:29.000000 frequenz-microgrid-betterproto-0.17.0.1/src/frequenz_microgrid_betterproto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-23 10:06:29.000000 frequenz-microgrid-betterproto-0.17.0.1/src/frequenz_microgrid_betterproto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 10:06:29.000000 frequenz-microgrid-betterproto-0.17.0.1/src/frequenz_microgrid_betterproto.egg-info/top_level.txt
```

### Comparing `frequenz-microgrid-betterproto-0.17.0/LICENSE` & `frequenz-microgrid-betterproto-0.17.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/PKG-INFO` & `frequenz-microgrid-betterproto-0.17.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-microgrid-betterproto
-Version: 0.17.0
+Version: 0.17.0.1
 Summary: Bindings to the microgrid API generated using betterproto
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-microgrid-betterproto-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-microgrid-betterproto-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-microgrid-betterproto-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-microgrid-betterproto-python
```

### Comparing `frequenz-microgrid-betterproto-0.17.0/README.md` & `frequenz-microgrid-betterproto-0.17.0.1/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/proto/frequenz/api/microgrid/v1/microgrid.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/proto/frequenz/api/microgrid/v1/microgrid.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/annotations.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/auth.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/auth.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/backend.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/backend.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/billing.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/billing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/client.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/config_change.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/config_change.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/consumer.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/consumer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/context.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/control.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/control.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/distribution.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/distribution.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/documentation.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/documentation.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/endpoint.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/endpoint.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/field_behavior.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/http.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/httpbody.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/label.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/label.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/launch_stage.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/launch_stage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/log.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/log.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/logging.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/logging.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/metric.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/metric.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitored_resource.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitored_resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitoring.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitoring.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/quota.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/quota.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/resource.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/routing.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/service.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/service.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/source_info.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/source_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/system_parameter.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/system_parameter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/usage.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/api/usage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/cloud/extended_operations.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/v1/iam.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/v1/iam.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/iam_policy.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/iam_policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/options.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/options.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/policy.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/http_request.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/http_request.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/log_severity.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/log_severity.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/longrunning/operations.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/code.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/context/attribute_context.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/error_details.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/status.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/calendar_period.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/calendar_period.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/color.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/color.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/date.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/date.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/datetime.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/datetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/dayofweek.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/expr.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/expr.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/fraction.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/fraction.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/latlng.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/latlng.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/money.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/money.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/month.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/month.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/postal_address.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/postal_address.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/quaternion.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/quaternion.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/timeofday.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/api-common-protos/google/type/timeofday.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/decimal.proto` & `frequenz-microgrid-betterproto-0.17.0.1/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/decimal.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.17.0/pyproject.toml` & `frequenz-microgrid-betterproto-0.17.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # License: MIT
 # Copyright © 2024 Frequenz Energy-as-a-Service GmbH
 
 [build-system]
 requires = [
   "setuptools == 68.1.0",
   "setuptools_scm[toml] == 7.1.0",
-  "setuptools-betterproto == 0.1.0",
+  "setuptools-betterproto == 0.2.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-microgrid-betterproto"
 description = "Bindings to the microgrid API generated using betterproto"
 readme = "README.md"
```

### Comparing `frequenz-microgrid-betterproto-0.17.0/src/frequenz_microgrid_betterproto.egg-info/PKG-INFO` & `frequenz-microgrid-betterproto-0.17.0.1/src/frequenz_microgrid_betterproto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-microgrid-betterproto
-Version: 0.17.0
+Version: 0.17.0.1
 Summary: Bindings to the microgrid API generated using betterproto
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-microgrid-betterproto-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-microgrid-betterproto-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-microgrid-betterproto-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-microgrid-betterproto-python
```

### Comparing `frequenz-microgrid-betterproto-0.17.0/src/frequenz_microgrid_betterproto.egg-info/requires.txt` & `frequenz-microgrid-betterproto-0.17.0.1/src/frequenz_microgrid_betterproto.egg-info/requires.txt`

 * *Files identical despite different names*

