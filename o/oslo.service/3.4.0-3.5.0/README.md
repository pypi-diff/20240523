# Comparing `tmp/oslo.service-3.4.0.tar.gz` & `tmp/oslo.service-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslo.service-3.4.0.tar", last modified: Thu Feb 22 14:25:40 2024, max compression
+gzip compressed data, was "oslo.service-3.5.0.tar", last modified: Thu May 23 08:17:24 2024, max compression
```

## Comparing `oslo.service-3.4.0.tar` & `oslo.service-3.5.0.tar`

### file list

```diff
@@ -1,131 +1,132 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.280123 oslo.service-3.4.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-02-22 14:25:12.000000 oslo.service-3.4.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-02-22 14:25:12.000000 oslo.service-3.4.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1059 2024-02-22 14:25:12.000000 oslo.service-3.4.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-02-22 14:25:12.000000 oslo.service-3.4.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-02-22 14:25:12.000000 oslo.service-3.4.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6162 2024-02-22 14:25:40.000000 oslo.service-3.4.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      726 2024-02-22 14:25:12.000000 oslo.service-3.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23761 2024-02-22 14:25:40.000000 oslo.service-3.4.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-02-22 14:25:12.000000 oslo.service-3.4.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-02-22 14:25:12.000000 oslo.service-3.4.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2492 2024-02-22 14:25:40.280123 oslo.service-3.4.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1261 2024-02-22 14:25:12.000000 oslo.service-3.4.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2566 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/reference/eventlet_backdoor.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/reference/fixture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/reference/loopingcall.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/reference/periodic_task.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/reference/service.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/reference/sslutils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/reference/systemd.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/reference/threadgroup.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7991 2024-02-22 14:25:12.000000 oslo.service-3.4.0/doc/source/user/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/oslo.service.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2492 2024-02-22 14:25:40.000000 oslo.service-3.4.0/oslo.service.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3501 2024-02-22 14:25:40.000000 oslo.service-3.4.0/oslo.service.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 14:25:40.000000 oslo.service-3.4.0/oslo.service.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-02-22 14:25:40.000000 oslo.service-3.4.0/oslo.service.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 14:25:40.000000 oslo.service-3.4.0/oslo.service.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-22 14:25:40.000000 oslo.service-3.4.0/oslo.service.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-02-22 14:25:40.000000 oslo.service-3.4.0/oslo.service.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-02-22 14:25:40.000000 oslo.service-3.4.0/oslo.service.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.276123 oslo.service-3.4.0/oslo_service/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5802 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/_options.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9496 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/eventlet_backdoor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/fixture.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/oslo_service/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/oslo_service/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.276123 oslo.service-3.4.0/oslo_service/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4478 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/locale/en_GB/LC_MESSAGES/oslo_service.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18140 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/loopingcall.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8175 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/periodic_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29468 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/sslutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3101 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/systemd.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.276123 oslo.service-3.4.0/oslo_service/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1339 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2659 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5109 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/eventlet_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.276123 oslo.service-3.4.0/oslo_service/tests/ssl_cert/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/ssl_cert/ca.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1679 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/ssl_cert/ca.key
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1184 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/ssl_cert/certificate.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1679 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/ssl_cert/privatekey.key
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7940 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/test_eventlet_backdoor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/test_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16175 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/test_loopingcall.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13818 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/test_periodic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26685 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5769 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/test_sslutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2580 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/test_systemd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6195 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/test_threadgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14419 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/tests/test_wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18025 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/threadgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12496 2024-02-22 14:25:12.000000 oslo.service-3.4.0/oslo_service/wsgi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.276123 oslo.service-3.4.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/notes/add-timeout-looping-call-5cc396b75597c3c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/notes/add-wsgi_server_debug-opt-70d818b5b78bfc7c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/notes/add_reno-3b4ae0789e9c45b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/notes/drop-python27-support-1cfdf65193a03f3a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/notes/fix-find-object-in-backdoor-487bf78c4c502594.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/notes/native-threads-on-child-7150690c7caa1013.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/notes/profile-worker-5d3fd0f0251d62b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/notes/service-children-SIGHUP-15d0cf6d2a1bdbf9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/notes/support-pid-in-eventlet-backdoor-socket-path-1863eaad1dd08556.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/notes/threadgroup-cancel-bd89d72f383a3d9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/notes/timer-args-f578c8f9d08b217d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/notes/timer-stop_on_exception-9f21d7c4d6d1b0d9.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.280123 oslo.service-3.4.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.280123 oslo.service-3.4.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.280123 oslo.service-3.4.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9062 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.280123 oslo.service-3.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7386 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.272123 oslo.service-3.4.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 14:25:40.280123 oslo.service-3.4.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-22 14:25:12.000000 oslo.service-3.4.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2024-02-22 14:25:12.000000 oslo.service-3.4.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2024-02-22 14:25:40.280123 oslo.service-3.4.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-22 14:25:12.000000 oslo.service-3.4.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-02-22 14:25:12.000000 oslo.service-3.4.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1805 2024-02-22 14:25:12.000000 oslo.service-3.4.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.530955 oslo.service-3.5.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-05-23 08:16:55.000000 oslo.service-3.5.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-05-23 08:16:55.000000 oslo.service-3.5.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1059 2024-05-23 08:16:55.000000 oslo.service-3.5.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-05-23 08:16:55.000000 oslo.service-3.5.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-05-23 08:16:55.000000 oslo.service-3.5.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6234 2024-05-23 08:17:24.000000 oslo.service-3.5.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      726 2024-05-23 08:16:55.000000 oslo.service-3.5.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24095 2024-05-23 08:17:24.000000 oslo.service-3.5.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-05-23 08:16:55.000000 oslo.service-3.5.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-23 08:16:55.000000 oslo.service-3.5.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2492 2024-05-23 08:17:24.530955 oslo.service-3.5.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1261 2024-05-23 08:16:55.000000 oslo.service-3.5.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.510956 oslo.service-3.5.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.510956 oslo.service-3.5.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2566 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.510956 oslo.service-3.5.0/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.510956 oslo.service-3.5.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.514956 oslo.service-3.5.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.514956 oslo.service-3.5.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/reference/eventlet_backdoor.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/reference/fixture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/reference/loopingcall.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/reference/periodic_task.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/reference/service.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/reference/sslutils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/reference/systemd.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/reference/threadgroup.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.514956 oslo.service-3.5.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7991 2024-05-23 08:16:55.000000 oslo.service-3.5.0/doc/source/user/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.518956 oslo.service-3.5.0/oslo.service.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2492 2024-05-23 08:17:24.000000 oslo.service-3.5.0/oslo.service.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3532 2024-05-23 08:17:24.000000 oslo.service-3.5.0/oslo.service.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:17:24.000000 oslo.service-3.5.0/oslo.service.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-05-23 08:17:24.000000 oslo.service-3.5.0/oslo.service.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 08:17:24.000000 oslo.service-3.5.0/oslo.service.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 08:17:24.000000 oslo.service-3.5.0/oslo.service.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-05-23 08:17:24.000000 oslo.service-3.5.0/oslo.service.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-05-23 08:17:24.000000 oslo.service-3.5.0/oslo.service.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.518956 oslo.service-3.5.0/oslo_service/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5802 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/_options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9496 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/eventlet_backdoor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/fixture.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.506956 oslo.service-3.5.0/oslo_service/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.506956 oslo.service-3.5.0/oslo_service/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.522956 oslo.service-3.5.0/oslo_service/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4478 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/locale/en_GB/LC_MESSAGES/oslo_service.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18140 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/loopingcall.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8175 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/periodic_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29482 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3173 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/sslutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3101 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/systemd.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.522956 oslo.service-3.5.0/oslo_service/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1339 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2659 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5109 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/eventlet_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.526955 oslo.service-3.5.0/oslo_service/tests/ssl_cert/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/ssl_cert/ca.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1679 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/ssl_cert/ca.key
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1184 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/ssl_cert/certificate.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1679 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/ssl_cert/privatekey.key
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7940 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/test_eventlet_backdoor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/test_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16175 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/test_loopingcall.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13818 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/test_periodic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26685 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6065 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/test_sslutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2580 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/test_systemd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6195 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/test_threadgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14419 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/tests/test_wsgi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18025 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/threadgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12496 2024-05-23 08:16:55.000000 oslo.service-3.5.0/oslo_service/wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.506956 oslo.service-3.5.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.526955 oslo.service-3.5.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/notes/add-timeout-looping-call-5cc396b75597c3c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/notes/add-wsgi_server_debug-opt-70d818b5b78bfc7c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/notes/add_reno-3b4ae0789e9c45b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/notes/drop-python27-support-1cfdf65193a03f3a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/notes/fix-find-object-in-backdoor-487bf78c4c502594.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/notes/native-threads-on-child-7150690c7caa1013.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/notes/profile-worker-5d3fd0f0251d62b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/notes/service-children-SIGHUP-15d0cf6d2a1bdbf9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/notes/support-pid-in-eventlet-backdoor-socket-path-1863eaad1dd08556.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/notes/threadgroup-cancel-bd89d72f383a3d9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/notes/timer-args-f578c8f9d08b217d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/notes/timer-stop_on_exception-9f21d7c4d6d1b0d9.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.530955 oslo.service-3.5.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.530955 oslo.service-3.5.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.530955 oslo.service-3.5.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9062 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.506956 oslo.service-3.5.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.506956 oslo.service-3.5.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.530955 oslo.service-3.5.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7386 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.506956 oslo.service-3.5.0/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 08:17:24.530955 oslo.service-3.5.0/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 08:16:55.000000 oslo.service-3.5.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2024-05-23 08:16:55.000000 oslo.service-3.5.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2024-05-23 08:17:24.534955 oslo.service-3.5.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-23 08:16:55.000000 oslo.service-3.5.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-23 08:16:55.000000 oslo.service-3.5.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1805 2024-05-23 08:16:55.000000 oslo.service-3.5.0/tox.ini
```

### Comparing `oslo.service-3.4.0/.pre-commit-config.yaml` & `oslo.service-3.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/AUTHORS` & `oslo.service-3.5.0/AUTHORS`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 Hengqing Hu <hudayou@hotmail.com>
 Hervé Beraud <hberaud@redhat.com>
 Ian Wienand <iwienand@redhat.com>
 Ihar Hrachyshka <ihrachys@redhat.com>
 Ilya Shakhat <ishakhat@mirantis.com>
 Iswarya_Vakati <v.iswarya@nectechnologies.in>
 James Carey <jecarey@us.ibm.com>
+James Page <james.page@canonical.com>
 Jason Dunsmore <jasondunsmore@gmail.com>
 Jason Kölker <jason@koelker.net>
 Javeme <zhangmei.li@easystack.cn>
 Javier Pena <jpena@redhat.com>
 Jay Pipes <jaypipes@gmail.com>
 Jeff Peeler <jpeeler@redhat.com>
 Joe Gordon <joe.gordon0@gmail.com>
@@ -115,14 +116,15 @@
 Soren Hansen <soren@linux2go.dk>
 Stephen Finucane <sfinucan@redhat.com>
 Steve Martinelli <stevemar@ca.ibm.com>
 Steven Hardy <shardy@redhat.com>
 Surojit Pathak <suro@yahoo-inc.com>
 Takashi Kajinami <kajinamit@oss.nttdata.com>
 Takashi Natsume <takanattie@gmail.com>
+Terry Wilson <twilson@redhat.com>
 Thomas Herve <therve@redhat.com>
 Thomas Herve <thomas.herve@enovance.com>
 Tianhua Huang <huangtianhua@huawei.com>
 Tom Cammann <tom.cammann@hp.com>
 TommyLike <tommylikehu@gmail.com>
 Tony Breeds <tony@bakeyournoodle.com>
 Victor Sergeyev <vsergeyev@mirantis.com>
```

