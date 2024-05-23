# Comparing `tmp/docker-7.0.0b2.tar.gz` & `tmp/docker-7.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-7.0.0b2.tar", last modified: Mon Nov 27 21:26:36 2023, max compression
+gzip compressed data, was "docker-7.0.0b3.tar", last modified: Tue Dec  5 18:42:03 2023, max compression
```

## Comparing `docker-7.0.0b2.tar` & `docker-7.0.0b3.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.059630 docker-7.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-27 21:26:31.000000 docker-7.0.0b2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-11-27 21:26:31.000000 docker-7.0.0b2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-11-27 21:26:31.000000 docker-7.0.0b2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.019630 docker-7.0.0b2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.027630 docker-7.0.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2023-11-27 21:26:31.000000 docker-7.0.0b2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-11-27 21:26:31.000000 docker-7.0.0b2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-11-27 21:26:31.000000 docker-7.0.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-11-27 21:26:31.000000 docker-7.0.0b2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2023-11-27 21:26:31.000000 docker-7.0.0b2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-11-27 21:26:31.000000 docker-7.0.0b2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-11-27 21:26:31.000000 docker-7.0.0b2/Dockerfile-docs
--rw-r--r--   0 runner    (1001) docker     (127)    10758 2023-11-27 21:26:31.000000 docker-7.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2023-11-27 21:26:31.000000 docker-7.0.0b2/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-11-27 21:26:31.000000 docker-7.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2023-11-27 21:26:31.000000 docker-7.0.0b2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-11-27 21:26:36.059630 docker-7.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2023-11-27 21:26:31.000000 docker-7.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.027630 docker-7.0.0b2/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-11-27 21:26:35.000000 docker-7.0.0b2/docker/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.031630 docker-7.0.0b2/docker/api/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14587 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    19472 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    52896 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/exec_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20255 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    19215 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    18116 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/swarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/api/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    12990 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.031630 docker-7.0.0b2/docker/context/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/context/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/context/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.035630 docker-7.0.0b2/docker/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/credentials/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/credentials/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/credentials/store.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/credentials/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.035630 docker-7.0.0b2/docker/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/models/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    46729 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/models/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17999 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/models/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/models/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/models/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/models/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/models/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     8289 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/models/swarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/models/volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/tls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.035630 docker-7.0.0b2/docker/transport/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/transport/basehttpadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/transport/npipeconn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/transport/npipesocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/transport/sshconn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/transport/unixconn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.039630 docker-7.0.0b2/docker/types/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    27380 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/types/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/types/daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/types/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/types/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    33135 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/types/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/types/swarm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.039630 docker-7.0.0b2/docker/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8033 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/utils/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/utils/fnmatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/utils/json_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/utils/ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/utils/socket.py
--rw-r--r--   0 runner    (1001) docker     (127)    13801 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-11-27 21:26:31.000000 docker-7.0.0b2/docker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.055630 docker-7.0.0b2/docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-11-27 21:26:35.000000 docker-7.0.0b2/docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2023-11-27 21:26:36.000000 docker-7.0.0b2/docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 21:26:35.000000 docker-7.0.0b2/docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 21:26:35.000000 docker-7.0.0b2/docker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-11-27 21:26:35.000000 docker-7.0.0b2/docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-27 21:26:35.000000 docker-7.0.0b2/docker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.043630 docker-7.0.0b2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.043630 docker-7.0.0b2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.043630 docker-7.0.0b2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)    77557 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/change-log.md
--rw-r--r--   0 runner    (1001) docker     (127)      920 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/client.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/containers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/favicon_whale.png
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/images.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/networks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/nodes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/secrets.rst
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/services.rst
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/swarm.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/tls.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.043630 docker-7.0.0b2/docs/user_guides/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/user_guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/user_guides/multiplex.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/user_guides/swarm_services.md
--rw-r--r--   0 runner    (1001) docker     (127)      559 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs/volumes.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-27 21:26:31.000000 docker-7.0.0b2/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-11-27 21:26:31.000000 docker-7.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-11-27 21:26:31.000000 docker-7.0.0b2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-11-27 21:26:31.000000 docker-7.0.0b2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.043630 docker-7.0.0b2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      938 2023-11-27 21:26:31.000000 docker-7.0.0b2/scripts/release.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2186 2023-11-27 21:26:31.000000 docker-7.0.0b2/scripts/versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-11-27 21:26:36.059630 docker-7.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2023-11-27 21:26:31.000000 docker-7.0.0b2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-27 21:26:31.000000 docker-7.0.0b2/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.043630 docker-7.0.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/Dockerfile-dind-certs
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/Dockerfile-ssh-dind
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.043630 docker-7.0.0b2/tests/gpg-keys/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/gpg-keys/ownertrust
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/gpg-keys/secret
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.047630 docker-7.0.0b2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20159 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/api_build_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/api_client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/api_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    57865 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/api_container_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11874 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/api_exec_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/api_healthcheck_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12851 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/api_image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18806 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/api_network_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/api_plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/api_secret_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    62334 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/api_service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9622 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/api_swarm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/api_volume_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/context_api_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.047630 docker-7.0.0b2/tests/integration/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/credentials/create_gpg_key.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/credentials/store_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/credentials/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21026 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/models_containers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5806 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/models_images_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/models_networks_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/models_nodes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/models_resources_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13199 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/models_services_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/models_swarm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/models_volumes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/regression_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.023630 docker-7.0.0b2/tests/integration/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.047630 docker-7.0.0b2/tests/integration/testdata/dummy-plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/testdata/dummy-plugin/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.023630 docker-7.0.0b2/tests/integration/testdata/dummy-plugin/rootfs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.051630 docker-7.0.0b2/tests/integration/testdata/dummy-plugin/rootfs/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/integration/testdata/dummy-plugin/rootfs/dummy/file.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.051630 docker-7.0.0b2/tests/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19711 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/ssh/api_build_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/ssh/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.023630 docker-7.0.0b2/tests/ssh/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.051630 docker-7.0.0b2/tests/ssh/config/client/
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/ssh/config/client/id_rsa
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/ssh/config/client/id_rsa.pub
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.051630 docker-7.0.0b2/tests/ssh/config/server/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/ssh/config/server/known_ed25519
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/ssh/config/server/known_ed25519.pub
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/ssh/config/server/sshd_config
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/ssh/config/server/unknown_ed25519
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/ssh/config/server/unknown_ed25519.pub
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/ssh/connect_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.055630 docker-7.0.0b2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/api_build_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    59084 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/api_container_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/api_exec_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10969 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/api_image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/api_network_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21738 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/api_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/api_volume_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28247 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9812 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/context_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18285 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/dockertypes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17448 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/fake_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/fake_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/fake_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)    29177 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/models_containers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/models_images_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/models_networks_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/models_resources_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/models_secrets_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/models_services_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/sshadapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/swarm_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.023630 docker-7.0.0b2/tests/unit/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:36.055630 docker-7.0.0b2/tests/unit/testdata/certs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/testdata/certs/ca.pem
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/testdata/certs/cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/testdata/certs/key.pem
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/types_containers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16046 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/utils_build_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/utils_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/utils_json_stream_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/utils_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23036 2023-11-27 21:26:31.000000 docker-7.0.0b2/tests/unit/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2023-11-27 21:26:31.000000 docker-7.0.0b2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.250119 docker-7.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-05 18:41:56.000000 docker-7.0.0b3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-05 18:41:56.000000 docker-7.0.0b3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-05 18:41:56.000000 docker-7.0.0b3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.210119 docker-7.0.0b3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.218119 docker-7.0.0b3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2023-12-05 18:41:56.000000 docker-7.0.0b3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-12-05 18:41:56.000000 docker-7.0.0b3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2023-12-05 18:41:56.000000 docker-7.0.0b3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2023-12-05 18:41:56.000000 docker-7.0.0b3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2023-12-05 18:41:56.000000 docker-7.0.0b3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2023-12-05 18:41:56.000000 docker-7.0.0b3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2023-12-05 18:41:56.000000 docker-7.0.0b3/Dockerfile-docs
+-rw-r--r--   0 runner    (1001) docker     (127)    10758 2023-12-05 18:41:56.000000 docker-7.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2023-12-05 18:41:56.000000 docker-7.0.0b3/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2023-12-05 18:41:56.000000 docker-7.0.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2023-12-05 18:41:56.000000 docker-7.0.0b3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-12-05 18:42:03.250119 docker-7.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2023-12-05 18:41:56.000000 docker-7.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.218119 docker-7.0.0b3/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2023-12-05 18:42:03.000000 docker-7.0.0b3/docker/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.222119 docker-7.0.0b3/docker/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16106 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19472 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52896 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/exec_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20255 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19215 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18116 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/swarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/api/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12990 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.222119 docker-7.0.0b3/docker/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/context/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.226119 docker-7.0.0b3/docker/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/credentials/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/credentials/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/credentials/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/credentials/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.226119 docker-7.0.0b3/docker/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/models/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46729 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/models/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17999 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/models/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/models/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/models/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/models/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/models/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/models/swarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/models/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/tls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.226119 docker-7.0.0b3/docker/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/transport/basehttpadapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/transport/npipeconn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/transport/npipesocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/transport/sshconn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/transport/unixconn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.230119 docker-7.0.0b3/docker/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27380 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/types/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/types/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/types/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/types/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33135 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/types/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/types/swarm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.230119 docker-7.0.0b3/docker/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/utils/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/utils/fnmatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/utils/json_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/utils/ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/utils/socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13801 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2023-12-05 18:41:56.000000 docker-7.0.0b3/docker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.246119 docker-7.0.0b3/docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-12-05 18:42:03.000000 docker-7.0.0b3/docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2023-12-05 18:42:03.000000 docker-7.0.0b3/docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 18:42:03.000000 docker-7.0.0b3/docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 18:42:03.000000 docker-7.0.0b3/docker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-05 18:42:03.000000 docker-7.0.0b3/docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-05 18:42:03.000000 docker-7.0.0b3/docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.234119 docker-7.0.0b3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.234119 docker-7.0.0b3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.234119 docker-7.0.0b3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    77557 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/change-log.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/favicon_whale.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/images.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/secrets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/services.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/swarm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/tls.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.234119 docker-7.0.0b3/docs/user_guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/user_guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/user_guides/multiplex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/user_guides/swarm_services.md
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs/volumes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-05 18:41:56.000000 docker-7.0.0b3/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2023-12-05 18:41:56.000000 docker-7.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-05 18:41:56.000000 docker-7.0.0b3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-05 18:41:56.000000 docker-7.0.0b3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.234119 docker-7.0.0b3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      938 2023-12-05 18:41:56.000000 docker-7.0.0b3/scripts/release.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2186 2023-12-05 18:41:56.000000 docker-7.0.0b3/scripts/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-05 18:42:03.250119 docker-7.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2023-12-05 18:41:56.000000 docker-7.0.0b3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-05 18:41:56.000000 docker-7.0.0b3/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.234119 docker-7.0.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/Dockerfile-dind-certs
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/Dockerfile-ssh-dind
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.234119 docker-7.0.0b3/tests/gpg-keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/gpg-keys/ownertrust
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/gpg-keys/secret
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.238119 docker-7.0.0b3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20159 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/api_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/api_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/api_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57865 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/api_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11874 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/api_exec_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/api_healthcheck_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12851 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/api_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18806 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/api_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/api_plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/api_secret_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62334 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/api_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9622 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/api_swarm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/api_volume_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/context_api_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.238119 docker-7.0.0b3/tests/integration/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/credentials/create_gpg_key.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/credentials/store_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/credentials/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21026 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/models_containers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/models_images_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/models_networks_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/models_nodes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/models_resources_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13199 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/models_services_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/models_swarm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/models_volumes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/regression_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.214119 docker-7.0.0b3/tests/integration/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.242119 docker-7.0.0b3/tests/integration/testdata/dummy-plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/testdata/dummy-plugin/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.214119 docker-7.0.0b3/tests/integration/testdata/dummy-plugin/rootfs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.242119 docker-7.0.0b3/tests/integration/testdata/dummy-plugin/rootfs/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/integration/testdata/dummy-plugin/rootfs/dummy/file.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.242119 docker-7.0.0b3/tests/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19711 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/ssh/api_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/ssh/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.214119 docker-7.0.0b3/tests/ssh/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.242119 docker-7.0.0b3/tests/ssh/config/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/ssh/config/client/id_rsa
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/ssh/config/client/id_rsa.pub
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.242119 docker-7.0.0b3/tests/ssh/config/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/ssh/config/server/known_ed25519
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/ssh/config/server/known_ed25519.pub
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/ssh/config/server/sshd_config
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/ssh/config/server/unknown_ed25519
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/ssh/config/server/unknown_ed25519.pub
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/ssh/connect_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.246119 docker-7.0.0b3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/api_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59084 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/api_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/api_exec_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10969 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/api_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/api_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21738 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/api_volume_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28247 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9812 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/context_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18285 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/dockertypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17448 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/fake_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/fake_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/fake_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29177 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/models_containers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/models_images_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/models_networks_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/models_resources_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/models_secrets_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/models_services_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/sshadapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/swarm_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.214119 docker-7.0.0b3/tests/unit/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:42:03.246119 docker-7.0.0b3/tests/unit/testdata/certs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/testdata/certs/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/testdata/certs/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/testdata/certs/key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/types_containers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16046 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/utils_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/utils_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/utils_json_stream_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/utils_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23036 2023-12-05 18:41:56.000000 docker-7.0.0b3/tests/unit/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2023-12-05 18:41:56.000000 docker-7.0.0b3/tox.ini
```

### Comparing `docker-7.0.0b2/.github/workflows/ci.yml` & `docker-7.0.0b3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/.github/workflows/release.yml` & `docker-7.0.0b3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/CONTRIBUTING.md` & `docker-7.0.0b3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/LICENSE` & `docker-7.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/MAINTAINERS` & `docker-7.0.0b3/MAINTAINERS`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/Makefile` & `docker-7.0.0b3/Makefile`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/PKG-INFO` & `docker-7.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker
-Version: 7.0.0b2
+Version: 7.0.0b3
 Summary: A Python library for the Docker Engine API.
 Home-page: https://github.com/docker/docker-py
 Maintainer: Ulysses Souza
 Maintainer-email: ulysses.souza@docker.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docker-py.readthedocs.io
 Project-URL: Changelog, https://docker-py.readthedocs.io/en/stable/change-log.html
