# Comparing `tmp/jupyter_client-8.6.0.tar.gz` & `tmp/jupyter_client-8.6.1.tar.gz`

## Comparing `jupyter_client-8.6.0.tar` & `jupyter_client-8.6.1.tar`

### file list

```diff
@@ -1,97 +1,98 @@
--rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/.mailmap
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/.readthedocs.yaml
--rw-r--r--   0        0        0    83511 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/RELEASING.md
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/.github/dependabot.yml
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/.github/workflows/downstream.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/Makefile
--rw-r--r--   0        0        0    11008 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/conf.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/index.rst
--rw-r--r--   0        0        0     8615 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/kernels.rst
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/make.bat
--rw-r--r--   0        0        0    64106 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/messaging.rst
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/migration.md
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/pending-kernels.rst
--rw-r--r--   0        0        0    15275 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/provisioning.rst
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/wrapperkernels.rst
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/api/jupyter_client.asynchronous.rst
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/api/jupyter_client.blocking.rst
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/api/jupyter_client.ioloop.rst
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/api/jupyter_client.provisioning.rst
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/api/jupyter_client.rst
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/api/jupyter_client.ssh.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/api/modules.rst
--rw-r--r--   0        0        0   153577 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/figs/frontend-kernel.png
--rw-r--r--   0        0        0   283952 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/docs/figs/frontend-kernel.svg
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/_version.py
--rw-r--r--   0        0        0    14381 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/adapter.py
--rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/channels.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/channelsabc.py
--rw-r--r--   0        0        0    30834 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/client.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/clientabc.py
--rw-r--r--   0        0        0    25340 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/connect.py
--rw-r--r--   0        0        0    13913 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/consoleapp.py
--rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/jsonutil.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/kernelapp.py
--rw-r--r--   0        0        0    15663 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/kernelspec.py
--rw-r--r--   0        0        0    12048 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/kernelspecapp.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/launcher.py
--rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/localinterfaces.py
--rw-r--r--   0        0        0    30322 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/manager.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/managerabc.py
--rw-r--r--   0        0        0    22601 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/multikernelmanager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/py.typed
--rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/restarter.py
--rw-r--r--   0        0        0     4684 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/runapp.py
--rw-r--r--   0        0        0    37774 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/session.py
--rw-r--r--   0        0        0    11283 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/threaded.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/utils.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/win_interrupt.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/asynchronous/__init__.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/asynchronous/client.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/blocking/__init__.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/blocking/client.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/ioloop/__init__.py
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/ioloop/manager.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/ioloop/restarter.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/provisioning/__init__.py
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/provisioning/factory.py
--rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/provisioning/local_provisioner.py
--rw-r--r--   0        0        0     9970 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/provisioning/provisioner_base.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/ssh/__init__.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/ssh/forward.py
--rw-r--r--   0        0        0    13795 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/jupyter_client/ssh/tunnel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/conftest.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/problemkernel.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/signalkernel.py
--rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_adapter.py
--rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_client.py
--rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_connect.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_consoleapp.py
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_jsonutil.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_kernelapp.py
--rw-r--r--   0        0        0    19981 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_kernelmanager.py
--rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_kernelspec.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_kernelspecapp.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_localinterfaces.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_manager.py
--rw-r--r--   0        0        0    23126 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_multikernelmanager.py
--rw-r--r--   0        0        0    11892 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_provisioning.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_public_api.py
--rw-r--r--   0        0        0     8404 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_restarter.py
--rw-r--r--   0        0        0    19845 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_session.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/test_ssh.py
--rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/tests/utils.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/.gitignore
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/LICENSE
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/README.md
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/pyproject.toml
--rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 jupyter_client-8.6.0/PKG-INFO
+-rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/.mailmap
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/.readthedocs.yaml
+-rw-r--r--   0        0        0    86028 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/RELEASING.md
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/.github/workflows/downstream.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/.github/workflows/publish-changelog.yml
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/Makefile
+-rw-r--r--   0        0        0    11008 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/conf.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/index.rst
+-rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/kernels.rst
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/make.bat
+-rw-r--r--   0        0        0    64719 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/messaging.rst
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/migration.md
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/pending-kernels.rst
+-rw-r--r--   0        0        0    15275 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/provisioning.rst
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/wrapperkernels.rst
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/api/jupyter_client.asynchronous.rst
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/api/jupyter_client.blocking.rst
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/api/jupyter_client.ioloop.rst
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/api/jupyter_client.provisioning.rst
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/api/jupyter_client.rst
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/api/jupyter_client.ssh.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/api/modules.rst
+-rw-r--r--   0        0        0   153577 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/figs/frontend-kernel.png
+-rw-r--r--   0        0        0   283952 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/docs/figs/frontend-kernel.svg
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/_version.py
+-rw-r--r--   0        0        0    14381 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/adapter.py
+-rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/channels.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/channelsabc.py
+-rw-r--r--   0        0        0    30834 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/client.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/clientabc.py
+-rw-r--r--   0        0        0    25340 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/connect.py
+-rw-r--r--   0        0        0    13913 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/consoleapp.py
+-rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/jsonutil.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/kernelapp.py
+-rw-r--r--   0        0        0    15663 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/kernelspec.py
+-rw-r--r--   0        0        0    12048 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/kernelspecapp.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/launcher.py
+-rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/localinterfaces.py
+-rw-r--r--   0        0        0    30322 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/manager.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/managerabc.py
+-rw-r--r--   0        0        0    22601 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/multikernelmanager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/py.typed
+-rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/restarter.py
+-rw-r--r--   0        0        0     4684 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/runapp.py
+-rw-r--r--   0        0        0    37774 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/session.py
+-rw-r--r--   0        0        0    11283 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/threaded.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/utils.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/win_interrupt.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/asynchronous/__init__.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/asynchronous/client.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/blocking/__init__.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/blocking/client.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/ioloop/__init__.py
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/ioloop/manager.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/ioloop/restarter.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/provisioning/__init__.py
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/provisioning/factory.py
+-rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/provisioning/local_provisioner.py
+-rw-r--r--   0        0        0     9970 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/provisioning/provisioner_base.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/ssh/__init__.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/ssh/forward.py
+-rw-r--r--   0        0        0    13795 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/jupyter_client/ssh/tunnel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/conftest.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/problemkernel.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/signalkernel.py
+-rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_adapter.py
+-rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_client.py
+-rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_connect.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_consoleapp.py
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_jsonutil.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_kernelapp.py
+-rw-r--r--   0        0        0    19981 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_kernelmanager.py
+-rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_kernelspec.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_kernelspecapp.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_localinterfaces.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_manager.py
+-rw-r--r--   0        0        0    23126 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_multikernelmanager.py
+-rw-r--r--   0        0        0    11892 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_provisioning.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_public_api.py
+-rw-r--r--   0        0        0     8404 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_restarter.py
+-rw-r--r--   0        0        0    19845 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_session.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/test_ssh.py
+-rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/tests/utils.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/.gitignore
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/LICENSE
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/README.md
+-rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/pyproject.toml
+-rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 jupyter_client-8.6.1/PKG-INFO
```

### Comparing `jupyter_client-8.6.0/.mailmap` & `jupyter_client-8.6.1/.mailmap`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/.pre-commit-config.yaml` & `jupyter_client-8.6.1/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -17,31 +17,31 @@
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.27.0
+    rev: 0.27.4
     hooks:
       - id: check-github-workflows
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
       - id: mdformat
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.3"
+    rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         types_or: [yaml, html, json]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.6.1"
+    rev: "v1.8.0"
     hooks:
       - id: mypy
         files: jupyter_client
         stages: [manual]
         args: ["--install-types", "--non-interactive"]
         additional_dependencies:
           ["traitlets>=5.13", "ipykernel>=6.26", "jupyter_core>=5.3.2"]
@@ -62,18 +62,20 @@
     rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.3
+    rev: v0.2.0
     hooks:
       - id: ruff
+        types_or: [python, jupyter]
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
+        types_or: [python, jupyter]
 
   - repo: https://github.com/scientific-python/cookie
-    rev: "2023.10.27"
+    rev: "2024.01.24"
     hooks:
       - id: sp-repo-review
         additional_dependencies: ["repo-review[cli]"]
```

### Comparing `jupyter_client-8.6.0/CHANGELOG.md` & `jupyter_client-8.6.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,5220 +1,5377 @@
 00000000: 2320 4368 616e 6765 7320 696e 204a 7570  # Changes in Jup
 00000010: 7974 6572 2043 6c69 656e 7420 7b23 6368  yter Client {#ch
 00000020: 616e 6765 6c6f 677d 0a0a 3c21 2d2d 203c  angelog}..<!-- <
 00000030: 5354 4152 5420 4e45 5720 4348 414e 4745  START NEW CHANGE
 00000040: 4c4f 4720 454e 5452 593e 202d 2d3e 0a0a  LOG ENTRY> -->..
-00000050: 2323 2038 2e36 2e30 0a0a 285b 4675 6c6c  ## 8.6.0..([Full
+00000050: 2323 2038 2e36 2e31 0a0a 285b 4675 6c6c  ## 8.6.1..([Full
 00000060: 2043 6861 6e67 656c 6f67 5d28 6874 7470   Changelog](http
 00000070: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
 00000080: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
 00000090: 6c69 656e 742f 636f 6d70 6172 652f 7638  lient/compare/v8
-000000a0: 2e35 2e30 2e2e 2e32 6436 6635 3262 6466  .5.0...2d6f52bdf
-000000b0: 3532 3636 3638 3863 3531 6633 3237 3063  5266688c51f3270c
-000000c0: 6437 6534 3762 6264 3137 6337 3038 6329  d7e47bbd17c708c)
-000000d0: 290a 0a23 2323 2042 7567 7320 6669 7865  )..### Bugs fixe
-000000e0: 640a 0a2d 2046 6978 2070 6f73 7369 626c  d..- Fix possibl
-000000f0: 7920 6e6f 7420 6465 6669 6e65 6420 7472  y not defined tr
-00000100: 6163 6b65 7220 5b23 3939 315d 2868 7474  acker [#991](htt
-00000110: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000120: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00000130: 636c 6965 6e74 2f70 756c 6c2f 3939 3129  client/pull/991)
-00000140: 2028 5b40 6461 7669 6462 726f 6368 6172   ([@davidbrochar
-00000150: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
-00000160: 622e 636f 6d2f 6461 7669 6462 726f 6368  b.com/davidbroch
-00000170: 6172 7429 290a 2d20 4255 473a 2046 6978  art)).- BUG: Fix
-00000180: 204b 7761 7267 206f 6e6c 7920 696e 2075   Kwarg only in u
-00000190: 7064 6174 655f 656e 7620 5b23 3938 395d  pdate_env [#989]
-000001a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000001b0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-000001c0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-000001d0: 3938 3929 2028 5b40 4361 7272 6561 755d  989) ([@Carreau]
-000001e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000001f0: 636f 6d2f 4361 7272 6561 7529 290a 0a23  com/Carreau))..#
-00000200: 2323 204d 6169 6e74 656e 616e 6365 2061  ## Maintenance a
-00000210: 6e64 2075 706b 6565 7020 696d 7072 6f76  nd upkeep improv
-00000220: 656d 656e 7473 0a0a 2d20 5570 6461 7465  ements..- Update
-00000230: 2074 7970 696e 6720 666f 7220 7472 6169   typing for trai
-00000240: 746c 6574 7320 352e 3133 205b 2339 3935  tlets 5.13 [#995
-00000250: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000260: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00000270: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00000280: 2f39 3935 2920 285b 4062 6c69 6e6b 3130  /995) ([@blink10
-00000290: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
-000002a0: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
-000002b0: 2929 0a2d 2055 7365 2072 7566 6620 666f  )).- Use ruff fo
-000002c0: 726d 6174 205b 2339 3932 5d28 6874 7470  rmat [#992](http
-000002d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000002e0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-000002f0: 6c69 656e 742f 7075 6c6c 2f39 3932 2920  lient/pull/992) 
-00000300: 285b 4062 6c69 6e6b 3130 3733 5d28 6874  ([@blink1073](ht
-00000310: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000320: 2f62 6c69 6e6b 3130 3733 2929 0a2d 2055  /blink1073)).- U
-00000330: 6e75 7365 6420 602a 6172 6773 6020 696e  nused `*args` in
-00000340: 2060 4b65 726e 656c 4d61 6e61 6765 7260   `KernelManager`
-00000350: 2773 2060 5f5f 696e 6974 5f5f 6020 5b23  's `__init__` [#
-00000360: 3938 365d 2868 7474 7073 3a2f 2f67 6974  986](https://git
-00000370: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-00000380: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-00000390: 756c 6c2f 3938 3629 2028 5b40 4361 7272  ull/986) ([@Carr
-000003a0: 6561 755d 2868 7474 7073 3a2f 2f67 6974  eau](https://git
-000003b0: 6875 622e 636f 6d2f 4361 7272 6561 7529  hub.com/Carreau)
-000003c0: 290a 0a23 2323 2043 6f6e 7472 6962 7574  )..### Contribut
-000003d0: 6f72 7320 746f 2074 6869 7320 7265 6c65  ors to this rele
-000003e0: 6173 650a 0a28 5b47 6974 4875 6220 636f  ase..([GitHub co
-000003f0: 6e74 7269 6275 746f 7273 2070 6167 6520  ntributors page 
-00000400: 666f 7220 7468 6973 2072 656c 6561 7365  for this release
-00000410: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000420: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00000430: 7974 6572 5f63 6c69 656e 742f 6772 6170  yter_client/grap
-00000440: 6873 2f63 6f6e 7472 6962 7574 6f72 733f  hs/contributors?
-00000450: 6672 6f6d 3d32 3032 332d 3130 2d32 3526  from=2023-10-25&
-00000460: 746f 3d32 3032 332d 3131 2d30 3626 7479  to=2023-11-06&ty
-00000470: 7065 3d63 2929 0a0a 5b40 626c 696e 6b31  pe=c))..[@blink1
-00000480: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
-00000490: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
-000004a0: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
-000004b0: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
-000004c0: 2b69 6e76 6f6c 7665 7325 3341 626c 696e  +involves%3Ablin
-000004d0: 6b31 3037 332b 7570 6461 7465 6425 3341  k1073+updated%3A
-000004e0: 3230 3233 2d31 302d 3235 2e2e 3230 3233  2023-10-25..2023
-000004f0: 2d31 312d 3036 2674 7970 653d 4973 7375  -11-06&type=Issu
-00000500: 6573 2920 7c20 5b40 4361 7272 6561 755d  es) | [@Carreau]
-00000510: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000520: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
-00000530: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
-00000540: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
-00000550: 6f6c 7665 7325 3341 4361 7272 6561 752b  olves%3ACarreau+
-00000560: 7570 6461 7465 6425 3341 3230 3233 2d31  updated%3A2023-1
-00000570: 302d 3235 2e2e 3230 3233 2d31 312d 3036  0-25..2023-11-06
-00000580: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
-00000590: 5b40 6461 7669 6462 726f 6368 6172 745d  [@davidbrochart]
-000005a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000005b0: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
-000005c0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
-000005d0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
-000005e0: 6f6c 7665 7325 3341 6461 7669 6462 726f  olves%3Adavidbro
-000005f0: 6368 6172 742b 7570 6461 7465 6425 3341  chart+updated%3A
-00000600: 3230 3233 2d31 302d 3235 2e2e 3230 3233  2023-10-25..2023
-00000610: 2d31 312d 3036 2674 7970 653d 4973 7375  -11-06&type=Issu
-00000620: 6573 290a 0a3c 212d 2d20 3c45 4e44 204e  es)..<!-- <END N
-00000630: 4557 2043 4841 4e47 454c 4f47 2045 4e54  EW CHANGELOG ENT
-00000640: 5259 3e20 2d2d 3e0a 0a23 2320 382e 352e  RY> -->..## 8.5.
-00000650: 300a 0a28 5b46 756c 6c20 4368 616e 6765  0..([Full Change
-00000660: 6c6f 675d 2868 7474 7073 3a2f 2f67 6974  log](https://git
-00000670: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-00000680: 6a75 7079 7465 725f 636c 6965 6e74 2f63  jupyter_client/c
-00000690: 6f6d 7061 7265 2f76 382e 342e 302e 2e2e  ompare/v8.4.0...
-000006a0: 6666 3934 6533 3130 6332 6166 3335 3436  ff94e310c2af3546
-000006b0: 6632 6639 3338 3465 3662 3335 6664 3131  f2f9384e6b35fd11
-000006c0: 6333 6430 3961 3731 2929 0a0a 2323 2320  c3d09a71))..### 
-000006d0: 456e 6861 6e63 656d 656e 7473 206d 6164  Enhancements mad
-000006e0: 650a 0a2d 2041 6c6c 6f77 2074 6f20 7570  e..- Allow to up
-000006f0: 6461 7465 206b 6572 6e65 6c73 2065 6e76  date kernels env
-00000700: 2069 6e20 6265 7477 6565 6e20 7265 7374   in between rest
-00000710: 6172 742e 205b 2339 3837 5d28 6874 7470  art. [#987](http
-00000720: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00000730: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00000740: 6c69 656e 742f 7075 6c6c 2f39 3837 2920  lient/pull/987) 
-00000750: 285b 4043 6172 7265 6175 5d28 6874 7470  ([@Carreau](http
-00000760: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f43  s://github.com/C
-00000770: 6172 7265 6175 2929 0a0a 2323 2320 4d61  arreau))..### Ma
-00000780: 696e 7465 6e61 6e63 6520 616e 6420 7570  intenance and up
-00000790: 6b65 6570 2069 6d70 726f 7665 6d65 6e74  keep improvement
-000007a0: 730a 0a2d 2045 6e61 626c 6520 7374 7269  s..- Enable stri
-000007b0: 6374 2074 7970 696e 6720 5b23 3938 345d  ct typing [#984]
-000007c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000007d0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-000007e0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-000007f0: 3938 3429 2028 5b40 626c 696e 6b31 3037  984) ([@blink107
-00000800: 335d 2868 7474 7073 3a2f 2f67 6974 6875  3](https://githu
-00000810: 622e 636f 6d2f 626c 696e 6b31 3037 3329  b.com/blink1073)
-00000820: 290a 2d20 5570 6461 7465 2074 7970 696e  ).- Update typin
-00000830: 6773 2066 6f72 206d 7970 7920 312e 3620  gs for mypy 1.6 
-00000840: 5b23 3938 335d 2868 7474 7073 3a2f 2f67  [#983](https://g
-00000850: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
-00000860: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
-00000870: 2f70 756c 6c2f 3938 3329 2028 5b40 626c  /pull/983) ([@bl
-00000880: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
-00000890: 2f67 6974 6875 622e 636f 6d2f 626c 696e  /github.com/blin
-000008a0: 6b31 3037 3329 290a 0a23 2323 2043 6f6e  k1073))..### Con
-000008b0: 7472 6962 7574 6f72 7320 746f 2074 6869  tributors to thi
-000008c0: 7320 7265 6c65 6173 650a 0a28 5b47 6974  s release..([Git
-000008d0: 4875 6220 636f 6e74 7269 6275 746f 7273  Hub contributors
-000008e0: 2070 6167 6520 666f 7220 7468 6973 2072   page for this r
-000008f0: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
-00000900: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00000910: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00000920: 742f 6772 6170 6873 2f63 6f6e 7472 6962  t/graphs/contrib
-00000930: 7574 6f72 733f 6672 6f6d 3d32 3032 332d  utors?from=2023-
-00000940: 3130 2d31 3126 746f 3d32 3032 332d 3130  10-11&to=2023-10
-00000950: 2d32 3526 7479 7065 3d63 2929 0a0a 5b40  -25&type=c))..[@
-00000960: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
-00000970: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
-00000980: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
-00000990: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
-000009a0: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
-000009b0: 3341 626c 696e 6b31 3037 332b 7570 6461  3Ablink1073+upda
-000009c0: 7465 6425 3341 3230 3233 2d31 302d 3131  ted%3A2023-10-11
-000009d0: 2e2e 3230 3233 2d31 302d 3235 2674 7970  ..2023-10-25&typ
-000009e0: 653d 4973 7375 6573 2920 7c20 5b40 4361  e=Issues) | [@Ca
-000009f0: 7272 6561 755d 2868 7474 7073 3a2f 2f67  rreau](https://g
-00000a00: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
-00000a10: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
-00000a20: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
-00000a30: 6e74 2b69 6e76 6f6c 7665 7325 3341 4361  nt+involves%3ACa
-00000a40: 7272 6561 752b 7570 6461 7465 6425 3341  rreau+updated%3A
-00000a50: 3230 3233 2d31 302d 3131 2e2e 3230 3233  2023-10-11..2023
-00000a60: 2d31 302d 3235 2674 7970 653d 4973 7375  -10-25&type=Issu
-00000a70: 6573 290a 0a23 2320 382e 342e 300a 0a28  es)..## 8.4.0..(
-00000a80: 5b46 756c 6c20 4368 616e 6765 6c6f 675d  [Full Changelog]
-00000a90: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000aa0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-00000ab0: 7465 725f 636c 6965 6e74 2f63 6f6d 7061  ter_client/compa
-00000ac0: 7265 2f76 382e 332e 312e 2e2e 3734 3034  re/v8.3.1...7404
-00000ad0: 3433 3933 3233 3065 3730 3133 3466 3638  4393230e70134f68
-00000ae0: 6536 3634 6632 6566 3139 6661 6239 3262  e664f2ef19fab92b
-00000af0: 3737 3734 2929 0a0a 2323 2320 4d61 696e  7774))..### Main
-00000b00: 7465 6e61 6e63 6520 616e 6420 7570 6b65  tenance and upke
-00000b10: 6570 2069 6d70 726f 7665 6d65 6e74 730a  ep improvements.
-00000b20: 0a2d 2054 6573 7420 6f6e 2070 7974 686f  .- Test on pytho
-00000b30: 6e20 332e 3132 205b 2339 3738 5d28 6874  n 3.12 [#978](ht
-00000b40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000b50: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00000b60: 5f63 6c69 656e 742f 7075 6c6c 2f39 3738  _client/pull/978
-00000b70: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
-00000b80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000b90: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a2d  om/blink1073)).-
-00000ba0: 2055 7064 6174 6520 7479 7069 6e67 2066   Update typing f
-00000bb0: 6f72 2074 7261 6974 6c65 7473 2035 2e31  or traitlets 5.1
-00000bc0: 3120 5b23 3937 375d 2868 7474 7073 3a2f  1 [#977](https:/
-00000bd0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-00000be0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-00000bf0: 6e74 2f70 756c 6c2f 3937 3729 2028 5b40  nt/pull/977) ([@
-00000c00: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
-00000c10: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
-00000c20: 696e 6b31 3037 3329 290a 2d20 6368 6f72  ink1073)).- chor
-00000c30: 653a 2075 7064 6174 6520 7072 652d 636f  e: update pre-co
-00000c40: 6d6d 6974 2068 6f6f 6b73 205b 2339 3735  mmit hooks [#975
-00000c50: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000c60: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00000c70: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00000c80: 2f39 3735 2920 285b 4070 7265 2d63 6f6d  /975) ([@pre-com
-00000c90: 6d69 742d 6369 5d28 6874 7470 733a 2f2f  mit-ci](https://
-00000ca0: 6769 7468 7562 2e63 6f6d 2f70 7265 2d63  github.com/pre-c
-00000cb0: 6f6d 6d69 742d 6369 2929 0a2d 2055 7064  ommit-ci)).- Upd
-00000cc0: 6174 6520 7479 7069 6e67 7320 666f 7220  ate typings for 
-00000cd0: 7472 6169 746c 6574 7320 352e 3130 2e31  traitlets 5.10.1
-00000ce0: 205b 2339 3734 5d28 6874 7470 733a 2f2f   [#974](https://
-00000cf0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00000d00: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00000d10: 742f 7075 6c6c 2f39 3734 2920 285b 4062  t/pull/974) ([@b
-00000d20: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
-00000d30: 2f2f 6769 7468 7562 2e63 6f6d 2f62 6c69  //github.com/bli
-00000d40: 6e6b 3130 3733 2929 0a2d 2044 6f20 6e6f  nk1073)).- Do no
-00000d50: 7420 7573 6520 6461 7465 7469 6d65 2e75  t use datetime.u
-00000d60: 7463 6e6f 7728 2920 7468 6174 2069 7320  tcnow() that is 
-00000d70: 6465 7072 6563 6174 6564 2069 6e20 5079  deprecated in Py
-00000d80: 7468 6f6e 2033 2e31 3220 5b23 3937 325d  thon 3.12 [#972]
-00000d90: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000da0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-00000db0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-00000dc0: 3937 3229 2028 5b40 656c 6c65 7274 5d28  972) ([@ellert](
-00000dd0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000de0: 6f6d 2f65 6c6c 6572 7429 290a 2d20 5573  om/ellert)).- Us
-00000df0: 6520 7370 2d72 6570 6f2d 7265 7669 6577  e sp-repo-review
-00000e00: 205b 2339 3731 5d28 6874 7470 733a 2f2f   [#971](https://
-00000e10: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00000e20: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00000e30: 742f 7075 6c6c 2f39 3731 2920 285b 4062  t/pull/971) ([@b
-00000e40: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
-00000e50: 2f2f 6769 7468 7562 2e63 6f6d 2f62 6c69  //github.com/bli
-00000e60: 6e6b 3130 3733 2929 0a2d 2042 756d 7020  nk1073)).- Bump 
-00000e70: 6163 7469 6f6e 732f 6368 6563 6b6f 7574  actions/checkout
-00000e80: 2066 726f 6d20 3320 746f 2034 205b 2339   from 3 to 4 [#9
-00000e90: 3638 5d28 6874 7470 733a 2f2f 6769 7468  68](https://gith
-00000ea0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00000eb0: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-00000ec0: 6c6c 2f39 3638 2920 285b 4064 6570 656e  ll/968) ([@depen
-00000ed0: 6461 626f 745d 2868 7474 7073 3a2f 2f67  dabot](https://g
-00000ee0: 6974 6875 622e 636f 6d2f 6465 7065 6e64  ithub.com/depend
-00000ef0: 6162 6f74 2929 0a0a 2323 2320 436f 6e74  abot))..### Cont
-00000f00: 7269 6275 746f 7273 2074 6f20 7468 6973  ributors to this
-00000f10: 2072 656c 6561 7365 0a0a 285b 4769 7448   release..([GitH
-00000f20: 7562 2063 6f6e 7472 6962 7574 6f72 7320  ub contributors 
-00000f30: 7061 6765 2066 6f72 2074 6869 7320 7265  page for this re
-00000f40: 6c65 6173 655d 2868 7474 7073 3a2f 2f67  lease](https://g
-00000f50: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
-00000f60: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
-00000f70: 2f67 7261 7068 732f 636f 6e74 7269 6275  /graphs/contribu
-00000f80: 746f 7273 3f66 726f 6d3d 3230 3233 2d30  tors?from=2023-0
-00000f90: 382d 3239 2674 6f3d 3230 3233 2d31 302d  8-29&to=2023-10-
-00000fa0: 3131 2674 7970 653d 6329 290a 0a5b 4062  11&type=c))..[@b
-00000fb0: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
-00000fc0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
-00000fd0: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
-00000fe0: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
-00000ff0: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
-00001000: 4162 6c69 6e6b 3130 3733 2b75 7064 6174  Ablink1073+updat
-00001010: 6564 2533 4132 3032 332d 3038 2d32 392e  ed%3A2023-08-29.
-00001020: 2e32 3032 332d 3130 2d31 3126 7479 7065  .2023-10-11&type
-00001030: 3d49 7373 7565 7329 207c 205b 4064 6570  =Issues) | [@dep
-00001040: 656e 6461 626f 745d 2868 7474 7073 3a2f  endabot](https:/
-00001050: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-00001060: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-00001070: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-00001080: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-00001090: 6465 7065 6e64 6162 6f74 2b75 7064 6174  dependabot+updat
-000010a0: 6564 2533 4132 3032 332d 3038 2d32 392e  ed%3A2023-08-29.
-000010b0: 2e32 3032 332d 3130 2d31 3126 7479 7065  .2023-10-11&type
-000010c0: 3d49 7373 7565 7329 207c 205b 4065 6c6c  =Issues) | [@ell
-000010d0: 6572 745d 2868 7474 7073 3a2f 2f67 6974  ert](https://git
-000010e0: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
-000010f0: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
-00001100: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
-00001110: 2b69 6e76 6f6c 7665 7325 3341 656c 6c65  +involves%3Aelle
-00001120: 7274 2b75 7064 6174 6564 2533 4132 3032  rt+updated%3A202
-00001130: 332d 3038 2d32 392e 2e32 3032 332d 3130  3-08-29..2023-10
-00001140: 2d31 3126 7479 7065 3d49 7373 7565 7329  -11&type=Issues)
-00001150: 207c 205b 4070 7265 2d63 6f6d 6d69 742d   | [@pre-commit-
-00001160: 6369 5d28 6874 7470 733a 2f2f 6769 7468  ci](https://gith
-00001170: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
-00001180: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
-00001190: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
-000011a0: 696e 766f 6c76 6573 2533 4170 7265 2d63  involves%3Apre-c
-000011b0: 6f6d 6d69 742d 6369 2b75 7064 6174 6564  ommit-ci+updated
-000011c0: 2533 4132 3032 332d 3038 2d32 392e 2e32  %3A2023-08-29..2
-000011d0: 3032 332d 3130 2d31 3126 7479 7065 3d49  023-10-11&type=I
-000011e0: 7373 7565 7329 0a0a 2323 2038 2e33 2e31  ssues)..## 8.3.1
-000011f0: 0a0a 285b 4675 6c6c 2043 6861 6e67 656c  ..([Full Changel
-00001200: 6f67 5d28 6874 7470 733a 2f2f 6769 7468  og](https://gith
-00001210: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00001220: 7570 7974 6572 5f63 6c69 656e 742f 636f  upyter_client/co
-00001230: 6d70 6172 652f 7638 2e33 2e30 2e2e 2e62  mpare/v8.3.0...b
-00001240: 3466 3764 3934 3766 6165 3535 6134 6665  4f7d947fae55a4fe
-00001250: 3539 6132 3764 6630 3833 3061 3961 3738  59a27df0830a9a78
-00001260: 6463 6434 6531 3229 290a 0a23 2323 2045  dcd4e12))..### E
-00001270: 6e68 616e 6365 6d65 6e74 7320 6d61 6465  nhancements made
-00001280: 0a0a 2d20 5375 7070 6f72 7420 6578 7465  ..- Support exte
-00001290: 726e 616c 206b 6572 6e65 6c73 205b 2339  rnal kernels [#9
-000012a0: 3631 5d28 6874 7470 733a 2f2f 6769 7468  61](https://gith
-000012b0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-000012c0: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-000012d0: 6c6c 2f39 3631 2920 285b 4064 6176 6964  ll/961) ([@david
-000012e0: 6272 6f63 6861 7274 5d28 6874 7470 733a  brochart](https:
-000012f0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6176  //github.com/dav
-00001300: 6964 6272 6f63 6861 7274 2929 0a0a 2323  idbrochart))..##
-00001310: 2320 4275 6773 2066 6978 6564 0a0a 2d20  # Bugs fixed..- 
-00001320: 4d61 6b65 2063 6163 6865 5f70 6f72 7473  Make cache_ports
-00001330: 2063 6f6e 6669 6775 7261 626c 6520 7769   configurable wi
-00001340: 7468 2064 6566 6175 6c74 2076 616c 7565  th default value
-00001350: 206f 6620 4661 6c73 652e 205b 2339 3536   of False. [#956
-00001360: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001370: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00001380: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00001390: 2f39 3536 2920 285b 406a 6b69 7463 6869  /956) ([@jkitchi
-000013a0: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
-000013b0: 622e 636f 6d2f 6a6b 6974 6368 696e 2929  b.com/jkitchin))
-000013c0: 0a0a 2323 2320 4d61 696e 7465 6e61 6e63  ..### Maintenanc
-000013d0: 6520 616e 6420 7570 6b65 6570 2069 6d70  e and upkeep imp
-000013e0: 726f 7665 6d65 6e74 730a 0a23 2323 2043  rovements..### C
-000013f0: 6f6e 7472 6962 7574 6f72 7320 746f 2074  ontributors to t
-00001400: 6869 7320 7265 6c65 6173 650a 0a28 5b47  his release..([G
-00001410: 6974 4875 6220 636f 6e74 7269 6275 746f  itHub contributo
-00001420: 7273 2070 6167 6520 666f 7220 7468 6973  rs page for this
-00001430: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
-00001440: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-00001450: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-00001460: 656e 742f 6772 6170 6873 2f63 6f6e 7472  ent/graphs/contr
-00001470: 6962 7574 6f72 733f 6672 6f6d 3d32 3032  ibutors?from=202
-00001480: 332d 3036 2d32 3326 746f 3d32 3032 332d  3-06-23&to=2023-
-00001490: 3038 2d32 3926 7479 7065 3d63 2929 0a0a  08-29&type=c))..
-000014a0: 5b40 626c 696e 6b31 3037 335d 2868 7474  [@blink1073](htt
-000014b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000014c0: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
-000014d0: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
-000014e0: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
-000014f0: 7325 3341 626c 696e 6b31 3037 332b 7570  s%3Ablink1073+up
-00001500: 6461 7465 6425 3341 3230 3233 2d30 362d  dated%3A2023-06-
-00001510: 3233 2e2e 3230 3233 2d30 382d 3239 2674  23..2023-08-29&t
-00001520: 7970 653d 4973 7375 6573 2920 7c20 5b40  ype=Issues) | [@
-00001530: 6461 7669 6462 726f 6368 6172 745d 2868  davidbrochart](h
-00001540: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001550: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
-00001560: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
-00001570: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
-00001580: 7665 7325 3341 6461 7669 6462 726f 6368  ves%3Adavidbroch
-00001590: 6172 742b 7570 6461 7465 6425 3341 3230  art+updated%3A20
-000015a0: 3233 2d30 362d 3233 2e2e 3230 3233 2d30  23-06-23..2023-0
-000015b0: 382d 3239 2674 7970 653d 4973 7375 6573  8-29&type=Issues
-000015c0: 2920 7c20 5b40 6a6b 6974 6368 696e 5d28  ) | [@jkitchin](
-000015d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000015e0: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
-000015f0: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
-00001600: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
-00001610: 6c76 6573 2533 416a 6b69 7463 6869 6e2b  lves%3Ajkitchin+
-00001620: 7570 6461 7465 6425 3341 3230 3233 2d30  updated%3A2023-0
-00001630: 362d 3233 2e2e 3230 3233 2d30 382d 3239  6-23..2023-08-29
-00001640: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
-00001650: 5b40 6b65 7669 6e2d 6261 7465 735d 2868  [@kevin-bates](h
-00001660: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001670: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
-00001680: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
-00001690: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
-000016a0: 7665 7325 3341 6b65 7669 6e2d 6261 7465  ves%3Akevin-bate
-000016b0: 732b 7570 6461 7465 6425 3341 3230 3233  s+updated%3A2023
-000016c0: 2d30 362d 3233 2e2e 3230 3233 2d30 382d  -06-23..2023-08-
-000016d0: 3239 2674 7970 653d 4973 7375 6573 2920  29&type=Issues) 
-000016e0: 7c20 5b40 7072 652d 636f 6d6d 6974 2d63  | [@pre-commit-c
-000016f0: 695d 2868 7474 7073 3a2f 2f67 6974 6875  i](https://githu
-00001700: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
-00001710: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
-00001720: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
-00001730: 6e76 6f6c 7665 7325 3341 7072 652d 636f  nvolves%3Apre-co
-00001740: 6d6d 6974 2d63 692b 7570 6461 7465 6425  mmit-ci+updated%
-00001750: 3341 3230 3233 2d30 362d 3233 2e2e 3230  3A2023-06-23..20
-00001760: 3233 2d30 382d 3239 2674 7970 653d 4973  23-08-29&type=Is
-00001770: 7375 6573 2920 7c20 5b40 746d 6178 7765  sues) | [@tmaxwe
-00001780: 6c6c 2d61 6e74 6872 6f70 6963 5d28 6874  ll-anthropic](ht
-00001790: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000017a0: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
-000017b0: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
-000017c0: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
-000017d0: 6573 2533 4174 6d61 7877 656c 6c2d 616e  es%3Atmaxwell-an
-000017e0: 7468 726f 7069 632b 7570 6461 7465 6425  thropic+updated%
-000017f0: 3341 3230 3233 2d30 362d 3233 2e2e 3230  3A2023-06-23..20
-00001800: 3233 2d30 382d 3239 2674 7970 653d 4973  23-08-29&type=Is
-00001810: 7375 6573 290a 0a23 2320 382e 332e 300a  sues)..## 8.3.0.
-00001820: 0a28 5b46 756c 6c20 4368 616e 6765 6c6f  .([Full Changelo
-00001830: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
-00001840: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-00001850: 7079 7465 725f 636c 6965 6e74 2f63 6f6d  pyter_client/com
-00001860: 7061 7265 2f76 382e 322e 302e 2e2e 6264  pare/v8.2.0...bd
-00001870: 6462 3838 3534 6134 6161 3333 3234 6531  db8854a4aa3324e1
-00001880: 3238 6530 3439 3735 3339 6531 3732 3436  28e0497539e17246
-00001890: 6662 6636 3330 2929 0a0a 2323 2320 456e  fbf630))..### En
-000018a0: 6861 6e63 656d 656e 7473 206d 6164 650a  hancements made.
-000018b0: 0a2d 2041 6c6c 6f77 206b 7761 7267 7320  .- Allow kwargs 
-000018c0: 7768 656e 2077 7269 7469 6e67 2063 6f6e  when writing con
-000018d0: 6e65 6374 696f 6e5f 6669 6c65 205b 2339  nection_file [#9
-000018e0: 3533 5d28 6874 7470 733a 2f2f 6769 7468  53](https://gith
-000018f0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00001900: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-00001910: 6c6c 2f39 3533 2920 285b 4066 6563 6574  ll/953) ([@fecet
-00001920: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001930: 2e63 6f6d 2f66 6563 6574 2929 0a0a 2323  .com/fecet))..##
-00001940: 2320 4d61 696e 7465 6e61 6e63 6520 616e  # Maintenance an
-00001950: 6420 7570 6b65 6570 2069 6d70 726f 7665  d upkeep improve
-00001960: 6d65 6e74 730a 0a23 2323 2043 6f6e 7472  ments..### Contr
-00001970: 6962 7574 6f72 7320 746f 2074 6869 7320  ibutors to this 
-00001980: 7265 6c65 6173 650a 0a28 5b47 6974 4875  release..([GitHu
-00001990: 6220 636f 6e74 7269 6275 746f 7273 2070  b contributors p
-000019a0: 6167 6520 666f 7220 7468 6973 2072 656c  age for this rel
-000019b0: 6561 7365 5d28 6874 7470 733a 2f2f 6769  ease](https://gi
-000019c0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-000019d0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-000019e0: 6772 6170 6873 2f63 6f6e 7472 6962 7574  graphs/contribut
-000019f0: 6f72 733f 6672 6f6d 3d32 3032 332d 3034  ors?from=2023-04
-00001a00: 2d31 3326 746f 3d32 3032 332d 3036 2d32  -13&to=2023-06-2
-00001a10: 3326 7479 7065 3d63 2929 0a0a 5b40 6665  3&type=c))..[@fe
-00001a20: 6365 745d 2868 7474 7073 3a2f 2f67 6974  cet](https://git
-00001a30: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
-00001a40: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
-00001a50: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
-00001a60: 2b69 6e76 6f6c 7665 7325 3341 6665 6365  +involves%3Afece
-00001a70: 742b 7570 6461 7465 6425 3341 3230 3233  t+updated%3A2023
-00001a80: 2d30 342d 3133 2e2e 3230 3233 2d30 362d  -04-13..2023-06-
-00001a90: 3233 2674 7970 653d 4973 7375 6573 2920  23&type=Issues) 
-00001aa0: 7c20 5b40 7072 652d 636f 6d6d 6974 2d63  | [@pre-commit-c
-00001ab0: 695d 2868 7474 7073 3a2f 2f67 6974 6875  i](https://githu
-00001ac0: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
-00001ad0: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
-00001ae0: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
-00001af0: 6e76 6f6c 7665 7325 3341 7072 652d 636f  nvolves%3Apre-co
-00001b00: 6d6d 6974 2d63 692b 7570 6461 7465 6425  mmit-ci+updated%
-00001b10: 3341 3230 3233 2d30 342d 3133 2e2e 3230  3A2023-04-13..20
-00001b20: 3233 2d30 362d 3233 2674 7970 653d 4973  23-06-23&type=Is
-00001b30: 7375 6573 290a 0a23 2320 382e 322e 300a  sues)..## 8.2.0.
-00001b40: 0a28 5b46 756c 6c20 4368 616e 6765 6c6f  .([Full Changelo
-00001b50: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
-00001b60: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-00001b70: 7079 7465 725f 636c 6965 6e74 2f63 6f6d  pyter_client/com
-00001b80: 7061 7265 2f76 382e 312e 302e 2e2e 6462  pare/v8.1.0...db
-00001b90: 6636 6238 3166 6135 6162 3630 3665 6165  f6b81fa5ab606eae
-00001ba0: 6463 3565 3864 3038 3433 6465 6263 6531  dc5e8d0843debce1
-00001bb0: 3865 3837 3436 2929 0a0a 2323 2320 456e  8e8746))..### En
-00001bc0: 6861 6e63 656d 656e 7473 206d 6164 650a  hancements made.
-00001bd0: 0a2d 2075 7365 2063 2e66 2e46 7574 7572  .- use c.f.Futur
-00001be0: 6520 746f 2077 6169 7420 6163 726f 7373  e to wait across
-00001bf0: 2074 6872 6561 6473 205b 2339 3430 5d28   threads [#940](
-00001c00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001c10: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-00001c20: 6572 5f63 6c69 656e 742f 7075 6c6c 2f39  er_client/pull/9
-00001c30: 3430 2920 285b 406d 696e 726b 5d28 6874  40) ([@minrk](ht
-00001c40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001c50: 2f6d 696e 726b 2929 0a0a 2323 2320 4d61  /minrk))..### Ma
-00001c60: 696e 7465 6e61 6e63 6520 616e 6420 7570  intenance and up
-00001c70: 6b65 6570 2069 6d70 726f 7665 6d65 6e74  keep improvement
-00001c80: 730a 0a2d 2055 7365 206c 6f63 616c 2063  s..- Use local c
-00001c90: 6f76 6572 6167 6520 5b23 3934 355d 2868  overage [#945](h
-00001ca0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001cb0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00001cc0: 725f 636c 6965 6e74 2f70 756c 6c2f 3934  r_client/pull/94
-00001cd0: 3529 2028 5b40 626c 696e 6b31 3037 335d  5) ([@blink1073]
-00001ce0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001cf0: 636f 6d2f 626c 696e 6b31 3037 3329 290a  com/blink1073)).
-00001d00: 2d20 4164 6420 6d6f 7265 2070 726f 6a65  - Add more proje
-00001d10: 6374 2055 524c 7320 5b23 3934 345d 2868  ct URLs [#944](h
-00001d20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001d30: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00001d40: 725f 636c 6965 6e74 2f70 756c 6c2f 3934  r_client/pull/94
-00001d50: 3429 2028 5b40 6663 6f6c 6c6f 6e76 616c  4) ([@fcollonval
-00001d60: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001d70: 2e63 6f6d 2f66 636f 6c6c 6f6e 7661 6c29  .com/fcollonval)
-00001d80: 290a 0a23 2323 2043 6f6e 7472 6962 7574  )..### Contribut
-00001d90: 6f72 7320 746f 2074 6869 7320 7265 6c65  ors to this rele
-00001da0: 6173 650a 0a28 5b47 6974 4875 6220 636f  ase..([GitHub co
-00001db0: 6e74 7269 6275 746f 7273 2070 6167 6520  ntributors page 
-00001dc0: 666f 7220 7468 6973 2072 656c 6561 7365  for this release
-00001dd0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001de0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00001df0: 7974 6572 5f63 6c69 656e 742f 6772 6170  yter_client/grap
-00001e00: 6873 2f63 6f6e 7472 6962 7574 6f72 733f  hs/contributors?
-00001e10: 6672 6f6d 3d32 3032 332d 3033 2d32 3026  from=2023-03-20&
-00001e20: 746f 3d32 3032 332d 3034 2d31 3326 7479  to=2023-04-13&ty
-00001e30: 7065 3d63 2929 0a0a 5b40 626c 696e 6b31  pe=c))..[@blink1
-00001e40: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
-00001e50: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
-00001e60: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
-00001e70: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
-00001e80: 2b69 6e76 6f6c 7665 7325 3341 626c 696e  +involves%3Ablin
-00001e90: 6b31 3037 332b 7570 6461 7465 6425 3341  k1073+updated%3A
-00001ea0: 3230 3233 2d30 332d 3230 2e2e 3230 3233  2023-03-20..2023
-00001eb0: 2d30 342d 3133 2674 7970 653d 4973 7375  -04-13&type=Issu
-00001ec0: 6573 2920 7c20 5b40 6663 6f6c 6c6f 6e76  es) | [@fcollonv
-00001ed0: 616c 5d28 6874 7470 733a 2f2f 6769 7468  al](https://gith
-00001ee0: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
-00001ef0: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
-00001f00: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
-00001f10: 696e 766f 6c76 6573 2533 4166 636f 6c6c  involves%3Afcoll
-00001f20: 6f6e 7661 6c2b 7570 6461 7465 6425 3341  onval+updated%3A
-00001f30: 3230 3233 2d30 332d 3230 2e2e 3230 3233  2023-03-20..2023
-00001f40: 2d30 342d 3133 2674 7970 653d 4973 7375  -04-13&type=Issu
-00001f50: 6573 2920 7c20 5b40 6d69 6e72 6b5d 2868  es) | [@minrk](h
-00001f60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001f70: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
-00001f80: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
-00001f90: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
-00001fa0: 7665 7325 3341 6d69 6e72 6b2b 7570 6461  ves%3Aminrk+upda
-00001fb0: 7465 6425 3341 3230 3233 2d30 332d 3230  ted%3A2023-03-20
-00001fc0: 2e2e 3230 3233 2d30 342d 3133 2674 7970  ..2023-04-13&typ
-00001fd0: 653d 4973 7375 6573 2920 7c20 5b40 7072  e=Issues) | [@pr
-00001fe0: 652d 636f 6d6d 6974 2d63 695d 2868 7474  e-commit-ci](htt
-00001ff0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002000: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
-00002010: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
-00002020: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
-00002030: 7325 3341 7072 652d 636f 6d6d 6974 2d63  s%3Apre-commit-c
-00002040: 692b 7570 6461 7465 6425 3341 3230 3233  i+updated%3A2023
-00002050: 2d30 332d 3230 2e2e 3230 3233 2d30 342d  -03-20..2023-04-
-00002060: 3133 2674 7970 653d 4973 7375 6573 290a  13&type=Issues).
-00002070: 0a23 2320 382e 312e 300a 0a28 5b46 756c  .## 8.1.0..([Ful
-00002080: 6c20 4368 616e 6765 6c6f 675d 2868 7474  l Changelog](htt
-00002090: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000020a0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-000020b0: 636c 6965 6e74 2f63 6f6d 7061 7265 2f76  client/compare/v
-000020c0: 382e 302e 332e 2e2e 6533 6163 3761 3639  8.0.3...e3ac7a69
-000020d0: 3335 3564 6431 6166 3636 3033 3865 6461  355dd1af66038eda
-000020e0: 3736 3765 3531 6539 3265 6630 3334 6662  767e51e92ef034fb
-000020f0: 2929 0a0a 2323 2320 4275 6773 2066 6978  ))..### Bugs fix
-00002100: 6564 0a0a 2d20 5468 7265 6164 6564 5a4d  ed..- ThreadedZM
-00002110: 5153 7472 6561 6d3a 2063 6c6f 7365 2073  QStream: close s
-00002120: 7472 6561 6d20 6265 666f 7265 2073 6f63  tream before soc
-00002130: 6b65 7420 5b23 3933 365d 2868 7474 7073  ket [#936](https
-00002140: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00002150: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-00002160: 6965 6e74 2f70 756c 6c2f 3933 3629 2028  ient/pull/936) (
-00002170: 5b40 6d69 6e72 6b5d 2868 7474 7073 3a2f  [@minrk](https:/
-00002180: 2f67 6974 6875 622e 636f 6d2f 6d69 6e72  /github.com/minr
-00002190: 6b29 290a 0a23 2323 204d 6169 6e74 656e  k))..### Mainten
-000021a0: 616e 6365 2061 6e64 2075 706b 6565 7020  ance and upkeep 
-000021b0: 696d 7072 6f76 656d 656e 7473 0a0a 2323  improvements..##
-000021c0: 2320 446f 6375 6d65 6e74 6174 696f 6e20  # Documentation 
-000021d0: 696d 7072 6f76 656d 656e 7473 0a0a 2d20  improvements..- 
-000021e0: 4164 6473 2073 7065 6320 666f 7220 7468  Adds spec for th
-000021f0: 6520 636f 7079 546f 476c 6f62 616c 7320  e copyToGlobals 
-00002200: 7265 7175 6573 7420 5b23 3933 325d 2868  request [#932](h
-00002210: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002220: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00002230: 725f 636c 6965 6e74 2f70 756c 6c2f 3933  r_client/pull/93
-00002240: 3229 2028 5b40 6272 6963 6865 745d 2868  2) ([@brichet](h
-00002250: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002260: 6d2f 6272 6963 6865 7429 290a 0a23 2323  m/brichet))..###
-00002270: 2043 6f6e 7472 6962 7574 6f72 7320 746f   Contributors to
-00002280: 2074 6869 7320 7265 6c65 6173 650a 0a28   this release..(
-00002290: 5b47 6974 4875 6220 636f 6e74 7269 6275  [GitHub contribu
-000022a0: 746f 7273 2070 6167 6520 666f 7220 7468  tors page for th
-000022b0: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
-000022c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000022d0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-000022e0: 6c69 656e 742f 6772 6170 6873 2f63 6f6e  lient/graphs/con
-000022f0: 7472 6962 7574 6f72 733f 6672 6f6d 3d32  tributors?from=2
-00002300: 3032 332d 3032 2d31 3626 746f 3d32 3032  023-02-16&to=202
-00002310: 332d 3033 2d32 3026 7479 7065 3d63 2929  3-03-20&type=c))
-00002320: 0a0a 5b40 626c 696e 6b31 3037 335d 2868  ..[@blink1073](h
-00002330: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002340: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
-00002350: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
-00002360: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
-00002370: 7665 7325 3341 626c 696e 6b31 3037 332b  ves%3Ablink1073+
-00002380: 7570 6461 7465 6425 3341 3230 3233 2d30  updated%3A2023-0
-00002390: 322d 3136 2e2e 3230 3233 2d30 332d 3230  2-16..2023-03-20
-000023a0: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
-000023b0: 5b40 6272 6963 6865 745d 2868 7474 7073  [@brichet](https
-000023c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
-000023d0: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
-000023e0: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
-000023f0: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
-00002400: 3341 6272 6963 6865 742b 7570 6461 7465  3Abrichet+update
-00002410: 6425 3341 3230 3233 2d30 322d 3136 2e2e  d%3A2023-02-16..
-00002420: 3230 3233 2d30 332d 3230 2674 7970 653d  2023-03-20&type=
-00002430: 4973 7375 6573 2920 7c20 5b40 6d69 6e72  Issues) | [@minr
-00002440: 6b5d 2868 7474 7073 3a2f 2f67 6974 6875  k](https://githu
-00002450: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
-00002460: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
-00002470: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
-00002480: 6e76 6f6c 7665 7325 3341 6d69 6e72 6b2b  nvolves%3Aminrk+
-00002490: 7570 6461 7465 6425 3341 3230 3233 2d30  updated%3A2023-0
-000024a0: 322d 3136 2e2e 3230 3233 2d30 332d 3230  2-16..2023-03-20
-000024b0: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
-000024c0: 5b40 7072 652d 636f 6d6d 6974 2d63 695d  [@pre-commit-ci]
-000024d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000024e0: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
-000024f0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
-00002500: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
-00002510: 6f6c 7665 7325 3341 7072 652d 636f 6d6d  olves%3Apre-comm
-00002520: 6974 2d63 692b 7570 6461 7465 6425 3341  it-ci+updated%3A
-00002530: 3230 3233 2d30 322d 3136 2e2e 3230 3233  2023-02-16..2023
-00002540: 2d30 332d 3230 2674 7970 653d 4973 7375  -03-20&type=Issu
-00002550: 6573 290a 0a23 2320 382e 302e 330a 0a28  es)..## 8.0.3..(
-00002560: 5b46 756c 6c20 4368 616e 6765 6c6f 675d  [Full Changelog]
-00002570: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002580: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-00002590: 7465 725f 636c 6965 6e74 2f63 6f6d 7061  ter_client/compa
-000025a0: 7265 2f76 382e 302e 322e 2e2e 6463 3065  re/v8.0.2...dc0e
-000025b0: 6162 6131 6636 3039 3037 3936 3732 6563  aba1f609079672ec
-000025c0: 3733 3966 6364 3937 3764 6334 3434 3331  739fcd977dc44431
-000025d0: 6461 3932 2929 0a0a 2323 2320 4275 6773  da92))..### Bugs
-000025e0: 2066 6978 6564 0a0a 2d20 4669 7820 6b65   fixed..- Fix ke
-000025f0: 726e 656c 7370 6563 2070 7269 6e74 206f  rnelspec print o
-00002600: 7574 7075 7420 5b23 3933 335d 2868 7474  utput [#933](htt
-00002610: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002620: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00002630: 636c 6965 6e74 2f70 756c 6c2f 3933 3329  client/pull/933)
-00002640: 2028 5b40 6d69 6e72 6b5d 2868 7474 7073   ([@minrk](https
-00002650: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d69  ://github.com/mi
-00002660: 6e72 6b29 290a 2d20 446f 6e27 7420 656d  nrk)).- Don't em
-00002670: 6974 2061 2074 7261 696c 6e67 206e 6577  it a trailng new
-00002680: 6c69 6e65 2069 6e20 6261 7365 3634 2d65  line in base64-e
-00002690: 6e63 6f64 6564 2064 6174 6120 6c69 6b65  ncoded data like
-000026a0: 2027 696d 6167 652f 706e 6727 205b 2339   'image/png' [#9
-000026b0: 3331 5d28 6874 7470 733a 2f2f 6769 7468  31](https://gith
-000026c0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-000026d0: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-000026e0: 6c6c 2f39 3331 2920 285b 4078 6c30 5d28  ll/931) ([@xl0](
-000026f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002700: 6f6d 2f78 6c30 2929 0a0a 2323 2320 4d61  om/xl0))..### Ma
-00002710: 696e 7465 6e61 6e63 6520 616e 6420 7570  intenance and up
-00002720: 6b65 6570 2069 6d70 726f 7665 6d65 6e74  keep improvement
-00002730: 730a 0a2d 2041 6464 206c 6963 656e 7365  s..- Add license
-00002740: 205b 2339 3334 5d28 6874 7470 733a 2f2f   [#934](https://
-00002750: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00002760: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00002770: 742f 7075 6c6c 2f39 3334 2920 285b 4064  t/pull/934) ([@d
-00002780: 6373 6162 6138 395d 2868 7474 7073 3a2f  csaba89](https:/
-00002790: 2f67 6974 6875 622e 636f 6d2f 6463 7361  /github.com/dcsa
-000027a0: 6261 3839 2929 0a2d 2049 6d70 726f 7669  ba89)).- Improvi
-000027b0: 6e67 206a 736f 6e75 7469 6c20 7465 7374  ng jsonutil test
-000027c0: 7320 5b23 3932 395d 2868 7474 7073 3a2f  s [#929](https:/
-000027d0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-000027e0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-000027f0: 6e74 2f70 756c 6c2f 3932 3929 2028 5b40  nt/pull/929) ([@
-00002800: 616e 6472 6568 6f72 615d 2868 7474 7073  andrehora](https
-00002810: 3a2f 2f67 6974 6875 622e 636f 6d2f 616e  ://github.com/an
-00002820: 6472 6568 6f72 6129 290a 0a23 2323 2043  drehora))..### C
-00002830: 6f6e 7472 6962 7574 6f72 7320 746f 2074  ontributors to t
-00002840: 6869 7320 7265 6c65 6173 650a 0a28 5b47  his release..([G
-00002850: 6974 4875 6220 636f 6e74 7269 6275 746f  itHub contributo
-00002860: 7273 2070 6167 6520 666f 7220 7468 6973  rs page for this
-00002870: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
-00002880: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-00002890: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-000028a0: 656e 742f 6772 6170 6873 2f63 6f6e 7472  ent/graphs/contr
-000028b0: 6962 7574 6f72 733f 6672 6f6d 3d32 3032  ibutors?from=202
-000028c0: 332d 3031 2d33 3026 746f 3d32 3032 332d  3-01-30&to=2023-
-000028d0: 3032 2d31 3626 7479 7065 3d63 2929 0a0a  02-16&type=c))..
-000028e0: 5b40 616e 6472 6568 6f72 615d 2868 7474  [@andrehora](htt
-000028f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002900: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
-00002910: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
-00002920: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
-00002930: 7325 3341 616e 6472 6568 6f72 612b 7570  s%3Aandrehora+up
-00002940: 6461 7465 6425 3341 3230 3233 2d30 312d  dated%3A2023-01-
-00002950: 3330 2e2e 3230 3233 2d30 322d 3136 2674  30..2023-02-16&t
-00002960: 7970 653d 4973 7375 6573 2920 7c20 5b40  ype=Issues) | [@
-00002970: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
-00002980: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
-00002990: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
-000029a0: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
-000029b0: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
-000029c0: 3341 626c 696e 6b31 3037 332b 7570 6461  3Ablink1073+upda
-000029d0: 7465 6425 3341 3230 3233 2d30 312d 3330  ted%3A2023-01-30
-000029e0: 2e2e 3230 3233 2d30 322d 3136 2674 7970  ..2023-02-16&typ
-000029f0: 653d 4973 7375 6573 2920 7c20 5b40 6463  e=Issues) | [@dc
-00002a00: 7361 6261 3839 5d28 6874 7470 733a 2f2f  saba89](https://
-00002a10: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
-00002a20: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
-00002a30: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
-00002a40: 656e 742b 696e 766f 6c76 6573 2533 4164  ent+involves%3Ad
-00002a50: 6373 6162 6138 392b 7570 6461 7465 6425  csaba89+updated%
-00002a60: 3341 3230 3233 2d30 312d 3330 2e2e 3230  3A2023-01-30..20
-00002a70: 3233 2d30 322d 3136 2674 7970 653d 4973  23-02-16&type=Is
-00002a80: 7375 6573 2920 7c20 5b40 6b65 7669 6e2d  sues) | [@kevin-
-00002a90: 6261 7465 735d 2868 7474 7073 3a2f 2f67  bates](https://g
-00002aa0: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
-00002ab0: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
-00002ac0: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
-00002ad0: 6e74 2b69 6e76 6f6c 7665 7325 3341 6b65  nt+involves%3Ake
-00002ae0: 7669 6e2d 6261 7465 732b 7570 6461 7465  vin-bates+update
-00002af0: 6425 3341 3230 3233 2d30 312d 3330 2e2e  d%3A2023-01-30..
-00002b00: 3230 3233 2d30 322d 3136 2674 7970 653d  2023-02-16&type=
-00002b10: 4973 7375 6573 2920 7c20 5b40 6d69 6e72  Issues) | [@minr
-00002b20: 6b5d 2868 7474 7073 3a2f 2f67 6974 6875  k](https://githu
-00002b30: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
-00002b40: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
-00002b50: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
-00002b60: 6e76 6f6c 7665 7325 3341 6d69 6e72 6b2b  nvolves%3Aminrk+
-00002b70: 7570 6461 7465 6425 3341 3230 3233 2d30  updated%3A2023-0
-00002b80: 312d 3330 2e2e 3230 3233 2d30 322d 3136  1-30..2023-02-16
-00002b90: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
-00002ba0: 5b40 7072 652d 636f 6d6d 6974 2d63 695d  [@pre-commit-ci]
-00002bb0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002bc0: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
-00002bd0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
-00002be0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
-00002bf0: 6f6c 7665 7325 3341 7072 652d 636f 6d6d  olves%3Apre-comm
-00002c00: 6974 2d63 692b 7570 6461 7465 6425 3341  it-ci+updated%3A
-00002c10: 3230 3233 2d30 312d 3330 2e2e 3230 3233  2023-01-30..2023
-00002c20: 2d30 322d 3136 2674 7970 653d 4973 7375  -02-16&type=Issu
-00002c30: 6573 2920 7c20 5b40 786c 305d 2868 7474  es) | [@xl0](htt
-00002c40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002c50: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
-00002c60: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
-00002c70: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
-00002c80: 7325 3341 786c 302b 7570 6461 7465 6425  s%3Axl0+updated%
-00002c90: 3341 3230 3233 2d30 312d 3330 2e2e 3230  3A2023-01-30..20
-00002ca0: 3233 2d30 322d 3136 2674 7970 653d 4973  23-02-16&type=Is
-00002cb0: 7375 6573 290a 0a23 2320 382e 302e 320a  sues)..## 8.0.2.
-00002cc0: 0a28 5b46 756c 6c20 4368 616e 6765 6c6f  .([Full Changelo
-00002cd0: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
-00002ce0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-00002cf0: 7079 7465 725f 636c 6965 6e74 2f63 6f6d  pyter_client/com
-00002d00: 7061 7265 2f76 382e 302e 312e 2e2e 3731  pare/v8.0.1...71
-00002d10: 3764 3336 6564 6364 3963 6535 3935 6637  7d36edcd9ce595f7
-00002d20: 3237 6438 6235 6132 3765 3237 3063 3261  27d8b5a27e270c2a
-00002d30: 3665 3263 3436 2929 0a0a 2323 2320 4275  6e2c46))..### Bu
-00002d40: 6773 2066 6978 6564 0a0a 2d20 4164 6420  gs fixed..- Add 
-00002d50: 7061 7065 726d 696c 6c20 646f 776e 7374  papermill downst
-00002d60: 7265 616d 2063 6865 636b 2061 6e64 2066  ream check and f
-00002d70: 6978 206b 6572 6e65 6c20 636c 6965 6e74  ix kernel client
-00002d80: 2072 6570 6c69 6573 205b 2339 3235 5d28   replies [#925](
+000000a0: 2e36 2e30 2e2e 2e38 6133 3332 3761 6535  .6.0...8a3327ae5
+000000b0: 3832 3437 6265 3733 3464 3531 6634 3463  8247be734d51f44c
+000000c0: 3632 3933 3534 6630 6636 3030 3636 3029  629354f0f600660)
+000000d0: 290a 0a23 2323 204d 6169 6e74 656e 616e  )..### Maintenan
+000000e0: 6365 2061 6e64 2075 706b 6565 7020 696d  ce and upkeep im
+000000f0: 7072 6f76 656d 656e 7473 0a0a 2d20 5570  provements..- Up
+00000100: 6461 7465 2052 656c 6561 7365 2053 6372  date Release Scr
+00000110: 6970 7473 205b 2331 3031 365d 2868 7474  ipts [#1016](htt
+00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000130: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00000140: 636c 6965 6e74 2f70 756c 6c2f 3130 3136  client/pull/1016
+00000150: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
+00000160: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000170: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a2d  om/blink1073)).-
+00000180: 2063 686f 7265 3a20 7570 6461 7465 2070   chore: update p
+00000190: 7265 2d63 6f6d 6d69 7420 686f 6f6b 7320  re-commit hooks 
+000001a0: 5b23 3130 3038 5d28 6874 7470 733a 2f2f  [#1008](https://
+000001b0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+000001c0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+000001d0: 742f 7075 6c6c 2f31 3030 3829 2028 5b40  t/pull/1008) ([@
+000001e0: 7072 652d 636f 6d6d 6974 2d63 695d 2868  pre-commit-ci](h
+000001f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000200: 6d2f 7072 652d 636f 6d6d 6974 2d63 6929  m/pre-commit-ci)
+00000210: 290a 2d20 6368 6f72 653a 2075 7064 6174  ).- chore: updat
+00000220: 6520 7072 652d 636f 6d6d 6974 2068 6f6f  e pre-commit hoo
+00000230: 6b73 205b 2331 3030 325d 2868 7474 7073  ks [#1002](https
+00000240: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00000250: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+00000260: 6965 6e74 2f70 756c 6c2f 3130 3032 2920  ient/pull/1002) 
+00000270: 285b 4070 7265 2d63 6f6d 6d69 742d 6369  ([@pre-commit-ci
+00000280: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000290: 2e63 6f6d 2f70 7265 2d63 6f6d 6d69 742d  .com/pre-commit-
+000002a0: 6369 2929 0a2d 2042 756d 7020 6163 7469  ci)).- Bump acti
+000002b0: 6f6e 732f 7365 7475 702d 7079 7468 6f6e  ons/setup-python
+000002c0: 2066 726f 6d20 3420 746f 2035 205b 2331   from 4 to 5 [#1
+000002d0: 3030 305d 2868 7474 7073 3a2f 2f67 6974  000](https://git
+000002e0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+000002f0: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+00000300: 756c 6c2f 3130 3030 2920 285b 4064 6570  ull/1000) ([@dep
+00000310: 656e 6461 626f 745d 2868 7474 7073 3a2f  endabot](https:/
+00000320: 2f67 6974 6875 622e 636f 6d2f 6465 7065  /github.com/depe
+00000330: 6e64 6162 6f74 2929 0a2d 2063 686f 7265  ndabot)).- chore
+00000340: 3a20 7570 6461 7465 2070 7265 2d63 6f6d  : update pre-com
+00000350: 6d69 7420 686f 6f6b 7320 5b23 3939 395d  mit hooks [#999]
+00000360: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000370: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00000380: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00000390: 3939 3929 2028 5b40 7072 652d 636f 6d6d  999) ([@pre-comm
+000003a0: 6974 2d63 695d 2868 7474 7073 3a2f 2f67  it-ci](https://g
+000003b0: 6974 6875 622e 636f 6d2f 7072 652d 636f  ithub.com/pre-co
+000003c0: 6d6d 6974 2d63 6929 290a 2d20 4275 6d70  mmit-ci)).- Bump
+000003d0: 2063 6f6e 6461 2d69 6e63 7562 6174 6f72   conda-incubator
+000003e0: 2f73 6574 7570 2d6d 696e 6963 6f6e 6461  /setup-miniconda
+000003f0: 2066 726f 6d20 3220 746f 2033 205b 2339   from 2 to 3 [#9
+00000400: 3938 5d28 6874 7470 733a 2f2f 6769 7468  98](https://gith
+00000410: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00000420: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+00000430: 6c6c 2f39 3938 2920 285b 4064 6570 656e  ll/998) ([@depen
+00000440: 6461 626f 745d 2868 7474 7073 3a2f 2f67  dabot](https://g
+00000450: 6974 6875 622e 636f 6d2f 6465 7065 6e64  ithub.com/depend
+00000460: 6162 6f74 2929 0a2d 2063 686f 7265 3a20  abot)).- chore: 
+00000470: 7570 6461 7465 2070 7265 2d63 6f6d 6d69  update pre-commi
+00000480: 7420 686f 6f6b 7320 5b23 3939 365d 2868  t hooks [#996](h
+00000490: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000004a0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+000004b0: 725f 636c 6965 6e74 2f70 756c 6c2f 3939  r_client/pull/99
+000004c0: 3629 2028 5b40 7072 652d 636f 6d6d 6974  6) ([@pre-commit
+000004d0: 2d63 695d 2868 7474 7073 3a2f 2f67 6974  -ci](https://git
+000004e0: 6875 622e 636f 6d2f 7072 652d 636f 6d6d  hub.com/pre-comm
+000004f0: 6974 2d63 6929 290a 0a23 2323 2044 6f63  it-ci))..### Doc
+00000500: 756d 656e 7461 7469 6f6e 2069 6d70 726f  umentation impro
+00000510: 7665 6d65 6e74 730a 0a2d 2046 6978 2064  vements..- Fix d
+00000520: 6f63 7320 7265 6665 7265 6e63 6520 5b23  ocs reference [#
+00000530: 3130 3137 5d28 6874 7470 733a 2f2f 6769  1017](https://gi
+00000540: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+00000550: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+00000560: 7075 6c6c 2f31 3031 3729 2028 5b40 626c  pull/1017) ([@bl
+00000570: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
+00000580: 2f67 6974 6875 622e 636f 6d2f 626c 696e  /github.com/blin
+00000590: 6b31 3037 3329 290a 2d20 4164 6420 646f  k1073)).- Add do
+000005a0: 6373 2061 626f 7574 2070 6163 6b61 6769  cs about packagi
+000005b0: 6e67 206b 6572 6e65 6c73 205b 2331 3031  ng kernels [#101
+000005c0: 335d 2868 7474 7073 3a2f 2f67 6974 6875  3](https://githu
+000005d0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+000005e0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+000005f0: 6c2f 3130 3133 2920 285b 4062 6c69 6e6b  l/1013) ([@blink
+00000600: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
+00000610: 7468 7562 2e63 6f6d 2f62 6c69 6e6b 3130  thub.com/blink10
+00000620: 3733 2929 0a2d 2043 6c61 7269 6679 2077  73)).- Clarify w
+00000630: 6861 7420 6120 7265 7374 6172 7420 6d65  hat a restart me
+00000640: 616e 7320 5b23 3936 365d 2868 7474 7073  ans [#966](https
+00000650: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00000660: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+00000670: 6965 6e74 2f70 756c 6c2f 3936 3629 2028  ient/pull/966) (
+00000680: 5b40 6d6c 7563 6f6f 6c5d 2868 7474 7073  [@mlucool](https
+00000690: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d6c  ://github.com/ml
+000006a0: 7563 6f6f 6c29 290a 0a23 2323 2043 6f6e  ucool))..### Con
+000006b0: 7472 6962 7574 6f72 7320 746f 2074 6869  tributors to thi
+000006c0: 7320 7265 6c65 6173 650a 0a28 5b47 6974  s release..([Git
+000006d0: 4875 6220 636f 6e74 7269 6275 746f 7273  Hub contributors
+000006e0: 2070 6167 6520 666f 7220 7468 6973 2072   page for this r
+000006f0: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
+00000700: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00000710: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00000720: 742f 6772 6170 6873 2f63 6f6e 7472 6962  t/graphs/contrib
+00000730: 7574 6f72 733f 6672 6f6d 3d32 3032 332d  utors?from=2023-
+00000740: 3131 2d30 3626 746f 3d32 3032 342d 3033  11-06&to=2024-03
+00000750: 2d31 3226 7479 7065 3d63 2929 0a0a 5b40  -12&type=c))..[@
+00000760: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
+00000770: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
+00000780: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
+00000790: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
+000007a0: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
+000007b0: 3341 626c 696e 6b31 3037 332b 7570 6461  3Ablink1073+upda
+000007c0: 7465 6425 3341 3230 3233 2d31 312d 3036  ted%3A2023-11-06
+000007d0: 2e2e 3230 3234 2d30 332d 3132 2674 7970  ..2024-03-12&typ
+000007e0: 653d 4973 7375 6573 2920 7c20 5b40 6465  e=Issues) | [@de
+000007f0: 7065 6e64 6162 6f74 5d28 6874 7470 733a  pendabot](https:
+00000800: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+00000810: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+00000820: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+00000830: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+00000840: 4164 6570 656e 6461 626f 742b 7570 6461  Adependabot+upda
+00000850: 7465 6425 3341 3230 3233 2d31 312d 3036  ted%3A2023-11-06
+00000860: 2e2e 3230 3234 2d30 332d 3132 2674 7970  ..2024-03-12&typ
+00000870: 653d 4973 7375 6573 2920 7c20 5b40 6d6c  e=Issues) | [@ml
+00000880: 7563 6f6f 6c5d 2868 7474 7073 3a2f 2f67  ucool](https://g
+00000890: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+000008a0: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+000008b0: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+000008c0: 6e74 2b69 6e76 6f6c 7665 7325 3341 6d6c  nt+involves%3Aml
+000008d0: 7563 6f6f 6c2b 7570 6461 7465 6425 3341  ucool+updated%3A
+000008e0: 3230 3233 2d31 312d 3036 2e2e 3230 3234  2023-11-06..2024
+000008f0: 2d30 332d 3132 2674 7970 653d 4973 7375  -03-12&type=Issu
+00000900: 6573 2920 7c20 5b40 7072 652d 636f 6d6d  es) | [@pre-comm
+00000910: 6974 2d63 695d 2868 7474 7073 3a2f 2f67  it-ci](https://g
+00000920: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+00000930: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+00000940: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+00000950: 6e74 2b69 6e76 6f6c 7665 7325 3341 7072  nt+involves%3Apr
+00000960: 652d 636f 6d6d 6974 2d63 692b 7570 6461  e-commit-ci+upda
+00000970: 7465 6425 3341 3230 3233 2d31 312d 3036  ted%3A2023-11-06
+00000980: 2e2e 3230 3234 2d30 332d 3132 2674 7970  ..2024-03-12&typ
+00000990: 653d 4973 7375 6573 2920 7c20 5b40 5a73  e=Issues) | [@Zs
+000009a0: 6169 6c65 725d 2868 7474 7073 3a2f 2f67  ailer](https://g
+000009b0: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+000009c0: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+000009d0: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+000009e0: 6e74 2b69 6e76 6f6c 7665 7325 3341 5a73  nt+involves%3AZs
+000009f0: 6169 6c65 722b 7570 6461 7465 6425 3341  ailer+updated%3A
+00000a00: 3230 3233 2d31 312d 3036 2e2e 3230 3234  2023-11-06..2024
+00000a10: 2d30 332d 3132 2674 7970 653d 4973 7375  -03-12&type=Issu
+00000a20: 6573 290a 0a3c 212d 2d20 3c45 4e44 204e  es)..<!-- <END N
+00000a30: 4557 2043 4841 4e47 454c 4f47 2045 4e54  EW CHANGELOG ENT
+00000a40: 5259 3e20 2d2d 3e0a 0a23 2320 382e 362e  RY> -->..## 8.6.
+00000a50: 300a 0a28 5b46 756c 6c20 4368 616e 6765  0..([Full Change
+00000a60: 6c6f 675d 2868 7474 7073 3a2f 2f67 6974  log](https://git
+00000a70: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00000a80: 6a75 7079 7465 725f 636c 6965 6e74 2f63  jupyter_client/c
+00000a90: 6f6d 7061 7265 2f76 382e 352e 302e 2e2e  ompare/v8.5.0...
+00000aa0: 3264 3666 3532 6264 6635 3236 3636 3838  2d6f52bdf5266688
+00000ab0: 6335 3166 3332 3730 6364 3765 3437 6262  c51f3270cd7e47bb
+00000ac0: 6431 3763 3730 3863 2929 0a0a 2323 2320  d17c708c))..### 
+00000ad0: 4275 6773 2066 6978 6564 0a0a 2d20 4669  Bugs fixed..- Fi
+00000ae0: 7820 706f 7373 6962 6c79 206e 6f74 2064  x possibly not d
+00000af0: 6566 696e 6564 2074 7261 636b 6572 205b  efined tracker [
+00000b00: 2339 3931 5d28 6874 7470 733a 2f2f 6769  #991](https://gi
+00000b10: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+00000b20: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+00000b30: 7075 6c6c 2f39 3931 2920 285b 4064 6176  pull/991) ([@dav
+00000b40: 6964 6272 6f63 6861 7274 5d28 6874 7470  idbrochart](http
+00000b50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00000b60: 6176 6964 6272 6f63 6861 7274 2929 0a2d  avidbrochart)).-
+00000b70: 2042 5547 3a20 4669 7820 4b77 6172 6720   BUG: Fix Kwarg 
+00000b80: 6f6e 6c79 2069 6e20 7570 6461 7465 5f65  only in update_e
+00000b90: 6e76 205b 2339 3839 5d28 6874 7470 733a  nv [#989](https:
+00000ba0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+00000bb0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+00000bc0: 656e 742f 7075 6c6c 2f39 3839 2920 285b  ent/pull/989) ([
+00000bd0: 4043 6172 7265 6175 5d28 6874 7470 733a  @Carreau](https:
+00000be0: 2f2f 6769 7468 7562 2e63 6f6d 2f43 6172  //github.com/Car
+00000bf0: 7265 6175 2929 0a0a 2323 2320 4d61 696e  reau))..### Main
+00000c00: 7465 6e61 6e63 6520 616e 6420 7570 6b65  tenance and upke
+00000c10: 6570 2069 6d70 726f 7665 6d65 6e74 730a  ep improvements.
+00000c20: 0a2d 2055 7064 6174 6520 7479 7069 6e67  .- Update typing
+00000c30: 2066 6f72 2074 7261 6974 6c65 7473 2035   for traitlets 5
+00000c40: 2e31 3320 5b23 3939 355d 2868 7474 7073  .13 [#995](https
+00000c50: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00000c60: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+00000c70: 6965 6e74 2f70 756c 6c2f 3939 3529 2028  ient/pull/995) (
+00000c80: 5b40 626c 696e 6b31 3037 335d 2868 7474  [@blink1073](htt
+00000c90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000ca0: 626c 696e 6b31 3037 3329 290a 2d20 5573  blink1073)).- Us
+00000cb0: 6520 7275 6666 2066 6f72 6d61 7420 5b23  e ruff format [#
+00000cc0: 3939 325d 2868 7474 7073 3a2f 2f67 6974  992](https://git
+00000cd0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00000ce0: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+00000cf0: 756c 6c2f 3939 3229 2028 5b40 626c 696e  ull/992) ([@blin
+00000d00: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
+00000d10: 6974 6875 622e 636f 6d2f 626c 696e 6b31  ithub.com/blink1
+00000d20: 3037 3329 290a 2d20 556e 7573 6564 2060  073)).- Unused `
+00000d30: 2a61 7267 7360 2069 6e20 604b 6572 6e65  *args` in `Kerne
+00000d40: 6c4d 616e 6167 6572 6027 7320 605f 5f69  lManager`'s `__i
+00000d50: 6e69 745f 5f60 205b 2339 3836 5d28 6874  nit__` [#986](ht
+00000d60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000d70: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+00000d80: 5f63 6c69 656e 742f 7075 6c6c 2f39 3836  _client/pull/986
+00000d90: 2920 285b 4043 6172 7265 6175 5d28 6874  ) ([@Carreau](ht
+00000da0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000db0: 2f43 6172 7265 6175 2929 0a0a 2323 2320  /Carreau))..### 
+00000dc0: 436f 6e74 7269 6275 746f 7273 2074 6f20  Contributors to 
+00000dd0: 7468 6973 2072 656c 6561 7365 0a0a 285b  this release..([
+00000de0: 4769 7448 7562 2063 6f6e 7472 6962 7574  GitHub contribut
+00000df0: 6f72 7320 7061 6765 2066 6f72 2074 6869  ors page for thi
+00000e00: 7320 7265 6c65 6173 655d 2868 7474 7073  s release](https
+00000e10: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00000e20: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+00000e30: 6965 6e74 2f67 7261 7068 732f 636f 6e74  ient/graphs/cont
+00000e40: 7269 6275 746f 7273 3f66 726f 6d3d 3230  ributors?from=20
+00000e50: 3233 2d31 302d 3235 2674 6f3d 3230 3233  23-10-25&to=2023
+00000e60: 2d31 312d 3036 2674 7970 653d 6329 290a  -11-06&type=c)).
+00000e70: 0a5b 4062 6c69 6e6b 3130 3733 5d28 6874  .[@blink1073](ht
+00000e80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000e90: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+00000ea0: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+00000eb0: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+00000ec0: 6573 2533 4162 6c69 6e6b 3130 3733 2b75  es%3Ablink1073+u
+00000ed0: 7064 6174 6564 2533 4132 3032 332d 3130  pdated%3A2023-10
+00000ee0: 2d32 352e 2e32 3032 332d 3131 2d30 3626  -25..2023-11-06&
+00000ef0: 7479 7065 3d49 7373 7565 7329 207c 205b  type=Issues) | [
+00000f00: 4043 6172 7265 6175 5d28 6874 7470 733a  @Carreau](https:
+00000f10: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+00000f20: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+00000f30: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+00000f40: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+00000f50: 4143 6172 7265 6175 2b75 7064 6174 6564  ACarreau+updated
+00000f60: 2533 4132 3032 332d 3130 2d32 352e 2e32  %3A2023-10-25..2
+00000f70: 3032 332d 3131 2d30 3626 7479 7065 3d49  023-11-06&type=I
+00000f80: 7373 7565 7329 207c 205b 4064 6176 6964  ssues) | [@david
+00000f90: 6272 6f63 6861 7274 5d28 6874 7470 733a  brochart](https:
+00000fa0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+00000fb0: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+00000fc0: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+00000fd0: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+00000fe0: 4164 6176 6964 6272 6f63 6861 7274 2b75  Adavidbrochart+u
+00000ff0: 7064 6174 6564 2533 4132 3032 332d 3130  pdated%3A2023-10
+00001000: 2d32 352e 2e32 3032 332d 3131 2d30 3626  -25..2023-11-06&
+00001010: 7479 7065 3d49 7373 7565 7329 0a0a 2323  type=Issues)..##
+00001020: 2038 2e35 2e30 0a0a 285b 4675 6c6c 2043   8.5.0..([Full C
+00001030: 6861 6e67 656c 6f67 5d28 6874 7470 733a  hangelog](https:
+00001040: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+00001050: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+00001060: 656e 742f 636f 6d70 6172 652f 7638 2e34  ent/compare/v8.4
+00001070: 2e30 2e2e 2e66 6639 3465 3331 3063 3261  .0...ff94e310c2a
+00001080: 6633 3534 3666 3266 3933 3834 6536 6233  f3546f2f9384e6b3
+00001090: 3566 6431 3163 3364 3039 6137 3129 290a  5fd11c3d09a71)).
+000010a0: 0a23 2323 2045 6e68 616e 6365 6d65 6e74  .### Enhancement
+000010b0: 7320 6d61 6465 0a0a 2d20 416c 6c6f 7720  s made..- Allow 
+000010c0: 746f 2075 7064 6174 6520 6b65 726e 656c  to update kernel
+000010d0: 7320 656e 7620 696e 2062 6574 7765 656e  s env in between
+000010e0: 2072 6573 7461 7274 2e20 5b23 3938 375d   restart. [#987]
+000010f0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001100: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00001110: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00001120: 3938 3729 2028 5b40 4361 7272 6561 755d  987) ([@Carreau]
+00001130: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001140: 636f 6d2f 4361 7272 6561 7529 290a 0a23  com/Carreau))..#
+00001150: 2323 204d 6169 6e74 656e 616e 6365 2061  ## Maintenance a
+00001160: 6e64 2075 706b 6565 7020 696d 7072 6f76  nd upkeep improv
+00001170: 656d 656e 7473 0a0a 2d20 456e 6162 6c65  ements..- Enable
+00001180: 2073 7472 6963 7420 7479 7069 6e67 205b   strict typing [
+00001190: 2339 3834 5d28 6874 7470 733a 2f2f 6769  #984](https://gi
+000011a0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+000011b0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+000011c0: 7075 6c6c 2f39 3834 2920 285b 4062 6c69  pull/984) ([@bli
+000011d0: 6e6b 3130 3733 5d28 6874 7470 733a 2f2f  nk1073](https://
+000011e0: 6769 7468 7562 2e63 6f6d 2f62 6c69 6e6b  github.com/blink
+000011f0: 3130 3733 2929 0a2d 2055 7064 6174 6520  1073)).- Update 
+00001200: 7479 7069 6e67 7320 666f 7220 6d79 7079  typings for mypy
+00001210: 2031 2e36 205b 2339 3833 5d28 6874 7470   1.6 [#983](http
+00001220: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00001230: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
+00001240: 6c69 656e 742f 7075 6c6c 2f39 3833 2920  lient/pull/983) 
+00001250: 285b 4062 6c69 6e6b 3130 3733 5d28 6874  ([@blink1073](ht
+00001260: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001270: 2f62 6c69 6e6b 3130 3733 2929 0a0a 2323  /blink1073))..##
+00001280: 2320 436f 6e74 7269 6275 746f 7273 2074  # Contributors t
+00001290: 6f20 7468 6973 2072 656c 6561 7365 0a0a  o this release..
+000012a0: 285b 4769 7448 7562 2063 6f6e 7472 6962  ([GitHub contrib
+000012b0: 7574 6f72 7320 7061 6765 2066 6f72 2074  utors page for t
+000012c0: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
+000012d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000012e0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+000012f0: 636c 6965 6e74 2f67 7261 7068 732f 636f  client/graphs/co
+00001300: 6e74 7269 6275 746f 7273 3f66 726f 6d3d  ntributors?from=
+00001310: 3230 3233 2d31 302d 3131 2674 6f3d 3230  2023-10-11&to=20
+00001320: 3233 2d31 302d 3235 2674 7970 653d 6329  23-10-25&type=c)
+00001330: 290a 0a5b 4062 6c69 6e6b 3130 3733 5d28  )..[@blink1073](
+00001340: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001350: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
+00001360: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
+00001370: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
+00001380: 6c76 6573 2533 4162 6c69 6e6b 3130 3733  lves%3Ablink1073
+00001390: 2b75 7064 6174 6564 2533 4132 3032 332d  +updated%3A2023-
+000013a0: 3130 2d31 312e 2e32 3032 332d 3130 2d32  10-11..2023-10-2
+000013b0: 3526 7479 7065 3d49 7373 7565 7329 207c  5&type=Issues) |
+000013c0: 205b 4043 6172 7265 6175 5d28 6874 7470   [@Carreau](http
+000013d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+000013e0: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
+000013f0: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
+00001400: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
+00001410: 2533 4143 6172 7265 6175 2b75 7064 6174  %3ACarreau+updat
+00001420: 6564 2533 4132 3032 332d 3130 2d31 312e  ed%3A2023-10-11.
+00001430: 2e32 3032 332d 3130 2d32 3526 7479 7065  .2023-10-25&type
+00001440: 3d49 7373 7565 7329 0a0a 2323 2038 2e34  =Issues)..## 8.4
+00001450: 2e30 0a0a 285b 4675 6c6c 2043 6861 6e67  .0..([Full Chang
+00001460: 656c 6f67 5d28 6874 7470 733a 2f2f 6769  elog](https://gi
+00001470: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+00001480: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+00001490: 636f 6d70 6172 652f 7638 2e33 2e31 2e2e  compare/v8.3.1..
+000014a0: 2e37 3430 3434 3339 3332 3330 6537 3031  .74044393230e701
+000014b0: 3334 6636 3865 3636 3466 3265 6631 3966  34f68e664f2ef19f
+000014c0: 6162 3932 6237 3737 3429 290a 0a23 2323  ab92b7774))..###
+000014d0: 204d 6169 6e74 656e 616e 6365 2061 6e64   Maintenance and
+000014e0: 2075 706b 6565 7020 696d 7072 6f76 656d   upkeep improvem
+000014f0: 656e 7473 0a0a 2d20 5465 7374 206f 6e20  ents..- Test on 
+00001500: 7079 7468 6f6e 2033 2e31 3220 5b23 3937  python 3.12 [#97
+00001510: 385d 2868 7474 7073 3a2f 2f67 6974 6875  8](https://githu
+00001520: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00001530: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00001540: 6c2f 3937 3829 2028 5b40 626c 696e 6b31  l/978) ([@blink1
+00001550: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
+00001560: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
+00001570: 3329 290a 2d20 5570 6461 7465 2074 7970  3)).- Update typ
+00001580: 696e 6720 666f 7220 7472 6169 746c 6574  ing for traitlet
+00001590: 7320 352e 3131 205b 2339 3737 5d28 6874  s 5.11 [#977](ht
+000015a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000015b0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+000015c0: 5f63 6c69 656e 742f 7075 6c6c 2f39 3737  _client/pull/977
+000015d0: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
+000015e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000015f0: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a2d  om/blink1073)).-
+00001600: 2063 686f 7265 3a20 7570 6461 7465 2070   chore: update p
+00001610: 7265 2d63 6f6d 6d69 7420 686f 6f6b 7320  re-commit hooks 
+00001620: 5b23 3937 355d 2868 7474 7073 3a2f 2f67  [#975](https://g
+00001630: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00001640: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00001650: 2f70 756c 6c2f 3937 3529 2028 5b40 7072  /pull/975) ([@pr
+00001660: 652d 636f 6d6d 6974 2d63 695d 2868 7474  e-commit-ci](htt
+00001670: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001680: 7072 652d 636f 6d6d 6974 2d63 6929 290a  pre-commit-ci)).
+00001690: 2d20 5570 6461 7465 2074 7970 696e 6773  - Update typings
+000016a0: 2066 6f72 2074 7261 6974 6c65 7473 2035   for traitlets 5
+000016b0: 2e31 302e 3120 5b23 3937 345d 2868 7474  .10.1 [#974](htt
+000016c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000016d0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+000016e0: 636c 6965 6e74 2f70 756c 6c2f 3937 3429  client/pull/974)
+000016f0: 2028 5b40 626c 696e 6b31 3037 335d 2868   ([@blink1073](h
+00001700: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001710: 6d2f 626c 696e 6b31 3037 3329 290a 2d20  m/blink1073)).- 
+00001720: 446f 206e 6f74 2075 7365 2064 6174 6574  Do not use datet
+00001730: 696d 652e 7574 636e 6f77 2829 2074 6861  ime.utcnow() tha
+00001740: 7420 6973 2064 6570 7265 6361 7465 6420  t is deprecated 
+00001750: 696e 2050 7974 686f 6e20 332e 3132 205b  in Python 3.12 [
+00001760: 2339 3732 5d28 6874 7470 733a 2f2f 6769  #972](https://gi
+00001770: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+00001780: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+00001790: 7075 6c6c 2f39 3732 2920 285b 4065 6c6c  pull/972) ([@ell
+000017a0: 6572 745d 2868 7474 7073 3a2f 2f67 6974  ert](https://git
+000017b0: 6875 622e 636f 6d2f 656c 6c65 7274 2929  hub.com/ellert))
+000017c0: 0a2d 2055 7365 2073 702d 7265 706f 2d72  .- Use sp-repo-r
+000017d0: 6576 6965 7720 5b23 3937 315d 2868 7474  eview [#971](htt
+000017e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000017f0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00001800: 636c 6965 6e74 2f70 756c 6c2f 3937 3129  client/pull/971)
+00001810: 2028 5b40 626c 696e 6b31 3037 335d 2868   ([@blink1073](h
+00001820: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001830: 6d2f 626c 696e 6b31 3037 3329 290a 2d20  m/blink1073)).- 
+00001840: 4275 6d70 2061 6374 696f 6e73 2f63 6865  Bump actions/che
+00001850: 636b 6f75 7420 6672 6f6d 2033 2074 6f20  ckout from 3 to 
+00001860: 3420 5b23 3936 385d 2868 7474 7073 3a2f  4 [#968](https:/
+00001870: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00001880: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00001890: 6e74 2f70 756c 6c2f 3936 3829 2028 5b40  nt/pull/968) ([@
+000018a0: 6465 7065 6e64 6162 6f74 5d28 6874 7470  dependabot](http
+000018b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+000018c0: 6570 656e 6461 626f 7429 290a 0a23 2323  ependabot))..###
+000018d0: 2043 6f6e 7472 6962 7574 6f72 7320 746f   Contributors to
+000018e0: 2074 6869 7320 7265 6c65 6173 650a 0a28   this release..(
+000018f0: 5b47 6974 4875 6220 636f 6e74 7269 6275  [GitHub contribu
+00001900: 746f 7273 2070 6167 6520 666f 7220 7468  tors page for th
+00001910: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
+00001920: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00001930: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
+00001940: 6c69 656e 742f 6772 6170 6873 2f63 6f6e  lient/graphs/con
+00001950: 7472 6962 7574 6f72 733f 6672 6f6d 3d32  tributors?from=2
+00001960: 3032 332d 3038 2d32 3926 746f 3d32 3032  023-08-29&to=202
+00001970: 332d 3130 2d31 3126 7479 7065 3d63 2929  3-10-11&type=c))
+00001980: 0a0a 5b40 626c 696e 6b31 3037 335d 2868  ..[@blink1073](h
+00001990: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000019a0: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
+000019b0: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
+000019c0: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
+000019d0: 7665 7325 3341 626c 696e 6b31 3037 332b  ves%3Ablink1073+
+000019e0: 7570 6461 7465 6425 3341 3230 3233 2d30  updated%3A2023-0
+000019f0: 382d 3239 2e2e 3230 3233 2d31 302d 3131  8-29..2023-10-11
+00001a00: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
+00001a10: 5b40 6465 7065 6e64 6162 6f74 5d28 6874  [@dependabot](ht
+00001a20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001a30: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+00001a40: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+00001a50: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+00001a60: 6573 2533 4164 6570 656e 6461 626f 742b  es%3Adependabot+
+00001a70: 7570 6461 7465 6425 3341 3230 3233 2d30  updated%3A2023-0
+00001a80: 382d 3239 2e2e 3230 3233 2d31 302d 3131  8-29..2023-10-11
+00001a90: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
+00001aa0: 5b40 656c 6c65 7274 5d28 6874 7470 733a  [@ellert](https:
+00001ab0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+00001ac0: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+00001ad0: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+00001ae0: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+00001af0: 4165 6c6c 6572 742b 7570 6461 7465 6425  Aellert+updated%
+00001b00: 3341 3230 3233 2d30 382d 3239 2e2e 3230  3A2023-08-29..20
+00001b10: 3233 2d31 302d 3131 2674 7970 653d 4973  23-10-11&type=Is
+00001b20: 7375 6573 2920 7c20 5b40 7072 652d 636f  sues) | [@pre-co
+00001b30: 6d6d 6974 2d63 695d 2868 7474 7073 3a2f  mmit-ci](https:/
+00001b40: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
+00001b50: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
+00001b60: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
+00001b70: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
+00001b80: 7072 652d 636f 6d6d 6974 2d63 692b 7570  pre-commit-ci+up
+00001b90: 6461 7465 6425 3341 3230 3233 2d30 382d  dated%3A2023-08-
+00001ba0: 3239 2e2e 3230 3233 2d31 302d 3131 2674  29..2023-10-11&t
+00001bb0: 7970 653d 4973 7375 6573 290a 0a23 2320  ype=Issues)..## 
+00001bc0: 382e 332e 310a 0a28 5b46 756c 6c20 4368  8.3.1..([Full Ch
+00001bd0: 616e 6765 6c6f 675d 2868 7474 7073 3a2f  angelog](https:/
+00001be0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00001bf0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00001c00: 6e74 2f63 6f6d 7061 7265 2f76 382e 332e  nt/compare/v8.3.
+00001c10: 302e 2e2e 6234 6637 6439 3437 6661 6535  0...b4f7d947fae5
+00001c20: 3561 3466 6535 3961 3237 6466 3038 3330  5a4fe59a27df0830
+00001c30: 6139 6137 3864 6364 3465 3132 2929 0a0a  a9a78dcd4e12))..
+00001c40: 2323 2320 456e 6861 6e63 656d 656e 7473  ### Enhancements
+00001c50: 206d 6164 650a 0a2d 2053 7570 706f 7274   made..- Support
+00001c60: 2065 7874 6572 6e61 6c20 6b65 726e 656c   external kernel
+00001c70: 7320 5b23 3936 315d 2868 7474 7073 3a2f  s [#961](https:/
+00001c80: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00001c90: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00001ca0: 6e74 2f70 756c 6c2f 3936 3129 2028 5b40  nt/pull/961) ([@
+00001cb0: 6461 7669 6462 726f 6368 6172 745d 2868  davidbrochart](h
+00001cc0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001cd0: 6d2f 6461 7669 6462 726f 6368 6172 7429  m/davidbrochart)
+00001ce0: 290a 0a23 2323 2042 7567 7320 6669 7865  )..### Bugs fixe
+00001cf0: 640a 0a2d 204d 616b 6520 6361 6368 655f  d..- Make cache_
+00001d00: 706f 7274 7320 636f 6e66 6967 7572 6162  ports configurab
+00001d10: 6c65 2077 6974 6820 6465 6661 756c 7420  le with default 
+00001d20: 7661 6c75 6520 6f66 2046 616c 7365 2e20  value of False. 
+00001d30: 5b23 3935 365d 2868 7474 7073 3a2f 2f67  [#956](https://g
+00001d40: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00001d50: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00001d60: 2f70 756c 6c2f 3935 3629 2028 5b40 6a6b  /pull/956) ([@jk
+00001d70: 6974 6368 696e 5d28 6874 7470 733a 2f2f  itchin](https://
+00001d80: 6769 7468 7562 2e63 6f6d 2f6a 6b69 7463  github.com/jkitc
+00001d90: 6869 6e29 290a 0a23 2323 204d 6169 6e74  hin))..### Maint
+00001da0: 656e 616e 6365 2061 6e64 2075 706b 6565  enance and upkee
+00001db0: 7020 696d 7072 6f76 656d 656e 7473 0a0a  p improvements..
+00001dc0: 2323 2320 436f 6e74 7269 6275 746f 7273  ### Contributors
+00001dd0: 2074 6f20 7468 6973 2072 656c 6561 7365   to this release
+00001de0: 0a0a 285b 4769 7448 7562 2063 6f6e 7472  ..([GitHub contr
+00001df0: 6962 7574 6f72 7320 7061 6765 2066 6f72  ibutors page for
+00001e00: 2074 6869 7320 7265 6c65 6173 655d 2868   this release](h
+00001e10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001e20: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+00001e30: 725f 636c 6965 6e74 2f67 7261 7068 732f  r_client/graphs/
+00001e40: 636f 6e74 7269 6275 746f 7273 3f66 726f  contributors?fro
+00001e50: 6d3d 3230 3233 2d30 362d 3233 2674 6f3d  m=2023-06-23&to=
+00001e60: 3230 3233 2d30 382d 3239 2674 7970 653d  2023-08-29&type=
+00001e70: 6329 290a 0a5b 4062 6c69 6e6b 3130 3733  c))..[@blink1073
+00001e80: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001e90: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
+00001ea0: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
+00001eb0: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
+00001ec0: 766f 6c76 6573 2533 4162 6c69 6e6b 3130  volves%3Ablink10
+00001ed0: 3733 2b75 7064 6174 6564 2533 4132 3032  73+updated%3A202
+00001ee0: 332d 3036 2d32 332e 2e32 3032 332d 3038  3-06-23..2023-08
+00001ef0: 2d32 3926 7479 7065 3d49 7373 7565 7329  -29&type=Issues)
+00001f00: 207c 205b 4064 6176 6964 6272 6f63 6861   | [@davidbrocha
+00001f10: 7274 5d28 6874 7470 733a 2f2f 6769 7468  rt](https://gith
+00001f20: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
+00001f30: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
+00001f40: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
+00001f50: 696e 766f 6c76 6573 2533 4164 6176 6964  involves%3Adavid
+00001f60: 6272 6f63 6861 7274 2b75 7064 6174 6564  brochart+updated
+00001f70: 2533 4132 3032 332d 3036 2d32 332e 2e32  %3A2023-06-23..2
+00001f80: 3032 332d 3038 2d32 3926 7479 7065 3d49  023-08-29&type=I
+00001f90: 7373 7565 7329 207c 205b 406a 6b69 7463  ssues) | [@jkitc
+00001fa0: 6869 6e5d 2868 7474 7073 3a2f 2f67 6974  hin](https://git
+00001fb0: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
+00001fc0: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
+00001fd0: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
+00001fe0: 2b69 6e76 6f6c 7665 7325 3341 6a6b 6974  +involves%3Ajkit
+00001ff0: 6368 696e 2b75 7064 6174 6564 2533 4132  chin+updated%3A2
+00002000: 3032 332d 3036 2d32 332e 2e32 3032 332d  023-06-23..2023-
+00002010: 3038 2d32 3926 7479 7065 3d49 7373 7565  08-29&type=Issue
+00002020: 7329 207c 205b 406b 6576 696e 2d62 6174  s) | [@kevin-bat
+00002030: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+00002040: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
+00002050: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
+00002060: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
+00002070: 696e 766f 6c76 6573 2533 416b 6576 696e  involves%3Akevin
+00002080: 2d62 6174 6573 2b75 7064 6174 6564 2533  -bates+updated%3
+00002090: 4132 3032 332d 3036 2d32 332e 2e32 3032  A2023-06-23..202
+000020a0: 332d 3038 2d32 3926 7479 7065 3d49 7373  3-08-29&type=Iss
+000020b0: 7565 7329 207c 205b 4070 7265 2d63 6f6d  ues) | [@pre-com
+000020c0: 6d69 742d 6369 5d28 6874 7470 733a 2f2f  mit-ci](https://
+000020d0: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
+000020e0: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
+000020f0: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
+00002100: 656e 742b 696e 766f 6c76 6573 2533 4170  ent+involves%3Ap
+00002110: 7265 2d63 6f6d 6d69 742d 6369 2b75 7064  re-commit-ci+upd
+00002120: 6174 6564 2533 4132 3032 332d 3036 2d32  ated%3A2023-06-2
+00002130: 332e 2e32 3032 332d 3038 2d32 3926 7479  3..2023-08-29&ty
+00002140: 7065 3d49 7373 7565 7329 207c 205b 4074  pe=Issues) | [@t
+00002150: 6d61 7877 656c 6c2d 616e 7468 726f 7069  maxwell-anthropi
+00002160: 635d 2868 7474 7073 3a2f 2f67 6974 6875  c](https://githu
+00002170: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
+00002180: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
+00002190: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
+000021a0: 6e76 6f6c 7665 7325 3341 746d 6178 7765  nvolves%3Atmaxwe
+000021b0: 6c6c 2d61 6e74 6872 6f70 6963 2b75 7064  ll-anthropic+upd
+000021c0: 6174 6564 2533 4132 3032 332d 3036 2d32  ated%3A2023-06-2
+000021d0: 332e 2e32 3032 332d 3038 2d32 3926 7479  3..2023-08-29&ty
+000021e0: 7065 3d49 7373 7565 7329 0a0a 2323 2038  pe=Issues)..## 8
+000021f0: 2e33 2e30 0a0a 285b 4675 6c6c 2043 6861  .3.0..([Full Cha
+00002200: 6e67 656c 6f67 5d28 6874 7470 733a 2f2f  ngelog](https://
+00002210: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00002220: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00002230: 742f 636f 6d70 6172 652f 7638 2e32 2e30  t/compare/v8.2.0
+00002240: 2e2e 2e62 6464 6238 3835 3461 3461 6133  ...bddb8854a4aa3
+00002250: 3332 3465 3132 3865 3034 3937 3533 3965  324e128e0497539e
+00002260: 3137 3234 3666 6266 3633 3029 290a 0a23  17246fbf630))..#
+00002270: 2323 2045 6e68 616e 6365 6d65 6e74 7320  ## Enhancements 
+00002280: 6d61 6465 0a0a 2d20 416c 6c6f 7720 6b77  made..- Allow kw
+00002290: 6172 6773 2077 6865 6e20 7772 6974 696e  args when writin
+000022a0: 6720 636f 6e6e 6563 7469 6f6e 5f66 696c  g connection_fil
+000022b0: 6520 5b23 3935 335d 2868 7474 7073 3a2f  e [#953](https:/
+000022c0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+000022d0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+000022e0: 6e74 2f70 756c 6c2f 3935 3329 2028 5b40  nt/pull/953) ([@
+000022f0: 6665 6365 745d 2868 7474 7073 3a2f 2f67  fecet](https://g
+00002300: 6974 6875 622e 636f 6d2f 6665 6365 7429  ithub.com/fecet)
+00002310: 290a 0a23 2323 204d 6169 6e74 656e 616e  )..### Maintenan
+00002320: 6365 2061 6e64 2075 706b 6565 7020 696d  ce and upkeep im
+00002330: 7072 6f76 656d 656e 7473 0a0a 2323 2320  provements..### 
+00002340: 436f 6e74 7269 6275 746f 7273 2074 6f20  Contributors to 
+00002350: 7468 6973 2072 656c 6561 7365 0a0a 285b  this release..([
+00002360: 4769 7448 7562 2063 6f6e 7472 6962 7574  GitHub contribut
+00002370: 6f72 7320 7061 6765 2066 6f72 2074 6869  ors page for thi
+00002380: 7320 7265 6c65 6173 655d 2868 7474 7073  s release](https
+00002390: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+000023a0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+000023b0: 6965 6e74 2f67 7261 7068 732f 636f 6e74  ient/graphs/cont
+000023c0: 7269 6275 746f 7273 3f66 726f 6d3d 3230  ributors?from=20
+000023d0: 3233 2d30 342d 3133 2674 6f3d 3230 3233  23-04-13&to=2023
+000023e0: 2d30 362d 3233 2674 7970 653d 6329 290a  -06-23&type=c)).
+000023f0: 0a5b 4066 6563 6574 5d28 6874 7470 733a  .[@fecet](https:
+00002400: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+00002410: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+00002420: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+00002430: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+00002440: 4166 6563 6574 2b75 7064 6174 6564 2533  Afecet+updated%3
+00002450: 4132 3032 332d 3034 2d31 332e 2e32 3032  A2023-04-13..202
+00002460: 332d 3036 2d32 3326 7479 7065 3d49 7373  3-06-23&type=Iss
+00002470: 7565 7329 207c 205b 4070 7265 2d63 6f6d  ues) | [@pre-com
+00002480: 6d69 742d 6369 5d28 6874 7470 733a 2f2f  mit-ci](https://
+00002490: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
+000024a0: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
+000024b0: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
+000024c0: 656e 742b 696e 766f 6c76 6573 2533 4170  ent+involves%3Ap
+000024d0: 7265 2d63 6f6d 6d69 742d 6369 2b75 7064  re-commit-ci+upd
+000024e0: 6174 6564 2533 4132 3032 332d 3034 2d31  ated%3A2023-04-1
+000024f0: 332e 2e32 3032 332d 3036 2d32 3326 7479  3..2023-06-23&ty
+00002500: 7065 3d49 7373 7565 7329 0a0a 2323 2038  pe=Issues)..## 8
+00002510: 2e32 2e30 0a0a 285b 4675 6c6c 2043 6861  .2.0..([Full Cha
+00002520: 6e67 656c 6f67 5d28 6874 7470 733a 2f2f  ngelog](https://
+00002530: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00002540: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00002550: 742f 636f 6d70 6172 652f 7638 2e31 2e30  t/compare/v8.1.0
+00002560: 2e2e 2e64 6266 3662 3831 6661 3561 6236  ...dbf6b81fa5ab6
+00002570: 3036 6561 6564 6335 6538 6430 3834 3364  06eaedc5e8d0843d
+00002580: 6562 6365 3138 6538 3734 3629 290a 0a23  ebce18e8746))..#
+00002590: 2323 2045 6e68 616e 6365 6d65 6e74 7320  ## Enhancements 
+000025a0: 6d61 6465 0a0a 2d20 7573 6520 632e 662e  made..- use c.f.
+000025b0: 4675 7475 7265 2074 6f20 7761 6974 2061  Future to wait a
+000025c0: 6372 6f73 7320 7468 7265 6164 7320 5b23  cross threads [#
+000025d0: 3934 305d 2868 7474 7073 3a2f 2f67 6974  940](https://git
+000025e0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+000025f0: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+00002600: 756c 6c2f 3934 3029 2028 5b40 6d69 6e72  ull/940) ([@minr
+00002610: 6b5d 2868 7474 7073 3a2f 2f67 6974 6875  k](https://githu
+00002620: 622e 636f 6d2f 6d69 6e72 6b29 290a 0a23  b.com/minrk))..#
+00002630: 2323 204d 6169 6e74 656e 616e 6365 2061  ## Maintenance a
+00002640: 6e64 2075 706b 6565 7020 696d 7072 6f76  nd upkeep improv
+00002650: 656d 656e 7473 0a0a 2d20 5573 6520 6c6f  ements..- Use lo
+00002660: 6361 6c20 636f 7665 7261 6765 205b 2339  cal coverage [#9
+00002670: 3435 5d28 6874 7470 733a 2f2f 6769 7468  45](https://gith
+00002680: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00002690: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+000026a0: 6c6c 2f39 3435 2920 285b 4062 6c69 6e6b  ll/945) ([@blink
+000026b0: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
+000026c0: 7468 7562 2e63 6f6d 2f62 6c69 6e6b 3130  thub.com/blink10
+000026d0: 3733 2929 0a2d 2041 6464 206d 6f72 6520  73)).- Add more 
+000026e0: 7072 6f6a 6563 7420 5552 4c73 205b 2339  project URLs [#9
+000026f0: 3434 5d28 6874 7470 733a 2f2f 6769 7468  44](https://gith
+00002700: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00002710: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+00002720: 6c6c 2f39 3434 2920 285b 4066 636f 6c6c  ll/944) ([@fcoll
+00002730: 6f6e 7661 6c5d 2868 7474 7073 3a2f 2f67  onval](https://g
+00002740: 6974 6875 622e 636f 6d2f 6663 6f6c 6c6f  ithub.com/fcollo
+00002750: 6e76 616c 2929 0a0a 2323 2320 436f 6e74  nval))..### Cont
+00002760: 7269 6275 746f 7273 2074 6f20 7468 6973  ributors to this
+00002770: 2072 656c 6561 7365 0a0a 285b 4769 7448   release..([GitH
+00002780: 7562 2063 6f6e 7472 6962 7574 6f72 7320  ub contributors 
+00002790: 7061 6765 2066 6f72 2074 6869 7320 7265  page for this re
+000027a0: 6c65 6173 655d 2868 7474 7073 3a2f 2f67  lease](https://g
+000027b0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+000027c0: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+000027d0: 2f67 7261 7068 732f 636f 6e74 7269 6275  /graphs/contribu
+000027e0: 746f 7273 3f66 726f 6d3d 3230 3233 2d30  tors?from=2023-0
+000027f0: 332d 3230 2674 6f3d 3230 3233 2d30 342d  3-20&to=2023-04-
+00002800: 3133 2674 7970 653d 6329 290a 0a5b 4062  13&type=c))..[@b
+00002810: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
+00002820: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+00002830: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+00002840: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+00002850: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+00002860: 4162 6c69 6e6b 3130 3733 2b75 7064 6174  Ablink1073+updat
+00002870: 6564 2533 4132 3032 332d 3033 2d32 302e  ed%3A2023-03-20.
+00002880: 2e32 3032 332d 3034 2d31 3326 7479 7065  .2023-04-13&type
+00002890: 3d49 7373 7565 7329 207c 205b 4066 636f  =Issues) | [@fco
+000028a0: 6c6c 6f6e 7661 6c5d 2868 7474 7073 3a2f  llonval](https:/
+000028b0: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
+000028c0: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
+000028d0: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
+000028e0: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
+000028f0: 6663 6f6c 6c6f 6e76 616c 2b75 7064 6174  fcollonval+updat
+00002900: 6564 2533 4132 3032 332d 3033 2d32 302e  ed%3A2023-03-20.
+00002910: 2e32 3032 332d 3034 2d31 3326 7479 7065  .2023-04-13&type
+00002920: 3d49 7373 7565 7329 207c 205b 406d 696e  =Issues) | [@min
+00002930: 726b 5d28 6874 7470 733a 2f2f 6769 7468  rk](https://gith
+00002940: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
+00002950: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
+00002960: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
+00002970: 696e 766f 6c76 6573 2533 416d 696e 726b  involves%3Aminrk
+00002980: 2b75 7064 6174 6564 2533 4132 3032 332d  +updated%3A2023-
+00002990: 3033 2d32 302e 2e32 3032 332d 3034 2d31  03-20..2023-04-1
+000029a0: 3326 7479 7065 3d49 7373 7565 7329 207c  3&type=Issues) |
+000029b0: 205b 4070 7265 2d63 6f6d 6d69 742d 6369   [@pre-commit-ci
+000029c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000029d0: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
+000029e0: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
+000029f0: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
+00002a00: 766f 6c76 6573 2533 4170 7265 2d63 6f6d  volves%3Apre-com
+00002a10: 6d69 742d 6369 2b75 7064 6174 6564 2533  mit-ci+updated%3
+00002a20: 4132 3032 332d 3033 2d32 302e 2e32 3032  A2023-03-20..202
+00002a30: 332d 3034 2d31 3326 7479 7065 3d49 7373  3-04-13&type=Iss
+00002a40: 7565 7329 0a0a 2323 2038 2e31 2e30 0a0a  ues)..## 8.1.0..
+00002a50: 285b 4675 6c6c 2043 6861 6e67 656c 6f67  ([Full Changelog
+00002a60: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002a70: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00002a80: 7974 6572 5f63 6c69 656e 742f 636f 6d70  yter_client/comp
+00002a90: 6172 652f 7638 2e30 2e33 2e2e 2e65 3361  are/v8.0.3...e3a
+00002aa0: 6337 6136 3933 3535 6464 3161 6636 3630  c7a69355dd1af660
+00002ab0: 3338 6564 6137 3637 6535 3165 3932 6566  38eda767e51e92ef
+00002ac0: 3033 3466 6229 290a 0a23 2323 2042 7567  034fb))..### Bug
+00002ad0: 7320 6669 7865 640a 0a2d 2054 6872 6561  s fixed..- Threa
+00002ae0: 6465 645a 4d51 5374 7265 616d 3a20 636c  dedZMQStream: cl
+00002af0: 6f73 6520 7374 7265 616d 2062 6566 6f72  ose stream befor
+00002b00: 6520 736f 636b 6574 205b 2339 3336 5d28  e socket [#936](
+00002b10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002b20: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00002b30: 6572 5f63 6c69 656e 742f 7075 6c6c 2f39  er_client/pull/9
+00002b40: 3336 2920 285b 406d 696e 726b 5d28 6874  36) ([@minrk](ht
+00002b50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002b60: 2f6d 696e 726b 2929 0a0a 2323 2320 4d61  /minrk))..### Ma
+00002b70: 696e 7465 6e61 6e63 6520 616e 6420 7570  intenance and up
+00002b80: 6b65 6570 2069 6d70 726f 7665 6d65 6e74  keep improvement
+00002b90: 730a 0a23 2323 2044 6f63 756d 656e 7461  s..### Documenta
+00002ba0: 7469 6f6e 2069 6d70 726f 7665 6d65 6e74  tion improvement
+00002bb0: 730a 0a2d 2041 6464 7320 7370 6563 2066  s..- Adds spec f
+00002bc0: 6f72 2074 6865 2063 6f70 7954 6f47 6c6f  or the copyToGlo
+00002bd0: 6261 6c73 2072 6571 7565 7374 205b 2339  bals request [#9
+00002be0: 3332 5d28 6874 7470 733a 2f2f 6769 7468  32](https://gith
+00002bf0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00002c00: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+00002c10: 6c6c 2f39 3332 2920 285b 4062 7269 6368  ll/932) ([@brich
+00002c20: 6574 5d28 6874 7470 733a 2f2f 6769 7468  et](https://gith
+00002c30: 7562 2e63 6f6d 2f62 7269 6368 6574 2929  ub.com/brichet))
+00002c40: 0a0a 2323 2320 436f 6e74 7269 6275 746f  ..### Contributo
+00002c50: 7273 2074 6f20 7468 6973 2072 656c 6561  rs to this relea
+00002c60: 7365 0a0a 285b 4769 7448 7562 2063 6f6e  se..([GitHub con
+00002c70: 7472 6962 7574 6f72 7320 7061 6765 2066  tributors page f
+00002c80: 6f72 2074 6869 7320 7265 6c65 6173 655d  or this release]
+00002c90: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00002ca0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00002cb0: 7465 725f 636c 6965 6e74 2f67 7261 7068  ter_client/graph
+00002cc0: 732f 636f 6e74 7269 6275 746f 7273 3f66  s/contributors?f
+00002cd0: 726f 6d3d 3230 3233 2d30 322d 3136 2674  rom=2023-02-16&t
+00002ce0: 6f3d 3230 3233 2d30 332d 3230 2674 7970  o=2023-03-20&typ
+00002cf0: 653d 6329 290a 0a5b 4062 6c69 6e6b 3130  e=c))..[@blink10
+00002d00: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
+00002d10: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
+00002d20: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
+00002d30: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
+00002d40: 696e 766f 6c76 6573 2533 4162 6c69 6e6b  involves%3Ablink
+00002d50: 3130 3733 2b75 7064 6174 6564 2533 4132  1073+updated%3A2
+00002d60: 3032 332d 3032 2d31 362e 2e32 3032 332d  023-02-16..2023-
+00002d70: 3033 2d32 3026 7479 7065 3d49 7373 7565  03-20&type=Issue
+00002d80: 7329 207c 205b 4062 7269 6368 6574 5d28  s) | [@brichet](
 00002d90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002da0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-00002db0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f39  er_client/pull/9
-00002dc0: 3235 2920 285b 4062 6c69 6e6b 3130 3733  25) ([@blink1073
-00002dd0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00002de0: 2e63 6f6d 2f62 6c69 6e6b 3130 3733 2929  .com/blink1073))
-00002df0: 0a0a 2323 2320 4d61 696e 7465 6e61 6e63  ..### Maintenanc
-00002e00: 6520 616e 6420 7570 6b65 6570 2069 6d70  e and upkeep imp
-00002e10: 726f 7665 6d65 6e74 730a 0a2d 2041 646f  rovements..- Ado
-00002e20: 7074 206d 6f72 6520 7275 6666 2072 756c  pt more ruff rul
-00002e30: 6573 205b 2339 3234 5d28 6874 7470 733a  es [#924](https:
-00002e40: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-00002e50: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-00002e60: 656e 742f 7075 6c6c 2f39 3234 2920 285b  ent/pull/924) ([
-00002e70: 4062 6c69 6e6b 3130 3733 5d28 6874 7470  @blink1073](http
-00002e80: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-00002e90: 6c69 6e6b 3130 3733 2929 0a2d 2050 7265  link1073)).- Pre
-00002ea0: 6665 7220 7072 696e 7420 696e 206b 6572  fer print in ker
-00002eb0: 6e65 6c73 7065 6361 7070 205b 2339 3233  nelspecapp [#923
-00002ec0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00002ed0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00002ee0: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00002ef0: 2f39 3233 2920 285b 4062 6c69 6e6b 3130  /923) ([@blink10
-00002f00: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
-00002f10: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
-00002f20: 2929 0a0a 2323 2320 436f 6e74 7269 6275  ))..### Contribu
-00002f30: 746f 7273 2074 6f20 7468 6973 2072 656c  tors to this rel
-00002f40: 6561 7365 0a0a 285b 4769 7448 7562 2063  ease..([GitHub c
-00002f50: 6f6e 7472 6962 7574 6f72 7320 7061 6765  ontributors page
-00002f60: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
-00002f70: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00002f80: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-00002f90: 7079 7465 725f 636c 6965 6e74 2f67 7261  pyter_client/gra
-00002fa0: 7068 732f 636f 6e74 7269 6275 746f 7273  phs/contributors
-00002fb0: 3f66 726f 6d3d 3230 3233 2d30 312d 3236  ?from=2023-01-26
-00002fc0: 2674 6f3d 3230 3233 2d30 312d 3330 2674  &to=2023-01-30&t
-00002fd0: 7970 653d 6329 290a 0a5b 4062 6c69 6e6b  ype=c))..[@blink
-00002fe0: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
-00002ff0: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
-00003000: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
-00003010: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
-00003020: 742b 696e 766f 6c76 6573 2533 4162 6c69  t+involves%3Abli
-00003030: 6e6b 3130 3733 2b75 7064 6174 6564 2533  nk1073+updated%3
-00003040: 4132 3032 332d 3031 2d32 362e 2e32 3032  A2023-01-26..202
-00003050: 332d 3031 2d33 3026 7479 7065 3d49 7373  3-01-30&type=Iss
-00003060: 7565 7329 0a0a 2323 2038 2e30 2e31 0a0a  ues)..## 8.0.1..
-00003070: 285b 4675 6c6c 2043 6861 6e67 656c 6f67  ([Full Changelog
-00003080: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00003090: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-000030a0: 7974 6572 5f63 6c69 656e 742f 636f 6d70  yter_client/comp
-000030b0: 6172 652f 7638 2e30 2e30 2e2e 2e64 6336  are/v8.0.0...dc6
-000030c0: 3131 3363 3336 3065 3035 3132 3234 3330  113c360e05122430
-000030d0: 6238 6531 3330 3337 3465 3966 3465 3462  b8e130374e9f4e4b
-000030e0: 3730 3164 3729 290a 0a23 2323 2042 7567  701d7))..### Bug
-000030f0: 7320 6669 7865 640a 0a2d 2046 6978 206a  s fixed..- Fix j
-00003100: 736f 6e5f 6f75 7470 7574 2069 6e20 6b65  son_output in ke
-00003110: 726e 656c 7370 6563 2061 7070 205b 2339  rnelspec app [#9
-00003120: 3231 5d28 6874 7470 733a 2f2f 6769 7468  21](https://gith
-00003130: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00003140: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-00003150: 6c6c 2f39 3231 2920 285b 4062 6c69 6e6b  ll/921) ([@blink
-00003160: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
-00003170: 7468 7562 2e63 6f6d 2f62 6c69 6e6b 3130  thub.com/blink10
-00003180: 3733 2929 0a0a 2323 2320 436f 6e74 7269  73))..### Contri
-00003190: 6275 746f 7273 2074 6f20 7468 6973 2072  butors to this r
-000031a0: 656c 6561 7365 0a0a 285b 4769 7448 7562  elease..([GitHub
-000031b0: 2063 6f6e 7472 6962 7574 6f72 7320 7061   contributors pa
-000031c0: 6765 2066 6f72 2074 6869 7320 7265 6c65  ge for this rele
-000031d0: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
-000031e0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-000031f0: 6a75 7079 7465 725f 636c 6965 6e74 2f67  jupyter_client/g
-00003200: 7261 7068 732f 636f 6e74 7269 6275 746f  raphs/contributo
-00003210: 7273 3f66 726f 6d3d 3230 3233 2d30 312d  rs?from=2023-01-
-00003220: 3236 2674 6f3d 3230 3233 2d30 312d 3236  26&to=2023-01-26
-00003230: 2674 7970 653d 6329 290a 0a5b 4062 6c69  &type=c))..[@bli
-00003240: 6e6b 3130 3733 5d28 6874 7470 733a 2f2f  nk1073](https://
-00003250: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
-00003260: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
-00003270: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
-00003280: 656e 742b 696e 766f 6c76 6573 2533 4162  ent+involves%3Ab
-00003290: 6c69 6e6b 3130 3733 2b75 7064 6174 6564  link1073+updated
-000032a0: 2533 4132 3032 332d 3031 2d32 362e 2e32  %3A2023-01-26..2
-000032b0: 3032 332d 3031 2d32 3626 7479 7065 3d49  023-01-26&type=I
-000032c0: 7373 7565 7329 0a0a 2323 2038 2e30 2e30  ssues)..## 8.0.0
-000032d0: 0a0a 285b 4675 6c6c 2043 6861 6e67 656c  ..([Full Changel
-000032e0: 6f67 5d28 6874 7470 733a 2f2f 6769 7468  og](https://gith
-000032f0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00003300: 7570 7974 6572 5f63 6c69 656e 742f 636f  upyter_client/co
-00003310: 6d70 6172 652f 7637 2e33 2e35 2e2e 2e37  mpare/v7.3.5...7
-00003320: 3630 6137 3833 3564 3862 3230 6139 6461  60a7835d8b20a9da
-00003330: 6561 3337 3337 3735 3962 3137 3531 6435  ea3737759b1751d5
-00003340: 6535 3564 6164 3829 290a 0a54 6869 7320  e55dad8))..This 
-00003350: 7265 6c65 6173 6520 6973 2070 7269 6d61  release is prima
-00003360: 7269 6c79 2066 6f63 7573 6564 206f 6e20  rily focused on 
-00003370: 696d 7072 6f76 696e 6720 6061 7379 6e63  improving `async
-00003380: 696f 6020 7375 7070 6f72 742c 2077 6869  io` support, whi
-00003390: 6c65 2061 696d 696e 6720 746f 2068 6176  le aiming to hav
-000033a0: 6520 6d69 6e69 6d61 6c20 4150 4920 6368  e minimal API ch
-000033b0: 616e 6765 732e 0a0a 2323 2320 456e 6861  anges...### Enha
-000033c0: 6e63 656d 656e 7473 206d 6164 650a 0a2d  ncements made..-
-000033d0: 2052 656d 6f76 6520 6e65 7374 2d61 7379   Remove nest-asy
-000033e0: 6e63 696f 2064 6570 656e 6465 6e63 7920  ncio dependency 
-000033f0: 5b23 3833 355d 2868 7474 7073 3a2f 2f67  [#835](https://g
-00003400: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
-00003410: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
-00003420: 2f70 756c 6c2f 3833 3529 2028 5b40 626c  /pull/835) ([@bl
-00003430: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
-00003440: 2f67 6974 6875 622e 636f 6d2f 626c 696e  /github.com/blin
-00003450: 6b31 3037 3329 290a 0a23 2323 2042 7567  k1073))..### Bug
-00003460: 7320 6669 7865 640a 0a2d 2041 6c6c 6f77  s fixed..- Allow
-00003470: 2069 6e74 6572 7275 7074 2064 7572 696e   interrupt durin
-00003480: 6720 7265 7374 6172 7420 6f66 2070 656e  g restart of pen
-00003490: 6469 6e67 206b 6572 6e65 6c73 205b 2338  ding kernels [#8
-000034a0: 3938 5d28 6874 7470 733a 2f2f 6769 7468  98](https://gith
-000034b0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-000034c0: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-000034d0: 6c6c 2f38 3938 2920 285b 4062 6c69 6e6b  ll/898) ([@blink
-000034e0: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
-000034f0: 7468 7562 2e63 6f6d 2f62 6c69 6e6b 3130  thub.com/blink10
-00003500: 3733 2929 0a2d 2046 6978 2063 6f6e 6e65  73)).- Fix conne
-00003510: 6374 696f 6e20 7265 636f 6e63 696c 6961  ction reconcilia
-00003520: 7469 6f6e 2074 6f20 6861 6e64 6c65 2072  tion to handle r
-00003530: 6573 7461 7274 7320 5b23 3838 325d 2868  estarts [#882](h
-00003540: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003550: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00003560: 725f 636c 6965 6e74 2f70 756c 6c2f 3838  r_client/pull/88
-00003570: 3229 2028 5b40 6b65 7669 6e2d 6261 7465  2) ([@kevin-bate
-00003580: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00003590: 622e 636f 6d2f 6b65 7669 6e2d 6261 7465  b.com/kevin-bate
-000035a0: 7329 290a 2d20 5265 636f 6e63 696c 6520  s)).- Reconcile 
-000035b0: 636f 6e6e 6563 7469 6f6e 2069 6e66 6f72  connection infor
-000035c0: 6d61 7469 6f6e 205b 2338 3739 5d28 6874  mation [#879](ht
-000035d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000035e0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-000035f0: 5f63 6c69 656e 742f 7075 6c6c 2f38 3739  _client/pull/879
-00003600: 2920 285b 406b 6576 696e 2d62 6174 6573  ) ([@kevin-bates
+00002da0: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
+00002db0: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
+00002dc0: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
+00002dd0: 6c76 6573 2533 4162 7269 6368 6574 2b75  lves%3Abrichet+u
+00002de0: 7064 6174 6564 2533 4132 3032 332d 3032  pdated%3A2023-02
+00002df0: 2d31 362e 2e32 3032 332d 3033 2d32 3026  -16..2023-03-20&
+00002e00: 7479 7065 3d49 7373 7565 7329 207c 205b  type=Issues) | [
+00002e10: 406d 696e 726b 5d28 6874 7470 733a 2f2f  @minrk](https://
+00002e20: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
+00002e30: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
+00002e40: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
+00002e50: 656e 742b 696e 766f 6c76 6573 2533 416d  ent+involves%3Am
+00002e60: 696e 726b 2b75 7064 6174 6564 2533 4132  inrk+updated%3A2
+00002e70: 3032 332d 3032 2d31 362e 2e32 3032 332d  023-02-16..2023-
+00002e80: 3033 2d32 3026 7479 7065 3d49 7373 7565  03-20&type=Issue
+00002e90: 7329 207c 205b 4070 7265 2d63 6f6d 6d69  s) | [@pre-commi
+00002ea0: 742d 6369 5d28 6874 7470 733a 2f2f 6769  t-ci](https://gi
+00002eb0: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
+00002ec0: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
+00002ed0: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
+00002ee0: 742b 696e 766f 6c76 6573 2533 4170 7265  t+involves%3Apre
+00002ef0: 2d63 6f6d 6d69 742d 6369 2b75 7064 6174  -commit-ci+updat
+00002f00: 6564 2533 4132 3032 332d 3032 2d31 362e  ed%3A2023-02-16.
+00002f10: 2e32 3032 332d 3033 2d32 3026 7479 7065  .2023-03-20&type
+00002f20: 3d49 7373 7565 7329 0a0a 2323 2038 2e30  =Issues)..## 8.0
+00002f30: 2e33 0a0a 285b 4675 6c6c 2043 6861 6e67  .3..([Full Chang
+00002f40: 656c 6f67 5d28 6874 7470 733a 2f2f 6769  elog](https://gi
+00002f50: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+00002f60: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+00002f70: 636f 6d70 6172 652f 7638 2e30 2e32 2e2e  compare/v8.0.2..
+00002f80: 2e64 6330 6561 6261 3166 3630 3930 3739  .dc0eaba1f609079
+00002f90: 3637 3265 6337 3339 6663 6439 3737 6463  672ec739fcd977dc
+00002fa0: 3434 3433 3164 6139 3229 290a 0a23 2323  44431da92))..###
+00002fb0: 2042 7567 7320 6669 7865 640a 0a2d 2046   Bugs fixed..- F
+00002fc0: 6978 206b 6572 6e65 6c73 7065 6320 7072  ix kernelspec pr
+00002fd0: 696e 7420 6f75 7470 7574 205b 2339 3333  int output [#933
+00002fe0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002ff0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00003000: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00003010: 2f39 3333 2920 285b 406d 696e 726b 5d28  /933) ([@minrk](
+00003020: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003030: 6f6d 2f6d 696e 726b 2929 0a2d 2044 6f6e  om/minrk)).- Don
+00003040: 2774 2065 6d69 7420 6120 7472 6169 6c6e  't emit a trailn
+00003050: 6720 6e65 776c 696e 6520 696e 2062 6173  g newline in bas
+00003060: 6536 342d 656e 636f 6465 6420 6461 7461  e64-encoded data
+00003070: 206c 696b 6520 2769 6d61 6765 2f70 6e67   like 'image/png
+00003080: 2720 5b23 3933 315d 2868 7474 7073 3a2f  ' [#931](https:/
+00003090: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+000030a0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+000030b0: 6e74 2f70 756c 6c2f 3933 3129 2028 5b40  nt/pull/931) ([@
+000030c0: 786c 305d 2868 7474 7073 3a2f 2f67 6974  xl0](https://git
+000030d0: 6875 622e 636f 6d2f 786c 3029 290a 0a23  hub.com/xl0))..#
+000030e0: 2323 204d 6169 6e74 656e 616e 6365 2061  ## Maintenance a
+000030f0: 6e64 2075 706b 6565 7020 696d 7072 6f76  nd upkeep improv
+00003100: 656d 656e 7473 0a0a 2d20 4164 6420 6c69  ements..- Add li
+00003110: 6365 6e73 6520 5b23 3933 345d 2868 7474  cense [#934](htt
+00003120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00003130: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00003140: 636c 6965 6e74 2f70 756c 6c2f 3933 3429  client/pull/934)
+00003150: 2028 5b40 6463 7361 6261 3839 5d28 6874   ([@dcsaba89](ht
+00003160: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00003170: 2f64 6373 6162 6138 3929 290a 2d20 496d  /dcsaba89)).- Im
+00003180: 7072 6f76 696e 6720 6a73 6f6e 7574 696c  proving jsonutil
+00003190: 2074 6573 7473 205b 2339 3239 5d28 6874   tests [#929](ht
+000031a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000031b0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+000031c0: 5f63 6c69 656e 742f 7075 6c6c 2f39 3239  _client/pull/929
+000031d0: 2920 285b 4061 6e64 7265 686f 7261 5d28  ) ([@andrehora](
+000031e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000031f0: 6f6d 2f61 6e64 7265 686f 7261 2929 0a0a  om/andrehora))..
+00003200: 2323 2320 436f 6e74 7269 6275 746f 7273  ### Contributors
+00003210: 2074 6f20 7468 6973 2072 656c 6561 7365   to this release
+00003220: 0a0a 285b 4769 7448 7562 2063 6f6e 7472  ..([GitHub contr
+00003230: 6962 7574 6f72 7320 7061 6765 2066 6f72  ibutors page for
+00003240: 2074 6869 7320 7265 6c65 6173 655d 2868   this release](h
+00003250: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00003260: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+00003270: 725f 636c 6965 6e74 2f67 7261 7068 732f  r_client/graphs/
+00003280: 636f 6e74 7269 6275 746f 7273 3f66 726f  contributors?fro
+00003290: 6d3d 3230 3233 2d30 312d 3330 2674 6f3d  m=2023-01-30&to=
+000032a0: 3230 3233 2d30 322d 3136 2674 7970 653d  2023-02-16&type=
+000032b0: 6329 290a 0a5b 4061 6e64 7265 686f 7261  c))..[@andrehora
+000032c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000032d0: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
+000032e0: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
+000032f0: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
+00003300: 766f 6c76 6573 2533 4161 6e64 7265 686f  volves%3Aandreho
+00003310: 7261 2b75 7064 6174 6564 2533 4132 3032  ra+updated%3A202
+00003320: 332d 3031 2d33 302e 2e32 3032 332d 3032  3-01-30..2023-02
+00003330: 2d31 3626 7479 7065 3d49 7373 7565 7329  -16&type=Issues)
+00003340: 207c 205b 4062 6c69 6e6b 3130 3733 5d28   | [@blink1073](
+00003350: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003360: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
+00003370: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
+00003380: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
+00003390: 6c76 6573 2533 4162 6c69 6e6b 3130 3733  lves%3Ablink1073
+000033a0: 2b75 7064 6174 6564 2533 4132 3032 332d  +updated%3A2023-
+000033b0: 3031 2d33 302e 2e32 3032 332d 3032 2d31  01-30..2023-02-1
+000033c0: 3626 7479 7065 3d49 7373 7565 7329 207c  6&type=Issues) |
+000033d0: 205b 4064 6373 6162 6138 395d 2868 7474   [@dcsaba89](htt
+000033e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000033f0: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
+00003400: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
+00003410: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
+00003420: 7325 3341 6463 7361 6261 3839 2b75 7064  s%3Adcsaba89+upd
+00003430: 6174 6564 2533 4132 3032 332d 3031 2d33  ated%3A2023-01-3
+00003440: 302e 2e32 3032 332d 3032 2d31 3626 7479  0..2023-02-16&ty
+00003450: 7065 3d49 7373 7565 7329 207c 205b 406b  pe=Issues) | [@k
+00003460: 6576 696e 2d62 6174 6573 5d28 6874 7470  evin-bates](http
+00003470: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00003480: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
+00003490: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
+000034a0: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
+000034b0: 2533 416b 6576 696e 2d62 6174 6573 2b75  %3Akevin-bates+u
+000034c0: 7064 6174 6564 2533 4132 3032 332d 3031  pdated%3A2023-01
+000034d0: 2d33 302e 2e32 3032 332d 3032 2d31 3626  -30..2023-02-16&
+000034e0: 7479 7065 3d49 7373 7565 7329 207c 205b  type=Issues) | [
+000034f0: 406d 696e 726b 5d28 6874 7470 733a 2f2f  @minrk](https://
+00003500: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
+00003510: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
+00003520: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
+00003530: 656e 742b 696e 766f 6c76 6573 2533 416d  ent+involves%3Am
+00003540: 696e 726b 2b75 7064 6174 6564 2533 4132  inrk+updated%3A2
+00003550: 3032 332d 3031 2d33 302e 2e32 3032 332d  023-01-30..2023-
+00003560: 3032 2d31 3626 7479 7065 3d49 7373 7565  02-16&type=Issue
+00003570: 7329 207c 205b 4070 7265 2d63 6f6d 6d69  s) | [@pre-commi
+00003580: 742d 6369 5d28 6874 7470 733a 2f2f 6769  t-ci](https://gi
+00003590: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
+000035a0: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
+000035b0: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
+000035c0: 742b 696e 766f 6c76 6573 2533 4170 7265  t+involves%3Apre
+000035d0: 2d63 6f6d 6d69 742d 6369 2b75 7064 6174  -commit-ci+updat
+000035e0: 6564 2533 4132 3032 332d 3031 2d33 302e  ed%3A2023-01-30.
+000035f0: 2e32 3032 332d 3032 2d31 3626 7479 7065  .2023-02-16&type
+00003600: 3d49 7373 7565 7329 207c 205b 4078 6c30  =Issues) | [@xl0
 00003610: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00003620: 2e63 6f6d 2f6b 6576 696e 2d62 6174 6573  .com/kevin-bates
-00003630: 2929 0a2d 2057 6f72 6b61 726f 756e 6420  )).- Workaround 
-00003640: 666f 7220 6c61 756e 6368 2062 7567 205b  for launch bug [
-00003650: 2338 3631 5d28 6874 7470 733a 2f2f 6769  #861](https://gi
-00003660: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-00003670: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-00003680: 7075 6c6c 2f38 3631 2920 285b 4062 6c69  pull/861) ([@bli
-00003690: 6e6b 3130 3733 5d28 6874 7470 733a 2f2f  nk1073](https://
-000036a0: 6769 7468 7562 2e63 6f6d 2f62 6c69 6e6b  github.com/blink
-000036b0: 3130 3733 2929 0a2d 2044 6566 6572 2063  1073)).- Defer c
-000036c0: 7265 6174 696f 6e20 6f66 2072 6561 6479  reation of ready
-000036d0: 2066 7574 7572 6520 5b23 3835 385d 2868   future [#858](h
-000036e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000036f0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00003700: 725f 636c 6965 6e74 2f70 756c 6c2f 3835  r_client/pull/85
-00003710: 3829 2028 5b40 626c 696e 6b31 3037 335d  8) ([@blink1073]
-00003720: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003730: 636f 6d2f 626c 696e 6b31 3037 3329 290a  com/blink1073)).
-00003740: 2d20 4669 7820 6861 6e64 6c69 6e67 206f  - Fix handling o
-00003750: 6620 696e 6974 6961 6c20 7265 6164 7920  f initial ready 
-00003760: 7072 6f6d 6973 6520 5b23 3835 345d 2868  promise [#854](h
-00003770: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003780: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00003790: 725f 636c 6965 6e74 2f70 756c 6c2f 3835  r_client/pull/85
-000037a0: 3429 2028 5b40 626c 696e 6b31 3037 335d  4) ([@blink1073]
-000037b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000037c0: 636f 6d2f 626c 696e 6b31 3037 3329 290a  com/blink1073)).
-000037d0: 2d20 5265 7665 7274 2022 4669 7820 7065  - Revert "Fix pe
-000037e0: 6e64 696e 6720 6b65 726e 656c 7320 6167  nding kernels ag
-000037f0: 6169 6e22 205b 2338 3533 5d28 6874 7470  ain" [#853](http
-00003800: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00003810: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00003820: 6c69 656e 742f 7075 6c6c 2f38 3533 2920  lient/pull/853) 
-00003830: 285b 4062 6c69 6e6b 3130 3733 5d28 6874  ([@blink1073](ht
-00003840: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003850: 2f62 6c69 6e6b 3130 3733 2929 0a2d 2046  /blink1073)).- F
-00003860: 6978 2070 656e 6469 6e67 206b 6572 6e65  ix pending kerne
-00003870: 6c73 2061 6761 696e 205b 2338 3435 5d28  ls again [#845](
-00003880: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00003890: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-000038a0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f38  er_client/pull/8
-000038b0: 3435 2920 285b 4062 6c69 6e6b 3130 3733  45) ([@blink1073
-000038c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000038d0: 2e63 6f6d 2f62 6c69 6e6b 3130 3733 2929  .com/blink1073))
-000038e0: 0a2d 2055 7365 2070 7974 6573 745f 6173  .- Use pytest_as
-000038f0: 796e 6369 6f20 6669 7874 7572 6520 5b23  yncio fixture [#
-00003900: 3832 365d 2868 7474 7073 3a2f 2f67 6974  826](https://git
-00003910: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-00003920: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-00003930: 756c 6c2f 3832 3629 2028 5b40 6461 7669  ull/826) ([@davi
-00003940: 6462 726f 6368 6172 745d 2868 7474 7073  dbrochart](https
-00003950: 3a2f 2f67 6974 6875 622e 636f 6d2f 6461  ://github.com/da
-00003960: 7669 6462 726f 6368 6172 7429 290a 0a23  vidbrochart))..#
-00003970: 2323 204d 6169 6e74 656e 616e 6365 2061  ## Maintenance a
-00003980: 6e64 2075 706b 6565 7020 696d 7072 6f76  nd upkeep improv
-00003990: 656d 656e 7473 0a0a 2d20 4d41 494e 543a  ements..- MAINT:
-000039a0: 2044 6f6e 2774 2066 6f72 6d61 7420 6c6f   Don't format lo
-000039b0: 6720 696e 206c 6f67 2063 616c 6c2e 205b  g in log call. [
-000039c0: 2339 3139 5d28 6874 7470 733a 2f2f 6769  #919](https://gi
-000039d0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-000039e0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-000039f0: 7075 6c6c 2f39 3139 2920 285b 4043 6172  pull/919) ([@Car
-00003a00: 7265 6175 5d28 6874 7470 733a 2f2f 6769  reau](https://gi
-00003a10: 7468 7562 2e63 6f6d 2f43 6172 7265 6175  thub.com/Carreau
-00003a20: 2929 0a2d 2052 656d 6f76 6520 6465 7072  )).- Remove depr
-00003a30: 6563 6174 6564 207a 6d71 2069 6d70 6f72  ecated zmq impor
-00003a40: 7473 205b 2339 3135 5d28 6874 7470 733a  ts [#915](https:
-00003a50: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-00003a60: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-00003a70: 656e 742f 7075 6c6c 2f39 3135 2920 285b  ent/pull/915) ([
-00003a80: 4062 6c69 6e6b 3130 3733 5d28 6874 7470  @blink1073](http
-00003a90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-00003aa0: 6c69 6e6b 3130 3733 2929 0a2d 204d 4149  link1073)).- MAI
-00003ab0: 4e54 3a20 636f 6e73 6973 7465 6e74 6c79  NT: consistently
-00003ac0: 2075 7365 2072 656c 6174 6976 6520 696d   use relative im
-00003ad0: 706f 7274 732e 205b 2339 3132 5d28 6874  ports. [#912](ht
-00003ae0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003af0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00003b00: 5f63 6c69 656e 742f 7075 6c6c 2f39 3132  _client/pull/912
-00003b10: 2920 285b 4043 6172 7265 6175 5d28 6874  ) ([@Carreau](ht
-00003b20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003b30: 2f43 6172 7265 6175 2929 0a2d 2053 796e  /Carreau)).- Syn
-00003b40: 6320 6c69 6e74 2064 6570 7320 5b23 3931  c lint deps [#91
-00003b50: 315d 2868 7474 7073 3a2f 2f67 6974 6875  1](https://githu
-00003b60: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-00003b70: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-00003b80: 6c2f 3931 3129 2028 5b40 626c 696e 6b31  l/911) ([@blink1
-00003b90: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
-00003ba0: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
-00003bb0: 3329 290a 2d20 4d41 494e 543a 2050 726f  3)).- MAINT: Pro
-00003bc0: 7065 7220 7479 7069 6e67 2061 6e64 2063  per typing and c
-00003bd0: 6173 7420 5b23 3930 365d 2868 7474 7073  ast [#906](https
-00003be0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00003bf0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-00003c00: 6965 6e74 2f70 756c 6c2f 3930 3629 2028  ient/pull/906) (
-00003c10: 5b40 4361 7272 6561 755d 2868 7474 7073  [@Carreau](https
-00003c20: 3a2f 2f67 6974 6875 622e 636f 6d2f 4361  ://github.com/Ca
-00003c30: 7272 6561 7529 290a 2d20 4d41 494e 543a  rreau)).- MAINT:
-00003c40: 205c 5b5f 6173 796e 635f 5c5d 7374 6172   \[_async_\]star
-00003c50: 745f 6b65 726e 656c 2073 686f 756c 6420  t_kernel should 
-00003c60: 6f6e 6c79 2074 616b 6520 6b77 6172 6720  only take kwarg 
-00003c70: 6f6e 6c79 2e20 5b23 3930 355d 2868 7474  only. [#905](htt
-00003c80: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003c90: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00003ca0: 636c 6965 6e74 2f70 756c 6c2f 3930 3529  client/pull/905)
-00003cb0: 2028 5b40 4361 7272 6561 755d 2868 7474   ([@Carreau](htt
-00003cc0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003cd0: 4361 7272 6561 7529 290a 2d20 4164 6420  Carreau)).- Add 
-00003ce0: 6d6f 7265 2063 6920 6368 6563 6b73 205b  more ci checks [
-00003cf0: 2339 3033 5d28 6874 7470 733a 2f2f 6769  #903](https://gi
-00003d00: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-00003d10: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-00003d20: 7075 6c6c 2f39 3033 2920 285b 4062 6c69  pull/903) ([@bli
-00003d30: 6e6b 3130 3733 5d28 6874 7470 733a 2f2f  nk1073](https://
-00003d40: 6769 7468 7562 2e63 6f6d 2f62 6c69 6e6b  github.com/blink
-00003d50: 3130 3733 2929 0a2d 2041 6c6c 6f77 2072  1073)).- Allow r
-00003d60: 656c 6561 7369 6e67 2066 726f 6d20 7265  eleasing from re
-00003d70: 706f 205b 2338 3939 5d28 6874 7470 733a  po [#899](https:
-00003d80: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-00003d90: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-00003da0: 656e 742f 7075 6c6c 2f38 3939 2920 285b  ent/pull/899) ([
-00003db0: 4062 6c69 6e6b 3130 3733 5d28 6874 7470  @blink1073](http
-00003dc0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-00003dd0: 6c69 6e6b 3130 3733 2929 0a2d 2046 6978  link1073)).- Fix
-00003de0: 206a 7570 7974 6572 5f63 6f72 6520 7069   jupyter_core pi
-00003df0: 6e6e 696e 6720 5b23 3839 365d 2868 7474  nning [#896](htt
-00003e00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003e10: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00003e20: 636c 6965 6e74 2f70 756c 6c2f 3839 3629  client/pull/896)
-00003e30: 2028 5b40 6f70 6869 6532 3030 5d28 6874   ([@ophie200](ht
-00003e40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003e50: 2f6f 7068 6965 3230 3029 290a 2d20 4164  /ophie200)).- Ad
-00003e60: 6f70 7420 7275 6666 2061 6e64 2072 6564  opt ruff and red
-00003e70: 7563 6520 7072 652d 636f 6d6d 6974 2075  uce pre-commit u
-00003e80: 7361 6765 205b 2338 3935 5d28 6874 7470  sage [#895](http
-00003e90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00003ea0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00003eb0: 6c69 656e 742f 7075 6c6c 2f38 3935 2920  lient/pull/895) 
-00003ec0: 285b 4062 6c69 6e6b 3130 3733 5d28 6874  ([@blink1073](ht
-00003ed0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003ee0: 2f62 6c69 6e6b 3130 3733 2929 0a2d 2055  /blink1073)).- U
-00003ef0: 7365 2070 7974 6573 742d 6a75 7079 7465  se pytest-jupyte
-00003f00: 7220 5b23 3839 315d 2868 7474 7073 3a2f  r [#891](https:/
-00003f10: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-00003f20: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-00003f30: 6e74 2f70 756c 6c2f 3839 3129 2028 5b40  nt/pull/891) ([@
-00003f40: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
-00003f50: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
-00003f60: 696e 6b31 3037 3329 290a 2d20 496d 706f  ink1073)).- Impo
-00003f70: 7274 2065 6e73 7572 655f 6173 796e 6320  rt ensure_async 
-00003f80: 616e 6420 7275 6e5f 7379 6e63 2066 726f  and run_sync fro
-00003f90: 6d20 6a75 7079 7465 725f 636f 7265 205b  m jupyter_core [
-00003fa0: 2338 3839 5d28 6874 7470 733a 2f2f 6769  #889](https://gi
-00003fb0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-00003fc0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-00003fd0: 7075 6c6c 2f38 3839 2920 285b 4064 6176  pull/889) ([@dav
-00003fe0: 6964 6272 6f63 6861 7274 5d28 6874 7470  idbrochart](http
-00003ff0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-00004000: 6176 6964 6272 6f63 6861 7274 2929 0a2d  avidbrochart)).-
-00004010: 2055 7365 2062 6173 6520 7365 7475 7020   Use base setup 
-00004020: 6465 7065 6e64 656e 6379 2074 7970 6520  dependency type 
-00004030: 5b23 3838 385d 2868 7474 7073 3a2f 2f67  [#888](https://g
-00004040: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
-00004050: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
-00004060: 2f70 756c 6c2f 3838 3829 2028 5b40 626c  /pull/888) ([@bl
-00004070: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
-00004080: 2f67 6974 6875 622e 636f 6d2f 626c 696e  /github.com/blin
-00004090: 6b31 3037 3329 290a 2d20 4d6f 7265 2043  k1073)).- More C
-000040a0: 4920 436c 6561 6e75 7020 5b23 3838 365d  I Cleanup [#886]
-000040b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000040c0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-000040d0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-000040e0: 3838 3629 2028 5b40 626c 696e 6b31 3037  886) ([@blink107
-000040f0: 335d 2868 7474 7073 3a2f 2f67 6974 6875  3](https://githu
-00004100: 622e 636f 6d2f 626c 696e 6b31 3037 3329  b.com/blink1073)
-00004110: 290a 2d20 4d6f 7265 2063 6f76 6572 6167  ).- More coverag
-00004120: 6520 5b23 3838 355d 2868 7474 7073 3a2f  e [#885](https:/
-00004130: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-00004140: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-00004150: 6e74 2f70 756c 6c2f 3838 3529 2028 5b40  nt/pull/885) ([@
-00004160: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
-00004170: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
-00004180: 696e 6b31 3037 3329 290a 2d20 436c 6561  ink1073)).- Clea
-00004190: 6e20 7570 2077 6f72 6b66 6c6f 7720 616e  n up workflow an
-000041a0: 6420 7079 7072 6f6a 6563 7420 5b23 3838  d pyproject [#88
-000041b0: 345d 2868 7474 7073 3a2f 2f67 6974 6875  4](https://githu
-000041c0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-000041d0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-000041e0: 6c2f 3838 3429 2028 5b40 626c 696e 6b31  l/884) ([@blink1
-000041f0: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
-00004200: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
-00004210: 3329 290a 2d20 4164 6420 6d6f 7265 2063  3)).- Add more c
-00004220: 6f76 6572 6167 6520 5b23 3837 375d 2868  overage [#877](h
-00004230: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004240: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00004250: 725f 636c 6965 6e74 2f70 756c 6c2f 3837  r_client/pull/87
-00004260: 3729 2028 5b40 626c 696e 6b31 3037 335d  7) ([@blink1073]
-00004270: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00004280: 636f 6d2f 626c 696e 6b31 3037 3329 290a  com/blink1073)).
-00004290: 2d20 4164 6420 636f 7665 7261 6765 2063  - Add coverage c
-000042a0: 6f6e 6669 6720 5b23 3837 365d 2868 7474  onfig [#876](htt
-000042b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000042c0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-000042d0: 636c 6965 6e74 2f70 756c 6c2f 3837 3629  client/pull/876)
-000042e0: 2028 5b40 626c 696e 6b31 3037 335d 2868   ([@blink1073](h
-000042f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004300: 6d2f 626c 696e 6b31 3037 3329 290a 2d20  m/blink1073)).- 
-00004310: 4275 6d70 2061 6374 696f 6e73 2f73 6574  Bump actions/set
-00004320: 7570 2d70 7974 686f 6e20 6672 6f6d 2032  up-python from 2
-00004330: 2074 6f20 3420 5b23 3837 345d 2868 7474   to 4 [#874](htt
-00004340: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00004350: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00004360: 636c 6965 6e74 2f70 756c 6c2f 3837 3429  client/pull/874)
-00004370: 2028 5b40 6465 7065 6e64 6162 6f74 5d28   ([@dependabot](
-00004380: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00004390: 6f6d 2f64 6570 656e 6461 626f 7429 290a  om/dependabot)).
-000043a0: 2d20 4275 6d70 2061 6374 696f 6e73 2f63  - Bump actions/c
-000043b0: 6865 636b 6f75 7420 6672 6f6d 2032 2074  heckout from 2 t
-000043c0: 6f20 3320 5b23 3837 335d 2868 7474 7073  o 3 [#873](https
-000043d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-000043e0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-000043f0: 6965 6e74 2f70 756c 6c2f 3837 3329 2028  ient/pull/873) (
-00004400: 5b40 6465 7065 6e64 6162 6f74 5d28 6874  [@dependabot](ht
-00004410: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00004420: 2f64 6570 656e 6461 626f 7429 290a 2d20  /dependabot)).- 
-00004430: 5573 6520 706c 6174 666f 726d 2064 6972  Use platform dir
-00004440: 7320 696e 2074 6573 7473 205b 2338 3732  s in tests [#872
-00004450: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00004460: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00004470: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00004480: 2f38 3732 2920 285b 4062 6c69 6e6b 3130  /872) ([@blink10
-00004490: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
-000044a0: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
-000044b0: 2929 0a2d 2043 6c65 616e 2075 7020 7479  )).- Clean up ty
-000044c0: 7065 7320 616e 6420 7265 6d6f 7665 2075  pes and remove u
-000044d0: 7365 206f 6620 656e 7472 7970 6f69 6e74  se of entrypoint
-000044e0: 7320 5b23 3837 315d 2868 7474 7073 3a2f  s [#871](https:/
-000044f0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-00004500: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-00004510: 6e74 2f70 756c 6c2f 3837 3129 2028 5b40  nt/pull/871) ([@
-00004520: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
-00004530: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
-00004540: 696e 6b31 3037 3329 290a 2d20 4164 6420  ink1073)).- Add 
-00004550: 6465 7065 6e64 6162 6f74 205b 2338 3730  dependabot [#870
-00004560: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00004570: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00004580: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00004590: 2f38 3730 2920 285b 4062 6c69 6e6b 3130  /870) ([@blink10
-000045a0: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
-000045b0: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
-000045c0: 2929 0a2d 2053 7570 706f 7274 2050 7974  )).- Support Pyt
-000045d0: 686f 6e20 332e 382d 332e 3131 205b 2338  hon 3.8-3.11 [#8
-000045e0: 3636 5d28 6874 7470 733a 2f2f 6769 7468  66](https://gith
-000045f0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00004600: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-00004610: 6c6c 2f38 3636 2920 285b 4062 6c69 6e6b  ll/866) ([@blink
-00004620: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
-00004630: 7468 7562 2e63 6f6d 2f62 6c69 6e6b 3130  thub.com/blink10
-00004640: 3733 2929 0a2d 2046 6978 2061 7373 6572  73)).- Fix asser
-00004650: 7469 6f6e 2069 6e20 6054 6573 7453 6573  tion in `TestSes
-00004660: 7369 6f6e 2e74 6573 745f 7365 7269 616c  sion.test_serial
-00004670: 697a 6560 205b 2338 3630 5d28 6874 7470  ize` [#860](http
-00004680: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00004690: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-000046a0: 6c69 656e 742f 7075 6c6c 2f38 3630 2920  lient/pull/860) 
-000046b0: 285b 4073 616d 7261 745d 2868 7474 7073  ([@samrat](https
-000046c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7361  ://github.com/sa
-000046d0: 6d72 6174 2929 0a2d 204d 6169 6e74 656e  mrat)).- Mainten
-000046e0: 616e 6365 2063 6c65 616e 7570 205b 2338  ance cleanup [#8
-000046f0: 3536 5d28 6874 7470 733a 2f2f 6769 7468  56](https://gith
-00004700: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00004710: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-00004720: 6c6c 2f38 3536 2920 285b 4062 6c69 6e6b  ll/856) ([@blink
-00004730: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
-00004740: 7468 7562 2e63 6f6d 2f62 6c69 6e6b 3130  thub.com/blink10
-00004750: 3733 2929 0a2d 2049 676e 6f72 6520 7761  73)).- Ignore wa
-00004760: 726e 696e 6773 2069 6e20 7072 6572 656c  rnings in prerel
-00004770: 6561 7365 7320 7465 7374 205b 2338 3434  eases test [#844
-00004780: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00004790: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-000047a0: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-000047b0: 2f38 3434 2920 285b 4062 6c69 6e6b 3130  /844) ([@blink10
-000047c0: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
-000047d0: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
-000047e0: 2929 0a2d 2055 7365 2068 6174 6368 2066  )).- Use hatch f
-000047f0: 6f72 2076 6572 7369 6f6e 205b 2338 3337  or version [#837
-00004800: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00004810: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00004820: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00004830: 2f38 3337 2920 285b 4062 6c69 6e6b 3130  /837) ([@blink10
-00004840: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
-00004850: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
-00004860: 2929 0a2d 204d 6f76 6520 7465 7374 7320  )).- Move tests 
-00004870: 746f 2074 6f70 206c 6576 656c 205b 2338  to top level [#8
-00004880: 3334 5d28 6874 7470 733a 2f2f 6769 7468  34](https://gith
-00004890: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-000048a0: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-000048b0: 6c6c 2f38 3334 2920 285b 4062 6c69 6e6b  ll/834) ([@blink
-000048c0: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
-000048d0: 7468 7562 2e63 6f6d 2f62 6c69 6e6b 3130  thub.com/blink10
-000048e0: 3733 2929 0a2d 2046 6978 206e 6263 6f6e  73)).- Fix nbcon
-000048f0: 7665 7274 2064 6f77 6e73 7472 6561 6d20  vert downstream 
-00004900: 7465 7374 205b 2338 3237 5d28 6874 7470  test [#827](http
-00004910: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00004920: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00004930: 6c69 656e 742f 7075 6c6c 2f38 3237 2920  lient/pull/827) 
-00004940: 285b 4062 6c69 6e6b 3130 3733 5d28 6874  ([@blink1073](ht
-00004950: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00004960: 2f62 6c69 6e6b 3130 3733 2929 0a0a 2323  /blink1073))..##
-00004970: 2320 446f 6375 6d65 6e74 6174 696f 6e20  # Documentation 
-00004980: 696d 7072 6f76 656d 656e 7473 0a0a 2d20  improvements..- 
-00004990: 5265 666c 6563 7420 6375 7272 656e 7420  Reflect current 
-000049a0: 7072 6f74 6f63 6f6c 2076 6572 7369 6f6e  protocol version
-000049b0: 2069 6e20 646f 6375 6d65 6e74 6174 696f   in documentatio
-000049c0: 6e20 5b23 3931 385d 2868 7474 7073 3a2f  n [#918](https:/
-000049d0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-000049e0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-000049f0: 6e74 2f70 756c 6c2f 3931 3829 2028 5b40  nt/pull/918) ([@
-00004a00: 5379 6c76 6169 6e43 6f72 6c61 795d 2868  SylvainCorlay](h
-00004a10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004a20: 6d2f 5379 6c76 6169 6e43 6f72 6c61 7929  m/SylvainCorlay)
-00004a30: 290a 2d20 4164 6420 6675 6c6c 2061 7069  ).- Add full api
-00004a40: 2064 6f63 7320 5b23 3930 385d 2868 7474   docs [#908](htt
-00004a50: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00004a60: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00004a70: 636c 6965 6e74 2f70 756c 6c2f 3930 3829  client/pull/908)
-00004a80: 2028 5b40 626c 696e 6b31 3037 335d 2868   ([@blink1073](h
-00004a90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004aa0: 6d2f 626c 696e 6b31 3037 3329 290a 2d20  m/blink1073)).- 
-00004ab0: 4164 6420 6d6f 7265 2063 6920 6368 6563  Add more ci chec
-00004ac0: 6b73 205b 2339 3033 5d28 6874 7470 733a  ks [#903](https:
-00004ad0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-00004ae0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-00004af0: 656e 742f 7075 6c6c 2f39 3033 2920 285b  ent/pull/903) ([
-00004b00: 4062 6c69 6e6b 3130 3733 5d28 6874 7470  @blink1073](http
-00004b10: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-00004b20: 6c69 6e6b 3130 3733 2929 0a2d 2053 7769  link1073)).- Swi
-00004b30: 7463 6820 746f 2070 7964 6174 6120 7370  tch to pydata sp
-00004b40: 6869 6e78 2074 6865 6d65 205b 2338 3430  hinx theme [#840
-00004b50: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00004b60: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00004b70: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00004b80: 2f38 3430 2920 285b 4062 6c69 6e6b 3130  /840) ([@blink10
-00004b90: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
-00004ba0: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
-00004bb0: 2929 0a0a 2323 2320 436f 6e74 7269 6275  ))..### Contribu
-00004bc0: 746f 7273 2074 6f20 7468 6973 2072 656c  tors to this rel
-00004bd0: 6561 7365 0a0a 285b 4769 7448 7562 2063  ease..([GitHub c
-00004be0: 6f6e 7472 6962 7574 6f72 7320 7061 6765  ontributors page
-00004bf0: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
-00004c00: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00004c10: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-00004c20: 7079 7465 725f 636c 6965 6e74 2f67 7261  pyter_client/gra
-00004c30: 7068 732f 636f 6e74 7269 6275 746f 7273  phs/contributors
-00004c40: 3f66 726f 6d3d 3230 3232 2d30 382d 3235  ?from=2022-08-25
-00004c50: 2674 6f3d 3230 3233 2d30 312d 3236 2674  &to=2023-01-26&t
-00004c60: 7970 653d 6329 290a 0a5b 4061 726f 676f  ype=c))..[@arogo
-00004c70: 7a68 6e69 6b6f 765d 2868 7474 7073 3a2f  zhnikov](https:/
-00004c80: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-00004c90: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-00004ca0: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-00004cb0: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-00004cc0: 6172 6f67 6f7a 686e 696b 6f76 2b75 7064  arogozhnikov+upd
-00004cd0: 6174 6564 2533 4132 3032 322d 3038 2d32  ated%3A2022-08-2
-00004ce0: 352e 2e32 3032 332d 3031 2d32 3626 7479  5..2023-01-26&ty
-00004cf0: 7065 3d49 7373 7565 7329 207c 205b 4062  pe=Issues) | [@b
-00004d00: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
-00004d10: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
-00004d20: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
-00004d30: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
-00004d40: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
-00004d50: 4162 6c69 6e6b 3130 3733 2b75 7064 6174  Ablink1073+updat
-00004d60: 6564 2533 4132 3032 322d 3038 2d32 352e  ed%3A2022-08-25.
-00004d70: 2e32 3032 332d 3031 2d32 3626 7479 7065  .2023-01-26&type
-00004d80: 3d49 7373 7565 7329 207c 205b 4043 6172  =Issues) | [@Car
-00004d90: 7265 6175 5d28 6874 7470 733a 2f2f 6769  reau](https://gi
-00004da0: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
-00004db0: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
-00004dc0: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
-00004dd0: 742b 696e 766f 6c76 6573 2533 4143 6172  t+involves%3ACar
-00004de0: 7265 6175 2b75 7064 6174 6564 2533 4132  reau+updated%3A2
-00004df0: 3032 322d 3038 2d32 352e 2e32 3032 332d  022-08-25..2023-
-00004e00: 3031 2d32 3626 7479 7065 3d49 7373 7565  01-26&type=Issue
-00004e10: 7329 207c 205b 4063 636f 7264 6f62 6131  s) | [@ccordoba1
-00004e20: 325d 2868 7474 7073 3a2f 2f67 6974 6875  2](https://githu
-00004e30: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
-00004e40: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
-00004e50: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
-00004e60: 6e76 6f6c 7665 7325 3341 6363 6f72 646f  nvolves%3Accordo
-00004e70: 6261 3132 2b75 7064 6174 6564 2533 4132  ba12+updated%3A2
-00004e80: 3032 322d 3038 2d32 352e 2e32 3032 332d  022-08-25..2023-
-00004e90: 3031 2d32 3626 7479 7065 3d49 7373 7565  01-26&type=Issue
-00004ea0: 7329 207c 205b 4064 6176 6964 6272 6f63  s) | [@davidbroc
-00004eb0: 6861 7274 5d28 6874 7470 733a 2f2f 6769  hart](https://gi
-00004ec0: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
-00004ed0: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
-00004ee0: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
-00004ef0: 742b 696e 766f 6c76 6573 2533 4164 6176  t+involves%3Adav
-00004f00: 6964 6272 6f63 6861 7274 2b75 7064 6174  idbrochart+updat
-00004f10: 6564 2533 4132 3032 322d 3038 2d32 352e  ed%3A2022-08-25.
-00004f20: 2e32 3032 332d 3031 2d32 3626 7479 7065  .2023-01-26&type
-00004f30: 3d49 7373 7565 7329 207c 205b 4064 6570  =Issues) | [@dep
-00004f40: 656e 6461 626f 745d 2868 7474 7073 3a2f  endabot](https:/
-00004f50: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-00004f60: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-00004f70: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-00004f80: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-00004f90: 6465 7065 6e64 6162 6f74 2b75 7064 6174  dependabot+updat
-00004fa0: 6564 2533 4132 3032 322d 3038 2d32 352e  ed%3A2022-08-25.
-00004fb0: 2e32 3032 332d 3031 2d32 3626 7479 7065  .2023-01-26&type
-00004fc0: 3d49 7373 7565 7329 207c 205b 406b 6576  =Issues) | [@kev
-00004fd0: 696e 2d62 6174 6573 5d28 6874 7470 733a  in-bates](https:
-00004fe0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
-00004ff0: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
-00005000: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
-00005010: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
-00005020: 416b 6576 696e 2d62 6174 6573 2b75 7064  Akevin-bates+upd
-00005030: 6174 6564 2533 4132 3032 322d 3038 2d32  ated%3A2022-08-2
-00005040: 352e 2e32 3032 332d 3031 2d32 3626 7479  5..2023-01-26&ty
-00005050: 7065 3d49 7373 7565 7329 207c 205b 406d  pe=Issues) | [@m
-00005060: 6565 7365 656b 7364 6576 5d28 6874 7470  eeseeksdev](http
-00005070: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00005080: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
-00005090: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
-000050a0: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
-000050b0: 2533 416d 6565 7365 656b 7364 6576 2b75  %3Ameeseeksdev+u
-000050c0: 7064 6174 6564 2533 4132 3032 322d 3038  pdated%3A2022-08
-000050d0: 2d32 352e 2e32 3032 332d 3031 2d32 3626  -25..2023-01-26&
-000050e0: 7479 7065 3d49 7373 7565 7329 207c 205b  type=Issues) | [
-000050f0: 406d 696e 726b 5d28 6874 7470 733a 2f2f  @minrk](https://
-00005100: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
-00005110: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
-00005120: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
-00005130: 656e 742b 696e 766f 6c76 6573 2533 416d  ent+involves%3Am
-00005140: 696e 726b 2b75 7064 6174 6564 2533 4132  inrk+updated%3A2
-00005150: 3032 322d 3038 2d32 352e 2e32 3032 332d  022-08-25..2023-
-00005160: 3031 2d32 3626 7479 7065 3d49 7373 7565  01-26&type=Issue
-00005170: 7329 207c 205b 406f 7068 6965 3230 305d  s) | [@ophie200]
-00005180: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00005190: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
-000051a0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
-000051b0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
-000051c0: 6f6c 7665 7325 3341 6f70 6869 6532 3030  olves%3Aophie200
-000051d0: 2b75 7064 6174 6564 2533 4132 3032 322d  +updated%3A2022-
-000051e0: 3038 2d32 352e 2e32 3032 332d 3031 2d32  08-25..2023-01-2
-000051f0: 3626 7479 7065 3d49 7373 7565 7329 207c  6&type=Issues) |
-00005200: 205b 4070 7265 2d63 6f6d 6d69 742d 6369   [@pre-commit-ci
-00005210: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00005220: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
-00005230: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
-00005240: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
-00005250: 766f 6c76 6573 2533 4170 7265 2d63 6f6d  volves%3Apre-com
-00005260: 6d69 742d 6369 2b75 7064 6174 6564 2533  mit-ci+updated%3
-00005270: 4132 3032 322d 3038 2d32 352e 2e32 3032  A2022-08-25..202
-00005280: 332d 3031 2d32 3626 7479 7065 3d49 7373  3-01-26&type=Iss
-00005290: 7565 7329 207c 205b 4073 616d 7261 745d  ues) | [@samrat]
-000052a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000052b0: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
-000052c0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
-000052d0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
-000052e0: 6f6c 7665 7325 3341 7361 6d72 6174 2b75  olves%3Asamrat+u
-000052f0: 7064 6174 6564 2533 4132 3032 322d 3038  pdated%3A2022-08
-00005300: 2d32 352e 2e32 3032 332d 3031 2d32 3626  -25..2023-01-26&
-00005310: 7479 7065 3d49 7373 7565 7329 207c 205b  type=Issues) | [
-00005320: 4053 796c 7661 696e 436f 726c 6179 5d28  @SylvainCorlay](
-00005330: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00005340: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
-00005350: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
-00005360: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
-00005370: 6c76 6573 2533 4153 796c 7661 696e 436f  lves%3ASylvainCo
-00005380: 726c 6179 2b75 7064 6174 6564 2533 4132  rlay+updated%3A2
-00005390: 3032 322d 3038 2d32 352e 2e32 3032 332d  022-08-25..2023-
-000053a0: 3031 2d32 3626 7479 7065 3d49 7373 7565  01-26&type=Issue
-000053b0: 7329 207c 205b 405a 7361 696c 6572 5d28  s) | [@Zsailer](
-000053c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000053d0: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
-000053e0: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
-000053f0: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
-00005400: 6c76 6573 2533 415a 7361 696c 6572 2b75  lves%3AZsailer+u
-00005410: 7064 6174 6564 2533 4132 3032 322d 3038  pdated%3A2022-08
-00005420: 2d32 352e 2e32 3032 332d 3031 2d32 3626  -25..2023-01-26&
-00005430: 7479 7065 3d49 7373 7565 7329 0a0a 2323  type=Issues)..##
-00005440: 2038 2e30 2e30 7263 300a 0a28 5b46 756c   8.0.0rc0..([Ful
-00005450: 6c20 4368 616e 6765 6c6f 675d 2868 7474  l Changelog](htt
-00005460: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00005470: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00005480: 636c 6965 6e74 2f63 6f6d 7061 7265 2f76  client/compare/v
-00005490: 382e 302e 3062 332e 2e2e 6266 3633 3765  8.0.0b3...bf637e
-000054a0: 6439 3534 3331 3938 6436 6463 6139 3664  d9543198d6dca96d
-000054b0: 3734 3862 3033 3037 6564 3031 6231 3663  748b0307ed01b16c
-000054c0: 3934 2929 0a0a 2323 2320 4d61 696e 7465  94))..### Mainte
-000054d0: 6e61 6e63 6520 616e 6420 7570 6b65 6570  nance and upkeep
-000054e0: 2069 6d70 726f 7665 6d65 6e74 730a 0a2d   improvements..-
-000054f0: 2041 6c6c 6f77 2072 656c 6561 7369 6e67   Allow releasing
-00005500: 2066 726f 6d20 7265 706f 205b 2338 3939   from repo [#899
-00005510: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00005520: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00005530: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00005540: 2f38 3939 2920 285b 4062 6c69 6e6b 3130  /899) ([@blink10
-00005550: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
-00005560: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
-00005570: 2929 0a0a 2323 2320 436f 6e74 7269 6275  ))..### Contribu
-00005580: 746f 7273 2074 6f20 7468 6973 2072 656c  tors to this rel
-00005590: 6561 7365 0a0a 285b 4769 7448 7562 2063  ease..([GitHub c
-000055a0: 6f6e 7472 6962 7574 6f72 7320 7061 6765  ontributors page
-000055b0: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
-000055c0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-000055d0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-000055e0: 7079 7465 725f 636c 6965 6e74 2f67 7261  pyter_client/gra
-000055f0: 7068 732f 636f 6e74 7269 6275 746f 7273  phs/contributors
-00005600: 3f66 726f 6d3d 3230 3232 2d31 322d 3133  ?from=2022-12-13
-00005610: 2674 6f3d 3230 3232 2d31 322d 3139 2674  &to=2022-12-19&t
-00005620: 7970 653d 6329 290a 0a5b 4062 6c69 6e6b  ype=c))..[@blink
-00005630: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
-00005640: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
-00005650: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
-00005660: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
-00005670: 742b 696e 766f 6c76 6573 2533 4162 6c69  t+involves%3Abli
-00005680: 6e6b 3130 3733 2b75 7064 6174 6564 2533  nk1073+updated%3
-00005690: 4132 3032 322d 3132 2d31 332e 2e32 3032  A2022-12-13..202
-000056a0: 322d 3132 2d31 3926 7479 7065 3d49 7373  2-12-19&type=Iss
-000056b0: 7565 7329 0a0a 2323 2038 2e30 2e30 6233  ues)..## 8.0.0b3
-000056c0: 0a0a 285b 4675 6c6c 2043 6861 6e67 656c  ..([Full Changel
-000056d0: 6f67 5d28 6874 7470 733a 2f2f 6769 7468  og](https://gith
-000056e0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-000056f0: 7570 7974 6572 5f63 6c69 656e 742f 636f  upyter_client/co
-00005700: 6d70 6172 652f 7638 2e30 2e30 6232 2e2e  mpare/v8.0.0b2..
-00005710: 2e62 3531 6133 6235 6431 6130 6431 6138  .b51a3b5d1a0d1a8
-00005720: 6164 3339 3063 3131 3231 3530 3632 3137  ad390c1121506217
-00005730: 3930 3964 6131 6334 6629 290a 0a23 2323  909da1c4f))..###
-00005740: 2042 7567 7320 6669 7865 640a 0a2d 2041   Bugs fixed..- A
-00005750: 6c6c 6f77 2069 6e74 6572 7275 7074 2064  llow interrupt d
-00005760: 7572 696e 6720 7265 7374 6172 7420 6f66  uring restart of
-00005770: 2070 656e 6469 6e67 206b 6572 6e65 6c73   pending kernels
-00005780: 205b 2338 3938 5d28 6874 7470 733a 2f2f   [#898](https://
-00005790: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-000057a0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-000057b0: 742f 7075 6c6c 2f38 3938 2920 285b 4062  t/pull/898) ([@b
-000057c0: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
-000057d0: 2f2f 6769 7468 7562 2e63 6f6d 2f62 6c69  //github.com/bli
-000057e0: 6e6b 3130 3733 2929 0a0a 2323 2320 436f  nk1073))..### Co
-000057f0: 6e74 7269 6275 746f 7273 2074 6f20 7468  ntributors to th
-00005800: 6973 2072 656c 6561 7365 0a0a 285b 4769  is release..([Gi
-00005810: 7448 7562 2063 6f6e 7472 6962 7574 6f72  tHub contributor
-00005820: 7320 7061 6765 2066 6f72 2074 6869 7320  s page for this 
-00005830: 7265 6c65 6173 655d 2868 7474 7073 3a2f  release](https:/
-00005840: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-00005850: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-00005860: 6e74 2f67 7261 7068 732f 636f 6e74 7269  nt/graphs/contri
-00005870: 6275 746f 7273 3f66 726f 6d3d 3230 3232  butors?from=2022
-00005880: 2d31 322d 3038 2674 6f3d 3230 3232 2d31  -12-08&to=2022-1
-00005890: 322d 3133 2674 7970 653d 6329 290a 0a5b  2-13&type=c))..[
-000058a0: 4062 6c69 6e6b 3130 3733 5d28 6874 7470  @blink1073](http
-000058b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-000058c0: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
-000058d0: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
-000058e0: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
-000058f0: 2533 4162 6c69 6e6b 3130 3733 2b75 7064  %3Ablink1073+upd
-00005900: 6174 6564 2533 4132 3032 322d 3132 2d30  ated%3A2022-12-0
-00005910: 382e 2e32 3032 322d 3132 2d31 3326 7479  8..2022-12-13&ty
-00005920: 7065 3d49 7373 7565 7329 0a0a 2323 2038  pe=Issues)..## 8
-00005930: 2e30 2e30 6232 0a0a 285b 4675 6c6c 2043  .0.0b2..([Full C
-00005940: 6861 6e67 656c 6f67 5d28 6874 7470 733a  hangelog](https:
-00005950: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-00005960: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-00005970: 656e 742f 636f 6d70 6172 652f 7638 2e30  ent/compare/v8.0
-00005980: 2e30 6231 2e2e 2e66 6633 3361 6466 3738  .0b1...ff33adf78
-00005990: 3466 3262 6432 3538 3134 6437 6564 3661  4f2bd25814d7ed6a
-000059a0: 6537 6336 3635 3163 6565 3833 3736 6529  e7c6651cee8376e)
-000059b0: 290a 0a23 2323 204d 6169 6e74 656e 616e  )..### Maintenan
-000059c0: 6365 2061 6e64 2075 706b 6565 7020 696d  ce and upkeep im
-000059d0: 7072 6f76 656d 656e 7473 0a0a 2d20 4669  provements..- Fi
-000059e0: 7820 6a75 7079 7465 725f 636f 7265 2070  x jupyter_core p
-000059f0: 696e 6e69 6e67 205b 2338 3936 5d28 6874  inning [#896](ht
-00005a00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00005a10: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00005a20: 5f63 6c69 656e 742f 7075 6c6c 2f38 3936  _client/pull/896
-00005a30: 2920 285b 406f 7068 6965 3230 305d 2868  ) ([@ophie200](h
-00005a40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00005a50: 6d2f 6f70 6869 6532 3030 2929 0a2d 2041  m/ophie200)).- A
-00005a60: 646f 7074 2072 7566 6620 616e 6420 7265  dopt ruff and re
-00005a70: 6475 6365 2070 7265 2d63 6f6d 6d69 7420  duce pre-commit 
-00005a80: 7573 6167 6520 5b23 3839 355d 2868 7474  usage [#895](htt
-00005a90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00005aa0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00005ab0: 636c 6965 6e74 2f70 756c 6c2f 3839 3529  client/pull/895)
-00005ac0: 2028 5b40 626c 696e 6b31 3037 335d 2868   ([@blink1073](h
-00005ad0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00005ae0: 6d2f 626c 696e 6b31 3037 3329 290a 0a23  m/blink1073))..#
-00005af0: 2323 2043 6f6e 7472 6962 7574 6f72 7320  ## Contributors 
-00005b00: 746f 2074 6869 7320 7265 6c65 6173 650a  to this release.
-00005b10: 0a28 5b47 6974 4875 6220 636f 6e74 7269  .([GitHub contri
-00005b20: 6275 746f 7273 2070 6167 6520 666f 7220  butors page for 
-00005b30: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
-00005b40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00005b50: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00005b60: 5f63 6c69 656e 742f 6772 6170 6873 2f63  _client/graphs/c
-00005b70: 6f6e 7472 6962 7574 6f72 733f 6672 6f6d  ontributors?from
-00005b80: 3d32 3032 322d 3132 2d30 3526 746f 3d32  =2022-12-05&to=2
-00005b90: 3032 322d 3132 2d30 3826 7479 7065 3d63  022-12-08&type=c
-00005ba0: 2929 0a0a 5b40 626c 696e 6b31 3037 335d  ))..[@blink1073]
-00005bb0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00005bc0: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
-00005bd0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
-00005be0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
-00005bf0: 6f6c 7665 7325 3341 626c 696e 6b31 3037  olves%3Ablink107
-00005c00: 332b 7570 6461 7465 6425 3341 3230 3232  3+updated%3A2022
-00005c10: 2d31 322d 3035 2e2e 3230 3232 2d31 322d  -12-05..2022-12-
-00005c20: 3038 2674 7970 653d 4973 7375 6573 2920  08&type=Issues) 
-00005c30: 7c20 5b40 6461 7669 6462 726f 6368 6172  | [@davidbrochar
-00005c40: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
-00005c50: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
-00005c60: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
-00005c70: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
-00005c80: 6e76 6f6c 7665 7325 3341 6461 7669 6462  nvolves%3Adavidb
-00005c90: 726f 6368 6172 742b 7570 6461 7465 6425  rochart+updated%
-00005ca0: 3341 3230 3232 2d31 322d 3035 2e2e 3230  3A2022-12-05..20
-00005cb0: 3232 2d31 322d 3038 2674 7970 653d 4973  22-12-08&type=Is
-00005cc0: 7375 6573 2920 7c20 5b40 6f70 6869 6532  sues) | [@ophie2
-00005cd0: 3030 5d28 6874 7470 733a 2f2f 6769 7468  00](https://gith
-00005ce0: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
-00005cf0: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
-00005d00: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
-00005d10: 696e 766f 6c76 6573 2533 416f 7068 6965  involves%3Aophie
-00005d20: 3230 302b 7570 6461 7465 6425 3341 3230  200+updated%3A20
-00005d30: 3232 2d31 322d 3035 2e2e 3230 3232 2d31  22-12-05..2022-1
-00005d40: 322d 3038 2674 7970 653d 4973 7375 6573  2-08&type=Issues
-00005d50: 2920 7c20 5b40 7072 652d 636f 6d6d 6974  ) | [@pre-commit
-00005d60: 2d63 695d 2868 7474 7073 3a2f 2f67 6974  -ci](https://git
-00005d70: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
-00005d80: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
-00005d90: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
-00005da0: 2b69 6e76 6f6c 7665 7325 3341 7072 652d  +involves%3Apre-
-00005db0: 636f 6d6d 6974 2d63 692b 7570 6461 7465  commit-ci+update
-00005dc0: 6425 3341 3230 3232 2d31 322d 3035 2e2e  d%3A2022-12-05..
-00005dd0: 3230 3232 2d31 322d 3038 2674 7970 653d  2022-12-08&type=
-00005de0: 4973 7375 6573 290a 0a23 2320 382e 302e  Issues)..## 8.0.
-00005df0: 3062 310a 0a4e 6f20 6d65 7267 6564 2050  0b1..No merged P
-00005e00: 5273 0a0a 2323 2038 2e30 2e30 6230 0a0a  Rs..## 8.0.0b0..
-00005e10: 285b 4675 6c6c 2043 6861 6e67 656c 6f67  ([Full Changelog
-00005e20: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00005e30: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00005e40: 7974 6572 5f63 6c69 656e 742f 636f 6d70  yter_client/comp
-00005e50: 6172 652f 7638 2e30 2e30 6134 2e2e 2e65  are/v8.0.0a4...e
-00005e60: 3431 3966 6634 6136 3531 6236 6163 3763  419ff4a651b6ac7c
-00005e70: 6435 3333 3032 3363 3264 6433 6264 3339  d533023c2dd3bd39
-00005e80: 3164 6536 6562 3629 290a 0a23 2323 204d  1de6eb6))..### M
-00005e90: 6169 6e74 656e 616e 6365 2061 6e64 2075  aintenance and u
-00005ea0: 706b 6565 7020 696d 7072 6f76 656d 656e  pkeep improvemen
-00005eb0: 7473 0a0a 2d20 5573 6520 7079 7465 7374  ts..- Use pytest
-00005ec0: 2d6a 7570 7974 6572 205b 2338 3931 5d28  -jupyter [#891](
-00005ed0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00005ee0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-00005ef0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f38  er_client/pull/8
-00005f00: 3931 2920 285b 4062 6c69 6e6b 3130 3733  91) ([@blink1073
-00005f10: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00005f20: 2e63 6f6d 2f62 6c69 6e6b 3130 3733 2929  .com/blink1073))
-00005f30: 0a2d 2049 6d70 6f72 7420 656e 7375 7265  .- Import ensure
-00005f40: 5f61 7379 6e63 2061 6e64 2072 756e 5f73  _async and run_s
-00005f50: 796e 6320 6672 6f6d 206a 7570 7974 6572  ync from jupyter
-00005f60: 5f63 6f72 6520 5b23 3838 395d 2868 7474  _core [#889](htt
-00005f70: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00005f80: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00005f90: 636c 6965 6e74 2f70 756c 6c2f 3838 3929  client/pull/889)
-00005fa0: 2028 5b40 6461 7669 6462 726f 6368 6172   ([@davidbrochar
-00005fb0: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
-00005fc0: 622e 636f 6d2f 6461 7669 6462 726f 6368  b.com/davidbroch
-00005fd0: 6172 7429 290a 2d20 5573 6520 6261 7365  art)).- Use base
-00005fe0: 2073 6574 7570 2064 6570 656e 6465 6e63   setup dependenc
-00005ff0: 7920 7479 7065 205b 2338 3838 5d28 6874  y type [#888](ht
-00006000: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00006010: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00006020: 5f63 6c69 656e 742f 7075 6c6c 2f38 3838  _client/pull/888
-00006030: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
-00006040: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00006050: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a2d  om/blink1073)).-
-00006060: 204d 6f72 6520 4349 2043 6c65 616e 7570   More CI Cleanup
-00006070: 205b 2338 3836 5d28 6874 7470 733a 2f2f   [#886](https://
-00006080: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00006090: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-000060a0: 742f 7075 6c6c 2f38 3836 2920 285b 4062  t/pull/886) ([@b
-000060b0: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
-000060c0: 2f2f 6769 7468 7562 2e63 6f6d 2f62 6c69  //github.com/bli
-000060d0: 6e6b 3130 3733 2929 0a2d 204d 6f72 6520  nk1073)).- More 
-000060e0: 636f 7665 7261 6765 205b 2338 3835 5d28  coverage [#885](
-000060f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00006100: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-00006110: 6572 5f63 6c69 656e 742f 7075 6c6c 2f38  er_client/pull/8
-00006120: 3835 2920 285b 4062 6c69 6e6b 3130 3733  85) ([@blink1073
-00006130: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00006140: 2e63 6f6d 2f62 6c69 6e6b 3130 3733 2929  .com/blink1073))
-00006150: 0a2d 2043 6c65 616e 2075 7020 776f 726b  .- Clean up work
-00006160: 666c 6f77 2061 6e64 2070 7970 726f 6a65  flow and pyproje
-00006170: 6374 205b 2338 3834 5d28 6874 7470 733a  ct [#884](https:
-00006180: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-00006190: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-000061a0: 656e 742f 7075 6c6c 2f38 3834 2920 285b  ent/pull/884) ([
-000061b0: 4062 6c69 6e6b 3130 3733 5d28 6874 7470  @blink1073](http
-000061c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-000061d0: 6c69 6e6b 3130 3733 2929 0a0a 2323 2320  link1073))..### 
-000061e0: 436f 6e74 7269 6275 746f 7273 2074 6f20  Contributors to 
-000061f0: 7468 6973 2072 656c 6561 7365 0a0a 285b  this release..([
-00006200: 4769 7448 7562 2063 6f6e 7472 6962 7574  GitHub contribut
-00006210: 6f72 7320 7061 6765 2066 6f72 2074 6869  ors page for thi
-00006220: 7320 7265 6c65 6173 655d 2868 7474 7073  s release](https
-00006230: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00006240: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-00006250: 6965 6e74 2f67 7261 7068 732f 636f 6e74  ient/graphs/cont
-00006260: 7269 6275 746f 7273 3f66 726f 6d3d 3230  ributors?from=20
-00006270: 3232 2d31 312d 3136 2674 6f3d 3230 3232  22-11-16&to=2022
-00006280: 2d31 312d 3239 2674 7970 653d 6329 290a  -11-29&type=c)).
-00006290: 0a5b 4061 726f 676f 7a68 6e69 6b6f 765d  .[@arogozhnikov]
-000062a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000062b0: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
-000062c0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
-000062d0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
-000062e0: 6f6c 7665 7325 3341 6172 6f67 6f7a 686e  olves%3Aarogozhn
-000062f0: 696b 6f76 2b75 7064 6174 6564 2533 4132  ikov+updated%3A2
-00006300: 3032 322d 3131 2d31 362e 2e32 3032 322d  022-11-16..2022-
-00006310: 3131 2d32 3926 7479 7065 3d49 7373 7565  11-29&type=Issue
-00006320: 7329 207c 205b 4062 6c69 6e6b 3130 3733  s) | [@blink1073
-00006330: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00006340: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
-00006350: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
-00006360: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
-00006370: 766f 6c76 6573 2533 4162 6c69 6e6b 3130  volves%3Ablink10
-00006380: 3733 2b75 7064 6174 6564 2533 4132 3032  73+updated%3A202
-00006390: 322d 3131 2d31 362e 2e32 3032 322d 3131  2-11-16..2022-11
-000063a0: 2d32 3926 7479 7065 3d49 7373 7565 7329  -29&type=Issues)
-000063b0: 207c 205b 4064 6176 6964 6272 6f63 6861   | [@davidbrocha
-000063c0: 7274 5d28 6874 7470 733a 2f2f 6769 7468  rt](https://gith
-000063d0: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
-000063e0: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
-000063f0: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
-00006400: 696e 766f 6c76 6573 2533 4164 6176 6964  involves%3Adavid
-00006410: 6272 6f63 6861 7274 2b75 7064 6174 6564  brochart+updated
-00006420: 2533 4132 3032 322d 3131 2d31 362e 2e32  %3A2022-11-16..2
-00006430: 3032 322d 3131 2d32 3926 7479 7065 3d49  022-11-29&type=I
-00006440: 7373 7565 7329 207c 205b 406b 6576 696e  ssues) | [@kevin
-00006450: 2d62 6174 6573 5d28 6874 7470 733a 2f2f  -bates](https://
-00006460: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
-00006470: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
-00006480: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
-00006490: 656e 742b 696e 766f 6c76 6573 2533 416b  ent+involves%3Ak
-000064a0: 6576 696e 2d62 6174 6573 2b75 7064 6174  evin-bates+updat
-000064b0: 6564 2533 4132 3032 322d 3131 2d31 362e  ed%3A2022-11-16.
-000064c0: 2e32 3032 322d 3131 2d32 3926 7479 7065  .2022-11-29&type
-000064d0: 3d49 7373 7565 7329 207c 205b 4070 7265  =Issues) | [@pre
-000064e0: 2d63 6f6d 6d69 742d 6369 5d28 6874 7470  -commit-ci](http
-000064f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00006500: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
-00006510: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
-00006520: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
-00006530: 2533 4170 7265 2d63 6f6d 6d69 742d 6369  %3Apre-commit-ci
-00006540: 2b75 7064 6174 6564 2533 4132 3032 322d  +updated%3A2022-
-00006550: 3131 2d31 362e 2e32 3032 322d 3131 2d32  11-16..2022-11-2
-00006560: 3926 7479 7065 3d49 7373 7565 7329 0a0a  9&type=Issues)..
-00006570: 2323 2038 2e30 2e30 6134 0a0a 285b 4675  ## 8.0.0a4..([Fu
-00006580: 6c6c 2043 6861 6e67 656c 6f67 5d28 6874  ll Changelog](ht
-00006590: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000065a0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-000065b0: 5f63 6c69 656e 742f 636f 6d70 6172 652f  _client/compare/
-000065c0: 7638 2e30 2e30 6133 2e2e 2e31 3037 6363  v8.0.0a3...107cc
-000065d0: 6464 3036 6339 6236 3766 6330 3831 3230  dd06c9b67fc08120
-000065e0: 3461 6537 6330 6537 3132 3361 3137 6362  4ae7c0e7123a17cb
-000065f0: 3063 3429 290a 0a23 2323 2042 7567 7320  0c4))..### Bugs 
-00006600: 6669 7865 640a 0a2d 2046 6978 2063 6f6e  fixed..- Fix con
-00006610: 6e65 6374 696f 6e20 7265 636f 6e63 696c  nection reconcil
-00006620: 6961 7469 6f6e 2074 6f20 6861 6e64 6c65  iation to handle
-00006630: 2072 6573 7461 7274 7320 5b23 3838 325d   restarts [#882]
-00006640: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00006650: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-00006660: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-00006670: 3838 3229 2028 5b40 6b65 7669 6e2d 6261  882) ([@kevin-ba
-00006680: 7465 735d 2868 7474 7073 3a2f 2f67 6974  tes](https://git
-00006690: 6875 622e 636f 6d2f 6b65 7669 6e2d 6261  hub.com/kevin-ba
-000066a0: 7465 7329 290a 0a23 2323 204d 6169 6e74  tes))..### Maint
-000066b0: 656e 616e 6365 2061 6e64 2075 706b 6565  enance and upkee
-000066c0: 7020 696d 7072 6f76 656d 656e 7473 0a0a  p improvements..
-000066d0: 2d20 4164 6420 6d6f 7265 2063 6f76 6572  - Add more cover
-000066e0: 6167 6520 5b23 3837 375d 2868 7474 7073  age [#877](https
-000066f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00006700: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-00006710: 6965 6e74 2f70 756c 6c2f 3837 3729 2028  ient/pull/877) (
-00006720: 5b40 626c 696e 6b31 3037 335d 2868 7474  [@blink1073](htt
-00006730: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00006740: 626c 696e 6b31 3037 3329 290a 0a23 2323  blink1073))..###
-00006750: 2043 6f6e 7472 6962 7574 6f72 7320 746f   Contributors to
-00006760: 2074 6869 7320 7265 6c65 6173 650a 0a28   this release..(
-00006770: 5b47 6974 4875 6220 636f 6e74 7269 6275  [GitHub contribu
-00006780: 746f 7273 2070 6167 6520 666f 7220 7468  tors page for th
-00006790: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
-000067a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000067b0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-000067c0: 6c69 656e 742f 6772 6170 6873 2f63 6f6e  lient/graphs/con
-000067d0: 7472 6962 7574 6f72 733f 6672 6f6d 3d32  tributors?from=2
-000067e0: 3032 322d 3131 2d31 3526 746f 3d32 3032  022-11-15&to=202
-000067f0: 322d 3131 2d31 3626 7479 7065 3d63 2929  2-11-16&type=c))
-00006800: 0a0a 5b40 626c 696e 6b31 3037 335d 2868  ..[@blink1073](h
-00006810: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00006820: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
-00006830: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
-00006840: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
-00006850: 7665 7325 3341 626c 696e 6b31 3037 332b  ves%3Ablink1073+
-00006860: 7570 6461 7465 6425 3341 3230 3232 2d31  updated%3A2022-1
-00006870: 312d 3135 2e2e 3230 3232 2d31 312d 3136  1-15..2022-11-16
-00006880: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
-00006890: 5b40 6b65 7669 6e2d 6261 7465 735d 2868  [@kevin-bates](h
-000068a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000068b0: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
-000068c0: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
-000068d0: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
-000068e0: 7665 7325 3341 6b65 7669 6e2d 6261 7465  ves%3Akevin-bate
-000068f0: 732b 7570 6461 7465 6425 3341 3230 3232  s+updated%3A2022
-00006900: 2d31 312d 3135 2e2e 3230 3232 2d31 312d  -11-15..2022-11-
-00006910: 3136 2674 7970 653d 4973 7375 6573 290a  16&type=Issues).
-00006920: 0a23 2320 382e 302e 3061 330a 0a28 5b46  .## 8.0.0a3..([F
-00006930: 756c 6c20 4368 616e 6765 6c6f 675d 2868  ull Changelog](h
-00006940: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00006950: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00006960: 725f 636c 6965 6e74 2f63 6f6d 7061 7265  r_client/compare
-00006970: 2f76 382e 302e 3061 322e 2e2e 3130 6636  /v8.0.0a2...10f6
-00006980: 3963 3962 3561 6335 3562 3932 6236 3531  9c9b5ac55b92b651
-00006990: 6631 6635 3566 6132 3831 3466 3831 6633  f1f55fa2814f81f3
-000069a0: 6365 3531 2929 0a0a 2323 2320 4275 6773  ce51))..### Bugs
-000069b0: 2066 6978 6564 0a0a 2d20 5265 636f 6e63   fixed..- Reconc
-000069c0: 696c 6520 636f 6e6e 6563 7469 6f6e 2069  ile connection i
-000069d0: 6e66 6f72 6d61 7469 6f6e 205b 2338 3739  nformation [#879
-000069e0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000069f0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00006a00: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00006a10: 2f38 3739 2920 285b 406b 6576 696e 2d62  /879) ([@kevin-b
-00006a20: 6174 6573 5d28 6874 7470 733a 2f2f 6769  ates](https://gi
-00006a30: 7468 7562 2e63 6f6d 2f6b 6576 696e 2d62  thub.com/kevin-b
-00006a40: 6174 6573 2929 0a0a 2323 2320 4d61 696e  ates))..### Main
-00006a50: 7465 6e61 6e63 6520 616e 6420 7570 6b65  tenance and upke
-00006a60: 6570 2069 6d70 726f 7665 6d65 6e74 730a  ep improvements.
-00006a70: 0a2d 2041 6464 2063 6f76 6572 6167 6520  .- Add coverage 
-00006a80: 636f 6e66 6967 205b 2338 3736 5d28 6874  config [#876](ht
-00006a90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00006aa0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00006ab0: 5f63 6c69 656e 742f 7075 6c6c 2f38 3736  _client/pull/876
-00006ac0: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
-00006ad0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00006ae0: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a2d  om/blink1073)).-
-00006af0: 2042 756d 7020 6163 7469 6f6e 732f 7365   Bump actions/se
-00006b00: 7475 702d 7079 7468 6f6e 2066 726f 6d20  tup-python from 
-00006b10: 3220 746f 2034 205b 2338 3734 5d28 6874  2 to 4 [#874](ht
-00006b20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00006b30: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00006b40: 5f63 6c69 656e 742f 7075 6c6c 2f38 3734  _client/pull/874
-00006b50: 2920 285b 4064 6570 656e 6461 626f 745d  ) ([@dependabot]
-00006b60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00006b70: 636f 6d2f 6465 7065 6e64 6162 6f74 2929  com/dependabot))
-00006b80: 0a2d 2042 756d 7020 6163 7469 6f6e 732f  .- Bump actions/
-00006b90: 6368 6563 6b6f 7574 2066 726f 6d20 3220  checkout from 2 
-00006ba0: 746f 2033 205b 2338 3733 5d28 6874 7470  to 3 [#873](http
-00006bb0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00006bc0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00006bd0: 6c69 656e 742f 7075 6c6c 2f38 3733 2920  lient/pull/873) 
-00006be0: 285b 4064 6570 656e 6461 626f 745d 2868  ([@dependabot](h
-00006bf0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00006c00: 6d2f 6465 7065 6e64 6162 6f74 2929 0a2d  m/dependabot)).-
-00006c10: 2043 6c65 616e 2075 7020 7479 7065 7320   Clean up types 
-00006c20: 616e 6420 7265 6d6f 7665 2075 7365 206f  and remove use o
-00006c30: 6620 656e 7472 7970 6f69 6e74 7320 5b23  f entrypoints [#
-00006c40: 3837 315d 2868 7474 7073 3a2f 2f67 6974  871](https://git
-00006c50: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-00006c60: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-00006c70: 756c 6c2f 3837 3129 2028 5b40 626c 696e  ull/871) ([@blin
-00006c80: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
-00006c90: 6974 6875 622e 636f 6d2f 626c 696e 6b31  ithub.com/blink1
-00006ca0: 3037 3329 290a 2d20 4164 6420 6465 7065  073)).- Add depe
-00006cb0: 6e64 6162 6f74 205b 2338 3730 5d28 6874  ndabot [#870](ht
-00006cc0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00006cd0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00006ce0: 5f63 6c69 656e 742f 7075 6c6c 2f38 3730  _client/pull/870
-00006cf0: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
-00006d00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00006d10: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a0a  om/blink1073))..
-00006d20: 2323 2320 436f 6e74 7269 6275 746f 7273  ### Contributors
-00006d30: 2074 6f20 7468 6973 2072 656c 6561 7365   to this release
-00006d40: 0a0a 285b 4769 7448 7562 2063 6f6e 7472  ..([GitHub contr
-00006d50: 6962 7574 6f72 7320 7061 6765 2066 6f72  ibutors page for
-00006d60: 2074 6869 7320 7265 6c65 6173 655d 2868   this release](h
-00006d70: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00006d80: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00006d90: 725f 636c 6965 6e74 2f67 7261 7068 732f  r_client/graphs/
-00006da0: 636f 6e74 7269 6275 746f 7273 3f66 726f  contributors?fro
-00006db0: 6d3d 3230 3232 2d31 312d 3039 2674 6f3d  m=2022-11-09&to=
-00006dc0: 3230 3232 2d31 312d 3135 2674 7970 653d  2022-11-15&type=
-00006dd0: 6329 290a 0a5b 4062 6c69 6e6b 3130 3733  c))..[@blink1073
-00006de0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00006df0: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
-00006e00: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
-00006e10: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
-00006e20: 766f 6c76 6573 2533 4162 6c69 6e6b 3130  volves%3Ablink10
-00006e30: 3733 2b75 7064 6174 6564 2533 4132 3032  73+updated%3A202
-00006e40: 322d 3131 2d30 392e 2e32 3032 322d 3131  2-11-09..2022-11
-00006e50: 2d31 3526 7479 7065 3d49 7373 7565 7329  -15&type=Issues)
-00006e60: 207c 205b 4064 6570 656e 6461 626f 745d   | [@dependabot]
-00006e70: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00006e80: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
-00006e90: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
-00006ea0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
-00006eb0: 6f6c 7665 7325 3341 6465 7065 6e64 6162  olves%3Adependab
-00006ec0: 6f74 2b75 7064 6174 6564 2533 4132 3032  ot+updated%3A202
-00006ed0: 322d 3131 2d30 392e 2e32 3032 322d 3131  2-11-09..2022-11
-00006ee0: 2d31 3526 7479 7065 3d49 7373 7565 7329  -15&type=Issues)
-00006ef0: 207c 205b 406b 6576 696e 2d62 6174 6573   | [@kevin-bates
-00006f00: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00006f10: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
-00006f20: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
-00006f30: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
-00006f40: 766f 6c76 6573 2533 416b 6576 696e 2d62  volves%3Akevin-b
-00006f50: 6174 6573 2b75 7064 6174 6564 2533 4132  ates+updated%3A2
-00006f60: 3032 322d 3131 2d30 392e 2e32 3032 322d  022-11-09..2022-
-00006f70: 3131 2d31 3526 7479 7065 3d49 7373 7565  11-15&type=Issue
-00006f80: 7329 207c 205b 4070 7265 2d63 6f6d 6d69  s) | [@pre-commi
-00006f90: 742d 6369 5d28 6874 7470 733a 2f2f 6769  t-ci](https://gi
-00006fa0: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
-00006fb0: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
-00006fc0: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
-00006fd0: 742b 696e 766f 6c76 6573 2533 4170 7265  t+involves%3Apre
-00006fe0: 2d63 6f6d 6d69 742d 6369 2b75 7064 6174  -commit-ci+updat
-00006ff0: 6564 2533 4132 3032 322d 3131 2d30 392e  ed%3A2022-11-09.
-00007000: 2e32 3032 322d 3131 2d31 3526 7479 7065  .2022-11-15&type
-00007010: 3d49 7373 7565 7329 0a0a 2323 2038 2e30  =Issues)..## 8.0
-00007020: 2e30 6132 0a0a 285b 4675 6c6c 2043 6861  .0a2..([Full Cha
-00007030: 6e67 656c 6f67 5d28 6874 7470 733a 2f2f  ngelog](https://
-00007040: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00007050: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00007060: 742f 636f 6d70 6172 652f 7638 2e30 2e30  t/compare/v8.0.0
-00007070: 6131 2e2e 2e32 3638 6133 6335 6338 3932  a1...268a3c5c892
-00007080: 6533 6534 3265 3736 6335 6563 3132 3061  e3e42e76c5ec120a
-00007090: 3734 6465 3130 6662 3034 3231 3829 290a  74de10fb04218)).
-000070a0: 0a23 2323 204d 6169 6e74 656e 616e 6365  .### Maintenance
-000070b0: 2061 6e64 2075 706b 6565 7020 696d 7072   and upkeep impr
-000070c0: 6f76 656d 656e 7473 0a0a 2d20 5573 6520  ovements..- Use 
-000070d0: 706c 6174 666f 726d 2064 6972 7320 696e  platform dirs in
-000070e0: 2074 6573 7473 205b 2338 3732 5d28 6874   tests [#872](ht
-000070f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00007100: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00007110: 5f63 6c69 656e 742f 7075 6c6c 2f38 3732  _client/pull/872
-00007120: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
-00007130: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00007140: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a2d  om/blink1073)).-
-00007150: 2053 7570 706f 7274 2050 7974 686f 6e20   Support Python 
-00007160: 332e 382d 332e 3131 205b 2338 3636 5d28  3.8-3.11 [#866](
-00007170: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00007180: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-00007190: 6572 5f63 6c69 656e 742f 7075 6c6c 2f38  er_client/pull/8
-000071a0: 3636 2920 285b 4062 6c69 6e6b 3130 3733  66) ([@blink1073
-000071b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000071c0: 2e63 6f6d 2f62 6c69 6e6b 3130 3733 2929  .com/blink1073))
-000071d0: 0a0a 2323 2320 436f 6e74 7269 6275 746f  ..### Contributo
-000071e0: 7273 2074 6f20 7468 6973 2072 656c 6561  rs to this relea
-000071f0: 7365 0a0a 285b 4769 7448 7562 2063 6f6e  se..([GitHub con
-00007200: 7472 6962 7574 6f72 7320 7061 6765 2066  tributors page f
-00007210: 6f72 2074 6869 7320 7265 6c65 6173 655d  or this release]
-00007220: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00007230: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-00007240: 7465 725f 636c 6965 6e74 2f67 7261 7068  ter_client/graph
-00007250: 732f 636f 6e74 7269 6275 746f 7273 3f66  s/contributors?f
-00007260: 726f 6d3d 3230 3232 2d31 302d 3235 2674  rom=2022-10-25&t
-00007270: 6f3d 3230 3232 2d31 312d 3039 2674 7970  o=2022-11-09&typ
-00007280: 653d 6329 290a 0a5b 4062 6c69 6e6b 3130  e=c))..[@blink10
-00007290: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
-000072a0: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
-000072b0: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
-000072c0: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
-000072d0: 696e 766f 6c76 6573 2533 4162 6c69 6e6b  involves%3Ablink
-000072e0: 3130 3733 2b75 7064 6174 6564 2533 4132  1073+updated%3A2
-000072f0: 3032 322d 3130 2d32 352e 2e32 3032 322d  022-10-25..2022-
-00007300: 3131 2d30 3926 7479 7065 3d49 7373 7565  11-09&type=Issue
-00007310: 7329 207c 205b 4070 7265 2d63 6f6d 6d69  s) | [@pre-commi
-00007320: 742d 6369 5d28 6874 7470 733a 2f2f 6769  t-ci](https://gi
-00007330: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
-00007340: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
-00007350: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
-00007360: 742b 696e 766f 6c76 6573 2533 4170 7265  t+involves%3Apre
-00007370: 2d63 6f6d 6d69 742d 6369 2b75 7064 6174  -commit-ci+updat
-00007380: 6564 2533 4132 3032 322d 3130 2d32 352e  ed%3A2022-10-25.
-00007390: 2e32 3032 322d 3131 2d30 3926 7479 7065  .2022-11-09&type
-000073a0: 3d49 7373 7565 7329 0a0a 2323 2038 2e30  =Issues)..## 8.0
-000073b0: 2e30 6131 0a0a 285b 4675 6c6c 2043 6861  .0a1..([Full Cha
-000073c0: 6e67 656c 6f67 5d28 6874 7470 733a 2f2f  ngelog](https://
-000073d0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-000073e0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-000073f0: 742f 636f 6d70 6172 652f 7638 2e30 2e30  t/compare/v8.0.0
-00007400: 6130 2e2e 2e33 3562 3636 6438 6137 3338  a0...35b66d8a738
-00007410: 6236 6339 3632 3966 6665 6164 3330 3863  b6c9629ffead308c
-00007420: 3966 3938 3162 6565 3131 3438 6629 290a  9f981bee1148f)).
-00007430: 0a23 2323 2042 7567 7320 6669 7865 640a  .### Bugs fixed.
-00007440: 0a2d 2057 6f72 6b61 726f 756e 6420 666f  .- Workaround fo
-00007450: 7220 6c61 756e 6368 2062 7567 205b 2338  r launch bug [#8
-00007460: 3631 5d28 6874 7470 733a 2f2f 6769 7468  61](https://gith
-00007470: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00007480: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-00007490: 6c6c 2f38 3631 2920 285b 4062 6c69 6e6b  ll/861) ([@blink
-000074a0: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
-000074b0: 7468 7562 2e63 6f6d 2f62 6c69 6e6b 3130  thub.com/blink10
-000074c0: 3733 2929 0a2d 2044 6566 6572 2063 7265  73)).- Defer cre
-000074d0: 6174 696f 6e20 6f66 2072 6561 6479 2066  ation of ready f
-000074e0: 7574 7572 6520 5b23 3835 385d 2868 7474  uture [#858](htt
-000074f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00007500: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00007510: 636c 6965 6e74 2f70 756c 6c2f 3835 3829  client/pull/858)
-00007520: 2028 5b40 626c 696e 6b31 3037 335d 2868   ([@blink1073](h
-00007530: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00007540: 6d2f 626c 696e 6b31 3037 3329 290a 0a23  m/blink1073))..#
-00007550: 2323 204d 6169 6e74 656e 616e 6365 2061  ## Maintenance a
-00007560: 6e64 2075 706b 6565 7020 696d 7072 6f76  nd upkeep improv
-00007570: 656d 656e 7473 0a0a 2d20 4669 7820 6173  ements..- Fix as
-00007580: 7365 7274 696f 6e20 696e 2060 5465 7374  sertion in `Test
-00007590: 5365 7373 696f 6e2e 7465 7374 5f73 6572  Session.test_ser
-000075a0: 6961 6c69 7a65 6020 5b23 3836 305d 2868  ialize` [#860](h
-000075b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000075c0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-000075d0: 725f 636c 6965 6e74 2f70 756c 6c2f 3836  r_client/pull/86
-000075e0: 3029 2028 5b40 7361 6d72 6174 5d28 6874  0) ([@samrat](ht
-000075f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00007600: 2f73 616d 7261 7429 290a 2d20 4d61 696e  /samrat)).- Main
-00007610: 7465 6e61 6e63 6520 636c 6561 6e75 7020  tenance cleanup 
-00007620: 5b23 3835 365d 2868 7474 7073 3a2f 2f67  [#856](https://g
-00007630: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
-00007640: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
-00007650: 2f70 756c 6c2f 3835 3629 2028 5b40 626c  /pull/856) ([@bl
-00007660: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
-00007670: 2f67 6974 6875 622e 636f 6d2f 626c 696e  /github.com/blin
-00007680: 6b31 3037 3329 290a 0a23 2323 2043 6f6e  k1073))..### Con
-00007690: 7472 6962 7574 6f72 7320 746f 2074 6869  tributors to thi
-000076a0: 7320 7265 6c65 6173 650a 0a28 5b47 6974  s release..([Git
-000076b0: 4875 6220 636f 6e74 7269 6275 746f 7273  Hub contributors
-000076c0: 2070 6167 6520 666f 7220 7468 6973 2072   page for this r
-000076d0: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
-000076e0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-000076f0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00007700: 742f 6772 6170 6873 2f63 6f6e 7472 6962  t/graphs/contrib
-00007710: 7574 6f72 733f 6672 6f6d 3d32 3032 322d  utors?from=2022-
-00007720: 3130 2d31 3226 746f 3d32 3032 322d 3130  10-12&to=2022-10
-00007730: 2d32 3526 7479 7065 3d63 2929 0a0a 5b40  -25&type=c))..[@
-00007740: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
-00007750: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
-00007760: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
-00007770: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
-00007780: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
-00007790: 3341 626c 696e 6b31 3037 332b 7570 6461  3Ablink1073+upda
-000077a0: 7465 6425 3341 3230 3232 2d31 302d 3132  ted%3A2022-10-12
-000077b0: 2e2e 3230 3232 2d31 302d 3235 2674 7970  ..2022-10-25&typ
-000077c0: 653d 4973 7375 6573 2920 7c20 5b40 7072  e=Issues) | [@pr
-000077d0: 652d 636f 6d6d 6974 2d63 695d 2868 7474  e-commit-ci](htt
-000077e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000077f0: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
-00007800: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
-00007810: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
-00007820: 7325 3341 7072 652d 636f 6d6d 6974 2d63  s%3Apre-commit-c
-00007830: 692b 7570 6461 7465 6425 3341 3230 3232  i+updated%3A2022
-00007840: 2d31 302d 3132 2e2e 3230 3232 2d31 302d  -10-12..2022-10-
-00007850: 3235 2674 7970 653d 4973 7375 6573 2920  25&type=Issues) 
-00007860: 7c20 5b40 7361 6d72 6174 5d28 6874 7470  | [@samrat](http
-00007870: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00007880: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
-00007890: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
-000078a0: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
-000078b0: 2533 4173 616d 7261 742b 7570 6461 7465  %3Asamrat+update
-000078c0: 6425 3341 3230 3232 2d31 302d 3132 2e2e  d%3A2022-10-12..
-000078d0: 3230 3232 2d31 302d 3235 2674 7970 653d  2022-10-25&type=
-000078e0: 4973 7375 6573 290a 0a23 2320 382e 302e  Issues)..## 8.0.
-000078f0: 3061 300a 0a28 5b46 756c 6c20 4368 616e  0a0..([Full Chan
-00007900: 6765 6c6f 675d 2868 7474 7073 3a2f 2f67  gelog](https://g
-00007910: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
-00007920: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
-00007930: 2f63 6f6d 7061 7265 2f76 372e 332e 352e  /compare/v7.3.5.
-00007940: 2e2e 3036 6539 6362 3366 6232 3961 3839  ..06e9cb3fb29a89
-00007950: 3561 3361 3134 6536 6533 3961 6235 3234  5a3a14e6e39ab524
-00007960: 6131 3362 6563 3835 6563 2929 0a0a 2323  a13bec85ec))..##
-00007970: 2320 456e 6861 6e63 656d 656e 7473 206d  # Enhancements m
-00007980: 6164 650a 0a2d 2052 656d 6f76 6520 6e65  ade..- Remove ne
-00007990: 7374 2d61 7379 6e63 696f 2064 6570 656e  st-asyncio depen
-000079a0: 6465 6e63 7920 5b23 3833 355d 2868 7474  dency [#835](htt
-000079b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000079c0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-000079d0: 636c 6965 6e74 2f70 756c 6c2f 3833 3529  client/pull/835)
-000079e0: 2028 5b40 626c 696e 6b31 3037 335d 2868   ([@blink1073](h
-000079f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00007a00: 6d2f 626c 696e 6b31 3037 3329 290a 0a23  m/blink1073))..#
-00007a10: 2323 2042 7567 7320 6669 7865 640a 0a2d  ## Bugs fixed..-
-00007a20: 2046 6978 2068 616e 646c 696e 6720 6f66   Fix handling of
-00007a30: 2069 6e69 7469 616c 2072 6561 6479 2070   initial ready p
-00007a40: 726f 6d69 7365 205b 2338 3534 5d28 6874  romise [#854](ht
-00007a50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00007a60: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00007a70: 5f63 6c69 656e 742f 7075 6c6c 2f38 3534  _client/pull/854
-00007a80: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
-00007a90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00007aa0: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a2d  om/blink1073)).-
-00007ab0: 2055 7365 2070 7974 6573 745f 6173 796e   Use pytest_asyn
-00007ac0: 6369 6f20 6669 7874 7572 6520 5b23 3832  cio fixture [#82
-00007ad0: 365d 2868 7474 7073 3a2f 2f67 6974 6875  6](https://githu
-00007ae0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-00007af0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-00007b00: 6c2f 3832 3629 2028 5b40 6461 7669 6462  l/826) ([@davidb
-00007b10: 726f 6368 6172 745d 2868 7474 7073 3a2f  rochart](https:/
-00007b20: 2f67 6974 6875 622e 636f 6d2f 6461 7669  /github.com/davi
-00007b30: 6462 726f 6368 6172 7429 290a 0a23 2323  dbrochart))..###
-00007b40: 204d 6169 6e74 656e 616e 6365 2061 6e64   Maintenance and
-00007b50: 2075 706b 6565 7020 696d 7072 6f76 656d   upkeep improvem
-00007b60: 656e 7473 0a0a 2d20 4967 6e6f 7265 2077  ents..- Ignore w
-00007b70: 6172 6e69 6e67 7320 696e 2070 7265 7265  arnings in prere
-00007b80: 6c65 6173 6573 2074 6573 7420 5b23 3834  leases test [#84
-00007b90: 345d 2868 7474 7073 3a2f 2f67 6974 6875  4](https://githu
-00007ba0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-00007bb0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-00007bc0: 6c2f 3834 3429 2028 5b40 626c 696e 6b31  l/844) ([@blink1
-00007bd0: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
-00007be0: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
-00007bf0: 3329 290a 2d20 5573 6520 6861 7463 6820  3)).- Use hatch 
-00007c00: 666f 7220 7665 7273 696f 6e20 5b23 3833  for version [#83
-00007c10: 375d 2868 7474 7073 3a2f 2f67 6974 6875  7](https://githu
-00007c20: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-00007c30: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-00007c40: 6c2f 3833 3729 2028 5b40 626c 696e 6b31  l/837) ([@blink1
-00007c50: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
-00007c60: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
-00007c70: 3329 290a 2d20 4d6f 7665 2074 6573 7473  3)).- Move tests
-00007c80: 2074 6f20 746f 7020 6c65 7665 6c20 5b23   to top level [#
-00007c90: 3833 345d 2868 7474 7073 3a2f 2f67 6974  834](https://git
-00007ca0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-00007cb0: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-00007cc0: 756c 6c2f 3833 3429 2028 5b40 626c 696e  ull/834) ([@blin
-00007cd0: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
-00007ce0: 6974 6875 622e 636f 6d2f 626c 696e 6b31  ithub.com/blink1
-00007cf0: 3037 3329 290a 2d20 4669 7820 6e62 636f  073)).- Fix nbco
-00007d00: 6e76 6572 7420 646f 776e 7374 7265 616d  nvert downstream
-00007d10: 2074 6573 7420 5b23 3832 375d 2868 7474   test [#827](htt
-00007d20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00007d30: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00007d40: 636c 6965 6e74 2f70 756c 6c2f 3832 3729  client/pull/827)
-00007d50: 2028 5b40 626c 696e 6b31 3037 335d 2868   ([@blink1073](h
-00007d60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00007d70: 6d2f 626c 696e 6b31 3037 3329 290a 0a23  m/blink1073))..#
-00007d80: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
-00007d90: 2069 6d70 726f 7665 6d65 6e74 730a 0a2d   improvements..-
-00007da0: 2053 7769 7463 6820 746f 2070 7964 6174   Switch to pydat
-00007db0: 6120 7370 6869 6e78 2074 6865 6d65 205b  a sphinx theme [
-00007dc0: 2338 3430 5d28 6874 7470 733a 2f2f 6769  #840](https://gi
-00007dd0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-00007de0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-00007df0: 7075 6c6c 2f38 3430 2920 285b 4062 6c69  pull/840) ([@bli
-00007e00: 6e6b 3130 3733 5d28 6874 7470 733a 2f2f  nk1073](https://
-00007e10: 6769 7468 7562 2e63 6f6d 2f62 6c69 6e6b  github.com/blink
-00007e20: 3130 3733 2929 0a0a 2323 2320 436f 6e74  1073))..### Cont
-00007e30: 7269 6275 746f 7273 2074 6f20 7468 6973  ributors to this
-00007e40: 2072 656c 6561 7365 0a0a 285b 4769 7448   release..([GitH
-00007e50: 7562 2063 6f6e 7472 6962 7574 6f72 7320  ub contributors 
-00007e60: 7061 6765 2066 6f72 2074 6869 7320 7265  page for this re
-00007e70: 6c65 6173 655d 2868 7474 7073 3a2f 2f67  lease](https://g
-00007e80: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
-00007e90: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
-00007ea0: 2f67 7261 7068 732f 636f 6e74 7269 6275  /graphs/contribu
-00007eb0: 746f 7273 3f66 726f 6d3d 3230 3232 2d30  tors?from=2022-0
-00007ec0: 382d 3235 2674 6f3d 3230 3232 2d31 302d  8-25&to=2022-10-
-00007ed0: 3132 2674 7970 653d 6329 290a 0a5b 4062  12&type=c))..[@b
-00007ee0: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
-00007ef0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
-00007f00: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
-00007f10: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
-00007f20: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
-00007f30: 4162 6c69 6e6b 3130 3733 2b75 7064 6174  Ablink1073+updat
-00007f40: 6564 2533 4132 3032 322d 3038 2d32 352e  ed%3A2022-08-25.
-00007f50: 2e32 3032 322d 3130 2d31 3226 7479 7065  .2022-10-12&type
-00007f60: 3d49 7373 7565 7329 207c 205b 4063 636f  =Issues) | [@cco
-00007f70: 7264 6f62 6131 325d 2868 7474 7073 3a2f  rdoba12](https:/
-00007f80: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-00007f90: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-00007fa0: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-00007fb0: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-00007fc0: 6363 6f72 646f 6261 3132 2b75 7064 6174  ccordoba12+updat
-00007fd0: 6564 2533 4132 3032 322d 3038 2d32 352e  ed%3A2022-08-25.
-00007fe0: 2e32 3032 322d 3130 2d31 3226 7479 7065  .2022-10-12&type
-00007ff0: 3d49 7373 7565 7329 207c 205b 4064 6176  =Issues) | [@dav
-00008000: 6964 6272 6f63 6861 7274 5d28 6874 7470  idbrochart](http
-00008010: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00008020: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
-00008030: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
-00008040: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
-00008050: 2533 4164 6176 6964 6272 6f63 6861 7274  %3Adavidbrochart
-00008060: 2b75 7064 6174 6564 2533 4132 3032 322d  +updated%3A2022-
-00008070: 3038 2d32 352e 2e32 3032 322d 3130 2d31  08-25..2022-10-1
-00008080: 3226 7479 7065 3d49 7373 7565 7329 207c  2&type=Issues) |
-00008090: 205b 406d 696e 726b 5d28 6874 7470 733a   [@minrk](https:
-000080a0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
-000080b0: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
-000080c0: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
-000080d0: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
-000080e0: 416d 696e 726b 2b75 7064 6174 6564 2533  Aminrk+updated%3
-000080f0: 4132 3032 322d 3038 2d32 352e 2e32 3032  A2022-08-25..202
-00008100: 322d 3130 2d31 3226 7479 7065 3d49 7373  2-10-12&type=Iss
-00008110: 7565 7329 207c 205b 4070 7265 2d63 6f6d  ues) | [@pre-com
-00008120: 6d69 742d 6369 5d28 6874 7470 733a 2f2f  mit-ci](https://
-00008130: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
-00008140: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
-00008150: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
-00008160: 656e 742b 696e 766f 6c76 6573 2533 4170  ent+involves%3Ap
-00008170: 7265 2d63 6f6d 6d69 742d 6369 2b75 7064  re-commit-ci+upd
-00008180: 6174 6564 2533 4132 3032 322d 3038 2d32  ated%3A2022-08-2
-00008190: 352e 2e32 3032 322d 3130 2d31 3226 7479  5..2022-10-12&ty
-000081a0: 7065 3d49 7373 7565 7329 207c 205b 405a  pe=Issues) | [@Z
-000081b0: 7361 696c 6572 5d28 6874 7470 733a 2f2f  sailer](https://
-000081c0: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
-000081d0: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
-000081e0: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
-000081f0: 656e 742b 696e 766f 6c76 6573 2533 415a  ent+involves%3AZ
-00008200: 7361 696c 6572 2b75 7064 6174 6564 2533  sailer+updated%3
-00008210: 4132 3032 322d 3038 2d32 352e 2e32 3032  A2022-08-25..202
-00008220: 322d 3130 2d31 3226 7479 7065 3d49 7373  2-10-12&type=Iss
-00008230: 7565 7329 0a0a 2323 2037 2e33 2e35 0a0a  ues)..## 7.3.5..
-00008240: 285b 4675 6c6c 2043 6861 6e67 656c 6f67  ([Full Changelog
-00008250: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00008260: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00008270: 7974 6572 5f63 6c69 656e 742f 636f 6d70  yter_client/comp
-00008280: 6172 652f 7637 2e33 2e34 2e2e 2e62 6335  are/v7.3.4...bc5
-00008290: 6465 6435 3433 3963 6135 3562 6436 3734  ded5439ca55bd674
-000082a0: 3038 3835 6562 3361 3434 6361 3662 6333  0885eb3a44ca6bc3
-000082b0: 6532 3234 3329 290a 0a23 2323 2045 6e68  e2243))..### Enh
-000082c0: 616e 6365 6d65 6e74 7320 6d61 6465 0a0a  ancements made..
-000082d0: 2d20 6164 6420 6041 7379 6e63 4b65 726e  - add `AsyncKern
-000082e0: 656c 436c 6965 6e74 6020 746f 2060 646f  elClient` to `do
-000082f0: 632f 6170 692f 636c 6965 6e74 2e72 7374  c/api/client.rst
-00008300: 6020 5b23 3831 395d 2868 7474 7073 3a2f  ` [#819](https:/
-00008310: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-00008320: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-00008330: 6e74 2f70 756c 6c2f 3831 3929 2028 5b40  nt/pull/819) ([@
-00008340: 6865 6c69 6f7a 3131 5d28 6874 7470 733a  helioz11](https:
-00008350: 2f2f 6769 7468 7562 2e63 6f6d 2f68 656c  //github.com/hel
-00008360: 696f 7a31 3129 290a 0a23 2323 2042 7567  ioz11))..### Bug
-00008370: 7320 6669 7865 640a 0a2d 2055 7365 2074  s fixed..- Use t
-00008380: 6f72 6e61 646f 2036 2e32 2773 2050 6572  ornado 6.2's Per
-00008390: 696f 6469 6343 616c 6c62 6163 6b20 696e  iodicCallback in
-000083a0: 2072 6573 7461 7274 6572 205b 2338 3232   restarter [#822
-000083b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000083c0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-000083d0: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-000083e0: 2f38 3232 2920 285b 4076 6964 6172 7466  /822) ([@vidartf
-000083f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00008400: 2e63 6f6d 2f76 6964 6172 7466 2929 0a2d  .com/vidartf)).-
-00008410: 204d 616b 6520 5c5f 7374 6469 6e5f 686f   Make \_stdin_ho
-00008420: 6f6b 5f64 6566 6175 6c74 2061 7379 6e63  ok_default async
-00008430: 205b 2338 3134 5d28 6874 7470 733a 2f2f   [#814](https://
-00008440: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00008450: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00008460: 742f 7075 6c6c 2f38 3134 2920 285b 4064  t/pull/814) ([@d
-00008470: 6176 6964 6272 6f63 6861 7274 5d28 6874  avidbrochart](ht
-00008480: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00008490: 2f64 6176 6964 6272 6f63 6861 7274 2929  /davidbrochart))
-000084a0: 0a0a 2323 2320 4d61 696e 7465 6e61 6e63  ..### Maintenanc
-000084b0: 6520 616e 6420 7570 6b65 6570 2069 6d70  e and upkeep imp
-000084c0: 726f 7665 6d65 6e74 730a 0a2d 205c 5b70  rovements..- \[p
-000084d0: 7265 2d63 6f6d 6d69 742e 6369 5c5d 2070  re-commit.ci\] p
-000084e0: 7265 2d63 6f6d 6d69 7420 6175 746f 7570  re-commit autoup
-000084f0: 6461 7465 205b 2338 3234 5d28 6874 7470  date [#824](http
-00008500: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00008510: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00008520: 6c69 656e 742f 7075 6c6c 2f38 3234 2920  lient/pull/824) 
-00008530: 285b 4070 7265 2d63 6f6d 6d69 742d 6369  ([@pre-commit-ci
-00008540: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00008550: 2e63 6f6d 2f70 7265 2d63 6f6d 6d69 742d  .com/pre-commit-
-00008560: 6369 2929 0a2d 205c 5b70 7265 2d63 6f6d  ci)).- \[pre-com
-00008570: 6d69 742e 6369 5c5d 2070 7265 2d63 6f6d  mit.ci\] pre-com
-00008580: 6d69 7420 6175 746f 7570 6461 7465 205b  mit autoupdate [
-00008590: 2338 3231 5d28 6874 7470 733a 2f2f 6769  #821](https://gi
-000085a0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-000085b0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-000085c0: 7075 6c6c 2f38 3231 2920 285b 4070 7265  pull/821) ([@pre
-000085d0: 2d63 6f6d 6d69 742d 6369 5d28 6874 7470  -commit-ci](http
-000085e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-000085f0: 7265 2d63 6f6d 6d69 742d 6369 2929 0a2d  re-commit-ci)).-
-00008600: 205c 5b70 7265 2d63 6f6d 6d69 742e 6369   \[pre-commit.ci
-00008610: 5c5d 2070 7265 2d63 6f6d 6d69 7420 6175  \] pre-commit au
-00008620: 746f 7570 6461 7465 205b 2338 3230 5d28  toupdate [#820](
-00008630: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00008640: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-00008650: 6572 5f63 6c69 656e 742f 7075 6c6c 2f38  er_client/pull/8
-00008660: 3230 2920 285b 4070 7265 2d63 6f6d 6d69  20) ([@pre-commi
-00008670: 742d 6369 5d28 6874 7470 733a 2f2f 6769  t-ci](https://gi
-00008680: 7468 7562 2e63 6f6d 2f70 7265 2d63 6f6d  thub.com/pre-com
-00008690: 6d69 742d 6369 2929 0a2d 205c 5b70 7265  mit-ci)).- \[pre
-000086a0: 2d63 6f6d 6d69 742e 6369 5c5d 2070 7265  -commit.ci\] pre
-000086b0: 2d63 6f6d 6d69 7420 6175 746f 7570 6461  -commit autoupda
-000086c0: 7465 205b 2338 3138 5d28 6874 7470 733a  te [#818](https:
-000086d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-000086e0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-000086f0: 656e 742f 7075 6c6c 2f38 3138 2920 285b  ent/pull/818) ([
-00008700: 4070 7265 2d63 6f6d 6d69 742d 6369 5d28  @pre-commit-ci](
-00008710: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00008720: 6f6d 2f70 7265 2d63 6f6d 6d69 742d 6369  om/pre-commit-ci
-00008730: 2929 0a2d 205c 5b70 7265 2d63 6f6d 6d69  )).- \[pre-commi
-00008740: 742e 6369 5c5d 2070 7265 2d63 6f6d 6d69  t.ci\] pre-commi
-00008750: 7420 6175 746f 7570 6461 7465 205b 2338  t autoupdate [#8
-00008760: 3136 5d28 6874 7470 733a 2f2f 6769 7468  16](https://gith
-00008770: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00008780: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-00008790: 6c6c 2f38 3136 2920 285b 4070 7265 2d63  ll/816) ([@pre-c
-000087a0: 6f6d 6d69 742d 6369 5d28 6874 7470 733a  ommit-ci](https:
-000087b0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7265  //github.com/pre
-000087c0: 2d63 6f6d 6d69 742d 6369 2929 0a2d 205c  -commit-ci)).- \
-000087d0: 5b70 7265 2d63 6f6d 6d69 742e 6369 5c5d  [pre-commit.ci\]
-000087e0: 2070 7265 2d63 6f6d 6d69 7420 6175 746f   pre-commit auto
-000087f0: 7570 6461 7465 205b 2338 3135 5d28 6874  update [#815](ht
-00008800: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00008810: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00008820: 5f63 6c69 656e 742f 7075 6c6c 2f38 3135  _client/pull/815
-00008830: 2920 285b 4070 7265 2d63 6f6d 6d69 742d  ) ([@pre-commit-
-00008840: 6369 5d28 6874 7470 733a 2f2f 6769 7468  ci](https://gith
-00008850: 7562 2e63 6f6d 2f70 7265 2d63 6f6d 6d69  ub.com/pre-commi
-00008860: 742d 6369 2929 0a2d 205c 5b70 7265 2d63  t-ci)).- \[pre-c
-00008870: 6f6d 6d69 742e 6369 5c5d 2070 7265 2d63  ommit.ci\] pre-c
-00008880: 6f6d 6d69 7420 6175 746f 7570 6461 7465  ommit autoupdate
-00008890: 205b 2338 3132 5d28 6874 7470 733a 2f2f   [#812](https://
-000088a0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-000088b0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-000088c0: 742f 7075 6c6c 2f38 3132 2920 285b 4070  t/pull/812) ([@p
-000088d0: 7265 2d63 6f6d 6d69 742d 6369 5d28 6874  re-commit-ci](ht
-000088e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000088f0: 2f70 7265 2d63 6f6d 6d69 742d 6369 2929  /pre-commit-ci))
-00008900: 0a2d 205c 5b70 7265 2d63 6f6d 6d69 742e  .- \[pre-commit.
-00008910: 6369 5c5d 2070 7265 2d63 6f6d 6d69 7420  ci\] pre-commit 
-00008920: 6175 746f 7570 6461 7465 205b 2338 3130  autoupdate [#810
-00008930: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00008940: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00008950: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00008960: 2f38 3130 2920 285b 4070 7265 2d63 6f6d  /810) ([@pre-com
-00008970: 6d69 742d 6369 5d28 6874 7470 733a 2f2f  mit-ci](https://
-00008980: 6769 7468 7562 2e63 6f6d 2f70 7265 2d63  github.com/pre-c
-00008990: 6f6d 6d69 742d 6369 2929 0a2d 205c 5b70  ommit-ci)).- \[p
-000089a0: 7265 2d63 6f6d 6d69 742e 6369 5c5d 2070  re-commit.ci\] p
-000089b0: 7265 2d63 6f6d 6d69 7420 6175 746f 7570  re-commit autoup
-000089c0: 6461 7465 205b 2338 3039 5d28 6874 7470  date [#809](http
-000089d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000089e0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-000089f0: 6c69 656e 742f 7075 6c6c 2f38 3039 2920  lient/pull/809) 
-00008a00: 285b 4070 7265 2d63 6f6d 6d69 742d 6369  ([@pre-commit-ci
-00008a10: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00008a20: 2e63 6f6d 2f70 7265 2d63 6f6d 6d69 742d  .com/pre-commit-
-00008a30: 6369 2929 0a2d 205c 5b70 7265 2d63 6f6d  ci)).- \[pre-com
-00008a40: 6d69 742e 6369 5c5d 2070 7265 2d63 6f6d  mit.ci\] pre-com
-00008a50: 6d69 7420 6175 746f 7570 6461 7465 205b  mit autoupdate [
-00008a60: 2338 3037 5d28 6874 7470 733a 2f2f 6769  #807](https://gi
-00008a70: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-00008a80: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-00008a90: 7075 6c6c 2f38 3037 2920 285b 4070 7265  pull/807) ([@pre
-00008aa0: 2d63 6f6d 6d69 742d 6369 5d28 6874 7470  -commit-ci](http
-00008ab0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00008ac0: 7265 2d63 6f6d 6d69 742d 6369 2929 0a0a  re-commit-ci))..
-00008ad0: 2323 2320 436f 6e74 7269 6275 746f 7273  ### Contributors
-00008ae0: 2074 6f20 7468 6973 2072 656c 6561 7365   to this release
-00008af0: 0a0a 285b 4769 7448 7562 2063 6f6e 7472  ..([GitHub contr
-00008b00: 6962 7574 6f72 7320 7061 6765 2066 6f72  ibutors page for
-00008b10: 2074 6869 7320 7265 6c65 6173 655d 2868   this release](h
-00008b20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00008b30: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00008b40: 725f 636c 6965 6e74 2f67 7261 7068 732f  r_client/graphs/
-00008b50: 636f 6e74 7269 6275 746f 7273 3f66 726f  contributors?fro
-00008b60: 6d3d 3230 3232 2d30 362d 3038 2674 6f3d  m=2022-06-08&to=
-00008b70: 3230 3232 2d30 382d 3235 2674 7970 653d  2022-08-25&type=
-00008b80: 6329 290a 0a5b 4062 6c69 6e6b 3130 3733  c))..[@blink1073
-00008b90: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00008ba0: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
-00008bb0: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
-00008bc0: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
-00008bd0: 766f 6c76 6573 2533 4162 6c69 6e6b 3130  volves%3Ablink10
-00008be0: 3733 2b75 7064 6174 6564 2533 4132 3032  73+updated%3A202
-00008bf0: 322d 3036 2d30 382e 2e32 3032 322d 3038  2-06-08..2022-08
-00008c00: 2d32 3526 7479 7065 3d49 7373 7565 7329  -25&type=Issues)
-00008c10: 207c 205b 4064 6176 6964 6272 6f63 6861   | [@davidbrocha
-00008c20: 7274 5d28 6874 7470 733a 2f2f 6769 7468  rt](https://gith
-00008c30: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
-00008c40: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
-00008c50: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
-00008c60: 696e 766f 6c76 6573 2533 4164 6176 6964  involves%3Adavid
-00008c70: 6272 6f63 6861 7274 2b75 7064 6174 6564  brochart+updated
-00008c80: 2533 4132 3032 322d 3036 2d30 382e 2e32  %3A2022-06-08..2
-00008c90: 3032 322d 3038 2d32 3526 7479 7065 3d49  022-08-25&type=I
-00008ca0: 7373 7565 7329 207c 205b 4068 656c 696f  ssues) | [@helio
-00008cb0: 7a31 315d 2868 7474 7073 3a2f 2f67 6974  z11](https://git
-00008cc0: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
-00008cd0: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
-00008ce0: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
-00008cf0: 2b69 6e76 6f6c 7665 7325 3341 6865 6c69  +involves%3Aheli
-00008d00: 6f7a 3131 2b75 7064 6174 6564 2533 4132  oz11+updated%3A2
-00008d10: 3032 322d 3036 2d30 382e 2e32 3032 322d  022-06-08..2022-
-00008d20: 3038 2d32 3526 7479 7065 3d49 7373 7565  08-25&type=Issue
-00008d30: 7329 207c 205b 4070 7265 2d63 6f6d 6d69  s) | [@pre-commi
-00008d40: 742d 6369 5d28 6874 7470 733a 2f2f 6769  t-ci](https://gi
-00008d50: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
-00008d60: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
-00008d70: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
-00008d80: 742b 696e 766f 6c76 6573 2533 4170 7265  t+involves%3Apre
-00008d90: 2d63 6f6d 6d69 742d 6369 2b75 7064 6174  -commit-ci+updat
-00008da0: 6564 2533 4132 3032 322d 3036 2d30 382e  ed%3A2022-06-08.
-00008db0: 2e32 3032 322d 3038 2d32 3526 7479 7065  .2022-08-25&type
-00008dc0: 3d49 7373 7565 7329 207c 205b 4076 6964  =Issues) | [@vid
-00008dd0: 6172 7466 5d28 6874 7470 733a 2f2f 6769  artf](https://gi
-00008de0: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
-00008df0: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
-00008e00: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
-00008e10: 742b 696e 766f 6c76 6573 2533 4176 6964  t+involves%3Avid
-00008e20: 6172 7466 2b75 7064 6174 6564 2533 4132  artf+updated%3A2
-00008e30: 3032 322d 3036 2d30 382e 2e32 3032 322d  022-06-08..2022-
-00008e40: 3038 2d32 3526 7479 7065 3d49 7373 7565  08-25&type=Issue
-00008e50: 7329 0a0a 2323 2037 2e33 2e34 0a0a 285b  s)..## 7.3.4..([
-00008e60: 4675 6c6c 2043 6861 6e67 656c 6f67 5d28  Full Changelog](
-00008e70: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00008e80: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-00008e90: 6572 5f63 6c69 656e 742f 636f 6d70 6172  er_client/compar
-00008ea0: 652f 7637 2e33 2e33 2e2e 2e63 6134 6362  e/v7.3.3...ca4cb
-00008eb0: 3264 3661 3462 3935 6136 3932 3564 6538  2d6a4b95a6925de8
-00008ec0: 3561 3437 6233 3233 6432 3233 3530 3332  5a47b323d2235032
-00008ed0: 6337 3429 290a 0a23 2323 2042 7567 7320  c74))..### Bugs 
-00008ee0: 6669 7865 640a 0a2d 2052 6576 6572 7420  fixed..- Revert 
-00008ef0: 6c61 7465 7374 2063 6861 6e67 6573 2074  latest changes t
-00008f00: 6f20 6054 6872 6561 6465 645a 4d51 536f  o `ThreadedZMQSo
-00008f10: 636b 6574 4368 616e 6e65 6c60 2062 6563  cketChannel` bec
-00008f20: 6175 7365 2074 6865 7920 6272 6561 6b20  ause they break 
-00008f30: 5174 636f 6e73 6f6c 6520 5b23 3830 335d  Qtconsole [#803]
-00008f40: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00008f50: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-00008f60: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-00008f70: 3830 3329 2028 5b40 6363 6f72 646f 6261  803) ([@ccordoba
-00008f80: 3132 5d28 6874 7470 733a 2f2f 6769 7468  12](https://gith
-00008f90: 7562 2e63 6f6d 2f63 636f 7264 6f62 6131  ub.com/ccordoba1
-00008fa0: 3229 290a 0a23 2323 204d 6169 6e74 656e  2))..### Mainten
-00008fb0: 616e 6365 2061 6e64 2075 706b 6565 7020  ance and upkeep 
-00008fc0: 696d 7072 6f76 656d 656e 7473 0a0a 2d20  improvements..- 
-00008fd0: 4669 7820 7370 6869 6e78 2035 2e30 2073  Fix sphinx 5.0 s
-00008fe0: 7570 706f 7274 205b 2338 3034 5d28 6874  upport [#804](ht
-00008ff0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00009000: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00009010: 5f63 6c69 656e 742f 7075 6c6c 2f38 3034  _client/pull/804
-00009020: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
-00009030: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00009040: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a2d  om/blink1073)).-
-00009050: 205c 5b70 7265 2d63 6f6d 6d69 742e 6369   \[pre-commit.ci
-00009060: 5c5d 2070 7265 2d63 6f6d 6d69 7420 6175  \] pre-commit au
-00009070: 746f 7570 6461 7465 205b 2337 3939 5d28  toupdate [#799](
-00009080: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00009090: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-000090a0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f37  er_client/pull/7
-000090b0: 3939 2920 285b 4070 7265 2d63 6f6d 6d69  99) ([@pre-commi
-000090c0: 742d 6369 5d28 6874 7470 733a 2f2f 6769  t-ci](https://gi
-000090d0: 7468 7562 2e63 6f6d 2f70 7265 2d63 6f6d  thub.com/pre-com
-000090e0: 6d69 742d 6369 2929 0a0a 2323 2320 436f  mit-ci))..### Co
-000090f0: 6e74 7269 6275 746f 7273 2074 6f20 7468  ntributors to th
-00009100: 6973 2072 656c 6561 7365 0a0a 285b 4769  is release..([Gi
-00009110: 7448 7562 2063 6f6e 7472 6962 7574 6f72  tHub contributor
-00009120: 7320 7061 6765 2066 6f72 2074 6869 7320  s page for this 
-00009130: 7265 6c65 6173 655d 2868 7474 7073 3a2f  release](https:/
+00003620: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
+00003630: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
+00003640: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
+00003650: 766f 6c76 6573 2533 4178 6c30 2b75 7064  volves%3Axl0+upd
+00003660: 6174 6564 2533 4132 3032 332d 3031 2d33  ated%3A2023-01-3
+00003670: 302e 2e32 3032 332d 3032 2d31 3626 7479  0..2023-02-16&ty
+00003680: 7065 3d49 7373 7565 7329 0a0a 2323 2038  pe=Issues)..## 8
+00003690: 2e30 2e32 0a0a 285b 4675 6c6c 2043 6861  .0.2..([Full Cha
+000036a0: 6e67 656c 6f67 5d28 6874 7470 733a 2f2f  ngelog](https://
+000036b0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+000036c0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+000036d0: 742f 636f 6d70 6172 652f 7638 2e30 2e31  t/compare/v8.0.1
+000036e0: 2e2e 2e37 3137 6433 3665 6463 6439 6365  ...717d36edcd9ce
+000036f0: 3539 3566 3732 3764 3862 3561 3237 6532  595f727d8b5a27e2
+00003700: 3730 6332 6136 6532 6334 3629 290a 0a23  70c2a6e2c46))..#
+00003710: 2323 2042 7567 7320 6669 7865 640a 0a2d  ## Bugs fixed..-
+00003720: 2041 6464 2070 6170 6572 6d69 6c6c 2064   Add papermill d
+00003730: 6f77 6e73 7472 6561 6d20 6368 6563 6b20  ownstream check 
+00003740: 616e 6420 6669 7820 6b65 726e 656c 2063  and fix kernel c
+00003750: 6c69 656e 7420 7265 706c 6965 7320 5b23  lient replies [#
+00003760: 3932 355d 2868 7474 7073 3a2f 2f67 6974  925](https://git
+00003770: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00003780: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+00003790: 756c 6c2f 3932 3529 2028 5b40 626c 696e  ull/925) ([@blin
+000037a0: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
+000037b0: 6974 6875 622e 636f 6d2f 626c 696e 6b31  ithub.com/blink1
+000037c0: 3037 3329 290a 0a23 2323 204d 6169 6e74  073))..### Maint
+000037d0: 656e 616e 6365 2061 6e64 2075 706b 6565  enance and upkee
+000037e0: 7020 696d 7072 6f76 656d 656e 7473 0a0a  p improvements..
+000037f0: 2d20 4164 6f70 7420 6d6f 7265 2072 7566  - Adopt more ruf
+00003800: 6620 7275 6c65 7320 5b23 3932 345d 2868  f rules [#924](h
+00003810: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00003820: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+00003830: 725f 636c 6965 6e74 2f70 756c 6c2f 3932  r_client/pull/92
+00003840: 3429 2028 5b40 626c 696e 6b31 3037 335d  4) ([@blink1073]
+00003850: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00003860: 636f 6d2f 626c 696e 6b31 3037 3329 290a  com/blink1073)).
+00003870: 2d20 5072 6566 6572 2070 7269 6e74 2069  - Prefer print i
+00003880: 6e20 6b65 726e 656c 7370 6563 6170 7020  n kernelspecapp 
+00003890: 5b23 3932 335d 2868 7474 7073 3a2f 2f67  [#923](https://g
+000038a0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+000038b0: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+000038c0: 2f70 756c 6c2f 3932 3329 2028 5b40 626c  /pull/923) ([@bl
+000038d0: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
+000038e0: 2f67 6974 6875 622e 636f 6d2f 626c 696e  /github.com/blin
+000038f0: 6b31 3037 3329 290a 0a23 2323 2043 6f6e  k1073))..### Con
+00003900: 7472 6962 7574 6f72 7320 746f 2074 6869  tributors to thi
+00003910: 7320 7265 6c65 6173 650a 0a28 5b47 6974  s release..([Git
+00003920: 4875 6220 636f 6e74 7269 6275 746f 7273  Hub contributors
+00003930: 2070 6167 6520 666f 7220 7468 6973 2072   page for this r
+00003940: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
+00003950: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00003960: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00003970: 742f 6772 6170 6873 2f63 6f6e 7472 6962  t/graphs/contrib
+00003980: 7574 6f72 733f 6672 6f6d 3d32 3032 332d  utors?from=2023-
+00003990: 3031 2d32 3626 746f 3d32 3032 332d 3031  01-26&to=2023-01
+000039a0: 2d33 3026 7479 7065 3d63 2929 0a0a 5b40  -30&type=c))..[@
+000039b0: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
+000039c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
+000039d0: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
+000039e0: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
+000039f0: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
+00003a00: 3341 626c 696e 6b31 3037 332b 7570 6461  3Ablink1073+upda
+00003a10: 7465 6425 3341 3230 3233 2d30 312d 3236  ted%3A2023-01-26
+00003a20: 2e2e 3230 3233 2d30 312d 3330 2674 7970  ..2023-01-30&typ
+00003a30: 653d 4973 7375 6573 290a 0a23 2320 382e  e=Issues)..## 8.
+00003a40: 302e 310a 0a28 5b46 756c 6c20 4368 616e  0.1..([Full Chan
+00003a50: 6765 6c6f 675d 2868 7474 7073 3a2f 2f67  gelog](https://g
+00003a60: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00003a70: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00003a80: 2f63 6f6d 7061 7265 2f76 382e 302e 302e  /compare/v8.0.0.
+00003a90: 2e2e 6463 3631 3133 6333 3630 6530 3531  ..dc6113c360e051
+00003aa0: 3232 3433 3062 3865 3133 3033 3734 6539  22430b8e130374e9
+00003ab0: 6634 6534 6237 3031 6437 2929 0a0a 2323  f4e4b701d7))..##
+00003ac0: 2320 4275 6773 2066 6978 6564 0a0a 2d20  # Bugs fixed..- 
+00003ad0: 4669 7820 6a73 6f6e 5f6f 7574 7075 7420  Fix json_output 
+00003ae0: 696e 206b 6572 6e65 6c73 7065 6320 6170  in kernelspec ap
+00003af0: 7020 5b23 3932 315d 2868 7474 7073 3a2f  p [#921](https:/
+00003b00: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00003b10: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00003b20: 6e74 2f70 756c 6c2f 3932 3129 2028 5b40  nt/pull/921) ([@
+00003b30: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
+00003b40: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
+00003b50: 696e 6b31 3037 3329 290a 0a23 2323 2043  ink1073))..### C
+00003b60: 6f6e 7472 6962 7574 6f72 7320 746f 2074  ontributors to t
+00003b70: 6869 7320 7265 6c65 6173 650a 0a28 5b47  his release..([G
+00003b80: 6974 4875 6220 636f 6e74 7269 6275 746f  itHub contributo
+00003b90: 7273 2070 6167 6520 666f 7220 7468 6973  rs page for this
+00003ba0: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
+00003bb0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+00003bc0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+00003bd0: 656e 742f 6772 6170 6873 2f63 6f6e 7472  ent/graphs/contr
+00003be0: 6962 7574 6f72 733f 6672 6f6d 3d32 3032  ibutors?from=202
+00003bf0: 332d 3031 2d32 3626 746f 3d32 3032 332d  3-01-26&to=2023-
+00003c00: 3031 2d32 3626 7479 7065 3d63 2929 0a0a  01-26&type=c))..
+00003c10: 5b40 626c 696e 6b31 3037 335d 2868 7474  [@blink1073](htt
+00003c20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00003c30: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
+00003c40: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
+00003c50: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
+00003c60: 7325 3341 626c 696e 6b31 3037 332b 7570  s%3Ablink1073+up
+00003c70: 6461 7465 6425 3341 3230 3233 2d30 312d  dated%3A2023-01-
+00003c80: 3236 2e2e 3230 3233 2d30 312d 3236 2674  26..2023-01-26&t
+00003c90: 7970 653d 4973 7375 6573 290a 0a23 2320  ype=Issues)..## 
+00003ca0: 382e 302e 300a 0a28 5b46 756c 6c20 4368  8.0.0..([Full Ch
+00003cb0: 616e 6765 6c6f 675d 2868 7474 7073 3a2f  angelog](https:/
+00003cc0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00003cd0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00003ce0: 6e74 2f63 6f6d 7061 7265 2f76 372e 332e  nt/compare/v7.3.
+00003cf0: 352e 2e2e 3736 3061 3738 3335 6438 6232  5...760a7835d8b2
+00003d00: 3061 3964 6165 6133 3733 3737 3539 6231  0a9daea3737759b1
+00003d10: 3735 3164 3565 3535 6461 6438 2929 0a0a  751d5e55dad8))..
+00003d20: 5468 6973 2072 656c 6561 7365 2069 7320  This release is 
+00003d30: 7072 696d 6172 696c 7920 666f 6375 7365  primarily focuse
+00003d40: 6420 6f6e 2069 6d70 726f 7669 6e67 2060  d on improving `
+00003d50: 6173 796e 6369 6f60 2073 7570 706f 7274  asyncio` support
+00003d60: 2c20 7768 696c 6520 6169 6d69 6e67 2074  , while aiming t
+00003d70: 6f20 6861 7665 206d 696e 696d 616c 2041  o have minimal A
+00003d80: 5049 2063 6861 6e67 6573 2e0a 0a23 2323  PI changes...###
+00003d90: 2045 6e68 616e 6365 6d65 6e74 7320 6d61   Enhancements ma
+00003da0: 6465 0a0a 2d20 5265 6d6f 7665 206e 6573  de..- Remove nes
+00003db0: 742d 6173 796e 6369 6f20 6465 7065 6e64  t-asyncio depend
+00003dc0: 656e 6379 205b 2338 3335 5d28 6874 7470  ency [#835](http
+00003dd0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00003de0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
+00003df0: 6c69 656e 742f 7075 6c6c 2f38 3335 2920  lient/pull/835) 
+00003e00: 285b 4062 6c69 6e6b 3130 3733 5d28 6874  ([@blink1073](ht
+00003e10: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00003e20: 2f62 6c69 6e6b 3130 3733 2929 0a0a 2323  /blink1073))..##
+00003e30: 2320 4275 6773 2066 6978 6564 0a0a 2d20  # Bugs fixed..- 
+00003e40: 416c 6c6f 7720 696e 7465 7272 7570 7420  Allow interrupt 
+00003e50: 6475 7269 6e67 2072 6573 7461 7274 206f  during restart o
+00003e60: 6620 7065 6e64 696e 6720 6b65 726e 656c  f pending kernel
+00003e70: 7320 5b23 3839 385d 2868 7474 7073 3a2f  s [#898](https:/
+00003e80: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00003e90: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00003ea0: 6e74 2f70 756c 6c2f 3839 3829 2028 5b40  nt/pull/898) ([@
+00003eb0: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
+00003ec0: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
+00003ed0: 696e 6b31 3037 3329 290a 2d20 4669 7820  ink1073)).- Fix 
+00003ee0: 636f 6e6e 6563 7469 6f6e 2072 6563 6f6e  connection recon
+00003ef0: 6369 6c69 6174 696f 6e20 746f 2068 616e  ciliation to han
+00003f00: 646c 6520 7265 7374 6172 7473 205b 2338  dle restarts [#8
+00003f10: 3832 5d28 6874 7470 733a 2f2f 6769 7468  82](https://gith
+00003f20: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00003f30: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+00003f40: 6c6c 2f38 3832 2920 285b 406b 6576 696e  ll/882) ([@kevin
+00003f50: 2d62 6174 6573 5d28 6874 7470 733a 2f2f  -bates](https://
+00003f60: 6769 7468 7562 2e63 6f6d 2f6b 6576 696e  github.com/kevin
+00003f70: 2d62 6174 6573 2929 0a2d 2052 6563 6f6e  -bates)).- Recon
+00003f80: 6369 6c65 2063 6f6e 6e65 6374 696f 6e20  cile connection 
+00003f90: 696e 666f 726d 6174 696f 6e20 5b23 3837  information [#87
+00003fa0: 395d 2868 7474 7073 3a2f 2f67 6974 6875  9](https://githu
+00003fb0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00003fc0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00003fd0: 6c2f 3837 3929 2028 5b40 6b65 7669 6e2d  l/879) ([@kevin-
+00003fe0: 6261 7465 735d 2868 7474 7073 3a2f 2f67  bates](https://g
+00003ff0: 6974 6875 622e 636f 6d2f 6b65 7669 6e2d  ithub.com/kevin-
+00004000: 6261 7465 7329 290a 2d20 576f 726b 6172  bates)).- Workar
+00004010: 6f75 6e64 2066 6f72 206c 6175 6e63 6820  ound for launch 
+00004020: 6275 6720 5b23 3836 315d 2868 7474 7073  bug [#861](https
+00004030: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00004040: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+00004050: 6965 6e74 2f70 756c 6c2f 3836 3129 2028  ient/pull/861) (
+00004060: 5b40 626c 696e 6b31 3037 335d 2868 7474  [@blink1073](htt
+00004070: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004080: 626c 696e 6b31 3037 3329 290a 2d20 4465  blink1073)).- De
+00004090: 6665 7220 6372 6561 7469 6f6e 206f 6620  fer creation of 
+000040a0: 7265 6164 7920 6675 7475 7265 205b 2338  ready future [#8
+000040b0: 3538 5d28 6874 7470 733a 2f2f 6769 7468  58](https://gith
+000040c0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+000040d0: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+000040e0: 6c6c 2f38 3538 2920 285b 4062 6c69 6e6b  ll/858) ([@blink
+000040f0: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
+00004100: 7468 7562 2e63 6f6d 2f62 6c69 6e6b 3130  thub.com/blink10
+00004110: 3733 2929 0a2d 2046 6978 2068 616e 646c  73)).- Fix handl
+00004120: 696e 6720 6f66 2069 6e69 7469 616c 2072  ing of initial r
+00004130: 6561 6479 2070 726f 6d69 7365 205b 2338  eady promise [#8
+00004140: 3534 5d28 6874 7470 733a 2f2f 6769 7468  54](https://gith
+00004150: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00004160: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+00004170: 6c6c 2f38 3534 2920 285b 4062 6c69 6e6b  ll/854) ([@blink
+00004180: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
+00004190: 7468 7562 2e63 6f6d 2f62 6c69 6e6b 3130  thub.com/blink10
+000041a0: 3733 2929 0a2d 2052 6576 6572 7420 2246  73)).- Revert "F
+000041b0: 6978 2070 656e 6469 6e67 206b 6572 6e65  ix pending kerne
+000041c0: 6c73 2061 6761 696e 2220 5b23 3835 335d  ls again" [#853]
+000041d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000041e0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+000041f0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00004200: 3835 3329 2028 5b40 626c 696e 6b31 3037  853) ([@blink107
+00004210: 335d 2868 7474 7073 3a2f 2f67 6974 6875  3](https://githu
+00004220: 622e 636f 6d2f 626c 696e 6b31 3037 3329  b.com/blink1073)
+00004230: 290a 2d20 4669 7820 7065 6e64 696e 6720  ).- Fix pending 
+00004240: 6b65 726e 656c 7320 6167 6169 6e20 5b23  kernels again [#
+00004250: 3834 355d 2868 7474 7073 3a2f 2f67 6974  845](https://git
+00004260: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00004270: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+00004280: 756c 6c2f 3834 3529 2028 5b40 626c 696e  ull/845) ([@blin
+00004290: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
+000042a0: 6974 6875 622e 636f 6d2f 626c 696e 6b31  ithub.com/blink1
+000042b0: 3037 3329 290a 2d20 5573 6520 7079 7465  073)).- Use pyte
+000042c0: 7374 5f61 7379 6e63 696f 2066 6978 7475  st_asyncio fixtu
+000042d0: 7265 205b 2338 3236 5d28 6874 7470 733a  re [#826](https:
+000042e0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+000042f0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+00004300: 656e 742f 7075 6c6c 2f38 3236 2920 285b  ent/pull/826) ([
+00004310: 4064 6176 6964 6272 6f63 6861 7274 5d28  @davidbrochart](
+00004320: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004330: 6f6d 2f64 6176 6964 6272 6f63 6861 7274  om/davidbrochart
+00004340: 2929 0a0a 2323 2320 4d61 696e 7465 6e61  ))..### Maintena
+00004350: 6e63 6520 616e 6420 7570 6b65 6570 2069  nce and upkeep i
+00004360: 6d70 726f 7665 6d65 6e74 730a 0a2d 204d  mprovements..- M
+00004370: 4149 4e54 3a20 446f 6e27 7420 666f 726d  AINT: Don't form
+00004380: 6174 206c 6f67 2069 6e20 6c6f 6720 6361  at log in log ca
+00004390: 6c6c 2e20 5b23 3931 395d 2868 7474 7073  ll. [#919](https
+000043a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+000043b0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+000043c0: 6965 6e74 2f70 756c 6c2f 3931 3929 2028  ient/pull/919) (
+000043d0: 5b40 4361 7272 6561 755d 2868 7474 7073  [@Carreau](https
+000043e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4361  ://github.com/Ca
+000043f0: 7272 6561 7529 290a 2d20 5265 6d6f 7665  rreau)).- Remove
+00004400: 2064 6570 7265 6361 7465 6420 7a6d 7120   deprecated zmq 
+00004410: 696d 706f 7274 7320 5b23 3931 355d 2868  imports [#915](h
+00004420: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00004430: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+00004440: 725f 636c 6965 6e74 2f70 756c 6c2f 3931  r_client/pull/91
+00004450: 3529 2028 5b40 626c 696e 6b31 3037 335d  5) ([@blink1073]
+00004460: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00004470: 636f 6d2f 626c 696e 6b31 3037 3329 290a  com/blink1073)).
+00004480: 2d20 4d41 494e 543a 2063 6f6e 7369 7374  - MAINT: consist
+00004490: 656e 746c 7920 7573 6520 7265 6c61 7469  ently use relati
+000044a0: 7665 2069 6d70 6f72 7473 2e20 5b23 3931  ve imports. [#91
+000044b0: 325d 2868 7474 7073 3a2f 2f67 6974 6875  2](https://githu
+000044c0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+000044d0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+000044e0: 6c2f 3931 3229 2028 5b40 4361 7272 6561  l/912) ([@Carrea
+000044f0: 755d 2868 7474 7073 3a2f 2f67 6974 6875  u](https://githu
+00004500: 622e 636f 6d2f 4361 7272 6561 7529 290a  b.com/Carreau)).
+00004510: 2d20 5379 6e63 206c 696e 7420 6465 7073  - Sync lint deps
+00004520: 205b 2339 3131 5d28 6874 7470 733a 2f2f   [#911](https://
+00004530: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00004540: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00004550: 742f 7075 6c6c 2f39 3131 2920 285b 4062  t/pull/911) ([@b
+00004560: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
+00004570: 2f2f 6769 7468 7562 2e63 6f6d 2f62 6c69  //github.com/bli
+00004580: 6e6b 3130 3733 2929 0a2d 204d 4149 4e54  nk1073)).- MAINT
+00004590: 3a20 5072 6f70 6572 2074 7970 696e 6720  : Proper typing 
+000045a0: 616e 6420 6361 7374 205b 2339 3036 5d28  and cast [#906](
+000045b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000045c0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+000045d0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f39  er_client/pull/9
+000045e0: 3036 2920 285b 4043 6172 7265 6175 5d28  06) ([@Carreau](
+000045f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004600: 6f6d 2f43 6172 7265 6175 2929 0a2d 204d  om/Carreau)).- M
+00004610: 4149 4e54 3a20 5c5b 5f61 7379 6e63 5f5c  AINT: \[_async_\
+00004620: 5d73 7461 7274 5f6b 6572 6e65 6c20 7368  ]start_kernel sh
+00004630: 6f75 6c64 206f 6e6c 7920 7461 6b65 206b  ould only take k
+00004640: 7761 7267 206f 6e6c 792e 205b 2339 3035  warg only. [#905
+00004650: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004660: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00004670: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00004680: 2f39 3035 2920 285b 4043 6172 7265 6175  /905) ([@Carreau
+00004690: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000046a0: 2e63 6f6d 2f43 6172 7265 6175 2929 0a2d  .com/Carreau)).-
+000046b0: 2041 6464 206d 6f72 6520 6369 2063 6865   Add more ci che
+000046c0: 636b 7320 5b23 3930 335d 2868 7474 7073  cks [#903](https
+000046d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+000046e0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+000046f0: 6965 6e74 2f70 756c 6c2f 3930 3329 2028  ient/pull/903) (
+00004700: 5b40 626c 696e 6b31 3037 335d 2868 7474  [@blink1073](htt
+00004710: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004720: 626c 696e 6b31 3037 3329 290a 2d20 416c  blink1073)).- Al
+00004730: 6c6f 7720 7265 6c65 6173 696e 6720 6672  low releasing fr
+00004740: 6f6d 2072 6570 6f20 5b23 3839 395d 2868  om repo [#899](h
+00004750: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00004760: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+00004770: 725f 636c 6965 6e74 2f70 756c 6c2f 3839  r_client/pull/89
+00004780: 3929 2028 5b40 626c 696e 6b31 3037 335d  9) ([@blink1073]
+00004790: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000047a0: 636f 6d2f 626c 696e 6b31 3037 3329 290a  com/blink1073)).
+000047b0: 2d20 4669 7820 6a75 7079 7465 725f 636f  - Fix jupyter_co
+000047c0: 7265 2070 696e 6e69 6e67 205b 2338 3936  re pinning [#896
+000047d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000047e0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+000047f0: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00004800: 2f38 3936 2920 285b 406f 7068 6965 3230  /896) ([@ophie20
+00004810: 305d 2868 7474 7073 3a2f 2f67 6974 6875  0](https://githu
+00004820: 622e 636f 6d2f 6f70 6869 6532 3030 2929  b.com/ophie200))
+00004830: 0a2d 2041 646f 7074 2072 7566 6620 616e  .- Adopt ruff an
+00004840: 6420 7265 6475 6365 2070 7265 2d63 6f6d  d reduce pre-com
+00004850: 6d69 7420 7573 6167 6520 5b23 3839 355d  mit usage [#895]
+00004860: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00004870: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00004880: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00004890: 3839 3529 2028 5b40 626c 696e 6b31 3037  895) ([@blink107
+000048a0: 335d 2868 7474 7073 3a2f 2f67 6974 6875  3](https://githu
+000048b0: 622e 636f 6d2f 626c 696e 6b31 3037 3329  b.com/blink1073)
+000048c0: 290a 2d20 5573 6520 7079 7465 7374 2d6a  ).- Use pytest-j
+000048d0: 7570 7974 6572 205b 2338 3931 5d28 6874  upyter [#891](ht
+000048e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000048f0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+00004900: 5f63 6c69 656e 742f 7075 6c6c 2f38 3931  _client/pull/891
+00004910: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
+00004920: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004930: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a2d  om/blink1073)).-
+00004940: 2049 6d70 6f72 7420 656e 7375 7265 5f61   Import ensure_a
+00004950: 7379 6e63 2061 6e64 2072 756e 5f73 796e  sync and run_syn
+00004960: 6320 6672 6f6d 206a 7570 7974 6572 5f63  c from jupyter_c
+00004970: 6f72 6520 5b23 3838 395d 2868 7474 7073  ore [#889](https
+00004980: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00004990: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+000049a0: 6965 6e74 2f70 756c 6c2f 3838 3929 2028  ient/pull/889) (
+000049b0: 5b40 6461 7669 6462 726f 6368 6172 745d  [@davidbrochart]
+000049c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000049d0: 636f 6d2f 6461 7669 6462 726f 6368 6172  com/davidbrochar
+000049e0: 7429 290a 2d20 5573 6520 6261 7365 2073  t)).- Use base s
+000049f0: 6574 7570 2064 6570 656e 6465 6e63 7920  etup dependency 
+00004a00: 7479 7065 205b 2338 3838 5d28 6874 7470  type [#888](http
+00004a10: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00004a20: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
+00004a30: 6c69 656e 742f 7075 6c6c 2f38 3838 2920  lient/pull/888) 
+00004a40: 285b 4062 6c69 6e6b 3130 3733 5d28 6874  ([@blink1073](ht
+00004a50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00004a60: 2f62 6c69 6e6b 3130 3733 2929 0a2d 204d  /blink1073)).- M
+00004a70: 6f72 6520 4349 2043 6c65 616e 7570 205b  ore CI Cleanup [
+00004a80: 2338 3836 5d28 6874 7470 733a 2f2f 6769  #886](https://gi
+00004a90: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+00004aa0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+00004ab0: 7075 6c6c 2f38 3836 2920 285b 4062 6c69  pull/886) ([@bli
+00004ac0: 6e6b 3130 3733 5d28 6874 7470 733a 2f2f  nk1073](https://
+00004ad0: 6769 7468 7562 2e63 6f6d 2f62 6c69 6e6b  github.com/blink
+00004ae0: 3130 3733 2929 0a2d 204d 6f72 6520 636f  1073)).- More co
+00004af0: 7665 7261 6765 205b 2338 3835 5d28 6874  verage [#885](ht
+00004b00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00004b10: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+00004b20: 5f63 6c69 656e 742f 7075 6c6c 2f38 3835  _client/pull/885
+00004b30: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
+00004b40: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004b50: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a2d  om/blink1073)).-
+00004b60: 2043 6c65 616e 2075 7020 776f 726b 666c   Clean up workfl
+00004b70: 6f77 2061 6e64 2070 7970 726f 6a65 6374  ow and pyproject
+00004b80: 205b 2338 3834 5d28 6874 7470 733a 2f2f   [#884](https://
+00004b90: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00004ba0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00004bb0: 742f 7075 6c6c 2f38 3834 2920 285b 4062  t/pull/884) ([@b
+00004bc0: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
+00004bd0: 2f2f 6769 7468 7562 2e63 6f6d 2f62 6c69  //github.com/bli
+00004be0: 6e6b 3130 3733 2929 0a2d 2041 6464 206d  nk1073)).- Add m
+00004bf0: 6f72 6520 636f 7665 7261 6765 205b 2338  ore coverage [#8
+00004c00: 3737 5d28 6874 7470 733a 2f2f 6769 7468  77](https://gith
+00004c10: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00004c20: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+00004c30: 6c6c 2f38 3737 2920 285b 4062 6c69 6e6b  ll/877) ([@blink
+00004c40: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
+00004c50: 7468 7562 2e63 6f6d 2f62 6c69 6e6b 3130  thub.com/blink10
+00004c60: 3733 2929 0a2d 2041 6464 2063 6f76 6572  73)).- Add cover
+00004c70: 6167 6520 636f 6e66 6967 205b 2338 3736  age config [#876
+00004c80: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004c90: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00004ca0: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00004cb0: 2f38 3736 2920 285b 4062 6c69 6e6b 3130  /876) ([@blink10
+00004cc0: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
+00004cd0: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
+00004ce0: 2929 0a2d 2042 756d 7020 6163 7469 6f6e  )).- Bump action
+00004cf0: 732f 7365 7475 702d 7079 7468 6f6e 2066  s/setup-python f
+00004d00: 726f 6d20 3220 746f 2034 205b 2338 3734  rom 2 to 4 [#874
+00004d10: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004d20: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00004d30: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00004d40: 2f38 3734 2920 285b 4064 6570 656e 6461  /874) ([@dependa
+00004d50: 626f 745d 2868 7474 7073 3a2f 2f67 6974  bot](https://git
+00004d60: 6875 622e 636f 6d2f 6465 7065 6e64 6162  hub.com/dependab
+00004d70: 6f74 2929 0a2d 2042 756d 7020 6163 7469  ot)).- Bump acti
+00004d80: 6f6e 732f 6368 6563 6b6f 7574 2066 726f  ons/checkout fro
+00004d90: 6d20 3220 746f 2033 205b 2338 3733 5d28  m 2 to 3 [#873](
+00004da0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004db0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00004dc0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f38  er_client/pull/8
+00004dd0: 3733 2920 285b 4064 6570 656e 6461 626f  73) ([@dependabo
+00004de0: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00004df0: 622e 636f 6d2f 6465 7065 6e64 6162 6f74  b.com/dependabot
+00004e00: 2929 0a2d 2055 7365 2070 6c61 7466 6f72  )).- Use platfor
+00004e10: 6d20 6469 7273 2069 6e20 7465 7374 7320  m dirs in tests 
+00004e20: 5b23 3837 325d 2868 7474 7073 3a2f 2f67  [#872](https://g
+00004e30: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00004e40: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00004e50: 2f70 756c 6c2f 3837 3229 2028 5b40 626c  /pull/872) ([@bl
+00004e60: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
+00004e70: 2f67 6974 6875 622e 636f 6d2f 626c 696e  /github.com/blin
+00004e80: 6b31 3037 3329 290a 2d20 436c 6561 6e20  k1073)).- Clean 
+00004e90: 7570 2074 7970 6573 2061 6e64 2072 656d  up types and rem
+00004ea0: 6f76 6520 7573 6520 6f66 2065 6e74 7279  ove use of entry
+00004eb0: 706f 696e 7473 205b 2338 3731 5d28 6874  points [#871](ht
+00004ec0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00004ed0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+00004ee0: 5f63 6c69 656e 742f 7075 6c6c 2f38 3731  _client/pull/871
+00004ef0: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
+00004f00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004f10: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a2d  om/blink1073)).-
+00004f20: 2041 6464 2064 6570 656e 6461 626f 7420   Add dependabot 
+00004f30: 5b23 3837 305d 2868 7474 7073 3a2f 2f67  [#870](https://g
+00004f40: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00004f50: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00004f60: 2f70 756c 6c2f 3837 3029 2028 5b40 626c  /pull/870) ([@bl
+00004f70: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
+00004f80: 2f67 6974 6875 622e 636f 6d2f 626c 696e  /github.com/blin
+00004f90: 6b31 3037 3329 290a 2d20 5375 7070 6f72  k1073)).- Suppor
+00004fa0: 7420 5079 7468 6f6e 2033 2e38 2d33 2e31  t Python 3.8-3.1
+00004fb0: 3120 5b23 3836 365d 2868 7474 7073 3a2f  1 [#866](https:/
+00004fc0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00004fd0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00004fe0: 6e74 2f70 756c 6c2f 3836 3629 2028 5b40  nt/pull/866) ([@
+00004ff0: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
+00005000: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
+00005010: 696e 6b31 3037 3329 290a 2d20 4669 7820  ink1073)).- Fix 
+00005020: 6173 7365 7274 696f 6e20 696e 2060 5465  assertion in `Te
+00005030: 7374 5365 7373 696f 6e2e 7465 7374 5f73  stSession.test_s
+00005040: 6572 6961 6c69 7a65 6020 5b23 3836 305d  erialize` [#860]
+00005050: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00005060: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00005070: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00005080: 3836 3029 2028 5b40 7361 6d72 6174 5d28  860) ([@samrat](
+00005090: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000050a0: 6f6d 2f73 616d 7261 7429 290a 2d20 4d61  om/samrat)).- Ma
+000050b0: 696e 7465 6e61 6e63 6520 636c 6561 6e75  intenance cleanu
+000050c0: 7020 5b23 3835 365d 2868 7474 7073 3a2f  p [#856](https:/
+000050d0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+000050e0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+000050f0: 6e74 2f70 756c 6c2f 3835 3629 2028 5b40  nt/pull/856) ([@
+00005100: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
+00005110: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
+00005120: 696e 6b31 3037 3329 290a 2d20 4967 6e6f  ink1073)).- Igno
+00005130: 7265 2077 6172 6e69 6e67 7320 696e 2070  re warnings in p
+00005140: 7265 7265 6c65 6173 6573 2074 6573 7420  rereleases test 
+00005150: 5b23 3834 345d 2868 7474 7073 3a2f 2f67  [#844](https://g
+00005160: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00005170: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00005180: 2f70 756c 6c2f 3834 3429 2028 5b40 626c  /pull/844) ([@bl
+00005190: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
+000051a0: 2f67 6974 6875 622e 636f 6d2f 626c 696e  /github.com/blin
+000051b0: 6b31 3037 3329 290a 2d20 5573 6520 6861  k1073)).- Use ha
+000051c0: 7463 6820 666f 7220 7665 7273 696f 6e20  tch for version 
+000051d0: 5b23 3833 375d 2868 7474 7073 3a2f 2f67  [#837](https://g
+000051e0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+000051f0: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00005200: 2f70 756c 6c2f 3833 3729 2028 5b40 626c  /pull/837) ([@bl
+00005210: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
+00005220: 2f67 6974 6875 622e 636f 6d2f 626c 696e  /github.com/blin
+00005230: 6b31 3037 3329 290a 2d20 4d6f 7665 2074  k1073)).- Move t
+00005240: 6573 7473 2074 6f20 746f 7020 6c65 7665  ests to top leve
+00005250: 6c20 5b23 3833 345d 2868 7474 7073 3a2f  l [#834](https:/
+00005260: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00005270: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00005280: 6e74 2f70 756c 6c2f 3833 3429 2028 5b40  nt/pull/834) ([@
+00005290: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
+000052a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
+000052b0: 696e 6b31 3037 3329 290a 2d20 4669 7820  ink1073)).- Fix 
+000052c0: 6e62 636f 6e76 6572 7420 646f 776e 7374  nbconvert downst
+000052d0: 7265 616d 2074 6573 7420 5b23 3832 375d  ream test [#827]
+000052e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000052f0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00005300: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00005310: 3832 3729 2028 5b40 626c 696e 6b31 3037  827) ([@blink107
+00005320: 335d 2868 7474 7073 3a2f 2f67 6974 6875  3](https://githu
+00005330: 622e 636f 6d2f 626c 696e 6b31 3037 3329  b.com/blink1073)
+00005340: 290a 0a23 2323 2044 6f63 756d 656e 7461  )..### Documenta
+00005350: 7469 6f6e 2069 6d70 726f 7665 6d65 6e74  tion improvement
+00005360: 730a 0a2d 2052 6566 6c65 6374 2063 7572  s..- Reflect cur
+00005370: 7265 6e74 2070 726f 746f 636f 6c20 7665  rent protocol ve
+00005380: 7273 696f 6e20 696e 2064 6f63 756d 656e  rsion in documen
+00005390: 7461 7469 6f6e 205b 2339 3138 5d28 6874  tation [#918](ht
+000053a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000053b0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+000053c0: 5f63 6c69 656e 742f 7075 6c6c 2f39 3138  _client/pull/918
+000053d0: 2920 285b 4053 796c 7661 696e 436f 726c  ) ([@SylvainCorl
+000053e0: 6179 5d28 6874 7470 733a 2f2f 6769 7468  ay](https://gith
+000053f0: 7562 2e63 6f6d 2f53 796c 7661 696e 436f  ub.com/SylvainCo
+00005400: 726c 6179 2929 0a2d 2041 6464 2066 756c  rlay)).- Add ful
+00005410: 6c20 6170 6920 646f 6373 205b 2339 3038  l api docs [#908
+00005420: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00005430: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00005440: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00005450: 2f39 3038 2920 285b 4062 6c69 6e6b 3130  /908) ([@blink10
+00005460: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
+00005470: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
+00005480: 2929 0a2d 2041 6464 206d 6f72 6520 6369  )).- Add more ci
+00005490: 2063 6865 636b 7320 5b23 3930 335d 2868   checks [#903](h
+000054a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000054b0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+000054c0: 725f 636c 6965 6e74 2f70 756c 6c2f 3930  r_client/pull/90
+000054d0: 3329 2028 5b40 626c 696e 6b31 3037 335d  3) ([@blink1073]
+000054e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000054f0: 636f 6d2f 626c 696e 6b31 3037 3329 290a  com/blink1073)).
+00005500: 2d20 5377 6974 6368 2074 6f20 7079 6461  - Switch to pyda
+00005510: 7461 2073 7068 696e 7820 7468 656d 6520  ta sphinx theme 
+00005520: 5b23 3834 305d 2868 7474 7073 3a2f 2f67  [#840](https://g
+00005530: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00005540: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00005550: 2f70 756c 6c2f 3834 3029 2028 5b40 626c  /pull/840) ([@bl
+00005560: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
+00005570: 2f67 6974 6875 622e 636f 6d2f 626c 696e  /github.com/blin
+00005580: 6b31 3037 3329 290a 0a23 2323 2043 6f6e  k1073))..### Con
+00005590: 7472 6962 7574 6f72 7320 746f 2074 6869  tributors to thi
+000055a0: 7320 7265 6c65 6173 650a 0a28 5b47 6974  s release..([Git
+000055b0: 4875 6220 636f 6e74 7269 6275 746f 7273  Hub contributors
+000055c0: 2070 6167 6520 666f 7220 7468 6973 2072   page for this r
+000055d0: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
+000055e0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+000055f0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00005600: 742f 6772 6170 6873 2f63 6f6e 7472 6962  t/graphs/contrib
+00005610: 7574 6f72 733f 6672 6f6d 3d32 3032 322d  utors?from=2022-
+00005620: 3038 2d32 3526 746f 3d32 3032 332d 3031  08-25&to=2023-01
+00005630: 2d32 3626 7479 7065 3d63 2929 0a0a 5b40  -26&type=c))..[@
+00005640: 6172 6f67 6f7a 686e 696b 6f76 5d28 6874  arogozhnikov](ht
+00005650: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00005660: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+00005670: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+00005680: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+00005690: 6573 2533 4161 726f 676f 7a68 6e69 6b6f  es%3Aarogozhniko
+000056a0: 762b 7570 6461 7465 6425 3341 3230 3232  v+updated%3A2022
+000056b0: 2d30 382d 3235 2e2e 3230 3233 2d30 312d  -08-25..2023-01-
+000056c0: 3236 2674 7970 653d 4973 7375 6573 2920  26&type=Issues) 
+000056d0: 7c20 5b40 626c 696e 6b31 3037 335d 2868  | [@blink1073](h
+000056e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000056f0: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
+00005700: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
+00005710: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
+00005720: 7665 7325 3341 626c 696e 6b31 3037 332b  ves%3Ablink1073+
+00005730: 7570 6461 7465 6425 3341 3230 3232 2d30  updated%3A2022-0
+00005740: 382d 3235 2e2e 3230 3233 2d30 312d 3236  8-25..2023-01-26
+00005750: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
+00005760: 5b40 4361 7272 6561 755d 2868 7474 7073  [@Carreau](https
+00005770: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
+00005780: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
+00005790: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
+000057a0: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
+000057b0: 3341 4361 7272 6561 752b 7570 6461 7465  3ACarreau+update
+000057c0: 6425 3341 3230 3232 2d30 382d 3235 2e2e  d%3A2022-08-25..
+000057d0: 3230 3233 2d30 312d 3236 2674 7970 653d  2023-01-26&type=
+000057e0: 4973 7375 6573 2920 7c20 5b40 6363 6f72  Issues) | [@ccor
+000057f0: 646f 6261 3132 5d28 6874 7470 733a 2f2f  doba12](https://
+00005800: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
+00005810: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
+00005820: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
+00005830: 656e 742b 696e 766f 6c76 6573 2533 4163  ent+involves%3Ac
+00005840: 636f 7264 6f62 6131 322b 7570 6461 7465  cordoba12+update
+00005850: 6425 3341 3230 3232 2d30 382d 3235 2e2e  d%3A2022-08-25..
+00005860: 3230 3233 2d30 312d 3236 2674 7970 653d  2023-01-26&type=
+00005870: 4973 7375 6573 2920 7c20 5b40 6461 7669  Issues) | [@davi
+00005880: 6462 726f 6368 6172 745d 2868 7474 7073  dbrochart](https
+00005890: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
+000058a0: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
+000058b0: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
+000058c0: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
+000058d0: 3341 6461 7669 6462 726f 6368 6172 742b  3Adavidbrochart+
+000058e0: 7570 6461 7465 6425 3341 3230 3232 2d30  updated%3A2022-0
+000058f0: 382d 3235 2e2e 3230 3233 2d30 312d 3236  8-25..2023-01-26
+00005900: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
+00005910: 5b40 6465 7065 6e64 6162 6f74 5d28 6874  [@dependabot](ht
+00005920: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00005930: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+00005940: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+00005950: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+00005960: 6573 2533 4164 6570 656e 6461 626f 742b  es%3Adependabot+
+00005970: 7570 6461 7465 6425 3341 3230 3232 2d30  updated%3A2022-0
+00005980: 382d 3235 2e2e 3230 3233 2d30 312d 3236  8-25..2023-01-26
+00005990: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
+000059a0: 5b40 6b65 7669 6e2d 6261 7465 735d 2868  [@kevin-bates](h
+000059b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000059c0: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
+000059d0: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
+000059e0: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
+000059f0: 7665 7325 3341 6b65 7669 6e2d 6261 7465  ves%3Akevin-bate
+00005a00: 732b 7570 6461 7465 6425 3341 3230 3232  s+updated%3A2022
+00005a10: 2d30 382d 3235 2e2e 3230 3233 2d30 312d  -08-25..2023-01-
+00005a20: 3236 2674 7970 653d 4973 7375 6573 2920  26&type=Issues) 
+00005a30: 7c20 5b40 6d65 6573 6565 6b73 6465 765d  | [@meeseeksdev]
+00005a40: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00005a50: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
+00005a60: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
+00005a70: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
+00005a80: 6f6c 7665 7325 3341 6d65 6573 6565 6b73  olves%3Ameeseeks
+00005a90: 6465 762b 7570 6461 7465 6425 3341 3230  dev+updated%3A20
+00005aa0: 3232 2d30 382d 3235 2e2e 3230 3233 2d30  22-08-25..2023-0
+00005ab0: 312d 3236 2674 7970 653d 4973 7375 6573  1-26&type=Issues
+00005ac0: 2920 7c20 5b40 6d69 6e72 6b5d 2868 7474  ) | [@minrk](htt
+00005ad0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00005ae0: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
+00005af0: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
+00005b00: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
+00005b10: 7325 3341 6d69 6e72 6b2b 7570 6461 7465  s%3Aminrk+update
+00005b20: 6425 3341 3230 3232 2d30 382d 3235 2e2e  d%3A2022-08-25..
+00005b30: 3230 3233 2d30 312d 3236 2674 7970 653d  2023-01-26&type=
+00005b40: 4973 7375 6573 2920 7c20 5b40 6f70 6869  Issues) | [@ophi
+00005b50: 6532 3030 5d28 6874 7470 733a 2f2f 6769  e200](https://gi
+00005b60: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
+00005b70: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
+00005b80: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
+00005b90: 742b 696e 766f 6c76 6573 2533 416f 7068  t+involves%3Aoph
+00005ba0: 6965 3230 302b 7570 6461 7465 6425 3341  ie200+updated%3A
+00005bb0: 3230 3232 2d30 382d 3235 2e2e 3230 3233  2022-08-25..2023
+00005bc0: 2d30 312d 3236 2674 7970 653d 4973 7375  -01-26&type=Issu
+00005bd0: 6573 2920 7c20 5b40 7072 652d 636f 6d6d  es) | [@pre-comm
+00005be0: 6974 2d63 695d 2868 7474 7073 3a2f 2f67  it-ci](https://g
+00005bf0: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+00005c00: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+00005c10: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+00005c20: 6e74 2b69 6e76 6f6c 7665 7325 3341 7072  nt+involves%3Apr
+00005c30: 652d 636f 6d6d 6974 2d63 692b 7570 6461  e-commit-ci+upda
+00005c40: 7465 6425 3341 3230 3232 2d30 382d 3235  ted%3A2022-08-25
+00005c50: 2e2e 3230 3233 2d30 312d 3236 2674 7970  ..2023-01-26&typ
+00005c60: 653d 4973 7375 6573 2920 7c20 5b40 7361  e=Issues) | [@sa
+00005c70: 6d72 6174 5d28 6874 7470 733a 2f2f 6769  mrat](https://gi
+00005c80: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
+00005c90: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
+00005ca0: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
+00005cb0: 742b 696e 766f 6c76 6573 2533 4173 616d  t+involves%3Asam
+00005cc0: 7261 742b 7570 6461 7465 6425 3341 3230  rat+updated%3A20
+00005cd0: 3232 2d30 382d 3235 2e2e 3230 3233 2d30  22-08-25..2023-0
+00005ce0: 312d 3236 2674 7970 653d 4973 7375 6573  1-26&type=Issues
+00005cf0: 2920 7c20 5b40 5379 6c76 6169 6e43 6f72  ) | [@SylvainCor
+00005d00: 6c61 795d 2868 7474 7073 3a2f 2f67 6974  lay](https://git
+00005d10: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
+00005d20: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
+00005d30: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
+00005d40: 2b69 6e76 6f6c 7665 7325 3341 5379 6c76  +involves%3ASylv
+00005d50: 6169 6e43 6f72 6c61 792b 7570 6461 7465  ainCorlay+update
+00005d60: 6425 3341 3230 3232 2d30 382d 3235 2e2e  d%3A2022-08-25..
+00005d70: 3230 3233 2d30 312d 3236 2674 7970 653d  2023-01-26&type=
+00005d80: 4973 7375 6573 2920 7c20 5b40 5a73 6169  Issues) | [@Zsai
+00005d90: 6c65 725d 2868 7474 7073 3a2f 2f67 6974  ler](https://git
+00005da0: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
+00005db0: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
+00005dc0: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
+00005dd0: 2b69 6e76 6f6c 7665 7325 3341 5a73 6169  +involves%3AZsai
+00005de0: 6c65 722b 7570 6461 7465 6425 3341 3230  ler+updated%3A20
+00005df0: 3232 2d30 382d 3235 2e2e 3230 3233 2d30  22-08-25..2023-0
+00005e00: 312d 3236 2674 7970 653d 4973 7375 6573  1-26&type=Issues
+00005e10: 290a 0a23 2320 382e 302e 3072 6330 0a0a  )..## 8.0.0rc0..
+00005e20: 285b 4675 6c6c 2043 6861 6e67 656c 6f67  ([Full Changelog
+00005e30: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00005e40: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00005e50: 7974 6572 5f63 6c69 656e 742f 636f 6d70  yter_client/comp
+00005e60: 6172 652f 7638 2e30 2e30 6233 2e2e 2e62  are/v8.0.0b3...b
+00005e70: 6636 3337 6564 3935 3433 3139 3864 3664  f637ed9543198d6d
+00005e80: 6361 3936 6437 3438 6230 3330 3765 6430  ca96d748b0307ed0
+00005e90: 3162 3136 6339 3429 290a 0a23 2323 204d  1b16c94))..### M
+00005ea0: 6169 6e74 656e 616e 6365 2061 6e64 2075  aintenance and u
+00005eb0: 706b 6565 7020 696d 7072 6f76 656d 656e  pkeep improvemen
+00005ec0: 7473 0a0a 2d20 416c 6c6f 7720 7265 6c65  ts..- Allow rele
+00005ed0: 6173 696e 6720 6672 6f6d 2072 6570 6f20  asing from repo 
+00005ee0: 5b23 3839 395d 2868 7474 7073 3a2f 2f67  [#899](https://g
+00005ef0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00005f00: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00005f10: 2f70 756c 6c2f 3839 3929 2028 5b40 626c  /pull/899) ([@bl
+00005f20: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
+00005f30: 2f67 6974 6875 622e 636f 6d2f 626c 696e  /github.com/blin
+00005f40: 6b31 3037 3329 290a 0a23 2323 2043 6f6e  k1073))..### Con
+00005f50: 7472 6962 7574 6f72 7320 746f 2074 6869  tributors to thi
+00005f60: 7320 7265 6c65 6173 650a 0a28 5b47 6974  s release..([Git
+00005f70: 4875 6220 636f 6e74 7269 6275 746f 7273  Hub contributors
+00005f80: 2070 6167 6520 666f 7220 7468 6973 2072   page for this r
+00005f90: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
+00005fa0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00005fb0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00005fc0: 742f 6772 6170 6873 2f63 6f6e 7472 6962  t/graphs/contrib
+00005fd0: 7574 6f72 733f 6672 6f6d 3d32 3032 322d  utors?from=2022-
+00005fe0: 3132 2d31 3326 746f 3d32 3032 322d 3132  12-13&to=2022-12
+00005ff0: 2d31 3926 7479 7065 3d63 2929 0a0a 5b40  -19&type=c))..[@
+00006000: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
+00006010: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
+00006020: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
+00006030: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
+00006040: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
+00006050: 3341 626c 696e 6b31 3037 332b 7570 6461  3Ablink1073+upda
+00006060: 7465 6425 3341 3230 3232 2d31 322d 3133  ted%3A2022-12-13
+00006070: 2e2e 3230 3232 2d31 322d 3139 2674 7970  ..2022-12-19&typ
+00006080: 653d 4973 7375 6573 290a 0a23 2320 382e  e=Issues)..## 8.
+00006090: 302e 3062 330a 0a28 5b46 756c 6c20 4368  0.0b3..([Full Ch
+000060a0: 616e 6765 6c6f 675d 2868 7474 7073 3a2f  angelog](https:/
+000060b0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+000060c0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+000060d0: 6e74 2f63 6f6d 7061 7265 2f76 382e 302e  nt/compare/v8.0.
+000060e0: 3062 322e 2e2e 6235 3161 3362 3564 3161  0b2...b51a3b5d1a
+000060f0: 3064 3161 3861 6433 3930 6331 3132 3135  0d1a8ad390c11215
+00006100: 3036 3231 3739 3039 6461 3163 3466 2929  06217909da1c4f))
+00006110: 0a0a 2323 2320 4275 6773 2066 6978 6564  ..### Bugs fixed
+00006120: 0a0a 2d20 416c 6c6f 7720 696e 7465 7272  ..- Allow interr
+00006130: 7570 7420 6475 7269 6e67 2072 6573 7461  upt during resta
+00006140: 7274 206f 6620 7065 6e64 696e 6720 6b65  rt of pending ke
+00006150: 726e 656c 7320 5b23 3839 385d 2868 7474  rnels [#898](htt
+00006160: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00006170: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00006180: 636c 6965 6e74 2f70 756c 6c2f 3839 3829  client/pull/898)
+00006190: 2028 5b40 626c 696e 6b31 3037 335d 2868   ([@blink1073](h
+000061a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000061b0: 6d2f 626c 696e 6b31 3037 3329 290a 0a23  m/blink1073))..#
+000061c0: 2323 2043 6f6e 7472 6962 7574 6f72 7320  ## Contributors 
+000061d0: 746f 2074 6869 7320 7265 6c65 6173 650a  to this release.
+000061e0: 0a28 5b47 6974 4875 6220 636f 6e74 7269  .([GitHub contri
+000061f0: 6275 746f 7273 2070 6167 6520 666f 7220  butors page for 
+00006200: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
+00006210: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00006220: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+00006230: 5f63 6c69 656e 742f 6772 6170 6873 2f63  _client/graphs/c
+00006240: 6f6e 7472 6962 7574 6f72 733f 6672 6f6d  ontributors?from
+00006250: 3d32 3032 322d 3132 2d30 3826 746f 3d32  =2022-12-08&to=2
+00006260: 3032 322d 3132 2d31 3326 7479 7065 3d63  022-12-13&type=c
+00006270: 2929 0a0a 5b40 626c 696e 6b31 3037 335d  ))..[@blink1073]
+00006280: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00006290: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
+000062a0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
+000062b0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
+000062c0: 6f6c 7665 7325 3341 626c 696e 6b31 3037  olves%3Ablink107
+000062d0: 332b 7570 6461 7465 6425 3341 3230 3232  3+updated%3A2022
+000062e0: 2d31 322d 3038 2e2e 3230 3232 2d31 322d  -12-08..2022-12-
+000062f0: 3133 2674 7970 653d 4973 7375 6573 290a  13&type=Issues).
+00006300: 0a23 2320 382e 302e 3062 320a 0a28 5b46  .## 8.0.0b2..([F
+00006310: 756c 6c20 4368 616e 6765 6c6f 675d 2868  ull Changelog](h
+00006320: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00006330: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+00006340: 725f 636c 6965 6e74 2f63 6f6d 7061 7265  r_client/compare
+00006350: 2f76 382e 302e 3062 312e 2e2e 6666 3333  /v8.0.0b1...ff33
+00006360: 6164 6637 3834 6632 6264 3235 3831 3464  adf784f2bd25814d
+00006370: 3765 6436 6165 3763 3636 3531 6365 6538  7ed6ae7c6651cee8
+00006380: 3337 3665 2929 0a0a 2323 2320 4d61 696e  376e))..### Main
+00006390: 7465 6e61 6e63 6520 616e 6420 7570 6b65  tenance and upke
+000063a0: 6570 2069 6d70 726f 7665 6d65 6e74 730a  ep improvements.
+000063b0: 0a2d 2046 6978 206a 7570 7974 6572 5f63  .- Fix jupyter_c
+000063c0: 6f72 6520 7069 6e6e 696e 6720 5b23 3839  ore pinning [#89
+000063d0: 365d 2868 7474 7073 3a2f 2f67 6974 6875  6](https://githu
+000063e0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+000063f0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00006400: 6c2f 3839 3629 2028 5b40 6f70 6869 6532  l/896) ([@ophie2
+00006410: 3030 5d28 6874 7470 733a 2f2f 6769 7468  00](https://gith
+00006420: 7562 2e63 6f6d 2f6f 7068 6965 3230 3029  ub.com/ophie200)
+00006430: 290a 2d20 4164 6f70 7420 7275 6666 2061  ).- Adopt ruff a
+00006440: 6e64 2072 6564 7563 6520 7072 652d 636f  nd reduce pre-co
+00006450: 6d6d 6974 2075 7361 6765 205b 2338 3935  mmit usage [#895
+00006460: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00006470: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00006480: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00006490: 2f38 3935 2920 285b 4062 6c69 6e6b 3130  /895) ([@blink10
+000064a0: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
+000064b0: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
+000064c0: 2929 0a0a 2323 2320 436f 6e74 7269 6275  ))..### Contribu
+000064d0: 746f 7273 2074 6f20 7468 6973 2072 656c  tors to this rel
+000064e0: 6561 7365 0a0a 285b 4769 7448 7562 2063  ease..([GitHub c
+000064f0: 6f6e 7472 6962 7574 6f72 7320 7061 6765  ontributors page
+00006500: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
+00006510: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00006520: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00006530: 7079 7465 725f 636c 6965 6e74 2f67 7261  pyter_client/gra
+00006540: 7068 732f 636f 6e74 7269 6275 746f 7273  phs/contributors
+00006550: 3f66 726f 6d3d 3230 3232 2d31 322d 3035  ?from=2022-12-05
+00006560: 2674 6f3d 3230 3232 2d31 322d 3038 2674  &to=2022-12-08&t
+00006570: 7970 653d 6329 290a 0a5b 4062 6c69 6e6b  ype=c))..[@blink
+00006580: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
+00006590: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
+000065a0: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
+000065b0: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
+000065c0: 742b 696e 766f 6c76 6573 2533 4162 6c69  t+involves%3Abli
+000065d0: 6e6b 3130 3733 2b75 7064 6174 6564 2533  nk1073+updated%3
+000065e0: 4132 3032 322d 3132 2d30 352e 2e32 3032  A2022-12-05..202
+000065f0: 322d 3132 2d30 3826 7479 7065 3d49 7373  2-12-08&type=Iss
+00006600: 7565 7329 207c 205b 4064 6176 6964 6272  ues) | [@davidbr
+00006610: 6f63 6861 7274 5d28 6874 7470 733a 2f2f  ochart](https://
+00006620: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
+00006630: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
+00006640: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
+00006650: 656e 742b 696e 766f 6c76 6573 2533 4164  ent+involves%3Ad
+00006660: 6176 6964 6272 6f63 6861 7274 2b75 7064  avidbrochart+upd
+00006670: 6174 6564 2533 4132 3032 322d 3132 2d30  ated%3A2022-12-0
+00006680: 352e 2e32 3032 322d 3132 2d30 3826 7479  5..2022-12-08&ty
+00006690: 7065 3d49 7373 7565 7329 207c 205b 406f  pe=Issues) | [@o
+000066a0: 7068 6965 3230 305d 2868 7474 7073 3a2f  phie200](https:/
+000066b0: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
+000066c0: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
+000066d0: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
+000066e0: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
+000066f0: 6f70 6869 6532 3030 2b75 7064 6174 6564  ophie200+updated
+00006700: 2533 4132 3032 322d 3132 2d30 352e 2e32  %3A2022-12-05..2
+00006710: 3032 322d 3132 2d30 3826 7479 7065 3d49  022-12-08&type=I
+00006720: 7373 7565 7329 207c 205b 4070 7265 2d63  ssues) | [@pre-c
+00006730: 6f6d 6d69 742d 6369 5d28 6874 7470 733a  ommit-ci](https:
+00006740: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+00006750: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+00006760: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+00006770: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+00006780: 4170 7265 2d63 6f6d 6d69 742d 6369 2b75  Apre-commit-ci+u
+00006790: 7064 6174 6564 2533 4132 3032 322d 3132  pdated%3A2022-12
+000067a0: 2d30 352e 2e32 3032 322d 3132 2d30 3826  -05..2022-12-08&
+000067b0: 7479 7065 3d49 7373 7565 7329 0a0a 2323  type=Issues)..##
+000067c0: 2038 2e30 2e30 6231 0a0a 4e6f 206d 6572   8.0.0b1..No mer
+000067d0: 6765 6420 5052 730a 0a23 2320 382e 302e  ged PRs..## 8.0.
+000067e0: 3062 300a 0a28 5b46 756c 6c20 4368 616e  0b0..([Full Chan
+000067f0: 6765 6c6f 675d 2868 7474 7073 3a2f 2f67  gelog](https://g
+00006800: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00006810: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00006820: 2f63 6f6d 7061 7265 2f76 382e 302e 3061  /compare/v8.0.0a
+00006830: 342e 2e2e 6534 3139 6666 3461 3635 3162  4...e419ff4a651b
+00006840: 3661 6337 6364 3533 3330 3233 6332 6464  6ac7cd533023c2dd
+00006850: 3362 6433 3931 6465 3665 6236 2929 0a0a  3bd391de6eb6))..
+00006860: 2323 2320 4d61 696e 7465 6e61 6e63 6520  ### Maintenance 
+00006870: 616e 6420 7570 6b65 6570 2069 6d70 726f  and upkeep impro
+00006880: 7665 6d65 6e74 730a 0a2d 2055 7365 2070  vements..- Use p
+00006890: 7974 6573 742d 6a75 7079 7465 7220 5b23  ytest-jupyter [#
+000068a0: 3839 315d 2868 7474 7073 3a2f 2f67 6974  891](https://git
+000068b0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+000068c0: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+000068d0: 756c 6c2f 3839 3129 2028 5b40 626c 696e  ull/891) ([@blin
+000068e0: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
+000068f0: 6974 6875 622e 636f 6d2f 626c 696e 6b31  ithub.com/blink1
+00006900: 3037 3329 290a 2d20 496d 706f 7274 2065  073)).- Import e
+00006910: 6e73 7572 655f 6173 796e 6320 616e 6420  nsure_async and 
+00006920: 7275 6e5f 7379 6e63 2066 726f 6d20 6a75  run_sync from ju
+00006930: 7079 7465 725f 636f 7265 205b 2338 3839  pyter_core [#889
+00006940: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00006950: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00006960: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00006970: 2f38 3839 2920 285b 4064 6176 6964 6272  /889) ([@davidbr
+00006980: 6f63 6861 7274 5d28 6874 7470 733a 2f2f  ochart](https://
+00006990: 6769 7468 7562 2e63 6f6d 2f64 6176 6964  github.com/david
+000069a0: 6272 6f63 6861 7274 2929 0a2d 2055 7365  brochart)).- Use
+000069b0: 2062 6173 6520 7365 7475 7020 6465 7065   base setup depe
+000069c0: 6e64 656e 6379 2074 7970 6520 5b23 3838  ndency type [#88
+000069d0: 385d 2868 7474 7073 3a2f 2f67 6974 6875  8](https://githu
+000069e0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+000069f0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00006a00: 6c2f 3838 3829 2028 5b40 626c 696e 6b31  l/888) ([@blink1
+00006a10: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
+00006a20: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
+00006a30: 3329 290a 2d20 4d6f 7265 2043 4920 436c  3)).- More CI Cl
+00006a40: 6561 6e75 7020 5b23 3838 365d 2868 7474  eanup [#886](htt
+00006a50: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00006a60: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00006a70: 636c 6965 6e74 2f70 756c 6c2f 3838 3629  client/pull/886)
+00006a80: 2028 5b40 626c 696e 6b31 3037 335d 2868   ([@blink1073](h
+00006a90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00006aa0: 6d2f 626c 696e 6b31 3037 3329 290a 2d20  m/blink1073)).- 
+00006ab0: 4d6f 7265 2063 6f76 6572 6167 6520 5b23  More coverage [#
+00006ac0: 3838 355d 2868 7474 7073 3a2f 2f67 6974  885](https://git
+00006ad0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00006ae0: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+00006af0: 756c 6c2f 3838 3529 2028 5b40 626c 696e  ull/885) ([@blin
+00006b00: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
+00006b10: 6974 6875 622e 636f 6d2f 626c 696e 6b31  ithub.com/blink1
+00006b20: 3037 3329 290a 2d20 436c 6561 6e20 7570  073)).- Clean up
+00006b30: 2077 6f72 6b66 6c6f 7720 616e 6420 7079   workflow and py
+00006b40: 7072 6f6a 6563 7420 5b23 3838 345d 2868  project [#884](h
+00006b50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00006b60: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+00006b70: 725f 636c 6965 6e74 2f70 756c 6c2f 3838  r_client/pull/88
+00006b80: 3429 2028 5b40 626c 696e 6b31 3037 335d  4) ([@blink1073]
+00006b90: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00006ba0: 636f 6d2f 626c 696e 6b31 3037 3329 290a  com/blink1073)).
+00006bb0: 0a23 2323 2043 6f6e 7472 6962 7574 6f72  .### Contributor
+00006bc0: 7320 746f 2074 6869 7320 7265 6c65 6173  s to this releas
+00006bd0: 650a 0a28 5b47 6974 4875 6220 636f 6e74  e..([GitHub cont
+00006be0: 7269 6275 746f 7273 2070 6167 6520 666f  ributors page fo
+00006bf0: 7220 7468 6973 2072 656c 6561 7365 5d28  r this release](
+00006c00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00006c10: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00006c20: 6572 5f63 6c69 656e 742f 6772 6170 6873  er_client/graphs
+00006c30: 2f63 6f6e 7472 6962 7574 6f72 733f 6672  /contributors?fr
+00006c40: 6f6d 3d32 3032 322d 3131 2d31 3626 746f  om=2022-11-16&to
+00006c50: 3d32 3032 322d 3131 2d32 3926 7479 7065  =2022-11-29&type
+00006c60: 3d63 2929 0a0a 5b40 6172 6f67 6f7a 686e  =c))..[@arogozhn
+00006c70: 696b 6f76 5d28 6874 7470 733a 2f2f 6769  ikov](https://gi
+00006c80: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
+00006c90: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
+00006ca0: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
+00006cb0: 742b 696e 766f 6c76 6573 2533 4161 726f  t+involves%3Aaro
+00006cc0: 676f 7a68 6e69 6b6f 762b 7570 6461 7465  gozhnikov+update
+00006cd0: 6425 3341 3230 3232 2d31 312d 3136 2e2e  d%3A2022-11-16..
+00006ce0: 3230 3232 2d31 312d 3239 2674 7970 653d  2022-11-29&type=
+00006cf0: 4973 7375 6573 2920 7c20 5b40 626c 696e  Issues) | [@blin
+00006d00: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
+00006d10: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+00006d20: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+00006d30: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+00006d40: 6e74 2b69 6e76 6f6c 7665 7325 3341 626c  nt+involves%3Abl
+00006d50: 696e 6b31 3037 332b 7570 6461 7465 6425  ink1073+updated%
+00006d60: 3341 3230 3232 2d31 312d 3136 2e2e 3230  3A2022-11-16..20
+00006d70: 3232 2d31 312d 3239 2674 7970 653d 4973  22-11-29&type=Is
+00006d80: 7375 6573 2920 7c20 5b40 6461 7669 6462  sues) | [@davidb
+00006d90: 726f 6368 6172 745d 2868 7474 7073 3a2f  rochart](https:/
+00006da0: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
+00006db0: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
+00006dc0: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
+00006dd0: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
+00006de0: 6461 7669 6462 726f 6368 6172 742b 7570  davidbrochart+up
+00006df0: 6461 7465 6425 3341 3230 3232 2d31 312d  dated%3A2022-11-
+00006e00: 3136 2e2e 3230 3232 2d31 312d 3239 2674  16..2022-11-29&t
+00006e10: 7970 653d 4973 7375 6573 2920 7c20 5b40  ype=Issues) | [@
+00006e20: 6b65 7669 6e2d 6261 7465 735d 2868 7474  kevin-bates](htt
+00006e30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00006e40: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
+00006e50: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
+00006e60: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
+00006e70: 7325 3341 6b65 7669 6e2d 6261 7465 732b  s%3Akevin-bates+
+00006e80: 7570 6461 7465 6425 3341 3230 3232 2d31  updated%3A2022-1
+00006e90: 312d 3136 2e2e 3230 3232 2d31 312d 3239  1-16..2022-11-29
+00006ea0: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
+00006eb0: 5b40 7072 652d 636f 6d6d 6974 2d63 695d  [@pre-commit-ci]
+00006ec0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00006ed0: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
+00006ee0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
+00006ef0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
+00006f00: 6f6c 7665 7325 3341 7072 652d 636f 6d6d  olves%3Apre-comm
+00006f10: 6974 2d63 692b 7570 6461 7465 6425 3341  it-ci+updated%3A
+00006f20: 3230 3232 2d31 312d 3136 2e2e 3230 3232  2022-11-16..2022
+00006f30: 2d31 312d 3239 2674 7970 653d 4973 7375  -11-29&type=Issu
+00006f40: 6573 290a 0a23 2320 382e 302e 3061 340a  es)..## 8.0.0a4.
+00006f50: 0a28 5b46 756c 6c20 4368 616e 6765 6c6f  .([Full Changelo
+00006f60: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
+00006f70: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00006f80: 7079 7465 725f 636c 6965 6e74 2f63 6f6d  pyter_client/com
+00006f90: 7061 7265 2f76 382e 302e 3061 332e 2e2e  pare/v8.0.0a3...
+00006fa0: 3130 3763 6364 6430 3663 3962 3637 6663  107ccdd06c9b67fc
+00006fb0: 3038 3132 3034 6165 3763 3065 3731 3233  081204ae7c0e7123
+00006fc0: 6131 3763 6230 6334 2929 0a0a 2323 2320  a17cb0c4))..### 
+00006fd0: 4275 6773 2066 6978 6564 0a0a 2d20 4669  Bugs fixed..- Fi
+00006fe0: 7820 636f 6e6e 6563 7469 6f6e 2072 6563  x connection rec
+00006ff0: 6f6e 6369 6c69 6174 696f 6e20 746f 2068  onciliation to h
+00007000: 616e 646c 6520 7265 7374 6172 7473 205b  andle restarts [
+00007010: 2338 3832 5d28 6874 7470 733a 2f2f 6769  #882](https://gi
+00007020: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+00007030: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+00007040: 7075 6c6c 2f38 3832 2920 285b 406b 6576  pull/882) ([@kev
+00007050: 696e 2d62 6174 6573 5d28 6874 7470 733a  in-bates](https:
+00007060: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 6576  //github.com/kev
+00007070: 696e 2d62 6174 6573 2929 0a0a 2323 2320  in-bates))..### 
+00007080: 4d61 696e 7465 6e61 6e63 6520 616e 6420  Maintenance and 
+00007090: 7570 6b65 6570 2069 6d70 726f 7665 6d65  upkeep improveme
+000070a0: 6e74 730a 0a2d 2041 6464 206d 6f72 6520  nts..- Add more 
+000070b0: 636f 7665 7261 6765 205b 2338 3737 5d28  coverage [#877](
+000070c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000070d0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+000070e0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f38  er_client/pull/8
+000070f0: 3737 2920 285b 4062 6c69 6e6b 3130 3733  77) ([@blink1073
+00007100: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00007110: 2e63 6f6d 2f62 6c69 6e6b 3130 3733 2929  .com/blink1073))
+00007120: 0a0a 2323 2320 436f 6e74 7269 6275 746f  ..### Contributo
+00007130: 7273 2074 6f20 7468 6973 2072 656c 6561  rs to this relea
+00007140: 7365 0a0a 285b 4769 7448 7562 2063 6f6e  se..([GitHub con
+00007150: 7472 6962 7574 6f72 7320 7061 6765 2066  tributors page f
+00007160: 6f72 2074 6869 7320 7265 6c65 6173 655d  or this release]
+00007170: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00007180: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00007190: 7465 725f 636c 6965 6e74 2f67 7261 7068  ter_client/graph
+000071a0: 732f 636f 6e74 7269 6275 746f 7273 3f66  s/contributors?f
+000071b0: 726f 6d3d 3230 3232 2d31 312d 3135 2674  rom=2022-11-15&t
+000071c0: 6f3d 3230 3232 2d31 312d 3136 2674 7970  o=2022-11-16&typ
+000071d0: 653d 6329 290a 0a5b 4062 6c69 6e6b 3130  e=c))..[@blink10
+000071e0: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
+000071f0: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
+00007200: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
+00007210: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
+00007220: 696e 766f 6c76 6573 2533 4162 6c69 6e6b  involves%3Ablink
+00007230: 3130 3733 2b75 7064 6174 6564 2533 4132  1073+updated%3A2
+00007240: 3032 322d 3131 2d31 352e 2e32 3032 322d  022-11-15..2022-
+00007250: 3131 2d31 3626 7479 7065 3d49 7373 7565  11-16&type=Issue
+00007260: 7329 207c 205b 406b 6576 696e 2d62 6174  s) | [@kevin-bat
+00007270: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+00007280: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
+00007290: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
+000072a0: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
+000072b0: 696e 766f 6c76 6573 2533 416b 6576 696e  involves%3Akevin
+000072c0: 2d62 6174 6573 2b75 7064 6174 6564 2533  -bates+updated%3
+000072d0: 4132 3032 322d 3131 2d31 352e 2e32 3032  A2022-11-15..202
+000072e0: 322d 3131 2d31 3626 7479 7065 3d49 7373  2-11-16&type=Iss
+000072f0: 7565 7329 0a0a 2323 2038 2e30 2e30 6133  ues)..## 8.0.0a3
+00007300: 0a0a 285b 4675 6c6c 2043 6861 6e67 656c  ..([Full Changel
+00007310: 6f67 5d28 6874 7470 733a 2f2f 6769 7468  og](https://gith
+00007320: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00007330: 7570 7974 6572 5f63 6c69 656e 742f 636f  upyter_client/co
+00007340: 6d70 6172 652f 7638 2e30 2e30 6132 2e2e  mpare/v8.0.0a2..
+00007350: 2e31 3066 3639 6339 6235 6163 3535 6239  .10f69c9b5ac55b9
+00007360: 3262 3635 3166 3166 3535 6661 3238 3134  2b651f1f55fa2814
+00007370: 6638 3166 3363 6535 3129 290a 0a23 2323  f81f3ce51))..###
+00007380: 2042 7567 7320 6669 7865 640a 0a2d 2052   Bugs fixed..- R
+00007390: 6563 6f6e 6369 6c65 2063 6f6e 6e65 6374  econcile connect
+000073a0: 696f 6e20 696e 666f 726d 6174 696f 6e20  ion information 
+000073b0: 5b23 3837 395d 2868 7474 7073 3a2f 2f67  [#879](https://g
+000073c0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+000073d0: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+000073e0: 2f70 756c 6c2f 3837 3929 2028 5b40 6b65  /pull/879) ([@ke
+000073f0: 7669 6e2d 6261 7465 735d 2868 7474 7073  vin-bates](https
+00007400: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b65  ://github.com/ke
+00007410: 7669 6e2d 6261 7465 7329 290a 0a23 2323  vin-bates))..###
+00007420: 204d 6169 6e74 656e 616e 6365 2061 6e64   Maintenance and
+00007430: 2075 706b 6565 7020 696d 7072 6f76 656d   upkeep improvem
+00007440: 656e 7473 0a0a 2d20 4164 6420 636f 7665  ents..- Add cove
+00007450: 7261 6765 2063 6f6e 6669 6720 5b23 3837  rage config [#87
+00007460: 365d 2868 7474 7073 3a2f 2f67 6974 6875  6](https://githu
+00007470: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00007480: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00007490: 6c2f 3837 3629 2028 5b40 626c 696e 6b31  l/876) ([@blink1
+000074a0: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
+000074b0: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
+000074c0: 3329 290a 2d20 4275 6d70 2061 6374 696f  3)).- Bump actio
+000074d0: 6e73 2f73 6574 7570 2d70 7974 686f 6e20  ns/setup-python 
+000074e0: 6672 6f6d 2032 2074 6f20 3420 5b23 3837  from 2 to 4 [#87
+000074f0: 345d 2868 7474 7073 3a2f 2f67 6974 6875  4](https://githu
+00007500: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00007510: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00007520: 6c2f 3837 3429 2028 5b40 6465 7065 6e64  l/874) ([@depend
+00007530: 6162 6f74 5d28 6874 7470 733a 2f2f 6769  abot](https://gi
+00007540: 7468 7562 2e63 6f6d 2f64 6570 656e 6461  thub.com/dependa
+00007550: 626f 7429 290a 2d20 4275 6d70 2061 6374  bot)).- Bump act
+00007560: 696f 6e73 2f63 6865 636b 6f75 7420 6672  ions/checkout fr
+00007570: 6f6d 2032 2074 6f20 3320 5b23 3837 335d  om 2 to 3 [#873]
+00007580: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00007590: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+000075a0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+000075b0: 3837 3329 2028 5b40 6465 7065 6e64 6162  873) ([@dependab
+000075c0: 6f74 5d28 6874 7470 733a 2f2f 6769 7468  ot](https://gith
+000075d0: 7562 2e63 6f6d 2f64 6570 656e 6461 626f  ub.com/dependabo
+000075e0: 7429 290a 2d20 436c 6561 6e20 7570 2074  t)).- Clean up t
+000075f0: 7970 6573 2061 6e64 2072 656d 6f76 6520  ypes and remove 
+00007600: 7573 6520 6f66 2065 6e74 7279 706f 696e  use of entrypoin
+00007610: 7473 205b 2338 3731 5d28 6874 7470 733a  ts [#871](https:
+00007620: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+00007630: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+00007640: 656e 742f 7075 6c6c 2f38 3731 2920 285b  ent/pull/871) ([
+00007650: 4062 6c69 6e6b 3130 3733 5d28 6874 7470  @blink1073](http
+00007660: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
+00007670: 6c69 6e6b 3130 3733 2929 0a2d 2041 6464  link1073)).- Add
+00007680: 2064 6570 656e 6461 626f 7420 5b23 3837   dependabot [#87
+00007690: 305d 2868 7474 7073 3a2f 2f67 6974 6875  0](https://githu
+000076a0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+000076b0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+000076c0: 6c2f 3837 3029 2028 5b40 626c 696e 6b31  l/870) ([@blink1
+000076d0: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
+000076e0: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
+000076f0: 3329 290a 0a23 2323 2043 6f6e 7472 6962  3))..### Contrib
+00007700: 7574 6f72 7320 746f 2074 6869 7320 7265  utors to this re
+00007710: 6c65 6173 650a 0a28 5b47 6974 4875 6220  lease..([GitHub 
+00007720: 636f 6e74 7269 6275 746f 7273 2070 6167  contributors pag
+00007730: 6520 666f 7220 7468 6973 2072 656c 6561  e for this relea
+00007740: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
+00007750: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00007760: 7570 7974 6572 5f63 6c69 656e 742f 6772  upyter_client/gr
+00007770: 6170 6873 2f63 6f6e 7472 6962 7574 6f72  aphs/contributor
+00007780: 733f 6672 6f6d 3d32 3032 322d 3131 2d30  s?from=2022-11-0
+00007790: 3926 746f 3d32 3032 322d 3131 2d31 3526  9&to=2022-11-15&
+000077a0: 7479 7065 3d63 2929 0a0a 5b40 626c 696e  type=c))..[@blin
+000077b0: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
+000077c0: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+000077d0: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+000077e0: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+000077f0: 6e74 2b69 6e76 6f6c 7665 7325 3341 626c  nt+involves%3Abl
+00007800: 696e 6b31 3037 332b 7570 6461 7465 6425  ink1073+updated%
+00007810: 3341 3230 3232 2d31 312d 3039 2e2e 3230  3A2022-11-09..20
+00007820: 3232 2d31 312d 3135 2674 7970 653d 4973  22-11-15&type=Is
+00007830: 7375 6573 2920 7c20 5b40 6465 7065 6e64  sues) | [@depend
+00007840: 6162 6f74 5d28 6874 7470 733a 2f2f 6769  abot](https://gi
+00007850: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
+00007860: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
+00007870: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
+00007880: 742b 696e 766f 6c76 6573 2533 4164 6570  t+involves%3Adep
+00007890: 656e 6461 626f 742b 7570 6461 7465 6425  endabot+updated%
+000078a0: 3341 3230 3232 2d31 312d 3039 2e2e 3230  3A2022-11-09..20
+000078b0: 3232 2d31 312d 3135 2674 7970 653d 4973  22-11-15&type=Is
+000078c0: 7375 6573 2920 7c20 5b40 6b65 7669 6e2d  sues) | [@kevin-
+000078d0: 6261 7465 735d 2868 7474 7073 3a2f 2f67  bates](https://g
+000078e0: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+000078f0: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+00007900: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+00007910: 6e74 2b69 6e76 6f6c 7665 7325 3341 6b65  nt+involves%3Ake
+00007920: 7669 6e2d 6261 7465 732b 7570 6461 7465  vin-bates+update
+00007930: 6425 3341 3230 3232 2d31 312d 3039 2e2e  d%3A2022-11-09..
+00007940: 3230 3232 2d31 312d 3135 2674 7970 653d  2022-11-15&type=
+00007950: 4973 7375 6573 2920 7c20 5b40 7072 652d  Issues) | [@pre-
+00007960: 636f 6d6d 6974 2d63 695d 2868 7474 7073  commit-ci](https
+00007970: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
+00007980: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
+00007990: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
+000079a0: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
+000079b0: 3341 7072 652d 636f 6d6d 6974 2d63 692b  3Apre-commit-ci+
+000079c0: 7570 6461 7465 6425 3341 3230 3232 2d31  updated%3A2022-1
+000079d0: 312d 3039 2e2e 3230 3232 2d31 312d 3135  1-09..2022-11-15
+000079e0: 2674 7970 653d 4973 7375 6573 290a 0a23  &type=Issues)..#
+000079f0: 2320 382e 302e 3061 320a 0a28 5b46 756c  # 8.0.0a2..([Ful
+00007a00: 6c20 4368 616e 6765 6c6f 675d 2868 7474  l Changelog](htt
+00007a10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00007a20: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00007a30: 636c 6965 6e74 2f63 6f6d 7061 7265 2f76  client/compare/v
+00007a40: 382e 302e 3061 312e 2e2e 3236 3861 3363  8.0.0a1...268a3c
+00007a50: 3563 3839 3265 3365 3432 6537 3663 3565  5c892e3e42e76c5e
+00007a60: 6331 3230 6137 3464 6531 3066 6230 3432  c120a74de10fb042
+00007a70: 3138 2929 0a0a 2323 2320 4d61 696e 7465  18))..### Mainte
+00007a80: 6e61 6e63 6520 616e 6420 7570 6b65 6570  nance and upkeep
+00007a90: 2069 6d70 726f 7665 6d65 6e74 730a 0a2d   improvements..-
+00007aa0: 2055 7365 2070 6c61 7466 6f72 6d20 6469   Use platform di
+00007ab0: 7273 2069 6e20 7465 7374 7320 5b23 3837  rs in tests [#87
+00007ac0: 325d 2868 7474 7073 3a2f 2f67 6974 6875  2](https://githu
+00007ad0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00007ae0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00007af0: 6c2f 3837 3229 2028 5b40 626c 696e 6b31  l/872) ([@blink1
+00007b00: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
+00007b10: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
+00007b20: 3329 290a 2d20 5375 7070 6f72 7420 5079  3)).- Support Py
+00007b30: 7468 6f6e 2033 2e38 2d33 2e31 3120 5b23  thon 3.8-3.11 [#
+00007b40: 3836 365d 2868 7474 7073 3a2f 2f67 6974  866](https://git
+00007b50: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00007b60: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+00007b70: 756c 6c2f 3836 3629 2028 5b40 626c 696e  ull/866) ([@blin
+00007b80: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
+00007b90: 6974 6875 622e 636f 6d2f 626c 696e 6b31  ithub.com/blink1
+00007ba0: 3037 3329 290a 0a23 2323 2043 6f6e 7472  073))..### Contr
+00007bb0: 6962 7574 6f72 7320 746f 2074 6869 7320  ibutors to this 
+00007bc0: 7265 6c65 6173 650a 0a28 5b47 6974 4875  release..([GitHu
+00007bd0: 6220 636f 6e74 7269 6275 746f 7273 2070  b contributors p
+00007be0: 6167 6520 666f 7220 7468 6973 2072 656c  age for this rel
+00007bf0: 6561 7365 5d28 6874 7470 733a 2f2f 6769  ease](https://gi
+00007c00: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+00007c10: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+00007c20: 6772 6170 6873 2f63 6f6e 7472 6962 7574  graphs/contribut
+00007c30: 6f72 733f 6672 6f6d 3d32 3032 322d 3130  ors?from=2022-10
+00007c40: 2d32 3526 746f 3d32 3032 322d 3131 2d30  -25&to=2022-11-0
+00007c50: 3926 7479 7065 3d63 2929 0a0a 5b40 626c  9&type=c))..[@bl
+00007c60: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
+00007c70: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
+00007c80: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
+00007c90: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
+00007ca0: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
+00007cb0: 626c 696e 6b31 3037 332b 7570 6461 7465  blink1073+update
+00007cc0: 6425 3341 3230 3232 2d31 302d 3235 2e2e  d%3A2022-10-25..
+00007cd0: 3230 3232 2d31 312d 3039 2674 7970 653d  2022-11-09&type=
+00007ce0: 4973 7375 6573 2920 7c20 5b40 7072 652d  Issues) | [@pre-
+00007cf0: 636f 6d6d 6974 2d63 695d 2868 7474 7073  commit-ci](https
+00007d00: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
+00007d10: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
+00007d20: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
+00007d30: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
+00007d40: 3341 7072 652d 636f 6d6d 6974 2d63 692b  3Apre-commit-ci+
+00007d50: 7570 6461 7465 6425 3341 3230 3232 2d31  updated%3A2022-1
+00007d60: 302d 3235 2e2e 3230 3232 2d31 312d 3039  0-25..2022-11-09
+00007d70: 2674 7970 653d 4973 7375 6573 290a 0a23  &type=Issues)..#
+00007d80: 2320 382e 302e 3061 310a 0a28 5b46 756c  # 8.0.0a1..([Ful
+00007d90: 6c20 4368 616e 6765 6c6f 675d 2868 7474  l Changelog](htt
+00007da0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00007db0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00007dc0: 636c 6965 6e74 2f63 6f6d 7061 7265 2f76  client/compare/v
+00007dd0: 382e 302e 3061 302e 2e2e 3335 6236 3664  8.0.0a0...35b66d
+00007de0: 3861 3733 3862 3663 3936 3239 6666 6561  8a738b6c9629ffea
+00007df0: 6433 3038 6339 6639 3831 6265 6531 3134  d308c9f981bee114
+00007e00: 3866 2929 0a0a 2323 2320 4275 6773 2066  8f))..### Bugs f
+00007e10: 6978 6564 0a0a 2d20 576f 726b 6172 6f75  ixed..- Workarou
+00007e20: 6e64 2066 6f72 206c 6175 6e63 6820 6275  nd for launch bu
+00007e30: 6720 5b23 3836 315d 2868 7474 7073 3a2f  g [#861](https:/
+00007e40: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00007e50: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00007e60: 6e74 2f70 756c 6c2f 3836 3129 2028 5b40  nt/pull/861) ([@
+00007e70: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
+00007e80: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
+00007e90: 696e 6b31 3037 3329 290a 2d20 4465 6665  ink1073)).- Defe
+00007ea0: 7220 6372 6561 7469 6f6e 206f 6620 7265  r creation of re
+00007eb0: 6164 7920 6675 7475 7265 205b 2338 3538  ady future [#858
+00007ec0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00007ed0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00007ee0: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00007ef0: 2f38 3538 2920 285b 4062 6c69 6e6b 3130  /858) ([@blink10
+00007f00: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
+00007f10: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
+00007f20: 2929 0a0a 2323 2320 4d61 696e 7465 6e61  ))..### Maintena
+00007f30: 6e63 6520 616e 6420 7570 6b65 6570 2069  nce and upkeep i
+00007f40: 6d70 726f 7665 6d65 6e74 730a 0a2d 2046  mprovements..- F
+00007f50: 6978 2061 7373 6572 7469 6f6e 2069 6e20  ix assertion in 
+00007f60: 6054 6573 7453 6573 7369 6f6e 2e74 6573  `TestSession.tes
+00007f70: 745f 7365 7269 616c 697a 6560 205b 2338  t_serialize` [#8
+00007f80: 3630 5d28 6874 7470 733a 2f2f 6769 7468  60](https://gith
+00007f90: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00007fa0: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+00007fb0: 6c6c 2f38 3630 2920 285b 4073 616d 7261  ll/860) ([@samra
+00007fc0: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00007fd0: 622e 636f 6d2f 7361 6d72 6174 2929 0a2d  b.com/samrat)).-
+00007fe0: 204d 6169 6e74 656e 616e 6365 2063 6c65   Maintenance cle
+00007ff0: 616e 7570 205b 2338 3536 5d28 6874 7470  anup [#856](http
+00008000: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00008010: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
+00008020: 6c69 656e 742f 7075 6c6c 2f38 3536 2920  lient/pull/856) 
+00008030: 285b 4062 6c69 6e6b 3130 3733 5d28 6874  ([@blink1073](ht
+00008040: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00008050: 2f62 6c69 6e6b 3130 3733 2929 0a0a 2323  /blink1073))..##
+00008060: 2320 436f 6e74 7269 6275 746f 7273 2074  # Contributors t
+00008070: 6f20 7468 6973 2072 656c 6561 7365 0a0a  o this release..
+00008080: 285b 4769 7448 7562 2063 6f6e 7472 6962  ([GitHub contrib
+00008090: 7574 6f72 7320 7061 6765 2066 6f72 2074  utors page for t
+000080a0: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
+000080b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000080c0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+000080d0: 636c 6965 6e74 2f67 7261 7068 732f 636f  client/graphs/co
+000080e0: 6e74 7269 6275 746f 7273 3f66 726f 6d3d  ntributors?from=
+000080f0: 3230 3232 2d31 302d 3132 2674 6f3d 3230  2022-10-12&to=20
+00008100: 3232 2d31 302d 3235 2674 7970 653d 6329  22-10-25&type=c)
+00008110: 290a 0a5b 4062 6c69 6e6b 3130 3733 5d28  )..[@blink1073](
+00008120: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00008130: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
+00008140: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
+00008150: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
+00008160: 6c76 6573 2533 4162 6c69 6e6b 3130 3733  lves%3Ablink1073
+00008170: 2b75 7064 6174 6564 2533 4132 3032 322d  +updated%3A2022-
+00008180: 3130 2d31 322e 2e32 3032 322d 3130 2d32  10-12..2022-10-2
+00008190: 3526 7479 7065 3d49 7373 7565 7329 207c  5&type=Issues) |
+000081a0: 205b 4070 7265 2d63 6f6d 6d69 742d 6369   [@pre-commit-ci
+000081b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000081c0: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
+000081d0: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
+000081e0: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
+000081f0: 766f 6c76 6573 2533 4170 7265 2d63 6f6d  volves%3Apre-com
+00008200: 6d69 742d 6369 2b75 7064 6174 6564 2533  mit-ci+updated%3
+00008210: 4132 3032 322d 3130 2d31 322e 2e32 3032  A2022-10-12..202
+00008220: 322d 3130 2d32 3526 7479 7065 3d49 7373  2-10-25&type=Iss
+00008230: 7565 7329 207c 205b 4073 616d 7261 745d  ues) | [@samrat]
+00008240: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00008250: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
+00008260: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
+00008270: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
+00008280: 6f6c 7665 7325 3341 7361 6d72 6174 2b75  olves%3Asamrat+u
+00008290: 7064 6174 6564 2533 4132 3032 322d 3130  pdated%3A2022-10
+000082a0: 2d31 322e 2e32 3032 322d 3130 2d32 3526  -12..2022-10-25&
+000082b0: 7479 7065 3d49 7373 7565 7329 0a0a 2323  type=Issues)..##
+000082c0: 2038 2e30 2e30 6130 0a0a 285b 4675 6c6c   8.0.0a0..([Full
+000082d0: 2043 6861 6e67 656c 6f67 5d28 6874 7470   Changelog](http
+000082e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+000082f0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
+00008300: 6c69 656e 742f 636f 6d70 6172 652f 7637  lient/compare/v7
+00008310: 2e33 2e35 2e2e 2e30 3665 3963 6233 6662  .3.5...06e9cb3fb
+00008320: 3239 6138 3935 6133 6131 3465 3665 3339  29a895a3a14e6e39
+00008330: 6162 3532 3461 3133 6265 6338 3565 6329  ab524a13bec85ec)
+00008340: 290a 0a23 2323 2045 6e68 616e 6365 6d65  )..### Enhanceme
+00008350: 6e74 7320 6d61 6465 0a0a 2d20 5265 6d6f  nts made..- Remo
+00008360: 7665 206e 6573 742d 6173 796e 6369 6f20  ve nest-asyncio 
+00008370: 6465 7065 6e64 656e 6379 205b 2338 3335  dependency [#835
+00008380: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00008390: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+000083a0: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+000083b0: 2f38 3335 2920 285b 4062 6c69 6e6b 3130  /835) ([@blink10
+000083c0: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
+000083d0: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
+000083e0: 2929 0a0a 2323 2320 4275 6773 2066 6978  ))..### Bugs fix
+000083f0: 6564 0a0a 2d20 4669 7820 6861 6e64 6c69  ed..- Fix handli
+00008400: 6e67 206f 6620 696e 6974 6961 6c20 7265  ng of initial re
+00008410: 6164 7920 7072 6f6d 6973 6520 5b23 3835  ady promise [#85
+00008420: 345d 2868 7474 7073 3a2f 2f67 6974 6875  4](https://githu
+00008430: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00008440: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00008450: 6c2f 3835 3429 2028 5b40 626c 696e 6b31  l/854) ([@blink1
+00008460: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
+00008470: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
+00008480: 3329 290a 2d20 5573 6520 7079 7465 7374  3)).- Use pytest
+00008490: 5f61 7379 6e63 696f 2066 6978 7475 7265  _asyncio fixture
+000084a0: 205b 2338 3236 5d28 6874 7470 733a 2f2f   [#826](https://
+000084b0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+000084c0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+000084d0: 742f 7075 6c6c 2f38 3236 2920 285b 4064  t/pull/826) ([@d
+000084e0: 6176 6964 6272 6f63 6861 7274 5d28 6874  avidbrochart](ht
+000084f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00008500: 2f64 6176 6964 6272 6f63 6861 7274 2929  /davidbrochart))
+00008510: 0a0a 2323 2320 4d61 696e 7465 6e61 6e63  ..### Maintenanc
+00008520: 6520 616e 6420 7570 6b65 6570 2069 6d70  e and upkeep imp
+00008530: 726f 7665 6d65 6e74 730a 0a2d 2049 676e  rovements..- Ign
+00008540: 6f72 6520 7761 726e 696e 6773 2069 6e20  ore warnings in 
+00008550: 7072 6572 656c 6561 7365 7320 7465 7374  prereleases test
+00008560: 205b 2338 3434 5d28 6874 7470 733a 2f2f   [#844](https://
+00008570: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00008580: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00008590: 742f 7075 6c6c 2f38 3434 2920 285b 4062  t/pull/844) ([@b
+000085a0: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
+000085b0: 2f2f 6769 7468 7562 2e63 6f6d 2f62 6c69  //github.com/bli
+000085c0: 6e6b 3130 3733 2929 0a2d 2055 7365 2068  nk1073)).- Use h
+000085d0: 6174 6368 2066 6f72 2076 6572 7369 6f6e  atch for version
+000085e0: 205b 2338 3337 5d28 6874 7470 733a 2f2f   [#837](https://
+000085f0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00008600: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00008610: 742f 7075 6c6c 2f38 3337 2920 285b 4062  t/pull/837) ([@b
+00008620: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
+00008630: 2f2f 6769 7468 7562 2e63 6f6d 2f62 6c69  //github.com/bli
+00008640: 6e6b 3130 3733 2929 0a2d 204d 6f76 6520  nk1073)).- Move 
+00008650: 7465 7374 7320 746f 2074 6f70 206c 6576  tests to top lev
+00008660: 656c 205b 2338 3334 5d28 6874 7470 733a  el [#834](https:
+00008670: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+00008680: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+00008690: 656e 742f 7075 6c6c 2f38 3334 2920 285b  ent/pull/834) ([
+000086a0: 4062 6c69 6e6b 3130 3733 5d28 6874 7470  @blink1073](http
+000086b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
+000086c0: 6c69 6e6b 3130 3733 2929 0a2d 2046 6978  link1073)).- Fix
+000086d0: 206e 6263 6f6e 7665 7274 2064 6f77 6e73   nbconvert downs
+000086e0: 7472 6561 6d20 7465 7374 205b 2338 3237  tream test [#827
+000086f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00008700: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00008710: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00008720: 2f38 3237 2920 285b 4062 6c69 6e6b 3130  /827) ([@blink10
+00008730: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
+00008740: 7562 2e63 6f6d 2f62 6c69 6e6b 3130 3733  ub.com/blink1073
+00008750: 2929 0a0a 2323 2320 446f 6375 6d65 6e74  ))..### Document
+00008760: 6174 696f 6e20 696d 7072 6f76 656d 656e  ation improvemen
+00008770: 7473 0a0a 2d20 5377 6974 6368 2074 6f20  ts..- Switch to 
+00008780: 7079 6461 7461 2073 7068 696e 7820 7468  pydata sphinx th
+00008790: 656d 6520 5b23 3834 305d 2868 7474 7073  eme [#840](https
+000087a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+000087b0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+000087c0: 6965 6e74 2f70 756c 6c2f 3834 3029 2028  ient/pull/840) (
+000087d0: 5b40 626c 696e 6b31 3037 335d 2868 7474  [@blink1073](htt
+000087e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000087f0: 626c 696e 6b31 3037 3329 290a 0a23 2323  blink1073))..###
+00008800: 2043 6f6e 7472 6962 7574 6f72 7320 746f   Contributors to
+00008810: 2074 6869 7320 7265 6c65 6173 650a 0a28   this release..(
+00008820: 5b47 6974 4875 6220 636f 6e74 7269 6275  [GitHub contribu
+00008830: 746f 7273 2070 6167 6520 666f 7220 7468  tors page for th
+00008840: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
+00008850: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00008860: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
+00008870: 6c69 656e 742f 6772 6170 6873 2f63 6f6e  lient/graphs/con
+00008880: 7472 6962 7574 6f72 733f 6672 6f6d 3d32  tributors?from=2
+00008890: 3032 322d 3038 2d32 3526 746f 3d32 3032  022-08-25&to=202
+000088a0: 322d 3130 2d31 3226 7479 7065 3d63 2929  2-10-12&type=c))
+000088b0: 0a0a 5b40 626c 696e 6b31 3037 335d 2868  ..[@blink1073](h
+000088c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000088d0: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
+000088e0: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
+000088f0: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
+00008900: 7665 7325 3341 626c 696e 6b31 3037 332b  ves%3Ablink1073+
+00008910: 7570 6461 7465 6425 3341 3230 3232 2d30  updated%3A2022-0
+00008920: 382d 3235 2e2e 3230 3232 2d31 302d 3132  8-25..2022-10-12
+00008930: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
+00008940: 5b40 6363 6f72 646f 6261 3132 5d28 6874  [@ccordoba12](ht
+00008950: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00008960: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+00008970: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+00008980: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+00008990: 6573 2533 4163 636f 7264 6f62 6131 322b  es%3Accordoba12+
+000089a0: 7570 6461 7465 6425 3341 3230 3232 2d30  updated%3A2022-0
+000089b0: 382d 3235 2e2e 3230 3232 2d31 302d 3132  8-25..2022-10-12
+000089c0: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
+000089d0: 5b40 6461 7669 6462 726f 6368 6172 745d  [@davidbrochart]
+000089e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000089f0: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
+00008a00: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
+00008a10: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
+00008a20: 6f6c 7665 7325 3341 6461 7669 6462 726f  olves%3Adavidbro
+00008a30: 6368 6172 742b 7570 6461 7465 6425 3341  chart+updated%3A
+00008a40: 3230 3232 2d30 382d 3235 2e2e 3230 3232  2022-08-25..2022
+00008a50: 2d31 302d 3132 2674 7970 653d 4973 7375  -10-12&type=Issu
+00008a60: 6573 2920 7c20 5b40 6d69 6e72 6b5d 2868  es) | [@minrk](h
+00008a70: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00008a80: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
+00008a90: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
+00008aa0: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
+00008ab0: 7665 7325 3341 6d69 6e72 6b2b 7570 6461  ves%3Aminrk+upda
+00008ac0: 7465 6425 3341 3230 3232 2d30 382d 3235  ted%3A2022-08-25
+00008ad0: 2e2e 3230 3232 2d31 302d 3132 2674 7970  ..2022-10-12&typ
+00008ae0: 653d 4973 7375 6573 2920 7c20 5b40 7072  e=Issues) | [@pr
+00008af0: 652d 636f 6d6d 6974 2d63 695d 2868 7474  e-commit-ci](htt
+00008b00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00008b10: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
+00008b20: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
+00008b30: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
+00008b40: 7325 3341 7072 652d 636f 6d6d 6974 2d63  s%3Apre-commit-c
+00008b50: 692b 7570 6461 7465 6425 3341 3230 3232  i+updated%3A2022
+00008b60: 2d30 382d 3235 2e2e 3230 3232 2d31 302d  -08-25..2022-10-
+00008b70: 3132 2674 7970 653d 4973 7375 6573 2920  12&type=Issues) 
+00008b80: 7c20 5b40 5a73 6169 6c65 725d 2868 7474  | [@Zsailer](htt
+00008b90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00008ba0: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
+00008bb0: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
+00008bc0: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
+00008bd0: 7325 3341 5a73 6169 6c65 722b 7570 6461  s%3AZsailer+upda
+00008be0: 7465 6425 3341 3230 3232 2d30 382d 3235  ted%3A2022-08-25
+00008bf0: 2e2e 3230 3232 2d31 302d 3132 2674 7970  ..2022-10-12&typ
+00008c00: 653d 4973 7375 6573 290a 0a23 2320 372e  e=Issues)..## 7.
+00008c10: 332e 350a 0a28 5b46 756c 6c20 4368 616e  3.5..([Full Chan
+00008c20: 6765 6c6f 675d 2868 7474 7073 3a2f 2f67  gelog](https://g
+00008c30: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00008c40: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00008c50: 2f63 6f6d 7061 7265 2f76 372e 332e 342e  /compare/v7.3.4.
+00008c60: 2e2e 6263 3564 6564 3534 3339 6361 3535  ..bc5ded5439ca55
+00008c70: 6264 3637 3430 3838 3565 6233 6134 3463  bd6740885eb3a44c
+00008c80: 6136 6263 3365 3232 3433 2929 0a0a 2323  a6bc3e2243))..##
+00008c90: 2320 456e 6861 6e63 656d 656e 7473 206d  # Enhancements m
+00008ca0: 6164 650a 0a2d 2061 6464 2060 4173 796e  ade..- add `Asyn
+00008cb0: 634b 6572 6e65 6c43 6c69 656e 7460 2074  cKernelClient` t
+00008cc0: 6f20 6064 6f63 2f61 7069 2f63 6c69 656e  o `doc/api/clien
+00008cd0: 742e 7273 7460 205b 2338 3139 5d28 6874  t.rst` [#819](ht
+00008ce0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00008cf0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+00008d00: 5f63 6c69 656e 742f 7075 6c6c 2f38 3139  _client/pull/819
+00008d10: 2920 285b 4068 656c 696f 7a31 315d 2868  ) ([@helioz11](h
+00008d20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00008d30: 6d2f 6865 6c69 6f7a 3131 2929 0a0a 2323  m/helioz11))..##
+00008d40: 2320 4275 6773 2066 6978 6564 0a0a 2d20  # Bugs fixed..- 
+00008d50: 5573 6520 746f 726e 6164 6f20 362e 3227  Use tornado 6.2'
+00008d60: 7320 5065 7269 6f64 6963 4361 6c6c 6261  s PeriodicCallba
+00008d70: 636b 2069 6e20 7265 7374 6172 7465 7220  ck in restarter 
+00008d80: 5b23 3832 325d 2868 7474 7073 3a2f 2f67  [#822](https://g
+00008d90: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00008da0: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00008db0: 2f70 756c 6c2f 3832 3229 2028 5b40 7669  /pull/822) ([@vi
+00008dc0: 6461 7274 665d 2868 7474 7073 3a2f 2f67  dartf](https://g
+00008dd0: 6974 6875 622e 636f 6d2f 7669 6461 7274  ithub.com/vidart
+00008de0: 6629 290a 2d20 4d61 6b65 205c 5f73 7464  f)).- Make \_std
+00008df0: 696e 5f68 6f6f 6b5f 6465 6661 756c 7420  in_hook_default 
+00008e00: 6173 796e 6320 5b23 3831 345d 2868 7474  async [#814](htt
+00008e10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00008e20: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00008e30: 636c 6965 6e74 2f70 756c 6c2f 3831 3429  client/pull/814)
+00008e40: 2028 5b40 6461 7669 6462 726f 6368 6172   ([@davidbrochar
+00008e50: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00008e60: 622e 636f 6d2f 6461 7669 6462 726f 6368  b.com/davidbroch
+00008e70: 6172 7429 290a 0a23 2323 204d 6169 6e74  art))..### Maint
+00008e80: 656e 616e 6365 2061 6e64 2075 706b 6565  enance and upkee
+00008e90: 7020 696d 7072 6f76 656d 656e 7473 0a0a  p improvements..
+00008ea0: 2d20 5c5b 7072 652d 636f 6d6d 6974 2e63  - \[pre-commit.c
+00008eb0: 695c 5d20 7072 652d 636f 6d6d 6974 2061  i\] pre-commit a
+00008ec0: 7574 6f75 7064 6174 6520 5b23 3832 345d  utoupdate [#824]
+00008ed0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00008ee0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00008ef0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00008f00: 3832 3429 2028 5b40 7072 652d 636f 6d6d  824) ([@pre-comm
+00008f10: 6974 2d63 695d 2868 7474 7073 3a2f 2f67  it-ci](https://g
+00008f20: 6974 6875 622e 636f 6d2f 7072 652d 636f  ithub.com/pre-co
+00008f30: 6d6d 6974 2d63 6929 290a 2d20 5c5b 7072  mmit-ci)).- \[pr
+00008f40: 652d 636f 6d6d 6974 2e63 695c 5d20 7072  e-commit.ci\] pr
+00008f50: 652d 636f 6d6d 6974 2061 7574 6f75 7064  e-commit autoupd
+00008f60: 6174 6520 5b23 3832 315d 2868 7474 7073  ate [#821](https
+00008f70: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00008f80: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+00008f90: 6965 6e74 2f70 756c 6c2f 3832 3129 2028  ient/pull/821) (
+00008fa0: 5b40 7072 652d 636f 6d6d 6974 2d63 695d  [@pre-commit-ci]
+00008fb0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00008fc0: 636f 6d2f 7072 652d 636f 6d6d 6974 2d63  com/pre-commit-c
+00008fd0: 6929 290a 2d20 5c5b 7072 652d 636f 6d6d  i)).- \[pre-comm
+00008fe0: 6974 2e63 695c 5d20 7072 652d 636f 6d6d  it.ci\] pre-comm
+00008ff0: 6974 2061 7574 6f75 7064 6174 6520 5b23  it autoupdate [#
+00009000: 3832 305d 2868 7474 7073 3a2f 2f67 6974  820](https://git
+00009010: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00009020: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+00009030: 756c 6c2f 3832 3029 2028 5b40 7072 652d  ull/820) ([@pre-
+00009040: 636f 6d6d 6974 2d63 695d 2868 7474 7073  commit-ci](https
+00009050: 3a2f 2f67 6974 6875 622e 636f 6d2f 7072  ://github.com/pr
+00009060: 652d 636f 6d6d 6974 2d63 6929 290a 2d20  e-commit-ci)).- 
+00009070: 5c5b 7072 652d 636f 6d6d 6974 2e63 695c  \[pre-commit.ci\
+00009080: 5d20 7072 652d 636f 6d6d 6974 2061 7574  ] pre-commit aut
+00009090: 6f75 7064 6174 6520 5b23 3831 385d 2868  oupdate [#818](h
+000090a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000090b0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+000090c0: 725f 636c 6965 6e74 2f70 756c 6c2f 3831  r_client/pull/81
+000090d0: 3829 2028 5b40 7072 652d 636f 6d6d 6974  8) ([@pre-commit
+000090e0: 2d63 695d 2868 7474 7073 3a2f 2f67 6974  -ci](https://git
+000090f0: 6875 622e 636f 6d2f 7072 652d 636f 6d6d  hub.com/pre-comm
+00009100: 6974 2d63 6929 290a 2d20 5c5b 7072 652d  it-ci)).- \[pre-
+00009110: 636f 6d6d 6974 2e63 695c 5d20 7072 652d  commit.ci\] pre-
+00009120: 636f 6d6d 6974 2061 7574 6f75 7064 6174  commit autoupdat
+00009130: 6520 5b23 3831 365d 2868 7474 7073 3a2f  e [#816](https:/
 00009140: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
 00009150: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-00009160: 6e74 2f67 7261 7068 732f 636f 6e74 7269  nt/graphs/contri
-00009170: 6275 746f 7273 3f66 726f 6d3d 3230 3232  butors?from=2022
-00009180: 2d30 362d 3037 2674 6f3d 3230 3232 2d30  -06-07&to=2022-0
-00009190: 362d 3038 2674 7970 653d 6329 290a 0a5b  6-08&type=c))..[
-000091a0: 4062 6c69 6e6b 3130 3733 5d28 6874 7470  @blink1073](http
-000091b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-000091c0: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
-000091d0: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
-000091e0: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
-000091f0: 2533 4162 6c69 6e6b 3130 3733 2b75 7064  %3Ablink1073+upd
-00009200: 6174 6564 2533 4132 3032 322d 3036 2d30  ated%3A2022-06-0
-00009210: 372e 2e32 3032 322d 3036 2d30 3826 7479  7..2022-06-08&ty
-00009220: 7065 3d49 7373 7565 7329 207c 205b 4063  pe=Issues) | [@c
-00009230: 636f 7264 6f62 6131 325d 2868 7474 7073  cordoba12](https
-00009240: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
-00009250: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
-00009260: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
-00009270: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
-00009280: 3341 6363 6f72 646f 6261 3132 2b75 7064  3Accordoba12+upd
-00009290: 6174 6564 2533 4132 3032 322d 3036 2d30  ated%3A2022-06-0
-000092a0: 372e 2e32 3032 322d 3036 2d30 3826 7479  7..2022-06-08&ty
-000092b0: 7065 3d49 7373 7565 7329 207c 205b 4070  pe=Issues) | [@p
-000092c0: 7265 2d63 6f6d 6d69 742d 6369 5d28 6874  re-commit-ci](ht
-000092d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000092e0: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
-000092f0: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
-00009300: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
-00009310: 6573 2533 4170 7265 2d63 6f6d 6d69 742d  es%3Apre-commit-
-00009320: 6369 2b75 7064 6174 6564 2533 4132 3032  ci+updated%3A202
-00009330: 322d 3036 2d30 372e 2e32 3032 322d 3036  2-06-07..2022-06
-00009340: 2d30 3826 7479 7065 3d49 7373 7565 7329  -08&type=Issues)
-00009350: 0a0a 2323 2037 2e33 2e33 0a0a 285b 4675  ..## 7.3.3..([Fu
-00009360: 6c6c 2043 6861 6e67 656c 6f67 5d28 6874  ll Changelog](ht
-00009370: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00009380: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00009390: 5f63 6c69 656e 742f 636f 6d70 6172 652f  _client/compare/
-000093a0: 7637 2e33 2e32 2e2e 2e33 3763 6133 3764  v7.3.2...37ca37d
-000093b0: 3836 3564 6232 3630 6537 6461 3666 6138  865db260e7da6fa8
-000093c0: 3533 3339 6265 3435 3064 3666 6433 6333  5339be450d6fd3c3
-000093d0: 6329 290a 0a23 2323 2042 7567 7320 6669  c))..### Bugs fi
-000093e0: 7865 640a 0a2d 2041 6464 206c 6f63 616c  xed..- Add local
-000093f0: 2d70 726f 7669 7369 6f6e 6572 2065 6e74  -provisioner ent
-00009400: 7279 2070 6f69 6e74 2074 6f20 7079 7072  ry point to pypr
-00009410: 6f6a 6563 742e 746f 6d6c 2046 6978 6573  oject.toml Fixes
-00009420: 2023 3830 3020 5b23 3830 315d 2868 7474   #800 [#801](htt
-00009430: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00009440: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00009450: 636c 6965 6e74 2f70 756c 6c2f 3830 3129  client/pull/801)
-00009460: 2028 5b40 7574 6b6f 6e6f 735d 2868 7474   ([@utkonos](htt
-00009470: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00009480: 7574 6b6f 6e6f 7329 290a 0a23 2323 2043  utkonos))..### C
-00009490: 6f6e 7472 6962 7574 6f72 7320 746f 2074  ontributors to t
-000094a0: 6869 7320 7265 6c65 6173 650a 0a28 5b47  his release..([G
-000094b0: 6974 4875 6220 636f 6e74 7269 6275 746f  itHub contributo
-000094c0: 7273 2070 6167 6520 666f 7220 7468 6973  rs page for this
-000094d0: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
-000094e0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-000094f0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-00009500: 656e 742f 6772 6170 6873 2f63 6f6e 7472  ent/graphs/contr
-00009510: 6962 7574 6f72 733f 6672 6f6d 3d32 3032  ibutors?from=202
-00009520: 322d 3036 2d30 3626 746f 3d32 3032 322d  2-06-06&to=2022-
-00009530: 3036 2d30 3726 7479 7065 3d63 2929 0a0a  06-07&type=c))..
-00009540: 5b40 7574 6b6f 6e6f 735d 2868 7474 7073  [@utkonos](https
-00009550: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
-00009560: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
-00009570: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
-00009580: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
-00009590: 3341 7574 6b6f 6e6f 732b 7570 6461 7465  3Autkonos+update
-000095a0: 6425 3341 3230 3232 2d30 362d 3036 2e2e  d%3A2022-06-06..
-000095b0: 3230 3232 2d30 362d 3037 2674 7970 653d  2022-06-07&type=
-000095c0: 4973 7375 6573 290a 0a23 2320 372e 332e  Issues)..## 7.3.
-000095d0: 320a 0a28 5b46 756c 6c20 4368 616e 6765  2..([Full Change
-000095e0: 6c6f 675d 2868 7474 7073 3a2f 2f67 6974  log](https://git
-000095f0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-00009600: 6a75 7079 7465 725f 636c 6965 6e74 2f63  jupyter_client/c
-00009610: 6f6d 7061 7265 2f76 372e 332e 312e 2e2e  ompare/v7.3.1...
-00009620: 6338 3137 3731 3431 3664 3965 3039 6530  c81771416d9e09e0
-00009630: 6539 3262 6537 3939 6633 6538 3534 3964  e92be799f3e8549d
-00009640: 3064 6235 3765 3433 2929 0a0a 2323 2320  0db57e43))..### 
-00009650: 456e 6861 6e63 656d 656e 7473 206d 6164  Enhancements mad
-00009660: 650a 0a2d 2043 6f72 7265 6374 2060 416e  e..- Correct `An
-00009670: 7960 2074 7970 6520 616e 6e6f 7461 7469  y` type annotati
-00009680: 6f6e 732e 205b 2337 3931 5d28 6874 7470  ons. [#791](http
-00009690: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000096a0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-000096b0: 6c69 656e 742f 7075 6c6c 2f37 3931 2920  lient/pull/791) 
-000096c0: 285b 406a 6f6f 7568 615d 2868 7474 7073  ([@joouha](https
-000096d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a6f  ://github.com/jo
-000096e0: 6f75 6861 2929 0a0a 2323 2320 4d61 696e  ouha))..### Main
-000096f0: 7465 6e61 6e63 6520 616e 6420 7570 6b65  tenance and upke
-00009700: 6570 2069 6d70 726f 7665 6d65 6e74 730a  ep improvements.
-00009710: 0a2d 205c 5b70 7265 2d63 6f6d 6d69 742e  .- \[pre-commit.
-00009720: 6369 5c5d 2070 7265 2d63 6f6d 6d69 7420  ci\] pre-commit 
-00009730: 6175 746f 7570 6461 7465 205b 2337 3932  autoupdate [#792
-00009740: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00009750: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00009760: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00009770: 2f37 3932 2920 285b 4070 7265 2d63 6f6d  /792) ([@pre-com
-00009780: 6d69 742d 6369 5d28 6874 7470 733a 2f2f  mit-ci](https://
-00009790: 6769 7468 7562 2e63 6f6d 2f70 7265 2d63  github.com/pre-c
-000097a0: 6f6d 6d69 742d 6369 2929 0a2d 2055 7365  ommit-ci)).- Use
-000097b0: 2068 6174 6368 2062 6163 6b65 6e64 205b   hatch backend [
-000097c0: 2337 3839 5d28 6874 7470 733a 2f2f 6769  #789](https://gi
-000097d0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-000097e0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-000097f0: 7075 6c6c 2f37 3839 2920 285b 4062 6c69  pull/789) ([@bli
-00009800: 6e6b 3130 3733 5d28 6874 7470 733a 2f2f  nk1073](https://
-00009810: 6769 7468 7562 2e63 6f6d 2f62 6c69 6e6b  github.com/blink
-00009820: 3130 3733 2929 0a2d 205c 5b70 7265 2d63  1073)).- \[pre-c
-00009830: 6f6d 6d69 742e 6369 5c5d 2070 7265 2d63  ommit.ci\] pre-c
-00009840: 6f6d 6d69 7420 6175 746f 7570 6461 7465  ommit autoupdate
-00009850: 205b 2337 3838 5d28 6874 7470 733a 2f2f   [#788](https://
-00009860: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00009870: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00009880: 742f 7075 6c6c 2f37 3838 2920 285b 4070  t/pull/788) ([@p
-00009890: 7265 2d63 6f6d 6d69 742d 6369 5d28 6874  re-commit-ci](ht
-000098a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000098b0: 2f70 7265 2d63 6f6d 6d69 742d 6369 2929  /pre-commit-ci))
-000098c0: 0a2d 2055 7365 2066 6c69 7420 6275 696c  .- Use flit buil
-000098d0: 6420 6261 636b 656e 6420 5b23 3738 315d  d backend [#781]
-000098e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000098f0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-00009900: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-00009910: 3738 3129 2028 5b40 626c 696e 6b31 3037  781) ([@blink107
-00009920: 335d 2868 7474 7073 3a2f 2f67 6974 6875  3](https://githu
-00009930: 622e 636f 6d2f 626c 696e 6b31 3037 3329  b.com/blink1073)
-00009940: 290a 0a23 2323 2043 6f6e 7472 6962 7574  )..### Contribut
-00009950: 6f72 7320 746f 2074 6869 7320 7265 6c65  ors to this rele
-00009960: 6173 650a 0a28 5b47 6974 4875 6220 636f  ase..([GitHub co
-00009970: 6e74 7269 6275 746f 7273 2070 6167 6520  ntributors page 
-00009980: 666f 7220 7468 6973 2072 656c 6561 7365  for this release
-00009990: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000099a0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-000099b0: 7974 6572 5f63 6c69 656e 742f 6772 6170  yter_client/grap
-000099c0: 6873 2f63 6f6e 7472 6962 7574 6f72 733f  hs/contributors?
-000099d0: 6672 6f6d 3d32 3032 322d 3035 2d30 3826  from=2022-05-08&
-000099e0: 746f 3d32 3032 322d 3036 2d30 3626 7479  to=2022-06-06&ty
-000099f0: 7065 3d63 2929 0a0a 5b40 626c 696e 6b31  pe=c))..[@blink1
+00009160: 6e74 2f70 756c 6c2f 3831 3629 2028 5b40  nt/pull/816) ([@
+00009170: 7072 652d 636f 6d6d 6974 2d63 695d 2868  pre-commit-ci](h
+00009180: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00009190: 6d2f 7072 652d 636f 6d6d 6974 2d63 6929  m/pre-commit-ci)
+000091a0: 290a 2d20 5c5b 7072 652d 636f 6d6d 6974  ).- \[pre-commit
+000091b0: 2e63 695c 5d20 7072 652d 636f 6d6d 6974  .ci\] pre-commit
+000091c0: 2061 7574 6f75 7064 6174 6520 5b23 3831   autoupdate [#81
+000091d0: 355d 2868 7474 7073 3a2f 2f67 6974 6875  5](https://githu
+000091e0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+000091f0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00009200: 6c2f 3831 3529 2028 5b40 7072 652d 636f  l/815) ([@pre-co
+00009210: 6d6d 6974 2d63 695d 2868 7474 7073 3a2f  mmit-ci](https:/
+00009220: 2f67 6974 6875 622e 636f 6d2f 7072 652d  /github.com/pre-
+00009230: 636f 6d6d 6974 2d63 6929 290a 2d20 5c5b  commit-ci)).- \[
+00009240: 7072 652d 636f 6d6d 6974 2e63 695c 5d20  pre-commit.ci\] 
+00009250: 7072 652d 636f 6d6d 6974 2061 7574 6f75  pre-commit autou
+00009260: 7064 6174 6520 5b23 3831 325d 2868 7474  pdate [#812](htt
+00009270: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00009280: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00009290: 636c 6965 6e74 2f70 756c 6c2f 3831 3229  client/pull/812)
+000092a0: 2028 5b40 7072 652d 636f 6d6d 6974 2d63   ([@pre-commit-c
+000092b0: 695d 2868 7474 7073 3a2f 2f67 6974 6875  i](https://githu
+000092c0: 622e 636f 6d2f 7072 652d 636f 6d6d 6974  b.com/pre-commit
+000092d0: 2d63 6929 290a 2d20 5c5b 7072 652d 636f  -ci)).- \[pre-co
+000092e0: 6d6d 6974 2e63 695c 5d20 7072 652d 636f  mmit.ci\] pre-co
+000092f0: 6d6d 6974 2061 7574 6f75 7064 6174 6520  mmit autoupdate 
+00009300: 5b23 3831 305d 2868 7474 7073 3a2f 2f67  [#810](https://g
+00009310: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00009320: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00009330: 2f70 756c 6c2f 3831 3029 2028 5b40 7072  /pull/810) ([@pr
+00009340: 652d 636f 6d6d 6974 2d63 695d 2868 7474  e-commit-ci](htt
+00009350: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00009360: 7072 652d 636f 6d6d 6974 2d63 6929 290a  pre-commit-ci)).
+00009370: 2d20 5c5b 7072 652d 636f 6d6d 6974 2e63  - \[pre-commit.c
+00009380: 695c 5d20 7072 652d 636f 6d6d 6974 2061  i\] pre-commit a
+00009390: 7574 6f75 7064 6174 6520 5b23 3830 395d  utoupdate [#809]
+000093a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000093b0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+000093c0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+000093d0: 3830 3929 2028 5b40 7072 652d 636f 6d6d  809) ([@pre-comm
+000093e0: 6974 2d63 695d 2868 7474 7073 3a2f 2f67  it-ci](https://g
+000093f0: 6974 6875 622e 636f 6d2f 7072 652d 636f  ithub.com/pre-co
+00009400: 6d6d 6974 2d63 6929 290a 2d20 5c5b 7072  mmit-ci)).- \[pr
+00009410: 652d 636f 6d6d 6974 2e63 695c 5d20 7072  e-commit.ci\] pr
+00009420: 652d 636f 6d6d 6974 2061 7574 6f75 7064  e-commit autoupd
+00009430: 6174 6520 5b23 3830 375d 2868 7474 7073  ate [#807](https
+00009440: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00009450: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+00009460: 6965 6e74 2f70 756c 6c2f 3830 3729 2028  ient/pull/807) (
+00009470: 5b40 7072 652d 636f 6d6d 6974 2d63 695d  [@pre-commit-ci]
+00009480: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00009490: 636f 6d2f 7072 652d 636f 6d6d 6974 2d63  com/pre-commit-c
+000094a0: 6929 290a 0a23 2323 2043 6f6e 7472 6962  i))..### Contrib
+000094b0: 7574 6f72 7320 746f 2074 6869 7320 7265  utors to this re
+000094c0: 6c65 6173 650a 0a28 5b47 6974 4875 6220  lease..([GitHub 
+000094d0: 636f 6e74 7269 6275 746f 7273 2070 6167  contributors pag
+000094e0: 6520 666f 7220 7468 6973 2072 656c 6561  e for this relea
+000094f0: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
+00009500: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00009510: 7570 7974 6572 5f63 6c69 656e 742f 6772  upyter_client/gr
+00009520: 6170 6873 2f63 6f6e 7472 6962 7574 6f72  aphs/contributor
+00009530: 733f 6672 6f6d 3d32 3032 322d 3036 2d30  s?from=2022-06-0
+00009540: 3826 746f 3d32 3032 322d 3038 2d32 3526  8&to=2022-08-25&
+00009550: 7479 7065 3d63 2929 0a0a 5b40 626c 696e  type=c))..[@blin
+00009560: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
+00009570: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+00009580: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+00009590: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+000095a0: 6e74 2b69 6e76 6f6c 7665 7325 3341 626c  nt+involves%3Abl
+000095b0: 696e 6b31 3037 332b 7570 6461 7465 6425  ink1073+updated%
+000095c0: 3341 3230 3232 2d30 362d 3038 2e2e 3230  3A2022-06-08..20
+000095d0: 3232 2d30 382d 3235 2674 7970 653d 4973  22-08-25&type=Is
+000095e0: 7375 6573 2920 7c20 5b40 6461 7669 6462  sues) | [@davidb
+000095f0: 726f 6368 6172 745d 2868 7474 7073 3a2f  rochart](https:/
+00009600: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
+00009610: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
+00009620: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
+00009630: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
+00009640: 6461 7669 6462 726f 6368 6172 742b 7570  davidbrochart+up
+00009650: 6461 7465 6425 3341 3230 3232 2d30 362d  dated%3A2022-06-
+00009660: 3038 2e2e 3230 3232 2d30 382d 3235 2674  08..2022-08-25&t
+00009670: 7970 653d 4973 7375 6573 2920 7c20 5b40  ype=Issues) | [@
+00009680: 6865 6c69 6f7a 3131 5d28 6874 7470 733a  helioz11](https:
+00009690: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+000096a0: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+000096b0: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+000096c0: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+000096d0: 4168 656c 696f 7a31 312b 7570 6461 7465  Ahelioz11+update
+000096e0: 6425 3341 3230 3232 2d30 362d 3038 2e2e  d%3A2022-06-08..
+000096f0: 3230 3232 2d30 382d 3235 2674 7970 653d  2022-08-25&type=
+00009700: 4973 7375 6573 2920 7c20 5b40 7072 652d  Issues) | [@pre-
+00009710: 636f 6d6d 6974 2d63 695d 2868 7474 7073  commit-ci](https
+00009720: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
+00009730: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
+00009740: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
+00009750: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
+00009760: 3341 7072 652d 636f 6d6d 6974 2d63 692b  3Apre-commit-ci+
+00009770: 7570 6461 7465 6425 3341 3230 3232 2d30  updated%3A2022-0
+00009780: 362d 3038 2e2e 3230 3232 2d30 382d 3235  6-08..2022-08-25
+00009790: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
+000097a0: 5b40 7669 6461 7274 665d 2868 7474 7073  [@vidartf](https
+000097b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
+000097c0: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
+000097d0: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
+000097e0: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
+000097f0: 3341 7669 6461 7274 662b 7570 6461 7465  3Avidartf+update
+00009800: 6425 3341 3230 3232 2d30 362d 3038 2e2e  d%3A2022-06-08..
+00009810: 3230 3232 2d30 382d 3235 2674 7970 653d  2022-08-25&type=
+00009820: 4973 7375 6573 290a 0a23 2320 372e 332e  Issues)..## 7.3.
+00009830: 340a 0a28 5b46 756c 6c20 4368 616e 6765  4..([Full Change
+00009840: 6c6f 675d 2868 7474 7073 3a2f 2f67 6974  log](https://git
+00009850: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00009860: 6a75 7079 7465 725f 636c 6965 6e74 2f63  jupyter_client/c
+00009870: 6f6d 7061 7265 2f76 372e 332e 332e 2e2e  ompare/v7.3.3...
+00009880: 6361 3463 6232 6436 6134 6239 3561 3639  ca4cb2d6a4b95a69
+00009890: 3235 6465 3835 6134 3762 3332 3364 3232  25de85a47b323d22
+000098a0: 3335 3033 3263 3734 2929 0a0a 2323 2320  35032c74))..### 
+000098b0: 4275 6773 2066 6978 6564 0a0a 2d20 5265  Bugs fixed..- Re
+000098c0: 7665 7274 206c 6174 6573 7420 6368 616e  vert latest chan
+000098d0: 6765 7320 746f 2060 5468 7265 6164 6564  ges to `Threaded
+000098e0: 5a4d 5153 6f63 6b65 7443 6861 6e6e 656c  ZMQSocketChannel
+000098f0: 6020 6265 6361 7573 6520 7468 6579 2062  ` because they b
+00009900: 7265 616b 2051 7463 6f6e 736f 6c65 205b  reak Qtconsole [
+00009910: 2338 3033 5d28 6874 7470 733a 2f2f 6769  #803](https://gi
+00009920: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+00009930: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+00009940: 7075 6c6c 2f38 3033 2920 285b 4063 636f  pull/803) ([@cco
+00009950: 7264 6f62 6131 325d 2868 7474 7073 3a2f  rdoba12](https:/
+00009960: 2f67 6974 6875 622e 636f 6d2f 6363 6f72  /github.com/ccor
+00009970: 646f 6261 3132 2929 0a0a 2323 2320 4d61  doba12))..### Ma
+00009980: 696e 7465 6e61 6e63 6520 616e 6420 7570  intenance and up
+00009990: 6b65 6570 2069 6d70 726f 7665 6d65 6e74  keep improvement
+000099a0: 730a 0a2d 2046 6978 2073 7068 696e 7820  s..- Fix sphinx 
+000099b0: 352e 3020 7375 7070 6f72 7420 5b23 3830  5.0 support [#80
+000099c0: 345d 2868 7474 7073 3a2f 2f67 6974 6875  4](https://githu
+000099d0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+000099e0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+000099f0: 6c2f 3830 3429 2028 5b40 626c 696e 6b31  l/804) ([@blink1
 00009a00: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
-00009a10: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
-00009a20: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
-00009a30: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
-00009a40: 2b69 6e76 6f6c 7665 7325 3341 626c 696e  +involves%3Ablin
-00009a50: 6b31 3037 332b 7570 6461 7465 6425 3341  k1073+updated%3A
-00009a60: 3230 3232 2d30 352d 3038 2e2e 3230 3232  2022-05-08..2022
-00009a70: 2d30 362d 3036 2674 7970 653d 4973 7375  -06-06&type=Issu
-00009a80: 6573 2920 7c20 5b40 6a6f 6f75 6861 5d28  es) | [@joouha](
-00009a90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00009aa0: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
-00009ab0: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
-00009ac0: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
-00009ad0: 6c76 6573 2533 416a 6f6f 7568 612b 7570  lves%3Ajoouha+up
-00009ae0: 6461 7465 6425 3341 3230 3232 2d30 352d  dated%3A2022-05-
-00009af0: 3038 2e2e 3230 3232 2d30 362d 3036 2674  08..2022-06-06&t
-00009b00: 7970 653d 4973 7375 6573 2920 7c20 5b40  ype=Issues) | [@
-00009b10: 7072 652d 636f 6d6d 6974 2d63 695d 2868  pre-commit-ci](h
-00009b20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00009b30: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
-00009b40: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
-00009b50: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
-00009b60: 7665 7325 3341 7072 652d 636f 6d6d 6974  ves%3Apre-commit
-00009b70: 2d63 692b 7570 6461 7465 6425 3341 3230  -ci+updated%3A20
-00009b80: 3232 2d30 352d 3038 2e2e 3230 3232 2d30  22-05-08..2022-0
-00009b90: 362d 3036 2674 7970 653d 4973 7375 6573  6-06&type=Issues
-00009ba0: 290a 0a23 2320 372e 332e 310a 0a28 5b46  )..## 7.3.1..([F
-00009bb0: 756c 6c20 4368 616e 6765 6c6f 675d 2868  ull Changelog](h
-00009bc0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00009bd0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00009be0: 725f 636c 6965 6e74 2f63 6f6d 7061 7265  r_client/compare
-00009bf0: 2f76 372e 332e 302e 2e2e 3464 6638 6134  /v7.3.0...4df8a4
-00009c00: 3830 3731 3634 3964 3334 3838 6138 3830  8071649d3488a880
-00009c10: 6536 3132 3933 6566 6432 3662 3761 6666  e61293efd26b7aff
-00009c20: 3164 2929 0a0a 2323 2320 4275 6773 2066  1d))..### Bugs f
-00009c30: 6978 6564 0a0a 2d20 4368 6563 6b20 7468  ixed..- Check th
-00009c40: 6174 2063 6861 6e6e 656c 7320 6578 6973  at channels exis
-00009c50: 7420 6265 666f 7265 2061 736b 696e 6720  t before asking 
-00009c60: 6966 2074 6865 7920 6172 6520 616c 6976  if they are aliv
-00009c70: 6520 5b23 3738 355d 2868 7474 7073 3a2f  e [#785](https:/
-00009c80: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-00009c90: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-00009ca0: 6e74 2f70 756c 6c2f 3738 3529 2028 5b40  nt/pull/785) ([@
-00009cb0: 6363 6f72 646f 6261 3132 5d28 6874 7470  ccordoba12](http
-00009cc0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-00009cd0: 636f 7264 6f62 6131 3229 290a 2d20 556e  cordoba12)).- Un
-00009ce0: 6963 6f64 6520 6572 726f 7220 636f 7272  icode error corr
-00009cf0: 6563 7469 6f6e 2075 7369 6e67 2045 7272  ection using Err
-00009d00: 6f72 2048 616e 646c 6572 205b 2337 3739  or Handler [#779
-00009d10: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00009d20: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00009d30: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00009d40: 2f37 3739 2920 285b 4068 7861 7761 785d  /779) ([@hxawax]
-00009d50: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00009d60: 636f 6d2f 6878 6177 6178 2929 0a0a 2323  com/hxawax))..##
-00009d70: 2320 4d61 696e 7465 6e61 6e63 6520 616e  # Maintenance an
-00009d80: 6420 7570 6b65 6570 2069 6d70 726f 7665  d upkeep improve
-00009d90: 6d65 6e74 730a 0a2d 2041 6c6c 6f77 2062  ments..- Allow b
-00009da0: 6f74 2050 5273 2074 6f20 6265 2061 7574  ot PRs to be aut
-00009db0: 6f6d 6174 6963 616c 6c79 206c 6162 656c  omatically label
-00009dc0: 6564 205b 2337 3834 5d28 6874 7470 733a  ed [#784](https:
-00009dd0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-00009de0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-00009df0: 656e 742f 7075 6c6c 2f37 3834 2920 285b  ent/pull/784) ([
-00009e00: 4062 6c69 6e6b 3130 3733 5d28 6874 7470  @blink1073](http
-00009e10: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-00009e20: 6c69 6e6b 3130 3733 2929 0a2d 205c 5b70  link1073)).- \[p
-00009e30: 7265 2d63 6f6d 6d69 742e 6369 5c5d 2070  re-commit.ci\] p
-00009e40: 7265 2d63 6f6d 6d69 7420 6175 746f 7570  re-commit autoup
-00009e50: 6461 7465 205b 2337 3833 5d28 6874 7470  date [#783](http
-00009e60: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00009e70: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00009e80: 6c69 656e 742f 7075 6c6c 2f37 3833 2920  lient/pull/783) 
-00009e90: 285b 4070 7265 2d63 6f6d 6d69 742d 6369  ([@pre-commit-ci
-00009ea0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00009eb0: 2e63 6f6d 2f70 7265 2d63 6f6d 6d69 742d  .com/pre-commit-
-00009ec0: 6369 2929 0a0a 2323 2320 436f 6e74 7269  ci))..### Contri
-00009ed0: 6275 746f 7273 2074 6f20 7468 6973 2072  butors to this r
-00009ee0: 656c 6561 7365 0a0a 285b 4769 7448 7562  elease..([GitHub
-00009ef0: 2063 6f6e 7472 6962 7574 6f72 7320 7061   contributors pa
-00009f00: 6765 2066 6f72 2074 6869 7320 7265 6c65  ge for this rele
-00009f10: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
-00009f20: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-00009f30: 6a75 7079 7465 725f 636c 6965 6e74 2f67  jupyter_client/g
-00009f40: 7261 7068 732f 636f 6e74 7269 6275 746f  raphs/contributo
-00009f50: 7273 3f66 726f 6d3d 3230 3232 2d30 342d  rs?from=2022-04-
-00009f60: 3235 2674 6f3d 3230 3232 2d30 352d 3038  25&to=2022-05-08
-00009f70: 2674 7970 653d 6329 290a 0a5b 4062 6c69  &type=c))..[@bli
-00009f80: 6e6b 3130 3733 5d28 6874 7470 733a 2f2f  nk1073](https://
-00009f90: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
-00009fa0: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
-00009fb0: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
-00009fc0: 656e 742b 696e 766f 6c76 6573 2533 4162  ent+involves%3Ab
-00009fd0: 6c69 6e6b 3130 3733 2b75 7064 6174 6564  link1073+updated
-00009fe0: 2533 4132 3032 322d 3034 2d32 352e 2e32  %3A2022-04-25..2
-00009ff0: 3032 322d 3035 2d30 3826 7479 7065 3d49  022-05-08&type=I
-0000a000: 7373 7565 7329 207c 205b 4063 636f 7264  ssues) | [@ccord
-0000a010: 6f62 6131 325d 2868 7474 7073 3a2f 2f67  oba12](https://g
-0000a020: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
-0000a030: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
-0000a040: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
-0000a050: 6e74 2b69 6e76 6f6c 7665 7325 3341 6363  nt+involves%3Acc
-0000a060: 6f72 646f 6261 3132 2b75 7064 6174 6564  ordoba12+updated
-0000a070: 2533 4132 3032 322d 3034 2d32 352e 2e32  %3A2022-04-25..2
-0000a080: 3032 322d 3035 2d30 3826 7479 7065 3d49  022-05-08&type=I
-0000a090: 7373 7565 7329 207c 205b 4068 7861 7761  ssues) | [@hxawa
-0000a0a0: 785d 2868 7474 7073 3a2f 2f67 6974 6875  x](https://githu
-0000a0b0: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
-0000a0c0: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
-0000a0d0: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
-0000a0e0: 6e76 6f6c 7665 7325 3341 6878 6177 6178  nvolves%3Ahxawax
-0000a0f0: 2b75 7064 6174 6564 2533 4132 3032 322d  +updated%3A2022-
-0000a100: 3034 2d32 352e 2e32 3032 322d 3035 2d30  04-25..2022-05-0
-0000a110: 3826 7479 7065 3d49 7373 7565 7329 207c  8&type=Issues) |
-0000a120: 205b 4070 7265 2d63 6f6d 6d69 742d 6369   [@pre-commit-ci
-0000a130: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000a140: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
-0000a150: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
-0000a160: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
-0000a170: 766f 6c76 6573 2533 4170 7265 2d63 6f6d  volves%3Apre-com
-0000a180: 6d69 742d 6369 2b75 7064 6174 6564 2533  mit-ci+updated%3
-0000a190: 4132 3032 322d 3034 2d32 352e 2e32 3032  A2022-04-25..202
-0000a1a0: 322d 3035 2d30 3826 7479 7065 3d49 7373  2-05-08&type=Iss
-0000a1b0: 7565 7329 0a0a 2323 2037 2e33 2e30 0a0a  ues)..## 7.3.0..
-0000a1c0: 285b 4675 6c6c 2043 6861 6e67 656c 6f67  ([Full Changelog
-0000a1d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000a1e0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-0000a1f0: 7974 6572 5f63 6c69 656e 742f 636f 6d70  yter_client/comp
-0000a200: 6172 652f 7637 2e32 2e32 2e2e 2e66 6135  are/v7.2.2...fa5
-0000a210: 3937 6439 6364 6364 6332 3737 6162 6461  97d9cdcdc277abda
-0000a220: 3263 3363 6162 3461 6565 6531 3539 3364  2c3cab4aeee1593d
-0000a230: 3361 3965 3229 290a 0a23 2323 2042 7567  3a9e2))..### Bug
-0000a240: 7320 6669 7865 640a 0a2d 2046 6978 2073  s fixed..- Fix s
-0000a250: 6875 7464 6f77 6e20 616e 6420 636c 6561  hutdown and clea
-0000a260: 6e75 7020 6265 6861 7669 6f72 205b 2337  nup behavior [#7
-0000a270: 3732 5d28 6874 7470 733a 2f2f 6769 7468  72](https://gith
-0000a280: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-0000a290: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-0000a2a0: 6c6c 2f37 3732 2920 285b 4062 6c69 6e6b  ll/772) ([@blink
-0000a2b0: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
-0000a2c0: 7468 7562 2e63 6f6d 2f62 6c69 6e6b 3130  thub.com/blink10
-0000a2d0: 3733 2929 0a0a 2323 2320 4d61 696e 7465  73))..### Mainte
-0000a2e0: 6e61 6e63 6520 616e 6420 7570 6b65 6570  nance and upkeep
-0000a2f0: 2069 6d70 726f 7665 6d65 6e74 730a 0a2d   improvements..-
-0000a300: 205c 5b70 7265 2d63 6f6d 6d69 742e 6369   \[pre-commit.ci
-0000a310: 5c5d 2070 7265 2d63 6f6d 6d69 7420 6175  \] pre-commit au
-0000a320: 746f 7570 6461 7465 205b 2337 3733 5d28  toupdate [#773](
-0000a330: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000a340: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-0000a350: 6572 5f63 6c69 656e 742f 7075 6c6c 2f37  er_client/pull/7
-0000a360: 3733 2920 285b 4070 7265 2d63 6f6d 6d69  73) ([@pre-commi
-0000a370: 742d 6369 5d28 6874 7470 733a 2f2f 6769  t-ci](https://gi
-0000a380: 7468 7562 2e63 6f6d 2f70 7265 2d63 6f6d  thub.com/pre-com
-0000a390: 6d69 742d 6369 2929 0a2d 205c 5b70 7265  mit-ci)).- \[pre
-0000a3a0: 2d63 6f6d 6d69 742e 6369 5c5d 2070 7265  -commit.ci\] pre
-0000a3b0: 2d63 6f6d 6d69 7420 6175 746f 7570 6461  -commit autoupda
-0000a3c0: 7465 205b 2337 3730 5d28 6874 7470 733a  te [#770](https:
-0000a3d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-0000a3e0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-0000a3f0: 656e 742f 7075 6c6c 2f37 3730 2920 285b  ent/pull/770) ([
-0000a400: 4070 7265 2d63 6f6d 6d69 742d 6369 5d28  @pre-commit-ci](
-0000a410: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000a420: 6f6d 2f70 7265 2d63 6f6d 6d69 742d 6369  om/pre-commit-ci
-0000a430: 2929 0a2d 2049 6d70 726f 7665 206d 7970  )).- Improve myp
-0000a440: 7920 636f 6e66 6967 205b 2337 3639 5d28  y config [#769](
-0000a450: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000a460: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-0000a470: 6572 5f63 6c69 656e 742f 7075 6c6c 2f37  er_client/pull/7
-0000a480: 3639 2920 285b 4062 6c69 6e6b 3130 3733  69) ([@blink1073
-0000a490: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000a4a0: 2e63 6f6d 2f62 6c69 6e6b 3130 3733 2929  .com/blink1073))
-0000a4b0: 0a2d 2043 6c65 616e 2075 7020 7072 652d  .- Clean up pre-
-0000a4c0: 636f 6d6d 6974 205b 2337 3638 5d28 6874  commit [#768](ht
-0000a4d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000a4e0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-0000a4f0: 5f63 6c69 656e 742f 7075 6c6c 2f37 3638  _client/pull/768
-0000a500: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
-0000a510: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000a520: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a0a  om/blink1073))..
-0000a530: 2323 2320 436f 6e74 7269 6275 746f 7273  ### Contributors
-0000a540: 2074 6f20 7468 6973 2072 656c 6561 7365   to this release
-0000a550: 0a0a 285b 4769 7448 7562 2063 6f6e 7472  ..([GitHub contr
-0000a560: 6962 7574 6f72 7320 7061 6765 2066 6f72  ibutors page for
-0000a570: 2074 6869 7320 7265 6c65 6173 655d 2868   this release](h
-0000a580: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000a590: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-0000a5a0: 725f 636c 6965 6e74 2f67 7261 7068 732f  r_client/graphs/
-0000a5b0: 636f 6e74 7269 6275 746f 7273 3f66 726f  contributors?fro
-0000a5c0: 6d3d 3230 3232 2d30 342d 3037 2674 6f3d  m=2022-04-07&to=
-0000a5d0: 3230 3232 2d30 342d 3235 2674 7970 653d  2022-04-25&type=
-0000a5e0: 6329 290a 0a5b 4062 6c69 6e6b 3130 3733  c))..[@blink1073
-0000a5f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000a600: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
-0000a610: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
-0000a620: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
-0000a630: 766f 6c76 6573 2533 4162 6c69 6e6b 3130  volves%3Ablink10
-0000a640: 3733 2b75 7064 6174 6564 2533 4132 3032  73+updated%3A202
-0000a650: 322d 3034 2d30 372e 2e32 3032 322d 3034  2-04-07..2022-04
-0000a660: 2d32 3526 7479 7065 3d49 7373 7565 7329  -25&type=Issues)
-0000a670: 207c 205b 4070 7265 2d63 6f6d 6d69 742d   | [@pre-commit-
-0000a680: 6369 5d28 6874 7470 733a 2f2f 6769 7468  ci](https://gith
-0000a690: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
-0000a6a0: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
-0000a6b0: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
-0000a6c0: 696e 766f 6c76 6573 2533 4170 7265 2d63  involves%3Apre-c
-0000a6d0: 6f6d 6d69 742d 6369 2b75 7064 6174 6564  ommit-ci+updated
-0000a6e0: 2533 4132 3032 322d 3034 2d30 372e 2e32  %3A2022-04-07..2
-0000a6f0: 3032 322d 3034 2d32 3526 7479 7065 3d49  022-04-25&type=I
-0000a700: 7373 7565 7329 0a0a 2323 2037 2e32 2e32  ssues)..## 7.2.2
-0000a710: 0a0a 285b 4675 6c6c 2043 6861 6e67 656c  ..([Full Changel
-0000a720: 6f67 5d28 6874 7470 733a 2f2f 6769 7468  og](https://gith
-0000a730: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-0000a740: 7570 7974 6572 5f63 6c69 656e 742f 636f  upyter_client/co
-0000a750: 6d70 6172 652f 7637 2e32 2e31 2e2e 2e30  mpare/v7.2.1...0
-0000a760: 3162 3230 3935 6439 3663 3831 6335 3665  1b2095d96c81c56e
-0000a770: 6466 3866 3564 6634 3465 3132 6534 3736  df8f5df44e12e476
-0000a780: 6232 6263 6438 3729 290a 0a23 2323 204d  b2bcd87))..### M
-0000a790: 6169 6e74 656e 616e 6365 2061 6e64 2075  aintenance and u
-0000a7a0: 706b 6565 7020 696d 7072 6f76 656d 656e  pkeep improvemen
-0000a7b0: 7473 0a0a 2d20 496e 636c 7564 6520 7079  ts..- Include py
-0000a7c0: 2e74 7970 6564 2066 696c 6520 5b23 3736  .typed file [#76
-0000a7d0: 365d 2868 7474 7073 3a2f 2f67 6974 6875  6](https://githu
-0000a7e0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-0000a7f0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-0000a800: 6c2f 3736 3629 2028 5b40 626c 696e 6b31  l/766) ([@blink1
-0000a810: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
-0000a820: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
-0000a830: 3329 290a 2d20 5c5b 7072 652d 636f 6d6d  3)).- \[pre-comm
-0000a840: 6974 2e63 695c 5d20 7072 652d 636f 6d6d  it.ci\] pre-comm
-0000a850: 6974 2061 7574 6f75 7064 6174 6520 5b23  it autoupdate [#
-0000a860: 3736 355d 2868 7474 7073 3a2f 2f67 6974  765](https://git
-0000a870: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-0000a880: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-0000a890: 756c 6c2f 3736 3529 2028 5b40 7072 652d  ull/765) ([@pre-
-0000a8a0: 636f 6d6d 6974 2d63 695d 2868 7474 7073  commit-ci](https
-0000a8b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7072  ://github.com/pr
-0000a8c0: 652d 636f 6d6d 6974 2d63 6929 290a 2d20  e-commit-ci)).- 
-0000a8d0: 4d6f 7265 2043 6c65 616e 7570 205b 2337  More Cleanup [#7
-0000a8e0: 3634 5d28 6874 7470 733a 2f2f 6769 7468  64](https://gith
-0000a8f0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-0000a900: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-0000a910: 6c6c 2f37 3634 2920 285b 4062 6c69 6e6b  ll/764) ([@blink
-0000a920: 3130 3733 5d28 6874 7470 733a 2f2f 6769  1073](https://gi
-0000a930: 7468 7562 2e63 6f6d 2f62 6c69 6e6b 3130  thub.com/blink10
-0000a940: 3733 2929 0a0a 2323 2320 436f 6e74 7269  73))..### Contri
-0000a950: 6275 746f 7273 2074 6f20 7468 6973 2072  butors to this r
-0000a960: 656c 6561 7365 0a0a 285b 4769 7448 7562  elease..([GitHub
-0000a970: 2063 6f6e 7472 6962 7574 6f72 7320 7061   contributors pa
-0000a980: 6765 2066 6f72 2074 6869 7320 7265 6c65  ge for this rele
-0000a990: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
-0000a9a0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-0000a9b0: 6a75 7079 7465 725f 636c 6965 6e74 2f67  jupyter_client/g
-0000a9c0: 7261 7068 732f 636f 6e74 7269 6275 746f  raphs/contributo
-0000a9d0: 7273 3f66 726f 6d3d 3230 3232 2d30 332d  rs?from=2022-03-
-0000a9e0: 3330 2674 6f3d 3230 3232 2d30 342d 3037  30&to=2022-04-07
-0000a9f0: 2674 7970 653d 6329 290a 0a5b 4062 6c69  &type=c))..[@bli
-0000aa00: 6e6b 3130 3733 5d28 6874 7470 733a 2f2f  nk1073](https://
-0000aa10: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
-0000aa20: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
-0000aa30: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
-0000aa40: 656e 742b 696e 766f 6c76 6573 2533 4162  ent+involves%3Ab
-0000aa50: 6c69 6e6b 3130 3733 2b75 7064 6174 6564  link1073+updated
-0000aa60: 2533 4132 3032 322d 3033 2d33 302e 2e32  %3A2022-03-30..2
-0000aa70: 3032 322d 3034 2d30 3726 7479 7065 3d49  022-04-07&type=I
-0000aa80: 7373 7565 7329 207c 205b 4064 6176 6964  ssues) | [@david
-0000aa90: 6272 6f63 6861 7274 5d28 6874 7470 733a  brochart](https:
-0000aaa0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
-0000aab0: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
-0000aac0: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
-0000aad0: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
-0000aae0: 4164 6176 6964 6272 6f63 6861 7274 2b75  Adavidbrochart+u
-0000aaf0: 7064 6174 6564 2533 4132 3032 322d 3033  pdated%3A2022-03
-0000ab00: 2d33 302e 2e32 3032 322d 3034 2d30 3726  -30..2022-04-07&
-0000ab10: 7479 7065 3d49 7373 7565 7329 207c 205b  type=Issues) | [
-0000ab20: 4065 6368 6172 6c65 735d 2868 7474 7073  @echarles](https
-0000ab30: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
-0000ab40: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
-0000ab50: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
-0000ab60: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
-0000ab70: 3341 6563 6861 726c 6573 2b75 7064 6174  3Aecharles+updat
-0000ab80: 6564 2533 4132 3032 322d 3033 2d33 302e  ed%3A2022-03-30.
-0000ab90: 2e32 3032 322d 3034 2d30 3726 7479 7065  .2022-04-07&type
-0000aba0: 3d49 7373 7565 7329 207c 205b 4070 7265  =Issues) | [@pre
-0000abb0: 2d63 6f6d 6d69 742d 6369 5d28 6874 7470  -commit-ci](http
-0000abc0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-0000abd0: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
-0000abe0: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
-0000abf0: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
-0000ac00: 2533 4170 7265 2d63 6f6d 6d69 742d 6369  %3Apre-commit-ci
-0000ac10: 2b75 7064 6174 6564 2533 4132 3032 322d  +updated%3A2022-
-0000ac20: 3033 2d33 302e 2e32 3032 322d 3034 2d30  03-30..2022-04-0
-0000ac30: 3726 7479 7065 3d49 7373 7565 7329 0a0a  7&type=Issues)..
-0000ac40: 2323 2037 2e32 2e31 0a0a 285b 4675 6c6c  ## 7.2.1..([Full
-0000ac50: 2043 6861 6e67 656c 6f67 5d28 6874 7470   Changelog](http
-0000ac60: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-0000ac70: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-0000ac80: 6c69 656e 742f 636f 6d70 6172 652f 7637  lient/compare/v7
-0000ac90: 2e32 2e30 2e2e 2e36 3833 6538 6464 3936  .2.0...683e8dd96
-0000aca0: 6563 6435 3264 6134 3861 3835 6636 3765  ecd52da48a85f67e
-0000acb0: 3461 6533 3164 3835 6631 6336 3631 3629  4ae31d85f1c6616)
-0000acc0: 290a 0a23 2323 204d 6169 6e74 656e 616e  )..### Maintenan
-0000acd0: 6365 2061 6e64 2075 706b 6565 7020 696d  ce and upkeep im
-0000ace0: 7072 6f76 656d 656e 7473 0a0a 2d20 4861  provements..- Ha
-0000acf0: 6e64 6c65 2057 6172 6e69 6e67 7320 5b23  ndle Warnings [#
-0000ad00: 3736 305d 2868 7474 7073 3a2f 2f67 6974  760](https://git
+00009a10: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
+00009a20: 3329 290a 2d20 5c5b 7072 652d 636f 6d6d  3)).- \[pre-comm
+00009a30: 6974 2e63 695c 5d20 7072 652d 636f 6d6d  it.ci\] pre-comm
+00009a40: 6974 2061 7574 6f75 7064 6174 6520 5b23  it autoupdate [#
+00009a50: 3739 395d 2868 7474 7073 3a2f 2f67 6974  799](https://git
+00009a60: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00009a70: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+00009a80: 756c 6c2f 3739 3929 2028 5b40 7072 652d  ull/799) ([@pre-
+00009a90: 636f 6d6d 6974 2d63 695d 2868 7474 7073  commit-ci](https
+00009aa0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7072  ://github.com/pr
+00009ab0: 652d 636f 6d6d 6974 2d63 6929 290a 0a23  e-commit-ci))..#
+00009ac0: 2323 2043 6f6e 7472 6962 7574 6f72 7320  ## Contributors 
+00009ad0: 746f 2074 6869 7320 7265 6c65 6173 650a  to this release.
+00009ae0: 0a28 5b47 6974 4875 6220 636f 6e74 7269  .([GitHub contri
+00009af0: 6275 746f 7273 2070 6167 6520 666f 7220  butors page for 
+00009b00: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
+00009b10: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00009b20: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+00009b30: 5f63 6c69 656e 742f 6772 6170 6873 2f63  _client/graphs/c
+00009b40: 6f6e 7472 6962 7574 6f72 733f 6672 6f6d  ontributors?from
+00009b50: 3d32 3032 322d 3036 2d30 3726 746f 3d32  =2022-06-07&to=2
+00009b60: 3032 322d 3036 2d30 3826 7479 7065 3d63  022-06-08&type=c
+00009b70: 2929 0a0a 5b40 626c 696e 6b31 3037 335d  ))..[@blink1073]
+00009b80: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00009b90: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
+00009ba0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
+00009bb0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
+00009bc0: 6f6c 7665 7325 3341 626c 696e 6b31 3037  olves%3Ablink107
+00009bd0: 332b 7570 6461 7465 6425 3341 3230 3232  3+updated%3A2022
+00009be0: 2d30 362d 3037 2e2e 3230 3232 2d30 362d  -06-07..2022-06-
+00009bf0: 3038 2674 7970 653d 4973 7375 6573 2920  08&type=Issues) 
+00009c00: 7c20 5b40 6363 6f72 646f 6261 3132 5d28  | [@ccordoba12](
+00009c10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00009c20: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
+00009c30: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
+00009c40: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
+00009c50: 6c76 6573 2533 4163 636f 7264 6f62 6131  lves%3Accordoba1
+00009c60: 322b 7570 6461 7465 6425 3341 3230 3232  2+updated%3A2022
+00009c70: 2d30 362d 3037 2e2e 3230 3232 2d30 362d  -06-07..2022-06-
+00009c80: 3038 2674 7970 653d 4973 7375 6573 2920  08&type=Issues) 
+00009c90: 7c20 5b40 7072 652d 636f 6d6d 6974 2d63  | [@pre-commit-c
+00009ca0: 695d 2868 7474 7073 3a2f 2f67 6974 6875  i](https://githu
+00009cb0: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
+00009cc0: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
+00009cd0: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
+00009ce0: 6e76 6f6c 7665 7325 3341 7072 652d 636f  nvolves%3Apre-co
+00009cf0: 6d6d 6974 2d63 692b 7570 6461 7465 6425  mmit-ci+updated%
+00009d00: 3341 3230 3232 2d30 362d 3037 2e2e 3230  3A2022-06-07..20
+00009d10: 3232 2d30 362d 3038 2674 7970 653d 4973  22-06-08&type=Is
+00009d20: 7375 6573 290a 0a23 2320 372e 332e 330a  sues)..## 7.3.3.
+00009d30: 0a28 5b46 756c 6c20 4368 616e 6765 6c6f  .([Full Changelo
+00009d40: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
+00009d50: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00009d60: 7079 7465 725f 636c 6965 6e74 2f63 6f6d  pyter_client/com
+00009d70: 7061 7265 2f76 372e 332e 322e 2e2e 3337  pare/v7.3.2...37
+00009d80: 6361 3337 6438 3635 6462 3236 3065 3764  ca37d865db260e7d
+00009d90: 6136 6661 3835 3333 3962 6534 3530 6436  a6fa85339be450d6
+00009da0: 6664 3363 3363 2929 0a0a 2323 2320 4275  fd3c3c))..### Bu
+00009db0: 6773 2066 6978 6564 0a0a 2d20 4164 6420  gs fixed..- Add 
+00009dc0: 6c6f 6361 6c2d 7072 6f76 6973 696f 6e65  local-provisione
+00009dd0: 7220 656e 7472 7920 706f 696e 7420 746f  r entry point to
+00009de0: 2070 7970 726f 6a65 6374 2e74 6f6d 6c20   pyproject.toml 
+00009df0: 4669 7865 7320 2338 3030 205b 2338 3031  Fixes #800 [#801
+00009e00: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00009e10: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00009e20: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00009e30: 2f38 3031 2920 285b 4075 746b 6f6e 6f73  /801) ([@utkonos
+00009e40: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00009e50: 2e63 6f6d 2f75 746b 6f6e 6f73 2929 0a0a  .com/utkonos))..
+00009e60: 2323 2320 436f 6e74 7269 6275 746f 7273  ### Contributors
+00009e70: 2074 6f20 7468 6973 2072 656c 6561 7365   to this release
+00009e80: 0a0a 285b 4769 7448 7562 2063 6f6e 7472  ..([GitHub contr
+00009e90: 6962 7574 6f72 7320 7061 6765 2066 6f72  ibutors page for
+00009ea0: 2074 6869 7320 7265 6c65 6173 655d 2868   this release](h
+00009eb0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00009ec0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+00009ed0: 725f 636c 6965 6e74 2f67 7261 7068 732f  r_client/graphs/
+00009ee0: 636f 6e74 7269 6275 746f 7273 3f66 726f  contributors?fro
+00009ef0: 6d3d 3230 3232 2d30 362d 3036 2674 6f3d  m=2022-06-06&to=
+00009f00: 3230 3232 2d30 362d 3037 2674 7970 653d  2022-06-07&type=
+00009f10: 6329 290a 0a5b 4075 746b 6f6e 6f73 5d28  c))..[@utkonos](
+00009f20: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00009f30: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
+00009f40: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
+00009f50: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
+00009f60: 6c76 6573 2533 4175 746b 6f6e 6f73 2b75  lves%3Autkonos+u
+00009f70: 7064 6174 6564 2533 4132 3032 322d 3036  pdated%3A2022-06
+00009f80: 2d30 362e 2e32 3032 322d 3036 2d30 3726  -06..2022-06-07&
+00009f90: 7479 7065 3d49 7373 7565 7329 0a0a 2323  type=Issues)..##
+00009fa0: 2037 2e33 2e32 0a0a 285b 4675 6c6c 2043   7.3.2..([Full C
+00009fb0: 6861 6e67 656c 6f67 5d28 6874 7470 733a  hangelog](https:
+00009fc0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+00009fd0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+00009fe0: 656e 742f 636f 6d70 6172 652f 7637 2e33  ent/compare/v7.3
+00009ff0: 2e31 2e2e 2e63 3831 3737 3134 3136 6439  .1...c81771416d9
+0000a000: 6530 3965 3065 3932 6265 3739 3966 3365  e09e0e92be799f3e
+0000a010: 3835 3439 6430 6462 3537 6534 3329 290a  8549d0db57e43)).
+0000a020: 0a23 2323 2045 6e68 616e 6365 6d65 6e74  .### Enhancement
+0000a030: 7320 6d61 6465 0a0a 2d20 436f 7272 6563  s made..- Correc
+0000a040: 7420 6041 6e79 6020 7479 7065 2061 6e6e  t `Any` type ann
+0000a050: 6f74 6174 696f 6e73 2e20 5b23 3739 315d  otations. [#791]
+0000a060: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000a070: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+0000a080: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+0000a090: 3739 3129 2028 5b40 6a6f 6f75 6861 5d28  791) ([@joouha](
+0000a0a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000a0b0: 6f6d 2f6a 6f6f 7568 6129 290a 0a23 2323  om/joouha))..###
+0000a0c0: 204d 6169 6e74 656e 616e 6365 2061 6e64   Maintenance and
+0000a0d0: 2075 706b 6565 7020 696d 7072 6f76 656d   upkeep improvem
+0000a0e0: 656e 7473 0a0a 2d20 5c5b 7072 652d 636f  ents..- \[pre-co
+0000a0f0: 6d6d 6974 2e63 695c 5d20 7072 652d 636f  mmit.ci\] pre-co
+0000a100: 6d6d 6974 2061 7574 6f75 7064 6174 6520  mmit autoupdate 
+0000a110: 5b23 3739 325d 2868 7474 7073 3a2f 2f67  [#792](https://g
+0000a120: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+0000a130: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+0000a140: 2f70 756c 6c2f 3739 3229 2028 5b40 7072  /pull/792) ([@pr
+0000a150: 652d 636f 6d6d 6974 2d63 695d 2868 7474  e-commit-ci](htt
+0000a160: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000a170: 7072 652d 636f 6d6d 6974 2d63 6929 290a  pre-commit-ci)).
+0000a180: 2d20 5573 6520 6861 7463 6820 6261 636b  - Use hatch back
+0000a190: 656e 6420 5b23 3738 395d 2868 7474 7073  end [#789](https
+0000a1a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+0000a1b0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+0000a1c0: 6965 6e74 2f70 756c 6c2f 3738 3929 2028  ient/pull/789) (
+0000a1d0: 5b40 626c 696e 6b31 3037 335d 2868 7474  [@blink1073](htt
+0000a1e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000a1f0: 626c 696e 6b31 3037 3329 290a 2d20 5c5b  blink1073)).- \[
+0000a200: 7072 652d 636f 6d6d 6974 2e63 695c 5d20  pre-commit.ci\] 
+0000a210: 7072 652d 636f 6d6d 6974 2061 7574 6f75  pre-commit autou
+0000a220: 7064 6174 6520 5b23 3738 385d 2868 7474  pdate [#788](htt
+0000a230: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000a240: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+0000a250: 636c 6965 6e74 2f70 756c 6c2f 3738 3829  client/pull/788)
+0000a260: 2028 5b40 7072 652d 636f 6d6d 6974 2d63   ([@pre-commit-c
+0000a270: 695d 2868 7474 7073 3a2f 2f67 6974 6875  i](https://githu
+0000a280: 622e 636f 6d2f 7072 652d 636f 6d6d 6974  b.com/pre-commit
+0000a290: 2d63 6929 290a 2d20 5573 6520 666c 6974  -ci)).- Use flit
+0000a2a0: 2062 7569 6c64 2062 6163 6b65 6e64 205b   build backend [
+0000a2b0: 2337 3831 5d28 6874 7470 733a 2f2f 6769  #781](https://gi
+0000a2c0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+0000a2d0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+0000a2e0: 7075 6c6c 2f37 3831 2920 285b 4062 6c69  pull/781) ([@bli
+0000a2f0: 6e6b 3130 3733 5d28 6874 7470 733a 2f2f  nk1073](https://
+0000a300: 6769 7468 7562 2e63 6f6d 2f62 6c69 6e6b  github.com/blink
+0000a310: 3130 3733 2929 0a0a 2323 2320 436f 6e74  1073))..### Cont
+0000a320: 7269 6275 746f 7273 2074 6f20 7468 6973  ributors to this
+0000a330: 2072 656c 6561 7365 0a0a 285b 4769 7448   release..([GitH
+0000a340: 7562 2063 6f6e 7472 6962 7574 6f72 7320  ub contributors 
+0000a350: 7061 6765 2066 6f72 2074 6869 7320 7265  page for this re
+0000a360: 6c65 6173 655d 2868 7474 7073 3a2f 2f67  lease](https://g
+0000a370: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+0000a380: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+0000a390: 2f67 7261 7068 732f 636f 6e74 7269 6275  /graphs/contribu
+0000a3a0: 746f 7273 3f66 726f 6d3d 3230 3232 2d30  tors?from=2022-0
+0000a3b0: 352d 3038 2674 6f3d 3230 3232 2d30 362d  5-08&to=2022-06-
+0000a3c0: 3036 2674 7970 653d 6329 290a 0a5b 4062  06&type=c))..[@b
+0000a3d0: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
+0000a3e0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+0000a3f0: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+0000a400: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+0000a410: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+0000a420: 4162 6c69 6e6b 3130 3733 2b75 7064 6174  Ablink1073+updat
+0000a430: 6564 2533 4132 3032 322d 3035 2d30 382e  ed%3A2022-05-08.
+0000a440: 2e32 3032 322d 3036 2d30 3626 7479 7065  .2022-06-06&type
+0000a450: 3d49 7373 7565 7329 207c 205b 406a 6f6f  =Issues) | [@joo
+0000a460: 7568 615d 2868 7474 7073 3a2f 2f67 6974  uha](https://git
+0000a470: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
+0000a480: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
+0000a490: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
+0000a4a0: 2b69 6e76 6f6c 7665 7325 3341 6a6f 6f75  +involves%3Ajoou
+0000a4b0: 6861 2b75 7064 6174 6564 2533 4132 3032  ha+updated%3A202
+0000a4c0: 322d 3035 2d30 382e 2e32 3032 322d 3036  2-05-08..2022-06
+0000a4d0: 2d30 3626 7479 7065 3d49 7373 7565 7329  -06&type=Issues)
+0000a4e0: 207c 205b 4070 7265 2d63 6f6d 6d69 742d   | [@pre-commit-
+0000a4f0: 6369 5d28 6874 7470 733a 2f2f 6769 7468  ci](https://gith
+0000a500: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
+0000a510: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
+0000a520: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
+0000a530: 696e 766f 6c76 6573 2533 4170 7265 2d63  involves%3Apre-c
+0000a540: 6f6d 6d69 742d 6369 2b75 7064 6174 6564  ommit-ci+updated
+0000a550: 2533 4132 3032 322d 3035 2d30 382e 2e32  %3A2022-05-08..2
+0000a560: 3032 322d 3036 2d30 3626 7479 7065 3d49  022-06-06&type=I
+0000a570: 7373 7565 7329 0a0a 2323 2037 2e33 2e31  ssues)..## 7.3.1
+0000a580: 0a0a 285b 4675 6c6c 2043 6861 6e67 656c  ..([Full Changel
+0000a590: 6f67 5d28 6874 7470 733a 2f2f 6769 7468  og](https://gith
+0000a5a0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+0000a5b0: 7570 7974 6572 5f63 6c69 656e 742f 636f  upyter_client/co
+0000a5c0: 6d70 6172 652f 7637 2e33 2e30 2e2e 2e34  mpare/v7.3.0...4
+0000a5d0: 6466 3861 3438 3037 3136 3439 6433 3438  df8a48071649d348
+0000a5e0: 3861 3838 3065 3631 3239 3365 6664 3236  8a880e61293efd26
+0000a5f0: 6237 6166 6631 6429 290a 0a23 2323 2042  b7aff1d))..### B
+0000a600: 7567 7320 6669 7865 640a 0a2d 2043 6865  ugs fixed..- Che
+0000a610: 636b 2074 6861 7420 6368 616e 6e65 6c73  ck that channels
+0000a620: 2065 7869 7374 2062 6566 6f72 6520 6173   exist before as
+0000a630: 6b69 6e67 2069 6620 7468 6579 2061 7265  king if they are
+0000a640: 2061 6c69 7665 205b 2337 3835 5d28 6874   alive [#785](ht
+0000a650: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000a660: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+0000a670: 5f63 6c69 656e 742f 7075 6c6c 2f37 3835  _client/pull/785
+0000a680: 2920 285b 4063 636f 7264 6f62 6131 325d  ) ([@ccordoba12]
+0000a690: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000a6a0: 636f 6d2f 6363 6f72 646f 6261 3132 2929  com/ccordoba12))
+0000a6b0: 0a2d 2055 6e69 636f 6465 2065 7272 6f72  .- Unicode error
+0000a6c0: 2063 6f72 7265 6374 696f 6e20 7573 696e   correction usin
+0000a6d0: 6720 4572 726f 7220 4861 6e64 6c65 7220  g Error Handler 
+0000a6e0: 5b23 3737 395d 2868 7474 7073 3a2f 2f67  [#779](https://g
+0000a6f0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+0000a700: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+0000a710: 2f70 756c 6c2f 3737 3929 2028 5b40 6878  /pull/779) ([@hx
+0000a720: 6177 6178 5d28 6874 7470 733a 2f2f 6769  awax](https://gi
+0000a730: 7468 7562 2e63 6f6d 2f68 7861 7761 7829  thub.com/hxawax)
+0000a740: 290a 0a23 2323 204d 6169 6e74 656e 616e  )..### Maintenan
+0000a750: 6365 2061 6e64 2075 706b 6565 7020 696d  ce and upkeep im
+0000a760: 7072 6f76 656d 656e 7473 0a0a 2d20 416c  provements..- Al
+0000a770: 6c6f 7720 626f 7420 5052 7320 746f 2062  low bot PRs to b
+0000a780: 6520 6175 746f 6d61 7469 6361 6c6c 7920  e automatically 
+0000a790: 6c61 6265 6c65 6420 5b23 3738 345d 2868  labeled [#784](h
+0000a7a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000a7b0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+0000a7c0: 725f 636c 6965 6e74 2f70 756c 6c2f 3738  r_client/pull/78
+0000a7d0: 3429 2028 5b40 626c 696e 6b31 3037 335d  4) ([@blink1073]
+0000a7e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000a7f0: 636f 6d2f 626c 696e 6b31 3037 3329 290a  com/blink1073)).
+0000a800: 2d20 5c5b 7072 652d 636f 6d6d 6974 2e63  - \[pre-commit.c
+0000a810: 695c 5d20 7072 652d 636f 6d6d 6974 2061  i\] pre-commit a
+0000a820: 7574 6f75 7064 6174 6520 5b23 3738 335d  utoupdate [#783]
+0000a830: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000a840: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+0000a850: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+0000a860: 3738 3329 2028 5b40 7072 652d 636f 6d6d  783) ([@pre-comm
+0000a870: 6974 2d63 695d 2868 7474 7073 3a2f 2f67  it-ci](https://g
+0000a880: 6974 6875 622e 636f 6d2f 7072 652d 636f  ithub.com/pre-co
+0000a890: 6d6d 6974 2d63 6929 290a 0a23 2323 2043  mmit-ci))..### C
+0000a8a0: 6f6e 7472 6962 7574 6f72 7320 746f 2074  ontributors to t
+0000a8b0: 6869 7320 7265 6c65 6173 650a 0a28 5b47  his release..([G
+0000a8c0: 6974 4875 6220 636f 6e74 7269 6275 746f  itHub contributo
+0000a8d0: 7273 2070 6167 6520 666f 7220 7468 6973  rs page for this
+0000a8e0: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
+0000a8f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+0000a900: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+0000a910: 656e 742f 6772 6170 6873 2f63 6f6e 7472  ent/graphs/contr
+0000a920: 6962 7574 6f72 733f 6672 6f6d 3d32 3032  ibutors?from=202
+0000a930: 322d 3034 2d32 3526 746f 3d32 3032 322d  2-04-25&to=2022-
+0000a940: 3035 2d30 3826 7479 7065 3d63 2929 0a0a  05-08&type=c))..
+0000a950: 5b40 626c 696e 6b31 3037 335d 2868 7474  [@blink1073](htt
+0000a960: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000a970: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
+0000a980: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
+0000a990: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
+0000a9a0: 7325 3341 626c 696e 6b31 3037 332b 7570  s%3Ablink1073+up
+0000a9b0: 6461 7465 6425 3341 3230 3232 2d30 342d  dated%3A2022-04-
+0000a9c0: 3235 2e2e 3230 3232 2d30 352d 3038 2674  25..2022-05-08&t
+0000a9d0: 7970 653d 4973 7375 6573 2920 7c20 5b40  ype=Issues) | [@
+0000a9e0: 6363 6f72 646f 6261 3132 5d28 6874 7470  ccordoba12](http
+0000a9f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+0000aa00: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
+0000aa10: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
+0000aa20: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
+0000aa30: 2533 4163 636f 7264 6f62 6131 322b 7570  %3Accordoba12+up
+0000aa40: 6461 7465 6425 3341 3230 3232 2d30 342d  dated%3A2022-04-
+0000aa50: 3235 2e2e 3230 3232 2d30 352d 3038 2674  25..2022-05-08&t
+0000aa60: 7970 653d 4973 7375 6573 2920 7c20 5b40  ype=Issues) | [@
+0000aa70: 6878 6177 6178 5d28 6874 7470 733a 2f2f  hxawax](https://
+0000aa80: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
+0000aa90: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
+0000aaa0: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
+0000aab0: 656e 742b 696e 766f 6c76 6573 2533 4168  ent+involves%3Ah
+0000aac0: 7861 7761 782b 7570 6461 7465 6425 3341  xawax+updated%3A
+0000aad0: 3230 3232 2d30 342d 3235 2e2e 3230 3232  2022-04-25..2022
+0000aae0: 2d30 352d 3038 2674 7970 653d 4973 7375  -05-08&type=Issu
+0000aaf0: 6573 2920 7c20 5b40 7072 652d 636f 6d6d  es) | [@pre-comm
+0000ab00: 6974 2d63 695d 2868 7474 7073 3a2f 2f67  it-ci](https://g
+0000ab10: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+0000ab20: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+0000ab30: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+0000ab40: 6e74 2b69 6e76 6f6c 7665 7325 3341 7072  nt+involves%3Apr
+0000ab50: 652d 636f 6d6d 6974 2d63 692b 7570 6461  e-commit-ci+upda
+0000ab60: 7465 6425 3341 3230 3232 2d30 342d 3235  ted%3A2022-04-25
+0000ab70: 2e2e 3230 3232 2d30 352d 3038 2674 7970  ..2022-05-08&typ
+0000ab80: 653d 4973 7375 6573 290a 0a23 2320 372e  e=Issues)..## 7.
+0000ab90: 332e 300a 0a28 5b46 756c 6c20 4368 616e  3.0..([Full Chan
+0000aba0: 6765 6c6f 675d 2868 7474 7073 3a2f 2f67  gelog](https://g
+0000abb0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+0000abc0: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+0000abd0: 2f63 6f6d 7061 7265 2f76 372e 322e 322e  /compare/v7.2.2.
+0000abe0: 2e2e 6661 3539 3764 3963 6463 6463 3237  ..fa597d9cdcdc27
+0000abf0: 3761 6264 6132 6333 6361 6234 6165 6565  7abda2c3cab4aeee
+0000ac00: 3135 3933 6433 6139 6532 2929 0a0a 2323  1593d3a9e2))..##
+0000ac10: 2320 4275 6773 2066 6978 6564 0a0a 2d20  # Bugs fixed..- 
+0000ac20: 4669 7820 7368 7574 646f 776e 2061 6e64  Fix shutdown and
+0000ac30: 2063 6c65 616e 7570 2062 6568 6176 696f   cleanup behavio
+0000ac40: 7220 5b23 3737 325d 2868 7474 7073 3a2f  r [#772](https:/
+0000ac50: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+0000ac60: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+0000ac70: 6e74 2f70 756c 6c2f 3737 3229 2028 5b40  nt/pull/772) ([@
+0000ac80: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
+0000ac90: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
+0000aca0: 696e 6b31 3037 3329 290a 0a23 2323 204d  ink1073))..### M
+0000acb0: 6169 6e74 656e 616e 6365 2061 6e64 2075  aintenance and u
+0000acc0: 706b 6565 7020 696d 7072 6f76 656d 656e  pkeep improvemen
+0000acd0: 7473 0a0a 2d20 5c5b 7072 652d 636f 6d6d  ts..- \[pre-comm
+0000ace0: 6974 2e63 695c 5d20 7072 652d 636f 6d6d  it.ci\] pre-comm
+0000acf0: 6974 2061 7574 6f75 7064 6174 6520 5b23  it autoupdate [#
+0000ad00: 3737 335d 2868 7474 7073 3a2f 2f67 6974  773](https://git
 0000ad10: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
 0000ad20: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-0000ad30: 756c 6c2f 3736 3029 2028 5b40 626c 696e  ull/760) ([@blin
-0000ad40: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
-0000ad50: 6974 6875 622e 636f 6d2f 626c 696e 6b31  ithub.com/blink1
-0000ad60: 3037 3329 290a 0a23 2323 2043 6f6e 7472  073))..### Contr
-0000ad70: 6962 7574 6f72 7320 746f 2074 6869 7320  ibutors to this 
-0000ad80: 7265 6c65 6173 650a 0a28 5b47 6974 4875  release..([GitHu
-0000ad90: 6220 636f 6e74 7269 6275 746f 7273 2070  b contributors p
-0000ada0: 6167 6520 666f 7220 7468 6973 2072 656c  age for this rel
-0000adb0: 6561 7365 5d28 6874 7470 733a 2f2f 6769  ease](https://gi
-0000adc0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-0000add0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-0000ade0: 6772 6170 6873 2f63 6f6e 7472 6962 7574  graphs/contribut
-0000adf0: 6f72 733f 6672 6f6d 3d32 3032 322d 3033  ors?from=2022-03
-0000ae00: 2d32 3926 746f 3d32 3032 322d 3033 2d33  -29&to=2022-03-3
-0000ae10: 3026 7479 7065 3d63 2929 0a0a 5b40 626c  0&type=c))..[@bl
-0000ae20: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
-0000ae30: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-0000ae40: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-0000ae50: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-0000ae60: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-0000ae70: 626c 696e 6b31 3037 332b 7570 6461 7465  blink1073+update
-0000ae80: 6425 3341 3230 3232 2d30 332d 3239 2e2e  d%3A2022-03-29..
-0000ae90: 3230 3232 2d30 332d 3330 2674 7970 653d  2022-03-30&type=
-0000aea0: 4973 7375 6573 290a 0a23 2320 372e 322e  Issues)..## 7.2.
-0000aeb0: 300a 0a28 5b46 756c 6c20 4368 616e 6765  0..([Full Change
-0000aec0: 6c6f 675d 2868 7474 7073 3a2f 2f67 6974  log](https://git
-0000aed0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-0000aee0: 6a75 7079 7465 725f 636c 6965 6e74 2f63  jupyter_client/c
-0000aef0: 6f6d 7061 7265 2f76 372e 312e 322e 2e2e  ompare/v7.1.2...
-0000af00: 3039 3864 6533 6535 3162 6434 6565 3162  098de3e51bd4ee1b
-0000af10: 3161 3361 6465 6438 3839 6538 6631 3039  1a3aded889e8f109
-0000af20: 6163 3565 6666 3839 2929 0a0a 2323 2320  ac5eff89))..### 
-0000af30: 456e 6861 6e63 656d 656e 7473 206d 6164  Enhancements mad
-0000af40: 650a 0a2d 2055 7064 6174 6520 636f 6e73  e..- Update cons
-0000af50: 6f6c 6561 7070 2e70 7920 5b23 3733 335d  oleapp.py [#733]
-0000af60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000af70: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-0000af80: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-0000af90: 3733 3329 2028 5b40 796f 752d 6e2d 675d  733) ([@you-n-g]
-0000afa0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000afb0: 636f 6d2f 796f 752d 6e2d 6729 290a 0a23  com/you-n-g))..#
-0000afc0: 2323 2042 7567 7320 6669 7865 640a 0a2d  ## Bugs fixed..-
-0000afd0: 204a 736f 6e20 7061 636b 6572 3a20 6861   Json packer: ha
-0000afe0: 6e64 6c65 2054 7970 6545 7272 6f72 2061  ndle TypeError a
-0000aff0: 6e64 2066 616c 6c62 6163 6b20 746f 206f  nd fallback to o
-0000b000: 6c64 206a 736f 6e5f 636c 6561 6e20 5b23  ld json_clean [#
-0000b010: 3735 325d 2868 7474 7073 3a2f 2f67 6974  752](https://git
-0000b020: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-0000b030: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-0000b040: 756c 6c2f 3735 3229 2028 5b40 6d61 7274  ull/752) ([@mart
-0000b050: 696e 5265 6e6f 755d 2868 7474 7073 3a2f  inRenou](https:/
-0000b060: 2f67 6974 6875 622e 636f 6d2f 6d61 7274  /github.com/mart
-0000b070: 696e 5265 6e6f 7529 290a 2d20 5072 6566  inRenou)).- Pref
-0000b080: 6572 2073 656e 6469 6e67 2073 6967 6e61  er sending signa
-0000b090: 6c73 2074 6f20 6b65 726e 656c 2070 726f  ls to kernel pro
-0000b0a0: 6365 7373 2067 726f 7570 205b 2337 3433  cess group [#743
-0000b0b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000b0c0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-0000b0d0: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-0000b0e0: 2f37 3433 2920 285b 406b 6576 696e 2d62  /743) ([@kevin-b
-0000b0f0: 6174 6573 5d28 6874 7470 733a 2f2f 6769  ates](https://gi
-0000b100: 7468 7562 2e63 6f6d 2f6b 6576 696e 2d62  thub.com/kevin-b
-0000b110: 6174 6573 2929 0a0a 2323 2320 4d61 696e  ates))..### Main
-0000b120: 7465 6e61 6e63 6520 616e 6420 7570 6b65  tenance and upke
-0000b130: 6570 2069 6d70 726f 7665 6d65 6e74 730a  ep improvements.
-0000b140: 0a2d 204d 6f63 6b20 6973 206e 6f74 206e  .- Mock is not n
-0000b150: 6565 6465 6420 5b23 3735 385d 2868 7474  eeded [#758](htt
-0000b160: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000b170: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-0000b180: 636c 6965 6e74 2f70 756c 6c2f 3735 3829  client/pull/758)
-0000b190: 2028 5b40 6872 6f6e 636f 6b5d 2868 7474   ([@hroncok](htt
-0000b1a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000b1b0: 6872 6f6e 636f 6b29 290a 2d20 4164 6420  hroncok)).- Add 
-0000b1c0: 7079 7465 7374 206f 7074 7320 616e 6420  pytest opts and 
-0000b1d0: 636c 6561 6e20 7570 2077 6f72 6b66 6c6f  clean up workflo
-0000b1e0: 7773 205b 2337 3537 5d28 6874 7470 733a  ws [#757](https:
-0000b1f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-0000b200: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-0000b210: 656e 742f 7075 6c6c 2f37 3537 2920 285b  ent/pull/757) ([
-0000b220: 4062 6c69 6e6b 3130 3733 5d28 6874 7470  @blink1073](http
-0000b230: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-0000b240: 6c69 6e6b 3130 3733 2929 0a2d 2043 6c65  link1073)).- Cle
-0000b250: 616e 2075 7020 6465 7065 6e64 656e 6379  an up dependency
-0000b260: 2068 616e 646c 696e 6720 5b23 3735 305d   handling [#750]
-0000b270: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000b280: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-0000b290: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-0000b2a0: 3735 3029 2028 5b40 626c 696e 6b31 3037  750) ([@blink107
-0000b2b0: 335d 2868 7474 7073 3a2f 2f67 6974 6875  3](https://githu
-0000b2c0: 622e 636f 6d2f 626c 696e 6b31 3037 3329  b.com/blink1073)
-0000b2d0: 290a 2d20 5573 6520 6275 696c 7420 696e  ).- Use built in
-0000b2e0: 2072 756e 2063 616e 6365 6c6c 6174 696f   run cancellatio
-0000b2f0: 6e20 5b23 3734 325d 2868 7474 7073 3a2f  n [#742](https:/
-0000b300: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-0000b310: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-0000b320: 6e74 2f70 756c 6c2f 3734 3229 2028 5b40  nt/pull/742) ([@
-0000b330: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
-0000b340: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
-0000b350: 696e 6b31 3037 3329 290a 0a23 2323 2043  ink1073))..### C
-0000b360: 6f6e 7472 6962 7574 6f72 7320 746f 2074  ontributors to t
-0000b370: 6869 7320 7265 6c65 6173 650a 0a28 5b47  his release..([G
-0000b380: 6974 4875 6220 636f 6e74 7269 6275 746f  itHub contributo
-0000b390: 7273 2070 6167 6520 666f 7220 7468 6973  rs page for this
-0000b3a0: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
-0000b3b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-0000b3c0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-0000b3d0: 656e 742f 6772 6170 6873 2f63 6f6e 7472  ent/graphs/contr
-0000b3e0: 6962 7574 6f72 733f 6672 6f6d 3d32 3032  ibutors?from=202
-0000b3f0: 322d 3031 2d32 3126 746f 3d32 3032 322d  2-01-21&to=2022-
-0000b400: 3033 2d32 3826 7479 7065 3d63 2929 0a0a  03-28&type=c))..
-0000b410: 5b40 626c 696e 6b31 3037 335d 2868 7474  [@blink1073](htt
-0000b420: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000b430: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
-0000b440: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
-0000b450: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
-0000b460: 7325 3341 626c 696e 6b31 3037 332b 7570  s%3Ablink1073+up
-0000b470: 6461 7465 6425 3341 3230 3232 2d30 312d  dated%3A2022-01-
-0000b480: 3231 2e2e 3230 3232 2d30 332d 3238 2674  21..2022-03-28&t
-0000b490: 7970 653d 4973 7375 6573 2920 7c20 5b40  ype=Issues) | [@
-0000b4a0: 6461 7669 6462 726f 6368 6172 745d 2868  davidbrochart](h
-0000b4b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000b4c0: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
-0000b4d0: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
-0000b4e0: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
-0000b4f0: 7665 7325 3341 6461 7669 6462 726f 6368  ves%3Adavidbroch
-0000b500: 6172 742b 7570 6461 7465 6425 3341 3230  art+updated%3A20
-0000b510: 3232 2d30 312d 3231 2e2e 3230 3232 2d30  22-01-21..2022-0
-0000b520: 332d 3238 2674 7970 653d 4973 7375 6573  3-28&type=Issues
-0000b530: 2920 7c20 5b40 6563 6861 726c 6573 5d28  ) | [@echarles](
-0000b540: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000b550: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
-0000b560: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
-0000b570: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
-0000b580: 6c76 6573 2533 4165 6368 6172 6c65 732b  lves%3Aecharles+
-0000b590: 7570 6461 7465 6425 3341 3230 3232 2d30  updated%3A2022-0
-0000b5a0: 312d 3231 2e2e 3230 3232 2d30 332d 3238  1-21..2022-03-28
-0000b5b0: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
-0000b5c0: 5b40 6872 6f6e 636f 6b5d 2868 7474 7073  [@hroncok](https
-0000b5d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
-0000b5e0: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
-0000b5f0: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
-0000b600: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
-0000b610: 3341 6872 6f6e 636f 6b2b 7570 6461 7465  3Ahroncok+update
-0000b620: 6425 3341 3230 3232 2d30 312d 3231 2e2e  d%3A2022-01-21..
-0000b630: 3230 3232 2d30 332d 3238 2674 7970 653d  2022-03-28&type=
-0000b640: 4973 7375 6573 2920 7c20 5b40 6b65 7669  Issues) | [@kevi
-0000b650: 6e2d 6261 7465 735d 2868 7474 7073 3a2f  n-bates](https:/
-0000b660: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-0000b670: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-0000b680: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-0000b690: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-0000b6a0: 6b65 7669 6e2d 6261 7465 732b 7570 6461  kevin-bates+upda
-0000b6b0: 7465 6425 3341 3230 3232 2d30 312d 3231  ted%3A2022-01-21
-0000b6c0: 2e2e 3230 3232 2d30 332d 3238 2674 7970  ..2022-03-28&typ
-0000b6d0: 653d 4973 7375 6573 2920 7c20 5b40 6d61  e=Issues) | [@ma
-0000b6e0: 7274 696e 5265 6e6f 755d 2868 7474 7073  rtinRenou](https
-0000b6f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
-0000b700: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
-0000b710: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
-0000b720: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
-0000b730: 3341 6d61 7274 696e 5265 6e6f 752b 7570  3AmartinRenou+up
-0000b740: 6461 7465 6425 3341 3230 3232 2d30 312d  dated%3A2022-01-
-0000b750: 3231 2e2e 3230 3232 2d30 332d 3238 2674  21..2022-03-28&t
-0000b760: 7970 653d 4973 7375 6573 2920 7c20 5b40  ype=Issues) | [@
-0000b770: 796f 752d 6e2d 675d 2868 7474 7073 3a2f  you-n-g](https:/
-0000b780: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-0000b790: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-0000b7a0: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-0000b7b0: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-0000b7c0: 796f 752d 6e2d 672b 7570 6461 7465 6425  you-n-g+updated%
-0000b7d0: 3341 3230 3232 2d30 312d 3231 2e2e 3230  3A2022-01-21..20
-0000b7e0: 3232 2d30 332d 3238 2674 7970 653d 4973  22-03-28&type=Is
-0000b7f0: 7375 6573 290a 0a23 2320 372e 312e 320a  sues)..## 7.1.2.
-0000b800: 0a28 5b46 756c 6c20 4368 616e 6765 6c6f  .([Full Changelo
-0000b810: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
-0000b820: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-0000b830: 7079 7465 725f 636c 6965 6e74 2f63 6f6d  pyter_client/com
-0000b840: 7061 7265 2f76 372e 312e 312e 2e2e 3263  pare/v7.1.1...2c
-0000b850: 3966 6266 3439 3966 3633 6434 3238 3738  9fbf499f63d42878
-0000b860: 3531 3032 3162 3866 3865 6663 3964 3363  51021b8f8efc9d3c
-0000b870: 3065 3333 3665 2929 0a0a 2323 2320 4275  0e336e))..### Bu
-0000b880: 6773 2066 6978 6564 0a0a 2d20 4177 6169  gs fixed..- Awai
-0000b890: 7420 606b 6572 6e65 6c2e 7265 6164 7960  t `kernel.ready`
-0000b8a0: 2069 6e20 605f 6173 796e 635f 7368 7574   in `_async_shut
-0000b8b0: 646f 776e 5f6b 6572 6e65 6c60 205b 2337  down_kernel` [#7
-0000b8c0: 3430 5d28 6874 7470 733a 2f2f 6769 7468  40](https://gith
-0000b8d0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-0000b8e0: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-0000b8f0: 6c6c 2f37 3430 2920 285b 406a 7470 696f  ll/740) ([@jtpio
-0000b900: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000b910: 2e63 6f6d 2f6a 7470 696f 2929 0a0a 2323  .com/jtpio))..##
-0000b920: 2320 436f 6e74 7269 6275 746f 7273 2074  # Contributors t
-0000b930: 6f20 7468 6973 2072 656c 6561 7365 0a0a  o this release..
-0000b940: 285b 4769 7448 7562 2063 6f6e 7472 6962  ([GitHub contrib
-0000b950: 7574 6f72 7320 7061 6765 2066 6f72 2074  utors page for t
-0000b960: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
-0000b970: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000b980: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-0000b990: 636c 6965 6e74 2f67 7261 7068 732f 636f  client/graphs/co
-0000b9a0: 6e74 7269 6275 746f 7273 3f66 726f 6d3d  ntributors?from=
-0000b9b0: 3230 3232 2d30 312d 3134 2674 6f3d 3230  2022-01-14&to=20
-0000b9c0: 3232 2d30 312d 3231 2674 7970 653d 6329  22-01-21&type=c)
-0000b9d0: 290a 0a5b 406a 7470 696f 5d28 6874 7470  )..[@jtpio](http
-0000b9e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-0000b9f0: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
-0000ba00: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
-0000ba10: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
-0000ba20: 2533 416a 7470 696f 2b75 7064 6174 6564  %3Ajtpio+updated
-0000ba30: 2533 4132 3032 322d 3031 2d31 342e 2e32  %3A2022-01-14..2
-0000ba40: 3032 322d 3031 2d32 3126 7479 7065 3d49  022-01-21&type=I
-0000ba50: 7373 7565 7329 207c 205b 405a 7361 696c  ssues) | [@Zsail
-0000ba60: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
-0000ba70: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
-0000ba80: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
-0000ba90: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
-0000baa0: 696e 766f 6c76 6573 2533 415a 7361 696c  involves%3AZsail
-0000bab0: 6572 2b75 7064 6174 6564 2533 4132 3032  er+updated%3A202
-0000bac0: 322d 3031 2d31 342e 2e32 3032 322d 3031  2-01-14..2022-01
-0000bad0: 2d32 3126 7479 7065 3d49 7373 7565 7329  -21&type=Issues)
-0000bae0: 0a0a 2323 2037 2e31 2e31 0a0a 285b 4675  ..## 7.1.1..([Fu
-0000baf0: 6c6c 2043 6861 6e67 656c 6f67 5d28 6874  ll Changelog](ht
-0000bb00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000bb10: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-0000bb20: 5f63 6c69 656e 742f 636f 6d70 6172 652f  _client/compare/
-0000bb30: 7637 2e31 2e30 2e2e 2e34 3432 3837 3135  v7.1.0...4428715
-0000bb40: 6236 3537 3431 6464 6363 6163 3933 3035  b65741ddccac9305
-0000bb50: 6433 3138 6434 6163 6530 3866 6137 3131  d318d4ace08fa711
-0000bb60: 6129 290a 0a23 2323 2045 6e68 616e 6365  a))..### Enhance
-0000bb70: 6d65 6e74 7320 6d61 6465 0a0a 2d20 4675  ments made..- Fu
-0000bb80: 7274 6865 7220 696d 7072 6f76 656d 656e  rther improvemen
-0000bb90: 7473 2074 6f20 7065 6e64 696e 6720 6b65  ts to pending ke
-0000bba0: 726e 656c 7320 6d61 6e61 6765 6d65 6e74  rnels management
-0000bbb0: 205b 2337 3332 5d28 6874 7470 733a 2f2f   [#732](https://
-0000bbc0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-0000bbd0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-0000bbe0: 742f 7075 6c6c 2f37 3332 2920 285b 405a  t/pull/732) ([@Z
-0000bbf0: 7361 696c 6572 5d28 6874 7470 733a 2f2f  sailer](https://
-0000bc00: 6769 7468 7562 2e63 6f6d 2f5a 7361 696c  github.com/Zsail
-0000bc10: 6572 2929 0a0a 2323 2320 4d61 696e 7465  er))..### Mainte
-0000bc20: 6e61 6e63 6520 616e 6420 7570 6b65 6570  nance and upkeep
-0000bc30: 2069 6d70 726f 7665 6d65 6e74 730a 0a2d   improvements..-
-0000bc40: 2054 6573 7420 6167 6169 6e73 7420 616c   Test against al
-0000bc50: 6c20 6b65 726e 656c 7320 696e 206a 7570  l kernels in jup
-0000bc60: 7974 6572 206b 6572 6e65 6c20 7465 7374  yter kernel test
-0000bc70: 2061 6e64 2063 6c65 616e 2075 7020 4349   and clean up CI
-0000bc80: 205b 2337 3331 5d28 6874 7470 733a 2f2f   [#731](https://
-0000bc90: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-0000bca0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-0000bcb0: 742f 7075 6c6c 2f37 3331 2920 285b 4062  t/pull/731) ([@b
-0000bcc0: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
-0000bcd0: 2f2f 6769 7468 7562 2e63 6f6d 2f62 6c69  //github.com/bli
-0000bce0: 6e6b 3130 3733 2929 0a2d 2052 6570 6c61  nk1073)).- Repla
-0000bcf0: 6365 206d 6173 7465 7220 7769 7468 206d  ce master with m
-0000bd00: 6169 6e20 5b23 3732 395d 2868 7474 7073  ain [#729](https
-0000bd10: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-0000bd20: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-0000bd30: 6965 6e74 2f70 756c 6c2f 3732 3929 2028  ient/pull/729) (
-0000bd40: 5b40 6461 7669 6462 726f 6368 6172 745d  [@davidbrochart]
-0000bd50: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000bd60: 636f 6d2f 6461 7669 6462 726f 6368 6172  com/davidbrochar
-0000bd70: 7429 290a 0a23 2323 2044 6f63 756d 656e  t))..### Documen
-0000bd80: 7461 7469 6f6e 2069 6d70 726f 7665 6d65  tation improveme
-0000bd90: 6e74 730a 0a2d 205c 5b44 4f43 5c5d 2069  nts..- \[DOC\] i
-0000bda0: 6d70 726f 7665 206b 6572 6e65 6c20 7072  mprove kernel pr
-0000bdb0: 6f76 6973 696f 6e65 7220 646f 6320 5b23  ovisioner doc [#
-0000bdc0: 3733 305d 2868 7474 7073 3a2f 2f67 6974  730](https://git
-0000bdd0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-0000bde0: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-0000bdf0: 756c 6c2f 3733 3029 2028 5b40 6162 7a79  ull/730) ([@abzy
-0000be00: 6d65 696e 736a 7475 5d28 6874 7470 733a  meinsjtu](https:
-0000be10: 2f2f 6769 7468 7562 2e63 6f6d 2f61 627a  //github.com/abz
-0000be20: 796d 6569 6e73 6a74 7529 290a 2d20 6164  ymeinsjtu)).- ad
-0000be30: 6420 6368 616e 6765 6c6f 6720 666f 7220  d changelog for 
-0000be40: 6d65 7373 6167 6520 7370 6563 205b 2335  message spec [#5
-0000be50: 3235 5d28 6874 7470 733a 2f2f 6769 7468  25](https://gith
-0000be60: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-0000be70: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-0000be80: 6c6c 2f35 3235 2920 285b 406d 696e 726b  ll/525) ([@minrk
-0000be90: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000bea0: 2e63 6f6d 2f6d 696e 726b 2929 0a0a 2323  .com/minrk))..##
-0000beb0: 2320 436f 6e74 7269 6275 746f 7273 2074  # Contributors t
-0000bec0: 6f20 7468 6973 2072 656c 6561 7365 0a0a  o this release..
-0000bed0: 285b 4769 7448 7562 2063 6f6e 7472 6962  ([GitHub contrib
-0000bee0: 7574 6f72 7320 7061 6765 2066 6f72 2074  utors page for t
-0000bef0: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
-0000bf00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000bf10: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-0000bf20: 636c 6965 6e74 2f67 7261 7068 732f 636f  client/graphs/co
-0000bf30: 6e74 7269 6275 746f 7273 3f66 726f 6d3d  ntributors?from=
-0000bf40: 3230 3231 2d31 312d 3232 2674 6f3d 3230  2021-11-22&to=20
-0000bf50: 3232 2d30 312d 3134 2674 7970 653d 6329  22-01-14&type=c)
-0000bf60: 290a 0a5b 4061 627a 796d 6569 6e73 6a74  )..[@abzymeinsjt
-0000bf70: 755d 2868 7474 7073 3a2f 2f67 6974 6875  u](https://githu
-0000bf80: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
-0000bf90: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
-0000bfa0: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
-0000bfb0: 6e76 6f6c 7665 7325 3341 6162 7a79 6d65  nvolves%3Aabzyme
-0000bfc0: 696e 736a 7475 2b75 7064 6174 6564 2533  insjtu+updated%3
-0000bfd0: 4132 3032 312d 3131 2d32 322e 2e32 3032  A2021-11-22..202
-0000bfe0: 322d 3031 2d31 3426 7479 7065 3d49 7373  2-01-14&type=Iss
-0000bff0: 7565 7329 207c 205b 4062 6c69 6e6b 3130  ues) | [@blink10
-0000c000: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
-0000c010: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
-0000c020: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
-0000c030: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
-0000c040: 696e 766f 6c76 6573 2533 4162 6c69 6e6b  involves%3Ablink
-0000c050: 3130 3733 2b75 7064 6174 6564 2533 4132  1073+updated%3A2
-0000c060: 3032 312d 3131 2d32 322e 2e32 3032 322d  021-11-22..2022-
-0000c070: 3031 2d31 3426 7479 7065 3d49 7373 7565  01-14&type=Issue
-0000c080: 7329 207c 205b 4042 6f50 656e 675d 2868  s) | [@BoPeng](h
-0000c090: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000c0a0: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
-0000c0b0: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
-0000c0c0: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
-0000c0d0: 7665 7325 3341 426f 5065 6e67 2b75 7064  ves%3ABoPeng+upd
-0000c0e0: 6174 6564 2533 4132 3032 312d 3131 2d32  ated%3A2021-11-2
-0000c0f0: 322e 2e32 3032 322d 3031 2d31 3426 7479  2..2022-01-14&ty
-0000c100: 7065 3d49 7373 7565 7329 207c 205b 4064  pe=Issues) | [@d
-0000c110: 6176 6964 6272 6f63 6861 7274 5d28 6874  avidbrochart](ht
-0000c120: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000c130: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
-0000c140: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
-0000c150: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
-0000c160: 6573 2533 4164 6176 6964 6272 6f63 6861  es%3Adavidbrocha
-0000c170: 7274 2b75 7064 6174 6564 2533 4132 3032  rt+updated%3A202
-0000c180: 312d 3131 2d32 322e 2e32 3032 322d 3031  1-11-22..2022-01
-0000c190: 2d31 3426 7479 7065 3d49 7373 7565 7329  -14&type=Issues)
-0000c1a0: 207c 205b 406d 696e 726b 5d28 6874 7470   | [@minrk](http
-0000c1b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-0000c1c0: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
-0000c1d0: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
-0000c1e0: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
-0000c1f0: 2533 416d 696e 726b 2b75 7064 6174 6564  %3Aminrk+updated
-0000c200: 2533 4132 3032 312d 3131 2d32 322e 2e32  %3A2021-11-22..2
-0000c210: 3032 322d 3031 2d31 3426 7479 7065 3d49  022-01-14&type=I
-0000c220: 7373 7565 7329 207c 205b 4072 6762 6b72  ssues) | [@rgbkr
-0000c230: 6b5d 2868 7474 7073 3a2f 2f67 6974 6875  k](https://githu
-0000c240: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
-0000c250: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
-0000c260: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
-0000c270: 6e76 6f6c 7665 7325 3341 7267 626b 726b  nvolves%3Argbkrk
-0000c280: 2b75 7064 6174 6564 2533 4132 3032 312d  +updated%3A2021-
-0000c290: 3131 2d32 322e 2e32 3032 322d 3031 2d31  11-22..2022-01-1
-0000c2a0: 3426 7479 7065 3d49 7373 7565 7329 207c  4&type=Issues) |
-0000c2b0: 205b 4077 696c 6c69 6e67 635d 2868 7474   [@willingc](htt
-0000c2c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000c2d0: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
-0000c2e0: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
-0000c2f0: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
-0000c300: 7325 3341 7769 6c6c 696e 6763 2b75 7064  s%3Awillingc+upd
-0000c310: 6174 6564 2533 4132 3032 312d 3131 2d32  ated%3A2021-11-2
-0000c320: 322e 2e32 3032 322d 3031 2d31 3426 7479  2..2022-01-14&ty
-0000c330: 7065 3d49 7373 7565 7329 207c 205b 405a  pe=Issues) | [@Z
-0000c340: 7361 696c 6572 5d28 6874 7470 733a 2f2f  sailer](https://
-0000c350: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
-0000c360: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
-0000c370: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
-0000c380: 656e 742b 696e 766f 6c76 6573 2533 415a  ent+involves%3AZ
-0000c390: 7361 696c 6572 2b75 7064 6174 6564 2533  sailer+updated%3
-0000c3a0: 4132 3032 312d 3131 2d32 322e 2e32 3032  A2021-11-22..202
-0000c3b0: 322d 3031 2d31 3426 7479 7065 3d49 7373  2-01-14&type=Iss
-0000c3c0: 7565 7329 0a0a 2323 2037 2e31 2e30 0a0a  ues)..## 7.1.0..
-0000c3d0: 285b 4675 6c6c 2043 6861 6e67 656c 6f67  ([Full Changelog
-0000c3e0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000c3f0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-0000c400: 7974 6572 5f63 6c69 656e 742f 636f 6d70  yter_client/comp
-0000c410: 6172 652f 7637 2e30 2e36 2e2e 2e36 6237  are/v7.0.6...6b7
-0000c420: 3636 3033 3537 3866 6433 6137 3666 6435  6603578fd3a76fd5
-0000c430: 3737 6433 3331 3933 3933 6339 3933 3366  77d3319393c9933f
-0000c440: 3533 6162 3029 290a 0a23 2323 2045 6e68  53ab0))..### Enh
-0000c450: 616e 6365 6d65 6e74 7320 6d61 6465 0a0a  ancements made..
-0000c460: 2d20 4164 6420 7375 7070 6f72 7420 666f  - Add support fo
-0000c470: 7220 7065 6e64 696e 6720 6b65 726e 656c  r pending kernel
-0000c480: 7320 5b23 3731 325d 2868 7474 7073 3a2f  s [#712](https:/
-0000c490: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-0000c4a0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-0000c4b0: 6e74 2f70 756c 6c2f 3731 3229 2028 5b40  nt/pull/712) ([@
-0000c4c0: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
-0000c4d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
-0000c4e0: 696e 6b31 3037 3329 290a 0a23 2323 2042  ink1073))..### B
-0000c4f0: 7567 7320 6669 7865 640a 0a2d 2049 6d70  ugs fixed..- Imp
-0000c500: 726f 7665 2072 6573 7461 7274 6572 206c  rove restarter l
-0000c510: 6f67 6963 205b 2337 3137 5d28 6874 7470  ogic [#717](http
-0000c520: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-0000c530: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-0000c540: 6c69 656e 742f 7075 6c6c 2f37 3137 2920  lient/pull/717) 
-0000c550: 285b 4076 6964 6172 7466 5d28 6874 7470  ([@vidartf](http
-0000c560: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f76  s://github.com/v
-0000c570: 6964 6172 7466 2929 0a2d 2053 6574 2073  idartf)).- Set s
-0000c580: 7469 636b 7920 6269 7420 6f6e 6c79 206f  ticky bit only o
-0000c590: 6e20 7468 6520 6469 7265 6374 6f72 7920  n the directory 
-0000c5a0: 5b23 3731 315d 2868 7474 7073 3a2f 2f67  [#711](https://g
-0000c5b0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
-0000c5c0: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
-0000c5d0: 2f70 756c 6c2f 3731 3129 2028 5b40 6369  /pull/711) ([@ci
-0000c5e0: 3469 6334 5d28 6874 7470 733a 2f2f 6769  4ic4](https://gi
-0000c5f0: 7468 7562 2e63 6f6d 2f63 6934 6963 3429  thub.com/ci4ic4)
-0000c600: 290a 0a23 2323 204d 6169 6e74 656e 616e  )..### Maintenan
-0000c610: 6365 2061 6e64 2075 706b 6565 7020 696d  ce and upkeep im
-0000c620: 7072 6f76 656d 656e 7473 0a0a 2d20 456e  provements..- En
-0000c630: 666f 7263 6520 6c61 6265 6c73 206f 6e20  force labels on 
-0000c640: 5052 7320 5b23 3732 305d 2868 7474 7073  PRs [#720](https
-0000c650: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-0000c660: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-0000c670: 6965 6e74 2f70 756c 6c2f 3732 3029 2028  ient/pull/720) (
-0000c680: 5b40 626c 696e 6b31 3037 335d 2868 7474  [@blink1073](htt
-0000c690: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000c6a0: 626c 696e 6b31 3037 3329 290a 0a23 2323  blink1073))..###
-0000c6b0: 2043 6f6e 7472 6962 7574 6f72 7320 746f   Contributors to
-0000c6c0: 2074 6869 7320 7265 6c65 6173 650a 0a28   this release..(
-0000c6d0: 5b47 6974 4875 6220 636f 6e74 7269 6275  [GitHub contribu
-0000c6e0: 746f 7273 2070 6167 6520 666f 7220 7468  tors page for th
-0000c6f0: 6973 2072 656c 6561 7365 5d28 6874 7470  is release](http
-0000c700: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-0000c710: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-0000c720: 6c69 656e 742f 6772 6170 6873 2f63 6f6e  lient/graphs/con
-0000c730: 7472 6962 7574 6f72 733f 6672 6f6d 3d32  tributors?from=2
-0000c740: 3032 312d 3130 2d30 3126 746f 3d32 3032  021-10-01&to=202
-0000c750: 312d 3131 2d32 3226 7479 7065 3d63 2929  1-11-22&type=c))
-0000c760: 0a0a 5b40 626c 696e 6b31 3037 335d 2868  ..[@blink1073](h
-0000c770: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000c780: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
-0000c790: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
-0000c7a0: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
-0000c7b0: 7665 7325 3341 626c 696e 6b31 3037 332b  ves%3Ablink1073+
-0000c7c0: 7570 6461 7465 6425 3341 3230 3231 2d31  updated%3A2021-1
-0000c7d0: 302d 3031 2e2e 3230 3231 2d31 312d 3232  0-01..2021-11-22
-0000c7e0: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
-0000c7f0: 5b40 6369 3469 6334 5d28 6874 7470 733a  [@ci4ic4](https:
-0000c800: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
-0000c810: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
-0000c820: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
-0000c830: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
-0000c840: 4163 6934 6963 342b 7570 6461 7465 6425  Aci4ic4+updated%
-0000c850: 3341 3230 3231 2d31 302d 3031 2e2e 3230  3A2021-10-01..20
-0000c860: 3231 2d31 312d 3232 2674 7970 653d 4973  21-11-22&type=Is
-0000c870: 7375 6573 2920 7c20 5b40 6461 7669 6462  sues) | [@davidb
-0000c880: 726f 6368 6172 745d 2868 7474 7073 3a2f  rochart](https:/
-0000c890: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-0000c8a0: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-0000c8b0: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-0000c8c0: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-0000c8d0: 6461 7669 6462 726f 6368 6172 742b 7570  davidbrochart+up
-0000c8e0: 6461 7465 6425 3341 3230 3231 2d31 302d  dated%3A2021-10-
-0000c8f0: 3031 2e2e 3230 3231 2d31 312d 3232 2674  01..2021-11-22&t
-0000c900: 7970 653d 4973 7375 6573 2920 7c20 5b40  ype=Issues) | [@
-0000c910: 6b65 7669 6e2d 6261 7465 735d 2868 7474  kevin-bates](htt
-0000c920: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000c930: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
-0000c940: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
-0000c950: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
-0000c960: 7325 3341 6b65 7669 6e2d 6261 7465 732b  s%3Akevin-bates+
-0000c970: 7570 6461 7465 6425 3341 3230 3231 2d31  updated%3A2021-1
-0000c980: 302d 3031 2e2e 3230 3231 2d31 312d 3232  0-01..2021-11-22
-0000c990: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
-0000c9a0: 5b40 7669 6461 7274 665d 2868 7474 7073  [@vidartf](https
-0000c9b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
-0000c9c0: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
-0000c9d0: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
-0000c9e0: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
-0000c9f0: 3341 7669 6461 7274 662b 7570 6461 7465  3Avidartf+update
-0000ca00: 6425 3341 3230 3231 2d31 302d 3031 2e2e  d%3A2021-10-01..
-0000ca10: 3230 3231 2d31 312d 3232 2674 7970 653d  2021-11-22&type=
-0000ca20: 4973 7375 6573 290a 0a23 2320 372e 302e  Issues)..## 7.0.
-0000ca30: 360a 0a28 5b46 756c 6c20 4368 616e 6765  6..([Full Change
-0000ca40: 6c6f 675d 2868 7474 7073 3a2f 2f67 6974  log](https://git
-0000ca50: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-0000ca60: 6a75 7079 7465 725f 636c 6965 6e74 2f63  jupyter_client/c
-0000ca70: 6f6d 7061 7265 2f76 372e 302e 352e 2e2e  ompare/v7.0.5...
-0000ca80: 3538 6231 3164 6630 6563 6237 3239 6566  58b11df0ecb729ef
-0000ca90: 6661 6363 3539 6365 3238 6539 6634 3331  facc59ce28e9f431
-0000caa0: 6661 3963 3661 3464 2929 0a0a 2323 2320  fa9c6a4d))..### 
-0000cab0: 4275 6773 2066 6978 6564 0a0a 2d20 4661  Bugs fixed..- Fa
-0000cac0: 6c6c 6261 636b 2074 6f20 7468 6520 6f6c  llback to the ol
-0000cad0: 6420 6970 796b 6572 6e65 6c20 226a 736f  d ipykernel "jso
-0000cae0: 6e5f 636c 6561 6e22 2069 6620 7765 2061  n_clean" if we a
-0000caf0: 7265 206e 6f74 2061 626c 6520 746f 2073  re not able to s
-0000cb00: 6572 6961 6c69 7a65 2061 204a 534f 4e20  erialize a JSON 
-0000cb10: 6d65 7373 6167 6520 5b23 3730 385d 2868  message [#708](h
-0000cb20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000cb30: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-0000cb40: 725f 636c 6965 6e74 2f70 756c 6c2f 3730  r_client/pull/70
-0000cb50: 3829 2028 5b40 6d61 7274 696e 5265 6e6f  8) ([@martinReno
-0000cb60: 755d 2868 7474 7073 3a2f 2f67 6974 6875  u](https://githu
-0000cb70: 622e 636f 6d2f 6d61 7274 696e 5265 6e6f  b.com/martinReno
-0000cb80: 7529 290a 0a23 2323 204f 7468 6572 206d  u))..### Other m
-0000cb90: 6572 6765 6420 5052 730a 0a2d 2041 6464  erged PRs..- Add
-0000cba0: 2074 6573 7420 666f 7220 7365 7269 616c   test for serial
-0000cbb0: 697a 696e 6720 6279 7465 7320 5b23 3730  izing bytes [#70
-0000cbc0: 375d 2868 7474 7073 3a2f 2f67 6974 6875  7](https://githu
-0000cbd0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-0000cbe0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-0000cbf0: 6c2f 3730 3729 2028 5b40 6d61 7274 696e  l/707) ([@martin
-0000cc00: 5265 6e6f 755d 2868 7474 7073 3a2f 2f67  Renou](https://g
-0000cc10: 6974 6875 622e 636f 6d2f 6d61 7274 696e  ithub.com/martin
-0000cc20: 5265 6e6f 7529 290a 0a23 2323 2043 6f6e  Renou))..### Con
-0000cc30: 7472 6962 7574 6f72 7320 746f 2074 6869  tributors to thi
-0000cc40: 7320 7265 6c65 6173 650a 0a28 5b47 6974  s release..([Git
-0000cc50: 4875 6220 636f 6e74 7269 6275 746f 7273  Hub contributors
-0000cc60: 2070 6167 6520 666f 7220 7468 6973 2072   page for this r
-0000cc70: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
-0000cc80: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-0000cc90: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-0000cca0: 742f 6772 6170 6873 2f63 6f6e 7472 6962  t/graphs/contrib
-0000ccb0: 7574 6f72 733f 6672 6f6d 3d32 3032 312d  utors?from=2021-
-0000ccc0: 3039 2d32 3926 746f 3d32 3032 312d 3130  09-29&to=2021-10
-0000ccd0: 2d30 3126 7479 7065 3d63 2929 0a0a 5b40  -01&type=c))..[@
-0000cce0: 6d61 7274 696e 5265 6e6f 755d 2868 7474  martinRenou](htt
-0000ccf0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000cd00: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
-0000cd10: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
-0000cd20: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
-0000cd30: 7325 3341 6d61 7274 696e 5265 6e6f 752b  s%3AmartinRenou+
-0000cd40: 7570 6461 7465 6425 3341 3230 3231 2d30  updated%3A2021-0
-0000cd50: 392d 3239 2e2e 3230 3231 2d31 302d 3031  9-29..2021-10-01
-0000cd60: 2674 7970 653d 4973 7375 6573 290a 0a23  &type=Issues)..#
-0000cd70: 2320 372e 302e 350a 0a28 5b46 756c 6c20  # 7.0.5..([Full 
-0000cd80: 4368 616e 6765 6c6f 675d 2868 7474 7073  Changelog](https
-0000cd90: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-0000cda0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-0000cdb0: 6965 6e74 2f63 6f6d 7061 7265 2f76 372e  ient/compare/v7.
-0000cdc0: 302e 342e 2e2e 6533 3739 6266 3931 6665  0.4...e379bf91fe
-0000cdd0: 6136 3335 3236 6239 6334 6363 3636 3739  a63526b9c4cc6679
-0000cde0: 6537 3935 3361 3332 3562 3534 3063 2929  e7953a325b540c))
-0000cdf0: 0a0a 2323 2320 4275 6773 2066 6978 6564  ..### Bugs fixed
-0000ce00: 0a0a 2d20 6176 6f69 6420 7573 6520 6f66  ..- avoid use of
-0000ce10: 2064 6570 7265 6361 7465 6420 7a6d 712e   deprecated zmq.
-0000ce20: 7574 696c 732e 6a73 6f6e 6170 6920 5b23  utils.jsonapi [#
-0000ce30: 3730 335d 2868 7474 7073 3a2f 2f67 6974  703](https://git
-0000ce40: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-0000ce50: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-0000ce60: 756c 6c2f 3730 3329 2028 5b40 6d69 6e72  ull/703) ([@minr
-0000ce70: 6b5d 2868 7474 7073 3a2f 2f67 6974 6875  k](https://githu
-0000ce80: 622e 636f 6d2f 6d69 6e72 6b29 290a 0a23  b.com/minrk))..#
-0000ce90: 2323 204d 6169 6e74 656e 616e 6365 2061  ## Maintenance a
-0000cea0: 6e64 2075 706b 6565 7020 696d 7072 6f76  nd upkeep improv
-0000ceb0: 656d 656e 7473 0a0a 2d20 5573 6520 6c6f  ements..- Use lo
-0000cec0: 6767 6572 2e77 6172 6e69 6e67 2069 6e73  gger.warning ins
-0000ced0: 7465 6164 206f 6620 6465 7072 6563 6174  tead of deprecat
-0000cee0: 6564 2077 6172 6e20 6d65 7468 6f64 205b  ed warn method [
-0000cef0: 2337 3030 5d28 6874 7470 733a 2f2f 6769  #700](https://gi
-0000cf00: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-0000cf10: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-0000cf20: 7075 6c6c 2f37 3030 2920 285b 406b 6576  pull/700) ([@kev
-0000cf30: 696e 2d62 6174 6573 5d28 6874 7470 733a  in-bates](https:
-0000cf40: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 6576  //github.com/kev
-0000cf50: 696e 2d62 6174 6573 2929 0a0a 2323 2320  in-bates))..### 
-0000cf60: 436f 6e74 7269 6275 746f 7273 2074 6f20  Contributors to 
-0000cf70: 7468 6973 2072 656c 6561 7365 0a0a 285b  this release..([
-0000cf80: 4769 7448 7562 2063 6f6e 7472 6962 7574  GitHub contribut
-0000cf90: 6f72 7320 7061 6765 2066 6f72 2074 6869  ors page for thi
-0000cfa0: 7320 7265 6c65 6173 655d 2868 7474 7073  s release](https
-0000cfb0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-0000cfc0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-0000cfd0: 6965 6e74 2f67 7261 7068 732f 636f 6e74  ient/graphs/cont
-0000cfe0: 7269 6275 746f 7273 3f66 726f 6d3d 3230  ributors?from=20
-0000cff0: 3231 2d30 392d 3238 2674 6f3d 3230 3231  21-09-28&to=2021
-0000d000: 2d30 392d 3239 2674 7970 653d 6329 290a  -09-29&type=c)).
-0000d010: 0a5b 406b 6576 696e 2d62 6174 6573 5d28  .[@kevin-bates](
+0000ad30: 756c 6c2f 3737 3329 2028 5b40 7072 652d  ull/773) ([@pre-
+0000ad40: 636f 6d6d 6974 2d63 695d 2868 7474 7073  commit-ci](https
+0000ad50: 3a2f 2f67 6974 6875 622e 636f 6d2f 7072  ://github.com/pr
+0000ad60: 652d 636f 6d6d 6974 2d63 6929 290a 2d20  e-commit-ci)).- 
+0000ad70: 5c5b 7072 652d 636f 6d6d 6974 2e63 695c  \[pre-commit.ci\
+0000ad80: 5d20 7072 652d 636f 6d6d 6974 2061 7574  ] pre-commit aut
+0000ad90: 6f75 7064 6174 6520 5b23 3737 305d 2868  oupdate [#770](h
+0000ada0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000adb0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+0000adc0: 725f 636c 6965 6e74 2f70 756c 6c2f 3737  r_client/pull/77
+0000add0: 3029 2028 5b40 7072 652d 636f 6d6d 6974  0) ([@pre-commit
+0000ade0: 2d63 695d 2868 7474 7073 3a2f 2f67 6974  -ci](https://git
+0000adf0: 6875 622e 636f 6d2f 7072 652d 636f 6d6d  hub.com/pre-comm
+0000ae00: 6974 2d63 6929 290a 2d20 496d 7072 6f76  it-ci)).- Improv
+0000ae10: 6520 6d79 7079 2063 6f6e 6669 6720 5b23  e mypy config [#
+0000ae20: 3736 395d 2868 7474 7073 3a2f 2f67 6974  769](https://git
+0000ae30: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+0000ae40: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+0000ae50: 756c 6c2f 3736 3929 2028 5b40 626c 696e  ull/769) ([@blin
+0000ae60: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
+0000ae70: 6974 6875 622e 636f 6d2f 626c 696e 6b31  ithub.com/blink1
+0000ae80: 3037 3329 290a 2d20 436c 6561 6e20 7570  073)).- Clean up
+0000ae90: 2070 7265 2d63 6f6d 6d69 7420 5b23 3736   pre-commit [#76
+0000aea0: 385d 2868 7474 7073 3a2f 2f67 6974 6875  8](https://githu
+0000aeb0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+0000aec0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+0000aed0: 6c2f 3736 3829 2028 5b40 626c 696e 6b31  l/768) ([@blink1
+0000aee0: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
+0000aef0: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
+0000af00: 3329 290a 0a23 2323 2043 6f6e 7472 6962  3))..### Contrib
+0000af10: 7574 6f72 7320 746f 2074 6869 7320 7265  utors to this re
+0000af20: 6c65 6173 650a 0a28 5b47 6974 4875 6220  lease..([GitHub 
+0000af30: 636f 6e74 7269 6275 746f 7273 2070 6167  contributors pag
+0000af40: 6520 666f 7220 7468 6973 2072 656c 6561  e for this relea
+0000af50: 7365 5d28 6874 7470 733a 2f2f 6769 7468  se](https://gith
+0000af60: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+0000af70: 7570 7974 6572 5f63 6c69 656e 742f 6772  upyter_client/gr
+0000af80: 6170 6873 2f63 6f6e 7472 6962 7574 6f72  aphs/contributor
+0000af90: 733f 6672 6f6d 3d32 3032 322d 3034 2d30  s?from=2022-04-0
+0000afa0: 3726 746f 3d32 3032 322d 3034 2d32 3526  7&to=2022-04-25&
+0000afb0: 7479 7065 3d63 2929 0a0a 5b40 626c 696e  type=c))..[@blin
+0000afc0: 6b31 3037 335d 2868 7474 7073 3a2f 2f67  k1073](https://g
+0000afd0: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+0000afe0: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+0000aff0: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+0000b000: 6e74 2b69 6e76 6f6c 7665 7325 3341 626c  nt+involves%3Abl
+0000b010: 696e 6b31 3037 332b 7570 6461 7465 6425  ink1073+updated%
+0000b020: 3341 3230 3232 2d30 342d 3037 2e2e 3230  3A2022-04-07..20
+0000b030: 3232 2d30 342d 3235 2674 7970 653d 4973  22-04-25&type=Is
+0000b040: 7375 6573 2920 7c20 5b40 7072 652d 636f  sues) | [@pre-co
+0000b050: 6d6d 6974 2d63 695d 2868 7474 7073 3a2f  mmit-ci](https:/
+0000b060: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
+0000b070: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
+0000b080: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
+0000b090: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
+0000b0a0: 7072 652d 636f 6d6d 6974 2d63 692b 7570  pre-commit-ci+up
+0000b0b0: 6461 7465 6425 3341 3230 3232 2d30 342d  dated%3A2022-04-
+0000b0c0: 3037 2e2e 3230 3232 2d30 342d 3235 2674  07..2022-04-25&t
+0000b0d0: 7970 653d 4973 7375 6573 290a 0a23 2320  ype=Issues)..## 
+0000b0e0: 372e 322e 320a 0a28 5b46 756c 6c20 4368  7.2.2..([Full Ch
+0000b0f0: 616e 6765 6c6f 675d 2868 7474 7073 3a2f  angelog](https:/
+0000b100: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+0000b110: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+0000b120: 6e74 2f63 6f6d 7061 7265 2f76 372e 322e  nt/compare/v7.2.
+0000b130: 312e 2e2e 3031 6232 3039 3564 3936 6338  1...01b2095d96c8
+0000b140: 3163 3536 6564 6638 6635 6466 3434 6531  1c56edf8f5df44e1
+0000b150: 3265 3437 3662 3262 6364 3837 2929 0a0a  2e476b2bcd87))..
+0000b160: 2323 2320 4d61 696e 7465 6e61 6e63 6520  ### Maintenance 
+0000b170: 616e 6420 7570 6b65 6570 2069 6d70 726f  and upkeep impro
+0000b180: 7665 6d65 6e74 730a 0a2d 2049 6e63 6c75  vements..- Inclu
+0000b190: 6465 2070 792e 7479 7065 6420 6669 6c65  de py.typed file
+0000b1a0: 205b 2337 3636 5d28 6874 7470 733a 2f2f   [#766](https://
+0000b1b0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+0000b1c0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+0000b1d0: 742f 7075 6c6c 2f37 3636 2920 285b 4062  t/pull/766) ([@b
+0000b1e0: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
+0000b1f0: 2f2f 6769 7468 7562 2e63 6f6d 2f62 6c69  //github.com/bli
+0000b200: 6e6b 3130 3733 2929 0a2d 205c 5b70 7265  nk1073)).- \[pre
+0000b210: 2d63 6f6d 6d69 742e 6369 5c5d 2070 7265  -commit.ci\] pre
+0000b220: 2d63 6f6d 6d69 7420 6175 746f 7570 6461  -commit autoupda
+0000b230: 7465 205b 2337 3635 5d28 6874 7470 733a  te [#765](https:
+0000b240: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+0000b250: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+0000b260: 656e 742f 7075 6c6c 2f37 3635 2920 285b  ent/pull/765) ([
+0000b270: 4070 7265 2d63 6f6d 6d69 742d 6369 5d28  @pre-commit-ci](
+0000b280: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000b290: 6f6d 2f70 7265 2d63 6f6d 6d69 742d 6369  om/pre-commit-ci
+0000b2a0: 2929 0a2d 204d 6f72 6520 436c 6561 6e75  )).- More Cleanu
+0000b2b0: 7020 5b23 3736 345d 2868 7474 7073 3a2f  p [#764](https:/
+0000b2c0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+0000b2d0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+0000b2e0: 6e74 2f70 756c 6c2f 3736 3429 2028 5b40  nt/pull/764) ([@
+0000b2f0: 626c 696e 6b31 3037 335d 2868 7474 7073  blink1073](https
+0000b300: 3a2f 2f67 6974 6875 622e 636f 6d2f 626c  ://github.com/bl
+0000b310: 696e 6b31 3037 3329 290a 0a23 2323 2043  ink1073))..### C
+0000b320: 6f6e 7472 6962 7574 6f72 7320 746f 2074  ontributors to t
+0000b330: 6869 7320 7265 6c65 6173 650a 0a28 5b47  his release..([G
+0000b340: 6974 4875 6220 636f 6e74 7269 6275 746f  itHub contributo
+0000b350: 7273 2070 6167 6520 666f 7220 7468 6973  rs page for this
+0000b360: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
+0000b370: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+0000b380: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+0000b390: 656e 742f 6772 6170 6873 2f63 6f6e 7472  ent/graphs/contr
+0000b3a0: 6962 7574 6f72 733f 6672 6f6d 3d32 3032  ibutors?from=202
+0000b3b0: 322d 3033 2d33 3026 746f 3d32 3032 322d  2-03-30&to=2022-
+0000b3c0: 3034 2d30 3726 7479 7065 3d63 2929 0a0a  04-07&type=c))..
+0000b3d0: 5b40 626c 696e 6b31 3037 335d 2868 7474  [@blink1073](htt
+0000b3e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000b3f0: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
+0000b400: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
+0000b410: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
+0000b420: 7325 3341 626c 696e 6b31 3037 332b 7570  s%3Ablink1073+up
+0000b430: 6461 7465 6425 3341 3230 3232 2d30 332d  dated%3A2022-03-
+0000b440: 3330 2e2e 3230 3232 2d30 342d 3037 2674  30..2022-04-07&t
+0000b450: 7970 653d 4973 7375 6573 2920 7c20 5b40  ype=Issues) | [@
+0000b460: 6461 7669 6462 726f 6368 6172 745d 2868  davidbrochart](h
+0000b470: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000b480: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
+0000b490: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
+0000b4a0: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
+0000b4b0: 7665 7325 3341 6461 7669 6462 726f 6368  ves%3Adavidbroch
+0000b4c0: 6172 742b 7570 6461 7465 6425 3341 3230  art+updated%3A20
+0000b4d0: 3232 2d30 332d 3330 2e2e 3230 3232 2d30  22-03-30..2022-0
+0000b4e0: 342d 3037 2674 7970 653d 4973 7375 6573  4-07&type=Issues
+0000b4f0: 2920 7c20 5b40 6563 6861 726c 6573 5d28  ) | [@echarles](
+0000b500: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000b510: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
+0000b520: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
+0000b530: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
+0000b540: 6c76 6573 2533 4165 6368 6172 6c65 732b  lves%3Aecharles+
+0000b550: 7570 6461 7465 6425 3341 3230 3232 2d30  updated%3A2022-0
+0000b560: 332d 3330 2e2e 3230 3232 2d30 342d 3037  3-30..2022-04-07
+0000b570: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
+0000b580: 5b40 7072 652d 636f 6d6d 6974 2d63 695d  [@pre-commit-ci]
+0000b590: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000b5a0: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
+0000b5b0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
+0000b5c0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
+0000b5d0: 6f6c 7665 7325 3341 7072 652d 636f 6d6d  olves%3Apre-comm
+0000b5e0: 6974 2d63 692b 7570 6461 7465 6425 3341  it-ci+updated%3A
+0000b5f0: 3230 3232 2d30 332d 3330 2e2e 3230 3232  2022-03-30..2022
+0000b600: 2d30 342d 3037 2674 7970 653d 4973 7375  -04-07&type=Issu
+0000b610: 6573 290a 0a23 2320 372e 322e 310a 0a28  es)..## 7.2.1..(
+0000b620: 5b46 756c 6c20 4368 616e 6765 6c6f 675d  [Full Changelog]
+0000b630: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000b640: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+0000b650: 7465 725f 636c 6965 6e74 2f63 6f6d 7061  ter_client/compa
+0000b660: 7265 2f76 372e 322e 302e 2e2e 3638 3365  re/v7.2.0...683e
+0000b670: 3864 6439 3665 6364 3532 6461 3438 6138  8dd96ecd52da48a8
+0000b680: 3566 3637 6534 6165 3331 6438 3566 3163  5f67e4ae31d85f1c
+0000b690: 3636 3136 2929 0a0a 2323 2320 4d61 696e  6616))..### Main
+0000b6a0: 7465 6e61 6e63 6520 616e 6420 7570 6b65  tenance and upke
+0000b6b0: 6570 2069 6d70 726f 7665 6d65 6e74 730a  ep improvements.
+0000b6c0: 0a2d 2048 616e 646c 6520 5761 726e 696e  .- Handle Warnin
+0000b6d0: 6773 205b 2337 3630 5d28 6874 7470 733a  gs [#760](https:
+0000b6e0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+0000b6f0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+0000b700: 656e 742f 7075 6c6c 2f37 3630 2920 285b  ent/pull/760) ([
+0000b710: 4062 6c69 6e6b 3130 3733 5d28 6874 7470  @blink1073](http
+0000b720: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
+0000b730: 6c69 6e6b 3130 3733 2929 0a0a 2323 2320  link1073))..### 
+0000b740: 436f 6e74 7269 6275 746f 7273 2074 6f20  Contributors to 
+0000b750: 7468 6973 2072 656c 6561 7365 0a0a 285b  this release..([
+0000b760: 4769 7448 7562 2063 6f6e 7472 6962 7574  GitHub contribut
+0000b770: 6f72 7320 7061 6765 2066 6f72 2074 6869  ors page for thi
+0000b780: 7320 7265 6c65 6173 655d 2868 7474 7073  s release](https
+0000b790: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+0000b7a0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+0000b7b0: 6965 6e74 2f67 7261 7068 732f 636f 6e74  ient/graphs/cont
+0000b7c0: 7269 6275 746f 7273 3f66 726f 6d3d 3230  ributors?from=20
+0000b7d0: 3232 2d30 332d 3239 2674 6f3d 3230 3232  22-03-29&to=2022
+0000b7e0: 2d30 332d 3330 2674 7970 653d 6329 290a  -03-30&type=c)).
+0000b7f0: 0a5b 4062 6c69 6e6b 3130 3733 5d28 6874  .[@blink1073](ht
+0000b800: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000b810: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+0000b820: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+0000b830: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+0000b840: 6573 2533 4162 6c69 6e6b 3130 3733 2b75  es%3Ablink1073+u
+0000b850: 7064 6174 6564 2533 4132 3032 322d 3033  pdated%3A2022-03
+0000b860: 2d32 392e 2e32 3032 322d 3033 2d33 3026  -29..2022-03-30&
+0000b870: 7479 7065 3d49 7373 7565 7329 0a0a 2323  type=Issues)..##
+0000b880: 2037 2e32 2e30 0a0a 285b 4675 6c6c 2043   7.2.0..([Full C
+0000b890: 6861 6e67 656c 6f67 5d28 6874 7470 733a  hangelog](https:
+0000b8a0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+0000b8b0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+0000b8c0: 656e 742f 636f 6d70 6172 652f 7637 2e31  ent/compare/v7.1
+0000b8d0: 2e32 2e2e 2e30 3938 6465 3365 3531 6264  .2...098de3e51bd
+0000b8e0: 3465 6531 6231 6133 6164 6564 3838 3965  4ee1b1a3aded889e
+0000b8f0: 3866 3130 3961 6335 6566 6638 3929 290a  8f109ac5eff89)).
+0000b900: 0a23 2323 2045 6e68 616e 6365 6d65 6e74  .### Enhancement
+0000b910: 7320 6d61 6465 0a0a 2d20 5570 6461 7465  s made..- Update
+0000b920: 2063 6f6e 736f 6c65 6170 702e 7079 205b   consoleapp.py [
+0000b930: 2337 3333 5d28 6874 7470 733a 2f2f 6769  #733](https://gi
+0000b940: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+0000b950: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+0000b960: 7075 6c6c 2f37 3333 2920 285b 4079 6f75  pull/733) ([@you
+0000b970: 2d6e 2d67 5d28 6874 7470 733a 2f2f 6769  -n-g](https://gi
+0000b980: 7468 7562 2e63 6f6d 2f79 6f75 2d6e 2d67  thub.com/you-n-g
+0000b990: 2929 0a0a 2323 2320 4275 6773 2066 6978  ))..### Bugs fix
+0000b9a0: 6564 0a0a 2d20 4a73 6f6e 2070 6163 6b65  ed..- Json packe
+0000b9b0: 723a 2068 616e 646c 6520 5479 7065 4572  r: handle TypeEr
+0000b9c0: 726f 7220 616e 6420 6661 6c6c 6261 636b  ror and fallback
+0000b9d0: 2074 6f20 6f6c 6420 6a73 6f6e 5f63 6c65   to old json_cle
+0000b9e0: 616e 205b 2337 3532 5d28 6874 7470 733a  an [#752](https:
+0000b9f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+0000ba00: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+0000ba10: 656e 742f 7075 6c6c 2f37 3532 2920 285b  ent/pull/752) ([
+0000ba20: 406d 6172 7469 6e52 656e 6f75 5d28 6874  @martinRenou](ht
+0000ba30: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000ba40: 2f6d 6172 7469 6e52 656e 6f75 2929 0a2d  /martinRenou)).-
+0000ba50: 2050 7265 6665 7220 7365 6e64 696e 6720   Prefer sending 
+0000ba60: 7369 676e 616c 7320 746f 206b 6572 6e65  signals to kerne
+0000ba70: 6c20 7072 6f63 6573 7320 6772 6f75 7020  l process group 
+0000ba80: 5b23 3734 335d 2868 7474 7073 3a2f 2f67  [#743](https://g
+0000ba90: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+0000baa0: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+0000bab0: 2f70 756c 6c2f 3734 3329 2028 5b40 6b65  /pull/743) ([@ke
+0000bac0: 7669 6e2d 6261 7465 735d 2868 7474 7073  vin-bates](https
+0000bad0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b65  ://github.com/ke
+0000bae0: 7669 6e2d 6261 7465 7329 290a 0a23 2323  vin-bates))..###
+0000baf0: 204d 6169 6e74 656e 616e 6365 2061 6e64   Maintenance and
+0000bb00: 2075 706b 6565 7020 696d 7072 6f76 656d   upkeep improvem
+0000bb10: 656e 7473 0a0a 2d20 4d6f 636b 2069 7320  ents..- Mock is 
+0000bb20: 6e6f 7420 6e65 6564 6564 205b 2337 3538  not needed [#758
+0000bb30: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000bb40: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+0000bb50: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+0000bb60: 2f37 3538 2920 285b 4068 726f 6e63 6f6b  /758) ([@hroncok
+0000bb70: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000bb80: 2e63 6f6d 2f68 726f 6e63 6f6b 2929 0a2d  .com/hroncok)).-
+0000bb90: 2041 6464 2070 7974 6573 7420 6f70 7473   Add pytest opts
+0000bba0: 2061 6e64 2063 6c65 616e 2075 7020 776f   and clean up wo
+0000bbb0: 726b 666c 6f77 7320 5b23 3735 375d 2868  rkflows [#757](h
+0000bbc0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000bbd0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+0000bbe0: 725f 636c 6965 6e74 2f70 756c 6c2f 3735  r_client/pull/75
+0000bbf0: 3729 2028 5b40 626c 696e 6b31 3037 335d  7) ([@blink1073]
+0000bc00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000bc10: 636f 6d2f 626c 696e 6b31 3037 3329 290a  com/blink1073)).
+0000bc20: 2d20 436c 6561 6e20 7570 2064 6570 656e  - Clean up depen
+0000bc30: 6465 6e63 7920 6861 6e64 6c69 6e67 205b  dency handling [
+0000bc40: 2337 3530 5d28 6874 7470 733a 2f2f 6769  #750](https://gi
+0000bc50: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+0000bc60: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+0000bc70: 7075 6c6c 2f37 3530 2920 285b 4062 6c69  pull/750) ([@bli
+0000bc80: 6e6b 3130 3733 5d28 6874 7470 733a 2f2f  nk1073](https://
+0000bc90: 6769 7468 7562 2e63 6f6d 2f62 6c69 6e6b  github.com/blink
+0000bca0: 3130 3733 2929 0a2d 2055 7365 2062 7569  1073)).- Use bui
+0000bcb0: 6c74 2069 6e20 7275 6e20 6361 6e63 656c  lt in run cancel
+0000bcc0: 6c61 7469 6f6e 205b 2337 3432 5d28 6874  lation [#742](ht
+0000bcd0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000bce0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+0000bcf0: 5f63 6c69 656e 742f 7075 6c6c 2f37 3432  _client/pull/742
+0000bd00: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
+0000bd10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000bd20: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a0a  om/blink1073))..
+0000bd30: 2323 2320 436f 6e74 7269 6275 746f 7273  ### Contributors
+0000bd40: 2074 6f20 7468 6973 2072 656c 6561 7365   to this release
+0000bd50: 0a0a 285b 4769 7448 7562 2063 6f6e 7472  ..([GitHub contr
+0000bd60: 6962 7574 6f72 7320 7061 6765 2066 6f72  ibutors page for
+0000bd70: 2074 6869 7320 7265 6c65 6173 655d 2868   this release](h
+0000bd80: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000bd90: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+0000bda0: 725f 636c 6965 6e74 2f67 7261 7068 732f  r_client/graphs/
+0000bdb0: 636f 6e74 7269 6275 746f 7273 3f66 726f  contributors?fro
+0000bdc0: 6d3d 3230 3232 2d30 312d 3231 2674 6f3d  m=2022-01-21&to=
+0000bdd0: 3230 3232 2d30 332d 3238 2674 7970 653d  2022-03-28&type=
+0000bde0: 6329 290a 0a5b 4062 6c69 6e6b 3130 3733  c))..[@blink1073
+0000bdf0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000be00: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
+0000be10: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
+0000be20: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
+0000be30: 766f 6c76 6573 2533 4162 6c69 6e6b 3130  volves%3Ablink10
+0000be40: 3733 2b75 7064 6174 6564 2533 4132 3032  73+updated%3A202
+0000be50: 322d 3031 2d32 312e 2e32 3032 322d 3033  2-01-21..2022-03
+0000be60: 2d32 3826 7479 7065 3d49 7373 7565 7329  -28&type=Issues)
+0000be70: 207c 205b 4064 6176 6964 6272 6f63 6861   | [@davidbrocha
+0000be80: 7274 5d28 6874 7470 733a 2f2f 6769 7468  rt](https://gith
+0000be90: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
+0000bea0: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
+0000beb0: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
+0000bec0: 696e 766f 6c76 6573 2533 4164 6176 6964  involves%3Adavid
+0000bed0: 6272 6f63 6861 7274 2b75 7064 6174 6564  brochart+updated
+0000bee0: 2533 4132 3032 322d 3031 2d32 312e 2e32  %3A2022-01-21..2
+0000bef0: 3032 322d 3033 2d32 3826 7479 7065 3d49  022-03-28&type=I
+0000bf00: 7373 7565 7329 207c 205b 4065 6368 6172  ssues) | [@echar
+0000bf10: 6c65 735d 2868 7474 7073 3a2f 2f67 6974  les](https://git
+0000bf20: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
+0000bf30: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
+0000bf40: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
+0000bf50: 2b69 6e76 6f6c 7665 7325 3341 6563 6861  +involves%3Aecha
+0000bf60: 726c 6573 2b75 7064 6174 6564 2533 4132  rles+updated%3A2
+0000bf70: 3032 322d 3031 2d32 312e 2e32 3032 322d  022-01-21..2022-
+0000bf80: 3033 2d32 3826 7479 7065 3d49 7373 7565  03-28&type=Issue
+0000bf90: 7329 207c 205b 4068 726f 6e63 6f6b 5d28  s) | [@hroncok](
+0000bfa0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000bfb0: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
+0000bfc0: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
+0000bfd0: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
+0000bfe0: 6c76 6573 2533 4168 726f 6e63 6f6b 2b75  lves%3Ahroncok+u
+0000bff0: 7064 6174 6564 2533 4132 3032 322d 3031  pdated%3A2022-01
+0000c000: 2d32 312e 2e32 3032 322d 3033 2d32 3826  -21..2022-03-28&
+0000c010: 7479 7065 3d49 7373 7565 7329 207c 205b  type=Issues) | [
+0000c020: 406b 6576 696e 2d62 6174 6573 5d28 6874  @kevin-bates](ht
+0000c030: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000c040: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+0000c050: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+0000c060: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+0000c070: 6573 2533 416b 6576 696e 2d62 6174 6573  es%3Akevin-bates
+0000c080: 2b75 7064 6174 6564 2533 4132 3032 322d  +updated%3A2022-
+0000c090: 3031 2d32 312e 2e32 3032 322d 3033 2d32  01-21..2022-03-2
+0000c0a0: 3826 7479 7065 3d49 7373 7565 7329 207c  8&type=Issues) |
+0000c0b0: 205b 406d 6172 7469 6e52 656e 6f75 5d28   [@martinRenou](
+0000c0c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000c0d0: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
+0000c0e0: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
+0000c0f0: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
+0000c100: 6c76 6573 2533 416d 6172 7469 6e52 656e  lves%3AmartinRen
+0000c110: 6f75 2b75 7064 6174 6564 2533 4132 3032  ou+updated%3A202
+0000c120: 322d 3031 2d32 312e 2e32 3032 322d 3033  2-01-21..2022-03
+0000c130: 2d32 3826 7479 7065 3d49 7373 7565 7329  -28&type=Issues)
+0000c140: 207c 205b 4079 6f75 2d6e 2d67 5d28 6874   | [@you-n-g](ht
+0000c150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000c160: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+0000c170: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+0000c180: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+0000c190: 6573 2533 4179 6f75 2d6e 2d67 2b75 7064  es%3Ayou-n-g+upd
+0000c1a0: 6174 6564 2533 4132 3032 322d 3031 2d32  ated%3A2022-01-2
+0000c1b0: 312e 2e32 3032 322d 3033 2d32 3826 7479  1..2022-03-28&ty
+0000c1c0: 7065 3d49 7373 7565 7329 0a0a 2323 2037  pe=Issues)..## 7
+0000c1d0: 2e31 2e32 0a0a 285b 4675 6c6c 2043 6861  .1.2..([Full Cha
+0000c1e0: 6e67 656c 6f67 5d28 6874 7470 733a 2f2f  ngelog](https://
+0000c1f0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+0000c200: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+0000c210: 742f 636f 6d70 6172 652f 7637 2e31 2e31  t/compare/v7.1.1
+0000c220: 2e2e 2e32 6339 6662 6634 3939 6636 3364  ...2c9fbf499f63d
+0000c230: 3432 3837 3835 3130 3231 6238 6638 6566  4287851021b8f8ef
+0000c240: 6339 6433 6330 6533 3336 6529 290a 0a23  c9d3c0e336e))..#
+0000c250: 2323 2042 7567 7320 6669 7865 640a 0a2d  ## Bugs fixed..-
+0000c260: 2041 7761 6974 2060 6b65 726e 656c 2e72   Await `kernel.r
+0000c270: 6561 6479 6020 696e 2060 5f61 7379 6e63  eady` in `_async
+0000c280: 5f73 6875 7464 6f77 6e5f 6b65 726e 656c  _shutdown_kernel
+0000c290: 6020 5b23 3734 305d 2868 7474 7073 3a2f  ` [#740](https:/
+0000c2a0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+0000c2b0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+0000c2c0: 6e74 2f70 756c 6c2f 3734 3029 2028 5b40  nt/pull/740) ([@
+0000c2d0: 6a74 7069 6f5d 2868 7474 7073 3a2f 2f67  jtpio](https://g
+0000c2e0: 6974 6875 622e 636f 6d2f 6a74 7069 6f29  ithub.com/jtpio)
+0000c2f0: 290a 0a23 2323 2043 6f6e 7472 6962 7574  )..### Contribut
+0000c300: 6f72 7320 746f 2074 6869 7320 7265 6c65  ors to this rele
+0000c310: 6173 650a 0a28 5b47 6974 4875 6220 636f  ase..([GitHub co
+0000c320: 6e74 7269 6275 746f 7273 2070 6167 6520  ntributors page 
+0000c330: 666f 7220 7468 6973 2072 656c 6561 7365  for this release
+0000c340: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000c350: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+0000c360: 7974 6572 5f63 6c69 656e 742f 6772 6170  yter_client/grap
+0000c370: 6873 2f63 6f6e 7472 6962 7574 6f72 733f  hs/contributors?
+0000c380: 6672 6f6d 3d32 3032 322d 3031 2d31 3426  from=2022-01-14&
+0000c390: 746f 3d32 3032 322d 3031 2d32 3126 7479  to=2022-01-21&ty
+0000c3a0: 7065 3d63 2929 0a0a 5b40 6a74 7069 6f5d  pe=c))..[@jtpio]
+0000c3b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000c3c0: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
+0000c3d0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
+0000c3e0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
+0000c3f0: 6f6c 7665 7325 3341 6a74 7069 6f2b 7570  olves%3Ajtpio+up
+0000c400: 6461 7465 6425 3341 3230 3232 2d30 312d  dated%3A2022-01-
+0000c410: 3134 2e2e 3230 3232 2d30 312d 3231 2674  14..2022-01-21&t
+0000c420: 7970 653d 4973 7375 6573 2920 7c20 5b40  ype=Issues) | [@
+0000c430: 5a73 6169 6c65 725d 2868 7474 7073 3a2f  Zsailer](https:/
+0000c440: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
+0000c450: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
+0000c460: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
+0000c470: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
+0000c480: 5a73 6169 6c65 722b 7570 6461 7465 6425  Zsailer+updated%
+0000c490: 3341 3230 3232 2d30 312d 3134 2e2e 3230  3A2022-01-14..20
+0000c4a0: 3232 2d30 312d 3231 2674 7970 653d 4973  22-01-21&type=Is
+0000c4b0: 7375 6573 290a 0a23 2320 372e 312e 310a  sues)..## 7.1.1.
+0000c4c0: 0a28 5b46 756c 6c20 4368 616e 6765 6c6f  .([Full Changelo
+0000c4d0: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
+0000c4e0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+0000c4f0: 7079 7465 725f 636c 6965 6e74 2f63 6f6d  pyter_client/com
+0000c500: 7061 7265 2f76 372e 312e 302e 2e2e 3434  pare/v7.1.0...44
+0000c510: 3238 3731 3562 3635 3734 3164 6463 6361  28715b65741ddcca
+0000c520: 6339 3330 3564 3331 3864 3461 6365 3038  c9305d318d4ace08
+0000c530: 6661 3731 3161 2929 0a0a 2323 2320 456e  fa711a))..### En
+0000c540: 6861 6e63 656d 656e 7473 206d 6164 650a  hancements made.
+0000c550: 0a2d 2046 7572 7468 6572 2069 6d70 726f  .- Further impro
+0000c560: 7665 6d65 6e74 7320 746f 2070 656e 6469  vements to pendi
+0000c570: 6e67 206b 6572 6e65 6c73 206d 616e 6167  ng kernels manag
+0000c580: 656d 656e 7420 5b23 3733 325d 2868 7474  ement [#732](htt
+0000c590: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000c5a0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+0000c5b0: 636c 6965 6e74 2f70 756c 6c2f 3733 3229  client/pull/732)
+0000c5c0: 2028 5b40 5a73 6169 6c65 725d 2868 7474   ([@Zsailer](htt
+0000c5d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000c5e0: 5a73 6169 6c65 7229 290a 0a23 2323 204d  Zsailer))..### M
+0000c5f0: 6169 6e74 656e 616e 6365 2061 6e64 2075  aintenance and u
+0000c600: 706b 6565 7020 696d 7072 6f76 656d 656e  pkeep improvemen
+0000c610: 7473 0a0a 2d20 5465 7374 2061 6761 696e  ts..- Test again
+0000c620: 7374 2061 6c6c 206b 6572 6e65 6c73 2069  st all kernels i
+0000c630: 6e20 6a75 7079 7465 7220 6b65 726e 656c  n jupyter kernel
+0000c640: 2074 6573 7420 616e 6420 636c 6561 6e20   test and clean 
+0000c650: 7570 2043 4920 5b23 3733 315d 2868 7474  up CI [#731](htt
+0000c660: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000c670: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+0000c680: 636c 6965 6e74 2f70 756c 6c2f 3733 3129  client/pull/731)
+0000c690: 2028 5b40 626c 696e 6b31 3037 335d 2868   ([@blink1073](h
+0000c6a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000c6b0: 6d2f 626c 696e 6b31 3037 3329 290a 2d20  m/blink1073)).- 
+0000c6c0: 5265 706c 6163 6520 6d61 7374 6572 2077  Replace master w
+0000c6d0: 6974 6820 6d61 696e 205b 2337 3239 5d28  ith main [#729](
+0000c6e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000c6f0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+0000c700: 6572 5f63 6c69 656e 742f 7075 6c6c 2f37  er_client/pull/7
+0000c710: 3239 2920 285b 4064 6176 6964 6272 6f63  29) ([@davidbroc
+0000c720: 6861 7274 5d28 6874 7470 733a 2f2f 6769  hart](https://gi
+0000c730: 7468 7562 2e63 6f6d 2f64 6176 6964 6272  thub.com/davidbr
+0000c740: 6f63 6861 7274 2929 0a0a 2323 2320 446f  ochart))..### Do
+0000c750: 6375 6d65 6e74 6174 696f 6e20 696d 7072  cumentation impr
+0000c760: 6f76 656d 656e 7473 0a0a 2d20 5c5b 444f  ovements..- \[DO
+0000c770: 435c 5d20 696d 7072 6f76 6520 6b65 726e  C\] improve kern
+0000c780: 656c 2070 726f 7669 7369 6f6e 6572 2064  el provisioner d
+0000c790: 6f63 205b 2337 3330 5d28 6874 7470 733a  oc [#730](https:
+0000c7a0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+0000c7b0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+0000c7c0: 656e 742f 7075 6c6c 2f37 3330 2920 285b  ent/pull/730) ([
+0000c7d0: 4061 627a 796d 6569 6e73 6a74 755d 2868  @abzymeinsjtu](h
+0000c7e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000c7f0: 6d2f 6162 7a79 6d65 696e 736a 7475 2929  m/abzymeinsjtu))
+0000c800: 0a2d 2061 6464 2063 6861 6e67 656c 6f67  .- add changelog
+0000c810: 2066 6f72 206d 6573 7361 6765 2073 7065   for message spe
+0000c820: 6320 5b23 3532 355d 2868 7474 7073 3a2f  c [#525](https:/
+0000c830: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+0000c840: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+0000c850: 6e74 2f70 756c 6c2f 3532 3529 2028 5b40  nt/pull/525) ([@
+0000c860: 6d69 6e72 6b5d 2868 7474 7073 3a2f 2f67  minrk](https://g
+0000c870: 6974 6875 622e 636f 6d2f 6d69 6e72 6b29  ithub.com/minrk)
+0000c880: 290a 0a23 2323 2043 6f6e 7472 6962 7574  )..### Contribut
+0000c890: 6f72 7320 746f 2074 6869 7320 7265 6c65  ors to this rele
+0000c8a0: 6173 650a 0a28 5b47 6974 4875 6220 636f  ase..([GitHub co
+0000c8b0: 6e74 7269 6275 746f 7273 2070 6167 6520  ntributors page 
+0000c8c0: 666f 7220 7468 6973 2072 656c 6561 7365  for this release
+0000c8d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000c8e0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+0000c8f0: 7974 6572 5f63 6c69 656e 742f 6772 6170  yter_client/grap
+0000c900: 6873 2f63 6f6e 7472 6962 7574 6f72 733f  hs/contributors?
+0000c910: 6672 6f6d 3d32 3032 312d 3131 2d32 3226  from=2021-11-22&
+0000c920: 746f 3d32 3032 322d 3031 2d31 3426 7479  to=2022-01-14&ty
+0000c930: 7065 3d63 2929 0a0a 5b40 6162 7a79 6d65  pe=c))..[@abzyme
+0000c940: 696e 736a 7475 5d28 6874 7470 733a 2f2f  insjtu](https://
+0000c950: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
+0000c960: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
+0000c970: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
+0000c980: 656e 742b 696e 766f 6c76 6573 2533 4161  ent+involves%3Aa
+0000c990: 627a 796d 6569 6e73 6a74 752b 7570 6461  bzymeinsjtu+upda
+0000c9a0: 7465 6425 3341 3230 3231 2d31 312d 3232  ted%3A2021-11-22
+0000c9b0: 2e2e 3230 3232 2d30 312d 3134 2674 7970  ..2022-01-14&typ
+0000c9c0: 653d 4973 7375 6573 2920 7c20 5b40 626c  e=Issues) | [@bl
+0000c9d0: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
+0000c9e0: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
+0000c9f0: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
+0000ca00: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
+0000ca10: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
+0000ca20: 626c 696e 6b31 3037 332b 7570 6461 7465  blink1073+update
+0000ca30: 6425 3341 3230 3231 2d31 312d 3232 2e2e  d%3A2021-11-22..
+0000ca40: 3230 3232 2d30 312d 3134 2674 7970 653d  2022-01-14&type=
+0000ca50: 4973 7375 6573 2920 7c20 5b40 426f 5065  Issues) | [@BoPe
+0000ca60: 6e67 5d28 6874 7470 733a 2f2f 6769 7468  ng](https://gith
+0000ca70: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
+0000ca80: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
+0000ca90: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
+0000caa0: 696e 766f 6c76 6573 2533 4142 6f50 656e  involves%3ABoPen
+0000cab0: 672b 7570 6461 7465 6425 3341 3230 3231  g+updated%3A2021
+0000cac0: 2d31 312d 3232 2e2e 3230 3232 2d30 312d  -11-22..2022-01-
+0000cad0: 3134 2674 7970 653d 4973 7375 6573 2920  14&type=Issues) 
+0000cae0: 7c20 5b40 6461 7669 6462 726f 6368 6172  | [@davidbrochar
+0000caf0: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+0000cb00: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
+0000cb10: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
+0000cb20: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
+0000cb30: 6e76 6f6c 7665 7325 3341 6461 7669 6462  nvolves%3Adavidb
+0000cb40: 726f 6368 6172 742b 7570 6461 7465 6425  rochart+updated%
+0000cb50: 3341 3230 3231 2d31 312d 3232 2e2e 3230  3A2021-11-22..20
+0000cb60: 3232 2d30 312d 3134 2674 7970 653d 4973  22-01-14&type=Is
+0000cb70: 7375 6573 2920 7c20 5b40 6d69 6e72 6b5d  sues) | [@minrk]
+0000cb80: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000cb90: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
+0000cba0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
+0000cbb0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
+0000cbc0: 6f6c 7665 7325 3341 6d69 6e72 6b2b 7570  olves%3Aminrk+up
+0000cbd0: 6461 7465 6425 3341 3230 3231 2d31 312d  dated%3A2021-11-
+0000cbe0: 3232 2e2e 3230 3232 2d30 312d 3134 2674  22..2022-01-14&t
+0000cbf0: 7970 653d 4973 7375 6573 2920 7c20 5b40  ype=Issues) | [@
+0000cc00: 7267 626b 726b 5d28 6874 7470 733a 2f2f  rgbkrk](https://
+0000cc10: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
+0000cc20: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
+0000cc30: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
+0000cc40: 656e 742b 696e 766f 6c76 6573 2533 4172  ent+involves%3Ar
+0000cc50: 6762 6b72 6b2b 7570 6461 7465 6425 3341  gbkrk+updated%3A
+0000cc60: 3230 3231 2d31 312d 3232 2e2e 3230 3232  2021-11-22..2022
+0000cc70: 2d30 312d 3134 2674 7970 653d 4973 7375  -01-14&type=Issu
+0000cc80: 6573 2920 7c20 5b40 7769 6c6c 696e 6763  es) | [@willingc
+0000cc90: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000cca0: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
+0000ccb0: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
+0000ccc0: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
+0000ccd0: 766f 6c76 6573 2533 4177 696c 6c69 6e67  volves%3Awilling
+0000cce0: 632b 7570 6461 7465 6425 3341 3230 3231  c+updated%3A2021
+0000ccf0: 2d31 312d 3232 2e2e 3230 3232 2d30 312d  -11-22..2022-01-
+0000cd00: 3134 2674 7970 653d 4973 7375 6573 2920  14&type=Issues) 
+0000cd10: 7c20 5b40 5a73 6169 6c65 725d 2868 7474  | [@Zsailer](htt
+0000cd20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000cd30: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
+0000cd40: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
+0000cd50: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
+0000cd60: 7325 3341 5a73 6169 6c65 722b 7570 6461  s%3AZsailer+upda
+0000cd70: 7465 6425 3341 3230 3231 2d31 312d 3232  ted%3A2021-11-22
+0000cd80: 2e2e 3230 3232 2d30 312d 3134 2674 7970  ..2022-01-14&typ
+0000cd90: 653d 4973 7375 6573 290a 0a23 2320 372e  e=Issues)..## 7.
+0000cda0: 312e 300a 0a28 5b46 756c 6c20 4368 616e  1.0..([Full Chan
+0000cdb0: 6765 6c6f 675d 2868 7474 7073 3a2f 2f67  gelog](https://g
+0000cdc0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+0000cdd0: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+0000cde0: 2f63 6f6d 7061 7265 2f76 372e 302e 362e  /compare/v7.0.6.
+0000cdf0: 2e2e 3662 3736 3630 3335 3738 6664 3361  ..6b76603578fd3a
+0000ce00: 3736 6664 3537 3764 3333 3139 3339 3363  76fd577d3319393c
+0000ce10: 3939 3333 6635 3361 6230 2929 0a0a 2323  9933f53ab0))..##
+0000ce20: 2320 456e 6861 6e63 656d 656e 7473 206d  # Enhancements m
+0000ce30: 6164 650a 0a2d 2041 6464 2073 7570 706f  ade..- Add suppo
+0000ce40: 7274 2066 6f72 2070 656e 6469 6e67 206b  rt for pending k
+0000ce50: 6572 6e65 6c73 205b 2337 3132 5d28 6874  ernels [#712](ht
+0000ce60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000ce70: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+0000ce80: 5f63 6c69 656e 742f 7075 6c6c 2f37 3132  _client/pull/712
+0000ce90: 2920 285b 4062 6c69 6e6b 3130 3733 5d28  ) ([@blink1073](
+0000cea0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000ceb0: 6f6d 2f62 6c69 6e6b 3130 3733 2929 0a0a  om/blink1073))..
+0000cec0: 2323 2320 4275 6773 2066 6978 6564 0a0a  ### Bugs fixed..
+0000ced0: 2d20 496d 7072 6f76 6520 7265 7374 6172  - Improve restar
+0000cee0: 7465 7220 6c6f 6769 6320 5b23 3731 375d  ter logic [#717]
+0000cef0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000cf00: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+0000cf10: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+0000cf20: 3731 3729 2028 5b40 7669 6461 7274 665d  717) ([@vidartf]
+0000cf30: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000cf40: 636f 6d2f 7669 6461 7274 6629 290a 2d20  com/vidartf)).- 
+0000cf50: 5365 7420 7374 6963 6b79 2062 6974 206f  Set sticky bit o
+0000cf60: 6e6c 7920 6f6e 2074 6865 2064 6972 6563  nly on the direc
+0000cf70: 746f 7279 205b 2337 3131 5d28 6874 7470  tory [#711](http
+0000cf80: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+0000cf90: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
+0000cfa0: 6c69 656e 742f 7075 6c6c 2f37 3131 2920  lient/pull/711) 
+0000cfb0: 285b 4063 6934 6963 345d 2868 7474 7073  ([@ci4ic4](https
+0000cfc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6369  ://github.com/ci
+0000cfd0: 3469 6334 2929 0a0a 2323 2320 4d61 696e  4ic4))..### Main
+0000cfe0: 7465 6e61 6e63 6520 616e 6420 7570 6b65  tenance and upke
+0000cff0: 6570 2069 6d70 726f 7665 6d65 6e74 730a  ep improvements.
+0000d000: 0a2d 2045 6e66 6f72 6365 206c 6162 656c  .- Enforce label
+0000d010: 7320 6f6e 2050 5273 205b 2337 3230 5d28  s on PRs [#720](
 0000d020: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000d030: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
-0000d040: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
-0000d050: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
-0000d060: 6c76 6573 2533 416b 6576 696e 2d62 6174  lves%3Akevin-bat
-0000d070: 6573 2b75 7064 6174 6564 2533 4132 3032  es+updated%3A202
-0000d080: 312d 3039 2d32 382e 2e32 3032 312d 3039  1-09-28..2021-09
-0000d090: 2d32 3926 7479 7065 3d49 7373 7565 7329  -29&type=Issues)
-0000d0a0: 207c 205b 406d 696e 726b 5d28 6874 7470   | [@minrk](http
-0000d0b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-0000d0c0: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
-0000d0d0: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
-0000d0e0: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
-0000d0f0: 2533 416d 696e 726b 2b75 7064 6174 6564  %3Aminrk+updated
-0000d100: 2533 4132 3032 312d 3039 2d32 382e 2e32  %3A2021-09-28..2
-0000d110: 3032 312d 3039 2d32 3926 7479 7065 3d49  021-09-29&type=I
-0000d120: 7373 7565 7329 0a0a 2323 2037 2e30 2e34  ssues)..## 7.0.4
-0000d130: 0a0a 285b 4675 6c6c 2043 6861 6e67 656c  ..([Full Changel
-0000d140: 6f67 5d28 6874 7470 733a 2f2f 6769 7468  og](https://gith
-0000d150: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-0000d160: 7570 7974 6572 5f63 6c69 656e 742f 636f  upyter_client/co
-0000d170: 6d70 6172 652f 7637 2e30 2e33 2e2e 2e35  mpare/v7.0.3...5
-0000d180: 6235 3730 3135 3263 3064 3838 6464 3565  b570152c0d88dd5e
-0000d190: 3066 6631 3731 3163 3735 6663 3939 3837  0ff1711c75fc9987
-0000d1a0: 6566 3736 3235 3629 290a 0a23 2323 2042  ef76256))..### B
-0000d1b0: 7567 7320 6669 7865 640a 0a2d 2046 6978  ugs fixed..- Fix
-0000d1c0: 206a 736f 6e5f 6465 6661 756c 7420 736f   json_default so
-0000d1d0: 2074 6861 7420 6974 2773 2063 6c6f 7365   that it's close
-0000d1e0: 7220 746f 2077 6861 7420 6970 796b 6572  r to what ipyker
-0000d1f0: 6e65 6c20 6861 6420 6265 666f 7265 205b  nel had before [
-0000d200: 2336 3938 5d28 6874 7470 733a 2f2f 6769  #698](https://gi
-0000d210: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-0000d220: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-0000d230: 7075 6c6c 2f36 3938 2920 285b 406d 6172  pull/698) ([@mar
-0000d240: 7469 6e52 656e 6f75 5d28 6874 7470 733a  tinRenou](https:
-0000d250: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6172  //github.com/mar
-0000d260: 7469 6e52 656e 6f75 2929 0a2d 2043 6c65  tinRenou)).- Cle
-0000d270: 616e 2075 7020 7468 6520 7065 6e64 696e  an up the pendin
-0000d280: 6720 7461 736b 205b 2336 3937 5d28 6874  g task [#697](ht
-0000d290: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000d2a0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-0000d2b0: 5f63 6c69 656e 742f 7075 6c6c 2f36 3937  _client/pull/697
-0000d2c0: 2920 285b 4073 6869 6e67 6f37 385d 2868  ) ([@shingo78](h
-0000d2d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000d2e0: 6d2f 7368 696e 676f 3738 2929 0a2d 2066  m/shingo78)).- f
-0000d2f0: 6978 206b 6572 6e65 6c20 6361 6e20 6f6e  ix kernel can on
-0000d300: 6c79 2072 6573 7461 7274 206f 6e63 6520  ly restart once 
-0000d310: 6973 7375 6520 5b23 3639 355d 2868 7474  issue [#695](htt
-0000d320: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000d330: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-0000d340: 636c 6965 6e74 2f70 756c 6c2f 3639 3529  client/pull/695)
-0000d350: 2028 5b40 6d6f 6661 6e6b 655d 2868 7474   ([@mofanke](htt
-0000d360: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000d370: 6d6f 6661 6e6b 6529 290a 2d20 5072 6576  mofanke)).- Prev
-0000d380: 656e 7420 6661 696c 7572 6520 6966 206b  ent failure if k
-0000d390: 6572 6e65 6c20 6973 206e 6f74 2066 6f75  ernel is not fou
-0000d3a0: 6e64 2077 6865 6e20 7368 7574 7469 6e67  nd when shutting
-0000d3b0: 2069 7420 646f 776e 205b 2336 3934 5d28   it down [#694](
-0000d3c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000d3d0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-0000d3e0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f36  er_client/pull/6
-0000d3f0: 3934 2920 285b 406d 6172 7469 6e52 656e  94) ([@martinRen
-0000d400: 6f75 5d28 6874 7470 733a 2f2f 6769 7468  ou](https://gith
-0000d410: 7562 2e63 6f6d 2f6d 6172 7469 6e52 656e  ub.com/martinRen
-0000d420: 6f75 2929 0a0a 2323 2320 436f 6e74 7269  ou))..### Contri
-0000d430: 6275 746f 7273 2074 6f20 7468 6973 2072  butors to this r
-0000d440: 656c 6561 7365 0a0a 285b 4769 7448 7562  elease..([GitHub
-0000d450: 2063 6f6e 7472 6962 7574 6f72 7320 7061   contributors pa
-0000d460: 6765 2066 6f72 2074 6869 7320 7265 6c65  ge for this rele
-0000d470: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
-0000d480: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-0000d490: 6a75 7079 7465 725f 636c 6965 6e74 2f67  jupyter_client/g
-0000d4a0: 7261 7068 732f 636f 6e74 7269 6275 746f  raphs/contributo
-0000d4b0: 7273 3f66 726f 6d3d 3230 3231 2d30 392d  rs?from=2021-09-
-0000d4c0: 3136 2674 6f3d 3230 3231 2d30 392d 3238  16&to=2021-09-28
-0000d4d0: 2674 7970 653d 6329 290a 0a5b 4064 6176  &type=c))..[@dav
-0000d4e0: 6964 6272 6f63 6861 7274 5d28 6874 7470  idbrochart](http
-0000d4f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-0000d500: 6561 7263 683f 713d 7265 706f 2533 416a  earch?q=repo%3Aj
-0000d510: 7570 7974 6572 2532 466a 7570 7974 6572  upyter%2Fjupyter
-0000d520: 5f63 6c69 656e 742b 696e 766f 6c76 6573  _client+involves
-0000d530: 2533 4164 6176 6964 6272 6f63 6861 7274  %3Adavidbrochart
-0000d540: 2b75 7064 6174 6564 2533 4132 3032 312d  +updated%3A2021-
-0000d550: 3039 2d31 362e 2e32 3032 312d 3039 2d32  09-16..2021-09-2
-0000d560: 3826 7479 7065 3d49 7373 7565 7329 207c  8&type=Issues) |
-0000d570: 205b 406d 6172 7469 6e52 656e 6f75 5d28   [@martinRenou](
-0000d580: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000d590: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
-0000d5a0: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
-0000d5b0: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
-0000d5c0: 6c76 6573 2533 416d 6172 7469 6e52 656e  lves%3AmartinRen
-0000d5d0: 6f75 2b75 7064 6174 6564 2533 4132 3032  ou+updated%3A202
-0000d5e0: 312d 3039 2d31 362e 2e32 3032 312d 3039  1-09-16..2021-09
-0000d5f0: 2d32 3826 7479 7065 3d49 7373 7565 7329  -28&type=Issues)
-0000d600: 207c 205b 406d 6f66 616e 6b65 5d28 6874   | [@mofanke](ht
-0000d610: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000d620: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
-0000d630: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
-0000d640: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
-0000d650: 6573 2533 416d 6f66 616e 6b65 2b75 7064  es%3Amofanke+upd
-0000d660: 6174 6564 2533 4132 3032 312d 3039 2d31  ated%3A2021-09-1
-0000d670: 362e 2e32 3032 312d 3039 2d32 3826 7479  6..2021-09-28&ty
-0000d680: 7065 3d49 7373 7565 7329 207c 205b 4073  pe=Issues) | [@s
-0000d690: 6869 6e67 6f37 385d 2868 7474 7073 3a2f  hingo78](https:/
-0000d6a0: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-0000d6b0: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-0000d6c0: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-0000d6d0: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-0000d6e0: 7368 696e 676f 3738 2b75 7064 6174 6564  shingo78+updated
-0000d6f0: 2533 4132 3032 312d 3039 2d31 362e 2e32  %3A2021-09-16..2
-0000d700: 3032 312d 3039 2d32 3826 7479 7065 3d49  021-09-28&type=I
-0000d710: 7373 7565 7329 0a0a 2323 2037 2e30 2e33  ssues)..## 7.0.3
-0000d720: 0a0a 285b 4675 6c6c 2043 6861 6e67 656c  ..([Full Changel
-0000d730: 6f67 5d28 6874 7470 733a 2f2f 6769 7468  og](https://gith
-0000d740: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-0000d750: 7570 7974 6572 5f63 6c69 656e 742f 636f  upyter_client/co
-0000d760: 6d70 6172 652f 7637 2e30 2e32 2e2e 2e65  mpare/v7.0.2...e
-0000d770: 3265 3835 3463 3434 3564 3639 3761 6531  2e854c445d697ae1
-0000d780: 6331 3838 3137 3165 6130 3733 3135 3332  c188171ea0731532
-0000d790: 6236 6163 3064 3929 290a 0a23 2323 2042  b6ac0d9))..### B
-0000d7a0: 7567 7320 6669 7865 640a 0a2d 2041 6464  ugs fixed..- Add
-0000d7b0: 7265 7373 206d 6973 7369 6e67 2060 6c6f  ress missing `lo
-0000d7c0: 6361 6c2d 7072 6f76 6973 696f 6e65 7260  cal-provisioner`
-0000d7d0: 2073 6365 6e61 7269 6f20 5b23 3639 325d   scenario [#692]
-0000d7e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000d7f0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-0000d800: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-0000d810: 3639 3229 2028 5b40 6b65 7669 6e2d 6261  692) ([@kevin-ba
-0000d820: 7465 735d 2868 7474 7073 3a2f 2f67 6974  tes](https://git
-0000d830: 6875 622e 636f 6d2f 6b65 7669 6e2d 6261  hub.com/kevin-ba
-0000d840: 7465 7329 290a 2d20 7573 6520 606c 6f61  tes)).- use `loa
-0000d850: 645f 636f 6e6e 6563 7469 6f6e 5f69 6e66  d_connection_inf
-0000d860: 6f28 696e 666f 2960 2077 6865 6e20 636f  o(info)` when co
-0000d870: 6e73 7472 7563 7469 6e67 2061 2062 6c6f  nstructing a blo
-0000d880: 636b 696e 6720 636c 6965 6e74 205b 2336  cking client [#6
-0000d890: 3838 5d28 6874 7470 733a 2f2f 6769 7468  88](https://gith
-0000d8a0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-0000d8b0: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-0000d8c0: 6c6c 2f36 3838 2920 285b 406d 696e 726b  ll/688) ([@minrk
-0000d8d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000d8e0: 2e63 6f6d 2f6d 696e 726b 2929 0a0a 2323  .com/minrk))..##
-0000d8f0: 2320 436f 6e74 7269 6275 746f 7273 2074  # Contributors t
-0000d900: 6f20 7468 6973 2072 656c 6561 7365 0a0a  o this release..
-0000d910: 285b 4769 7448 7562 2063 6f6e 7472 6962  ([GitHub contrib
-0000d920: 7574 6f72 7320 7061 6765 2066 6f72 2074  utors page for t
-0000d930: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
-0000d940: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000d950: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-0000d960: 636c 6965 6e74 2f67 7261 7068 732f 636f  client/graphs/co
-0000d970: 6e74 7269 6275 746f 7273 3f66 726f 6d3d  ntributors?from=
-0000d980: 3230 3231 2d30 382d 3330 2674 6f3d 3230  2021-08-30&to=20
-0000d990: 3231 2d30 392d 3136 2674 7970 653d 6329  21-09-16&type=c)
-0000d9a0: 290a 0a5b 406b 6576 696e 2d62 6174 6573  )..[@kevin-bates
-0000d9b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000d9c0: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
-0000d9d0: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
-0000d9e0: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
-0000d9f0: 766f 6c76 6573 2533 416b 6576 696e 2d62  volves%3Akevin-b
-0000da00: 6174 6573 2b75 7064 6174 6564 2533 4132  ates+updated%3A2
-0000da10: 3032 312d 3038 2d33 302e 2e32 3032 312d  021-08-30..2021-
-0000da20: 3039 2d31 3626 7479 7065 3d49 7373 7565  09-16&type=Issue
-0000da30: 7329 207c 205b 406d 696e 726b 5d28 6874  s) | [@minrk](ht
-0000da40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000da50: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
-0000da60: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
-0000da70: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
-0000da80: 6573 2533 416d 696e 726b 2b75 7064 6174  es%3Aminrk+updat
-0000da90: 6564 2533 4132 3032 312d 3038 2d33 302e  ed%3A2021-08-30.
-0000daa0: 2e32 3032 312d 3039 2d31 3626 7479 7065  .2021-09-16&type
-0000dab0: 3d49 7373 7565 7329 0a0a 2323 2037 2e30  =Issues)..## 7.0
-0000dac0: 2e32 0a0a 285b 4675 6c6c 2043 6861 6e67  .2..([Full Chang
-0000dad0: 656c 6f67 5d28 6874 7470 733a 2f2f 6769  elog](https://gi
-0000dae0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-0000daf0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-0000db00: 636f 6d70 6172 652f 7637 2e30 2e31 2e2e  compare/v7.0.1..
-0000db10: 2e62 3261 3233 6438 6638 6234 6632 3461  .b2a23d8f8b4f24a
-0000db20: 3262 6339 3038 6236 6439 3530 3437 3234  2bc908b6d9504724
-0000db30: 3266 3464 6138 3763 6429 290a 0a23 2323  2f4da87cd))..###
-0000db40: 2042 7567 7320 6669 7865 640a 0a2d 2044   Bugs fixed..- D
-0000db50: 6f6e 2774 2073 6574 2065 7665 6e74 206c  on't set event l
-0000db60: 6f6f 7020 706f 6c69 6379 206f 6e20 5769  oop policy on Wi
-0000db70: 6e64 6f77 7320 6174 2069 6d70 6f72 7420  ndows at import 
-0000db80: 7469 6d65 205b 2336 3836 5d28 6874 7470  time [#686](http
-0000db90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-0000dba0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-0000dbb0: 6c69 656e 742f 7075 6c6c 2f36 3836 2920  lient/pull/686) 
-0000dbc0: 285b 406d 696e 726b 5d28 6874 7470 733a  ([@minrk](https:
-0000dbd0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 696e  //github.com/min
-0000dbe0: 726b 2929 0a0a 2323 2320 446f 6375 6d65  rk))..### Docume
-0000dbf0: 6e74 6174 696f 6e20 696d 7072 6f76 656d  ntation improvem
-0000dc00: 656e 7473 0a0a 2d20 496d 7072 6f76 6520  ents..- Improve 
-0000dc10: 6d69 6772 6174 696f 6e20 6775 6964 6520  migration guide 
-0000dc20: 5b23 3638 355d 2868 7474 7073 3a2f 2f67  [#685](https://g
-0000dc30: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
-0000dc40: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
-0000dc50: 2f70 756c 6c2f 3638 3529 2028 5b40 6461  /pull/685) ([@da
-0000dc60: 7669 6462 726f 6368 6172 745d 2868 7474  vidbrochart](htt
-0000dc70: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000dc80: 6461 7669 6462 726f 6368 6172 7429 290a  davidbrochart)).
-0000dc90: 0a23 2323 2043 6f6e 7472 6962 7574 6f72  .### Contributor
-0000dca0: 7320 746f 2074 6869 7320 7265 6c65 6173  s to this releas
-0000dcb0: 650a 0a28 5b47 6974 4875 6220 636f 6e74  e..([GitHub cont
-0000dcc0: 7269 6275 746f 7273 2070 6167 6520 666f  ributors page fo
-0000dcd0: 7220 7468 6973 2072 656c 6561 7365 5d28  r this release](
-0000dce0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000dcf0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-0000dd00: 6572 5f63 6c69 656e 742f 6772 6170 6873  er_client/graphs
-0000dd10: 2f63 6f6e 7472 6962 7574 6f72 733f 6672  /contributors?fr
-0000dd20: 6f6d 3d32 3032 312d 3038 2d32 3026 746f  om=2021-08-20&to
-0000dd30: 3d32 3032 312d 3038 2d33 3026 7479 7065  =2021-08-30&type
-0000dd40: 3d63 2929 0a0a 5b40 626c 696e 6b31 3037  =c))..[@blink107
-0000dd50: 335d 2868 7474 7073 3a2f 2f67 6974 6875  3](https://githu
-0000dd60: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
-0000dd70: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
-0000dd80: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
-0000dd90: 6e76 6f6c 7665 7325 3341 626c 696e 6b31  nvolves%3Ablink1
-0000dda0: 3037 332b 7570 6461 7465 6425 3341 3230  073+updated%3A20
-0000ddb0: 3231 2d30 382d 3230 2e2e 3230 3231 2d30  21-08-20..2021-0
-0000ddc0: 382d 3330 2674 7970 653d 4973 7375 6573  8-30&type=Issues
-0000ddd0: 2920 7c20 5b40 6461 7669 6462 726f 6368  ) | [@davidbroch
-0000dde0: 6172 745d 2868 7474 7073 3a2f 2f67 6974  art](https://git
-0000ddf0: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
-0000de00: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
-0000de10: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
-0000de20: 2b69 6e76 6f6c 7665 7325 3341 6461 7669  +involves%3Adavi
-0000de30: 6462 726f 6368 6172 742b 7570 6461 7465  dbrochart+update
-0000de40: 6425 3341 3230 3231 2d30 382d 3230 2e2e  d%3A2021-08-20..
-0000de50: 3230 3231 2d30 382d 3330 2674 7970 653d  2021-08-30&type=
-0000de60: 4973 7375 6573 2920 7c20 5b40 6468 6972  Issues) | [@dhir
-0000de70: 7363 6866 656c 645d 2868 7474 7073 3a2f  schfeld](https:/
-0000de80: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-0000de90: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-0000dea0: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-0000deb0: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-0000dec0: 6468 6972 7363 6866 656c 642b 7570 6461  dhirschfeld+upda
-0000ded0: 7465 6425 3341 3230 3231 2d30 382d 3230  ted%3A2021-08-20
-0000dee0: 2e2e 3230 3231 2d30 382d 3330 2674 7970  ..2021-08-30&typ
-0000def0: 653d 4973 7375 6573 2920 7c20 5b40 6a61  e=Issues) | [@ja
-0000df00: 6e6b 6174 696e 735d 2868 7474 7073 3a2f  nkatins](https:/
-0000df10: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-0000df20: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-0000df30: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-0000df40: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-0000df50: 6a61 6e6b 6174 696e 732b 7570 6461 7465  jankatins+update
-0000df60: 6425 3341 3230 3231 2d30 382d 3230 2e2e  d%3A2021-08-20..
-0000df70: 3230 3231 2d30 382d 3330 2674 7970 653d  2021-08-30&type=
-0000df80: 4973 7375 6573 2920 7c20 5b40 6b65 7669  Issues) | [@kevi
-0000df90: 6e2d 6261 7465 735d 2868 7474 7073 3a2f  n-bates](https:/
-0000dfa0: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-0000dfb0: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-0000dfc0: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-0000dfd0: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-0000dfe0: 6b65 7669 6e2d 6261 7465 732b 7570 6461  kevin-bates+upda
-0000dff0: 7465 6425 3341 3230 3231 2d30 382d 3230  ted%3A2021-08-20
-0000e000: 2e2e 3230 3231 2d30 382d 3330 2674 7970  ..2021-08-30&typ
-0000e010: 653d 4973 7375 6573 2920 7c20 5b40 6d69  e=Issues) | [@mi
-0000e020: 6e72 6b5d 2868 7474 7073 3a2f 2f67 6974  nrk](https://git
-0000e030: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
-0000e040: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
-0000e050: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
-0000e060: 2b69 6e76 6f6c 7665 7325 3341 6d69 6e72  +involves%3Aminr
-0000e070: 6b2b 7570 6461 7465 6425 3341 3230 3231  k+updated%3A2021
-0000e080: 2d30 382d 3230 2e2e 3230 3231 2d30 382d  -08-20..2021-08-
-0000e090: 3330 2674 7970 653d 4973 7375 6573 2920  30&type=Issues) 
-0000e0a0: 7c20 5b40 7461 6b6c 7579 7665 725d 2868  | [@takluyver](h
-0000e0b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000e0c0: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
-0000e0d0: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
-0000e0e0: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
-0000e0f0: 7665 7325 3341 7461 6b6c 7579 7665 722b  ves%3Atakluyver+
-0000e100: 7570 6461 7465 6425 3341 3230 3231 2d30  updated%3A2021-0
-0000e110: 382d 3230 2e2e 3230 3231 2d30 382d 3330  8-20..2021-08-30
-0000e120: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
-0000e130: 5b40 7975 7669 7061 6e64 615d 2868 7474  [@yuvipanda](htt
-0000e140: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000e150: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
-0000e160: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
-0000e170: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
-0000e180: 7325 3341 7975 7669 7061 6e64 612b 7570  s%3Ayuvipanda+up
-0000e190: 6461 7465 6425 3341 3230 3231 2d30 382d  dated%3A2021-08-
-0000e1a0: 3230 2e2e 3230 3231 2d30 382d 3330 2674  20..2021-08-30&t
-0000e1b0: 7970 653d 4973 7375 6573 290a 0a23 2320  ype=Issues)..## 
-0000e1c0: 372e 302e 310a 0a28 5b46 756c 6c20 4368  7.0.1..([Full Ch
-0000e1d0: 616e 6765 6c6f 675d 2868 7474 7073 3a2f  angelog](https:/
-0000e1e0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-0000e1f0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-0000e200: 6e74 2f63 6f6d 7061 7265 2f76 372e 302e  nt/compare/v7.0.
-0000e210: 302e 2e2e 3063 6539 6632 3933 6561 3537  0...0ce9f293ea57
-0000e220: 3464 3631 6361 6534 3338 3436 3964 6635  4d61cae438469df5
-0000e230: 6535 3332 3938 3731 3362 3633 2929 0a0a  e53298713b63))..
-0000e240: 2323 2320 4d65 7267 6564 2050 5273 0a0a  ### Merged PRs..
-0000e250: 2d20 5573 6520 666f 726d 616c 206d 6574  - Use formal met
-0000e260: 686f 6420 6e61 6d65 7320 7768 656e 2063  hod names when c
-0000e270: 616c 6c65 6420 696e 7465 726e 616c 6c79  alled internally
-0000e280: 205b 2336 3833 5d28 6874 7470 733a 2f2f   [#683](https://
-0000e290: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-0000e2a0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-0000e2b0: 742f 7075 6c6c 2f36 3833 2920 285b 406b  t/pull/683) ([@k
-0000e2c0: 6576 696e 2d62 6174 6573 5d28 6874 7470  evin-bates](http
-0000e2d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
-0000e2e0: 6576 696e 2d62 6174 6573 2929 0a0a 2323  evin-bates))..##
-0000e2f0: 2320 436f 6e74 7269 6275 746f 7273 2074  # Contributors t
-0000e300: 6f20 7468 6973 2072 656c 6561 7365 0a0a  o this release..
-0000e310: 285b 4769 7448 7562 2063 6f6e 7472 6962  ([GitHub contrib
-0000e320: 7574 6f72 7320 7061 6765 2066 6f72 2074  utors page for t
-0000e330: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
-0000e340: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000e350: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-0000e360: 636c 6965 6e74 2f67 7261 7068 732f 636f  client/graphs/co
-0000e370: 6e74 7269 6275 746f 7273 3f66 726f 6d3d  ntributors?from=
-0000e380: 3230 3231 2d30 382d 3139 2674 6f3d 3230  2021-08-19&to=20
-0000e390: 3231 2d30 382d 3230 2674 7970 653d 6329  21-08-20&type=c)
-0000e3a0: 290a 0a5b 406b 6576 696e 2d62 6174 6573  )..[@kevin-bates
-0000e3b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000e3c0: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
-0000e3d0: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
-0000e3e0: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
-0000e3f0: 766f 6c76 6573 2533 416b 6576 696e 2d62  volves%3Akevin-b
-0000e400: 6174 6573 2b75 7064 6174 6564 2533 4132  ates+updated%3A2
-0000e410: 3032 312d 3038 2d31 392e 2e32 3032 312d  021-08-19..2021-
-0000e420: 3038 2d32 3026 7479 7065 3d49 7373 7565  08-20&type=Issue
-0000e430: 7329 0a0a 2323 2037 2e30 2e30 0a0a 285b  s)..## 7.0.0..([
-0000e440: 4675 6c6c 2043 6861 6e67 656c 6f67 5d28  Full Changelog](
-0000e450: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000e460: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-0000e470: 6572 5f63 6c69 656e 742f 636f 6d70 6172  er_client/compar
-0000e480: 652f 3236 6131 3663 3063 3931 6532 3435  e/26a16c0c91e245
-0000e490: 6637 3430 3361 6132 3761 3831 3266 6565  f7403aa27a812fee
-0000e4a0: 3565 3930 3564 3239 3634 2e2e 2e33 3137  5e905d2964...317
-0000e4b0: 3530 6263 3837 6261 6638 3833 3737 6263  50bc87baf88377bc
-0000e4c0: 6336 3936 3765 3232 3762 3635 3062 3338  c6967e227b650b38
-0000e4d0: 6661 3837 3229 290a 0a23 2323 2053 756d  fa872))..### Sum
-0000e4e0: 6d61 7279 0a0a 5468 6520 372e 3020 7265  mary..The 7.0 re
-0000e4f0: 6c65 6173 6520 6272 696e 6773 2061 206d  lease brings a m
-0000e500: 616a 6f72 2066 6561 7475 7265 2069 6e20  ajor feature in 
-0000e510: 5b4b 6572 6e65 6c20 5072 6f76 6973 696f  [Kernel Provisio
-0000e520: 6e65 7273 5d28 6874 7470 733a 2f2f 6769  ners](https://gi
-0000e530: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-0000e540: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-0000e550: 626c 6f62 2f6d 6173 7465 722f 646f 6373  blob/master/docs
-0000e560: 2f70 726f 7669 7369 6f6e 696e 672e 7273  /provisioning.rs
-0000e570: 7429 2c20 7768 6963 6820 656e 6162 6c65  t), which enable
-0000e580: 2074 6865 2061 6269 6c69 7479 2066 6f72   the ability for
-0000e590: 2074 6869 7264 2070 6172 7469 6573 2074   third parties t
-0000e5a0: 6f20 6d61 6e61 6765 2074 6865 206c 6966  o manage the lif
-0000e5b0: 6563 7963 6c65 206f 6620 6120 6b65 726e  ecycle of a kern
-0000e5c0: 656c 2773 2072 756e 7469 6d65 2065 6e76  el's runtime env
-0000e5d0: 6972 6f6e 6d65 6e74 2e0a 0a42 6569 6e67  ironment...Being
-0000e5e0: 2061 206d 616a 6f72 2072 656c 6561 7365   a major release
-0000e5f0: 2c20 7468 6572 6520 6172 6520 736f 6d65  , there are some
-0000e600: 2062 6163 6b77 6172 6420 696e 636f 6d70   backward incomp
-0000e610: 6174 6962 6c65 2063 6861 6e67 6573 2e20  atible changes. 
-0000e620: 506c 6561 7365 2073 6565 2074 6865 205b  Please see the [
-0000e630: 6d69 6772 6174 696f 6e20 6775 6964 655d  migration guide]
-0000e640: 2868 7474 7073 3a2f 2f6a 7570 7974 6572  (https://jupyter
-0000e650: 2d63 6c69 656e 742e 7265 6164 7468 6564  -client.readthed
-0000e660: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-0000e670: 2f6d 6967 7261 7469 6f6e 2e68 746d 6c29  /migration.html)
-0000e680: 2066 6f72 2066 7572 7468 6572 2064 6574   for further det
-0000e690: 6169 6c73 2e0a 0a23 2323 2045 6e68 616e  ails...### Enhan
-0000e6a0: 6365 6d65 6e74 7320 6d61 6465 0a0a 2d20  cements made..- 
-0000e6b0: 4b65 726e 656c 2050 726f 7669 7369 6f6e  Kernel Provision
-0000e6c0: 696e 6720 2d20 696e 6974 6961 6c20 696d  ing - initial im
-0000e6d0: 706c 656d 656e 7461 7469 6f6e 205b 2336  plementation [#6
-0000e6e0: 3132 5d28 6874 7470 733a 2f2f 6769 7468  12](https://gith
-0000e6f0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-0000e700: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-0000e710: 6c6c 2f36 3132 2920 285b 406b 6576 696e  ll/612) ([@kevin
-0000e720: 2d62 6174 6573 5d28 6874 7470 733a 2f2f  -bates](https://
-0000e730: 6769 7468 7562 2e63 6f6d 2f6b 6576 696e  github.com/kevin
-0000e740: 2d62 6174 6573 2929 0a0a 2323 2320 4275  -bates))..### Bu
-0000e750: 6773 2066 6978 6564 0a0a 2d20 4669 7820  gs fixed..- Fix 
-0000e760: 7570 2073 6f6d 6520 6173 796e 6320 6d65  up some async me
-0000e770: 7468 6f64 2061 6c69 6173 6573 2069 6e20  thod aliases in 
-0000e780: 4b65 726e 656c 4d61 6e61 6765 7220 5b23  KernelManager [#
-0000e790: 3637 305d 2868 7474 7073 3a2f 2f67 6974  670](https://git
-0000e7a0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-0000e7b0: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-0000e7c0: 756c 6c2f 3637 3029 2028 5b40 6b65 7669  ull/670) ([@kevi
-0000e7d0: 6e2d 6261 7465 735d 2868 7474 7073 3a2f  n-bates](https:/
-0000e7e0: 2f67 6974 6875 622e 636f 6d2f 6b65 7669  /github.com/kevi
-0000e7f0: 6e2d 6261 7465 7329 290a 2d20 5375 7070  n-bates)).- Supp
-0000e800: 6f72 7420 6061 6e73 7765 725f 7965 7360  ort `answer_yes`
-0000e810: 2077 6865 6e20 7265 6d6f 7669 6e67 206b   when removing k
-0000e820: 6572 6e65 6c20 7370 6563 7320 5b23 3635  ernel specs [#65
-0000e830: 395d 2868 7474 7073 3a2f 2f67 6974 6875  9](https://githu
-0000e840: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-0000e850: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-0000e860: 6c2f 3635 3929 2028 5b40 6461 7669 6462  l/659) ([@davidb
-0000e870: 726f 6368 6172 745d 2868 7474 7073 3a2f  rochart](https:/
-0000e880: 2f67 6974 6875 622e 636f 6d2f 6461 7669  /github.com/davi
-0000e890: 6462 726f 6368 6172 7429 290a 2d20 496e  dbrochart)).- In
-0000e8a0: 636c 7564 6520 7072 6f63 6573 7320 4944  clude process ID
-0000e8b0: 2069 6e20 6d65 7373 6167 6520 4944 205b   in message ID [
-0000e8c0: 2336 3535 5d28 6874 7470 733a 2f2f 6769  #655](https://gi
-0000e8d0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-0000e8e0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-0000e8f0: 7075 6c6c 2f36 3535 2920 285b 4074 616b  pull/655) ([@tak
-0000e900: 6c75 7976 6572 5d28 6874 7470 733a 2f2f  luyver](https://
-0000e910: 6769 7468 7562 2e63 6f6d 2f74 616b 6c75  github.com/taklu
-0000e920: 7976 6572 2929 0a2d 2046 6978 2071 7463  yver)).- Fix qtc
-0000e930: 6f6e 736f 6c65 2069 7373 7565 7320 5b23  onsole issues [#
-0000e940: 3633 385d 2868 7474 7073 3a2f 2f67 6974  638](https://git
-0000e950: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-0000e960: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-0000e970: 756c 6c2f 3633 3829 2028 5b40 6461 7669  ull/638) ([@davi
-0000e980: 6462 726f 6368 6172 745d 2868 7474 7073  dbrochart](https
-0000e990: 3a2f 2f67 6974 6875 622e 636f 6d2f 6461  ://github.com/da
-0000e9a0: 7669 6462 726f 6368 6172 7429 290a 0a23  vidbrochart))..#
-0000e9b0: 2323 204d 6169 6e74 656e 616e 6365 2061  ## Maintenance a
-0000e9c0: 6e64 2075 706b 6565 7020 696d 7072 6f76  nd upkeep improv
-0000e9d0: 656d 656e 7473 0a0a 2d20 4164 6465 6420  ements..- Added 
-0000e9e0: 6465 6275 6767 6572 206b 6579 2069 6e20  debugger key in 
-0000e9f0: 606b 6572 6e65 6c5f 696e 666f 5f72 6570  `kernel_info_rep
-0000ea00: 6c79 6020 5b23 3438 365d 2868 7474 7073  ly` [#486](https
-0000ea10: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-0000ea20: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-0000ea30: 6965 6e74 2f70 756c 6c2f 3438 3629 2028  ient/pull/486) (
-0000ea40: 5b40 4a6f 6861 6e4d 6162 696c 6c65 5d28  [@JohanMabille](
-0000ea50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000ea60: 6f6d 2f4a 6f68 616e 4d61 6269 6c6c 6529  om/JohanMabille)
-0000ea70: 290a 2d20 5072 6570 6172 6520 666f 7220  ).- Prepare for 
-0000ea80: 7573 6520 7769 7468 204a 7570 7974 6572  use with Jupyter
-0000ea90: 2052 656c 6561 7365 7220 5b23 3637 365d   Releaser [#676]
-0000eaa0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000eab0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-0000eac0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-0000ead0: 3637 3629 2028 5b40 6166 7368 696e 5d28  676) ([@afshin](
-0000eae0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000eaf0: 6f6d 2f61 6673 6869 6e29 290a 2d20 466f  om/afshin)).- Fo
-0000eb00: 7263 6520 696e 7374 616c 6c20 606a 7570  rce install `jup
-0000eb10: 7974 6572 5f63 6c69 656e 7460 206d 6173  yter_client` mas
-0000eb20: 7465 7220 5b23 3637 355d 2868 7474 7073  ter [#675](https
-0000eb30: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-0000eb40: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-0000eb50: 6965 6e74 2f70 756c 6c2f 3637 3529 2028  ient/pull/675) (
-0000eb60: 5b40 6461 7669 6462 726f 6368 6172 745d  [@davidbrochart]
-0000eb70: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000eb80: 636f 6d2f 6461 7669 6462 726f 6368 6172  com/davidbrochar
-0000eb90: 7429 290a 2d20 4669 7820 7072 6f6a 6563  t)).- Fix projec
-0000eba0: 7420 6e61 6d65 205b 2336 3734 5d28 6874  t name [#674](ht
+0000d030: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+0000d040: 6572 5f63 6c69 656e 742f 7075 6c6c 2f37  er_client/pull/7
+0000d050: 3230 2920 285b 4062 6c69 6e6b 3130 3733  20) ([@blink1073
+0000d060: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000d070: 2e63 6f6d 2f62 6c69 6e6b 3130 3733 2929  .com/blink1073))
+0000d080: 0a0a 2323 2320 436f 6e74 7269 6275 746f  ..### Contributo
+0000d090: 7273 2074 6f20 7468 6973 2072 656c 6561  rs to this relea
+0000d0a0: 7365 0a0a 285b 4769 7448 7562 2063 6f6e  se..([GitHub con
+0000d0b0: 7472 6962 7574 6f72 7320 7061 6765 2066  tributors page f
+0000d0c0: 6f72 2074 6869 7320 7265 6c65 6173 655d  or this release]
+0000d0d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000d0e0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+0000d0f0: 7465 725f 636c 6965 6e74 2f67 7261 7068  ter_client/graph
+0000d100: 732f 636f 6e74 7269 6275 746f 7273 3f66  s/contributors?f
+0000d110: 726f 6d3d 3230 3231 2d31 302d 3031 2674  rom=2021-10-01&t
+0000d120: 6f3d 3230 3231 2d31 312d 3232 2674 7970  o=2021-11-22&typ
+0000d130: 653d 6329 290a 0a5b 4062 6c69 6e6b 3130  e=c))..[@blink10
+0000d140: 3733 5d28 6874 7470 733a 2f2f 6769 7468  73](https://gith
+0000d150: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
+0000d160: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
+0000d170: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
+0000d180: 696e 766f 6c76 6573 2533 4162 6c69 6e6b  involves%3Ablink
+0000d190: 3130 3733 2b75 7064 6174 6564 2533 4132  1073+updated%3A2
+0000d1a0: 3032 312d 3130 2d30 312e 2e32 3032 312d  021-10-01..2021-
+0000d1b0: 3131 2d32 3226 7479 7065 3d49 7373 7565  11-22&type=Issue
+0000d1c0: 7329 207c 205b 4063 6934 6963 345d 2868  s) | [@ci4ic4](h
+0000d1d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000d1e0: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
+0000d1f0: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
+0000d200: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
+0000d210: 7665 7325 3341 6369 3469 6334 2b75 7064  ves%3Aci4ic4+upd
+0000d220: 6174 6564 2533 4132 3032 312d 3130 2d30  ated%3A2021-10-0
+0000d230: 312e 2e32 3032 312d 3131 2d32 3226 7479  1..2021-11-22&ty
+0000d240: 7065 3d49 7373 7565 7329 207c 205b 4064  pe=Issues) | [@d
+0000d250: 6176 6964 6272 6f63 6861 7274 5d28 6874  avidbrochart](ht
+0000d260: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000d270: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+0000d280: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+0000d290: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+0000d2a0: 6573 2533 4164 6176 6964 6272 6f63 6861  es%3Adavidbrocha
+0000d2b0: 7274 2b75 7064 6174 6564 2533 4132 3032  rt+updated%3A202
+0000d2c0: 312d 3130 2d30 312e 2e32 3032 312d 3131  1-10-01..2021-11
+0000d2d0: 2d32 3226 7479 7065 3d49 7373 7565 7329  -22&type=Issues)
+0000d2e0: 207c 205b 406b 6576 696e 2d62 6174 6573   | [@kevin-bates
+0000d2f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000d300: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
+0000d310: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
+0000d320: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
+0000d330: 766f 6c76 6573 2533 416b 6576 696e 2d62  volves%3Akevin-b
+0000d340: 6174 6573 2b75 7064 6174 6564 2533 4132  ates+updated%3A2
+0000d350: 3032 312d 3130 2d30 312e 2e32 3032 312d  021-10-01..2021-
+0000d360: 3131 2d32 3226 7479 7065 3d49 7373 7565  11-22&type=Issue
+0000d370: 7329 207c 205b 4076 6964 6172 7466 5d28  s) | [@vidartf](
+0000d380: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000d390: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
+0000d3a0: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
+0000d3b0: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
+0000d3c0: 6c76 6573 2533 4176 6964 6172 7466 2b75  lves%3Avidartf+u
+0000d3d0: 7064 6174 6564 2533 4132 3032 312d 3130  pdated%3A2021-10
+0000d3e0: 2d30 312e 2e32 3032 312d 3131 2d32 3226  -01..2021-11-22&
+0000d3f0: 7479 7065 3d49 7373 7565 7329 0a0a 2323  type=Issues)..##
+0000d400: 2037 2e30 2e36 0a0a 285b 4675 6c6c 2043   7.0.6..([Full C
+0000d410: 6861 6e67 656c 6f67 5d28 6874 7470 733a  hangelog](https:
+0000d420: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+0000d430: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+0000d440: 656e 742f 636f 6d70 6172 652f 7637 2e30  ent/compare/v7.0
+0000d450: 2e35 2e2e 2e35 3862 3131 6466 3065 6362  .5...58b11df0ecb
+0000d460: 3732 3965 6666 6163 6335 3963 6532 3865  729effacc59ce28e
+0000d470: 3966 3433 3166 6139 6336 6134 6429 290a  9f431fa9c6a4d)).
+0000d480: 0a23 2323 2042 7567 7320 6669 7865 640a  .### Bugs fixed.
+0000d490: 0a2d 2046 616c 6c62 6163 6b20 746f 2074  .- Fallback to t
+0000d4a0: 6865 206f 6c64 2069 7079 6b65 726e 656c  he old ipykernel
+0000d4b0: 2022 6a73 6f6e 5f63 6c65 616e 2220 6966   "json_clean" if
+0000d4c0: 2077 6520 6172 6520 6e6f 7420 6162 6c65   we are not able
+0000d4d0: 2074 6f20 7365 7269 616c 697a 6520 6120   to serialize a 
+0000d4e0: 4a53 4f4e 206d 6573 7361 6765 205b 2337  JSON message [#7
+0000d4f0: 3038 5d28 6874 7470 733a 2f2f 6769 7468  08](https://gith
+0000d500: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+0000d510: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+0000d520: 6c6c 2f37 3038 2920 285b 406d 6172 7469  ll/708) ([@marti
+0000d530: 6e52 656e 6f75 5d28 6874 7470 733a 2f2f  nRenou](https://
+0000d540: 6769 7468 7562 2e63 6f6d 2f6d 6172 7469  github.com/marti
+0000d550: 6e52 656e 6f75 2929 0a0a 2323 2320 4f74  nRenou))..### Ot
+0000d560: 6865 7220 6d65 7267 6564 2050 5273 0a0a  her merged PRs..
+0000d570: 2d20 4164 6420 7465 7374 2066 6f72 2073  - Add test for s
+0000d580: 6572 6961 6c69 7a69 6e67 2062 7974 6573  erializing bytes
+0000d590: 205b 2337 3037 5d28 6874 7470 733a 2f2f   [#707](https://
+0000d5a0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+0000d5b0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+0000d5c0: 742f 7075 6c6c 2f37 3037 2920 285b 406d  t/pull/707) ([@m
+0000d5d0: 6172 7469 6e52 656e 6f75 5d28 6874 7470  artinRenou](http
+0000d5e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+0000d5f0: 6172 7469 6e52 656e 6f75 2929 0a0a 2323  artinRenou))..##
+0000d600: 2320 436f 6e74 7269 6275 746f 7273 2074  # Contributors t
+0000d610: 6f20 7468 6973 2072 656c 6561 7365 0a0a  o this release..
+0000d620: 285b 4769 7448 7562 2063 6f6e 7472 6962  ([GitHub contrib
+0000d630: 7574 6f72 7320 7061 6765 2066 6f72 2074  utors page for t
+0000d640: 6869 7320 7265 6c65 6173 655d 2868 7474  his release](htt
+0000d650: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000d660: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+0000d670: 636c 6965 6e74 2f67 7261 7068 732f 636f  client/graphs/co
+0000d680: 6e74 7269 6275 746f 7273 3f66 726f 6d3d  ntributors?from=
+0000d690: 3230 3231 2d30 392d 3239 2674 6f3d 3230  2021-09-29&to=20
+0000d6a0: 3231 2d31 302d 3031 2674 7970 653d 6329  21-10-01&type=c)
+0000d6b0: 290a 0a5b 406d 6172 7469 6e52 656e 6f75  )..[@martinRenou
+0000d6c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000d6d0: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
+0000d6e0: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
+0000d6f0: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
+0000d700: 766f 6c76 6573 2533 416d 6172 7469 6e52  volves%3AmartinR
+0000d710: 656e 6f75 2b75 7064 6174 6564 2533 4132  enou+updated%3A2
+0000d720: 3032 312d 3039 2d32 392e 2e32 3032 312d  021-09-29..2021-
+0000d730: 3130 2d30 3126 7479 7065 3d49 7373 7565  10-01&type=Issue
+0000d740: 7329 0a0a 2323 2037 2e30 2e35 0a0a 285b  s)..## 7.0.5..([
+0000d750: 4675 6c6c 2043 6861 6e67 656c 6f67 5d28  Full Changelog](
+0000d760: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000d770: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+0000d780: 6572 5f63 6c69 656e 742f 636f 6d70 6172  er_client/compar
+0000d790: 652f 7637 2e30 2e34 2e2e 2e65 3337 3962  e/v7.0.4...e379b
+0000d7a0: 6639 3166 6561 3633 3532 3662 3963 3463  f91fea63526b9c4c
+0000d7b0: 6336 3637 3965 3739 3533 6133 3235 6235  c6679e7953a325b5
+0000d7c0: 3430 6329 290a 0a23 2323 2042 7567 7320  40c))..### Bugs 
+0000d7d0: 6669 7865 640a 0a2d 2061 766f 6964 2075  fixed..- avoid u
+0000d7e0: 7365 206f 6620 6465 7072 6563 6174 6564  se of deprecated
+0000d7f0: 207a 6d71 2e75 7469 6c73 2e6a 736f 6e61   zmq.utils.jsona
+0000d800: 7069 205b 2337 3033 5d28 6874 7470 733a  pi [#703](https:
+0000d810: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+0000d820: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+0000d830: 656e 742f 7075 6c6c 2f37 3033 2920 285b  ent/pull/703) ([
+0000d840: 406d 696e 726b 5d28 6874 7470 733a 2f2f  @minrk](https://
+0000d850: 6769 7468 7562 2e63 6f6d 2f6d 696e 726b  github.com/minrk
+0000d860: 2929 0a0a 2323 2320 4d61 696e 7465 6e61  ))..### Maintena
+0000d870: 6e63 6520 616e 6420 7570 6b65 6570 2069  nce and upkeep i
+0000d880: 6d70 726f 7665 6d65 6e74 730a 0a2d 2055  mprovements..- U
+0000d890: 7365 206c 6f67 6765 722e 7761 726e 696e  se logger.warnin
+0000d8a0: 6720 696e 7374 6561 6420 6f66 2064 6570  g instead of dep
+0000d8b0: 7265 6361 7465 6420 7761 726e 206d 6574  recated warn met
+0000d8c0: 686f 6420 5b23 3730 305d 2868 7474 7073  hod [#700](https
+0000d8d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+0000d8e0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+0000d8f0: 6965 6e74 2f70 756c 6c2f 3730 3029 2028  ient/pull/700) (
+0000d900: 5b40 6b65 7669 6e2d 6261 7465 735d 2868  [@kevin-bates](h
+0000d910: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000d920: 6d2f 6b65 7669 6e2d 6261 7465 7329 290a  m/kevin-bates)).
+0000d930: 0a23 2323 2043 6f6e 7472 6962 7574 6f72  .### Contributor
+0000d940: 7320 746f 2074 6869 7320 7265 6c65 6173  s to this releas
+0000d950: 650a 0a28 5b47 6974 4875 6220 636f 6e74  e..([GitHub cont
+0000d960: 7269 6275 746f 7273 2070 6167 6520 666f  ributors page fo
+0000d970: 7220 7468 6973 2072 656c 6561 7365 5d28  r this release](
+0000d980: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000d990: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+0000d9a0: 6572 5f63 6c69 656e 742f 6772 6170 6873  er_client/graphs
+0000d9b0: 2f63 6f6e 7472 6962 7574 6f72 733f 6672  /contributors?fr
+0000d9c0: 6f6d 3d32 3032 312d 3039 2d32 3826 746f  om=2021-09-28&to
+0000d9d0: 3d32 3032 312d 3039 2d32 3926 7479 7065  =2021-09-29&type
+0000d9e0: 3d63 2929 0a0a 5b40 6b65 7669 6e2d 6261  =c))..[@kevin-ba
+0000d9f0: 7465 735d 2868 7474 7073 3a2f 2f67 6974  tes](https://git
+0000da00: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
+0000da10: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
+0000da20: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
+0000da30: 2b69 6e76 6f6c 7665 7325 3341 6b65 7669  +involves%3Akevi
+0000da40: 6e2d 6261 7465 732b 7570 6461 7465 6425  n-bates+updated%
+0000da50: 3341 3230 3231 2d30 392d 3238 2e2e 3230  3A2021-09-28..20
+0000da60: 3231 2d30 392d 3239 2674 7970 653d 4973  21-09-29&type=Is
+0000da70: 7375 6573 2920 7c20 5b40 6d69 6e72 6b5d  sues) | [@minrk]
+0000da80: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000da90: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
+0000daa0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
+0000dab0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
+0000dac0: 6f6c 7665 7325 3341 6d69 6e72 6b2b 7570  olves%3Aminrk+up
+0000dad0: 6461 7465 6425 3341 3230 3231 2d30 392d  dated%3A2021-09-
+0000dae0: 3238 2e2e 3230 3231 2d30 392d 3239 2674  28..2021-09-29&t
+0000daf0: 7970 653d 4973 7375 6573 290a 0a23 2320  ype=Issues)..## 
+0000db00: 372e 302e 340a 0a28 5b46 756c 6c20 4368  7.0.4..([Full Ch
+0000db10: 616e 6765 6c6f 675d 2868 7474 7073 3a2f  angelog](https:/
+0000db20: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+0000db30: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+0000db40: 6e74 2f63 6f6d 7061 7265 2f76 372e 302e  nt/compare/v7.0.
+0000db50: 332e 2e2e 3562 3537 3031 3532 6330 6438  3...5b570152c0d8
+0000db60: 3864 6435 6530 6666 3137 3131 6337 3566  8dd5e0ff1711c75f
+0000db70: 6339 3938 3765 6637 3632 3536 2929 0a0a  c9987ef76256))..
+0000db80: 2323 2320 4275 6773 2066 6978 6564 0a0a  ### Bugs fixed..
+0000db90: 2d20 4669 7820 6a73 6f6e 5f64 6566 6175  - Fix json_defau
+0000dba0: 6c74 2073 6f20 7468 6174 2069 7427 7320  lt so that it's 
+0000dbb0: 636c 6f73 6572 2074 6f20 7768 6174 2069  closer to what i
+0000dbc0: 7079 6b65 726e 656c 2068 6164 2062 6566  pykernel had bef
+0000dbd0: 6f72 6520 5b23 3639 385d 2868 7474 7073  ore [#698](https
+0000dbe0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+0000dbf0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+0000dc00: 6965 6e74 2f70 756c 6c2f 3639 3829 2028  ient/pull/698) (
+0000dc10: 5b40 6d61 7274 696e 5265 6e6f 755d 2868  [@martinRenou](h
+0000dc20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000dc30: 6d2f 6d61 7274 696e 5265 6e6f 7529 290a  m/martinRenou)).
+0000dc40: 2d20 436c 6561 6e20 7570 2074 6865 2070  - Clean up the p
+0000dc50: 656e 6469 6e67 2074 6173 6b20 5b23 3639  ending task [#69
+0000dc60: 375d 2868 7474 7073 3a2f 2f67 6974 6875  7](https://githu
+0000dc70: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+0000dc80: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+0000dc90: 6c2f 3639 3729 2028 5b40 7368 696e 676f  l/697) ([@shingo
+0000dca0: 3738 5d28 6874 7470 733a 2f2f 6769 7468  78](https://gith
+0000dcb0: 7562 2e63 6f6d 2f73 6869 6e67 6f37 3829  ub.com/shingo78)
+0000dcc0: 290a 2d20 6669 7820 6b65 726e 656c 2063  ).- fix kernel c
+0000dcd0: 616e 206f 6e6c 7920 7265 7374 6172 7420  an only restart 
+0000dce0: 6f6e 6365 2069 7373 7565 205b 2336 3935  once issue [#695
+0000dcf0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000dd00: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+0000dd10: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+0000dd20: 2f36 3935 2920 285b 406d 6f66 616e 6b65  /695) ([@mofanke
+0000dd30: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000dd40: 2e63 6f6d 2f6d 6f66 616e 6b65 2929 0a2d  .com/mofanke)).-
+0000dd50: 2050 7265 7665 6e74 2066 6169 6c75 7265   Prevent failure
+0000dd60: 2069 6620 6b65 726e 656c 2069 7320 6e6f   if kernel is no
+0000dd70: 7420 666f 756e 6420 7768 656e 2073 6875  t found when shu
+0000dd80: 7474 696e 6720 6974 2064 6f77 6e20 5b23  tting it down [#
+0000dd90: 3639 345d 2868 7474 7073 3a2f 2f67 6974  694](https://git
+0000dda0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+0000ddb0: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+0000ddc0: 756c 6c2f 3639 3429 2028 5b40 6d61 7274  ull/694) ([@mart
+0000ddd0: 696e 5265 6e6f 755d 2868 7474 7073 3a2f  inRenou](https:/
+0000dde0: 2f67 6974 6875 622e 636f 6d2f 6d61 7274  /github.com/mart
+0000ddf0: 696e 5265 6e6f 7529 290a 0a23 2323 2043  inRenou))..### C
+0000de00: 6f6e 7472 6962 7574 6f72 7320 746f 2074  ontributors to t
+0000de10: 6869 7320 7265 6c65 6173 650a 0a28 5b47  his release..([G
+0000de20: 6974 4875 6220 636f 6e74 7269 6275 746f  itHub contributo
+0000de30: 7273 2070 6167 6520 666f 7220 7468 6973  rs page for this
+0000de40: 2072 656c 6561 7365 5d28 6874 7470 733a   release](https:
+0000de50: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+0000de60: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+0000de70: 656e 742f 6772 6170 6873 2f63 6f6e 7472  ent/graphs/contr
+0000de80: 6962 7574 6f72 733f 6672 6f6d 3d32 3032  ibutors?from=202
+0000de90: 312d 3039 2d31 3626 746f 3d32 3032 312d  1-09-16&to=2021-
+0000dea0: 3039 2d32 3826 7479 7065 3d63 2929 0a0a  09-28&type=c))..
+0000deb0: 5b40 6461 7669 6462 726f 6368 6172 745d  [@davidbrochart]
+0000dec0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000ded0: 636f 6d2f 7365 6172 6368 3f71 3d72 6570  com/search?q=rep
+0000dee0: 6f25 3341 6a75 7079 7465 7225 3246 6a75  o%3Ajupyter%2Fju
+0000def0: 7079 7465 725f 636c 6965 6e74 2b69 6e76  pyter_client+inv
+0000df00: 6f6c 7665 7325 3341 6461 7669 6462 726f  olves%3Adavidbro
+0000df10: 6368 6172 742b 7570 6461 7465 6425 3341  chart+updated%3A
+0000df20: 3230 3231 2d30 392d 3136 2e2e 3230 3231  2021-09-16..2021
+0000df30: 2d30 392d 3238 2674 7970 653d 4973 7375  -09-28&type=Issu
+0000df40: 6573 2920 7c20 5b40 6d61 7274 696e 5265  es) | [@martinRe
+0000df50: 6e6f 755d 2868 7474 7073 3a2f 2f67 6974  nou](https://git
+0000df60: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
+0000df70: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
+0000df80: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
+0000df90: 2b69 6e76 6f6c 7665 7325 3341 6d61 7274  +involves%3Amart
+0000dfa0: 696e 5265 6e6f 752b 7570 6461 7465 6425  inRenou+updated%
+0000dfb0: 3341 3230 3231 2d30 392d 3136 2e2e 3230  3A2021-09-16..20
+0000dfc0: 3231 2d30 392d 3238 2674 7970 653d 4973  21-09-28&type=Is
+0000dfd0: 7375 6573 2920 7c20 5b40 6d6f 6661 6e6b  sues) | [@mofank
+0000dfe0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+0000dff0: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
+0000e000: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
+0000e010: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
+0000e020: 6e76 6f6c 7665 7325 3341 6d6f 6661 6e6b  nvolves%3Amofank
+0000e030: 652b 7570 6461 7465 6425 3341 3230 3231  e+updated%3A2021
+0000e040: 2d30 392d 3136 2e2e 3230 3231 2d30 392d  -09-16..2021-09-
+0000e050: 3238 2674 7970 653d 4973 7375 6573 2920  28&type=Issues) 
+0000e060: 7c20 5b40 7368 696e 676f 3738 5d28 6874  | [@shingo78](ht
+0000e070: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000e080: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+0000e090: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+0000e0a0: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+0000e0b0: 6573 2533 4173 6869 6e67 6f37 382b 7570  es%3Ashingo78+up
+0000e0c0: 6461 7465 6425 3341 3230 3231 2d30 392d  dated%3A2021-09-
+0000e0d0: 3136 2e2e 3230 3231 2d30 392d 3238 2674  16..2021-09-28&t
+0000e0e0: 7970 653d 4973 7375 6573 290a 0a23 2320  ype=Issues)..## 
+0000e0f0: 372e 302e 330a 0a28 5b46 756c 6c20 4368  7.0.3..([Full Ch
+0000e100: 616e 6765 6c6f 675d 2868 7474 7073 3a2f  angelog](https:/
+0000e110: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+0000e120: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+0000e130: 6e74 2f63 6f6d 7061 7265 2f76 372e 302e  nt/compare/v7.0.
+0000e140: 322e 2e2e 6532 6538 3534 6334 3435 6436  2...e2e854c445d6
+0000e150: 3937 6165 3163 3138 3831 3731 6561 3037  97ae1c188171ea07
+0000e160: 3331 3533 3262 3661 6330 6439 2929 0a0a  31532b6ac0d9))..
+0000e170: 2323 2320 4275 6773 2066 6978 6564 0a0a  ### Bugs fixed..
+0000e180: 2d20 4164 6472 6573 7320 6d69 7373 696e  - Address missin
+0000e190: 6720 606c 6f63 616c 2d70 726f 7669 7369  g `local-provisi
+0000e1a0: 6f6e 6572 6020 7363 656e 6172 696f 205b  oner` scenario [
+0000e1b0: 2336 3932 5d28 6874 7470 733a 2f2f 6769  #692](https://gi
+0000e1c0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+0000e1d0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+0000e1e0: 7075 6c6c 2f36 3932 2920 285b 406b 6576  pull/692) ([@kev
+0000e1f0: 696e 2d62 6174 6573 5d28 6874 7470 733a  in-bates](https:
+0000e200: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 6576  //github.com/kev
+0000e210: 696e 2d62 6174 6573 2929 0a2d 2075 7365  in-bates)).- use
+0000e220: 2060 6c6f 6164 5f63 6f6e 6e65 6374 696f   `load_connectio
+0000e230: 6e5f 696e 666f 2869 6e66 6f29 6020 7768  n_info(info)` wh
+0000e240: 656e 2063 6f6e 7374 7275 6374 696e 6720  en constructing 
+0000e250: 6120 626c 6f63 6b69 6e67 2063 6c69 656e  a blocking clien
+0000e260: 7420 5b23 3638 385d 2868 7474 7073 3a2f  t [#688](https:/
+0000e270: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+0000e280: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+0000e290: 6e74 2f70 756c 6c2f 3638 3829 2028 5b40  nt/pull/688) ([@
+0000e2a0: 6d69 6e72 6b5d 2868 7474 7073 3a2f 2f67  minrk](https://g
+0000e2b0: 6974 6875 622e 636f 6d2f 6d69 6e72 6b29  ithub.com/minrk)
+0000e2c0: 290a 0a23 2323 2043 6f6e 7472 6962 7574  )..### Contribut
+0000e2d0: 6f72 7320 746f 2074 6869 7320 7265 6c65  ors to this rele
+0000e2e0: 6173 650a 0a28 5b47 6974 4875 6220 636f  ase..([GitHub co
+0000e2f0: 6e74 7269 6275 746f 7273 2070 6167 6520  ntributors page 
+0000e300: 666f 7220 7468 6973 2072 656c 6561 7365  for this release
+0000e310: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000e320: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+0000e330: 7974 6572 5f63 6c69 656e 742f 6772 6170  yter_client/grap
+0000e340: 6873 2f63 6f6e 7472 6962 7574 6f72 733f  hs/contributors?
+0000e350: 6672 6f6d 3d32 3032 312d 3038 2d33 3026  from=2021-08-30&
+0000e360: 746f 3d32 3032 312d 3039 2d31 3626 7479  to=2021-09-16&ty
+0000e370: 7065 3d63 2929 0a0a 5b40 6b65 7669 6e2d  pe=c))..[@kevin-
+0000e380: 6261 7465 735d 2868 7474 7073 3a2f 2f67  bates](https://g
+0000e390: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+0000e3a0: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+0000e3b0: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+0000e3c0: 6e74 2b69 6e76 6f6c 7665 7325 3341 6b65  nt+involves%3Ake
+0000e3d0: 7669 6e2d 6261 7465 732b 7570 6461 7465  vin-bates+update
+0000e3e0: 6425 3341 3230 3231 2d30 382d 3330 2e2e  d%3A2021-08-30..
+0000e3f0: 3230 3231 2d30 392d 3136 2674 7970 653d  2021-09-16&type=
+0000e400: 4973 7375 6573 2920 7c20 5b40 6d69 6e72  Issues) | [@minr
+0000e410: 6b5d 2868 7474 7073 3a2f 2f67 6974 6875  k](https://githu
+0000e420: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
+0000e430: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
+0000e440: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
+0000e450: 6e76 6f6c 7665 7325 3341 6d69 6e72 6b2b  nvolves%3Aminrk+
+0000e460: 7570 6461 7465 6425 3341 3230 3231 2d30  updated%3A2021-0
+0000e470: 382d 3330 2e2e 3230 3231 2d30 392d 3136  8-30..2021-09-16
+0000e480: 2674 7970 653d 4973 7375 6573 290a 0a23  &type=Issues)..#
+0000e490: 2320 372e 302e 320a 0a28 5b46 756c 6c20  # 7.0.2..([Full 
+0000e4a0: 4368 616e 6765 6c6f 675d 2868 7474 7073  Changelog](https
+0000e4b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+0000e4c0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+0000e4d0: 6965 6e74 2f63 6f6d 7061 7265 2f76 372e  ient/compare/v7.
+0000e4e0: 302e 312e 2e2e 6232 6132 3364 3866 3862  0.1...b2a23d8f8b
+0000e4f0: 3466 3234 6132 6263 3930 3862 3664 3935  4f24a2bc908b6d95
+0000e500: 3034 3732 3432 6634 6461 3837 6364 2929  047242f4da87cd))
+0000e510: 0a0a 2323 2320 4275 6773 2066 6978 6564  ..### Bugs fixed
+0000e520: 0a0a 2d20 446f 6e27 7420 7365 7420 6576  ..- Don't set ev
+0000e530: 656e 7420 6c6f 6f70 2070 6f6c 6963 7920  ent loop policy 
+0000e540: 6f6e 2057 696e 646f 7773 2061 7420 696d  on Windows at im
+0000e550: 706f 7274 2074 696d 6520 5b23 3638 365d  port time [#686]
+0000e560: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000e570: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+0000e580: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+0000e590: 3638 3629 2028 5b40 6d69 6e72 6b5d 2868  686) ([@minrk](h
+0000e5a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000e5b0: 6d2f 6d69 6e72 6b29 290a 0a23 2323 2044  m/minrk))..### D
+0000e5c0: 6f63 756d 656e 7461 7469 6f6e 2069 6d70  ocumentation imp
+0000e5d0: 726f 7665 6d65 6e74 730a 0a2d 2049 6d70  rovements..- Imp
+0000e5e0: 726f 7665 206d 6967 7261 7469 6f6e 2067  rove migration g
+0000e5f0: 7569 6465 205b 2336 3835 5d28 6874 7470  uide [#685](http
+0000e600: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+0000e610: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
+0000e620: 6c69 656e 742f 7075 6c6c 2f36 3835 2920  lient/pull/685) 
+0000e630: 285b 4064 6176 6964 6272 6f63 6861 7274  ([@davidbrochart
+0000e640: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000e650: 2e63 6f6d 2f64 6176 6964 6272 6f63 6861  .com/davidbrocha
+0000e660: 7274 2929 0a0a 2323 2320 436f 6e74 7269  rt))..### Contri
+0000e670: 6275 746f 7273 2074 6f20 7468 6973 2072  butors to this r
+0000e680: 656c 6561 7365 0a0a 285b 4769 7448 7562  elease..([GitHub
+0000e690: 2063 6f6e 7472 6962 7574 6f72 7320 7061   contributors pa
+0000e6a0: 6765 2066 6f72 2074 6869 7320 7265 6c65  ge for this rele
+0000e6b0: 6173 655d 2868 7474 7073 3a2f 2f67 6974  ase](https://git
+0000e6c0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+0000e6d0: 6a75 7079 7465 725f 636c 6965 6e74 2f67  jupyter_client/g
+0000e6e0: 7261 7068 732f 636f 6e74 7269 6275 746f  raphs/contributo
+0000e6f0: 7273 3f66 726f 6d3d 3230 3231 2d30 382d  rs?from=2021-08-
+0000e700: 3230 2674 6f3d 3230 3231 2d30 382d 3330  20&to=2021-08-30
+0000e710: 2674 7970 653d 6329 290a 0a5b 4062 6c69  &type=c))..[@bli
+0000e720: 6e6b 3130 3733 5d28 6874 7470 733a 2f2f  nk1073](https://
+0000e730: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
+0000e740: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
+0000e750: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
+0000e760: 656e 742b 696e 766f 6c76 6573 2533 4162  ent+involves%3Ab
+0000e770: 6c69 6e6b 3130 3733 2b75 7064 6174 6564  link1073+updated
+0000e780: 2533 4132 3032 312d 3038 2d32 302e 2e32  %3A2021-08-20..2
+0000e790: 3032 312d 3038 2d33 3026 7479 7065 3d49  021-08-30&type=I
+0000e7a0: 7373 7565 7329 207c 205b 4064 6176 6964  ssues) | [@david
+0000e7b0: 6272 6f63 6861 7274 5d28 6874 7470 733a  brochart](https:
+0000e7c0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+0000e7d0: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+0000e7e0: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+0000e7f0: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+0000e800: 4164 6176 6964 6272 6f63 6861 7274 2b75  Adavidbrochart+u
+0000e810: 7064 6174 6564 2533 4132 3032 312d 3038  pdated%3A2021-08
+0000e820: 2d32 302e 2e32 3032 312d 3038 2d33 3026  -20..2021-08-30&
+0000e830: 7479 7065 3d49 7373 7565 7329 207c 205b  type=Issues) | [
+0000e840: 4064 6869 7273 6368 6665 6c64 5d28 6874  @dhirschfeld](ht
+0000e850: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000e860: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+0000e870: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+0000e880: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+0000e890: 6573 2533 4164 6869 7273 6368 6665 6c64  es%3Adhirschfeld
+0000e8a0: 2b75 7064 6174 6564 2533 4132 3032 312d  +updated%3A2021-
+0000e8b0: 3038 2d32 302e 2e32 3032 312d 3038 2d33  08-20..2021-08-3
+0000e8c0: 3026 7479 7065 3d49 7373 7565 7329 207c  0&type=Issues) |
+0000e8d0: 205b 406a 616e 6b61 7469 6e73 5d28 6874   [@jankatins](ht
+0000e8e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000e8f0: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+0000e900: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+0000e910: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+0000e920: 6573 2533 416a 616e 6b61 7469 6e73 2b75  es%3Ajankatins+u
+0000e930: 7064 6174 6564 2533 4132 3032 312d 3038  pdated%3A2021-08
+0000e940: 2d32 302e 2e32 3032 312d 3038 2d33 3026  -20..2021-08-30&
+0000e950: 7479 7065 3d49 7373 7565 7329 207c 205b  type=Issues) | [
+0000e960: 406b 6576 696e 2d62 6174 6573 5d28 6874  @kevin-bates](ht
+0000e970: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000e980: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+0000e990: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+0000e9a0: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+0000e9b0: 6573 2533 416b 6576 696e 2d62 6174 6573  es%3Akevin-bates
+0000e9c0: 2b75 7064 6174 6564 2533 4132 3032 312d  +updated%3A2021-
+0000e9d0: 3038 2d32 302e 2e32 3032 312d 3038 2d33  08-20..2021-08-3
+0000e9e0: 3026 7479 7065 3d49 7373 7565 7329 207c  0&type=Issues) |
+0000e9f0: 205b 406d 696e 726b 5d28 6874 7470 733a   [@minrk](https:
+0000ea00: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+0000ea10: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+0000ea20: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+0000ea30: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+0000ea40: 416d 696e 726b 2b75 7064 6174 6564 2533  Aminrk+updated%3
+0000ea50: 4132 3032 312d 3038 2d32 302e 2e32 3032  A2021-08-20..202
+0000ea60: 312d 3038 2d33 3026 7479 7065 3d49 7373  1-08-30&type=Iss
+0000ea70: 7565 7329 207c 205b 4074 616b 6c75 7976  ues) | [@takluyv
+0000ea80: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
+0000ea90: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
+0000eaa0: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
+0000eab0: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
+0000eac0: 696e 766f 6c76 6573 2533 4174 616b 6c75  involves%3Ataklu
+0000ead0: 7976 6572 2b75 7064 6174 6564 2533 4132  yver+updated%3A2
+0000eae0: 3032 312d 3038 2d32 302e 2e32 3032 312d  021-08-20..2021-
+0000eaf0: 3038 2d33 3026 7479 7065 3d49 7373 7565  08-30&type=Issue
+0000eb00: 7329 207c 205b 4079 7576 6970 616e 6461  s) | [@yuvipanda
+0000eb10: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000eb20: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
+0000eb30: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
+0000eb40: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
+0000eb50: 766f 6c76 6573 2533 4179 7576 6970 616e  volves%3Ayuvipan
+0000eb60: 6461 2b75 7064 6174 6564 2533 4132 3032  da+updated%3A202
+0000eb70: 312d 3038 2d32 302e 2e32 3032 312d 3038  1-08-20..2021-08
+0000eb80: 2d33 3026 7479 7065 3d49 7373 7565 7329  -30&type=Issues)
+0000eb90: 0a0a 2323 2037 2e30 2e31 0a0a 285b 4675  ..## 7.0.1..([Fu
+0000eba0: 6c6c 2043 6861 6e67 656c 6f67 5d28 6874  ll Changelog](ht
 0000ebb0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 0000ebc0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-0000ebd0: 5f63 6c69 656e 742f 7075 6c6c 2f36 3734  _client/pull/674
-0000ebe0: 2920 285b 4076 6964 6172 7466 5d28 6874  ) ([@vidartf](ht
-0000ebf0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000ec00: 2f76 6964 6172 7466 2929 0a2d 2052 656e  /vidartf)).- Ren
-0000ec10: 616d 6520 7472 6169 7420 746f 2060 616c  ame trait to `al
-0000ec20: 6c6f 7765 645f 6b65 726e 656c 7370 6563  lowed_kernelspec
-0000ec30: 7360 205b 2336 3732 5d28 6874 7470 733a  s` [#672](https:
-0000ec40: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-0000ec50: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-0000ec60: 656e 742f 7075 6c6c 2f36 3732 2920 285b  ent/pull/672) ([
-0000ec70: 4062 6c69 6e6b 3130 3733 5d28 6874 7470  @blink1073](http
-0000ec80: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-0000ec90: 6c69 6e6b 3130 3733 2929 0a2d 2052 656d  link1073)).- Rem
-0000eca0: 6f76 6520 626c 6f63 6b20 7061 7261 6d65  ove block parame
-0000ecb0: 7465 7220 6672 6f6d 2060 6765 745f 6d73  ter from `get_ms
-0000ecc0: 6728 2960 205b 2336 3731 5d28 6874 7470  g()` [#671](http
-0000ecd0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-0000ece0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-0000ecf0: 6c69 656e 742f 7075 6c6c 2f36 3731 2920  lient/pull/671) 
-0000ed00: 285b 4064 6176 6964 6272 6f63 6861 7274  ([@davidbrochart
+0000ebd0: 5f63 6c69 656e 742f 636f 6d70 6172 652f  _client/compare/
+0000ebe0: 7637 2e30 2e30 2e2e 2e30 6365 3966 3239  v7.0.0...0ce9f29
+0000ebf0: 3365 6135 3734 6436 3163 6165 3433 3834  3ea574d61cae4384
+0000ec00: 3639 6466 3565 3533 3239 3837 3133 6236  69df5e53298713b6
+0000ec10: 3329 290a 0a23 2323 204d 6572 6765 6420  3))..### Merged 
+0000ec20: 5052 730a 0a2d 2055 7365 2066 6f72 6d61  PRs..- Use forma
+0000ec30: 6c20 6d65 7468 6f64 206e 616d 6573 2077  l method names w
+0000ec40: 6865 6e20 6361 6c6c 6564 2069 6e74 6572  hen called inter
+0000ec50: 6e61 6c6c 7920 5b23 3638 335d 2868 7474  nally [#683](htt
+0000ec60: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000ec70: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+0000ec80: 636c 6965 6e74 2f70 756c 6c2f 3638 3329  client/pull/683)
+0000ec90: 2028 5b40 6b65 7669 6e2d 6261 7465 735d   ([@kevin-bates]
+0000eca0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000ecb0: 636f 6d2f 6b65 7669 6e2d 6261 7465 7329  com/kevin-bates)
+0000ecc0: 290a 0a23 2323 2043 6f6e 7472 6962 7574  )..### Contribut
+0000ecd0: 6f72 7320 746f 2074 6869 7320 7265 6c65  ors to this rele
+0000ece0: 6173 650a 0a28 5b47 6974 4875 6220 636f  ase..([GitHub co
+0000ecf0: 6e74 7269 6275 746f 7273 2070 6167 6520  ntributors page 
+0000ed00: 666f 7220 7468 6973 2072 656c 6561 7365  for this release
 0000ed10: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000ed20: 2e63 6f6d 2f64 6176 6964 6272 6f63 6861  .com/davidbrocha
-0000ed30: 7274 2929 0a2d 204f 6e6c 7920 696d 706f  rt)).- Only impo
-0000ed40: 7274 2060 6e65 7374 5f61 7379 6e63 696f  rt `nest_asyncio
-0000ed50: 6020 6c6f 6361 6c6c 7920 5b23 3636 355d  ` locally [#665]
-0000ed60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000ed70: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-0000ed80: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-0000ed90: 3636 3529 2028 5b40 5379 6c76 6169 6e43  665) ([@SylvainC
-0000eda0: 6f72 6c61 795d 2868 7474 7073 3a2f 2f67  orlay](https://g
-0000edb0: 6974 6875 622e 636f 6d2f 5379 6c76 6169  ithub.com/Sylvai
-0000edc0: 6e43 6f72 6c61 7929 290a 2d20 5573 6520  nCorlay)).- Use 
-0000edd0: 6120 6465 6661 756c 7420 7365 7269 616c  a default serial
-0000ede0: 697a 6572 2074 6861 7420 6973 206e 6f74  izer that is not
-0000edf0: 206f 6e6c 7920 666f 7220 6461 7465 2074   only for date t
-0000ee00: 7970 6573 205b 2336 3634 5d28 6874 7470  ypes [#664](http
-0000ee10: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-0000ee20: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-0000ee30: 6c69 656e 742f 7075 6c6c 2f36 3634 2920  lient/pull/664) 
-0000ee40: 285b 406d 6172 7469 6e52 656e 6f75 5d28  ([@martinRenou](
-0000ee50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000ee60: 6f6d 2f6d 6172 7469 6e52 656e 6f75 2929  om/martinRenou))
-0000ee70: 0a2d 2055 7064 6174 6564 2060 6465 6275  .- Updated `debu
-0000ee80: 675f 696e 666f 5f72 6573 706f 6e73 6560  g_info_response`
-0000ee90: 205b 2336 3537 5d28 6874 7470 733a 2f2f   [#657](https://
-0000eea0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-0000eeb0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-0000eec0: 742f 7075 6c6c 2f36 3537 2920 285b 404a  t/pull/657) ([@J
-0000eed0: 6f68 616e 4d61 6269 6c6c 655d 2868 7474  ohanMabille](htt
-0000eee0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000eef0: 4a6f 6861 6e4d 6162 696c 6c65 2929 0a2d  JohanMabille)).-
-0000ef00: 2044 6f20 6e6f 7420 626c 6f63 6b20 6f6e   Do not block on
-0000ef10: 2065 7869 7420 5b23 3635 315d 2868 7474   exit [#651](htt
-0000ef20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000ef30: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-0000ef40: 636c 6965 6e74 2f70 756c 6c2f 3635 3129  client/pull/651)
-0000ef50: 2028 5b40 696d 7061 6374 3237 5d28 6874   ([@impact27](ht
-0000ef60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000ef70: 2f69 6d70 6163 7432 3729 290a 2d20 5570  /impact27)).- Up
-0000ef80: 6461 7465 2074 6573 7420 6b65 726e 656c  date test kernel
-0000ef90: 2077 6974 6820 6e61 7469 7665 2063 6f72   with native cor
-0000efa0: 6f75 7469 6e65 2c20 7265 6d6f 7665 2060  outine, remove `
-0000efb0: 6173 796e 635f 6765 6e65 7261 746f 7260  async_generator`
-0000efc0: 2064 6570 656e 6465 6e63 7920 5b23 3634   dependency [#64
-0000efd0: 365d 2868 7474 7073 3a2f 2f67 6974 6875  6](https://githu
-0000efe0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-0000eff0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-0000f000: 6c2f 3634 3629 2028 5b40 6b65 7669 6e2d  l/646) ([@kevin-
-0000f010: 6261 7465 735d 2868 7474 7073 3a2f 2f67  bates](https://g
-0000f020: 6974 6875 622e 636f 6d2f 6b65 7669 6e2d  ithub.com/kevin-
-0000f030: 6261 7465 7329 290a 2d20 6073 6574 7570  bates)).- `setup
-0000f040: 2e70 7960 2061 6e64 2043 4920 696d 7072  .py` and CI impr
-0000f050: 6f76 656d 656e 7473 205b 2336 3435 5d28  ovements [#645](
-0000f060: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000f070: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-0000f080: 6572 5f63 6c69 656e 742f 7075 6c6c 2f36  er_client/pull/6
-0000f090: 3435 2920 285b 4064 6f6c 6669 6e75 735d  45) ([@dolfinus]
-0000f0a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000f0b0: 636f 6d2f 646f 6c66 696e 7573 2929 0a2d  com/dolfinus)).-
-0000f0c0: 2054 6573 7420 646f 776e 7374 7265 616d   Test downstream
-0000f0d0: 2070 726f 6a65 6374 7320 5b23 3634 345d   projects [#644]
-0000f0e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000f0f0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-0000f100: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-0000f110: 3634 3429 2028 5b40 6461 7669 6462 726f  644) ([@davidbro
-0000f120: 6368 6172 745d 2868 7474 7073 3a2f 2f67  chart](https://g
-0000f130: 6974 6875 622e 636f 6d2f 6461 7669 6462  ithub.com/davidb
-0000f140: 726f 6368 6172 7429 290a 2d20 5265 6d6f  rochart)).- Remo
-0000f150: 7665 2064 6570 7265 6361 7469 6f6e 7320  ve deprecations 
-0000f160: 696e 206b 6572 6e65 6c20 6d61 6e61 6765  in kernel manage
-0000f170: 7220 5b23 3634 335d 2868 7474 7073 3a2f  r [#643](https:/
-0000f180: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-0000f190: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-0000f1a0: 6e74 2f70 756c 6c2f 3634 3329 2028 5b40  nt/pull/643) ([@
-0000f1b0: 6b65 7669 6e2d 6261 7465 735d 2868 7474  kevin-bates](htt
-0000f1c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000f1d0: 6b65 7669 6e2d 6261 7465 7329 290a 2d20  kevin-bates)).- 
-0000f1e0: 4164 6420 6062 6c6f 636b 3d54 7275 6560  Add `block=True`
-0000f1f0: 2062 6163 6b20 746f 2060 6765 745f 6d73   back to `get_ms
-0000f200: 6728 2960 205b 2336 3431 5d28 6874 7470  g()` [#641](http
-0000f210: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-0000f220: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-0000f230: 6c69 656e 742f 7075 6c6c 2f36 3431 2920  lient/pull/641) 
-0000f240: 285b 4064 6176 6964 6272 6f63 6861 7274  ([@davidbrochart
-0000f250: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000f260: 2e63 6f6d 2f64 6176 6964 6272 6f63 6861  .com/davidbrocha
-0000f270: 7274 2929 0a2d 2050 696e 2060 7079 7468  rt)).- Pin `pyth
-0000f280: 6f6e 3e3d 332e 362e 3160 205b 2336 3336  on>=3.6.1` [#636
-0000f290: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000f2a0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-0000f2b0: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-0000f2c0: 2f36 3336 2920 285b 4064 6176 6964 6272  /636) ([@davidbr
-0000f2d0: 6f63 6861 7274 5d28 6874 7470 733a 2f2f  ochart](https://
-0000f2e0: 6769 7468 7562 2e63 6f6d 2f64 6176 6964  github.com/david
-0000f2f0: 6272 6f63 6861 7274 2929 0a2d 2055 7365  brochart)).- Use
-0000f300: 2060 7072 652d 636f 6d6d 6974 6020 5b23   `pre-commit` [#
-0000f310: 3633 315d 2868 7474 7073 3a2f 2f67 6974  631](https://git
-0000f320: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-0000f330: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-0000f340: 756c 6c2f 3633 3129 2028 5b40 6461 7669  ull/631) ([@davi
-0000f350: 6462 726f 6368 6172 745d 2868 7474 7073  dbrochart](https
-0000f360: 3a2f 2f67 6974 6875 622e 636f 6d2f 6461  ://github.com/da
-0000f370: 7669 6462 726f 6368 6172 7429 290a 2d20  vidbrochart)).- 
-0000f380: 4174 7465 6d70 7420 4349 2077 6974 6820  Attempt CI with 
-0000f390: 6069 7079 6b65 726e 656c 6020 362e 3020  `ipykernel` 6.0 
-0000f3a0: 7072 6572 656c 6561 7365 205b 2336 3239  prerelease [#629
-0000f3b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000f3c0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-0000f3d0: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-0000f3e0: 2f36 3239 2920 285b 4053 796c 7661 696e  /629) ([@Sylvain
-0000f3f0: 436f 726c 6179 5d28 6874 7470 733a 2f2f  Corlay](https://
-0000f400: 6769 7468 7562 2e63 6f6d 2f53 796c 7661  github.com/Sylva
-0000f410: 696e 436f 726c 6179 2929 0a2d 204d 616b  inCorlay)).- Mak
-0000f420: 6520 604b 6572 6e65 6c4d 616e 6167 6572  e `KernelManager
-0000f430: 6020 7375 6263 6c61 7373 2074 6573 7473  ` subclass tests
-0000f440: 2044 5259 205b 2336 3238 5d28 6874 7470   DRY [#628](http
-0000f450: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-0000f460: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-0000f470: 6c69 656e 742f 7075 6c6c 2f36 3238 2920  lient/pull/628) 
-0000f480: 285b 4064 6176 6964 6272 6f63 6861 7274  ([@davidbrochart
-0000f490: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000f4a0: 2e63 6f6d 2f64 6176 6964 6272 6f63 6861  .com/davidbrocha
-0000f4b0: 7274 2929 0a2d 2041 6464 2074 6573 7473  rt)).- Add tests
-0000f4c0: 2074 6f20 656e 7375 7265 204d 756c 7469   to ensure Multi
-0000f4d0: 4b65 726e 656c 4d61 6e61 6765 7220 7375  KernelManager su
-0000f4e0: 6263 6c61 7373 206d 6574 686f 6473 2061  bclass methods a
-0000f4f0: 7265 2063 616c 6c65 6420 5b23 3632 375d  re called [#627]
-0000f500: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000f510: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-0000f520: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-0000f530: 3632 3729 2028 5b40 6b65 7669 6e2d 6261  627) ([@kevin-ba
-0000f540: 7465 735d 2868 7474 7073 3a2f 2f67 6974  tes](https://git
-0000f550: 6875 622e 636f 6d2f 6b65 7669 6e2d 6261  hub.com/kevin-ba
-0000f560: 7465 7329 290a 2d20 4164 6420 7479 7065  tes)).- Add type
-0000f570: 2061 6e6e 6f74 6174 696f 6e73 2c20 7265   annotations, re
-0000f580: 6661 6374 6f72 2073 796e 632f 6173 796e  factor sync/asyn
-0000f590: 6320 5b23 3632 335d 2868 7474 7073 3a2f  c [#623](https:/
-0000f5a0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-0000f5b0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-0000f5c0: 6e74 2f70 756c 6c2f 3632 3329 2028 5b40  nt/pull/623) ([@
-0000f5d0: 6461 7669 6462 726f 6368 6172 745d 2868  davidbrochart](h
-0000f5e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000f5f0: 6d2f 6461 7669 6462 726f 6368 6172 7429  m/davidbrochart)
-0000f600: 290a 0a23 2323 2044 6f63 756d 656e 7461  )..### Documenta
-0000f610: 7469 6f6e 2069 6d70 726f 7665 6d65 6e74  tion improvement
-0000f620: 730a 0a2d 2043 7265 6174 6520 6d69 6772  s..- Create migr
-0000f630: 6174 696f 6e20 6775 6964 6520 5b23 3638  ation guide [#68
-0000f640: 315d 2868 7474 7073 3a2f 2f67 6974 6875  1](https://githu
-0000f650: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-0000f660: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-0000f670: 6c2f 3638 3129 2028 5b40 626c 696e 6b31  l/681) ([@blink1
-0000f680: 3037 335d 2868 7474 7073 3a2f 2f67 6974  073](https://git
-0000f690: 6875 622e 636f 6d2f 626c 696e 6b31 3037  hub.com/blink107
-0000f6a0: 3329 290a 2d20 5570 6461 7465 2063 6861  3)).- Update cha
-0000f6b0: 6e67 656c 6f67 2066 6f72 2037 2e30 2e30  ngelog for 7.0.0
-0000f6c0: 7263 3020 5b23 3637 335d 2868 7474 7073  rc0 [#673](https
-0000f6d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-0000f6e0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-0000f6f0: 6965 6e74 2f70 756c 6c2f 3637 3329 2028  ient/pull/673) (
-0000f700: 5b40 626c 696e 6b31 3037 335d 2868 7474  [@blink1073](htt
-0000f710: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000f720: 626c 696e 6b31 3037 3329 290a 2d20 4164  blink1073)).- Ad
-0000f730: 6465 6420 646f 6375 6d65 6e74 6174 696f  ded documentatio
-0000f740: 6e20 666f 7220 6072 6963 6849 6e73 7065  n for `richInspe
-0000f750: 6374 5661 7269 6162 6c65 7360 2072 6571  ctVariables` req
-0000f760: 7565 7374 205b 2336 3534 5d28 6874 7470  uest [#654](http
-0000f770: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-0000f780: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-0000f790: 6c69 656e 742f 7075 6c6c 2f36 3534 2920  lient/pull/654) 
-0000f7a0: 285b 404a 6f68 616e 4d61 6269 6c6c 655d  ([@JohanMabille]
-0000f7b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000f7c0: 636f 6d2f 4a6f 6861 6e4d 6162 696c 6c65  com/JohanMabille
-0000f7d0: 2929 0a2d 2043 6861 6e67 6520 746f 2060  )).- Change to `
-0000f7e0: 6564 6974 5f6d 6167 6963 6020 7061 796c  edit_magic` payl
-0000f7f0: 6f61 6420 5b23 3635 325d 2868 7474 7073  oad [#652](https
-0000f800: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-0000f810: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-0000f820: 6965 6e74 2f70 756c 6c2f 3635 3229 2028  ient/pull/652) (
-0000f830: 5b40 7969 747a 6368 616b 5d28 6874 7470  [@yitzchak](http
-0000f840: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f79  s://github.com/y
-0000f850: 6974 7a63 6861 6b29 290a 2d20 4164 6465  itzchak)).- Adde
-0000f860: 6420 6d69 7373 696e 6720 646f 6375 6d65  d missing docume
-0000f870: 6e74 6174 696f 6e20 666f 7220 7468 6520  ntation for the 
-0000f880: 696e 7370 6563 7456 6172 6961 626c 6573  inspectVariables
-0000f890: 2072 6571 7565 7374 2061 6e64 2072 6573   request and res
-0000f8a0: 70e2 80a6 205b 2336 3439 5d28 6874 7470  p... [#649](http
-0000f8b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-0000f8c0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-0000f8d0: 6c69 656e 742f 7075 6c6c 2f36 3439 2920  lient/pull/649) 
-0000f8e0: 285b 404a 6f68 616e 4d61 6269 6c6c 655d  ([@JohanMabille]
-0000f8f0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000f900: 636f 6d2f 4a6f 6861 6e4d 6162 696c 6c65  com/JohanMabille
-0000f910: 2929 0a2d 2041 6464 2073 7461 7475 7320  )).- Add status 
-0000f920: 6669 656c 6420 746f 206f 7468 6572 2072  field to other r
-0000f930: 6570 6c69 6573 2069 6e20 646f 6375 6d65  eplies in docume
-0000f940: 6e74 6174 696f 6e20 5b23 3634 385d 2868  ntation [#648](h
-0000f950: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000f960: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-0000f970: 725f 636c 6965 6e74 2f70 756c 6c2f 3634  r_client/pull/64
-0000f980: 3829 2028 5b40 7969 747a 6368 616b 5d28  8) ([@yitzchak](
-0000f990: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000f9a0: 6f6d 2f79 6974 7a63 6861 6b29 290a 0a23  om/yitzchak))..#
-0000f9b0: 2323 2043 6f6e 7472 6962 7574 6f72 7320  ## Contributors 
-0000f9c0: 746f 2074 6869 7320 7265 6c65 6173 650a  to this release.
-0000f9d0: 0a28 5b47 6974 4875 6220 636f 6e74 7269  .([GitHub contri
-0000f9e0: 6275 746f 7273 2070 6167 6520 666f 7220  butors page for 
-0000f9f0: 7468 6973 2072 656c 6561 7365 5d28 6874  this release](ht
-0000fa00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000fa10: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-0000fa20: 5f63 6c69 656e 742f 6772 6170 6873 2f63  _client/graphs/c
-0000fa30: 6f6e 7472 6962 7574 6f72 733f 6672 6f6d  ontributors?from
-0000fa40: 3d32 3032 312d 3033 2d31 3426 746f 3d32  =2021-03-14&to=2
-0000fa50: 3032 312d 3038 2d31 3626 7479 7065 3d63  021-08-16&type=c
-0000fa60: 2929 0a0a 5b40 6166 7368 696e 5d28 6874  ))..[@afshin](ht
-0000fa70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000fa80: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
-0000fa90: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
-0000faa0: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
-0000fab0: 6573 2533 4161 6673 6869 6e2b 7570 6461  es%3Aafshin+upda
-0000fac0: 7465 6425 3341 3230 3231 2d30 332d 3134  ted%3A2021-03-14
-0000fad0: 2e2e 3230 3231 2d30 382d 3136 2674 7970  ..2021-08-16&typ
-0000fae0: 653d 4973 7375 6573 2920 7c20 5b40 626c  e=Issues) | [@bl
-0000faf0: 696e 6b31 3037 335d 2868 7474 7073 3a2f  ink1073](https:/
-0000fb00: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-0000fb10: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-0000fb20: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-0000fb30: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-0000fb40: 626c 696e 6b31 3037 332b 7570 6461 7465  blink1073+update
-0000fb50: 6425 3341 3230 3231 2d30 332d 3134 2e2e  d%3A2021-03-14..
-0000fb60: 3230 3231 2d30 382d 3136 2674 7970 653d  2021-08-16&type=
-0000fb70: 4973 7375 6573 2920 7c20 5b40 4361 7272  Issues) | [@Carr
-0000fb80: 6561 755d 2868 7474 7073 3a2f 2f67 6974  eau](https://git
-0000fb90: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
-0000fba0: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
-0000fbb0: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
-0000fbc0: 2b69 6e76 6f6c 7665 7325 3341 4361 7272  +involves%3ACarr
-0000fbd0: 6561 752b 7570 6461 7465 6425 3341 3230  eau+updated%3A20
-0000fbe0: 3231 2d30 332d 3134 2e2e 3230 3231 2d30  21-03-14..2021-0
-0000fbf0: 382d 3136 2674 7970 653d 4973 7375 6573  8-16&type=Issues
-0000fc00: 2920 7c20 5b40 6363 6f72 646f 6261 3132  ) | [@ccordoba12
-0000fc10: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-0000fc20: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
-0000fc30: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
-0000fc40: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
-0000fc50: 766f 6c76 6573 2533 4163 636f 7264 6f62  volves%3Accordob
-0000fc60: 6131 322b 7570 6461 7465 6425 3341 3230  a12+updated%3A20
-0000fc70: 3231 2d30 332d 3134 2e2e 3230 3231 2d30  21-03-14..2021-0
-0000fc80: 382d 3136 2674 7970 653d 4973 7375 6573  8-16&type=Issues
-0000fc90: 2920 7c20 5b40 6461 7669 6462 726f 6368  ) | [@davidbroch
-0000fca0: 6172 745d 2868 7474 7073 3a2f 2f67 6974  art](https://git
-0000fcb0: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
-0000fcc0: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
-0000fcd0: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
-0000fce0: 2b69 6e76 6f6c 7665 7325 3341 6461 7669  +involves%3Adavi
-0000fcf0: 6462 726f 6368 6172 742b 7570 6461 7465  dbrochart+update
-0000fd00: 6425 3341 3230 3231 2d30 332d 3134 2e2e  d%3A2021-03-14..
-0000fd10: 3230 3231 2d30 382d 3136 2674 7970 653d  2021-08-16&type=
-0000fd20: 4973 7375 6573 2920 7c20 5b40 6468 6972  Issues) | [@dhir
-0000fd30: 7363 6866 656c 645d 2868 7474 7073 3a2f  schfeld](https:/
-0000fd40: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-0000fd50: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-0000fd60: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-0000fd70: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-0000fd80: 6468 6972 7363 6866 656c 642b 7570 6461  dhirschfeld+upda
-0000fd90: 7465 6425 3341 3230 3231 2d30 332d 3134  ted%3A2021-03-14
-0000fda0: 2e2e 3230 3231 2d30 382d 3136 2674 7970  ..2021-08-16&typ
-0000fdb0: 653d 4973 7375 6573 2920 7c20 5b40 646f  e=Issues) | [@do
-0000fdc0: 6c66 696e 7573 5d28 6874 7470 733a 2f2f  lfinus](https://
-0000fdd0: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
-0000fde0: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
-0000fdf0: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
-0000fe00: 656e 742b 696e 766f 6c76 6573 2533 4164  ent+involves%3Ad
-0000fe10: 6f6c 6669 6e75 732b 7570 6461 7465 6425  olfinus+updated%
-0000fe20: 3341 3230 3231 2d30 332d 3134 2e2e 3230  3A2021-03-14..20
-0000fe30: 3231 2d30 382d 3136 2674 7970 653d 4973  21-08-16&type=Is
-0000fe40: 7375 6573 2920 7c20 5b40 6563 6861 726c  sues) | [@echarl
-0000fe50: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-0000fe60: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
-0000fe70: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
-0000fe80: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
-0000fe90: 696e 766f 6c76 6573 2533 4165 6368 6172  involves%3Aechar
-0000fea0: 6c65 732b 7570 6461 7465 6425 3341 3230  les+updated%3A20
-0000feb0: 3231 2d30 332d 3134 2e2e 3230 3231 2d30  21-03-14..2021-0
-0000fec0: 382d 3136 2674 7970 653d 4973 7375 6573  8-16&type=Issues
-0000fed0: 2920 7c20 5b40 696d 7061 6374 3237 5d28  ) | [@impact27](
-0000fee0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000fef0: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
-0000ff00: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
-0000ff10: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
-0000ff20: 6c76 6573 2533 4169 6d70 6163 7432 372b  lves%3Aimpact27+
-0000ff30: 7570 6461 7465 6425 3341 3230 3231 2d30  updated%3A2021-0
-0000ff40: 332d 3134 2e2e 3230 3231 2d30 382d 3136  3-14..2021-08-16
-0000ff50: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
-0000ff60: 5b40 4a6f 6861 6e4d 6162 696c 6c65 5d28  [@JohanMabille](
-0000ff70: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000ff80: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
-0000ff90: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
-0000ffa0: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
-0000ffb0: 6c76 6573 2533 414a 6f68 616e 4d61 6269  lves%3AJohanMabi
-0000ffc0: 6c6c 652b 7570 6461 7465 6425 3341 3230  lle+updated%3A20
-0000ffd0: 3231 2d30 332d 3134 2e2e 3230 3231 2d30  21-03-14..2021-0
-0000ffe0: 382d 3136 2674 7970 653d 4973 7375 6573  8-16&type=Issues
-0000fff0: 2920 7c20 5b40 6b65 7669 6e2d 6261 7465  ) | [@kevin-bate
-00010000: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00010010: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
-00010020: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
-00010030: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
-00010040: 6e76 6f6c 7665 7325 3341 6b65 7669 6e2d  nvolves%3Akevin-
-00010050: 6261 7465 732b 7570 6461 7465 6425 3341  bates+updated%3A
-00010060: 3230 3231 2d30 332d 3134 2e2e 3230 3231  2021-03-14..2021
-00010070: 2d30 382d 3136 2674 7970 653d 4973 7375  -08-16&type=Issu
-00010080: 6573 2920 7c20 5b40 6d61 7274 696e 5265  es) | [@martinRe
-00010090: 6e6f 755d 2868 7474 7073 3a2f 2f67 6974  nou](https://git
-000100a0: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
-000100b0: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
-000100c0: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
-000100d0: 2b69 6e76 6f6c 7665 7325 3341 6d61 7274  +involves%3Amart
-000100e0: 696e 5265 6e6f 752b 7570 6461 7465 6425  inRenou+updated%
-000100f0: 3341 3230 3231 2d30 332d 3134 2e2e 3230  3A2021-03-14..20
-00010100: 3231 2d30 382d 3136 2674 7970 653d 4973  21-08-16&type=Is
-00010110: 7375 6573 2920 7c20 5b40 6d61 7474 6970  sues) | [@mattip
-00010120: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00010130: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
-00010140: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
-00010150: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
-00010160: 766f 6c76 6573 2533 416d 6174 7469 702b  volves%3Amattip+
-00010170: 7570 6461 7465 6425 3341 3230 3231 2d30  updated%3A2021-0
-00010180: 332d 3134 2e2e 3230 3231 2d30 382d 3136  3-14..2021-08-16
-00010190: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
-000101a0: 5b40 6d69 6e72 6b5d 2868 7474 7073 3a2f  [@minrk](https:/
-000101b0: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
-000101c0: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
-000101d0: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
-000101e0: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
-000101f0: 6d69 6e72 6b2b 7570 6461 7465 6425 3341  minrk+updated%3A
-00010200: 3230 3231 2d30 332d 3134 2e2e 3230 3231  2021-03-14..2021
-00010210: 2d30 382d 3136 2674 7970 653d 4973 7375  -08-16&type=Issu
-00010220: 6573 2920 7c20 5b40 4d53 6561 6c5d 2868  es) | [@MSeal](h
-00010230: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00010240: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
-00010250: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
-00010260: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
-00010270: 7665 7325 3341 4d53 6561 6c2b 7570 6461  ves%3AMSeal+upda
-00010280: 7465 6425 3341 3230 3231 2d30 332d 3134  ted%3A2021-03-14
-00010290: 2e2e 3230 3231 2d30 382d 3136 2674 7970  ..2021-08-16&typ
-000102a0: 653d 4973 7375 6573 2920 7c20 5b40 5379  e=Issues) | [@Sy
-000102b0: 6c76 6169 6e43 6f72 6c61 795d 2868 7474  lvainCorlay](htt
-000102c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000102d0: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
-000102e0: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
-000102f0: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
-00010300: 7325 3341 5379 6c76 6169 6e43 6f72 6c61  s%3ASylvainCorla
-00010310: 792b 7570 6461 7465 6425 3341 3230 3231  y+updated%3A2021
-00010320: 2d30 332d 3134 2e2e 3230 3231 2d30 382d  -03-14..2021-08-
-00010330: 3136 2674 7970 653d 4973 7375 6573 2920  16&type=Issues) 
-00010340: 7c20 5b40 7461 6b6c 7579 7665 725d 2868  | [@takluyver](h
-00010350: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00010360: 6d2f 7365 6172 6368 3f71 3d72 6570 6f25  m/search?q=repo%
-00010370: 3341 6a75 7079 7465 7225 3246 6a75 7079  3Ajupyter%2Fjupy
-00010380: 7465 725f 636c 6965 6e74 2b69 6e76 6f6c  ter_client+invol
-00010390: 7665 7325 3341 7461 6b6c 7579 7665 722b  ves%3Atakluyver+
-000103a0: 7570 6461 7465 6425 3341 3230 3231 2d30  updated%3A2021-0
-000103b0: 332d 3134 2e2e 3230 3231 2d30 382d 3136  3-14..2021-08-16
-000103c0: 2674 7970 653d 4973 7375 6573 2920 7c20  &type=Issues) | 
-000103d0: 5b40 7669 6461 7274 665d 2868 7474 7073  [@vidartf](https
-000103e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
-000103f0: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
-00010400: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
-00010410: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
-00010420: 3341 7669 6461 7274 662b 7570 6461 7465  3Avidartf+update
-00010430: 6425 3341 3230 3231 2d30 332d 3134 2e2e  d%3A2021-03-14..
-00010440: 3230 3231 2d30 382d 3136 2674 7970 653d  2021-08-16&type=
-00010450: 4973 7375 6573 2920 7c20 5b40 7969 747a  Issues) | [@yitz
-00010460: 6368 616b 5d28 6874 7470 733a 2f2f 6769  chak](https://gi
-00010470: 7468 7562 2e63 6f6d 2f73 6561 7263 683f  thub.com/search?
-00010480: 713d 7265 706f 2533 416a 7570 7974 6572  q=repo%3Ajupyter
-00010490: 2532 466a 7570 7974 6572 5f63 6c69 656e  %2Fjupyter_clien
-000104a0: 742b 696e 766f 6c76 6573 2533 4179 6974  t+involves%3Ayit
-000104b0: 7a63 6861 6b2b 7570 6461 7465 6425 3341  zchak+updated%3A
-000104c0: 3230 3231 2d30 332d 3134 2e2e 3230 3231  2021-03-14..2021
-000104d0: 2d30 382d 3136 2674 7970 653d 4973 7375  -08-16&type=Issu
-000104e0: 6573 290a 0a23 2320 362e 322e 300a 0a2d  es)..## 6.2.0..-
-000104f0: 2059 616e 6b65 6420 2850 7950 4929 2061   Yanked (PyPI) a
-00010500: 6e64 206d 6172 6b65 6420 6173 2062 726f  nd marked as bro
-00010510: 6b65 6e20 2863 6f6e 6461 290a 0a23 2320  ken (conda)..## 
-00010520: 362e 312e 3133 0a0a 2d20 5961 6e6b 6564  6.1.13..- Yanked
-00010530: 2028 5079 5049 2920 616e 6420 6d61 726b   (PyPI) and mark
-00010540: 6564 2061 7320 6272 6f6b 656e 2028 636f  ed as broken (co
-00010550: 6e64 6129 0a0a 2323 2036 2e31 2e31 320a  nda)..## 6.1.12.
-00010560: 0a2d 2053 6875 7464 6f77 6e20 7265 7175  .- Shutdown requ
-00010570: 6573 7420 7365 7175 656e 6365 2068 6173  est sequence has
-00010580: 2062 6565 6e20 6d6f 6469 6669 6564 2074   been modified t
-00010590: 6f20 6265 206d 6f72 6520 6772 6163 6566  o be more gracef
-000105a0: 756c 2c20 6974 0a20 206e 6f77 2069 7320  ul, it.  now is 
-000105b0: 7072 6563 6564 6564 2062 7920 696e 7465  preceded by inte
-000105c0: 7272 7570 742c 2061 6e64 2077 696c 6c20  rrupt, and will 
-000105d0: 616c 736f 2073 656e 6420 6120 6053 4947  also send a `SIG
-000105e0: 5445 524d 6020 6265 666f 7265 0a20 2066  TERM` before.  f
-000105f0: 6f72 6369 626c 7920 6b69 6c6c 696e 6720  orcibly killing 
-00010600: 7468 6520 6b65 726e 656c 2e20 5b23 3632  the kernel. [#62
-00010610: 305d 2868 7474 7073 3a2f 2f67 6974 6875  0](https://githu
-00010620: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-00010630: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-00010640: 6c2f 3632 3029 0a2d 2052 656d 6f76 616c  l/620).- Removal
-00010650: 206f 6620 6069 7079 7468 6f6e 5f67 656e   of `ipython_gen
-00010660: 7574 696c 7360 2061 7320 6120 6465 7065  utils` as a depe
-00010670: 6e64 656e 6379 2e20 4974 2077 6173 2069  ndency. It was i
-00010680: 6d70 6c69 6369 740a 2020 6265 666f 7265  mplicit.  before
-00010690: 3b20 6275 7420 7265 7175 6972 6564 2062  ; but required b
-000106a0: 7920 6174 206c 6561 7374 2074 7261 6974  y at least trait
-000106b0: 6c65 7473 2074 6875 7320 6176 6f69 6469  lets thus avoidi
-000106c0: 6e67 2069 7373 7565 732e 2057 650a 2020  ng issues. We.  
-000106d0: 6172 6520 776f 726b 696e 6720 6f6e 2063  are working on c
-000106e0: 6f6d 706c 6574 656c 7920 7265 6d6f 7669  ompletely removi
-000106f0: 6e67 2069 7420 6672 6f6d 2061 6c6c 206a  ng it from all j
-00010700: 7570 7974 6572 2064 6570 656e 6465 6e63  upyter dependenc
-00010710: 6965 733b 0a20 2061 7320 6974 206d 6967  ies;.  as it mig
-00010720: 6874 206c 6561 6420 746f 2069 7373 7565  ht lead to issue
-00010730: 7320 7061 636b 6167 696e 6720 666f 7220  s packaging for 
-00010740: 5079 7468 6f6e 2033 2e31 302c 2061 6e64  Python 3.10, and
-00010750: 2077 6173 206d 6f73 746c 790a 2020 7573   was mostly.  us
-00010760: 6564 2066 6f72 2063 6f6d 7061 7469 6269  ed for compatibi
-00010770: 6c69 7479 2077 6974 6820 7079 7468 6f6e  lity with python
-00010780: 2032 2e20 285b 2336 3230 5d28 6874 7470   2. ([#620](http
-00010790: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000107a0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-000107b0: 6c69 656e 742f 7075 6c6c 2f36 3230 292c  lient/pull/620),
-000107c0: 205b 2336 3035 5d28 6874 7470 733a 2f2f   [#605](https://
-000107d0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-000107e0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-000107f0: 742f 7075 6c6c 2f36 3035 2929 0a2d 2041  t/pull/605)).- A
-00010800: 6464 7265 7373 2061 2072 6163 6520 636f  ddress a race co
-00010810: 6e64 6974 696f 6e20 6265 7477 6565 6e20  ndition between 
-00010820: 6073 6875 7464 6f77 6e5f 6b65 726e 656c  `shutdown_kernel
-00010830: 6020 616e 6420 7265 7374 6172 7465 722e  ` and restarter.
-00010840: 0a20 2028 5b23 3630 375d 2868 7474 7073  .  ([#607](https
-00010850: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00010860: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-00010870: 6965 6e74 2f70 756c 6c2f 3630 3729 2e29  ient/pull/607).)
-00010880: 0a0a 5365 6520 7468 6520 5b66 756c 6c20  ..See the [full 
-00010890: 6c69 7374 206f 660a 7075 6c6c 2d72 6571  list of.pull-req
-000108a0: 7565 7374 735d 2868 7474 7073 3a2f 2f67  uests](https://g
-000108b0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
-000108c0: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
-000108d0: 2f6d 696c 6573 746f 6e65 2f32 373f 636c  /milestone/27?cl
-000108e0: 6f73 6564 3d31 290a 0a23 2320 362e 312e  osed=1)..## 6.1.
-000108f0: 3131 0a0a 2d20 4d6f 7665 206a 6564 6920  11..- Move jedi 
-00010900: 7069 6e6e 696e 6720 746f 2074 6573 7420  pinning to test 
-00010910: 7265 7175 6972 656d 656e 7473 205b 2335  requirements [#5
-00010920: 3939 5d28 6874 7470 733a 2f2f 6769 7468  99](https://gith
-00010930: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00010940: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-00010950: 6c6c 2f35 3939 290a 0a23 2320 362e 312e  ll/599)..## 6.1.
-00010960: 3130 0a0a 2d20 4164 6420 6368 616e 6765  10..- Add change
-00010970: 2070 6172 616d 6574 6572 206e 6565 6465   parameter neede
-00010980: 6420 666f 7220 6f62 7365 7276 6572 206d  d for observer m
-00010990: 6574 686f 6420 6f66 0a20 206b 6572 6e65  ethod of.  kerne
-000109a0: 6c5f 7370 6563 5f6d 616e 6167 6572 2074  l_spec_manager t
-000109b0: 7261 6974 205b 2335 3938 5d28 6874 7470  rait [#598](http
-000109c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000109d0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-000109e0: 6c69 656e 742f 7075 6c6c 2f35 3938 290a  lient/pull/598).
-000109f0: 0a23 2320 362e 312e 390a 0a2d 2050 696e  .## 6.1.9..- Pin
-00010a00: 206a 6564 695c 3c3d 302e 3137 2e32 205b   jedi\<=0.17.2 [
-00010a10: 2335 3936 5d28 6874 7470 733a 2f2f 6769  #596](https://gi
-00010a20: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-00010a30: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-00010a40: 7075 6c6c 2f35 3936 290a 0a23 2320 362e  pull/596)..## 6.
-00010a50: 312e 380a 0a2d 2044 6f63 2075 7064 6174  1.8..- Doc updat
-00010a60: 6573 2028 5b23 3536 335d 2868 7474 7073  es ([#563](https
-00010a70: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00010a80: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-00010a90: 6965 6e74 2f70 756c 6c2f 3536 3329 2c0a  ient/pull/563),.
-00010aa0: 2020 5b23 3536 345d 2868 7474 7073 3a2f    [#564](https:/
-00010ab0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-00010ac0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-00010ad0: 6e74 2f70 756c 6c2f 3536 3429 2c20 5b23  nt/pull/564), [#
-00010ae0: 3538 375d 2868 7474 7073 3a2f 2f67 6974  587](https://git
-00010af0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-00010b00: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-00010b10: 756c 6c2f 3538 3729 290a 2d20 4669 7820  ull/587)).- Fix 
-00010b20: 7061 7468 2074 6f20 7468 6520 636f 6e6e  path to the conn
-00010b30: 6563 7469 6f6e 2066 696c 6520 5b23 3536  ection file [#56
-00010b40: 385d 2868 7474 7073 3a2f 2f67 6974 6875  8](https://githu
-00010b50: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-00010b60: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-00010b70: 6c2f 3536 3829 0a2d 2043 6f64 6520 636c  l/568).- Code cl
-00010b80: 6561 6e75 7020 285b 2335 3734 5d28 6874  eanup ([#574](ht
-00010b90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00010ba0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00010bb0: 5f63 6c69 656e 742f 7075 6c6c 2f35 3734  _client/pull/574
-00010bc0: 292c 0a20 205b 2335 3739 5d28 6874 7470  ),.  [#579](http
-00010bd0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00010be0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00010bf0: 6c69 656e 742f 7075 6c6c 2f35 3739 2929  lient/pull/579))
-00010c00: 0a2d 2053 696c 656e 6365 206b 696c 6c5f  .- Silence kill_
-00010c10: 6b65 726e 656c 2077 6865 6e20 6e6f 2070  kernel when no p
-00010c20: 726f 6365 7373 2069 7320 7072 6573 656e  rocess is presen
-00010c30: 740a 2020 5b23 3537 365d 2868 7474 7073  t.  [#576](https
-00010c40: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00010c50: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-00010c60: 6965 6e74 2f70 756c 6c2f 3537 3629 0a2d  ient/pull/576).-
-00010c70: 2052 656d 6f76 6520 6578 7472 615f 656e   Remove extra_en
-00010c80: 7620 616e 6420 636f 7272 6573 706f 6e64  v and correspond
-00010c90: 696e 6720 7465 7374 205b 2335 3831 5d28  ing test [#581](
-00010ca0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00010cb0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-00010cc0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f35  er_client/pull/5
-00010cd0: 3831 290a 2d20 4164 6420 646f 6375 6d65  81).- Add docume
-00010ce0: 6e74 6174 696f 6e20 6465 7065 6e64 656e  ntation dependen
-00010cf0: 6369 6573 2074 6f20 7365 7475 702e 7079  cies to setup.py
-00010d00: 205b 2335 3832 5d28 6874 7470 733a 2f2f   [#582](https://
-00010d10: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00010d20: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00010d30: 742f 7075 6c6c 2f35 3832 290a 2d20 4669  t/pull/582).- Fi
-00010d40: 7820 666f 7220 5769 6e64 6f77 7320 6c6f  x for Windows lo
-00010d50: 6361 6c68 6f73 7420 4950 2061 6464 7265  calhost IP addre
-00010d60: 7373 6573 205b 2335 3834 5d28 6874 7470  sses [#584](http
-00010d70: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00010d80: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00010d90: 6c69 656e 742f 7075 6c6c 2f35 3834 290a  lient/pull/584).
-00010da0: 2d20 4472 6f70 2054 7261 7669 7320 4349  - Drop Travis CI
-00010db0: 2c20 6164 6420 4769 7448 7562 2041 6374  , add GitHub Act
-00010dc0: 696f 6e73 205b 2335 3836 5d28 6874 7470  ions [#586](http
-00010dd0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00010de0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00010df0: 6c69 656e 742f 7075 6c6c 2f35 3836 290a  lient/pull/586).
-00010e00: 2d20 4164 6170 7420 4b65 726e 656c 4d61  - Adapt KernelMa
-00010e10: 6e61 6765 722e 5c5f 6b65 726e 656c 5f73  nager.\_kernel_s
-00010e20: 7065 635f 6d61 6e61 6765 725f 6368 616e  pec_manager_chan
-00010e30: 6765 6420 746f 206f 6273 6572 7665 0a20  ged to observe. 
-00010e40: 205b 2335 3838 5d28 6874 7470 733a 2f2f   [#588](https://
-00010e50: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00010e60: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00010e70: 742f 7075 6c6c 2f35 3838 290a 2d20 416c  t/pull/588).- Al
-00010e80: 6c6f 7720 7573 6520 7e2f 2069 6e20 7468  low use ~/ in th
-00010e90: 6520 6b65 726e 656c 2773 2063 6f6d 6d61  e kernel's comma
-00010ea0: 6e64 206f 7220 6974 7320 6172 6775 6d65  nd or its argume
-00010eb0: 6e74 730a 2020 5b23 3538 395d 2868 7474  nts.  [#589](htt
-00010ec0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00010ed0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00010ee0: 636c 6965 6e74 2f70 756c 6c2f 3538 3929  client/pull/589)
-00010ef0: 0a2d 2043 6861 6e67 6520 7761 6974 5f66  .- Change wait_f
-00010f00: 6f72 5f72 6561 6479 206c 6f67 6963 205b  or_ready logic [
-00010f10: 2335 3932 5d28 6874 7470 733a 2f2f 6769  #592](https://gi
-00010f20: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-00010f30: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-00010f40: 7075 6c6c 2f35 3932 290a 2d20 4669 7820  pull/592).- Fix 
-00010f50: 7465 7374 5f73 6573 7369 6f6e 2077 6974  test_session wit
-00010f60: 6820 6d73 6770 6163 6b20 7631 205b 2335  h msgpack v1 [#5
-00010f70: 3934 5d28 6874 7470 733a 2f2f 6769 7468  94](https://gith
-00010f80: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00010f90: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-00010fa0: 6c6c 2f35 3934 290a 0a23 2320 362e 312e  ll/594)..## 6.1.
-00010fb0: 360a 0a2d 2052 656d 6f76 6564 2077 6172  6..- Removed war
-00010fc0: 6e69 6e67 7320 696e 206d 6f72 6520 6361  nings in more ca
-00010fd0: 7365 7320 666f 7220 4b65 726e 656c 4d61  ses for KernelMa
-00010fe0: 6e61 6765 7273 2074 6861 7420 7573 6520  nagers that use 
-00010ff0: 6e65 770a 2020 636c 6561 6e75 7020 6d65  new.  cleanup me
-00011000: 7468 6f64 205b 2335 3630 5d28 6874 7470  thod [#560](http
-00011010: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00011020: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00011030: 6c69 656e 742f 7075 6c6c 2f35 3630 290a  lient/pull/560).
-00011040: 2d20 536f 6d65 2069 6d70 726f 7665 6420  - Some improved 
-00011050: 7465 7374 7320 7769 7468 2061 2063 6f6e  tests with a con
-00011060: 7665 7273 696f 6e20 746f 2070 7974 6573  version to pytes
-00011070: 7420 7061 7474 6572 6e0a 2020 5b23 3536  t pattern.  [#56
-00011080: 315d 2868 7474 7073 3a2f 2f67 6974 6875  1](https://githu
-00011090: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-000110a0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-000110b0: 6c2f 3536 3129 0a0a 2323 2036 2e31 2e35  l/561)..## 6.1.5
-000110c0: 0a0a 2d20 4772 6163 6566 756c 6c79 2043  ..- Gracefully C
-000110d0: 6c6f 7365 205a 4d51 2043 6f6e 7465 7874  lose ZMQ Context
-000110e0: 2075 706f 6e20 6b65 726e 656c 2073 6875   upon kernel shu
-000110f0: 7464 6f77 6e20 746f 2066 6978 206d 656d  tdown to fix mem
-00011100: 6f72 7920 6c65 616b 0a20 205b 2335 3438  ory leak.  [#548
-00011110: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00011120: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00011130: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00011140: 2f35 3438 290a 2d20 4669 7820 666f 7220  /548).- Fix for 
-00011150: 6368 6169 6e65 6420 6578 6365 7074 696f  chained exceptio
-00011160: 6e73 2074 6f20 7072 6573 6572 7665 2073  ns to preserve s
-00011170: 7461 636b 730a 2020 285b 2335 3532 5d28  tacks.  ([#552](
-00011180: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00011190: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-000111a0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f35  er_client/pull/5
-000111b0: 3532 292c 205b 2335 3534 5d28 6874 7470  52), [#554](http
-000111c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000111d0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-000111e0: 6c69 656e 742f 7075 6c6c 2f35 3534 2929  lient/pull/554))
-000111f0: 0a2d 2046 6978 2073 7461 7274 5f6b 6572  .- Fix start_ker
-00011200: 6e65 6c20 6572 726f 7220 7768 656e 2070  nel error when p
-00011210: 6173 7369 6e67 206b 6572 6e65 6c5f 6964  assing kernel_id
-00011220: 0a20 205b 2335 3437 5d28 6874 7470 733a  .  [#547](https:
-00011230: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-00011240: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-00011250: 656e 742f 7075 6c6c 2f35 3437 290a 2d20  ent/pull/547).- 
-00011260: 5570 6461 7465 2074 6f20 7265 6c65 6173  Update to releas
-00011270: 696e 6720 646f 6373 205b 2335 3433 5d28  ing docs [#543](
-00011280: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00011290: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-000112a0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f35  er_client/pull/5
-000112b0: 3433 290a 0a23 2320 362e 312e 340a 0a28  43)..## 6.1.4..(
-000112c0: 4465 6c65 7465 6420 7265 6c65 6173 6520  Deleted release 
-000112d0: 7769 7468 2069 6e63 6f72 7265 6374 206c  with incorrect l
-000112e0: 6f63 616c 2066 696c 6573 290a 0a23 2320  ocal files)..## 
-000112f0: 362e 312e 330a 0a2d 2041 6464 2041 7379  6.1.3..- Add Asy
-00011300: 6e63 4b65 726e 656c 436c 6965 6e74 2063  ncKernelClient c
-00011310: 6c69 656e 745f 636c 6173 7320 746f 2041  lient_class to A
-00011320: 7379 6e63 4b65 726e 656c 4d61 6e61 6765  syncKernelManage
-00011330: 720a 2020 5b23 3534 325d 2868 7474 7073  r.  [#542](https
-00011340: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00011350: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-00011360: 6965 6e74 2f70 756c 6c2f 3534 3229 0a2d  ient/pull/542).-
-00011370: 2044 6f63 2066 6978 2066 6f72 2078 6575   Doc fix for xeu
-00011380: 7320 6879 7065 726c 696e 6b73 205b 2335  s hyperlinks [#5
-00011390: 3430 5d28 6874 7470 733a 2f2f 6769 7468  40](https://gith
-000113a0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-000113b0: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-000113c0: 6c6c 2f35 3430 290a 2d20 446f 6320 7479  ll/540).- Doc ty
-000113d0: 706f 2066 6978 205b 2335 3339 5d28 6874  po fix [#539](ht
-000113e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000113f0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00011400: 5f63 6c69 656e 742f 7075 6c6c 2f35 3339  _client/pull/539
-00011410: 290a 0a23 2320 362e 312e 320a 0a2d 2046  )..## 6.1.2..- F
-00011420: 6978 6564 2061 2062 7567 2063 6175 7369  ixed a bug causi
-00011430: 6e67 2063 6c69 656e 7473 2074 6f20 736f  ng clients to so
-00011440: 6d65 7469 6d65 7320 6861 6e67 2061 6674  metimes hang aft
-00011450: 6572 2061 2073 746f 7020 6361 6c6c 2077  er a stop call w
-00011460: 6173 0a20 206d 6164 6520 5b23 3533 365d  as.  made [#536]
-00011470: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00011480: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-00011490: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-000114a0: 3533 3629 0a0a 2323 2036 2e31 2e31 0a0a  536)..## 6.1.1..
-000114b0: 2d20 5375 6270 726f 6365 7373 206b 696c  - Subprocess kil
-000114c0: 6c20 6163 7469 6f6e 2066 6978 2066 6f72  l action fix for
-000114d0: 2061 7379 6e63 2065 7865 6375 7469 6f6e   async execution
-000114e0: 0a20 205b 2335 3335 5d28 6874 7470 733a  .  [#535](https:
-000114f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-00011500: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-00011510: 656e 742f 7075 6c6c 2f35 3335 290a 2d20  ent/pull/535).- 
-00011520: 446f 6320 6669 7820 666f 7220 7865 7573  Doc fix for xeus
-00011530: 206b 6572 6e65 6c20 6c69 7374 205b 2335   kernel list [#5
-00011540: 3334 5d28 6874 7470 733a 2f2f 6769 7468  34](https://gith
-00011550: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00011560: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-00011570: 6c6c 2f35 3334 290a 0a23 2320 362e 312e  ll/534)..## 6.1.
-00011580: 300a 0a54 6869 7320 7265 6c65 6173 6520  0..This release 
-00011590: 696e 636c 7564 6573 2073 7570 706f 7274  includes support
-000115a0: 2066 6f72 2061 7379 6e63 696f 2070 6174   for asyncio pat
-000115b0: 7465 726e 7321 2044 6f77 6e73 7472 6561  terns! Downstrea
-000115c0: 6d20 746f 6f6c 730a 7368 6f75 6c64 2073  m tools.should s
-000115d0: 6f6f 6e20 6861 7665 2072 656c 6561 7365  oon have release
-000115e0: 7320 746f 2061 6464 6974 696f 6e61 6c6c  s to additionall
-000115f0: 7920 7375 7070 6f72 7420 6173 796e 6320  y support async 
-00011600: 7061 7474 6572 6e73 2e0a 0a2d 2041 7379  patterns...- Asy
-00011610: 6e63 4b65 726e 656c 4d61 6e61 6765 7220  ncKernelManager 
-00011620: 616e 6420 4173 796e 634d 756c 7469 4b65  and AsyncMultiKe
-00011630: 726e 656c 4d61 6e61 6765 7220 6172 6520  rnelManager are 
-00011640: 6e6f 7720 6176 6169 6c61 626c 6520 666f  now available fo
-00011650: 720a 2020 6173 796e 6320 6a75 7079 7465  r.  async jupyte
-00011660: 725f 636c 6965 6e74 2069 6e74 6572 6163  r_client interac
-00011670: 7469 6f6e 7320 285b 2335 3238 5d28 6874  tions ([#528](ht
-00011680: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00011690: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-000116a0: 5f63 6c69 656e 742f 7075 6c6c 2f35 3238  _client/pull/528
-000116b0: 292c 205b 2335 3239 5d28 6874 7470 733a  ), [#529](https:
-000116c0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-000116d0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-000116e0: 656e 742f 7075 6c6c 2f35 3239 2929 0a2d  ent/pull/529)).-
-000116f0: 2052 656d 6f76 6564 2075 6e75 7365 6420   Removed unused 
-00011700: 7370 6869 6e78 2064 6570 656e 6465 6e63  sphinx dependenc
-00011710: 7920 285b 2335 3138 5d28 6874 7470 733a  y ([#518](https:
-00011720: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
-00011730: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
-00011740: 656e 742f 7075 6c6c 2f35 3138 292c 205b  ent/pull/518), [
-00011750: 2335 3138 5d28 6874 7470 733a 2f2f 6769  #518](https://gi
-00011760: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-00011770: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-00011780: 7075 6c6c 2f35 3138 2929 2e0a 2d20 4164  pull/518))..- Ad
-00011790: 6465 6420 696e 7374 616c 6c20 696e 7374  ded install inst
-000117a0: 7275 6374 696f 6e73 2066 6f72 2070 6970  ructions for pip
-000117b0: 2074 6f20 646f 6375 6d65 6e74 6174 696f   to documentatio
-000117c0: 6e0a 2020 5b23 3532 315d 2868 7474 7073  n.  [#521](https
-000117d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-000117e0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-000117f0: 6965 6e74 2f70 756c 6c2f 3532 3129 0a2d  ient/pull/521).-
-00011800: 2049 6d70 726f 7665 6420 646f 6373 2061   Improved docs a
-00011810: 726f 756e 6420 7665 7273 696f 6e20 7072  round version pr
-00011820: 6f74 6f63 6f6c 2061 6e64 206d 6573 7361  otocol and messa
-00011830: 6769 6e67 0a20 2028 5b23 3532 325d 2868  ging.  ([#522](h
-00011840: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00011850: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00011860: 725f 636c 6965 6e74 2f70 756c 6c2f 3532  r_client/pull/52
-00011870: 3229 2c20 5b23 3532 365d 2868 7474 7073  2), [#526](https
-00011880: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00011890: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-000118a0: 6965 6e74 2f70 756c 6c2f 3532 3629 290a  ient/pull/526)).
-000118b0: 0a23 2320 362e 302e 300a 0a54 6865 2067  .## 6.0.0..The g
-000118c0: 6974 2068 6973 746f 7279 2068 6164 2074  it history had t
-000118d0: 6f20 6265 2072 6577 6f72 6b65 6420 6865  o be reworked he
-000118e0: 6176 696c 7920 696e 206d 6572 6769 6e67  avily in merging
-000118f0: 2035 2e78 2061 6e64 206d 6173 7465 722c   5.x and master,
-00011900: 2073 6f0a 6120 6c69 6e6b 2074 6f20 616c   so.a link to al
-00011910: 6c20 7468 6520 6368 616e 6765 7320 6174  l the changes at
-00011920: 206f 6e63 6520 696e 2067 6974 6875 6220   once in github 
-00011930: 6861 6420 6265 656e 206c 6566 7420 6f75  had been left ou
-00011940: 7420 6173 2069 7427 730a 6a75 7374 2063  t as it's.just c
-00011950: 6f6e 6675 7369 6e67 2e0a 0a41 6e20 6578  onfusing...An ex
-00011960: 6369 7469 6e67 2063 6861 6e67 6520 696e  citing change in
-00011970: 2074 6869 7320 7265 6c65 6173 6520 6973   this release is
-00011980: 2073 6f6d 6520 6173 796e 6320 7375 7070   some async supp
-00011990: 6f72 7420 2868 7567 6520 7468 616e 6b73  ort (huge thanks
-000119a0: 2074 6f0a 4064 6176 6964 6272 6f63 6861   to.@davidbrocha
-000119b0: 7274 2066 6f72 2064 6f69 6e67 206d 6f73  rt for doing mos
-000119c0: 7420 6f66 2074 6865 2077 6f72 6b29 2120  t of the work)! 
-000119d0: 5365 6520 6c69 6e6b 6564 2050 5220 6265  See linked PR be
-000119e0: 6c6f 7720 666f 720a 6d6f 7265 2064 6574  low for.more det
-000119f0: 6169 6c73 2c20 7765 2772 6520 776f 726b  ails, we're work
-00011a00: 696e 6720 6f6e 2069 6e74 6567 7261 7469  ing on integrati
-00011a10: 6e67 2074 6869 7320 696e 746f 206e 6263  ng this into nbc
-00011a20: 6c69 656e 7420 6173 2077 656c 6c0a 696e  lient as well.in
-00011a30: 2074 6865 206e 6561 7220 6675 7475 7265   the near future
-00011a40: 2e0a 0a4e 6577 2046 6561 7475 7265 733a  ...New Features:
-00011a50: 0a0a 2d20 4164 6465 6420 6173 796e 6320  ..- Added async 
-00011a60: 4150 4920 5b23 3530 365d 2868 7474 7073  API [#506](https
-00011a70: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00011a80: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-00011a90: 6965 6e74 2f70 756c 6c2f 3530 3629 0a0a  ient/pull/506)..
-00011aa0: 4368 616e 6765 733a 0a0a 2d20 5079 7468  Changes:..- Pyth
-00011ab0: 6f6e 2033 2e38 2074 6573 7469 6e67 2061  on 3.8 testing a
-00011ac0: 6e64 2073 7570 706f 7274 2061 6464 6564  nd support added
-00011ad0: 205b 2335 3039 5d28 6874 7470 733a 2f2f   [#509](https://
-00011ae0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00011af0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00011b00: 742f 7075 6c6c 2f35 3039 290a 2d20 5365  t/pull/509).- Se
-00011b10: 7373 696f 6e2e 6d73 675f 6964 206f 7074  ssion.msg_id opt
-00011b20: 696d 697a 6174 696f 6e20 5b23 3439 335d  imization [#493]
-00011b30: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00011b40: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-00011b50: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-00011b60: 3439 3329 0a2d 204f 6e6c 7920 6361 6368  493).- Only cach
-00011b70: 6520 706f 7274 7320 6966 2074 6865 2063  e ports if the c
-00011b80: 6163 6865 5f70 6f72 7473 2066 6c61 6720  ache_ports flag 
-00011b90: 6973 2073 6574 2074 6f20 5472 7565 0a20  is set to True. 
-00011ba0: 205b 2334 3932 5d28 6874 7470 733a 2f2f   [#492](https://
-00011bb0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00011bc0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00011bd0: 742f 7075 6c6c 2f34 3932 290a 2d20 5265  t/pull/492).- Re
-00011be0: 6d6f 7665 6420 6469 7265 6374 2064 6570  moved direct dep
-00011bf0: 656e 6465 6e63 7920 6f6e 2070 7977 696e  endency on pywin
-00011c00: 3332 2061 7320 7468 6973 2069 7320 6e6f  32 as this is no
-00011c10: 7720 696e 206a 7570 7974 6572 2063 6f72  w in jupyter cor
-00011c20: 650a 2020 5b23 3438 395d 2868 7474 7073  e.  [#489](https
-00011c30: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00011c40: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-00011c50: 6965 6e74 2f70 756c 6c2f 3438 3929 0a0a  ient/pull/489)..
-00011c60: 4669 7865 733a 0a0a 2d20 5072 6576 656e  Fixes:..- Preven
-00011c70: 7420 7477 6f20 6b65 726e 656c 7320 746f  t two kernels to
-00011c80: 2068 6176 6520 7468 6520 7361 6d65 2070   have the same p
-00011c90: 6f72 7473 205b 2334 3930 5d28 6874 7470  orts [#490](http
-00011ca0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00011cb0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00011cc0: 6c69 656e 742f 7075 6c6c 2f34 3930 290a  lient/pull/490).
-00011cd0: 0a44 6f63 733a 0a0a 2d20 446f 6375 6d65  .Docs:..- Docume
-00011ce0: 6e74 2074 6865 2068 616e 646c 696e 6720  nt the handling 
-00011cf0: 6f66 2065 7272 6f72 2069 6e20 646f 5f65  of error in do_e
-00011d00: 7865 6375 7465 0a20 205b 2335 3030 5d28  xecute.  [#500](
+0000ed20: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+0000ed30: 7974 6572 5f63 6c69 656e 742f 6772 6170  yter_client/grap
+0000ed40: 6873 2f63 6f6e 7472 6962 7574 6f72 733f  hs/contributors?
+0000ed50: 6672 6f6d 3d32 3032 312d 3038 2d31 3926  from=2021-08-19&
+0000ed60: 746f 3d32 3032 312d 3038 2d32 3026 7479  to=2021-08-20&ty
+0000ed70: 7065 3d63 2929 0a0a 5b40 6b65 7669 6e2d  pe=c))..[@kevin-
+0000ed80: 6261 7465 735d 2868 7474 7073 3a2f 2f67  bates](https://g
+0000ed90: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+0000eda0: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+0000edb0: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+0000edc0: 6e74 2b69 6e76 6f6c 7665 7325 3341 6b65  nt+involves%3Ake
+0000edd0: 7669 6e2d 6261 7465 732b 7570 6461 7465  vin-bates+update
+0000ede0: 6425 3341 3230 3231 2d30 382d 3139 2e2e  d%3A2021-08-19..
+0000edf0: 3230 3231 2d30 382d 3230 2674 7970 653d  2021-08-20&type=
+0000ee00: 4973 7375 6573 290a 0a23 2320 372e 302e  Issues)..## 7.0.
+0000ee10: 300a 0a28 5b46 756c 6c20 4368 616e 6765  0..([Full Change
+0000ee20: 6c6f 675d 2868 7474 7073 3a2f 2f67 6974  log](https://git
+0000ee30: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+0000ee40: 6a75 7079 7465 725f 636c 6965 6e74 2f63  jupyter_client/c
+0000ee50: 6f6d 7061 7265 2f32 3661 3136 6330 6339  ompare/26a16c0c9
+0000ee60: 3165 3234 3566 3734 3033 6161 3237 6138  1e245f7403aa27a8
+0000ee70: 3132 6665 6535 6539 3035 6432 3936 342e  12fee5e905d2964.
+0000ee80: 2e2e 3331 3735 3062 6338 3762 6166 3838  ..31750bc87baf88
+0000ee90: 3337 3762 6363 3639 3637 6532 3237 6236  377bcc6967e227b6
+0000eea0: 3530 6233 3866 6138 3732 2929 0a0a 2323  50b38fa872))..##
+0000eeb0: 2320 5375 6d6d 6172 790a 0a54 6865 2037  # Summary..The 7
+0000eec0: 2e30 2072 656c 6561 7365 2062 7269 6e67  .0 release bring
+0000eed0: 7320 6120 6d61 6a6f 7220 6665 6174 7572  s a major featur
+0000eee0: 6520 696e 205b 4b65 726e 656c 2050 726f  e in [Kernel Pro
+0000eef0: 7669 7369 6f6e 6572 735d 2868 7474 7073  visioners](https
+0000ef00: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+0000ef10: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+0000ef20: 6965 6e74 2f62 6c6f 622f 6d61 7374 6572  ient/blob/master
+0000ef30: 2f64 6f63 732f 7072 6f76 6973 696f 6e69  /docs/provisioni
+0000ef40: 6e67 2e72 7374 292c 2077 6869 6368 2065  ng.rst), which e
+0000ef50: 6e61 626c 6520 7468 6520 6162 696c 6974  nable the abilit
+0000ef60: 7920 666f 7220 7468 6972 6420 7061 7274  y for third part
+0000ef70: 6965 7320 746f 206d 616e 6167 6520 7468  ies to manage th
+0000ef80: 6520 6c69 6665 6379 636c 6520 6f66 2061  e lifecycle of a
+0000ef90: 206b 6572 6e65 6c27 7320 7275 6e74 696d   kernel's runtim
+0000efa0: 6520 656e 7669 726f 6e6d 656e 742e 0a0a  e environment...
+0000efb0: 4265 696e 6720 6120 6d61 6a6f 7220 7265  Being a major re
+0000efc0: 6c65 6173 652c 2074 6865 7265 2061 7265  lease, there are
+0000efd0: 2073 6f6d 6520 6261 636b 7761 7264 2069   some backward i
+0000efe0: 6e63 6f6d 7061 7469 626c 6520 6368 616e  ncompatible chan
+0000eff0: 6765 732e 2050 6c65 6173 6520 7365 6520  ges. Please see 
+0000f000: 7468 6520 5b6d 6967 7261 7469 6f6e 2067  the [migration g
+0000f010: 7569 6465 5d28 6874 7470 733a 2f2f 6a75  uide](https://ju
+0000f020: 7079 7465 722d 636c 6965 6e74 2e72 6561  pyter-client.rea
+0000f030: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+0000f040: 6174 6573 742f 6d69 6772 6174 696f 6e2e  atest/migration.
+0000f050: 6874 6d6c 2920 666f 7220 6675 7274 6865  html) for furthe
+0000f060: 7220 6465 7461 696c 732e 0a0a 2323 2320  r details...### 
+0000f070: 456e 6861 6e63 656d 656e 7473 206d 6164  Enhancements mad
+0000f080: 650a 0a2d 204b 6572 6e65 6c20 5072 6f76  e..- Kernel Prov
+0000f090: 6973 696f 6e69 6e67 202d 2069 6e69 7469  isioning - initi
+0000f0a0: 616c 2069 6d70 6c65 6d65 6e74 6174 696f  al implementatio
+0000f0b0: 6e20 5b23 3631 325d 2868 7474 7073 3a2f  n [#612](https:/
+0000f0c0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+0000f0d0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+0000f0e0: 6e74 2f70 756c 6c2f 3631 3229 2028 5b40  nt/pull/612) ([@
+0000f0f0: 6b65 7669 6e2d 6261 7465 735d 2868 7474  kevin-bates](htt
+0000f100: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000f110: 6b65 7669 6e2d 6261 7465 7329 290a 0a23  kevin-bates))..#
+0000f120: 2323 2042 7567 7320 6669 7865 640a 0a2d  ## Bugs fixed..-
+0000f130: 2046 6978 2075 7020 736f 6d65 2061 7379   Fix up some asy
+0000f140: 6e63 206d 6574 686f 6420 616c 6961 7365  nc method aliase
+0000f150: 7320 696e 204b 6572 6e65 6c4d 616e 6167  s in KernelManag
+0000f160: 6572 205b 2336 3730 5d28 6874 7470 733a  er [#670](https:
+0000f170: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+0000f180: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+0000f190: 656e 742f 7075 6c6c 2f36 3730 2920 285b  ent/pull/670) ([
+0000f1a0: 406b 6576 696e 2d62 6174 6573 5d28 6874  @kevin-bates](ht
+0000f1b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000f1c0: 2f6b 6576 696e 2d62 6174 6573 2929 0a2d  /kevin-bates)).-
+0000f1d0: 2053 7570 706f 7274 2060 616e 7377 6572   Support `answer
+0000f1e0: 5f79 6573 6020 7768 656e 2072 656d 6f76  _yes` when remov
+0000f1f0: 696e 6720 6b65 726e 656c 2073 7065 6373  ing kernel specs
+0000f200: 205b 2336 3539 5d28 6874 7470 733a 2f2f   [#659](https://
+0000f210: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+0000f220: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+0000f230: 742f 7075 6c6c 2f36 3539 2920 285b 4064  t/pull/659) ([@d
+0000f240: 6176 6964 6272 6f63 6861 7274 5d28 6874  avidbrochart](ht
+0000f250: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000f260: 2f64 6176 6964 6272 6f63 6861 7274 2929  /davidbrochart))
+0000f270: 0a2d 2049 6e63 6c75 6465 2070 726f 6365  .- Include proce
+0000f280: 7373 2049 4420 696e 206d 6573 7361 6765  ss ID in message
+0000f290: 2049 4420 5b23 3635 355d 2868 7474 7073   ID [#655](https
+0000f2a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+0000f2b0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+0000f2c0: 6965 6e74 2f70 756c 6c2f 3635 3529 2028  ient/pull/655) (
+0000f2d0: 5b40 7461 6b6c 7579 7665 725d 2868 7474  [@takluyver](htt
+0000f2e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000f2f0: 7461 6b6c 7579 7665 7229 290a 2d20 4669  takluyver)).- Fi
+0000f300: 7820 7174 636f 6e73 6f6c 6520 6973 7375  x qtconsole issu
+0000f310: 6573 205b 2336 3338 5d28 6874 7470 733a  es [#638](https:
+0000f320: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+0000f330: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+0000f340: 656e 742f 7075 6c6c 2f36 3338 2920 285b  ent/pull/638) ([
+0000f350: 4064 6176 6964 6272 6f63 6861 7274 5d28  @davidbrochart](
+0000f360: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000f370: 6f6d 2f64 6176 6964 6272 6f63 6861 7274  om/davidbrochart
+0000f380: 2929 0a0a 2323 2320 4d61 696e 7465 6e61  ))..### Maintena
+0000f390: 6e63 6520 616e 6420 7570 6b65 6570 2069  nce and upkeep i
+0000f3a0: 6d70 726f 7665 6d65 6e74 730a 0a2d 2041  mprovements..- A
+0000f3b0: 6464 6564 2064 6562 7567 6765 7220 6b65  dded debugger ke
+0000f3c0: 7920 696e 2060 6b65 726e 656c 5f69 6e66  y in `kernel_inf
+0000f3d0: 6f5f 7265 706c 7960 205b 2334 3836 5d28  o_reply` [#486](
+0000f3e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000f3f0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+0000f400: 6572 5f63 6c69 656e 742f 7075 6c6c 2f34  er_client/pull/4
+0000f410: 3836 2920 285b 404a 6f68 616e 4d61 6269  86) ([@JohanMabi
+0000f420: 6c6c 655d 2868 7474 7073 3a2f 2f67 6974  lle](https://git
+0000f430: 6875 622e 636f 6d2f 4a6f 6861 6e4d 6162  hub.com/JohanMab
+0000f440: 696c 6c65 2929 0a2d 2050 7265 7061 7265  ille)).- Prepare
+0000f450: 2066 6f72 2075 7365 2077 6974 6820 4a75   for use with Ju
+0000f460: 7079 7465 7220 5265 6c65 6173 6572 205b  pyter Releaser [
+0000f470: 2336 3736 5d28 6874 7470 733a 2f2f 6769  #676](https://gi
+0000f480: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+0000f490: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+0000f4a0: 7075 6c6c 2f36 3736 2920 285b 4061 6673  pull/676) ([@afs
+0000f4b0: 6869 6e5d 2868 7474 7073 3a2f 2f67 6974  hin](https://git
+0000f4c0: 6875 622e 636f 6d2f 6166 7368 696e 2929  hub.com/afshin))
+0000f4d0: 0a2d 2046 6f72 6365 2069 6e73 7461 6c6c  .- Force install
+0000f4e0: 2060 6a75 7079 7465 725f 636c 6965 6e74   `jupyter_client
+0000f4f0: 6020 6d61 7374 6572 205b 2336 3735 5d28  ` master [#675](
+0000f500: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000f510: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+0000f520: 6572 5f63 6c69 656e 742f 7075 6c6c 2f36  er_client/pull/6
+0000f530: 3735 2920 285b 4064 6176 6964 6272 6f63  75) ([@davidbroc
+0000f540: 6861 7274 5d28 6874 7470 733a 2f2f 6769  hart](https://gi
+0000f550: 7468 7562 2e63 6f6d 2f64 6176 6964 6272  thub.com/davidbr
+0000f560: 6f63 6861 7274 2929 0a2d 2046 6978 2070  ochart)).- Fix p
+0000f570: 726f 6a65 6374 206e 616d 6520 5b23 3637  roject name [#67
+0000f580: 345d 2868 7474 7073 3a2f 2f67 6974 6875  4](https://githu
+0000f590: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+0000f5a0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+0000f5b0: 6c2f 3637 3429 2028 5b40 7669 6461 7274  l/674) ([@vidart
+0000f5c0: 665d 2868 7474 7073 3a2f 2f67 6974 6875  f](https://githu
+0000f5d0: 622e 636f 6d2f 7669 6461 7274 6629 290a  b.com/vidartf)).
+0000f5e0: 2d20 5265 6e61 6d65 2074 7261 6974 2074  - Rename trait t
+0000f5f0: 6f20 6061 6c6c 6f77 6564 5f6b 6572 6e65  o `allowed_kerne
+0000f600: 6c73 7065 6373 6020 5b23 3637 325d 2868  lspecs` [#672](h
+0000f610: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000f620: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+0000f630: 725f 636c 6965 6e74 2f70 756c 6c2f 3637  r_client/pull/67
+0000f640: 3229 2028 5b40 626c 696e 6b31 3037 335d  2) ([@blink1073]
+0000f650: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000f660: 636f 6d2f 626c 696e 6b31 3037 3329 290a  com/blink1073)).
+0000f670: 2d20 5265 6d6f 7665 2062 6c6f 636b 2070  - Remove block p
+0000f680: 6172 616d 6574 6572 2066 726f 6d20 6067  arameter from `g
+0000f690: 6574 5f6d 7367 2829 6020 5b23 3637 315d  et_msg()` [#671]
+0000f6a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000f6b0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+0000f6c0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+0000f6d0: 3637 3129 2028 5b40 6461 7669 6462 726f  671) ([@davidbro
+0000f6e0: 6368 6172 745d 2868 7474 7073 3a2f 2f67  chart](https://g
+0000f6f0: 6974 6875 622e 636f 6d2f 6461 7669 6462  ithub.com/davidb
+0000f700: 726f 6368 6172 7429 290a 2d20 4f6e 6c79  rochart)).- Only
+0000f710: 2069 6d70 6f72 7420 606e 6573 745f 6173   import `nest_as
+0000f720: 796e 6369 6f60 206c 6f63 616c 6c79 205b  yncio` locally [
+0000f730: 2336 3635 5d28 6874 7470 733a 2f2f 6769  #665](https://gi
+0000f740: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+0000f750: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+0000f760: 7075 6c6c 2f36 3635 2920 285b 4053 796c  pull/665) ([@Syl
+0000f770: 7661 696e 436f 726c 6179 5d28 6874 7470  vainCorlay](http
+0000f780: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
+0000f790: 796c 7661 696e 436f 726c 6179 2929 0a2d  ylvainCorlay)).-
+0000f7a0: 2055 7365 2061 2064 6566 6175 6c74 2073   Use a default s
+0000f7b0: 6572 6961 6c69 7a65 7220 7468 6174 2069  erializer that i
+0000f7c0: 7320 6e6f 7420 6f6e 6c79 2066 6f72 2064  s not only for d
+0000f7d0: 6174 6520 7479 7065 7320 5b23 3636 345d  ate types [#664]
+0000f7e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000f7f0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+0000f800: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+0000f810: 3636 3429 2028 5b40 6d61 7274 696e 5265  664) ([@martinRe
+0000f820: 6e6f 755d 2868 7474 7073 3a2f 2f67 6974  nou](https://git
+0000f830: 6875 622e 636f 6d2f 6d61 7274 696e 5265  hub.com/martinRe
+0000f840: 6e6f 7529 290a 2d20 5570 6461 7465 6420  nou)).- Updated 
+0000f850: 6064 6562 7567 5f69 6e66 6f5f 7265 7370  `debug_info_resp
+0000f860: 6f6e 7365 6020 5b23 3635 375d 2868 7474  onse` [#657](htt
+0000f870: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000f880: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+0000f890: 636c 6965 6e74 2f70 756c 6c2f 3635 3729  client/pull/657)
+0000f8a0: 2028 5b40 4a6f 6861 6e4d 6162 696c 6c65   ([@JohanMabille
+0000f8b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000f8c0: 2e63 6f6d 2f4a 6f68 616e 4d61 6269 6c6c  .com/JohanMabill
+0000f8d0: 6529 290a 2d20 446f 206e 6f74 2062 6c6f  e)).- Do not blo
+0000f8e0: 636b 206f 6e20 6578 6974 205b 2336 3531  ck on exit [#651
+0000f8f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000f900: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+0000f910: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+0000f920: 2f36 3531 2920 285b 4069 6d70 6163 7432  /651) ([@impact2
+0000f930: 375d 2868 7474 7073 3a2f 2f67 6974 6875  7](https://githu
+0000f940: 622e 636f 6d2f 696d 7061 6374 3237 2929  b.com/impact27))
+0000f950: 0a2d 2055 7064 6174 6520 7465 7374 206b  .- Update test k
+0000f960: 6572 6e65 6c20 7769 7468 206e 6174 6976  ernel with nativ
+0000f970: 6520 636f 726f 7574 696e 652c 2072 656d  e coroutine, rem
+0000f980: 6f76 6520 6061 7379 6e63 5f67 656e 6572  ove `async_gener
+0000f990: 6174 6f72 6020 6465 7065 6e64 656e 6379  ator` dependency
+0000f9a0: 205b 2336 3436 5d28 6874 7470 733a 2f2f   [#646](https://
+0000f9b0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+0000f9c0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+0000f9d0: 742f 7075 6c6c 2f36 3436 2920 285b 406b  t/pull/646) ([@k
+0000f9e0: 6576 696e 2d62 6174 6573 5d28 6874 7470  evin-bates](http
+0000f9f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
+0000fa00: 6576 696e 2d62 6174 6573 2929 0a2d 2060  evin-bates)).- `
+0000fa10: 7365 7475 702e 7079 6020 616e 6420 4349  setup.py` and CI
+0000fa20: 2069 6d70 726f 7665 6d65 6e74 7320 5b23   improvements [#
+0000fa30: 3634 355d 2868 7474 7073 3a2f 2f67 6974  645](https://git
+0000fa40: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+0000fa50: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+0000fa60: 756c 6c2f 3634 3529 2028 5b40 646f 6c66  ull/645) ([@dolf
+0000fa70: 696e 7573 5d28 6874 7470 733a 2f2f 6769  inus](https://gi
+0000fa80: 7468 7562 2e63 6f6d 2f64 6f6c 6669 6e75  thub.com/dolfinu
+0000fa90: 7329 290a 2d20 5465 7374 2064 6f77 6e73  s)).- Test downs
+0000faa0: 7472 6561 6d20 7072 6f6a 6563 7473 205b  tream projects [
+0000fab0: 2336 3434 5d28 6874 7470 733a 2f2f 6769  #644](https://gi
+0000fac0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+0000fad0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+0000fae0: 7075 6c6c 2f36 3434 2920 285b 4064 6176  pull/644) ([@dav
+0000faf0: 6964 6272 6f63 6861 7274 5d28 6874 7470  idbrochart](http
+0000fb00: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+0000fb10: 6176 6964 6272 6f63 6861 7274 2929 0a2d  avidbrochart)).-
+0000fb20: 2052 656d 6f76 6520 6465 7072 6563 6174   Remove deprecat
+0000fb30: 696f 6e73 2069 6e20 6b65 726e 656c 206d  ions in kernel m
+0000fb40: 616e 6167 6572 205b 2336 3433 5d28 6874  anager [#643](ht
+0000fb50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000fb60: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+0000fb70: 5f63 6c69 656e 742f 7075 6c6c 2f36 3433  _client/pull/643
+0000fb80: 2920 285b 406b 6576 696e 2d62 6174 6573  ) ([@kevin-bates
+0000fb90: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+0000fba0: 2e63 6f6d 2f6b 6576 696e 2d62 6174 6573  .com/kevin-bates
+0000fbb0: 2929 0a2d 2041 6464 2060 626c 6f63 6b3d  )).- Add `block=
+0000fbc0: 5472 7565 6020 6261 636b 2074 6f20 6067  True` back to `g
+0000fbd0: 6574 5f6d 7367 2829 6020 5b23 3634 315d  et_msg()` [#641]
+0000fbe0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000fbf0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+0000fc00: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+0000fc10: 3634 3129 2028 5b40 6461 7669 6462 726f  641) ([@davidbro
+0000fc20: 6368 6172 745d 2868 7474 7073 3a2f 2f67  chart](https://g
+0000fc30: 6974 6875 622e 636f 6d2f 6461 7669 6462  ithub.com/davidb
+0000fc40: 726f 6368 6172 7429 290a 2d20 5069 6e20  rochart)).- Pin 
+0000fc50: 6070 7974 686f 6e3e 3d33 2e36 2e31 6020  `python>=3.6.1` 
+0000fc60: 5b23 3633 365d 2868 7474 7073 3a2f 2f67  [#636](https://g
+0000fc70: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+0000fc80: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+0000fc90: 2f70 756c 6c2f 3633 3629 2028 5b40 6461  /pull/636) ([@da
+0000fca0: 7669 6462 726f 6368 6172 745d 2868 7474  vidbrochart](htt
+0000fcb0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000fcc0: 6461 7669 6462 726f 6368 6172 7429 290a  davidbrochart)).
+0000fcd0: 2d20 5573 6520 6070 7265 2d63 6f6d 6d69  - Use `pre-commi
+0000fce0: 7460 205b 2336 3331 5d28 6874 7470 733a  t` [#631](https:
+0000fcf0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+0000fd00: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+0000fd10: 656e 742f 7075 6c6c 2f36 3331 2920 285b  ent/pull/631) ([
+0000fd20: 4064 6176 6964 6272 6f63 6861 7274 5d28  @davidbrochart](
+0000fd30: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000fd40: 6f6d 2f64 6176 6964 6272 6f63 6861 7274  om/davidbrochart
+0000fd50: 2929 0a2d 2041 7474 656d 7074 2043 4920  )).- Attempt CI 
+0000fd60: 7769 7468 2060 6970 796b 6572 6e65 6c60  with `ipykernel`
+0000fd70: 2036 2e30 2070 7265 7265 6c65 6173 6520   6.0 prerelease 
+0000fd80: 5b23 3632 395d 2868 7474 7073 3a2f 2f67  [#629](https://g
+0000fd90: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+0000fda0: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+0000fdb0: 2f70 756c 6c2f 3632 3929 2028 5b40 5379  /pull/629) ([@Sy
+0000fdc0: 6c76 6169 6e43 6f72 6c61 795d 2868 7474  lvainCorlay](htt
+0000fdd0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000fde0: 5379 6c76 6169 6e43 6f72 6c61 7929 290a  SylvainCorlay)).
+0000fdf0: 2d20 4d61 6b65 2060 4b65 726e 656c 4d61  - Make `KernelMa
+0000fe00: 6e61 6765 7260 2073 7562 636c 6173 7320  nager` subclass 
+0000fe10: 7465 7374 7320 4452 5920 5b23 3632 385d  tests DRY [#628]
+0000fe20: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000fe30: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+0000fe40: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+0000fe50: 3632 3829 2028 5b40 6461 7669 6462 726f  628) ([@davidbro
+0000fe60: 6368 6172 745d 2868 7474 7073 3a2f 2f67  chart](https://g
+0000fe70: 6974 6875 622e 636f 6d2f 6461 7669 6462  ithub.com/davidb
+0000fe80: 726f 6368 6172 7429 290a 2d20 4164 6420  rochart)).- Add 
+0000fe90: 7465 7374 7320 746f 2065 6e73 7572 6520  tests to ensure 
+0000fea0: 4d75 6c74 694b 6572 6e65 6c4d 616e 6167  MultiKernelManag
+0000feb0: 6572 2073 7562 636c 6173 7320 6d65 7468  er subclass meth
+0000fec0: 6f64 7320 6172 6520 6361 6c6c 6564 205b  ods are called [
+0000fed0: 2336 3237 5d28 6874 7470 733a 2f2f 6769  #627](https://gi
+0000fee0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+0000fef0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+0000ff00: 7075 6c6c 2f36 3237 2920 285b 406b 6576  pull/627) ([@kev
+0000ff10: 696e 2d62 6174 6573 5d28 6874 7470 733a  in-bates](https:
+0000ff20: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 6576  //github.com/kev
+0000ff30: 696e 2d62 6174 6573 2929 0a2d 2041 6464  in-bates)).- Add
+0000ff40: 2074 7970 6520 616e 6e6f 7461 7469 6f6e   type annotation
+0000ff50: 732c 2072 6566 6163 746f 7220 7379 6e63  s, refactor sync
+0000ff60: 2f61 7379 6e63 205b 2336 3233 5d28 6874  /async [#623](ht
+0000ff70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000ff80: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+0000ff90: 5f63 6c69 656e 742f 7075 6c6c 2f36 3233  _client/pull/623
+0000ffa0: 2920 285b 4064 6176 6964 6272 6f63 6861  ) ([@davidbrocha
+0000ffb0: 7274 5d28 6874 7470 733a 2f2f 6769 7468  rt](https://gith
+0000ffc0: 7562 2e63 6f6d 2f64 6176 6964 6272 6f63  ub.com/davidbroc
+0000ffd0: 6861 7274 2929 0a0a 2323 2320 446f 6375  hart))..### Docu
+0000ffe0: 6d65 6e74 6174 696f 6e20 696d 7072 6f76  mentation improv
+0000fff0: 656d 656e 7473 0a0a 2d20 4372 6561 7465  ements..- Create
+00010000: 206d 6967 7261 7469 6f6e 2067 7569 6465   migration guide
+00010010: 205b 2336 3831 5d28 6874 7470 733a 2f2f   [#681](https://
+00010020: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00010030: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00010040: 742f 7075 6c6c 2f36 3831 2920 285b 4062  t/pull/681) ([@b
+00010050: 6c69 6e6b 3130 3733 5d28 6874 7470 733a  link1073](https:
+00010060: 2f2f 6769 7468 7562 2e63 6f6d 2f62 6c69  //github.com/bli
+00010070: 6e6b 3130 3733 2929 0a2d 2055 7064 6174  nk1073)).- Updat
+00010080: 6520 6368 616e 6765 6c6f 6720 666f 7220  e changelog for 
+00010090: 372e 302e 3072 6330 205b 2336 3733 5d28  7.0.0rc0 [#673](
+000100a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000100b0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+000100c0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f36  er_client/pull/6
+000100d0: 3733 2920 285b 4062 6c69 6e6b 3130 3733  73) ([@blink1073
+000100e0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000100f0: 2e63 6f6d 2f62 6c69 6e6b 3130 3733 2929  .com/blink1073))
+00010100: 0a2d 2041 6464 6564 2064 6f63 756d 656e  .- Added documen
+00010110: 7461 7469 6f6e 2066 6f72 2060 7269 6368  tation for `rich
+00010120: 496e 7370 6563 7456 6172 6961 626c 6573  InspectVariables
+00010130: 6020 7265 7175 6573 7420 5b23 3635 345d  ` request [#654]
+00010140: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00010150: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00010160: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00010170: 3635 3429 2028 5b40 4a6f 6861 6e4d 6162  654) ([@JohanMab
+00010180: 696c 6c65 5d28 6874 7470 733a 2f2f 6769  ille](https://gi
+00010190: 7468 7562 2e63 6f6d 2f4a 6f68 616e 4d61  thub.com/JohanMa
+000101a0: 6269 6c6c 6529 290a 2d20 4368 616e 6765  bille)).- Change
+000101b0: 2074 6f20 6065 6469 745f 6d61 6769 6360   to `edit_magic`
+000101c0: 2070 6179 6c6f 6164 205b 2336 3532 5d28   payload [#652](
+000101d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000101e0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+000101f0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f36  er_client/pull/6
+00010200: 3532 2920 285b 4079 6974 7a63 6861 6b5d  52) ([@yitzchak]
+00010210: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00010220: 636f 6d2f 7969 747a 6368 616b 2929 0a2d  com/yitzchak)).-
+00010230: 2041 6464 6564 206d 6973 7369 6e67 2064   Added missing d
+00010240: 6f63 756d 656e 7461 7469 6f6e 2066 6f72  ocumentation for
+00010250: 2074 6865 2069 6e73 7065 6374 5661 7269   the inspectVari
+00010260: 6162 6c65 7320 7265 7175 6573 7420 616e  ables request an
+00010270: 6420 7265 7370 e280 a620 5b23 3634 395d  d resp... [#649]
+00010280: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00010290: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+000102a0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+000102b0: 3634 3929 2028 5b40 4a6f 6861 6e4d 6162  649) ([@JohanMab
+000102c0: 696c 6c65 5d28 6874 7470 733a 2f2f 6769  ille](https://gi
+000102d0: 7468 7562 2e63 6f6d 2f4a 6f68 616e 4d61  thub.com/JohanMa
+000102e0: 6269 6c6c 6529 290a 2d20 4164 6420 7374  bille)).- Add st
+000102f0: 6174 7573 2066 6965 6c64 2074 6f20 6f74  atus field to ot
+00010300: 6865 7220 7265 706c 6965 7320 696e 2064  her replies in d
+00010310: 6f63 756d 656e 7461 7469 6f6e 205b 2336  ocumentation [#6
+00010320: 3438 5d28 6874 7470 733a 2f2f 6769 7468  48](https://gith
+00010330: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00010340: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+00010350: 6c6c 2f36 3438 2920 285b 4079 6974 7a63  ll/648) ([@yitzc
+00010360: 6861 6b5d 2868 7474 7073 3a2f 2f67 6974  hak](https://git
+00010370: 6875 622e 636f 6d2f 7969 747a 6368 616b  hub.com/yitzchak
+00010380: 2929 0a0a 2323 2320 436f 6e74 7269 6275  ))..### Contribu
+00010390: 746f 7273 2074 6f20 7468 6973 2072 656c  tors to this rel
+000103a0: 6561 7365 0a0a 285b 4769 7448 7562 2063  ease..([GitHub c
+000103b0: 6f6e 7472 6962 7574 6f72 7320 7061 6765  ontributors page
+000103c0: 2066 6f72 2074 6869 7320 7265 6c65 6173   for this releas
+000103d0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+000103e0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+000103f0: 7079 7465 725f 636c 6965 6e74 2f67 7261  pyter_client/gra
+00010400: 7068 732f 636f 6e74 7269 6275 746f 7273  phs/contributors
+00010410: 3f66 726f 6d3d 3230 3231 2d30 332d 3134  ?from=2021-03-14
+00010420: 2674 6f3d 3230 3231 2d30 382d 3136 2674  &to=2021-08-16&t
+00010430: 7970 653d 6329 290a 0a5b 4061 6673 6869  ype=c))..[@afshi
+00010440: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
+00010450: 622e 636f 6d2f 7365 6172 6368 3f71 3d72  b.com/search?q=r
+00010460: 6570 6f25 3341 6a75 7079 7465 7225 3246  epo%3Ajupyter%2F
+00010470: 6a75 7079 7465 725f 636c 6965 6e74 2b69  jupyter_client+i
+00010480: 6e76 6f6c 7665 7325 3341 6166 7368 696e  nvolves%3Aafshin
+00010490: 2b75 7064 6174 6564 2533 4132 3032 312d  +updated%3A2021-
+000104a0: 3033 2d31 342e 2e32 3032 312d 3038 2d31  03-14..2021-08-1
+000104b0: 3626 7479 7065 3d49 7373 7565 7329 207c  6&type=Issues) |
+000104c0: 205b 4062 6c69 6e6b 3130 3733 5d28 6874   [@blink1073](ht
+000104d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000104e0: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+000104f0: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+00010500: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+00010510: 6573 2533 4162 6c69 6e6b 3130 3733 2b75  es%3Ablink1073+u
+00010520: 7064 6174 6564 2533 4132 3032 312d 3033  pdated%3A2021-03
+00010530: 2d31 342e 2e32 3032 312d 3038 2d31 3626  -14..2021-08-16&
+00010540: 7479 7065 3d49 7373 7565 7329 207c 205b  type=Issues) | [
+00010550: 4043 6172 7265 6175 5d28 6874 7470 733a  @Carreau](https:
+00010560: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+00010570: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+00010580: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+00010590: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+000105a0: 4143 6172 7265 6175 2b75 7064 6174 6564  ACarreau+updated
+000105b0: 2533 4132 3032 312d 3033 2d31 342e 2e32  %3A2021-03-14..2
+000105c0: 3032 312d 3038 2d31 3626 7479 7065 3d49  021-08-16&type=I
+000105d0: 7373 7565 7329 207c 205b 4063 636f 7264  ssues) | [@ccord
+000105e0: 6f62 6131 325d 2868 7474 7073 3a2f 2f67  oba12](https://g
+000105f0: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+00010600: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+00010610: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+00010620: 6e74 2b69 6e76 6f6c 7665 7325 3341 6363  nt+involves%3Acc
+00010630: 6f72 646f 6261 3132 2b75 7064 6174 6564  ordoba12+updated
+00010640: 2533 4132 3032 312d 3033 2d31 342e 2e32  %3A2021-03-14..2
+00010650: 3032 312d 3038 2d31 3626 7479 7065 3d49  021-08-16&type=I
+00010660: 7373 7565 7329 207c 205b 4064 6176 6964  ssues) | [@david
+00010670: 6272 6f63 6861 7274 5d28 6874 7470 733a  brochart](https:
+00010680: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+00010690: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+000106a0: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+000106b0: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+000106c0: 4164 6176 6964 6272 6f63 6861 7274 2b75  Adavidbrochart+u
+000106d0: 7064 6174 6564 2533 4132 3032 312d 3033  pdated%3A2021-03
+000106e0: 2d31 342e 2e32 3032 312d 3038 2d31 3626  -14..2021-08-16&
+000106f0: 7479 7065 3d49 7373 7565 7329 207c 205b  type=Issues) | [
+00010700: 4064 6869 7273 6368 6665 6c64 5d28 6874  @dhirschfeld](ht
+00010710: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00010720: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+00010730: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+00010740: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+00010750: 6573 2533 4164 6869 7273 6368 6665 6c64  es%3Adhirschfeld
+00010760: 2b75 7064 6174 6564 2533 4132 3032 312d  +updated%3A2021-
+00010770: 3033 2d31 342e 2e32 3032 312d 3038 2d31  03-14..2021-08-1
+00010780: 3626 7479 7065 3d49 7373 7565 7329 207c  6&type=Issues) |
+00010790: 205b 4064 6f6c 6669 6e75 735d 2868 7474   [@dolfinus](htt
+000107a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000107b0: 7365 6172 6368 3f71 3d72 6570 6f25 3341  search?q=repo%3A
+000107c0: 6a75 7079 7465 7225 3246 6a75 7079 7465  jupyter%2Fjupyte
+000107d0: 725f 636c 6965 6e74 2b69 6e76 6f6c 7665  r_client+involve
+000107e0: 7325 3341 646f 6c66 696e 7573 2b75 7064  s%3Adolfinus+upd
+000107f0: 6174 6564 2533 4132 3032 312d 3033 2d31  ated%3A2021-03-1
+00010800: 342e 2e32 3032 312d 3038 2d31 3626 7479  4..2021-08-16&ty
+00010810: 7065 3d49 7373 7565 7329 207c 205b 4065  pe=Issues) | [@e
+00010820: 6368 6172 6c65 735d 2868 7474 7073 3a2f  charles](https:/
+00010830: 2f67 6974 6875 622e 636f 6d2f 7365 6172  /github.com/sear
+00010840: 6368 3f71 3d72 6570 6f25 3341 6a75 7079  ch?q=repo%3Ajupy
+00010850: 7465 7225 3246 6a75 7079 7465 725f 636c  ter%2Fjupyter_cl
+00010860: 6965 6e74 2b69 6e76 6f6c 7665 7325 3341  ient+involves%3A
+00010870: 6563 6861 726c 6573 2b75 7064 6174 6564  echarles+updated
+00010880: 2533 4132 3032 312d 3033 2d31 342e 2e32  %3A2021-03-14..2
+00010890: 3032 312d 3038 2d31 3626 7479 7065 3d49  021-08-16&type=I
+000108a0: 7373 7565 7329 207c 205b 4069 6d70 6163  ssues) | [@impac
+000108b0: 7432 375d 2868 7474 7073 3a2f 2f67 6974  t27](https://git
+000108c0: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
+000108d0: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
+000108e0: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
+000108f0: 2b69 6e76 6f6c 7665 7325 3341 696d 7061  +involves%3Aimpa
+00010900: 6374 3237 2b75 7064 6174 6564 2533 4132  ct27+updated%3A2
+00010910: 3032 312d 3033 2d31 342e 2e32 3032 312d  021-03-14..2021-
+00010920: 3038 2d31 3626 7479 7065 3d49 7373 7565  08-16&type=Issue
+00010930: 7329 207c 205b 404a 6f68 616e 4d61 6269  s) | [@JohanMabi
+00010940: 6c6c 655d 2868 7474 7073 3a2f 2f67 6974  lle](https://git
+00010950: 6875 622e 636f 6d2f 7365 6172 6368 3f71  hub.com/search?q
+00010960: 3d72 6570 6f25 3341 6a75 7079 7465 7225  =repo%3Ajupyter%
+00010970: 3246 6a75 7079 7465 725f 636c 6965 6e74  2Fjupyter_client
+00010980: 2b69 6e76 6f6c 7665 7325 3341 4a6f 6861  +involves%3AJoha
+00010990: 6e4d 6162 696c 6c65 2b75 7064 6174 6564  nMabille+updated
+000109a0: 2533 4132 3032 312d 3033 2d31 342e 2e32  %3A2021-03-14..2
+000109b0: 3032 312d 3038 2d31 3626 7479 7065 3d49  021-08-16&type=I
+000109c0: 7373 7565 7329 207c 205b 406b 6576 696e  ssues) | [@kevin
+000109d0: 2d62 6174 6573 5d28 6874 7470 733a 2f2f  -bates](https://
+000109e0: 6769 7468 7562 2e63 6f6d 2f73 6561 7263  github.com/searc
+000109f0: 683f 713d 7265 706f 2533 416a 7570 7974  h?q=repo%3Ajupyt
+00010a00: 6572 2532 466a 7570 7974 6572 5f63 6c69  er%2Fjupyter_cli
+00010a10: 656e 742b 696e 766f 6c76 6573 2533 416b  ent+involves%3Ak
+00010a20: 6576 696e 2d62 6174 6573 2b75 7064 6174  evin-bates+updat
+00010a30: 6564 2533 4132 3032 312d 3033 2d31 342e  ed%3A2021-03-14.
+00010a40: 2e32 3032 312d 3038 2d31 3626 7479 7065  .2021-08-16&type
+00010a50: 3d49 7373 7565 7329 207c 205b 406d 6172  =Issues) | [@mar
+00010a60: 7469 6e52 656e 6f75 5d28 6874 7470 733a  tinRenou](https:
+00010a70: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6561  //github.com/sea
+00010a80: 7263 683f 713d 7265 706f 2533 416a 7570  rch?q=repo%3Ajup
+00010a90: 7974 6572 2532 466a 7570 7974 6572 5f63  yter%2Fjupyter_c
+00010aa0: 6c69 656e 742b 696e 766f 6c76 6573 2533  lient+involves%3
+00010ab0: 416d 6172 7469 6e52 656e 6f75 2b75 7064  AmartinRenou+upd
+00010ac0: 6174 6564 2533 4132 3032 312d 3033 2d31  ated%3A2021-03-1
+00010ad0: 342e 2e32 3032 312d 3038 2d31 3626 7479  4..2021-08-16&ty
+00010ae0: 7065 3d49 7373 7565 7329 207c 205b 406d  pe=Issues) | [@m
+00010af0: 6174 7469 705d 2868 7474 7073 3a2f 2f67  attip](https://g
+00010b00: 6974 6875 622e 636f 6d2f 7365 6172 6368  ithub.com/search
+00010b10: 3f71 3d72 6570 6f25 3341 6a75 7079 7465  ?q=repo%3Ajupyte
+00010b20: 7225 3246 6a75 7079 7465 725f 636c 6965  r%2Fjupyter_clie
+00010b30: 6e74 2b69 6e76 6f6c 7665 7325 3341 6d61  nt+involves%3Ama
+00010b40: 7474 6970 2b75 7064 6174 6564 2533 4132  ttip+updated%3A2
+00010b50: 3032 312d 3033 2d31 342e 2e32 3032 312d  021-03-14..2021-
+00010b60: 3038 2d31 3626 7479 7065 3d49 7373 7565  08-16&type=Issue
+00010b70: 7329 207c 205b 406d 696e 726b 5d28 6874  s) | [@minrk](ht
+00010b80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00010b90: 2f73 6561 7263 683f 713d 7265 706f 2533  /search?q=repo%3
+00010ba0: 416a 7570 7974 6572 2532 466a 7570 7974  Ajupyter%2Fjupyt
+00010bb0: 6572 5f63 6c69 656e 742b 696e 766f 6c76  er_client+involv
+00010bc0: 6573 2533 416d 696e 726b 2b75 7064 6174  es%3Aminrk+updat
+00010bd0: 6564 2533 4132 3032 312d 3033 2d31 342e  ed%3A2021-03-14.
+00010be0: 2e32 3032 312d 3038 2d31 3626 7479 7065  .2021-08-16&type
+00010bf0: 3d49 7373 7565 7329 207c 205b 404d 5365  =Issues) | [@MSe
+00010c00: 616c 5d28 6874 7470 733a 2f2f 6769 7468  al](https://gith
+00010c10: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
+00010c20: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
+00010c30: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
+00010c40: 696e 766f 6c76 6573 2533 414d 5365 616c  involves%3AMSeal
+00010c50: 2b75 7064 6174 6564 2533 4132 3032 312d  +updated%3A2021-
+00010c60: 3033 2d31 342e 2e32 3032 312d 3038 2d31  03-14..2021-08-1
+00010c70: 3626 7479 7065 3d49 7373 7565 7329 207c  6&type=Issues) |
+00010c80: 205b 4053 796c 7661 696e 436f 726c 6179   [@SylvainCorlay
+00010c90: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00010ca0: 2e63 6f6d 2f73 6561 7263 683f 713d 7265  .com/search?q=re
+00010cb0: 706f 2533 416a 7570 7974 6572 2532 466a  po%3Ajupyter%2Fj
+00010cc0: 7570 7974 6572 5f63 6c69 656e 742b 696e  upyter_client+in
+00010cd0: 766f 6c76 6573 2533 4153 796c 7661 696e  volves%3ASylvain
+00010ce0: 436f 726c 6179 2b75 7064 6174 6564 2533  Corlay+updated%3
+00010cf0: 4132 3032 312d 3033 2d31 342e 2e32 3032  A2021-03-14..202
+00010d00: 312d 3038 2d31 3626 7479 7065 3d49 7373  1-08-16&type=Iss
+00010d10: 7565 7329 207c 205b 4074 616b 6c75 7976  ues) | [@takluyv
+00010d20: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
+00010d30: 7562 2e63 6f6d 2f73 6561 7263 683f 713d  ub.com/search?q=
+00010d40: 7265 706f 2533 416a 7570 7974 6572 2532  repo%3Ajupyter%2
+00010d50: 466a 7570 7974 6572 5f63 6c69 656e 742b  Fjupyter_client+
+00010d60: 696e 766f 6c76 6573 2533 4174 616b 6c75  involves%3Ataklu
+00010d70: 7976 6572 2b75 7064 6174 6564 2533 4132  yver+updated%3A2
+00010d80: 3032 312d 3033 2d31 342e 2e32 3032 312d  021-03-14..2021-
+00010d90: 3038 2d31 3626 7479 7065 3d49 7373 7565  08-16&type=Issue
+00010da0: 7329 207c 205b 4076 6964 6172 7466 5d28  s) | [@vidartf](
+00010db0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00010dc0: 6f6d 2f73 6561 7263 683f 713d 7265 706f  om/search?q=repo
+00010dd0: 2533 416a 7570 7974 6572 2532 466a 7570  %3Ajupyter%2Fjup
+00010de0: 7974 6572 5f63 6c69 656e 742b 696e 766f  yter_client+invo
+00010df0: 6c76 6573 2533 4176 6964 6172 7466 2b75  lves%3Avidartf+u
+00010e00: 7064 6174 6564 2533 4132 3032 312d 3033  pdated%3A2021-03
+00010e10: 2d31 342e 2e32 3032 312d 3038 2d31 3626  -14..2021-08-16&
+00010e20: 7479 7065 3d49 7373 7565 7329 207c 205b  type=Issues) | [
+00010e30: 4079 6974 7a63 6861 6b5d 2868 7474 7073  @yitzchak](https
+00010e40: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
+00010e50: 6172 6368 3f71 3d72 6570 6f25 3341 6a75  arch?q=repo%3Aju
+00010e60: 7079 7465 7225 3246 6a75 7079 7465 725f  pyter%2Fjupyter_
+00010e70: 636c 6965 6e74 2b69 6e76 6f6c 7665 7325  client+involves%
+00010e80: 3341 7969 747a 6368 616b 2b75 7064 6174  3Ayitzchak+updat
+00010e90: 6564 2533 4132 3032 312d 3033 2d31 342e  ed%3A2021-03-14.
+00010ea0: 2e32 3032 312d 3038 2d31 3626 7479 7065  .2021-08-16&type
+00010eb0: 3d49 7373 7565 7329 0a0a 2323 2036 2e32  =Issues)..## 6.2
+00010ec0: 2e30 0a0a 2d20 5961 6e6b 6564 2028 5079  .0..- Yanked (Py
+00010ed0: 5049 2920 616e 6420 6d61 726b 6564 2061  PI) and marked a
+00010ee0: 7320 6272 6f6b 656e 2028 636f 6e64 6129  s broken (conda)
+00010ef0: 0a0a 2323 2036 2e31 2e31 330a 0a2d 2059  ..## 6.1.13..- Y
+00010f00: 616e 6b65 6420 2850 7950 4929 2061 6e64  anked (PyPI) and
+00010f10: 206d 6172 6b65 6420 6173 2062 726f 6b65   marked as broke
+00010f20: 6e20 2863 6f6e 6461 290a 0a23 2320 362e  n (conda)..## 6.
+00010f30: 312e 3132 0a0a 2d20 5368 7574 646f 776e  1.12..- Shutdown
+00010f40: 2072 6571 7565 7374 2073 6571 7565 6e63   request sequenc
+00010f50: 6520 6861 7320 6265 656e 206d 6f64 6966  e has been modif
+00010f60: 6965 6420 746f 2062 6520 6d6f 7265 2067  ied to be more g
+00010f70: 7261 6365 6675 6c2c 2069 740a 2020 6e6f  raceful, it.  no
+00010f80: 7720 6973 2070 7265 6365 6465 6420 6279  w is preceded by
+00010f90: 2069 6e74 6572 7275 7074 2c20 616e 6420   interrupt, and 
+00010fa0: 7769 6c6c 2061 6c73 6f20 7365 6e64 2061  will also send a
+00010fb0: 2060 5349 4754 4552 4d60 2062 6566 6f72   `SIGTERM` befor
+00010fc0: 650a 2020 666f 7263 6962 6c79 206b 696c  e.  forcibly kil
+00010fd0: 6c69 6e67 2074 6865 206b 6572 6e65 6c2e  ling the kernel.
+00010fe0: 205b 2336 3230 5d28 6874 7470 733a 2f2f   [#620](https://
+00010ff0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00011000: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00011010: 742f 7075 6c6c 2f36 3230 290a 2d20 5265  t/pull/620).- Re
+00011020: 6d6f 7661 6c20 6f66 2060 6970 7974 686f  moval of `ipytho
+00011030: 6e5f 6765 6e75 7469 6c73 6020 6173 2061  n_genutils` as a
+00011040: 2064 6570 656e 6465 6e63 792e 2049 7420   dependency. It 
+00011050: 7761 7320 696d 706c 6963 6974 0a20 2062  was implicit.  b
+00011060: 6566 6f72 653b 2062 7574 2072 6571 7569  efore; but requi
+00011070: 7265 6420 6279 2061 7420 6c65 6173 7420  red by at least 
+00011080: 7472 6169 746c 6574 7320 7468 7573 2061  traitlets thus a
+00011090: 766f 6964 696e 6720 6973 7375 6573 2e20  voiding issues. 
+000110a0: 5765 0a20 2061 7265 2077 6f72 6b69 6e67  We.  are working
+000110b0: 206f 6e20 636f 6d70 6c65 7465 6c79 2072   on completely r
+000110c0: 656d 6f76 696e 6720 6974 2066 726f 6d20  emoving it from 
+000110d0: 616c 6c20 6a75 7079 7465 7220 6465 7065  all jupyter depe
+000110e0: 6e64 656e 6369 6573 3b0a 2020 6173 2069  ndencies;.  as i
+000110f0: 7420 6d69 6768 7420 6c65 6164 2074 6f20  t might lead to 
+00011100: 6973 7375 6573 2070 6163 6b61 6769 6e67  issues packaging
+00011110: 2066 6f72 2050 7974 686f 6e20 332e 3130   for Python 3.10
+00011120: 2c20 616e 6420 7761 7320 6d6f 7374 6c79  , and was mostly
+00011130: 0a20 2075 7365 6420 666f 7220 636f 6d70  .  used for comp
+00011140: 6174 6962 696c 6974 7920 7769 7468 2070  atibility with p
+00011150: 7974 686f 6e20 322e 2028 5b23 3632 305d  ython 2. ([#620]
+00011160: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00011170: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00011180: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00011190: 3632 3029 2c20 5b23 3630 355d 2868 7474  620), [#605](htt
+000111a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000111b0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+000111c0: 636c 6965 6e74 2f70 756c 6c2f 3630 3529  client/pull/605)
+000111d0: 290a 2d20 4164 6472 6573 7320 6120 7261  ).- Address a ra
+000111e0: 6365 2063 6f6e 6469 7469 6f6e 2062 6574  ce condition bet
+000111f0: 7765 656e 2060 7368 7574 646f 776e 5f6b  ween `shutdown_k
+00011200: 6572 6e65 6c60 2061 6e64 2072 6573 7461  ernel` and resta
+00011210: 7274 6572 2e0a 2020 285b 2336 3037 5d28  rter..  ([#607](
+00011220: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00011230: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00011240: 6572 5f63 6c69 656e 742f 7075 6c6c 2f36  er_client/pull/6
+00011250: 3037 292e 290a 0a53 6565 2074 6865 205b  07).)..See the [
+00011260: 6675 6c6c 206c 6973 7420 6f66 0a70 756c  full list of.pul
+00011270: 6c2d 7265 7175 6573 7473 5d28 6874 7470  l-requests](http
+00011280: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00011290: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
+000112a0: 6c69 656e 742f 6d69 6c65 7374 6f6e 652f  lient/milestone/
+000112b0: 3237 3f63 6c6f 7365 643d 3129 0a0a 2323  27?closed=1)..##
+000112c0: 2036 2e31 2e31 310a 0a2d 204d 6f76 6520   6.1.11..- Move 
+000112d0: 6a65 6469 2070 696e 6e69 6e67 2074 6f20  jedi pinning to 
+000112e0: 7465 7374 2072 6571 7569 7265 6d65 6e74  test requirement
+000112f0: 7320 5b23 3539 395d 2868 7474 7073 3a2f  s [#599](https:/
+00011300: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00011310: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00011320: 6e74 2f70 756c 6c2f 3539 3929 0a0a 2323  nt/pull/599)..##
+00011330: 2036 2e31 2e31 300a 0a2d 2041 6464 2063   6.1.10..- Add c
+00011340: 6861 6e67 6520 7061 7261 6d65 7465 7220  hange parameter 
+00011350: 6e65 6564 6564 2066 6f72 206f 6273 6572  needed for obser
+00011360: 7665 7220 6d65 7468 6f64 206f 660a 2020  ver method of.  
+00011370: 6b65 726e 656c 5f73 7065 635f 6d61 6e61  kernel_spec_mana
+00011380: 6765 7220 7472 6169 7420 5b23 3539 385d  ger trait [#598]
+00011390: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000113a0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+000113b0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+000113c0: 3539 3829 0a0a 2323 2036 2e31 2e39 0a0a  598)..## 6.1.9..
+000113d0: 2d20 5069 6e20 6a65 6469 5c3c 3d30 2e31  - Pin jedi\<=0.1
+000113e0: 372e 3220 5b23 3539 365d 2868 7474 7073  7.2 [#596](https
+000113f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00011400: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+00011410: 6965 6e74 2f70 756c 6c2f 3539 3629 0a0a  ient/pull/596)..
+00011420: 2323 2036 2e31 2e38 0a0a 2d20 446f 6320  ## 6.1.8..- Doc 
+00011430: 7570 6461 7465 7320 285b 2335 3633 5d28  updates ([#563](
+00011440: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00011450: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00011460: 6572 5f63 6c69 656e 742f 7075 6c6c 2f35  er_client/pull/5
+00011470: 3633 292c 0a20 205b 2335 3634 5d28 6874  63),.  [#564](ht
+00011480: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00011490: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+000114a0: 5f63 6c69 656e 742f 7075 6c6c 2f35 3634  _client/pull/564
+000114b0: 292c 205b 2335 3837 5d28 6874 7470 733a  ), [#587](https:
+000114c0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+000114d0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+000114e0: 656e 742f 7075 6c6c 2f35 3837 2929 0a2d  ent/pull/587)).-
+000114f0: 2046 6978 2070 6174 6820 746f 2074 6865   Fix path to the
+00011500: 2063 6f6e 6e65 6374 696f 6e20 6669 6c65   connection file
+00011510: 205b 2335 3638 5d28 6874 7470 733a 2f2f   [#568](https://
+00011520: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00011530: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00011540: 742f 7075 6c6c 2f35 3638 290a 2d20 436f  t/pull/568).- Co
+00011550: 6465 2063 6c65 616e 7570 2028 5b23 3537  de cleanup ([#57
+00011560: 345d 2868 7474 7073 3a2f 2f67 6974 6875  4](https://githu
+00011570: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00011580: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00011590: 6c2f 3537 3429 2c0a 2020 5b23 3537 395d  l/574),.  [#579]
+000115a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000115b0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+000115c0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+000115d0: 3537 3929 290a 2d20 5369 6c65 6e63 6520  579)).- Silence 
+000115e0: 6b69 6c6c 5f6b 6572 6e65 6c20 7768 656e  kill_kernel when
+000115f0: 206e 6f20 7072 6f63 6573 7320 6973 2070   no process is p
+00011600: 7265 7365 6e74 0a20 205b 2335 3736 5d28  resent.  [#576](
+00011610: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00011620: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00011630: 6572 5f63 6c69 656e 742f 7075 6c6c 2f35  er_client/pull/5
+00011640: 3736 290a 2d20 5265 6d6f 7665 2065 7874  76).- Remove ext
+00011650: 7261 5f65 6e76 2061 6e64 2063 6f72 7265  ra_env and corre
+00011660: 7370 6f6e 6469 6e67 2074 6573 7420 5b23  sponding test [#
+00011670: 3538 315d 2868 7474 7073 3a2f 2f67 6974  581](https://git
+00011680: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00011690: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+000116a0: 756c 6c2f 3538 3129 0a2d 2041 6464 2064  ull/581).- Add d
+000116b0: 6f63 756d 656e 7461 7469 6f6e 2064 6570  ocumentation dep
+000116c0: 656e 6465 6e63 6965 7320 746f 2073 6574  endencies to set
+000116d0: 7570 2e70 7920 5b23 3538 325d 2868 7474  up.py [#582](htt
+000116e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000116f0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00011700: 636c 6965 6e74 2f70 756c 6c2f 3538 3229  client/pull/582)
+00011710: 0a2d 2046 6978 2066 6f72 2057 696e 646f  .- Fix for Windo
+00011720: 7773 206c 6f63 616c 686f 7374 2049 5020  ws localhost IP 
+00011730: 6164 6472 6573 7365 7320 5b23 3538 345d  addresses [#584]
+00011740: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00011750: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00011760: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00011770: 3538 3429 0a2d 2044 726f 7020 5472 6176  584).- Drop Trav
+00011780: 6973 2043 492c 2061 6464 2047 6974 4875  is CI, add GitHu
+00011790: 6220 4163 7469 6f6e 7320 5b23 3538 365d  b Actions [#586]
+000117a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000117b0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+000117c0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+000117d0: 3538 3629 0a2d 2041 6461 7074 204b 6572  586).- Adapt Ker
+000117e0: 6e65 6c4d 616e 6167 6572 2e5c 5f6b 6572  nelManager.\_ker
+000117f0: 6e65 6c5f 7370 6563 5f6d 616e 6167 6572  nel_spec_manager
+00011800: 5f63 6861 6e67 6564 2074 6f20 6f62 7365  _changed to obse
+00011810: 7276 650a 2020 5b23 3538 385d 2868 7474  rve.  [#588](htt
+00011820: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00011830: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00011840: 636c 6965 6e74 2f70 756c 6c2f 3538 3829  client/pull/588)
+00011850: 0a2d 2041 6c6c 6f77 2075 7365 207e 2f20  .- Allow use ~/ 
+00011860: 696e 2074 6865 206b 6572 6e65 6c27 7320  in the kernel's 
+00011870: 636f 6d6d 616e 6420 6f72 2069 7473 2061  command or its a
+00011880: 7267 756d 656e 7473 0a20 205b 2335 3839  rguments.  [#589
+00011890: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000118a0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+000118b0: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+000118c0: 2f35 3839 290a 2d20 4368 616e 6765 2077  /589).- Change w
+000118d0: 6169 745f 666f 725f 7265 6164 7920 6c6f  ait_for_ready lo
+000118e0: 6769 6320 5b23 3539 325d 2868 7474 7073  gic [#592](https
+000118f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00011900: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+00011910: 6965 6e74 2f70 756c 6c2f 3539 3229 0a2d  ient/pull/592).-
+00011920: 2046 6978 2074 6573 745f 7365 7373 696f   Fix test_sessio
+00011930: 6e20 7769 7468 206d 7367 7061 636b 2076  n with msgpack v
+00011940: 3120 5b23 3539 345d 2868 7474 7073 3a2f  1 [#594](https:/
+00011950: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00011960: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00011970: 6e74 2f70 756c 6c2f 3539 3429 0a0a 2323  nt/pull/594)..##
+00011980: 2036 2e31 2e36 0a0a 2d20 5265 6d6f 7665   6.1.6..- Remove
+00011990: 6420 7761 726e 696e 6773 2069 6e20 6d6f  d warnings in mo
+000119a0: 7265 2063 6173 6573 2066 6f72 204b 6572  re cases for Ker
+000119b0: 6e65 6c4d 616e 6167 6572 7320 7468 6174  nelManagers that
+000119c0: 2075 7365 206e 6577 0a20 2063 6c65 616e   use new.  clean
+000119d0: 7570 206d 6574 686f 6420 5b23 3536 305d  up method [#560]
+000119e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000119f0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00011a00: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00011a10: 3536 3029 0a2d 2053 6f6d 6520 696d 7072  560).- Some impr
+00011a20: 6f76 6564 2074 6573 7473 2077 6974 6820  oved tests with 
+00011a30: 6120 636f 6e76 6572 7369 6f6e 2074 6f20  a conversion to 
+00011a40: 7079 7465 7374 2070 6174 7465 726e 0a20  pytest pattern. 
+00011a50: 205b 2335 3631 5d28 6874 7470 733a 2f2f   [#561](https://
+00011a60: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00011a70: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00011a80: 742f 7075 6c6c 2f35 3631 290a 0a23 2320  t/pull/561)..## 
+00011a90: 362e 312e 350a 0a2d 2047 7261 6365 6675  6.1.5..- Gracefu
+00011aa0: 6c6c 7920 436c 6f73 6520 5a4d 5120 436f  lly Close ZMQ Co
+00011ab0: 6e74 6578 7420 7570 6f6e 206b 6572 6e65  ntext upon kerne
+00011ac0: 6c20 7368 7574 646f 776e 2074 6f20 6669  l shutdown to fi
+00011ad0: 7820 6d65 6d6f 7279 206c 6561 6b0a 2020  x memory leak.  
+00011ae0: 5b23 3534 385d 2868 7474 7073 3a2f 2f67  [#548](https://g
+00011af0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00011b00: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00011b10: 2f70 756c 6c2f 3534 3829 0a2d 2046 6978  /pull/548).- Fix
+00011b20: 2066 6f72 2063 6861 696e 6564 2065 7863   for chained exc
+00011b30: 6570 7469 6f6e 7320 746f 2070 7265 7365  eptions to prese
+00011b40: 7276 6520 7374 6163 6b73 0a20 2028 5b23  rve stacks.  ([#
+00011b50: 3535 325d 2868 7474 7073 3a2f 2f67 6974  552](https://git
+00011b60: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00011b70: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+00011b80: 756c 6c2f 3535 3229 2c20 5b23 3535 345d  ull/552), [#554]
+00011b90: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00011ba0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00011bb0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00011bc0: 3535 3429 290a 2d20 4669 7820 7374 6172  554)).- Fix star
+00011bd0: 745f 6b65 726e 656c 2065 7272 6f72 2077  t_kernel error w
+00011be0: 6865 6e20 7061 7373 696e 6720 6b65 726e  hen passing kern
+00011bf0: 656c 5f69 640a 2020 5b23 3534 375d 2868  el_id.  [#547](h
+00011c00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00011c10: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+00011c20: 725f 636c 6965 6e74 2f70 756c 6c2f 3534  r_client/pull/54
+00011c30: 3729 0a2d 2055 7064 6174 6520 746f 2072  7).- Update to r
+00011c40: 656c 6561 7369 6e67 2064 6f63 7320 5b23  eleasing docs [#
+00011c50: 3534 335d 2868 7474 7073 3a2f 2f67 6974  543](https://git
+00011c60: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00011c70: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+00011c80: 756c 6c2f 3534 3329 0a0a 2323 2036 2e31  ull/543)..## 6.1
+00011c90: 2e34 0a0a 2844 656c 6574 6564 2072 656c  .4..(Deleted rel
+00011ca0: 6561 7365 2077 6974 6820 696e 636f 7272  ease with incorr
+00011cb0: 6563 7420 6c6f 6361 6c20 6669 6c65 7329  ect local files)
+00011cc0: 0a0a 2323 2036 2e31 2e33 0a0a 2d20 4164  ..## 6.1.3..- Ad
+00011cd0: 6420 4173 796e 634b 6572 6e65 6c43 6c69  d AsyncKernelCli
+00011ce0: 656e 7420 636c 6965 6e74 5f63 6c61 7373  ent client_class
+00011cf0: 2074 6f20 4173 796e 634b 6572 6e65 6c4d   to AsyncKernelM
+00011d00: 616e 6167 6572 0a20 205b 2335 3432 5d28  anager.  [#542](
 00011d10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
 00011d20: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
 00011d30: 6572 5f63 6c69 656e 742f 7075 6c6c 2f35  er_client/pull/5
-00011d40: 3030 290a 0a42 7265 616b 696e 6720 6368  00)..Breaking ch
-00011d50: 616e 6765 733a 0a0a 2d20 4472 6f70 7065  anges:..- Droppe
-00011d60: 6420 7375 7070 6f72 7420 666f 7220 5079  d support for Py
-00011d70: 7468 6f6e 2032 2e37 210a 0a23 2320 352e  thon 2.7!..## 5.
-00011d80: 332e 350a 0a2d 2042 6163 6b70 6f72 7465  3.5..- Backporte
-00011d90: 6420 6d65 6d6f 7279 206c 6561 6b20 6669  d memory leak fi
-00011da0: 7820 5b23 3534 385d 2868 7474 7073 3a2f  x [#548](https:/
-00011db0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-00011dc0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-00011dd0: 6e74 2f70 756c 6c2f 3534 3829 0a20 205b  nt/pull/548).  [
-00011de0: 2335 3535 5d28 6874 7470 733a 2f2f 6769  #555](https://gi
-00011df0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-00011e00: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-00011e10: 7075 6c6c 2f35 3535 292e 0a0a 2323 2035  pull/555)...## 5
-00011e20: 2e33 2e34 0a0a 2d20 4368 616e 6765 6420  .3.4..- Changed 
-00011e30: 7365 6375 7265 5f77 7269 7465 2074 6f20  secure_write to 
-00011e40: 6265 2069 6d70 6f72 7465 6420 6672 6f6d  be imported from
-00011e50: 206a 7570 7974 6572 5f63 6f72 6520 7769   jupyter_core wi
-00011e60: 7468 2066 6978 2066 6f72 0a20 2065 7874  th fix for.  ext
-00011e70: 656e 6465 6420 7573 6572 6e61 6d65 7320  ended usernames 
-00011e80: 696e 2057 696e 646f 7773 205b 2334 3833  in Windows [#483
-00011e90: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00011ea0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00011eb0: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00011ec0: 2f34 3833 292e 0a0a 2323 2035 2e33 2e33  /483)...## 5.3.3
-00011ed0: 0a0a 2d20 4669 7865 6420 6973 7375 6520  ..- Fixed issue 
-00011ee0: 7769 7468 206e 6f6e 2d65 6e67 6c69 7368  with non-english
-00011ef0: 2077 696e 646f 7773 2070 6572 6d69 7373   windows permiss
-00011f00: 696f 6e73 0a20 205b 2334 3738 5d28 6874  ions.  [#478](ht
-00011f10: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00011f20: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00011f30: 5f63 6c69 656e 742f 7075 6c6c 2f34 3738  _client/pull/478
-00011f40: 292e 2050 6f74 656e 7469 616c 2069 7373  ). Potential iss
-00011f50: 7565 2073 7469 6c6c 206f 7065 6e0a 2020  ue still open.  
-00011f60: 696e 2075 7365 2077 6974 6820 6a75 7079  in use with jupy
-00011f70: 6572 6c61 622e 0a0a 2323 2035 2e33 2e32  erlab...## 5.3.2
-00011f80: 0a0a 2d20 496d 706f 7274 616e 7420 6669  ..- Important fi
-00011f90: 6c65 7320 6372 6561 7469 6f6e 206e 6f77  les creation now
-00011fa0: 2063 6865 636b 7320 756d 6173 6b20 7065   checks umask pe
-00011fb0: 726d 6973 7369 6f6e 730a 2020 5b23 3436  rmissions.  [#46
-00011fc0: 395d 2868 7474 7073 3a2f 2f67 6974 6875  9](https://githu
-00011fd0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-00011fe0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-00011ff0: 6c2f 3436 3929 2e0a 0a23 2320 352e 332e  l/469)...## 5.3.
-00012000: 310a 0a2d 2046 6978 2062 7567 2077 6974  1..- Fix bug wit
-00012010: 6820 636f 6e74 726f 6c20 6368 616e 6e65  h control channe
-00012020: 6c20 736f 636b 6574 2069 6e74 726f 6475  l socket introdu
-00012030: 6365 6420 696e 2035 2e33 2e30 0a20 205b  ced in 5.3.0.  [
-00012040: 2334 3536 5d28 6874 7470 733a 2f2f 6769  #456](https://gi
-00012050: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-00012060: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-00012070: 7075 6c6c 2f34 3536 292e 0a0a 2323 2035  pull/456)...## 5
-00012080: 2e33 2e30 0a0a 5b35 2e33 2e30 206f 6e0a  .3.0..[5.3.0 on.
-00012090: 4769 7448 7562 5d28 6874 7470 733a 2f2f  GitHub](https://
-000120a0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-000120b0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-000120c0: 742f 6d69 6c65 7374 6f6e 6573 2f35 2e33  t/milestones/5.3
-000120d0: 2e30 290a 0a4e 6577 2046 6561 7475 7265  .0)..New Feature
-000120e0: 733a 0a0a 2d20 4d75 6c74 6970 726f 6365  s:..- Multiproce
-000120f0: 7373 696e 6720 616e 6420 5468 7265 6164  ssing and Thread
-00012100: 696e 6720 7375 7070 6f72 7420 5b23 3433  ing support [#43
-00012110: 375d 2868 7474 7073 3a2f 2f67 6974 6875  7](https://githu
-00012120: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-00012130: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-00012140: 6c2f 3433 3729 2061 6e64 205b 2334 3530  l/437) and [#450
-00012150: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00012160: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
-00012170: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
-00012180: 2f34 3530 290a 2d20 5365 7475 7020 7061  /450).- Setup pa
-00012190: 636b 6167 6520 6c6f 6e67 5f64 6573 6372  ckage long_descr
-000121a0: 6970 7469 6f6e 205b 2334 3131 5d28 6874  iption [#411](ht
-000121b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000121c0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-000121d0: 5f63 6c69 656e 742f 7075 6c6c 2f34 3131  _client/pull/411
-000121e0: 290a 0a43 6861 6e67 6573 3a0a 0a2d 2043  )..Changes:..- C
-000121f0: 6f6e 7472 6f6c 2063 6861 6e6e 656c 206e  ontrol channel n
-00012200: 6f77 2069 6e20 7468 6520 7075 626c 6963  ow in the public
-00012210: 2041 5049 205b 2334 3437 5d28 6874 7470   API [#447](http
-00012220: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00012230: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00012240: 6c69 656e 742f 7075 6c6c 2f34 3437 290a  lient/pull/447).
-00012250: 2d20 436c 6f73 696e 6720 4a75 7079 7465  - Closing Jupyte
-00012260: 7220 436c 6965 6e74 2069 7320 6e6f 7720  r Client is now 
-00012270: 6661 7374 6572 205b 2334 3230 5d28 6874  faster [#420](ht
-00012280: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00012290: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-000122a0: 5f63 6c69 656e 742f 7075 6c6c 2f34 3230  _client/pull/420
-000122b0: 290a 2d20 5069 7020 7375 7070 6f72 7420  ).- Pip support 
-000122c0: 696d 7072 6f76 656d 656e 7473 205b 2334  improvements [#4
-000122d0: 3231 5d28 6874 7470 733a 2f2f 6769 7468  21](https://gith
-000122e0: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-000122f0: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-00012300: 6c6c 2f34 3231 290a 0a42 7265 616b 696e  ll/421)..Breakin
-00012310: 6720 6368 616e 6765 733a 0a0a 2d20 4472  g changes:..- Dr
-00012320: 6f70 7065 6420 7375 7070 6f72 7420 666f  opped support fo
-00012330: 7220 5079 7468 6f6e 2033 2e33 2061 6e64  r Python 3.3 and
-00012340: 2033 2e34 2028 7570 7374 7265 616d 2070   3.4 (upstream p
-00012350: 6163 6b61 6765 7320 6472 6f70 7065 640a  ackages dropped.
-00012360: 2020 7375 7070 6f72 7420 616c 7265 6164    support alread
-00012370: 7929 0a0a 2323 2035 2e32 2e34 0a0a 5b35  y)..## 5.2.4..[5
-00012380: 2e32 2e34 206f 6e0a 4769 7448 7562 5d28  .2.4 on.GitHub](
-00012390: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000123a0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-000123b0: 6572 5f63 6c69 656e 742f 6d69 6c65 7374  er_client/milest
-000123c0: 6f6e 6573 2f35 2e32 2e34 290a 0a2d 2050  ones/5.2.4)..- P
-000123d0: 7265 7665 6e74 2063 7265 6174 696e 6720  revent creating 
-000123e0: 6e65 7720 636f 6e73 6f6c 6520 7769 6e64  new console wind
-000123f0: 6f77 7320 6f6e 2057 696e 646f 7773 0a20  ows on Windows. 
-00012400: 205b 2333 3436 5d28 6874 7470 733a 2f2f   [#346](https://
-00012410: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00012420: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00012430: 742f 7075 6c6c 2f33 3436 290a 2d20 4669  t/pull/346).- Fi
-00012440: 7820 696e 7465 7272 7570 7473 206f 6e20  x interrupts on 
-00012450: 5079 7468 6f6e 2033 2e37 206f 6e20 5769  Python 3.7 on Wi
-00012460: 6e64 6f77 7320 5b23 3430 385d 2868 7474  ndows [#408](htt
-00012470: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00012480: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00012490: 636c 6965 6e74 2f70 756c 6c2f 3430 3829  client/pull/408)
-000124a0: 0a0a 2323 2035 2e32 2e33 0a0a 5b35 2e32  ..## 5.2.3..[5.2
-000124b0: 2e33 206f 6e0a 4769 7448 7562 5d28 6874  .3 on.GitHub](ht
-000124c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000124d0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-000124e0: 5f63 6c69 656e 742f 6d69 6c65 7374 6f6e  _client/mileston
-000124f0: 6573 2f35 2e32 2e33 290a 0a2d 2046 6978  es/5.2.3)..- Fix
-00012500: 2068 616e 6720 6f6e 2063 6c6f 7365 2069   hang on close i
-00012510: 6e20 602e 5468 7265 6164 6564 4b65 726e  n `.ThreadedKern
-00012520: 656c 436c 6965 6e74 6020 2875 7365 6420  elClient` (used 
-00012530: 696e 2051 7443 6f6e 736f 6c65 2920 7768  in QtConsole) wh
-00012540: 656e 2075 7369 6e67 2074 6f72 6e61 646f  en using tornado
-00012550: 2077 6974 6820 6173 796e 6369 6f0a 2020   with asyncio.  
-00012560: 2864 6566 6175 6c74 2062 6568 6176 696f  (default behavio
-00012570: 7220 6f66 2074 6f72 6e61 646f 2035 2c20  r of tornado 5, 
-00012580: 7365 6520 5b23 3335 325d 2868 7474 7073  see [#352](https
-00012590: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-000125a0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-000125b0: 6965 6e74 2f70 756c 6c2f 3335 3229 292e  ient/pull/352)).
-000125c0: 0a2d 2046 6978 2065 7272 6f72 7320 7768  .- Fix errors wh
-000125d0: 656e 2075 7369 6e67 2064 6570 7265 6361  en using depreca
-000125e0: 7465 640a 2020 602e 4b65 726e 656c 4d61  ted.  `.KernelMa
-000125f0: 6e61 6765 722e 6b65 726e 656c 5f63 6d64  nager.kernel_cmd
-00012600: 600a 2020 285b 2333 3433 5d28 6874 7470  `.  ([#343](http
-00012610: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00012620: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
-00012630: 6c69 656e 742f 7075 6c6c 2f33 3433 292c  lient/pull/343),
-00012640: 205b 2333 3434 5d28 6874 7470 733a 2f2f   [#344](https://
-00012650: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
-00012660: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
-00012670: 742f 7075 6c6c 2f33 3434 2929 2e0a 0a23  t/pull/344))...#
-00012680: 2320 352e 322e 320a 0a5b 352e 322e 3220  # 5.2.2..[5.2.2 
-00012690: 6f6e 0a47 6974 4875 625d 2868 7474 7073  on.GitHub](https
-000126a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-000126b0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-000126c0: 6965 6e74 2f6d 696c 6573 746f 6e65 732f  ient/milestones/
-000126d0: 352e 322e 3229 0a0a 2d20 4669 7820 602e  5.2.2)..- Fix `.
-000126e0: 4b65 726e 656c 5370 6563 4d61 6e61 6765  KernelSpecManage
-000126f0: 722e 6765 745f 616c 6c5f 7370 6563 7360  r.get_all_specs`
-00012700: 206d 6574 686f 6420 696e 2073 7562 636c   method in subcl
-00012710: 6173 7365 7320 7468 6174 206f 6e6c 7920  asses that only 
-00012720: 6f76 6572 7269 6465 0a20 2060 2e4b 6572  override.  `.Ker
-00012730: 6e65 6c53 7065 634d 616e 6167 6572 2e66  nelSpecManager.f
-00012740: 696e 645f 6b65 726e 656c 5f73 7065 6373  ind_kernel_specs
-00012750: 6020 616e 640a 2020 602e 4b65 726e 656c  ` and.  `.Kernel
-00012760: 5370 6563 4d61 6e61 6765 722e 6765 745f  SpecManager.get_
-00012770: 6b65 726e 656c 5f73 7065 6360 2e0a 2020  kernel_spec`..  
-00012780: 5365 6520 5b23 3333 385d 2868 7474 7073  See [#338](https
-00012790: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-000127a0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-000127b0: 6965 6e74 2f69 7373 7565 732f 3333 3829  ient/issues/338)
-000127c0: 2061 6e64 0a20 205b 2333 3339 5d28 6874   and.  [#339](ht
-000127d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000127e0: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-000127f0: 5f63 6c69 656e 742f 7075 6c6c 2f33 3339  _client/pull/339
-00012800: 292e 0a2d 2045 6c69 6d69 6e61 7465 206f  )..- Eliminate o
-00012810: 6363 6173 696f 6e61 6c20 6572 726f 7220  ccasional error 
-00012820: 6d65 7373 6167 6573 2064 7572 696e 6720  messages during 
-00012830: 7072 6f63 6573 7320 6578 6974 0a20 205b  process exit.  [
-00012840: 2333 3336 5d28 6874 7470 733a 2f2f 6769  #336](https://gi
-00012850: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-00012860: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-00012870: 7075 6c6c 2f33 3336 292e 0a2d 2049 6d70  pull/336)..- Imp
-00012880: 726f 7665 2065 7272 6f72 206d 6573 7361  rove error messa
-00012890: 6765 2077 6865 6e20 6174 7465 6d70 7469  ge when attempti
-000128a0: 6e67 2074 6f20 6269 6e64 206f 6e20 696e  ng to bind on in
-000128b0: 7661 6c69 6420 6164 6472 6573 730a 2020  valid address.  
-000128c0: 5b23 3333 305d 2868 7474 7073 3a2f 2f67  [#330](https://g
-000128d0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
-000128e0: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
-000128f0: 2f70 756c 6c2f 3333 3029 2e0a 2d20 4164  /pull/330)..- Ad
-00012900: 6420 6d69 7373 696e 6720 6469 7265 6374  d missing direct
-00012910: 2064 6570 656e 6465 6e63 7920 6f6e 2074   dependency on t
-00012920: 6f72 6e61 646f 205b 2333 3233 5d28 6874  ornado [#323](ht
-00012930: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00012940: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00012950: 5f63 6c69 656e 742f 7075 6c6c 2f33 3233  _client/pull/323
-00012960: 292e 0a0a 2323 2035 2e32 2e31 0a0a 5b35  )...## 5.2.1..[5
-00012970: 2e32 2e31 206f 6e0a 4769 7448 7562 5d28  .2.1 on.GitHub](
-00012980: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00012990: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-000129a0: 6572 5f63 6c69 656e 742f 6d69 6c65 7374  er_client/milest
-000129b0: 6f6e 6573 2f35 2e32 2e31 290a 0a2d 2041  ones/5.2.1)..- A
-000129c0: 6464 2070 6172 656e 7468 6573 6973 2074  dd parenthesis t
-000129d0: 6f20 636f 6e64 6974 696f 6e61 6c20 7079  o conditional py
-000129e0: 7465 7374 2072 6571 7569 7265 6d65 6e74  test requirement
-000129f0: 2074 6f20 776f 726b 2061 726f 756e 6420   to work around 
-00012a00: 610a 2020 6275 6720 696e 2074 6865 2060  a.  bug in the `
-00012a10: 7768 6565 6c60 2070 6163 6b61 6765 2c20  wheel` package, 
-00012a20: 7468 6174 2067 656e 6572 6174 6520 6120  that generate a 
-00012a30: 602e 7768 6c60 2077 6869 6368 206f 7468  `.whl` which oth
-00012a40: 6572 7769 7365 0a20 2061 6c77 6179 7320  erwise.  always 
-00012a50: 6465 7065 6e64 7320 6f6e 2060 7079 7465  depends on `pyte
-00012a60: 7374 6020 7365 6520 5b23 3332 345d 2868  st` see [#324](h
-00012a70: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00012a80: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00012a90: 725f 636c 6965 6e74 2f69 7373 7565 732f  r_client/issues/
-00012aa0: 3332 3429 616e 6420 5b23 3332 355d 2868  324)and [#325](h
-00012ab0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00012ac0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00012ad0: 725f 636c 6965 6e74 2f70 756c 6c2f 3332  r_client/pull/32
-00012ae0: 3529 2e0a 0a23 2320 352e 320a 0a5b 352e  5)...## 5.2..[5.
-00012af0: 3220 6f6e 0a47 6974 4875 625d 2868 7474  2 on.GitHub](htt
-00012b00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00012b10: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00012b20: 636c 6965 6e74 2f6d 696c 6573 746f 6e65  client/milestone
-00012b30: 732f 352e 3229 0a0a 2d20 4465 6669 6e65  s/5.2)..- Define
-00012b40: 204a 7570 7974 6572 2070 726f 746f 636f   Jupyter protoco
-00012b50: 6c20 7665 7273 696f 6e20 352e 333a 0a20  l version 5.3:. 
-00012b60: 202d 204b 6572 6e65 6c73 2063 616e 206e   - Kernels can n
-00012b70: 6f77 206f 7074 2074 6f20 6265 2069 6e74  ow opt to be int
-00012b80: 6572 7275 7074 6564 2062 7920 6120 6d65  errupted by a me
-00012b90: 7373 6167 6520 7365 6e74 206f 6e20 7468  ssage sent on th
-00012ba0: 650a 2020 2020 636f 6e74 726f 6c20 6368  e.    control ch
-00012bb0: 616e 6e65 6c20 696e 7374 6561 6420 6f66  annel instead of
-00012bc0: 2061 2073 7973 7465 6d20 7369 676e 616c   a system signal
-00012bd0: 2e20 5365 650a 2020 2020 606b 6572 6e65  . See.    `kerne
-00012be0: 6c73 7065 6373 6020 616e 640a 2020 2020  lspecs` and.    
-00012bf0: 606d 7367 696e 675f 696e 7465 7272 7570  `msging_interrup
-00012c00: 7460 0a20 2020 205b 2332 3934 5d28 6874  t`.    [#294](ht
-00012c10: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00012c20: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00012c30: 5f63 6c69 656e 742f 7075 6c6c 2f32 3934  _client/pull/294
-00012c40: 292e 0a2d 204e 6577 2060 6a75 7079 7465  )..- New `jupyte
-00012c50: 7220 6b65 726e 656c 6020 636f 6d6d 616e  r kernel` comman
-00012c60: 6420 746f 206c 6175 6e63 6820 616e 2069  d to launch an i
-00012c70: 6e73 7461 6c6c 6564 206b 6572 6e65 6c20  nstalled kernel 
-00012c80: 6279 206e 616d 650a 2020 5b23 3234 305d  by name.  [#240]
-00012c90: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00012ca0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
-00012cb0: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
-00012cc0: 3234 3029 2e0a 2d20 4b65 726e 656c 7370  240)..- Kernelsp
-00012cd0: 6563 7320 7768 6572 6520 7468 6520 636f  ecs where the co
-00012ce0: 6d6d 616e 6420 7374 6172 7473 2077 6974  mmand starts wit
-00012cf0: 6820 652e 672e 2060 7079 7468 6f6e 3360  h e.g. `python3`
-00012d00: 206f 720a 2020 6070 7974 686f 6e33 2e36   or.  `python3.6
-00012d10: 602d 2d2d 6d61 7463 6869 6e67 2074 6865  `---matching the
-00012d20: 2076 6572 7369 6f6e 2060 6a75 7079 7465   version `jupyte
-00012d30: 725f 636c 6965 6e74 6020 6973 2072 756e  r_client` is run
-00012d40: 6e69 6e67 0a20 206f 6e2d 2d2d 6172 6520  ning.  on---are 
-00012d50: 6e6f 7720 6c61 756e 6368 6564 2077 6974  now launched wit
-00012d60: 6820 7468 6520 7361 6d65 2050 7974 686f  h the same Pytho
-00012d70: 6e20 6578 6563 7574 6162 6c65 2061 7320  n executable as 
-00012d80: 7468 650a 2020 6c61 756e 6368 696e 6720  the.  launching 
-00012d90: 7072 6f63 6573 7320 5b23 3330 365d 2868  process [#306](h
-00012da0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00012db0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
-00012dc0: 725f 636c 6965 6e74 2f70 756c 6c2f 3330  r_client/pull/30
-00012dd0: 3629 2e20 5468 6973 0a20 2065 7874 656e  6). This.  exten
-00012de0: 6473 2074 6865 2073 7065 6369 616c 2068  ds the special h
-00012df0: 616e 646c 696e 6720 6f66 2060 7079 7468  andling of `pyth
-00012e00: 6f6e 6020 6164 6465 6420 696e 2035 2e30  on` added in 5.0
-00012e10: 2e0a 2d20 436f 6d6d 616e 6420 6c69 6e65  ..- Command line
-00012e20: 2061 7267 756d 656e 7473 2073 7065 6369   arguments speci
-00012e30: 6669 6564 2062 7920 6120 6b65 726e 656c  fied by a kernel
-00012e40: 7370 6563 2063 616e 206e 6f77 2069 6e63  spec can now inc
-00012e50: 6c75 6465 0a20 2060 7b72 6573 6f75 7263  lude.  `{resourc
-00012e60: 655f 6469 727d 602c 2077 6869 6368 2077  e_dir}`, which w
-00012e70: 696c 6c20 6265 2073 7562 7374 6974 7574  ill be substitut
-00012e80: 6564 2077 6974 6820 7468 6520 6b65 726e  ed with the kern
-00012e90: 656c 7370 6563 0a20 2072 6573 6f75 7263  elspec.  resourc
-00012ea0: 6520 6469 7265 6374 6f72 7920 7061 7468  e directory path
-00012eb0: 2077 6865 6e20 7468 6520 6b65 726e 656c   when the kernel
-00012ec0: 2069 7320 6c61 756e 6368 6564 0a20 205b   is launched.  [
-00012ed0: 2332 3839 5d28 6874 7470 733a 2f2f 6769  #289](https://gi
-00012ee0: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
-00012ef0: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
-00012f00: 7075 6c6c 2f32 3839 292e 0a2d 204b 6572  pull/289)..- Ker
-00012f10: 6e65 6c73 7065 6373 206e 6f77 2068 6176  nelspecs now hav
-00012f20: 6520 616e 206f 7074 696f 6e61 6c20 606d  e an optional `m
-00012f30: 6574 6164 6174 6160 2066 6965 6c64 2074  etadata` field t
-00012f40: 6f20 686f 6c64 2061 7262 6974 7261 7279  o hold arbitrary
-00012f50: 0a20 206d 6574 6164 6174 6120 6162 6f75  .  metadata abou
-00012f60: 7420 6b65 726e 656c 732d 2d2d 7365 6520  t kernels---see 
-00012f70: 606b 6572 6e65 6c73 7065 6373 6020 5b23  `kernelspecs` [#
-00012f80: 3237 345d 2868 7474 7073 3a2f 2f67 6974  274](https://git
-00012f90: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-00012fa0: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-00012fb0: 756c 6c2f 3237 3429 2e0a 2d20 4d61 6b65  ull/274)..- Make
-00012fc0: 2074 6865 2060 4b65 726e 656c 5265 7374   the `KernelRest
-00012fd0: 6172 7465 7260 2063 6c61 7373 2075 7365  arter` class use
-00012fe0: 6420 6279 2061 2060 4b65 726e 656c 4d61  d by a `KernelMa
-00012ff0: 6e61 6765 7260 0a20 2063 6f6e 6669 6775  nager`.  configu
-00013000: 7261 626c 6520 5b23 3239 305d 2868 7474  rable [#290](htt
-00013010: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00013020: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00013030: 636c 6965 6e74 2f70 756c 6c2f 3239 3029  client/pull/290)
-00013040: 2e0a 2d20 5768 656e 206b 696c 6c69 6e67  ..- When killing
-00013050: 2061 206b 6572 6e65 6c20 6f6e 2055 6e69   a kernel on Uni
-00013060: 782c 206b 696c 6c20 6974 7320 7072 6f63  x, kill its proc
-00013070: 6573 7320 6772 6f75 700a 2020 5b23 3331  ess group.  [#31
-00013080: 345d 2868 7474 7073 3a2f 2f67 6974 6875  4](https://githu
-00013090: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
-000130a0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
-000130b0: 6c2f 3331 3429 2e0a 2d20 4966 2061 206b  l/314)..- If a k
-000130c0: 6572 6e65 6c20 6469 6573 2073 6f6f 6e20  ernel dies soon 
-000130d0: 6166 7465 7220 7374 6172 7469 6e67 2c20  after starting, 
-000130e0: 7265 6173 7369 676e 2072 616e 646f 6d20  reassign random 
-000130f0: 706f 7274 7320 6265 666f 7265 0a20 2072  ports before.  r
-00013100: 6573 7461 7274 696e 6720 6974 2c20 696e  estarting it, in
-00013110: 2063 6173 6520 6f6e 6520 6f66 2074 6865   case one of the
-00013120: 2070 7265 7669 6f75 736c 7920 6368 6f73   previously chos
-00013130: 656e 2070 6f72 7473 2068 6173 2062 6565  en ports has bee
-00013140: 6e0a 2020 626f 756e 6420 6279 2061 6e6f  n.  bound by ano
-00013150: 7468 6572 2070 726f 6365 7373 205b 2332  ther process [#2
-00013160: 3739 5d28 6874 7470 733a 2f2f 6769 7468  79](https://gith
-00013170: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00013180: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-00013190: 6c6c 2f32 3739 292e 0a2d 2041 766f 6964  ll/279)..- Avoid
-000131a0: 2075 6e6e 6563 6573 7361 7279 2066 696c   unnecessary fil
-000131b0: 6573 7973 7465 6d20 6f70 6572 6174 696f  esystem operatio
-000131c0: 6e73 2077 6865 6e20 6669 6e64 696e 6720  ns when finding 
-000131d0: 6120 6b65 726e 656c 7370 6563 0a20 2077  a kernelspec.  w
-000131e0: 6974 6820 602e 4b65 726e 656c 5370 6563  ith `.KernelSpec
-000131f0: 4d61 6e61 6765 722e 6765 745f 6b65 726e  Manager.get_kern
-00013200: 656c 5f73 7065 6360 205b 2333 3131 5d28  el_spec` [#311](
-00013210: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00013220: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-00013230: 6572 5f63 6c69 656e 742f 7075 6c6c 2f33  er_client/pull/3
-00013240: 3131 292e 0a2d 2060 2e4b 6572 6e65 6c53  11)..- `.KernelS
-00013250: 7065 634d 616e 6167 6572 2e67 6574 5f61  pecManager.get_a
-00013260: 6c6c 5f73 7065 6373 600a 2020 7769 6c6c  ll_specs`.  will
-00013270: 206e 6f20 6c6f 6e67 6572 2072 6169 7365   no longer raise
-00013280: 2061 6e20 6578 6365 7074 696f 6e20 6f6e   an exception on
-00013290: 2065 6e63 6f75 6e74 6572 696e 6720 616e   encountering an
-000132a0: 2069 6e76 616c 6964 0a20 2060 6b65 726e   invalid.  `kern
-000132b0: 656c 2e6a 736f 6e60 2066 696c 652e 2049  el.json` file. I
-000132c0: 7420 7769 6c6c 2072 6169 7365 2061 2077  t will raise a w
-000132d0: 6172 6e69 6e67 2061 6e64 2063 6f6e 7469  arning and conti
-000132e0: 6e75 650a 2020 5b23 3331 305d 2868 7474  nue.  [#310](htt
-000132f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00013300: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
-00013310: 636c 6965 6e74 2f70 756c 6c2f 3331 3029  client/pull/310)
-00013320: 2e0a 2d20 4368 6563 6b20 666f 7220 6e6f  ..- Check for no
-00013330: 6e2d 636f 6e74 6967 756f 7573 2062 7566  n-contiguous buf
-00013340: 6665 7273 2062 6566 6f72 6520 7472 7969  fers before tryi
-00013350: 6e67 2074 6f20 7365 6e64 2074 6865 6d20  ng to send them 
-00013360: 7468 726f 7567 680a 2020 5a4d 5120 5b23  through.  ZMQ [#
-00013370: 3235 385d 2868 7474 7073 3a2f 2f67 6974  258](https://git
-00013380: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-00013390: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-000133a0: 756c 6c2f 3235 3829 2e0a 2d20 436f 6d70  ull/258)..- Comp
-000133b0: 6174 6962 696c 6974 7920 7769 7468 2075  atibility with u
-000133c0: 7063 6f6d 696e 6720 546f 726e 6164 6f20  pcoming Tornado 
-000133d0: 7665 7273 696f 6e20 352e 300a 2020 5b23  version 5.0.  [#
-000133e0: 3330 345d 2868 7474 7073 3a2f 2f67 6974  304](https://git
-000133f0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-00013400: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
-00013410: 756c 6c2f 3330 3429 2e0a 2d20 5369 6d70  ull/304)..- Simp
-00013420: 6c69 6679 2073 6574 7570 2063 6f64 6520  lify setup code 
-00013430: 6279 2061 6c77 6179 7320 7573 696e 6720  by always using 
-00013440: 7365 7475 7074 6f6f 6c73 0a20 205b 2332  setuptools.  [#2
-00013450: 3834 5d28 6874 7470 733a 2f2f 6769 7468  84](https://gith
-00013460: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
-00013470: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
-00013480: 6c6c 2f32 3834 292e 0a2d 2053 6f66 7465  ll/284)..- Softe
-00013490: 6e20 7761 726e 696e 6773 2077 6865 6e20  n warnings when 
-000134a0: 7365 7474 696e 6720 7468 6520 7374 6963  setting the stic
-000134b0: 6b79 2062 6974 206f 6e20 7275 6e74 696d  ky bit on runtim
-000134c0: 6520 6669 6c65 7320 6661 696c 730a 2020  e files fails.  
-000134d0: 5b23 3238 365d 2868 7474 7073 3a2f 2f67  [#286](https://g
-000134e0: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
-000134f0: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
-00013500: 2f70 756c 6c2f 3238 3629 2e0a 2d20 5661  /pull/286)..- Va
-00013510: 7269 6f75 7320 636f 7272 6563 7469 6f6e  rious correction
-00013520: 7320 616e 6420 696d 7072 6f76 656d 656e  s and improvemen
-00013530: 7473 2074 6f20 646f 6375 6d65 6e74 6174  ts to documentat
-00013540: 696f 6e2e 0a0a 2323 2035 2e31 0a0a 5b35  ion...## 5.1..[5
-00013550: 2e31 206f 6e0a 4769 7448 7562 5d28 6874  .1 on.GitHub](ht
-00013560: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00013570: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
-00013580: 5f63 6c69 656e 742f 6d69 6c65 7374 6f6e  _client/mileston
-00013590: 6573 2f35 2e31 290a 0a2d 2044 6566 696e  es/5.1)..- Defin
-000135a0: 6520 4a75 7079 7465 7220 7072 6f74 6f63  e Jupyter protoc
-000135b0: 6f6c 2076 6572 7369 6f6e 2035 2e32 2c20  ol version 5.2, 
-000135c0: 7265 736f 6c76 696e 6720 616d 6269 6775  resolving ambigu
-000135d0: 6974 7920 6f66 0a20 2060 6375 7273 6f72  ity of.  `cursor
-000135e0: 5f70 6f73 6020 6669 656c 6420 696e 2074  _pos` field in t
-000135f0: 6865 2070 7265 7365 6e63 6520 6f66 2075  he presence of u
-00013600: 6e69 636f 6465 2073 7572 726f 6761 7465  nicode surrogate
-00013610: 2070 6169 7273 2e0a 0a20 203a 3a3a 207b   pairs...  ::: {
-00013620: 2e73 6565 616c 736f 7d0a 2020 6063 7572  .seealso}.  `cur
-00013630: 736f 725f 706f 735f 756e 6963 6f64 655f  sor_pos_unicode_
-00013640: 6e6f 7465 600a 2020 3a3a 3a0a 0a2d 2041  note`.  :::..- A
-00013650: 6464 2060 5365 7373 696f 6e2e 636c 6f6e  dd `Session.clon
-00013660: 6560 2066 6f72 206d 616b 696e 6720 6120  e` for making a 
-00013670: 636f 7079 0a20 206f 6620 6120 5365 7373  copy.  of a Sess
-00013680: 696f 6e20 6f62 6a65 6374 2077 6974 686f  ion object witho
-00013690: 7574 2073 6861 7269 6e67 2074 6865 2064  ut sharing the d
-000136a0: 6967 6573 7420 6869 7374 6f72 792e 2052  igest history. R
-000136b0: 6575 7369 6e67 2061 0a20 2073 696e 676c  eusing a.  singl
-000136c0: 6520 5365 7373 696f 6e20 6f62 6a65 6374  e Session object
-000136d0: 2074 6f20 636f 6e6e 6563 7420 6d75 6c74   to connect mult
-000136e0: 6970 6c65 2073 6f63 6b65 7473 2074 6f20  iple sockets to 
-000136f0: 7468 6520 7361 6d65 2049 4f50 7562 0a20  the same IOPub. 
-00013700: 2070 6565 7220 6361 6e20 6361 7573 6520   peer can cause 
-00013710: 6469 6765 7374 2063 6f6c 6c69 7369 6f6e  digest collision
-00013720: 732e 0a0a 2d20 4176 6f69 6420 676c 6f62  s...- Avoid glob
-00013730: 616c 2072 6566 6572 656e 6365 7320 7072  al references pr
-00013740: 6576 656e 7469 6e67 2067 6172 6261 6765  eventing garbage
-00013750: 2063 6f6c 6c65 6374 696f 6e20 6f66 2062   collection of b
-00013760: 6163 6b67 726f 756e 640a 2020 7468 7265  ackground.  thre
-00013770: 6164 732e 0a0a 2323 2035 2e30 0a0a 2323  ads...## 5.0..##
-00013780: 2320 352e 302e 310a 0a5b 352e 302e 3120  # 5.0.1..[5.0.1 
-00013790: 6f6e 0a47 6974 4875 625d 2868 7474 7073  on.GitHub](https
-000137a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-000137b0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-000137c0: 6965 6e74 2f6d 696c 6573 746f 6e65 732f  ient/milestones/
-000137d0: 352e 302e 3129 0a0a 2d20 5570 6461 7465  5.0.1)..- Update
-000137e0: 2069 6e74 6572 6e61 6c20 7072 6f74 6f63   internal protoc
-000137f0: 6f6c 2076 6572 7369 6f6e 206e 756d 6265  ol version numbe
-00013800: 7220 746f 2035 2e31 2c20 7768 6963 6820  r to 5.1, which 
-00013810: 7368 6f75 6c64 2068 6176 650a 2020 6265  should have.  be
-00013820: 656e 2064 6f6e 6520 696e 2035 2e30 2e30  en done in 5.0.0
-00013830: 2e0a 0a23 2323 2035 2e30 2e30 0a0a 5b35  ...### 5.0.0..[5
-00013840: 2e30 2e30 206f 6e0a 4769 7448 7562 5d28  .0.0 on.GitHub](
-00013850: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00013860: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-00013870: 6572 5f63 6c69 656e 742f 6d69 6c65 7374  er_client/milest
-00013880: 6f6e 6573 2f35 2e30 290a 0a4e 6577 2066  ones/5.0)..New f
-00013890: 6561 7475 7265 733a 0a0a 2d20 496d 706c  eatures:..- Impl
-000138a0: 656d 656e 7420 4a75 7079 7465 7220 7072  ement Jupyter pr
-000138b0: 6f74 6f63 6f6c 2076 6572 7369 6f6e 2035  otocol version 5
-000138c0: 2e31 2e0a 0a2d 2049 6e74 726f 6475 6365  .1...- Introduce
-000138d0: 2060 6a75 7079 7465 7220 7275 6e60 2063   `jupyter run` c
-000138e0: 6f6d 6d61 6e64 0a20 2066 6f72 2072 756e  ommand.  for run
-000138f0: 6e69 6e67 2073 6372 6970 7473 2077 6974  ning scripts wit
-00013900: 6820 6120 6b65 726e 656c 2c20 666f 7220  h a kernel, for 
-00013910: 696e 7374 616e 6365 3a0a 0a20 2060 6060  instance:..  ```
-00013920: 0a20 206a 7570 7974 6572 2072 756e 202d  .  jupyter run -
-00013930: 2d6b 6572 6e65 6c20 7079 7468 6f6e 3320  -kernel python3 
-00013940: 6d79 7363 7269 7074 2e70 790a 2020 6060  myscript.py.  ``
-00013950: 600a 0a2d 204e 6577 206d 6574 686f 640a  `..- New method.
-00013960: 2020 602e 426c 6f63 6b69 6e67 4b65 726e    `.BlockingKern
-00013970: 656c 436c 6965 6e74 2e65 7865 6375 7465  elClient.execute
-00013980: 5f69 6e74 6572 6163 7469 7665 6020 666f  _interactive` fo
-00013990: 7220 7275 6e6e 696e 6720 636f 6465 2061  r running code a
-000139a0: 6e64 2063 6170 7475 7269 6e67 206f 7220  nd capturing or 
-000139b0: 7265 6469 7370 6c61 7969 6e67 2069 7473  redisplaying its
-000139c0: 0a20 206f 7574 7075 742e 0a0a 2d20 4e65  .  output...- Ne
-000139d0: 7720 604b 6572 6e65 6c4d 616e 6167 6572  w `KernelManager
-000139e0: 2e73 6875 7464 6f77 6e5f 7761 6974 5f74  .shutdown_wait_t
-000139f0: 696d 6560 2063 6f6e 6669 6775 7261 626c  ime` configurabl
-00013a00: 6520 666f 7220 6164 6a75 7374 696e 670a  e for adjusting.
-00013a10: 2020 7468 6520 7469 6d65 2066 6f72 2061    the time for a
-00013a20: 206b 6572 6e65 6c20 6d61 6e61 6765 7220   kernel manager 
-00013a30: 746f 2077 6169 7420 6166 7465 7220 706f  to wait after po
-00013a40: 6c69 7465 6c79 2072 6571 7565 7374 696e  litely requestin
-00013a50: 670a 2020 7368 7574 646f 776e 2062 6566  g.  shutdown bef
-00013a60: 6f72 6520 6974 2072 6573 6f72 7473 2074  ore it resorts t
-00013a70: 6f20 666f 7263 6566 756c 2074 6572 6d69  o forceful termi
-00013a80: 6e61 7469 6f6e 2e0a 0a46 6978 6573 3a0a  nation...Fixes:.
-00013a90: 0a2d 2053 6574 2073 7469 636b 7920 6269  .- Set sticky bi
-00013aa0: 7420 6f6e 2063 6f6e 6e65 6374 696f 6e2d  t on connection-
-00013ab0: 6669 6c65 2064 6972 6563 746f 7279 2074  file directory t
-00013ac0: 6f20 6176 6f69 6420 6765 7474 696e 6720  o avoid getting 
-00013ad0: 636c 6561 6e65 640a 2020 7570 2e0a 2d20  cleaned.  up..- 
-00013ae0: 606a 7570 7974 6572 5f63 6c69 656e 742e  `jupyter_client.
-00013af0: 6c61 756e 6368 6572 2e6c 6175 6e63 685f  launcher.launch_
-00013b00: 6b65 726e 656c 6020 7061 7373 6573 2074  kernel` passes t
-00013b10: 6872 6f75 6768 2061 6464 6974 696f 6e61  hrough additiona
-00013b20: 6c20 6f70 7469 6f6e 7320 746f 2074 6865  l options to the
-00013b30: 2075 6e64 6572 6c79 696e 670a 2020 506f   underlying.  Po
-00013b40: 7065 6e2c 206d 6174 6368 696e 6720 604b  pen, matching `K
-00013b50: 6572 6e65 6c4d 616e 6167 6572 2e73 7461  ernelManager.sta
-00013b60: 7274 5f6b 6572 6e65 6c60 2e0a 2d20 4368  rt_kernel`..- Ch
-00013b70: 6563 6b20 7479 7065 7320 6f66 2060 6275  eck types of `bu
-00013b80: 6666 6572 7360 2061 7267 756d 656e 7420  ffers` argument 
-00013b90: 696e 0a20 2060 2e53 6573 7369 6f6e 2e73  in.  `.Session.s
-00013ba0: 656e 6460 2c20 736f 2074 6861 7420 5479  end`, so that Ty
-00013bb0: 7065 4572 726f 7273 0a20 2061 7265 2072  peErrors.  are r
-00013bc0: 6169 7365 6420 696d 6d65 6469 6174 656c  aised immediatel
-00013bd0: 792c 2072 6174 6865 7220 7468 616e 2069  y, rather than i
-00013be0: 6e20 7468 6520 6576 656e 746c 6f6f 702e  n the eventloop.
-00013bf0: 0a0a 4368 616e 6765 733a 0a0a 2d20 496e  ..Changes:..- In
-00013c00: 206b 6572 6e65 6c73 7065 6373 2c20 6966   kernelspecs, if
-00013c10: 2074 6865 2065 7865 6375 7461 626c 6520   the executable 
-00013c20: 6973 2074 6865 2073 7472 696e 6720 6070  is the string `p
-00013c30: 7974 686f 6e60 2028 6173 206f 7070 6f73  ython` (as oppos
-00013c40: 6564 0a20 2074 6f20 616e 2061 6273 6f6c  ed.  to an absol
-00013c50: 7574 6520 7061 7468 292c 2060 7379 732e  ute path), `sys.
-00013c60: 6578 6563 7574 6162 6c65 6020 7769 6c6c  executable` will
-00013c70: 2062 6520 7573 6564 2072 6174 6865 7220   be used rather 
-00013c80: 7468 616e 0a20 2072 6573 6f6c 7669 6e67  than.  resolving
-00013c90: 2060 7079 7468 6f6e 6020 6f6e 2050 4154   `python` on PAT
-00013ca0: 482e 2054 6869 7320 7368 6f75 6c64 2065  H. This should e
-00013cb0: 6e61 626c 6520 5079 7468 6f6e 2d62 6173  nable Python-bas
-00013cc0: 6564 206b 6572 6e65 6c73 0a20 2074 6f20  ed kernels.  to 
-00013cd0: 696e 7374 616c 6c20 6b65 726e 656c 7370  install kernelsp
-00013ce0: 6563 7320 6173 2070 6172 7420 6f66 2077  ecs as part of w
-00013cf0: 6865 656c 732e 0a2d 206b 6572 6e65 6c73  heels..- kernels
-00013d00: 7065 6320 6e61 6d65 7320 6172 6520 6e6f  pec names are no
-00013d10: 7720 7661 6c69 6461 7465 642e 2054 6865  w validated. The
-00013d20: 7920 7368 6f75 6c64 206f 6e6c 7920 696e  y should only in
-00013d30: 636c 7564 6520 6173 6369 690a 2020 6c65  clude ascii.  le
-00013d40: 7474 6572 7320 616e 6420 6e75 6d62 6572  tters and number
-00013d50: 732c 2070 6c75 7320 7065 7269 6f64 2c20  s, plus period, 
-00013d60: 6879 7068 656e 2c20 616e 6420 756e 6465  hyphen, and unde
-00013d70: 7273 636f 7265 2e0a 0a42 6163 6b77 6172  rscore...Backwar
-00013d80: 642d 696e 636f 6d70 6174 6962 6c65 2063  d-incompatible c
-00013d90: 6861 6e67 6573 3a0a 0a2d 203a 7079 602e  hanges:..- :py`.
-00013da0: 6461 7465 7469 6d65 6020 6f62 6a65 6374  datetime` object
-00013db0: 7320 7265 7475 726e 6564 2069 6e0a 2020  s returned in.  
-00013dc0: 7061 7273 6564 206d 6573 7361 6765 7320  parsed messages 
-00013dd0: 6172 6520 6e6f 7720 616c 7761 7973 2074  are now always t
-00013de0: 696d 657a 6f6e 652d 6177 6172 652e 2054  imezone-aware. T
-00013df0: 696d 6573 7461 6d70 7320 696e 0a20 206d  imestamps in.  m
-00013e00: 6573 7361 6765 7320 7769 7468 6f75 7420  essages without 
-00013e10: 7469 6d65 7a6f 6e65 2069 6e66 6f20 6172  timezone info ar
-00013e20: 6520 696e 7465 7270 7265 7465 6420 6173  e interpreted as
-00013e30: 2074 6865 206c 6f63 616c 0a20 2074 696d   the local.  tim
-00013e40: 657a 6f6e 652c 2061 7320 7468 6973 2077  ezone, as this w
-00013e50: 6173 2074 6865 2062 6568 6176 696f 7220  as the behavior 
-00013e60: 696e 2065 6172 6c69 6572 2076 6572 7369  in earlier versi
-00013e70: 6f6e 732e 0a0a 2323 2034 2e34 0a0a 2323  ons...## 4.4..##
-00013e80: 2320 342e 342e 300a 0a5b 342e 3420 6f6e  # 4.4.0..[4.4 on
-00013e90: 0a47 6974 4875 625d 2868 7474 7073 3a2f  .GitHub](https:/
-00013ea0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
-00013eb0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
-00013ec0: 6e74 2f6d 696c 6573 746f 6e65 732f 342e  nt/milestones/4.
-00013ed0: 3429 0a0a 2d20 4164 6420 602e 4b65 726e  4)..- Add `.Kern
-00013ee0: 656c 436c 6965 6e74 2e6c 6f61 645f 636f  elClient.load_co
-00013ef0: 6e6e 6563 7469 6f6e 5f69 6e66 6f60 206f  nnection_info` o
-00013f00: 6e20 4b65 726e 656c 436c 6965 6e74 2c20  n KernelClient, 
-00013f10: 6574 632e 2066 6f72 206c 6f61 6469 6e67  etc. for loading
-00013f20: 2063 6f6e 6e65 6374 696f 6e20 696e 666f   connection info
-00013f30: 0a20 2064 6972 6563 746c 7920 6672 6f6d  .  directly from
-00013f40: 2061 2064 6963 742c 206e 6f74 206a 7573   a dict, not jus
-00013f50: 7420 6672 6f6d 2066 696c 6573 2e0a 2d20  t from files..- 
-00013f60: 496e 636c 7564 6520 7061 7265 6e74 2068  Include parent h
-00013f70: 6561 6465 7273 2077 6865 6e20 6164 6170  eaders when adap
-00013f80: 7469 6e67 206d 6573 7361 6765 7320 6672  ting messages fr
-00013f90: 6f6d 206f 6c64 6572 2070 726f 746f 636f  om older protoco
-00013fa0: 6c0a 2020 696d 706c 656d 656e 7461 7469  l.  implementati
-00013fb0: 6f6e 7320 2874 7265 6174 7320 7061 7265  ons (treats pare
-00013fc0: 6e74 2068 6561 6465 7273 2074 6865 2073  nt headers the s
-00013fd0: 616d 6520 6173 2068 6561 6465 7273 292e  ame as headers).
-00013fe0: 0a2d 2043 6f6d 7061 7469 6269 6c69 7479  .- Compatibility
-00013ff0: 2066 6978 6573 2069 6e20 7465 7374 7320   fixes in tests 
-00014000: 666f 7220 7265 6365 6e74 2063 6861 6e67  for recent chang
-00014010: 6573 2069 6e20 6970 796b 6572 6e65 6c2e  es in ipykernel.
-00014020: 0a0a 2323 2034 2e33 0a0a 2323 2320 342e  ..## 4.3..### 4.
-00014030: 332e 300a 0a5b 342e 3320 6f6e 0a47 6974  3.0..[4.3 on.Git
-00014040: 4875 625d 2868 7474 7073 3a2f 2f67 6974  Hub](https://git
-00014050: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
-00014060: 6a75 7079 7465 725f 636c 6965 6e74 2f6d  jupyter_client/m
-00014070: 696c 6573 746f 6e65 732f 342e 3329 0a0a  ilestones/4.3)..
-00014080: 2d20 4164 6473 2060 2d2d 7379 732d 7072  - Adds `--sys-pr
-00014090: 6566 6978 6020 6172 6775 6d65 6e74 2074  efix` argument t
-000140a0: 6f0a 2020 606a 7570 7974 6572 206b 6572  o.  `jupyter ker
-000140b0: 6e65 6c73 7065 6320 696e 7374 616c 6c60  nelspec install`
-000140c0: 2c20 666f 720a 2020 6265 7474 6572 2073  , for.  better s
-000140d0: 796d 6d65 7472 7920 7769 7468 2060 6a75  ymmetry with `ju
-000140e0: 7079 7465 7220 6e62 6578 7465 6e73 696f  pyter nbextensio
-000140f0: 6e20 696e 7374 616c 6c60 2c20 6574 632e  n install`, etc.
-00014100: 0a0a 2323 2034 2e32 0a0a 2323 2320 342e  ..## 4.2..### 4.
-00014110: 322e 320a 0a5b 342e 322e 3220 6f6e 0a47  2.2..[4.2.2 on.G
-00014120: 6974 4875 625d 2868 7474 7073 3a2f 2f67  itHub](https://g
-00014130: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
-00014140: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
-00014150: 2f6d 696c 6573 746f 6e65 732f 342e 322e  /milestones/4.2.
-00014160: 3229 0a0a 2d20 416e 6f74 6865 7220 6669  2)..- Another fi
-00014170: 7820 666f 7220 7468 6520 6073 7461 7274  x for the `start
-00014180: 5f6e 6577 5f6b 6572 6e65 6c60 2069 7373  _new_kernel` iss
-00014190: 7565 2069 6e20 342e 322e 3120 6166 6665  ue in 4.2.1 affe
-000141a0: 6374 696e 6720 736c 6f77 2d73 7461 7274  cting slow-start
-000141b0: 696e 6720 6b65 726e 656c 732e 0a0a 2323  ing kernels...##
-000141c0: 2320 342e 322e 310a 0a5b 342e 322e 3120  # 4.2.1..[4.2.1 
-000141d0: 6f6e 0a47 6974 4875 625d 2868 7474 7073  on.GitHub](https
-000141e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-000141f0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
-00014200: 6965 6e74 2f6d 696c 6573 746f 6e65 732f  ient/milestones/
-00014210: 342e 322e 3129 0a0a 2d20 4669 7820 7265  4.2.1)..- Fix re
-00014220: 6772 6573 7369 6f6e 2069 6e20 342e 3220  gression in 4.2 
-00014230: 6361 7573 696e 6720 6073 7461 7274 5f6e  causing `start_n
-00014240: 6577 5f6b 6572 6e65 6c60 2074 6f20 6661  ew_kernel` to fa
-00014250: 696c 2077 6869 6c65 2077 6169 7469 6e67  il while waiting
-00014260: 2066 6f72 206b 6572 6e65 6c73 2074 6f20   for kernels to 
-00014270: 6265 636f 6d65 2061 7661 696c 6162 6c65  become available
-00014280: 2e0a 0a23 2323 2034 2e32 2e30 0a0a 5b34  ...### 4.2.0..[4
-00014290: 2e32 2e30 206f 6e0a 4769 7448 7562 5d28  .2.0 on.GitHub](
-000142a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000142b0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-000142c0: 6572 5f63 6c69 656e 742f 6d69 6c65 7374  er_client/milest
-000142d0: 6f6e 6573 2f34 2e32 290a 0a2d 2061 6464  ones/4.2)..- add
-000142e0: 6564 2060 6a75 7079 7465 7220 6b65 726e  ed `jupyter kern
-000142f0: 656c 7370 6563 2072 656d 6f76 6560 0a20  elspec remove`. 
-00014300: 2066 6f72 2072 656d 6f76 696e 6720 6b65   for removing ke
-00014310: 726e 656c 7370 6563 730a 2d20 616c 6c6f  rnelspecs.- allo
-00014320: 7720 7370 6563 6966 7969 6e67 2074 6865  w specifying the
-00014330: 2065 6e76 6972 6f6e 6d65 6e74 2066 6f72   environment for
-00014340: 206b 6572 6e65 6c20 7072 6f63 6573 7365   kernel processe
-00014350: 7320 7669 6120 7468 6520 6065 6e76 600a  s via the `env`.
-00014360: 2020 6172 6775 6d65 6e74 0a2d 2061 6464    argument.- add
-00014370: 6564 2060 6e61 6d65 6020 6669 656c 6420  ed `name` field 
-00014380: 746f 2063 6f6e 6e65 6374 696f 6e20 6669  to connection fi
-00014390: 6c65 7320 6964 656e 7469 6679 696e 6720  les identifying 
-000143a0: 7468 6520 6b65 726e 656c 7370 6563 0a20  the kernelspec. 
-000143b0: 206e 616d 652c 2073 6f20 7468 6174 2063   name, so that c
-000143c0: 6f6e 7375 6d65 7273 206f 6620 636f 6e6e  onsumers of conn
-000143d0: 6563 7469 6f6e 2066 696c 6573 2028 616c  ection files (al
-000143e0: 7465 726e 6174 6520 6672 6f6e 7465 6e64  ternate frontend
-000143f0: 7329 0a20 2063 616e 2069 6465 6e74 6966  s).  can identif
-00014400: 7920 7468 6520 6b65 726e 656c 7370 6563  y the kernelspec
-00014410: 2069 6e20 7573 650a 2d20 6164 6465 6420   in use.- added 
-00014420: 604b 6572 6e65 6c53 7065 634d 616e 6167  `KernelSpecManag
-00014430: 6572 2e67 6574 5f61 6c6c 5f73 7065 6373  er.get_all_specs
-00014440: 6020 666f 7220 6765 7474 696e 6720 616c  ` for getting al
-00014450: 6c20 6b65 726e 656c 7370 6563 7320 6d6f  l kernelspecs mo
-00014460: 7265 2065 6666 6963 6965 6e74 6c79 0a2d  re efficiently.-
-00014470: 2076 6172 696f 7573 2069 6d70 726f 7665   various improve
-00014480: 6d65 6e74 7320 746f 2065 7272 6f72 206d  ments to error m
-00014490: 6573 7361 6765 7320 616e 6420 646f 6375  essages and docu
-000144a0: 6d65 6e74 6174 696f 6e0a 0a23 2320 342e  mentation..## 4.
-000144b0: 310a 0a23 2323 2034 2e31 2e30 0a0a 5b34  1..### 4.1.0..[4
-000144c0: 2e31 2e30 206f 6e0a 4769 7448 7562 5d28  .1.0 on.GitHub](
-000144d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000144e0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
-000144f0: 6572 5f63 6c69 656e 742f 6d69 6c65 7374  er_client/milest
-00014500: 6f6e 6573 2f34 2e31 290a 0a48 6967 686c  ones/4.1)..Highl
-00014510: 6967 6874 733a 0a0a 2d20 5365 7475 7074  ights:..- Setupt
-00014520: 6f6f 6c73 2066 6978 6573 2066 6f72 2060  ools fixes for `
-00014530: 6a75 7079 7465 7220 6b65 726e 656c 7370  jupyter kernelsp
-00014540: 6563 600a 2d20 606a 7570 7974 6572 206b  ec`.- `jupyter k
-00014550: 6572 6e65 6c73 7065 6320 6c69 7374 6020  ernelspec list` 
-00014560: 696e 636c 7564 6573 2070 6174 6873 0a2d  includes paths.-
-00014570: 2061 6464 2060 4b65 726e 656c 4d61 6e61   add `KernelMana
-00014580: 6765 722e 626c 6f63 6b69 6e67 5f63 6c69  ger.blocking_cli
-00014590: 656e 7460 0a2d 2070 726f 7669 7369 6f6e  ent`.- provision
-000145a0: 616c 2069 6d70 6c65 6d65 6e74 6174 696f  al implementatio
-000145b0: 6e20 6f66 2060 636f 6d6d 5f69 6e66 6f60  n of `comm_info`
-000145c0: 2072 6571 7565 7374 7320 6672 6f6d 2075   requests from u
-000145d0: 7063 6f6d 696e 6720 352e 310a 2020 7265  pcoming 5.1.  re
-000145e0: 6c65 6173 6520 6f66 2074 6865 2070 726f  lease of the pro
-000145f0: 746f 636f 6c0a 0a23 2320 342e 300a 0a54  tocol..## 4.0..T
-00014600: 6865 2066 6972 7374 2072 656c 6561 7365  he first release
-00014610: 206f 6620 4a75 7079 7465 7220 436c 6965   of Jupyter Clie
-00014620: 6e74 2061 7320 6974 7320 6f77 6e20 7061  nt as its own pa
-00014630: 636b 6167 652e 0a                        ckage..
+00011d40: 3432 290a 2d20 446f 6320 6669 7820 666f  42).- Doc fix fo
+00011d50: 7220 7865 7573 2068 7970 6572 6c69 6e6b  r xeus hyperlink
+00011d60: 7320 5b23 3534 305d 2868 7474 7073 3a2f  s [#540](https:/
+00011d70: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00011d80: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00011d90: 6e74 2f70 756c 6c2f 3534 3029 0a2d 2044  nt/pull/540).- D
+00011da0: 6f63 2074 7970 6f20 6669 7820 5b23 3533  oc typo fix [#53
+00011db0: 395d 2868 7474 7073 3a2f 2f67 6974 6875  9](https://githu
+00011dc0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00011dd0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00011de0: 6c2f 3533 3929 0a0a 2323 2036 2e31 2e32  l/539)..## 6.1.2
+00011df0: 0a0a 2d20 4669 7865 6420 6120 6275 6720  ..- Fixed a bug 
+00011e00: 6361 7573 696e 6720 636c 6965 6e74 7320  causing clients 
+00011e10: 746f 2073 6f6d 6574 696d 6573 2068 616e  to sometimes han
+00011e20: 6720 6166 7465 7220 6120 7374 6f70 2063  g after a stop c
+00011e30: 616c 6c20 7761 730a 2020 6d61 6465 205b  all was.  made [
+00011e40: 2335 3336 5d28 6874 7470 733a 2f2f 6769  #536](https://gi
+00011e50: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+00011e60: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+00011e70: 7075 6c6c 2f35 3336 290a 0a23 2320 362e  pull/536)..## 6.
+00011e80: 312e 310a 0a2d 2053 7562 7072 6f63 6573  1.1..- Subproces
+00011e90: 7320 6b69 6c6c 2061 6374 696f 6e20 6669  s kill action fi
+00011ea0: 7820 666f 7220 6173 796e 6320 6578 6563  x for async exec
+00011eb0: 7574 696f 6e0a 2020 5b23 3533 355d 2868  ution.  [#535](h
+00011ec0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00011ed0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+00011ee0: 725f 636c 6965 6e74 2f70 756c 6c2f 3533  r_client/pull/53
+00011ef0: 3529 0a2d 2044 6f63 2066 6978 2066 6f72  5).- Doc fix for
+00011f00: 2078 6575 7320 6b65 726e 656c 206c 6973   xeus kernel lis
+00011f10: 7420 5b23 3533 345d 2868 7474 7073 3a2f  t [#534](https:/
+00011f20: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00011f30: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00011f40: 6e74 2f70 756c 6c2f 3533 3429 0a0a 2323  nt/pull/534)..##
+00011f50: 2036 2e31 2e30 0a0a 5468 6973 2072 656c   6.1.0..This rel
+00011f60: 6561 7365 2069 6e63 6c75 6465 7320 7375  ease includes su
+00011f70: 7070 6f72 7420 666f 7220 6173 796e 6369  pport for asynci
+00011f80: 6f20 7061 7474 6572 6e73 2120 446f 776e  o patterns! Down
+00011f90: 7374 7265 616d 2074 6f6f 6c73 0a73 686f  stream tools.sho
+00011fa0: 756c 6420 736f 6f6e 2068 6176 6520 7265  uld soon have re
+00011fb0: 6c65 6173 6573 2074 6f20 6164 6469 7469  leases to additi
+00011fc0: 6f6e 616c 6c79 2073 7570 706f 7274 2061  onally support a
+00011fd0: 7379 6e63 2070 6174 7465 726e 732e 0a0a  sync patterns...
+00011fe0: 2d20 4173 796e 634b 6572 6e65 6c4d 616e  - AsyncKernelMan
+00011ff0: 6167 6572 2061 6e64 2041 7379 6e63 4d75  ager and AsyncMu
+00012000: 6c74 694b 6572 6e65 6c4d 616e 6167 6572  ltiKernelManager
+00012010: 2061 7265 206e 6f77 2061 7661 696c 6162   are now availab
+00012020: 6c65 2066 6f72 0a20 2061 7379 6e63 206a  le for.  async j
+00012030: 7570 7974 6572 5f63 6c69 656e 7420 696e  upyter_client in
+00012040: 7465 7261 6374 696f 6e73 2028 5b23 3532  teractions ([#52
+00012050: 385d 2868 7474 7073 3a2f 2f67 6974 6875  8](https://githu
+00012060: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00012070: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00012080: 6c2f 3532 3829 2c20 5b23 3532 395d 2868  l/528), [#529](h
+00012090: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000120a0: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+000120b0: 725f 636c 6965 6e74 2f70 756c 6c2f 3532  r_client/pull/52
+000120c0: 3929 290a 2d20 5265 6d6f 7665 6420 756e  9)).- Removed un
+000120d0: 7573 6564 2073 7068 696e 7820 6465 7065  used sphinx depe
+000120e0: 6e64 656e 6379 2028 5b23 3531 385d 2868  ndency ([#518](h
+000120f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00012100: 6d2f 6a75 7079 7465 722f 6a75 7079 7465  m/jupyter/jupyte
+00012110: 725f 636c 6965 6e74 2f70 756c 6c2f 3531  r_client/pull/51
+00012120: 3829 2c20 5b23 3531 385d 2868 7474 7073  8), [#518](https
+00012130: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00012140: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+00012150: 6965 6e74 2f70 756c 6c2f 3531 3829 292e  ient/pull/518)).
+00012160: 0a2d 2041 6464 6564 2069 6e73 7461 6c6c  .- Added install
+00012170: 2069 6e73 7472 7563 7469 6f6e 7320 666f   instructions fo
+00012180: 7220 7069 7020 746f 2064 6f63 756d 656e  r pip to documen
+00012190: 7461 7469 6f6e 0a20 205b 2335 3231 5d28  tation.  [#521](
+000121a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000121b0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+000121c0: 6572 5f63 6c69 656e 742f 7075 6c6c 2f35  er_client/pull/5
+000121d0: 3231 290a 2d20 496d 7072 6f76 6564 2064  21).- Improved d
+000121e0: 6f63 7320 6172 6f75 6e64 2076 6572 7369  ocs around versi
+000121f0: 6f6e 2070 726f 746f 636f 6c20 616e 6420  on protocol and 
+00012200: 6d65 7373 6167 696e 670a 2020 285b 2335  messaging.  ([#5
+00012210: 3232 5d28 6874 7470 733a 2f2f 6769 7468  22](https://gith
+00012220: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00012230: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+00012240: 6c6c 2f35 3232 292c 205b 2335 3236 5d28  ll/522), [#526](
+00012250: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00012260: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00012270: 6572 5f63 6c69 656e 742f 7075 6c6c 2f35  er_client/pull/5
+00012280: 3236 2929 0a0a 2323 2036 2e30 2e30 0a0a  26))..## 6.0.0..
+00012290: 5468 6520 6769 7420 6869 7374 6f72 7920  The git history 
+000122a0: 6861 6420 746f 2062 6520 7265 776f 726b  had to be rework
+000122b0: 6564 2068 6561 7669 6c79 2069 6e20 6d65  ed heavily in me
+000122c0: 7267 696e 6720 352e 7820 616e 6420 6d61  rging 5.x and ma
+000122d0: 7374 6572 2c20 736f 0a61 206c 696e 6b20  ster, so.a link 
+000122e0: 746f 2061 6c6c 2074 6865 2063 6861 6e67  to all the chang
+000122f0: 6573 2061 7420 6f6e 6365 2069 6e20 6769  es at once in gi
+00012300: 7468 7562 2068 6164 2062 6565 6e20 6c65  thub had been le
+00012310: 6674 206f 7574 2061 7320 6974 2773 0a6a  ft out as it's.j
+00012320: 7573 7420 636f 6e66 7573 696e 672e 0a0a  ust confusing...
+00012330: 416e 2065 7863 6974 696e 6720 6368 616e  An exciting chan
+00012340: 6765 2069 6e20 7468 6973 2072 656c 6561  ge in this relea
+00012350: 7365 2069 7320 736f 6d65 2061 7379 6e63  se is some async
+00012360: 2073 7570 706f 7274 2028 6875 6765 2074   support (huge t
+00012370: 6861 6e6b 7320 746f 0a40 6461 7669 6462  hanks to.@davidb
+00012380: 726f 6368 6172 7420 666f 7220 646f 696e  rochart for doin
+00012390: 6720 6d6f 7374 206f 6620 7468 6520 776f  g most of the wo
+000123a0: 726b 2921 2053 6565 206c 696e 6b65 6420  rk)! See linked 
+000123b0: 5052 2062 656c 6f77 2066 6f72 0a6d 6f72  PR below for.mor
+000123c0: 6520 6465 7461 696c 732c 2077 6527 7265  e details, we're
+000123d0: 2077 6f72 6b69 6e67 206f 6e20 696e 7465   working on inte
+000123e0: 6772 6174 696e 6720 7468 6973 2069 6e74  grating this int
+000123f0: 6f20 6e62 636c 6965 6e74 2061 7320 7765  o nbclient as we
+00012400: 6c6c 0a69 6e20 7468 6520 6e65 6172 2066  ll.in the near f
+00012410: 7574 7572 652e 0a0a 4e65 7720 4665 6174  uture...New Feat
+00012420: 7572 6573 3a0a 0a2d 2041 6464 6564 2061  ures:..- Added a
+00012430: 7379 6e63 2041 5049 205b 2335 3036 5d28  sync API [#506](
+00012440: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00012450: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00012460: 6572 5f63 6c69 656e 742f 7075 6c6c 2f35  er_client/pull/5
+00012470: 3036 290a 0a43 6861 6e67 6573 3a0a 0a2d  06)..Changes:..-
+00012480: 2050 7974 686f 6e20 332e 3820 7465 7374   Python 3.8 test
+00012490: 696e 6720 616e 6420 7375 7070 6f72 7420  ing and support 
+000124a0: 6164 6465 6420 5b23 3530 395d 2868 7474  added [#509](htt
+000124b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000124c0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+000124d0: 636c 6965 6e74 2f70 756c 6c2f 3530 3929  client/pull/509)
+000124e0: 0a2d 2053 6573 7369 6f6e 2e6d 7367 5f69  .- Session.msg_i
+000124f0: 6420 6f70 7469 6d69 7a61 7469 6f6e 205b  d optimization [
+00012500: 2334 3933 5d28 6874 7470 733a 2f2f 6769  #493](https://gi
+00012510: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+00012520: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+00012530: 7075 6c6c 2f34 3933 290a 2d20 4f6e 6c79  pull/493).- Only
+00012540: 2063 6163 6865 2070 6f72 7473 2069 6620   cache ports if 
+00012550: 7468 6520 6361 6368 655f 706f 7274 7320  the cache_ports 
+00012560: 666c 6167 2069 7320 7365 7420 746f 2054  flag is set to T
+00012570: 7275 650a 2020 5b23 3439 325d 2868 7474  rue.  [#492](htt
+00012580: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00012590: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+000125a0: 636c 6965 6e74 2f70 756c 6c2f 3439 3229  client/pull/492)
+000125b0: 0a2d 2052 656d 6f76 6564 2064 6972 6563  .- Removed direc
+000125c0: 7420 6465 7065 6e64 656e 6379 206f 6e20  t dependency on 
+000125d0: 7079 7769 6e33 3220 6173 2074 6869 7320  pywin32 as this 
+000125e0: 6973 206e 6f77 2069 6e20 6a75 7079 7465  is now in jupyte
+000125f0: 7220 636f 7265 0a20 205b 2334 3839 5d28  r core.  [#489](
+00012600: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00012610: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00012620: 6572 5f63 6c69 656e 742f 7075 6c6c 2f34  er_client/pull/4
+00012630: 3839 290a 0a46 6978 6573 3a0a 0a2d 2050  89)..Fixes:..- P
+00012640: 7265 7665 6e74 2074 776f 206b 6572 6e65  revent two kerne
+00012650: 6c73 2074 6f20 6861 7665 2074 6865 2073  ls to have the s
+00012660: 616d 6520 706f 7274 7320 5b23 3439 305d  ame ports [#490]
+00012670: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00012680: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00012690: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+000126a0: 3439 3029 0a0a 446f 6373 3a0a 0a2d 2044  490)..Docs:..- D
+000126b0: 6f63 756d 656e 7420 7468 6520 6861 6e64  ocument the hand
+000126c0: 6c69 6e67 206f 6620 6572 726f 7220 696e  ling of error in
+000126d0: 2064 6f5f 6578 6563 7574 650a 2020 5b23   do_execute.  [#
+000126e0: 3530 305d 2868 7474 7073 3a2f 2f67 6974  500](https://git
+000126f0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00012700: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+00012710: 756c 6c2f 3530 3029 0a0a 4272 6561 6b69  ull/500)..Breaki
+00012720: 6e67 2063 6861 6e67 6573 3a0a 0a2d 2044  ng changes:..- D
+00012730: 726f 7070 6564 2073 7570 706f 7274 2066  ropped support f
+00012740: 6f72 2050 7974 686f 6e20 322e 3721 0a0a  or Python 2.7!..
+00012750: 2323 2035 2e33 2e35 0a0a 2d20 4261 636b  ## 5.3.5..- Back
+00012760: 706f 7274 6564 206d 656d 6f72 7920 6c65  ported memory le
+00012770: 616b 2066 6978 205b 2335 3438 5d28 6874  ak fix [#548](ht
+00012780: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00012790: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+000127a0: 5f63 6c69 656e 742f 7075 6c6c 2f35 3438  _client/pull/548
+000127b0: 290a 2020 5b23 3535 355d 2868 7474 7073  ).  [#555](https
+000127c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+000127d0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+000127e0: 6965 6e74 2f70 756c 6c2f 3535 3529 2e0a  ient/pull/555)..
+000127f0: 0a23 2320 352e 332e 340a 0a2d 2043 6861  .## 5.3.4..- Cha
+00012800: 6e67 6564 2073 6563 7572 655f 7772 6974  nged secure_writ
+00012810: 6520 746f 2062 6520 696d 706f 7274 6564  e to be imported
+00012820: 2066 726f 6d20 6a75 7079 7465 725f 636f   from jupyter_co
+00012830: 7265 2077 6974 6820 6669 7820 666f 720a  re with fix for.
+00012840: 2020 6578 7465 6e64 6564 2075 7365 726e    extended usern
+00012850: 616d 6573 2069 6e20 5769 6e64 6f77 7320  ames in Windows 
+00012860: 5b23 3438 335d 2868 7474 7073 3a2f 2f67  [#483](https://g
+00012870: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00012880: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00012890: 2f70 756c 6c2f 3438 3329 2e0a 0a23 2320  /pull/483)...## 
+000128a0: 352e 332e 330a 0a2d 2046 6978 6564 2069  5.3.3..- Fixed i
+000128b0: 7373 7565 2077 6974 6820 6e6f 6e2d 656e  ssue with non-en
+000128c0: 676c 6973 6820 7769 6e64 6f77 7320 7065  glish windows pe
+000128d0: 726d 6973 7369 6f6e 730a 2020 5b23 3437  rmissions.  [#47
+000128e0: 385d 2868 7474 7073 3a2f 2f67 6974 6875  8](https://githu
+000128f0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00012900: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00012910: 6c2f 3437 3829 2e20 506f 7465 6e74 6961  l/478). Potentia
+00012920: 6c20 6973 7375 6520 7374 696c 6c20 6f70  l issue still op
+00012930: 656e 0a20 2069 6e20 7573 6520 7769 7468  en.  in use with
+00012940: 206a 7570 7965 726c 6162 2e0a 0a23 2320   jupyerlab...## 
+00012950: 352e 332e 320a 0a2d 2049 6d70 6f72 7461  5.3.2..- Importa
+00012960: 6e74 2066 696c 6573 2063 7265 6174 696f  nt files creatio
+00012970: 6e20 6e6f 7720 6368 6563 6b73 2075 6d61  n now checks uma
+00012980: 736b 2070 6572 6d69 7373 696f 6e73 0a20  sk permissions. 
+00012990: 205b 2334 3639 5d28 6874 7470 733a 2f2f   [#469](https://
+000129a0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+000129b0: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+000129c0: 742f 7075 6c6c 2f34 3639 292e 0a0a 2323  t/pull/469)...##
+000129d0: 2035 2e33 2e31 0a0a 2d20 4669 7820 6275   5.3.1..- Fix bu
+000129e0: 6720 7769 7468 2063 6f6e 7472 6f6c 2063  g with control c
+000129f0: 6861 6e6e 656c 2073 6f63 6b65 7420 696e  hannel socket in
+00012a00: 7472 6f64 7563 6564 2069 6e20 352e 332e  troduced in 5.3.
+00012a10: 300a 2020 5b23 3435 365d 2868 7474 7073  0.  [#456](https
+00012a20: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00012a30: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+00012a40: 6965 6e74 2f70 756c 6c2f 3435 3629 2e0a  ient/pull/456)..
+00012a50: 0a23 2320 352e 332e 300a 0a5b 352e 332e  .## 5.3.0..[5.3.
+00012a60: 3020 6f6e 0a47 6974 4875 625d 2868 7474  0 on.GitHub](htt
+00012a70: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00012a80: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00012a90: 636c 6965 6e74 2f6d 696c 6573 746f 6e65  client/milestone
+00012aa0: 732f 352e 332e 3029 0a0a 4e65 7720 4665  s/5.3.0)..New Fe
+00012ab0: 6174 7572 6573 3a0a 0a2d 204d 756c 7469  atures:..- Multi
+00012ac0: 7072 6f63 6573 7369 6e67 2061 6e64 2054  processing and T
+00012ad0: 6872 6561 6469 6e67 2073 7570 706f 7274  hreading support
+00012ae0: 205b 2334 3337 5d28 6874 7470 733a 2f2f   [#437](https://
+00012af0: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00012b00: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00012b10: 742f 7075 6c6c 2f34 3337 2920 616e 6420  t/pull/437) and 
+00012b20: 5b23 3435 305d 2868 7474 7073 3a2f 2f67  [#450](https://g
+00012b30: 6974 6875 622e 636f 6d2f 6a75 7079 7465  ithub.com/jupyte
+00012b40: 722f 6a75 7079 7465 725f 636c 6965 6e74  r/jupyter_client
+00012b50: 2f70 756c 6c2f 3435 3029 0a2d 2053 6574  /pull/450).- Set
+00012b60: 7570 2070 6163 6b61 6765 206c 6f6e 675f  up package long_
+00012b70: 6465 7363 7269 7074 696f 6e20 5b23 3431  description [#41
+00012b80: 315d 2868 7474 7073 3a2f 2f67 6974 6875  1](https://githu
+00012b90: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00012ba0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00012bb0: 6c2f 3431 3129 0a0a 4368 616e 6765 733a  l/411)..Changes:
+00012bc0: 0a0a 2d20 436f 6e74 726f 6c20 6368 616e  ..- Control chan
+00012bd0: 6e65 6c20 6e6f 7720 696e 2074 6865 2070  nel now in the p
+00012be0: 7562 6c69 6320 4150 4920 5b23 3434 375d  ublic API [#447]
+00012bf0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00012c00: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00012c10: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00012c20: 3434 3729 0a2d 2043 6c6f 7369 6e67 204a  447).- Closing J
+00012c30: 7570 7974 6572 2043 6c69 656e 7420 6973  upyter Client is
+00012c40: 206e 6f77 2066 6173 7465 7220 5b23 3432   now faster [#42
+00012c50: 305d 2868 7474 7073 3a2f 2f67 6974 6875  0](https://githu
+00012c60: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00012c70: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00012c80: 6c2f 3432 3029 0a2d 2050 6970 2073 7570  l/420).- Pip sup
+00012c90: 706f 7274 2069 6d70 726f 7665 6d65 6e74  port improvement
+00012ca0: 7320 5b23 3432 315d 2868 7474 7073 3a2f  s [#421](https:/
+00012cb0: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00012cc0: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00012cd0: 6e74 2f70 756c 6c2f 3432 3129 0a0a 4272  nt/pull/421)..Br
+00012ce0: 6561 6b69 6e67 2063 6861 6e67 6573 3a0a  eaking changes:.
+00012cf0: 0a2d 2044 726f 7070 6564 2073 7570 706f  .- Dropped suppo
+00012d00: 7274 2066 6f72 2050 7974 686f 6e20 332e  rt for Python 3.
+00012d10: 3320 616e 6420 332e 3420 2875 7073 7472  3 and 3.4 (upstr
+00012d20: 6561 6d20 7061 636b 6167 6573 2064 726f  eam packages dro
+00012d30: 7070 6564 0a20 2073 7570 706f 7274 2061  pped.  support a
+00012d40: 6c72 6561 6479 290a 0a23 2320 352e 322e  lready)..## 5.2.
+00012d50: 340a 0a5b 352e 322e 3420 6f6e 0a47 6974  4..[5.2.4 on.Git
+00012d60: 4875 625d 2868 7474 7073 3a2f 2f67 6974  Hub](https://git
+00012d70: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00012d80: 6a75 7079 7465 725f 636c 6965 6e74 2f6d  jupyter_client/m
+00012d90: 696c 6573 746f 6e65 732f 352e 322e 3429  ilestones/5.2.4)
+00012da0: 0a0a 2d20 5072 6576 656e 7420 6372 6561  ..- Prevent crea
+00012db0: 7469 6e67 206e 6577 2063 6f6e 736f 6c65  ting new console
+00012dc0: 2077 696e 646f 7773 206f 6e20 5769 6e64   windows on Wind
+00012dd0: 6f77 730a 2020 5b23 3334 365d 2868 7474  ows.  [#346](htt
+00012de0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00012df0: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00012e00: 636c 6965 6e74 2f70 756c 6c2f 3334 3629  client/pull/346)
+00012e10: 0a2d 2046 6978 2069 6e74 6572 7275 7074  .- Fix interrupt
+00012e20: 7320 6f6e 2050 7974 686f 6e20 332e 3720  s on Python 3.7 
+00012e30: 6f6e 2057 696e 646f 7773 205b 2334 3038  on Windows [#408
+00012e40: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00012e50: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00012e60: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00012e70: 2f34 3038 290a 0a23 2320 352e 322e 330a  /408)..## 5.2.3.
+00012e80: 0a5b 352e 322e 3320 6f6e 0a47 6974 4875  .[5.2.3 on.GitHu
+00012e90: 625d 2868 7474 7073 3a2f 2f67 6974 6875  b](https://githu
+00012ea0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00012eb0: 7079 7465 725f 636c 6965 6e74 2f6d 696c  pyter_client/mil
+00012ec0: 6573 746f 6e65 732f 352e 322e 3329 0a0a  estones/5.2.3)..
+00012ed0: 2d20 4669 7820 6861 6e67 206f 6e20 636c  - Fix hang on cl
+00012ee0: 6f73 6520 696e 2060 2e54 6872 6561 6465  ose in `.Threade
+00012ef0: 644b 6572 6e65 6c43 6c69 656e 7460 2028  dKernelClient` (
+00012f00: 7573 6564 2069 6e20 5174 436f 6e73 6f6c  used in QtConsol
+00012f10: 6529 2077 6865 6e20 7573 696e 6720 746f  e) when using to
+00012f20: 726e 6164 6f20 7769 7468 2061 7379 6e63  rnado with async
+00012f30: 696f 0a20 2028 6465 6661 756c 7420 6265  io.  (default be
+00012f40: 6861 7669 6f72 206f 6620 746f 726e 6164  havior of tornad
+00012f50: 6f20 352c 2073 6565 205b 2333 3532 5d28  o 5, see [#352](
+00012f60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00012f70: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00012f80: 6572 5f63 6c69 656e 742f 7075 6c6c 2f33  er_client/pull/3
+00012f90: 3532 2929 2e0a 2d20 4669 7820 6572 726f  52))..- Fix erro
+00012fa0: 7273 2077 6865 6e20 7573 696e 6720 6465  rs when using de
+00012fb0: 7072 6563 6174 6564 0a20 2060 2e4b 6572  precated.  `.Ker
+00012fc0: 6e65 6c4d 616e 6167 6572 2e6b 6572 6e65  nelManager.kerne
+00012fd0: 6c5f 636d 6460 0a20 2028 5b23 3334 335d  l_cmd`.  ([#343]
+00012fe0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00012ff0: 636f 6d2f 6a75 7079 7465 722f 6a75 7079  com/jupyter/jupy
+00013000: 7465 725f 636c 6965 6e74 2f70 756c 6c2f  ter_client/pull/
+00013010: 3334 3329 2c20 5b23 3334 345d 2868 7474  343), [#344](htt
+00013020: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00013030: 6a75 7079 7465 722f 6a75 7079 7465 725f  jupyter/jupyter_
+00013040: 636c 6965 6e74 2f70 756c 6c2f 3334 3429  client/pull/344)
+00013050: 292e 0a0a 2323 2035 2e32 2e32 0a0a 5b35  )...## 5.2.2..[5
+00013060: 2e32 2e32 206f 6e0a 4769 7448 7562 5d28  .2.2 on.GitHub](
+00013070: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00013080: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00013090: 6572 5f63 6c69 656e 742f 6d69 6c65 7374  er_client/milest
+000130a0: 6f6e 6573 2f35 2e32 2e32 290a 0a2d 2046  ones/5.2.2)..- F
+000130b0: 6978 2060 2e4b 6572 6e65 6c53 7065 634d  ix `.KernelSpecM
+000130c0: 616e 6167 6572 2e67 6574 5f61 6c6c 5f73  anager.get_all_s
+000130d0: 7065 6373 6020 6d65 7468 6f64 2069 6e20  pecs` method in 
+000130e0: 7375 6263 6c61 7373 6573 2074 6861 7420  subclasses that 
+000130f0: 6f6e 6c79 206f 7665 7272 6964 650a 2020  only override.  
+00013100: 602e 4b65 726e 656c 5370 6563 4d61 6e61  `.KernelSpecMana
+00013110: 6765 722e 6669 6e64 5f6b 6572 6e65 6c5f  ger.find_kernel_
+00013120: 7370 6563 7360 2061 6e64 0a20 2060 2e4b  specs` and.  `.K
+00013130: 6572 6e65 6c53 7065 634d 616e 6167 6572  ernelSpecManager
+00013140: 2e67 6574 5f6b 6572 6e65 6c5f 7370 6563  .get_kernel_spec
+00013150: 602e 0a20 2053 6565 205b 2333 3338 5d28  `..  See [#338](
+00013160: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00013170: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00013180: 6572 5f63 6c69 656e 742f 6973 7375 6573  er_client/issues
+00013190: 2f33 3338 2920 616e 640a 2020 5b23 3333  /338) and.  [#33
+000131a0: 395d 2868 7474 7073 3a2f 2f67 6974 6875  9](https://githu
+000131b0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+000131c0: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+000131d0: 6c2f 3333 3929 2e0a 2d20 456c 696d 696e  l/339)..- Elimin
+000131e0: 6174 6520 6f63 6361 7369 6f6e 616c 2065  ate occasional e
+000131f0: 7272 6f72 206d 6573 7361 6765 7320 6475  rror messages du
+00013200: 7269 6e67 2070 726f 6365 7373 2065 7869  ring process exi
+00013210: 740a 2020 5b23 3333 365d 2868 7474 7073  t.  [#336](https
+00013220: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00013230: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+00013240: 6965 6e74 2f70 756c 6c2f 3333 3629 2e0a  ient/pull/336)..
+00013250: 2d20 496d 7072 6f76 6520 6572 726f 7220  - Improve error 
+00013260: 6d65 7373 6167 6520 7768 656e 2061 7474  message when att
+00013270: 656d 7074 696e 6720 746f 2062 696e 6420  empting to bind 
+00013280: 6f6e 2069 6e76 616c 6964 2061 6464 7265  on invalid addre
+00013290: 7373 0a20 205b 2333 3330 5d28 6874 7470  ss.  [#330](http
+000132a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+000132b0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
+000132c0: 6c69 656e 742f 7075 6c6c 2f33 3330 292e  lient/pull/330).
+000132d0: 0a2d 2041 6464 206d 6973 7369 6e67 2064  .- Add missing d
+000132e0: 6972 6563 7420 6465 7065 6e64 656e 6379  irect dependency
+000132f0: 206f 6e20 746f 726e 6164 6f20 5b23 3332   on tornado [#32
+00013300: 335d 2868 7474 7073 3a2f 2f67 6974 6875  3](https://githu
+00013310: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00013320: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00013330: 6c2f 3332 3329 2e0a 0a23 2320 352e 322e  l/323)...## 5.2.
+00013340: 310a 0a5b 352e 322e 3120 6f6e 0a47 6974  1..[5.2.1 on.Git
+00013350: 4875 625d 2868 7474 7073 3a2f 2f67 6974  Hub](https://git
+00013360: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00013370: 6a75 7079 7465 725f 636c 6965 6e74 2f6d  jupyter_client/m
+00013380: 696c 6573 746f 6e65 732f 352e 322e 3129  ilestones/5.2.1)
+00013390: 0a0a 2d20 4164 6420 7061 7265 6e74 6865  ..- Add parenthe
+000133a0: 7369 7320 746f 2063 6f6e 6469 7469 6f6e  sis to condition
+000133b0: 616c 2070 7974 6573 7420 7265 7175 6972  al pytest requir
+000133c0: 656d 656e 7420 746f 2077 6f72 6b20 6172  ement to work ar
+000133d0: 6f75 6e64 2061 0a20 2062 7567 2069 6e20  ound a.  bug in 
+000133e0: 7468 6520 6077 6865 656c 6020 7061 636b  the `wheel` pack
+000133f0: 6167 652c 2074 6861 7420 6765 6e65 7261  age, that genera
+00013400: 7465 2061 2060 2e77 686c 6020 7768 6963  te a `.whl` whic
+00013410: 6820 6f74 6865 7277 6973 650a 2020 616c  h otherwise.  al
+00013420: 7761 7973 2064 6570 656e 6473 206f 6e20  ways depends on 
+00013430: 6070 7974 6573 7460 2073 6565 205b 2333  `pytest` see [#3
+00013440: 3234 5d28 6874 7470 733a 2f2f 6769 7468  24](https://gith
+00013450: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00013460: 7570 7974 6572 5f63 6c69 656e 742f 6973  upyter_client/is
+00013470: 7375 6573 2f33 3234 2961 6e64 205b 2333  sues/324)and [#3
+00013480: 3235 5d28 6874 7470 733a 2f2f 6769 7468  25](https://gith
+00013490: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+000134a0: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+000134b0: 6c6c 2f33 3235 292e 0a0a 2323 2035 2e32  ll/325)...## 5.2
+000134c0: 0a0a 5b35 2e32 206f 6e0a 4769 7448 7562  ..[5.2 on.GitHub
+000134d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000134e0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+000134f0: 7974 6572 5f63 6c69 656e 742f 6d69 6c65  yter_client/mile
+00013500: 7374 6f6e 6573 2f35 2e32 290a 0a2d 2044  stones/5.2)..- D
+00013510: 6566 696e 6520 4a75 7079 7465 7220 7072  efine Jupyter pr
+00013520: 6f74 6f63 6f6c 2076 6572 7369 6f6e 2035  otocol version 5
+00013530: 2e33 3a0a 2020 2d20 4b65 726e 656c 7320  .3:.  - Kernels 
+00013540: 6361 6e20 6e6f 7720 6f70 7420 746f 2062  can now opt to b
+00013550: 6520 696e 7465 7272 7570 7465 6420 6279  e interrupted by
+00013560: 2061 206d 6573 7361 6765 2073 656e 7420   a message sent 
+00013570: 6f6e 2074 6865 0a20 2020 2063 6f6e 7472  on the.    contr
+00013580: 6f6c 2063 6861 6e6e 656c 2069 6e73 7465  ol channel inste
+00013590: 6164 206f 6620 6120 7379 7374 656d 2073  ad of a system s
+000135a0: 6967 6e61 6c2e 2053 6565 0a20 2020 2060  ignal. See.    `
+000135b0: 6b65 726e 656c 7370 6563 7360 2061 6e64  kernelspecs` and
+000135c0: 0a20 2020 2060 6d73 6769 6e67 5f69 6e74  .    `msging_int
+000135d0: 6572 7275 7074 600a 2020 2020 5b23 3239  errupt`.    [#29
+000135e0: 345d 2868 7474 7073 3a2f 2f67 6974 6875  4](https://githu
+000135f0: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00013600: 7079 7465 725f 636c 6965 6e74 2f70 756c  pyter_client/pul
+00013610: 6c2f 3239 3429 2e0a 2d20 4e65 7720 606a  l/294)..- New `j
+00013620: 7570 7974 6572 206b 6572 6e65 6c60 2063  upyter kernel` c
+00013630: 6f6d 6d61 6e64 2074 6f20 6c61 756e 6368  ommand to launch
+00013640: 2061 6e20 696e 7374 616c 6c65 6420 6b65   an installed ke
+00013650: 726e 656c 2062 7920 6e61 6d65 0a20 205b  rnel by name.  [
+00013660: 2332 3430 5d28 6874 7470 733a 2f2f 6769  #240](https://gi
+00013670: 7468 7562 2e63 6f6d 2f6a 7570 7974 6572  thub.com/jupyter
+00013680: 2f6a 7570 7974 6572 5f63 6c69 656e 742f  /jupyter_client/
+00013690: 7075 6c6c 2f32 3430 292e 0a2d 204b 6572  pull/240)..- Ker
+000136a0: 6e65 6c73 7065 6373 2077 6865 7265 2074  nelspecs where t
+000136b0: 6865 2063 6f6d 6d61 6e64 2073 7461 7274  he command start
+000136c0: 7320 7769 7468 2065 2e67 2e20 6070 7974  s with e.g. `pyt
+000136d0: 686f 6e33 6020 6f72 0a20 2060 7079 7468  hon3` or.  `pyth
+000136e0: 6f6e 332e 3660 2d2d 2d6d 6174 6368 696e  on3.6`---matchin
+000136f0: 6720 7468 6520 7665 7273 696f 6e20 606a  g the version `j
+00013700: 7570 7974 6572 5f63 6c69 656e 7460 2069  upyter_client` i
+00013710: 7320 7275 6e6e 696e 670a 2020 6f6e 2d2d  s running.  on--
+00013720: 2d61 7265 206e 6f77 206c 6175 6e63 6865  -are now launche
+00013730: 6420 7769 7468 2074 6865 2073 616d 6520  d with the same 
+00013740: 5079 7468 6f6e 2065 7865 6375 7461 626c  Python executabl
+00013750: 6520 6173 2074 6865 0a20 206c 6175 6e63  e as the.  launc
+00013760: 6869 6e67 2070 726f 6365 7373 205b 2333  hing process [#3
+00013770: 3036 5d28 6874 7470 733a 2f2f 6769 7468  06](https://gith
+00013780: 7562 2e63 6f6d 2f6a 7570 7974 6572 2f6a  ub.com/jupyter/j
+00013790: 7570 7974 6572 5f63 6c69 656e 742f 7075  upyter_client/pu
+000137a0: 6c6c 2f33 3036 292e 2054 6869 730a 2020  ll/306). This.  
+000137b0: 6578 7465 6e64 7320 7468 6520 7370 6563  extends the spec
+000137c0: 6961 6c20 6861 6e64 6c69 6e67 206f 6620  ial handling of 
+000137d0: 6070 7974 686f 6e60 2061 6464 6564 2069  `python` added i
+000137e0: 6e20 352e 302e 0a2d 2043 6f6d 6d61 6e64  n 5.0..- Command
+000137f0: 206c 696e 6520 6172 6775 6d65 6e74 7320   line arguments 
+00013800: 7370 6563 6966 6965 6420 6279 2061 206b  specified by a k
+00013810: 6572 6e65 6c73 7065 6320 6361 6e20 6e6f  ernelspec can no
+00013820: 7720 696e 636c 7564 650a 2020 607b 7265  w include.  `{re
+00013830: 736f 7572 6365 5f64 6972 7d60 2c20 7768  source_dir}`, wh
+00013840: 6963 6820 7769 6c6c 2062 6520 7375 6273  ich will be subs
+00013850: 7469 7475 7465 6420 7769 7468 2074 6865  tituted with the
+00013860: 206b 6572 6e65 6c73 7065 630a 2020 7265   kernelspec.  re
+00013870: 736f 7572 6365 2064 6972 6563 746f 7279  source directory
+00013880: 2070 6174 6820 7768 656e 2074 6865 206b   path when the k
+00013890: 6572 6e65 6c20 6973 206c 6175 6e63 6865  ernel is launche
+000138a0: 640a 2020 5b23 3238 395d 2868 7474 7073  d.  [#289](https
+000138b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+000138c0: 7079 7465 722f 6a75 7079 7465 725f 636c  pyter/jupyter_cl
+000138d0: 6965 6e74 2f70 756c 6c2f 3238 3929 2e0a  ient/pull/289)..
+000138e0: 2d20 4b65 726e 656c 7370 6563 7320 6e6f  - Kernelspecs no
+000138f0: 7720 6861 7665 2061 6e20 6f70 7469 6f6e  w have an option
+00013900: 616c 2060 6d65 7461 6461 7461 6020 6669  al `metadata` fi
+00013910: 656c 6420 746f 2068 6f6c 6420 6172 6269  eld to hold arbi
+00013920: 7472 6172 790a 2020 6d65 7461 6461 7461  trary.  metadata
+00013930: 2061 626f 7574 206b 6572 6e65 6c73 2d2d   about kernels--
+00013940: 2d73 6565 2060 6b65 726e 656c 7370 6563  -see `kernelspec
+00013950: 7360 205b 2332 3734 5d28 6874 7470 733a  s` [#274](https:
+00013960: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+00013970: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+00013980: 656e 742f 7075 6c6c 2f32 3734 292e 0a2d  ent/pull/274)..-
+00013990: 204d 616b 6520 7468 6520 604b 6572 6e65   Make the `Kerne
+000139a0: 6c52 6573 7461 7274 6572 6020 636c 6173  lRestarter` clas
+000139b0: 7320 7573 6564 2062 7920 6120 604b 6572  s used by a `Ker
+000139c0: 6e65 6c4d 616e 6167 6572 600a 2020 636f  nelManager`.  co
+000139d0: 6e66 6967 7572 6162 6c65 205b 2332 3930  nfigurable [#290
+000139e0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000139f0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00013a00: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00013a10: 2f32 3930 292e 0a2d 2057 6865 6e20 6b69  /290)..- When ki
+00013a20: 6c6c 696e 6720 6120 6b65 726e 656c 206f  lling a kernel o
+00013a30: 6e20 556e 6978 2c20 6b69 6c6c 2069 7473  n Unix, kill its
+00013a40: 2070 726f 6365 7373 2067 726f 7570 0a20   process group. 
+00013a50: 205b 2333 3134 5d28 6874 7470 733a 2f2f   [#314](https://
+00013a60: 6769 7468 7562 2e63 6f6d 2f6a 7570 7974  github.com/jupyt
+00013a70: 6572 2f6a 7570 7974 6572 5f63 6c69 656e  er/jupyter_clien
+00013a80: 742f 7075 6c6c 2f33 3134 292e 0a2d 2049  t/pull/314)..- I
+00013a90: 6620 6120 6b65 726e 656c 2064 6965 7320  f a kernel dies 
+00013aa0: 736f 6f6e 2061 6674 6572 2073 7461 7274  soon after start
+00013ab0: 696e 672c 2072 6561 7373 6967 6e20 7261  ing, reassign ra
+00013ac0: 6e64 6f6d 2070 6f72 7473 2062 6566 6f72  ndom ports befor
+00013ad0: 650a 2020 7265 7374 6172 7469 6e67 2069  e.  restarting i
+00013ae0: 742c 2069 6e20 6361 7365 206f 6e65 206f  t, in case one o
+00013af0: 6620 7468 6520 7072 6576 696f 7573 6c79  f the previously
+00013b00: 2063 686f 7365 6e20 706f 7274 7320 6861   chosen ports ha
+00013b10: 7320 6265 656e 0a20 2062 6f75 6e64 2062  s been.  bound b
+00013b20: 7920 616e 6f74 6865 7220 7072 6f63 6573  y another proces
+00013b30: 7320 5b23 3237 395d 2868 7474 7073 3a2f  s [#279](https:/
+00013b40: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00013b50: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00013b60: 6e74 2f70 756c 6c2f 3237 3929 2e0a 2d20  nt/pull/279)..- 
+00013b70: 4176 6f69 6420 756e 6e65 6365 7373 6172  Avoid unnecessar
+00013b80: 7920 6669 6c65 7379 7374 656d 206f 7065  y filesystem ope
+00013b90: 7261 7469 6f6e 7320 7768 656e 2066 696e  rations when fin
+00013ba0: 6469 6e67 2061 206b 6572 6e65 6c73 7065  ding a kernelspe
+00013bb0: 630a 2020 7769 7468 2060 2e4b 6572 6e65  c.  with `.Kerne
+00013bc0: 6c53 7065 634d 616e 6167 6572 2e67 6574  lSpecManager.get
+00013bd0: 5f6b 6572 6e65 6c5f 7370 6563 6020 5b23  _kernel_spec` [#
+00013be0: 3331 315d 2868 7474 7073 3a2f 2f67 6974  311](https://git
+00013bf0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00013c00: 6a75 7079 7465 725f 636c 6965 6e74 2f70  jupyter_client/p
+00013c10: 756c 6c2f 3331 3129 2e0a 2d20 602e 4b65  ull/311)..- `.Ke
+00013c20: 726e 656c 5370 6563 4d61 6e61 6765 722e  rnelSpecManager.
+00013c30: 6765 745f 616c 6c5f 7370 6563 7360 0a20  get_all_specs`. 
+00013c40: 2077 696c 6c20 6e6f 206c 6f6e 6765 7220   will no longer 
+00013c50: 7261 6973 6520 616e 2065 7863 6570 7469  raise an excepti
+00013c60: 6f6e 206f 6e20 656e 636f 756e 7465 7269  on on encounteri
+00013c70: 6e67 2061 6e20 696e 7661 6c69 640a 2020  ng an invalid.  
+00013c80: 606b 6572 6e65 6c2e 6a73 6f6e 6020 6669  `kernel.json` fi
+00013c90: 6c65 2e20 4974 2077 696c 6c20 7261 6973  le. It will rais
+00013ca0: 6520 6120 7761 726e 696e 6720 616e 6420  e a warning and 
+00013cb0: 636f 6e74 696e 7565 0a20 205b 2333 3130  continue.  [#310
+00013cc0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00013cd0: 2e63 6f6d 2f6a 7570 7974 6572 2f6a 7570  .com/jupyter/jup
+00013ce0: 7974 6572 5f63 6c69 656e 742f 7075 6c6c  yter_client/pull
+00013cf0: 2f33 3130 292e 0a2d 2043 6865 636b 2066  /310)..- Check f
+00013d00: 6f72 206e 6f6e 2d63 6f6e 7469 6775 6f75  or non-contiguou
+00013d10: 7320 6275 6666 6572 7320 6265 666f 7265  s buffers before
+00013d20: 2074 7279 696e 6720 746f 2073 656e 6420   trying to send 
+00013d30: 7468 656d 2074 6872 6f75 6768 0a20 205a  them through.  Z
+00013d40: 4d51 205b 2332 3538 5d28 6874 7470 733a  MQ [#258](https:
+00013d50: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+00013d60: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+00013d70: 656e 742f 7075 6c6c 2f32 3538 292e 0a2d  ent/pull/258)..-
+00013d80: 2043 6f6d 7061 7469 6269 6c69 7479 2077   Compatibility w
+00013d90: 6974 6820 7570 636f 6d69 6e67 2054 6f72  ith upcoming Tor
+00013da0: 6e61 646f 2076 6572 7369 6f6e 2035 2e30  nado version 5.0
+00013db0: 0a20 205b 2333 3034 5d28 6874 7470 733a  .  [#304](https:
+00013dc0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+00013dd0: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+00013de0: 656e 742f 7075 6c6c 2f33 3034 292e 0a2d  ent/pull/304)..-
+00013df0: 2053 696d 706c 6966 7920 7365 7475 7020   Simplify setup 
+00013e00: 636f 6465 2062 7920 616c 7761 7973 2075  code by always u
+00013e10: 7369 6e67 2073 6574 7570 746f 6f6c 730a  sing setuptools.
+00013e20: 2020 5b23 3238 345d 2868 7474 7073 3a2f    [#284](https:/
+00013e30: 2f67 6974 6875 622e 636f 6d2f 6a75 7079  /github.com/jupy
+00013e40: 7465 722f 6a75 7079 7465 725f 636c 6965  ter/jupyter_clie
+00013e50: 6e74 2f70 756c 6c2f 3238 3429 2e0a 2d20  nt/pull/284)..- 
+00013e60: 536f 6674 656e 2077 6172 6e69 6e67 7320  Soften warnings 
+00013e70: 7768 656e 2073 6574 7469 6e67 2074 6865  when setting the
+00013e80: 2073 7469 636b 7920 6269 7420 6f6e 2072   sticky bit on r
+00013e90: 756e 7469 6d65 2066 696c 6573 2066 6169  untime files fai
+00013ea0: 6c73 0a20 205b 2332 3836 5d28 6874 7470  ls.  [#286](http
+00013eb0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00013ec0: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
+00013ed0: 6c69 656e 742f 7075 6c6c 2f32 3836 292e  lient/pull/286).
+00013ee0: 0a2d 2056 6172 696f 7573 2063 6f72 7265  .- Various corre
+00013ef0: 6374 696f 6e73 2061 6e64 2069 6d70 726f  ctions and impro
+00013f00: 7665 6d65 6e74 7320 746f 2064 6f63 756d  vements to docum
+00013f10: 656e 7461 7469 6f6e 2e0a 0a23 2320 352e  entation...## 5.
+00013f20: 310a 0a5b 352e 3120 6f6e 0a47 6974 4875  1..[5.1 on.GitHu
+00013f30: 625d 2868 7474 7073 3a2f 2f67 6974 6875  b](https://githu
+00013f40: 622e 636f 6d2f 6a75 7079 7465 722f 6a75  b.com/jupyter/ju
+00013f50: 7079 7465 725f 636c 6965 6e74 2f6d 696c  pyter_client/mil
+00013f60: 6573 746f 6e65 732f 352e 3129 0a0a 2d20  estones/5.1)..- 
+00013f70: 4465 6669 6e65 204a 7570 7974 6572 2070  Define Jupyter p
+00013f80: 726f 746f 636f 6c20 7665 7273 696f 6e20  rotocol version 
+00013f90: 352e 322c 2072 6573 6f6c 7669 6e67 2061  5.2, resolving a
+00013fa0: 6d62 6967 7569 7479 206f 660a 2020 6063  mbiguity of.  `c
+00013fb0: 7572 736f 725f 706f 7360 2066 6965 6c64  ursor_pos` field
+00013fc0: 2069 6e20 7468 6520 7072 6573 656e 6365   in the presence
+00013fd0: 206f 6620 756e 6963 6f64 6520 7375 7272   of unicode surr
+00013fe0: 6f67 6174 6520 7061 6972 732e 0a0a 2020  ogate pairs...  
+00013ff0: 3a3a 3a20 7b2e 7365 6561 6c73 6f7d 0a20  ::: {.seealso}. 
+00014000: 2060 6375 7273 6f72 5f70 6f73 5f75 6e69   `cursor_pos_uni
+00014010: 636f 6465 5f6e 6f74 6560 0a20 203a 3a3a  code_note`.  :::
+00014020: 0a0a 2d20 4164 6420 6053 6573 7369 6f6e  ..- Add `Session
+00014030: 2e63 6c6f 6e65 6020 666f 7220 6d61 6b69  .clone` for maki
+00014040: 6e67 2061 2063 6f70 790a 2020 6f66 2061  ng a copy.  of a
+00014050: 2053 6573 7369 6f6e 206f 626a 6563 7420   Session object 
+00014060: 7769 7468 6f75 7420 7368 6172 696e 6720  without sharing 
+00014070: 7468 6520 6469 6765 7374 2068 6973 746f  the digest histo
+00014080: 7279 2e20 5265 7573 696e 6720 610a 2020  ry. Reusing a.  
+00014090: 7369 6e67 6c65 2053 6573 7369 6f6e 206f  single Session o
+000140a0: 626a 6563 7420 746f 2063 6f6e 6e65 6374  bject to connect
+000140b0: 206d 756c 7469 706c 6520 736f 636b 6574   multiple socket
+000140c0: 7320 746f 2074 6865 2073 616d 6520 494f  s to the same IO
+000140d0: 5075 620a 2020 7065 6572 2063 616e 2063  Pub.  peer can c
+000140e0: 6175 7365 2064 6967 6573 7420 636f 6c6c  ause digest coll
+000140f0: 6973 696f 6e73 2e0a 0a2d 2041 766f 6964  isions...- Avoid
+00014100: 2067 6c6f 6261 6c20 7265 6665 7265 6e63   global referenc
+00014110: 6573 2070 7265 7665 6e74 696e 6720 6761  es preventing ga
+00014120: 7262 6167 6520 636f 6c6c 6563 7469 6f6e  rbage collection
+00014130: 206f 6620 6261 636b 6772 6f75 6e64 0a20   of background. 
+00014140: 2074 6872 6561 6473 2e0a 0a23 2320 352e   threads...## 5.
+00014150: 300a 0a23 2323 2035 2e30 2e31 0a0a 5b35  0..### 5.0.1..[5
+00014160: 2e30 2e31 206f 6e0a 4769 7448 7562 5d28  .0.1 on.GitHub](
+00014170: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00014180: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00014190: 6572 5f63 6c69 656e 742f 6d69 6c65 7374  er_client/milest
+000141a0: 6f6e 6573 2f35 2e30 2e31 290a 0a2d 2055  ones/5.0.1)..- U
+000141b0: 7064 6174 6520 696e 7465 726e 616c 2070  pdate internal p
+000141c0: 726f 746f 636f 6c20 7665 7273 696f 6e20  rotocol version 
+000141d0: 6e75 6d62 6572 2074 6f20 352e 312c 2077  number to 5.1, w
+000141e0: 6869 6368 2073 686f 756c 6420 6861 7665  hich should have
+000141f0: 0a20 2062 6565 6e20 646f 6e65 2069 6e20  .  been done in 
+00014200: 352e 302e 302e 0a0a 2323 2320 352e 302e  5.0.0...### 5.0.
+00014210: 300a 0a5b 352e 302e 3020 6f6e 0a47 6974  0..[5.0.0 on.Git
+00014220: 4875 625d 2868 7474 7073 3a2f 2f67 6974  Hub](https://git
+00014230: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00014240: 6a75 7079 7465 725f 636c 6965 6e74 2f6d  jupyter_client/m
+00014250: 696c 6573 746f 6e65 732f 352e 3029 0a0a  ilestones/5.0)..
+00014260: 4e65 7720 6665 6174 7572 6573 3a0a 0a2d  New features:..-
+00014270: 2049 6d70 6c65 6d65 6e74 204a 7570 7974   Implement Jupyt
+00014280: 6572 2070 726f 746f 636f 6c20 7665 7273  er protocol vers
+00014290: 696f 6e20 352e 312e 0a0a 2d20 496e 7472  ion 5.1...- Intr
+000142a0: 6f64 7563 6520 606a 7570 7974 6572 2072  oduce `jupyter r
+000142b0: 756e 6020 636f 6d6d 616e 640a 2020 666f  un` command.  fo
+000142c0: 7220 7275 6e6e 696e 6720 7363 7269 7074  r running script
+000142d0: 7320 7769 7468 2061 206b 6572 6e65 6c2c  s with a kernel,
+000142e0: 2066 6f72 2069 6e73 7461 6e63 653a 0a0a   for instance:..
+000142f0: 2020 6060 600a 2020 6a75 7079 7465 7220    ```.  jupyter 
+00014300: 7275 6e20 2d2d 6b65 726e 656c 2070 7974  run --kernel pyt
+00014310: 686f 6e33 206d 7973 6372 6970 742e 7079  hon3 myscript.py
+00014320: 0a20 2060 6060 0a0a 2d20 4e65 7720 6d65  .  ```..- New me
+00014330: 7468 6f64 0a20 2060 2e42 6c6f 636b 696e  thod.  `.Blockin
+00014340: 674b 6572 6e65 6c43 6c69 656e 742e 6578  gKernelClient.ex
+00014350: 6563 7574 655f 696e 7465 7261 6374 6976  ecute_interactiv
+00014360: 6560 2066 6f72 2072 756e 6e69 6e67 2063  e` for running c
+00014370: 6f64 6520 616e 6420 6361 7074 7572 696e  ode and capturin
+00014380: 6720 6f72 2072 6564 6973 706c 6179 696e  g or redisplayin
+00014390: 6720 6974 730a 2020 6f75 7470 7574 2e0a  g its.  output..
+000143a0: 0a2d 204e 6577 2060 4b65 726e 656c 4d61  .- New `KernelMa
+000143b0: 6e61 6765 722e 7368 7574 646f 776e 5f77  nager.shutdown_w
+000143c0: 6169 745f 7469 6d65 6020 636f 6e66 6967  ait_time` config
+000143d0: 7572 6162 6c65 2066 6f72 2061 646a 7573  urable for adjus
+000143e0: 7469 6e67 0a20 2074 6865 2074 696d 6520  ting.  the time 
+000143f0: 666f 7220 6120 6b65 726e 656c 206d 616e  for a kernel man
+00014400: 6167 6572 2074 6f20 7761 6974 2061 6674  ager to wait aft
+00014410: 6572 2070 6f6c 6974 656c 7920 7265 7175  er politely requ
+00014420: 6573 7469 6e67 0a20 2073 6875 7464 6f77  esting.  shutdow
+00014430: 6e20 6265 666f 7265 2069 7420 7265 736f  n before it reso
+00014440: 7274 7320 746f 2066 6f72 6365 6675 6c20  rts to forceful 
+00014450: 7465 726d 696e 6174 696f 6e2e 0a0a 4669  termination...Fi
+00014460: 7865 733a 0a0a 2d20 5365 7420 7374 6963  xes:..- Set stic
+00014470: 6b79 2062 6974 206f 6e20 636f 6e6e 6563  ky bit on connec
+00014480: 7469 6f6e 2d66 696c 6520 6469 7265 6374  tion-file direct
+00014490: 6f72 7920 746f 2061 766f 6964 2067 6574  ory to avoid get
+000144a0: 7469 6e67 2063 6c65 616e 6564 0a20 2075  ting cleaned.  u
+000144b0: 702e 0a2d 2060 6a75 7079 7465 725f 636c  p..- `jupyter_cl
+000144c0: 6965 6e74 2e6c 6175 6e63 6865 722e 6c61  ient.launcher.la
+000144d0: 756e 6368 5f6b 6572 6e65 6c60 2070 6173  unch_kernel` pas
+000144e0: 7365 7320 7468 726f 7567 6820 6164 6469  ses through addi
+000144f0: 7469 6f6e 616c 206f 7074 696f 6e73 2074  tional options t
+00014500: 6f20 7468 6520 756e 6465 726c 7969 6e67  o the underlying
+00014510: 0a20 2050 6f70 656e 2c20 6d61 7463 6869  .  Popen, matchi
+00014520: 6e67 2060 4b65 726e 656c 4d61 6e61 6765  ng `KernelManage
+00014530: 722e 7374 6172 745f 6b65 726e 656c 602e  r.start_kernel`.
+00014540: 0a2d 2043 6865 636b 2074 7970 6573 206f  .- Check types o
+00014550: 6620 6062 7566 6665 7273 6020 6172 6775  f `buffers` argu
+00014560: 6d65 6e74 2069 6e0a 2020 602e 5365 7373  ment in.  `.Sess
+00014570: 696f 6e2e 7365 6e64 602c 2073 6f20 7468  ion.send`, so th
+00014580: 6174 2054 7970 6545 7272 6f72 730a 2020  at TypeErrors.  
+00014590: 6172 6520 7261 6973 6564 2069 6d6d 6564  are raised immed
+000145a0: 6961 7465 6c79 2c20 7261 7468 6572 2074  iately, rather t
+000145b0: 6861 6e20 696e 2074 6865 2065 7665 6e74  han in the event
+000145c0: 6c6f 6f70 2e0a 0a43 6861 6e67 6573 3a0a  loop...Changes:.
+000145d0: 0a2d 2049 6e20 6b65 726e 656c 7370 6563  .- In kernelspec
+000145e0: 732c 2069 6620 7468 6520 6578 6563 7574  s, if the execut
+000145f0: 6162 6c65 2069 7320 7468 6520 7374 7269  able is the stri
+00014600: 6e67 2060 7079 7468 6f6e 6020 2861 7320  ng `python` (as 
+00014610: 6f70 706f 7365 640a 2020 746f 2061 6e20  opposed.  to an 
+00014620: 6162 736f 6c75 7465 2070 6174 6829 2c20  absolute path), 
+00014630: 6073 7973 2e65 7865 6375 7461 626c 6560  `sys.executable`
+00014640: 2077 696c 6c20 6265 2075 7365 6420 7261   will be used ra
+00014650: 7468 6572 2074 6861 6e0a 2020 7265 736f  ther than.  reso
+00014660: 6c76 696e 6720 6070 7974 686f 6e60 206f  lving `python` o
+00014670: 6e20 5041 5448 2e20 5468 6973 2073 686f  n PATH. This sho
+00014680: 756c 6420 656e 6162 6c65 2050 7974 686f  uld enable Pytho
+00014690: 6e2d 6261 7365 6420 6b65 726e 656c 730a  n-based kernels.
+000146a0: 2020 746f 2069 6e73 7461 6c6c 206b 6572    to install ker
+000146b0: 6e65 6c73 7065 6373 2061 7320 7061 7274  nelspecs as part
+000146c0: 206f 6620 7768 6565 6c73 2e0a 2d20 6b65   of wheels..- ke
+000146d0: 726e 656c 7370 6563 206e 616d 6573 2061  rnelspec names a
+000146e0: 7265 206e 6f77 2076 616c 6964 6174 6564  re now validated
+000146f0: 2e20 5468 6579 2073 686f 756c 6420 6f6e  . They should on
+00014700: 6c79 2069 6e63 6c75 6465 2061 7363 6969  ly include ascii
+00014710: 0a20 206c 6574 7465 7273 2061 6e64 206e  .  letters and n
+00014720: 756d 6265 7273 2c20 706c 7573 2070 6572  umbers, plus per
+00014730: 696f 642c 2068 7970 6865 6e2c 2061 6e64  iod, hyphen, and
+00014740: 2075 6e64 6572 7363 6f72 652e 0a0a 4261   underscore...Ba
+00014750: 636b 7761 7264 2d69 6e63 6f6d 7061 7469  ckward-incompati
+00014760: 626c 6520 6368 616e 6765 733a 0a0a 2d20  ble changes:..- 
+00014770: 3a70 7960 2e64 6174 6574 696d 6560 206f  :py`.datetime` o
+00014780: 626a 6563 7473 2072 6574 7572 6e65 6420  bjects returned 
+00014790: 696e 0a20 2070 6172 7365 6420 6d65 7373  in.  parsed mess
+000147a0: 6167 6573 2061 7265 206e 6f77 2061 6c77  ages are now alw
+000147b0: 6179 7320 7469 6d65 7a6f 6e65 2d61 7761  ays timezone-awa
+000147c0: 7265 2e20 5469 6d65 7374 616d 7073 2069  re. Timestamps i
+000147d0: 6e0a 2020 6d65 7373 6167 6573 2077 6974  n.  messages wit
+000147e0: 686f 7574 2074 696d 657a 6f6e 6520 696e  hout timezone in
+000147f0: 666f 2061 7265 2069 6e74 6572 7072 6574  fo are interpret
+00014800: 6564 2061 7320 7468 6520 6c6f 6361 6c0a  ed as the local.
+00014810: 2020 7469 6d65 7a6f 6e65 2c20 6173 2074    timezone, as t
+00014820: 6869 7320 7761 7320 7468 6520 6265 6861  his was the beha
+00014830: 7669 6f72 2069 6e20 6561 726c 6965 7220  vior in earlier 
+00014840: 7665 7273 696f 6e73 2e0a 0a23 2320 342e  versions...## 4.
+00014850: 340a 0a23 2323 2034 2e34 2e30 0a0a 5b34  4..### 4.4.0..[4
+00014860: 2e34 206f 6e0a 4769 7448 7562 5d28 6874  .4 on.GitHub](ht
+00014870: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00014880: 2f6a 7570 7974 6572 2f6a 7570 7974 6572  /jupyter/jupyter
+00014890: 5f63 6c69 656e 742f 6d69 6c65 7374 6f6e  _client/mileston
+000148a0: 6573 2f34 2e34 290a 0a2d 2041 6464 2060  es/4.4)..- Add `
+000148b0: 2e4b 6572 6e65 6c43 6c69 656e 742e 6c6f  .KernelClient.lo
+000148c0: 6164 5f63 6f6e 6e65 6374 696f 6e5f 696e  ad_connection_in
+000148d0: 666f 6020 6f6e 204b 6572 6e65 6c43 6c69  fo` on KernelCli
+000148e0: 656e 742c 2065 7463 2e20 666f 7220 6c6f  ent, etc. for lo
+000148f0: 6164 696e 6720 636f 6e6e 6563 7469 6f6e  ading connection
+00014900: 2069 6e66 6f0a 2020 6469 7265 6374 6c79   info.  directly
+00014910: 2066 726f 6d20 6120 6469 6374 2c20 6e6f   from a dict, no
+00014920: 7420 6a75 7374 2066 726f 6d20 6669 6c65  t just from file
+00014930: 732e 0a2d 2049 6e63 6c75 6465 2070 6172  s..- Include par
+00014940: 656e 7420 6865 6164 6572 7320 7768 656e  ent headers when
+00014950: 2061 6461 7074 696e 6720 6d65 7373 6167   adapting messag
+00014960: 6573 2066 726f 6d20 6f6c 6465 7220 7072  es from older pr
+00014970: 6f74 6f63 6f6c 0a20 2069 6d70 6c65 6d65  otocol.  impleme
+00014980: 6e74 6174 696f 6e73 2028 7472 6561 7473  ntations (treats
+00014990: 2070 6172 656e 7420 6865 6164 6572 7320   parent headers 
+000149a0: 7468 6520 7361 6d65 2061 7320 6865 6164  the same as head
+000149b0: 6572 7329 2e0a 2d20 436f 6d70 6174 6962  ers)..- Compatib
+000149c0: 696c 6974 7920 6669 7865 7320 696e 2074  ility fixes in t
+000149d0: 6573 7473 2066 6f72 2072 6563 656e 7420  ests for recent 
+000149e0: 6368 616e 6765 7320 696e 2069 7079 6b65  changes in ipyke
+000149f0: 726e 656c 2e0a 0a23 2320 342e 330a 0a23  rnel...## 4.3..#
+00014a00: 2323 2034 2e33 2e30 0a0a 5b34 2e33 206f  ## 4.3.0..[4.3 o
+00014a10: 6e0a 4769 7448 7562 5d28 6874 7470 733a  n.GitHub](https:
+00014a20: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7570  //github.com/jup
+00014a30: 7974 6572 2f6a 7570 7974 6572 5f63 6c69  yter/jupyter_cli
+00014a40: 656e 742f 6d69 6c65 7374 6f6e 6573 2f34  ent/milestones/4
+00014a50: 2e33 290a 0a2d 2041 6464 7320 602d 2d73  .3)..- Adds `--s
+00014a60: 7973 2d70 7265 6669 7860 2061 7267 756d  ys-prefix` argum
+00014a70: 656e 7420 746f 0a20 2060 6a75 7079 7465  ent to.  `jupyte
+00014a80: 7220 6b65 726e 656c 7370 6563 2069 6e73  r kernelspec ins
+00014a90: 7461 6c6c 602c 2066 6f72 0a20 2062 6574  tall`, for.  bet
+00014aa0: 7465 7220 7379 6d6d 6574 7279 2077 6974  ter symmetry wit
+00014ab0: 6820 606a 7570 7974 6572 206e 6265 7874  h `jupyter nbext
+00014ac0: 656e 7369 6f6e 2069 6e73 7461 6c6c 602c  ension install`,
+00014ad0: 2065 7463 2e0a 0a23 2320 342e 320a 0a23   etc...## 4.2..#
+00014ae0: 2323 2034 2e32 2e32 0a0a 5b34 2e32 2e32  ## 4.2.2..[4.2.2
+00014af0: 206f 6e0a 4769 7448 7562 5d28 6874 7470   on.GitHub](http
+00014b00: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00014b10: 7570 7974 6572 2f6a 7570 7974 6572 5f63  upyter/jupyter_c
+00014b20: 6c69 656e 742f 6d69 6c65 7374 6f6e 6573  lient/milestones
+00014b30: 2f34 2e32 2e32 290a 0a2d 2041 6e6f 7468  /4.2.2)..- Anoth
+00014b40: 6572 2066 6978 2066 6f72 2074 6865 2060  er fix for the `
+00014b50: 7374 6172 745f 6e65 775f 6b65 726e 656c  start_new_kernel
+00014b60: 6020 6973 7375 6520 696e 2034 2e32 2e31  ` issue in 4.2.1
+00014b70: 2061 6666 6563 7469 6e67 2073 6c6f 772d   affecting slow-
+00014b80: 7374 6172 7469 6e67 206b 6572 6e65 6c73  starting kernels
+00014b90: 2e0a 0a23 2323 2034 2e32 2e31 0a0a 5b34  ...### 4.2.1..[4
+00014ba0: 2e32 2e31 206f 6e0a 4769 7448 7562 5d28  .2.1 on.GitHub](
+00014bb0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00014bc0: 6f6d 2f6a 7570 7974 6572 2f6a 7570 7974  om/jupyter/jupyt
+00014bd0: 6572 5f63 6c69 656e 742f 6d69 6c65 7374  er_client/milest
+00014be0: 6f6e 6573 2f34 2e32 2e31 290a 0a2d 2046  ones/4.2.1)..- F
+00014bf0: 6978 2072 6567 7265 7373 696f 6e20 696e  ix regression in
+00014c00: 2034 2e32 2063 6175 7369 6e67 2060 7374   4.2 causing `st
+00014c10: 6172 745f 6e65 775f 6b65 726e 656c 6020  art_new_kernel` 
+00014c20: 746f 2066 6169 6c20 7768 696c 6520 7761  to fail while wa
+00014c30: 6974 696e 6720 666f 7220 6b65 726e 656c  iting for kernel
+00014c40: 7320 746f 2062 6563 6f6d 6520 6176 6169  s to become avai
+00014c50: 6c61 626c 652e 0a0a 2323 2320 342e 322e  lable...### 4.2.
+00014c60: 300a 0a5b 342e 322e 3020 6f6e 0a47 6974  0..[4.2.0 on.Git
+00014c70: 4875 625d 2868 7474 7073 3a2f 2f67 6974  Hub](https://git
+00014c80: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00014c90: 6a75 7079 7465 725f 636c 6965 6e74 2f6d  jupyter_client/m
+00014ca0: 696c 6573 746f 6e65 732f 342e 3229 0a0a  ilestones/4.2)..
+00014cb0: 2d20 6164 6465 6420 606a 7570 7974 6572  - added `jupyter
+00014cc0: 206b 6572 6e65 6c73 7065 6320 7265 6d6f   kernelspec remo
+00014cd0: 7665 600a 2020 666f 7220 7265 6d6f 7669  ve`.  for removi
+00014ce0: 6e67 206b 6572 6e65 6c73 7065 6373 0a2d  ng kernelspecs.-
+00014cf0: 2061 6c6c 6f77 2073 7065 6369 6679 696e   allow specifyin
+00014d00: 6720 7468 6520 656e 7669 726f 6e6d 656e  g the environmen
+00014d10: 7420 666f 7220 6b65 726e 656c 2070 726f  t for kernel pro
+00014d20: 6365 7373 6573 2076 6961 2074 6865 2060  cesses via the `
+00014d30: 656e 7660 0a20 2061 7267 756d 656e 740a  env`.  argument.
+00014d40: 2d20 6164 6465 6420 606e 616d 6560 2066  - added `name` f
+00014d50: 6965 6c64 2074 6f20 636f 6e6e 6563 7469  ield to connecti
+00014d60: 6f6e 2066 696c 6573 2069 6465 6e74 6966  on files identif
+00014d70: 7969 6e67 2074 6865 206b 6572 6e65 6c73  ying the kernels
+00014d80: 7065 630a 2020 6e61 6d65 2c20 736f 2074  pec.  name, so t
+00014d90: 6861 7420 636f 6e73 756d 6572 7320 6f66  hat consumers of
+00014da0: 2063 6f6e 6e65 6374 696f 6e20 6669 6c65   connection file
+00014db0: 7320 2861 6c74 6572 6e61 7465 2066 726f  s (alternate fro
+00014dc0: 6e74 656e 6473 290a 2020 6361 6e20 6964  ntends).  can id
+00014dd0: 656e 7469 6679 2074 6865 206b 6572 6e65  entify the kerne
+00014de0: 6c73 7065 6320 696e 2075 7365 0a2d 2061  lspec in use.- a
+00014df0: 6464 6564 2060 4b65 726e 656c 5370 6563  dded `KernelSpec
+00014e00: 4d61 6e61 6765 722e 6765 745f 616c 6c5f  Manager.get_all_
+00014e10: 7370 6563 7360 2066 6f72 2067 6574 7469  specs` for getti
+00014e20: 6e67 2061 6c6c 206b 6572 6e65 6c73 7065  ng all kernelspe
+00014e30: 6373 206d 6f72 6520 6566 6669 6369 656e  cs more efficien
+00014e40: 746c 790a 2d20 7661 7269 6f75 7320 696d  tly.- various im
+00014e50: 7072 6f76 656d 656e 7473 2074 6f20 6572  provements to er
+00014e60: 726f 7220 6d65 7373 6167 6573 2061 6e64  ror messages and
+00014e70: 2064 6f63 756d 656e 7461 7469 6f6e 0a0a   documentation..
+00014e80: 2323 2034 2e31 0a0a 2323 2320 342e 312e  ## 4.1..### 4.1.
+00014e90: 300a 0a5b 342e 312e 3020 6f6e 0a47 6974  0..[4.1.0 on.Git
+00014ea0: 4875 625d 2868 7474 7073 3a2f 2f67 6974  Hub](https://git
+00014eb0: 6875 622e 636f 6d2f 6a75 7079 7465 722f  hub.com/jupyter/
+00014ec0: 6a75 7079 7465 725f 636c 6965 6e74 2f6d  jupyter_client/m
+00014ed0: 696c 6573 746f 6e65 732f 342e 3129 0a0a  ilestones/4.1)..
+00014ee0: 4869 6768 6c69 6768 7473 3a0a 0a2d 2053  Highlights:..- S
+00014ef0: 6574 7570 746f 6f6c 7320 6669 7865 7320  etuptools fixes 
+00014f00: 666f 7220 606a 7570 7974 6572 206b 6572  for `jupyter ker
+00014f10: 6e65 6c73 7065 6360 0a2d 2060 6a75 7079  nelspec`.- `jupy
+00014f20: 7465 7220 6b65 726e 656c 7370 6563 206c  ter kernelspec l
+00014f30: 6973 7460 2069 6e63 6c75 6465 7320 7061  ist` includes pa
+00014f40: 7468 730a 2d20 6164 6420 604b 6572 6e65  ths.- add `Kerne
+00014f50: 6c4d 616e 6167 6572 2e62 6c6f 636b 696e  lManager.blockin
+00014f60: 675f 636c 6965 6e74 600a 2d20 7072 6f76  g_client`.- prov
+00014f70: 6973 696f 6e61 6c20 696d 706c 656d 656e  isional implemen
+00014f80: 7461 7469 6f6e 206f 6620 6063 6f6d 6d5f  tation of `comm_
+00014f90: 696e 666f 6020 7265 7175 6573 7473 2066  info` requests f
+00014fa0: 726f 6d20 7570 636f 6d69 6e67 2035 2e31  rom upcoming 5.1
+00014fb0: 0a20 2072 656c 6561 7365 206f 6620 7468  .  release of th
+00014fc0: 6520 7072 6f74 6f63 6f6c 0a0a 2323 2034  e protocol..## 4
+00014fd0: 2e30 0a0a 5468 6520 6669 7273 7420 7265  .0..The first re
+00014fe0: 6c65 6173 6520 6f66 204a 7570 7974 6572  lease of Jupyter
+00014ff0: 2043 6c69 656e 7420 6173 2069 7473 206f   Client as its o
+00015000: 776e 2070 6163 6b61 6765 2e0a            wn package..
```

### Comparing `jupyter_client-8.6.0/RELEASING.md` & `jupyter_client-8.6.1/RELEASING.md`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/.github/workflows/downstream.yml` & `jupyter_client-8.6.1/.github/workflows/downstream.yml`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
       - name: Checkout
         uses: actions/checkout@v4
 
       - name: Base Setup
         uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
 
       - name: Setup conda ${{ matrix.python-version }}
-        uses: conda-incubator/setup-miniconda@v2
+        uses: conda-incubator/setup-miniconda@v3
         with:
           auto-update-conda: true
           activate-environment: jupyter_kernel_test
           miniforge-variant: Mambaforge
           python-version: ${{ matrix.python-version }}
 
       - name: Test jupyter_kernel_test
@@ -93,15 +93,15 @@
     runs-on: ubuntu-latest
     timeout-minutes: 20
     steps:
       - name: Checkout
         uses: actions/checkout@v4
 
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.9"
           architecture: "x64"
 
       - name: Install System Packages
         run: |
           sudo apt-get update
```

### Comparing `jupyter_client-8.6.0/.github/workflows/main.yml` & `jupyter_client-8.6.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/.github/workflows/prep-release.yml` & `jupyter_client-8.6.1/.github/workflows/prep-release.yml`

 * *Files 10% similar despite different names*

```diff
@@ -8,33 +8,40 @@
         required: false
       branch:
         description: "The branch to target"
         required: false
       post_version_spec:
         description: "Post Version Specifier"
         required: false
+      silent:
+        description: "Set a placeholder in the changelog and don't publish the release."
+        required: false
+        type: boolean
       since:
         description: "Use PRs with activity since this date or git reference"
         required: false
       since_last_stable:
         description: "Use PRs with activity since the last stable git tag"
         required: false
         type: boolean
 jobs:
   prep_release:
     runs-on: ubuntu-latest
+    permissions:
+      contents: write
     steps:
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
 
       - name: Prep Release
         id: prep-release
         uses: jupyter-server/jupyter_releaser/.github/actions/prep-release@v2
         with:
-          token: ${{ secrets.ADMIN_GITHUB_TOKEN }}
+          token: ${{ secrets.GITHUB_TOKEN }}
           version_spec: ${{ github.event.inputs.version_spec }}
+          silent: ${{ github.event.inputs.silent }}
           post_version_spec: ${{ github.event.inputs.post_version_spec }}
           target: ${{ github.event.inputs.target }}
           branch: ${{ github.event.inputs.branch }}
           since: ${{ github.event.inputs.since }}
           since_last_stable: ${{ github.event.inputs.since_last_stable }}
 
       - name: "** Next Step **"
```

### Comparing `jupyter_client-8.6.0/.github/workflows/publish-release.yml` & `jupyter_client-8.6.1/.github/workflows/publish-release.yml`

 * *Files 12% similar despite different names*

```diff
@@ -11,38 +11,40 @@
       steps_to_skip:
         description: "Comma separated list of steps to skip"
         required: false
 
 jobs:
   publish_release:
     runs-on: ubuntu-latest
+    environment: release
+    permissions:
+      id-token: write
     steps:
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
 
+      - uses: actions/create-github-app-token@v1
+        id: app-token
+        with:
+          app-id: ${{ vars.APP_ID }}
+          private-key: ${{ secrets.APP_PRIVATE_KEY }}
+
       - name: Populate Release
         id: populate-release
         uses: jupyter-server/jupyter_releaser/.github/actions/populate-release@v2
         with:
-          token: ${{ secrets.ADMIN_GITHUB_TOKEN }}
-          target: ${{ github.event.inputs.target }}
+          token: ${{ steps.app-token.outputs.token }}
           branch: ${{ github.event.inputs.branch }}
           release_url: ${{ github.event.inputs.release_url }}
           steps_to_skip: ${{ github.event.inputs.steps_to_skip }}
 
       - name: Finalize Release
         id: finalize-release
-        env:
-          PYPI_TOKEN: ${{ secrets.PYPI_TOKEN }}
-          PYPI_TOKEN_MAP: ${{ secrets.PYPI_TOKEN_MAP }}
-          TWINE_USERNAME: __token__
-          NPM_TOKEN: ${{ secrets.NPM_TOKEN }}
-        uses: jupyter-server/jupyter-releaser/.github/actions/finalize-release@v2
+        uses: jupyter-server/jupyter_releaser/.github/actions/finalize-release@v2
         with:
-          token: ${{ secrets.ADMIN_GITHUB_TOKEN }}
-          target: ${{ github.event.inputs.target }}
+          token: ${{ steps.app-token.outputs.token }}
           release_url: ${{ steps.populate-release.outputs.release_url }}
 
       - name: "** Next Step **"
         if: ${{ success() }}
         run: |
           echo "Verify the final release"
           echo ${{ steps.finalize-release.outputs.release_url }}
```

### Comparing `jupyter_client-8.6.0/docs/Makefile` & `jupyter_client-8.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/docs/conf.py` & `jupyter_client-8.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/docs/index.rst` & `jupyter_client-8.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/docs/kernels.rst` & `jupyter_client-8.6.1/docs/kernels.rst`

 * *Files 5% similar despite different names*

```diff
@@ -180,7 +180,25 @@
 To start the terminal console or the Qt console with a specific kernel::
 
     jupyter console --kernel bash
     jupyter qtconsole --kernel bash
 
 The notebook offers you the available kernels in a dropdown menu from the 'New'
 button.
+
+
+.. _packaging-kernels:
+
+Packaging
+=========
+
+To release your kernel as a Python package, we recommend following the pattern
+used in the `echo_kernel`_, which uses the `hatch`_  build backend and
+a build file that creates the kernel directory with the ``kernel.json`` and
+kernel icons, which is included as ``shared-data``, ending up in the
+``share/jupyter/kernels/`` folder in the user's installed environment.
+See `pyproject.toml`_ and `hatch_build.py`_ for more details.
+
+.. _hatch: https://hatch.pypa.io/latest/
+.. _pyproject.toml: https://github.com/jupyter/echo_kernel/blob/main/pyproject.toml
+.. _hatch_build.py: https://github.com/jupyter/echo_kernel/blob/main/hatch_build.py
+.. _echo_kernel: https://github.com/jupyter/echo_kernel
```

### Comparing `jupyter_client-8.6.0/docs/make.bat` & `jupyter_client-8.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/docs/messaging.rst` & `jupyter_client-8.6.1/docs/messaging.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1045,14 +1045,23 @@
 - when the user chooses to close the client application via a menu or window
   control.
 - when the user types 'exit' or 'quit' (or their uppercase magic equivalents).
 - when the user chooses a GUI method (like the 'Ctrl-C' shortcut in the
   IPythonQt client) to force a kernel restart to get a clean kernel without
   losing client-side state like history or inlined figures.
 
+Implementation recommendation for starting kernels: A restart should optimally
+preserve as many resources outside the kernel as possible (e.g. only restart the
+kernel and its subprocesses and not any parent processes). That is, ideally a
+restart should be "in-place". For local kernels, there is typically no parent
+process so a "hard" restart and an in-place restart are identical whereas for
+remote kernels this is not generally the same. As an example, if a remote kernel
+is run in a container, during an in-place restart the container may be kept
+running and a new kernel process within it would be started.
+
 The client sends a shutdown request to the kernel, and once it receives the
 reply message (which is otherwise empty), it can assume that the kernel has
 completed shutdown safely.  The request is sent on the ``control`` channel.
 
 Upon their own shutdown, client applications will typically execute a last
 minute sanity check and forcefully terminate any kernel that is still alive, to
 avoid leaving stray processes in the user's machine.
```

### Comparing `jupyter_client-8.6.0/docs/migration.md` & `jupyter_client-8.6.1/docs/migration.md`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/docs/pending-kernels.rst` & `jupyter_client-8.6.1/docs/pending-kernels.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/docs/provisioning.rst` & `jupyter_client-8.6.1/docs/provisioning.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/docs/wrapperkernels.rst` & `jupyter_client-8.6.1/docs/wrapperkernels.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 The `Metakernel <https://github.com/Calysto/metakernel/#>`_ library makes it easier to
 write a wrapper kernel that includes a base set of line and cell magics.  It
 also has a ``ProcessKernel`` subclass that makes it easy to write kernels that
 use ``pexpect``.
 See `Octave Kernel <https://github.com/Calysto/octave_kernel>`_ as an example.
 
+If releasing a wrapper kernel as a Python package, see the steps in :ref:`packaging-kernels`.
 
 Required steps
 --------------
 
 Subclass :class:`ipykernel.kernelbase.Kernel`, and implement the
 following methods and attributes:
 
@@ -82,15 +83,15 @@
 Now create a `JSON kernel spec file <https://jupyter-client.readthedocs.io/en/latest/kernels.html#kernel-specs>`_ and install it using ``jupyter kernelspec install </path/to/kernel>``. Place your kernel module anywhere Python can import it (try current directory for testing). Finally, you can run your kernel using ``jupyter console --kernel <mykernelname>``. Note that ``<mykernelname>`` in the below example is ``echo``.
 
 Example
 -------
 
 .. seealso::
 
-    `echo_kernel <https://github.com/jupyter/echo_kernel>`__
+    `echo_kernel <https://github.com/jupyter/echo_kernel>`_
       A packaged, installable version of the condensed example below.
 
 ``echokernel.py`` will simply echo any input it's given to stdout::
 
     from ipykernel.kernelbase import Kernel
 
     class EchoKernel(Kernel):
```

### Comparing `jupyter_client-8.6.0/docs/api/jupyter_client.provisioning.rst` & `jupyter_client-8.6.1/docs/api/jupyter_client.provisioning.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/docs/api/jupyter_client.rst` & `jupyter_client-8.6.1/docs/api/jupyter_client.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/docs/figs/frontend-kernel.png` & `jupyter_client-8.6.1/docs/figs/frontend-kernel.png`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/docs/figs/frontend-kernel.svg` & `jupyter_client-8.6.1/docs/figs/frontend-kernel.svg`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/__init__.py` & `jupyter_client-8.6.1/jupyter_client/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/_version.py` & `jupyter_client-8.6.1/jupyter_client/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The version information for jupyter client."""
 import re
 from typing import List, Union
 
-__version__ = "8.6.0"
+__version__ = "8.6.1"
 
 # Build up version_info tuple for backwards compatibility
 pattern = r"(?P<major>\d+).(?P<minor>\d+).(?P<patch>\d+)(?P<rest>.*)"
 match = re.match(pattern, __version__)
 if match:
     parts: List[Union[int, str]] = [int(match[part]) for part in ["major", "minor", "patch"]]
     if match["rest"]:
```

### Comparing `jupyter_client-8.6.0/jupyter_client/adapter.py` & `jupyter_client-8.6.1/jupyter_client/adapter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/channels.py` & `jupyter_client-8.6.1/jupyter_client/channels.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/channelsabc.py` & `jupyter_client-8.6.1/jupyter_client/channelsabc.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/client.py` & `jupyter_client-8.6.1/jupyter_client/client.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/clientabc.py` & `jupyter_client-8.6.1/jupyter_client/clientabc.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/connect.py` & `jupyter_client-8.6.1/jupyter_client/connect.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/consoleapp.py` & `jupyter_client-8.6.1/jupyter_client/consoleapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/jsonutil.py` & `jupyter_client-8.6.1/jupyter_client/jsonutil.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/kernelapp.py` & `jupyter_client-8.6.1/jupyter_client/kernelapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/kernelspec.py` & `jupyter_client-8.6.1/jupyter_client/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/kernelspecapp.py` & `jupyter_client-8.6.1/jupyter_client/kernelspecapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/launcher.py` & `jupyter_client-8.6.1/jupyter_client/launcher.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/localinterfaces.py` & `jupyter_client-8.6.1/jupyter_client/localinterfaces.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/manager.py` & `jupyter_client-8.6.1/jupyter_client/manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/managerabc.py` & `jupyter_client-8.6.1/jupyter_client/managerabc.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/multikernelmanager.py` & `jupyter_client-8.6.1/jupyter_client/multikernelmanager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/restarter.py` & `jupyter_client-8.6.1/jupyter_client/restarter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/runapp.py` & `jupyter_client-8.6.1/jupyter_client/runapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/session.py` & `jupyter_client-8.6.1/jupyter_client/session.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/threaded.py` & `jupyter_client-8.6.1/jupyter_client/threaded.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/utils.py` & `jupyter_client-8.6.1/jupyter_client/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/win_interrupt.py` & `jupyter_client-8.6.1/jupyter_client/win_interrupt.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/asynchronous/client.py` & `jupyter_client-8.6.1/jupyter_client/asynchronous/client.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/blocking/client.py` & `jupyter_client-8.6.1/jupyter_client/blocking/client.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/ioloop/manager.py` & `jupyter_client-8.6.1/jupyter_client/ioloop/manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/ioloop/restarter.py` & `jupyter_client-8.6.1/jupyter_client/ioloop/restarter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/provisioning/factory.py` & `jupyter_client-8.6.1/jupyter_client/provisioning/factory.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/provisioning/local_provisioner.py` & `jupyter_client-8.6.1/jupyter_client/provisioning/local_provisioner.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/provisioning/provisioner_base.py` & `jupyter_client-8.6.1/jupyter_client/provisioning/provisioner_base.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/ssh/forward.py` & `jupyter_client-8.6.1/jupyter_client/ssh/forward.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/jupyter_client/ssh/tunnel.py` & `jupyter_client-8.6.1/jupyter_client/ssh/tunnel.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/problemkernel.py` & `jupyter_client-8.6.1/tests/problemkernel.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/signalkernel.py` & `jupyter_client-8.6.1/tests/signalkernel.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_adapter.py` & `jupyter_client-8.6.1/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_client.py` & `jupyter_client-8.6.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_connect.py` & `jupyter_client-8.6.1/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_consoleapp.py` & `jupyter_client-8.6.1/tests/test_consoleapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_jsonutil.py` & `jupyter_client-8.6.1/tests/test_jsonutil.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_kernelapp.py` & `jupyter_client-8.6.1/tests/test_kernelapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_kernelmanager.py` & `jupyter_client-8.6.1/tests/test_kernelmanager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_kernelspec.py` & `jupyter_client-8.6.1/tests/test_kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_kernelspecapp.py` & `jupyter_client-8.6.1/tests/test_kernelspecapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def test_kernelspec_sub_apps(jp_kernel_dir):
     app = InstallKernelSpec()
     prefix = os.path.dirname(os.environ["JUPYTER_DATA_DIR"])
     kernel_dir = os.path.join(prefix, "share/jupyter/kernels")
     app.kernel_spec_manager.kernel_dirs.append(kernel_dir)
-    app.prefix = prefix = prefix
+    app.prefix = prefix
     app.initialize([str(jp_kernel_dir)])
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         app.start()
 
     app1 = ListKernelSpecs()
     app1.kernel_spec_manager.kernel_dirs.append(kernel_dir)
```

### Comparing `jupyter_client-8.6.0/tests/test_localinterfaces.py` & `jupyter_client-8.6.1/tests/test_localinterfaces.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_manager.py` & `jupyter_client-8.6.1/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_multikernelmanager.py` & `jupyter_client-8.6.1/tests/test_multikernelmanager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_provisioning.py` & `jupyter_client-8.6.1/tests/test_provisioning.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_public_api.py` & `jupyter_client-8.6.1/tests/test_public_api.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_restarter.py` & `jupyter_client-8.6.1/tests/test_restarter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/test_session.py` & `jupyter_client-8.6.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/tests/utils.py` & `jupyter_client-8.6.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/LICENSE` & `jupyter_client-8.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/README.md` & `jupyter_client-8.6.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.6.0/pyproject.toml` & `jupyter_client-8.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,18 @@
 [tool.hatch.envs.typing.scripts]
 test = "pre-commit run --all-files --hook-stage manual mypy"
 
 [tool.hatch.envs.lint]
 dependencies = ["pre-commit"]
 detached = true
 [tool.hatch.envs.lint.scripts]
-build = ["pre-commit run --all-files ruff"]
+build = [
+  "pre-commit run --all-files ruff",
+  "pre-commit run --all-files ruff-format"
+]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 xfail_strict = true
 log_cli_level = "info"
 addopts = [
   "-raXs", "--durations=10", "--color=yes", "--doctest-modules",
@@ -158,20 +161,18 @@
 python_version = "3.8"
 strict = true
 disallow_any_generics = false
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 no_implicit_reexport = false
 pretty = true
 show_error_context = true
-show_error_codes = true
 warn_return_any = false
 warn_unreachable = true
 
 [tool.ruff]
-target-version = "py38"
 line-length = 100
 
 [tool.ruff.lint]
 select = [
   "A",
   "B",
   "C",
@@ -274,8 +275,8 @@
 ignore-property-decorators=true
 ignore-nested-functions=true
 ignore-nested-classes=true
 fail-under=90
 exclude = ["docs", "test"]
 
 [tool.repo-review]
-ignore = ["PY007", "PP308", "GH102"]
+ignore = ["GH102"]
```

### Comparing `jupyter_client-8.6.0/PKG-INFO` & `jupyter_client-8.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_client
-Version: 8.6.0
+Version: 8.6.1
 Summary: Jupyter protocol implementation and client libraries
 Project-URL: Homepage, https://jupyter.org
 Project-URL: Documentation, https://jupyter-client.readthedocs.io/
 Project-URL: Source, https://github.com/jupyter/jupyter_client
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -63,15 +63,15 @@
 Requires-Dist: sphinx>=4; extra == 'docs'
 Requires-Dist: sphinxcontrib-github-alt; extra == 'docs'
 Requires-Dist: sphinxcontrib-spelling; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: ipykernel>=6.14; extra == 'test'
 Requires-Dist: mypy; extra == 'test'
-Requires-Dist: paramiko; sys_platform == 'win32' and extra == 'test'
+Requires-Dist: paramiko; (sys_platform == 'win32') and extra == 'test'
 Requires-Dist: pre-commit; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-jupyter[client]>=0.4.1; extra == 'test'
 Requires-Dist: pytest-timeout; extra == 'test'
 Description-Content-Type: text/markdown
```