### Comparing `oslo.service-3.4.0/CONTRIBUTING.rst` & `oslo.service-3.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/ChangeLog` & `oslo.service-3.5.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 CHANGES
 =======
 
+3.5.0
+-----
+
+* reno: Update master for unmaintained/zed
+* Remove old excludes
+* Update sslutils.wrap for newer Pythons
+* Make signal handling order predictable
+* Update master for stable/2024.1
+* reno: Update master for unmaintained/xena
+* reno: Update master for unmaintained/wallaby
+* reno: Update master for unmaintained/victoria
+
 3.4.0
 -----
 
 * Switch to coverage command
 * reno: Update master for unmaintained/yoga
 * pre-commit: Integrate doc8 and bandit
 * pre-commit: Bump versions
```

### Comparing `oslo.service-3.4.0/LICENSE` & `oslo.service-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/PKG-INFO` & `oslo.service-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: oslo.service
-Version: 3.4.0
+Version: 3.5.0
 Summary: oslo.service library
 Home-page: https://docs.openstack.org/oslo.service/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `oslo.service-3.4.0/README.rst` & `oslo.service-3.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/doc/source/conf.py` & `oslo.service-3.5.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/doc/source/configuration/index.rst` & `oslo.service-3.5.0/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/doc/source/index.rst` & `oslo.service-3.5.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/doc/source/user/usage.rst` & `oslo.service-3.5.0/doc/source/user/usage.rst`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo.service.egg-info/PKG-INFO` & `oslo.service-3.5.0/oslo.service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: oslo.service