```

### Comparing `docker-7.0.0b2/README.md` & `docker-7.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/api/build.py` & `docker-7.0.0b3/docker/api/build.py`

 * *Files 8% similar despite different names*

```diff
@@ -125,21 +125,24 @@
         buildargs = buildargs or {}
         if path is None and fileobj is None:
             raise TypeError("Either path or fileobj needs to be provided.")
         if gzip and encoding is not None:
             raise errors.DockerException(
                 'Can not use custom encoding if gzip is enabled'
             )
-
+        if tag is not None:
+            if not utils.match_tag(tag):
+                raise errors.DockerException(
+                    f"invalid tag '{tag}': invalid reference format"
+            )
         for key in container_limits.keys():
             if key not in constants.CONTAINER_LIMITS_KEYS:
                 raise errors.DockerException(
-                    f'Invalid container_limits key {key}'
+                    f"invalid tag '{tag}': invalid reference format"
                 )
-
         if custom_context:
             if not fileobj:
                 raise TypeError("You must specify fileobj with custom_context")
             context = fileobj
         elif fileobj is not None:
             context = utils.mkbuildcontext(fileobj)
         elif path.startswith(('http://', 'https://',
@@ -272,29 +275,56 @@
 
         if context is not None and not custom_context:
             context.close()
 
         return self._stream_helper(response, decode=decode)
 
     @utils.minimum_version('1.31')
-    def prune_builds(self):
+    def prune_builds(self, filters=None, keep_storage=None, all=None):
         """
         Delete the builder cache
 
+        Args:
+            filters (dict): Filters to process on the prune list.
+                Needs Docker API v1.39+
+                Available filters:
+                - dangling (bool):  When set to true (or 1), prune only
+                unused and untagged images.
+                - until (str): Can be Unix timestamps, date formatted
+                timestamps, or Go duration strings (e.g. 10m, 1h30m) computed
+                relative to the daemon's local time.
+            keep_storage (int): Amount of disk space in bytes to keep for cache.
+                Needs Docker API v1.39+
+            all (bool): Remove all types of build cache.
+                Needs Docker API v1.39+
+
         Returns:
             (dict): A dictionary containing information about the operation's
                     result. The ``SpaceReclaimed`` key indicates the amount of
                     bytes of disk space reclaimed.
 
         Raises:
             :py:class:`docker.errors.APIError`
                 If the server returns an error.
         """
         url = self._url("/build/prune")
-        return self._result(self._post(url), True)
+        if (filters, keep_storage, all) != (None, None, None) \
+                and utils.version_lt(self._version, '1.39'):
+            raise errors.InvalidVersion(
+                '`filters`, `keep_storage`, and `all` args are only available '
+                'for API version > 1.38'
+            )
+        params = {}
+        if filters is not None:
+            params['filters'] = utils.convert_filters(filters)
+        if keep_storage is not None:
+            params['keep-storage'] = keep_storage
+        if all is not None:
+            params['all'] = all
+        return self._result(self._post(url, params=params), True)
 
     def _set_auth_headers(self, headers):
         log.debug('Looking for auth config')
 
         # If we don't have any auth data so far, try reloading the config
         # file one more time in case anything showed up in there.
         if not self._auth_configs or self._auth_configs.is_empty:
```

### Comparing `docker-7.0.0b2/docker/api/client.py` & `docker-7.0.0b3/docker/api/client.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/api/config.py` & `docker-7.0.0b3/docker/api/config.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/api/container.py` & `docker-7.0.0b3/docker/api/container.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/api/daemon.py` & `docker-7.0.0b3/docker/api/daemon.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/api/exec_api.py` & `docker-7.0.0b3/docker/api/exec_api.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/api/image.py` & `docker-7.0.0b3/docker/api/image.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/api/network.py` & `docker-7.0.0b3/docker/api/network.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/api/plugin.py` & `docker-7.0.0b3/docker/api/plugin.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/api/secret.py` & `docker-7.0.0b3/docker/api/secret.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/api/service.py` & `docker-7.0.0b3/docker/api/service.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/api/swarm.py` & `docker-7.0.0b3/docker/api/swarm.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/api/volume.py` & `docker-7.0.0b3/docker/api/volume.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/auth.py` & `docker-7.0.0b3/docker/auth.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/client.py` & `docker-7.0.0b3/docker/client.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/constants.py` & `docker-7.0.0b3/docker/constants.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/context/api.py` & `docker-7.0.0b3/docker/context/api.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/context/config.py` & `docker-7.0.0b3/docker/context/config.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/context/context.py` & `docker-7.0.0b3/docker/context/context.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/credentials/store.py` & `docker-7.0.0b3/docker/credentials/store.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/errors.py` & `docker-7.0.0b3/docker/errors.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/models/configs.py` & `docker-7.0.0b3/docker/models/configs.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/models/containers.py` & `docker-7.0.0b3/docker/models/containers.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/models/images.py` & `docker-7.0.0b3/docker/models/images.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/models/networks.py` & `docker-7.0.0b3/docker/models/networks.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/models/nodes.py` & `docker-7.0.0b3/docker/models/nodes.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/models/plugins.py` & `docker-7.0.0b3/docker/models/plugins.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/models/resource.py` & `docker-7.0.0b3/docker/models/resource.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/models/secrets.py` & `docker-7.0.0b3/docker/models/secrets.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/models/services.py` & `docker-7.0.0b3/docker/models/services.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/models/swarm.py` & `docker-7.0.0b3/docker/models/swarm.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/models/volumes.py` & `docker-7.0.0b3/docker/models/volumes.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/tls.py` & `docker-7.0.0b3/docker/tls.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/transport/npipeconn.py` & `docker-7.0.0b3/docker/transport/npipeconn.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/transport/npipesocket.py` & `docker-7.0.0b3/docker/transport/npipesocket.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/transport/sshconn.py` & `docker-7.0.0b3/docker/transport/sshconn.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/transport/unixconn.py` & `docker-7.0.0b3/docker/transport/unixconn.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/types/__init__.py` & `docker-7.0.0b3/docker/types/__init__.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/types/containers.py` & `docker-7.0.0b3/docker/types/containers.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/types/daemon.py` & `docker-7.0.0b3/docker/types/daemon.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/types/healthcheck.py` & `docker-7.0.0b3/docker/types/healthcheck.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/types/networks.py` & `docker-7.0.0b3/docker/types/networks.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/types/services.py` & `docker-7.0.0b3/docker/types/services.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/types/swarm.py` & `docker-7.0.0b3/docker/types/swarm.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/utils/__init__.py` & `docker-7.0.0b3/docker/utils/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from .build import create_archive, exclude_paths, mkbuildcontext, tar
+from .build import match_tag, create_archive, exclude_paths, mkbuildcontext, tar
 from .decorators import check_resource, minimum_version, update_headers
 from .utils import (
     compare_version, convert_port_bindings, convert_volume_binds,
     parse_repository_tag, parse_host,
     kwargs_from_env, convert_filters, datetime_to_timestamp,
     create_host_config, parse_bytes, parse_env_file, version_lt,
     version_gte, decode_json_header, split_command, create_ipam_config,
```

### Comparing `docker-7.0.0b2/docker/utils/build.py` & `docker-7.0.0b3/docker/utils/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 import tempfile
 
 from .fnmatch import fnmatch
 from ..constants import IS_WINDOWS_PLATFORM
 
 
 _SEP = re.compile('/|\\\\') if IS_WINDOWS_PLATFORM else re.compile('/')
+_TAG = re.compile(
+    r"^[a-z0-9]+((\.|_|__|-+)[a-z0-9]+)*(\/[a-z0-9]+((\.|_|__|-+)[a-z0-9]+)*)*" \
+        + "(:[a-zA-Z0-9_][a-zA-Z0-9._-]{0,127})?$"
+)
+
+
+def match_tag(tag: str) -> bool:
+    return bool(_TAG.match(tag))
 
 
 def tar(path, exclude=None, dockerfile=None, fileobj=None, gzip=False):
     root = os.path.abspath(path)
     exclude = exclude or []
     dockerfile = dockerfile or (None, None)
     extra_files = []
```

### Comparing `docker-7.0.0b2/docker/utils/config.py` & `docker-7.0.0b3/docker/utils/config.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/utils/decorators.py` & `docker-7.0.0b3/docker/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/utils/fnmatch.py` & `docker-7.0.0b3/docker/utils/fnmatch.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/utils/json_stream.py` & `docker-7.0.0b3/docker/utils/json_stream.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/utils/ports.py` & `docker-7.0.0b3/docker/utils/ports.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/utils/proxy.py` & `docker-7.0.0b3/docker/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/utils/socket.py` & `docker-7.0.0b3/docker/utils/socket.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker/utils/utils.py` & `docker-7.0.0b3/docker/utils/utils.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docker.egg-info/PKG-INFO` & `docker-7.0.0b3/docker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker
-Version: 7.0.0b2
+Version: 7.0.0b3
 Summary: A Python library for the Docker Engine API.
 Home-page: https://github.com/docker/docker-py
 Maintainer: Ulysses Souza
 Maintainer-email: ulysses.souza@docker.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docker-py.readthedocs.io
 Project-URL: Changelog, https://docker-py.readthedocs.io/en/stable/change-log.html
```

### Comparing `docker-7.0.0b2/docker.egg-info/SOURCES.txt` & `docker-7.0.0b3/docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/api.rst` & `docker-7.0.0b3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/change-log.md` & `docker-7.0.0b3/docs/change-log.md`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/client.rst` & `docker-7.0.0b3/docs/client.rst`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/conf.py` & `docker-7.0.0b3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/containers.rst` & `docker-7.0.0b3/docs/containers.rst`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/favicon_whale.png` & `docker-7.0.0b3/docs/favicon_whale.png`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/images.rst` & `docker-7.0.0b3/docs/images.rst`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/index.rst` & `docker-7.0.0b3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/networks.rst` & `docker-7.0.0b3/docs/networks.rst`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/nodes.rst` & `docker-7.0.0b3/docs/nodes.rst`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/plugins.rst` & `docker-7.0.0b3/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/services.rst` & `docker-7.0.0b3/docs/services.rst`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/swarm.rst` & `docker-7.0.0b3/docs/swarm.rst`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/tls.rst` & `docker-7.0.0b3/docs/tls.rst`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/user_guides/multiplex.rst` & `docker-7.0.0b3/docs/user_guides/multiplex.rst`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/user_guides/swarm_services.md` & `docker-7.0.0b3/docs/user_guides/swarm_services.md`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/docs/volumes.rst` & `docker-7.0.0b3/docs/volumes.rst`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/scripts/release.sh` & `docker-7.0.0b3/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/scripts/versions.py` & `docker-7.0.0b3/scripts/versions.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/setup.py` & `docker-7.0.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/Dockerfile` & `docker-7.0.0b3/tests/Dockerfile`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/Dockerfile-dind-certs` & `docker-7.0.0b3/tests/Dockerfile-dind-certs`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/gpg-keys/secret` & `docker-7.0.0b3/tests/gpg-keys/secret`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/helpers.py` & `docker-7.0.0b3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/api_build_test.py` & `docker-7.0.0b3/tests/integration/api_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/api_client_test.py` & `docker-7.0.0b3/tests/integration/api_client_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/api_config_test.py` & `docker-7.0.0b3/tests/integration/api_config_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/api_container_test.py` & `docker-7.0.0b3/tests/integration/api_container_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/api_exec_test.py` & `docker-7.0.0b3/tests/integration/api_exec_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/api_healthcheck_test.py` & `docker-7.0.0b3/tests/integration/api_healthcheck_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/api_image_test.py` & `docker-7.0.0b3/tests/integration/api_image_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/api_network_test.py` & `docker-7.0.0b3/tests/integration/api_network_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/api_plugin_test.py` & `docker-7.0.0b3/tests/integration/api_plugin_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/api_secret_test.py` & `docker-7.0.0b3/tests/integration/api_secret_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/api_service_test.py` & `docker-7.0.0b3/tests/integration/api_service_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/api_swarm_test.py` & `docker-7.0.0b3/tests/integration/api_swarm_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/api_volume_test.py` & `docker-7.0.0b3/tests/integration/api_volume_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/base.py` & `docker-7.0.0b3/tests/integration/base.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/client_test.py` & `docker-7.0.0b3/tests/integration/client_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/conftest.py` & `docker-7.0.0b3/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/context_api_test.py` & `docker-7.0.0b3/tests/integration/context_api_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/credentials/store_test.py` & `docker-7.0.0b3/tests/integration/credentials/store_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/errors_test.py` & `docker-7.0.0b3/tests/integration/errors_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/models_containers_test.py` & `docker-7.0.0b3/tests/integration/models_containers_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/models_images_test.py` & `docker-7.0.0b3/tests/integration/models_images_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/models_networks_test.py` & `docker-7.0.0b3/tests/integration/models_networks_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/models_nodes_test.py` & `docker-7.0.0b3/tests/integration/models_nodes_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/models_resources_test.py` & `docker-7.0.0b3/tests/integration/models_resources_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/models_services_test.py` & `docker-7.0.0b3/tests/integration/models_services_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/models_swarm_test.py` & `docker-7.0.0b3/tests/integration/models_swarm_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/models_volumes_test.py` & `docker-7.0.0b3/tests/integration/models_volumes_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/integration/regression_test.py` & `docker-7.0.0b3/tests/integration/regression_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/ssh/api_build_test.py` & `docker-7.0.0b3/tests/ssh/api_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/ssh/base.py` & `docker-7.0.0b3/tests/ssh/base.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/ssh/config/client/id_rsa` & `docker-7.0.0b3/tests/ssh/config/client/id_rsa`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/ssh/config/client/id_rsa.pub` & `docker-7.0.0b3/tests/ssh/config/client/id_rsa.pub`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/ssh/connect_test.py` & `docker-7.0.0b3/tests/ssh/connect_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/api_build_test.py` & `docker-7.0.0b3/tests/unit/api_build_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,225 +1,252 @@
 import gzip
 import io
 import shutil
 
+import pytest
+
 import docker
-from docker import auth
+from docker import auth, errors
 from docker.api.build import process_dockerfile
 
-import pytest
-
 from ..helpers import make_tree
 from .api_test import BaseAPIClientTest, fake_request, url_prefix
 
 
 class BuildTest(BaseAPIClientTest):
     def test_build_container(self):
-        script = io.BytesIO('\n'.join([
-            'FROM busybox',
-            'RUN mkdir -p /tmp/test',
-            'EXPOSE 8080',
-            'ADD https://dl.dropboxusercontent.com/u/20637798/silence.tar.gz'
-            ' /tmp/silence.tar.gz'
-        ]).encode('ascii'))
+        script = io.BytesIO(
+            "\n".join(
+                [
+                    "FROM busybox",
+                    "RUN mkdir -p /tmp/test",
+                    "EXPOSE 8080",
+                    "ADD https://dl.dropboxusercontent.com/u/20637798/silence.tar.gz"
+                    " /tmp/silence.tar.gz",
+                ]
+            ).encode("ascii")
+        )
 
         self.client.build(fileobj=script)
 
     def test_build_container_pull(self):
-        script = io.BytesIO('\n'.join([
-            'FROM busybox',
-            'RUN mkdir -p /tmp/test',
-            'EXPOSE 8080',
-            'ADD https://dl.dropboxusercontent.com/u/20637798/silence.tar.gz'
-            ' /tmp/silence.tar.gz'
-        ]).encode('ascii'))
+        script = io.BytesIO(
+            "\n".join(
+                [
+                    "FROM busybox",
+                    "RUN mkdir -p /tmp/test",
+                    "EXPOSE 8080",
+                    "ADD https://dl.dropboxusercontent.com/u/20637798/silence.tar.gz"
+                    " /tmp/silence.tar.gz",
+                ]
+            ).encode("ascii")
+        )
 
         self.client.build(fileobj=script, pull=True)
 
     def test_build_container_custom_context(self):
-        script = io.BytesIO('\n'.join([
-            'FROM busybox',
-            'RUN mkdir -p /tmp/test',
-            'EXPOSE 8080',
-            'ADD https://dl.dropboxusercontent.com/u/20637798/silence.tar.gz'
-            ' /tmp/silence.tar.gz'
-        ]).encode('ascii'))
+        script = io.BytesIO(
+            "\n".join(
+                [
+                    "FROM busybox",
+                    "RUN mkdir -p /tmp/test",
+                    "EXPOSE 8080",
+                    "ADD https://dl.dropboxusercontent.com/u/20637798/silence.tar.gz"
+                    " /tmp/silence.tar.gz",
+                ]
+            ).encode("ascii")
+        )
         context = docker.utils.mkbuildcontext(script)
 
         self.client.build(fileobj=context, custom_context=True)
 
     def test_build_container_custom_context_gzip(self):
-        script = io.BytesIO('\n'.join([
-            'FROM busybox',
-            'RUN mkdir -p /tmp/test',
-            'EXPOSE 8080',
-            'ADD https://dl.dropboxusercontent.com/u/20637798/silence.tar.gz'
-            ' /tmp/silence.tar.gz'
-        ]).encode('ascii'))
+        script = io.BytesIO(
+            "\n".join(
+                [
+                    "FROM busybox",
+                    "RUN mkdir -p /tmp/test",
+                    "EXPOSE 8080",
+                    "ADD https://dl.dropboxusercontent.com/u/20637798/silence.tar.gz"
+                    " /tmp/silence.tar.gz",
+                ]
+            ).encode("ascii")
+        )
         context = docker.utils.mkbuildcontext(script)
         gz_context = gzip.GzipFile(fileobj=context)
 
-        self.client.build(
-            fileobj=gz_context,
-            custom_context=True,
-            encoding="gzip"
-        )
+        self.client.build(fileobj=gz_context, custom_context=True, encoding="gzip")
 
     def test_build_remote_with_registry_auth(self):
-        self.client._auth_configs = auth.AuthConfig({
-            'auths': {
-                'https://example.com': {
-                    'user': 'example',
-                    'password': 'example',
-                    'email': 'example@example.com'
+        self.client._auth_configs = auth.AuthConfig(
+            {
+                "auths": {
+                    "https://example.com": {
+                        "user": "example",
+                        "password": "example",
+                        "email": "example@example.com",
+                    }
                 }
             }
-        })
+        )
 
-        expected_params = {'t': None, 'q': False, 'dockerfile': None,
-                           'rm': False, 'nocache': False, 'pull': False,
-                           'forcerm': False,
-                           'remote': 'https://github.com/docker-library/mongo'}
+        expected_params = {
+            "t": None,
+            "q": False,
+            "dockerfile": None,
+            "rm": False,
+            "nocache": False,
+            "pull": False,
+            "forcerm": False,
+            "remote": "https://github.com/docker-library/mongo",
+        }
         expected_headers = {
-            'X-Registry-Config': auth.encode_header(
-                self.client._auth_configs.auths
-            )
+            "X-Registry-Config": auth.encode_header(self.client._auth_configs.auths)
         }
 
-        self.client.build(path='https://github.com/docker-library/mongo')
+        self.client.build(path="https://github.com/docker-library/mongo")
 
         fake_request.assert_called_with(
-            'POST',
+            "POST",
             f"{url_prefix}build",
             stream=True,
             data=None,
             headers=expected_headers,
             params=expected_params,
-            timeout=None
+            timeout=None,
         )
 
     def test_build_container_with_named_dockerfile(self):
-        self.client.build('.', dockerfile='nameddockerfile')
+        self.client.build(".", dockerfile="nameddockerfile")
+
+    def test_build_with_invalid_tag(self):
+        with pytest.raises(errors.DockerException):
+            self.client.build(".", tag="https://example.com")
 
     def test_build_container_with_container_limits(self):
-        self.client.build('.', container_limits={
-            'memory': 1024 * 1024,
-            'cpusetcpus': 1,
-            'cpushares': 1000,
-            'memswap': 1024 * 1024 * 8
-        })
+        self.client.build(
+            ".",
+            container_limits={
+                "memory": 1024 * 1024,
+                "cpusetcpus": 1,
+                "cpushares": 1000,
+                "memswap": 1024 * 1024 * 8,
+            },
+        )
 
     def test_build_container_invalid_container_limits(self):
         with pytest.raises(docker.errors.DockerException):
-            self.client.build('.', container_limits={
-                'foo': 'bar'
-            })
+            self.client.build(".", container_limits={"foo": "bar"})
 
     def test_set_auth_headers_with_empty_dict_and_auth_configs(self):
-        self.client._auth_configs = auth.AuthConfig({
-            'auths': {
-                'https://example.com': {
-                    'user': 'example',
-                    'password': 'example',
-                    'email': 'example@example.com'
+        self.client._auth_configs = auth.AuthConfig(
+            {
+                "auths": {
+                    "https://example.com": {
+                        "user": "example",
+                        "password": "example",
+                        "email": "example@example.com",
+                    }
                 }
             }
-        })
+        )
 
         headers = {}
         expected_headers = {
-            'X-Registry-Config': auth.encode_header(
-                self.client._auth_configs.auths
-            )
+            "X-Registry-Config": auth.encode_header(self.client._auth_configs.auths)
         }
 
         self.client._set_auth_headers(headers)
         assert headers == expected_headers
 
     def test_set_auth_headers_with_dict_and_auth_configs(self):
-        self.client._auth_configs = auth.AuthConfig({
-            'auths': {
-                'https://example.com': {
-                    'user': 'example',
-                    'password': 'example',
-                    'email': 'example@example.com'
+        self.client._auth_configs = auth.AuthConfig(
+            {
+                "auths": {
+                    "https://example.com": {
+                        "user": "example",
+                        "password": "example",
+                        "email": "example@example.com",
+                    }
                 }
             }
-        })
+        )
 
-        headers = {'foo': 'bar'}
+        headers = {"foo": "bar"}
         expected_headers = {
-            'X-Registry-Config': auth.encode_header(
-                self.client._auth_configs.auths
-            ),
-            'foo': 'bar'
+            "X-Registry-Config": auth.encode_header(self.client._auth_configs.auths),
+            "foo": "bar",
         }
 
         self.client._set_auth_headers(headers)
         assert headers == expected_headers
 
     def test_set_auth_headers_with_dict_and_no_auth_configs(self):
-        headers = {'foo': 'bar'}
-        expected_headers = {
-            'foo': 'bar'
-        }
+        headers = {"foo": "bar"}
+        expected_headers = {"foo": "bar"}
 
         self.client._set_auth_headers(headers)
         assert headers == expected_headers
 
     @pytest.mark.skipif(
-        not docker.constants.IS_WINDOWS_PLATFORM,
-        reason='Windows-specific syntax')
+        not docker.constants.IS_WINDOWS_PLATFORM, reason="Windows-specific syntax"
+    )
     def test_process_dockerfile_win_longpath_prefix(self):
         dirs = [
-            'foo', 'foo/bar', 'baz',
+            "foo",
+            "foo/bar",
+            "baz",
         ]
 
         files = [
-            'Dockerfile', 'foo/Dockerfile.foo', 'foo/bar/Dockerfile.bar',
-            'baz/Dockerfile.baz',
+            "Dockerfile",
+            "foo/Dockerfile.foo",
+            "foo/bar/Dockerfile.bar",
+            "baz/Dockerfile.baz",
         ]
 
         base = make_tree(dirs, files)
         self.addCleanup(shutil.rmtree, base)
 
         def pre(path):
             return docker.constants.WINDOWS_LONGPATH_PREFIX + path
 
         assert process_dockerfile(None, pre(base)) == (None, None)
-        assert process_dockerfile('Dockerfile', pre(base)) == (
-            'Dockerfile', None
-        )
-        assert process_dockerfile('foo/Dockerfile.foo', pre(base)) == (
-            'foo/Dockerfile.foo', None
+        assert process_dockerfile("Dockerfile", pre(base)) == ("Dockerfile", None)
+        assert process_dockerfile("foo/Dockerfile.foo", pre(base)) == (
+            "foo/Dockerfile.foo",
+            None,
+        )
+        assert process_dockerfile("../Dockerfile", pre(f"{base}\\foo"))[1] is not None
+        assert process_dockerfile("../baz/Dockerfile.baz", pre(f"{base}/baz")) == (
+            "../baz/Dockerfile.baz",
+            None,
         )
-        assert process_dockerfile(
-            '../Dockerfile', pre(f"{base}\\foo")
-        )[1] is not None
-        assert process_dockerfile(
-            '../baz/Dockerfile.baz', pre(f"{base}/baz")
-        ) == ('../baz/Dockerfile.baz', None)
 
     def test_process_dockerfile(self):
         dirs = [
-            'foo', 'foo/bar', 'baz',
+            "foo",
+            "foo/bar",
+            "baz",
         ]
 
         files = [
-            'Dockerfile', 'foo/Dockerfile.foo', 'foo/bar/Dockerfile.bar',
-            'baz/Dockerfile.baz',
+            "Dockerfile",
+            "foo/Dockerfile.foo",
+            "foo/bar/Dockerfile.bar",
+            "baz/Dockerfile.baz",
         ]
 
         base = make_tree(dirs, files)
         self.addCleanup(shutil.rmtree, base)
 
         assert process_dockerfile(None, base) == (None, None)
-        assert process_dockerfile('Dockerfile', base) == ('Dockerfile', None)
-        assert process_dockerfile('foo/Dockerfile.foo', base) == (
-            'foo/Dockerfile.foo', None
-        )
-        assert process_dockerfile(
-            '../Dockerfile', f"{base}/foo"
-        )[1] is not None
-        assert process_dockerfile('../baz/Dockerfile.baz', f"{base}/baz") == (
-            '../baz/Dockerfile.baz', None
+        assert process_dockerfile("Dockerfile", base) == ("Dockerfile", None)
+        assert process_dockerfile("foo/Dockerfile.foo", base) == (
+            "foo/Dockerfile.foo",
+            None,
+        )
+        assert process_dockerfile("../Dockerfile", f"{base}/foo")[1] is not None
+        assert process_dockerfile("../baz/Dockerfile.baz", f"{base}/baz") == (
+            "../baz/Dockerfile.baz",
+            None,
         )
```

### Comparing `docker-7.0.0b2/tests/unit/api_container_test.py` & `docker-7.0.0b3/tests/unit/api_container_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/api_exec_test.py` & `docker-7.0.0b3/tests/unit/api_exec_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/api_image_test.py` & `docker-7.0.0b3/tests/unit/api_image_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/api_network_test.py` & `docker-7.0.0b3/tests/unit/api_network_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/api_test.py` & `docker-7.0.0b3/tests/unit/api_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/api_volume_test.py` & `docker-7.0.0b3/tests/unit/api_volume_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/auth_test.py` & `docker-7.0.0b3/tests/unit/auth_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/client_test.py` & `docker-7.0.0b3/tests/unit/client_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/context_test.py` & `docker-7.0.0b3/tests/unit/context_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/dockertypes_test.py` & `docker-7.0.0b3/tests/unit/dockertypes_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/errors_test.py` & `docker-7.0.0b3/tests/unit/errors_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/fake_api.py` & `docker-7.0.0b3/tests/unit/fake_api.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/fake_api_client.py` & `docker-7.0.0b3/tests/unit/fake_api_client.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/fake_stat.py` & `docker-7.0.0b3/tests/unit/fake_stat.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/models_containers_test.py` & `docker-7.0.0b3/tests/unit/models_containers_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/models_images_test.py` & `docker-7.0.0b3/tests/unit/models_images_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/models_networks_test.py` & `docker-7.0.0b3/tests/unit/models_networks_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/models_resources_test.py` & `docker-7.0.0b3/tests/unit/models_resources_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/models_services_test.py` & `docker-7.0.0b3/tests/unit/models_services_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/sshadapter_test.py` & `docker-7.0.0b3/tests/unit/sshadapter_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/swarm_test.py` & `docker-7.0.0b3/tests/unit/swarm_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/utils_build_test.py` & `docker-7.0.0b3/tests/unit/utils_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/utils_config_test.py` & `docker-7.0.0b3/tests/unit/utils_config_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/utils_json_stream_test.py` & `docker-7.0.0b3/tests/unit/utils_json_stream_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/utils_proxy_test.py` & `docker-7.0.0b3/tests/unit/utils_proxy_test.py`

 * *Files identical despite different names*

### Comparing `docker-7.0.0b2/tests/unit/utils_test.py` & `docker-7.0.0b3/tests/unit/utils_test.py`

 * *Files identical despite different names*

