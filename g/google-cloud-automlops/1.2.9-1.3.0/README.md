# Comparing `tmp/google-cloud-automlops-1.2.9.tar.gz` & `tmp/google_cloud_automlops-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-automlops-1.2.9.tar", last modified: Wed Feb 21 21:22:17 2024, max compression
+gzip compressed data, was "google_cloud_automlops-1.3.0.tar", last modified: Thu May 23 13:55:14 2024, max compression
```

## Comparing `google-cloud-automlops-1.2.9.tar` & `google_cloud_automlops-1.3.0.tar`

### file list

```diff
@@ -1,147 +1,125 @@
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.652601 google-cloud-automlops-1.2.9/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google-cloud-automlops-1.2.9/LICENSE
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    34827 2024-02-21 21:22:17.652258 google-cloud-automlops-1.2.9/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    33623 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/README.md
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.626709 google-cloud-automlops-1.2.9/google_cloud_automlops/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    35085 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/AutoMLOps.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.628902 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.629280 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/cloudbuild/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/cloudbuild/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3937 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/cloudbuild/builder.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.629677 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/cloudbuild/templates/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/cloudbuild/templates/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2194 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/cloudbuild/templates/cloudbuild.yaml.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3010 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/configs.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1399 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/enums.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.630151 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/github_actions/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/github_actions/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     5293 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/github_actions/builder.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.630632 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/github_actions/templates/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/github_actions/templates/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3099 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/github_actions/templates/github_actions.yaml.j2
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.631041 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/gitops/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/gitops/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     5384 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/gitops/git_utils.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.631515 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/gitops/templates/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/gitops/templates/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2203 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/gitops/templates/gitignore.j2
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.632142 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1537 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/configs.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1192 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/enums.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.632831 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    24211 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/builder.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    10093 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/scaffold.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.633434 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     5663 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/README.md.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.633660 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/components/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/components/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.634157 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/components/component_base/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      275 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/components/component_base/Dockerfile.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/components/component_base/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.634527 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/components/component_base/src/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/components/component_base/src/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      740 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/components/component_base/src/task.py.j2
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.635479 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/model_monitoring/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/model_monitoring/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    12445 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/model_monitoring/monitor.py.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       72 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/model_monitoring/requirements.txt.j2
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.636266 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/pipelines/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/pipelines/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2511 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/pipelines/pipeline.py.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2875 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/pipelines/pipeline_runner.py.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      107 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/pipelines/requirements.txt.j2
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.637668 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/scripts/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/scripts/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      279 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/scripts/build_components.sh.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      263 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/scripts/build_pipeline_spec.sh.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      285 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/scripts/create_model_monitoring_job.sh.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      344 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/scripts/publish_to_topic.sh.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      511 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/scripts/run_all.sh.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      281 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/scripts/run_pipeline.sh.j2
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.637849 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/services/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/services/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.638813 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/services/submission_service/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      464 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/services/submission_service/Dockerfile.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/services/submission_service/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     6732 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/services/submission_service/main.py.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      266 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/services/submission_service/requirements.txt.j2
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.639664 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     7152 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/configs.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1055 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/enums.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.640101 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/gcloud/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/gcloud/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9770 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/gcloud/builder.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.640779 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/gcloud/templates/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/gcloud/templates/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8959 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/gcloud/templates/provision_resources.sh.j2
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.641472 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/pulumi/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/pulumi/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     6694 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/pulumi/builder.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.641992 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    22055 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/builder.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.642625 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.644950 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      789 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/data.tf.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1010 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/iam.tf.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     7124 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/main.tf.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2405 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/outputs.tf.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      148 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/provider.tf.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1273 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/variables.auto.tfvars.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2433 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/variables.tf.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      364 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/versions.tf.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      389 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/provision_resources.sh.j2
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.645785 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/state_bucket/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/state_bucket/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      976 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/state_bucket/main.tf.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      209 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/state_bucket/variables.auto.tfvars.j2
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      393 2024-01-09 15:22:38.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/state_bucket/variables.tf.j2
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.646647 google-cloud-automlops-1.2.9/google_cloud_automlops/utils/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/utils/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     5868 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/utils/constants.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    51482 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/google_cloud_automlops/utils/utils.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.651798 google-cloud-automlops-1.2.9/google_cloud_automlops.egg-info/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    34827 2024-02-21 21:22:17.000000 google-cloud-automlops-1.2.9/google_cloud_automlops.egg-info/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     6372 2024-02-21 21:22:17.000000 google-cloud-automlops-1.2.9/google_cloud_automlops.egg-info/SOURCES.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2024-02-21 21:22:17.000000 google-cloud-automlops-1.2.9/google_cloud_automlops.egg-info/dependency_links.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      205 2024-02-21 21:22:17.000000 google-cloud-automlops-1.2.9/google_cloud_automlops.egg-info/requires.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       29 2024-02-21 21:22:17.000000 google-cloud-automlops-1.2.9/google_cloud_automlops.egg-info/top_level.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2024-02-21 21:22:17.652660 google-cloud-automlops-1.2.9/setup.cfg
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2258 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/setup.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.647174 google-cloud-automlops-1.2.9/tests/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.647484 google-cloud-automlops-1.2.9/tests/unit/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.647678 google-cloud-automlops-1.2.9/tests/unit/deployments/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/deployments/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.648051 google-cloud-automlops-1.2.9/tests/unit/deployments/cloudbuild/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/deployments/cloudbuild/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     4201 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/deployments/cloudbuild/builder_test.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.648568 google-cloud-automlops-1.2.9/tests/unit/deployments/github_actions/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/deployments/github_actions/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     5025 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/deployments/github_actions/builder_test.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.648861 google-cloud-automlops-1.2.9/tests/unit/orchestration/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/orchestration/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.649542 google-cloud-automlops-1.2.9/tests/unit/orchestration/kfp/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/orchestration/kfp/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    42073 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/orchestration/kfp/builder_test.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11085 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/orchestration/kfp/scaffold_test.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.649923 google-cloud-automlops-1.2.9/tests/unit/provisioning/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/provisioning/__init__.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.650312 google-cloud-automlops-1.2.9/tests/unit/provisioning/gcloud/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/provisioning/gcloud/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    12251 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/provisioning/gcloud/builder_test.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.650886 google-cloud-automlops-1.2.9/tests/unit/provisioning/terraform/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/provisioning/terraform/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    23912 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/provisioning/terraform/builder_test.py
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-02-21 21:22:17.651327 google-cloud-automlops-1.2.9/tests/unit/utils/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/utils/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    19622 2024-02-13 14:12:27.000000 google-cloud-automlops-1.2.9/tests/unit/utils/utils_test.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.876716 google_cloud_automlops-1.3.0/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google_cloud_automlops-1.3.0/LICENSE
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    34889 2024-05-23 13:55:14.876383 google_cloud_automlops-1.3.0/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    33659 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/README.md
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.857467 google_cloud_automlops-1.3.0/google_cloud_automlops/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    32028 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/AutoMLOps.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.859397 google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2170 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/base.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2482 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/cloudbuild.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3712 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/github_actions.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.859562 google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/templates/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/templates/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.859912 google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/templates/cloudbuild/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/templates/cloudbuild/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2194 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/templates/cloudbuild/cloudbuild.yaml.j2
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.860266 google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/templates/github_actions/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/templates/github_actions/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3086 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/templates/github_actions/github_actions.yaml.j2
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.860923 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14664 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/base.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    20669 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/kfp.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.861136 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.861494 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     5663 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/README.md.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.861658 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/components/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/components/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.862000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/components/component_base/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      275 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/components/component_base/Dockerfile.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/components/component_base/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.862326 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/components/component_base/src/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/components/component_base/src/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      687 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/components/component_base/src/task.py.j2
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.862988 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/model_monitoring/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/model_monitoring/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    12445 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/model_monitoring/monitor.py.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       72 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/model_monitoring/requirements.txt.j2
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.863658 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/pipelines/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/pipelines/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2505 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/pipelines/pipeline.py.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2875 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/pipelines/pipeline_runner.py.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      107 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/pipelines/requirements.txt.j2
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.864847 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/scripts/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/scripts/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      279 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/scripts/build_components.sh.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      263 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/scripts/build_pipeline_spec.sh.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      285 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/scripts/create_model_monitoring_job.sh.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      344 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/scripts/publish_to_topic.sh.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      511 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/scripts/run_all.sh.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      281 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/scripts/run_pipeline.sh.j2
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.865040 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/services/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/services/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.865791 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/services/submission_service/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      464 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/services/submission_service/Dockerfile.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/services/submission_service/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     6732 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/services/submission_service/main.py.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      266 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/services/submission_service/requirements.txt.j2
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.866907 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     6032 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/base.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     3600 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/gcloud.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     4659 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/pulumi.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.867391 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.867819 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/gcloud/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/gcloud/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8959 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/gcloud/provision_resources.sh.j2
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.868245 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.869897 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      789 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/data.tf.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1010 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/iam.tf.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     7124 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/main.tf.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2405 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/outputs.tf.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      148 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/provider.tf.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1273 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/variables.auto.tfvars.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2433 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/variables.tf.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      364 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/versions.tf.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      389 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/provision_resources.sh.j2
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.870638 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/state_bucket/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/state_bucket/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      976 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/state_bucket/main.tf.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      209 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/state_bucket/variables.auto.tfvars.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      393 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/state_bucket/variables.tf.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    10991 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/terraform.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.871685 google_cloud_automlops-1.3.0/google_cloud_automlops/utils/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/utils/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     5635 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/utils/constants.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2396 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/utils/enums.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.872247 google_cloud_automlops-1.3.0/google_cloud_automlops/utils/templates/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/utils/templates/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2203 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/utils/templates/gitignore.j2
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    54189 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/google_cloud_automlops/utils/utils.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.875925 google_cloud_automlops-1.3.0/google_cloud_automlops.egg-info/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    34889 2024-05-23 13:55:14.000000 google_cloud_automlops-1.3.0/google_cloud_automlops.egg-info/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     5595 2024-05-23 13:55:14.000000 google_cloud_automlops-1.3.0/google_cloud_automlops.egg-info/SOURCES.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2024-05-23 13:55:14.000000 google_cloud_automlops-1.3.0/google_cloud_automlops.egg-info/dependency_links.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      216 2024-05-23 13:55:14.000000 google_cloud_automlops-1.3.0/google_cloud_automlops.egg-info/requires.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       29 2024-05-23 13:55:14.000000 google_cloud_automlops-1.3.0/google_cloud_automlops.egg-info/top_level.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2024-05-23 13:55:14.876774 google_cloud_automlops-1.3.0/setup.cfg
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2294 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/setup.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.872456 google_cloud_automlops-1.3.0/tests/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google_cloud_automlops-1.3.0/tests/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.872659 google_cloud_automlops-1.3.0/tests/unit/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google_cloud_automlops-1.3.0/tests/unit/__init__.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.873555 google_cloud_automlops-1.3.0/tests/unit/deployments/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google_cloud_automlops-1.3.0/tests/unit/deployments/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     5074 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/tests/unit/deployments/cloudbuild_tests.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     5877 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/tests/unit/deployments/github_actions_tests.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.874192 google_cloud_automlops-1.3.0/tests/unit/orchestration/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google_cloud_automlops-1.3.0/tests/unit/orchestration/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      724 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/tests/unit/orchestration/base_tests.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2237 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/tests/unit/orchestration/kfp_tests.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.875119 google_cloud_automlops-1.3.0/tests/unit/provisioning/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google_cloud_automlops-1.3.0/tests/unit/provisioning/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    12969 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/tests/unit/provisioning/gcloud_tests.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    25249 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/tests/unit/provisioning/terraform_tests.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2024-05-23 13:55:14.875576 google_cloud_automlops-1.3.0/tests/unit/utils/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      596 2024-02-13 14:12:27.000000 google_cloud_automlops-1.3.0/tests/unit/utils/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    16903 2024-05-23 13:54:38.000000 google_cloud_automlops-1.3.0/tests/unit/utils/utils_test.py
```

### Comparing `google-cloud-automlops-1.2.9/LICENSE` & `google_cloud_automlops-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/PKG-INFO` & `google_cloud_automlops-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.2.9
+Version: 1.3.0
 Summary: Build MLOps Pipelines in Minutes.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -20,18 +20,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docopt==0.6.2
 Requires-Dist: docstring-parser==0.15
 Requires-Dist: google-api-python-client==2.97.0
 Requires-Dist: google-auth==2.22.0
 Requires-Dist: importlib-resources==6.0.1
-Requires-Dist: Jinja2==3.1.2
+Requires-Dist: Jinja2==3.1.4
+Requires-Dist: kfp>=2.0.0
 Requires-Dist: packaging==23.1
 Requires-Dist: pipreqs==0.4.13
-Requires-Dist: pydantic==2.3.0
+Requires-Dist: pydantic==2.4.0
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: yarg==0.1.9
 
 # AutoMLOps
 
 AutoMLOps is a service that generates, provisions, deploys, and monitors CI/CD integrated MLOps pipelines, bridging the gap between Data Science and DevOps. AutoMLOps provides a repeatable process that dramatically reduces the time required to build MLOps pipelines. The service generates a containerized MLOps codebase, provides infrastructure-as-code to provision and maintain the underlying MLOps infra, provides deployment functionalities to trigger and run MLOps pipelines, monitoring capabilities to monitor models deployed to live endpoints, and optional automatic retraining of models on a recurring basis or if anomalies are detected during monitoring.
 
@@ -48,14 +49,15 @@
 # Dependencies
 - `docopt==0.6.2`
 - `docstring-parser==0.15`
 - `google-api-python-client==2.97.0`
 - `google-auth==2.22.0`
 - `importlib-resources==6.0.1`
 - `Jinja2==3.1.2`
+- `kfp>=2.0.0`
 - `packaging==23.1`
 - `pipreqs==0.4.13`
 - `pydantic==2.3.0`
 - `PyYAML==6.0.1`
 - `yarg==0.1.9`
 
 # Usage
@@ -115,15 +117,15 @@
 
 **Provisioning Frameworks**: Stands up necessary infra to run MLOps pipelines
 - gcloud
 - terraform
 - [coming soon] pulumi
 
 **Source Code Repositories**: Repository for versioning generated MLOps code
-- Cloud Source Repositories
+- [deprecating soon] Cloud Source Repositories
 - Bitbucket
 - Github
 - Gitlab
 
 # Prerequisites
 ### Generate
 In order to use `AutoMLOps.generate(...)`, the following are required:
@@ -136,15 +138,15 @@
 
 In order to use `AutoMLOps.provision(...)` with `provisioning_framework='terraform'`, the following are recommended:
 - [Terraform v1.5.6](https://www.terraform.io/downloads.html)
 
 ### Deploy
 In order to use `AutoMLOps.deploy(...)` with `use_ci=False`, the following are required:
 - Local python environment with these packages installed:
-    - `kfp<2.0.0`
+    - `kfp>=2.0.0`
     - `google-cloud-aiplatform`
     - `google-cloud-pipeline-components`
     - `google-cloud-storage`
     - `pyyaml`
 
 In order to use `AutoMLOps.deploy(...)` with `use_ci=True`, the following are required:
 - `git` installed
@@ -356,15 +358,15 @@
 - `workload_identity_provider`: Provider for workload identity federation.
 - `workload_identity_service_account`: Service account for workload identity federation (specify the full string).
 
 AutoMLOps will generate the resources specified by these parameters (e.g. Artifact Registry, Cloud Source Repo, etc.). If use_ci is set to True, AutoMLOps will turn the outputted AutoMLOps/ directory into a Git repo and use it for the source repo. If a cron formatted str is given as an arg for `schedule_pattern` then it will set up a Cloud Schedule to run accordingly. If `setup_model_monitoring` is set to true, a model_monitoring/ directory will be created and a monitoring section will be added to config/defaults.yaml with empty values. These values are then set by running `AutoMLOps.monitor()`.
 
 # Generating Code
 
-AutoMLOps generates code that is compatible with `kfp<2.0.0`. Upon running `AutoMLOps.generate(project_id='project-id', pipeline_params=pipeline_params, setup_model_monitoring=True, use_ci=True)`, a series of directories will be generated automatically:
+AutoMLOps generates code that is compatible with `kfp>=2.0.0`. Upon running `AutoMLOps.generate(project_id='project-id', pipeline_params=pipeline_params, setup_model_monitoring=True, use_ci=True)`, a series of directories will be generated automatically:
 
 ```bash
 .
 ├── components                                     : Custom vertex pipeline components.
     ├──component_base                              : Contains all the python files, Dockerfile and requirements.txt
         ├── Dockerfile                             : Dockerfile containing all the python files for the components.
         ├── requirements.txt                       : Package requirements for all the python files for the components.
```

### Comparing `google-cloud-automlops-1.2.9/README.md` & `google_cloud_automlops-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # Dependencies
 - `docopt==0.6.2`
 - `docstring-parser==0.15`
 - `google-api-python-client==2.97.0`
 - `google-auth==2.22.0`
 - `importlib-resources==6.0.1`
 - `Jinja2==3.1.2`
+- `kfp>=2.0.0`
 - `packaging==23.1`
 - `pipreqs==0.4.13`
 - `pydantic==2.3.0`
 - `PyYAML==6.0.1`
 - `yarg==0.1.9`
 
 # Usage
@@ -82,15 +83,15 @@
 
 **Provisioning Frameworks**: Stands up necessary infra to run MLOps pipelines
 - gcloud
 - terraform
 - [coming soon] pulumi
 
 **Source Code Repositories**: Repository for versioning generated MLOps code
-- Cloud Source Repositories
+- [deprecating soon] Cloud Source Repositories
 - Bitbucket
 - Github
 - Gitlab
 
 # Prerequisites
 ### Generate
 In order to use `AutoMLOps.generate(...)`, the following are required:
@@ -103,15 +104,15 @@
 
 In order to use `AutoMLOps.provision(...)` with `provisioning_framework='terraform'`, the following are recommended:
 - [Terraform v1.5.6](https://www.terraform.io/downloads.html)
 
 ### Deploy
 In order to use `AutoMLOps.deploy(...)` with `use_ci=False`, the following are required:
 - Local python environment with these packages installed:
-    - `kfp<2.0.0`
+    - `kfp>=2.0.0`
     - `google-cloud-aiplatform`
     - `google-cloud-pipeline-components`
     - `google-cloud-storage`
     - `pyyaml`
 
 In order to use `AutoMLOps.deploy(...)` with `use_ci=True`, the following are required:
 - `git` installed
@@ -323,15 +324,15 @@
 - `workload_identity_provider`: Provider for workload identity federation.
 - `workload_identity_service_account`: Service account for workload identity federation (specify the full string).
 
 AutoMLOps will generate the resources specified by these parameters (e.g. Artifact Registry, Cloud Source Repo, etc.). If use_ci is set to True, AutoMLOps will turn the outputted AutoMLOps/ directory into a Git repo and use it for the source repo. If a cron formatted str is given as an arg for `schedule_pattern` then it will set up a Cloud Schedule to run accordingly. If `setup_model_monitoring` is set to true, a model_monitoring/ directory will be created and a monitoring section will be added to config/defaults.yaml with empty values. These values are then set by running `AutoMLOps.monitor()`.
 
 # Generating Code
 
-AutoMLOps generates code that is compatible with `kfp<2.0.0`. Upon running `AutoMLOps.generate(project_id='project-id', pipeline_params=pipeline_params, setup_model_monitoring=True, use_ci=True)`, a series of directories will be generated automatically:
+AutoMLOps generates code that is compatible with `kfp>=2.0.0`. Upon running `AutoMLOps.generate(project_id='project-id', pipeline_params=pipeline_params, setup_model_monitoring=True, use_ci=True)`, a series of directories will be generated automatically:
 
 ```bash
 .
 ├── components                                     : Custom vertex pipeline components.
     ├──component_base                              : Contains all the python files, Dockerfile and requirements.txt
         ├── Dockerfile                             : Dockerfile containing all the python files for the components.
         ├── requirements.txt                       : Package requirements for all the python files for the components.
```

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/AutoMLOps.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/AutoMLOps.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""AutoMLOps is a tool that generates a production-style MLOps pipeline
-   from Jupyter Notebooks."""
+"""AutoMLOps is a tool that generates a production-style MLOps pipelines."""
 
 # pylint: disable=C0103
+# pylint: disable=inconsistent-return-statements
 # pylint: disable=line-too-long
 # pylint: disable=unused-import
+# pylint: disable=logging-fstring-interpolation
+# pylint: disable=global-at-module-level
+# pylint: disable=global-variable-undefined
 
 import functools
-import json
 import logging
 import os
 import sys
 import subprocess
 from typing import Callable, Dict, List, Optional
 
 from google_cloud_automlops.utils.constants import (
@@ -41,70 +43,65 @@
     GENERATED_DEFAULTS_FILE,
     GENERATED_DIRS,
     GENERATED_GITHUB_DIRS,
     GENERATED_MODEL_MONITORING_DIRS,
     GENERATED_RESOURCES_SH_FILE,
     GENERATED_SERVICES_DIRS,
     GENERATED_TERRAFORM_DIRS,
-    OUTPUT_DIR
 )
 from google_cloud_automlops.utils.utils import (
     account_permissions_warning,
     check_installation_versions,
+    coalesce,
     create_default_config,
     execute_process,
+    git_workflow,
     make_dirs,
     precheck_deployment_requirements,
     read_yaml_file,
     resources_generation_manifest,
     stringify_job_spec_list,
     validate_use_ci,
     write_file,
     write_yaml_file
 )
 # Orchestration imports
-from google_cloud_automlops.orchestration.kfp import builder as KfpBuilder
-from google_cloud_automlops.orchestration.kfp import scaffold as KfpScaffold
-from google_cloud_automlops.orchestration.enums import (
+from google_cloud_automlops.utils.enums import (
+    ArtifactRepository,
+    CodeRepository,
+    Deployer,
     Orchestrator,
-    PipelineJobSubmitter
-)
-from google_cloud_automlops.orchestration.configs import (
-    KfpConfig
+    PipelineJobSubmitter,
+    Provisioner
 )
+from google_cloud_automlops.orchestration.base import BaseComponent, BasePipeline, BaseServices
+from google_cloud_automlops.orchestration.kfp import KFPComponent, KFPPipeline, KFPServices
+
 # Provisioning imports
-from google_cloud_automlops.provisioning.pulumi import builder as PulumiBuilder
-from google_cloud_automlops.provisioning.terraform import builder as TerraformBuilder
-from google_cloud_automlops.provisioning.gcloud import builder as GcloudBuilder
-from google_cloud_automlops.provisioning.enums import Provisioner
-from google_cloud_automlops.provisioning.configs import (
-    PulumiConfig,
-    TerraformConfig,
-    GcloudConfig
-)
+from google_cloud_automlops.provisioning.base import Infrastructure
+from google_cloud_automlops.provisioning.terraform import Terraform
+from google_cloud_automlops.provisioning.gcloud import GCloud
+from google_cloud_automlops.provisioning.pulumi import Pulumi
+
 # Deployment imports
-from google_cloud_automlops.deployments.cloudbuild import builder as CloudBuildBuilder
-from google_cloud_automlops.deployments.github_actions import builder as GithubActionsBuilder
-from google_cloud_automlops.deployments.enums import (
-    ArtifactRepository,
-    CodeRepository,
-    Deployer
-)
-from google_cloud_automlops.deployments.configs import (
-    CloudBuildConfig,
-    GitHubActionsConfig
-)
-from google_cloud_automlops.deployments.gitops.git_utils import git_workflow
+from google_cloud_automlops.deployments.cloudbuild import CloudBuild
+from google_cloud_automlops.deployments.github_actions import GitHubActions
 
+# Set up logging
 logging.basicConfig(stream=sys.stdout, level=logging.INFO,
                     format='%(message)s')
 logging.getLogger('googleapiclient').setLevel(logging.WARNING)
 logger = logging.getLogger()
 
-make_dirs([OUTPUT_DIR])
+# Set up global dictionaries to hold pipeline and components
+global components_dict
+components_dict = {}
+# # Set up global pipeline glob
+# global pipeline_glob
+# pipeline_glob = None
 
 def launchAll(
     project_id: str,
     pipeline_params: Dict,
     artifact_repo_location: Optional[str] = DEFAULT_RESOURCE_LOCATION,
     artifact_repo_name: Optional[str] = None,
     artifact_repo_type: Optional[str] = ArtifactRepository.ARTIFACT_REGISTRY.value,
@@ -135,17 +132,16 @@
     storage_bucket_name: Optional[str] = None,
     hide_warnings: Optional[bool] = True,
     use_ci: Optional[bool] = False,
     vpc_connector: Optional[str] = DEFAULT_VPC_CONNECTOR,
     workload_identity_pool: Optional[str] = None,
     workload_identity_provider: Optional[str] = None,
     workload_identity_service_account: Optional[str] = None):
-    """Generates relevant pipeline and component artifacts,
-       then provisions resources, builds, compiles, and submits the PipelineJob.
-       Check constants file for variable default values.
+    """Generates relevant pipeline and component artifacts, then provisions resources, builds,
+    compiles, and submits the PipelineJob. Check constants file for variable default values.
 
     Args:
         project_id: The project ID.
         pipeline_params: Dictionary containing runtime pipeline parameters.
         artifact_repo_location: Region of the artifact repo (default use with Artifact Registry).
         artifact_repo_name: Artifact repo name where components are stored (default use with Artifact Registry).
         artifact_repo_type: The type of artifact repository to use (e.g. Artifact Registry, JFrog, etc.)        
@@ -251,61 +247,81 @@
     storage_bucket_location: Optional[str] = DEFAULT_RESOURCE_LOCATION,
     storage_bucket_name: Optional[str] = None,
     use_ci: Optional[bool] = False,
     vpc_connector: Optional[str] = DEFAULT_VPC_CONNECTOR,
     workload_identity_pool: Optional[str] = None, #TODO: integrate optional creation of pool and provider during provisioning stage
     workload_identity_provider: Optional[str] = None,
     workload_identity_service_account: Optional[str] = None):
-    """Generates relevant pipeline and component artifacts.
-       Check constants file for variable default values.
+    """Generates relevant pipeline and component artifacts. Check constants file for variable
+    default values.
 
     Args: See launchAll() function.
     """
     # Validate that use_ci=True if schedule_pattern parameter is set or setup_model_monitoring is True
     validate_use_ci(setup_model_monitoring, schedule_pattern, use_ci)
 
     # Validate currently supported tools
     if artifact_repo_type not in [e.value for e in ArtifactRepository]:
-        raise ValueError(f'Unsupported artifact repository type: {artifact_repo_type}')
+        raise ValueError(
+            f'Unsupported artifact repository type: {artifact_repo_type}. \
+            Supported frameworks include: {", ".join([e.value for e in ArtifactRepository])}'
+        )
     if source_repo_type not in [e.value for e in CodeRepository]:
-        raise ValueError(f'Unsupported source repository type: {source_repo_type}')
+        raise ValueError(
+            f'Unsupported source repository type: {source_repo_type}. \
+            Supported frameworks include: {", ".join([e.value for e in CodeRepository])}'
+        )
     if pipeline_job_submission_service_type not in [e.value for e in PipelineJobSubmitter]:
-        raise ValueError(f'Unsupported pipeline job submissions service type: {pipeline_job_submission_service_type}')
+        raise ValueError(
+            f'Unsupported pipeline job submissions service type: {pipeline_job_submission_service_type}. \
+            Supported frameworks include: {", ".join([e.value for e in PipelineJobSubmitter])}'
+        )
     if orchestration_framework not in [e.value for e in Orchestrator]:
-        raise ValueError(f'Unsupported orchestration framework: {orchestration_framework}')
+        raise ValueError(
+            f'Unsupported orchestration framework: {orchestration_framework}. \
+            Supported frameworks include: {", ".join([e.value for e in Orchestrator])}'
+        )
     if provisioning_framework not in [e.value for e in Provisioner]:
-        raise ValueError(f'Unsupported provisioning framework: {provisioning_framework}')
+        raise ValueError(
+            f'Unsupported provisioning framework: {provisioning_framework}. \
+            Supported frameworks include: {", ".join([e.value for e in Provisioner])}'
+        )
     if deployment_framework not in [e.value for e in Deployer]:
-        raise ValueError(f'Unsupported deployment framework: {deployment_framework}')
+        raise ValueError(
+            f'Unsupported deployment framework: {deployment_framework}. \
+            Supported frameworks include: {", ".join([e.value for e in Deployer])}'
+        )
 
-    logging.info(f'Writing directories under {BASE_DIR}')
     # Make standard directories
+    logging.info(f'Writing directories under {BASE_DIR}')
     make_dirs(GENERATED_DIRS)
+
     # Make optional directories
     if use_ci:
         make_dirs(GENERATED_SERVICES_DIRS)
     if provisioning_framework == Provisioner.TERRAFORM.value:
         make_dirs(GENERATED_TERRAFORM_DIRS)
     if deployment_framework == Deployer.GITHUB_ACTIONS.value:
         make_dirs(GENERATED_GITHUB_DIRS)
     if setup_model_monitoring:
         make_dirs(GENERATED_MODEL_MONITORING_DIRS)
 
     # Set derived vars if none were given for certain variables
-    derived_artifact_repo_name = f'{naming_prefix}-artifact-registry' if artifact_repo_name is None else artifact_repo_name
-    derived_build_trigger_name = f'{naming_prefix}-build-trigger' if build_trigger_name is None else build_trigger_name
-    derived_custom_training_job_specs = stringify_job_spec_list(custom_training_job_specs) if custom_training_job_specs is not None else custom_training_job_specs
-    derived_pipeline_job_runner_service_account = f'vertex-pipelines@{project_id}.iam.gserviceaccount.com' if pipeline_job_runner_service_account is None else pipeline_job_runner_service_account
-    derived_pipeline_job_submission_service_name = f'{naming_prefix}-job-submission-svc' if pipeline_job_submission_service_name is None else pipeline_job_submission_service_name
-    derived_pubsub_topic_name = f'{naming_prefix}-queueing-svc' if pubsub_topic_name is None else pubsub_topic_name
-    derived_schedule_name = f'{naming_prefix}-schedule' if schedule_name is None else schedule_name
-    derived_source_repo_name = f'{naming_prefix}-repository' if source_repo_name is None else source_repo_name
-    derived_storage_bucket_name = f'{project_id}-{naming_prefix}-bucket' if storage_bucket_name is None else storage_bucket_name
+    derived_artifact_repo_name = coalesce(artifact_repo_name, f'{naming_prefix}-artifact-registry')
+    derived_build_trigger_name = coalesce(build_trigger_name, f'{naming_prefix}-build-trigger')
+    derived_custom_training_job_specs = stringify_job_spec_list(custom_training_job_specs)
+    derived_pipeline_job_runner_service_account = coalesce(pipeline_job_runner_service_account, f'vertex-pipelines@{project_id}.iam.gserviceaccount.com')
+    derived_pipeline_job_submission_service_name = coalesce(pipeline_job_submission_service_name, f'{naming_prefix}-job-submission-svc')
+    derived_pubsub_topic_name = coalesce(pubsub_topic_name, f'{naming_prefix}-queueing-svc')
+    derived_schedule_name = coalesce(schedule_name, f'{naming_prefix}-schedule')
+    derived_source_repo_name = coalesce(source_repo_name, f'{naming_prefix}-repository')
+    derived_storage_bucket_name = coalesce(storage_bucket_name, f'{project_id}-{naming_prefix}-bucket')
 
     # Write defaults.yaml
+    logging.info(f'Writing configurations to {GENERATED_DEFAULTS_FILE}')
     defaults = create_default_config(
         artifact_repo_location=artifact_repo_location,
         artifact_repo_name=derived_artifact_repo_name,
         artifact_repo_type=artifact_repo_type,
         base_image=base_image,
         build_trigger_location=build_trigger_location,
         build_trigger_name=derived_build_trigger_name,
@@ -326,127 +342,73 @@
         source_repo_branch=source_repo_branch,
         source_repo_name=derived_source_repo_name,
         source_repo_type=source_repo_type,
         storage_bucket_location=storage_bucket_location,
         storage_bucket_name=derived_storage_bucket_name,
         use_ci=use_ci,
         vpc_connector=vpc_connector)
-    logging.info(f'Writing configurations to {GENERATED_DEFAULTS_FILE}')
-    # Write header and then yaml contents
     write_file(GENERATED_DEFAULTS_FILE, DEFAULTS_HEADER, 'w')
     write_yaml_file(GENERATED_DEFAULTS_FILE, defaults, 'a')
 
     # Generate files required to run a Kubeflow pipeline
     if orchestration_framework == Orchestrator.KFP.value:
-        logging.info(f'Writing README.md to {BASE_DIR}README.md')
-        logging.info(f'Writing kubeflow pipelines code to {BASE_DIR}pipelines, {BASE_DIR}components')
-        logging.info(f'Writing scripts to {BASE_DIR}scripts')
+
+        # Write kubeflow pipeline code
+        logging.info(f'Writing kubeflow pipelines code to {BASE_DIR}pipelines')
+        kfppipe = KFPPipeline(func=pipeline_glob.func,
+                              name=pipeline_glob.name,
+                              description=pipeline_glob.description,
+                              comps_dict=components_dict)
+        kfppipe.build(pipeline_params, derived_custom_training_job_specs)
+
+        # Write kubeflow components code
+        logging.info(f'Writing kubeflow components code to {BASE_DIR}components')
+        for comp in kfppipe.comps:
+            logging.info(f'     -- Writing {comp.name}')
+            KFPComponent(func=comp.func, packages_to_install=comp.packages_to_install).build()
+
+        # If user specified services, write services scripts
         if use_ci:
             logging.info(f'Writing submission service code to {BASE_DIR}services')
-        if setup_model_monitoring:
-            logging.info(f'Writing model monitoring code to {BASE_DIR}model_monitoring')
-        KfpBuilder.build(KfpConfig(
-            base_image=base_image,
-            custom_training_job_specs=derived_custom_training_job_specs,
-            setup_model_monitoring=setup_model_monitoring,
-            pipeline_params=pipeline_params,
-            pubsub_topic_name=derived_pubsub_topic_name,
-            use_ci=use_ci))
+            KFPServices().build()
 
     # Generate files required to provision resources
     if provisioning_framework == Provisioner.GCLOUD.value:
         logging.info(f'Writing gcloud provisioning code to {BASE_DIR}provision')
-        GcloudBuilder.build(project_id, GcloudConfig(
-            artifact_repo_location=artifact_repo_location,
-            artifact_repo_name=derived_artifact_repo_name,
-            artifact_repo_type=artifact_repo_type,
-            build_trigger_location=build_trigger_location,
-            build_trigger_name=derived_build_trigger_name,
-            deployment_framework=deployment_framework,
-            naming_prefix=naming_prefix,
-            pipeline_job_runner_service_account=derived_pipeline_job_runner_service_account,
-            pipeline_job_submission_service_location=pipeline_job_submission_service_location,
-            pipeline_job_submission_service_name=derived_pipeline_job_submission_service_name,
-            pipeline_job_submission_service_type=pipeline_job_submission_service_type,
-            pubsub_topic_name=derived_pubsub_topic_name,
-            schedule_location=schedule_location,
-            schedule_name=derived_schedule_name,
-            schedule_pattern=schedule_pattern,
-            source_repo_branch=source_repo_branch,
-            source_repo_name=derived_source_repo_name,
-            source_repo_type=source_repo_type,
-            storage_bucket_location=storage_bucket_location,
-            storage_bucket_name=derived_storage_bucket_name,
-            use_ci=use_ci,
-            vpc_connector=vpc_connector))
+        GCloud(provision_credentials_key=provision_credentials_key).build()
 
     elif provisioning_framework == Provisioner.TERRAFORM.value:
         logging.info(f'Writing terraform provisioning code to {BASE_DIR}provision')
-        TerraformBuilder.build(project_id, TerraformConfig(
-            artifact_repo_location=artifact_repo_location,
-            artifact_repo_name=derived_artifact_repo_name,
-            artifact_repo_type=artifact_repo_type,
-            build_trigger_location=build_trigger_location,
-            build_trigger_name=derived_build_trigger_name,
-            deployment_framework=deployment_framework,
-            naming_prefix=naming_prefix,
-            pipeline_job_runner_service_account=derived_pipeline_job_runner_service_account,
-            pipeline_job_submission_service_location=pipeline_job_submission_service_location,
-            pipeline_job_submission_service_name=derived_pipeline_job_submission_service_name,
-            pipeline_job_submission_service_type=pipeline_job_submission_service_type,
-            provision_credentials_key=provision_credentials_key,
-            pubsub_topic_name=derived_pubsub_topic_name,
-            schedule_location=schedule_location,
-            schedule_name=derived_schedule_name,
-            schedule_pattern=schedule_pattern,
-            source_repo_branch=source_repo_branch,
-            source_repo_name=derived_source_repo_name,
-            source_repo_type=source_repo_type,
-            storage_bucket_location=storage_bucket_location,
-            storage_bucket_name=derived_storage_bucket_name,
-            use_ci=use_ci,
-            vpc_connector=vpc_connector))
+        Terraform(provision_credentials_key=provision_credentials_key).build()
 
     # Pulumi - Currently a roadmap item
     # elif provisioning_framework == Provisioner.PULUMI.value:
-    #     PulumiBuilder.build(project_id, PulumiConfig)
+    #     Pulumi(provision_credentials_key=provision_credentials_key).build()
 
     # Generate files required to run cicd pipeline
     if deployment_framework == Deployer.CLOUDBUILD.value:
         logging.info(f'Writing cloud build config to {GENERATED_CLOUDBUILD_FILE}')
-        CloudBuildBuilder.build(CloudBuildConfig(
-                artifact_repo_location=artifact_repo_location,
-                artifact_repo_name=derived_artifact_repo_name,
-                naming_prefix=naming_prefix,
-                project_id=project_id,
-                pubsub_topic_name=derived_pubsub_topic_name,
-                use_ci=use_ci))
-    if deployment_framework == Deployer.GITHUB_ACTIONS.value:
+        CloudBuild().build()
+
+    elif deployment_framework == Deployer.GITHUB_ACTIONS.value:
         if project_number is None:
             raise ValueError('Project number must be specified in order to use to use Github Actions integration.')
         logging.info(f'Writing GitHub Actions config to {GENERATED_GITHUB_ACTIONS_FILE}')
-        GithubActionsBuilder.build(GitHubActionsConfig(
-                artifact_repo_location=artifact_repo_location,
-                artifact_repo_name=derived_artifact_repo_name,
-                naming_prefix=naming_prefix,
-                project_id=project_id,
-                project_number=project_number,
-                pubsub_topic_name=derived_pubsub_topic_name,
-                source_repo_branch=source_repo_branch,
-                use_ci=use_ci,
-                workload_identity_pool=workload_identity_pool,
-                workload_identity_provider=workload_identity_provider,
-                workload_identity_service_account=workload_identity_service_account))
+        GitHubActions(
+            project_number=project_number,
+            workload_identity_pool=workload_identity_pool,
+            workload_identity_provider=workload_identity_provider,
+            workload_identity_service_account=workload_identity_service_account
+        ).build()
     logging.info('Code Generation Complete.')
 
 
 def provision(hide_warnings: Optional[bool] = True):
-    """Provisions the necessary infra to run MLOps pipelines. 
-       The provisioning option (e.g. terraform, gcloud, etc.)
-       is set during the generate() step and stored in config/defaults.yaml. 
+    """Provisions the necessary infra to run MLOps pipelines. The provisioning option (e.g.
+    terraform, gcloud, etc.) is set during the generate() step and stored in config/defaults.yaml. 
 
     Args:
         hide_warnings: Boolean that specifies whether to show permissions warnings before provisioning.
     """
     defaults = read_yaml_file(GENERATED_DEFAULTS_FILE)
     provisioning_framework = defaults['tooling']['provisioning_framework']
 
@@ -458,45 +420,40 @@
         execute_process(f'./{GENERATED_RESOURCES_SH_FILE}', to_null=False)
     elif provisioning_framework == Provisioner.TERRAFORM.value:
         execute_process(f'./{GENERATED_RESOURCES_SH_FILE} state_bucket', to_null=False)
         execute_process(f'./{GENERATED_RESOURCES_SH_FILE} environment', to_null=False)
 
 
 def deprovision():
-    """De-provisions the infra stood up during the provision() step.
-       deprovision currently only works with terraform. 
-       The provisioning option (e.g. terraform, gcloud, etc.)
-       is set during the generate() step and stored in config/defaults.yaml. 
+    """De-provisions the infra stood up during the provision() step. Deprovision currently only
+    works with terraform. The provisioning option (e.g. terraform, gcloud, etc.) is set during the
+    generate() step and stored in config/defaults.yaml. 
     """
     defaults = read_yaml_file(GENERATED_DEFAULTS_FILE)
     provisioning_framework = defaults['tooling']['provisioning_framework']
 
     if provisioning_framework == Provisioner.GCLOUD.value:
         raise ValueError('De-provisioning is currently only supported for provisioning_framework={terraform, pulumi}.')
 
     execute_process(f'terraform -chdir={BASE_DIR}provision/environment destroy -auto-approve', to_null=False)
 
 
 def deploy(
     hide_warnings: Optional[bool] = True,
     precheck: Optional[bool] = False):
-
-    """Builds and pushes the component_base image, compiles the pipeline,
-       and submits a message to the queueing service to execute a PipelineJob.
-       The specifics of the deploy step are dependent on the defaults set during
-       the generate() step, particularly:
-       - use_ci: if use_ci is False, the deploy step will use scripts/run_all.sh,
-            which will submit the build job, compile the pipeline, and submit the
-            PipelineJob all from the local machine.
-       - artifact_repo_type: Determines which type of artifact repo the image
-            is pushed to.
-       - deployment_framework: Determines which build tool to use for building.
-       - source_repo_type: Determines which source repo to use for versioning code
-            and triggering the build.
-       Defaults are stored in config/defaults.yaml.
+    """Builds and pushes the component_base image, compiles the pipeline, and submits a message to
+    the queueing service to execute a PipelineJob. The specifics of the deploy step are dependent on
+    the defaults set during the generate() step, particularly:
+        - use_ci: if use_ci is False, the deploy step will use scripts/run_all.sh, which will submit
+            the build job, compile the pipeline, and submit the PipelineJob all from the local machine.
+        - artifact_repo_type: Determines which type of artifact repo the image is pushed to.
+        - deployment_framework: Determines which build tool to use for building.
+        - source_repo_type: Determines which source repo to use for versioning code and triggering
+            the build.
+    Defaults are stored in config/defaults.yaml.
 
     Args:
         hide_warnings: Boolean that specifies whether to show permissions warnings before deploying.
         precheck: Boolean that specifies whether to check if the infra exists before deploying.
     """
     defaults = read_yaml_file(GENERATED_DEFAULTS_FILE)
     use_ci = defaults['tooling']['use_ci']
@@ -534,24 +491,23 @@
     job_display_name: Optional[str] = None,
     monitoring_interval: Optional[int] = 1,
     monitoring_location: Optional[str] = DEFAULT_RESOURCE_LOCATION,
     sample_rate: Optional[float] = 0.8,
     skew_thresholds: Optional[dict] = None,
     training_dataset: Optional[str] = None):
     """Creates or updates a Vertex AI Model Monitoring Job for a deployed model endpoint.
-       - The predicted target field and model endpoint are required.
-       - alert_emails, if specified, will send monitoring updates to the specified email(s)
-       - auto_retraining_params will set up automatic retraining by creating a Log Sink and
-            forwarding anomaly logs to the Pub/Sub Topic for retraining the model with the
-            params specified here. If this field is left Null, the model will not be
-            automatically retrained when an anomaly is detected.
-       - drift_thresholds and skew_thresholds are optional, but at least 1 of them 
-            must be specified.
-       - training_dataset must be specified if skew_thresholds are provided.
-       Defaults are stored in config/defaults.yaml.
+        - The predicted target field and model endpoint are required.
+        - alert_emails, if specified, will send monitoring updates to the specified email(s)
+        - auto_retraining_params will set up automatic retraining by creating a Log Sink and
+            forwarding anomaly logs to the Pub/Sub Topic for retraining the model with the params
+            specified here. If this field is left Null, the model will not be automatically
+            retrained when an anomaly is detected.
+        - drift_thresholds and skew_thresholds are optional, but at least 1 of them must be specified.
+        - training_dataset must be specified if skew_thresholds are provided.
+    Defaults are stored in config/defaults.yaml.
 
     Args:
         target_field: Prediction target column name in training dataset.
         model_endpoint: Endpoint resource name of the deployed model to monitoring.
             Format: projects/{project}/locations/{location}/endpoints/{endpoint}
         alert_emails: Optional list of emails to send monitoring alerts.
             Email alerts not used if this value is set to None.
@@ -611,73 +567,70 @@
 
 def component(func: Optional[Callable] = None,
               *,
               packages_to_install: Optional[List[str]] = None):
     """Decorator for Python-function based components in AutoMLOps.
 
     Example usage:
-    from google_cloud_automlops import AutoMLOps
-    @AutoMLOps.component
-    def my_function_one(input: str, output: Output[Model]):
-      ...
+        from google_cloud_automlops import AutoMLOps
+        @AutoMLOps.component
+        def my_function_one(input: str, output: Output[Model]):
+        ...
+
     Args:
-        func: The python function to create a component from. The function
-            should have type annotations for all its arguments, indicating how
-            it is intended to be used (e.g. as an input/output Artifact object,
-            a plain parameter, or a path to a file).
-        packages_to_install: A list of optional packages to install before
-            executing func. These will always be installed at component runtime.
-  """
+        func: The python function to create a component from. The function should have type
+            annotations for all its arguments, indicating how it is intended to be used (e.g. as an
+            input/output Artifact object, a plain parameter, or a path to a file).
+        packages_to_install: A list of optional packages to install before executing func. These
+            will always be installed at component runtime.
+    """
     if func is None:
         return functools.partial(
             component,
             packages_to_install=packages_to_install)
     else:
-        return KfpScaffold.create_component_scaffold(
+        components_dict[func.__name__] = BaseComponent(
             func=func,
-            packages_to_install=packages_to_install)
+            packages_to_install=packages_to_install
+        )
+        return
 
 
 def pipeline(func: Optional[Callable] = None,
              *,
              name: Optional[str] = None,
              description: Optional[str] = None):
     """Decorator for Python-function based pipelines in AutoMLOps.
 
     Example usage:
-    from google_cloud_automlops import AutoMLOps
-    @AutoMLOps.pipeline
-    def pipeline(bq_table: str,
-                output_model_directory: str,
-                project: str,
-                region: str,
-                ):
-
-        dataset_task = create_dataset(
-            bq_table=bq_table,
-            project=project)
-      ...
+        from google_cloud_automlops import AutoMLOps
+        @AutoMLOps.pipeline
+        def pipeline(bq_table: str,
+                    output_model_directory: str,
+                    project: str,
+                    region: str,
+                    ):
+
+            dataset_task = create_dataset(
+                bq_table=bq_table,
+                project=project)
+        ...
+
     Args:
-        func: The python function to create a pipeline from. The function
-            should have type annotations for all its arguments, indicating how
-            it is intended to be used (e.g. as an input/output Artifact object,
-            a plain parameter, or a path to a file).
+        func: The python function to create a pipeline from. The function should have type
+            annotations for all its arguments, indicating how it is intended to be used (e.g. as an
+            input/output Artifact object, a plain parameter, or a path to a file).
         name: The name of the pipeline.
         description: Short description of what the pipeline does.
-  """
+    """
     if func is None:
         return functools.partial(
             pipeline,
             name=name,
             description=description)
     else:
-        return KfpScaffold.create_pipeline_scaffold(
-            func=func,
-            name=name,
-            description=description)
-
-
-def clear_cache():
-    """Deletes all temporary files stored in the cache directory."""
-    execute_process(f'rm -rf {OUTPUT_DIR}', to_null=False)
-    make_dirs([OUTPUT_DIR])
-    logging.info('Cache cleared.')
+        global pipeline_glob
+        pipeline_glob = BasePipeline(func=func,
+                                 name=name,
+                                 description=description,
+                                 comps_dict=components_dict)
+        return
```

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 import, with the end goal of becoming a Jupyter plugin to Vertex
 Workbench managed notebooks. The tool will generate yaml-component
 definitions, complete with Dockerfiles and requirements.txts for all
 Kubeflow components defined in a notebook. It will also generate a
 series of directories to support the creation of Vertex Pipelines.
 """
 # pylint: disable=invalid-name
-__version__ = '1.2.9'
+__version__ = '1.3.0'
 __author__ = 'Sean Rastatter'
 __credits__ = 'Google'
```

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/cloudbuild/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/cloudbuild/templates/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/templates/cloudbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/cloudbuild/templates/cloudbuild.yaml.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/templates/cloudbuild/cloudbuild.yaml.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/enums.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/utils/enums.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-# Copyright 2024 Google LLC. All Rights Reserved.
+# Copyright 2023 Google LLC. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Sets global enums."""
+"""Creates enums for orchestrator and submission service options
+as well as generic component, pipeline, and services objects."""
 
+# pylint: disable=anomalous-backslash-in-string
 # pylint: disable=C0103
 # pylint: disable=line-too-long
 
 from enum import Enum
 
 
 class Deployer(Enum):
@@ -25,20 +27,53 @@
 
     CLOUDBUILD = 'cloud-build'
     GITHUB_ACTIONS = 'github-actions'
     # GITLAB_CI = 'gitlab-ci'   # roadmap item
     # JENKINS = 'jenkins'   # roadmap item
 
 
+class Provisioner(Enum):
+    """Enum representing the available providers for infrastructure management."""
+
+    TERRAFORM = 'terraform'
+    # PULUMI = 'pulumi' roadmap item
+    GCLOUD = 'gcloud'
+
+
+class Orchestrator(Enum):
+    """Enum representing the available options for orchestration management."""
+
+    KFP = 'kfp'
+    # ARGO_WORKFLOWS = 'argo-workflows'   # roadmap item
+    # TFX = 'tfx'   # roadmap item
+    # AIRFLOW = 'airflow'   # roadmap item
+    # RAY = 'ray'   # roadmap item
+
+
+class ArtifactRepository(Enum):
+    """Enum representing the available options for artifact repositories."""
+
+    ARTIFACT_REGISTRY = 'artifact-registry'
+
+
 class CodeRepository(Enum):
     """Enum representing the available options for source code repositories."""
 
     BITBUCKET = 'bitbucket'   # roadmap item
     CLOUD_SOURCE_REPOSITORIES = 'cloud-source-repositories'
     GITHUB = 'github'
     GITLAB = 'gitlab'   # roadmap item
 
 
-class ArtifactRepository(Enum):
-    """Enum representing the available options for artifact repositories."""
+class PipelineJobSubmitter(Enum):
+    """Enum representing the available options for the Pipeline Job submission service."""
 
-    ARTIFACT_REGISTRY = 'artifact-registry'
+    CLOUD_FUNCTIONS = 'cloud-functions'
+    CLOUD_RUN = 'cloud-run'
+
+
+class PulumiRuntime(Enum):
+    """Enum representing the available pulumi runtimes."""
+
+    PYTHON = 'python'
+    TYPESCRIPT = 'typescript'
+    GO = 'go'
```

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/github_actions/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/templates/github_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/github_actions/builder.py` & `google_cloud_automlops-1.3.0/tests/unit/deployments/github_actions_tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,109 +8,126 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Builds KFP components and pipeline."""
-
 # pylint: disable=line-too-long
+# pylint: disable=missing-function-docstring
+# pylint: disable=missing-module-docstring
 
 try:
     from importlib.resources import files as import_files
 except ImportError:
     # Try backported to PY<37 `importlib_resources`
     from importlib_resources import files as import_files
 
-from jinja2 import Template
+from typing import List
+
+import pytest
 
-from google_cloud_automlops.utils.utils import write_file
 from google_cloud_automlops.utils.constants import (
-    GENERATED_GITHUB_ACTIONS_FILE,
     COMPONENT_BASE_RELATIVE_PATH,
     GENERATED_LICENSE,
     GENERATED_PARAMETER_VALUES_PATH,
     GITHUB_ACTIONS_TEMPLATES_PATH
 )
+from google_cloud_automlops.utils.utils import render_jinja
 
-from google_cloud_automlops.deployments.configs import GitHubActionsConfig
 
-def build(config: GitHubActionsConfig):
-    """Constructs scripts for resource deployment and running Kubeflow pipelines.
-
-    Args:
-        config.artifact_repo_location: Region of the artifact repo (default use with Artifact Registry).
-        config.artifact_repo_name: Artifact repo name where components are stored (default use with Artifact Registry).
-        config.naming_prefix: Unique value used to differentiate pipelines and services across AutoMLOps runs.
-        config.project_id: The project ID.
-        config.project_number: The project number.
-        config.pubsub_topic_name: The name of the pubsub topic to publish to.
-        config.source_repo_branch: The branch to use in the source repository.
-        config.use_ci: Flag that determines whether to use Cloud CI/CD.
-        config.workload_identity_pool: Pool for workload identity federation. 
-        config.workload_identity_provider: Provider for workload identity federation.
-        config.workload_identity_service_account: Service account for workload identity federation. 
-    """
-    # Write github actions config
-    write_file(GENERATED_GITHUB_ACTIONS_FILE, create_github_actions_jinja(
-        config.artifact_repo_location,
-        config.artifact_repo_name,
-        config.naming_prefix,
-        config.project_id,
-        config.project_number,
-        config.pubsub_topic_name,
-        config.source_repo_branch,
-        config.use_ci,
-        config.workload_identity_pool,
-        config.workload_identity_provider,
-        config.workload_identity_service_account), 'w')
-
-def create_github_actions_jinja(
-        artifact_repo_location: str,
-        artifact_repo_name: str,
-        naming_prefix: str,
-        project_id: str,
-        project_number: str,
-        pubsub_topic_name: str,
-        source_repo_branch: str,
-        use_ci: bool,
-        workload_identity_pool: str,
-        workload_identity_provider: str,
-        workload_identity_service_account: str) -> str:
-    """Generates content for the github_actions.yaml, to be written to the .github/workflows directory.
-        This file contains the ci/cd manifest for AutoMLOps.
+@pytest.mark.parametrize(
+    '''artifact_repo_location, artifact_repo_name, naming_prefix,'''
+    '''project_id, project_number, pubsub_topic_name, use_ci, source_repo_branch,'''
+    '''workload_identity_provider, workload_identity_pool, workload_identity_service_account, is_included,'''
+    '''expected_output_snippets''',
+    [
+        (
+            'us-central1', 'my-artifact-repo', 'my-prefix',
+            'my-project', 'my-project-number', 'my-topic', True, 'automlops',
+            'my-provider', 'my-pool', 'my-sa', True,
+            ['id: auth',
+             'id: build-push-component-base',
+             'id: install-pipeline-deps',
+             'id: build-pipeline-spec',
+             'id: publish-to-topic', 
+             'us-central1-docker.pkg.dev/my-project/my-artifact-repo/my-prefix/components/component_base:latest',
+             'gcloud pubsub topics publish my-topic --message']
+        ),
+        (
+            'us-central1', 'my-artifact-repo', 'my-prefix',
+            'my-project', 'my-project-number', 'my-topic', False, 'automlops',
+            'my-provider', 'my-pool', 'my-sa', True,
+            ['id: build-push-component-base',
+             'us-central1-docker.pkg.dev/my-project/my-artifact-repo/my-prefix/components/component_base:latest']
+        ),
+        (
+            'us-central1', 'my-artifact-repo', 'my-prefix',
+            'my-project', 'my-project-number', 'my-topic', False, 'automlops',
+            'my-provider', 'my-pool', 'my-sa', False,
+            ['id: install-pipeline-deps',
+             'id: build-pipeline-spec',
+             'id: publish-to-topic',
+             'gcloud pubsub topics publish my-topic --message']
+        ),
+    ]
+)
+def test_create_github_actions_jinja(
+    artifact_repo_location: str,
+    artifact_repo_name: str,
+    naming_prefix: str,
+    project_id: str,
+    project_number: str,
+    pubsub_topic_name: str,
+    use_ci: bool,
+    source_repo_branch: str,
+    workload_identity_pool: str,
+    workload_identity_provider: str,
+    workload_identity_service_account: str,
+    is_included: bool,
+    expected_output_snippets: List[str]):
+    """Tests create_github_actions_jinja, which generates content for the github actions file. 
+       There are three test cases for this function:
+        1. Checks that expected strings are included when use_ci=True. 
+        2. Checks that expected strings are included when use_ci=False. 
+        3. Checks that certain strings are not included when use_ci=False. 
 
     Args:
         artifact_repo_location: Region of the artifact repo (default use with Artifact Registry).
         artifact_repo_name: Artifact repo name where components are stored (default use with Artifact Registry).
         naming_prefix: Unique value used to differentiate pipelines and services across AutoMLOps runs.
         project_id: The project ID.
         project_number: The project number.
         pubsub_topic_name: The name of the pubsub topic to publish to.
         source_repo_branch: The branch to use in the source repository.
         use_ci: Flag that determines whether to use Cloud CI/CD.
         workload_identity_pool: Pool for workload identity federation. 
         workload_identity_provider: Provider for workload identity federation.
         workload_identity_service_account: Service account for workload identity federation. 
-
-    Returns:
-        str: Contents of github_actions.yaml.
+        is_included: Boolean that determines whether to check if the expected_output_snippets exist in the string or not.
+        expected_output_snippets: Strings that are expected to be included (or not) based on the is_included boolean.
     """
+
     template_file = import_files(GITHUB_ACTIONS_TEMPLATES_PATH) / 'github_actions.yaml.j2'
-    with template_file.open('r', encoding='utf-8') as f:
-        template = Template(f.read())
-        return template.render(
-            artifact_repo_location=artifact_repo_location,
-            artifact_repo_name=artifact_repo_name,
-            component_base_relative_path=COMPONENT_BASE_RELATIVE_PATH,
-            generated_license=GENERATED_LICENSE,
-            generated_parameter_values_path=GENERATED_PARAMETER_VALUES_PATH,
-            naming_prefix=naming_prefix,
-            project_id=project_id,
-            project_number=project_number,
-            pubsub_topic_name=pubsub_topic_name,
-            source_repo_branch=source_repo_branch,
-            use_ci=use_ci,
-            workload_identity_pool=workload_identity_pool,
-            workload_identity_provider=workload_identity_provider,
-            workload_identity_service_account=workload_identity_service_account)
+    github_actions_config = render_jinja(
+        template_path=template_file,
+        artifact_repo_location=artifact_repo_location,
+        artifact_repo_name=artifact_repo_name,
+        component_base_relative_path=COMPONENT_BASE_RELATIVE_PATH,
+        generated_license=GENERATED_LICENSE,
+        generated_parameter_values_path=GENERATED_PARAMETER_VALUES_PATH,
+        naming_prefix=naming_prefix,
+        project_id=project_id,
+        project_number=project_number,
+        pubsub_topic_name=pubsub_topic_name,
+        source_repo_branch=source_repo_branch,
+        use_ci=use_ci,
+        workload_identity_pool=workload_identity_pool,
+        workload_identity_provider=workload_identity_provider,
+        workload_identity_service_account=workload_identity_service_account
+    )
+
+    for snippet in expected_output_snippets:
+        if is_included:
+            assert snippet in github_actions_config
+        elif not is_included:
+            assert snippet not in github_actions_config
```

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/github_actions/templates/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/github_actions/templates/github_actions.yaml.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/deployments/templates/github_actions/github_actions.yaml.j2`

 * *Files 0% similar despite different names*

```diff
@@ -76,8 +76,7 @@
       - name: Publish PipelineJob to topic
         id: publish-to-topic
         shell: bash
         run: |
           gcloud pubsub topics publish {{pubsub_topic_name}} --message \
           "$(cat {{generated_parameter_values_path}})"
 {% endif %}   
-
```

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/gitops/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/gitops/templates/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/deployments/gitops/templates/gitignore.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/utils/templates/gitignore.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/components/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/components/component_base/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/README.md.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/README.md.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/components/component_base/src/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/components/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/model_monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/components/component_base/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/components/component_base/src/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/components/component_base/src/task.py.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/components/component_base/src/task.py.j2`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 {{generated_license}}
 import argparse
 import json
-from kfp.v2.components import executor{% if not kfp_spec_bool %}
+from kfp.dsl import executor
 
 import kfp
-from kfp.v2 import dsl
-from kfp.v2.dsl import *
+from kfp import dsl
+from kfp.dsl import *
 from typing import *
-{% endif %}
+
 {{custom_code_contents}}
 def main():
     """Main executor."""
     parser = argparse.ArgumentParser()
     parser.add_argument('--executor_input', type=str)
     parser.add_argument('--function_to_execute', type=str)
```

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/model_monitoring/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/model_monitoring/monitor.py.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/model_monitoring/monitor.py.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/pipelines/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/services/submission_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/pipelines/pipeline.py.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/pipelines/pipeline.py.j2`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import os
 {% if custom_training_job_specs is not none %}
 from functools import partial
 from google_cloud_pipeline_components.v1.custom_job import create_custom_training_job_op_from_component
 {% endif %}
 from google.cloud import storage
 import kfp
-from kfp.v2 import compiler, dsl
-from kfp.v2.dsl import *
+from kfp import compiler, dsl
+from kfp.dsl import *
 import yaml
 
 def upload_pipeline_spec(gs_pipeline_job_spec_path: str,
                          pipeline_job_spec_path: str,
                          storage_bucket_name: str):
     '''Upload pipeline job spec from local to GCS'''
     storage_client = storage.Client()
```

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/pipelines/pipeline_runner.py.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/pipelines/pipeline_runner.py.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/scripts/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/services/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/services/submission_service/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/gcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/orchestration/kfp/templates/services/submission_service/main.py.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/orchestration/templates/kfp/services/submission_service/main.py.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/gcloud/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/gcloud/templates/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/state_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/gcloud/templates/provision_resources.sh.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/gcloud/provision_resources.sh.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/pulumi/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/__init__.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/utils/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/__init__.py` & `google_cloud_automlops-1.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/__init__.py` & `google_cloud_automlops-1.3.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/data.tf.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/data.tf.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/iam.tf.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/iam.tf.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/main.tf.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/main.tf.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/outputs.tf.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/outputs.tf.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/variables.auto.tfvars.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/variables.auto.tfvars.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/environment/variables.tf.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/environment/variables.tf.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/state_bucket/__init__.py` & `google_cloud_automlops-1.3.0/tests/unit/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/provisioning/terraform/templates/state_bucket/main.tf.j2` & `google_cloud_automlops-1.3.0/google_cloud_automlops/provisioning/templates/terraform/state_bucket/main.tf.j2`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/utils/__init__.py` & `google_cloud_automlops-1.3.0/tests/unit/orchestration/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/utils/constants.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,14 @@
     '# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n'
     '# See the License for the specific language governing permissions and\n'
     '# limitations under the License.\n'
     '#\n'
     '# DISCLAIMER: This code is generated as part of the AutoMLOps output.\n'
 )
 
-# Placeholder
-PLACEHOLDER_IMAGE = 'AutoMLOps_image_tbd'
-
 ## Default values
 # Default docker base image
 DEFAULT_BASE_IMAGE = 'python:3.9-slim'
 # Default location of resources
 DEFAULT_RESOURCE_LOCATION = 'us-central1'
 # Default naming prefix for resources
 DEFAULT_NAMING_PREFIX = 'automlops-default-prefix'
@@ -78,15 +75,15 @@
 GENERATED_PIPELINE_REQUIREMENTS_FILE = BASE_DIR + 'pipelines/requirements.txt'
 GENERATED_PIPELINE_FILE = BASE_DIR + 'pipelines/pipeline.py'
 GENERATED_PIPELINE_RUNNER_FILE = BASE_DIR + 'pipelines/pipeline_runner.py'
 GENERATED_COMPONENT_BASE = BASE_DIR + 'components/component_base'
 GENERATED_COMPONENT_BASE_SRC = BASE_DIR + 'components/component_base/src'
 COMPONENT_BASE_RELATIVE_PATH = 'components/component_base'
 GENERATED_PARAMETER_VALUES_PATH = 'pipelines/runtime_parameters/pipeline_parameter_values.json'
-GENERATED_PIPELINE_JOB_SPEC_PATH = 'scripts/pipeline_spec/pipeline_job.json'
+GENERATED_PIPELINE_JOB_SPEC_PATH = 'scripts/pipeline_spec/pipeline_job.yaml'
 GENERATED_DIRS = [
     BASE_DIR,
     BASE_DIR + 'components',
     BASE_DIR + 'components/component_base',
     BASE_DIR + 'components/component_base/src',
     BASE_DIR + 'configs',
     BASE_DIR + 'images',
@@ -112,35 +109,28 @@
     BASE_DIR + '.github/workflows'
 ]
 
 GENERATED_MODEL_MONITORING_DIRS = [
     BASE_DIR + 'model_monitoring',
 ]
 
-# temporary files
-CACHE_DIR = '.AutoMLOps-cache'
-PIPELINE_CACHE_FILE = CACHE_DIR + '/pipeline_scaffold.py'
-
-# KFP Spec output_file location
-OUTPUT_DIR = CACHE_DIR
-
 # Generated kfp pipeline metadata name
 DEFAULT_PIPELINE_NAME = 'automlops-pipeline'
 
 # KFP v2 Migration constant
-PINNED_KFP_VERSION = 'kfp<2.0.0'
+PINNED_KFP_VERSION = 'kfp>=2.0.0'
 
 # Provisioning Template Paths
-TERRAFORM_TEMPLATES_PATH = 'google_cloud_automlops.provisioning.terraform.templates'
-PULUMI_TEMPLATES_PATH = 'google_cloud_automlops.provisioning.pulumi.templates'
-GCLOUD_TEMPLATES_PATH = 'google_cloud_automlops.provisioning.gcloud.templates'
-KFP_TEMPLATES_PATH = 'google_cloud_automlops.orchestration.kfp.templates'
-CLOUDBUILD_TEMPLATES_PATH = 'google_cloud_automlops.deployments.cloudbuild.templates'
-GITHUB_ACTIONS_TEMPLATES_PATH = 'google_cloud_automlops.deployments.github_actions.templates'
-GITOPS_TEMPLATES_PATH = 'google_cloud_automlops.deployments.gitops.templates'
+TERRAFORM_TEMPLATES_PATH = 'google_cloud_automlops.provisioning.templates.terraform'
+PULUMI_TEMPLATES_PATH = 'google_cloud_automlops.provisioning.templates.pulumi'
+GCLOUD_TEMPLATES_PATH = 'google_cloud_automlops.provisioning.templates.gcloud'
+KFP_TEMPLATES_PATH = 'google_cloud_automlops.orchestration.templates.kfp'
+CLOUDBUILD_TEMPLATES_PATH = 'google_cloud_automlops.deployments.templates.cloudbuild'
+GITHUB_ACTIONS_TEMPLATES_PATH = 'google_cloud_automlops.deployments.templates.github_actions'
+GITOPS_TEMPLATES_PATH = 'google_cloud_automlops.utils.templates'
 
 # Required IAM Roles for pipeline runner service account
 IAM_ROLES_RUNNER_SA = [
     'roles/aiplatform.user',
     'roles/artifactregistry.reader',
     'roles/cloudfunctions.admin',
     'roles/bigquery.user',
```

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops/utils/utils.py` & `google_cloud_automlops-1.3.0/google_cloud_automlops/utils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,73 +15,84 @@
 """Utility functions and globals to be used by all
    other modules in this directory."""
 
 # pylint: disable=C0103
 # pylint: disable=line-too-long
 # pylint: disable=broad-exception-caught
 
+try:
+    from importlib.resources import files as import_files
+except ImportError:
+    # Try backported to PY<37 `importlib_resources`
+    from importlib_resources import files as import_files
+
 import inspect
 import itertools
 import json
 import logging
 import os
 import subprocess
 import textwrap
 from typing import Callable
 
 from packaging import version
 import yaml
+from jinja2 import Template
 
 from googleapiclient import discovery
 import google.auth
 
 from google_cloud_automlops.utils.constants import (
-    CACHE_DIR,
+    BASE_DIR,
     DEFAULT_SCHEDULE_PATTERN,
+    GENERATED_DEFAULTS_FILE,
     GENERATED_PARAMETER_VALUES_PATH,
     GENERATED_PIPELINE_JOB_SPEC_PATH,
+    GITOPS_TEMPLATES_PATH,
     IAM_ROLES_RUNNER_SA,
     MIN_GCLOUD_BETA_VERSION,
     MIN_GCLOUD_SDK_VERSION,
     MIN_RECOMMENDED_TERRAFORM_VERSION,
-    PLACEHOLDER_IMAGE
 )
 
-from google_cloud_automlops.deployments.enums import (
-    ArtifactRepository,
-    CodeRepository,
-    Deployer
-)
-from google_cloud_automlops.provisioning.enums import Provisioner
-from google_cloud_automlops.orchestration.enums import (
+from google_cloud_automlops.utils.enums import (
     Orchestrator,
     PipelineJobSubmitter
 )
 
+from google_cloud_automlops.utils.enums import (
+    ArtifactRepository,
+    CodeRepository,
+    Deployer,
+    Provisioner
+)
+
+
 def make_dirs(directories: list):
     """Makes directories with the specified names.
 
     Args:
-        directories: Path of the directories to make.
+        directories (list): Path of the directories to make.
     """
     for d in directories:
         try:
             os.makedirs(d)
         except FileExistsError:
             pass
 
 
 def read_yaml_file(filepath: str) -> dict:
-    """Reads a yaml and returns file contents as a dict.
-       Defaults to utf-8 encoding.
+    """Reads a yaml and returns file contents as a dict. Defaults to utf-8 encoding.
 
     Args:
-        filepath: Path to the yaml.
+        filepath (str): Path to the yaml.
+
     Returns:
         dict: Contents of the yaml.
+
     Raises:
         Exception: If an error is encountered reading the file.
     """
     try:
         with open(filepath, 'r', encoding='utf-8') as file:
             file_dict = yaml.safe_load(file)
         file.close()
@@ -90,215 +101,168 @@
     return file_dict
 
 
 def write_yaml_file(filepath: str, contents: dict, mode: str):
     """Writes a dictionary to yaml. Defaults to utf-8 encoding.
 
     Args:
-        filepath: Path to the file.
-        contents: Dictionary to be written to yaml.
-        mode: Read/write mode to be used.
+        filepath (str): Path to the file.
+        contents (dict): Dictionary to be written to yaml.
+        mode (str): Read/write mode to be used.
+
     Raises:
-        Exception: If an error is encountered writing the file.
+        Exception: An error is encountered while writing the file.
     """
     try:
         with open(filepath, mode, encoding='utf-8') as file:
             yaml.safe_dump(contents, file, sort_keys=False)
         file.close()
     except yaml.YAMLError as err:
         raise yaml.YAMLError(f'Error writing to file. {err}') from err
 
 
 def read_file(filepath: str) -> str:
-    """Reads a file and returns contents as a string.
-       Defaults to utf-8 encoding.
+    """Reads a file and returns contents as a string. Defaults to utf-8 encoding.
 
     Args:
-        filepath: Path to the file.
+        filepath (str): Path to the file.
+
     Returns:
         str: Contents of the file.
+
     Raises:
-        Exception: If an error is encountered reading the file.
+        Exception: An error is encountered while reading the file.
     """
     try:
         with open(filepath, 'r', encoding='utf-8') as file:
             contents = file.read()
         file.close()
     except FileNotFoundError as err:
         raise FileNotFoundError(f'Error reading file. {err}') from err
     return contents
 
 
 def write_file(filepath: str, text: str, mode: str):
     """Writes a file at the specified path. Defaults to utf-8 encoding.
 
     Args:
-        filepath: Path to the file.
-        text: Text to be written to file.
-        mode: Read/write mode to be used.
+        filepath (str): Path to the file.
+        text (str): Text to be written to file.
+        mode (str): Read/write mode to be used.
+
     Raises:
-        Exception: If an error is encountered writing the file.
+        Exception: An error is encountered writing the file.
     """
     try:
         with open(filepath, mode, encoding='utf-8') as file:
             file.write(text)
         file.close()
     except OSError as err:
         raise OSError(f'Error writing to file. {err}') from err
 
 
 def write_and_chmod(filepath: str, text: str):
-    """Writes a file at the specified path and chmods the file
-       to allow for execution.
+    """Writes a file at the specified path and chmods the file to allow for execution.
 
     Args:
-        filepath: Path to the file.
-        text: Text to be written to file.
+        filepath (str): Path to the file.
+        text (str): Text to be written to file.
+
     Raises:
-        Exception: If an error is encountered chmod-ing the file.
+        Exception: An error is encountered while chmod-ing the file.
     """
     write_file(filepath, text, 'w')
     try:
         st = os.stat(filepath)
         os.chmod(filepath, st.st_mode | 0o111)
     except OSError as err:
         raise OSError(f'Error chmod-ing file. {err}') from err
 
 
 def delete_file(filepath: str):
-    """Deletes a file at the specified path.
-       If it does not exist, pass.
+    """Deletes a file at the specified path. If it does not exist, pass.
 
     Args:
-        filepath: Path to the file.
+        filepath (str): Path to the file.
     """
     try:
         os.remove(filepath)
     except OSError:
         pass
 
 
-def get_components_list(full_path: bool = True) -> list:
-    """Reads yamls in the cache directory, verifies they are component
-       yamls, and returns the name of the files.
-
-    Args:
-        full_path: Boolean; if false, stores only the filename w/o extension.
-    Returns:
-        list: Contains the names or paths of all component yamls in the dir.
-    """
-    components_list = []
-    elements = os.listdir(CACHE_DIR)
-    for file in list(filter(lambda y: ('.yaml' or '.yml') in y, elements)):
-        path = os.path.join(CACHE_DIR, file)
-        if is_component_config(path):
-            if full_path:
-                components_list.append(path)
-            else:
-                components_list.append(os.path.basename(file).split('.')[0])
-    return components_list
-
-
 def is_component_config(filepath: str) -> bool:
     """Checks to see if the given file is a component yaml.
 
     Args:
-        filepath: Path to a yaml file.
+        filepath (str): Path to a yaml file.
+
     Returns:
         bool: Whether the given file is a component yaml.
     """
     required_keys = ['name','inputs','implementation']
     file_dict = read_yaml_file(filepath)
     return all(key in file_dict.keys() for key in required_keys)
 
 
 def execute_process(command: str, to_null: bool):
     """Executes an external shell process.
 
     Args:
-        command: The string of the command to execute.
-        to_null: Determines where to send output.
+        command (str): Command to execute.
+        to_null (bool): Determines where to send output.
+
     Raises:
-        Exception: If an error occurs in executing the script.
+        Exception: An error occured while executing the script.
     """
     stdout = subprocess.DEVNULL if to_null else None
     try:
         subprocess.run([command],
                        shell=True,
                        check=True,
                        stdout=stdout,
                        stderr=subprocess.STDOUT)
     except subprocess.CalledProcessError as err:
         raise RuntimeError(f'Error executing process. {err}') from err
 
 
 def validate_use_ci(setup_model_monitoring: bool, schedule_pattern: str, use_ci: str):
     """Validates that the inputted schedule parameter and model_monitoring parameter align with the 
-        use_ci configuration.
+    use_ci configuration.
+
     Note: this function does not validate that schedule_pattern is a properly formatted cron value.
     Cron format validation is done in the backend by GCP.
-    
+
     Args:
-        setup_model_monitoring: Boolean parameter which specifies whether to set up a Vertex AI Model Monitoring Job.
-        schedule_pattern: Cron formatted value used to create a Scheduled retrain job.
-        use_ci: Flag that determines whether to use Cloud CI/CD.
+        setup_model_monitoring (bool): Specifies whether to set up a Vertex AI Model Monitoring Job.
+        schedule_pattern (str): Cron formatted value used to create a Scheduled retrain job.
+        use_ci (bool): Specifies whether to use Cloud CI/CD.
+
     Raises:
-        Exception: If use_ci validation fails.
+        Exception: use_ci validation failed.
     """
     if setup_model_monitoring and not use_ci:
         raise ValueError('use_ci must be set to True to use Model Monitoring.')
     if schedule_pattern != DEFAULT_SCHEDULE_PATTERN and not use_ci:
         raise ValueError('use_ci must be set to True to use Cloud Scheduler.')
 
 
-def update_params(params: list) -> list:
-    """Converts the parameter types from Python types
-       to Kubeflow types. Currently only supports
-       Python primitive types.
-
-    Args:
-        params: Pipeline parameters. A list of dictionaries,
-            each param is a dict containing keys:
-                'name': required, str param name.
-                'type': required, python primitive type.
-                'description': optional, str param desc.
-    Returns:
-        list: Params list with converted types.
-    Raises:
-        Exception: If an inputted type is not a primitive.
-    """
-    python_kfp_types_mapper = {
-        int: 'Integer',
-        str: 'String',
-        float: 'Float',
-        bool: 'Boolean',
-        list: 'JsonArray',
-        dict: 'JsonObject'
-    }
-    for param in params:
-        try:
-            param['type'] = python_kfp_types_mapper[param['type']]
-        except KeyError as err:
-            raise ValueError(f'Unsupported python type - we only support '
-                             f'primitive types at this time. {err}') from err
-    return params
-
-
 def get_function_source_definition(func: Callable) -> str:
     """Returns a formatted string of the source code.
 
     Args:
-        func: The python function to create a component from. The function
-            should have type annotations for all its arguments, indicating how
-            it is intended to be used (e.g. as an input/output Artifact object,
-            a plain parameter, or a path to a file).
+        func (Callable): The python function to create a component from. The function should have
+            type annotations for all its arguments, indicating how it is intended to be used (e.g.
+            as an input/output Artifact object, a plain parameter, or a path to a file).
+
     Returns:
         str: The source code from the inputted function.
+
     Raises:
-        Exception: If the preprocess operates failed.
+        Exception: The preprocess operations failed.
     """
     source_code = inspect.getsource(func)
     source_code = textwrap.dedent(source_code)
     source_code_lines = source_code.split('\n')
     source_code_lines = itertools.dropwhile(lambda x: not x.startswith('def'),
                                             source_code_lines)
     if not source_code_lines:
@@ -309,50 +273,41 @@
     return '\n'.join(source_code_lines)
 
 
 def stringify_job_spec_list(job_spec_list: list) -> list:
     """Takes in a list of job spec dictionaries and turns them into strings.
 
     Args:
-        job_spec: Dictionary with job spec info. e.g.
+        job_spec (list): Dictionary with job spec info. e.g.
             custom_training_job_specs = [{
                 'component_spec': 'train_model',
                 'display_name': 'train-model-accelerated',
                 'machine_type': 'a2-highgpu-1g',
                 'accelerator_type': 'NVIDIA_TESLA_A100',
                 'accelerator_count': 1
             }]
 
     Returns:
         list[str]: Python formatted dictionary code.
     """
+    if not job_spec_list:
+        return None
     output = []
     for spec in job_spec_list:
         mapping = {}
         if isinstance(spec['component_spec'], str):
             mapping['component_spec'] = spec['component_spec']
         else:
             raise ValueError('component_spec must be a string.')
         # Remove string quotes from component spec line
         mapping['spec_string'] = json.dumps(spec, sort_keys=True, indent=8).replace(f'''"{spec['component_spec']}"''', f'''{spec['component_spec']}''')
         mapping['spec_string'] = mapping['spec_string'].replace('}', '    }') # align closing bracket
         output.append(mapping)
     return output
 
-def is_using_kfp_spec(image: str) -> bool:
-    """Takes in an image string from a component yaml and determines if it came from kfp or not.
-
-    Args:
-        image: image string.
-
-    Returns:
-        bool: is the component using kfp spec.
-    """
-    return image != PLACEHOLDER_IMAGE
-
 
 def create_default_config(artifact_repo_location: str,
                           artifact_repo_name: str,
                           artifact_repo_type: str,
                           base_image: str,
                           build_trigger_location: str,
                           build_trigger_name: str,
@@ -373,49 +328,51 @@
                           source_repo_branch: str,
                           source_repo_name: str,
                           source_repo_type: str,
                           storage_bucket_location: str,
                           storage_bucket_name: str,
                           use_ci: bool,
                           vpc_connector: str) -> dict:
-    """Creates defaults.yaml file contents as a dict. This defaults
-       file is used by subsequent functions and by the pipeline
-       files themselves.
-
-    Args:
-        artifact_repo_location: Region of the artifact repo (default use with Artifact Registry).
-        artifact_repo_name: Artifact repo name where components are stored (default use with Artifact Registry).
-        artifact_repo_type: The type of artifact repository to use (e.g. Artifact Registry, JFrog, etc.)        
-        base_image: The image to use in the component base dockerfile.
-        build_trigger_location: The location of the build trigger (for cloud build).
-        build_trigger_name: The name of the build trigger (for cloud build).
-        deployment_framework: The CI tool to use (e.g. cloud build, github actions, etc.)
-        naming_prefix: Unique value used to differentiate pipelines and services across AutoMLOps runs.
-        orchestration_framework: The orchestration framework to use (e.g. kfp, tfx, etc.)
-        pipeline_job_runner_service_account: Service Account to run PipelineJobs.
-        pipeline_job_submission_service_location: The location of the cloud submission service.
-        pipeline_job_submission_service_name: The name of the cloud submission service.
-        pipeline_job_submission_service_type: The tool to host for the cloud submission service (e.g. cloud run, cloud functions).
-        project_id: The project ID.
-        provisioning_framework: The IaC tool to use (e.g. Terraform, Pulumi, etc.)
-        pubsub_topic_name: The name of the pubsub topic to publish to.
-        schedule_location: The location of the scheduler resource.
-        schedule_name: The name of the scheduler resource.
-        schedule_pattern: Cron formatted value used to create a Scheduled retrain job.
-        setup_model_monitoring: Boolean parameter which specifies whether to set up a Vertex AI Model Monitoring Job.
-        source_repo_branch: The branch to use in the source repository.
-        source_repo_name: The name of the source repository to use.
-        source_repo_type: The type of source repository to use (e.g. gitlab, github, etc.)
-        storage_bucket_location: Region of the GS bucket.
-        storage_bucket_name: GS bucket name where pipeline run metadata is stored.
-        use_ci: Flag that determines whether to use Cloud CI/CD.
-        vpc_connector: The name of the vpc connector to use.
+    """Creates defaults.yaml file contents as a dict. This defaults file is used by subsequent
+    functions and by the pipeline files themselves.
+
+    Args:
+        artifact_repo_location (str): Region of the artifact repo (default use with Artifact Registry).
+        artifact_repo_name (str): Artifact repo name where components are stored (default use with
+            Artifact Registry).
+        artifact_repo_type (str): Type of artifact repository to use (e.g. Artifact Registry, JFrog, etc.)        
+        base_image (str): Image to use in the component base dockerfile.
+        build_trigger_location (str): Location of the build trigger (for cloud build).
+        build_trigger_name (str): Name of the build trigger (for cloud build).
+        deployment_framework (str): Name of CI tool to use (e.g. cloud build, github actions, etc.)
+        naming_prefix (str): Unique value used to differentiate pipelines and services across
+            AutoMLOps runs.
+        orchestration_framework (str): Orchestration framework to use (e.g. kfp, tfx, etc.)
+        pipeline_job_runner_service_account (str): Service Account to run PipelineJobs.
+        pipeline_job_submission_service_location (str): Location of the cloud submission service.
+        pipeline_job_submission_service_name (str): Name of the cloud submission service.
+        pipeline_job_submission_service_type (str): Tool to host for the cloud submission service
+            (e.g. cloud run, cloud functions).
+        project_id (str): The project ID.
+        provisioning_framework (str): IaC tool to use (e.g. Terraform, Pulumi, etc.)
+        pubsub_topic_name (str): Name of the pubsub topic to publish to.
+        schedule_location (str): Location of the scheduler resource.
+        schedule_name (str): Name of the scheduler resource.
+        schedule_pattern (str): Cron formatted value used to create a Scheduled retrain job.
+        setup_model_monitoring (bool): Specifies whether to set up a Vertex AI Model Monitoring Job.
+        source_repo_branch (str): Branch to use in the source repository.
+        source_repo_name (str): Name of the source repository to use.
+        source_repo_type (str): Type of source repository to use (e.g. gitlab, github, etc.)
+        storage_bucket_location (str): Region of the GS bucket.
+        storage_bucket_name (str): GS bucket name where pipeline run metadata is stored.
+        use_ci (bool): Specifies whether to use Cloud CI/CD.
+        vpc_connector (str): Name of the vpc connector to use.
 
     Returns:
-        dict: Defaults yaml file content
+        dict: Defaults yaml file content.
     """
     defaults = {}
     defaults['gcp'] = {}
     defaults['gcp']['artifact_repo_location'] = artifact_repo_location
     defaults['gcp']['artifact_repo_name'] = artifact_repo_name
     defaults['gcp']['artifact_repo_type'] = artifact_repo_type
     defaults['gcp']['base_image'] = base_image
@@ -440,29 +397,29 @@
         defaults['gcp']['source_repository_type'] = source_repo_type
     defaults['gcp']['storage_bucket_location'] = storage_bucket_location
     defaults['gcp']['storage_bucket_name'] = storage_bucket_name
     if use_ci:
         defaults['gcp']['vpc_connector'] = vpc_connector
 
     defaults['pipelines'] = {}
-    defaults['pipelines']['gs_pipeline_job_spec_path'] = f'gs://{storage_bucket_name}/pipeline_root/{naming_prefix}/pipeline_job.json'
+    defaults['pipelines']['gs_pipeline_job_spec_path'] = f'gs://{storage_bucket_name}/pipeline_root/{naming_prefix}/pipeline_job.yaml'
     defaults['pipelines']['parameter_values_path'] = GENERATED_PARAMETER_VALUES_PATH
     defaults['pipelines']['pipeline_component_directory'] = 'components'
     defaults['pipelines']['pipeline_job_spec_path'] = GENERATED_PIPELINE_JOB_SPEC_PATH
     defaults['pipelines']['pipeline_region'] = storage_bucket_location
     defaults['pipelines']['pipeline_storage_path'] = f'gs://{storage_bucket_name}/pipeline_root'
 
     defaults['tooling'] = {}
     defaults['tooling']['deployment_framework'] = deployment_framework
     defaults['tooling']['provisioning_framework'] = provisioning_framework
     defaults['tooling']['orchestration_framework'] = orchestration_framework
     defaults['tooling']['use_ci'] = use_ci
 
     if setup_model_monitoring:
-        # These fields to be set when AutoMLOps.monitor() is called
+        # These fields will be set up if and when AutoMLOps.monitor() is called
         defaults['monitoring'] = {}
         defaults['monitoring']['target_field'] = None
         defaults['monitoring']['model_endpoint'] = None
         defaults['monitoring']['alert_emails'] = None
         defaults['monitoring']['auto_retraining_params'] = None
         defaults['monitoring']['drift_thresholds'] = None
         defaults['monitoring']['gs_auto_retraining_params_path'] = None
@@ -474,22 +431,22 @@
         defaults['monitoring']['skew_thresholds'] = None
         defaults['monitoring']['training_dataset'] = None
 
     return defaults
 
 
 def get_required_apis(defaults: dict) -> list:
-    """Returns the list of required APIs based on the user tooling selection
-       determined during the generate() step.
+    """Returns the list of required APIs based on the user tooling selection determined during
+    the generate() step.
 
     Args:
-        defaults: Dictionary contents of the Defaults yaml file (config/defaults.yaml)
+        defaults (dict): Contents of the Defaults yaml file (config/defaults.yaml).
 
     Returns:
-        list: The list of required APIs
+        list: Required APIs.
     """
     required_apis = [
         'cloudbuild.googleapis.com',
         'cloudresourcemanager.googleapis.com',
         'compute.googleapis.com',
         'iamcredentials.googleapis.com',
         'iam.googleapis.com',
@@ -512,23 +469,22 @@
             required_apis.append('sourcerepo.googleapis.com')
         if defaults['gcp']['setup_model_monitoring']:
             required_apis.append('logging.googleapis.com')
     return required_apis
 
 
 def get_provision_min_permissions(defaults: dict) -> list:
-    """Returns the list of minimum required permissions to run
-       the provision() step based on the user tooling selection
-       determined during the generate() step.
+    """Returns the list of minimum required permissions to run the provision() step based on the
+    user tooling selection determined during the generate() step.
 
     Args:
-        defaults: Dictionary contents of the Defaults yaml file (config/defaults.yaml)
+        defaults (dict): Contents of the Defaults yaml file (config/defaults.yaml).
 
     Returns:
-        list: The list of required permissions
+        list: Required permissions.
     """
     required_permissions = [
         'serviceusage.services.enable',
         'serviceusage.services.use',
         'resourcemanager.projects.setIamPolicy',
         'iam.serviceAccounts.list',
         'iam.serviceAccounts.create',
@@ -550,24 +506,23 @@
             required_permissions.extend(['cloudfunctions.functions.get', 'cloudfunctions.functions.create'])
         if defaults['gcp']['source_repository_type'] == CodeRepository.CLOUD_SOURCE_REPOSITORIES.value:
             required_permissions.extend(['source.repos.list', 'source.repos.create'])
     return required_permissions
 
 
 def get_provision_recommended_roles(defaults: dict) -> list:
-    """Returns the list of recommended roles to run
-       the provision() step based on the user tooling selection
-       determined during the generate() step. These roles have
-       the minimum permissions required for provision.
+    """Creates the list of recommended roles to run the provision() step based on the user tooling
+    selection determined during the generate() step. These roles have the minimum permissions
+    required for provision.
 
     Args:
-        defaults: Dictionary contents of the Defaults yaml file (config/defaults.yaml)
+        defaults (dict): Contents of the Defaults yaml file (config/defaults.yaml).
 
     Returns:
-        list: The list of recommended roles
+        list: Recommended provision roles.
     """
     recommended_roles = [
         'roles/serviceusage.serviceUsageAdmin',
         'roles/resourcemanager.projectIamAdmin',
         'roles/iam.serviceAccountAdmin',
         'roles/iam.serviceAccountUser',
         'roles/storage.admin']
@@ -585,25 +540,24 @@
             recommended_roles.append('roles/cloudfunctions.admin')
         if defaults['gcp']['source_repository_type'] == CodeRepository.CLOUD_SOURCE_REPOSITORIES.value:
             recommended_roles.append('roles/source.admin')
     return recommended_roles
 
 
 def get_deploy_with_precheck_min_permissions(defaults: dict) -> list:
-    """Returns the list of minimum required permissions to run
-       the deploy() step based on the user tooling selection
-       determined during the generate() step. This function is called
-       when precheck=True, which makes several API calls to determine if the infra
-       exists to run deploy() and increases the required list of permissions.
+    """Creates the list of minimum required permissions to run the deploy() step based on the user
+    tooling selection, determined during the generate() step. This function is called when
+    precheck=True, which makes several API calls to determine if the infra exists to run deploy()
+    and increases the required list of permissions.
 
     Args:
-        defaults: Dictionary contents of the Defaults yaml file (config/defaults.yaml)
+        defaults (dict): Contents of the Defaults yaml file (config/defaults.yaml).
 
     Returns:
-        list: The list of minimum permissions to deploy with precheck=True
+        list: Minimum permissions to deploy with precheck=True.
     """
     recommended_permissions = [
         'serviceusage.services.get',
         'resourcemanager.projects.getIamPolicy',
         'storage.buckets.update',
         'iam.serviceAccounts.get']
     if defaults['gcp']['artifact_repo_type'] == ArtifactRepository.ARTIFACT_REGISTRY.value:
@@ -620,25 +574,24 @@
             recommended_permissions.append('source.repos.update')
     elif not defaults['tooling']['use_ci']:
         recommended_permissions.extend(['cloudbuild.builds.get', 'aiplatform.pipelineJobs.create'])
     return recommended_permissions
 
 
 def get_deploy_with_precheck_recommended_roles(defaults: dict) -> list:
-    """Returns the list of recommended roles to run
-       the deploy() step based on the user tooling selection
-       determined during the generate() step. This function is called
-       when precheck=True, which makes several API calls to determine if the infra
-       exists to run deploy() and increases the required list of permissions.
+    """Returns the list of recommended roles to run the deploy() step based on the user tooling
+    selection determined during the generate() step. This function is called when precheck=True,
+    which makes several API calls to determine if the infra exists to run deploy() and increases the
+    required list of permissions.
 
     Args:
-        defaults: Dictionary contents of the Defaults yaml file (config/defaults.yaml)
+        defaults (dict): Contents of the Defaults yaml file (config/defaults.yaml).
 
     Returns:
-        list: The list of recommended roles to deploy with precheck=True
+        list: Recommended roles to deploy with precheck=True.
     """
     recommended_roles = [
         'roles/serviceusage.serviceUsageViewer',
         'roles/iam.roleViewer',
         'roles/storage.admin',
         'roles/iam.serviceAccountUser']
     if defaults['gcp']['artifact_repo_type'] == ArtifactRepository.ARTIFACT_REGISTRY.value:
@@ -655,100 +608,97 @@
             recommended_roles.append('roles/source.writer')
     elif not defaults['tooling']['use_ci']:
         recommended_roles.extend(['roles/cloudbuild.builds.editor', 'roles/aiplatform.user'])
     return recommended_roles
 
 
 def get_deploy_without_precheck_min_permissions(defaults: dict) -> list:
-    """Returns the list of minimum required permissions to run
-       the deploy() step based on the user tooling selection
-       determined during the generate() step. This function is called
-       when precheck=False, which decreases the required list of permissions.
+    """Creates the list of minimum required permissions to run the deploy() step based on the user
+    tooling selection determined during the generate() step. This function is called when
+    precheck=False, which decreases the required list of permissions.
 
     Args:
-        defaults: Dictionary contents of the Defaults yaml file (config/defaults.yaml)
+        defaults (dict): Contents of the Defaults yaml file (config/defaults.yaml).
 
     Returns:
-        list: The list of minimum permissions to deploy with precheck=False
+        list: Minimum permissions to deploy with precheck=False.
     """
     recommended_permissions = []
     if defaults['tooling']['use_ci']:
         if defaults['gcp']['source_repository_type'] == CodeRepository.CLOUD_SOURCE_REPOSITORIES.value:
             recommended_permissions.append('source.repos.update')
     elif not defaults['tooling']['use_ci']:
         recommended_permissions.extend(['cloudbuild.builds.create', 'storage.buckets.update', 'aiplatform.pipelineJobs.create'])
     return recommended_permissions
 
 
 def get_deploy_without_precheck_recommended_roles(defaults: dict) -> list:
-    """Returns the list of recommended roles to run
-       the deploy() step based on the user tooling selection
-       determined during the generate() step. This function is called
-       when precheck=False, which decreases the required list of permissions.
+    """Creates the list of recommended roles to run the deploy() step based on the user tooling
+    selection determined during the generate() step. This function is called when precheck=False,
+    which decreases the required list of permissions.
 
     Args:
-        defaults: Dictionary contents of the Defaults yaml file (config/defaults.yaml)
+        defaults (dict): Contents of the Defaults yaml file (config/defaults.yaml).
 
     Returns:
-        list: The list of recommended roles to deploy with precheck=False
+        list: Recommended roles to deploy with precheck=False.
     """
     recommended_roles = []
     if defaults['tooling']['use_ci']:
         if defaults['gcp']['source_repository_type'] == CodeRepository.CLOUD_SOURCE_REPOSITORIES.value:
             recommended_roles.append('roles/source.writer')
     elif not defaults['tooling']['use_ci']:
         recommended_roles.extend(['roles/cloudbuild.builds.editor', 'roles/storage.admin', 'roles/aiplatform.user'])
     return recommended_roles
 
 
 def get_model_monitoring_min_permissions(defaults: dict) -> list:
-    """Returns the list of minimum required permissions to run
-       the monitor() step based on the user tooling selection
-       determined during the generate() step.
+    """Creates the list of minimum required permissions to run the monitor() step based on the user
+    tooling selection determined during the generate() step.
 
     Args:
-        defaults: Dictionary contents of the Defaults yaml file (config/defaults.yaml)
+        defaults (dict): Contents of the Defaults yaml file (config/defaults.yaml).
 
     Returns:
-        list: The list of minimum permissions to create a monitoring job.
+        list: Minimum permissions to create a monitoring job.
     """
     recommended_permissions = [
         'aiplatform.endpoints.list',
         'aiplatform.modelDeploymentMonitoringJobs.list',
         'aiplatform.modelDeploymentMonitoringJobs.create',
         'aiplatform.modelDeploymentMonitoringJobs.update']
     if defaults['monitoring']['auto_retraining_params']:
         recommended_permissions.extend(['storage.buckets.update', 'logging.sinks.get', 'logging.sinks.create',
                                         'logging.sinks.update', 'iam.serviceAccounts.setIamPolicy'])
     return recommended_permissions
 
 
 def get_model_monitoring_recommended_roles(defaults: dict) -> list:
-    """Returns the list of recommended roles to run
-       the monitor() step based on the user tooling selection
-       determined during the generate() step.
+    """Creates the list of recommended roles to run the monitor() step based on the user tooling
+    selection determined during the generate() step.
 
     Args:
-        defaults: Dictionary contents of the Defaults yaml file (config/defaults.yaml)
+        defaults (dict): Contents of the Defaults yaml file (config/defaults.yaml).
 
     Returns:
-        list: The list of recommended roles to create a monitoring job.
+        list: Recommended roles to create a monitoring job.
     """
     recommended_roles = ['roles/aiplatform.user']
     if defaults['monitoring']['auto_retraining_params']:
         recommended_roles.extend(['roles/storage.admin', 'roles/logging.configWriter', 'roles/iam.serviceAccountAdmin'])
     return recommended_roles
 
 
 def account_permissions_warning(operation: str, defaults: dict):
     """Logs the current gcloud account and generates warnings based on the operation being performed.
 
     Args:
-        operation: Specifies which operation is being performed. Available options {provision, deploy_with_precheck, deploy_without_precheck, model_monitoring}
-        defaults: Dictionary contents of the Defaults yaml file (config/defaults.yaml)
+        operation (str): Specifies which operation is being performed. Available options {provision,
+            deploy_with_precheck, deploy_without_precheck, model_monitoring}.
+        defaults (dict): Contents of the Defaults yaml file (config/defaults.yaml).
     """
     bullet_nl = '\n-'
     gcp_account = subprocess.check_output(
         ['gcloud config list account --format "value(core.account)" 2> /dev/null'], shell=True, stderr=subprocess.STDOUT).decode('utf-8').strip('\n')
     if operation == 'provision':
         logging.warning(f'WARNING: Provisioning requires these permissions:\n-{bullet_nl.join(i for i in get_provision_min_permissions(defaults))}\n\n'
                         f'You are currently using: {gcp_account}. Please check your account permissions.\n'
@@ -768,18 +718,18 @@
         logging.warning(f'WARNING: Creating monitoring jobs requires these permissions:\n-{bullet_nl.join(i for i in get_model_monitoring_min_permissions(defaults))}\n\n'
                         f'You are currently using: {gcp_account}. Please check your account permissions.\n'
                         f'The following are the recommended roles for creating monitoring jobs:\n-{bullet_nl.join(i for i in get_model_monitoring_recommended_roles(defaults))}\n')
 
 
 def check_installation_versions(provisioning_framework: str):
     """Checks the version of the provisioning tool (e.g. terraform, gcloud) and generates warning if
-       either the tool is not installed, or if it below the recommended version.
+    either the tool is not installed, or if it below the recommended version.
 
     Args:
-        provisioning_framework: The IaC tool to use (e.g. Terraform, Pulumi, etc.)
+        provisioning_framework (str): The IaC tool to use (e.g. Terraform, Pulumi, etc.).
     """
     if provisioning_framework == Provisioner.GCLOUD.value:
         try:
             gcloud_sdk_version = subprocess.check_output(
                 ['gcloud info --format="value(basic.version)" 2> /dev/null'], shell=True, stderr=subprocess.STDOUT).decode('utf-8').strip('\n')
             if version.parse(MIN_GCLOUD_SDK_VERSION) > version.parse(gcloud_sdk_version):
                 logging.warning(f'WARNING: You are currently using version {gcloud_sdk_version} of the gcloud sdk. We recommend using at least version {MIN_GCLOUD_SDK_VERSION}.\n '
@@ -807,20 +757,19 @@
         except subprocess.CalledProcessError:
             logging.warning('WARNING: You do not have terraform installed. Please install terraform.\n')
 
     # check for pulumi versions
 
 
 def precheck_deployment_requirements(defaults: dict):
-    """Checks to see if the necessary MLOps infra exists to run
-       the deploy() step based on the user tooling selection
-       determined during the generate() step.
+    """Checks to see if the necessary MLOps infra exists to run the deploy() step based on the user
+    tooling selection determined during the generate() step.
 
     Args:
-        defaults: Dictionary contents of the Defaults yaml file (config/defaults.yaml)
+        defaults: Contents of the Defaults yaml file (config/defaults.yaml).
     """
     use_ci = defaults['tooling']['use_ci']
     artifact_repo_location = defaults['gcp']['artifact_repo_location']
     artifact_repo_name = defaults['gcp']['artifact_repo_name']
     artifact_repo_type = defaults['gcp']['artifact_repo_type']
     storage_bucket_name = defaults['gcp']['storage_bucket_name']
     pipeline_job_runner_service_account = defaults['gcp']['pipeline_job_runner_service_account']
@@ -939,15 +888,16 @@
             except Exception as err:
                 raise RuntimeError(f'Cloud Run Pipeline Job Submission Service {pipeline_job_submission_service_name} not found in project {project}. '
                                     'Please redeploy the submission service and continue.') from err
 
         if pipeline_job_submission_service_type == PipelineJobSubmitter.CLOUD_FUNCTIONS.value:
             logging.info(f'Checking for Cloud Functions Pipeline Job Submission Service in project {project}...')
             service = discovery.build('cloudfunctions', 'v1', credentials=credentials, cache_discovery=False)
-            request = service.projects().locations().functions().get(name=f'projects/{project}/locations/{pipeline_job_submission_service_location}/functions/{pipeline_job_submission_service_name}')
+            request = service.projects().locations().functions().get(
+                name=f'projects/{project}/locations/{pipeline_job_submission_service_location}/functions/{pipeline_job_submission_service_name}')
             try:
                 request.execute()
             except Exception as err:
                 raise RuntimeError(f'Cloud Functions Pipeline Job Submission Service {pipeline_job_submission_service_name} not found in project {project}. '
                                     'Please redeploy the submission service and continue.') from err         
 
         if deployment_framework == Deployer.CLOUDBUILD.value:
@@ -965,15 +915,15 @@
     logging.info('Precheck successfully completed, continuing to deployment.\n')
 
 
 def resources_generation_manifest(defaults: dict):
     """Logs urls of generated resources.
 
     Args:
-        defaults: Dictionary contents of the Defaults yaml file (config/defaults.yaml)
+        defaults (dict): Contents of the Defaults yaml file (config/defaults.yaml).
     """
     logging.info('Please wait for this build job to complete.')
     logging.info('\n'
                  '#################################################################\n'
                  '#                                                               #\n'
                  '#                       RESOURCES MANIFEST                      #\n'
                  '#---------------------------------------------------------------#\n'
@@ -1010,7 +960,97 @@
                 f'''Pipeline Job Submission Service (Cloud Functions): https://console.cloud.google.com/functions/details/{defaults['gcp']['pipeline_job_submission_service_location']}/{defaults['gcp']['pipeline_job_submission_service_name']}''')
         logging.info(
             f'''Pub/Sub Queueing Service Topic: https://console.cloud.google.com/cloudpubsub/topic/detail/{defaults['gcp']['pubsub_topic_name']}''')
         logging.info('Pub/Sub Queueing Service Subscriptions: https://console.cloud.google.com/cloudpubsub/subscription/list')
         if defaults['gcp']['schedule_pattern'] != DEFAULT_SCHEDULE_PATTERN:
             logging.info(
                 'Cloud Scheduler Job: https://console.cloud.google.com/cloudscheduler')
+
+def render_jinja(template_path, **template_vars):
+    """Renders a Jinja2 template with provided variables.
+
+    Args:
+        template_path (str): The path to the Jinja2 template file.
+        **template_vars: Keyword arguments representing variables to substitute in the template.
+
+    Returns:
+        str: The rendered template as a string.
+    """
+    with open(template_path, 'r', encoding='utf-8') as f:
+        template = Template(f.read())
+        return template.render(**template_vars)
+
+def coalesce(*arg):
+    """Creates the first non-None value from a sequence of arguments.
+
+    Returns:
+        The first non-None argument, or None if all arguments are None.
+    """
+    for el in arg:
+        if el is not None:
+            return el
+    return None
+
+def git_workflow():
+    """Initializes a git repo if one doesn't already exist,
+    then pushes to the specified branch and triggers a build job.
+    """
+    defaults = read_yaml_file(GENERATED_DEFAULTS_FILE)
+    deployment_framework = defaults['tooling']['deployment_framework']
+    source_repository_type = defaults['gcp']['source_repository_type']
+    if source_repository_type == CodeRepository.CLOUD_SOURCE_REPOSITORIES.value:
+        git_remote_origin_url = f'''https://source.developers.google.com/p/{defaults['gcp']['project_id']}/r/{defaults['gcp']['source_repository_name']}'''
+    elif source_repository_type == CodeRepository.GITHUB.value:
+        git_remote_origin_url = f'''git@github.com:{defaults['gcp']['source_repository_name']}.git'''
+    elif source_repository_type == CodeRepository.GITLAB.value:
+        git_remote_origin_url = f'''git@gitlab.com:{defaults['gcp']['source_repository_name']}.git'''
+    elif source_repository_type == CodeRepository.BITBUCKET.value:
+        git_remote_origin_url = f'''git@bitbucket.org:{defaults['gcp']['source_repository_name']}.git'''
+    else:
+        raise ValueError(f'source_repository_type "{source_repository_type}" not an available option.')
+
+    if not os.path.exists(f'{BASE_DIR}.git'):
+
+        # Initialize git and configure credentials
+        execute_process(f'git -C {BASE_DIR} init', to_null=False)
+        if source_repository_type == CodeRepository.CLOUD_SOURCE_REPOSITORIES.value:
+            execute_process(
+                f'''git -C {BASE_DIR} config --global credential.'https://source.developers.google.com'.helper gcloud.sh''', to_null=False)
+
+        # Add repo and branch
+        execute_process(
+            f'''git -C {BASE_DIR} remote add origin {git_remote_origin_url}''', to_null=False)
+        execute_process(
+            f'''git -C {BASE_DIR} checkout -B {defaults['gcp']['source_repository_branch']}''', to_null=False)
+        has_remote_branch = subprocess.check_output(
+            [f'''git -C {BASE_DIR} ls-remote origin {defaults['gcp']['source_repository_branch']}'''], shell=True, stderr=subprocess.STDOUT)
+
+        write_file(
+            f'{BASE_DIR}.gitignore',
+            render_jinja(template_path=import_files(GITOPS_TEMPLATES_PATH) / 'gitignore.j2'),
+            'w')
+
+        # This will initialize the branch, a second push will be required to trigger the cloudbuild job after initializing
+        if not has_remote_branch:
+            execute_process(f'git -C {BASE_DIR} add .gitignore', to_null=False)
+            execute_process(f'''git -C {BASE_DIR} commit -m 'init' ''', to_null=False)
+            execute_process(
+                f'''git -C {BASE_DIR} push origin {defaults['gcp']['source_repository_branch']} --force''', to_null=False)
+
+    # Check for remote origin url mismatch
+    actual_remote = subprocess.check_output(
+        [f'git -C {BASE_DIR} config --get remote.origin.url'], shell=True, stderr=subprocess.STDOUT).decode('utf-8').strip('\n')
+    if actual_remote != git_remote_origin_url:
+        raise RuntimeError(
+            f'Expected remote origin url {git_remote_origin_url} but found {actual_remote}. Reset your remote origin url to continue.')
+
+    # Add, commit, and push changes to CSR
+    execute_process(f'git -C {BASE_DIR} add .', to_null=False)
+    execute_process(f'''git -C {BASE_DIR} commit -m 'Run AutoMLOps' ''', to_null=False)
+    execute_process(
+        f'''git -C {BASE_DIR} push origin {defaults['gcp']['source_repository_branch']} --force''', to_null=False)
+    # pylint: disable=logging-fstring-interpolation
+    logging.info(
+        f'''Pushing code to {defaults['gcp']['source_repository_branch']} branch, triggering build...''')
+    if deployment_framework == Deployer.CLOUDBUILD.value:
+        logging.info(
+            f'''Cloud Build job running at: https://console.cloud.google.com/cloud-build/builds;region={defaults['gcp']['build_trigger_location']}''')
```

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops.egg-info/PKG-INFO` & `google_cloud_automlops-1.3.0/google_cloud_automlops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.2.9
+Version: 1.3.0
 Summary: Build MLOps Pipelines in Minutes.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -20,18 +20,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docopt==0.6.2
 Requires-Dist: docstring-parser==0.15
 Requires-Dist: google-api-python-client==2.97.0
 Requires-Dist: google-auth==2.22.0
 Requires-Dist: importlib-resources==6.0.1
-Requires-Dist: Jinja2==3.1.2
+Requires-Dist: Jinja2==3.1.4
+Requires-Dist: kfp>=2.0.0
 Requires-Dist: packaging==23.1
 Requires-Dist: pipreqs==0.4.13
-Requires-Dist: pydantic==2.3.0
+Requires-Dist: pydantic==2.4.0
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: yarg==0.1.9
 
 # AutoMLOps
 
 AutoMLOps is a service that generates, provisions, deploys, and monitors CI/CD integrated MLOps pipelines, bridging the gap between Data Science and DevOps. AutoMLOps provides a repeatable process that dramatically reduces the time required to build MLOps pipelines. The service generates a containerized MLOps codebase, provides infrastructure-as-code to provision and maintain the underlying MLOps infra, provides deployment functionalities to trigger and run MLOps pipelines, monitoring capabilities to monitor models deployed to live endpoints, and optional automatic retraining of models on a recurring basis or if anomalies are detected during monitoring.
 
@@ -48,14 +49,15 @@
 # Dependencies
 - `docopt==0.6.2`
 - `docstring-parser==0.15`
 - `google-api-python-client==2.97.0`
 - `google-auth==2.22.0`
 - `importlib-resources==6.0.1`
 - `Jinja2==3.1.2`
+- `kfp>=2.0.0`
 - `packaging==23.1`
 - `pipreqs==0.4.13`
 - `pydantic==2.3.0`
 - `PyYAML==6.0.1`
 - `yarg==0.1.9`
 
 # Usage
@@ -115,15 +117,15 @@
 
 **Provisioning Frameworks**: Stands up necessary infra to run MLOps pipelines
 - gcloud
 - terraform
 - [coming soon] pulumi
 
 **Source Code Repositories**: Repository for versioning generated MLOps code
-- Cloud Source Repositories
+- [deprecating soon] Cloud Source Repositories
 - Bitbucket
 - Github
 - Gitlab
 
 # Prerequisites
 ### Generate
 In order to use `AutoMLOps.generate(...)`, the following are required:
@@ -136,15 +138,15 @@
 
 In order to use `AutoMLOps.provision(...)` with `provisioning_framework='terraform'`, the following are recommended:
 - [Terraform v1.5.6](https://www.terraform.io/downloads.html)
 
 ### Deploy
 In order to use `AutoMLOps.deploy(...)` with `use_ci=False`, the following are required:
 - Local python environment with these packages installed:
-    - `kfp<2.0.0`
+    - `kfp>=2.0.0`
     - `google-cloud-aiplatform`
     - `google-cloud-pipeline-components`
     - `google-cloud-storage`
     - `pyyaml`
 
 In order to use `AutoMLOps.deploy(...)` with `use_ci=True`, the following are required:
 - `git` installed
@@ -356,15 +358,15 @@
 - `workload_identity_provider`: Provider for workload identity federation.
 - `workload_identity_service_account`: Service account for workload identity federation (specify the full string).
 
 AutoMLOps will generate the resources specified by these parameters (e.g. Artifact Registry, Cloud Source Repo, etc.). If use_ci is set to True, AutoMLOps will turn the outputted AutoMLOps/ directory into a Git repo and use it for the source repo. If a cron formatted str is given as an arg for `schedule_pattern` then it will set up a Cloud Schedule to run accordingly. If `setup_model_monitoring` is set to true, a model_monitoring/ directory will be created and a monitoring section will be added to config/defaults.yaml with empty values. These values are then set by running `AutoMLOps.monitor()`.
 
 # Generating Code
 
-AutoMLOps generates code that is compatible with `kfp<2.0.0`. Upon running `AutoMLOps.generate(project_id='project-id', pipeline_params=pipeline_params, setup_model_monitoring=True, use_ci=True)`, a series of directories will be generated automatically:
+AutoMLOps generates code that is compatible with `kfp>=2.0.0`. Upon running `AutoMLOps.generate(project_id='project-id', pipeline_params=pipeline_params, setup_model_monitoring=True, use_ci=True)`, a series of directories will be generated automatically:
 
 ```bash
 .
 ├── components                                     : Custom vertex pipeline components.
     ├──component_base                              : Contains all the python files, Dockerfile and requirements.txt
         ├── Dockerfile                             : Dockerfile containing all the python files for the components.
         ├── requirements.txt                       : Package requirements for all the python files for the components.
```

### Comparing `google-cloud-automlops-1.2.9/google_cloud_automlops.egg-info/SOURCES.txt` & `google_cloud_automlops-1.3.0/google_cloud_automlops.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,100 +5,87 @@
 google_cloud_automlops/__init__.py
 google_cloud_automlops.egg-info/PKG-INFO
 google_cloud_automlops.egg-info/SOURCES.txt
 google_cloud_automlops.egg-info/dependency_links.txt
 google_cloud_automlops.egg-info/requires.txt
 google_cloud_automlops.egg-info/top_level.txt
 google_cloud_automlops/deployments/__init__.py
-google_cloud_automlops/deployments/configs.py
-google_cloud_automlops/deployments/enums.py
-google_cloud_automlops/deployments/cloudbuild/__init__.py
-google_cloud_automlops/deployments/cloudbuild/builder.py
-google_cloud_automlops/deployments/cloudbuild/templates/__init__.py
-google_cloud_automlops/deployments/cloudbuild/templates/cloudbuild.yaml.j2
-google_cloud_automlops/deployments/github_actions/__init__.py
-google_cloud_automlops/deployments/github_actions/builder.py
-google_cloud_automlops/deployments/github_actions/templates/__init__.py
-google_cloud_automlops/deployments/github_actions/templates/github_actions.yaml.j2
-google_cloud_automlops/deployments/gitops/__init__.py
-google_cloud_automlops/deployments/gitops/git_utils.py
-google_cloud_automlops/deployments/gitops/templates/__init__.py
-google_cloud_automlops/deployments/gitops/templates/gitignore.j2
+google_cloud_automlops/deployments/base.py
+google_cloud_automlops/deployments/cloudbuild.py
+google_cloud_automlops/deployments/github_actions.py
+google_cloud_automlops/deployments/templates/__init__.py
+google_cloud_automlops/deployments/templates/cloudbuild/__init__.py
+google_cloud_automlops/deployments/templates/cloudbuild/cloudbuild.yaml.j2
+google_cloud_automlops/deployments/templates/github_actions/__init__.py
+google_cloud_automlops/deployments/templates/github_actions/github_actions.yaml.j2
 google_cloud_automlops/orchestration/__init__.py
-google_cloud_automlops/orchestration/configs.py
-google_cloud_automlops/orchestration/enums.py
-google_cloud_automlops/orchestration/kfp/__init__.py
-google_cloud_automlops/orchestration/kfp/builder.py
-google_cloud_automlops/orchestration/kfp/scaffold.py
-google_cloud_automlops/orchestration/kfp/templates/README.md.j2
-google_cloud_automlops/orchestration/kfp/templates/__init__.py
-google_cloud_automlops/orchestration/kfp/templates/components/__init__.py
-google_cloud_automlops/orchestration/kfp/templates/components/component_base/Dockerfile.j2
-google_cloud_automlops/orchestration/kfp/templates/components/component_base/__init__.py
-google_cloud_automlops/orchestration/kfp/templates/components/component_base/src/__init__.py
-google_cloud_automlops/orchestration/kfp/templates/components/component_base/src/task.py.j2
-google_cloud_automlops/orchestration/kfp/templates/model_monitoring/__init__.py
-google_cloud_automlops/orchestration/kfp/templates/model_monitoring/monitor.py.j2
-google_cloud_automlops/orchestration/kfp/templates/model_monitoring/requirements.txt.j2
-google_cloud_automlops/orchestration/kfp/templates/pipelines/__init__.py
-google_cloud_automlops/orchestration/kfp/templates/pipelines/pipeline.py.j2
-google_cloud_automlops/orchestration/kfp/templates/pipelines/pipeline_runner.py.j2
-google_cloud_automlops/orchestration/kfp/templates/pipelines/requirements.txt.j2
-google_cloud_automlops/orchestration/kfp/templates/scripts/__init__.py
-google_cloud_automlops/orchestration/kfp/templates/scripts/build_components.sh.j2
-google_cloud_automlops/orchestration/kfp/templates/scripts/build_pipeline_spec.sh.j2
-google_cloud_automlops/orchestration/kfp/templates/scripts/create_model_monitoring_job.sh.j2
-google_cloud_automlops/orchestration/kfp/templates/scripts/publish_to_topic.sh.j2
-google_cloud_automlops/orchestration/kfp/templates/scripts/run_all.sh.j2
-google_cloud_automlops/orchestration/kfp/templates/scripts/run_pipeline.sh.j2
-google_cloud_automlops/orchestration/kfp/templates/services/__init__.py
-google_cloud_automlops/orchestration/kfp/templates/services/submission_service/Dockerfile.j2
-google_cloud_automlops/orchestration/kfp/templates/services/submission_service/__init__.py
-google_cloud_automlops/orchestration/kfp/templates/services/submission_service/main.py.j2
-google_cloud_automlops/orchestration/kfp/templates/services/submission_service/requirements.txt.j2
+google_cloud_automlops/orchestration/base.py
+google_cloud_automlops/orchestration/kfp.py
+google_cloud_automlops/orchestration/templates/__init__.py
+google_cloud_automlops/orchestration/templates/kfp/README.md.j2
+google_cloud_automlops/orchestration/templates/kfp/__init__.py
+google_cloud_automlops/orchestration/templates/kfp/components/__init__.py
+google_cloud_automlops/orchestration/templates/kfp/components/component_base/Dockerfile.j2
+google_cloud_automlops/orchestration/templates/kfp/components/component_base/__init__.py
+google_cloud_automlops/orchestration/templates/kfp/components/component_base/src/__init__.py
+google_cloud_automlops/orchestration/templates/kfp/components/component_base/src/task.py.j2
+google_cloud_automlops/orchestration/templates/kfp/model_monitoring/__init__.py
+google_cloud_automlops/orchestration/templates/kfp/model_monitoring/monitor.py.j2
+google_cloud_automlops/orchestration/templates/kfp/model_monitoring/requirements.txt.j2
+google_cloud_automlops/orchestration/templates/kfp/pipelines/__init__.py
+google_cloud_automlops/orchestration/templates/kfp/pipelines/pipeline.py.j2
+google_cloud_automlops/orchestration/templates/kfp/pipelines/pipeline_runner.py.j2
+google_cloud_automlops/orchestration/templates/kfp/pipelines/requirements.txt.j2
+google_cloud_automlops/orchestration/templates/kfp/scripts/__init__.py
+google_cloud_automlops/orchestration/templates/kfp/scripts/build_components.sh.j2
+google_cloud_automlops/orchestration/templates/kfp/scripts/build_pipeline_spec.sh.j2
+google_cloud_automlops/orchestration/templates/kfp/scripts/create_model_monitoring_job.sh.j2
+google_cloud_automlops/orchestration/templates/kfp/scripts/publish_to_topic.sh.j2
+google_cloud_automlops/orchestration/templates/kfp/scripts/run_all.sh.j2
+google_cloud_automlops/orchestration/templates/kfp/scripts/run_pipeline.sh.j2
+google_cloud_automlops/orchestration/templates/kfp/services/__init__.py
+google_cloud_automlops/orchestration/templates/kfp/services/submission_service/Dockerfile.j2
+google_cloud_automlops/orchestration/templates/kfp/services/submission_service/__init__.py
+google_cloud_automlops/orchestration/templates/kfp/services/submission_service/main.py.j2
+google_cloud_automlops/orchestration/templates/kfp/services/submission_service/requirements.txt.j2
 google_cloud_automlops/provisioning/__init__.py
-google_cloud_automlops/provisioning/configs.py
-google_cloud_automlops/provisioning/enums.py
-google_cloud_automlops/provisioning/gcloud/__init__.py
-google_cloud_automlops/provisioning/gcloud/builder.py
-google_cloud_automlops/provisioning/gcloud/templates/__init__.py
-google_cloud_automlops/provisioning/gcloud/templates/provision_resources.sh.j2
-google_cloud_automlops/provisioning/pulumi/__init__.py
-google_cloud_automlops/provisioning/pulumi/builder.py
-google_cloud_automlops/provisioning/terraform/__init__.py
-google_cloud_automlops/provisioning/terraform/builder.py
-google_cloud_automlops/provisioning/terraform/templates/__init__.py
-google_cloud_automlops/provisioning/terraform/templates/provision_resources.sh.j2
-google_cloud_automlops/provisioning/terraform/templates/environment/__init__.py
-google_cloud_automlops/provisioning/terraform/templates/environment/data.tf.j2
-google_cloud_automlops/provisioning/terraform/templates/environment/iam.tf.j2
-google_cloud_automlops/provisioning/terraform/templates/environment/main.tf.j2
-google_cloud_automlops/provisioning/terraform/templates/environment/outputs.tf.j2
-google_cloud_automlops/provisioning/terraform/templates/environment/provider.tf.j2
-google_cloud_automlops/provisioning/terraform/templates/environment/variables.auto.tfvars.j2
-google_cloud_automlops/provisioning/terraform/templates/environment/variables.tf.j2
-google_cloud_automlops/provisioning/terraform/templates/environment/versions.tf.j2
-google_cloud_automlops/provisioning/terraform/templates/state_bucket/__init__.py
-google_cloud_automlops/provisioning/terraform/templates/state_bucket/main.tf.j2
-google_cloud_automlops/provisioning/terraform/templates/state_bucket/variables.auto.tfvars.j2
-google_cloud_automlops/provisioning/terraform/templates/state_bucket/variables.tf.j2
+google_cloud_automlops/provisioning/base.py
+google_cloud_automlops/provisioning/gcloud.py
+google_cloud_automlops/provisioning/pulumi.py
+google_cloud_automlops/provisioning/terraform.py
+google_cloud_automlops/provisioning/templates/__init__.py
+google_cloud_automlops/provisioning/templates/gcloud/__init__.py
+google_cloud_automlops/provisioning/templates/gcloud/provision_resources.sh.j2
+google_cloud_automlops/provisioning/templates/terraform/__init__.py
+google_cloud_automlops/provisioning/templates/terraform/provision_resources.sh.j2
+google_cloud_automlops/provisioning/templates/terraform/environment/__init__.py
+google_cloud_automlops/provisioning/templates/terraform/environment/data.tf.j2
+google_cloud_automlops/provisioning/templates/terraform/environment/iam.tf.j2
+google_cloud_automlops/provisioning/templates/terraform/environment/main.tf.j2
+google_cloud_automlops/provisioning/templates/terraform/environment/outputs.tf.j2
+google_cloud_automlops/provisioning/templates/terraform/environment/provider.tf.j2
+google_cloud_automlops/provisioning/templates/terraform/environment/variables.auto.tfvars.j2
+google_cloud_automlops/provisioning/templates/terraform/environment/variables.tf.j2
+google_cloud_automlops/provisioning/templates/terraform/environment/versions.tf.j2
+google_cloud_automlops/provisioning/templates/terraform/state_bucket/__init__.py
+google_cloud_automlops/provisioning/templates/terraform/state_bucket/main.tf.j2
+google_cloud_automlops/provisioning/templates/terraform/state_bucket/variables.auto.tfvars.j2
+google_cloud_automlops/provisioning/templates/terraform/state_bucket/variables.tf.j2
 google_cloud_automlops/utils/__init__.py
 google_cloud_automlops/utils/constants.py
+google_cloud_automlops/utils/enums.py
 google_cloud_automlops/utils/utils.py
+google_cloud_automlops/utils/templates/__init__.py
+google_cloud_automlops/utils/templates/gitignore.j2
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/deployments/__init__.py
-tests/unit/deployments/cloudbuild/__init__.py
-tests/unit/deployments/cloudbuild/builder_test.py
-tests/unit/deployments/github_actions/__init__.py
-tests/unit/deployments/github_actions/builder_test.py
+tests/unit/deployments/cloudbuild_tests.py
+tests/unit/deployments/github_actions_tests.py
 tests/unit/orchestration/__init__.py
-tests/unit/orchestration/kfp/__init__.py
-tests/unit/orchestration/kfp/builder_test.py
-tests/unit/orchestration/kfp/scaffold_test.py
+tests/unit/orchestration/base_tests.py
+tests/unit/orchestration/kfp_tests.py
 tests/unit/provisioning/__init__.py
-tests/unit/provisioning/gcloud/__init__.py
-tests/unit/provisioning/gcloud/builder_test.py
-tests/unit/provisioning/terraform/__init__.py
-tests/unit/provisioning/terraform/builder_test.py
+tests/unit/provisioning/gcloud_tests.py
+tests/unit/provisioning/terraform_tests.py
 tests/unit/utils/__init__.py
 tests/unit/utils/utils_test.py
```

### Comparing `google-cloud-automlops-1.2.9/setup.py` & `google_cloud_automlops-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as file:
     readme_contents = file.read()
 
 setup(
     name='google-cloud-automlops',
-    version='1.2.9',
+    version='1.3.0',
     description='Build MLOps Pipelines in Minutes.',
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     url='https://github.com/GoogleCloudPlatform/automlops',
     author='Sean Rastatter',
     author_email='srastatter@google.com',
     license='Apache-2.0',
@@ -33,18 +33,19 @@
     include_package_data=True,
     package_data={'':['*.j2']},
     install_requires=['docopt==0.6.2',
                       'docstring-parser==0.15',
                       'google-api-python-client==2.97.0',
                       'google-auth==2.22.0',
                       'importlib-resources==6.0.1',
-                      'Jinja2==3.1.2',
+                      'Jinja2==3.1.4',
+                      'kfp>=2.0.0',
                       'packaging==23.1',
                       'pipreqs==0.4.13',
-                      'pydantic==2.3.0',
+                      'pydantic==2.4.0',
                       'PyYAML==6.0.1',
                       'yarg==0.1.9'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX :: Linux',
```

### Comparing `google-cloud-automlops-1.2.9/tests/__init__.py` & `google_cloud_automlops-1.3.0/tests/unit/provisioning/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/tests/unit/__init__.py` & `google_cloud_automlops-1.3.0/tests/unit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.2.9/tests/unit/deployments/cloudbuild/builder_test.py` & `google_cloud_automlops-1.3.0/tests/unit/deployments/cloudbuild_tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,19 +11,32 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint: disable=line-too-long
 # pylint: disable=missing-module-docstring
 
+try:
+    from importlib.resources import files as import_files
+except ImportError:
+    # Try backported to PY<37 `importlib_resources`
+    from importlib_resources import files as import_files
+
 from typing import List
 
 import pytest
 
-from google_cloud_automlops.deployments.cloudbuild.builder import create_cloudbuild_jinja
+from google_cloud_automlops.utils.constants import (
+    BASE_DIR,
+    CLOUDBUILD_TEMPLATES_PATH,
+    COMPONENT_BASE_RELATIVE_PATH,
+    GENERATED_LICENSE,
+    GENERATED_PARAMETER_VALUES_PATH
+)
+from google_cloud_automlops.utils.utils import render_jinja
 
 @pytest.mark.parametrize(
     '''artifact_repo_location, artifact_repo_name, naming_prefix,'''
     '''project_id, pubsub_topic_name, use_ci, is_included,'''
     '''expected_output_snippets''',
     [
         (
@@ -77,20 +90,28 @@
         naming_prefix: Unique value used to differentiate pipelines and services across AutoMLOps runs.
         project_id: The project ID.
         pubsub_topic_name: The name of the pubsub topic to publish to.
         use_ci: Flag that determines whether to use Cloud CI/CD.
         is_included: Boolean that determines whether to check if the expected_output_snippets exist in the string or not.
         expected_output_snippets: Strings that are expected to be included (or not) based on the is_included boolean.
     """
-    cloudbuild_config = create_cloudbuild_jinja(
-        artifact_repo_location,
-        artifact_repo_name,
-        naming_prefix,
-        project_id,
-        pubsub_topic_name,
-        use_ci)
+    component_base_relative_path = COMPONENT_BASE_RELATIVE_PATH if use_ci else f'{BASE_DIR}{COMPONENT_BASE_RELATIVE_PATH}'
+    template_file = import_files(CLOUDBUILD_TEMPLATES_PATH) / 'cloudbuild.yaml.j2'
+
+    cloudbuild_config = render_jinja(
+        template_path=template_file,
+        artifact_repo_location=artifact_repo_location,
+        artifact_repo_name=artifact_repo_name,
+        component_base_relative_path=component_base_relative_path,
+        generated_licensed=GENERATED_LICENSE,
+        generated_parameter_values_path=GENERATED_PARAMETER_VALUES_PATH,
+        naming_prefix=naming_prefix,
+        project_id=project_id,
+        pubsub_topic_name=pubsub_topic_name,
+        use_ci=use_ci
+    )
 
     for snippet in expected_output_snippets:
         if is_included:
             assert snippet in cloudbuild_config
         elif not is_included:
             assert snippet not in cloudbuild_config
```

### Comparing `google-cloud-automlops-1.2.9/tests/unit/provisioning/gcloud/builder_test.py` & `google_cloud_automlops-1.3.0/tests/unit/provisioning/gcloud_tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,33 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint: disable=line-too-long
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-module-docstring
 
+try:
+    from importlib.resources import files as import_files
+except ImportError:
+    # Try backported to PY<37 `importlib_resources`
+    from importlib_resources import files as import_files
+
 from typing import List
 
 import pytest
 
-from google_cloud_automlops.provisioning.gcloud.builder import provision_resources_script_jinja
+from google_cloud_automlops.utils.utils import render_jinja
+
+from google_cloud_automlops.utils.constants import (
+    BASE_DIR,
+    GCLOUD_TEMPLATES_PATH,
+    GENERATED_LICENSE,
+    GENERATED_PARAMETER_VALUES_PATH,
+    IAM_ROLES_RUNNER_SA,
+)
 
 @pytest.mark.parametrize(
     '''artifact_repo_location, artifact_repo_name, artifact_repo_type, build_trigger_location,'''
     '''build_trigger_name, deployment_framework, naming_prefix, pipeline_job_runner_service_account,'''
     '''pipeline_job_submission_service_location, pipeline_job_submission_service_name, pipeline_job_submission_service_type,'''
     '''project_id, pubsub_topic_name,'''
     '''required_apis,'''
@@ -183,38 +197,43 @@
         source_repo_name: The name of the source repository to use.
         source_repo_type: The type of source repository to use (e.g. gitlab, github, etc.)
         storage_bucket_location: Region of the GS bucket.
         storage_bucket_name: GS bucket name where pipeline run metadata is stored.
         use_ci: Flag that determines whether to use Cloud CI/CD.
         vpc_connector: The name of the vpc connector to use.
     """
-    provision_resources_script = provision_resources_script_jinja(
-        artifact_repo_location=artifact_repo_location,
-        artifact_repo_name=artifact_repo_name,
-        artifact_repo_type=artifact_repo_type,
-        build_trigger_location=build_trigger_location,
-        build_trigger_name=build_trigger_name,
-        deployment_framework=deployment_framework,
-        naming_prefix=naming_prefix,
-        pipeline_job_runner_service_account=pipeline_job_runner_service_account,
-        pipeline_job_submission_service_location=pipeline_job_submission_service_location,
-        pipeline_job_submission_service_name=pipeline_job_submission_service_name,
-        pipeline_job_submission_service_type=pipeline_job_submission_service_type,
-        project_id=project_id,
-        pubsub_topic_name=pubsub_topic_name,
-        required_apis=required_apis,
-        schedule_location=schedule_location,
-        schedule_name=schedule_name,
-        schedule_pattern=schedule_pattern,
-        source_repo_branch=source_repo_branch,
-        source_repo_name=source_repo_name,
-        source_repo_type=source_repo_type,
-        storage_bucket_location=storage_bucket_location,
-        storage_bucket_name=storage_bucket_name,
-        use_ci=use_ci,
-        vpc_connector=vpc_connector)
+    provision_resources_script = render_jinja(
+            template_path=import_files(GCLOUD_TEMPLATES_PATH) / 'provision_resources.sh.j2',
+            artifact_repo_location=artifact_repo_location,
+            artifact_repo_name=artifact_repo_name,
+            artifact_repo_type=artifact_repo_type,
+            base_dir=BASE_DIR,
+            build_trigger_location=build_trigger_location,
+            build_trigger_name=build_trigger_name,
+            deployment_framework=deployment_framework,
+            generated_license=GENERATED_LICENSE,
+            generated_parameter_values_path=GENERATED_PARAMETER_VALUES_PATH,
+            naming_prefix=naming_prefix,
+            pipeline_job_runner_service_account=pipeline_job_runner_service_account,
+            pipeline_job_submission_service_location=pipeline_job_submission_service_location,
+            pipeline_job_submission_service_name=pipeline_job_submission_service_name,
+            pipeline_job_submission_service_type=pipeline_job_submission_service_type,
+            project_id=project_id,
+            pubsub_topic_name=pubsub_topic_name,
+            required_apis=required_apis,
+            required_iam_roles=IAM_ROLES_RUNNER_SA,
+            schedule_location=schedule_location,
+            schedule_name=schedule_name,
+            schedule_pattern=schedule_pattern,
+            source_repo_branch=source_repo_branch,
+            source_repo_name=source_repo_name,
+            source_repo_type=source_repo_type,
+            storage_bucket_location=storage_bucket_location,
+            storage_bucket_name=storage_bucket_name,
+            use_ci=use_ci,
+            vpc_connector=vpc_connector)
 
     for snippet in expected_output_snippets:
         if is_included:
             assert snippet in provision_resources_script
         elif not is_included:
             assert snippet not in provision_resources_script
```

### Comparing `google-cloud-automlops-1.2.9/tests/unit/provisioning/terraform/builder_test.py` & `google_cloud_automlops-1.3.0/tests/unit/provisioning/terraform_tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,30 +12,31 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint: disable=line-too-long
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-module-docstring
 
+try:
+    from importlib.resources import files as import_files
+except ImportError:
+    # Try backported to PY<37 `importlib_resources`
+    from importlib_resources import files as import_files
 from typing import List
 
 import pytest
 
-from google_cloud_automlops.utils.constants import GENERATED_LICENSE
-from google_cloud_automlops.provisioning.terraform.builder import (
-    create_environment_data_tf_jinja,
-    create_environment_iam_tf_jinja,
-    create_environment_main_tf_jinja,
-    create_environment_outputs_tf_jinja,
-    create_environment_provider_tf_jinja,
-    create_environment_variables_tf_jinja,
-    create_environment_versions_tf_jinja,
-    create_provision_resources_script_jinja,
-    create_state_bucket_variables_tf_jinja,
-    create_state_bucket_main_tf_jinja
+from google_cloud_automlops.utils.utils import render_jinja
+
+from google_cloud_automlops.utils.constants import (
+    BASE_DIR,
+    GENERATED_LICENSE,
+    GENERATED_PARAMETER_VALUES_PATH,
+    IAM_ROLES_RUNNER_SA,
+    TERRAFORM_TEMPLATES_PATH
 )
 
 
 @pytest.mark.parametrize(
     'required_apis, use_ci, is_included, expected_output_snippets',
     [
         (
@@ -66,15 +67,21 @@
 
     Args:
         required_apis: List of APIs that are required to run the service.
         use_ci: Flag that determines whether to use Cloud CI/CD.
         is_included: Boolean that determines whether to check if the expected_output_snippets exist in the string or not.
         expected_output_snippets: Strings that are expected to be included (or not) based on the is_included boolean.
     """
-    data_tf_str = create_environment_data_tf_jinja(required_apis, use_ci)
+    data_tf_str = render_jinja(
+        template_path=import_files(TERRAFORM_TEMPLATES_PATH + '.environment') / 'data.tf.j2',
+        generated_license=GENERATED_LICENSE,
+        required_apis=required_apis,
+        required_iam_roles=IAM_ROLES_RUNNER_SA,
+        use_ci=use_ci
+    )
 
     for snippet in expected_output_snippets:
         if is_included:
             assert snippet in data_tf_str
         elif not is_included:
             assert snippet not in data_tf_str
 
@@ -91,15 +98,18 @@
        There is one test case for this function:
         1. Checks for the apache license.
 
     Args:
         is_included: Boolean that determines whether to check if the expected_output_snippets exist in the string or not.
         expected_output_snippets: Strings that are expected to be included (or not) based on the is_included boolean.
     """
-    iam_tf_str = create_environment_iam_tf_jinja()
+    iam_tf_str = render_jinja(
+        template_path=import_files(TERRAFORM_TEMPLATES_PATH + '.environment') / 'iam.tf.j2',
+        generated_license=GENERATED_LICENSE
+    )
 
     for snippet in expected_output_snippets:
         if is_included:
             assert snippet in iam_tf_str
         elif not is_included:
             assert snippet not in iam_tf_str
 
@@ -216,23 +226,28 @@
         schedule_pattern: Cron formatted value used to create a Scheduled retrain job.
         source_repo_type: The type of source repository to use (e.g. gitlab, github, etc.)
         use_ci: Flag that determines whether to use Cloud CI/CD.
         vpc_connector: The name of the vpc connector to use.
         is_included: Boolean that determines whether to check if the expected_output_snippets exist in the string or not.
         expected_output_snippets: Strings that are expected to be included (or not) based on the is_included boolean.
     """
-    main_tf_str = create_environment_main_tf_jinja(
+    main_tf_str = render_jinja(
+        template_path=import_files(TERRAFORM_TEMPLATES_PATH + '.environment') / 'main.tf.j2',
         artifact_repo_type=artifact_repo_type,
+        base_dir=BASE_DIR,
         deployment_framework=deployment_framework,
+        generated_license=GENERATED_LICENSE,
+        generated_parameter_values_path=GENERATED_PARAMETER_VALUES_PATH,
         naming_prefix=naming_prefix,
         pipeline_job_submission_service_type=pipeline_job_submission_service_type,
         schedule_pattern=schedule_pattern,
         source_repo_type=source_repo_type,
         use_ci=use_ci,
-        vpc_connector=vpc_connector)
+        vpc_connector=vpc_connector
+    )
 
     for snippet in expected_output_snippets:
         if is_included:
             assert snippet in main_tf_str
         elif not is_included:
             assert snippet not in main_tf_str
 
@@ -351,21 +366,24 @@
         pipeline_job_submission_service_type: The tool to host for the cloud submission service (e.g. cloud run, cloud functions).
         schedule_pattern: Cron formatted value used to create a Scheduled retrain job.
         source_repo_type: The type of source repository to use (e.g. gitlab, github, etc.)
         use_ci: Flag that determines whether to use Cloud CI/CD.
         is_included: Boolean that determines whether to check if the expected_output_snippets exist in the string or not.
         expected_output_snippets: Strings that are expected to be included (or not) based on the is_included boolean.
     """
-    main_tf_str = create_environment_outputs_tf_jinja(
+    main_tf_str = render_jinja(
+        template_path=import_files(TERRAFORM_TEMPLATES_PATH + '.environment') / 'outputs.tf.j2',
         artifact_repo_type=artifact_repo_type,
         deployment_framework=deployment_framework,
+        generated_license=GENERATED_LICENSE,
         pipeline_job_submission_service_type=pipeline_job_submission_service_type,
         schedule_pattern=schedule_pattern,
         source_repo_type=source_repo_type,
-        use_ci=use_ci)
+        use_ci=use_ci
+    )
 
     for snippet in expected_output_snippets:
         if is_included:
             assert snippet in main_tf_str
         elif not is_included:
             assert snippet not in main_tf_str
 
@@ -382,15 +400,18 @@
        There is one test case for this function:
         1. Checks for the apache license.
 
     Args:
         is_included: Boolean that determines whether to check if the expected_output_snippets exist in the string or not.
         expected_output_snippets: Strings that are expected to be included (or not) based on the is_included boolean.
     """
-    provider_tf_str = create_environment_provider_tf_jinja()
+    provider_tf_str = render_jinja(
+        template_path=import_files(TERRAFORM_TEMPLATES_PATH + '.environment') / 'provider.tf.j2',
+        generated_license=GENERATED_LICENSE
+    )
 
     for snippet in expected_output_snippets:
         if is_included:
             assert snippet in provider_tf_str
         elif not is_included:
             assert snippet not in provider_tf_str
 
@@ -407,15 +428,18 @@
        There is one test case for this function:
         1. Checks for the apache license.
 
     Args:
         is_included: Boolean that determines whether to check if the expected_output_snippets exist in the string or not.
         expected_output_snippets: Strings that are expected to be included (or not) based on the is_included boolean.
     """
-    variables_tf_str = create_environment_variables_tf_jinja()
+    variables_tf_str = render_jinja(
+        template_path=import_files(TERRAFORM_TEMPLATES_PATH + '.environment') / 'variables.tf.j2',
+        generated_license=GENERATED_LICENSE
+    )
 
     for snippet in expected_output_snippets:
         if is_included:
             assert snippet in variables_tf_str
         elif not is_included:
             assert snippet not in variables_tf_str
 
@@ -434,15 +458,19 @@
         1. Checks for the apache license and state file storage_bucket backend.
 
     Args:
         storage_bucket_name: GS bucket name where pipeline run metadata is stored.
         is_included: Boolean that determines whether to check if the expected_output_snippets exist in the string or not.
         expected_output_snippets: Strings that are expected to be included (or not) based on the is_included boolean.
     """
-    versions_tf_str = create_environment_versions_tf_jinja(storage_bucket_name=storage_bucket_name)
+    versions_tf_str = render_jinja(
+        template_path=import_files(TERRAFORM_TEMPLATES_PATH + '.environment') / 'versions.tf.j2',
+        generated_license=GENERATED_LICENSE,
+        storage_bucket_name=storage_bucket_name
+    )
 
     for snippet in expected_output_snippets:
         if is_included:
             assert snippet in versions_tf_str
         elif not is_included:
             assert snippet not in versions_tf_str
 
@@ -459,15 +487,19 @@
        There is one test case for this function:
         1. Checks for the apache license and the Bash shebang.
 
     Args:
         is_included: Boolean that determines whether to check if the expected_output_snippets exist in the string or not.
         expected_output_snippets: Strings that are expected to be included (or not) based on the is_included boolean.
     """
-    provision_resources_script = create_provision_resources_script_jinja()
+    provision_resources_script = render_jinja(
+        template_path=import_files(TERRAFORM_TEMPLATES_PATH) / 'provision_resources.sh.j2',
+        base_dir=BASE_DIR,
+        generated_license=GENERATED_LICENSE
+    )
 
     for snippet in expected_output_snippets:
         if is_included:
             assert snippet in provision_resources_script
         elif not is_included:
             assert snippet not in provision_resources_script
 
@@ -484,15 +516,18 @@
        There is one test case for this function:
         1. Checks for the apache license.
 
     Args:
         is_included: Boolean that determines whether to check if the expected_output_snippets exist in the string or not.
         expected_output_snippets: Strings that are expected to be included (or not) based on the is_included boolean.
     """
-    variables_tf_str = create_state_bucket_variables_tf_jinja()
+    variables_tf_str = render_jinja(
+        template_path=import_files(TERRAFORM_TEMPLATES_PATH + '.state_bucket') / 'variables.tf.j2',
+        generated_license=GENERATED_LICENSE
+    )
 
     for snippet in expected_output_snippets:
         if is_included:
             assert snippet in variables_tf_str
         elif not is_included:
             assert snippet not in variables_tf_str
 
@@ -509,14 +544,17 @@
        There are eight test cases for this function:
         1. Checks for the apache license.
             
     Args:
         is_included: Boolean that determines whether to check if the expected_output_snippets exist in the string or not.
         expected_output_snippets: Strings that are expected to be included (or not) based on the is_included boolean.
     """
-    main_tf_str = create_state_bucket_main_tf_jinja()
+    main_tf_str = render_jinja(
+        template_path=import_files(TERRAFORM_TEMPLATES_PATH + '.state_bucket') / 'main.tf.j2',
+        generated_license=GENERATED_LICENSE
+    )
 
     for snippet in expected_output_snippets:
         if is_included:
             assert snippet in main_tf_str
         elif not is_included:
             assert snippet not in main_tf_str
```

### Comparing `google-cloud-automlops-1.2.9/tests/unit/utils/utils_test.py` & `google_cloud_automlops-1.3.0/tests/unit/utils/utils_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Unit tests for utils module."""
 
 # pylint: disable=line-too-long
 # pylint: disable=missing-function-docstring
+# pylint: disable=unused-import
 
 from contextlib import nullcontext as does_not_raise
 import os
+import tempfile
 from typing import Callable, List
 
-import pandas as pd
 import pytest
 import pytest_mock
 import yaml
 
 import google_cloud_automlops.utils.utils
 from google_cloud_automlops.utils.utils import (
     delete_file,
     execute_process,
-    get_components_list,
     get_function_source_definition,
     is_component_config,
     make_dirs,
     read_file,
     read_yaml_file,
+    render_jinja,
     stringify_job_spec_list,
-    update_params,
     validate_use_ci,
     write_and_chmod,
     write_file,
     write_yaml_file
 )
 
 
@@ -280,63 +280,14 @@
         with open(file=file_to_delete, mode='w', encoding='utf-8') as file:
             file.write('This is a test file.')
             delete_file(file_to_delete)
             assert not os.path.exists(file_to_delete)
 
 
 @pytest.mark.parametrize(
-    'comp_path, comp_name, patch_cwd, expectation',
-    [
-        (['component.yaml'], ['component'], True, does_not_raise()),
-        ([], [], True, does_not_raise()),
-        (['component.yaml'], ['component'], False, pytest.raises(FileNotFoundError))
-    ]
-)
-def test_get_components_list(mocker: pytest_mock.MockerFixture,
-                             comp_path: List[str],
-                             comp_name: List[str],
-                             patch_cwd: bool,
-                             expectation):
-    """Tests get_components_list, which reads yamls in .AutoMLOps-cache directory,
-    verifies they are component yamls, and returns the name of the files. There
-    are three test cases for this function:
-        1. Expected outcome, component list is pulled as expected.
-        2. Verifies an empty list comes back if no YAMLs are present.
-        3. Call function with a nonexistent dir, expecting OSError.
-
-    Args:
-        mocker: Mocker to patch the cache directory for component files.
-        comp_path (List[str]): Path(s) to component yamls.
-        comp_name (List[str]): Name(s) of components.
-        patch_cwd (bool): Boolean flag indicating whether to patch the current working
-            directory from CACHE_DIR to root
-        expectation: Any corresponding expected errors for each set of
-            parameters.
-    """
-    if patch_cwd:
-        mocker.patch.object(google_cloud_automlops.utils.utils, 'CACHE_DIR', '.')
-    if comp_path:
-        for file in comp_path:
-            with open(file=file, mode='w', encoding='utf-8') as f:
-                yaml.dump(
-                    {
-                        'name': 'value1', 
-                        'inputs': 'value2',
-                        'implementation': 'value3'
-                    },
-                    f)
-    with expectation:
-        assert get_components_list(full_path=False) == comp_name
-        assert get_components_list(full_path=True) == [os.path.join('.', file) for file in comp_path]
-    for file in comp_path:
-        if os.path.exists(file):
-            os.remove(file)
-
-
-@pytest.mark.parametrize(
     'yaml_contents, expectation',
     [
         (
             {
                 'name': 'value1',
                 'inputs': 'value2',
                 'implementation': 'value3'
@@ -427,45 +378,14 @@
     with expectation:
         validate_use_ci(schedule_pattern=sch_pattern,
                         setup_model_monitoring=setup_model_monitoring,
                         use_ci=use_ci)
 
 
 @pytest.mark.parametrize(
-    'params, expected_output',
-    [
-        ([{'name': 'param1', 'type': int}], [{'name': 'param1', 'type': 'Integer'}]),
-        ([{'name': 'param2', 'type': str}], [{'name': 'param2', 'type': 'String'}]),
-        ([{'name': 'param3', 'type': float}], [{'name': 'param3', 'type': 'Float'}]),
-        ([{'name': 'param4', 'type': bool}], [{'name': 'param4', 'type': 'Boolean'}]),
-        ([{'name': 'param5', 'type': list}], [{'name': 'param5', 'type': 'JsonArray'}]),
-        ([{'name': 'param6', 'type': dict}], [{'name': 'param6', 'type': 'JsonObject'}]),
-        ([{'name': 'param6', 'type': pd.DataFrame}], None)
-    ]
-)
-def test_update_params(params: List[dict], expected_output: List[dict]):
-    """Tests the update_params function, which reformats the source code type
-    labels as strings. There are seven test cases for this function, which test
-    for updating different parameter types.
-
-    Args:
-        params (List[dict]): Pipeline parameters. A list of dictionaries, each param is a dict containing keys:
-            'name': required, str param name.
-            'type': required, python primitive type.
-            'description': optional, str param desc.
-        expected_output (List[dict]): Expectation of whether or not the configuration is valid.
-    """
-    if expected_output is not None:
-        assert expected_output == update_params(params=params)
-    else:
-        with pytest.raises(ValueError):
-            assert update_params(params=params)
-
-
-@pytest.mark.parametrize(
     'func, expected_output',
     [
         (func1, 'def func1(x):\n    return x + 1\n'),
         (func2, 'def func2(x, y):\n    return x + y\n'),
         (func3, 'def func3(x, y, z):\n    return x + y + z\n'),
         (func4, 'def func4():\n\n    def inner_func():\n        res = 1 + 1\n        return res\n\n    return inner_func()\n')
     ]
@@ -525,7 +445,31 @@
         "machine_type": "a2-highgpu-1g"
     }'''
             }]
     """
 
     formatted_spec = stringify_job_spec_list(job_spec_list=job_spec_list)
     assert formatted_spec == expected_output
+
+
+@pytest.mark.parametrize(
+    'template_string, template_vars, expected_output',
+    [
+        ('Hello {{ name1 }} my name is {{ name2 }}', {'name1': 'Alice', 'name2': 'John'}, 'Hello Alice my name is John'),
+        ('The answer is: {{ result }}', {'result': 42}, 'The answer is: 42'),
+    ]
+)
+def test_render_jinja(template_string, template_vars, expected_output):
+    """Tests the render_jinja function using temporary files."""
+
+    with tempfile.TemporaryDirectory() as tmpdirname:  # Creates temp directory
+        template_path = os.path.join(tmpdirname, 'template.txt.j2')
+
+        # Write the template to the temporary file
+        with open(template_path, 'w', encoding='utf-8') as f:
+            f.write(template_string)
+
+        # Call the render_jinja function
+        result = render_jinja(template_path, **template_vars)
+
+        # Assertion
+        assert result == expected_output
```