-Version: 3.4.0
+Version: 3.5.0
 Summary: oslo.service library
 Home-page: https://docs.openstack.org/oslo.service/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `oslo.service-3.4.0/oslo.service.egg-info/SOURCES.txt` & `oslo.service-3.5.0/oslo.service.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 releasenotes/notes/service-children-SIGHUP-15d0cf6d2a1bdbf9.yaml
 releasenotes/notes/support-pid-in-eventlet-backdoor-socket-path-1863eaad1dd08556.yaml
 releasenotes/notes/threadgroup-cancel-bd89d72f383a3d9b.yaml
 releasenotes/notes/timer-args-f578c8f9d08b217d.yaml
 releasenotes/notes/timer-stop_on_exception-9f21d7c4d6d1b0d9.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
```

### Comparing `oslo.service-3.4.0/oslo_service/_i18n.py` & `oslo.service-3.5.0/oslo_service/_i18n.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/_options.py` & `oslo.service-3.5.0/oslo_service/_options.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/eventlet_backdoor.py` & `oslo.service-3.5.0/oslo_service/eventlet_backdoor.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/fixture.py` & `oslo.service-3.5.0/oslo_service/fixture.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/locale/en_GB/LC_MESSAGES/oslo_service.po` & `oslo.service-3.5.0/oslo_service/locale/en_GB/LC_MESSAGES/oslo_service.po`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/loopingcall.py` & `oslo.service-3.5.0/oslo_service/loopingcall.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/periodic_task.py` & `oslo.service-3.5.0/oslo_service/periodic_task.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/service.py` & `oslo.service-3.5.0/oslo_service/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         self._signals_by_name = dict((name, getattr(signal, name))
                                      for name in dir(signal)
                                      if name.startswith("SIG") and
                                      name not in self._ignore_signals)
         self.signals_to_name = dict(
             (sigval, name)
             for (name, sigval) in self._signals_by_name.items())
-        self._signal_handlers = collections.defaultdict(set)
+        self._signal_handlers = collections.defaultdict(list)
         self.clear()
 
     def clear(self):
         for sig in self._signal_handlers:
             signal.signal(sig, signal.SIG_DFL)
         self._signal_handlers.clear()
 
@@ -154,15 +154,15 @@
         for sig in signals:
             self.add_handler(sig, handler)
 
     def add_handler(self, sig, handler):
         if not self.is_signal_supported(sig):
             return
         signo = self._signals_by_name[sig]
-        self._signal_handlers[signo].add(handler)
+        self._signal_handlers[signo].append(handler)
         signal.signal(signo, self._handle_signal)
 
     def _handle_signal(self, signo, frame):
         # This method can be called anytime, even between two Python
         # instructions. It's scheduled by the C signal handler of Python using
         # Py_AddPendingCall().
         #
@@ -233,15 +233,15 @@
 
                 poll_hub.sleep = sleep_wrapper
 
             hub = eventlet.hubs.get_hub()
             self.__hub_module_file = sys.modules[hub.__module__].__file__
 
     def _handle_signal_cb(self, signo, frame):
-        for handler in self._signal_handlers[signo]:
+        for handler in reversed(self._signal_handlers[signo]):
             handler(signo, frame)
 
     def is_signal_supported(self, sig_name):
         return sig_name in self._signals_by_name
 
 
 class Launcher(object):
```

