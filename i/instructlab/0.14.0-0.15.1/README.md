# Comparing `tmp/instructlab-0.14.0.tar.gz` & `tmp/instructlab-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructlab-0.14.0.tar", last modified: Sat May  4 10:21:42 2024, max compression
+gzip compressed data, was "instructlab-0.15.1.tar", last modified: Thu May 23 18:28:38 2024, max compression
```

## Comparing `instructlab-0.14.0.tar` & `instructlab-0.15.1.tar`

### file list

```diff
@@ -1,183 +1,195 @@
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.616435 instructlab-0.14.0/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      191 2024-05-03 11:59:35.000000 instructlab-0.14.0/.dockerignore
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.526434 instructlab-0.14.0/.github/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      106 2024-04-17 18:23:40.000000 instructlab-0.14.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)      961 2024-05-04 10:19:54.000000 instructlab-0.14.0/.github/labeler.yml
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1916 2024-05-04 10:21:04.000000 instructlab-0.14.0/.github/mergify.yml
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.528434 instructlab-0.14.0/.github/workflows/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      705 2024-05-04 10:21:04.000000 instructlab-0.14.0/.github/workflows/actionlint.yml
--rw-r--r--   0 heimes    (1000) heimes    (1000)      442 2024-05-04 10:21:04.000000 instructlab-0.14.0/.github/workflows/docs.yml
--rw-r--r--   0 heimes    (1000) heimes    (1000)      335 2024-05-04 10:19:54.000000 instructlab-0.14.0/.github/workflows/label.yml
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2481 2024-05-04 10:21:04.000000 instructlab-0.14.0/.github/workflows/lint.yml
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.528434 instructlab-0.14.0/.github/workflows/matchers/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      624 2024-03-25 13:14:18.000000 instructlab-0.14.0/.github/workflows/matchers/pylint.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1945 2024-05-04 10:21:04.000000 instructlab-0.14.0/.github/workflows/pypi.yaml
--rw-r--r--   0 heimes    (1000) heimes    (1000)      684 2024-05-04 10:21:04.000000 instructlab-0.14.0/.github/workflows/spellcheck.yaml
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1176 2024-05-02 13:55:33.000000 instructlab-0.14.0/.github/workflows/stale_bot.yml
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2378 2024-05-04 10:21:04.000000 instructlab-0.14.0/.github/workflows/test.yml
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2390 2024-04-29 11:29:25.000000 instructlab-0.14.0/.gitignore
--rw-r--r--   0 heimes    (1000) heimes    (1000)      117 2024-05-02 13:55:33.000000 instructlab-0.14.0/.gitmodules
--rw-r--r--   0 heimes    (1000) heimes    (1000)      253 2024-03-07 08:09:54.000000 instructlab-0.14.0/.isort.cfg
--rw-r--r--   0 heimes    (1000) heimes    (1000)      386 2024-05-04 10:19:54.000000 instructlab-0.14.0/.markdownlint-cli2.yaml
--rw-r--r--   0 heimes    (1000) heimes    (1000)      416 2024-04-29 11:29:25.000000 instructlab-0.14.0/.pre-commit-config.yaml
--rw-r--r--   0 heimes    (1000) heimes    (1000)    21523 2024-04-29 11:29:25.000000 instructlab-0.14.0/.pylintrc
--rw-r--r--   0 heimes    (1000) heimes    (1000)      750 2024-05-04 10:19:54.000000 instructlab-0.14.0/.spellcheck-en-custom.txt
--rw-r--r--   0 heimes    (1000) heimes    (1000)      717 2024-05-02 13:55:33.000000 instructlab-0.14.0/.spellcheck.yml
--rw-r--r--   0 heimes    (1000) heimes    (1000)      251 2024-04-29 11:29:25.000000 instructlab-0.14.0/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.529434 instructlab-0.14.0/CONTRIBUTING/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     7841 2024-05-04 10:19:54.000000 instructlab-0.14.0/CONTRIBUTING/CONTRIBUTING.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2516 2024-05-02 13:55:33.000000 instructlab-0.14.0/CONTRIBUTING/FIRST_TIME_CONTRIBUTORS.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)      191 2024-04-29 11:29:25.000000 instructlab-0.14.0/CONTRIBUTOR_ROLES.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)    11359 2024-03-07 08:09:54.000000 instructlab-0.14.0/LICENSE
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.529434 instructlab-0.14.0/MAINTAINERS/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1730 2024-05-04 10:19:54.000000 instructlab-0.14.0/MAINTAINERS/STABLE.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)      168 2024-04-29 11:29:25.000000 instructlab-0.14.0/MAINTAINERS.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4230 2024-05-04 03:17:38.000000 instructlab-0.14.0/Makefile
--rw-r--r--   0 heimes    (1000) heimes    (1000)    25277 2024-05-04 10:21:42.616435 instructlab-0.14.0/PKG-INFO
--rw-r--r--   0 heimes    (1000) heimes    (1000)    23060 2024-05-04 10:19:54.000000 instructlab-0.14.0/README.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1193 2024-05-04 10:19:54.000000 instructlab-0.14.0/SECURITY.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)     7131 2024-04-29 11:29:25.000000 instructlab-0.14.0/TROUBLESHOOTING.md
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.530434 instructlab-0.14.0/containers/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.530434 instructlab-0.14.0/containers/bin/
--rwxr-xr-x   0 heimes    (1000) heimes    (1000)     2240 2024-04-29 11:29:25.000000 instructlab-0.14.0/containers/bin/debug-llama
--rwxr-xr-x   0 heimes    (1000) heimes    (1000)     2079 2024-04-29 11:29:25.000000 instructlab-0.14.0/containers/bin/debug-pytorch
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.531434 instructlab-0.14.0/containers/cuda/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1339 2024-05-04 10:19:54.000000 instructlab-0.14.0/containers/cuda/Containerfile
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.533434 instructlab-0.14.0/containers/rocm/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     5550 2024-04-29 11:29:25.000000 instructlab-0.14.0/containers/rocm/Containerfile
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4309 2024-05-02 13:55:33.000000 instructlab-0.14.0/containers/rocm/README.md
--rwxr-xr-x   0 heimes    (1000) heimes    (1000)      618 2024-04-29 11:29:25.000000 instructlab-0.14.0/containers/rocm/gfx-version.sh
--rwxr-xr-x   0 heimes    (1000) heimes    (1000)     1480 2024-04-29 11:29:25.000000 instructlab-0.14.0/containers/rocm/remove-gfx.sh
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1436 2024-04-29 11:29:25.000000 instructlab-0.14.0/containers/sitecustomize.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.538434 instructlab-0.14.0/docs/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      694 2024-04-17 18:23:40.000000 instructlab-0.14.0/docs/README.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3100 2024-05-04 10:19:44.000000 instructlab-0.14.0/docs/containerization.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2460 2024-04-29 11:29:25.000000 instructlab-0.14.0/docs/converting_GGUF.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3421 2024-05-04 10:19:44.000000 instructlab-0.14.0/docs/demo-slides.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)    13758 2024-05-04 10:19:44.000000 instructlab-0.14.0/docs/gpu-acceleration.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)    90583 2024-04-29 11:29:25.000000 instructlab-0.14.0/docs/workflow.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)     5737 2024-04-29 11:29:25.000000 instructlab-0.14.0/docs/workflow.puml
--rw-r--r--   0 heimes    (1000) heimes    (1000)      215 2024-04-29 11:29:25.000000 instructlab-0.14.0/governance.md
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.539434 instructlab-0.14.0/notebooks/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4436 2024-05-04 10:19:54.000000 instructlab-0.14.0/notebooks/README.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)    32489 2024-04-29 11:29:25.000000 instructlab-0.14.0/notebooks/Training_a_LoRA_With_Instruct_Lab.ipynb
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.545434 instructlab-0.14.0/notebooks/images/
--rw-r--r--   0 heimes    (1000) heimes    (1000)    83152 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/collab-copy-path.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)    89046 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/collab-file-upload-button.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)   165712 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/collab-folder-icon.png
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.561434 instructlab-0.14.0/notebooks/images/kaggle/
--rw-r--r--   0 heimes    (1000) heimes    (1000)   233502 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/kaggle/clear-outputs.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)    58512 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/kaggle/copy-file-path.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)    20354 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/kaggle/create-new-nb.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)     6779 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/kaggle/create.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)    18475 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/kaggle/file-click.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)    23953 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/kaggle/import-nb.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)   170886 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/kaggle/input-drop-files.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)    21422 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/kaggle/input-upload.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)    73216 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/kaggle/input.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)    34311 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/kaggle/new-dataset.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)    27504 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/kaggle/select-accelerator-p100.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)   294162 2024-03-07 08:09:54.000000 instructlab-0.14.0/notebooks/images/kaggle/select-accelerator.png
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2987 2024-05-04 10:19:54.000000 instructlab-0.14.0/pyproject.toml
--rw-r--r--   0 heimes    (1000) heimes    (1000)      181 2024-05-02 07:38:02.000000 instructlab-0.14.0/requirements-dev.txt
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1130 2024-05-04 03:17:38.000000 instructlab-0.14.0/requirements.txt
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.565434 instructlab-0.14.0/scripts/
--rwxr-xr-x   0 heimes    (1000) heimes    (1000)     8230 2024-05-04 10:19:54.000000 instructlab-0.14.0/scripts/functional-tests.sh
--rwxr-xr-x   0 heimes    (1000) heimes    (1000)     1091 2024-04-29 11:29:25.000000 instructlab-0.14.0/scripts/ruff.sh
--rw-r--r--   0 heimes    (1000) heimes    (1000)       38 2024-05-04 10:21:42.617435 instructlab-0.14.0/setup.cfg
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.515433 instructlab-0.14.0/src/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.570434 instructlab-0.14.0/src/instructlab/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/__init__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)      102 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/__main__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)      413 2024-05-04 10:21:42.000000 instructlab-0.14.0/src/instructlab/_version.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.572434 instructlab-0.14.0/src/instructlab/chat/
--rw-r--r--   0 heimes    (1000) heimes    (1000)    18979 2024-05-03 05:06:56.000000 instructlab-0.14.0/src/instructlab/chat/chat.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1095 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/client.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)      269 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/common.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4793 2024-05-04 06:44:12.000000 instructlab-0.14.0/src/instructlab/config.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.576434 instructlab-0.14.0/src/instructlab/generator/
--rw-r--r--   0 heimes    (1000) heimes    (1000)    11625 2024-05-02 13:55:33.000000 instructlab-0.14.0/src/instructlab/generator/README.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/generator/__init__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)    23176 2024-05-04 10:19:54.000000 instructlab-0.14.0/src/instructlab/generator/generate_data.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)   110936 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/generator/seed_tasks.jsonl
--rw-r--r--   0 heimes    (1000) heimes    (1000)     7154 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/generator/utils.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)    38577 2024-05-04 10:21:04.000000 instructlab-0.14.0/src/instructlab/lab.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.579434 instructlab-0.14.0/src/instructlab/llamacpp/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1077 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/llamacpp/LICENSE
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1288 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/llamacpp/README.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/llamacpp/__init__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)    60403 2024-05-04 06:44:12.000000 instructlab-0.14.0/src/instructlab/llamacpp/llamacpp_convert_to_gguf.py
--rwxr-xr-x   0 heimes    (1000) heimes    (1000)  1361544 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/llamacpp/quantize
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.587434 instructlab-0.14.0/src/instructlab/mlx_explore/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1065 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/mlx_explore/LICENSE
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1315 2024-05-02 13:55:33.000000 instructlab-0.14.0/src/instructlab/mlx_explore/README.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/mlx_explore/__init__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)    10556 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/mlx_explore/gguf_convert_to_mlx.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2456 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/mlx_explore/utils.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.516434 instructlab-0.14.0/src/instructlab/schema/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.590434 instructlab-0.14.0/src/instructlab/schema/v1/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1874 2024-05-03 09:59:05.000000 instructlab-0.14.0/src/instructlab/schema/v1/compositional_skills.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3244 2024-05-03 09:59:05.000000 instructlab-0.14.0/src/instructlab/schema/v1/knowledge.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      428 2024-05-03 09:59:05.000000 instructlab-0.14.0/src/instructlab/schema/v1/version.json
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.591435 instructlab-0.14.0/src/instructlab/schema/v2/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1935 2024-05-03 09:59:05.000000 instructlab-0.14.0/src/instructlab/schema/v2/compositional_skills.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3305 2024-05-03 09:59:05.000000 instructlab-0.14.0/src/instructlab/schema/v2/knowledge.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)      390 2024-05-03 09:59:05.000000 instructlab-0.14.0/src/instructlab/schema/v2/version.json
--rw-r--r--   0 heimes    (1000) heimes    (1000)     7971 2024-05-04 10:19:54.000000 instructlab-0.14.0/src/instructlab/server.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.592435 instructlab-0.14.0/src/instructlab/train/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/__init__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     9543 2024-05-04 10:19:54.000000 instructlab-0.14.0/src/instructlab/train/linux_train.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.599434 instructlab-0.14.0/src/instructlab/train/lora_mlx/
--rw-r--r--   0 heimes    (1000) heimes    (1000)       28 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/.gitignore
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1065 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/LICENSE
--rw-r--r--   0 heimes    (1000) heimes    (1000)     8084 2024-05-04 07:10:18.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/README.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/__init__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2290 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/convert.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2910 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/fuse.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)    10329 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/lora.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2882 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/make_data.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.603435 instructlab-0.14.0/src/instructlab/train/lora_mlx/models/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1233 2024-05-02 13:55:33.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/models/README.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/models/__init__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)      357 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/models/base.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     6819 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/models/llama.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2677 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/models/lora.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     8318 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/models/mixtral.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)    11484 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/models/models.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4503 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/models/phi2.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)      874 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/prepare_model.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)       30 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/requirements.txt
--rw-r--r--   0 heimes    (1000) heimes    (1000)     6719 2024-04-29 11:29:25.000000 instructlab-0.14.0/src/instructlab/train/lora_mlx/utils.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)    18101 2024-05-04 10:21:04.000000 instructlab-0.14.0/src/instructlab/utils.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.615435 instructlab-0.14.0/src/instructlab.egg-info/
--rw-r--r--   0 heimes    (1000) heimes    (1000)    25277 2024-05-04 10:21:42.000000 instructlab-0.14.0/src/instructlab.egg-info/PKG-INFO
--rw-r--r--   0 heimes    (1000) heimes    (1000)     4719 2024-05-04 10:21:42.000000 instructlab-0.14.0/src/instructlab.egg-info/SOURCES.txt
--rw-r--r--   0 heimes    (1000) heimes    (1000)        1 2024-05-04 10:21:42.000000 instructlab-0.14.0/src/instructlab.egg-info/dependency_links.txt
--rw-r--r--   0 heimes    (1000) heimes    (1000)       45 2024-05-04 10:21:42.000000 instructlab-0.14.0/src/instructlab.egg-info/entry_points.txt
--rw-r--r--   0 heimes    (1000) heimes    (1000)      684 2024-05-04 10:21:42.000000 instructlab-0.14.0/src/instructlab.egg-info/requires.txt
--rw-r--r--   0 heimes    (1000) heimes    (1000)       12 2024-05-04 10:21:42.000000 instructlab-0.14.0/src/instructlab.egg-info/top_level.txt
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.610435 instructlab-0.14.0/tests/
--rw-r--r--   0 heimes    (1000) heimes    (1000)        0 2024-03-25 13:14:18.000000 instructlab-0.14.0/tests/__init__.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)      749 2024-04-29 11:29:25.000000 instructlab-0.14.0/tests/conftest.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2873 2024-04-29 11:29:25.000000 instructlab-0.14.0/tests/taxonomy.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     5100 2024-04-29 11:29:25.000000 instructlab-0.14.0/tests/test_config.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1112 2024-04-29 11:29:25.000000 instructlab-0.14.0/tests/test_lab.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     8382 2024-04-29 11:29:25.000000 instructlab-0.14.0/tests/test_lab_diff.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1488 2024-04-29 11:29:25.000000 instructlab-0.14.0/tests/test_lab_download.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     9467 2024-05-02 13:55:33.000000 instructlab-0.14.0/tests/test_lab_generate.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3991 2024-04-29 11:29:25.000000 instructlab-0.14.0/tests/test_lab_init.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)    15600 2024-05-04 03:17:38.000000 instructlab-0.14.0/tests/test_lab_train.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)      523 2024-04-29 11:29:25.000000 instructlab-0.14.0/tests/test_notebooks.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1816 2024-05-04 10:19:54.000000 instructlab-0.14.0/tests/test_utils.py
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.613435 instructlab-0.14.0/tests/testdata/
--rw-r--r--   0 heimes    (1000) heimes    (1000)      571 2024-05-02 13:55:33.000000 instructlab-0.14.0/tests/testdata/invalid_yaml.yaml
--rw-r--r--   0 heimes    (1000) heimes    (1000)      545 2024-05-02 13:55:33.000000 instructlab-0.14.0/tests/testdata/knowledge_valid.yaml
--rw-r--r--   0 heimes    (1000) heimes    (1000)      252 2024-05-02 13:55:33.000000 instructlab-0.14.0/tests/testdata/skill_incomplete.yaml
--rw-r--r--   0 heimes    (1000) heimes    (1000)      338 2024-05-02 13:55:33.000000 instructlab-0.14.0/tests/testdata/skill_invalid_answer.yaml
--rw-r--r--   0 heimes    (1000) heimes    (1000)      374 2024-05-02 13:55:33.000000 instructlab-0.14.0/tests/testdata/skill_valid_answer.yaml
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.614435 instructlab-0.14.0/tests/testdata/temp_repo/
-drwxr-xr-x   0 heimes    (1000) heimes    (1000)        0 2024-05-04 10:21:42.615435 instructlab-0.14.0/tests/testdata/temp_repo/docs/
--rw-r--r--   0 heimes    (1000) heimes    (1000)     1302 2024-04-29 11:29:25.000000 instructlab-0.14.0/tests/testdata/temp_repo/docs/skill-wiki.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)      832 2024-04-29 11:29:25.000000 instructlab-0.14.0/tests/testdata/temp_repo/knowledge-wiki.md
--rw-r--r--   0 heimes    (1000) heimes    (1000)     3017 2024-05-04 10:19:54.000000 instructlab-0.14.0/tests/testdata/testdata.py
--rw-r--r--   0 heimes    (1000) heimes    (1000)     2399 2024-05-02 13:55:33.000000 instructlab-0.14.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.923701 instructlab-0.15.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-23 18:28:35.000000 instructlab-0.15.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/actionlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/mergify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/actionlint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/e2e.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/image-cuda.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/lint.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/.github/workflows/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/matchers/pylint.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/spellcheck.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/stale_bot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-23 18:28:35.000000 instructlab-0.15.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-23 18:28:35.000000 instructlab-0.15.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-23 18:28:35.000000 instructlab-0.15.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-23 18:28:35.000000 instructlab-0.15.1/.markdownlint-cli2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-23 18:28:35.000000 instructlab-0.15.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    21523 2024-05-23 18:28:35.000000 instructlab-0.15.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-23 18:28:35.000000 instructlab-0.15.1/.spellcheck-en-custom.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-23 18:28:35.000000 instructlab-0.15.1/.spellcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-23 18:28:35.000000 instructlab-0.15.1/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/CONTRIBUTING/
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-05-23 18:28:35.000000 instructlab-0.15.1/CONTRIBUTING/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-23 18:28:35.000000 instructlab-0.15.1/CONTRIBUTING/FIRST_TIME_CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-23 18:28:35.000000 instructlab-0.15.1/CONTRIBUTOR_ROLES.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-23 18:28:35.000000 instructlab-0.15.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-23 18:28:35.000000 instructlab-0.15.1/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-23 18:28:35.000000 instructlab-0.15.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    30417 2024-05-23 18:28:38.923701 instructlab-0.15.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27980 2024-05-23 18:28:35.000000 instructlab-0.15.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 18:28:35.000000 instructlab-0.15.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-23 18:28:35.000000 instructlab-0.15.1/TROUBLESHOOTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/containers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/containers/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2240 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/bin/debug-llama
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2079 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/bin/debug-pytorch
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/containers/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/cuda/Containerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/containers/hpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/hpu/Containerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.903701 instructlab-0.15.1/containers/rocm/
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/rocm/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/rocm/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      618 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/rocm/gfx-version.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1480 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/rocm/remove-gfx.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/sitecustomize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.903701 instructlab-0.15.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/STABLE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/containerization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/converting_GGUF.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/demo-slides.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14107 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/gpu-acceleration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/habana-gaudi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/release-strategy.md
+-rw-r--r--   0 runner    (1001) docker     (127)    90583 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/workflow.puml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-23 18:28:35.000000 instructlab-0.15.1/governance.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.903701 instructlab-0.15.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32510 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/Training_a_LoRA_With_Instruct_Lab.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.903701 instructlab-0.15.1/notebooks/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    83152 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/collab-copy-path.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89046 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/collab-file-upload-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165712 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/collab-folder-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.907701 instructlab-0.15.1/notebooks/images/kaggle/
+-rw-r--r--   0 runner    (1001) docker     (127)   233502 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/clear-outputs.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58512 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/copy-file-path.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20354 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/create-new-nb.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/create.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18475 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/file-click.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23953 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/import-nb.png
+-rw-r--r--   0 runner    (1001) docker     (127)   170886 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/input-drop-files.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21422 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/input-upload.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73216 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/input.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34311 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/new-dataset.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27504 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/select-accelerator-p100.png
+-rw-r--r--   0 runner    (1001) docker     (127)   294162 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/select-accelerator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-23 18:28:35.000000 instructlab-0.15.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-23 18:28:35.000000 instructlab-0.15.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-23 18:28:35.000000 instructlab-0.15.1/requirements-hpu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-23 18:28:35.000000 instructlab-0.15.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.907701 instructlab-0.15.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5262 2024-05-23 18:28:35.000000 instructlab-0.15.1/scripts/basic-workflow-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11088 2024-05-23 18:28:35.000000 instructlab-0.15.1/scripts/functional-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1091 2024-05-23 18:28:35.000000 instructlab-0.15.1/scripts/ruff.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.907701 instructlab-0.15.1/scripts/test-data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-23 18:28:35.000000 instructlab-0.15.1/scripts/test-data/basic-workflow-fixture-qna.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:28:38.923701 instructlab-0.15.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.891701 instructlab-0.15.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.911702 instructlab-0.15.1/src/instructlab/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.911702 instructlab-0.15.1/src/instructlab/chat/
+-rw-r--r--   0 runner    (1001) docker     (127)    19642 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/chat/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.911702 instructlab-0.15.1/src/instructlab/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/generator/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23232 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/generator/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110936 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/generator/seed_tasks.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/generator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44198 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/lab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.911702 instructlab-0.15.1/src/instructlab/llamacpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/llamacpp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/llamacpp/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/llamacpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60403 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/llamacpp/llamacpp_convert_to_gguf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1361544 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/llamacpp/quantize
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.915701 instructlab-0.15.1/src/instructlab/mlx_explore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/mlx_explore/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/mlx_explore/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/mlx_explore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10556 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/mlx_explore/gguf_convert_to_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/mlx_explore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.891701 instructlab-0.15.1/src/instructlab/schema/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.915701 instructlab-0.15.1/src/instructlab/schema/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/schema/v1/compositional_skills.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/schema/v1/knowledge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/schema/v1/version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.915701 instructlab-0.15.1/src/instructlab/schema/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/schema/v2/compositional_skills.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/schema/v2/knowledge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/schema/v2/version.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.915701 instructlab-0.15.1/src/instructlab/train/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13425 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/linux_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.919701 instructlab-0.15.1/src/instructlab/train/lora_mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/make_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.919701 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/mixtral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/phi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/prepare_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.923701 instructlab-0.15.1/src/instructlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30417 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.919701 instructlab-0.15.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_lab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_lab_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_lab_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_lab_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_lab_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16370 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_lab_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.923701 instructlab-0.15.1/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/invalid_yaml.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/knowledge_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/skill_incomplete.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/skill_invalid_answer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/skill_valid_answer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.923701 instructlab-0.15.1/tests/testdata/temp_repo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.923701 instructlab-0.15.1/tests/testdata/temp_repo/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/temp_repo/docs/skill-wiki.md
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/temp_repo/knowledge-wiki.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/testdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-23 18:28:35.000000 instructlab-0.15.1/tox.ini
```

### Comparing `instructlab-0.14.0/.github/workflows/actionlint.yml` & `instructlab-0.15.1/.github/workflows/actionlint.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # SPDX-License-Identifier: Apache-2.0
 
 name: Lint GitHub Actions workflows
 on:
   push:
     branches:
       - "main"
+      - "release-**"
     paths:
       - '.github/**'
   pull_request:
     branches:
       - "main"
+      - '.github/**'
     paths:
       - '.github/**'
 
 defaults:
   run:
     shell: bash
```

### Comparing `instructlab-0.14.0/.github/workflows/matchers/pylint.json` & `instructlab-0.15.1/.github/workflows/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/.github/workflows/spellcheck.yaml` & `instructlab-0.15.1/.github/workflows/spellcheck.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # SPDX-License-Identifier: Apache-2.0
 
 name: Spellcheck
 
 on:
   pull_request:
-    branches: [main]
+    branches:
+      - main
+      - "release-**"
     paths:
       - '**.md'
       - .github/**
 
 permissions:
   contents: read
```

### Comparing `instructlab-0.14.0/.github/workflows/stale_bot.yml` & `instructlab-0.15.1/.github/workflows/stale_bot.yml`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/.gitignore` & `instructlab-0.15.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -153,7 +153,10 @@
 .tox
 
 # config
 config.yaml
 
 # Spelling
 dictionary.dic
+
+# Man pages
+man
```

### Comparing `instructlab-0.14.0/.pylintrc` & `instructlab-0.15.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/.spellcheck.yml` & `instructlab-0.15.1/.spellcheck.yml`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 - name: markdown
   aspell:
     lang: en
     d: en_US
     camel-case: true
     mode: markdown
   sources:
-  - "**/*.md|!REVIEWERS.md|!build/**|!.tox/**|!src/instructlab/schema/**"
+  - "**/*.md|!REVIEWERS.md|!build/**|!.tox/**|!src/instructlab/schema/**|!venv/**|!taxonomy/**"
   dictionary:
     wordlists:
     - .spellcheck-en-custom.txt
   pipeline:
   - pyspelling.filters.context:
       context_visible_first: true
       escapes: '\\[\\`~]'
```

### Comparing `instructlab-0.14.0/CONTRIBUTING/CONTRIBUTING.md` & `instructlab-0.15.1/CONTRIBUTING/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
 
 The following tools are required:
 
 - [`git`](https://git-scm.com)
 - [`python`](https://www.python.org) (v3.9+)
 - [`pip`](https://pypi.org/project/pip/) (v23.0+)
 - [`expect`](https://core.tcl-lang.org/expect/index) (for functional tests)
+- [`coreutils`](https://www.gnu.org/software/coreutils/) (for functional tests)
+- [`bash`](https://www.gnu.org/software/bash/) (v5+, for functional tests)
 
 You can setup your dev environment using [`tox`](https://tox.wiki/en/latest/), an environment orchestrator which allows for setting up environments for and invoking builds, unit tests, formatting, linting, etc. Install tox with:
 
 ```shell
 pip install -r requirements-dev.txt
 ```
```

### Comparing `instructlab-0.14.0/CONTRIBUTING/FIRST_TIME_CONTRIBUTORS.md` & `instructlab-0.15.1/CONTRIBUTING/FIRST_TIME_CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/LICENSE` & `instructlab-0.15.1/LICENSE`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/MAINTAINERS/STABLE.md` & `instructlab-0.15.1/docs/STABLE.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Moving the stable tag
 =====================
 
-Because we do not have a PyPI package where folks can just install latest, our `README.md` instructions describe installing from the GitHub using a "stable" tag.
+Because we do not have a PyPI package where folks can just install latest, our `README.md` instructions describe installing from the GitHub using a `stable` tag.
 
 To support this, we move the stable tag to the latest release, as needed.
 
-This can be done by:
+This can be done via the following steps:
 
-Get current:
+Assume that the upstream repository (`instructlab/instructlab`) is using the `upstream` Git remote
+
+Get current tags from the upstream:
 
 ```ShellSession
 $ git switch main
-$ git fetch
-$ git pull
+$ git fetch upstream
+$ git pull upstream
 # Just making sure you are up-to-date locally
 $ git tag --list
 $ git show-ref --tags
 ```
 
 Using v0.x.y as the example desired stable version:
 
@@ -43,27 +45,23 @@
 
 Verify the tag SHA hashes look correct:
 
 ```ShellSession
 $ git show-ref --tags
 ```
 
-Push the new tag to remote (origin) with `-f` (force) flag.
-
-I usually test first w/o --force and expect an error if I have everything right.
+You can then push the new tag upstream with `-f` (force) flag - I usually test first without `--force` and expect an error if I have everything right.
 
 ```ShellSession
-$ git push origin stable
+$ git push upstream stable
 ! [rejected]        stable -> stable (already exists)
 error: failed to push some refs to 'https://github.com/instructlab/instructlab.git'
 hint: Updates were rejected because the tag already exists in the remote.
 ```
 
-If you are sure. Push with force.
+If you are sure, push with force to upstream and prepare to live with the consequences of your actions.
 
 ```ShellSession
-git push -f origin stable
+git push -f upstream stable
 ```
 
-Check the Tags on GitHub web.
-
-> PLEASE!  Whenever you move the `stable` tag, give `@Josh Boyer` a heads-up so that Red Hat is using the new tag.
+Finally, check the tags on the GitHub web UI to ensure everything looks correct.
```

### Comparing `instructlab-0.14.0/Makefile` & `instructlab-0.15.1/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 
 CUDA_CONTAINERFILE = $(CURDIR)/containers/cuda/Containerfile
 CUDA_DEPS = \
 	$(CUDA_CONTAINERFILE) \
 	$(COMMON_DEPS) \
 	$(NULL)
 
+HPU_CONTAINERFILE = $(CURDIR)/containers/hpu/Containerfile
+HPU_DEPS = \
+	$(HPU_CONTAINERFILE) \
+	$(CURDIR)/requirements-hpu.txt \
+	$(COMMON_DEPS) \
+	$(NULL)
+
 ROCM_CONTAINERFILE = containers/rocm/Containerfile
 ROCM_DEPS = \
 	$(ROCM_CONTAINERFILE) \
 	$(COMMON_DEPS) \
 	containers/rocm/remove-gfx.sh \
 	$(NULL)
 
@@ -50,14 +57,23 @@
 .PHONY: cuda
 cuda: $(CUDA_DEPS)  ## Build container for NVidia CUDA
 	$(CENGINE) build $(BUILD_ARGS) \
 		-t $(CONTAINER_PREFIX):$@ \
 		-f $(CUDA_CONTAINERFILE) \
 		.
 
+# The base container uses uids beyond 65535. Rootless builds may not work
+# unless the user account has extended subordinate ids up to 2**24 - 1.
+.PHONY: hpu
+hpu: $(HPU_DEPS)  ## Build container for Intel Gaudi HPU
+	$(CENGINE) build $(BUILD_ARGS) \
+		-t $(CONTAINER_PREFIX):$@ \
+		-f $< \
+		.
+
 define build-rocm =
 	@echo "Building ROCm container for GPU arch '$(1)', version '$(2)'"
 	$(CENGINE) build $(BUILD_ARGS) \
 		--build-arg AMDGPU_ARCH=$(1) \
 		--build-arg HSA_OVERRIDE_GFX_VERSION=$(2) \
 		-t $(CONTAINER_PREFIX):rocm-$(1) \
 		-t $(CONTAINER_PREFIX):rocm \
@@ -122,15 +138,22 @@
 
 .PHONY: verify
 verify: ## Run tox -e fmt,lint,spellcheck against code
 	tox p -e ruff,fastlint,spellcheck
 
 .PHONY: spellcheck-sort
 spellcheck-sort: .spellcheck-en-custom.txt
-	sort -d -f -o $< $<
+	sort -d -o $< $<
+
+.PHONY: man
+man:
+	tox -e docs
+
+.PHONY: docs
+docs: man ## Run tox -e docs against code
 
 ##@ Linting
 
 #
 # If you want to see the full commands, run:
 #   NOISY_BUILD=y make
 #
```

### Comparing `instructlab-0.14.0/PKG-INFO` & `instructlab-0.15.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,163 +1,180 @@
-Metadata-Version: 2.1
-Name: instructlab
-Version: 0.14.0
-Summary: CLI for interacting with InstructLab
-Author-email: TBD <jon@example.com>
-License: Apache-2.0 AND MIT
-Project-URL: homepage, https://instructlab.io
-Project-URL: source, https://github.com/instructlab/instructlab
-Project-URL: issues, https://github.com/instructlab/instructlab/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: click<9.0.0,>=8.1.7
-Requires-Dist: click-didyoumean<0.4.0,>=0.3.0
-Requires-Dist: datasets<3.0.0,>=2.18.0
-Requires-Dist: gguf<0.7.0,>=0.6.0
-Requires-Dist: GitPython<4.0.0,>=3.1.42
-Requires-Dist: httpx
-Requires-Dist: jsonschema<5.0.0,>=4.21.1
-Requires-Dist: llama_cpp_python[server]==0.2.55
-Requires-Dist: mlx<0.6.0,>=0.5.1; sys_platform == "darwin" and platform_machine == "arm64"
-Requires-Dist: numpy<2.0.0,>=1.26.4
-Requires-Dist: openai<2.0.0,>=1.13.3
-Requires-Dist: peft<0.10.0,>=0.9.0
-Requires-Dist: prompt-toolkit<4.0.0,>=3.0.38
-Requires-Dist: pydantic
-Requires-Dist: pydantic_yaml
-Requires-Dist: PyYAML<7.0.0,>=6.0.1
-Requires-Dist: rich<14.0.0,>=13.3.1
-Requires-Dist: rouge-score<0.2.0,>=0.1.2
-Requires-Dist: sentencepiece<0.3.0,>=0.2.0
-Requires-Dist: tokenizers<0.16.0,>=0.15.2
-Requires-Dist: toml<0.11.0,>=0.10.2
-Requires-Dist: torch<3.0.0,>=2.2.1
-Requires-Dist: tqdm<5.0.0,>=4.66.2
-Requires-Dist: transformers<=4.38.2,>=4.30.0
-Requires-Dist: trl<0.8.0,>=0.7.11
-Requires-Dist: wandb<0.17.0,>=0.16.4
-Requires-Dist: langchain-text-splitters
-Requires-Dist: yamllint<1.36.0,>=1.35.1
-
 # InstructLab 🐶 (`ilab`)
 
 ![Lint](https://github.com/instructlab/instructlab/actions/workflows/lint.yml/badge.svg?branch=main)
 ![Tests](https://github.com/instructlab/instructlab/actions/workflows/test.yml/badge.svg?branch=main)
 ![Build](https://github.com/instructlab/instructlab/actions/workflows/pypi.yaml/badge.svg?branch=main)
-[![Demo](https://img.shields.io/badge/Demo-v0.13.0-blue)](https://asciinema.org/a/PmRU7IrReep04FY6qpzo2Zclc)
+![Release](https://img.shields.io/github/v/release/instructlab/instructlab)
 ![License](https://img.shields.io/github/license/instructlab/instructlab)
 
 ## 📖 Contents
 
-- [❓What is `ilab`](#-what-is-ilab)
+- [Welcome to the InstructLab CLI](#welcome-to-the-instructlab-cli)
+- [❓ What is `ilab`](#-what-is-ilab)
 - [📋 Requirements](#-requirements)
 - [✅ Getting started](#-getting-started)
-  - [🧰 Installing`ilab`](#-installing-ilab)
-  - [🏗️ Initialize `ilab`](#%EF%B8%8F-initialize-ilab)
+  - [🧰 Installing `ilab`](#-installing-ilab)
+    - [To install with no GPU acceleration and PyTorch without CUDA bindings](#to-install-with-no-gpu-acceleration-and-pytorch-without-cuda-bindings)
+    - [To install with AMD ROCm](#to-install-with-amd-rocm)
+    - [To install with Apple Metal on M1/M2/M3 Mac](#to-install-with-apple-metal-on-m1m2m3-mac)
+    - [To install with Nvidia CUDA](#to-install-with-nvidia-cuda)
+    - [Example output](#example-output)
+    - [Bash (version 4.4 or newer)](#bash-version-44-or-newer)
+    - [Zsh](#zsh)
+    - [Fish](#fish)
+  - [🏗️ Initialize `ilab`](#️-initialize-ilab)
+    - [Example output](#example-output-1)
+    - [Example output](#example-output-2)
   - [📥 Download the model](#-download-the-model)
   - [🍴 Serving the model](#-serving-the-model)
   - [📣 Chat with the model (Optional)](#-chat-with-the-model-optional)
 - [💻 Creating new knowledge or skills and training the model](#-creating-new-knowledge-or-skills-and-training-the-model)
   - [🎁 Contribute knowledge or compositional skills](#-contribute-knowledge-or-compositional-skills)
   - [📜 List and validate your new data](#-list-and-validate-your-new-data)
   - [🚀 Generate a synthetic dataset](#-generate-a-synthetic-dataset)
+    - [Example output](#example-output-3)
   - [👩‍🏫 Train the model](#-train-the-model)
-  - [Test the newly trained model](#-test-the-newly-trained-model)
+    - [Train the model locally on Linux](#train-the-model-locally-on-linux)
+    - [Train the model locally on an M-series Mac](#train-the-model-locally-on-an-m-series-mac)
+    - [Training the model locally with GPU acceleration](#training-the-model-locally-with-gpu-acceleration)
+    - [Training the model in the cloud](#training-the-model-in-the-cloud)
+  - [📜 Test the newly trained model](#-test-the-newly-trained-model)
   - [🍴 Serve the newly trained model](#-serve-the-newly-trained-model)
-  - [📣 Chat with the new model (not optional this time)](#-chat-with-the-new-model-not-optional-this-time)
+- [📣 Chat with the new model (not optional this time)](#-chat-with-the-new-model-not-optional-this-time)
 - [🎁 Submit your new knowledge or skills](#-submit-your-new-knowledge-or-skills)
-- [📬 Contributing to Instruct-Lab CLI](#-contributing)
+- [📬 Contributing](#-contributing)
 
 ## Welcome to the InstructLab CLI
 
 InstructLab 🐶 uses a novel synthetic data-based alignment tuning method for
 Large Language Models (LLMs.) The "**lab**" in Instruct**Lab** 🐶 stands for
 [**L**arge-Scale **A**lignment for Chat**B**ots](https://arxiv.org/abs/2403.01081) [1].
 
 [1] Shivchander Sudalairaj*, Abhishek Bhandwaldar*, Aldo Pareja*, Kai Xu, David D. Cox, Akash Srivastava*. "LAB: Large-Scale Alignment for ChatBots", arXiv preprint arXiv: 2403.01081, 2024. (* denotes equal contributions)
 
 ## ❓ What is `ilab`
 
-`ilab` is a Command-Line Interface (CLI) tool that allows you to:
+`ilab` is a Command-Line Interface (CLI) tool that allows you to perform the following actions:
 
 1. Download a pre-trained Large Language Model (LLM).
 1. Chat with the LLM.
 
-To add new knowledge and skills to the pre-trained LLM you have to add new information to the companion [taxonomy](https://github.com/instructlab/taxonomy.git) repository.
-After that is done, you can:
+To add new knowledge and skills to the pre-trained LLM, add information to the companion [taxonomy](https://github.com/instructlab/taxonomy.git) repository.
+
+After you have added knowledge and skills to the taxonomy, you can perform the following actions:
 
 1. Use `ilab` to generate new synthetic training data based on the changes in your local `taxonomy` repository.
 1. Re-train the LLM with the new training data.
 1. Chat with the re-trained LLM to see the results.
 
-The full process is described graphically in the [workflow diagram](./docs/workflow.png).
+```mermaid
+graph TD;
+  download-->chat
+  chat[Chat with the LLM]-->add
+  add[Add new knowledge\nor skill to taxonomy]-->generate[generate new\nsynthetic training data]
+  generate-->train
+  train[Re-train]-->|Chat with\nthe re-trained LLM\nto see the results|chat
+```
+
+For an overview of the full workflow, see the [workflow diagram](./docs/workflow.png).
 
 > [!IMPORTANT]
-> It is important to understand that running InstructLab on a laptop will give you a low-fidelity approximation of both synthetic data generation (using the `ilab generate` command)
-> and model instruction tuning (using the `ilab train` command, which uses QLoRA.) The quality of the results you get using these tools on a laptop will not be as high-fidelity as they might be using
-> a larger teacher model and a different training method. We have optimized InstructLab to enable community members with modest hardware to be able to use the technique. If you have more sophisticated
-> hardware, you can configure InstructLab to use a larger teacher model [such as Mixtral](https://huggingface.co/docs/transformers/model_doc/mixtral) in order to achieve higher-fidelity results.
+> We have optimized InstructLab so that community members with commodity hardware can perform these steps. However, running InstructLab on a laptop will provide a low-fidelity approximation of synthetic data generation
+> (using the `ilab generate` command) and model instruction tuning (using the `ilab train` command, which uses QLoRA). To achieve higher quality, use more sophisticated hardware and configure InstructLab to use a
+> larger teacher model [such as Mixtral](https://huggingface.co/docs/transformers/model_doc/mixtral).
 
 ## 📋 Requirements
 
 - **🍎 Apple M1/M2/M3 Mac or 🐧 Linux system** (tested on Fedora). We anticipate support for more operating systems in the future.
 - C++ compiler
 - Python 3.9+ (<3.12 for PyTorch JIT)
 - Approximately 60GB disk space (entire process)
 
 > **NOTE:** PyTorch 2.2.1 does not support `torch.compile` with Python 3.12. On Fedora 39+, install `python3.11-devel` and create the virtual env with `python3.11` if you wish to use PyTorch's JIT compiler.
+<!-- -->
+> **NOTE:** When installing the `ilab` CLI on macOS, you may have to run the `xcode select --install` command to install the required packages previously listed.
 
 ## ✅ Getting started
 
 ### 🧰 Installing `ilab`
 
-1. If you are on Fedora Linux, install C++, Python 3.9+, and other necessary tools by running the following command:
+1. When installing on Fedora Linux, install C++, Python 3.9+, and other necessary tools by running the following command:
 
    ```shell
    sudo dnf install g++ gcc make pip python3 python3-devel python3-GitPython
    ```
 
    Optional: If `g++` is not found, try `gcc-c++` by running the following command:
 
-     ```shell
-     sudo dnf install gcc-c++ gcc make pip python3 python3-devel python3-GitPython
-     ```
+   ```shell
+   sudo dnf install gcc-c++ gcc make pip python3 python3-devel python3-GitPython
+   ```
+
+   If you are running on macOS, this installation is not necessary and you can begin your process with the following step.  
 
 2. Create a new directory called `instructlab` to store the files the `ilab` CLI needs when running and `cd` into the directory by running the following command:
 
    ```shell
    mkdir instructlab
    cd instructlab
    ```
 
    > **NOTE:** The following steps in this document use [Python venv](https://docs.python.org/3/library/venv.html) for virtual environments. However, if you use another tool such as [pyenv](https://github.com/pyenv/pyenv) or [Conda Miniforge](https://github.com/conda-forge/miniforge) for managing Python environments on your machine continue to use that tool instead. Otherwise, you may have issues with packages that are installed but not found in `venv`.
 
 3. Install and activate your `venv` environment by running the following command:
 
+   > **NOTE**: ⏳ `pip install` may take some time, depending on your internet connection. In case installation fails with error ``unsupported instruction `vpdpbusd'``, append `-C cmake.args="-DLLAMA_NATIVE=off"` to `pip install` command.
+
+   See [the GPU acceleration documentation](./docs/gpu-acceleration.md) for how to
+   to enable hardware acceleration for inference and training on AMD ROCm,
+   Apple Metal Performance Shaders (MPS), and Nvidia CUDA.
+
+   #### To install with no GPU acceleration and PyTorch without CUDA bindings
+
    ```shell
-   python3 -m venv venv
+   python3 -m venv --upgrade-deps venv
    source venv/bin/activate
-   pip install git+https://github.com/instructlab/instructlab.git@stable
+   (venv) $ pip cache remove llama_cpp_python
+   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable --extra-index-url=https://download.pytorch.org/whl/cpu
    ```
 
-   > **NOTE**: ⏳ `pip install` may take some time, depending on your internet connection.
+   #### To install with AMD ROCm
+
+   ```shell
+   python3 -m venv --upgrade-deps venv
+   source venv/bin/activate
+   (venv) $ pip cache remove llama_cpp_python
+   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable \
+       --extra-index-url https://download.pytorch.org/whl/rocm6.0 \
+       -C cmake.args="-DLLAMA_HIPBLAS=on" \
+       -C cmake.args="-DAMDGPU_TARGETS=all" \
+       -C cmake.args="-DCMAKE_C_COMPILER=/opt/rocm/llvm/bin/clang" \
+       -C cmake.args="-DCMAKE_CXX_COMPILER=/opt/rocm/llvm/bin/clang++" \
+       -C cmake.args="-DCMAKE_PREFIX_PATH=/opt/rocm"
+   ```
+
+   On Fedora 40+, use `-DCMAKE_C_COMPILER=clang-17` and `-DCMAKE_CXX_COMPILER=clang++-17`.
+
+   #### To install with Apple Metal on M1/M2/M3 Mac
+
+   ```shell
+   python3 -m venv --upgrade-deps venv
+   source venv/bin/activate
+   (venv) $ pip cache remove llama_cpp_python
+   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable -C cmake.args="-DLLAMA_METAL=on"
+   ```
+
+   #### To install with Nvidia CUDA
+
+   ```shell
+   python3 -m venv --upgrade-deps venv
+   source venv/bin/activate
+   (venv) $ pip cache remove llama_cpp_python
+   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable -C cmake.args="-DLLAMA_CUBLAS=on"
+   ```
 
 4. From your `venv` environment, verify `ilab` is installed correctly, by running the `ilab` command.
 
    ```shell
    ilab
    ```
 
@@ -192,14 +209,63 @@
 
    > **IMPORTANT:** every `ilab` command needs to be run from within your Python virtual environment. To enter the Python environment, run the following command:
 
    ```shell
    source venv/bin/activate
    ```
 
+5. You may optionally enable tab completion for the `ilab` command.
+
+   #### Bash (version 4.4 or newer)
+
+   Enable tab completion in `bash` with the following command:
+
+   ```sh
+   eval "$(_ILAB_COMPLETE=bash_source ilab)"
+   ```
+
+   To have this enabled automatically every time you open a new shell,
+   you can save the completion script and source it from `~/.bashrc`:
+
+   ```sh
+   _ILAB_COMPLETE=bash_source ilab > ~/.ilab-complete.bash
+   echo ". ~/.ilab-complete.bash" >> ~/.bashrc
+   ```
+
+   #### Zsh
+
+   Enable tab completion in `zsh` with the following command:
+
+   ```sh
+   eval "$(_ILAB_COMPLETE=zsh_source ilab)"
+   ```
+
+   To have this enabled automatically every time you open a new shell,
+   you can save the completion script and source it from `~/.zshrc`:
+
+   ```sh
+   _ILAB_COMPLETE=zsh_source ilab > ~/.ilab-complete.zsh
+   echo ". ~/.ilab-complete.zsh" >> ~/.zshrc
+   ```
+
+   #### Fish
+
+   Enable tab completion in `fish` with the following command:
+
+   ```sh
+   _ILAB_COMPLETE=fish_source ilab | source
+   ```
+
+   To have this enabled automatically every time you open a new shell,
+   you can save the completion script and source it from `~/.bashrc`:
+
+   ```sh
+   _ILAB_COMPLETE=fish_source ilab > ~/.config/fish/completions/ilab.fish
+   ```
+
 ### 🏗️ Initialize `ilab`
 
 1. Initialize `ilab` by running the following command:
 
    ```shell
    ilab init
    ```
@@ -224,15 +290,15 @@
    (venv) $ ilab init
    Welcome to InstructLab CLI. This guide will help you set up your environment.
    Please provide the following values to initiate the environment [press Enter for defaults]:
    Path to taxonomy repo [taxonomy]: <ENTER>
    `taxonomy` seems to not exists or is empty. Should I clone https://github.com/instructlab/taxonomy.git for you? [y/N]: y
    Cloning https://github.com/instructlab/taxonomy.git...
    Generating `config.yaml` in the current directory...
-   Initialization completed successfully, you're ready to start using `lab`. Enjoy!
+   Initialization completed successfully, you're ready to start using `ilab`. Enjoy!
    ```
 
    `ilab` will use the default configuration file unless otherwise specified. You can override this behavior with the `--config` parameter for any `ilab` command.
 
    The taxonomy repository uses [submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules) to incorporate the [taxonomy schema](https://github.com/instructlab/schema.git).
    When the `ilab init` command clones the taxonomy repository, it automatically handles the submodules.
    If you clone the taxonomy repository yourself, be sure to use the [`--recurse-submodules`](https://git-scm.com/docs/git-clone#Documentation/git-clone.txt---recurse-submodulesltpathspecgt) option on the `git clone` command and the `git pull` command when pulling updates from the remote repository.
@@ -308,15 +374,15 @@
 >>>                                                                                                                                                                                                                               [S][default]
 ```
 
 ## 💻 Creating new knowledge or skills and training the model
 
 ### 🎁 Contribute knowledge or compositional skills
 
-Contribute new knowledge or compositional skills to your local [taxonomy](https://github.com/instructlab/taxonomy.git) repository.
+1. Contribute new knowledge or compositional skills to your local [taxonomy](https://github.com/instructlab/taxonomy.git) repository.
 
 Detailed contribution instructions can be found in the [taxonomy repository](https://github.com/instructlab/taxonomy/blob/main/README.md).
 
 > [!IMPORTANT]
 > There is a limit to how much content can exist in the question/answer pairs for the model to process. Due to this, only add a maximum of around 2300 words to your question and answer seed example pairs in the `qna.yaml` file.
 
 ### 📜 List and validate your new data
@@ -333,14 +399,16 @@
    (venv) $ ilab diff
    compositional_skills/writing/freeform/foo-lang/foo-lang.yaml
    Taxonomy in /taxonomy/ is valid :)
    ```
 
 ### 🚀 Generate a synthetic dataset
 
+Before following these instructions, ensure the existing model you are adding skills or knowledge to is still running.
+
 1. To generate a synthetic dataset based on your newly added knowledge or skill set in [taxonomy](https://github.com/instructlab/taxonomy.git) repository, run the following command:
 
    ```shell
    ilab generate
    ```
 
    > **NOTE:** ⏳ This can take from 15 minutes to 1+ hours to complete, depending on your computing resources.
@@ -386,27 +454,23 @@
 
 #### Train the model locally on Linux
 
 ```shell
 ilab train
 ```
 
-> **NOTE:** ⏳ This step can potentially take **several hours** to complete depending on your computing resources.
+> **NOTE:** ⏳ This step can potentially take **several hours** to complete depending on your computing resources. Please stop `ilab chat` and `ilab serve` first to free resources.
 
 `ilab train` outputs a brand-new model that can be served in the `models` directory called `ggml-model-f16.gguf`.
 
 ```shell
  (venv) $ ls models
  ggml-merlinite-7b-lab-Q4_K_M.gguf  ggml-model-f16.gguf
 ```
 
-> **NOTE:** `ilab train` ships with experimental support for GPU acceleration with Nvidia CUDA
-or AMD ROCm. See [the GPU acceleration documentation](./docs/gpu-acceleration.md) for more
-details.
-
 #### Train the model locally on an M-series Mac
 
 To train the model locally on your M-Series Mac is as easy as running:
 
 ```shell
 ilab train
 ```
@@ -420,14 +484,22 @@
 (venv) $ ls instructlab-merlinite-7b-lab-mlx-q
 adapters-010.npz        adapters-050.npz        adapters-090.npz        config.json             tokenizer.model
 adapters-020.npz        adapters-060.npz        adapters-100.npz        model.safetensors       tokenizer_config.json
 adapters-030.npz        adapters-070.npz        adapters.npz            special_tokens_map.json
 adapters-040.npz        adapters-080.npz        added_tokens.json       tokenizer.jso
 ```
 
+#### Training the model locally with GPU acceleration
+
+Training has experimental support for GPU acceleration with Nvidia CUDA or AMD ROCm. Please see [the GPU acceleration documentation](./docs/gpu-acceleration.md) for more details. At present, hardware acceleration requires a data center GPU or high-end consumer GPU with at least 18 GB free memory.
+
+```shell
+ilab train --device=cuda
+```
+
 #### Training the model in the cloud
 
 Follow the instructions in [Training](./notebooks/README.md).
 
 ⏳ Approximate amount of time taken on each platform:
 
 - *Google Colab*: **5-10 minutes** with a T4 GPU
@@ -460,15 +532,15 @@
 
 2. Convert the newly trained model by running the following command:
 
    ```shell
    ilab convert
    ```
 
-3. Serve the newly trained model locally via `ilab serve` command with the `--model`
+3. Serve the newly trained model locally via `ilab serve` command with the `--model-path`
 argument to specify your new model:
 
    ```shell
    ilab serve --model-path <New model name>
    ```
 
    Which model should you select to serve? After running the `ilab convert` command, a few files and directories are generated. The one you will want to serve will end in `.gguf`
```

### Comparing `instructlab-0.14.0/README.md` & `instructlab-0.15.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,236 @@
+Metadata-Version: 2.1
+Name: instructlab
+Version: 0.15.1
+Summary: CLI for interacting with InstructLab
+Author-email: TBD <jon@example.com>
+License: Apache-2.0 AND MIT
+Project-URL: homepage, https://instructlab.io
+Project-URL: source, https://github.com/instructlab/instructlab
+Project-URL: issues, https://github.com/instructlab/instructlab/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click<9.0.0,>=8.1.7
+Requires-Dist: click-didyoumean<0.4.0,>=0.3.0
+Requires-Dist: datasets<3.0.0,>=2.18.0
+Requires-Dist: gguf<0.7.0,>=0.6.0
+Requires-Dist: GitPython<4.0.0,>=3.1.42
+Requires-Dist: httpx<1.0.0,>=0.25.0
+Requires-Dist: jsonschema<5.0.0,>=4.21.1
+Requires-Dist: llama_cpp_python[server]==0.2.75
+Requires-Dist: mlx<0.6.0,>=0.5.1; sys_platform == "darwin" and platform_machine == "arm64"
+Requires-Dist: numpy<2.0.0,>=1.23.5; python_version == "3.10"
+Requires-Dist: numpy<2.0.0,>=1.26.4; python_version != "3.10"
+Requires-Dist: openai<2.0.0,>=1.13.3
+Requires-Dist: peft<0.10.0,>=0.9.0
+Requires-Dist: prompt-toolkit<4.0.0,>=3.0.38
+Requires-Dist: pydantic<3.0.0,>=2.6.0
+Requires-Dist: pydantic_yaml<2.0.0,>=1.2.0
+Requires-Dist: PyYAML<7.0.0,>=6.0.0
+Requires-Dist: rich<14.0.0,>=13.3.1
+Requires-Dist: rouge-score<0.2.0,>=0.1.2
+Requires-Dist: sentencepiece<0.3.0,>=0.2.0
+Requires-Dist: tokenizers<0.16.0,>=0.15.2
+Requires-Dist: toml<0.11.0,>=0.10.2
+Requires-Dist: torch<3.0.0,>=2.2.0a0; python_version == "3.10"
+Requires-Dist: torch<3.0.0,>=2.2.1; python_version != "3.10"
+Requires-Dist: tqdm<5.0.0,>=4.66.2
+Requires-Dist: transformers<=4.38.2,>=4.30.0
+Requires-Dist: trl<0.8.0,>=0.7.11
+Requires-Dist: wandb<0.17.0,>=0.16.4
+Requires-Dist: langchain-text-splitters
+Requires-Dist: yamllint<1.36.0,>=1.35.1
+
 # InstructLab 🐶 (`ilab`)
 
 ![Lint](https://github.com/instructlab/instructlab/actions/workflows/lint.yml/badge.svg?branch=main)
 ![Tests](https://github.com/instructlab/instructlab/actions/workflows/test.yml/badge.svg?branch=main)
 ![Build](https://github.com/instructlab/instructlab/actions/workflows/pypi.yaml/badge.svg?branch=main)
-[![Demo](https://img.shields.io/badge/Demo-v0.13.0-blue)](https://asciinema.org/a/PmRU7IrReep04FY6qpzo2Zclc)
+![Release](https://img.shields.io/github/v/release/instructlab/instructlab)
 ![License](https://img.shields.io/github/license/instructlab/instructlab)
 
 ## 📖 Contents
 
-- [❓What is `ilab`](#-what-is-ilab)
+- [Welcome to the InstructLab CLI](#welcome-to-the-instructlab-cli)
+- [❓ What is `ilab`](#-what-is-ilab)
 - [📋 Requirements](#-requirements)
 - [✅ Getting started](#-getting-started)
-  - [🧰 Installing`ilab`](#-installing-ilab)
-  - [🏗️ Initialize `ilab`](#%EF%B8%8F-initialize-ilab)
+  - [🧰 Installing `ilab`](#-installing-ilab)
+    - [To install with no GPU acceleration and PyTorch without CUDA bindings](#to-install-with-no-gpu-acceleration-and-pytorch-without-cuda-bindings)
+    - [To install with AMD ROCm](#to-install-with-amd-rocm)
+    - [To install with Apple Metal on M1/M2/M3 Mac](#to-install-with-apple-metal-on-m1m2m3-mac)
+    - [To install with Nvidia CUDA](#to-install-with-nvidia-cuda)
+    - [Example output](#example-output)
+    - [Bash (version 4.4 or newer)](#bash-version-44-or-newer)
+    - [Zsh](#zsh)
+    - [Fish](#fish)
+  - [🏗️ Initialize `ilab`](#️-initialize-ilab)
+    - [Example output](#example-output-1)
+    - [Example output](#example-output-2)
   - [📥 Download the model](#-download-the-model)
   - [🍴 Serving the model](#-serving-the-model)
   - [📣 Chat with the model (Optional)](#-chat-with-the-model-optional)
 - [💻 Creating new knowledge or skills and training the model](#-creating-new-knowledge-or-skills-and-training-the-model)
   - [🎁 Contribute knowledge or compositional skills](#-contribute-knowledge-or-compositional-skills)
   - [📜 List and validate your new data](#-list-and-validate-your-new-data)
   - [🚀 Generate a synthetic dataset](#-generate-a-synthetic-dataset)
+    - [Example output](#example-output-3)
   - [👩‍🏫 Train the model](#-train-the-model)
-  - [Test the newly trained model](#-test-the-newly-trained-model)
+    - [Train the model locally on Linux](#train-the-model-locally-on-linux)
+    - [Train the model locally on an M-series Mac](#train-the-model-locally-on-an-m-series-mac)
+    - [Training the model locally with GPU acceleration](#training-the-model-locally-with-gpu-acceleration)
+    - [Training the model in the cloud](#training-the-model-in-the-cloud)
+  - [📜 Test the newly trained model](#-test-the-newly-trained-model)
   - [🍴 Serve the newly trained model](#-serve-the-newly-trained-model)
-  - [📣 Chat with the new model (not optional this time)](#-chat-with-the-new-model-not-optional-this-time)
+- [📣 Chat with the new model (not optional this time)](#-chat-with-the-new-model-not-optional-this-time)
 - [🎁 Submit your new knowledge or skills](#-submit-your-new-knowledge-or-skills)
-- [📬 Contributing to Instruct-Lab CLI](#-contributing)
+- [📬 Contributing](#-contributing)
 
 ## Welcome to the InstructLab CLI
 
 InstructLab 🐶 uses a novel synthetic data-based alignment tuning method for
 Large Language Models (LLMs.) The "**lab**" in Instruct**Lab** 🐶 stands for
 [**L**arge-Scale **A**lignment for Chat**B**ots](https://arxiv.org/abs/2403.01081) [1].
 
 [1] Shivchander Sudalairaj*, Abhishek Bhandwaldar*, Aldo Pareja*, Kai Xu, David D. Cox, Akash Srivastava*. "LAB: Large-Scale Alignment for ChatBots", arXiv preprint arXiv: 2403.01081, 2024. (* denotes equal contributions)
 
 ## ❓ What is `ilab`
 
-`ilab` is a Command-Line Interface (CLI) tool that allows you to:
+`ilab` is a Command-Line Interface (CLI) tool that allows you to perform the following actions:
 
 1. Download a pre-trained Large Language Model (LLM).
 1. Chat with the LLM.
 
-To add new knowledge and skills to the pre-trained LLM you have to add new information to the companion [taxonomy](https://github.com/instructlab/taxonomy.git) repository.
-After that is done, you can:
+To add new knowledge and skills to the pre-trained LLM, add information to the companion [taxonomy](https://github.com/instructlab/taxonomy.git) repository.
+
+After you have added knowledge and skills to the taxonomy, you can perform the following actions:
 
 1. Use `ilab` to generate new synthetic training data based on the changes in your local `taxonomy` repository.
 1. Re-train the LLM with the new training data.
 1. Chat with the re-trained LLM to see the results.
 
-The full process is described graphically in the [workflow diagram](./docs/workflow.png).
+```mermaid
+graph TD;
+  download-->chat
+  chat[Chat with the LLM]-->add
+  add[Add new knowledge\nor skill to taxonomy]-->generate[generate new\nsynthetic training data]
+  generate-->train
+  train[Re-train]-->|Chat with\nthe re-trained LLM\nto see the results|chat
+```
+
+For an overview of the full workflow, see the [workflow diagram](./docs/workflow.png).
 
 > [!IMPORTANT]
-> It is important to understand that running InstructLab on a laptop will give you a low-fidelity approximation of both synthetic data generation (using the `ilab generate` command)
-> and model instruction tuning (using the `ilab train` command, which uses QLoRA.) The quality of the results you get using these tools on a laptop will not be as high-fidelity as they might be using
-> a larger teacher model and a different training method. We have optimized InstructLab to enable community members with modest hardware to be able to use the technique. If you have more sophisticated
-> hardware, you can configure InstructLab to use a larger teacher model [such as Mixtral](https://huggingface.co/docs/transformers/model_doc/mixtral) in order to achieve higher-fidelity results.
+> We have optimized InstructLab so that community members with commodity hardware can perform these steps. However, running InstructLab on a laptop will provide a low-fidelity approximation of synthetic data generation
+> (using the `ilab generate` command) and model instruction tuning (using the `ilab train` command, which uses QLoRA). To achieve higher quality, use more sophisticated hardware and configure InstructLab to use a
+> larger teacher model [such as Mixtral](https://huggingface.co/docs/transformers/model_doc/mixtral).
 
 ## 📋 Requirements
 
 - **🍎 Apple M1/M2/M3 Mac or 🐧 Linux system** (tested on Fedora). We anticipate support for more operating systems in the future.
 - C++ compiler
 - Python 3.9+ (<3.12 for PyTorch JIT)
 - Approximately 60GB disk space (entire process)
 
 > **NOTE:** PyTorch 2.2.1 does not support `torch.compile` with Python 3.12. On Fedora 39+, install `python3.11-devel` and create the virtual env with `python3.11` if you wish to use PyTorch's JIT compiler.
+<!-- -->
+> **NOTE:** When installing the `ilab` CLI on macOS, you may have to run the `xcode select --install` command to install the required packages previously listed.
 
 ## ✅ Getting started
 
 ### 🧰 Installing `ilab`
 
-1. If you are on Fedora Linux, install C++, Python 3.9+, and other necessary tools by running the following command:
+1. When installing on Fedora Linux, install C++, Python 3.9+, and other necessary tools by running the following command:
 
    ```shell
    sudo dnf install g++ gcc make pip python3 python3-devel python3-GitPython
    ```
 
    Optional: If `g++` is not found, try `gcc-c++` by running the following command:
 
-     ```shell
-     sudo dnf install gcc-c++ gcc make pip python3 python3-devel python3-GitPython
-     ```
+   ```shell
+   sudo dnf install gcc-c++ gcc make pip python3 python3-devel python3-GitPython
+   ```
+
+   If you are running on macOS, this installation is not necessary and you can begin your process with the following step.  
 
 2. Create a new directory called `instructlab` to store the files the `ilab` CLI needs when running and `cd` into the directory by running the following command:
 
    ```shell
    mkdir instructlab
    cd instructlab
    ```
 
    > **NOTE:** The following steps in this document use [Python venv](https://docs.python.org/3/library/venv.html) for virtual environments. However, if you use another tool such as [pyenv](https://github.com/pyenv/pyenv) or [Conda Miniforge](https://github.com/conda-forge/miniforge) for managing Python environments on your machine continue to use that tool instead. Otherwise, you may have issues with packages that are installed but not found in `venv`.
 
 3. Install and activate your `venv` environment by running the following command:
 
+   > **NOTE**: ⏳ `pip install` may take some time, depending on your internet connection. In case installation fails with error ``unsupported instruction `vpdpbusd'``, append `-C cmake.args="-DLLAMA_NATIVE=off"` to `pip install` command.
+
+   See [the GPU acceleration documentation](./docs/gpu-acceleration.md) for how to
+   to enable hardware acceleration for inference and training on AMD ROCm,
+   Apple Metal Performance Shaders (MPS), and Nvidia CUDA.
+
+   #### To install with no GPU acceleration and PyTorch without CUDA bindings
+
    ```shell
-   python3 -m venv venv
+   python3 -m venv --upgrade-deps venv
    source venv/bin/activate
-   pip install git+https://github.com/instructlab/instructlab.git@stable
+   (venv) $ pip cache remove llama_cpp_python
+   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable --extra-index-url=https://download.pytorch.org/whl/cpu
    ```
 
-   > **NOTE**: ⏳ `pip install` may take some time, depending on your internet connection.
+   #### To install with AMD ROCm
+
+   ```shell
+   python3 -m venv --upgrade-deps venv
+   source venv/bin/activate
+   (venv) $ pip cache remove llama_cpp_python
+   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable \
+       --extra-index-url https://download.pytorch.org/whl/rocm6.0 \
+       -C cmake.args="-DLLAMA_HIPBLAS=on" \
+       -C cmake.args="-DAMDGPU_TARGETS=all" \
+       -C cmake.args="-DCMAKE_C_COMPILER=/opt/rocm/llvm/bin/clang" \
+       -C cmake.args="-DCMAKE_CXX_COMPILER=/opt/rocm/llvm/bin/clang++" \
+       -C cmake.args="-DCMAKE_PREFIX_PATH=/opt/rocm"
+   ```
+
+   On Fedora 40+, use `-DCMAKE_C_COMPILER=clang-17` and `-DCMAKE_CXX_COMPILER=clang++-17`.
+
+   #### To install with Apple Metal on M1/M2/M3 Mac
+
+   ```shell
+   python3 -m venv --upgrade-deps venv
+   source venv/bin/activate
+   (venv) $ pip cache remove llama_cpp_python
+   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable -C cmake.args="-DLLAMA_METAL=on"
+   ```
+
+   #### To install with Nvidia CUDA
+
+   ```shell
+   python3 -m venv --upgrade-deps venv
+   source venv/bin/activate
+   (venv) $ pip cache remove llama_cpp_python
+   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable -C cmake.args="-DLLAMA_CUBLAS=on"
+   ```
 
 4. From your `venv` environment, verify `ilab` is installed correctly, by running the `ilab` command.
 
    ```shell
    ilab
    ```
 
@@ -138,14 +265,63 @@
 
    > **IMPORTANT:** every `ilab` command needs to be run from within your Python virtual environment. To enter the Python environment, run the following command:
 
    ```shell
    source venv/bin/activate
    ```
 
+5. You may optionally enable tab completion for the `ilab` command.
+
+   #### Bash (version 4.4 or newer)
+
+   Enable tab completion in `bash` with the following command:
+
+   ```sh
+   eval "$(_ILAB_COMPLETE=bash_source ilab)"
+   ```
+
+   To have this enabled automatically every time you open a new shell,
+   you can save the completion script and source it from `~/.bashrc`:
+
+   ```sh
+   _ILAB_COMPLETE=bash_source ilab > ~/.ilab-complete.bash
+   echo ". ~/.ilab-complete.bash" >> ~/.bashrc
+   ```
+
+   #### Zsh
+
+   Enable tab completion in `zsh` with the following command:
+
+   ```sh
+   eval "$(_ILAB_COMPLETE=zsh_source ilab)"
+   ```
+
+   To have this enabled automatically every time you open a new shell,
+   you can save the completion script and source it from `~/.zshrc`:
+
+   ```sh
+   _ILAB_COMPLETE=zsh_source ilab > ~/.ilab-complete.zsh
+   echo ". ~/.ilab-complete.zsh" >> ~/.zshrc
+   ```
+
+   #### Fish
+
+   Enable tab completion in `fish` with the following command:
+
+   ```sh
+   _ILAB_COMPLETE=fish_source ilab | source
+   ```
+
+   To have this enabled automatically every time you open a new shell,
+   you can save the completion script and source it from `~/.bashrc`:
+
+   ```sh
+   _ILAB_COMPLETE=fish_source ilab > ~/.config/fish/completions/ilab.fish
+   ```
+
 ### 🏗️ Initialize `ilab`
 
 1. Initialize `ilab` by running the following command:
 
    ```shell
    ilab init
    ```
@@ -170,15 +346,15 @@
    (venv) $ ilab init
    Welcome to InstructLab CLI. This guide will help you set up your environment.
    Please provide the following values to initiate the environment [press Enter for defaults]:
    Path to taxonomy repo [taxonomy]: <ENTER>
    `taxonomy` seems to not exists or is empty. Should I clone https://github.com/instructlab/taxonomy.git for you? [y/N]: y
    Cloning https://github.com/instructlab/taxonomy.git...
    Generating `config.yaml` in the current directory...
-   Initialization completed successfully, you're ready to start using `lab`. Enjoy!
+   Initialization completed successfully, you're ready to start using `ilab`. Enjoy!
    ```
 
    `ilab` will use the default configuration file unless otherwise specified. You can override this behavior with the `--config` parameter for any `ilab` command.
 
    The taxonomy repository uses [submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules) to incorporate the [taxonomy schema](https://github.com/instructlab/schema.git).
    When the `ilab init` command clones the taxonomy repository, it automatically handles the submodules.
    If you clone the taxonomy repository yourself, be sure to use the [`--recurse-submodules`](https://git-scm.com/docs/git-clone#Documentation/git-clone.txt---recurse-submodulesltpathspecgt) option on the `git clone` command and the `git pull` command when pulling updates from the remote repository.
@@ -254,15 +430,15 @@
 >>>                                                                                                                                                                                                                               [S][default]
 ```
 
 ## 💻 Creating new knowledge or skills and training the model
 
 ### 🎁 Contribute knowledge or compositional skills
 
-Contribute new knowledge or compositional skills to your local [taxonomy](https://github.com/instructlab/taxonomy.git) repository.
+1. Contribute new knowledge or compositional skills to your local [taxonomy](https://github.com/instructlab/taxonomy.git) repository.
 
 Detailed contribution instructions can be found in the [taxonomy repository](https://github.com/instructlab/taxonomy/blob/main/README.md).
 
 > [!IMPORTANT]
 > There is a limit to how much content can exist in the question/answer pairs for the model to process. Due to this, only add a maximum of around 2300 words to your question and answer seed example pairs in the `qna.yaml` file.
 
 ### 📜 List and validate your new data
@@ -279,14 +455,16 @@
    (venv) $ ilab diff
    compositional_skills/writing/freeform/foo-lang/foo-lang.yaml
    Taxonomy in /taxonomy/ is valid :)
    ```
 
 ### 🚀 Generate a synthetic dataset
 
+Before following these instructions, ensure the existing model you are adding skills or knowledge to is still running.
+
 1. To generate a synthetic dataset based on your newly added knowledge or skill set in [taxonomy](https://github.com/instructlab/taxonomy.git) repository, run the following command:
 
    ```shell
    ilab generate
    ```
 
    > **NOTE:** ⏳ This can take from 15 minutes to 1+ hours to complete, depending on your computing resources.
@@ -332,27 +510,23 @@
 
 #### Train the model locally on Linux
 
 ```shell
 ilab train
 ```
 
-> **NOTE:** ⏳ This step can potentially take **several hours** to complete depending on your computing resources.
+> **NOTE:** ⏳ This step can potentially take **several hours** to complete depending on your computing resources. Please stop `ilab chat` and `ilab serve` first to free resources.
 
 `ilab train` outputs a brand-new model that can be served in the `models` directory called `ggml-model-f16.gguf`.
 
 ```shell
  (venv) $ ls models
  ggml-merlinite-7b-lab-Q4_K_M.gguf  ggml-model-f16.gguf
 ```
 
-> **NOTE:** `ilab train` ships with experimental support for GPU acceleration with Nvidia CUDA
-or AMD ROCm. See [the GPU acceleration documentation](./docs/gpu-acceleration.md) for more
-details.
-
 #### Train the model locally on an M-series Mac
 
 To train the model locally on your M-Series Mac is as easy as running:
 
 ```shell
 ilab train
 ```
@@ -366,14 +540,22 @@
 (venv) $ ls instructlab-merlinite-7b-lab-mlx-q
 adapters-010.npz        adapters-050.npz        adapters-090.npz        config.json             tokenizer.model
 adapters-020.npz        adapters-060.npz        adapters-100.npz        model.safetensors       tokenizer_config.json
 adapters-030.npz        adapters-070.npz        adapters.npz            special_tokens_map.json
 adapters-040.npz        adapters-080.npz        added_tokens.json       tokenizer.jso
 ```
 
+#### Training the model locally with GPU acceleration
+
+Training has experimental support for GPU acceleration with Nvidia CUDA or AMD ROCm. Please see [the GPU acceleration documentation](./docs/gpu-acceleration.md) for more details. At present, hardware acceleration requires a data center GPU or high-end consumer GPU with at least 18 GB free memory.
+
+```shell
+ilab train --device=cuda
+```
+
 #### Training the model in the cloud
 
 Follow the instructions in [Training](./notebooks/README.md).
 
 ⏳ Approximate amount of time taken on each platform:
 
 - *Google Colab*: **5-10 minutes** with a T4 GPU
@@ -406,15 +588,15 @@
 
 2. Convert the newly trained model by running the following command:
 
    ```shell
    ilab convert
    ```
 
-3. Serve the newly trained model locally via `ilab serve` command with the `--model`
+3. Serve the newly trained model locally via `ilab serve` command with the `--model-path`
 argument to specify your new model:
 
    ```shell
    ilab serve --model-path <New model name>
    ```
 
    Which model should you select to serve? After running the `ilab convert` command, a few files and directories are generated. The one you will want to serve will end in `.gguf`
```

### Comparing `instructlab-0.14.0/TROUBLESHOOTING.md` & `instructlab-0.15.1/TROUBLESHOOTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 1. Increase the number of instructions generated by passing the `--num-instructions` flag to the `ilab generate` command as follows: `ilab generate --num-instructions 1000`.
    The `--num-instructions` flag will generate 1000 points of synthetic data based on your provided examples. The greater the number of instructions generated, the better the model will be trained (within reasonable limits).
 
 2. Adjust the rouge threshold via `--rouge-threshold` parameter. Rogue threshold is a parameter that determines how likely a synthetic data point, generated by the model, will be added to the output based on how similar it is to previously generated data points.
     The value of rouge threshold ranges from 1.0 to 0.0, where 1.0 indicates maximum leniency (every newly generated data point is accepted) and 0.0 indicates maximum strictness (every newly generated data point is rejected). Setting a rouge threshold value closer to 0.0 would force the model to generate data that is different from what it has already generated, leading to a more diverse dataset overall. Rouge threshold can be set as follows: `ilab generate --rouge-threshold 0.75`
 
-3. Using a better model via `--model-dir`. Larger models can lead to better data generation. This option requires users to be familiar with various existing models, and which specific models would suit their needs. This could mean either using a model with more nodes than the default InstructLab `merlinite-7b-lab` model, such as the `Mixtral-8x7B-Instruct-v0.1` model, or using an unquantized version of the InstructLab `merlinite-7b-lab` model. It can be used as follows: `ilab generate --model mixtral0-88x7B-INstruct-v0.1`
+3. Using a better model via `--model`. Larger models can lead to better data generation. This option requires users to be familiar with various existing models, and which specific models would suit their needs. This could mean either using a model with more nodes than the default InstructLab `merlinite-7b-lab` model, such as the `Mixtral-8x7B-Instruct-v0.1` model, or using an unquantized version of the InstructLab `merlinite-7b-lab` model. It can be used as follows: `ilab generate --model Mixtral-8x7B-Instruct-v0.1`
 
 4. Set the number of CPU cores that can be used to generate data via `--num-cpus`. This defaults to 10, but increasing this value could potentially lead to better generated data. It can be used as follows: `ilab generate --num-cpus 15`
 
 ### Training
 
 The training step is run with the `ilab train` command. This step trains the model on the synthetic data that was generated. The output of this step is a set of adapter files with the general format `adapters-xxx.npz`, where `xxx` is a number. These adapter files represent a snapshot of the model's trained state and are periodically written to disk.
```

### Comparing `instructlab-0.14.0/containers/bin/debug-llama` & `instructlab-0.15.1/containers/bin/debug-llama`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/containers/bin/debug-pytorch` & `instructlab-0.15.1/containers/bin/debug-pytorch`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/containers/cuda/Containerfile` & `instructlab-0.15.1/containers/cuda/Containerfile`

 * *Files 12% similar despite different names*

```diff
@@ -10,11 +10,13 @@
 RUN dnf install -y libcudnn8 nvidia-driver-NVML nvidia-driver-cuda-libs
 RUN python3.11 -m pip install --force-reinstall nvidia-cuda-nvcc-cu12
 RUN export LD_LIBRARY_PATH="$LD_LIBRARY_PATH:/usr/local/cuda/lib64:/usr/local/cuda/extras/CUPTI/lib64" \
     && export CUDA_HOME=/usr/local/cuda \
     && export PATH="/usr/local/cuda/bin:$PATH" \
     && export XLA_TARGET=cuda120 \
     && export XLA_FLAGS=--xla_gpu_cuda_data_dir=/usr/local/cuda
-RUN CMAKE_ARGS="-DLLAMA_CUBLAS=on" python3.11 -m pip install -r https://raw.githubusercontent.com/instructlab/instructlab/stable/requirements.txt --force-reinstall --no-cache-dir llama-cpp-python
-RUN python3.11 -m pip install git+https://github.com/instructlab/instructlab.git@stable
-CMD ["/bin/bash"]
 
+ARG GIT_TAG=stable
+RUN CMAKE_ARGS="-DLLAMA_CUBLAS=on" CFLAGS="-mno-avx" python3.11 -m pip install -r https://raw.githubusercontent.com/instructlab/instructlab/${GIT_TAG}/requirements.txt --force-reinstall --no-cache-dir llama-cpp-python
+RUN python3.11 -m pip install git+https://github.com/instructlab/instructlab.git@${GIT_TAG}
+
+CMD ["/bin/bash"]
```

### Comparing `instructlab-0.14.0/containers/rocm/Containerfile` & `instructlab-0.15.1/containers/rocm/Containerfile`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/containers/rocm/README.md` & `instructlab-0.15.1/containers/rocm/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/containers/rocm/gfx-version.sh` & `instructlab-0.15.1/containers/rocm/gfx-version.sh`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/containers/rocm/remove-gfx.sh` & `instructlab-0.15.1/containers/rocm/remove-gfx.sh`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/containers/sitecustomize.py` & `instructlab-0.15.1/containers/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/docs/README.md` & `instructlab-0.15.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/docs/converting_GGUF.md` & `instructlab-0.15.1/docs/converting_GGUF.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/docs/demo-slides.md` & `instructlab-0.15.1/docs/demo-slides.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 source venv/bin/activate.fish
 ```
 
 <!-- pause -->
 Install CLI
 
 ```fish
-pip install git+https://github.com/instructlab/cli.git@v0.13.0
+pip install git+https://github.com/instructlab/cli.git@stable
 ```
 
 <!-- pause -->
 Initialize workspace
 
 ```fish
 ilab init
```

### Comparing `instructlab-0.14.0/docs/gpu-acceleration.md` & `instructlab-0.15.1/docs/gpu-acceleration.md`

 * *Files 12% similar despite different names*

```diff
@@ -31,21 +31,44 @@
 
   # Create and activate new Python 3.11 venv
   python3.11 -m venv venv
   source venv/bin/activate
 
   # Install lab (assumes a locally-cloned repo)
   # You can clone the repo if you haven't already done so (either one)
-  # gh repo clone instructlab/instructlab
-  # git clone https://github.com/instructlab/instructlab.git
-  pip3 install ./instructlab/
+  # gh repo clone instructlab/instructlab -- --recurse-submodules
+  # git clone --recurse-submodules https://github.com/instructlab/instructlab.git
+  pip install ./instructlab/
   ```
 
 With Python 3.11 installed, it's time to replace some packages!
 
+### llama-cpp-python backends
+
+Go to the project's GitHub to see
+the [supported backends](https://github.com/abetlen/llama-cpp-python?tab=readme-ov-file#supported-backends).
+
+Whichever backend you choose, you'll see a `pip install` command. First
+you have to purge pip's wheel cache to force a rebuild of llama-cpp-python:
+
+ ```shell
+ pip cache remove llama_cpp_python
+ ```
+
+You'll want to add a few options to ensure it gets installed over the
+existing package, has the desired backend, and the correct version.
+
+```shell
+pip install --force-reinstall llama_cpp_python==0.2.55 -C cmake.args="-DLLAMA_$BACKEND=on"
+```
+
+where `$BACKEND` is one of `HIPBLAS` (ROCm), `CUBLAS` (CUDA), `METAL`
+(Apple Silicon MPS), `CLBLAST` (OpenCL), or another backend listed in
+llama-cpp-python's documentation.
+
 ### Nvidia/CUDA
 
 `torch` should already ship with CUDA support, so you only have to replace
 `llama-cpp-python`.
 
 Ensure you have the latest proprietary Nvidia drivers installed.  You can
 easily validate whether you are using `nouveau` or `nvidia` kernel drivers with
@@ -85,30 +108,31 @@
 
 sudo dnf clean all
 sudo dnf -y install cuda-toolkit-12-4 nvtop
 ```
 
 Go to the project's GitHub to see the
 [supported backends](https://github.com/abetlen/llama-cpp-python?tab=readme-ov-file#supported-backends).
-Find the `cuBLAS (CUDA)` backend. You'll see a `pip3 install` command.
+Find the `cuBLAS (CUDA)` backend. You'll see a `pip install` command.
 You'll want to add a few options to ensure it gets installed over the
-existing package: `--force-reinstall` and `--no-cache-dir`. Your final
+existing package: `--force-reinstall`. Your final
 command should look like this:
 
 ```shell
 # Veryify CUDA can be found in your PATH variable
 export CUDA_HOME=/usr/local/cuda
 export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/cuda/lib64:/usr/local/cuda/extras/CUPTI/lib64
 export PATH=$PATH:$CUDA_HOME/bin
 
 # Recompile llama-cpp-python using CUDA
-CMAKE_ARGS="-DLLAMA_CUBLAS=on" pip3 install --force-reinstall --no-cache-dir llama-cpp-python
+pip cache remove llama_cpp_python
+pip install --force-reinstall llama_cpp_python==0.2.55 -C cmake.args="-DLLAMA_CUBLAS=on"
 
 # Re-install InstructLab
-pip3 install instructlab/.
+pip install instructlab/.
 ```
 
 Proceed to the `Initialize` section of
 the [CLI README](https://github.com/instructlab/instructlab?tab=readme-ov-file#%EF%B8%8F-initialize-lab),
 and use the `nvtop` utility to validate GPU utilization when interacting
 with `ilab chat` or `ilab generate`
 
@@ -132,40 +156,29 @@
 `torch` does not yet ship with AMD ROCm support, so you'll need to install a version compiled with support.
 
 Visit [PyTorch "Get Started Locally" page](https://pytorch.org/get-started/locally/)
 and use the matrix installer tool to find the ROCm package. `Stable, Linux, Pip,
 Python, ROCm 5.7` in the matrix installer spits out the following command:
 
 ```shell
-pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/rocm5.7
+pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/rocm6.0
 ```
 
 You don't need `torchvision` or `torchaudio`, so get rid of those. You also want
 to make _very_ sure you're installing the right package, and not the old one
 that doesn't have GPU support, so you should add these options:
 `--force-reinstall` and `--no-cache-dir`. Your command should look like below.
 Run it to install the new version of `torch`.
 
 ```shell
-pip3 install torch --force-reinstall --no-cache-dir --index-url https://download.pytorch.org/whl/rocm5.7
+pip install torch --force-reinstall --no-cache-dir --index-url https://download.pytorch.org/whl/rocm6.0
 ```
 
 With that done, it's time to move on to `llama-cpp-python`.
 
-Go to the project's GitHub to see
-the [supported backends](https://github.com/abetlen/llama-cpp-python?tab=readme-ov-file#supported-backends).
-There are several possible backends that may work on AMD; `CLBlast (OpenCL)`
-and `hipBLAS (ROCm)` have been tested to work. It may be worth installing others
-to see if they work for you, but your mileage may vary. Instructions for the
-tested backends are included below!
-
-Whichever backend you choose, you'll see a `pip3 install` command. You'll want
-to add a few options to ensure it gets installed over the existing package:
-`--force-reinstall` and `--no-cache-dir`.
-
 #### hipBLAS
 
 If using hipBLAS you may need to install additional ROCm and hipBLAS
 Dependencies:
 
 ```shell
 # Optionally enable repo.radeon.com repository, available through AMD documentation or Radeon Software for Linux for RHEL 9.3 at https://www.amd.com/en/support/linux-drivers
@@ -194,25 +207,27 @@
       Name:                    amdgcn-amd-amdhsa--gfx103
 ```
 
 In this case, `gfx1100` is the model we're looking for (our dedicated GPU) so
 we'll include that in our build command as follows:
 
 ```shell
-CMAKE_ARGS="-DLLAMA_HIPBLAS=on -DCMAKE_C_COMPILER=/opt/rocm/llvm/bin/clang -DCMAKE_CXX_COMPILER=/opt/rocm/llvm/bin/clang++ -DCMAKE_PREFIX_PATH=/opt/rocm -DAMDGPU_TARGETS=gfx1100" FORCE_CMAKE=1 pip install llama-cpp-python --force-reinstall --no-cache-dir
+export PATH=/opt/rocm/llvm/bin:$PATH
+pip cache remove llama_cpp_python
+CMAKE_ARGS="-DLLAMA_HIPBLAS=on -DCMAKE_C_COMPILER='/opt/rocm/llvm/bin/clang' -DCMAKE_CXX_COMPILER=/opt/rocm/llvm/bin/clang++ -DCMAKE_PREFIX_PATH=/opt/rocm -DAMDGPU_TARGETS=gfx1100" FORCE_CMAKE=1 pip install --force-reinstall llama_cpp_python==0.2.55
 ```
 
 > **Note:** This is explicitly forcing the build to use the ROCm compilers and
 > prefix path for dependency resolution in the CMake build.  This works around
 > an issue in the CMake and ROCm version in Fedora 39 and below and is fixed in
 > Fedora 40.  With Fedora 40's ROCm packages, use
 > `CMAKE_ARGS="-DLLAMA_HIPBLAS=on -DCMAKE_C_COMPILER=/usr/bin/clang
 > -DCMAKE_CXX_COMPILER=/usr/bin/clang++ -DAMDGPU_TARGETS=gfx1100"` instead.
 
-Once that package is installed, recompile `ilab` with `pip3 install .`.  You also
+Once that package is installed, recompile `ilab` with `pip install .`.  You also
 need to tell `HIP` which GPU to use - you can find this out via `rocminfo`
 although it is typically GPU 0.  To set which device is visible to HIP, we'll
 set `export HIP_VISIBLE_DEVICES=0` for GPU 0.   You may also have to set
 `HSA_OVERRIDE_GFX_VERSION` to override ROCm GFX version detection, for example
 `export HSA_OVERRIDE_GFX_VERSION=10.3.0` to force an unsupported `gfx1032` card
 to use use supported `gfx1030` version.  The environment variable
 `AMD_LOG_LEVEL` enables debug logging of ROCm libraries, for example
@@ -221,37 +236,39 @@
 Now you can skip to the `Testing` section.
 
 #### CLBlast (OpenCL)
 
 Your final command should look like so (this uses `CLBlast`):
 
 ```shell
-CMAKE_ARGS="-DLLAMA_CLBLAST=on" pip3 install --force-reinstall --no-cache-dir llama-cpp-python
+pip cache remove llama_cpp_python
+pip install --force-reinstall llama_cpp_python==0.2.55 -C cmake.args="-DLLAMA_CLBLAST=on"
 ```
 
-Once that package is installed, recompile `ilab` with `pip3 install .` and skip
+Once that package is installed, recompile `ilab` with `pip install .` and skip
 to the `Testing` section.
 
 ### Metal/Apple Silicon
 
 The `ilab` default installation should have Metal support by default. If that
 isn't the case, these steps might help to enable it.
 
 `torch` should already ship with Metal support, so you only have to
 replace `llama-cpp-python`. Go to the project's GitHub to see the
 [supported backends](https://github.com/abetlen/llama-cpp-python?tab=readme-ov-file#supported-backends).
-Find the `Metal` backend. You'll see a `pip3 install` command. You'll want to
+Find the `Metal` backend. You'll see a `pip install` command. You'll want to
 add a few options to ensure it gets installed over the existing package:
 `--force-reinstall` and `--no-cache-dir`. Your final command should look like so:
 
 ```shell
-CMAKE_ARGS="-DLLAMA_METAL=on" pip3 install --force-reinstall --no-cache-dir llama-cpp-python
+pip cache remove llama_cpp_python
+pip install --force-reinstall llama_cpp_python==0.2.55 -C cmake.args="-DLLAMA_METAL=on"
 ```
 
-Once that package is installed, recompile `ilab` with `pip3 install .` and skip
+Once that package is installed, recompile `ilab` with `pip install .` and skip
 to the `Testing` section.
 
 ### Testing
 
 Test your changes by chatting to the LLM. Run `ilab serve` and `ilab chat` and
 chat to the LLM. If you notice significantly faster inference, congratulations!
 You've enabled GPU acceleration. You should also notice that the `ilab generate`
```

### Comparing `instructlab-0.14.0/docs/workflow.png` & `instructlab-0.15.1/docs/workflow.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/docs/workflow.puml` & `instructlab-0.15.1/docs/workflow.puml`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/README.md` & `instructlab-0.15.1/notebooks/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -22,26 +22,25 @@
 ### Google Colab
 
 Pre-requisites:
 
 * [Google Colab](https://research.google.com/colaboratory/faq.html)
 * A Gmail account that you're logged into. This will allow you to use Google Colab, which in the free tier will give you access to an NVidia T4 x 15GB GPU.
 
-**NOTE: At present, you'll need to download the notebook and upload it to Google Colab. To upload a notebook go to [Google Colab](https://colab.research.google.com) and you will be prompted to upload a notebook. Once this repository is open sourced, we will make an 'Open in Colab' button.**
-
 ## Running the notebook
 
 [The notebook](./Training_a_LoRA_With_Instruct_Lab.ipynb) in this folder will walk you through:
 
+1. [Open the notebook in Google Colab](https://colab.research.google.com/github/instructlab/instructlab/blob/main/notebooks/Training_a_LoRA_With_Instruct_Lab.ipynb)
 1. Uploading the output of `ilab generate` (a synthetic dataset created based on your hand written prompts/responses).
 1. Checking the base model before training
 1. Setting up and training a LoRA. A LoRA uses Parameter Efficient Fine-tuning (PEFT) methods to fine-tune a model on a small subset of the overall parameters, allowing you to conduct fine-tuning in a fraction of the time, on a fraction of the hardware required. The resultant model should be updated and better handle your queries than the base model.
 1. Inspecting the output model to make sure the LoRA training had the desired effect (i.e. the output has improved).
 
-Once you have finished training and the output looks good, we encourage you go to stage, [Testing the fine-tuned model](../README.md#👩🏽‍🔬-3-testing-the-fine-tuned-model)
+Once you have finished training and the output looks good, we encourage you go to stage, [Testing the fine-tuned model](../README.md#-test-the-newly-trained-model)
 
 ### Kaggle (Unsupported and deprecated)
 
 Using a [Kaggle Notebook](https://github.com/instructlab/instructlab/blob/main/notebooks/Training_a_LoRA_With_Instruct_Lab.ipynb)
 and the NVIDIA P100 provided in the free tier, we will fine tune a LoRA.
 
 #### Pre-requisites
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `instructlab-0.14.0/notebooks/Training_a_LoRA_With_Instruct_Lab.ipynb` & `instructlab-0.15.1/notebooks/Training_a_LoRA_With_Instruct_Lab.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998898237179488%*

 * *Differences: {"'cells'": "{22: {'source': {insert: [(2, 'Recall the [paper on "*

 * *            "LoRA](https://arxiv.org/abs/2106.09685):\\n')], delete: [2]}}, 37: {'source': "*

 * *            '{insert: [(2, "Now that you have trained your LoRA, you must decide, does it look '*

 * *            'good? If yes, please [open a '*

 * *            "PR](https://github.com/instructlab/taxonomy/blob/main/CONTRIBUTING.md), if not that's "*

 * *            'OK, update your prompts, generate a new synthetic data set and try again.\\n")], '*

 * *            'd […]*

```diff
@@ -455,15 +455,15 @@
             "cell_type": "markdown",
             "metadata": {
                 "id": "_IE988CoeLGE"
             },
             "source": [
                 "## Configuring the LoRA\n",
                 "\n",
-                "Recall the paper on LoRA, which is the gospel https://arxiv.org/abs/2106.09685\n",
+                "Recall the [paper on LoRA](https://arxiv.org/abs/2106.09685):\n",
                 "\n",
                 "> From this point forth, we shall be leaving the firm foundation of fact and journeying together through the murky marshes of memory into thickets of wildest guesswork.\n",
                 "-- Albus Dumbledore\n",
                 "\n",
                 "There are 4 common 'knobs' to adjust when training a LoRA/qLoRA - note from this point on, I'm just going to refer to everything as LoRA- a LoRA proved a better method of finetuning, by just targeting certain modules, instead of the entire network. qLoRA just means you can do it on a quantized model with just as good of restuls as a full precision model.\n",
                 "\n",
                 "Which is a good segway to our first 'knob': `target_modules`.\n",
@@ -744,15 +744,15 @@
             "cell_type": "markdown",
             "metadata": {
                 "id": "gt6OfXHD1_tO"
             },
             "source": [
                 "# Next Steps\n",
                 "\n",
-                "Now that you have trained your LoRA, you must decide, does it look good? If yes, please open a PR **TODO: Link to Contrib docs**, if not that's OK, update your prompts, generate a new synthetic data set and try again.\n",
+                "Now that you have trained your LoRA, you must decide, does it look good? If yes, please [open a PR](https://github.com/instructlab/taxonomy/blob/main/CONTRIBUTING.md), if not that's OK, update your prompts, generate a new synthetic data set and try again.\n",
                 "\n",
                 "But the fun doesn't stop there.\n",
                 "\n",
                 "Maybe you want to play with your trained model a bit more.\n",
                 "\n",
                 "Two options exist:\n",
                 "\n",
```

### Comparing `instructlab-0.14.0/notebooks/images/collab-copy-path.png` & `instructlab-0.15.1/notebooks/images/collab-copy-path.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/collab-file-upload-button.png` & `instructlab-0.15.1/notebooks/images/collab-file-upload-button.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/collab-folder-icon.png` & `instructlab-0.15.1/notebooks/images/collab-folder-icon.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/kaggle/clear-outputs.png` & `instructlab-0.15.1/notebooks/images/kaggle/clear-outputs.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/kaggle/copy-file-path.png` & `instructlab-0.15.1/notebooks/images/kaggle/copy-file-path.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/kaggle/create-new-nb.png` & `instructlab-0.15.1/notebooks/images/kaggle/create-new-nb.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/kaggle/create.png` & `instructlab-0.15.1/notebooks/images/kaggle/create.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/kaggle/file-click.png` & `instructlab-0.15.1/notebooks/images/kaggle/file-click.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/kaggle/import-nb.png` & `instructlab-0.15.1/notebooks/images/kaggle/import-nb.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/kaggle/input-drop-files.png` & `instructlab-0.15.1/notebooks/images/kaggle/input-drop-files.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/kaggle/input-upload.png` & `instructlab-0.15.1/notebooks/images/kaggle/input-upload.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/kaggle/input.png` & `instructlab-0.15.1/notebooks/images/kaggle/input.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/kaggle/new-dataset.png` & `instructlab-0.15.1/notebooks/images/kaggle/new-dataset.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/kaggle/select-accelerator-p100.png` & `instructlab-0.15.1/notebooks/images/kaggle/select-accelerator-p100.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/notebooks/images/kaggle/select-accelerator.png` & `instructlab-0.15.1/notebooks/images/kaggle/select-accelerator.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/pyproject.toml` & `instructlab-0.15.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,27 +24,29 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
-dynamic = ["dependencies", "version"]
+dynamic = ["dependencies", "optional-dependencies", "version"]
 
 [project.scripts]
 # defines ilab executable
 ilab = "instructlab.lab:cli"
 
 [project.urls]
 homepage = "https://instructlab.io"
 source = "https://github.com/instructlab/instructlab"
 issues = "https://github.com/instructlab/instructlab/issues"
 
 [tool.setuptools_scm]
 version_file = "src/instructlab/_version.py"
+# do not include +gREV local version, required for Test PyPI upload
+local_scheme = "no-local-version"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
@@ -79,20 +81,25 @@
     # "E",  # pycodestyle
     # "F",  # Pyflakes
     "Q",  # flake8-quotes
     # Ruff does not support isort's import_headings feature, yet.
     # "I",  # isort
     # "UP",  # pyupgrade
     # "SIM",  # flake8-simplify
+    "TID",  # flake8-tidy-imports
 ]
 ignore = [
     # some embedded strings are longer than 88 characters
     "E501",  # line too long
+    "TID252",  # Prefer absolute imports over relative imports from parent modules
 ]
 
+[tool.ruff.lint.flake8-tidy-imports.banned-api]
+"yamllint".msg = "yamllint is for CLI usage only."
+
 [tool.ruff.lint.isort]
 # same as .isort.cfg
 from-first = true
 # not supported yet
 # import-heading-future=Future
 # import-heading-stdlib=Standard
 # import-heading-thirdparty=Third Party
```

### Comparing `instructlab-0.14.0/requirements.txt` & `instructlab-0.15.1/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -4,33 +4,37 @@
 click-didyoumean>=0.3.0,<0.4.0
 datasets>=2.18.0,<3.0.0
 gguf>=0.6.0,<0.7.0
 GitPython>=3.1.42,<4.0.0
 # Linux: 4-bit quantization with BitsAndBytes is not ready to use, yet.
 # see https://github.com/instructlab/instructlab/issues/579
 # bitsandbytes; sys_platform=='linux' and platform_machine=='x86_64'
-httpx
+httpx>=0.25.0,<1.0.0
 jsonschema>=4.21.1,<5.0.0
-# pin version, lift restriction after testing >=0.2.58
-# see https://github.com/abetlen/llama-cpp-python/issues/1286
-llama_cpp_python[server]==0.2.55
+llama_cpp_python[server]==0.2.75
 mlx>=0.5.1,<0.6.0; sys_platform == 'darwin' and platform_machine == 'arm64'
-numpy>=1.26.4,<2.0.0
+# HabanaLabs / Intel Gaudi env comes with Python 3.10 and slightly older
+# versions of some dependencies. Use '3.10' as an indicator.
+# Habana installer has NumPy 1.23.5
+numpy>=1.23.5,<2.0.0 ; python_version == '3.10'
+numpy>=1.26.4,<2.0.0 ; python_version != '3.10'
 openai>=1.13.3,<2.0.0
 peft>=0.9.0,<0.10.0
 prompt-toolkit>=3.0.38,<4.0.0
-pydantic
-pydantic_yaml
-PyYAML>=6.0.1,<7.0.0
+pydantic>=2.6.0,<3.0.0
+pydantic_yaml>=1.2.0,<2.0.0
+PyYAML>=6.0.0,<7.0.0
 rich>=13.3.1,<14.0.0
 rouge-score>=0.1.2,<0.2.0
 sentencepiece>=0.2.0,<0.3.0
 tokenizers>=0.15.2,<0.16.0
 toml>=0.10.2,<0.11.0
-torch>=2.2.1,<3.0.0
+# Habana installer has 2.2.0a0+git8964477 with oneMKL
+torch>=2.2.0a0,<3.0.0 ; python_version == '3.10'
+torch>=2.2.1,<3.0.0 ; python_version != '3.10'
 tqdm>=4.66.2,<5.0.0
 transformers>=4.30.0,<=4.38.2
 trl>=0.7.11,<0.8.0
 wandb>=0.16.4,<0.17.0
 langchain-text-splitters
 # the below library should NOT be imported into any python files
 # it is for CLI usage ONLY
```

### Comparing `instructlab-0.14.0/scripts/functional-tests.sh` & `instructlab-0.15.1/scripts/functional-tests.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,83 @@
 #!/usr/bin/env bash
 # SPDX-License-Identifier: Apache-2.0
 
 set -ex
 
 # build a prompt string that includes the time, source file, line number, and function name
-export PS4='+$(printf "%(%Y-%m-%d %T)T") ${BASH_SOURCE}:${LINENO}: ${FUNCNAME[0]:+${FUNCNAME[0]}(): }'
+export PS4='+$(date +"%Y-%m-%d %T") ${BASH_VERSION}:${BASH_SOURCE}:${LINENO}: ${FUNCNAME[0]:+${FUNCNAME[0]}(): }'
 
 pip install .
 
 export TEST_CTX_SIZE_LAB_SERVE_LOG_FILE=test_ctx_size_lab_serve.log
 export TEST_CTX_SIZE_LAB_CHAT_LOG_FILE=test_ctx_size_lab_chat.log
 
-for cmd in ilab expect; do
+for cmd in ilab expect timeout; do
     if ! type -p $cmd; then
         echo "Error: $cmd is not installed"
         exit 1
     fi
 done
 
 PID_SERVE=
 PID_CHAT=
 
+chat_shot="ilab chat -qq"
+
 cleanup() {
     set +e
     if [ "${1:-0}" -ne 0 ]; then
         echo "Error occurred in function: ${FUNCNAME[1]} with exit code: $1"
     fi
     for pid in $PID_SERVE $PID_CHAT; do
         if [ -n "$pid" ]; then
-            kill $pid
+            kill "$pid"
+            wait "$pid"
         fi
     done
     rm -f "$TEST_CTX_SIZE_LAB_SERVE_LOG_FILE" \
         "$TEST_CTX_SIZE_LAB_CHAT_LOG_FILE" \
         test_session_history
     rm -rf test_taxonomy
-    # revert log level change from test_temp_server()
-    sed -i 's/DEBUG/INFO/g' config.yaml
     # revert port change from test_bind_port()
-    sed -i 's/9999/8000/g' config.yaml
+    sed -i.bak 's/9999/8000/g' config.yaml
+    rm -f config.yaml.bak
+    # revert model name change from test_model_print()
+    sed -i.bak "s/baz/merlinite-7b-lab-Q4_K_M/g" config.yaml
+    mv models/foo.gguf models/merlinite-7b-lab-Q4_K_M.gguf
     set -e
 }
 
 trap 'cleanup "$?"' EXIT QUIT INT TERM
 
 rm -f config.yaml
 
 # print version
 ilab --version
 
 # pipe 3 carriage returns to ilab init to get past the prompts
 echo -e "\n\n\n" | ilab init
 
 # Enable Debug in func tests
-sed -i -e 's/log_level:.*/log_level: DEBUG/g;' config.yaml
+sed -i.bak -e 's/log_level:.*/log_level: DEBUG/g;' config.yaml
+
+# It looks like GitHub action MacOS runner does not have graphics
+# so we need to disable the GPU layers if we are running in GitHub actions
+if [[ "$(uname)" == "Darwin" ]]; then
+    if command -v system_profiler; then
+        if system_profiler SPDisplaysDataType|grep "Metal Support"; then
+            echo "Metal GPU detected"
+        else
+            echo "No Metal GPU detected"
+            sed -i.bak -e 's/gpu_layers: -1/gpu_layers: 0/g;' config.yaml
+        fi
+    else
+        echo "system_profiler not found, cannot determine GPU"
+    fi
+fi
 
 # download the latest version of the ilab
 ilab download
 
 # check that ilab serve is working
 test_bind_port(){
     expect -c '
@@ -73,67 +93,67 @@
     spawn ilab serve
     expect {
         "error while attempting to bind on address " { puts OK }
         default { exit 1 }
     }
 
     # configure a different port
-    exec sed -i 's/8000/9999/g' config.yaml
+    exec sed -i.bak 's/8000/9999/g' config.yaml
 
     # check that ilab serve is working on the new port
     # catch ERROR strings in the output
     spawn ilab serve
     expect {
         "http://127.0.0.1:9999/docs" { puts OK }
         default { exit 1 }
     }
 '
 }
 
 test_ctx_size(){
     # A context size of 55 will allow a small message
-    ilab serve --max-ctx-size 55 &> "$TEST_CTX_SIZE_LAB_SERVE_LOG_FILE" &
+    ilab serve --max-ctx-size 25 &> "$TEST_CTX_SIZE_LAB_SERVE_LOG_FILE" &
     PID_SERVE=$!
 
     # Make sure the server has time to open the port
     # if "ilab chat" tests it before its open then it will run its own server without --max-ctx-size 1
-    sleep 5
+    wait_for_server
 
-    # Should succeed
-    ilab chat -qq "Hello"
+    # SHOULD SUCCEED: ilab chat will trim the SYS_PROMPT then take the second message
+    ${chat_shot} "Hello"
 
-    # the error is expected so let's ignore it to not fall into the trap
-    set +e
-    # now chat with the server and exceed the context size
-    ilab chat &> "$TEST_CTX_SIZE_LAB_CHAT_LOG_FILE" <<EOF &
-hello, I am a ci message that should not finish because I am too long for the context window, tell me about your day please, I love to hear all about it, tell me about the time you could only take 55 tokens
-EOF
+    # SHOULD FAIL: ilab chat will trim the SYS_PROMPT AND the second message, then raise an error
+    # The errors from failures will be written into the serve log and chat log files
+    ${chat_shot} "hello, I am a ci message that should not finish because I am too long for the context window, tell me about your day please?
+    How many tokens could you take today. Could you tell me about the time you could only take twenty five tokens" &> "$TEST_CTX_SIZE_LAB_CHAT_LOG_FILE" &
     PID_CHAT=$!
-    wait_for_pid_to_disappear $PID_CHAT
-    # reset the PID_CHAT variable so that the cleanup function doesn't try to kill it
-    PID_CHAT=
-
-    # re-activate the error trap
-    set -e
 
     # look for the context size error in the server logs
-    timeout 10 bash -c '
+    if ! timeout 20 bash -c '
         until grep -q "exceed context window of" "$TEST_CTX_SIZE_LAB_SERVE_LOG_FILE"; do
         echo "waiting for context size error"
         sleep 1
     done
-'
+'; then
+        echo "context size error not found in server logs"
+        cat $TEST_CTX_SIZE_LAB_SERVE_LOG_FILE
+        exit 1
+    fi
 
     # look for the context size error in the chat logs
-    timeout 10 bash -c '
+    if ! timeout 20 bash -c '
         until grep -q "Message too large for context size." "$TEST_CTX_SIZE_LAB_CHAT_LOG_FILE"; do
         echo "waiting for chat error"
         sleep 1
     done
-'
+'; then
+        echo "context size error not found in chat logs"
+        cat $TEST_CTX_SIZE_LAB_CHAT_LOG_FILE
+        exit 1
+    fi
 }
 
 test_server_shutdown_while_chatting(){
     # we don't want to fall into the trap function since the failure is expected
     # so we force the command to return 0
     timeout 10 ilab serve || true &
 
@@ -148,28 +168,14 @@
         expect {
             "Connection to the server was closed" { exit 0 }
             timeout { exit 1 }
         }
     '
 }
 