### Comparing `oslo.service-3.4.0/oslo_service/sslutils.py` & `oslo.service-3.5.0/oslo_service/sslutils.py`

 * *Files 26% similar despite different names*

```diff
@@ -73,32 +73,31 @@
                              "option value in your configuration file"))
 
     return use_ssl
 
 
 def wrap(conf, sock):
     conf.register_opts(_options.ssl_opts, config_section)
-    ssl_kwargs = {
-        'server_side': True,
-        'certfile': conf.ssl.cert_file,
-        'keyfile': conf.ssl.key_file,
-        'cert_reqs': ssl.CERT_NONE,
-    }
+
+    ssl_version = ssl.PROTOCOL_TLS_SERVER
+    if conf.ssl.version:
+        key = conf.ssl.version.lower()
+        try:
+            ssl_version = _SSL_PROTOCOLS[key]
+        except KeyError:
+            raise RuntimeError(
+                _("Invalid SSL version : %s") % conf.ssl.version)
+
+    context = ssl.SSLContext(ssl_version)
+    context.load_cert_chain(conf.ssl.cert_file, conf.ssl.key_file)
 
     if conf.ssl.ca_file:
-        ssl_kwargs['ca_certs'] = conf.ssl.ca_file
-        ssl_kwargs['cert_reqs'] = ssl.CERT_REQUIRED
+        context.verify_mode = ssl.CERT_REQUIRED
+        context.load_verify_locations(conf.ssl.ca_file)
+    else:
+        context.check_hostname = False
+        context.verify_mode = ssl.CERT_NONE
+
+    if conf.ssl.ciphers:
+        context.set_ciphers(conf.ssl.ciphers)
 
-        if conf.ssl.version:
-            key = conf.ssl.version.lower()
-            try:
-                ssl_kwargs['ssl_version'] = _SSL_PROTOCOLS[key]
-            except KeyError:
-                raise RuntimeError(
-                    _("Invalid SSL version : %s") % conf.ssl.version)
-
-        if conf.ssl.ciphers:
-            ssl_kwargs['ciphers'] = conf.ssl.ciphers
-
-    # NOTE(eezhova): SSL/TLS protocol version is injected in ssl_kwargs above,
-    # so skipping bandit check
-    return ssl.wrap_socket(sock, **ssl_kwargs)  # nosec
+    return context.wrap_socket(sock, server_side=True)
```

### Comparing `oslo.service-3.4.0/oslo_service/systemd.py` & `oslo.service-3.5.0/oslo_service/systemd.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/__init__.py` & `oslo.service-3.5.0/oslo_service/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/base.py` & `oslo.service-3.5.0/oslo_service/tests/base.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/eventlet_service.py` & `oslo.service-3.5.0/oslo_service/tests/eventlet_service.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/ssl_cert/ca.crt` & `oslo.service-3.5.0/oslo_service/tests/ssl_cert/ca.crt`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/ssl_cert/ca.key` & `oslo.service-3.5.0/oslo_service/tests/ssl_cert/ca.key`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/ssl_cert/certificate.crt` & `oslo.service-3.5.0/oslo_service/tests/ssl_cert/certificate.crt`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/ssl_cert/privatekey.key` & `oslo.service-3.5.0/oslo_service/tests/ssl_cert/privatekey.key`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/test_eventlet_backdoor.py` & `oslo.service-3.5.0/oslo_service/tests/test_eventlet_backdoor.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/test_fixture.py` & `oslo.service-3.5.0/oslo_service/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/test_loopingcall.py` & `oslo.service-3.5.0/oslo_service/tests/test_loopingcall.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/test_periodic.py` & `oslo.service-3.5.0/oslo_service/tests/test_periodic.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/test_service.py` & `oslo.service-3.5.0/oslo_service/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/test_sslutils.py` & `oslo.service-3.5.0/oslo_service/tests/test_sslutils.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,61 +74,70 @@
                               group=sslutils.config_section)
         self.conf.set_default("key_file", self.key_file_name,
                               group=sslutils.config_section)
         self.conf.set_default("ca_file", "/no/such/file",
                               group=sslutils.config_section)
         self.assertRaises(RuntimeError, sslutils.is_enabled, self.conf)
 
-    @mock.patch("ssl.wrap_socket")
+    @mock.patch("ssl.SSLContext")
     @mock.patch("os.path.exists")
-    def _test_wrap(self, exists_mock, wrap_socket_mock, **kwargs):
+    def _test_wrap(self, exists_mock, ssl_context_mock,
+                   ca_file=None,
+                   ciphers=None,
+                   ssl_version=None):
         exists_mock.return_value = True
         sock = mock.Mock()
+        context = mock.Mock()
+        ssl_context_mock.return_value = context
         self.conf.set_default("cert_file", self.cert_file_name,
                               group=sslutils.config_section)
         self.conf.set_default("key_file", self.key_file_name,
                               group=sslutils.config_section)
-        ssl_kwargs = {'server_side': True,
-                      'certfile': self.conf.ssl.cert_file,
-                      'keyfile': self.conf.ssl.key_file,
-                      'cert_reqs': ssl.CERT_NONE,
-                      }
-        if kwargs:
-            ssl_kwargs.update(**kwargs)
         sslutils.wrap(self.conf, sock)