-wait_for_pid_to_disappear(){
-    for i in $(seq 1 20); do
-        if ! test -d /proc/$1; then
-            break
-        fi
-        # error if the process is still running
-        if [ $i -eq 20 ]; then
-            echo "chat process is still running"
-            exit 1
-        fi
-        sleep 1
-    done
-}
-
 test_loading_session_history(){
     ilab serve --max-ctx-size 128 &
     PID_SERVE=$!
 
     # chat with the server
     expect -c '
         set timeout 120
@@ -216,31 +222,28 @@
   - question: what is 2+5
     answer: it is 7
   - question: what is 7+3
     answer: it is 10
 task_description: "simple maths"
 EOF
 
-    sed -i -e 's/num_instructions:.*/num_instructions: 1/g' config.yaml
+    sed -i.bak -e 's/num_instructions:.*/num_instructions: 1/g' config.yaml
 
     # This should be finished in a minut or so but time it out incase it goes wrong
     timeout 10m ilab generate --taxonomy-path test_taxonomy/compositional_skills/simple_math.yaml
 
     # Test if generated was created and contains files
     ls -l generated/*
     if [ $(cat $(ls -tr generated/generated_* | tail -n 1) | jq ". | length" ) -lt 1 ] ; then
         echo "Not enough generated results"
         exit 1
     fi
 }
 
 test_temp_server(){
-    nc -l 8000 --keep-open &
-    PID_SERVE=$!
-    sed -i 's/INFO/DEBUG/g' config.yaml
     expect -c '
         set timeout 120
         spawn ilab chat
         expect {
             "Starting a temporary server at" { exit 0 }
             timeout { exit 1 }
         }
@@ -290,14 +293,89 @@
             "Disconnected from client (via refresh/close)" { exit 1 }
         }
         send "exit\r"
         expect eof
     '
 }
 
+test_server_welcome_message(){
+    # test that the server welcome message is displayed
+    ilab serve &
+    PID_SERVE=$!
+
+    wait_for_server
+}
+
+wait_for_server(){
+    if ! timeout 30 bash -c '
+        until curl 127.0.0.1:8000|grep "{\"message\":\"Hello from InstructLab! Visit us at https://instructlab.ai\"}"; do
+            echo "waiting for server to start"
+            sleep 1
+        done
+    '; then
+        echo "server did not start"
+        exit 1
+    fi
+}
+
+test_model_print(){
+    mv models/merlinite-7b-lab-Q4_K_M.gguf models/foo.gguf
+    ilab serve --model-path models/foo.gguf &
+    PID_SERVE=$!
+
+    wait_for_server
+
+    # validate that we print the model from the server since it is different from the config
+    expect -c '
+        spawn ilab chat
+        expect {
+            -re "Welcome to InstructLab Chat w/ \\\u001b\\\[1mMODELS/FOO\\.GGUF" { exit 0 }
+            eof { catch wait result; exit [lindex $result 3] }
+            timeout { exit 1 }
+        }
+    '
+
+    # validate that we print the model from the CLI
+    expect -c '
+        set timeout 30
+        spawn ilab chat -m bar
+        expect {
+            -re "Welcome to InstructLab Chat w/ \\\u001b\\\[1mBAR\\\u001b\\\[0m" { exit 0 }
+            eof { catch wait result; exit [lindex $result 3] }
+            timeout { exit 1 }
+        }
+    '
+
+    # validate that we print the model from the config
+    expect -c '
+        exec sed -i.bak "s/merlinite-7b-lab-Q4_K_M/baz/g" config.yaml
+        spawn ilab chat
+        expect {
+            -re "Welcome to InstructLab Chat w/ \\\u001b\\\[1mBAZ\\\u001b\\\[0m" {
+                exec sed -i.bak "s/baz/merlinite-7b-lab-Q4_K_M/g" config.yaml
+                exit 0
+            }
+            eof { catch wait result; exit [lindex $result 3] }
+            timeout { exit 1 }
+        }
+    '
+
+    # If we don't specify a model, validate that we print the model reported
+    # by the server since it is different from the config.
+    expect -c '
+        spawn ilab chat
+        expect {
+            -re "Welcome to InstructLab Chat w/ \\\u001b\\\[1mMODELS/FOO\\.GGUF" { exit 0 }
+            eof { catch wait result; exit [lindex $result 3] }
+            timeout { exit 1 }
+        }
+    '
+
+}
+
 ########
 # MAIN #
 ########
 # call cleanup in-between each test so they can run without conflicting with the server/chat process
 test_bind_port
 cleanup
 test_ctx_size
@@ -310,9 +388,13 @@
 test_temp_server
 cleanup
 test_temp_server_sigint
 cleanup
 test_no_chat_logs
 cleanup
 test_temp_server_ignore_internal_messages
+cleanup
+test_server_welcome_message
+cleanup
+test_model_print
 
 exit 0
```

### Comparing `instructlab-0.14.0/scripts/ruff.sh` & `instructlab-0.15.1/scripts/ruff.sh`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/chat/chat.py` & `instructlab-0.15.1/src/instructlab/chat/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,34 +55,40 @@
 PROMPT_PREFIX = ">>> "
 
 
 class ChatException(Exception):
     """An exception raised during chat step."""
 
 
+class ChatQuitException(Exception):
+    """A quit command was executed during chat."""
+
+
 # TODO Autosave chat history
 class ConsoleChatBot:  # pylint: disable=too-many-instance-attributes
     def __init__(
         self,
         model,
         client,
         vi_mode=False,
         prompt=True,
         vertical_overflow="ellipsis",
         loaded={},
         log_file=None,
         greedy_mode=False,
+        max_tokens=None,
     ):
         self.client = client
         self.model = model
         self.vi_mode = vi_mode
         self.vertical_overflow = vertical_overflow
         self.loaded = loaded
         self.log_file = log_file
         self.greedy_mode = greedy_mode
+        self.max_tokens = max_tokens
 
         self.console = Console()
 
         self.input = None
         if prompt:
             os.makedirs(os.path.dirname(PROMPT_HISTORY_FILEPATH), exist_ok=True)
             self.input = PromptSession(history=FileHistory(PROMPT_HISTORY_FILEPATH))
@@ -135,15 +141,15 @@
                 ),  # loaded context/session file
                 # TODO: Fix openai package to fix the openai error.
                 # *([] if openai.proxy is None else [('#d08770 bold', "[proxied]")]), # indicate prox
             ]
         )
 
     def _handle_quit(self, content):
-        raise EOFError
+        raise ChatQuitException
 
     def _handle_help(self, content):
         self._sys_print(Markdown(HELP_MD))
         raise KeyboardInterrupt
 
     def _handle_multiline(self, content):
         temp = content == "/m"  # soft multiline only for next prompt
@@ -301,15 +307,15 @@
         raise KeyboardInterrupt
 
     def _update_conversation(self, content, role):
         assert role in ("user", "assistant")
         message = {"role": role, "content": content}
         self.info["messages"].append(message)
 
-    def start_prompt(self, content=None, box=True, logger=None):
+    def start_prompt(self, logger, content=None, box=True):
         handlers = {
             "/q": self._handle_quit,
             "quit": self._handle_quit,
             "exit": self._handle_quit,
             "/h": self._handle_help,
             "/a": self._handle_amend,
             "/c": self._handle_context,
@@ -351,41 +357,48 @@
 
         # Optional parameters
         create_params = {}
         if self.greedy_mode:
             # https://platform.openai.com/docs/api-reference/chat/create#chat-create-temperature
             create_params["temperature"] = 0
 
+        if self.max_tokens:
+            create_params["max_tokens"] = self.max_tokens
+
         # Get and parse response
         try:
             while True:
                 # Loop to catch situations where we need to retry, such as context length exceeded
                 try:
                     response = self.client.chat.completions.create(
                         model=self.model,
                         messages=self.info["messages"],
                         stream=True,
                         **create_params,
                     )
                 except openai.BadRequestError as e:
+                    logger.debug(f"BadRequestError: {e}")
                     if e.code == "context_length_exceeded":
                         if len(self.info["messages"]) > 1:
                             # Trim the oldest entry in our message history
                             logger.debug(
                                 "Trimming message history to attempt to fit context length"
                             )
                             self.info["messages"] = self.info["messages"][1:]
                             continue
-                        else:
-                            # We only have a single message and it's still to big.
-                            self.console.print(
-                                "Message too large for context size.", style="bold red"
-                            )
-                            self.info["messages"].pop()
-                            raise KeyboardInterrupt
+                        # We only have a single message and it's still to big.
+                        self.console.print(
+                            "Message too large for context size.", style="bold red"
+                        )
+                        self.info["messages"].pop()
+                        raise KeyboardInterrupt from e
+                except openai.InternalServerError as e:
+                    logger.debug(f"InternalServerError: {e}")
+                    self.info["messages"].clear()
+                    raise KeyboardInterrupt from e
                 assert (
                     next(response).choices[0].delta.role == "assistant"
                 ), 'first response should be {"role": "assistant"}'
                 break
         except openai.AuthenticationError as e:
             self.console.print(
                 "Invalid API Key. Please set it in your config file.", style="bold red"
@@ -449,14 +462,15 @@
     config,
     question,
     model,
     context,
     session,
     qq,
     greedy_mode,
+    max_tokens,
     tls_insecure,
     tls_client_cert: Optional[str] = None,
     tls_client_key: Optional[str] = None,
     tls_client_passwd: Optional[str] = None,
 ):
     """Starts a CLI-based chat with the server"""
     orig_cert = (tls_client_cert, tls_client_key, tls_client_passwd)
@@ -507,42 +521,45 @@
         log_file=log_file,
         prompt=not qq,
         vertical_overflow=("visible" if config.visible_overflow else "ellipsis"),
         loaded=loaded,
         greedy_mode=(
             greedy_mode if greedy_mode else config.greedy_mode
         ),  # The CLI flag can only be used to enable
+        max_tokens=(max_tokens if max_tokens else config.max_tokens),
     )
 
     if not qq and session is None:
         # Greet
         ccb.greet(help=True)
 
     # Use the input question to start with
     if len(question) > 0:
         question = " ".join(question)
         if not qq:
             print(f"{PROMPT_PREFIX}{question}")
         try:
-            ccb.start_prompt(question, box=(not qq))
+            ccb.start_prompt(logger, content=question, box=(not qq))
         except ChatException as exc:
             raise ChatException(f"API issue found while executing chat: {exc}")
-        except KeyboardInterrupt:
+        except (ChatQuitException, KeyboardInterrupt, EOFError):
             return
 
     if qq:
         return
 
     # load the history
     if session is not None:
         ccb._load_session_history(loaded)
 
     # Start chatting
     while True:
         try:
-            ccb.start_prompt(logger=logger)
+            ccb.start_prompt(logger)
         except KeyboardInterrupt:
             continue
         except ChatException as exc:
             raise ChatException(f"API issue found while executing chat: {exc}")
         except httpx.RemoteProtocolError:
             raise ChatException(f"Connection to the server was closed")
+        except (ChatQuitException, EOFError):
+            return
```

### Comparing `instructlab-0.14.0/src/instructlab/client.py` & `instructlab-0.15.1/src/instructlab/client.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/config.py` & `instructlab-0.15.1/src/instructlab/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # SPDX-License-Identifier: Apache-2.0
 
 # Standard
 from typing import Optional
 
 # Third Party
-from pydantic import BaseModel, ConfigDict, PositiveInt, StrictStr, ValidationError
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+    PositiveInt,
+    StrictStr,
+    ValidationError,
+    field_validator,
+)
 import httpx
 import yaml
 
 DEFAULT_API_KEY = "no_api_key"
 DEFAULT_CONFIG = "config.yaml"
 DEFAULT_MODEL = "merlinite-7b-lab-Q4_K_M"
 DEFAULT_MODEL_PATH = f"models/{DEFAULT_MODEL}.gguf"
@@ -34,85 +41,106 @@
 
 class _general(BaseModel):
     """Class describing various top-level configuration options for all commands."""
 
     # model configuration
     model_config = ConfigDict(extra="ignore")
 
-    # optional fields
-    log_level: Optional[StrictStr] = "INFO"
+    # additional fields with defaults
+    log_level: StrictStr = "INFO"
+
+    @field_validator("log_level")
+    def validate_log_level(cls, v):
+        # TODO: remove 'valid_levels' once we switch to support Python 3.11+ and call
+        # "logging.getLevelNamesMapping()" instead
+        valid_levels = [
+            "DEBUG",
+            "INFO",
+            "WARNING",
+            "WARN",
+            "FATAL",
+            "CRITICAL",
+            "ERROR",
+            "NOTSET",
+        ]
+        if v.upper() not in valid_levels:
+            raise ValueError(
+                f"'{v}' is not a valid log level name. valid levels: {valid_levels}"
+            )
+        return v.upper()
 
 
 class _chat(BaseModel):
     """Class describing configuration of the chat sub-command."""
 
     # model configuration
     model_config = ConfigDict(extra="ignore")
 
     # required fields
     model: StrictStr
 
-    # optional fields
-    vi_mode: Optional[bool] = False
-    visible_overflow: Optional[bool] = True
-    context: Optional[str] = "default"
+    # additional fields with defaults
+    vi_mode: bool = False
+    visible_overflow: bool = True
+    context: str = "default"
     session: Optional[str] = None
-    logs_dir: Optional[str] = "data/chatlogs"
-    greedy_mode: Optional[bool] = False
+    logs_dir: str = "data/chatlogs"
+    greedy_mode: bool = False
+    max_tokens: Optional[int] = None
 
 
 class _generate(BaseModel):
     """Class describing configuration of the generate sub-command."""
 
     # model configuration
     model_config = ConfigDict(extra="ignore")
 
     # required fields
     model: StrictStr
     taxonomy_path: StrictStr
     taxonomy_base: StrictStr
 
-    # optional fields
-    num_cpus: Optional[PositiveInt] = DEFAULT_NUM_CPUS
-    chunk_word_count: Optional[PositiveInt] = DEFAULT_CHUNK_WORD_COUNT
-    num_instructions: Optional[PositiveInt] = DEFAULT_NUM_INSTRUCTIONS
-    output_dir: Optional[StrictStr] = DEFAULT_GENERATED_FILES_OUTPUT_DIR
-    prompt_file: Optional[StrictStr] = DEFAULT_PROMPT_FILE
-    seed_file: Optional[StrictStr] = "seed_tasks.json"
+    # additional fields with defaults
+    num_cpus: PositiveInt = DEFAULT_NUM_CPUS
+    chunk_word_count: PositiveInt = DEFAULT_CHUNK_WORD_COUNT
+    num_instructions: PositiveInt = DEFAULT_NUM_INSTRUCTIONS
+    output_dir: StrictStr = DEFAULT_GENERATED_FILES_OUTPUT_DIR
+    prompt_file: StrictStr = DEFAULT_PROMPT_FILE
+    seed_file: StrictStr = "seed_tasks.json"
 
 
 class _serve(BaseModel):
     """Class describing configuration of the serve sub-command."""
 
     # model configuration
     model_config = ConfigDict(extra="ignore", protected_namespaces=())
 
     # required fields
     model_path: StrictStr
 
-    # optional fields
-    host_port: Optional[StrictStr] = "127.0.0.1:8000"
-    gpu_layers: Optional[int] = -1
-    max_ctx_size: Optional[PositiveInt] = 4096
+    # additional fields with defaults
+    host_port: StrictStr = "127.0.0.1:8000"
+    gpu_layers: int = -1
+    max_ctx_size: PositiveInt = 4096
 
     def api_base(self):
         """Returns server API URL, based on the configured host and port"""
         return get_api_base(self.host_port)
 
 
 class Config(BaseModel):
     """Configuration for the InstructLab CLI."""
 
     # required fields
     chat: _chat
     generate: _generate
     serve: _serve
 
-    # optional fields
-    general: Optional[_general] = _general()
+    # additional fields with defaults
+    general: _general = _general()
 
     # model configuration
     model_config = ConfigDict(extra="ignore")
 
 
 def get_default_config():
     """Generates default configuration for CLI"""
```

### Comparing `instructlab-0.14.0/src/instructlab/generator/README.md` & `instructlab-0.15.1/src/instructlab/generator/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/generator/generate_data.py` & `instructlab-0.15.1/src/instructlab/generator/generate_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,19 +495,20 @@
         keep = 0
         assess_start = time.time()
         for instruction_data_entry in instruction_data:
             # computing similarity with the pre-tokenized instructions
             new_instruction_tokens = scorer._tokenizer.tokenize(
                 instruction_data_entry["instruction"]
             )
-            with mpctx.Pool(num_cpus) as p:
-                rouge_scores = p.map(
+            with mpctx.Pool(num_cpus) as pool:
+                rouge_scores = pool.map(
                     partial(rouge_scorer._score_lcs, new_instruction_tokens),
                     all_instruction_tokens,
                 )
+            pool.join()
             instruction_data_entry["taxonomy_path"] = selected_taxonomy
             rouge_scores = [score.fmeasure for score in rouge_scores]
             # Comment out extra info not currently being used:
             # most_similar_instructions = {
             #    all_instructions[i]: rouge_scores[i] for i in np.argsort(rouge_scores)[-10:][::-1]
             # }
             if max(rouge_scores) > rouge_threshold:
@@ -554,13 +555,15 @@
         with open(
             os.path.join(output_dir, output_file_test), "w", encoding="utf-8"
         ) as outfile:
             for entry in test_data:
                 json.dump(entry, outfile, ensure_ascii=False)
                 outfile.write("\n")
 
+    progress_bar.close()
+
     if total_discarded or total_rouged:
         logger.info(
             f"{len(machine_instruction_data)} instructions generated, {total_discarded} discarded due to format (see {output_file_discarded}), {total_rouged} discarded due to rouge score"
         )
     generate_duration = time.time() - generate_start
     logger.info(f"Generation took {generate_duration:.2f}s")
```

### Comparing `instructlab-0.14.0/src/instructlab/generator/seed_tasks.jsonl` & `instructlab-0.15.1/src/instructlab/generator/seed_tasks.jsonl`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/generator/utils.py` & `instructlab-0.15.1/src/instructlab/generator/utils.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/lab.py` & `instructlab-0.15.1/src/instructlab/lab.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # pylint: disable=too-many-lines
 
 # Standard
 from glob import glob
 from os.path import basename, dirname, exists, splitext
 import json
 import logging
+import multiprocessing
 import os
 import shutil
 import sys
 import typing
 
 # Third Party
 from click_didyoumean import DYMGroup
@@ -21,74 +22,78 @@
 import click
 import yaml
 
 # Local
 # NOTE: Subcommands are using local imports to speed up startup time.
 from . import config, utils
 
+# 'fork' is unsafe and incompatible with some hardware accelerators.
+# Python 3.14 will switch to 'spawn' on all platforms.
+multiprocessing.set_start_method(
+    config.DEFAULT_MULTIPROCESSING_START_METHOD, force=True
+)
+
 # Set logging level of OpenAI client and httpx library to ERROR to suppress INFO messages
 logging.getLogger("openai").setLevel(logging.ERROR)
 logging.getLogger("httpx").setLevel(logging.ERROR)
 
 if typing.TYPE_CHECKING:
     # Third Party
     import torch
 
 
 class Lab:
     """Lab object holds high-level information about ilab CLI"""
 
-    def __init__(self, filename):
-        self.config_file = filename
-        self.config = config.read_config(filename)
+    def __init__(self, config_obj: config.Config):
+        self.config = config_obj
         FORMAT = "%(levelname)s %(asctime)s %(filename)s:%(lineno)d %(message)s"
         logging.basicConfig(format=FORMAT)
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(self.config.general.log_level.upper())
 
 
-# pylint: disable=unused-argument
-def configure(ctx, param, filename):
-    """Configure is responsible for reading the config file, initiating Lab object and CLI context."""
-    # skip configuration reading when invoked command is `init`
-    if len(sys.argv) > 0 and sys.argv[1] in ("init", "--help"):
-        return
-
-    if not exists(filename):
-        raise click.ClickException(
-            f"`{filename}` does not exists, please run `ilab init` or point to a valid configuration file using `--config=<path>`."
-        )
-
-    try:
-        ctx.obj = Lab(filename)
-    except config.ConfigException as ex:
-        raise click.ClickException(str(ex))
-
-    # default_map holds a dictionary with default values for each command parameters
-    ctx.default_map = config.get_dict(ctx.obj.config)
-
-
 @click.group(cls=DYMGroup)
 @click.option(
     "--config",
+    "config_file",
     type=click.Path(),
     default=config.DEFAULT_CONFIG,
     show_default=True,
-    callback=configure,
-    is_eager=True,
     help="Path to a configuration file.",
 )
 @click.version_option(package_name="instructlab")
 @click.pass_context
 # pylint: disable=redefined-outer-name
-def cli(ctx, config):
+def cli(ctx, config_file):
     """CLI for interacting with InstructLab.
 
     If this is your first time running InstructLab, it's best to start with `ilab init` to create the environment.
     """
+    # ilab init or "--help" have no config file
+    # CliRunner does fill ctx.invoke_subcommand in option callbacks. We have
+    # to validate config_file here.
+    if ctx.invoked_subcommand != "init" and "--help" not in sys.argv[1:]:
+        if config_file == "DEFAULT":
+            config_obj = config.get_default_config()
+        elif not os.path.isfile(config_file):
+            config_obj = None
+            ctx.fail(
+                f"`{config_file}` does not exists, please run `ilab init` "
+                "or point to a valid configuration file using `--config=<path>`."
+            )
+        else:
+            try:
+                config_obj = config.read_config(config_file)
+            except config.ConfigException as ex:
+                raise click.ClickException(str(ex))
+
+        ctx.obj = Lab(config_obj)
+        # default_map holds a dictionary with default values for each command parameters
+        ctx.default_map = config.get_dict(ctx.obj.config)
 
 
 @cli.command()
 @click.option(
     "--interactive/--non-interactive",
     default=True,
     show_default=True,
@@ -241,42 +246,44 @@
         taxonomy_base = ctx.obj.config.generate.taxonomy_base
     if not taxonomy_path:
         taxonomy_path = ctx.obj.config.generate.taxonomy_path
     if not ctx.obj:
         logger = logging.getLogger(__name__)
     else:
         logger = ctx.obj.logger
-    if quiet:
-        try:
-            read_taxonomy(logger, taxonomy_path, taxonomy_base, yaml_rules)
-        except (SystemExit, yaml.YAMLError) as exc:
-            raise SystemExit(1) from exc
-        return
-    try:
-        updated_taxonomy_files = get_taxonomy_diff(taxonomy_path, taxonomy_base)
-    except (SystemExit, GitError) as exc:
-        click.secho(
-            f"Reading taxonomy failed with the following error: {exc}",
-            fg="red",
-        )
-        return
-    for f in updated_taxonomy_files:
-        click.echo(f)
+
+    if not quiet:
+        is_file = os.path.isfile(taxonomy_path)
+        if is_file:  # taxonomy_path is file
+            click.echo(taxonomy_path)
+        else:  # taxonomy_path is dir
+            try:
+                updated_taxonomy_files = get_taxonomy_diff(taxonomy_path, taxonomy_base)
+            except (SystemExit, GitError) as exc:
+                click.secho(
+                    f"Reading taxonomy failed with the following error: {exc}",
+                    fg="red",
+                )
+                raise SystemExit(1) from exc
+            for f in updated_taxonomy_files:
+                click.echo(f)
     try:
         read_taxonomy(logger, taxonomy_path, taxonomy_base, yaml_rules)
     except (SystemExit, yaml.YAMLError) as exc:
+        if not quiet:
+            click.secho(
+                f"Reading taxonomy failed with the following error: {exc}",
+                fg="red",
+            )
+        raise SystemExit(1) from exc
+    if not quiet:
         click.secho(
-            f"Reading taxonomy failed with the following error: {exc}",
-            fg="red",
+            f"Taxonomy in /{taxonomy_path}/ is valid :)",
+            fg="green",
         )
-        raise SystemExit(1) from exc
-    click.secho(
-        f"Taxonomy in /{taxonomy_path}/ is valid :)",
-        fg="green",
-    )
 
 
 # ilab list => ilab diff
 # ilab check => ilab diff --quiet
 utils.make_lab_diff_aliases(cli, diff)
 
 
@@ -471,25 +478,38 @@
     # pylint: disable=C0415
     # Local
     from .generator.generate_data import generate_data
     from .generator.utils import GenerateException
     from .server import ensure_server
 
     server_process = None
+    server_queue = None
     logger = logging.getLogger("TODO")
     prompt_file_path = config.DEFAULT_PROMPT_FILE
     if ctx.obj is not None:
         logger = ctx.obj.logger
         prompt_file_path = ctx.obj.config.generate.prompt_file
 
     if endpoint_url:
         api_base = endpoint_url
     else:
+        # Third Party
+        import llama_cpp
+
+        if not llama_cpp.llama_supports_gpu_offload():
+            # TODO: check for working offloading. The function only checks
+            # for compile time defines like `GGML_USE_CUDA`.
+            click.secho(
+                "llama_cpp_python is built without hardware acceleration. "
+                "ilab generate will be very slow.",
+                fg="red",
+            )
+
         try:
-            server_process, api_base = ensure_server(
+            server_process, api_base, server_queue = ensure_server(
                 ctx.obj.logger,
                 ctx.obj.config.serve,
                 tls_insecure,
                 tls_client_cert,
                 tls_client_key,
                 tls_client_passwd,
                 model_family,
@@ -528,17 +548,19 @@
     except GenerateException as exc:
         click.secho(
             f"Generating dataset failed with the following error: {exc}",
             fg="red",
         )
         raise click.exceptions.Exit(1)
     finally:
-        if server_process:
+        if server_process and server_queue:
             server_process.terminate()
             server_process.join(timeout=30)
+            server_queue.close()
+            server_queue.join_thread()
 
 
 @cli.command()
 @click.argument(
     "question",
     nargs=-1,
     type=click.UNPROCESSED,
@@ -570,14 +592,19 @@
 @click.option(
     "-gm",
     "--greedy-mode",
     is_flag=True,
     help="Use model greedy decoding. Useful for debugging and reproducing errors.",
 )
 @click.option(
+    "--max-tokens",
+    type=click.INT,
+    help="Set a maximum number of tokens to request from the model endpoint.",
+)
+@click.option(
     "--endpoint-url",
     type=click.STRING,
     help="Custom URL endpoint for OpenAI-compatible API. Defaults to the `ilab serve` endpoint.",
 )
 @click.option(
     "--api-key",
     type=click.STRING,
@@ -620,72 +647,125 @@
     ctx,
     question,
     model,
     context,
     session,
     quick_question,
     greedy_mode,
+    max_tokens,
     endpoint_url,
     api_key,
     tls_insecure,
     tls_client_cert,
     tls_client_key,
     tls_client_passwd,
     model_family,
 ):
     """Run a chat using the modified model"""
     # pylint: disable=C0415
     # Local
     from .chat.chat import ChatException, chat_cli
-    from .server import ensure_server
+    from .client import ClientException, list_models
+    from .server import ensure_server, is_temp_server_running
 
     if endpoint_url:
         api_base = endpoint_url
         server_process = None
+        server_queue = None
     else:
         try:
-            server_process, api_base = ensure_server(
+            server_process, api_base, server_queue = ensure_server(
                 ctx.obj.logger,
                 ctx.obj.config.serve,
                 tls_insecure,
                 tls_client_cert,
                 tls_client_key,
                 tls_client_passwd,
                 model_family,
             )
         except Exception as exc:
             click.secho(f"Failed to start server: {exc}", fg="red")
             raise click.exceptions.Exit(1)
         if not api_base:
             api_base = ctx.obj.config.serve.api_base()
 
+    # if only the chat is running (`ilab chat`) and the temp server is not, the chat interacts
+    # in server mode (`ilab serve` is running somewhere, or we are talking to another
+    # OpenAI compatible endpoint).
+    if not is_temp_server_running():
+        # Try to get the model name right if we know we're talking to a local `ilab serve`.
+        #
+        # If the model from the CLI and the one in the config are the same, use the one from the
+        # server if they are different else let's use what the user provided
+        #
+        # 'model' will always get a value and never be None so it's hard to distinguish whether
+        # the value came from the user input or the default value.
+        # We can only assume that if the value is the same as the default value and the value
+        # from the config is the same as the default value, then the user didn't provide a value
+        # we then compare it with the value from the server to see if it's different
+        if (
+            model == config.DEFAULT_MODEL
+            and ctx.obj.config.chat.model == config.DEFAULT_MODEL
+            and api_base == ctx.obj.config.serve.api_base()
+        ):
+            try:
+                models = list_models(
+                    api_base=api_base,
+                    tls_insecure=tls_insecure,
+                    tls_client_cert=tls_client_cert,
+                    tls_client_key=tls_client_key,
+                    tls_client_passwd=tls_client_passwd,
+                )
+
+                # Currently, we only present a single model so we can safely assume that the first model
+                server_model = models.data[0].id if models is not None else None
+
+                # override 'model' with the first returned model if not provided so that the chat print
+                # the model used by the server
+                model = (
+                    server_model
+                    if server_model is not None
+                    and server_model != ctx.obj.config.chat.model
+                    else model
+                )
+
+            except ClientException as exc:
+                click.secho(
+                    f"Failed to list models from {api_base}. Please check the API key and endpoint.",
+                    fg="red",
+                )
+                raise click.exceptions.Exit(1) from exc
+
     try:
         chat_cli(
             logger=ctx.obj.logger,
             api_base=api_base,
             api_key=api_key,
             config=ctx.obj.config.chat,
             question=question,
             model=model,
             context=context,
             session=session,
             qq=quick_question,
             greedy_mode=greedy_mode,
+            max_tokens=max_tokens,
             tls_insecure=tls_insecure,
             tls_client_cert=tls_client_cert,
             tls_client_key=tls_client_key,
             tls_client_passwd=tls_client_passwd,
         )
     except ChatException as exc:
         click.secho(f"Executing chat failed with: {exc}", fg="red")
         raise click.exceptions.Exit(1)
     finally:
-        if server_process:
+        if server_process and server_queue:
             server_process.terminate()
             server_process.join(timeout=30)
+            server_queue.close()
+            server_queue.join_thread()
 
 
 @cli.command()
 @click.option(
     "--repository",
     default="instructlab/merlinite-7b-lab-GGUF",  # TODO: add to config.yaml
     show_default=True,
@@ -705,39 +785,46 @@
 )
 @click.option(
     "--model-dir",
     default=dirname(config.DEFAULT_MODEL_PATH),
     show_default=True,
     help="The local directory to download the model files into.",
 )
-@click.option("--hf-token", envvar="HF_TOKEN")
+@click.option(
+    "--hf-token",
+    default="",
+    envvar="HF_TOKEN",
+    help="User access token for connecting to the Hugging Face Hub.",
+)
 @click.pass_context
 def download(ctx, repository, release, filename, model_dir, hf_token):
     """Download the model(s) to train"""
     click.echo(f"Downloading model from {repository}@{release} to {model_dir}...")
     if hf_token == "" and "instructlab" not in repository:
         raise ValueError(
-            "HF_TOKEN var needs to be set in your environment to download HF Model. The HF Token is used to authenticate your identity to the Hugginface Hub."
+            """HF_TOKEN var needs to be set in your environment to download HF Model. 
+            Alternatively, the token can be passed with --hf-token flag. 
+            The HF Token is used to authenticate your identity to the Hugging Face Hub."""
         )
     try:
         if ctx.obj is not None:
             hf_logging.set_verbosity(ctx.obj.config.general.log_level.upper())
-        files = list_repo_files(repo_id=repository, token=os.getenv("HF_TOKEN"))
+        files = list_repo_files(repo_id=repository, token=hf_token)
         if any(".safetensors" in string for string in files):
             if not os.path.exists(os.path.join(model_dir, repository)):
                 os.makedirs(name=os.path.join(model_dir, repository), exist_ok=True)
             snapshot_download(
-                token=os.getenv("HF_TOKEN"),
+                token=hf_token,
                 repo_id=repository,
                 revision=release,
                 local_dir=os.path.join(model_dir, repository),
             )
         else:
             hf_hub_download(
-                token=os.getenv("HF_TOKEN"),
+                token=hf_token,
                 repo_id=repository,
                 revision=release,
                 filename=filename,
                 local_dir=model_dir,
             )
     except Exception as exc:
         click.secho(
@@ -747,34 +834,34 @@
         raise click.exceptions.Exit(1)
 
 
 class TorchDeviceParam(click.ParamType):
     """Parse and convert device string
 
     Returns a torch.device object:
-    - type is one of 'cpu' or 'cuda')
-    - index is None or CUDA/ROCm device index (0 for first GPU)
+    - type is one of 'cpu', 'cuda', 'hpu'
+    - index is None or device index (e.g. 0 for first GPU)
     """
 
     name = "deviceinfo"
-    supported_devices = {"cuda", "cpu"}
+    supported_devices = {"cuda", "cpu", "hpu"}
 
     def convert(self, value, param, ctx) -> "torch.device":
         # pylint: disable=C0415
         # Function local import, import torch can take more than a second
         # Third Party
         import torch
 
         if not isinstance(value, torch.device):
             try:
                 device = torch.device(value)
             except RuntimeError as e:
                 self.fail(str(e), param, ctx)
 
-        if device.type not in {"cuda", "cpu"}:
+        if device.type not in self.supported_devices:
             supported = ", ".join(repr(s) for s in sorted(self.supported_devices))
             self.fail(
                 f"Unsupported device type '{device.type}'. Only devices "
                 f"types {supported}, and indexed device strings like 'cuda:0' "
                 "are supported for now.",
                 param,
                 ctx,
@@ -789,14 +876,22 @@
                     param,
                     ctx,
                 )
             # map unqualified 'cuda' to current device
             if device.index is None:
                 device = torch.device(device.type, torch.cuda.current_device())
 
+        if device.type == "hpu":
+            click.secho(
+                "WARNING: HPU support is experimental, unstable, and not "
+                "optimized, yet.",
+                fg="red",
+                bold=True,
+            )
+
         return device
 
 
 TORCH_DEVICE = TorchDeviceParam()
 
 
 @cli.command()
@@ -913,14 +1008,21 @@
         try:
             os.listdir(input_dir)  # Test to throw FileNotFound exception
             if not os.path.isdir(data_dir):
                 os.mkdir(data_dir)
             # generated input files reverse sorted by name (contains timestamp)
             train_files = sorted(glob(input_dir + "/train_*"), reverse=True)
             test_files = sorted(glob(input_dir + "/test_*"), reverse=True)
+
+            if not train_files or not test_files:
+                click.secho(
+                    f"{input_dir} does not contain training or test files, did you run `ilab generate`?",
+                    fg="red",
+                )
+                raise click.exceptions.Exit(1)
             if len(train_files) > 1 or len(test_files) > 1:
                 # pylint: disable=f-string-without-interpolation
                 click.secho(
                     f"Found multiple files from `ilab generate`. Using the most recent generation.",
                     fg="yellow",
                 )
             # First file is latest (by above reverse sort and timestamped names)
@@ -934,27 +1036,22 @@
             raise click.exceptions.Exit(1)
         except OSError as exc:
             click.secho(
                 f"Could not create data dir: {exc}",
                 fg="red",
             )
             raise click.exceptions.Exit(1)
-        except IndexError as exc:
-            click.secho(
-                f"Could not copy into data directory: {exc}",
-                fg="red",
-            )
-            raise click.exceptions.Exit(1)
 
     if not utils.is_macos_with_m_chip():
         # Local
         from .llamacpp.llamacpp_convert_to_gguf import convert_llama_to_gguf
         from .train.linux_train import linux_train
 
         linux_train(
+            ctx=ctx,
             train_file=train_files[0],
             test_file=test_files[0],
             model_name=model_name,
             num_epochs=num_epochs,
             device=device,
             four_bit_quant=four_bit_quant,
         )
@@ -998,14 +1095,21 @@
         print("Copied ", config_json[0], "to ", final_results_dir)
         shutil.copy(generation_config_json[0], final_results_dir)
         print("Copied ", generation_config_json[0], "to ", final_results_dir)
         for file in safe_tensors:
             shutil.copy(file, final_results_dir)
             print("Copied ", file, "to ", final_results_dir)
 
+        if four_bit_quant:
+            print(
+                "SKIPPING CONVERSION to gguf. This is unsupported with --4-bit-quant. "
+                + "See https://github.com/instructlab/instructlab/issues/579."
+            )
+            return
+
         convert_llama_to_gguf(model=final_results_dir, pad_vocab=True)
 
         gguf_models_dir = "./models"
         if not os.path.isdir(gguf_models_dir):
             os.mkdir(gguf_models_dir)
         shutil.copy(final_results_dir + "/ggml-model-f16.gguf", gguf_models_dir)
         # cleanup original copy of model
@@ -1167,23 +1271,36 @@
 )
 @click.option(
     "-sq",
     "--skip-quantize",
     is_flag=True,
     help="Whether to skip quantization while converting to GGUF.",
 )
+@click.option(
+    "--model-name",
+    help="Name of the model being trained/converted. Informs the naming of the final trained model file",
+    default=None,
+    show_default=True,
+)
 @utils.macos_requirement(echo_func=click.secho, exit_exception=click.exceptions.Exit)
-def convert(model_dir, adapter_file, skip_de_quantize, skip_quantize):
+@click.pass_context
+def convert(ctx, model_dir, adapter_file, skip_de_quantize, skip_quantize, model_name):
     """Converts model to GGUF"""
     # pylint: disable=C0415
     # Local
     from .llamacpp.llamacpp_convert_to_gguf import convert_llama_to_gguf
     from .train.lora_mlx.convert import convert_between_mlx_and_pytorch
     from .train.lora_mlx.fuse import fine_tune
 
+    # compute model name from model-dir if not supplied
+    if model_name is None:
+        mlx_q_suffix = "-mlx-q"
+        model_name = model_dir.split("/")[-1]
+        model_name = model_name.replace(mlx_q_suffix, "")
+
     if adapter_file is None:
         adapter_file = os.path.join(model_dir, "adapters.npz")
     cli_dir = os.path.dirname(os.path.abspath(__file__))
 
     source_model_dir = model_dir
     model_dir_fused = f"{source_model_dir}-fused"
 
@@ -1191,23 +1308,40 @@
     fine_tune(
         model=source_model_dir,
         save_path=model_dir_fused,
         adapter_file=adapter_file,
         de_quantize=not skip_de_quantize,
     )
 
-    model_dir_fused_pt = f"{model_dir_fused}-pt"
+    ctx.obj.logger.info(f"deleting {source_model_dir}...")
+    shutil.rmtree(source_model_dir)
 
+    model_dir_fused_pt = f"{model_name}-trained"
     # this converts MLX to PyTorch
     convert_between_mlx_and_pytorch(
         hf_path=model_dir_fused, mlx_path=model_dir_fused_pt, local=True, to_pt=True
     )
 
-    convert_llama_to_gguf(model=model_dir_fused_pt, pad_vocab=True)
+    ctx.obj.logger.info(f"deleting {model_dir_fused}...")
+    shutil.rmtree(model_dir_fused)
 
-    # quantize 4-bi GGUF (optional)
+    convert_llama_to_gguf(
+        model=model_dir_fused_pt,
+        pad_vocab=True,
+        skip_unknown=True,
+        outfile=f"{model_dir_fused_pt}/{model_name}.gguf",
+    )
+
+    ctx.obj.logger.info(f"deleting safetensors files from {model_dir_fused_pt}...")
+    for file in glob(os.path.join(model_dir_fused_pt, "*.safetensors")):
+        os.remove(file)
+
+    # quantize to 4-bit GGUF (optional)
     if not skip_quantize:
-        gguf_model_dir = f"{model_dir_fused_pt}/ggml-model-f16.gguf"
-        gguf_model_q_dir = f"{model_dir_fused_pt}/ggml-model-Q4_K_M.gguf"
+        gguf_model_dir = f"{model_dir_fused_pt}/{model_name}.gguf"
+        gguf_model_q_dir = f"{model_dir_fused_pt}/{model_name}-Q4_K_M.gguf"
         script = os.path.join(cli_dir, "llamacpp/quantize")
         cmd = f"{script} {gguf_model_dir} {gguf_model_q_dir} Q4_K_M"
         os.system("{}".format(cmd))
+
+    ctx.obj.logger.info(f"deleting {model_dir_fused_pt}/{model_name}.gguf...")
+    os.remove(os.path.join(model_dir_fused_pt, f"{model_name}.gguf"))
```

### Comparing `instructlab-0.14.0/src/instructlab/llamacpp/LICENSE` & `instructlab-0.15.1/src/instructlab/llamacpp/LICENSE`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/llamacpp/README.md` & `instructlab-0.15.1/src/instructlab/llamacpp/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/llamacpp/llamacpp_convert_to_gguf.py` & `instructlab-0.15.1/src/instructlab/llamacpp/llamacpp_convert_to_gguf.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/llamacpp/quantize` & `instructlab-0.15.1/src/instructlab/llamacpp/quantize`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/mlx_explore/LICENSE` & `instructlab-0.15.1/src/instructlab/mlx_explore/LICENSE`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/mlx_explore/README.md` & `instructlab-0.15.1/src/instructlab/mlx_explore/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/mlx_explore/gguf_convert_to_mlx.py` & `instructlab-0.15.1/src/instructlab/mlx_explore/gguf_convert_to_mlx.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/mlx_explore/utils.py` & `instructlab-0.15.1/src/instructlab/mlx_explore/utils.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/schema/v1/compositional_skills.json` & `instructlab-0.15.1/src/instructlab/schema/v1/compositional_skills.json`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/schema/v1/knowledge.json` & `instructlab-0.15.1/src/instructlab/schema/v1/knowledge.json`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/schema/v2/compositional_skills.json` & `instructlab-0.15.1/src/instructlab/schema/v2/compositional_skills.json`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/schema/v2/knowledge.json` & `instructlab-0.15.1/src/instructlab/schema/v2/knowledge.json`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/server.py` & `instructlab-0.15.1/src/instructlab/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,25 +57,26 @@
     model_family,
 ):
     """Checks if server is running, if not starts one as a subprocess. Returns the server process
     and the URL where it's available."""
     try:
         api_base = serve_config.api_base()
         logger.debug(f"Trying to connect to {api_base}...")
+        # pylint: disable=duplicate-code
         list_models(
             api_base=api_base,
             tls_insecure=tls_insecure,
             tls_client_cert=tls_client_cert,
             tls_client_key=tls_client_key,
             tls_client_passwd=tls_client_passwd,
         )
-        return (None, None)
+        return (None, None, None)
+        # pylint: enable=duplicate-code
     except ClientException:
         tried_ports = set()
-        # TODO: use default server, "spawn" doesn't work?
         mpctx = multiprocessing.get_context(None)
         # use a queue to communicate between the main process and the server process
         queue = mpctx.Queue()
         port = random.randint(1024, 65535)
         host = serve_config.host_port.rsplit(":", 1)[0]
         logger.debug(f"Trying port {port}...")
 
@@ -115,15 +116,14 @@
                 "gpu_layers": serve_config.gpu_layers,
                 "max_ctx_size": serve_config.max_ctx_size,
                 "model_family": model_family,
                 "port": port,
                 "host": host,
                 "queue": queue,
             },
-            daemon=True,
         )
         server_process.start()
 
         # in case the server takes some time to fail we wait a bit
         count = 0
         while server_process.is_alive():
             sleep(0.1)
@@ -132,15 +132,15 @@
             count += 1
 
         # if the queue is not empty it means the server failed to start
         if not queue.empty():
             # pylint: disable=raise-missing-from
             raise queue.get()
 
-        return (server_process, temp_api_base)
+        return (server_process, temp_api_base, queue)
 
 
 def server(
     logger,
     model_path,
     gpu_layers,
     max_ctx_size,
@@ -159,17 +159,25 @@
         n_gpu_layers=gpu_layers,
         verbose=logger.level == logging.DEBUG,
     )
     if threads is not None:
         settings.n_threads = threads
     try:
         app = create_app(settings=settings)
+
+        @app.get("/")
+        def read_root():
+            return {
+                "message": "Hello from InstructLab! Visit us at https://instructlab.ai"
+            }
     except ValueError as exc:
         if queue:
             queue.put(exc)
+            queue.close()
+            queue.join_thread()
             return
         raise ServerException(f"failed creating the server application: {exc}") from exc
 
     template = ""
     eos_token = "<|endoftext|>"
     bos_token = ""
     for template_dict in templates:
@@ -186,14 +194,16 @@
                 bos_token=bos_token,
             ).to_chat_handler()
         )
     # pylint: disable=broad-exception-caught
     except Exception as exc:
         if queue:
             queue.put(exc)
+            queue.close()
+            queue.join_thread()
             return
         raise ServerException(f"failed creating the server application: {exc}") from exc
 
     logger.info("Starting server process, press CTRL+C to shutdown server...")
     logger.info(
         f"After application startup complete see http://{host}:{port}/docs for API."
     )
@@ -219,14 +229,18 @@
             redirect_stdout(f),
             redirect_stderr(f),
         ):
             s.run()
     else:
         s.run()
 
+    if queue:
+        queue.close()
+        queue.join_thread()
+
 
 def can_bind_to_port(host, port):
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         try:
             s.bind((host, port))
             return True
         except socket.error:
```

### Comparing `instructlab-0.14.0/src/instructlab/train/linux_train.py` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/lora.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,302 +1,349 @@
-# SPDX-License-Identifier: Apache-2.0
+# SPDX-License-Identifier: MIT
+# Copyright © 2023 Apple Inc.
 
 # Standard
+from pathlib import Path
 from typing import Optional
+import json
+import math
+import time
 
 # Third Party
-from datasets import load_dataset
-from peft import LoraConfig
-from transformers import (
-    AutoConfig,
-    AutoModelForCausalLM,
-    AutoTokenizer,
-    BitsAndBytesConfig,
-    StoppingCriteria,
-    StoppingCriteriaList,
-    TrainingArguments,
-)
-from trl import DataCollatorForCompletionOnlyLM, SFTTrainer
-import torch
+from mlx.utils import tree_flatten, tree_unflatten
+import mlx.core as mx
+import mlx.nn as nn
+import mlx.optimizers as optim
+import numpy as np
 
 # Local
-from ..chat.chat import CONTEXTS
-from ..config import DEFAULT_MULTIPROCESSING_START_METHOD
+from . import utils as lora_utils
+from .models.lora import LoRALinear
 
-# TODO CPU: Look into using these extensions
-# import intel_extension_for_pytorch as ipex
 
-# 'fork' incompatible with some hardware accelerators
-torch.multiprocessing.set_start_method(DEFAULT_MULTIPROCESSING_START_METHOD)
-
-
-class StoppingCriteriaSub(StoppingCriteria):
-    def __init__(self, stops=[], encounters=1):
-        super().__init__()
-        self.stops = [stop for stop in stops]
-
-    def __call__(
-        self, input_ids: torch.LongTensor, scores: torch.FloatTensor, **kwargs
-    ) -> bool:
-        for seq in input_ids:
-            for stop in self.stops:
-                if stop == seq[-1]:
-                    return True
-        return False
-
-
-def create_prompt(
-    user: str,
-    system: str = CONTEXTS["default"],
-):
-    return f"""\
-    <|system|>
-    {system}
-    <|user|>
-    {user}
-    <|assistant|>
+class Dataset:
+    """
+    Light-weight wrapper to hold lines from a jsonl file
     """
 
+    def __init__(self, path: Path, key: str = "text"):
+        if not path.exists():
+            self._data = None
+        else:
+            with open(path, "r") as fid:
+                self._data = [json.loads(l) for l in fid]
+        self._key = key
+
+    def __getitem__(self, idx: int):
+        return self._data[idx][self._key]
+
+    def __len__(self):
+        return len(self._data)
+
+
+def load(data, train, test):
+    def load_and_check(name):
+        dataset_path = Path(data) / f"{name}.jsonl"
+        try:
+            return Dataset(dataset_path)
+        except Exception as e:
+            print(f"Unable to build dataset {dataset_path} ({e})")
+            raise
+
+    names = ("train", "valid", "test")
+    train_dataset_path, valid_dataset_path, test_dataset_path = (
+        load_and_check(n) for n in names
+    )
 
-def formatting_prompts_func(example):
-    output_texts = []
-    for i in range(len(example["system"])):
-        text = f"<|system|>\n{example['system'][i]}\n<|user|>\n{example['user'][i]}\n<|assistant|>\n{example['assistant'][i]}<|endoftext|>"
-        output_texts.append(text)
-    return output_texts
-
-
-def report_cuda_device(args_device, min_vram=0):
-    """Report CUDA/ROCm device properties"""
-    print(f"  NVidia CUDA version: {torch.version.cuda or 'n/a'}")
-    print(f"  AMD ROCm HIP version: {torch.version.hip or 'n/a'}")
-
-    def _gib(size: int) -> str:
-        return "{:.1f} GiB".format(size / 1024**3)
-
-    for idx in range(torch.cuda.device_count()):
-        device = torch.device("cuda", idx)
-        name = torch.cuda.get_device_name(device)
-        free, total = torch.cuda.mem_get_info(device)
-        capmin, capmax = torch.cuda.get_device_capability(device)
-        print(
-            f"  {device} is '{name}' ({_gib(free)} of {_gib(total)} free, "
-            f"capability: {capmin}.{capmax})"
+    if train and len(train_dataset_path) == 0:
+        raise ValueError(
+            "Training set not found or empty. Must provide training set for fine-tuning."
         )
-
-    if args_device.index is None:
-        index = torch.cuda.current_device()
-    else:
-        index = args_device.index
-
-    free = torch.cuda.mem_get_info(index)[0]
-    if free < min_vram:
-        print(
-            f"  WARNING: You have less than {min_vram} GiB of free GPU "
-            "memory on '{index}'. Training may fail, use slow shared "
-            "host memory, or move some layers to CPU."
+    if train and len(valid_dataset_path) == 0:
+        raise ValueError(
+            "Validation set not found or empty. Must provide validation set for fine-tuning."
         )
-        print(
-            "  Training does not use the local InstructLab serve. Consider "
-            "stopping the server to free up about 5 GiB of GPU memory."
+    if test and len(test_dataset_path) == 0:
+        raise ValueError(
+            "Test set not found or empty. Must provide test set for evaluation."
         )
+    return train_dataset_path, valid_dataset_path, test_dataset_path
 
 
-def linux_train(
-    train_file: str,
-    test_file: str,
-    model_name: str,
-    num_epochs: Optional[int] = None,
-    device: torch.device = torch.device("cpu"),
-    four_bit_quant: bool = False,
+def loss(model, inputs, targets, lengths):
+    # Run model on inputs
+    logits, _ = model(inputs)
+    logits = logits.astype(mx.float32)
+
+    # Mask padding tokens
+    length_mask = mx.arange(inputs.shape[1])[None, :] < lengths[:, None]
+
+    # Calculate the loss
+    ce = nn.losses.cross_entropy(logits, targets) * length_mask
+    ntoks = length_mask.sum()
+    ce = ce.sum() / ntoks
+    return ce, ntoks
+
+
+def iterate_batches(dset, tokenizer, batch_size, train=False):
+    # Shuffle indices
+    while True:
+        indices = np.arange(len(dset))
+        if train:
+            indices = np.random.permutation(indices)
+
+        # Collect batches from dataset
+        for i in range(0, len(indices) - batch_size + 1, batch_size):
+            # Encode batch
+            batch = [tokenizer.encode(dset[indices[i + j]]) for j in range(batch_size)]
+            lengths = [len(x) for x in batch]
+
+            # Check if any sequence is longer than 2048 tokens
+            if max(lengths) > 2048:
+                print(
+                    "[WARNING] Some sequences are longer than 2048 tokens. "
+                    "Consider pre-splitting your data to save memory."
+                )
+
+            # Pad to the max length
+            batch_arr = np.zeros((batch_size, max(lengths)), np.int32)
+
+            for j in range(batch_size):
+                batch_arr[j, : lengths[j]] = batch[j]
+            batch = mx.array(batch_arr)
+            yield batch[:, :-1], batch[:, 1:], mx.array(lengths)
+
+        if not train:
+            break
+
+
+def evaluate(model, dataset, loss, tokenizer, batch_size, num_batches):
+    all_losses = []
+    ntokens = 0
+    for it, batch in zip(
+        range(num_batches),
+        iterate_batches(dataset, tokenizer, batch_size),
+    ):
+        losses, toks = loss(model, *batch)
+        all_losses.append((losses * toks).item())
+        ntokens += toks.item()
+
+    return np.sum(all_losses) / ntokens
+
+
+def train_model(
+    model,
+    train_set,
+    val_set,
+    optimizer,
+    loss,
+    tokenizer,
+    iters,
+    batch_size,
+    steps_per_report,
+    steps_per_eval,
+    val_batches,
+    save_every,
+    adapter_file,
 ):
-    """Lab Train for Linux!"""
-    print("LINUX_TRAIN.PY: NUM EPOCHS IS: ", num_epochs)
-    print("LINUX_TRAIN.PY: TRAIN FILE IS: ", train_file)
-    print("LINUX_TRAIN.PY: TEST FILE IS: ", test_file)
-
-    print(f"LINUX_TRAIN.PY: Using device '{device}'")
-    if device.type == "cuda":
-        # estimated by watching nvtop / radeontop during training
-        min_vram = 11 if four_bit_quant else 17
-        report_cuda_device(device, min_vram)
-
-    print("LINUX_TRAIN.PY: LOADING DATASETS")
-    # Get the file name
-    train_dataset = load_dataset("json", data_files=train_file, split="train")
-
-    test_dataset = load_dataset("json", data_files=test_file, split="train")
-    train_dataset.to_pandas().head()
-
-    tokenizer = AutoTokenizer.from_pretrained(model_name, trust_remote_code=True)
-    tokenizer.pad_token = tokenizer.eos_token
-
-    response_template = "\n<|assistant|>\n"
-
-    response_template_ids = tokenizer.encode(
-        response_template, add_special_tokens=False
-    )[2:]
-    collator = DataCollatorForCompletionOnlyLM(
-        response_template_ids, tokenizer=tokenizer
-    )
+    # Create value and grad function for loss
+    loss_value_and_grad = nn.value_and_grad(model, loss)
 
-    if four_bit_quant:
-        print("LINUX_TRAIN.PY: USING 4-bit quantization with BitsAndBytes")
-        use_fp16 = True
-        bnb_config = BitsAndBytesConfig(
-            load_in_4bit=True,
-            bnb_4bit_quant_type="nf4",
-            bnb_4bit_use_double_quant=True,
-            bnb_4bit_compute_dtype=torch.float16,  # if not set will throw a warning about slow speeds when training
-        )
+    losses = []
+    n_tokens = 0
+
+    # Main training loop
+    start = time.perf_counter()
+    for it, batch in zip(
+        range(iters),
+        iterate_batches(train_set, tokenizer, batch_size, train=True),
+    ):
+        # Forward and backward pass
+        (lvalue, toks), grad = loss_value_and_grad(model, *batch)
+
+        # Model update
+        optimizer.update(model, grad)
+        mx.eval(model.parameters(), optimizer.state, lvalue)
+
+        # Record loss
+        losses.append(lvalue.item())
+        n_tokens += toks.item()
+
+        # Report training loss if needed
+        if (it + 1) % steps_per_report == 0:
+            train_loss = np.mean(losses)
+
+            stop = time.perf_counter()
+            print(
+                f"Iter {it+1:03d}: Train loss {train_loss:.3f}, "
+                f"It/sec {steps_per_report / (stop - start):.3f}, "
+                f"Tokens/sec {float(n_tokens) / (stop - start):.3f}"
+            )
+            losses = []
+            n_tokens = 0
+            start = time.perf_counter()
+
+        # Report validation loss if needed
+        if it == 0 or (it + 1) % steps_per_eval == 0:
+            stop = time.perf_counter()
+            val_loss = evaluate(
+                model, val_set, loss, tokenizer, batch_size, val_batches
+            )
+            epoch = (it * batch_size) // len(train_set)
+            print(
+                f"Epoch {epoch + 1}: "
+                f"Iter {it + 1}: "
+                f"Val loss {val_loss:.3f}, "
+                f"Val took {(time.perf_counter() - stop):.3f}s"
+            )
+
+            start = time.perf_counter()
+
+        # Save adapter weights if needed
+        if (it + 1) % save_every == 0:
+            mx.savez(adapter_file, **dict(tree_flatten(model.trainable_parameters())))
+            a, b = adapter_file.split(".")
+            fn = f"{a}-{it+1:03d}.{b}"
+            mx.savez(fn, **dict(tree_flatten(model.trainable_parameters())))
+            print(f"Iter {it + 1}: Saved adapter weights to {fn}.")
+
+
+def generate(model, prompt, tokenizer, stream, temp, max_tokens):
+    if stream:
+        print(prompt, end="", flush=True)
+
+    prompt = mx.array(tokenizer.encode(prompt))
+
+    tokens = []
+    skip = 0
+    for token, n in zip(
+        lora_utils.generate(prompt, model, temp),
+        range(max_tokens),
+    ):
+        if token == tokenizer.eos_token_id:
+            break
+
+        tokens.append(token.item())
+        s = tokenizer.decode(tokens)
+        if len(s) - skip > 1:
+            if stream:
+                print(s[skip:-1], end="", flush=True)
+            skip = len(s) - 1
+    if stream:
+        print(tokenizer.decode(tokens)[skip:], flush=True)
     else:
-        print("LINUX_TRAIN.PY: NOT USING 4-bit quantization")
-        use_fp16 = False
-        bnb_config = None
-
-    # Loading the model
-    print("LINUX_TRAIN.PY: LOADING THE BASE MODEL")
-    config = AutoConfig.from_pretrained(
-        model_name, torchscript=True, trust_remote_code=True
-    )
+        print("=" * 10)
+        print(tokenizer.decode(tokens).strip())
+        print("=" * 10)
+    if len(tokens) == 0:
+        print("No tokens generated for this prompt")
+        return
+
+
+def load_and_train(
+    model: str = "mlx_model",
+    max_tokens: int = 100,
+    temp: float = 0.8,
+    prompt: Optional[str] = None,
+    train: bool = False,
+    data: str = "data/",
+    lora_layers: int = 16,
+    batch_size: int = 4,
+    iters: int = 1000,
+    val_batches: int = 25,
+    learning_rate: float = 1e-5,
+    steps_per_report: int = 10,
+    steps_per_eval: int = 200,
+    resume_adapter_file: Optional[str] = None,
+    adapter_file: str = "adapters.npz",
+    save_every: int = 100,
+    test: bool = False,
+    stream: bool = False,
+    no_adapter: bool = False,
+    test_batches: int = 500,
+    seed: int = 0,
+):
+    """LoRA or QLoRA fine tuning."""
+    np.random.seed(seed)
 
-    model = AutoModelForCausalLM.from_pretrained(
-        model_name,
-        torch_dtype="auto",
-        quantization_config=bnb_config,
-        config=config,
-        trust_remote_code=True,
-        low_cpu_mem_usage=True,
-    )
-    if model.device != device:
-        model = model.to(device)
-    print(f"LINUX_TRAIN.PY: Model device {model.device}")
-    if model.device.type == "cuda":
-        print(torch.cuda.memory_summary())
-
-    print("LINUX_TRAIN.PY: SANITY CHECKING THE BASE MODEL")
-    stop_words = ["<|endoftext|>", "<|assistant|>"]
-    stop_words_ids = [
-        tokenizer(stop_word, return_tensors="pt", add_special_tokens=False)[
-            "input_ids"
-        ].squeeze()
-        for stop_word in stop_words
-    ]
-    stopping_criteria = StoppingCriteriaList(
-        [StoppingCriteriaSub(stops=stop_words_ids)]
-    )
+    print("Loading pretrained model")
+    model, tokenizer, _ = lora_utils.load(model)
 
-    def model_generate(user):
-        text = create_prompt(user=user)
+    # Freeze all layers other than LORA linears
+    model.freeze()
+    if not no_adapter:
+        for l in model.model.layers[len(model.model.layers) - lora_layers :]:
+            l.self_attn.q_proj = LoRALinear.from_linear(l.self_attn.q_proj)
+            l.self_attn.v_proj = LoRALinear.from_linear(l.self_attn.v_proj)
+            if hasattr(l, "block_sparse_moe"):
+                l.block_sparse_moe.gate = LoRALinear.from_linear(
+                    l.block_sparse_moe.gate
+                )
+    else:
+        print("LoRA init skipped")
 
-        input_ids = tokenizer(text, return_tensors="pt").input_ids.to(model.device)
-        outputs = model.generate(
-            input_ids=input_ids,
-            max_new_tokens=256,
-            pad_token_id=tokenizer.eos_token_id,
-            temperature=0.7,
-            top_p=0.9,
-            stopping_criteria=stopping_criteria,
-            do_sample=True,
+    p = sum(v.size for _, v in tree_flatten(model.parameters())) / 10**6
+    print(f"Total parameters {p:.3f}M")
+    p = sum(v.size for _, v in tree_flatten(model.trainable_parameters())) / 10**6
+    print(f"Trainable parameters {p:.3f}M")
+
+    print("Loading datasets")
+    train_set, valid_set, test_set = load(data, train, test)
+
+    # Resume training the given adapters.
+    if resume_adapter_file is not None:
+        print(f"Loading pretrained adapters from {resume_adapter_file}")
+        model.load_weights(resume_adapter_file, strict=False)
+
+    if train:
+        print("Training")
+        opt = optim.Adam(learning_rate=learning_rate)
+
+        # Train model
+        train_model(
+            model,
+            train_set,
+            valid_set,
+            opt,
+            loss,
+            tokenizer,
+            iters,
+            batch_size,
+            steps_per_report,
+            steps_per_eval,
+            val_batches,
+            save_every,
+            adapter_file,
         )
-        return tokenizer.batch_decode([o[:-1] for o in outputs])[0]
-
-    assistant_old_lst = [
-        model_generate(d["user"]).split(response_template.strip())[-1].strip()
-        for d in test_dataset
-    ]
-    attention_layers = [
-        module for module in model.modules() if "attention" in str(type(module)).lower()
-    ]
-
-    print("LINUX_TRAIN.PY: GETTING THE ATTENTION LAYERS")
-    # Print information about the attention modules
-    for i, layer in enumerate(attention_layers):
-        for par in list(layer.named_parameters()):
-            mod = par[0]
-            if isinstance(mod, str):
-                mod.split(".")[0]
-        break
-
-    print("LINUX_TRAIN.PY: CONFIGURING LoRA")
-
-    lora_alpha = 32
-    lora_dropout = 0.1
-    lora_r = 4
-
-    target_modules = ["q_proj", "k_proj", "v_proj", "o_proj"]
-
-    peft_config = LoraConfig(
-        lora_alpha=lora_alpha,
-        lora_dropout=lora_dropout,
-        r=lora_r,
-        bias="none",
-        task_type="CAUSAL_LM",
-        target_modules=target_modules,
-    )
-
-    output_dir = "./training_results"
-    per_device_train_batch_size = 1
 
-    training_arguments = TrainingArguments(
-        output_dir=output_dir,
-        num_train_epochs=num_epochs,
-        per_device_train_batch_size=per_device_train_batch_size,
-        fp16=use_fp16,
-        bf16=not use_fp16,
-        # use_ipex=True, # TODO CPU test this possible optimization
-        use_cpu=model.device.type == "cpu",
-        save_strategy="epoch",
-        report_to="none",
-        # options to reduce GPU memory usage and improve performance
-        # https://huggingface.co/docs/transformers/perf_train_gpu_one
-        # https://stackoverflow.com/a/75793317
-        # torch_compile=True,
-        # fp16=False,  # fp16 increases memory consumption 1.5x
-        # gradient_accumulation_steps=8,
-        # gradient_checkpointing=True,
-        # eval_accumulation_steps=1,
-        # per_device_eval_batch_size=1,
-    )
-
-    max_seq_length = 300
-    tokenizer.padding_side = "right"
-    trainer = SFTTrainer(
-        model=model,
-        train_dataset=train_dataset,
-        eval_dataset=test_dataset,
-        peft_config=peft_config,
-        formatting_func=formatting_prompts_func,
-        data_collator=collator,
-        max_seq_length=max_seq_length,
-        tokenizer=tokenizer,
-        args=training_arguments,
-    )
+        # Save adapter weights
+        mx.savez(adapter_file, **dict(tree_flatten(model.trainable_parameters())))
 
-    print("LINUX_TRAIN.PY: TRAINING")
-    trainer.train()
-
-    model.config.use_cache = True
-
-    print("LINUX_TRAIN.PY: RUNNING INFERENCE ON THE OUTPUT MODEL")
+    if not no_adapter:
+        # Load the LoRA adapter weights which we assume should exist by this point
+        if not Path(adapter_file).is_file():
+            raise ValueError(
+                f"Adapter file {adapter_file} missing. "
+                "Use --train to learn and save the adapters.npz."
+            )
+        model.load_weights(adapter_file, strict=False)
+    else:
+        print("LoRA loading skipped")
 
-    for i, (d, assistant_old) in enumerate(zip(test_dataset, assistant_old_lst)):
-        assistant_new = (
-            model_generate(d["user"]).split(response_template.strip())[-1].strip()
+    if test:
+        print("Testing")
+        model.eval()
+        test_loss = evaluate(
+            model,
+            test_set,
+            loss,
+            tokenizer,
+            batch_size,
+            num_batches=test_batches,
         )
-        assistant_expected = d["assistant"]
+        test_ppl = math.exp(test_loss)
 
-        print(f"\n===\ntest {i}\n===\n")
-        print("\n===\nuser\n===\n")
-        print(d["user"])
-        print("\n===\nassistant_old\n===\n")
-        print(assistant_old)
-        print("\n===\nassistant_new\n===\n")
-        print(assistant_new)
-        print("\n===\nassistant_expected\n===\n")
-        print(assistant_expected)
-
-    print("LINUX_TRAIN.PY: MERGING ADAPTERS")
-    model = trainer.model.merge_and_unload()
-    model.save_pretrained("./training_results/merged_model")
+        print(f"Test loss {test_loss:.3f}, Test ppl {test_ppl:.3f}.")
 
-    print("LINUX_TRAIN.PY: FINISHED")
+    if prompt is not None:
+        print("Generating")
+        generate(model, prompt, tokenizer, stream, temp, max_tokens)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `instructlab-0.14.0/src/instructlab/train/lora_mlx/LICENSE` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/LICENSE`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/train/lora_mlx/README.md` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/train/lora_mlx/convert.py` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/convert.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/train/lora_mlx/fuse.py` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/fuse.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/train/lora_mlx/make_data.py` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/make_data.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/train/lora_mlx/models/README.md` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/models/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/train/lora_mlx/models/llama.py` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/models/llama.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/train/lora_mlx/models/lora.py` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/models/lora.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/train/lora_mlx/models/mixtral.py` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/train/lora_mlx/models/models.py` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/models/models.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/train/lora_mlx/models/phi2.py` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/models/phi2.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/train/lora_mlx/prepare_model.py` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/prepare_model.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/train/lora_mlx/utils.py` & `instructlab-0.15.1/src/instructlab/train/lora_mlx/utils.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/src/instructlab/utils.py` & `instructlab-0.15.1/src/instructlab/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 extends: relaxed
 
 rules:
   line-length:
     max: 120
 """
 
+DEFAULT_CHUNK_OVERLAP = 100
+
 logging.basicConfig(
     level=logging.INFO,
     format="%(levelname)s %(asctime)s %(filename)s:%(lineno)d %(message)s",
 )
 
 
 class TaxonomyReadingException(Exception):
@@ -217,52 +219,62 @@
             logger.debug("Processing files...")
             for pattern in file_patterns:
                 for file_path in glob.glob(os.path.join(repo.working_dir, pattern)):
                     if os.path.isfile(file_path) and file_path.endswith(".md"):
                         with open(file_path, "r", encoding="utf-8") as file:
                             file_contents.append(file.read())
 
-            return file_contents
+            if file_contents:
+                return file_contents
+            raise SystemExit("Couldn't find knowledge documents")
         except (OSError, exc.GitCommandError, FileNotFoundError) as e:
             raise e
 
 
 def git_clone_checkout(
     repo_url: str, temp_dir: str, commit_hash: str, skip_checkout: bool
 ) -> Repo:
     repo = Repo.clone_from(repo_url, temp_dir)
     if not skip_checkout:
         repo.git.checkout(commit_hash)
     return repo
 
 
+def num_tokens_from_words(num_words) -> int:
+    return int(num_words * 1.3)  # 1 word ~ 1.3 token
+
+
+def num_chars_from_tokens(num_tokens) -> int:
+    return int(num_tokens * 4)  # 1 token ~ 4 English character
+
+
 def chunk_document(documents: List, server_ctx_size, chunk_word_count) -> List[str]:
     """
     Iterates over the documents and splits them into chunks based on the word count provided by the user.
     Args:
         documents (dict): List of documents retrieved from git (can also consist of a single document).
         server_ctx_size (int): Context window size of server.
         chunk_word_count (int): Maximum number of words to chunk a document.
     Returns:
          List[str]: List of chunked documents.
     """
-    no_tokens_per_doc = int(chunk_word_count * 1.3)  # 1 word ~ 1.3 token
+    no_tokens_per_doc = num_tokens_from_words(chunk_word_count)
     if no_tokens_per_doc > int(server_ctx_size - 1024):
         raise ValueError(
             "Error: {}".format(
                 str(
                     f"Given word count ({chunk_word_count}) per doc will exceed the server context window size ({server_ctx_size})"
                 )
             )
         )
     content = []
     text_splitter = RecursiveCharacterTextSplitter(
-        separators=["\n\n", "\n"],
-        chunk_size=int(no_tokens_per_doc * 4),  # 1 token ~ 4 English character
-        chunk_overlap=100,
+        separators=["\n\n", "\n", " "],
+        chunk_size=num_chars_from_tokens(no_tokens_per_doc),
+        chunk_overlap=DEFAULT_CHUNK_OVERLAP,
     )
 
     for docs in documents:
         temp = text_splitter.create_documents([docs])
         content.extend([item.page_content for item in temp])
 
     return content
```

### Comparing `instructlab-0.14.0/src/instructlab.egg-info/PKG-INFO` & `instructlab-0.15.1/src/instructlab.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructlab
-Version: 0.14.0
+Version: 0.15.1
 Summary: CLI for interacting with InstructLab
 Author-email: TBD <jon@example.com>
 License: Apache-2.0 AND MIT
 Project-URL: homepage, https://instructlab.io
 Project-URL: source, https://github.com/instructlab/instructlab
 Project-URL: issues, https://github.com/instructlab/instructlab/issues
 Classifier: Development Status :: 3 - Alpha
@@ -24,140 +24,213 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click<9.0.0,>=8.1.7
 Requires-Dist: click-didyoumean<0.4.0,>=0.3.0
 Requires-Dist: datasets<3.0.0,>=2.18.0
 Requires-Dist: gguf<0.7.0,>=0.6.0
 Requires-Dist: GitPython<4.0.0,>=3.1.42
-Requires-Dist: httpx
+Requires-Dist: httpx<1.0.0,>=0.25.0
 Requires-Dist: jsonschema<5.0.0,>=4.21.1
-Requires-Dist: llama_cpp_python[server]==0.2.55
+Requires-Dist: llama_cpp_python[server]==0.2.75
 Requires-Dist: mlx<0.6.0,>=0.5.1; sys_platform == "darwin" and platform_machine == "arm64"
-Requires-Dist: numpy<2.0.0,>=1.26.4
+Requires-Dist: numpy<2.0.0,>=1.23.5; python_version == "3.10"
+Requires-Dist: numpy<2.0.0,>=1.26.4; python_version != "3.10"
 Requires-Dist: openai<2.0.0,>=1.13.3
 Requires-Dist: peft<0.10.0,>=0.9.0
 Requires-Dist: prompt-toolkit<4.0.0,>=3.0.38
-Requires-Dist: pydantic
-Requires-Dist: pydantic_yaml
-Requires-Dist: PyYAML<7.0.0,>=6.0.1
+Requires-Dist: pydantic<3.0.0,>=2.6.0
+Requires-Dist: pydantic_yaml<2.0.0,>=1.2.0
+Requires-Dist: PyYAML<7.0.0,>=6.0.0
 Requires-Dist: rich<14.0.0,>=13.3.1
 Requires-Dist: rouge-score<0.2.0,>=0.1.2
 Requires-Dist: sentencepiece<0.3.0,>=0.2.0
 Requires-Dist: tokenizers<0.16.0,>=0.15.2
 Requires-Dist: toml<0.11.0,>=0.10.2
-Requires-Dist: torch<3.0.0,>=2.2.1
+Requires-Dist: torch<3.0.0,>=2.2.0a0; python_version == "3.10"
+Requires-Dist: torch<3.0.0,>=2.2.1; python_version != "3.10"
 Requires-Dist: tqdm<5.0.0,>=4.66.2
 Requires-Dist: transformers<=4.38.2,>=4.30.0
 Requires-Dist: trl<0.8.0,>=0.7.11
 Requires-Dist: wandb<0.17.0,>=0.16.4
 Requires-Dist: langchain-text-splitters
 Requires-Dist: yamllint<1.36.0,>=1.35.1
 
 # InstructLab 🐶 (`ilab`)
 
 ![Lint](https://github.com/instructlab/instructlab/actions/workflows/lint.yml/badge.svg?branch=main)
 ![Tests](https://github.com/instructlab/instructlab/actions/workflows/test.yml/badge.svg?branch=main)
 ![Build](https://github.com/instructlab/instructlab/actions/workflows/pypi.yaml/badge.svg?branch=main)
-[![Demo](https://img.shields.io/badge/Demo-v0.13.0-blue)](https://asciinema.org/a/PmRU7IrReep04FY6qpzo2Zclc)
+![Release](https://img.shields.io/github/v/release/instructlab/instructlab)
 ![License](https://img.shields.io/github/license/instructlab/instructlab)
 
 ## 📖 Contents
 
-- [❓What is `ilab`](#-what-is-ilab)
+- [Welcome to the InstructLab CLI](#welcome-to-the-instructlab-cli)
+- [❓ What is `ilab`](#-what-is-ilab)
 - [📋 Requirements](#-requirements)
 - [✅ Getting started](#-getting-started)
-  - [🧰 Installing`ilab`](#-installing-ilab)
-  - [🏗️ Initialize `ilab`](#%EF%B8%8F-initialize-ilab)
+  - [🧰 Installing `ilab`](#-installing-ilab)
+    - [To install with no GPU acceleration and PyTorch without CUDA bindings](#to-install-with-no-gpu-acceleration-and-pytorch-without-cuda-bindings)
+    - [To install with AMD ROCm](#to-install-with-amd-rocm)
+    - [To install with Apple Metal on M1/M2/M3 Mac](#to-install-with-apple-metal-on-m1m2m3-mac)
+    - [To install with Nvidia CUDA](#to-install-with-nvidia-cuda)
+    - [Example output](#example-output)
+    - [Bash (version 4.4 or newer)](#bash-version-44-or-newer)
+    - [Zsh](#zsh)
+    - [Fish](#fish)
+  - [🏗️ Initialize `ilab`](#️-initialize-ilab)
+    - [Example output](#example-output-1)
+    - [Example output](#example-output-2)
   - [📥 Download the model](#-download-the-model)
   - [🍴 Serving the model](#-serving-the-model)
   - [📣 Chat with the model (Optional)](#-chat-with-the-model-optional)
 - [💻 Creating new knowledge or skills and training the model](#-creating-new-knowledge-or-skills-and-training-the-model)
   - [🎁 Contribute knowledge or compositional skills](#-contribute-knowledge-or-compositional-skills)
   - [📜 List and validate your new data](#-list-and-validate-your-new-data)
   - [🚀 Generate a synthetic dataset](#-generate-a-synthetic-dataset)
+    - [Example output](#example-output-3)
   - [👩‍🏫 Train the model](#-train-the-model)
-  - [Test the newly trained model](#-test-the-newly-trained-model)
+    - [Train the model locally on Linux](#train-the-model-locally-on-linux)
+    - [Train the model locally on an M-series Mac](#train-the-model-locally-on-an-m-series-mac)
+    - [Training the model locally with GPU acceleration](#training-the-model-locally-with-gpu-acceleration)
+    - [Training the model in the cloud](#training-the-model-in-the-cloud)
+  - [📜 Test the newly trained model](#-test-the-newly-trained-model)
   - [🍴 Serve the newly trained model](#-serve-the-newly-trained-model)
-  - [📣 Chat with the new model (not optional this time)](#-chat-with-the-new-model-not-optional-this-time)
+- [📣 Chat with the new model (not optional this time)](#-chat-with-the-new-model-not-optional-this-time)
 - [🎁 Submit your new knowledge or skills](#-submit-your-new-knowledge-or-skills)
-- [📬 Contributing to Instruct-Lab CLI](#-contributing)
+- [📬 Contributing](#-contributing)
 
 ## Welcome to the InstructLab CLI
 
 InstructLab 🐶 uses a novel synthetic data-based alignment tuning method for
 Large Language Models (LLMs.) The "**lab**" in Instruct**Lab** 🐶 stands for
 [**L**arge-Scale **A**lignment for Chat**B**ots](https://arxiv.org/abs/2403.01081) [1].
 
 [1] Shivchander Sudalairaj*, Abhishek Bhandwaldar*, Aldo Pareja*, Kai Xu, David D. Cox, Akash Srivastava*. "LAB: Large-Scale Alignment for ChatBots", arXiv preprint arXiv: 2403.01081, 2024. (* denotes equal contributions)
 
 ## ❓ What is `ilab`
 
-`ilab` is a Command-Line Interface (CLI) tool that allows you to:
+`ilab` is a Command-Line Interface (CLI) tool that allows you to perform the following actions:
 
 1. Download a pre-trained Large Language Model (LLM).
 1. Chat with the LLM.
 
-To add new knowledge and skills to the pre-trained LLM you have to add new information to the companion [taxonomy](https://github.com/instructlab/taxonomy.git) repository.
-After that is done, you can:
+To add new knowledge and skills to the pre-trained LLM, add information to the companion [taxonomy](https://github.com/instructlab/taxonomy.git) repository.
+
+After you have added knowledge and skills to the taxonomy, you can perform the following actions:
 
 1. Use `ilab` to generate new synthetic training data based on the changes in your local `taxonomy` repository.
 1. Re-train the LLM with the new training data.
 1. Chat with the re-trained LLM to see the results.
 
-The full process is described graphically in the [workflow diagram](./docs/workflow.png).
+```mermaid
+graph TD;
+  download-->chat
+  chat[Chat with the LLM]-->add
+  add[Add new knowledge\nor skill to taxonomy]-->generate[generate new\nsynthetic training data]
+  generate-->train
+  train[Re-train]-->|Chat with\nthe re-trained LLM\nto see the results|chat
+```
+
+For an overview of the full workflow, see the [workflow diagram](./docs/workflow.png).
 
 > [!IMPORTANT]
-> It is important to understand that running InstructLab on a laptop will give you a low-fidelity approximation of both synthetic data generation (using the `ilab generate` command)
-> and model instruction tuning (using the `ilab train` command, which uses QLoRA.) The quality of the results you get using these tools on a laptop will not be as high-fidelity as they might be using
-> a larger teacher model and a different training method. We have optimized InstructLab to enable community members with modest hardware to be able to use the technique. If you have more sophisticated
-> hardware, you can configure InstructLab to use a larger teacher model [such as Mixtral](https://huggingface.co/docs/transformers/model_doc/mixtral) in order to achieve higher-fidelity results.
+> We have optimized InstructLab so that community members with commodity hardware can perform these steps. However, running InstructLab on a laptop will provide a low-fidelity approximation of synthetic data generation
+> (using the `ilab generate` command) and model instruction tuning (using the `ilab train` command, which uses QLoRA). To achieve higher quality, use more sophisticated hardware and configure InstructLab to use a
+> larger teacher model [such as Mixtral](https://huggingface.co/docs/transformers/model_doc/mixtral).
 
 ## 📋 Requirements
 
 - **🍎 Apple M1/M2/M3 Mac or 🐧 Linux system** (tested on Fedora). We anticipate support for more operating systems in the future.
 - C++ compiler
 - Python 3.9+ (<3.12 for PyTorch JIT)
 - Approximately 60GB disk space (entire process)
 
 > **NOTE:** PyTorch 2.2.1 does not support `torch.compile` with Python 3.12. On Fedora 39+, install `python3.11-devel` and create the virtual env with `python3.11` if you wish to use PyTorch's JIT compiler.
+<!-- -->
+> **NOTE:** When installing the `ilab` CLI on macOS, you may have to run the `xcode select --install` command to install the required packages previously listed.
 
 ## ✅ Getting started
 
 ### 🧰 Installing `ilab`
 
-1. If you are on Fedora Linux, install C++, Python 3.9+, and other necessary tools by running the following command:
+1. When installing on Fedora Linux, install C++, Python 3.9+, and other necessary tools by running the following command:
 
    ```shell
    sudo dnf install g++ gcc make pip python3 python3-devel python3-GitPython
    ```
 
    Optional: If `g++` is not found, try `gcc-c++` by running the following command:
 
-     ```shell
-     sudo dnf install gcc-c++ gcc make pip python3 python3-devel python3-GitPython
-     ```
+   ```shell
+   sudo dnf install gcc-c++ gcc make pip python3 python3-devel python3-GitPython
+   ```
+
+   If you are running on macOS, this installation is not necessary and you can begin your process with the following step.  
 
 2. Create a new directory called `instructlab` to store the files the `ilab` CLI needs when running and `cd` into the directory by running the following command:
 
    ```shell
    mkdir instructlab
    cd instructlab
    ```
 
    > **NOTE:** The following steps in this document use [Python venv](https://docs.python.org/3/library/venv.html) for virtual environments. However, if you use another tool such as [pyenv](https://github.com/pyenv/pyenv) or [Conda Miniforge](https://github.com/conda-forge/miniforge) for managing Python environments on your machine continue to use that tool instead. Otherwise, you may have issues with packages that are installed but not found in `venv`.
 
 3. Install and activate your `venv` environment by running the following command:
 
+   > **NOTE**: ⏳ `pip install` may take some time, depending on your internet connection. In case installation fails with error ``unsupported instruction `vpdpbusd'``, append `-C cmake.args="-DLLAMA_NATIVE=off"` to `pip install` command.
+
+   See [the GPU acceleration documentation](./docs/gpu-acceleration.md) for how to
+   to enable hardware acceleration for inference and training on AMD ROCm,
+   Apple Metal Performance Shaders (MPS), and Nvidia CUDA.
+
+   #### To install with no GPU acceleration and PyTorch without CUDA bindings
+
+   ```shell
+   python3 -m venv --upgrade-deps venv
+   source venv/bin/activate
+   (venv) $ pip cache remove llama_cpp_python
+   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable --extra-index-url=https://download.pytorch.org/whl/cpu
+   ```
+
+   #### To install with AMD ROCm
+
    ```shell
-   python3 -m venv venv
+   python3 -m venv --upgrade-deps venv
    source venv/bin/activate
-   pip install git+https://github.com/instructlab/instructlab.git@stable
+   (venv) $ pip cache remove llama_cpp_python
+   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable \
+       --extra-index-url https://download.pytorch.org/whl/rocm6.0 \
+       -C cmake.args="-DLLAMA_HIPBLAS=on" \
+       -C cmake.args="-DAMDGPU_TARGETS=all" \
+       -C cmake.args="-DCMAKE_C_COMPILER=/opt/rocm/llvm/bin/clang" \
+       -C cmake.args="-DCMAKE_CXX_COMPILER=/opt/rocm/llvm/bin/clang++" \
+       -C cmake.args="-DCMAKE_PREFIX_PATH=/opt/rocm"
    ```
 
-   > **NOTE**: ⏳ `pip install` may take some time, depending on your internet connection.
+   On Fedora 40+, use `-DCMAKE_C_COMPILER=clang-17` and `-DCMAKE_CXX_COMPILER=clang++-17`.
+
+   #### To install with Apple Metal on M1/M2/M3 Mac
+
+   ```shell
+   python3 -m venv --upgrade-deps venv
+   source venv/bin/activate
+   (venv) $ pip cache remove llama_cpp_python
+   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable -C cmake.args="-DLLAMA_METAL=on"
+   ```
+
+   #### To install with Nvidia CUDA
+
+   ```shell
+   python3 -m venv --upgrade-deps venv
+   source venv/bin/activate
+   (venv) $ pip cache remove llama_cpp_python
+   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable -C cmake.args="-DLLAMA_CUBLAS=on"
+   ```
 
 4. From your `venv` environment, verify `ilab` is installed correctly, by running the `ilab` command.
 
    ```shell
    ilab
    ```
 
@@ -192,14 +265,63 @@
 
    > **IMPORTANT:** every `ilab` command needs to be run from within your Python virtual environment. To enter the Python environment, run the following command:
 
    ```shell
    source venv/bin/activate
    ```
 
+5. You may optionally enable tab completion for the `ilab` command.
+
+   #### Bash (version 4.4 or newer)
+
+   Enable tab completion in `bash` with the following command:
+
+   ```sh
+   eval "$(_ILAB_COMPLETE=bash_source ilab)"
+   ```
+
+   To have this enabled automatically every time you open a new shell,
+   you can save the completion script and source it from `~/.bashrc`:
+
+   ```sh
+   _ILAB_COMPLETE=bash_source ilab > ~/.ilab-complete.bash
+   echo ". ~/.ilab-complete.bash" >> ~/.bashrc
+   ```
+
+   #### Zsh
+
+   Enable tab completion in `zsh` with the following command:
+
+   ```sh
+   eval "$(_ILAB_COMPLETE=zsh_source ilab)"
+   ```
+
+   To have this enabled automatically every time you open a new shell,
+   you can save the completion script and source it from `~/.zshrc`:
+
+   ```sh
+   _ILAB_COMPLETE=zsh_source ilab > ~/.ilab-complete.zsh
+   echo ". ~/.ilab-complete.zsh" >> ~/.zshrc
+   ```
+
+   #### Fish
+
+   Enable tab completion in `fish` with the following command:
+
+   ```sh
+   _ILAB_COMPLETE=fish_source ilab | source
+   ```
+
+   To have this enabled automatically every time you open a new shell,
+   you can save the completion script and source it from `~/.bashrc`:
+
+   ```sh
+   _ILAB_COMPLETE=fish_source ilab > ~/.config/fish/completions/ilab.fish
+   ```
+
 ### 🏗️ Initialize `ilab`
 
 1. Initialize `ilab` by running the following command:
 
    ```shell
    ilab init
    ```
@@ -224,15 +346,15 @@
    (venv) $ ilab init
    Welcome to InstructLab CLI. This guide will help you set up your environment.
    Please provide the following values to initiate the environment [press Enter for defaults]:
    Path to taxonomy repo [taxonomy]: <ENTER>
    `taxonomy` seems to not exists or is empty. Should I clone https://github.com/instructlab/taxonomy.git for you? [y/N]: y
    Cloning https://github.com/instructlab/taxonomy.git...
    Generating `config.yaml` in the current directory...
-   Initialization completed successfully, you're ready to start using `lab`. Enjoy!
+   Initialization completed successfully, you're ready to start using `ilab`. Enjoy!
    ```
 
    `ilab` will use the default configuration file unless otherwise specified. You can override this behavior with the `--config` parameter for any `ilab` command.
 
    The taxonomy repository uses [submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules) to incorporate the [taxonomy schema](https://github.com/instructlab/schema.git).
    When the `ilab init` command clones the taxonomy repository, it automatically handles the submodules.
    If you clone the taxonomy repository yourself, be sure to use the [`--recurse-submodules`](https://git-scm.com/docs/git-clone#Documentation/git-clone.txt---recurse-submodulesltpathspecgt) option on the `git clone` command and the `git pull` command when pulling updates from the remote repository.
@@ -308,15 +430,15 @@
 >>>                                                                                                                                                                                                                               [S][default]
 ```
 
 ## 💻 Creating new knowledge or skills and training the model
 
 ### 🎁 Contribute knowledge or compositional skills
 
-Contribute new knowledge or compositional skills to your local [taxonomy](https://github.com/instructlab/taxonomy.git) repository.
+1. Contribute new knowledge or compositional skills to your local [taxonomy](https://github.com/instructlab/taxonomy.git) repository.
 
 Detailed contribution instructions can be found in the [taxonomy repository](https://github.com/instructlab/taxonomy/blob/main/README.md).
 
 > [!IMPORTANT]
 > There is a limit to how much content can exist in the question/answer pairs for the model to process. Due to this, only add a maximum of around 2300 words to your question and answer seed example pairs in the `qna.yaml` file.
 
 ### 📜 List and validate your new data
@@ -333,14 +455,16 @@
    (venv) $ ilab diff
    compositional_skills/writing/freeform/foo-lang/foo-lang.yaml
    Taxonomy in /taxonomy/ is valid :)
    ```
 
 ### 🚀 Generate a synthetic dataset
 
+Before following these instructions, ensure the existing model you are adding skills or knowledge to is still running.
+
 1. To generate a synthetic dataset based on your newly added knowledge or skill set in [taxonomy](https://github.com/instructlab/taxonomy.git) repository, run the following command:
 
    ```shell
    ilab generate
    ```
 
    > **NOTE:** ⏳ This can take from 15 minutes to 1+ hours to complete, depending on your computing resources.
@@ -386,27 +510,23 @@
 
 #### Train the model locally on Linux
 
 ```shell
 ilab train
 ```
 
-> **NOTE:** ⏳ This step can potentially take **several hours** to complete depending on your computing resources.
+> **NOTE:** ⏳ This step can potentially take **several hours** to complete depending on your computing resources. Please stop `ilab chat` and `ilab serve` first to free resources.
 
 `ilab train` outputs a brand-new model that can be served in the `models` directory called `ggml-model-f16.gguf`.
 
 ```shell
  (venv) $ ls models
  ggml-merlinite-7b-lab-Q4_K_M.gguf  ggml-model-f16.gguf
 ```
 
-> **NOTE:** `ilab train` ships with experimental support for GPU acceleration with Nvidia CUDA
-or AMD ROCm. See [the GPU acceleration documentation](./docs/gpu-acceleration.md) for more
-details.
-
 #### Train the model locally on an M-series Mac
 
 To train the model locally on your M-Series Mac is as easy as running:
 
 ```shell
 ilab train
 ```
@@ -420,14 +540,22 @@
 (venv) $ ls instructlab-merlinite-7b-lab-mlx-q
 adapters-010.npz        adapters-050.npz        adapters-090.npz        config.json             tokenizer.model
 adapters-020.npz        adapters-060.npz        adapters-100.npz        model.safetensors       tokenizer_config.json
 adapters-030.npz        adapters-070.npz        adapters.npz            special_tokens_map.json
 adapters-040.npz        adapters-080.npz        added_tokens.json       tokenizer.jso
 ```
 
+#### Training the model locally with GPU acceleration
+
+Training has experimental support for GPU acceleration with Nvidia CUDA or AMD ROCm. Please see [the GPU acceleration documentation](./docs/gpu-acceleration.md) for more details. At present, hardware acceleration requires a data center GPU or high-end consumer GPU with at least 18 GB free memory.
+
+```shell
+ilab train --device=cuda
+```
+
 #### Training the model in the cloud
 
 Follow the instructions in [Training](./notebooks/README.md).
 
 ⏳ Approximate amount of time taken on each platform:
 
 - *Google Colab*: **5-10 minutes** with a T4 GPU
@@ -460,15 +588,15 @@
 
 2. Convert the newly trained model by running the following command:
 
    ```shell
    ilab convert
    ```
 
-3. Serve the newly trained model locally via `ilab serve` command with the `--model`
+3. Serve the newly trained model locally via `ilab serve` command with the `--model-path`
 argument to specify your new model:
 
    ```shell
    ilab serve --model-path <New model name>
    ```
 
    Which model should you select to serve? After running the `ilab convert` command, a few files and directories are generated. The one you will want to serve will end in `.gguf`
```

### Comparing `instructlab-0.14.0/src/instructlab.egg-info/SOURCES.txt` & `instructlab-0.15.1/src/instructlab.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,44 +14,52 @@
 Makefile
 README.md
 SECURITY.md
 TROUBLESHOOTING.md
 governance.md
 pyproject.toml
 requirements-dev.txt
+requirements-hpu.txt
 requirements.txt
 tox.ini
 .github/PULL_REQUEST_TEMPLATE.md
-.github/labeler.yml
+.github/actionlint.yaml
 .github/mergify.yml
+.github/ISSUE_TEMPLATE/bug_report.md
+.github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/actionlint.yml
 .github/workflows/docs.yml
-.github/workflows/label.yml
+.github/workflows/e2e.yml
+.github/workflows/image-cuda.yml
 .github/workflows/lint.yml
 .github/workflows/pypi.yaml
 .github/workflows/spellcheck.yaml
 .github/workflows/stale_bot.yml
 .github/workflows/test.yml
 .github/workflows/matchers/pylint.json
 CONTRIBUTING/CONTRIBUTING.md
 CONTRIBUTING/FIRST_TIME_CONTRIBUTORS.md
-MAINTAINERS/STABLE.md
 containers/sitecustomize.py
 containers/bin/debug-llama
 containers/bin/debug-pytorch
 containers/cuda/Containerfile
+containers/hpu/Containerfile
 containers/rocm/Containerfile
 containers/rocm/README.md
 containers/rocm/gfx-version.sh
 containers/rocm/remove-gfx.sh
 docs/README.md
+docs/STABLE.md
+docs/ci.md
 docs/containerization.md
 docs/converting_GGUF.md
 docs/demo-slides.md
 docs/gpu-acceleration.md
+docs/habana-gaudi.md
+docs/release-strategy.md
 docs/workflow.png
 docs/workflow.puml
 notebooks/README.md
 notebooks/Training_a_LoRA_With_Instruct_Lab.ipynb
 notebooks/images/collab-copy-path.png
 notebooks/images/collab-file-upload-button.png
 notebooks/images/collab-folder-icon.png
@@ -63,16 +71,18 @@
 notebooks/images/kaggle/import-nb.png
 notebooks/images/kaggle/input-drop-files.png
 notebooks/images/kaggle/input-upload.png
 notebooks/images/kaggle/input.png
 notebooks/images/kaggle/new-dataset.png
 notebooks/images/kaggle/select-accelerator-p100.png
 notebooks/images/kaggle/select-accelerator.png
+scripts/basic-workflow-tests.sh
 scripts/functional-tests.sh
 scripts/ruff.sh
+scripts/test-data/basic-workflow-fixture-qna.yaml
 src/instructlab/__init__.py
 src/instructlab/__main__.py
 src/instructlab/_version.py
 src/instructlab/client.py
 src/instructlab/common.py
 src/instructlab/config.py
 src/instructlab/lab.py
```

### Comparing `instructlab-0.14.0/src/instructlab.egg-info/requires.txt` & `instructlab-0.15.1/src/instructlab.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 click<9.0.0,>=8.1.7
 click-didyoumean<0.4.0,>=0.3.0
 datasets<3.0.0,>=2.18.0
 gguf<0.7.0,>=0.6.0
 GitPython<4.0.0,>=3.1.42
-httpx
+httpx<1.0.0,>=0.25.0
 jsonschema<5.0.0,>=4.21.1
-llama_cpp_python[server]==0.2.55
-numpy<2.0.0,>=1.26.4
+llama_cpp_python[server]==0.2.75
 openai<2.0.0,>=1.13.3
 peft<0.10.0,>=0.9.0
 prompt-toolkit<4.0.0,>=3.0.38
-pydantic
-pydantic_yaml
-PyYAML<7.0.0,>=6.0.1
+pydantic<3.0.0,>=2.6.0
+pydantic_yaml<2.0.0,>=1.2.0
+PyYAML<7.0.0,>=6.0.0
 rich<14.0.0,>=13.3.1
 rouge-score<0.2.0,>=0.1.2
 sentencepiece<0.3.0,>=0.2.0
 tokenizers<0.16.0,>=0.15.2
 toml<0.11.0,>=0.10.2
-torch<3.0.0,>=2.2.1
 tqdm<5.0.0,>=4.66.2
 transformers<=4.38.2,>=4.30.0
 trl<0.8.0,>=0.7.11
 wandb<0.17.0,>=0.16.4
 langchain-text-splitters
 yamllint<1.36.0,>=1.35.1
 
+[:python_version != "3.10"]
+numpy<2.0.0,>=1.26.4
+torch<3.0.0,>=2.2.1
+
+[:python_version == "3.10"]
+numpy<2.0.0,>=1.23.5
+torch<3.0.0,>=2.2.0a0
+
 [:sys_platform == "darwin" and platform_machine == "arm64"]
 mlx<0.6.0,>=0.5.1
```

### Comparing `instructlab-0.14.0/tests/conftest.py` & `instructlab-0.15.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/tests/taxonomy.py` & `instructlab-0.15.1/tests/taxonomy.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,40 +42,46 @@
         self._repo.index.commit("Initial commit")
 
     @property
     def untracked_files(self) -> List[str]:
         """List untracked files in the repository"""
         return self._repo.untracked_files
 
-    def create_untracked(self, rel_path: str, contents: Optional[bytes] = None) -> None:
+    def create_untracked(self, rel_path: str, contents: Optional[bytes] = None) -> Path:
         """Create a new untracked file in the repository.
 
         Args:
             rel_path (str): Relative path (from repository root) to the file.
             contents (bytes): (optional) Byte string to be written to the file.
+        Returns:
+            file_path: The path to the created file.
         """
         taxonomy_path = Path(rel_path)
         assert not taxonomy_path.is_absolute()
         file_path = self.root.joinpath(taxonomy_path)
         file_path.parent.mkdir(exist_ok=True, parents=True)
         if not contents:
             assert taxonomy_path.parts[0] == "compositional_skills"
             file_path.write_text(TEST_VALID_COMPOSITIONAL_SKILL_YAML, encoding="utf-8")
         else:
             file_path.write_bytes(contents)
+        return file_path
 
-    def add_tracked(self, rel_path: str) -> None:
+    def add_tracked(self, rel_path: str) -> Path:
         """Add a new tracked file to the repository (and commits it).
 
         Args:
             rel_path (str): Relative path (from repository root) to the file.
+        Returns:
+            file_path: The path to the added file.
         """
-        self.create_untracked(rel_path)
+        file_path = self.create_untracked(rel_path)
         self._repo.index.add([rel_path])
         self._repo.index.commit("new commit")
+        return file_path
 
     def remove_file(self, rel_path: str) -> None:
         """Remove a file in the repository (tracked or not)
 
         Args:
             rel_path (str): Relative path (from repository root) to the file.
         """
```

### Comparing `instructlab-0.14.0/tests/test_config.py` & `instructlab-0.15.1/tests/test_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,54 @@
 # SPDX-License-Identifier: Apache-2.0
 
-# Standard
-import unittest
-
 # Third Party
 import pytest
 
 # First Party
 from instructlab import config
 
 
-class TestConfig(unittest.TestCase):
+class TestConfig:
     @pytest.fixture(autouse=True)
     def _init_tmpdir(self, tmpdir):
         self.tmpdir = tmpdir
 
     def _assert_defaults(self, cfg):
-        self.assertIsNotNone(cfg.general)
-        self.assertEqual(cfg.general.log_level, "INFO")
+        assert cfg.general is not None
+        assert cfg.general.log_level == "INFO"
 
-        self.assertIsNotNone(cfg.chat)
-        self.assertEqual(cfg.chat.model, "merlinite-7b-lab-Q4_K_M")
-        self.assertFalse(cfg.chat.vi_mode)
-        self.assertTrue(cfg.chat.visible_overflow)
-        self.assertEqual(cfg.chat.context, "default")
-        self.assertIsNone(cfg.chat.session)
-        self.assertEqual(cfg.chat.logs_dir, "data/chatlogs")
-        self.assertFalse(cfg.chat.greedy_mode)
-
-        self.assertIsNotNone(cfg.generate)
-        self.assertEqual(cfg.generate.model, "merlinite-7b-lab-Q4_K_M")
-        self.assertEqual(cfg.generate.taxonomy_path, "taxonomy")
-        self.assertEqual(cfg.generate.taxonomy_base, "origin/main")
-        self.assertEqual(cfg.generate.num_cpus, 10)
-        self.assertEqual(cfg.generate.num_instructions, 100)
-        self.assertEqual(cfg.generate.chunk_word_count, 1000)
-        self.assertEqual(cfg.generate.output_dir, "generated")
-        self.assertEqual(cfg.generate.prompt_file, "prompt.txt")
-        self.assertEqual(cfg.generate.seed_file, "seed_tasks.json")
-
-        self.assertIsNotNone(cfg.serve)
-        self.assertEqual(cfg.serve.model_path, "models/merlinite-7b-lab-Q4_K_M.gguf")
-        self.assertEqual(cfg.serve.gpu_layers, -1)
-        self.assertEqual(cfg.serve.host_port, "127.0.0.1:8000")
-        self.assertEqual(cfg.serve.max_ctx_size, 4096)
+        assert cfg.chat is not None
+        assert cfg.chat.model == "merlinite-7b-lab-Q4_K_M"
+        assert not cfg.chat.vi_mode
+        assert cfg.chat.visible_overflow
+        assert cfg.chat.context == "default"
+        assert cfg.chat.session is None
+        assert cfg.chat.logs_dir == "data/chatlogs"
+        assert not cfg.chat.greedy_mode
+
+        assert cfg.generate is not None
+        assert cfg.generate.model == "merlinite-7b-lab-Q4_K_M"
+        assert cfg.generate.taxonomy_path == "taxonomy"
+        assert cfg.generate.taxonomy_base == "origin/main"
+        assert cfg.generate.num_cpus == 10
+        assert cfg.generate.num_instructions == 100
+        assert cfg.generate.chunk_word_count == 1000
+        assert cfg.generate.output_dir == "generated"
+        assert cfg.generate.prompt_file == "prompt.txt"
+        assert cfg.generate.seed_file == "seed_tasks.json"
+
+        assert cfg.serve is not None
+        assert cfg.serve.model_path == "models/merlinite-7b-lab-Q4_K_M.gguf"
+        assert cfg.serve.gpu_layers == -1
+        assert cfg.serve.host_port == "127.0.0.1:8000"
+        assert cfg.serve.max_ctx_size == 4096
 
     def test_default_config(self):
         cfg = config.get_default_config()
-        self.assertIsNotNone(cfg)
+        assert cfg is not None
         self._assert_defaults(cfg)
 
     def test_minimal_config(self):
         config_path = self.tmpdir.join("config.yaml")
         with open(config_path, "w", encoding="utf-8") as config_file:
             config_file.write(
                 """chat:
@@ -61,15 +58,15 @@
   taxonomy_base: origin/main
   taxonomy_path: taxonomy
 serve:
   model_path: models/merlinite-7b-lab-Q4_K_M.gguf
 """
             )
         cfg = config.read_config(config_path)
-        self.assertIsNotNone(cfg)
+        assert cfg is not None
         self._assert_defaults(cfg)
 
     def test_full_config(self):
         config_path = self.tmpdir.join("config.yaml")
         with open(config_path, "w", encoding="utf-8") as config_file:
             config_file.write(
                 """general:
@@ -96,15 +93,15 @@
   gpu_layers: -1
   host_port: 127.0.0.1:8000
   max_ctx_size: 4096
   model_path: models/merlinite-7b-lab-Q4_K_M.gguf
 """
             )
         cfg = config.read_config(config_path)
-        self.assertIsNotNone(cfg)
+        assert cfg is not None
         self._assert_defaults(cfg)
 
     def test_config_unexpected_fields(self):
         print(dir(self.tmpdir))
         config_path = self.tmpdir.join("config.yaml")
         with open(config_path, "w", encoding="utf-8") as config_file:
             config_file.write(
@@ -157,7 +154,23 @@
 - missing chat: field required
 - missing generate->taxonomy_path: field required
 - missing generate->taxonomy_base: field required
 - missing serve: field required
 """,
         ):
             config.read_config(config_path)
+
+    def test_validate_log_level_invalid(self):
+        cfg = config.get_default_config()
+        with pytest.raises(ValueError):
+            cfg.general.validate_log_level("INVALID")
+
+    def test_validate_log_level_valid(self):
+        cfg = config.get_default_config()
+        assert cfg.general.validate_log_level("DEBUG") == "DEBUG"
+        assert cfg.general.validate_log_level("INFO") == "INFO"
+        assert cfg.general.validate_log_level("WARNING") == "WARNING"
+        assert cfg.general.validate_log_level("WARN") == "WARN"
+        assert cfg.general.validate_log_level("FATAL") == "FATAL"
+        assert cfg.general.validate_log_level("CRITICAL") == "CRITICAL"
+        assert cfg.general.validate_log_level("ERROR") == "ERROR"
+        assert cfg.general.validate_log_level("NOTSET") == "NOTSET"
```

### Comparing `instructlab-0.14.0/tests/test_lab.py` & `instructlab-0.15.1/tests/test_lab.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 # SPDX-License-Identifier: Apache-2.0
 
 # Standard
 import re
-import unittest
 
 # Third Party
 import click
 import pytest
 
 # First Party
 from instructlab import lab
 from instructlab.utils import is_macos_with_m_chip
 
 
-class TestConfig(unittest.TestCase):
+class TestConfig:
     def test_cli_params_hyphenated(self):
         flag_pattern = re.compile("-{1,2}[0-9a-z-]+")
         invalid_flags = []
         for name, cmd in lab.cli.commands.items():
             for param in cmd.params:
                 if not isinstance(param, click.Option):
                     continue
                 for opt in param.opts:
                     if not flag_pattern.fullmatch(opt):
                         invalid_flags.append(f"{name} {opt}")
-        self.assertFalse(
-            invalid_flags, "<- these commands are using non-hyphenated params"
-        )
+        assert not invalid_flags, "<- these commands are using non-hyphenated params"
+
+
+def test_llamap_cpp_import():
+    # pylint: disable=import-outside-toplevel
+    # Third Party
+    import llama_cpp
+
+    llama_cpp.llama_backend_init()
 
 
 def test_import_mlx():
     # smoke test to verify that mlx is always available on Apple Silicon
     # but never on Linux and Intel macOS.
     if is_macos_with_m_chip():
         assert __import__("mlx")
```

### Comparing `instructlab-0.14.0/tests/test_lab_download.py` & `instructlab-0.15.1/tests/test_lab_download.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 # SPDX-License-Identifier: Apache-2.0
 
 # Standard
 from unittest.mock import MagicMock, patch
-import unittest
 
 # Third Party
 from click.testing import CliRunner
 from huggingface_hub.utils import HfHubHTTPError
 
 # First Party
 from instructlab import lab
 
 
-class TestLabDownload(unittest.TestCase):
+class TestLabDownload:
     # When using `from X import Y` you need to understand that Y becomes part
     # of your module, so you should use `my_module.Y`` to patch.
     # When using `import X`, you should use `X.Y` to patch.
     # https://docs.python.org/3/library/unittest.mock.html#where-to-patch?
     @patch("instructlab.lab.hf_hub_download")
     def test_download(self, mock_hf_hub_download):
         runner = CliRunner()
         with runner.isolated_filesystem():
-            result = runner.invoke(lab.download)
-            self.assertEqual(
-                result.exit_code, 0, "command finished with an unexpected exit code"
+            result = runner.invoke(
+                lab.cli,
+                [
+                    "--config=DEFAULT",
+                    "download",
+                ],
             )
+            assert (
+                result.exit_code == 0
+            ), "command finished with an unexpected exit code"
             mock_hf_hub_download.assert_called_once()
 
     @patch(
         "instructlab.lab.hf_hub_download",
         MagicMock(side_effect=HfHubHTTPError("Could not reach hugging face server")),
     )
     def test_download_error(self):
         runner = CliRunner()
         with runner.isolated_filesystem():
-            result = runner.invoke(lab.download)
-            self.assertEqual(
-                result.exit_code, 1, "command finished with an unexpected exit code"
+            result = runner.invoke(
+                lab.cli,
+                [
+                    "--config=DEFAULT",
+                    "download",
+                ],
             )
-            self.assertIn("Could not reach hugging face server", result.output)
+            assert (
+                result.exit_code == 1
+            ), "command finished with an unexpected exit code"
+            assert "Could not reach hugging face server" in result.output
```

### Comparing `instructlab-0.14.0/tests/test_lab_generate.py` & `instructlab-0.15.1/tests/test_lab_generate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,146 +1,146 @@
 # SPDX-License-Identifier: Apache-2.0
+# pylint: disable=duplicate-code
 
 # Standard
 from unittest.mock import patch
 import fnmatch
 import logging
 import os
 import pathlib
-import unittest
 
 # Third Party
 from click.testing import CliRunner
+import pytest
 
 # First Party
 from instructlab import lab
 from instructlab.generator.generate_data import generate_data
 from instructlab.generator.utils import GenerateException
 
 # Local
 from .taxonomy import MockTaxonomy
 from .testdata import testdata
 
 
-class TestLabGenerate(unittest.TestCase):
+class TestLabGenerate:
     """Test collection for `ilab generate` command."""
 
     @patch(
         "instructlab.generator.generate_data.generate_data",
         side_effect=GenerateException("Connection Error"),
     )
     def test_generate_exception_error(self, generate_data_mock):
         runner = CliRunner()
         with runner.isolated_filesystem():
             mt = MockTaxonomy(pathlib.Path("taxonomy"))
             result = runner.invoke(
-                lab.generate,
+                lab.cli,
                 [
+                    "--config=DEFAULT",
+                    "generate",
                     "--taxonomy-base",
                     "main",
                     "--taxonomy-path",
                     mt.root,
                     "--endpoint-url",
                     "localhost:8000",
                 ],
             )
-            self.assertEqual(
-                result.exit_code, 1, "command finished with an unexpected exit code"
-            )
+            assert (
+                result.exit_code == 1
+            ), "command finished with an unexpected exit code"
             generate_data_mock.assert_called_once()
-            self.assertIn(
-                "Generating dataset failed with the following error: Connection Error",
-                result.output,
+            assert (
+                "Generating dataset failed with the following error: Connection Error"
+                in result.output
             )
             mt.teardown()
 
     def test_taxonomy_not_found(self):
         runner = CliRunner()
         with runner.isolated_filesystem():
             result = runner.invoke(
-                lab.generate,
+                lab.cli,
                 [
+                    "--config=DEFAULT",
+                    "generate",
                     "--endpoint-url",
                     "localhost:8000",
                 ],
             )
-            self.assertEqual(
-                result.exit_code, 1, "command finished with an unexpected exit code"
-            )
-            self.assertIn(
-                "Error: taxonomy (taxonomy) does not exist",
-                result.output,
-            )
+            assert (
+                result.exit_code == 1
+            ), "command finished with an unexpected exit code"
+            assert "Error: taxonomy (taxonomy) does not exist" in result.output
 
     def test_no_new_data(self):
         runner = CliRunner()
         with runner.isolated_filesystem():
             mt = MockTaxonomy(pathlib.Path("taxonomy"))
             result = runner.invoke(
-                lab.generate,
+                lab.cli,
                 [
+                    "--config=DEFAULT",
+                    "generate",
                     "--taxonomy-base",
                     "main",
                     "--taxonomy-path",
                     mt.root,
                     "--endpoint-url",
                     "localhost:8000",
                 ],
             )
-            self.assertEqual(
-                result.exit_code, 1, "command finished with an unexpected exit code"
-            )
-            self.assertIn(
-                "Nothing to generate. Exiting.",
-                result.output,
-            )
+            assert (
+                result.exit_code == 1
+            ), "command finished with an unexpected exit code"
+            assert "Nothing to generate. Exiting." in result.output
             mt.teardown()
 
     def test_new_data_invalid_answer(self):
         runner = CliRunner()
         with open("tests/testdata/skill_invalid_answer.yaml", "rb") as qnafile:
             with runner.isolated_filesystem():
                 mt = MockTaxonomy(pathlib.Path("taxonomy"))
                 mt.create_untracked(
                     "compositional_skills/tracked/qna.yaml", qnafile.read()
                 )
                 result = runner.invoke(
-                    lab.generate,
+                    lab.cli,
                     [
+                        "--config=DEFAULT",
+                        "generate",
                         "--taxonomy-base",
                         "main",
                         "--taxonomy-path",
                         mt.root,
                         "--endpoint-url",
                         "localhost:8000",
                     ],
                 )
-                self.assertEqual(
-                    result.exit_code, 1, "command finished with an unexpected exit code"
-                )
-                self.assertIn(
-                    "taxonomy files with errors",
-                    result.output,
-                )
+                assert (
+                    result.exit_code == 1
+                ), "command finished with an unexpected exit code"
+                assert "taxonomy files with errors" in result.output
                 mt.teardown()
 
     @patch(
         "instructlab.generator.generate_data.get_instructions_from_model",
         side_effect=GenerateException(
             "There was a problem connecting to the OpenAI server."
         ),
     )
-    def test_OpenAI_server_error(self, get_instructions_from_model):
+    def test_open_ai_server_error(self, get_instructions_from_model):
         with open("tests/testdata/skill_valid_answer.yaml", "rb") as qnafile:
             with CliRunner().isolated_filesystem():
                 mt = MockTaxonomy(pathlib.Path("taxonomy"))
                 mt.create_untracked(
                     "compositional_skills/tracked/qna.yaml", qnafile.read()
                 )
-                with self.assertRaises(GenerateException) as exc:
+                with pytest.raises(GenerateException) as exc:
                     generate_data(
                         logger=logging.getLogger("test_logger"),
                         api_base="localhost:8000",
                         api_key="",
                         model_family="merlinite",
                         model_name="test-model",
                         num_cpus=10,
@@ -151,17 +151,16 @@
                         prompt_file_path="prompt.txt",
                         rouge_threshold=0.9,
                         console_output=True,
                         chunk_word_count=1000,
                         server_ctx_size=4096,
                         tls_insecure=False,
                     )
-                self.assertIn(
-                    "There was a problem connecting to the OpenAI server",
-                    f"{exc.exception}",
+                assert "There was a problem connecting to the OpenAI server" in str(
+                    exc.value
                 )
                 get_instructions_from_model.assert_called_once()
                 mt.teardown()
 
     @patch(
         "instructlab.generator.generate_data.get_instructions_from_model",
         return_value=(testdata.generate_data_return_value, 0),
@@ -194,16 +193,16 @@
                 get_instructions_from_model.assert_called_once()
                 expected_files = [
                     "generated_my-model*.json",
                     "train_my-model*.jsonl",
                     "test_my-model*.jsonl",
                 ]
                 for f in os.listdir("generated"):
-                    self.assertTrue(
-                        any(fnmatch.fnmatch(f, pattern) for pattern in expected_files)
+                    assert any(
+                        fnmatch.fnmatch(f, pattern) for pattern in expected_files
                     )
                 mt.teardown()
 
     @patch(
         "instructlab.generator.generate_data.get_instructions_from_model",
         return_value=(testdata.generate_data_return_value, 0),
     )
@@ -240,11 +239,11 @@
                 read_taxonomy.assert_called_once()
                 expected_files = [
                     "generated_my-model*.json",
                     "train_my-model*.jsonl",
                     "test_my-model*.jsonl",
                 ]
                 for f in os.listdir("generated"):
-                    self.assertTrue(
-                        any(fnmatch.fnmatch(f, pattern) for pattern in expected_files)
+                    assert any(
+                        fnmatch.fnmatch(f, pattern) for pattern in expected_files
                     )
                 mt.teardown()
```

### Comparing `instructlab-0.14.0/tests/test_lab_init.py` & `instructlab-0.15.1/tests/test_lab_init.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 # SPDX-License-Identifier: Apache-2.0
+# pylint: disable=duplicate-code
 
 # Standard
 from unittest.mock import MagicMock, patch
 import os
-import unittest
 
 # Third Party
 from click.testing import CliRunner
 from git import GitError
 
 # First Party
 from instructlab import lab
 from instructlab.config import read_config
 
 
-class TestLabInit(unittest.TestCase):
+class TestLabInit:
     # When using `from X import Y` you need to understand that Y becomes part
     # of your module, so you should use `my_module.Y`` to patch.
     # When using `import X`, you should use `X.Y` to patch.
     # https://docs.python.org/3/library/unittest.mock.html#where-to-patch?
     @patch("instructlab.lab.Repo.clone_from")
     def test_init_noninteractive(self, mock_clone_from):
         runner = CliRunner()
         with runner.isolated_filesystem():
-            result = runner.invoke(lab.init, args=["--non-interactive"])
-            self.assertEqual(result.exit_code, 0)
-            self.assertIn("config.yaml", os.listdir())
+            result = runner.invoke(lab.cli, ["init", "--non-interactive"])
+            assert result.exit_code == 0
+            assert "config.yaml" in os.listdir()
             mock_clone_from.assert_called_once()
 
     def test_init_interactive(self):
         runner = CliRunner()
         with runner.isolated_filesystem():
-            result = runner.invoke(lab.init, input="\nn")
-            self.assertEqual(result.exit_code, 0)
-            self.assertIn("config.yaml", os.listdir())
+            result = runner.invoke(lab.cli, ["init"], input="\nn")
+            assert result.exit_code == 0
+            assert "config.yaml" in os.listdir()
 
     @patch(
         "instructlab.lab.Repo.clone_from",
         MagicMock(side_effect=GitError("Authentication failed")),
     )
     def test_init_interactive_git_error(self):
         runner = CliRunner()
         with runner.isolated_filesystem():
-            result = runner.invoke(lab.init, input="\ny")
-            self.assertEqual(
-                result.exit_code, 1, "command finished with an unexpected exit code"
+            result = runner.invoke(lab.cli, ["init"], input="\ny")
+            assert (
+                result.exit_code == 1
+            ), "command finished with an unexpected exit code"
+            assert (
+                "Failed to clone taxonomy repo: Authentication failed" in result.output
             )
-            self.assertIn(
-                "Failed to clone taxonomy repo: Authentication failed", result.output
-            )
-            self.assertIn("manually run", result.output)
+            assert "manually run" in result.output
 
     @patch("instructlab.lab.Repo.clone_from")
     def test_init_interactive_clone(self, mock_clone_from):
         runner = CliRunner()
         with runner.isolated_filesystem():
-            result = runner.invoke(lab.init, input="\ny")
-            self.assertEqual(result.exit_code, 0)
-            self.assertIn("config.yaml", os.listdir())
+            result = runner.invoke(lab.cli, ["init"], input="\ny")
+            assert result.exit_code == 0
+            assert "config.yaml" in os.listdir()
             mock_clone_from.assert_called_once()
 
     def test_init_interactive_with_preexisting_nonempty_taxonomy(self):
         runner = CliRunner()
         with runner.isolated_filesystem():
             os.makedirs("taxonomy/contents")
-            result = runner.invoke(lab.init, input="\n")
-            self.assertEqual(result.exit_code, 0)
-            self.assertIn("config.yaml", os.listdir())
-            self.assertIn("taxonomy", os.listdir())
+            result = runner.invoke(lab.cli, ["init"], input="\n")
+            assert result.exit_code == 0
+            assert "config.yaml" in os.listdir()
+            assert "taxonomy" in os.listdir()
 
     def test_init_interactive_with_preexisting_config(self):
         runner = CliRunner()
         with runner.isolated_filesystem():
             # first run to prime the config.yaml in current directory
-            result = runner.invoke(lab.init, input="non-default-taxonomy\nn")
-            self.assertEqual(result.exit_code, 0)
-            self.assertIn("config.yaml", os.listdir())
+            result = runner.invoke(lab.cli, ["init"], input="non-default-taxonomy\nn")
+            assert result.exit_code == 0
+            assert "config.yaml" in os.listdir()
             config = read_config("config.yaml")
-            self.assertEqual(config.generate.taxonomy_path, "non-default-taxonomy")
+            assert config.generate.taxonomy_path == "non-default-taxonomy"
 
             # second invocation should ask if we want to overwrite - yes, and change taxonomy path
-            result = runner.invoke(lab.init, input="y\ndifferent-taxonomy\nn")
-            self.assertEqual(result.exit_code, 0)
-            self.assertIn("config.yaml", os.listdir())
+            result = runner.invoke(lab.cli, ["init"], input="y\ndifferent-taxonomy\nn")
+            assert result.exit_code == 0
+            assert "config.yaml" in os.listdir()
             config = read_config("config.yaml")
-            self.assertEqual(config.generate.taxonomy_path, "different-taxonomy")
+            assert config.generate.taxonomy_path == "different-taxonomy"
 
             # third invocation should again ask, but this time don't overwrite
-            result = runner.invoke(lab.init, input="n")
-            self.assertEqual(result.exit_code, 0)
-            self.assertIn("config.yaml", os.listdir())
+            result = runner.invoke(lab.cli, ["init"], input="n")
+            assert result.exit_code == 0
+            assert "config.yaml" in os.listdir()
             config = read_config("config.yaml")
-            self.assertEqual(config.generate.taxonomy_path, "different-taxonomy")
+            assert config.generate.taxonomy_path == "different-taxonomy"
```

### Comparing `instructlab-0.14.0/tests/test_lab_train.py` & `instructlab-0.15.1/tests/test_lab_train.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # SPDX-License-Identifier: Apache-2.0
 
 # Standard
 from unittest.mock import patch
 import os
 import platform
 import sys
-import unittest
 
 # Third Party
 from click.testing import CliRunner
 import pytest
 
 # First Party
 from instructlab import lab
@@ -60,15 +59,15 @@
 
 
 def is_arm_mac():
     return sys.platform == "darwin" and platform.machine() == "arm64"
 
 
 @pytest.mark.usefixtures("mock_mlx_package")
-class TestLabTrain(unittest.TestCase):
+class TestLabTrain:
     """Test collection for `ilab train` command."""
 
     @patch("instructlab.lab.utils.is_macos_with_m_chip", return_value=True)
     @patch("instructlab.mlx_explore.gguf_convert_to_mlx.load")
     @patch("instructlab.train.lora_mlx.make_data.make_data")
     @patch("instructlab.train.lora_mlx.convert.convert_between_mlx_and_pytorch")
     @patch("instructlab.train.lora_mlx.lora.load_and_train")
@@ -79,43 +78,42 @@
         make_data_mock,
         load_mock,
         is_macos_with_m_chip_mock,
     ):
         runner = CliRunner()
         with runner.isolated_filesystem():
             setup_input_dir()
-            result = runner.invoke(lab.train, ["--input-dir", INPUT_DIR])
-            self.assertEqual(result.exit_code, 0)
+            result = runner.invoke(
+                lab.cli, ["--config=DEFAULT", "train", "--input-dir", INPUT_DIR]
+            )
+            assert result.exit_code == 0
             load_mock.assert_not_called()
             load_and_train_mock.assert_called_once()
-            self.assertIsNotNone(load_and_train_mock.call_args[1]["model"])
-            self.assertTrue(load_and_train_mock.call_args[1]["train"])
-            self.assertEqual(
-                load_and_train_mock.call_args[1]["data"], "./taxonomy_data"
-            )
-            self.assertIsNotNone(load_and_train_mock.call_args[1]["adapter_file"])
-            self.assertEqual(load_and_train_mock.call_args[1]["iters"], 100)
-            self.assertEqual(load_and_train_mock.call_args[1]["save_every"], 10)
-            self.assertEqual(load_and_train_mock.call_args[1]["steps_per_eval"], 10)
-            self.assertEqual(len(load_and_train_mock.call_args[1]), 7)
+            assert load_and_train_mock.call_args[1]["model"] is not None
+            assert load_and_train_mock.call_args[1]["train"]
+            assert load_and_train_mock.call_args[1]["data"] == "./taxonomy_data"
+            assert load_and_train_mock.call_args[1]["adapter_file"] is not None
+            assert load_and_train_mock.call_args[1]["iters"] == 100
+            assert load_and_train_mock.call_args[1]["save_every"] == 10
+            assert load_and_train_mock.call_args[1]["steps_per_eval"] == 10
+            assert len(load_and_train_mock.call_args[1]) == 7
             convert_between_mlx_and_pytorch_mock.assert_called_once()
-            self.assertIsNotNone(
-                convert_between_mlx_and_pytorch_mock.call_args[1]["hf_path"]
+            assert (
+                convert_between_mlx_and_pytorch_mock.call_args[1]["hf_path"] is not None
             )
-            self.assertIsNotNone(
+            assert (
                 convert_between_mlx_and_pytorch_mock.call_args[1]["mlx_path"]
+                is not None
             )
-            self.assertTrue(
-                convert_between_mlx_and_pytorch_mock.call_args[1]["quantize"]
-            )
-            self.assertFalse(convert_between_mlx_and_pytorch_mock.call_args[1]["local"])
-            self.assertEqual(len(convert_between_mlx_and_pytorch_mock.call_args[1]), 4)
+            assert convert_between_mlx_and_pytorch_mock.call_args[1]["quantize"]
+            assert not convert_between_mlx_and_pytorch_mock.call_args[1]["local"]
+            assert len(convert_between_mlx_and_pytorch_mock.call_args[1]) == 4
             make_data_mock.assert_called_once()
-            self.assertEqual(make_data_mock.call_args[1]["data_dir"], "./taxonomy_data")
-            self.assertEqual(len(make_data_mock.call_args[1]), 1)
+            assert make_data_mock.call_args[1]["data_dir"] == "./taxonomy_data"
+            assert len(make_data_mock.call_args[1]) == 1
             is_macos_with_m_chip_mock.assert_called_once()
 
     @patch("instructlab.lab.utils.is_macos_with_m_chip", return_value=True)
     @patch("instructlab.mlx_explore.gguf_convert_to_mlx.load")
     @patch("instructlab.train.lora_mlx.make_data.make_data")
     @patch("instructlab.train.lora_mlx.convert.convert_between_mlx_and_pytorch")
     @patch("instructlab.train.lora_mlx.lora.load_and_train")
@@ -127,83 +125,104 @@
         load_mock,
         is_macos_with_m_chip_mock,
     ):
         runner = CliRunner()
         with runner.isolated_filesystem():
             setup_input_dir()
             result = runner.invoke(
-                lab.train, ["--input-dir", INPUT_DIR, "--skip-quantize"]
+                lab.cli,
+                [
+                    "--config=DEFAULT",
+                    "train",
+                    "--input-dir",
+                    INPUT_DIR,
+                    "--skip-quantize",
+                ],
             )
-            self.assertEqual(result.exit_code, 0)
+            assert result.exit_code == 0
             load_mock.assert_not_called()
             load_and_train_mock.assert_called_once()
             convert_between_mlx_and_pytorch_mock.assert_called_once()
-            self.assertEqual(
-                convert_between_mlx_and_pytorch_mock.call_args[1]["quantize"], False
+            assert (
+                convert_between_mlx_and_pytorch_mock.call_args[1]["quantize"] is False
             )
             make_data_mock.assert_called_once()
             is_macos_with_m_chip_mock.assert_called_once()
 
     def test_input_error(self):
         runner = CliRunner()
         with runner.isolated_filesystem():
-            result = runner.invoke(lab.train, ["--input-dir", "invalid"])
-            self.assertIsNotNone(result.exception)
-            self.assertIn("No such file or directory: 'invalid'", result.output)
-            self.assertEqual(result.exit_code, 1)
+            result = runner.invoke(
+                lab.cli, ["--config=DEFAULT", "train", "--input-dir", "invalid"]
+            )
+            assert result.exception is not None
+            assert "No such file or directory: 'invalid'" in result.output
+            assert result.exit_code == 1
 
     def test_invalid_taxonomy(self):
         runner = CliRunner()
         with runner.isolated_filesystem():
             os.mkdir(INPUT_DIR)  # Leave out the test and train files
-            result = runner.invoke(lab.train, ["--input-dir", INPUT_DIR])
-            self.assertIsNotNone(result.exception)
-            self.assertIn(
-                "Could not copy into data directory: list index out of range",
-                result.output,
+            result = runner.invoke(
+                lab.cli, ["--config=DEFAULT", "train", "--input-dir", INPUT_DIR]
             )
-            self.assertEqual(result.exit_code, 1)
+            assert result.exception is not None
+            assert (
+                f"{INPUT_DIR} does not contain training or test files, did you run `ilab generate`?"
+                in result.output
+            )
+            assert result.exit_code == 1
 
     def test_invalid_data_dir(self):
         # The error comes from make_data itself so it's only really useful to test on a mac
         if is_arm_mac():
             runner = CliRunner()
             with runner.isolated_filesystem():
                 os.mkdir(INPUT_DIR)  # Leave out the test and train files
                 result = runner.invoke(
-                    lab.train, ["--data-dir", "invalid", "--input-dir", INPUT_DIR]
-                )
-                self.assertIsNotNone(result.exception)
-                self.assertIn(
-                    "Could not read from data directory",
-                    result.output,
+                    lab.cli,
+                    [
+                        "--config=DEFAULT",
+                        "train",
+                        "--data-dir",
+                        "invalid",
+                        "--input-dir",
+                        INPUT_DIR,
+                    ],
                 )
-                self.assertEqual(result.exit_code, 1)
+                assert result.exception is not None
+                assert "Could not read from data directory" in result.output
+                assert result.exit_code == 1
 
     @patch("instructlab.lab.utils.is_macos_with_m_chip", return_value=True)
     @patch(
         "instructlab.train.lora_mlx.make_data.make_data",
         side_effect=FileNotFoundError(),
     )
     def test_invalid_data_dir_synthetic(
         self, make_data_mock, is_macos_with_m_chip_mock
     ):
         runner = CliRunner()
         with runner.isolated_filesystem():
             os.mkdir(INPUT_DIR)  # Leave out the test and train files
             result = runner.invoke(
-                lab.train, ["--data-dir", "invalid", "--input-dir", INPUT_DIR]
+                lab.cli,
+                [
+                    "--config=DEFAULT",
+                    "train",
+                    "--data-dir",
+                    "invalid",
+                    "--input-dir",
+                    INPUT_DIR,
+                ],
             )
             make_data_mock.assert_called_once()
-            self.assertIsNotNone(result.exception)
-            self.assertIn(
-                "Could not read from data directory",
-                result.output,
-            )
-            self.assertEqual(result.exit_code, 1)
+            assert result.exception is not None
+            assert "Could not read from data directory" in result.output
+            assert result.exit_code == 1
             is_macos_with_m_chip_mock.assert_called_once()
 
     @patch("instructlab.lab.utils.is_macos_with_m_chip", return_value=True)
     @patch("instructlab.mlx_explore.gguf_convert_to_mlx.load")
     @patch("instructlab.train.lora_mlx.make_data.make_data")
     @patch("instructlab.train.lora_mlx.convert.convert_between_mlx_and_pytorch")
     @patch("instructlab.train.lora_mlx.lora.load_and_train")
@@ -215,17 +234,24 @@
         load_mock,
         is_macos_with_m_chip_mock,
     ):
         runner = CliRunner()
         with runner.isolated_filesystem():
             setup_input_dir()
             result = runner.invoke(
-                lab.train, ["--input-dir", INPUT_DIR, "--skip-preprocessing"]
+                lab.cli,
+                [
+                    "--config=DEFAULT",
+                    "train",
+                    "--input-dir",
+                    INPUT_DIR,
+                    "--skip-preprocessing",
+                ],
             )
-            self.assertEqual(result.exit_code, 0)
+            assert result.exit_code == 0
             load_mock.assert_not_called()
             load_and_train_mock.assert_called_once()
             convert_between_mlx_and_pytorch_mock.assert_called_once()
             make_data_mock.assert_not_called()
             is_macos_with_m_chip_mock.assert_called_once()
 
     @patch("instructlab.lab.utils.is_macos_with_m_chip", return_value=True)
@@ -256,23 +282,23 @@
                     "tokenizer",
                     "--gguf-model-path",
                     "gguf_model",
                     "--model-dir",
                     MODEL_DIR,
                 ],
             )
-            self.assertEqual(result.exit_code, 0)
+            assert result.exit_code == 0
             load_mock.assert_called_once()
             load_and_train_mock.assert_called_once()
             convert_between_mlx_and_pytorch_mock.assert_not_called()
             make_data_mock.assert_called_once()
             fetch_tokenizer_from_hub_mock.assert_called_once()
-            self.assertEqual(fetch_tokenizer_from_hub_mock.call_args[0][0], "tokenizer")
-            self.assertEqual(fetch_tokenizer_from_hub_mock.call_args[0][1], "tokenizer")
-            self.assertEqual(len(fetch_tokenizer_from_hub_mock.call_args[0]), 2)
+            assert fetch_tokenizer_from_hub_mock.call_args[0][0] == "tokenizer"
+            assert fetch_tokenizer_from_hub_mock.call_args[0][1] == "tokenizer"
+            assert len(fetch_tokenizer_from_hub_mock.call_args[0]) == 2
             is_macos_with_m_chip_mock.assert_called_once()
 
     @patch("instructlab.lab.utils.is_macos_with_m_chip", return_value=True)
     @patch("instructlab.mlx_explore.utils.fetch_tokenizer_from_hub")
     @patch("instructlab.mlx_explore.gguf_convert_to_mlx.load")
     @patch("instructlab.train.lora_mlx.make_data.make_data")
     @patch("instructlab.train.lora_mlx.convert.convert_between_mlx_and_pytorch")
@@ -300,15 +326,15 @@
                     "--gguf-model-path",
                     "gguf_model",
                     "--model-dir",
                     MODEL_DIR,
                     "--local",
                 ],
             )
-            self.assertEqual(result.exit_code, 0)
+            assert result.exit_code == 0
             load_mock.assert_called_once()
             load_and_train_mock.assert_called_once()
             convert_between_mlx_and_pytorch_mock.assert_not_called()
             make_data_mock.assert_called_once()
             fetch_tokenizer_from_hub_mock.assert_not_called()
             is_macos_with_m_chip_mock.assert_called_once()
 
@@ -321,60 +347,78 @@
         linux_train_mock,
         is_macos_with_m_chip_mock,
     ):
         runner = CliRunner()
         with runner.isolated_filesystem():
             setup_input_dir()
             setup_linux_dir()
-            result = runner.invoke(lab.train, ["--input-dir", INPUT_DIR])
-            self.assertEqual(result.exit_code, 0)
+            result = runner.invoke(
+                lab.cli, ["--config=DEFAULT", "train", "--input-dir", INPUT_DIR]
+            )
+            assert result.exit_code == 0
             convert_llama_to_gguf_mock.assert_called_once()
-            self.assertEqual(
-                convert_llama_to_gguf_mock.call_args[1]["model"],
-                "./training_results/final",
+            assert (
+                convert_llama_to_gguf_mock.call_args[1]["model"]
+                == "./training_results/final"
             )
-            self.assertEqual(convert_llama_to_gguf_mock.call_args[1]["pad_vocab"], True)
-            self.assertEqual(len(convert_llama_to_gguf_mock.call_args[1]), 2)
+            assert convert_llama_to_gguf_mock.call_args[1]["pad_vocab"] is True
+            assert len(convert_llama_to_gguf_mock.call_args[1]) == 2
             linux_train_mock.assert_called_once()
             print(linux_train_mock.call_args[1])
-            self.assertEqual(
-                linux_train_mock.call_args[1]["train_file"],
-                "test_generated/train_1.jsonl",
-            )
-            self.assertEqual(
-                linux_train_mock.call_args[1]["test_file"],
-                "test_generated/test_1.jsonl",
-            )
-            self.assertEqual(linux_train_mock.call_args[1]["num_epochs"], 1)
-            self.assertIsNotNone(linux_train_mock.call_args[1]["device"])
-            self.assertFalse(linux_train_mock.call_args[1]["four_bit_quant"])
-            self.assertEqual(len(linux_train_mock.call_args[1]), 6)
+            assert (
+                linux_train_mock.call_args[1]["train_file"]
+                == "test_generated/train_1.jsonl"
+            )
+            assert (
+                linux_train_mock.call_args[1]["test_file"]
+                == "test_generated/test_1.jsonl"
+            )
+            assert linux_train_mock.call_args[1]["num_epochs"] == 1
+            assert linux_train_mock.call_args[1]["device"] is not None
+            assert not linux_train_mock.call_args[1]["four_bit_quant"]
+            assert len(linux_train_mock.call_args[1]) == 7
             is_macos_with_m_chip_mock.assert_called_once()
-            self.assertFalse(os.path.isfile(LINUX_GGUF_FILE))
+            assert not os.path.isfile(LINUX_GGUF_FILE)
 
     @patch("instructlab.lab.utils.is_macos_with_m_chip", return_value=False)
     @patch("instructlab.train.linux_train.linux_train")
     @patch("instructlab.llamacpp.llamacpp_convert_to_gguf.convert_llama_to_gguf")
     def test_num_epochs(
         self, convert_llama_to_gguf_mock, linux_train_mock, is_macos_with_m_chip_mock
     ):
         runner = CliRunner()
         with runner.isolated_filesystem():
             setup_input_dir()
             setup_linux_dir()
             result = runner.invoke(
-                lab.train, ["--input-dir", INPUT_DIR, "--num-epochs", "2"]
+                lab.cli,
+                [
+                    "--config=DEFAULT",
+                    "train",
+                    "--input-dir",
+                    INPUT_DIR,
+                    "--num-epochs",
+                    "2",
+                ],
             )
-            self.assertEqual(result.exit_code, 0)
+            assert result.exit_code == 0
             convert_llama_to_gguf_mock.assert_called_once()
             linux_train_mock.assert_called_once()
-            self.assertEqual(linux_train_mock.call_args[1]["num_epochs"], 2)
+            assert linux_train_mock.call_args[1]["num_epochs"] == 2
             is_macos_with_m_chip_mock.assert_called_once()
-            self.assertFalse(os.path.isfile(LINUX_GGUF_FILE))
+            assert not os.path.isfile(LINUX_GGUF_FILE)
 
             # Test with invalid num_epochs
             result = runner.invoke(
-                lab.train, ["--input-dir", INPUT_DIR, "--num-epochs", "two"]
+                lab.cli,
+                [
+                    "--config=DEFAULT",
+                    "train",
+                    "--input-dir",
+                    INPUT_DIR,
+                    "--num-epochs",
+                    "two",
+                ],
             )
-            self.assertIsNotNone(result.exception)
-            self.assertEqual(result.exit_code, 2)
-            self.assertIn("'two' is not a valid integer", result.output)
+            assert result.exception is not None
+            assert result.exit_code == 2
+            assert "'two' is not a valid integer" in result.output
```

### Comparing `instructlab-0.14.0/tests/test_notebooks.py` & `instructlab-0.15.1/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/tests/testdata/invalid_yaml.yaml` & `instructlab-0.15.1/tests/testdata/invalid_yaml.yaml`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/tests/testdata/knowledge_valid.yaml` & `instructlab-0.15.1/tests/testdata/knowledge_valid.yaml`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/tests/testdata/temp_repo/docs/skill-wiki.md` & `instructlab-0.15.1/tests/testdata/temp_repo/docs/skill-wiki.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/tests/testdata/temp_repo/knowledge-wiki.md` & `instructlab-0.15.1/tests/testdata/temp_repo/knowledge-wiki.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.14.0/tests/testdata/testdata.py` & `instructlab-0.15.1/tests/testdata/testdata.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,27 @@
       While there is wide agreement among philosophers that propositional knowledge is a form of true belief, 
       many controversies focus on justification. This includes questions like how to understand justification, 
       whether it is needed at all, and whether something else besides it is needed. 
       These controversies intensified in the latter half of the 20th century due to a series of thought experiments 
       called Gettier cases that provoked alternative definitions."""
 ]
 
+long_line_documents = [
+    (
+        "Knowledge is an awareness of facts, a familiarity with individuals and situations,"
+        "or a practical skill. Knowledge of facts, also called propositional knowledge, is often characterized "
+        "as true belief that is distinct from opinion or guesswork by virtue of justification. "
+        "While there is wide agreement among philosophers that propositional knowledge is a form of true belief, "
+        "many controversies focus on justification. This includes questions like how to understand justification, "
+        "whether it is needed at all, and whether something else besides it is needed. "
+        "These controversies intensified in the latter half of the 20th century due to a series of thought experiments "
+        "called Gettier cases that provoked alternative definitions."
+    )
+]
+
 knowledge_seed_instruction = [
     {
         "instruction": "What is this knowledge about?",
         "input": "",
         "output": "It's a knowledge that makes the tests more knowledgeable",
         "taxonomy_path": "knowledge->textbook->puns-copy->general",
         "task_description": "For knowledge tests",
```

### Comparing `instructlab-0.14.0/tox.ini` & `instructlab-0.15.1/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -28,24 +28,25 @@
 # speed up testing.
 [testenv:lint]
 description = lint with pylint
 skip_install = true
 skipsdist = true
 deps = -r requirements-dev.txt
 commands =
-    {envpython} -m pylint src/instructlab/ tests/
+    {envpython} -m pylint --load-plugins pylint_pydantic src/instructlab/ tests/
 
 [testenv:fastlint]
 description = fast lint with pylint (without 3rd party modules)
 skip_install = true
 skipsdist = true
 deps =
     pylint
+    pylint-pydantic
 commands =
-    {envpython} -m pylint {posargs:--disable=import-error src/instructlab/ tests/}
+    {envpython} -m pylint --load-plugins pylint_pydantic {posargs:--disable=import-error src/instructlab/ tests/}
 
 [testenv:ruff]
 description = reformat and fix code with Ruff (and isort)
 skip_install = True
 skipsdist = true
 # keep in sync with .pre-commit-config.yaml
 deps =
@@ -63,13 +64,22 @@
 deps =
     pyspelling
 commands =
     sh -c 'command -v aspell || (echo "aspell is not installed. Please install it." && exit 1)'
     {envpython} -m pyspelling --config {toxinidir}/.spellcheck.yml --spellchecker aspell
 allowlist_externals = sh
 
+[testenv:docs]
+description = docs
+deps =
+    # TODO: switch to a release tag when it's cut
+    # We need https://github.com/click-contrib/click-man/pull/62 to handle hidden options
+    git+https://github.com/click-contrib/click-man@24ec8377e3c24378417f6fc4f571b4f585d7df6b
+commands =
+    click-man --target {toxinidir}/man ilab
+
 [gh]
 python =
     3.12 = py312-{unitcov, functional}
     3.11 = py311-{unitcov, functional}
     3.10 = py310-{unitcov, functional}
     3.9 = py39-{unitcov, functional}
```