-        wrap_socket_mock.assert_called_once_with(sock, **ssl_kwargs)
+        ssl_version = ssl_version or ssl.PROTOCOL_TLS_SERVER
+        ssl_context_mock.assert_called_once_with(ssl_version)
+        context.load_cert_chain.assert_called_once_with(
+            self.conf.ssl.cert_file,
+            self.conf.ssl.key_file,
+        )
+        if ca_file:
+            self.assertEqual(context.verify_mode, ssl.CERT_REQUIRED)
+            context.load_verify_locations.assert_called_once_with(
+                ca_file
+            )
+        else:
+            self.assertEqual(context.verify_mode, ssl.CERT_NONE)
+            self.assertFalse(context.check_hostname)
+        if ciphers:
+            context.set_ciphers.assert_called_once_with(
+                ciphers
+            )
+        context.wrap_socket.assert_called_once_with(sock, server_side=True)
 
     def test_wrap(self):
         self._test_wrap()
 
     def test_wrap_ca_file(self):
         self.conf.set_default("ca_file", self.ca_file_name,
                               group=sslutils.config_section)
-        ssl_kwargs = {'ca_certs': self.conf.ssl.ca_file,
-                      'cert_reqs': ssl.CERT_REQUIRED
-                      }
-        self._test_wrap(**ssl_kwargs)
+        self._test_wrap(ca_file=self.conf.ssl.ca_file)
 
     def test_wrap_ciphers(self):
         self.conf.set_default("ca_file", self.ca_file_name,
                               group=sslutils.config_section)
         ciphers = (
             'ECDH+AESGCM:DH+AESGCM:ECDH+AES256:DH+AES256:ECDH+AES128:DH+'
             'AES:ECDH+HIGH:DH+HIGH:ECDH+3DES:DH+3DES:RSA+AESGCM:RSA+AES:'
             'RSA+HIGH:RSA+3DES:!aNULL:!eNULL:!MD5:!DSS:!RC4'
         )
         self.conf.set_default("ciphers", ciphers,
                               group=sslutils.config_section)
-        ssl_kwargs = {'ca_certs': self.conf.ssl.ca_file,
-                      'cert_reqs': ssl.CERT_REQUIRED,
-                      'ciphers': ciphers}
-        self._test_wrap(**ssl_kwargs)
+        self._test_wrap(ca_file=self.conf.ssl.ca_file,
+                        ciphers=self.conf.ssl.ciphers)
 
     def test_wrap_ssl_version(self):
         self.conf.set_default("ca_file", self.ca_file_name,
                               group=sslutils.config_section)
         self.conf.set_default("version", "tlsv1",
                               group=sslutils.config_section)
-        ssl_kwargs = {'ca_certs': self.conf.ssl.ca_file,
-                      'cert_reqs': ssl.CERT_REQUIRED,
-                      'ssl_version': ssl.PROTOCOL_TLSv1}
-        self._test_wrap(**ssl_kwargs)
+        self._test_wrap(ca_file=self.conf.ssl.ca_file,
+                        ssl_version=ssl.PROTOCOL_TLSv1)
```

### Comparing `oslo.service-3.4.0/oslo_service/tests/test_systemd.py` & `oslo.service-3.5.0/oslo_service/tests/test_systemd.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/test_threadgroup.py` & `oslo.service-3.5.0/oslo_service/tests/test_threadgroup.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/tests/test_wsgi.py` & `oslo.service-3.5.0/oslo_service/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/threadgroup.py` & `oslo.service-3.5.0/oslo_service/threadgroup.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/version.py` & `oslo.service-3.5.0/oslo_service/version.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/oslo_service/wsgi.py` & `oslo.service-3.5.0/oslo_service/wsgi.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/releasenotes/notes/timer-args-f578c8f9d08b217d.yaml` & `oslo.service-3.5.0/releasenotes/notes/timer-args-f578c8f9d08b217d.yaml`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/releasenotes/source/conf.py` & `oslo.service-3.5.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `oslo.service-3.5.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `oslo.service-3.5.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/setup.cfg` & `oslo.service-3.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/setup.py` & `oslo.service-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `oslo.service-3.4.0/tox.ini` & `oslo.service-3.5.0/tox.ini`

 * *Files identical despite different names*

